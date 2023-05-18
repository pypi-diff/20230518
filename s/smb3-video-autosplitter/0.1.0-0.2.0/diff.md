# Comparing `tmp/smb3-video-autosplitter-0.1.0.tar.gz` & `tmp/smb3-video-autosplitter-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smb3-video-autosplitter-0.1.0.tar", last modified: Thu May 18 02:23:05 2023, max compression
+gzip compressed data, was "smb3-video-autosplitter-0.2.0.tar", last modified: Thu May 18 13:49:18 2023, max compression
```

## Comparing `smb3-video-autosplitter-0.1.0.tar` & `smb3-video-autosplitter-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 02:23:05.654145 smb3-video-autosplitter-0.1.0/
--rw-rw-rw-   0        0        0    35797 2021-01-02 05:14:00.000000 smb3-video-autosplitter-0.1.0/LICENSE
--rw-rw-rw-   0        0        0       67 2021-01-02 05:14:00.000000 smb3-video-autosplitter-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      555 2023-05-18 02:23:05.654145 smb3-video-autosplitter-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1414 2023-05-17 21:05:02.000000 smb3-video-autosplitter-0.1.0/README.rst
--rw-rw-rw-   0        0        0       91 2022-12-07 15:46:05.000000 smb3-video-autosplitter-0.1.0/requirements_test.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 02:23:05.654145 smb3-video-autosplitter-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      893 2023-05-18 02:22:51.000000 smb3-video-autosplitter-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-18 02:23:05.647138 smb3-video-autosplitter-0.1.0/smb3_video_autosplitter/
--rw-rw-rw-   0        0        0        0 2021-01-02 05:14:00.000000 smb3-video-autosplitter-0.1.0/smb3_video_autosplitter/__init__.py
--rw-rw-rw-   0        0        0     1924 2023-05-18 02:15:00.000000 smb3-video-autosplitter-0.1.0/smb3_video_autosplitter/autosplitter.py
--rw-rw-rw-   0        0        0     1333 2023-05-18 01:05:58.000000 smb3-video-autosplitter-0.1.0/smb3_video_autosplitter/livesplit.py
--rw-rw-rw-   0        0        0      767 2023-05-18 02:14:04.000000 smb3-video-autosplitter-0.1.0/smb3_video_autosplitter/logging.py
--rw-rw-rw-   0        0        0     1636 2023-05-18 02:21:11.000000 smb3-video-autosplitter-0.1.0/smb3_video_autosplitter/main.py
--rw-rw-rw-   0        0        0      774 2023-05-18 02:21:26.000000 smb3-video-autosplitter-0.1.0/smb3_video_autosplitter/opencv.py
--rw-rw-rw-   0        0        0      801 2023-05-18 02:04:57.000000 smb3-video-autosplitter-0.1.0/smb3_video_autosplitter/settings.py
--rw-rw-rw-   0        0        0     1552 2023-05-18 02:14:40.000000 smb3-video-autosplitter-0.1.0/smb3_video_autosplitter/util.py
-drwxrwxrwx   0        0        0        0 2023-05-18 02:23:05.653144 smb3-video-autosplitter-0.1.0/smb3_video_autosplitter.egg-info/
--rw-rw-rw-   0        0        0      555 2023-05-18 02:23:05.000000 smb3-video-autosplitter-0.1.0/smb3_video_autosplitter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      619 2023-05-18 02:23:05.000000 smb3-video-autosplitter-0.1.0/smb3_video_autosplitter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 02:23:05.000000 smb3-video-autosplitter-0.1.0/smb3_video_autosplitter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-18 02:23:05.000000 smb3-video-autosplitter-0.1.0/smb3_video_autosplitter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2023-05-18 02:23:05.000000 smb3-video-autosplitter-0.1.0/smb3_video_autosplitter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-18 02:22:59.000000 smb3-video-autosplitter-0.1.0/smb3_video_autosplitter.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-05-18 13:49:18.991605 smb3-video-autosplitter-0.2.0/
+-rw-rw-rw-   0        0        0    35797 2021-01-02 05:14:00.000000 smb3-video-autosplitter-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0       67 2021-01-02 05:14:00.000000 smb3-video-autosplitter-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      555 2023-05-18 13:49:18.991605 smb3-video-autosplitter-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1414 2023-05-17 21:05:02.000000 smb3-video-autosplitter-0.2.0/README.rst
+-rw-rw-rw-   0        0        0       91 2022-12-07 15:46:05.000000 smb3-video-autosplitter-0.2.0/requirements_test.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 13:49:18.991605 smb3-video-autosplitter-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      893 2023-05-18 13:48:52.000000 smb3-video-autosplitter-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 13:49:18.985600 smb3-video-autosplitter-0.2.0/smb3_video_autosplitter/
+-rw-rw-rw-   0        0        0        0 2021-01-02 05:14:00.000000 smb3-video-autosplitter-0.2.0/smb3_video_autosplitter/__init__.py
+-rw-rw-rw-   0        0        0     1994 2023-05-18 13:42:53.000000 smb3-video-autosplitter-0.2.0/smb3_video_autosplitter/autosplitter.py
+-rw-rw-rw-   0        0        0     1390 2023-05-18 13:20:19.000000 smb3-video-autosplitter-0.2.0/smb3_video_autosplitter/livesplit.py
+-rw-rw-rw-   0        0        0      767 2023-05-18 02:14:04.000000 smb3-video-autosplitter-0.2.0/smb3_video_autosplitter/logging.py
+-rw-rw-rw-   0        0        0     1636 2023-05-18 02:21:11.000000 smb3-video-autosplitter-0.2.0/smb3_video_autosplitter/main.py
+-rw-rw-rw-   0        0        0      774 2023-05-18 02:21:26.000000 smb3-video-autosplitter-0.2.0/smb3_video_autosplitter/opencv.py
+-rw-rw-rw-   0        0        0      791 2023-05-18 13:41:47.000000 smb3-video-autosplitter-0.2.0/smb3_video_autosplitter/settings.py
+-rw-rw-rw-   0        0        0     1552 2023-05-18 02:14:40.000000 smb3-video-autosplitter-0.2.0/smb3_video_autosplitter/util.py
+drwxrwxrwx   0        0        0        0 2023-05-18 13:49:18.990604 smb3-video-autosplitter-0.2.0/smb3_video_autosplitter.egg-info/
+-rw-rw-rw-   0        0        0      555 2023-05-18 13:49:18.000000 smb3-video-autosplitter-0.2.0/smb3_video_autosplitter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      619 2023-05-18 13:49:18.000000 smb3-video-autosplitter-0.2.0/smb3_video_autosplitter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 13:49:18.000000 smb3-video-autosplitter-0.2.0/smb3_video_autosplitter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-18 13:49:18.000000 smb3-video-autosplitter-0.2.0/smb3_video_autosplitter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2023-05-18 13:49:18.000000 smb3-video-autosplitter-0.2.0/smb3_video_autosplitter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-18 13:49:12.000000 smb3-video-autosplitter-0.2.0/smb3_video_autosplitter.egg-info/zip-safe
```

### Comparing `smb3-video-autosplitter-0.1.0/LICENSE` & `smb3-video-autosplitter-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smb3-video-autosplitter-0.1.0/PKG-INFO` & `smb3-video-autosplitter-0.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smb3-video-autosplitter
-Version: 0.1.0
+Version: 0.2.0
 Summary: Ingest video data to render smb3 eh manip stimuli
 Author: narfman0
 Author-email: narfman0@blastedstudios.com
 License: LICENSE
 Keywords: smb3-video-autosplitter
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `smb3-video-autosplitter-0.1.0/README.rst` & `smb3-video-autosplitter-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `smb3-video-autosplitter-0.1.0/setup.py` & `smb3-video-autosplitter-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="smb3-video-autosplitter",
-    version="0.1.0",
+    version="0.2.0",
     description=("Ingest video data to render smb3 eh manip stimuli"),
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `smb3-video-autosplitter-0.1.0/smb3_video_autosplitter/autosplitter.py` & `smb3-video-autosplitter-0.2.0/smb3_video_autosplitter/autosplitter.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 import cv2
 
 from smb3_video_autosplitter.livesplit import Livesplit
 from smb3_video_autosplitter.settings import Settings
 from smb3_video_autosplitter.util import locate_all_opencv
 
 LOGGER = logging.getLogger(__name__)
-SPLIT_COMMAND_NAME = "startorsplit"
 
 
 @dataclass
 class Split:
     path: str
     image: any
     region: list[int, int, int, int]
+    command_name: str
 
 
 class Autosplitter:
     def __init__(self, settings: Settings):
         self.settings = settings
         self.initialize_splits()
         self.earliest_next_trigger_time = 0
@@ -46,15 +46,18 @@
                 time.sleep(self.split_offset_s)
                 self.earliest_next_trigger_time = (
                     time.time() + self.settings.split_dedupe_wait_s
                 )
                 LOGGER.info(
                     f"Splitting after {split.path} observed {len(results)} times at {list(map(str, results))}"
                 )
-                self.livesplit.send(SPLIT_COMMAND_NAME)
+                self.livesplit.send(split.command_name)
 
     def initialize_splits(self):
         self.splits: list[Split] = []
         for split in self.settings.splits:
             image = cv2.imread(split.path)
             region = [split.x, split.y, split.width, split.height]
-            self.splits.append(Split(split.path, image, region))
+            self.splits.append(Split(split.path, image, region, split.command_name))
+
+    def terminate(self):
+        self.livesplit.terminate()
```

### Comparing `smb3-video-autosplitter-0.1.0/smb3_video_autosplitter/livesplit.py` & `smb3-video-autosplitter-0.2.0/smb3_video_autosplitter/livesplit.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,7 +37,10 @@
         except:
             raise LivesplitConnectFailedException()
         res = win32pipe.SetNamedPipeHandleState(
             self.handle, win32pipe.PIPE_READMODE_BYTE, None, None
         )
         if res == 0:
             print(f"SetNamedPipeHandleState return code: {res}")
+
+    def terminate(self):
+        self.handle.close()
```

### Comparing `smb3-video-autosplitter-0.1.0/smb3_video_autosplitter/logging.py` & `smb3-video-autosplitter-0.2.0/smb3_video_autosplitter/logging.py`

 * *Files identical despite different names*

### Comparing `smb3-video-autosplitter-0.1.0/smb3_video_autosplitter/main.py` & `smb3-video-autosplitter-0.2.0/smb3_video_autosplitter/main.py`

 * *Files identical despite different names*

### Comparing `smb3-video-autosplitter-0.1.0/smb3_video_autosplitter/opencv.py` & `smb3-video-autosplitter-0.2.0/smb3_video_autosplitter/opencv.py`

 * *Files identical despite different names*

### Comparing `smb3-video-autosplitter-0.1.0/smb3_video_autosplitter/settings.py` & `smb3-video-autosplitter-0.2.0/smb3_video_autosplitter/settings.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from dataclasses import dataclass
-from functools import lru_cache
 from typing import Optional
 
 from dataclass_wizard import YAMLWizard
 
 
 NES_FRAMERATE = 1008307711 / 256 / 65536
 NES_MS_PER_FRAME = 1000.0 / NES_FRAMERATE
@@ -12,14 +11,15 @@
 @dataclass
 class Split:
     path: str
     x: int
     y: int
     width: int
     height: int
+    command_name: str
 
 
 @dataclass
 class Settings(YAMLWizard):
     splits: list[Split]
     video_capture_source: int
     split_dedupe_wait_s: Optional[float] = 5.0
```

### Comparing `smb3-video-autosplitter-0.1.0/smb3_video_autosplitter/util.py` & `smb3-video-autosplitter-0.2.0/smb3_video_autosplitter/util.py`

 * *Files identical despite different names*

### Comparing `smb3-video-autosplitter-0.1.0/smb3_video_autosplitter.egg-info/PKG-INFO` & `smb3-video-autosplitter-0.2.0/smb3_video_autosplitter.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smb3-video-autosplitter
-Version: 0.1.0
+Version: 0.2.0
 Summary: Ingest video data to render smb3 eh manip stimuli
 Author: narfman0
 Author-email: narfman0@blastedstudios.com
 License: LICENSE
 Keywords: smb3-video-autosplitter
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `smb3-video-autosplitter-0.1.0/smb3_video_autosplitter.egg-info/SOURCES.txt` & `smb3-video-autosplitter-0.2.0/smb3_video_autosplitter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

