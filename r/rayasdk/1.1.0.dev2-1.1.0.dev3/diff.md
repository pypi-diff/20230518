# Comparing `tmp/rayasdk-1.1.0.dev2.tar.gz` & `tmp/rayasdk-1.1.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rayasdk-1.1.0.dev2.tar", last modified: Fri May 12 17:02:31 2023, max compression
+gzip compressed data, was "rayasdk-1.1.0.dev3.tar", last modified: Thu May 18 03:49:44 2023, max compression
```

## Comparing `rayasdk-1.1.0.dev2.tar` & `rayasdk-1.1.0.dev3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 santiagour  (1000) santiagour  (1000)        0 2023-05-12 17:02:31.632375 rayasdk-1.1.0.dev2/
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     6569 2023-05-12 17:02:31.632375 rayasdk-1.1.0.dev2/PKG-INFO
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     6219 2023-05-12 15:27:54.000000 rayasdk-1.1.0.dev2/README.md
-drwxrwxr-x   0 santiagour  (1000) santiagour  (1000)        0 2023-05-12 17:02:31.632375 rayasdk-1.1.0.dev2/rayasdk/
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)      546 2023-05-10 14:28:01.000000 rayasdk-1.1.0.dev2/rayasdk/__init__.py
--rwxrwxr-x   0 santiagour  (1000) santiagour  (1000)     4888 2023-05-10 18:21:31.000000 rayasdk-1.1.0.dev2/rayasdk/__main__.py
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     5150 2023-05-10 16:24:09.000000 rayasdk-1.1.0.dev2/rayasdk/connect.py
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     6202 2023-05-12 15:57:49.000000 rayasdk-1.1.0.dev2/rayasdk/constants.py
-drwxrwxr-x   0 santiagour  (1000) santiagour  (1000)        0 2023-05-12 17:02:31.632375 rayasdk-1.1.0.dev2/rayasdk/container_handlers/
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)        0 2023-05-04 20:26:47.000000 rayasdk-1.1.0.dev2/rayasdk/container_handlers/__init__.py
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     5576 2023-05-12 16:35:40.000000 rayasdk-1.1.0.dev2/rayasdk/container_handlers/docker_handler.py
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     9930 2023-05-12 17:01:05.000000 rayasdk-1.1.0.dev2/rayasdk/container_handlers/vcs.py
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     2568 2023-05-10 14:28:01.000000 rayasdk-1.1.0.dev2/rayasdk/initializer.py
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     1342 2023-05-10 14:28:01.000000 rayasdk-1.1.0.dev2/rayasdk/killer.py
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     1346 2023-05-10 14:28:01.000000 rayasdk-1.1.0.dev2/rayasdk/logger.py
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)      819 2023-05-10 14:28:01.000000 rayasdk-1.1.0.dev2/rayasdk/messages.py
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     5993 2023-05-12 15:27:54.000000 rayasdk-1.1.0.dev2/rayasdk/runner.py
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     4396 2023-05-10 16:24:09.000000 rayasdk-1.1.0.dev2/rayasdk/scanner.py
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     1749 2023-05-12 15:27:54.000000 rayasdk-1.1.0.dev2/rayasdk/simulator.py
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     2667 2023-05-10 16:38:58.000000 rayasdk-1.1.0.dev2/rayasdk/sshKeyGen.py
-drwxrwxr-x   0 santiagour  (1000) santiagour  (1000)        0 2023-05-12 17:02:31.632375 rayasdk-1.1.0.dev2/rayasdk/template/
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)      244 2023-05-04 20:26:47.000000 rayasdk-1.1.0.dev2/rayasdk/template/__main__.py
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)      551 2023-05-10 14:28:01.000000 rayasdk-1.1.0.dev2/rayasdk/template/app.py
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)      399 2023-05-10 14:16:37.000000 rayasdk-1.1.0.dev2/rayasdk/template/launch.json
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)      108 2023-05-04 20:26:47.000000 rayasdk-1.1.0.dev2/rayasdk/template/manifest.json
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     3123 2023-05-12 15:27:59.000000 rayasdk-1.1.0.dev2/rayasdk/utils.py
-drwxrwxr-x   0 santiagour  (1000) santiagour  (1000)        0 2023-05-12 17:02:31.632375 rayasdk-1.1.0.dev2/rayasdk.egg-info/
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     6569 2023-05-12 17:02:31.000000 rayasdk-1.1.0.dev2/rayasdk.egg-info/PKG-INFO
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)      702 2023-05-12 17:02:31.000000 rayasdk-1.1.0.dev2/rayasdk.egg-info/SOURCES.txt
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)        1 2023-05-12 17:02:31.000000 rayasdk-1.1.0.dev2/rayasdk.egg-info/dependency_links.txt
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)       51 2023-05-12 17:02:31.000000 rayasdk-1.1.0.dev2/rayasdk.egg-info/entry_points.txt
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)      103 2023-05-12 17:02:31.000000 rayasdk-1.1.0.dev2/rayasdk.egg-info/requires.txt
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)        8 2023-05-12 17:02:31.000000 rayasdk-1.1.0.dev2/rayasdk.egg-info/top_level.txt
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)       79 2023-05-12 17:02:31.632375 rayasdk-1.1.0.dev2/setup.cfg
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)      934 2023-05-12 17:02:21.000000 rayasdk-1.1.0.dev2/setup.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 03:49:44.264396 rayasdk-1.1.0.dev3/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     6569 2023-05-18 03:49:44.264396 rayasdk-1.1.0.dev3/PKG-INFO
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     6219 2023-05-11 21:39:47.000000 rayasdk-1.1.0.dev3/README.md
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 03:49:44.264396 rayasdk-1.1.0.dev3/rayasdk/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      546 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev3/rayasdk/__init__.py
+-rwxrwxr-x   0 camilo    (1000) camilo    (1000)     5154 2023-05-17 15:09:08.000000 rayasdk-1.1.0.dev3/rayasdk/__main__.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     5150 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev3/rayasdk/connect.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     6198 2023-05-17 15:09:08.000000 rayasdk-1.1.0.dev3/rayasdk/constants.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 03:49:44.264396 rayasdk-1.1.0.dev3/rayasdk/container_handlers/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-02-22 08:37:00.000000 rayasdk-1.1.0.dev3/rayasdk/container_handlers/__init__.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     5576 2023-05-17 15:09:08.000000 rayasdk-1.1.0.dev3/rayasdk/container_handlers/docker_handler.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     2568 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev3/rayasdk/initializer.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     1342 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev3/rayasdk/killer.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     1513 2023-05-17 15:09:08.000000 rayasdk-1.1.0.dev3/rayasdk/logger.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      819 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev3/rayasdk/messages.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     5993 2023-05-11 21:39:47.000000 rayasdk-1.1.0.dev3/rayasdk/runner.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     4396 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev3/rayasdk/scanner.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     1749 2023-05-11 21:39:47.000000 rayasdk-1.1.0.dev3/rayasdk/simulator.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     2667 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev3/rayasdk/sshKeyGen.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 03:49:44.264396 rayasdk-1.1.0.dev3/rayasdk/template/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      244 2023-02-22 08:37:00.000000 rayasdk-1.1.0.dev3/rayasdk/template/__main__.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      551 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev3/rayasdk/template/app.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      399 2023-04-17 17:27:42.000000 rayasdk-1.1.0.dev3/rayasdk/template/launch.json
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      108 2023-02-22 08:37:00.000000 rayasdk-1.1.0.dev3/rayasdk/template/manifest.json
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     3252 2023-05-17 15:09:08.000000 rayasdk-1.1.0.dev3/rayasdk/utils.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)    11007 2023-05-17 15:09:08.000000 rayasdk-1.1.0.dev3/rayasdk/vcs.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 03:49:44.264396 rayasdk-1.1.0.dev3/rayasdk.egg-info/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     6569 2023-05-18 03:49:44.000000 rayasdk-1.1.0.dev3/rayasdk.egg-info/PKG-INFO
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      683 2023-05-18 03:49:44.000000 rayasdk-1.1.0.dev3/rayasdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)        1 2023-05-18 03:49:44.000000 rayasdk-1.1.0.dev3/rayasdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)       51 2023-05-18 03:49:44.000000 rayasdk-1.1.0.dev3/rayasdk.egg-info/entry_points.txt
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      115 2023-05-18 03:49:44.000000 rayasdk-1.1.0.dev3/rayasdk.egg-info/requires.txt
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)        8 2023-05-18 03:49:44.000000 rayasdk-1.1.0.dev3/rayasdk.egg-info/top_level.txt
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)       79 2023-05-18 03:49:44.264396 rayasdk-1.1.0.dev3/setup.cfg
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     1253 2023-05-18 03:47:17.000000 rayasdk-1.1.0.dev3/setup.py
```

### Comparing `rayasdk-1.1.0.dev2/PKG-INFO` & `rayasdk-1.1.0.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rayasdk
-Version: 1.1.0.dev2
+Version: 1.1.0.dev3
 Summary: Raya SDK - Unlimited Robotics Software Development Kit
 Home-page: UNKNOWN
 Author: Unlimited Robotics
 Author-email: camilo@unlimited-robotics.com
 License: MIT
 Keywords: robotics,unlimited-robotics,gary
 Platform: UNKNOWN
```

### Comparing `rayasdk-1.1.0.dev2/README.md` & `rayasdk-1.1.0.dev3/README.md`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev2/rayasdk/__init__.py` & `rayasdk-1.1.0.dev3/rayasdk/__init__.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev2/rayasdk/__main__.py` & `rayasdk-1.1.0.dev3/rayasdk/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import argparse
 import os
 import sys
 import platform
 
 from rayasdk.connect import URConnect
-from rayasdk.container_handlers.vcs import URVCS, check_versions
+from rayasdk.vcs import URVCS, check_simulation_versions, check_sdk_version
 from rayasdk.logger import log_error, log_verbose, set_logger_level
 from rayasdk.scanner import URScanner
 from rayasdk.initializer import URInitializer
 from rayasdk.runner import URRunner
 from rayasdk.simulator import URSimulator
 from rayasdk.killer import URKiller
 from rayasdk.constants import *
@@ -102,18 +102,21 @@
             # Check for temp folder
             if not self.init_ursdk_folder():
                 return False
             # Check .ur folder
             if not self.check_global_folder():
                 log_error(f'Could not create .ur folder')
                 return False
-            # Do not check version on update
-            if self.args.command != URVCS().COMMAND:
-                # Check versions
-                if not check_versions():
+            # Check if sdk have an update
+            check_sdk_version()
+            # Check simulation version on simulator and update command
+            if self.args.command == URSimulator().COMMAND:
+                updated = check_simulation_versions()
+                if not updated and self.args.command == URSimulator().COMMAND:
+                    log_error('RayaOS is not up to date. To update run "rayasdk update"')
                     return False
             # Execute Command
             for obj in self.command_objects:
                 if self.args.command == type(obj).COMMAND:
                     return obj.run(self.args, self.unknownargs)
         except Exception as e:
             log_error(str(e))
```

### Comparing `rayasdk-1.1.0.dev2/rayasdk/connect.py` & `rayasdk-1.1.0.dev3/rayasdk/connect.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev2/rayasdk/constants.py` & `rayasdk-1.1.0.dev3/rayasdk/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 MANIFEST_PATH_ORIG = TEMPLATES_PATH / MANIFEST_FILE
 MANIFEST_PATH_DEST = CURRENT_PATH / MANIFEST_FILE
 EXECSETTINGS_PATH = CURRENT_PATH / EXECSETTINGS_FILE
 CONNECTION_SETTINGS_PATH = UR_HOME / CONNECTION_SETTINGS_FILE
 
 # Docker Environment
 RAYAENV_DOCKER_UR_ROOT = SIMS_HOME / 'ur_root'
-RAYAENV_DOCKER_UR_ROOT_REPO = 'git clone --branch garyunity git@github.com:Unlimited-Robotics/raya_root_folder_templates.git'
+RAYAENV_DOCKER_UR_ROOT_REPO = 'git clone --branch main git@github.com:Unlimited-Robotics/raya_root_folder_simulation.git'
 RAYAENV_DOCKER_IMGNAME = 'raya_os'
 RAYAENV_DOCKER_IMGNAME_DEV = 'raya_sim_dev'
 RAYAENV_DOCKER_IMG_VERSION_NAME = 'sim'
 RAYAENV_DOCKER_IMG_VERSION_GPU = 'sim_gpu'
 
 
 def check_if_gpu():
```

### Comparing `rayasdk-1.1.0.dev2/rayasdk/container_handlers/docker_handler.py` & `rayasdk-1.1.0.dev3/rayasdk/container_handlers/docker_handler.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev2/rayasdk/container_handlers/vcs.py` & `rayasdk-1.1.0.dev3/rayasdk/vcs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,49 @@
 import subprocess
 import requests
 import re
 
 from rayasdk.constants import *
 from rayasdk.logger import *
 from rayasdk.messages import *
-from rayasdk.utils import download_simulator
+from rayasdk.utils import download_simulator, simulator_not_found, RayaOS_not_found
 from rayasdk.container_handlers.docker_handler import *
 
 
-def check_versions():
+def check_simulation_versions():
     vcs = URVCS()
-    # If there is a major/minor version let the user know
-    if not vcs.full_updated() or not vcs.minor_updated():
-        log_warning('RayaOS is not up to date. To update run "rayasdk update"')
     # If there is a patch update available, update
     if not vcs.patch_updated():
-        for cpm in RAYA_OS_COMPONENTS:
-            if not vcs.patch_updated(cpm):
-                log_info(f'Updating {cpm}')
-                if not vcs.update_patch(cpm):
-                    log_error(f'Could not update {cpm}')
+        for raya_component in RAYA_OS_COMPONENTS:
+            # Do not check SDK
+            if raya_component == 'SDK':
+                continue
+            if not vcs.patch_updated(raya_component):
+                log_info(f'Updating {raya_component}')
+                if not vcs.update_patch(raya_component):
+                    log_error(f'Could not update {raya_component}')
                     return False
                 log_info('Run the command again')
                 return False
         log_info("All components are up to date.")
+    # If there is a major/minor version let the user know
+    if not vcs.full_updated() or not vcs.minor_updated():
+        return False
+    else:
+        return True
+
+def check_sdk_version():
+    vcs = URVCS()
+    component='SDK'
+    if not vcs.full_updated(component=component) or not vcs.minor_updated(component=component):
+        latest = vcs.get_latest_version(component=component)
+        log_warning((
+                'RayaSDK is not up to date. To update run '
+                f'\'pip install rayasdk=={latest}\''
+            ))
     return True
 
 
 class URVCS:
 
     COMMAND = 'update'
 
@@ -40,16 +55,22 @@
         self.parser = subparser.add_parser(
             type(self).COMMAND, help='Update the SDK, Unity or Docker')
 
     def run(self, args, unknownargs):
         self.args = args
         self.unknownargs = unknownargs
         log_info('Checking for updates...')
+        
+        if not self.full_updated() or simulator_not_found() or RayaOS_not_found():
+            download_input = input(f'Do you want to download the Simulator and RayaOS? [Y/n]')
+            if download_input not in ['y', 'Y', 'yes', 'Yes', 'YES', '']:
+                return False
+        
         if self.update_full():
-            log_info('Everything is up to date')
+            log_success('Everything is up to date')
             return True
         else:
             log_error('Update failed.')
             return False
 
     def __get_major(self, version):
         return int(version.split('.')[0])
@@ -110,96 +131,91 @@
                 f.close
                 update_constants()
                 return True
         except:
             log_error('Error updating the constants file')
             return False
 
-    def __update_sdk_packages(self):
-        return True
-        try:
-            pip_process = subprocess.Popen('pip install --upgrade rayasdk',
-                                           shell=True,
-                                           stdin=subprocess.PIPE,
-                                           stdout=subprocess.PIPE,
-                                           stderr=subprocess.PIPE)
-            output, err = pip_process.communicate()
-            if pip_process.returncode != 0:
-                log_error(err.decode())
-                raise Exception('pip upgrade failed')
-            return True
-        except Exception as error:
-            log_error(str(error))
-            return False
-
-    def full_updated(self):
-        for cpm in RAYA_OS_COMPONENTS:
-            local = self.__local_version(cpm)
-            latest = self.__get_latest_version(cpm)
+    def full_updated(self, component=None):
+        if component:
+            local = self.__local_version(component)
+            latest = self.__get_latest_version(component)
             diff_major = self.__get_major(latest) > self.__get_major(local)
             if diff_major:
+                log_warning((f'{component} have a major update, '
+                        f'current: \'{local}\' -> latest: \'{latest}\''))
                 return False
-        return True
+            else:
+                return True
+        
+        updated = True
+        for raya_component in RAYA_OS_COMPONENTS:
+            local = self.__local_version(raya_component)
+            latest = self.__get_latest_version(raya_component)
+            diff_major = self.__get_major(latest) > self.__get_major(local)
+            if diff_major:
+                log_warning((f'{raya_component} have a major update, '
+                        f'current: \'{local}\' -> latest: \'{latest}\''))
+                updated = False
+        return updated
 
     def update_full(self):
-
-        # update SDK
-        if self.__get_latest_version('SDK') != self.__local_version('SDK'):
-            if not self.__update_sdk_packages():
-                return False
-            self.__update_constants_file('SDK')
-            log_warning('SDK updated successfully')
-
         # Update Unity
         if self.__get_latest_version('Unity') != self.__local_version(
-                'Unity') or not os.path.exists(f'{SIM_BINARY}'):
+                'Unity') or simulator_not_found():
             response = requests.request("GET", VCS_URL)
             if not download_simulator(response=response.json()):
                 return False
             self.__update_constants_file('Unity')
-            log_warning('Simulator updated successfully')
+            log_success('Simulator updated successfully')
 
         # Update Docker
         if self.__get_latest_version('Docker') != self.__local_version(
-                'Docker') or not check_image():
+                'Docker') or RayaOS_not_found():
             version = self.__get_latest_version('Docker')
             if not download_raya_image(version):
                 return False
             self.__update_constants_file('Docker')
-            log_warning('Raya_OS updated successfully')
+            log_success('Raya_OS updated successfully')
 
         return True
 
     def minor_updated(self, component=None):
         '''Function to check if the latest version is a minor version'''
         if component:
             local = self.__local_version(component)
             latest = self.__get_latest_version(component)
             same_major = self.__get_major(latest) == self.__get_major(local)
             diff_minor = self.__get_minor(latest) > self.__get_minor(local)
             if same_major and diff_minor:
-                log_info(f'{component} have an update')
+                log_warning((f'{component} have a minor update, '
+                        f'current: \'{local}\' -> latest: \'{latest}\''))
                 return False
-
+            else:
+                return True
+        
+        updated = True
         for raya_component in RAYA_OS_COMPONENTS:
             local = self.__local_version(raya_component)
             latest = self.__get_latest_version(raya_component)
             same_major = self.__get_major(latest) == self.__get_major(local)
             diff_minor = self.__get_minor(latest) > self.__get_minor(local)
             if same_major and diff_minor:
-                log_info((f'{raya_component} have a minor update, '
-                          f'current: \'{local}\' -> latest: \'{latest}\''))
-                return False
-        return True
+                log_warning((f'{raya_component} have a minor update, '
+                        f'current: \'{local}\' -> latest: \'{latest}\''))
+                updated = False
+        return updated
 
     def update_minor(self, component):
+        download_input = input(f'Do you want to download the Simulator and the Docker Image? [Y/n]\'')
+        if download_input not in ['y', 'Y', 'yes', 'Yes', 'YES', '']:
+            return False
+        
         '''Update the component and return True if the update was successful'''
-        if component == 'SDK':
-            self.__update_sdk_packages()
-        elif component == 'Unity':
+        if component == 'Unity':
             response = requests.request("GET", VCS_URL)
             version = self.__get_latest_version(component)
             if download_simulator(response=response.json()):
                 if self.__update_constants_file(component):
                     return True
         elif component == 'Docker':
             version = self.__get_latest_version(component)
@@ -213,40 +229,45 @@
         if component:
             local = self.__local_version(component)
             latest = self.__get_latest_version(component)
             same_major = self.__get_major(latest) == self.__get_major(local)
             same_minor = self.__get_minor(latest) == self.__get_minor(local)
             diff_patch = self.__get_patch(local) != self.__get_patch(latest)
             if same_major and same_minor and diff_patch:
+                log_warning(
+                    (f'{component} have an patch update it is going to be'
+                     f' updated to version \'{latest}\', current \'{local}\''))
                 return False
             else:
                 return True
 
+        updated = True
         for raya_component in RAYA_OS_COMPONENTS:
             local = self.__local_version(raya_component)
             latest = self.__get_latest_version(raya_component)
             same_major = self.__get_major(latest) == self.__get_major(local)
             same_minor = self.__get_minor(latest) == self.__get_minor(local)
             diff_patch = self.__get_patch(local) != self.__get_patch(latest)
             if same_major and same_minor and diff_patch:
-                log_info(
+                log_warning(
                     (f'{raya_component} have an patch update it is going to be'
                      f' updated to version \'{latest}\', current \'{local}\''))
-                return False
-        return True
+                updated = False
+        return updated
 
     def update_patch(self, component):
         '''Update the component and return True if the update was successful'''
-        if component == 'SDK':
-            self.__update_sdk_packages()
-        elif component == 'Unity':
+        if component == 'Unity':
             response = requests.request("GET", VCS_URL)
             version = self.__get_latest_version(component)
             if download_simulator(response=response.json()):
                 if self.__update_constants_file(component):
                     return True
         elif component == 'Docker':
             version = self.__get_latest_version(component)
             if download_raya_image(version):
                 if self.__update_constants_file(component):
                     return True
         return False
+
+    def get_latest_version(self, component):
+        return self.__get_latest_version(component=component)
```

### Comparing `rayasdk-1.1.0.dev2/rayasdk/initializer.py` & `rayasdk-1.1.0.dev3/rayasdk/initializer.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev2/rayasdk/killer.py` & `rayasdk-1.1.0.dev3/rayasdk/killer.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev2/rayasdk/logger.py` & `rayasdk-1.1.0.dev3/rayasdk/logger.py`

 * *Files 24% similar despite different names*

```diff
@@ -55,7 +55,13 @@
 
 
 def log_error(msg, end='\n', flush=False):
     log(LogLevels.ERROR,
         f'{bcolors.FAIL}ERROR:{bcolors.ENDC} {msg}',
         end=end,
         flush=flush)
+
+def log_success(msg, end='\n', flush=False):
+    log(LogLevels.ERROR,
+        f'{bcolors.OKGREEN}SUCCESS:{bcolors.ENDC} {msg}',
+        end=end,
+        flush=flush)
```

### Comparing `rayasdk-1.1.0.dev2/rayasdk/messages.py` & `rayasdk-1.1.0.dev3/rayasdk/messages.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev2/rayasdk/runner.py` & `rayasdk-1.1.0.dev3/rayasdk/runner.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev2/rayasdk/scanner.py` & `rayasdk-1.1.0.dev3/rayasdk/scanner.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev2/rayasdk/simulator.py` & `rayasdk-1.1.0.dev3/rayasdk/simulator.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev2/rayasdk/sshKeyGen.py` & `rayasdk-1.1.0.dev3/rayasdk/sshKeyGen.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev2/rayasdk/template/app.py` & `rayasdk-1.1.0.dev3/rayasdk/template/app.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev2/rayasdk/utils.py` & `rayasdk-1.1.0.dev3/rayasdk/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,7 +101,13 @@
         with open(CONNECTION_SETTINGS_PATH, 'r', encoding='utf-8') as f:
             connection_settings = json.load(f)
         return connection_settings
     except OSError:
         raise Exception(
             (f'the file "{CONNECTION_SETTINGS_FILE}" was not found, '
              'run \'rayasdk connect\''))
+
+def simulator_not_found():
+    return not os.path.exists(f'{SIM_BINARY}')
+
+def RayaOS_not_found():
+    return not check_image()
```

### Comparing `rayasdk-1.1.0.dev2/rayasdk.egg-info/PKG-INFO` & `rayasdk-1.1.0.dev3/rayasdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rayasdk
-Version: 1.1.0.dev2
+Version: 1.1.0.dev3
 Summary: Raya SDK - Unlimited Robotics Software Development Kit
 Home-page: UNKNOWN
 Author: Unlimited Robotics
 Author-email: camilo@unlimited-robotics.com
 License: MIT
 Keywords: robotics,unlimited-robotics,gary
 Platform: UNKNOWN
```

### Comparing `rayasdk-1.1.0.dev2/rayasdk.egg-info/SOURCES.txt` & `rayasdk-1.1.0.dev3/rayasdk.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 rayasdk/logger.py
 rayasdk/messages.py
 rayasdk/runner.py
 rayasdk/scanner.py
 rayasdk/simulator.py
 rayasdk/sshKeyGen.py
 rayasdk/utils.py
+rayasdk/vcs.py
 rayasdk.egg-info/PKG-INFO
 rayasdk.egg-info/SOURCES.txt
 rayasdk.egg-info/dependency_links.txt
 rayasdk.egg-info/entry_points.txt
 rayasdk.egg-info/requires.txt
 rayasdk.egg-info/top_level.txt
 rayasdk/container_handlers/__init__.py
 rayasdk/container_handlers/docker_handler.py
-rayasdk/container_handlers/vcs.py
 rayasdk/template/__main__.py
 rayasdk/template/app.py
 rayasdk/template/launch.json
 rayasdk/template/manifest.json
```

### Comparing `rayasdk-1.1.0.dev2/setup.py` & `rayasdk-1.1.0.dev3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,46 @@
 from setuptools import setup, find_packages
+from pip_tools import get_last_release_version, get_last_prerelease_version
+
+VERSION = '1.1.0.dev3'
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
+if 'dev' in VERSION:
+    RAYA_VERSION = get_last_prerelease_version('raya')
+else:
+    RAYA_VERSION = get_last_release_version('raya')
+
 setup(
     name='rayasdk',
     packages=find_packages(),
-    version='1.1.0.dev2',
+    version=VERSION,
     license='MIT',
     description='Raya SDK - Unlimited Robotics Software Development Kit',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Unlimited Robotics',
     author_email='camilo@unlimited-robotics.com',
     url='',
     python_requires=">=3.8",
     download_url='',
     package_data={'': ['./template/*']},
     keywords=['robotics', 'unlimited-robotics', 'gary'],
     install_requires=[
-        'tabulate', 'importlib_metadata', 'tqdm', 'docker', 'progressbar',
-        'simple_file_checksum', 'gsutil', 'zeroconf', 'raya', 'paramiko'
+        f'raya=={RAYA_VERSION}',
+        'tabulate', 
+        'importlib_metadata', 
+        'tqdm', 
+        'docker', 
+        'progressbar',
+        'simple_file_checksum', 
+        'gsutil', 
+        'zeroconf', 
+        'paramiko',
     ],
     entry_points={
         'console_scripts': [
             'rayasdk = rayasdk.__main__:main',
         ],
     },
 )
```

