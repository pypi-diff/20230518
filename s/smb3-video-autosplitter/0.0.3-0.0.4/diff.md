# Comparing `tmp/smb3-video-autosplitter-0.0.3.tar.gz` & `tmp/smb3-video-autosplitter-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smb3-video-autosplitter-0.0.3.tar", last modified: Thu May 18 01:38:16 2023, max compression
+gzip compressed data, was "smb3-video-autosplitter-0.0.4.tar", last modified: Thu May 18 01:45:27 2023, max compression
```

## Comparing `smb3-video-autosplitter-0.0.3.tar` & `smb3-video-autosplitter-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 01:38:16.452275 smb3-video-autosplitter-0.0.3/
--rw-rw-rw-   0        0        0    35797 2021-01-02 05:14:00.000000 smb3-video-autosplitter-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       67 2021-01-02 05:14:00.000000 smb3-video-autosplitter-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      555 2023-05-18 01:38:16.451274 smb3-video-autosplitter-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1414 2023-05-17 21:05:02.000000 smb3-video-autosplitter-0.0.3/README.rst
--rw-rw-rw-   0        0        0       91 2022-12-07 15:46:05.000000 smb3-video-autosplitter-0.0.3/requirements_test.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 01:38:16.452275 smb3-video-autosplitter-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      893 2023-05-18 01:37:59.000000 smb3-video-autosplitter-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-18 01:38:16.444268 smb3-video-autosplitter-0.0.3/smb3_video_autosplitter/
--rw-rw-rw-   0        0        0        0 2021-01-02 05:14:00.000000 smb3-video-autosplitter-0.0.3/smb3_video_autosplitter/__init__.py
--rw-rw-rw-   0        0        0     1703 2023-05-18 01:37:11.000000 smb3-video-autosplitter-0.0.3/smb3_video_autosplitter/autosplitter.py
--rw-rw-rw-   0        0        0     1333 2023-05-18 01:05:58.000000 smb3-video-autosplitter-0.0.3/smb3_video_autosplitter/livesplit.py
--rw-rw-rw-   0        0        0      861 2023-05-18 01:20:54.000000 smb3-video-autosplitter-0.0.3/smb3_video_autosplitter/logging.py
--rw-rw-rw-   0        0        0     1440 2023-05-18 01:37:11.000000 smb3-video-autosplitter-0.0.3/smb3_video_autosplitter/main.py
--rw-rw-rw-   0        0        0      740 2023-05-18 01:26:12.000000 smb3-video-autosplitter-0.0.3/smb3_video_autosplitter/opencv.py
--rw-rw-rw-   0        0        0      800 2023-05-18 01:25:53.000000 smb3-video-autosplitter-0.0.3/smb3_video_autosplitter/settings.py
--rw-rw-rw-   0        0        0     1624 2023-05-18 01:19:24.000000 smb3-video-autosplitter-0.0.3/smb3_video_autosplitter/util.py
-drwxrwxrwx   0        0        0        0 2023-05-18 01:38:16.451274 smb3-video-autosplitter-0.0.3/smb3_video_autosplitter.egg-info/
--rw-rw-rw-   0        0        0      555 2023-05-18 01:38:16.000000 smb3-video-autosplitter-0.0.3/smb3_video_autosplitter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      619 2023-05-18 01:38:16.000000 smb3-video-autosplitter-0.0.3/smb3_video_autosplitter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 01:38:16.000000 smb3-video-autosplitter-0.0.3/smb3_video_autosplitter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-18 01:38:16.000000 smb3-video-autosplitter-0.0.3/smb3_video_autosplitter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2023-05-18 01:38:16.000000 smb3-video-autosplitter-0.0.3/smb3_video_autosplitter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-18 01:38:09.000000 smb3-video-autosplitter-0.0.3/smb3_video_autosplitter.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-05-18 01:45:27.804883 smb3-video-autosplitter-0.0.4/
+-rw-rw-rw-   0        0        0    35797 2021-01-02 05:14:00.000000 smb3-video-autosplitter-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       67 2021-01-02 05:14:00.000000 smb3-video-autosplitter-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      555 2023-05-18 01:45:27.803882 smb3-video-autosplitter-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1414 2023-05-17 21:05:02.000000 smb3-video-autosplitter-0.0.4/README.rst
+-rw-rw-rw-   0        0        0       91 2022-12-07 15:46:05.000000 smb3-video-autosplitter-0.0.4/requirements_test.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 01:45:27.804883 smb3-video-autosplitter-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      893 2023-05-18 01:45:11.000000 smb3-video-autosplitter-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 01:45:27.797875 smb3-video-autosplitter-0.0.4/smb3_video_autosplitter/
+-rw-rw-rw-   0        0        0        0 2021-01-02 05:14:00.000000 smb3-video-autosplitter-0.0.4/smb3_video_autosplitter/__init__.py
+-rw-rw-rw-   0        0        0     1751 2023-05-18 01:43:18.000000 smb3-video-autosplitter-0.0.4/smb3_video_autosplitter/autosplitter.py
+-rw-rw-rw-   0        0        0     1333 2023-05-18 01:05:58.000000 smb3-video-autosplitter-0.0.4/smb3_video_autosplitter/livesplit.py
+-rw-rw-rw-   0        0        0      861 2023-05-18 01:20:54.000000 smb3-video-autosplitter-0.0.4/smb3_video_autosplitter/logging.py
+-rw-rw-rw-   0        0        0     1440 2023-05-18 01:37:11.000000 smb3-video-autosplitter-0.0.4/smb3_video_autosplitter/main.py
+-rw-rw-rw-   0        0        0      740 2023-05-18 01:26:12.000000 smb3-video-autosplitter-0.0.4/smb3_video_autosplitter/opencv.py
+-rw-rw-rw-   0        0        0      800 2023-05-18 01:25:53.000000 smb3-video-autosplitter-0.0.4/smb3_video_autosplitter/settings.py
+-rw-rw-rw-   0        0        0     1624 2023-05-18 01:19:24.000000 smb3-video-autosplitter-0.0.4/smb3_video_autosplitter/util.py
+drwxrwxrwx   0        0        0        0 2023-05-18 01:45:27.803882 smb3-video-autosplitter-0.0.4/smb3_video_autosplitter.egg-info/
+-rw-rw-rw-   0        0        0      555 2023-05-18 01:45:27.000000 smb3-video-autosplitter-0.0.4/smb3_video_autosplitter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      619 2023-05-18 01:45:27.000000 smb3-video-autosplitter-0.0.4/smb3_video_autosplitter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 01:45:27.000000 smb3-video-autosplitter-0.0.4/smb3_video_autosplitter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-18 01:45:27.000000 smb3-video-autosplitter-0.0.4/smb3_video_autosplitter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2023-05-18 01:45:27.000000 smb3-video-autosplitter-0.0.4/smb3_video_autosplitter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-18 01:45:22.000000 smb3-video-autosplitter-0.0.4/smb3_video_autosplitter.egg-info/zip-safe
```

### Comparing `smb3-video-autosplitter-0.0.3/LICENSE` & `smb3-video-autosplitter-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `smb3-video-autosplitter-0.0.3/PKG-INFO` & `smb3-video-autosplitter-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smb3-video-autosplitter
-Version: 0.0.3
+Version: 0.0.4
 Summary: Ingest video data to render smb3 eh manip stimuli
 Author: narfman0
 Author-email: narfman0@blastedstudios.com
 License: LICENSE
 Keywords: smb3-video-autosplitter
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `smb3-video-autosplitter-0.0.3/README.rst` & `smb3-video-autosplitter-0.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `smb3-video-autosplitter-0.0.3/setup.py` & `smb3-video-autosplitter-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="smb3-video-autosplitter",
-    version="0.0.3",
+    version="0.0.4",
     description=("Ingest video data to render smb3 eh manip stimuli"),
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `smb3-video-autosplitter-0.0.3/smb3_video_autosplitter/autosplitter.py` & `smb3-video-autosplitter-0.0.4/smb3_video_autosplitter/autosplitter.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import cv2
 
 from smb3_video_autosplitter.livesplit import Livesplit
 from smb3_video_autosplitter.settings import Settings
 from smb3_video_autosplitter.util import locate_all_opencv
 
 LOGGER = logging.getLogger(__name__)
+SPLIT_COMMAND_NAME = "startorsplit"
 
 
 @dataclass
 class Split:
     path: str
     image: any
     region: list[int, int, int, int]
@@ -38,15 +39,15 @@
                 time.sleep(self.split_offset_s)
                 self.earliest_next_trigger_time = (
                     time.time() + self.settings.split_dedupe_wait_s
                 )
                 LOGGER.info(
                     f"Splitting after {split.path} observed {len(results)} times at {list(map(str, results))}"
                 )
-                self.livesplit.send("split")
+                self.livesplit.send(SPLIT_COMMAND_NAME)
 
     def initialize_splits(self):
         self.splits: list[Split] = []
         for split in self.settings.splits:
             image = cv2.imread(split.path)
             region = [split.x, split.y, split.width, split.height]
             self.splits.append(Split(split.path, image, region))
```

### Comparing `smb3-video-autosplitter-0.0.3/smb3_video_autosplitter/livesplit.py` & `smb3-video-autosplitter-0.0.4/smb3_video_autosplitter/livesplit.py`

 * *Files identical despite different names*

### Comparing `smb3-video-autosplitter-0.0.3/smb3_video_autosplitter/logging.py` & `smb3-video-autosplitter-0.0.4/smb3_video_autosplitter/logging.py`

 * *Files identical despite different names*

### Comparing `smb3-video-autosplitter-0.0.3/smb3_video_autosplitter/main.py` & `smb3-video-autosplitter-0.0.4/smb3_video_autosplitter/main.py`

 * *Files identical despite different names*

### Comparing `smb3-video-autosplitter-0.0.3/smb3_video_autosplitter/opencv.py` & `smb3-video-autosplitter-0.0.4/smb3_video_autosplitter/opencv.py`

 * *Files identical despite different names*

### Comparing `smb3-video-autosplitter-0.0.3/smb3_video_autosplitter/settings.py` & `smb3-video-autosplitter-0.0.4/smb3_video_autosplitter/settings.py`

 * *Files identical despite different names*

### Comparing `smb3-video-autosplitter-0.0.3/smb3_video_autosplitter/util.py` & `smb3-video-autosplitter-0.0.4/smb3_video_autosplitter/util.py`

 * *Files identical despite different names*

### Comparing `smb3-video-autosplitter-0.0.3/smb3_video_autosplitter.egg-info/PKG-INFO` & `smb3-video-autosplitter-0.0.4/smb3_video_autosplitter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smb3-video-autosplitter
-Version: 0.0.3
+Version: 0.0.4
 Summary: Ingest video data to render smb3 eh manip stimuli
 Author: narfman0
 Author-email: narfman0@blastedstudios.com
 License: LICENSE
 Keywords: smb3-video-autosplitter
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `smb3-video-autosplitter-0.0.3/smb3_video_autosplitter.egg-info/SOURCES.txt` & `smb3-video-autosplitter-0.0.4/smb3_video_autosplitter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

