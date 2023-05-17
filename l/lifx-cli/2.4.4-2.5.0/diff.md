# Comparing `tmp/lifx_cli-2.4.4.tar.gz` & `tmp/lifx_cli-2.5.0.tar.gz`

## Comparing `lifx_cli-2.4.4.tar` & `lifx_cli-2.5.0.tar`

### file list

```diff
@@ -1,14 +1,17 @@
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 lifx_cli-2.4.4/requirements.txt
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 lifx_cli-2.4.4/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 lifx_cli-2.4.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lifx_cli-2.4.4/src/lifx/__init__.py
--rwxr-xr-x   0        0        0     1951 2020-02-02 00:00:00.000000 lifx_cli-2.4.4/src/lifx/auth.py
--rwxr-xr-x   0        0        0     1762 2020-02-02 00:00:00.000000 lifx_cli-2.4.4/src/lifx/colors.py
--rwxr-xr-x   0        0        0    10649 2020-02-02 00:00:00.000000 lifx_cli-2.4.4/src/lifx/lifx.py
--rwxr-xr-x   0        0        0     4403 2020-02-02 00:00:00.000000 lifx_cli-2.4.4/src/lifx/lights.py
--rwxr-xr-x   0        0        0     1003 2020-02-02 00:00:00.000000 lifx_cli-2.4.4/src/lifx/scenes.py
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 lifx_cli-2.4.4/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 lifx_cli-2.4.4/LICENSE
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 lifx_cli-2.4.4/README.md
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 lifx_cli-2.4.4/pyproject.toml
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 lifx_cli-2.4.4/PKG-INFO
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 lifx_cli-2.5.0/requirements.txt
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 lifx_cli-2.5.0/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 lifx_cli-2.5.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lifx_cli-2.5.0/src/lifx/__init__.py
+-rwxr-xr-x   0        0        0     2098 2020-02-02 00:00:00.000000 lifx_cli-2.5.0/src/lifx/auth.py
+-rwxr-xr-x   0        0        0     1930 2020-02-02 00:00:00.000000 lifx_cli-2.5.0/src/lifx/colors.py
+-rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 lifx_cli-2.5.0/src/lifx/effects.py
+-rwxr-xr-x   0        0        0    11522 2020-02-02 00:00:00.000000 lifx_cli-2.5.0/src/lifx/lifx.py
+-rwxr-xr-x   0        0        0     2599 2020-02-02 00:00:00.000000 lifx_cli-2.5.0/src/lifx/lights.py
+-rwxr-xr-x   0        0        0     1349 2020-02-02 00:00:00.000000 lifx_cli-2.5.0/src/lifx/scenes.py
+-rwxr-xr-x   0        0        0     1038 2020-02-02 00:00:00.000000 lifx_cli-2.5.0/tests/lifx_cli_test.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 lifx_cli-2.5.0/tests/requirements.txt
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 lifx_cli-2.5.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 lifx_cli-2.5.0/LICENSE
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 lifx_cli-2.5.0/README.md
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 lifx_cli-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 lifx_cli-2.5.0/PKG-INFO
```

### Comparing `lifx_cli-2.4.4/.github/workflows/pylint.yml` & `lifx_cli-2.5.0/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.4.4/.github/workflows/python-publish.yml` & `lifx_cli-2.5.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.4.4/src/lifx/auth.py` & `lifx_cli-2.5.0/src/lifx/auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 """Configure and set authentication headers."""
-
 import sys
 import configparser
 from os import path, environ, getenv
 
+
 class Auth:
     """Configure and set authentication headers."""
 
     def __init__(self):
 
         self.auth_file = f'{path.expanduser("~")}/.keys'
         self.auth_file_section = 'lifx'
@@ -43,20 +43,24 @@
                     config.write(file)
 
         sys.exit(0)
 
     def auth(self):
         """Returns the headers required to authenticate to the LIFX API."""
 
-        if environ.get(self.auth_env_var):
-            token = getenv(self.auth_env_var)
-        else:
-            config = configparser.ConfigParser()
-            config.read(self.auth_file)
-
-            token = config[self.auth_file_section][self.auth_file_key]
+        try:
+            if environ.get(self.auth_env_var):
+                token = getenv(self.auth_env_var)
+            else:
+                config = configparser.ConfigParser()
+                config.read(self.auth_file)
+
+                token = config[self.auth_file_section][self.auth_file_key]
+        except KeyError:
+            print("Must configure an API token first.")
+            self.configure()
 
         headers = {
             'Authorization': f'Bearer {token}',
         }
 
         return headers
```

### Comparing `lifx_cli-2.4.4/src/lifx/colors.py` & `lifx_cli-2.5.0/src/lifx/colors.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 #!/usr/bin/env python3
 """Learn about how the CLI accepts color encoding."""
-
 import json
+import sys
+
 from requests import get
 from tabulate import tabulate
 from src.lifx.auth import Auth
 
+API = 'https://api.lifx.com/v1'
+
 COLOR_TABLE = [['[name]', 'white, red, orange, yellow, cyan, green, blue, purple, or pink',
                 'Sets hue and saturation only.'],
                ['hue:[0-360]', 'hue:120', 'Sets hue.'],
                ['saturation:[0.0-1.0]', 'saturation:0.5', 'Sets saturation.'],
                ['brightness:[0.0-1.0]', 'brightness:0.5', 'Sets brightness.'],
                ['kelvin:[1500-9000]', 'kelvin:5000', 'Sets kelvin to -c and saturation to 0.0.'],
                ['#RRGGBB', '#ff0000', 'Converts to HSBK.'],
-               ['rgb:[0-255],[0-255],[0-255]', 'rgb:255,255,0', '	Converts to HSBK.']]
+               ['rgb:[0-255],[0-255],[0-255]', 'rgb:255,255,0', 'Converts to HSBK.']]
 
 
 class Colors:
     """Learn about how the CLI accepts color encoding."""
     def __init__(self):
 
         self.auth = Auth()
@@ -28,16 +31,19 @@
         """Print color formatting information."""
 
         print(tabulate(COLOR_TABLE, headers=["Format", "Example", "Notes"]))
 
     def validate_color(self, color):
         """Validate the provided color with the LIFX API."""
 
-        url = f'https://api.lifx.com/v1/color?string={color}'
+        url = f'{API}/color?string={color}'
         response = get(url, headers=self.auth_headers, timeout=5)
+        if response.status_code != 200:
+            print(f"HTTP request failed. State code: {response.status_code}")
+            sys.exit(10)
         response = json.loads(response.content)
 
         hue = response['hue'] or 'None'
         saturation = response['saturation'] or 'None'
         brightness = response['brightness'] or 'None'
         kelvin = response['kelvin'] or 'None'
```

### Comparing `lifx_cli-2.4.4/src/lifx/lifx.py` & `lifx_cli-2.5.0/src/lifx/lifx.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,44 +4,56 @@
 Control your lights with the unofficial LIFX CLI. This CLI uses the
 LIFX HTTP endpoints to configure your lights.
 https://api.developer.lifx.com/reference/introduction
 """
 import argparse
 from src.lifx.auth import Auth
 from src.lifx.colors import Colors
+from src.lifx.effects import Effects
 from src.lifx.lights import Lights
 from src.lifx.scenes import Scenes
 
 auth = Auth()
-colors = Colors()
-light = Lights()
-scene = Scenes()
 
 LOGO = """
 ██      ██ ███████ ██   ██      ██████ ██      ██
 ██      ██ ██       ██ ██      ██      ██      ██
 ██      ██ █████     ███       ██      ██      ██
 ██      ██ ██       ██ ██      ██      ██      ██
 ███████ ██ ██      ██   ██      ██████ ███████ ██
 
 """
 
 
-def lights_sub_command(args):
+def lights_sub_command(args=None):
     """Control the actions for the 'lights' sub-command."""
-    devices = args.list_devices
-    light_id = args.light_id
-    toggle = args.toggle
-    group = args.group
-    state = args.state
-    color = args.color
-    power = args.power
-    brightness = args.brightness
-    infrared = args.infrared
-    duration = args.duration
+    light = Lights()
+
+    if isinstance(args, list):
+        devices = args[0]
+        light_id = args[1]
+        toggle = args[2]
+        group = args[3]
+        state = args[4]
+        color = args[5]
+        power = args[6]
+        brightness = args[7]
+        infrared = args[8]
+        duration = args[9]
+    else:
+        devices = args.list_devices
+        light_id = args.light_id
+        toggle = args.toggle
+        group = args.group
+        state = args.state
+        color = args.color
+        power = args.power
+        brightness = args.brightness
+        infrared = args.infrared
+        duration = args.duration
 
     if devices:
         light.get()
 
     if toggle:
         light.toggle(light_id, group)
 
@@ -49,50 +61,73 @@
         state_attributes = {'power': power,
                             'brightness': brightness,
                             'duration': duration,
                             'infrared': infrared}
         light.set_state(light_id, group, color, state_attributes)
 
 
-def scenes_sub_command(args):
+def scenes_sub_command(args=None):
     """Control the actions for the 'scenes' sub-command."""
-    scenes = args.list_scenes
-    scene_id = args.scene_id
+    scene = Scenes()
+
+    if isinstance(args, list):
+        scenes = args[0]
+        scene_id = args[1]
+    else:
+        scenes = args.list_scenes
+        scene_id = args.scene_id
 
     if scenes:
         scene.get()
 
     if scene_id:
         scene.activate(scene_id)
 
 
-def effects_sub_command(args):
+def effects_sub_command(args=None):
     """Control the actions for the 'effects' sub-command."""
-    list_effects = args.list_effects
-    light_id = args.light_id
-    group = args.group
-    color = args.color
-    breathe = args.breathe
-    pulse = args.pulse
-    stop = args.stop
+    effects = Effects()
+
+    if isinstance(args, list):
+        list_effects = args[0]
+        light_id = args[1]
+        group = args[2]
+        color = args[3]
+        breathe = args[4]
+        pulse = args[5]
+        stop = args[6]
+    else:
+        list_effects = args.list_effects
+        light_id = args.light_id
+        group = args.group
+        color = args.color
+        breathe = args.breathe
+        pulse = args.pulse
+        stop = args.stop
 
     if list_effects:
-        light.list_effects()
+        effects.list_effects()
     if breathe:
-        light.breathe_effect(light_id, group, color)
+        effects.breathe_effect(light_id, group, color)
     elif pulse:
-        light.pulse_effect(light_id, group, color)
+        effects.pulse_effect(light_id, group, color)
     elif stop:
-        light.stop_effect(light_id, group)
+        effects.stop_effect(light_id, group)
 
 
 def colors_sub_command(args):
     """Control the actions for the 'colors' sub-command."""
-    list_colors = args.list_colors
-    provided_color = args.colors
+    colors = Colors()
+
+    if isinstance(args, list):
+        list_colors = args[0]
+        provided_color = args[1]
+    else:
+        list_colors = args.list_colors
+        provided_color = args.colors
 
     if list_colors:
         colors.color_information()
 
     if provided_color:
         colors.validate_color(provided_color)
 
@@ -244,18 +279,17 @@
                                '--color',
                                default=False,
                                dest='colors',
                                action='store',
                                help='Validate a color using the LIFX API.')
 
     args = job_options.parse_args()
-    configure = args.configure
 
     # Configure authentication.
-    if configure:
+    if args.configure:
         auth.configure()
 
     # The 'lights' sub-command.
     if args.command == 'lights':
         lights_sub_command(args)
 
     # The 'scenes' sub-command.
```

### Comparing `lifx_cli-2.4.4/.gitignore` & `lifx_cli-2.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.4.4/LICENSE` & `lifx_cli-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.4.4/README.md` & `lifx_cli-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.4.4/pyproject.toml` & `lifx_cli-2.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lifx-cli"
-version = "2.4.4"
+version = "2.5.0"
 authors = [{name="Wes Henderson", email="info@necrux.com"}]
 description = "The Unofficial LIFX CLI"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
   'requests',
   'tabulate',
```

### Comparing `lifx_cli-2.4.4/PKG-INFO` & `lifx_cli-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifx-cli
-Version: 2.4.4
+Version: 2.5.0
 Summary: The Unofficial LIFX CLI
 Project-URL: Homepage, https://github.com/necrux/lifx-cli
 Project-URL: Bug Tracker, https://github.com/necrux/lifx-cli/issues
 Author-email: Wes Henderson <info@necrux.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

