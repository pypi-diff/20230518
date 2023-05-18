# Comparing `tmp/smb3-video-autosplitter-0.0.2.tar.gz` & `tmp/smb3-video-autosplitter-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smb3-video-autosplitter-0.0.2.tar", last modified: Wed May 17 21:06:40 2023, max compression
+gzip compressed data, was "smb3-video-autosplitter-0.0.3.tar", last modified: Thu May 18 01:38:16 2023, max compression
```

## Comparing `smb3-video-autosplitter-0.0.2.tar` & `smb3-video-autosplitter-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 21:06:40.990909 smb3-video-autosplitter-0.0.2/
--rw-rw-rw-   0        0        0    35797 2021-01-02 05:14:00.000000 smb3-video-autosplitter-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       67 2021-01-02 05:14:00.000000 smb3-video-autosplitter-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      558 2023-05-17 21:06:40.989908 smb3-video-autosplitter-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1414 2023-05-17 21:05:02.000000 smb3-video-autosplitter-0.0.2/README.rst
--rw-rw-rw-   0        0        0       91 2022-12-07 15:46:05.000000 smb3-video-autosplitter-0.0.2/requirements_test.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 21:06:40.990909 smb3-video-autosplitter-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      867 2023-05-16 20:30:23.000000 smb3-video-autosplitter-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-17 21:06:40.982901 smb3-video-autosplitter-0.0.2/smb3_video_autosplitter/
--rw-rw-rw-   0        0        0        0 2021-01-02 05:14:00.000000 smb3-video-autosplitter-0.0.2/smb3_video_autosplitter/__init__.py
--rw-rw-rw-   0        0        0     2406 2023-05-16 20:42:16.000000 smb3-video-autosplitter-0.0.2/smb3_video_autosplitter/autosplitter.py
--rw-rw-rw-   0        0        0      887 2023-05-16 20:23:41.000000 smb3-video-autosplitter-0.0.2/smb3_video_autosplitter/logging.py
--rw-rw-rw-   0        0        0     1400 2023-05-16 20:31:13.000000 smb3-video-autosplitter-0.0.2/smb3_video_autosplitter/main.py
--rw-rw-rw-   0        0        0      750 2023-05-16 20:31:02.000000 smb3-video-autosplitter-0.0.2/smb3_video_autosplitter/opencv.py
--rw-rw-rw-   0        0        0      312 2023-05-16 20:31:32.000000 smb3-video-autosplitter-0.0.2/smb3_video_autosplitter/settings.py
--rw-rw-rw-   0        0        0     1635 2023-05-16 20:24:03.000000 smb3-video-autosplitter-0.0.2/smb3_video_autosplitter/util.py
-drwxrwxrwx   0        0        0        0 2023-05-17 21:06:40.989908 smb3-video-autosplitter-0.0.2/smb3_video_autosplitter.egg-info/
--rw-rw-rw-   0        0        0      558 2023-05-17 21:06:40.000000 smb3-video-autosplitter-0.0.2/smb3_video_autosplitter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      582 2023-05-17 21:06:40.000000 smb3-video-autosplitter-0.0.2/smb3_video_autosplitter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 21:06:40.000000 smb3-video-autosplitter-0.0.2/smb3_video_autosplitter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-05-17 21:06:40.000000 smb3-video-autosplitter-0.0.2/smb3_video_autosplitter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2023-05-17 21:06:40.000000 smb3-video-autosplitter-0.0.2/smb3_video_autosplitter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-17 21:06:34.000000 smb3-video-autosplitter-0.0.2/smb3_video_autosplitter.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-05-18 01:38:16.452275 smb3-video-autosplitter-0.0.3/
+-rw-rw-rw-   0        0        0    35797 2021-01-02 05:14:00.000000 smb3-video-autosplitter-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       67 2021-01-02 05:14:00.000000 smb3-video-autosplitter-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      555 2023-05-18 01:38:16.451274 smb3-video-autosplitter-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1414 2023-05-17 21:05:02.000000 smb3-video-autosplitter-0.0.3/README.rst
+-rw-rw-rw-   0        0        0       91 2022-12-07 15:46:05.000000 smb3-video-autosplitter-0.0.3/requirements_test.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 01:38:16.452275 smb3-video-autosplitter-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      893 2023-05-18 01:37:59.000000 smb3-video-autosplitter-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 01:38:16.444268 smb3-video-autosplitter-0.0.3/smb3_video_autosplitter/
+-rw-rw-rw-   0        0        0        0 2021-01-02 05:14:00.000000 smb3-video-autosplitter-0.0.3/smb3_video_autosplitter/__init__.py
+-rw-rw-rw-   0        0        0     1703 2023-05-18 01:37:11.000000 smb3-video-autosplitter-0.0.3/smb3_video_autosplitter/autosplitter.py
+-rw-rw-rw-   0        0        0     1333 2023-05-18 01:05:58.000000 smb3-video-autosplitter-0.0.3/smb3_video_autosplitter/livesplit.py
+-rw-rw-rw-   0        0        0      861 2023-05-18 01:20:54.000000 smb3-video-autosplitter-0.0.3/smb3_video_autosplitter/logging.py
+-rw-rw-rw-   0        0        0     1440 2023-05-18 01:37:11.000000 smb3-video-autosplitter-0.0.3/smb3_video_autosplitter/main.py
+-rw-rw-rw-   0        0        0      740 2023-05-18 01:26:12.000000 smb3-video-autosplitter-0.0.3/smb3_video_autosplitter/opencv.py
+-rw-rw-rw-   0        0        0      800 2023-05-18 01:25:53.000000 smb3-video-autosplitter-0.0.3/smb3_video_autosplitter/settings.py
+-rw-rw-rw-   0        0        0     1624 2023-05-18 01:19:24.000000 smb3-video-autosplitter-0.0.3/smb3_video_autosplitter/util.py
+drwxrwxrwx   0        0        0        0 2023-05-18 01:38:16.451274 smb3-video-autosplitter-0.0.3/smb3_video_autosplitter.egg-info/
+-rw-rw-rw-   0        0        0      555 2023-05-18 01:38:16.000000 smb3-video-autosplitter-0.0.3/smb3_video_autosplitter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      619 2023-05-18 01:38:16.000000 smb3-video-autosplitter-0.0.3/smb3_video_autosplitter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 01:38:16.000000 smb3-video-autosplitter-0.0.3/smb3_video_autosplitter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-18 01:38:16.000000 smb3-video-autosplitter-0.0.3/smb3_video_autosplitter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2023-05-18 01:38:16.000000 smb3-video-autosplitter-0.0.3/smb3_video_autosplitter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-18 01:38:09.000000 smb3-video-autosplitter-0.0.3/smb3_video_autosplitter.egg-info/zip-safe
```

### Comparing `smb3-video-autosplitter-0.0.2/LICENSE` & `smb3-video-autosplitter-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `smb3-video-autosplitter-0.0.2/PKG-INFO` & `smb3-video-autosplitter-0.0.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: smb3-video-autosplitter
-Version: 0.0.2
+Version: 0.0.3
 Summary: Ingest video data to render smb3 eh manip stimuli
-Author: Jon Robison
+Author: narfman0
 Author-email: narfman0@blastedstudios.com
 License: LICENSE
 Keywords: smb3-video-autosplitter
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `smb3-video-autosplitter-0.0.2/README.rst` & `smb3-video-autosplitter-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `smb3-video-autosplitter-0.0.2/setup.py` & `smb3-video-autosplitter-0.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from setuptools import setup, find_packages
 
 setup(
     name="smb3-video-autosplitter",
-    version="0.0.2",
+    version="0.0.3",
     description=("Ingest video data to render smb3 eh manip stimuli"),
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     keywords="smb3-video-autosplitter",
-    author="Jon Robison",
+    author="narfman0",
     author_email="narfman0@blastedstudios.com",
     license="LICENSE",
     packages=find_packages(),
     include_package_data=True,
     zip_safe=True,
     install_requires=[
+        "dataclass_wizard",
         "opencv-python",
         "pygrabber",
         "pywin32",
         "pyyaml",
     ],
     test_suite="tests",
 )
```

### Comparing `smb3-video-autosplitter-0.0.2/smb3_video_autosplitter/autosplitter.py` & `smb3-video-autosplitter-0.0.3/smb3_video_autosplitter/autosplitter.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,73 +2,51 @@
 video based autosplitter for smb3
 """
 from dataclasses import dataclass
 import logging
 import time
 
 import cv2
-import win32file, win32pipe
 
-from smb3_video_autosplitter.util import locate_all_opencv, settings
+from smb3_video_autosplitter.livesplit import Livesplit
+from smb3_video_autosplitter.settings import Settings
+from smb3_video_autosplitter.util import locate_all_opencv
 
 LOGGER = logging.getLogger(__name__)
-SPLIT_DEDUPE_WAIT_S = settings.get("split_dedupe_wait_s", 5.0)
-SPLIT_OFFSET_FRAMES = settings.get("split_offset_frames", 40)
-SPLIT_OFFSET_S = (SPLIT_OFFSET_FRAMES * 16.64) / 1000
-
-
-class LivesplitConnectFailedException(Exception):
-    pass
 
 
 @dataclass
 class Split:
     path: str
     image: any
     region: list[int, int, int, int]
 
 
 class Autosplitter:
-    def __init__(self):
+    def __init__(self, settings: Settings):
+        self.settings = settings
         self.initialize_splits()
-        self.initialize_livesplit()
         self.earliest_next_trigger_time = 0
+        self.livesplit = Livesplit()
+        self.split_offset_s = (settings.split_offset_frames * 16.64) / 1000
 
     def tick(self, frame):
         if frame is None or self.earliest_next_trigger_time >= time.time():
             return
         for split in self.splits:
             results = list(locate_all_opencv(split.image, frame, region=split.region))
             if results:
-                time.sleep(SPLIT_OFFSET_S)
-                self.earliest_next_trigger_time = time.time() + SPLIT_DEDUPE_WAIT_S
+                time.sleep(self.split_offset_s)
+                self.earliest_next_trigger_time = (
+                    time.time() + self.settings.split_dedupe_wait_s
+                )
                 LOGGER.info(
                     f"Splitting after {split.path} observed {len(results)} times at {list(map(str, results))}"
                 )
-                win32file.WriteFile(self.handle, b"split\r\n")
-
-    def initialize_livesplit(self):
-        try:
-            self.handle = win32file.CreateFile(
-                r"\\.\pipe\LiveSplit",
-                win32file.GENERIC_READ | win32file.GENERIC_WRITE,
-                0,
-                None,
-                win32file.OPEN_EXISTING,
-                win32file.FILE_ATTRIBUTE_NORMAL,
-                None,
-            )
-        except:
-            raise LivesplitConnectFailedException()
-        res = win32pipe.SetNamedPipeHandleState(
-            self.handle, win32pipe.PIPE_READMODE_BYTE, None, None
-        )
-        if res == 0:
-            print(f"SetNamedPipeHandleState return code: {res}")
+                self.livesplit.send("split")
 
     def initialize_splits(self):
         self.splits: list[Split] = []
-        for split in settings.get("splits"):
-            path = split["path"]
-            image = cv2.imread(path)
-            region = [split["x"], split["y"], split["width"], split["height"]]
-            self.splits.append(Split(path, image, region))
+        for split in self.settings.splits:
+            image = cv2.imread(split.path)
+            region = [split.x, split.y, split.width, split.height]
+            self.splits.append(Split(split.path, image, region))
```

### Comparing `smb3-video-autosplitter-0.0.2/smb3_video_autosplitter/logging.py` & `smb3-video-autosplitter-0.0.3/smb3_video_autosplitter/logging.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
 
-from smb3_video_autosplitter.util import settings
+from smb3_video_autosplitter.settings import settings
 
 FILE_FORMAT = "[%(asctime)s] {%(pathname)s:%(lineno)d} %(levelname)s - %(message)s"
 
 
 def initialize_logging(
-    file_log_level=settings.get("file_log_level", "INFO"),
-    console_log_level=settings.get("console_log_level", "INFO"),
+    file_log_level=settings.file_log_level,
+    console_log_level=settings.console_log_level,
     filename="smb3_video_autosplitter.log",
 ):
     # set up logging to file
     logging.basicConfig(
         filename=filename, level=file_log_level, format=FILE_FORMAT, datefmt="%H:%M:%S"
     )
```

### Comparing `smb3-video-autosplitter-0.0.2/smb3_video_autosplitter/main.py` & `smb3-video-autosplitter-0.0.3/smb3_video_autosplitter/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 """
 video based autosplitter for smb3
 """
 import logging
 
 from pygrabber.dshow_graph import FilterGraph
 
-from smb3_video_autosplitter import settings
-from smb3_video_autosplitter.autosplitter import (
-    Autosplitter,
-    LivesplitConnectFailedException,
-)
+from smb3_video_autosplitter.settings import settings
+from smb3_video_autosplitter.autosplitter import Autosplitter
+from smb3_video_autosplitter.livesplit import LivesplitConnectFailedException
 from smb3_video_autosplitter.opencv import OpenCV
 
 from smb3_video_autosplitter.logging import initialize_logging
 
 LOGGER = logging.getLogger(__name__)
 
 
 def print_camera_info():
     graph = FilterGraph()
     input_devices = graph.get_input_devices()
-    video_capture_source = settings.get("video_capture_source")
+    video_capture_source = settings.video_capture_source
     if (
         video_capture_source == None
         or video_capture_source == -1
         or video_capture_source >= len(input_devices)
     ):
         LOGGER.warning(
             "No camera selected or invalid, please update to one of the below:"
@@ -35,15 +33,15 @@
 
 
 def main():
     initialize_logging()
     print_camera_info()
     opencv = OpenCV()
     try:
-        autosplitter = Autosplitter()
+        autosplitter = Autosplitter(settings)
     except LivesplitConnectFailedException:
         LOGGER.warning("Failed to connect to livesplit, is it running?")
         exit()
     while True:
         opencv.tick()
         autosplitter.tick(opencv.frame)
```

### Comparing `smb3-video-autosplitter-0.0.2/smb3_video_autosplitter/opencv.py` & `smb3-video-autosplitter-0.0.3/smb3_video_autosplitter/opencv.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from pygrabber.dshow_graph import FilterGraph
 import cv2
-from smb3_video_autosplitter.util import settings
+from smb3_video_autosplitter.settings import settings
 
 
 class OpenCV:
     def __init__(self):
         self.graph = FilterGraph()
-        self.graph.add_video_input_device(settings.get("video_capture_source"))
+        self.graph.add_video_input_device(settings.video_capture_source)
         self.graph.add_sample_grabber(self.on_frame_received)
         self.graph.add_null_render()
         self.graph.prepare_preview_graph()
         self.graph.run()
         self.frame = None
 
     def tick(self):
         self.graph.grab_frame()
-        if settings.get("show_capture_video") and self.frame is not None:
+        if settings.show_capture_video and self.frame is not None:
             cv2.imshow("capture", self.frame)
             _ = cv2.waitKey(1)
 
     def on_frame_received(self, frame):
         self.frame = frame
```

### Comparing `smb3-video-autosplitter-0.0.2/smb3_video_autosplitter/util.py` & `smb3-video-autosplitter-0.0.3/smb3_video_autosplitter/util.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import cv2
 import numpy as np
 
-from smb3_video_autosplitter import settings
+from smb3_video_autosplitter.settings import settings
 
 
 def locate_all_opencv(
     needleImage,
     haystackImage,
     limit=10000,
     region=None,  # [x, y, width, height]
-    confidence=float(settings.get("confidence", 0.95)),
+    confidence=settings.confidence,
 ):
     """
     RGBA images are treated as RBG (ignores alpha channel)
     """
 
     confidence = float(confidence)
```

### Comparing `smb3-video-autosplitter-0.0.2/smb3_video_autosplitter.egg-info/PKG-INFO` & `smb3-video-autosplitter-0.0.3/smb3_video_autosplitter.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: smb3-video-autosplitter
-Version: 0.0.2
+Version: 0.0.3
 Summary: Ingest video data to render smb3 eh manip stimuli
-Author: Jon Robison
+Author: narfman0
 Author-email: narfman0@blastedstudios.com
 License: LICENSE
 Keywords: smb3-video-autosplitter
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `smb3-video-autosplitter-0.0.2/smb3_video_autosplitter.egg-info/SOURCES.txt` & `smb3-video-autosplitter-0.0.3/smb3_video_autosplitter.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 MANIFEST.in
 README.rst
 requirements_test.txt
 setup.py
 smb3_video_autosplitter/__init__.py
 smb3_video_autosplitter/autosplitter.py
+smb3_video_autosplitter/livesplit.py
 smb3_video_autosplitter/logging.py
 smb3_video_autosplitter/main.py
 smb3_video_autosplitter/opencv.py
 smb3_video_autosplitter/settings.py
 smb3_video_autosplitter/util.py
 smb3_video_autosplitter.egg-info/PKG-INFO
 smb3_video_autosplitter.egg-info/SOURCES.txt
```

