# Comparing `tmp/rayasdk-1.1.0.dev6.tar.gz` & `tmp/rayasdk-1.1.0.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rayasdk-1.1.0.dev6.tar", last modified: Thu May 18 04:50:17 2023, max compression
+gzip compressed data, was "rayasdk-1.1.0.dev7.tar", last modified: Thu May 18 19:52:12 2023, max compression
```

## Comparing `rayasdk-1.1.0.dev6.tar` & `rayasdk-1.1.0.dev7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 04:50:17.006009 rayasdk-1.1.0.dev6/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     6569 2023-05-18 04:50:17.006009 rayasdk-1.1.0.dev6/PKG-INFO
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     6219 2023-05-11 21:39:47.000000 rayasdk-1.1.0.dev6/README.md
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 04:50:17.006009 rayasdk-1.1.0.dev6/rayasdk/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      546 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev6/rayasdk/__init__.py
--rwxrwxr-x   0 camilo    (1000) camilo    (1000)     5154 2023-05-17 15:09:08.000000 rayasdk-1.1.0.dev6/rayasdk/__main__.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     5150 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev6/rayasdk/connect.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     6198 2023-05-18 04:14:54.000000 rayasdk-1.1.0.dev6/rayasdk/constants.py
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 04:50:17.006009 rayasdk-1.1.0.dev6/rayasdk/container_handlers/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-02-22 08:37:00.000000 rayasdk-1.1.0.dev6/rayasdk/container_handlers/__init__.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     5576 2023-05-17 15:09:08.000000 rayasdk-1.1.0.dev6/rayasdk/container_handlers/docker_handler.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     2568 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev6/rayasdk/initializer.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     1342 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev6/rayasdk/killer.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     1513 2023-05-17 15:09:08.000000 rayasdk-1.1.0.dev6/rayasdk/logger.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      819 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev6/rayasdk/messages.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     5993 2023-05-11 21:39:47.000000 rayasdk-1.1.0.dev6/rayasdk/runner.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     4396 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev6/rayasdk/scanner.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     1749 2023-05-11 21:39:47.000000 rayasdk-1.1.0.dev6/rayasdk/simulator.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     2667 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev6/rayasdk/sshKeyGen.py
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 04:50:17.006009 rayasdk-1.1.0.dev6/rayasdk/template/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      244 2023-02-22 08:37:00.000000 rayasdk-1.1.0.dev6/rayasdk/template/__main__.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      551 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev6/rayasdk/template/app.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      399 2023-04-17 17:27:42.000000 rayasdk-1.1.0.dev6/rayasdk/template/launch.json
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      108 2023-02-22 08:37:00.000000 rayasdk-1.1.0.dev6/rayasdk/template/manifest.json
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     3252 2023-05-17 15:09:08.000000 rayasdk-1.1.0.dev6/rayasdk/utils.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)    11007 2023-05-17 15:09:08.000000 rayasdk-1.1.0.dev6/rayasdk/vcs.py
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 04:50:17.006009 rayasdk-1.1.0.dev6/rayasdk.egg-info/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     6569 2023-05-18 04:50:16.000000 rayasdk-1.1.0.dev6/rayasdk.egg-info/PKG-INFO
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      683 2023-05-18 04:50:16.000000 rayasdk-1.1.0.dev6/rayasdk.egg-info/SOURCES.txt
--rw-rw-r--   0 camilo    (1000) camilo    (1000)        1 2023-05-18 04:50:16.000000 rayasdk-1.1.0.dev6/rayasdk.egg-info/dependency_links.txt
--rw-rw-r--   0 camilo    (1000) camilo    (1000)       51 2023-05-18 04:50:16.000000 rayasdk-1.1.0.dev6/rayasdk.egg-info/entry_points.txt
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      103 2023-05-18 04:50:16.000000 rayasdk-1.1.0.dev6/rayasdk.egg-info/requires.txt
--rw-rw-r--   0 camilo    (1000) camilo    (1000)        8 2023-05-18 04:50:16.000000 rayasdk-1.1.0.dev6/rayasdk.egg-info/top_level.txt
--rw-rw-r--   0 camilo    (1000) camilo    (1000)       79 2023-05-18 04:50:17.006009 rayasdk-1.1.0.dev6/setup.cfg
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     1101 2023-05-18 04:49:56.000000 rayasdk-1.1.0.dev6/setup.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 19:52:12.813964 rayasdk-1.1.0.dev7/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     6569 2023-05-18 19:52:12.813964 rayasdk-1.1.0.dev7/PKG-INFO
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     6219 2023-05-11 21:39:47.000000 rayasdk-1.1.0.dev7/README.md
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 19:52:12.813964 rayasdk-1.1.0.dev7/rayasdk/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      546 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev7/rayasdk/__init__.py
+-rwxrwxr-x   0 camilo    (1000) camilo    (1000)     4901 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev7/rayasdk/__main__.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     5407 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev7/rayasdk/connect.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     3381 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev7/rayasdk/constants.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 19:52:12.813964 rayasdk-1.1.0.dev7/rayasdk/container_handlers/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-02-22 08:37:00.000000 rayasdk-1.1.0.dev7/rayasdk/container_handlers/__init__.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     7391 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev7/rayasdk/container_handlers/docker_handler.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     2787 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev7/rayasdk/initializer.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     1439 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev7/rayasdk/killer.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     1513 2023-05-17 15:09:08.000000 rayasdk-1.1.0.dev7/rayasdk/logger.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      819 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev7/rayasdk/messages.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     6355 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev7/rayasdk/runner.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     4398 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev7/rayasdk/scanner.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     5413 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev7/rayasdk/simulator.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     2657 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev7/rayasdk/sshKeyGen.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 19:52:12.813964 rayasdk-1.1.0.dev7/rayasdk/template/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      244 2023-02-22 08:37:00.000000 rayasdk-1.1.0.dev7/rayasdk/template/__main__.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      551 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev7/rayasdk/template/app.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      399 2023-04-17 17:27:42.000000 rayasdk-1.1.0.dev7/rayasdk/template/launch.json
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      108 2023-02-22 08:37:00.000000 rayasdk-1.1.0.dev7/rayasdk/template/manifest.json
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     1775 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev7/rayasdk/utils.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)    10212 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev7/rayasdk/vcs.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 19:52:12.813964 rayasdk-1.1.0.dev7/rayasdk.egg-info/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     6569 2023-05-18 19:52:12.000000 rayasdk-1.1.0.dev7/rayasdk.egg-info/PKG-INFO
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      683 2023-05-18 19:52:12.000000 rayasdk-1.1.0.dev7/rayasdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)        1 2023-05-18 19:52:12.000000 rayasdk-1.1.0.dev7/rayasdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)       51 2023-05-18 19:52:12.000000 rayasdk-1.1.0.dev7/rayasdk.egg-info/entry_points.txt
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      103 2023-05-18 19:52:12.000000 rayasdk-1.1.0.dev7/rayasdk.egg-info/requires.txt
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)        8 2023-05-18 19:52:12.000000 rayasdk-1.1.0.dev7/rayasdk.egg-info/top_level.txt
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)       79 2023-05-18 19:52:12.813964 rayasdk-1.1.0.dev7/setup.cfg
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     1101 2023-05-18 19:50:57.000000 rayasdk-1.1.0.dev7/setup.py
```

### Comparing `rayasdk-1.1.0.dev6/PKG-INFO` & `rayasdk-1.1.0.dev7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rayasdk
-Version: 1.1.0.dev6
+Version: 1.1.0.dev7
 Summary: Raya SDK - Unlimited Robotics Software Development Kit
 Home-page: UNKNOWN
 Author: Unlimited Robotics
 Author-email: camilo@unlimited-robotics.com
 License: MIT
 Keywords: robotics,unlimited-robotics,gary
 Platform: UNKNOWN
```

### Comparing `rayasdk-1.1.0.dev6/README.md` & `rayasdk-1.1.0.dev7/README.md`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev6/rayasdk/__init__.py` & `rayasdk-1.1.0.dev7/rayasdk/__init__.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev6/rayasdk/__main__.py` & `rayasdk-1.1.0.dev7/rayasdk/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,30 +2,38 @@
 
 # Copyright 2020 Unlimited Robotics
 
 import argparse
 import os
 import sys
 import platform
+import subprocess
 
+import rayasdk.constants as constants
 from rayasdk.connect import URConnect
 from rayasdk.vcs import URVCS, check_simulation_versions, check_sdk_version
-from rayasdk.logger import log_error, log_verbose, set_logger_level
+from rayasdk.logger import log_error, log_verbose, log_info, set_logger_level
 from rayasdk.scanner import URScanner
 from rayasdk.initializer import URInitializer
 from rayasdk.runner import URRunner
 from rayasdk.simulator import URSimulator
 from rayasdk.killer import URKiller
-from rayasdk.constants import *
-from rayasdk.utils import *
 
 
 class URSDK:
 
     def __init__(self):
+        # Check for temp folder
+        if not self.init_ursdk_folder():
+            return False
+        # Check .ur folder
+        if not self.check_global_folder():
+            log_error(f'Could not create .ur folder')
+            return False
+        
         self.command_objects = []
         self.command_objects.append(URInitializer())
         self.command_objects.append(URScanner())
         self.command_objects.append(URConnect())
         self.command_objects.append(URRunner())
         self.command_objects.append(URSimulator())
         self.command_objects.append(URKiller())
@@ -55,81 +63,70 @@
         # Parse arguments
         self.args, self.unknownargs = self.argparser.parse_known_args()
         # Setup Logger
         set_logger_level(self.args.verbose, self.args.quiet)
 
     def check_global_folder(self):
         try:
-            update_constants()
             # create folders that are needed in the .ur path
-            os.makedirs(SIMS_APPS, exist_ok=True)
-            os.makedirs(SIMS_DATA_APPS, exist_ok=True)
-            os.makedirs(SIMS_DATA_APPS_DEVEL, exist_ok=True)
+            os.makedirs(constants.SIMS_APPS, exist_ok=True)
+            os.makedirs(constants.SIMS_DATA_APPS, exist_ok=True)
+            os.makedirs(constants.SIMS_DATA_APPS_DEVEL, exist_ok=True)
             # if ur_root not exist or is empty clone it
-            if not os.path.exists(RAYAENV_DOCKER_UR_ROOT) or len(
-                    os.listdir(RAYAENV_DOCKER_UR_ROOT)) == 0:
-                log_info('Cloning raya_root_folder_templates...')
-                return_code = subprocess.call((
-                    f'{RAYAENV_DOCKER_UR_ROOT_REPO} {RAYAENV_DOCKER_UR_ROOT} && '
-                    f'cd {RAYAENV_DOCKER_UR_ROOT} && cp env.template env'),
-                                              shell=True,
-                                              stderr=subprocess.PIPE)
-                if return_code != 0:
-                    log_error(
-                        ('Error cloning the raya_root_folders_templates repo '
-                         'check if you have permitions'))
+            if not os.path.exists(constants.RAYAENV_DOCKER_UR_ROOT) or len(
+                    os.listdir(constants.RAYAENV_DOCKER_UR_ROOT)) == 0:
+                log_info('Preparing UR user folder...')
+                subprocess.call(
+                        args=constants.RAYAENV_DOCKER_UR_ROOT_REPO,
+                        shell=True,
+                        stderr=subprocess.PIPE
+                    )
+                log_info('Done')
 
         except OSError as exc:
             log_error(exc)
             return False
         return True
 
     def init_ursdk_folder(self):
-        if not os.path.exists(URSDK_TEMP_PATH):
+        if not os.path.exists(constants.URSDK_TEMP_PATH):
             log_verbose(
-                f'Folder {URSDK_TEMP_PATH} does not exists, creating it.')
+                f'Folder {constants.URSDK_TEMP_PATH} does not exists, creating it.')
             try:
-                os.mkdir(URSDK_TEMP_PATH)
+                os.mkdir(constants.URSDK_TEMP_PATH)
             except OSError as exc:
-                log_error(f'Folder {URSDK_TEMP_PATH} could not be created.')
+                log_error(f'Folder {constants.URSDK_TEMP_PATH} could not be created.')
                 return False
             return True
         else:
-            log_verbose(f'Folder {URSDK_TEMP_PATH} found.')
+            log_verbose(f'Folder {constants.URSDK_TEMP_PATH} found.')
             return True
 
     def run(self):
         try:
-            # Check for temp folder
-            if not self.init_ursdk_folder():
-                return False
-            # Check .ur folder
-            if not self.check_global_folder():
-                log_error(f'Could not create .ur folder')
-                return False
             # Check if sdk have an update
             check_sdk_version()
             # Check simulation version on simulator and update command
             if self.args.command == URSimulator().COMMAND:
                 updated = check_simulation_versions()
                 if not updated and self.args.command == URSimulator().COMMAND:
                     log_error('RayaOS is not up to date. To update run "rayasdk update"')
                     return False
             # Execute Command
             for obj in self.command_objects:
                 if self.args.command == type(obj).COMMAND:
                     return obj.run(self.args, self.unknownargs)
         except Exception as e:
-            log_error(str(e))
-            return False
+           log_error(str(e))
+           return False
 
 
 def main():
     if platform.system() not in ['Linux', 'Windows', 'Darwin']:
-        print(f'Platform \'{platform.system()}\' not supported.')
+        log_info(f'Platform \'{platform.system()}\' not supported.')
         exit(1)
     ursdk = URSDK()
     ret = ursdk.run()
     if not ret:
         log_verbose('Finished with error.')
         sys.exit(1)
     else:
```

### Comparing `rayasdk-1.1.0.dev6/rayasdk/connect.py` & `rayasdk-1.1.0.dev7/rayasdk/connect.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Copyright 2020 Unlimited Robotics
 import subprocess
+import json
 
+import rayasdk.constants as constants
 from rayasdk.sshKeyGen import SshKeyGen
-from rayasdk.logger import log_error, log_verbose, log_info
-from rayasdk.constants import *
-
-import json
+from rayasdk.logger import log_verbose, log_info
 
 
 class URConnect:
 
     COMMAND = 'connect'
 
     def __init__(self):
@@ -33,88 +32,88 @@
         self.args = args
         self.unknownargs = unknownargs
 
         robot_id = self.args.robot_id
         robot_ip = self.args.robot_ip
         try:
             exec_settings = dict()
-            exec_settings[JSON_EXECINFO_SIM] = False
-            exec_settings[JSON_EXECINFO_ROBCONN] = dict()
-            robot_connection = exec_settings[JSON_EXECINFO_ROBCONN]
-            robot_connection[JSON_EXECINFO_ROBID] = ''
-            robot_connection[JSON_EXECINFO_ROBIP] = ''
+            exec_settings[constants.JSON_EXECINFO_SIM] = False
+            exec_settings[constants.JSON_EXECINFO_ROBCONN] = dict()
+            robot_connection = exec_settings[constants.JSON_EXECINFO_ROBCONN]
+            robot_connection[constants.JSON_EXECINFO_ROBID] = ''
+            robot_connection[constants.JSON_EXECINFO_ROBIP] = ''
 
             if self.args.simulator:
-                exec_settings[JSON_EXECINFO_SIM] = True
+                exec_settings[constants.JSON_EXECINFO_SIM] = True
                 log_info(f'You have successfully connected to the simulator')
             else:
-                with open(LAST_SCANNING_PATH, 'r', encoding='utf-8') as f:
+                with open(constants.LAST_SCANNING_PATH, 'r', encoding='utf-8') as f:
                     scanned_robots = json.load(f)
                 # Check if robot is in last scan
                 for robot in scanned_robots:
                     scanned_robot = scanned_robots[robot]
                     is_robot_id = robot_id and robot_id in scanned_robot[
                         "ROBOT_ID"]
                     is_robot_ip = robot_ip and robot_ip in scanned_robot[
                         "ROBOT_IP"]
                     if is_robot_id or is_robot_ip:
-                        if JSON_EXECINFO_ROBCONN not in exec_settings:
+                        if constants.JSON_EXECINFO_ROBCONN not in exec_settings:
                             robot_connection = {}
 
-                        if robot_connection[JSON_EXECINFO_ROBID] != '':
+                        if robot_connection[constants.JSON_EXECINFO_ROBID] != '':
                             raise NameError(
                                 (f'\'{robot_id}\' was detected with '
                                  'multiple IP addresses, connect using the'
                                  ' \'--robot-ip\' argument instead.'))
 
-                        robot_connection[JSON_EXECINFO_ROBID] = \
-                            scanned_robot[JSON_SCAN_ID]
-                        robot_connection[JSON_EXECINFO_ROBIP] = \
-                            scanned_robot[JSON_SCAN_IP]
-                        robot_connection[JSON_EXECINFO_ROBSERIAL] = \
-                            scanned_robot[JSON_SCAN_SERIAL]
+                        robot_connection[constants.JSON_EXECINFO_ROBID] = \
+                            scanned_robot[constants.JSON_SCAN_ID]
+                        robot_connection[constants.JSON_EXECINFO_ROBIP] = \
+                            scanned_robot[constants.JSON_SCAN_IP]
+                        robot_connection[constants.JSON_EXECINFO_ROBSERIAL] = \
+                            scanned_robot[constants.JSON_SCAN_SERIAL]
 
                 # If the robot was not found on the scan raise exception
-                if robot_connection[JSON_EXECINFO_ROBID] == '':
+                if robot_connection[constants.JSON_EXECINFO_ROBID] == '':
                     if robot_id:
                         raise NameError(
                             (f'Robot ID "{robot_id}" not found in scan info, '
                              'verify it or scan again.'))
                     elif robot_ip:
                         raise NameError(
                             (f'Robot IP "{robot_ip}" not found in scan info, '
                              'verify it or scan again.'))
                     else:
                         raise KeyError('')
 
                 # Send ssh key to robot
-                SshKeyGen(user=SSH_USER,
-                          host=robot_connection[JSON_EXECINFO_ROBIP],
-                          port=SSH_PORT)
+                SshKeyGen(user=constants.SSH_USER,
+                          host=robot_connection[constants.JSON_EXECINFO_ROBIP],
+                          port=constants.SSH_PORT)
                 log_info(f'You have successfully connected to '
-                         f'{robot_connection[JSON_EXECINFO_ROBID]}')
+                         f'{robot_connection[constants.JSON_EXECINFO_ROBID]}')
 
             # Save connection globally
-            with open(CONNECTION_SETTINGS_PATH, 'w', encoding='utf-8') as f:
+            with open(constants.CONNECTION_SETTINGS_PATH, 'w', encoding='utf-8') as f:
                 settings = dict()
-                settings[JSON_EXECINFO_SIM] = exec_settings[JSON_EXECINFO_SIM]
-                settings[JSON_EXECINFO_ROBCONN] = exec_settings[
-                    JSON_EXECINFO_ROBCONN]
+                settings[constants.JSON_EXECINFO_SIM] = exec_settings[constants.JSON_EXECINFO_SIM]
+                settings[constants.JSON_EXECINFO_ROBCONN] = exec_settings[
+                    constants.JSON_EXECINFO_ROBCONN]
                 json.dump(settings, f, ensure_ascii=False, indent=4)
 
         except FileNotFoundError:
             raise Exception(
-                f'Could not write file "{CONNECTION_SETTINGS_FILE}".')
+                f'Could not write file "{constants.CONNECTION_SETTINGS_FILE}".')
         except OSError:
             raise Exception((f'Could not get scanning info, '
                              'execute "rayasdk scan" before this command.'))
         except subprocess.SubprocessError:
             raise Exception("SSH Key not send, Check if raya_os is running")
         except NameError as error:
             raise Exception(str(error))
         except KeyError as error:
-            print(error)
+            log_info(error)
             raise Exception((f'Scanning info malformed, '
                              'please scan again by running "rayasdk scan".'))
 
         log_verbose('\nCorrect!')
         return True
```

### Comparing `rayasdk-1.1.0.dev6/rayasdk/initializer.py` & `rayasdk-1.1.0.dev7/rayasdk/initializer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Copyright 2020 Unlimited Robotics
 
 import os
 import json
 from shutil import copyfile
 
+import rayasdk.constants as constants
 from rayasdk.logger import log_error, log_verbose, log_info
-from rayasdk.constants import *
-from rayasdk.utils import *
+from rayasdk.utils import validate_app_id_and_folder_name
 
 
 class URInitializer:
     COMMAND = 'init'
 
     def __init__(self):
         pass
@@ -25,50 +25,50 @@
                                  type=str)
         self.parser.add_argument('--app-name',
                                  help='application name',
                                  type=str)
 
     def create_files_tree(self):
         try:
-            os.mkdir(DOC_PATH)
-            os.mkdir(LOG_PATH)
-            os.mkdir(RES_PATH)
-            os.mkdir(SRC_PATH)
-            os.mkdir(VSCODE_PATH)
-            copyfile(APP_PATH_ORIG, APP_PATH_DEST)
-            copyfile(MANIFEST_PATH_ORIG, MANIFEST_PATH_DEST)
-            copyfile(ENTRYPOINT_PATH_ORIG, ENTRYPOINT_PATH_DEST)
+            os.mkdir(constants.DOC_PATH)
+            os.mkdir(constants.LOG_PATH)
+            os.mkdir(constants.RES_PATH)
+            os.mkdir(constants.SRC_PATH)
+            os.mkdir(constants.VSCODE_PATH)
+            copyfile(constants.APP_PATH_ORIG, constants.APP_PATH_DEST)
+            copyfile(constants.MANIFEST_PATH_ORIG, constants.MANIFEST_PATH_DEST)
+            copyfile(constants.ENTRYPOINT_PATH_ORIG, constants.ENTRYPOINT_PATH_DEST)
 
-            copyfile(VSCODE_SETTINGS_PATH_ORIG, VSCODE_SETTINGS_PATH_DEST)
+            copyfile(constants.VSCODE_SETTINGS_PATH_ORIG, constants.VSCODE_SETTINGS_PATH_DEST)
         except OSError as exc:
-            print(exc)
+            log_info(exc)
             raise Exception(f'Could not create files tree')
         return True
 
     def create_json_exec_info(self):
         exec_settings = {}
-        exec_settings[JSON_EXECINFO_APPID] = self.args.app_id
-        exec_settings[JSON_EXECINFO_APPNAME] = self.args.app_name
+        exec_settings[constants.JSON_EXECINFO_APPID] = self.args.app_id
+        exec_settings[constants.JSON_EXECINFO_APPNAME] = self.args.app_name
         try:
-            with open(EXECSETTINGS_PATH, 'w', encoding='utf-8') as f:
+            with open(constants.EXECSETTINGS_PATH, 'w', encoding='utf-8') as f:
                 json.dump(exec_settings, f, ensure_ascii=False, indent=4)
         except FileNotFoundError:
-            log_error(f'Could not write file "{EXECSETTINGS_FILE}".')
+            log_error(f'Could not write file "{constants.EXECSETTINGS_FILE}".')
             return False
         return True
 
     def run(self, args, unknownargs):
         self.args = args
         self.unknownargs = unknownargs
 
         # Check if the parent has the same name that the app id
         validate_app_id_and_folder_name(self.args.app_id)
 
         # Check if the directory is empty
-        if len(os.listdir(CURRENT_PATH)) != 0:
+        if len(os.listdir(constants.CURRENT_PATH)) != 0:
             raise Exception('Current directory is not empty.')
 
         # Files tree
         log_verbose('Creating application files tree...')
         self.create_files_tree()
 
         # Json SDK info
```

### Comparing `rayasdk-1.1.0.dev6/rayasdk/killer.py` & `rayasdk-1.1.0.dev7/rayasdk/killer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 # Copyright 2020 Unlimited Robotics
-import json
+
 import subprocess
 
-from rayasdk.container_handlers.docker_handler import kill_apps
-from rayasdk.logger import log_error, log_verbose, log_info
-from rayasdk.constants import *
-from rayasdk.utils import *
+import rayasdk.constants as constants
+from rayasdk.container_handlers.docker_handler import DockerHandler
+from rayasdk.logger import log_info
+from rayasdk.utils import open_connection_file
 
 
 class URKiller:
 
     COMMAND = 'kill'
 
     def __init__(self):
-        pass
+        self.docker_handler = DockerHandler()
 
     def init_parser(self, subparser):
         self.parser = subparser.add_parser(
             type(self).COMMAND,
             help="kills all the running apps on the Ra-Ya container.")
 
     def run(self, args, unknownargs):
         self.args = args
         self.unknownargs = unknownargs
 
         connection_settings = open_connection_file()
 
-        if connection_settings[JSON_EXECINFO_SIM]:
-            kill_apps()
+        if connection_settings[constants.JSON_EXECINFO_SIM]:
+            self.docker_handler.kill_apps()
         else:
-            host = connection_settings[JSON_EXECINFO_ROBCONN][
-                JSON_EXECINFO_ROBIP]
-            host_url = f'{SSH_USER}@{host}'
+            host = connection_settings[constants.JSON_EXECINFO_ROBCONN][
+                constants.JSON_EXECINFO_ROBIP]
+            host_url = f'{constants.SSH_USER}@{host}'
             self.kill_apps_robot(host_url=host_url)
 
         log_info('\nDone!')
         return True
 
     def kill_apps_robot(self, host_url):
         log_info(f'Killing all running apps...')
         cmd = 'pkill -9 -u rayadevel'
         command = (('ssh -t '
                     '-o LogLevel=QUIET '
-                    f'-p {SSH_PORT} {host_url} '
+                    f'-p {constants.SSH_PORT} {host_url} '
                     f'\'{cmd}\''))
         ret = subprocess.call(command, shell=True)
```

### Comparing `rayasdk-1.1.0.dev6/rayasdk/logger.py` & `rayasdk-1.1.0.dev7/rayasdk/logger.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev6/rayasdk/messages.py` & `rayasdk-1.1.0.dev7/rayasdk/messages.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev6/rayasdk/runner.py` & `rayasdk-1.1.0.dev7/rayasdk/runner.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # Copyright 2020 Unlimited Robotics
 
 import json
 import subprocess
 import os
 from pathlib import Path
 
-from rayasdk.constants import *
-from rayasdk.logger import *
-from rayasdk.utils import *
-from rayasdk.container_handlers.docker_handler import launch_app_on_sim
+import rayasdk.constants as constants
+from rayasdk.logger import log_error, log_info, log_warning
+from rayasdk.utils import open_connection_file, validate_app_id_and_folder_name
+from rayasdk.container_handlers.docker_handler import DockerHandler
 
 
 class URRunner:
 
     COMMAND = 'run'
 
     def __init__(self):
-        pass
+        self.docker_handler = DockerHandler()
 
     def init_parser(self, subparser):
         self.parser = subparser.add_parser(
             type(self).COMMAND,
             add_help=False,
             help="connect current raya project to a robot or simulator.")
         self.parser.add_argument(
@@ -33,126 +33,128 @@
         self.args = args
         self.unknownargs = unknownargs
         # Open connection file
         connection_settings = open_connection_file()
 
         # Open exec_settings file
         try:
-            with open(EXECSETTINGS_PATH, 'r', encoding='utf-8') as f:
+            with open(constants.EXECSETTINGS_PATH, 'r', encoding='utf-8') as f:
                 exec_settings = json.load(f)
-            app_id = exec_settings[JSON_EXECINFO_APPID]
+            app_id = exec_settings[constants.JSON_EXECINFO_APPID]
         except OSError:
-            log_error((f'Could not open "{EXECSETTINGS_FILE}" file, '
+            log_error((f'Could not open "{constants.EXECSETTINGS_FILE}" file, '
                        'project not initialized or file not valid.'))
             return False
         except KeyError as key:
-            log_error(f'{key} key not found on {EXECSETTINGS_FILE}.')
+            log_error(f'{key} key not found on {constants.EXECSETTINGS_FILE}.')
             return False
         # Check if the parent has the same name that the app id
         if not validate_app_id_and_folder_name(app_id):
             log_error('The name of the folder is different from the app-id.')
             return False
 
         # Execute app
         try:
-            if connection_settings[JSON_EXECINFO_SIM]:
+            if connection_settings[constants.JSON_EXECINFO_SIM]:
                 self.run_app_on_simulation(exec_settings, connection_settings)
             else:
                 self.run_app_on_remote(exec_settings, connection_settings)
         except Exception as error:
             log_error(str(error))
             return False
         return True
 
     def run_app_on_simulation(self, exec_settings, connection_settings):
-        app_id = exec_settings[JSON_EXECINFO_APPID]
+        app_id = exec_settings[constants.JSON_EXECINFO_APPID]
         origin_path = os.getcwd()
 
         # Sync the app in the folder of the simulation
         command = \
-            f'rsync --archive --delete {origin_path}/ {SIMS_APPS}/{app_id}'
+            f'rsync --archive --delete {origin_path}/ {constants.SIMS_APPS}/{app_id}'
         subprocess.call(command, shell=True)
 
         if self.args.debug:
             log_info('Waiting for debug client (VSCode)...')
 
-        launch_app_on_sim(app_id=app_id,
-                          args=self.unknownargs,
-                          debug=self.args.debug)
+        self.docker_handler.launch_app_on_sim(
+                app_id=app_id,
+                args=self.unknownargs,
+                debug=self.args.debug
+            )
 
     def run_app_on_remote(self, exec_settings, connection_settings):
-        app_id = exec_settings[JSON_EXECINFO_APPID]
-        robot_id = connection_settings[JSON_EXECINFO_ROBCONN]\
-                                                        [JSON_EXECINFO_ROBID]
-        host = connection_settings[JSON_EXECINFO_ROBCONN][JSON_EXECINFO_ROBIP]
-        hostname = f'{SSH_USER}@{host}'
+        app_id = exec_settings[constants.JSON_EXECINFO_APPID]
+        robot_id = connection_settings[constants.JSON_EXECINFO_ROBCONN]\
+                                                        [constants.JSON_EXECINFO_ROBID]
+        host = connection_settings[constants.JSON_EXECINFO_ROBCONN][constants.JSON_EXECINFO_ROBIP]
+        hostname = f'{constants.SSH_USER}@{host}'
 
         while True:
             try:
                 origin_path = os.getcwd()
                 command = (('rsync '
                             '--archive '
                             '--delete '
-                            f'--rsh=\'ssh -p{SSH_PORT}\' '
+                            f'--rsh=\'ssh -p{constants.SSH_PORT}\' '
                             f'{origin_path}/ '
-                            f'{hostname}:{SSH_APP_FOLDER}/{app_id}'))
+                            f'{hostname}:{constants.SSH_APP_FOLDER}/{app_id}'))
                 subprocess.run(command, shell=True,
                                capture_output=True).check_returncode()
 
             except subprocess.CalledProcessError as e:
                 if 'REMOTE HOST IDENTIFICATION HAS CHANGED' in str(e.stderr):
-                    print()
+                    log_info()
                     log_warning(
                         ('Host ID have changed, run \'rayasdk connect\' '
                          'again'))
                     command = (('ssh-keygen '
                                 f'-f "{Path.home()/".ssh"/"known_hosts"}" '
-                                f'-R "[{host}]:{SSH_PORT}"'))
+                                f'-R "[{host}]:{constants.SSH_PORT}"'))
                     subprocess.run(
                         command,
                         shell=True,
                         stdout=subprocess.DEVNULL,
                         stderr=subprocess.DEVNULL).check_returncode()
                     return
-                print()
+                log_info()
                 log_error('Can not send the app to the robot')
                 if 'No route to host' in str(e.stderr):
-                    print(('No toute to host. Check that the robot is powered'
+                    log_info(('No toute to host. Check that the robot is powered'
                            ' on'))
                 elif 'Connection refused' in str(e.stderr):
-                    print(
+                    log_info(
                         ('Connection refused. Check that the Ra-Ya system is '
                          'running on the robot'))
                 else:
-                    print('Check that the robot is powered on')
-                print(f'Trying to connect to: {robot_id} / {host}')
+                    log_info('Check that the robot is powered on')
+                log_info(f'Trying to connect to: {robot_id} / {host}')
                 return
 
             except Exception as error:
                 log_error(error)
                 return
 
             self.launch_app(app_id, hostname, self.unknownargs)
             return
 
     def launch_app(self, app_id, host_url, args):
-        execution_route = f'%s%s' % (SSH_APP_FOLDER, app_id)
+        execution_route = f'%s%s' % (constants.SSH_APP_FOLDER, app_id)
 
         if self.args.debug:
             cmd = (f'python3 -m debugpy --listen 5678 --wait-for-client '
                    './__main__.py ')
             cmd += ' '.join(args)
             command = (('ssh -2 -t '
                         '-o LogLevel=QUIET '
                         '-L 5678:localhost:5678 '
-                        f'-p {SSH_PORT} {host_url} '
+                        f'-p {constants.SSH_PORT} {host_url} '
                         f'\'cd {execution_route} && {cmd}\''))
-            print('Waiting for debug client (VSCode)...')
+            log_info('Waiting for debug client (VSCode)...')
         else:
             cmd = f'python3 __main__.py ' + ' '.join(args)
             command = (('ssh -t '
                         '-o LogLevel=QUIET '
-                        f'-p {SSH_PORT} {host_url} '
+                        f'-p {constants.SSH_PORT} {host_url} '
                         f'\'cd {execution_route} && {cmd}\''))
 
         subprocess.call(command, shell=True)
-        print('')
+        log_info('')
```

### Comparing `rayasdk-1.1.0.dev6/rayasdk/scanner.py` & `rayasdk-1.1.0.dev7/rayasdk/scanner.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import json
 import select
 import sys
 import time
 from tabulate import tabulate
 from zeroconf import ServiceBrowser, ServiceListener, Zeroconf
 
-from rayasdk.logger import log_error, log_info, log_verbose
-from rayasdk.constants import *
+import rayasdk.constants as constants
+from rayasdk.logger import log_info
 
 robots_info = dict()
 
 
 class URScanner:
     COMMAND = 'scan'
 
@@ -63,20 +63,20 @@
                 zero.close()
         except KeyboardInterrupt:
             pass
         finally:
             zeroconf.close()
 
         try:
-            if not self.__save_last_scan(path=LAST_SCANNING_PATH):
+            if not self.__save_last_scan(path=constants.LAST_SCANNING_PATH):
                 log_info('No robots found.')
             else:
                 log_info('Scan finish correctly')
         except FileNotFoundError:
-            raise Exception(f'Could not write file {LAST_SCANNING_PATH}.')
+            raise Exception(f'Could not write file {constants.LAST_SCANNING_PATH}.')
         return True
 
 
 class MyListener(ServiceListener):
 
     def __init__(self, print=False) -> None:
         self.print = print
```

### Comparing `rayasdk-1.1.0.dev6/rayasdk/sshKeyGen.py` & `rayasdk-1.1.0.dev7/rayasdk/sshKeyGen.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2020 Unlimited Robotics
 
 import os
 import sys
 import subprocess
 import glob
 
-from rayasdk.logger import log_error, log_verbose, log_info
+from rayasdk.logger import log_error, log_verbose
 
 # Constants
 CUR_USER_HOME = os.path.expanduser('~')
 PLATFORM = sys.platform
 
 if PLATFORM == 'windows':
     # https://stackoverflow.com/questions/23064052/how-to-modify-ssh-folder-files-in-windows
```

### Comparing `rayasdk-1.1.0.dev6/rayasdk/template/app.py` & `rayasdk-1.1.0.dev7/rayasdk/template/app.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev6/rayasdk/vcs.py` & `rayasdk-1.1.0.dev7/rayasdk/vcs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import subprocess
 import requests
 import re
 
-from rayasdk.constants import *
-from rayasdk.logger import *
+import rayasdk.constants as constants
+from rayasdk.logger import log_error, log_info, log_success, log_warning
 from rayasdk.messages import *
-from rayasdk.utils import download_simulator, simulator_not_found, RayaOS_not_found
-from rayasdk.container_handlers.docker_handler import *
+from rayasdk.container_handlers.docker_handler import DockerHandler
+from rayasdk.simulator import URSimulator
 
 
 def check_simulation_versions():
     vcs = URVCS()
     # If there is a patch update available, update
     if not vcs.patch_updated():
-        for raya_component in RAYA_OS_COMPONENTS:
+        for raya_component in constants.RAYA_OS_COMPONENTS:
             # Do not check SDK
             if raya_component == 'SDK':
                 continue
             if not vcs.patch_updated(raya_component):
                 log_info(f'Updating {raya_component}')
                 if not vcs.update_patch(raya_component):
                     log_error(f'Could not update {raya_component}')
@@ -27,14 +27,15 @@
         log_info("All components are up to date.")
     # If there is a major/minor version let the user know
     if not vcs.full_updated() or not vcs.minor_updated():
         return False
     else:
         return True
 
+
 def check_sdk_version():
     vcs = URVCS()
     component='SDK'
     if not vcs.full_updated(component=component) or not vcs.minor_updated(component=component):
         latest = vcs.get_latest_version(component=component)
         log_warning((
                 'RayaSDK is not up to date. To update run '
@@ -44,145 +45,134 @@
 
 
 class URVCS:
 
     COMMAND = 'update'
 
     def __init__(self):
-        self.current_version = None
-        self.host_os = platform.system()
+        self.docker_handler = DockerHandler()
+        self.simulator = URSimulator()
+        self.GARYSIM_VERSION = self.simulator.GARYSIM_VERSION
+        self.RAYAENV_DOCKER_VERSION = self.docker_handler.RAYAENV_DOCKER_VERSION
+        self.RAYAENV_DOCKER_IMAGE_NAME = self.docker_handler.RAYAENV_DOCKER_IMAGE_NAME
+
 
     def init_parser(self, subparser):
         self.parser = subparser.add_parser(
             type(self).COMMAND, help='Update the SDK, Unity or Docker')
+    
+    
+    
+
 
     def run(self, args, unknownargs):
         self.args = args
         self.unknownargs = unknownargs
         log_info('Checking for updates...')
         
-        if not self.full_updated() or simulator_not_found() or RayaOS_not_found():
+        if not self.full_updated() or self.simulator.simulator_not_found() or self.docker_handler.RayaOS_not_found():
             download_input = input(f'Do you want to download the Simulator and RayaOS? [Y/n]')
             if download_input not in ['y', 'Y', 'yes', 'Yes', 'YES', '']:
                 return False
         
         if self.update_full():
             log_success('Everything is up to date')
             return True
         else:
             log_error('Update failed.')
             return False
 
+
     def __get_major(self, version):
         return int(version.split('.')[0])
 
+
     def __get_minor(self, version):
         return int(version.split('.')[1])
 
+
     def __get_patch(self, version):
         patch = version.split('.')[2]
         if patch:
             return str(patch)
         return '0'
 
+
     def __local_version(self, component):
         '''
         Return the local version of the component
         '''
         if component == 'SDK':
             res = subprocess.check_output(
                 "pip show rayasdk --version|grep Version | awk '{print $2}'",
                 shell=True)
             return re.findall(r'\d+\.\d+\.\d+', res.decode('utf-8'))[0]
         elif component == 'Unity':
-            return GARYSIM_VERSION
+            return self.GARYSIM_VERSION
         elif component == 'Docker':
-            return RAYAENV_DOCKER_VERSION
+            return self.RAYAENV_DOCKER_VERSION
+
 
     def __get_latest_version(self, component):
         '''
         Return the latest version of the component
         '''
         # response = requests.request("GET", f'{VCS_URL}/latest/{component}')
         # return(data['versionId'])
-        response = requests.request("GET", f'{VCS_URL}')
+        response = requests.request("GET", f'{constants.VCS_URL}')
         data = response.json()
         for raya_component in data:
             if raya_component['name'] == component:
                 return raya_component['versionId']
-
-    def __update_constants_file(self, component):
-        new_lines = []
-        try:
-            with open(f'{UR_HOME}/versions.txt', 'r+') as f:
-                for line in f:
-                    if re.match(r'Docker:\d.\d.\d',
-                                line) and component == 'Docker':
-                        new_lines.append(
-                            f'Docker:{self.__get_latest_version(component)}\n')
-                    elif re.match(r'Unity:\d.\d.\d',
-                                  line) and component == 'Unity':
-                        new_lines.append(
-                            f'Unity:{self.__get_latest_version(component)}')
-                    else:
-                        new_lines.append(line)
-                f.seek(0)
-                f.writelines(new_lines)
-                f.truncate()
-                f.close
-                update_constants()
-                return True
-        except:
-            log_error('Error updating the constants file')
-            return False
-
+       
+            
     def full_updated(self, component=None):
         if component:
             local = self.__local_version(component)
             latest = self.__get_latest_version(component)
             diff_major = self.__get_major(latest) > self.__get_major(local)
             if diff_major:
                 log_warning((f'{component} have a major update, '
                         f'current: \'{local}\' -> latest: \'{latest}\''))
                 return False
             else:
                 return True
         
         updated = True
-        for raya_component in RAYA_OS_COMPONENTS:
+        for raya_component in constants.RAYA_OS_COMPONENTS:
             local = self.__local_version(raya_component)
             latest = self.__get_latest_version(raya_component)
             diff_major = self.__get_major(latest) > self.__get_major(local)
             if diff_major:
                 log_warning((f'{raya_component} have a major update, '
                         f'current: \'{local}\' -> latest: \'{latest}\''))
                 updated = False
         return updated
 
+
     def update_full(self):
         # Update Unity
         if self.__get_latest_version('Unity') != self.__local_version(
-                'Unity') or simulator_not_found():
-            response = requests.request("GET", VCS_URL)
-            if not download_simulator(response=response.json()):
+                'Unity') or self.simulator.simulator_not_found():
+            response = requests.request("GET", constants.VCS_URL)
+            if not self.simulator.download_simulator(response=response.json()):
                 return False
-            self.__update_constants_file('Unity')
             log_success('Simulator updated successfully')
 
         # Update Docker
         if self.__get_latest_version('Docker') != self.__local_version(
-                'Docker') or RayaOS_not_found():
+                'Docker') or self.docker_handler.RayaOS_not_found():
             version = self.__get_latest_version('Docker')
-            if not download_raya_image(version):
+            if not self.docker_handler.download_raya_image(version):
                 return False
-            self.__update_constants_file('Docker')
             log_success('Raya_OS updated successfully')
 
         return True
 
+
     def minor_updated(self, component=None):
         '''Function to check if the latest version is a minor version'''
         if component:
             local = self.__local_version(component)
             latest = self.__get_latest_version(component)
             same_major = self.__get_major(latest) == self.__get_major(local)
             diff_minor = self.__get_minor(latest) > self.__get_minor(local)
@@ -190,44 +180,44 @@
                 log_warning((f'{component} have a minor update, '
                         f'current: \'{local}\' -> latest: \'{latest}\''))
                 return False
             else:
                 return True
         
         updated = True
-        for raya_component in RAYA_OS_COMPONENTS:
+        for raya_component in constants.RAYA_OS_COMPONENTS:
             local = self.__local_version(raya_component)
             latest = self.__get_latest_version(raya_component)
             same_major = self.__get_major(latest) == self.__get_major(local)
             diff_minor = self.__get_minor(latest) > self.__get_minor(local)
             if same_major and diff_minor:
                 log_warning((f'{raya_component} have a minor update, '
                         f'current: \'{local}\' -> latest: \'{latest}\''))
                 updated = False
         return updated
 
+
     def update_minor(self, component):
         download_input = input(f'Do you want to download the Simulator and the Docker Image? [Y/n]\'')
         if download_input not in ['y', 'Y', 'yes', 'Yes', 'YES', '']:
             return False
         
         '''Update the component and return True if the update was successful'''
         if component == 'Unity':
-            response = requests.request("GET", VCS_URL)
+            response = requests.request("GET", constants.VCS_URL)
             version = self.__get_latest_version(component)
-            if download_simulator(response=response.json()):
-                if self.__update_constants_file(component):
-                    return True
+            if self.simulator.download_simulator(response=response.json()):
+                return True
         elif component == 'Docker':
             version = self.__get_latest_version(component)
-            if download_raya_image(version):
-                if self.__update_constants_file(component):
-                    return True
+            if self.docker_handler.download_raya_image(version):
+                return True
         return False
 
+
     def patch_updated(self, component=None):
         '''Function to check if the latest version is a patch'''
         if component:
             local = self.__local_version(component)
             latest = self.__get_latest_version(component)
             same_major = self.__get_major(latest) == self.__get_major(local)
             same_minor = self.__get_minor(latest) == self.__get_minor(local)
@@ -237,37 +227,37 @@
                     (f'{component} have an patch update it is going to be'
                      f' updated to version \'{latest}\', current \'{local}\''))
                 return False
             else:
                 return True
 
         updated = True
-        for raya_component in RAYA_OS_COMPONENTS:
+        for raya_component in constants.RAYA_OS_COMPONENTS:
             local = self.__local_version(raya_component)
             latest = self.__get_latest_version(raya_component)
             same_major = self.__get_major(latest) == self.__get_major(local)
             same_minor = self.__get_minor(latest) == self.__get_minor(local)
             diff_patch = self.__get_patch(local) != self.__get_patch(latest)
             if same_major and same_minor and diff_patch:
                 log_warning(
                     (f'{raya_component} have an patch update it is going to be'
                      f' updated to version \'{latest}\', current \'{local}\''))
                 updated = False
         return updated
 
+
     def update_patch(self, component):
         '''Update the component and return True if the update was successful'''
         if component == 'Unity':
-            response = requests.request("GET", VCS_URL)
+            response = requests.request("GET", constants.VCS_URL)
             version = self.__get_latest_version(component)
-            if download_simulator(response=response.json()):
-                if self.__update_constants_file(component):
-                    return True
+            if self.simulator.download_simulator(response=response.json()):
+                return True
         elif component == 'Docker':
             version = self.__get_latest_version(component)
-            if download_raya_image(version):
-                if self.__update_constants_file(component):
-                    return True
+            if self.docker_handler.download_raya_image(version):
+                return True
         return False
 
+
     def get_latest_version(self, component):
-        return self.__get_latest_version(component=component)
+        return self.__get_latest_version(component=component)
```

### Comparing `rayasdk-1.1.0.dev6/rayasdk.egg-info/PKG-INFO` & `rayasdk-1.1.0.dev7/rayasdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rayasdk
-Version: 1.1.0.dev6
+Version: 1.1.0.dev7
 Summary: Raya SDK - Unlimited Robotics Software Development Kit
 Home-page: UNKNOWN
 Author: Unlimited Robotics
 Author-email: camilo@unlimited-robotics.com
 License: MIT
 Keywords: robotics,unlimited-robotics,gary
 Platform: UNKNOWN
```

### Comparing `rayasdk-1.1.0.dev6/rayasdk.egg-info/SOURCES.txt` & `rayasdk-1.1.0.dev7/rayasdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev6/setup.py` & `rayasdk-1.1.0.dev7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 from pip_tools import get_last_release_version, get_last_prerelease_version
 
-VERSION = '1.1.0.dev6'
+VERSION = '1.1.0.dev7'
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='rayasdk',
     packages=find_packages(),
```

