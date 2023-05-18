# Comparing `tmp/pyvosklivesubtitle-0.1.7.tar.gz` & `tmp/pyvosklivesubtitle-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyvosklivesubtitle-0.1.7.tar", last modified: Thu May 18 20:17:21 2023, max compression
+gzip compressed data, was "dist\pyvosklivesubtitle-0.1.8.tar", last modified: Thu May 18 21:12:25 2023, max compression
```

## Comparing `pyvosklivesubtitle-0.1.7.tar` & `pyvosklivesubtitle-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 20:17:21.835658 pyvosklivesubtitle-0.1.7/
--rw-rw-rw-   0        0        0     1088 2022-11-03 03:32:17.000000 pyvosklivesubtitle-0.1.7/LICENSE
--rw-rw-rw-   0        0        0       34 2022-06-05 08:17:08.000000 pyvosklivesubtitle-0.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1490 2023-05-18 20:17:21.836408 pyvosklivesubtitle-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     6636 2023-04-24 13:05:36.000000 pyvosklivesubtitle-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 20:17:21.787343 pyvosklivesubtitle-0.1.7/pyvosklivesubtitle/
--rw-rw-rw-   0        0        0   146375 2023-05-18 20:15:26.000000 pyvosklivesubtitle-0.1.7/pyvosklivesubtitle/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 20:17:21.833411 pyvosklivesubtitle-0.1.7/pyvosklivesubtitle.egg-info/
--rw-rw-rw-   0        0        0     1490 2023-05-18 20:17:21.000000 pyvosklivesubtitle-0.1.7/pyvosklivesubtitle.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2023-05-18 20:17:21.000000 pyvosklivesubtitle-0.1.7/pyvosklivesubtitle.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 20:17:21.000000 pyvosklivesubtitle-0.1.7/pyvosklivesubtitle.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-05-18 20:17:21.000000 pyvosklivesubtitle-0.1.7/pyvosklivesubtitle.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      152 2023-05-18 20:17:21.000000 pyvosklivesubtitle-0.1.7/pyvosklivesubtitle.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-18 20:17:21.000000 pyvosklivesubtitle-0.1.7/pyvosklivesubtitle.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-05-18 20:17:21.838656 pyvosklivesubtitle-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1721 2023-05-08 18:46:09.000000 pyvosklivesubtitle-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 21:12:25.667247 pyvosklivesubtitle-0.1.8/
+-rw-rw-rw-   0        0        0     1088 2022-11-03 03:32:17.000000 pyvosklivesubtitle-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0       34 2022-06-05 08:17:08.000000 pyvosklivesubtitle-0.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     1490 2023-05-18 21:12:25.667996 pyvosklivesubtitle-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     6636 2023-04-24 13:05:36.000000 pyvosklivesubtitle-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 21:12:25.600262 pyvosklivesubtitle-0.1.8/pyvosklivesubtitle/
+-rw-rw-rw-   0        0        0   146376 2023-05-18 21:10:21.000000 pyvosklivesubtitle-0.1.8/pyvosklivesubtitle/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 21:12:25.665748 pyvosklivesubtitle-0.1.8/pyvosklivesubtitle.egg-info/
+-rw-rw-rw-   0        0        0     1490 2023-05-18 21:12:25.000000 pyvosklivesubtitle-0.1.8/pyvosklivesubtitle.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-05-18 21:12:25.000000 pyvosklivesubtitle-0.1.8/pyvosklivesubtitle.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 21:12:25.000000 pyvosklivesubtitle-0.1.8/pyvosklivesubtitle.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-05-18 21:12:25.000000 pyvosklivesubtitle-0.1.8/pyvosklivesubtitle.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      139 2023-05-18 21:12:25.000000 pyvosklivesubtitle-0.1.8/pyvosklivesubtitle.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-18 21:12:25.000000 pyvosklivesubtitle-0.1.8/pyvosklivesubtitle.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-05-18 21:12:25.676991 pyvosklivesubtitle-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1743 2023-05-18 21:12:20.000000 pyvosklivesubtitle-0.1.8/setup.py
```

### Comparing `pyvosklivesubtitle-0.1.7/LICENSE` & `pyvosklivesubtitle-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvosklivesubtitle-0.1.7/PKG-INFO` & `pyvosklivesubtitle-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: pyvosklivesubtitle
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Python based desktop aplication that can RECOGNIZE any live streaming in 21 languages that supported by VOSK then TRANSLATE and display it as LIVE SUBTITLES
 Home-page: https://github.com/botbahlul/pyvosklivesubtitle
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
 
 Copyright (c) 2022 Bot Bahlul
```

### Comparing `pyvosklivesubtitle-0.1.7/README.md` & `pyvosklivesubtitle-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `pyvosklivesubtitle-0.1.7/pyvosklivesubtitle/__init__.py` & `pyvosklivesubtitle-0.1.8/pyvosklivesubtitle/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,15 +319,15 @@
 MODEL_DIRS = [os.getenv('VOSK_MODEL_PATH'), Path('/usr/share/vosk'), Path.home() / 'AppData/Local/vosk', Path.home() / '.cache/vosk']
 
 def libvoskdir():
     if sys.platform == 'win32':
         libvosk = "libvosk.dll"
     elif sys.platform == 'linux':
         libvosk = "libvosk.so"
-    elif sys.platform == 'linux':
+    elif sys.platform == 'darwin':
         libvosk = "libvosk.dyld"
     dlldir = os.path.abspath(os.path.dirname(__file__))
     os.environ["PATH"] = dlldir + os.pathsep + os.environ['PATH']
     for path in os.environ["PATH"].split(os.pathsep):
         path = path.strip('"')
         if os.path.isfile(os.path.join(path, libvosk)):
             return path
@@ -557,15 +557,15 @@
     def GetPendingChunks(self):
         return _c.vosk_batch_recognizer_get_pending_chunks(self._handle)
 
 #=======================================================================================================================================#
 
 #============================================================== APP PARTS ==============================================================#
 
-VERSION = '0.1.7'
+VERSION = '0.1.8'
 
 arraylist_models = []
 arraylist_models.append("ca-es");
 arraylist_models.append("zh-cn")
 arraylist_models.append("cs-cz");
 arraylist_models.append("nl-nl");
 arraylist_models.append("en-us")
```

### Comparing `pyvosklivesubtitle-0.1.7/pyvosklivesubtitle.egg-info/PKG-INFO` & `pyvosklivesubtitle-0.1.8/pyvosklivesubtitle.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: pyvosklivesubtitle
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Python based desktop aplication that can RECOGNIZE any live streaming in 21 languages that supported by VOSK then TRANSLATE and display it as LIVE SUBTITLES
 Home-page: https://github.com/botbahlul/pyvosklivesubtitle
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
 
 Copyright (c) 2022 Bot Bahlul
```

### Comparing `pyvosklivesubtitle-0.1.7/setup.py` & `pyvosklivesubtitle-0.1.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python3.8
 from __future__ import unicode_literals
 import sys
+import platform
 import os
 import stat
 from pyvosklivesubtitle import VERSION
 
 #from setuptools import setup
 #from setuptools.command.install import install
 #from distutils import log
@@ -34,15 +35,15 @@
     "streamlink>=5.3.1",
     "six>=1.16.0",
     "pysrt>=1.1.2",
     "requests>=2.27.1",
     "tqdm>=4.64.0",
 ]
 
-if sys.platform == "win32":
+if platform.system == "Windows":
     install_requires.append("pywin32>=306")
 
 setup(
     name="pyvosklivesubtitle",
     description="A Python based desktop aplication that can RECOGNIZE any live streaming in 21 languages that supported by VOSK then TRANSLATE and display it as LIVE SUBTITLES",
     version=VERSION,
     include_package_data=True,
```

