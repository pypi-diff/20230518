# Comparing `tmp/smb3-video-autosplitter-0.0.5.tar.gz` & `tmp/smb3-video-autosplitter-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smb3-video-autosplitter-0.0.5.tar", last modified: Thu May 18 02:07:11 2023, max compression
+gzip compressed data, was "smb3-video-autosplitter-0.1.0.tar", last modified: Thu May 18 02:23:05 2023, max compression
```

## Comparing `smb3-video-autosplitter-0.0.5.tar` & `smb3-video-autosplitter-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 02:07:11.565168 smb3-video-autosplitter-0.0.5/
--rw-rw-rw-   0        0        0    35797 2021-01-02 05:14:00.000000 smb3-video-autosplitter-0.0.5/LICENSE
--rw-rw-rw-   0        0        0       67 2021-01-02 05:14:00.000000 smb3-video-autosplitter-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      555 2023-05-18 02:07:11.565168 smb3-video-autosplitter-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1414 2023-05-17 21:05:02.000000 smb3-video-autosplitter-0.0.5/README.rst
--rw-rw-rw-   0        0        0       91 2022-12-07 15:46:05.000000 smb3-video-autosplitter-0.0.5/requirements_test.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 02:07:11.566169 smb3-video-autosplitter-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      893 2023-05-18 02:06:59.000000 smb3-video-autosplitter-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-18 02:07:11.558163 smb3-video-autosplitter-0.0.5/smb3_video_autosplitter/
--rw-rw-rw-   0        0        0        0 2021-01-02 05:14:00.000000 smb3-video-autosplitter-0.0.5/smb3_video_autosplitter/__init__.py
--rw-rw-rw-   0        0        0     1751 2023-05-18 01:43:18.000000 smb3-video-autosplitter-0.0.5/smb3_video_autosplitter/autosplitter.py
--rw-rw-rw-   0        0        0     1333 2023-05-18 01:05:58.000000 smb3-video-autosplitter-0.0.5/smb3_video_autosplitter/livesplit.py
--rw-rw-rw-   0        0        0      857 2023-05-18 02:06:25.000000 smb3-video-autosplitter-0.0.5/smb3_video_autosplitter/logging.py
--rw-rw-rw-   0        0        0     1436 2023-05-18 02:06:20.000000 smb3-video-autosplitter-0.0.5/smb3_video_autosplitter/main.py
--rw-rw-rw-   0        0        0      736 2023-05-18 02:06:13.000000 smb3-video-autosplitter-0.0.5/smb3_video_autosplitter/opencv.py
--rw-rw-rw-   0        0        0      801 2023-05-18 02:04:57.000000 smb3-video-autosplitter-0.0.5/smb3_video_autosplitter/settings.py
--rw-rw-rw-   0        0        0     1654 2023-05-18 02:06:03.000000 smb3-video-autosplitter-0.0.5/smb3_video_autosplitter/util.py
-drwxrwxrwx   0        0        0        0 2023-05-18 02:07:11.564168 smb3-video-autosplitter-0.0.5/smb3_video_autosplitter.egg-info/
--rw-rw-rw-   0        0        0      555 2023-05-18 02:07:11.000000 smb3-video-autosplitter-0.0.5/smb3_video_autosplitter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      619 2023-05-18 02:07:11.000000 smb3-video-autosplitter-0.0.5/smb3_video_autosplitter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 02:07:11.000000 smb3-video-autosplitter-0.0.5/smb3_video_autosplitter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-18 02:07:11.000000 smb3-video-autosplitter-0.0.5/smb3_video_autosplitter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2023-05-18 02:07:11.000000 smb3-video-autosplitter-0.0.5/smb3_video_autosplitter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-18 02:07:05.000000 smb3-video-autosplitter-0.0.5/smb3_video_autosplitter.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-05-18 02:23:05.654145 smb3-video-autosplitter-0.1.0/
+-rw-rw-rw-   0        0        0    35797 2021-01-02 05:14:00.000000 smb3-video-autosplitter-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0       67 2021-01-02 05:14:00.000000 smb3-video-autosplitter-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      555 2023-05-18 02:23:05.654145 smb3-video-autosplitter-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1414 2023-05-17 21:05:02.000000 smb3-video-autosplitter-0.1.0/README.rst
+-rw-rw-rw-   0        0        0       91 2022-12-07 15:46:05.000000 smb3-video-autosplitter-0.1.0/requirements_test.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 02:23:05.654145 smb3-video-autosplitter-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      893 2023-05-18 02:22:51.000000 smb3-video-autosplitter-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 02:23:05.647138 smb3-video-autosplitter-0.1.0/smb3_video_autosplitter/
+-rw-rw-rw-   0        0        0        0 2021-01-02 05:14:00.000000 smb3-video-autosplitter-0.1.0/smb3_video_autosplitter/__init__.py
+-rw-rw-rw-   0        0        0     1924 2023-05-18 02:15:00.000000 smb3-video-autosplitter-0.1.0/smb3_video_autosplitter/autosplitter.py
+-rw-rw-rw-   0        0        0     1333 2023-05-18 01:05:58.000000 smb3-video-autosplitter-0.1.0/smb3_video_autosplitter/livesplit.py
+-rw-rw-rw-   0        0        0      767 2023-05-18 02:14:04.000000 smb3-video-autosplitter-0.1.0/smb3_video_autosplitter/logging.py
+-rw-rw-rw-   0        0        0     1636 2023-05-18 02:21:11.000000 smb3-video-autosplitter-0.1.0/smb3_video_autosplitter/main.py
+-rw-rw-rw-   0        0        0      774 2023-05-18 02:21:26.000000 smb3-video-autosplitter-0.1.0/smb3_video_autosplitter/opencv.py
+-rw-rw-rw-   0        0        0      801 2023-05-18 02:04:57.000000 smb3-video-autosplitter-0.1.0/smb3_video_autosplitter/settings.py
+-rw-rw-rw-   0        0        0     1552 2023-05-18 02:14:40.000000 smb3-video-autosplitter-0.1.0/smb3_video_autosplitter/util.py
+drwxrwxrwx   0        0        0        0 2023-05-18 02:23:05.653144 smb3-video-autosplitter-0.1.0/smb3_video_autosplitter.egg-info/
+-rw-rw-rw-   0        0        0      555 2023-05-18 02:23:05.000000 smb3-video-autosplitter-0.1.0/smb3_video_autosplitter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      619 2023-05-18 02:23:05.000000 smb3-video-autosplitter-0.1.0/smb3_video_autosplitter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 02:23:05.000000 smb3-video-autosplitter-0.1.0/smb3_video_autosplitter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-18 02:23:05.000000 smb3-video-autosplitter-0.1.0/smb3_video_autosplitter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2023-05-18 02:23:05.000000 smb3-video-autosplitter-0.1.0/smb3_video_autosplitter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-18 02:22:59.000000 smb3-video-autosplitter-0.1.0/smb3_video_autosplitter.egg-info/zip-safe
```

### Comparing `smb3-video-autosplitter-0.0.5/LICENSE` & `smb3-video-autosplitter-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smb3-video-autosplitter-0.0.5/PKG-INFO` & `smb3-video-autosplitter-0.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smb3-video-autosplitter
-Version: 0.0.5
+Version: 0.1.0
 Summary: Ingest video data to render smb3 eh manip stimuli
 Author: narfman0
 Author-email: narfman0@blastedstudios.com
 License: LICENSE
 Keywords: smb3-video-autosplitter
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `smb3-video-autosplitter-0.0.5/README.rst` & `smb3-video-autosplitter-0.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `smb3-video-autosplitter-0.0.5/setup.py` & `smb3-video-autosplitter-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="smb3-video-autosplitter",
-    version="0.0.5",
+    version="0.1.0",
     description=("Ingest video data to render smb3 eh manip stimuli"),
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `smb3-video-autosplitter-0.0.5/smb3_video_autosplitter/autosplitter.py` & `smb3-video-autosplitter-0.1.0/smb3_video_autosplitter/autosplitter.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,22 @@
         self.livesplit = Livesplit()
         self.split_offset_s = (settings.split_offset_frames * 16.64) / 1000
 
     def tick(self, frame):
         if frame is None or self.earliest_next_trigger_time >= time.time():
             return
         for split in self.splits:
-            results = list(locate_all_opencv(split.image, frame, region=split.region))
+            results = list(
+                locate_all_opencv(
+                    split.image,
+                    frame,
+                    region=split.region,
+                    confidence=self.settings.confidence,
+                )
+            )
             if results:
                 time.sleep(self.split_offset_s)
                 self.earliest_next_trigger_time = (
                     time.time() + self.settings.split_dedupe_wait_s
                 )
                 LOGGER.info(
                     f"Splitting after {split.path} observed {len(results)} times at {list(map(str, results))}"
```

### Comparing `smb3-video-autosplitter-0.0.5/smb3_video_autosplitter/livesplit.py` & `smb3-video-autosplitter-0.1.0/smb3_video_autosplitter/livesplit.py`

 * *Files identical despite different names*

### Comparing `smb3-video-autosplitter-0.0.5/smb3_video_autosplitter/logging.py` & `smb3-video-autosplitter-0.1.0/smb3_video_autosplitter/logging.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import logging
 
-from smb3_video_autosplitter.util import settings
-
 FILE_FORMAT = "[%(asctime)s] {%(pathname)s:%(lineno)d} %(levelname)s - %(message)s"
 
 
 def initialize_logging(
-    file_log_level=settings.file_log_level,
-    console_log_level=settings.console_log_level,
+    file_log_level="INFO",
+    console_log_level="INFO",
     filename="smb3_video_autosplitter.log",
 ):
     # set up logging to file
     logging.basicConfig(
         filename=filename, level=file_log_level, format=FILE_FORMAT, datefmt="%H:%M:%S"
     )
```

### Comparing `smb3-video-autosplitter-0.0.5/smb3_video_autosplitter/main.py` & `smb3-video-autosplitter-0.1.0/smb3_video_autosplitter/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,44 +4,48 @@
 import logging
 
 from pygrabber.dshow_graph import FilterGraph
 
 from smb3_video_autosplitter.autosplitter import Autosplitter
 from smb3_video_autosplitter.livesplit import LivesplitConnectFailedException
 from smb3_video_autosplitter.opencv import OpenCV
-from smb3_video_autosplitter.util import settings
+from smb3_video_autosplitter.settings import Settings
 
 from smb3_video_autosplitter.logging import initialize_logging
 
 LOGGER = logging.getLogger(__name__)
+SETTINGS = Settings.load()
 
 
 def print_camera_info():
     graph = FilterGraph()
     input_devices = graph.get_input_devices()
-    video_capture_source = settings.video_capture_source
+    video_capture_source = SETTINGS.video_capture_source
     if (
         video_capture_source == None
         or video_capture_source == -1
         or video_capture_source >= len(input_devices)
     ):
         LOGGER.warning(
             "No camera selected or invalid, please update to one of the below:"
         )
         LOGGER.warning(input_devices)
         exit()
     LOGGER.info(f"Selected video source: {input_devices[video_capture_source]}")
 
 
 def main():
-    initialize_logging()
+    initialize_logging(
+        file_log_level=SETTINGS.file_log_level,
+        console_log_level=SETTINGS.console_log_level,
+    )
     print_camera_info()
-    opencv = OpenCV()
+    opencv = OpenCV(SETTINGS.video_capture_source, SETTINGS.show_capture_video)
     try:
-        autosplitter = Autosplitter(settings)
+        autosplitter = Autosplitter(SETTINGS)
     except LivesplitConnectFailedException:
         LOGGER.warning("Failed to connect to livesplit, is it running?")
         exit()
     while True:
         opencv.tick()
         autosplitter.tick(opencv.frame)
```

### Comparing `smb3-video-autosplitter-0.0.5/smb3_video_autosplitter/settings.py` & `smb3-video-autosplitter-0.1.0/smb3_video_autosplitter/settings.py`

 * *Files identical despite different names*

### Comparing `smb3-video-autosplitter-0.0.5/smb3_video_autosplitter/util.py` & `smb3-video-autosplitter-0.1.0/smb3_video_autosplitter/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 import cv2
 import numpy as np
 
-from smb3_video_autosplitter.settings import Settings
-
-settings = Settings.load()
-
 
 def locate_all_opencv(
     needleImage,
     haystackImage,
     limit=10000,
     region=None,  # [x, y, width, height]
-    confidence=settings.confidence,
+    confidence=0.95,
 ):
     """
     RGBA images are treated as RBG (ignores alpha channel)
     """
 
     confidence = float(confidence)
```

### Comparing `smb3-video-autosplitter-0.0.5/smb3_video_autosplitter.egg-info/PKG-INFO` & `smb3-video-autosplitter-0.1.0/smb3_video_autosplitter.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smb3-video-autosplitter
-Version: 0.0.5
+Version: 0.1.0
 Summary: Ingest video data to render smb3 eh manip stimuli
 Author: narfman0
 Author-email: narfman0@blastedstudios.com
 License: LICENSE
 Keywords: smb3-video-autosplitter
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `smb3-video-autosplitter-0.0.5/smb3_video_autosplitter.egg-info/SOURCES.txt` & `smb3-video-autosplitter-0.1.0/smb3_video_autosplitter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

