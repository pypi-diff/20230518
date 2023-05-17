# Comparing `tmp/opensourceleg-1.1.2.tar.gz` & `tmp/opensourceleg-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensourceleg-1.1.2.tar", max compression
+gzip compressed data, was "opensourceleg-1.2.0.tar", max compression
```

## Comparing `opensourceleg-1.1.2.tar` & `opensourceleg-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    32471 2023-01-26 01:08:26.114591 opensourceleg-1.1.2/LICENSE
--rw-r--r--   0        0        0     1510 2023-04-13 18:12:03.062127 opensourceleg-1.1.2/README.md
--rw-r--r--   0        0        0      411 2023-04-13 17:30:19.791723 opensourceleg-1.1.2/opensourceleg/__init__.py
--rw-r--r--   0        0        0    17769 2023-05-11 19:00:34.462414 opensourceleg-1.1.2/opensourceleg/actuators.py
--rw-r--r--   0        0        0     1554 2023-05-11 18:11:48.610119 opensourceleg-1.1.2/opensourceleg/constants.py
--rw-r--r--   0        0        0      811 2023-05-11 18:11:48.616184 opensourceleg-1.1.2/opensourceleg/control.py
--rw-r--r--   0        0        0     2913 2023-05-17 20:17:53.921472 opensourceleg-1.1.2/opensourceleg/demo.py
--rw-r--r--   0        0        0      184 2023-05-11 15:09:10.436317 opensourceleg-1.1.2/opensourceleg/example.py
--rw-r--r--   0        0        0    10266 2023-05-11 18:11:48.618013 opensourceleg-1.1.2/opensourceleg/joints.py
--rw-r--r--   0        0        0      136 2023-03-19 23:25:36.020226 opensourceleg-1.1.2/opensourceleg/knee_encoder_map.npy
--rw-r--r--   0        0        0     8887 2023-05-11 18:11:49.772102 opensourceleg-1.1.2/opensourceleg/loadcell.py
--rw-r--r--   0        0        0     3713 2023-05-11 18:11:48.609099 opensourceleg-1.1.2/opensourceleg/logger.py
--rw-r--r--   0        0        0    10920 2023-05-17 20:17:53.921801 opensourceleg-1.1.2/opensourceleg/osl.py
--rw-r--r--   0        0        0     6986 2023-05-17 19:39:38.540874 opensourceleg-1.1.2/opensourceleg/state_machine.py
--rw-r--r--   0        0        0     3470 2023-05-11 18:11:49.648892 opensourceleg-1.1.2/opensourceleg/thermal.py
--rw-r--r--   0        0        0    21103 2023-05-17 17:39:09.073251 opensourceleg-1.1.2/opensourceleg/tui.py
--rw-r--r--   0        0        0     3529 2023-05-11 18:11:47.533081 opensourceleg-1.1.2/opensourceleg/units.py
--rw-r--r--   0        0        0    11525 2023-05-17 19:52:02.930040 opensourceleg-1.1.2/opensourceleg/utilities.py
--rw-r--r--   0        0        0     3668 2023-05-17 20:18:01.682453 opensourceleg-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     2864 1970-01-01 00:00:00.000000 opensourceleg-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0    32471 2023-01-26 01:08:26.114591 opensourceleg-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1510 2023-04-13 18:12:03.062127 opensourceleg-1.2.0/README.md
+-rw-r--r--   0        0        0      411 2023-04-13 17:30:19.791723 opensourceleg-1.2.0/opensourceleg/__init__.py
+-rw-r--r--   0        0        0    19660 2023-05-17 23:20:15.884488 opensourceleg-1.2.0/opensourceleg/actuators.py
+-rw-r--r--   0        0        0     1554 2023-05-11 18:11:48.610119 opensourceleg-1.2.0/opensourceleg/constants.py
+-rw-r--r--   0        0        0      811 2023-05-11 18:11:48.616184 opensourceleg-1.2.0/opensourceleg/control.py
+-rw-r--r--   0        0        0     3345 2023-05-17 23:17:38.367103 opensourceleg-1.2.0/opensourceleg/demo.py
+-rw-r--r--   0        0        0      184 2023-05-11 15:09:10.436317 opensourceleg-1.2.0/opensourceleg/example.py
+-rw-r--r--   0        0        0    10209 2023-05-17 22:37:53.276758 opensourceleg-1.2.0/opensourceleg/joints.py
+-rw-r--r--   0        0        0      136 2023-03-19 23:25:36.020226 opensourceleg-1.2.0/opensourceleg/knee_encoder_map.npy
+-rw-r--r--   0        0        0     8946 2023-05-17 22:38:25.771485 opensourceleg-1.2.0/opensourceleg/loadcell.py
+-rw-r--r--   0        0        0     3713 2023-05-11 18:11:48.609099 opensourceleg-1.2.0/opensourceleg/logger.py
+-rw-r--r--   0        0        0    13875 2023-05-17 23:07:45.277496 opensourceleg-1.2.0/opensourceleg/osl.py
+-rw-r--r--   0        0        0     8305 2023-05-17 22:14:38.697899 opensourceleg-1.2.0/opensourceleg/state_machine.py
+-rw-r--r--   0        0        0     3470 2023-05-11 18:11:49.648892 opensourceleg-1.2.0/opensourceleg/thermal.py
+-rw-r--r--   0        0        0    21102 2023-05-17 23:07:45.278313 opensourceleg-1.2.0/opensourceleg/tui.py
+-rw-r--r--   0        0        0     3529 2023-05-11 18:11:47.533081 opensourceleg-1.2.0/opensourceleg/units.py
+-rw-r--r--   0        0        0    11526 2023-05-17 22:41:33.215103 opensourceleg-1.2.0/opensourceleg/utilities.py
+-rw-r--r--   0        0        0     3668 2023-05-17 23:22:01.555582 opensourceleg-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2864 1970-01-01 00:00:00.000000 opensourceleg-1.2.0/PKG-INFO
```

### Comparing `opensourceleg-1.1.2/LICENSE` & `opensourceleg-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.1.2/README.md` & `opensourceleg-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.1.2/opensourceleg/actuators.py` & `opensourceleg-1.2.0/opensourceleg/actuators.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
+import os
 import time
 from dataclasses import dataclass
 
 import flexsea.fx_enums as fxe
 import numpy as np
-from flexsea.device import Device
-
-from opensourceleg.constants import Constants
-from opensourceleg.control import (
+from constants import Constants
+from control import (
     DEFAULT_CURRENT_GAINS,
     DEFAULT_IMPEDANCE_GAINS,
     DEFAULT_POSITION_GAINS,
 )
-from opensourceleg.logger import Logger
-from opensourceleg.units import DEFAULT_UNITS, UnitsDefinition
+from flexsea.device import Device
+from logger import Logger
+from units import DEFAULT_UNITS, UnitsDefinition
 
 
 @dataclass
 class ControlModes:
     voltage = fxe.FX_VOLTAGE
     current = fxe.FX_CURRENT
     position = fxe.FX_POSITION
@@ -231,15 +231,17 @@
 
         assert 0 <= kp <= 80, "kp must be between 0 and 80"
         assert 0 <= ki <= 800, "ki must be between 0 and 800"
         assert 0 <= ff <= 128, "ff must be between 0 and 128"
         assert 0 <= K, "K must be greater than 0"
         assert 0 <= B, "B must be greater than 0"
 
-        self._device.set_gains(kp=kp, ki=ki, kd=0, k=K, b=B, ff=ff)
+        self._device.set_gains(
+            kp=int(kp), ki=int(ki), kd=int(0), k=int(K), b=int(B), ff=int(ff)
+        )
         self._has_gains = True
 
         time.sleep(1 / self._device.frequency)
 
 
 class DephyActpack(Device):
     """Class for the Dephy Actpack
@@ -296,15 +298,23 @@
             "current": CurrentMode(self),
             "impedance": ImpedanceMode(self),
         }
 
         self._mode: ActpackMode = self._modes["voltage"]
 
     def start(self):
-        self.open(self._frequency, self._debug_level, log_enabled=self._dephy_log)
+        try:
+            self.open(self._frequency, self._debug_level, log_enabled=self._dephy_log)
+        except OSError as e:
+            print("\n")
+            self._log.error(
+                f"Need admin previleges to open the port '{self.port}'. \n\nPlease run the script with 'sudo' command or add the user to the dialout group.\n"
+            )
+            os._exit(1)
+
         time.sleep(0.1)
         self._data = self.read()
         self._mode.enter()
 
     def stop(self):
         self.set_mode("voltage")
         self.set_voltage(0, force=True)
@@ -496,136 +506,190 @@
 
     @property
     def joint_zero_position(self):
         return self._joint_zero_position
 
     @property
     def battery_voltage(self):
-        return self._units.convert_from_default_units(
-            self._data.batt_volt,
-            "voltage",
-        )
+        if self._data is not None:
+            return self._units.convert_from_default_units(
+                self._data.batt_volt,
+                "voltage",
+            )
+        else:
+            return 0
 
     @property
     def batter_current(self):
-        return self._units.convert_from_default_units(
-            self._data.batt_curr,
-            "current",
-        )
+        if self._data is not None:
+            return self._units.convert_from_default_units(
+                self._data.batt_curr,
+                "current",
+            )
+        else:
+            return 0
 
     @property
     def motor_voltage(self):
-        return self._units.convert_from_default_units(
-            self._data.mot_volt,
-            "voltage",
-        )
+        if self._data is not None:
+            return self._units.convert_from_default_units(
+                self._data.mot_volt,
+                "voltage",
+            )
+        else:
+            return 0
 
     @property
     def motor_current(self):
-        return self._units.convert_from_default_units(
-            self._data.mot_cur,
-            "current",
-        )
+        if self._data is not None:
+            return self._units.convert_from_default_units(
+                self._data.mot_cur,
+                "current",
+            )
+        else:
+            return 0
 
     @property
     def motor_torque(self):
-        return self._units.convert_from_default_units(
-            self._data.mot_cur * Constants.NM_PER_MILLIAMP,
-            "torque",
-        )
+        if self._data is not None:
+            return self._units.convert_from_default_units(
+                self._data.mot_cur * Constants.NM_PER_MILLIAMP,
+                "torque",
+            )
+        else:
+            return 0
 
     @property
     def motor_position(self):
-        return self._units.convert_from_default_units(
-            int(self._data.mot_ang) * Constants.RAD_PER_COUNT,
-            "position",
-        )
+        if self._data is not None:
+            return self._units.convert_from_default_units(
+                int(self._data.mot_ang) * Constants.RAD_PER_COUNT,
+                "position",
+            )
+        else:
+            return 0
 
     @property
     def motor_velocity(self):
-        return self._units.convert_from_default_units(
-            self._data.mot_vel * Constants.RAD_PER_DEG,
-            "velocity",
-        )
+        if self._data is not None:
+            return self._units.convert_from_default_units(
+                int(self._data.mot_vel) * Constants.RAD_PER_COUNT,
+                "velocity",
+            )
+        else:
+            return 0
 
     @property
     def motor_acceleration(self):
-        return self._units.convert_from_default_units(
-            self._data.mot_acc,
-            "acceleration",
-        )
+        if self._data is not None:
+            return self._units.convert_from_default_units(
+                self._data.mot_acc,
+                "acceleration",
+            )
+        else:
+            return 0
 
     @property
     def motor_torque(self):
-        return self._units.convert_from_default_units(
-            self.motor_current * Constants.NM_PER_AMP,
-            "torque",
-        )
+        if self._data is not None:
+            return self._units.convert_from_default_units(
+                self.motor_current * Constants.NM_PER_AMP,
+                "torque",
+            )
+        else:
+            return 0
 
     @property
     def joint_position(self):
-        return self._units.convert_from_default_units(
-            self._data.ank_ang * Constants.RAD_PER_COUNT,
-            "position",
-        )
+        if self._data is not None:
+            return self._units.convert_from_default_units(
+                self._data.ank_ang * Constants.RAD_PER_COUNT,
+                "position",
+            )
+        else:
+            return 0
 
     @property
     def joint_velocity(self):
-        return self._units.convert_from_default_units(
-            self._data.ank_vel * Constants.RAD_PER_COUNT,
-            "velocity",
-        )
+        if self._data is not None:
+            return self._units.convert_from_default_units(
+                self._data.ank_vel * Constants.RAD_PER_COUNT,
+                "velocity",
+            )
+        else:
+            return 0
 
     @property
     def genvars(self):
-        return np.array(
-            [
-                self._data.genvar_0,
-                self._data.genvar_1,
-                self._data.genvar_2,
-                self._data.genvar_3,
-                self._data.genvar_4,
-                self._data.genvar_5,
-            ]
-        )
+        if self._data is not None:
+            return np.array(
+                [
+                    self._data.genvar_0,
+                    self._data.genvar_1,
+                    self._data.genvar_2,
+                    self._data.genvar_3,
+                    self._data.genvar_4,
+                    self._data.genvar_5,
+                ]
+            )
+        else:
+            return np.zeros(6)
 
     @property
     def acc_x(self):
-        return self._units.convert_from_default_units(
-            self._data.accelx * Constants.M_PER_SEC_SQUARED_ACCLSB,
-            "gravity",
-        )
+        if self._data is not None:
+            return self._units.convert_from_default_units(
+                self._data.accelx * Constants.M_PER_SEC_SQUARED_ACCLSB,
+                "gravity",
+            )
+        else:
+            return 0
 
     @property
     def acc_y(self):
-        return self._units.convert_from_default_units(
-            self._data.accely * Constants.M_PER_SEC_SQUARED_ACCLSB,
-            "gravity",
-        )
+        if self._data is not None:
+            return self._units.convert_from_default_units(
+                self._data.accely * Constants.M_PER_SEC_SQUARED_ACCLSB,
+                "gravity",
+            )
+        else:
+            return 0
 
     @property
     def acc_z(self):
-        return self._units.convert_from_default_units(
-            self._data.accelz * Constants.M_PER_SEC_SQUARED_ACCLSB,
-            "gravity",
-        )
+        if self._data is not None:
+            return self._units.convert_from_default_units(
+                self._data.accelz * Constants.M_PER_SEC_SQUARED_ACCLSB,
+                "gravity",
+            )
+        else:
+            return 0
 
     @property
     def gyro_x(self):
-        return self._units.convert_from_default_units(
-            self._data.gyrox * Constants.RAD_PER_SEC_GYROLSB,
-            "velocity",
-        )
+        if self._data is not None:
+            return self._units.convert_from_default_units(
+                self._data.gyrox * Constants.RAD_PER_SEC_GYROLSB,
+                "velocity",
+            )
+        else:
+            return 0
 
     @property
     def gyro_y(self):
-        return self._units.convert_from_default_units(
-            self._data.gyroy * Constants.RAD_PER_SEC_GYROLSB,
-            "velocity",
-        )
+        if self._data is not None:
+            return self._units.convert_from_default_units(
+                self._data.gyroy * Constants.RAD_PER_SEC_GYROLSB,
+                "velocity",
+            )
+        else:
+            return 0
 
     @property
     def gyro_z(self):
-        return self._units.convert_from_default_units(
-            self._data.gyroz * Constants.RAD_PER_SEC_GYROLSB,
-            "velocity",
-        )
+        if self._data is not None:
+            return self._units.convert_from_default_units(
+                self._data.gyroz * Constants.RAD_PER_SEC_GYROLSB,
+                "velocity",
+            )
+        else:
+            return 0
```

### Comparing `opensourceleg-1.1.2/opensourceleg/constants.py` & `opensourceleg-1.2.0/opensourceleg/constants.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.1.2/opensourceleg/control.py` & `opensourceleg-1.2.0/opensourceleg/control.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.1.2/opensourceleg/demo.py` & `opensourceleg-1.2.0/opensourceleg/demo.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,77 +1,89 @@
-from opensourceleg.osl import OpenSourceLeg
-from opensourceleg.state_machine import Event, State
+from osl import OpenSourceLeg
+from state_machine import Event, State
 
 BODY_WEIGHT = 60.0  # kg
-FZ_LSTANCE = -0.0167 * BODY_WEIGHT
-FZ_ESWING = -0.00167 * BODY_WEIGHT
-FZ_ESTANCE = -0.02 * BODY_WEIGHT
-VELOCITY_LSWING = 0.135  # rad/sec
-POSITION_LSWING = 60  # deg
-POSITION_ESTANCE = 30  # deg
 
 
 def estance_to_lstance(osl: OpenSourceLeg):
-    if osl.loadcell.fz < FZ_LSTANCE:
+    """
+    Transition from early stance to late stance when the loadcell
+    reads a force greater than a threshold.
+    """
+    if osl.loadcell.fz < -0.0167 * BODY_WEIGHT:
         return True
     else:
         return False
 
 
 def lstance_to_eswing(osl: OpenSourceLeg):
-    if osl.loadcell.fz > FZ_ESWING:
+    """
+    Transition from late stance to early swing when the loadcell
+    reads a force less than a threshold.
+    """
+    if osl.loadcell.fz > -0.00267 * BODY_WEIGHT:
         return True
     else:
         return False
 
 
 def eswing_to_lswing(osl: OpenSourceLeg):
-    if (
-        osl.knee.output_position > POSITION_LSWING
-        and osl.knee.output_velocity < VELOCITY_LSWING
-    ):
+    """
+    Transition from early swing to late swing when the knee angle
+    is greater than a threshold and the knee velocity is less than
+    a threshold.
+    """
+    if osl.knee.output_position > 60 and osl.knee.output_velocity < 0.135:
         return True
     else:
         return False
 
 
 def eswing_to_estance(osl: OpenSourceLeg):
-    if osl.loadcell.fz < FZ_ESTANCE:
+    """
+    Transition from early swing to early stance when the loadcell
+    reads a force greater than a threshold.
+    """
+    if osl.loadcell.fz < -0.02 * BODY_WEIGHT:
         return True
     else:
         False
 
 
 def lswing_to_estance(osl: OpenSourceLeg):
-    if osl.loadcell.fz < FZ_ESTANCE or osl.knee.output_position < POSITION_ESTANCE:
+    """
+    Transition from late swing to early stance when the loadcell
+    reads a force greater than a threshold or the knee angle is
+    less than a threshold.
+    """
+    if osl.loadcell.fz < -0.02 * BODY_WEIGHT or osl.knee.output_position < 30:
         return True
     else:
         return False
 
 
 def main():
     osl = OpenSourceLeg(frequency=200)
     osl.units["position"] = "deg"
-    osl.log.info(f"Units: {osl.units}")
 
     osl.add_joint(
         name="knee",
         gear_ratio=41.4999,
     )
 
     osl.add_loadcell(
         dephy_mode=False,
     )
 
     osl.add_state_machine()
 
-    early_stance = State("e_stance", 5, 130, 100)
-    late_stance = State("l_stance", 5, 175, 0)
+    early_stance = State("e_stance", 5, 130, 450)
+    late_stance = State("l_stance", 5, 175, 200)
     early_swing = State("e_swing", 62, 40, 40)
-    late_swing = State("l_swing", 30, 60, 200)
+    late_swing = State("l_swing", 30, 100, 200)
 
     foot_flat = Event("foot_flat")
     heel_off = Event("heel_off")
     toe_off = Event("toe_off")
     pre_heel_strike = Event("pre_heel_strike")
     heel_strike = Event("heel_strike")
     misc = Event("misc")
@@ -115,12 +127,12 @@
         heel_strike,
         lswing_to_estance,
     )
 
     osl.add_tui()
 
     with osl:
-        osl.run(set_state_machine_parameters=False)
+        osl.run(set_state_machine_parameters=True)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `opensourceleg-1.1.2/opensourceleg/joints.py` & `opensourceleg-1.2.0/opensourceleg/joints.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import os
 import time
 
 import numpy as np
-
-from opensourceleg.actuators import DephyActpack
-from opensourceleg.constants import Constants
-from opensourceleg.logger import Logger
-from opensourceleg.units import DEFAULT_UNITS, UnitsDefinition
+from actuators import DephyActpack
+from constants import Constants
+from logger import Logger
+from units import DEFAULT_UNITS, UnitsDefinition
 
 
 class Joint(DephyActpack):
     def __init__(
         self,
         name: str = "knee",
         port: str = "/dev/ttyACM0",
```

### Comparing `opensourceleg-1.1.2/opensourceleg/loadcell.py` & `opensourceleg-1.2.0/opensourceleg/loadcell.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import time
 
 import numpy as np
+from joints import Joint
+from logger import Logger
 from smbus2 import SMBus
 
-from opensourceleg.joints import Joint
-from opensourceleg.logger import Logger
-
 
 class StrainAmp:
     """
     A class to directly manage the 6ch strain gauge amplifier over I2C.
     Author: Mitry Anderson
     """
 
@@ -239,32 +238,35 @@
 
     @property
     def is_zeroed(self):
         return self._zeroed
 
     @property
     def fx(self):
-        return self._loadcell_data[0][0]
+        return self.loadcell_data[0]
 
     @property
     def fy(self):
-        return self._loadcell_data[0][1]
+        return self.loadcell_data[1]
 
     @property
     def fz(self):
-        return self._loadcell_data[0][2]
+        return self.loadcell_data[2]
 
     @property
     def mx(self):
-        return self._loadcell_data[0][3]
+        return self.loadcell_data[3]
 
     @property
     def my(self):
-        return self._loadcell_data[0][4]
+        return self.loadcell_data[4]
 
     @property
     def mz(self):
-        return self._loadcell_data[0][5]
+        return self.loadcell_data[5]
 
     @property
     def loadcell_data(self):
-        return self._loadcell_data[0]
+        if self._loadcell_data is not None:
+            return self._loadcell_data[0]
+        else:
+            return [0.0, 0.0, 0.0, 0.0, 0.0, 0.0]
```

### Comparing `opensourceleg-1.1.2/opensourceleg/logger.py` & `opensourceleg-1.2.0/opensourceleg/logger.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.1.2/opensourceleg/osl.py` & `opensourceleg-1.2.0/opensourceleg/osl.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 import sys
 import time
 
 import numpy as np
 
 sys.path.append("../")
 
-from opensourceleg.joints import Joint
-from opensourceleg.loadcell import Loadcell
-from opensourceleg.logger import Logger
-from opensourceleg.state_machine import State, StateMachine
-from opensourceleg.units import DEFAULT_UNITS, UnitsDefinition
-from opensourceleg.utilities import SoftRealtimeLoop
-import opensourceleg.utilities as utilities
+import utilities as utilities
+from joints import Joint
+from loadcell import Loadcell
+from logger import Logger
+from state_machine import State, StateMachine
+from units import DEFAULT_UNITS, UnitsDefinition
+from utilities import SoftRealtimeLoop
 
 CURRENT_LIMIT = 8000
 
 
 class OpenSourceLeg:
     """
     OSL class: This class is the main class for the Open Source Leg project. It
@@ -37,14 +37,26 @@
 
     def __init__(
         self,
         frequency: int = 200,
         current_limit: float = 8000,
         file_name: str = "./osl.log",
     ) -> None:
+        """
+        Initialize the OSL class.
+
+        Parameters
+        ----------
+        frequency : int, optional
+            The frequency of the control loop, by default 200
+        current_limit : float, optional
+            The current limit of the motor in mA, by default 8000
+        file_name : str, optional
+            The name of the log file, by default "./osl.log"
+        """
 
         self._frequency: int = frequency
 
         self._has_knee: bool = False
         self._has_ankle: bool = False
         self._has_loadcell: bool = False
         self._has_tui: bool = False
@@ -108,15 +120,15 @@
         return f"OSL object. Frequency: {self._frequency} Hz"
 
     def add_tui(
         self,
         configuration: str = "state_machine",
         layout: str = "vertical",
     ):
-        from opensourceleg.tui import TUI
+        from tui import TUI
 
         self._has_tui = True
         self.tui = TUI(
             title="www.opensourceleg.com", frequency=self._frequency, layout=layout
         )
 
         if configuration == "state_machine":
@@ -133,23 +145,52 @@
         port: str = None,
         baud_rate: int = 230400,
         gear_ratio: float = 1.0,
         has_loadcell: bool = False,
         debug_level: int = 0,
         dephy_log: bool = False,
     ):
+        """
+        Add a joint to the OSL object.
+
+        Parameters
+        ----------
+        name : str, optional
+            The name of the joint, by default "knee"
+        port : str, optional
+            The serial port that the joint is connected to, by default None. If
+            None, the first active port will be used.
+        baud_rate : int, optional
+            The baud rate of the serial communication, by default 230400
+        gear_ratio : float, optional
+            The gear ratio of the joint, by default 1.0
+        has_loadcell : bool, optional
+            Whether the joint has a loadcell, by default False
+        debug_level : int, optional
+            The debug level of the joint, by default 0
+        dephy_log : bool, optional
+            Whether to log the joint data to the dephy log, by default False
+        """
 
         if "knee" in name.lower():
             self._has_knee = True
 
             if port is None:
-                if "knee" in name.lower():
-                    port = utilities.get_active_ports()[0]
+                ports = utilities.get_active_ports()
+
+                if len(ports) == 0:
+                    self.log.warn(
+                        "No active ports found, please ensure that the joint is connected and powered on."
+                    )
+
                 else:
-                    port = utilities.get_active_ports()[1]
+                    if "knee" in name.lower():
+                        port = ports[0]
+                    else:
+                        port = ports[1]
 
             self._knee = Joint(
                 name=name,
                 port=port,
                 baud_rate=baud_rate,
                 frequency=self._frequency,
                 gear_ratio=gear_ratio,
@@ -181,27 +222,46 @@
         self,
         dephy_mode: bool = False,
         joint: Joint = None,
         amp_gain: float = 125.0,
         exc: float = 5.0,
         loadcell_matrix=None,
     ):
+        """
+        Add a loadcell to the OSL object.
+
+        Parameters
+        ----------
+        dephy_mode : bool, optional
+            Whether the loadcell is in dephy mode ie. connected to the dephy actpack with an FFC cable, by default False
+        joint : Joint, optional
+            The joint that the loadcell is attached to, by default None
+        amp_gain : float, optional
+            The amplifier gain of the loadcell, by default 125.0
+        exc : float, optional
+            The excitation voltage of the loadcell, by default 5.0
+        loadcell_matrix : np.ndarray, optional
+            The loadcell calibration matrix, by default None
+        """
         self._has_loadcell = True
         self._loadcell = Loadcell(
             dephy_mode=dephy_mode,
             joint=joint,
             amp_gain=amp_gain,
             exc=exc,
             loadcell_matrix=loadcell_matrix,
             logger=self.log,
         )
 
     def add_state_machine(
         self,
     ):
+        """
+        Add a state machine to the OSL object.
+        """
         self.state_machine = StateMachine(osl=self)
         self._has_sm = True
 
     def update(
         self,
     ):
         if self.has_knee:
@@ -229,34 +289,56 @@
             if self._set_state_machine_parameters:
                 if self.has_knee:
                     self.knee.set_impedance_gains(
                         K=self.state_machine.current_state.stiffness,
                         B=self.state_machine.current_state.damping,
                     )
 
-                if self.has_ankle:
                     self.knee.set_output_position(
                         self.state_machine.current_state.equilibrium_angle
                     )
 
+                elif self.has_ankle:
+                    self.ankle.set_impedance_gains(
+                        K=self.state_machine.current_state.stiffness,
+                        B=self.state_machine.current_state.damping,
+                    )
+
+                    self.ankle.set_output_position(
+                        self.state_machine.current_state.equilibrium_angle
+                    )
+
     def run(self, set_state_machine_parameters: bool = False):
+        """
+        Run the OpenSourceLeg instance: update the joints, loadcell, and state machine.
+        If the instance has a TUI, run the TUI.
+        If the instance has a state machine and if set_state_machine_parameters is True,
+        set the joint impedance gains and equilibrium angles to the current state's values.
+
+        Parameters
+        ----------
+        set_state_machine_parameters : bool, optional
+            Whether to set the joint impedance gains and equilibrium angles to the current state's values, by default False
+        """
 
         self._set_state_machine_parameters = set_state_machine_parameters
         self.update()
 
+        time.sleep(0.1)
+
         if not self.has_tui:
             self.update()
 
         else:
             self.tui.add_update_callback(self.update)
             self.tui.run()
 
     def initialize_sm_tui(self):
 
-        from opensourceleg.tui import COLORS
+        from tui import COLORS
 
         self.tui.add_panel(
             name="top",
             layout="horizontal",
             border=False,
         )
 
@@ -279,21 +361,23 @@
         )
 
         self.tui.add_plot(
             name="fz_plot",
             parent="fz",
             object=self.loadcell,
             attribute="fz",
+            color=COLORS.cyan,
         )
 
         self.tui.add_plot(
             name="joint_position_plot",
             parent="joint_position",
             object=self.knee,
             attribute="output_position",
+            color=COLORS.yellow,
         )
 
         self.tui.add_state_visualizer(
             name="state_machine",
             parent="bottom",
             states=self.state_machine.states,
             object=self.state_machine,
@@ -301,26 +385,24 @@
             layout="horizontal",
         )
 
         self.tui.add_button(
             name="emergency_stop",
             parent="bottom",
             callback=self.estop,
-            color=COLORS.maize,
+            color=COLORS.red,
             border=True,
         )
 
     def estop(self, **kwargs):
         self.log.debug("[OSL] Emergency stop activated.")
 
         if self.has_tui:
             self.tui.quit()
 
-        self.__exit__(None, None, None)
-
     def home(self):
         if self.has_knee:
             self.log.debug("[OSL] Homing knee joint.")
             self.knee.home()
 
         if self.has_ankle:
             self.log.debug("[OSL] Homing ankle joint.")
@@ -414,14 +496,7 @@
 
     osl.units["position"] = "deg"
 
     osl.add_joint(
         name="knee",
         gear_ratio=41.61,
     )
-
-
-    # osl.add_state_machine()
-    # osl.add_tui()
-
-    # with osl:
-    #     osl.run(set_state_machine_parameters=True)
```

### Comparing `opensourceleg-1.1.2/opensourceleg/state_machine.py` & `opensourceleg-1.2.0/opensourceleg/state_machine.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,18 +2,30 @@
 # A simple and scalable Finite State Machine module
 
 from typing import Any, Callable, List, Optional
 
 
 class State:
     """
-    State class
+    A class to represent a state in a finite state machine.
     """
 
     def __init__(self, name, theta=0.0, k=0.0, b=0.0) -> None:
+        """
+        Parameters
+        ----------
+        name : str
+            The name of the state.
+        theta : float, optional
+            The theta parameter of the impedance model, by default 0.0
+        k : float, optional
+            The stiffness of the joint in PID units, by default 0.0
+        b : float, optional
+            The damping of the joint in PID units, by default 0.0
+        """
         self._name = name
 
         # Impedance parameters
         self._theta = theta
         self._k = k
         self._b = b
 
@@ -84,14 +96,20 @@
 
 class Event:
     """
     Event class
     """
 
     def __init__(self, name) -> None:
+        """
+        Parameters
+        ----------
+        name : str
+            The name of the event.
+        """
         self._name = name
 
     def __eq__(self, __o) -> bool:
         if __o.name == self._name:
             return True
         else:
             return False
@@ -184,14 +202,25 @@
         self.add_state(self._exit_state)
         self._initial_state = self._exit_state
 
         self._exited = True
         self._osl = osl
 
     def add_state(self, state: State, initial_state: bool = False):
+        """
+        Add a state to the state machine.
+
+        Parameters
+        ----------
+        state : State
+            The state to be added.
+        initial_state : bool, optional
+            Whether the state is the initial state, by default False
+
+        """
         if state in self._states:
             raise ValueError("State already exists.")
 
         self._states.append(state)
 
         if initial_state:
             self._initial_state = state
@@ -202,14 +231,28 @@
     def add_transition(
         self,
         source: State,
         destination: State,
         event: Event,
         callback: Callable[[Any], bool] = None,
     ) -> Optional[Transition]:
+        """
+        Add a transition to the state machine.
+
+        Parameters
+        ----------
+        source : State
+            The source state.
+        destination : State
+            The destination state.
+        event : Event
+            The event that triggers the transition.
+        callback : Callable[[Any], bool], optional
+            A callback function that returns a boolean value, which determines whether the transition is valid, by default None
+        """
         transition = None
 
         if (
             source in self._states
             and destination in self._states
             and event in self._events
         ):
```

### Comparing `opensourceleg-1.1.2/opensourceleg/thermal.py` & `opensourceleg-1.2.0/opensourceleg/thermal.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.1.2/opensourceleg/tui.py` & `opensourceleg-1.2.0/opensourceleg/tui.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
         self._state_vizualisers = {}
 
         self.frame = ttk.TTkFrame(
             parent=self.root_ttk,
             border=True,
             title=title,
-            titleColor=ttk.TTkColor.BOLD + ttk.TTkColor.fg(COLORS.maize),
+            titleColor=ttk.TTkColor.BOLD + ttk.TTkColor.fg(COLORS.cyan),
         )
 
         self.frame.setLayout(self._layouts[layout]())
         self._panels["root"] = self.frame
 
         self._update_callbacks: list[callable] = []
```

### Comparing `opensourceleg-1.1.2/opensourceleg/units.py` & `opensourceleg-1.2.0/opensourceleg/units.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.1.2/opensourceleg/utilities.py` & `opensourceleg-1.2.0/opensourceleg/utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -313,14 +313,15 @@
         else:
             delta = -1 * self.delta_per_update
         self.value += delta
 
         self.value = min(max(self.value, 0), 1)
         return self.value
 
+
 def get_active_ports():
     """
     Lists active serial ports.
     """
     if sys.platform.startswith("linux") or sys.platform.startswith("cygwin"):
         ports = glob.glob("/dev/tty[A-Za-z]C*")
     elif sys.platform.startswith("darwin"):
```

### Comparing `opensourceleg-1.1.2/pyproject.toml` & `opensourceleg-1.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "opensourceleg"
-version = "1.1.2"
+version = "1.2.0"
 description = "An open-source software library for numerical computation, data acquisition, and control of lower-limb robotic prosthesis."
 readme = "README.md"
 authors = ["Open-source Leg <opensourceleg@gmail.com>"]
 license = "GNU GPL v3.0"
 repository = "https://github.com/neurobionics/opensourceleg"
 homepage = "https://github.com/neurobionics/opensourceleg"
```

### Comparing `opensourceleg-1.1.2/PKG-INFO` & `opensourceleg-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensourceleg
-Version: 1.1.2
+Version: 1.2.0
 Summary: An open-source software library for numerical computation, data acquisition, and control of lower-limb robotic prosthesis.
 Home-page: https://github.com/neurobionics/opensourceleg
 License: GNU GPL v3.0
 Author: Open-source Leg
 Author-email: opensourceleg@gmail.com
 Requires-Python: >=3.9,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

