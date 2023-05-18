# Comparing `tmp/opensourceleg-1.2.0.tar.gz` & `tmp/opensourceleg-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensourceleg-1.2.0.tar", max compression
+gzip compressed data, was "opensourceleg-1.2.1.tar", max compression
```

## Comparing `opensourceleg-1.2.0.tar` & `opensourceleg-1.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    32471 2023-01-26 01:08:26.114591 opensourceleg-1.2.0/LICENSE
--rw-r--r--   0        0        0     1510 2023-04-13 18:12:03.062127 opensourceleg-1.2.0/README.md
--rw-r--r--   0        0        0      411 2023-04-13 17:30:19.791723 opensourceleg-1.2.0/opensourceleg/__init__.py
--rw-r--r--   0        0        0    19660 2023-05-17 23:20:15.884488 opensourceleg-1.2.0/opensourceleg/actuators.py
--rw-r--r--   0        0        0     1554 2023-05-11 18:11:48.610119 opensourceleg-1.2.0/opensourceleg/constants.py
--rw-r--r--   0        0        0      811 2023-05-11 18:11:48.616184 opensourceleg-1.2.0/opensourceleg/control.py
--rw-r--r--   0        0        0     3345 2023-05-17 23:17:38.367103 opensourceleg-1.2.0/opensourceleg/demo.py
--rw-r--r--   0        0        0      184 2023-05-11 15:09:10.436317 opensourceleg-1.2.0/opensourceleg/example.py
--rw-r--r--   0        0        0    10209 2023-05-17 22:37:53.276758 opensourceleg-1.2.0/opensourceleg/joints.py
--rw-r--r--   0        0        0      136 2023-03-19 23:25:36.020226 opensourceleg-1.2.0/opensourceleg/knee_encoder_map.npy
--rw-r--r--   0        0        0     8946 2023-05-17 22:38:25.771485 opensourceleg-1.2.0/opensourceleg/loadcell.py
--rw-r--r--   0        0        0     3713 2023-05-11 18:11:48.609099 opensourceleg-1.2.0/opensourceleg/logger.py
--rw-r--r--   0        0        0    13875 2023-05-17 23:07:45.277496 opensourceleg-1.2.0/opensourceleg/osl.py
--rw-r--r--   0        0        0     8305 2023-05-17 22:14:38.697899 opensourceleg-1.2.0/opensourceleg/state_machine.py
--rw-r--r--   0        0        0     3470 2023-05-11 18:11:49.648892 opensourceleg-1.2.0/opensourceleg/thermal.py
--rw-r--r--   0        0        0    21102 2023-05-17 23:07:45.278313 opensourceleg-1.2.0/opensourceleg/tui.py
--rw-r--r--   0        0        0     3529 2023-05-11 18:11:47.533081 opensourceleg-1.2.0/opensourceleg/units.py
--rw-r--r--   0        0        0    11526 2023-05-17 22:41:33.215103 opensourceleg-1.2.0/opensourceleg/utilities.py
--rw-r--r--   0        0        0     3668 2023-05-17 23:22:01.555582 opensourceleg-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2864 1970-01-01 00:00:00.000000 opensourceleg-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    32471 2023-01-26 01:08:26.114591 opensourceleg-1.2.1/LICENSE
+-rw-r--r--   0        0        0     1510 2023-04-13 18:12:03.062127 opensourceleg-1.2.1/README.md
+-rw-r--r--   0        0        0      411 2023-04-13 17:30:19.791723 opensourceleg-1.2.1/opensourceleg/__init__.py
+-rw-r--r--   0        0        0    19717 2023-05-18 00:38:28.485087 opensourceleg-1.2.1/opensourceleg/actuators.py
+-rw-r--r--   0        0        0     1554 2023-05-11 18:11:48.610119 opensourceleg-1.2.1/opensourceleg/constants.py
+-rw-r--r--   0        0        0      811 2023-05-11 18:11:48.616184 opensourceleg-1.2.1/opensourceleg/control.py
+-rw-r--r--   0        0        0     3373 2023-05-18 00:36:35.044683 opensourceleg-1.2.1/opensourceleg/demo.py
+-rw-r--r--   0        0        0      184 2023-05-11 15:09:10.436317 opensourceleg-1.2.1/opensourceleg/example.py
+-rw-r--r--   0        0        0    10266 2023-05-18 00:38:28.486647 opensourceleg-1.2.1/opensourceleg/joints.py
+-rw-r--r--   0        0        0      136 2023-03-19 23:25:36.020226 opensourceleg-1.2.1/opensourceleg/knee_encoder_map.npy
+-rw-r--r--   0        0        0     8975 2023-05-18 00:38:28.488117 opensourceleg-1.2.1/opensourceleg/loadcell.py
+-rw-r--r--   0        0        0     3713 2023-05-11 18:11:48.609099 opensourceleg-1.2.1/opensourceleg/logger.py
+-rw-r--r--   0        0        0    13987 2023-05-18 00:37:44.624641 opensourceleg-1.2.1/opensourceleg/osl.py
+-rw-r--r--   0        0        0     8305 2023-05-17 22:14:38.697899 opensourceleg-1.2.1/opensourceleg/state_machine.py
+-rw-r--r--   0        0        0     3470 2023-05-11 18:11:49.648892 opensourceleg-1.2.1/opensourceleg/thermal.py
+-rw-r--r--   0        0        0    21102 2023-05-18 00:38:00.668950 opensourceleg-1.2.1/opensourceleg/tui.py
+-rw-r--r--   0        0        0     3529 2023-05-11 18:11:47.533081 opensourceleg-1.2.1/opensourceleg/units.py
+-rw-r--r--   0        0        0    11526 2023-05-18 00:38:14.303748 opensourceleg-1.2.1/opensourceleg/utilities.py
+-rw-r--r--   0        0        0     3668 2023-05-18 00:41:02.342023 opensourceleg-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2864 1970-01-01 00:00:00.000000 opensourceleg-1.2.1/PKG-INFO
```

### Comparing `opensourceleg-1.2.0/LICENSE` & `opensourceleg-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.0/README.md` & `opensourceleg-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.0/opensourceleg/actuators.py` & `opensourceleg-1.2.1/opensourceleg/actuators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import os
 import time
 from dataclasses import dataclass
 
 import flexsea.fx_enums as fxe
 import numpy as np
-from constants import Constants
-from control import (
+from flexsea.device import Device
+
+from opensourceleg.constants import Constants
+from opensourceleg.control import (
     DEFAULT_CURRENT_GAINS,
     DEFAULT_IMPEDANCE_GAINS,
     DEFAULT_POSITION_GAINS,
 )
-from flexsea.device import Device
-from logger import Logger
-from units import DEFAULT_UNITS, UnitsDefinition
+from opensourceleg.logger import Logger
+from opensourceleg.units import DEFAULT_UNITS, UnitsDefinition
 
 
 @dataclass
 class ControlModes:
     voltage = fxe.FX_VOLTAGE
     current = fxe.FX_CURRENT
     position = fxe.FX_POSITION
```

### Comparing `opensourceleg-1.2.0/opensourceleg/constants.py` & `opensourceleg-1.2.1/opensourceleg/constants.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.0/opensourceleg/control.py` & `opensourceleg-1.2.1/opensourceleg/control.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.0/opensourceleg/demo.py` & `opensourceleg-1.2.1/opensourceleg/demo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from osl import OpenSourceLeg
-from state_machine import Event, State
+from opensourceleg.osl import OpenSourceLeg
+from opensourceleg.state_machine import Event, State
 
 BODY_WEIGHT = 60.0  # kg
 
 
 def estance_to_lstance(osl: OpenSourceLeg):
     """
     Transition from early stance to late stance when the loadcell
```

### Comparing `opensourceleg-1.2.0/opensourceleg/joints.py` & `opensourceleg-1.2.1/opensourceleg/joints.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import os
 import time
 
 import numpy as np
-from actuators import DephyActpack
-from constants import Constants
-from logger import Logger
-from units import DEFAULT_UNITS, UnitsDefinition
+
+from opensourceleg.actuators import DephyActpack
+from opensourceleg.constants import Constants
+from opensourceleg.logger import Logger
+from opensourceleg.units import DEFAULT_UNITS, UnitsDefinition
 
 
 class Joint(DephyActpack):
     def __init__(
         self,
         name: str = "knee",
         port: str = "/dev/ttyACM0",
```

### Comparing `opensourceleg-1.2.0/opensourceleg/loadcell.py` & `opensourceleg-1.2.1/opensourceleg/loadcell.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import time
 
 import numpy as np
-from joints import Joint
-from logger import Logger
 from smbus2 import SMBus
 
+from opensourceleg.joints import Joint
+from opensourceleg.logger import Logger
+
 
 class StrainAmp:
     """
     A class to directly manage the 6ch strain gauge amplifier over I2C.
     Author: Mitry Anderson
     """
```

### Comparing `opensourceleg-1.2.0/opensourceleg/logger.py` & `opensourceleg-1.2.1/opensourceleg/logger.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.0/opensourceleg/osl.py` & `opensourceleg-1.2.1/opensourceleg/osl.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 import sys
 import time
 
 import numpy as np
 
 sys.path.append("../")
 
-import utilities as utilities
-from joints import Joint
-from loadcell import Loadcell
-from logger import Logger
-from state_machine import State, StateMachine
-from units import DEFAULT_UNITS, UnitsDefinition
-from utilities import SoftRealtimeLoop
+import opensourceleg.utilities as utilities
+from opensourceleg.joints import Joint
+from opensourceleg.loadcell import Loadcell
+from opensourceleg.logger import Logger
+from opensourceleg.state_machine import State, StateMachine
+from opensourceleg.units import DEFAULT_UNITS, UnitsDefinition
+from opensourceleg.utilities import SoftRealtimeLoop
 
 CURRENT_LIMIT = 8000
 
 
 class OpenSourceLeg:
     """
     OSL class: This class is the main class for the Open Source Leg project. It
@@ -330,15 +330,15 @@
 
         else:
             self.tui.add_update_callback(self.update)
             self.tui.run()
 
     def initialize_sm_tui(self):
 
-        from tui import COLORS
+        from opensourceleg.tui import COLORS
 
         self.tui.add_panel(
             name="top",
             layout="horizontal",
             border=False,
         )
```

### Comparing `opensourceleg-1.2.0/opensourceleg/state_machine.py` & `opensourceleg-1.2.1/opensourceleg/state_machine.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.0/opensourceleg/thermal.py` & `opensourceleg-1.2.1/opensourceleg/thermal.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.0/opensourceleg/tui.py` & `opensourceleg-1.2.1/opensourceleg/tui.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.0/opensourceleg/units.py` & `opensourceleg-1.2.1/opensourceleg/units.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.0/opensourceleg/utilities.py` & `opensourceleg-1.2.1/opensourceleg/utilities.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.0/pyproject.toml` & `opensourceleg-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "opensourceleg"
-version = "1.2.0"
+version = "1.2.1"
 description = "An open-source software library for numerical computation, data acquisition, and control of lower-limb robotic prosthesis."
 readme = "README.md"
 authors = ["Open-source Leg <opensourceleg@gmail.com>"]
 license = "GNU GPL v3.0"
 repository = "https://github.com/neurobionics/opensourceleg"
 homepage = "https://github.com/neurobionics/opensourceleg"
```

### Comparing `opensourceleg-1.2.0/PKG-INFO` & `opensourceleg-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensourceleg
-Version: 1.2.0
+Version: 1.2.1
 Summary: An open-source software library for numerical computation, data acquisition, and control of lower-limb robotic prosthesis.
 Home-page: https://github.com/neurobionics/opensourceleg
 License: GNU GPL v3.0
 Author: Open-source Leg
 Author-email: opensourceleg@gmail.com
 Requires-Python: >=3.9,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

