# Comparing `tmp/augratin-23.5.17.2.tar.gz` & `tmp/augratin-23.5.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "augratin-23.5.17.2.tar", last modified: Wed May 17 23:58:05 2023, max compression
+gzip compressed data, was "augratin-23.5.18.tar", last modified: Thu May 18 15:22:55 2023, max compression
```

## Comparing `augratin-23.5.17.2.tar` & `augratin-23.5.18.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-17 23:58:05.261321 augratin-23.5.17.2/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-02-19 00:59:20.000000 augratin-23.5.17.2/LICENSE
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4837 2023-05-17 23:58:05.260321 augratin-23.5.17.2/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4060 2023-05-17 23:52:31.000000 augratin-23.5.17.2/README.md
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-17 23:58:05.206320 augratin-23.5.17.2/augratin/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-17 19:16:23.000000 augratin-23.5.17.2/augratin/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40275 2023-05-17 23:54:55.000000 augratin-23.5.17.2/augratin/__main__.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-17 23:58:05.259321 augratin-23.5.17.2/augratin/data/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-02-17 19:16:23.000000 augratin-23.5.17.2/augratin/data/JetBrainsMono-Regular.ttf
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    27092 2023-05-17 23:53:10.000000 augratin-23.5.17.2/augratin/data/dialog.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    22040 2023-02-17 19:16:23.000000 augratin-23.5.17.2/augratin/data/k6gte-augratin-128.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2015 2023-02-17 19:16:23.000000 augratin-23.5.17.2/augratin/data/k6gte-augratin-32.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6303 2023-02-17 19:16:23.000000 augratin-23.5.17.2/augratin/data/k6gte-augratin-64.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-17 19:16:23.000000 augratin-23.5.17.2/augratin/data/k6gte-augratin.desktop
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-17 23:58:05.260321 augratin-23.5.17.2/augratin/lib/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-17 19:16:23.000000 augratin-23.5.17.2/augratin/lib/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13705 2023-05-16 19:37:32.000000 augratin-23.5.17.2/augratin/lib/cat_interface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2071 2023-03-28 14:10:04.000000 augratin-23.5.17.2/augratin/lib/omnirig_interface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       49 2023-05-17 23:44:57.000000 augratin-23.5.17.2/augratin/lib/version.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-17 23:58:05.254321 augratin-23.5.17.2/augratin.egg-info/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4837 2023-05-17 23:58:05.000000 augratin-23.5.17.2/augratin.egg-info/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      591 2023-05-17 23:58:05.000000 augratin-23.5.17.2/augratin.egg-info/SOURCES.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-05-17 23:58:05.000000 augratin-23.5.17.2/augratin.egg-info/dependency_links.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       51 2023-05-17 23:58:05.000000 augratin-23.5.17.2/augratin.egg-info/entry_points.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       71 2023-05-17 23:58:05.000000 augratin-23.5.17.2/augratin.egg-info/requires.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       31 2023-05-17 23:58:05.000000 augratin-23.5.17.2/augratin.egg-info/top_level.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1144 2023-05-17 23:45:04.000000 augratin-23.5.17.2/pyproject.toml
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-05-17 23:58:05.261321 augratin-23.5.17.2/setup.cfg
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-18 15:22:55.489551 augratin-23.5.18/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-02-19 00:59:20.000000 augratin-23.5.18/LICENSE
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4917 2023-05-18 15:22:55.489551 augratin-23.5.18/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4142 2023-05-18 15:21:36.000000 augratin-23.5.18/README.md
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-18 15:22:55.486551 augratin-23.5.18/augratin/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-17 19:16:23.000000 augratin-23.5.18/augratin/__init__.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    40459 2023-05-18 15:05:48.000000 augratin-23.5.18/augratin/__main__.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-18 15:22:55.488551 augratin-23.5.18/augratin/data/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-02-17 19:16:23.000000 augratin-23.5.18/augratin/data/JetBrainsMono-Regular.ttf
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    27092 2023-05-17 23:53:10.000000 augratin-23.5.18/augratin/data/dialog.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    22040 2023-02-17 19:16:23.000000 augratin-23.5.18/augratin/data/k6gte-augratin-128.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2015 2023-02-17 19:16:23.000000 augratin-23.5.18/augratin/data/k6gte-augratin-32.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6303 2023-02-17 19:16:23.000000 augratin-23.5.18/augratin/data/k6gte-augratin-64.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-17 19:16:23.000000 augratin-23.5.18/augratin/data/k6gte-augratin.desktop
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-18 15:22:55.489551 augratin-23.5.18/augratin/lib/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-17 19:16:23.000000 augratin-23.5.18/augratin/lib/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13705 2023-05-16 19:37:32.000000 augratin-23.5.18/augratin/lib/cat_interface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2071 2023-03-28 14:10:04.000000 augratin-23.5.18/augratin/lib/omnirig_interface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-05-18 15:21:49.000000 augratin-23.5.18/augratin/lib/version.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-18 15:22:55.487551 augratin-23.5.18/augratin.egg-info/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4917 2023-05-18 15:22:55.000000 augratin-23.5.18/augratin.egg-info/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      591 2023-05-18 15:22:55.000000 augratin-23.5.18/augratin.egg-info/SOURCES.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-05-18 15:22:55.000000 augratin-23.5.18/augratin.egg-info/dependency_links.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       51 2023-05-18 15:22:55.000000 augratin-23.5.18/augratin.egg-info/entry_points.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       71 2023-05-18 15:22:55.000000 augratin-23.5.18/augratin.egg-info/requires.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       31 2023-05-18 15:22:55.000000 augratin-23.5.18/augratin.egg-info/top_level.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1142 2023-05-18 15:21:58.000000 augratin-23.5.18/pyproject.toml
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-05-18 15:22:55.489551 augratin-23.5.18/setup.cfg
```

### Comparing `augratin-23.5.17.2/LICENSE` & `augratin-23.5.18/LICENSE`

 * *Files identical despite different names*

### Comparing `augratin-23.5.17.2/PKG-INFO` & `augratin-23.5.18/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: augratin
-Version: 23.5.17.2
+Version: 23.5.18
 Summary: An aid for POTA hunters
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/augratin
 Project-URL: Bug Tracker, https://github.com/mbridak/augratin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -52,14 +52,15 @@
 All contacts are stored in an ADIF file in your home directory,
 which you can then import into your normal logging program.
 
 ![screenshot](https://github.com/mbridak/augratin/raw/master/pic/screenshot.png)
 
 ## Recent changes
 
+- [23-5-18] Fix crashes related to if flrig running w/ no radio, or flrig closes.
 - [23-5-17] Reworked bandmap display. Spots with QRT in comment are now muted. Center bandmap on RX freq when changing vfo or zooming display. Provided Non CAT control users to change bands.
 - [23-5-15] Start big code changes to impliment better bandmap.
 - [23-3-28] Merged in changes from @barryshaffer KK7JXG to add support for Omnirig on windows.
 - [23-3-7] Reduced network timeout for spot pulls from 15 to 5 seconds. Safer dictionary key access.
 - [23-2-17] Repackaged for PyPi and pip install
 
 ## Installing, Updating, Running, Removing
```

### Comparing `augratin-23.5.17.2/README.md` & `augratin-23.5.18/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 All contacts are stored in an ADIF file in your home directory,
 which you can then import into your normal logging program.
 
 ![screenshot](https://github.com/mbridak/augratin/raw/master/pic/screenshot.png)
 
 ## Recent changes
 
+- [23-5-18] Fix crashes related to if flrig running w/ no radio, or flrig closes.
 - [23-5-17] Reworked bandmap display. Spots with QRT in comment are now muted. Center bandmap on RX freq when changing vfo or zooming display. Provided Non CAT control users to change bands.
 - [23-5-15] Start big code changes to impliment better bandmap.
 - [23-3-28] Merged in changes from @barryshaffer KK7JXG to add support for Omnirig on windows.
 - [23-3-7] Reduced network timeout for spot pulls from 15 to 5 seconds. Safer dictionary key access.
 - [23-2-17] Repackaged for PyPi and pip install
 
 ## Installing, Updating, Running, Removing
```

### Comparing `augratin-23.5.17.2/augratin/__main__.py` & `augratin-23.5.18/augratin/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -403,19 +403,26 @@
         )
         data = io.BytesIO()
         self.map.save(data, close_file=False)
         self.mapview.setHtml(data.getvalue().decode())
 
     def poll_radio(self):
         """Get Freq and Mode changes"""
-        if self.cat_control:
-            newfreq = float(self.cat_control.get_vfo()) / 1000000
-            # newmode = self.cat_control.get_mode()
+        if self.cat_control.online:
+            try:
+                newfreq = float(self.cat_control.get_vfo()) / 1000000
+            except ValueError:
+                return
             if hasattr(self.cat_control, "get_bw"):
-                newbw = int(self.cat_control.get_bw())
+                try:
+                    newbw = int(self.cat_control.get_bw())
+                except TypeError:
+                    newbw = 0
+                except ValueError:
+                    newbw = 0
             else:
                 newbw = 0
             if self.rx_freq != newfreq:
                 self.rx_freq = newfreq
                 self.set_band(f"{self.getband(str(int(newfreq * 1000)))}m")
                 step, _ = self.determine_step_digits()
                 self.drawTXRXMarks(step)
```

### Comparing `augratin-23.5.17.2/augratin/data/JetBrainsMono-Regular.ttf` & `augratin-23.5.18/augratin/data/JetBrainsMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `augratin-23.5.17.2/augratin/data/dialog.ui` & `augratin-23.5.18/augratin/data/dialog.ui`

 * *Files identical despite different names*

### Comparing `augratin-23.5.17.2/augratin/data/k6gte-augratin-128.png` & `augratin-23.5.18/augratin/data/k6gte-augratin-128.png`

 * *Files identical despite different names*

### Comparing `augratin-23.5.17.2/augratin/data/k6gte-augratin-32.png` & `augratin-23.5.18/augratin/data/k6gte-augratin-32.png`

 * *Files identical despite different names*

### Comparing `augratin-23.5.17.2/augratin/data/k6gte-augratin-64.png` & `augratin-23.5.18/augratin/data/k6gte-augratin-64.png`

 * *Files identical despite different names*

### Comparing `augratin-23.5.17.2/augratin/lib/cat_interface.py` & `augratin-23.5.18/augratin/lib/cat_interface.py`

 * *Files identical despite different names*

### Comparing `augratin-23.5.17.2/augratin/lib/omnirig_interface.py` & `augratin-23.5.18/augratin/lib/omnirig_interface.py`

 * *Files identical despite different names*

### Comparing `augratin-23.5.17.2/augratin.egg-info/PKG-INFO` & `augratin-23.5.18/augratin.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: augratin
-Version: 23.5.17.2
+Version: 23.5.18
 Summary: An aid for POTA hunters
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/augratin
 Project-URL: Bug Tracker, https://github.com/mbridak/augratin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -52,14 +52,15 @@
 All contacts are stored in an ADIF file in your home directory,
 which you can then import into your normal logging program.
 
 ![screenshot](https://github.com/mbridak/augratin/raw/master/pic/screenshot.png)
 
 ## Recent changes
 
+- [23-5-18] Fix crashes related to if flrig running w/ no radio, or flrig closes.
 - [23-5-17] Reworked bandmap display. Spots with QRT in comment are now muted. Center bandmap on RX freq when changing vfo or zooming display. Provided Non CAT control users to change bands.
 - [23-5-15] Start big code changes to impliment better bandmap.
 - [23-3-28] Merged in changes from @barryshaffer KK7JXG to add support for Omnirig on windows.
 - [23-3-7] Reduced network timeout for spot pulls from 15 to 5 seconds. Safer dictionary key access.
 - [23-2-17] Repackaged for PyPi and pip install
 
 ## Installing, Updating, Running, Removing
```

### Comparing `augratin-23.5.17.2/augratin.egg-info/SOURCES.txt` & `augratin-23.5.18/augratin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `augratin-23.5.17.2/pyproject.toml` & `augratin-23.5.18/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "augratin" 
-version = "23.5.17.2"
+version = "23.5.18"
 description = "An aid for POTA hunters"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
   { name="Michael Bridak", email="michael.bridak@gmail.com" },
 ]
```

