# Comparing `tmp/augratin-23.5.18.tar.gz` & `tmp/augratin-23.5.18.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "augratin-23.5.18.tar", last modified: Thu May 18 15:22:55 2023, max compression
+gzip compressed data, was "augratin-23.5.18.1.tar", last modified: Thu May 18 18:37:36 2023, max compression
```

## Comparing `augratin-23.5.18.tar` & `augratin-23.5.18.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-18 15:22:55.489551 augratin-23.5.18/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-02-19 00:59:20.000000 augratin-23.5.18/LICENSE
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4917 2023-05-18 15:22:55.489551 augratin-23.5.18/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4142 2023-05-18 15:21:36.000000 augratin-23.5.18/README.md
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-18 15:22:55.486551 augratin-23.5.18/augratin/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-17 19:16:23.000000 augratin-23.5.18/augratin/__init__.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    40459 2023-05-18 15:05:48.000000 augratin-23.5.18/augratin/__main__.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-18 15:22:55.488551 augratin-23.5.18/augratin/data/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-02-17 19:16:23.000000 augratin-23.5.18/augratin/data/JetBrainsMono-Regular.ttf
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    27092 2023-05-17 23:53:10.000000 augratin-23.5.18/augratin/data/dialog.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    22040 2023-02-17 19:16:23.000000 augratin-23.5.18/augratin/data/k6gte-augratin-128.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2015 2023-02-17 19:16:23.000000 augratin-23.5.18/augratin/data/k6gte-augratin-32.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6303 2023-02-17 19:16:23.000000 augratin-23.5.18/augratin/data/k6gte-augratin-64.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-17 19:16:23.000000 augratin-23.5.18/augratin/data/k6gte-augratin.desktop
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-18 15:22:55.489551 augratin-23.5.18/augratin/lib/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-17 19:16:23.000000 augratin-23.5.18/augratin/lib/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13705 2023-05-16 19:37:32.000000 augratin-23.5.18/augratin/lib/cat_interface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2071 2023-03-28 14:10:04.000000 augratin-23.5.18/augratin/lib/omnirig_interface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-05-18 15:21:49.000000 augratin-23.5.18/augratin/lib/version.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-18 15:22:55.487551 augratin-23.5.18/augratin.egg-info/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4917 2023-05-18 15:22:55.000000 augratin-23.5.18/augratin.egg-info/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      591 2023-05-18 15:22:55.000000 augratin-23.5.18/augratin.egg-info/SOURCES.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-05-18 15:22:55.000000 augratin-23.5.18/augratin.egg-info/dependency_links.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       51 2023-05-18 15:22:55.000000 augratin-23.5.18/augratin.egg-info/entry_points.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       71 2023-05-18 15:22:55.000000 augratin-23.5.18/augratin.egg-info/requires.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       31 2023-05-18 15:22:55.000000 augratin-23.5.18/augratin.egg-info/top_level.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1142 2023-05-18 15:21:58.000000 augratin-23.5.18/pyproject.toml
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-05-18 15:22:55.489551 augratin-23.5.18/setup.cfg
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-18 18:37:36.142726 augratin-23.5.18.1/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-02-19 00:59:20.000000 augratin-23.5.18.1/LICENSE
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5080 2023-05-18 18:37:36.142726 augratin-23.5.18.1/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4303 2023-05-18 18:31:11.000000 augratin-23.5.18.1/README.md
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-18 18:37:36.129727 augratin-23.5.18.1/augratin/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-17 19:16:23.000000 augratin-23.5.18.1/augratin/__init__.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    41921 2023-05-18 18:27:05.000000 augratin-23.5.18.1/augratin/__main__.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-18 18:37:36.138726 augratin-23.5.18.1/augratin/data/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-02-17 19:16:23.000000 augratin-23.5.18.1/augratin/data/JetBrainsMono-Regular.ttf
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    27092 2023-05-17 23:53:10.000000 augratin-23.5.18.1/augratin/data/dialog.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    22040 2023-02-17 19:16:23.000000 augratin-23.5.18.1/augratin/data/k6gte-augratin-128.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2015 2023-02-17 19:16:23.000000 augratin-23.5.18.1/augratin/data/k6gte-augratin-32.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6303 2023-02-17 19:16:23.000000 augratin-23.5.18.1/augratin/data/k6gte-augratin-64.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-17 19:16:23.000000 augratin-23.5.18.1/augratin/data/k6gte-augratin.desktop
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-18 18:37:36.141726 augratin-23.5.18.1/augratin/lib/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-17 19:16:23.000000 augratin-23.5.18.1/augratin/lib/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13852 2023-05-18 16:38:33.000000 augratin-23.5.18.1/augratin/lib/cat_interface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2071 2023-03-28 14:10:04.000000 augratin-23.5.18.1/augratin/lib/omnirig_interface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       49 2023-05-18 18:32:25.000000 augratin-23.5.18.1/augratin/lib/version.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-18 18:37:36.132726 augratin-23.5.18.1/augratin.egg-info/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5080 2023-05-18 18:37:36.000000 augratin-23.5.18.1/augratin.egg-info/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      591 2023-05-18 18:37:36.000000 augratin-23.5.18.1/augratin.egg-info/SOURCES.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-05-18 18:37:36.000000 augratin-23.5.18.1/augratin.egg-info/dependency_links.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       51 2023-05-18 18:37:36.000000 augratin-23.5.18.1/augratin.egg-info/entry_points.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       71 2023-05-18 18:37:36.000000 augratin-23.5.18.1/augratin.egg-info/requires.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       31 2023-05-18 18:37:36.000000 augratin-23.5.18.1/augratin.egg-info/top_level.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1144 2023-05-18 18:32:28.000000 augratin-23.5.18.1/pyproject.toml
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-05-18 18:37:36.142726 augratin-23.5.18.1/setup.cfg
```

### Comparing `augratin-23.5.18/LICENSE` & `augratin-23.5.18.1/LICENSE`

 * *Files identical despite different names*

### Comparing `augratin-23.5.18/PKG-INFO` & `augratin-23.5.18.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: augratin
-Version: 23.5.18
+Version: 23.5.18.1
 Summary: An aid for POTA hunters
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/augratin
 Project-URL: Bug Tracker, https://github.com/mbridak/augratin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -52,15 +52,15 @@
 All contacts are stored in an ADIF file in your home directory,
 which you can then import into your normal logging program.
 
 ![screenshot](https://github.com/mbridak/augratin/raw/master/pic/screenshot.png)
 
 ## Recent changes
 
-- [23-5-18] Fix crashes related to if flrig running w/ no radio, or flrig closes.
+- [23-5-18] Fix crashes related to if flrig running w/ no radio, or flrig closes. Add dialog message window to initial startup if CAT control failed. For some reason I was missing the 17m band. Added back band selector for those who have CAT.
 - [23-5-17] Reworked bandmap display. Spots with QRT in comment are now muted. Center bandmap on RX freq when changing vfo or zooming display. Provided Non CAT control users to change bands.
 - [23-5-15] Start big code changes to impliment better bandmap.
 - [23-3-28] Merged in changes from @barryshaffer KK7JXG to add support for Omnirig on windows.
 - [23-3-7] Reduced network timeout for spot pulls from 15 to 5 seconds. Safer dictionary key access.
 - [23-2-17] Repackaged for PyPi and pip install
 
 ## Installing, Updating, Running, Removing
```

### Comparing `augratin-23.5.18/README.md` & `augratin-23.5.18.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 All contacts are stored in an ADIF file in your home directory,
 which you can then import into your normal logging program.
 
 ![screenshot](https://github.com/mbridak/augratin/raw/master/pic/screenshot.png)
 
 ## Recent changes
 
-- [23-5-18] Fix crashes related to if flrig running w/ no radio, or flrig closes.
+- [23-5-18] Fix crashes related to if flrig running w/ no radio, or flrig closes. Add dialog message window to initial startup if CAT control failed. For some reason I was missing the 17m band. Added back band selector for those who have CAT.
 - [23-5-17] Reworked bandmap display. Spots with QRT in comment are now muted. Center bandmap on RX freq when changing vfo or zooming display. Provided Non CAT control users to change bands.
 - [23-5-15] Start big code changes to impliment better bandmap.
 - [23-3-28] Merged in changes from @barryshaffer KK7JXG to add support for Omnirig on windows.
 - [23-3-7] Reduced network timeout for spot pulls from 15 to 5 seconds. Safer dictionary key access.
 - [23-2-17] Repackaged for PyPi and pip install
 
 ## Installing, Updating, Running, Removing
```

### Comparing `augratin-23.5.18/augratin/__main__.py` & `augratin-23.5.18.1/augratin/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,15 +153,17 @@
     bands = {
         "160m": (1.8, 2),
         "80m": (3.5, 4),
         "60m": (5.102, 5.4065),
         "40m": (7.0, 7.3),
         "30m": (10.1, 10.15),
         "20m": (14.0, 14.35),
+        "17m": (18.068, 18.168),
         "15m": (21.0, 21.45),
+        "12m": (24.89, 24.99),
         "10m": (28.0, 29.7),
         "6m": (50.0, 54.0),
         "4m": (70.0, 71.0),
         "2m": (144.0, 148.0),
     }
 
     def __init__(self, band: str) -> None:
@@ -310,14 +312,18 @@
     spots = None
     map = None
     loggable = False
     MAP_TILES = "OpenStreetMap"
 
     def __init__(self, parent=None):
         """Initialize class variables"""
+        super().__init__(parent)
+        data_path = WORKING_PATH + "/data/dialog.ui"
+        uic.loadUi(data_path, self)
+
         self.settings = {
             "mycall": "",
             "mygrid": "",
         }
         try:
             home = os.path.expanduser("~")
             if os.path.exists(f"{home}/.augratin.json"):
@@ -343,49 +349,61 @@
 
         self.cat_control = None
         local_flrig = self.check_process("flrig")
         local_rigctld = self.check_process("rigctld")
         local_omnirig = self.check_process("omnirig.exe")
 
         if FORCED_INTERFACE:
+            logger.debug("%s", f"Forced interface: {FORCED_INTERFACE} {SERVER_ADDRESS}")
             address, port = SERVER_ADDRESS.split(":")
             self.cat_control = CAT(FORCED_INTERFACE, address, int(port))
-
-        if self.cat_control is None:
+            if self.cat_control.online is False:
+                self.show_message_box(
+                    f"Was unable to connect to {FORCED_INTERFACE}.\n"
+                    f"Using Address: {address} Port: {port}"
+                )
+        else:
             if local_flrig:
                 if SERVER_ADDRESS:
                     address, port = SERVER_ADDRESS.split(":")
                 else:
                     address, port = "localhost", "12345"
-                    self.cat_control = CAT("flrig", address, int(port))
+                self.cat_control = CAT("flrig", address, int(port))
+                if self.cat_control.online is False:
+                    self.show_message_box(
+                        "Was unable to connect to flrig.\n"
+                        f"Using Address: {address} Port: {port}"
+                    )
             if local_rigctld:
                 if SERVER_ADDRESS:
                     address, port = SERVER_ADDRESS.split(":")
                 else:
                     address, port = "localhost", "4532"
-                    self.cat_control = CAT("rigctld", address, int(port))
+                self.cat_control = CAT("rigctld", address, int(port))
+                if self.cat_control.online is False:
+                    self.show_message_box(
+                        "Was unable to connect to rigctld.\n"
+                        f"Using Address: {address} Port: {port}"
+                    )
             if local_omnirig:
                 self.cat_control = OmniRigClient(OMNI_RIGNUMBER)
                 logging.debug("omnirig called")
 
-        super().__init__(parent)
-        data_path = WORKING_PATH + "/data/dialog.ui"
-        uic.loadUi(data_path, self)
         self.zoom_in_button.clicked.connect(self.dec_zoom)
         self.zoom_out_button.clicked.connect(self.inc_zoom)
         self.bandmap_scene = QtWidgets.QGraphicsScene()
         self.bandmap_scene.clear()
         self.bandmap_scene.setFocusOnTouch(False)
         self.bandmap_scene.selectionChanged.connect(self.spotclicked)
         self.bandmap_scene.setFont(QtGui.QFont("JetBrains Mono", pointSize=5))
         self.spotdb = Database()
         self.comboBox_mode.currentTextChanged.connect(self.getspots)
         self.comboBox_band.currentTextChanged.connect(self.nocat_bandchange)
-        if self.cat_control is not None:
-            self.comboBox_band.hide()
+        # if self.cat_control is not None:
+        #     self.comboBox_band.hide()
 
         self.mycall_field.textEdited.connect(self.save_call_and_grid)
         self.mygrid_field.textEdited.connect(self.save_call_and_grid)
         self.log_button.clicked.connect(self.log_contact)
         self.mycall_field.setText(self.settings.get("mycall", ""))
         self.mygrid_field.setText(self.settings.get("mygrid", ""))
         if self.settings.get("mygrid", "") == "":
@@ -403,38 +421,48 @@
         )
         data = io.BytesIO()
         self.map.save(data, close_file=False)
         self.mapview.setHtml(data.getvalue().decode())
 
     def poll_radio(self):
         """Get Freq and Mode changes"""
-        if self.cat_control.online:
-            try:
-                newfreq = float(self.cat_control.get_vfo()) / 1000000
-            except ValueError:
-                return
-            if hasattr(self.cat_control, "get_bw"):
+        if self.cat_control:
+            if self.cat_control.online:
                 try:
-                    newbw = int(self.cat_control.get_bw())
-                except TypeError:
-                    newbw = 0
+                    newfreq = float(self.cat_control.get_vfo()) / 1000000
                 except ValueError:
+                    return
+                if hasattr(self.cat_control, "get_bw"):
+                    try:
+                        newbw = int(self.cat_control.get_bw())
+                    except TypeError:
+                        newbw = 0
+                    except ValueError:
+                        newbw = 0
+                else:
                     newbw = 0
-            else:
-                newbw = 0
-            if self.rx_freq != newfreq:
-                self.rx_freq = newfreq
-                self.set_band(f"{self.getband(str(int(newfreq * 1000)))}m")
-                step, _ = self.determine_step_digits()
-                self.drawTXRXMarks(step)
-                self.center_on_rxfreq()
-            if self.bandwidth != newbw:
-                self.bandwidth = newbw
-                step, _ = self.determine_step_digits()
-                self.drawTXRXMarks(step)
+                if self.rx_freq != newfreq:
+                    self.rx_freq = newfreq
+                    self.set_band(f"{self.getband(str(int(newfreq * 1000)))}m")
+                    step, _ = self.determine_step_digits()
+                    self.drawTXRXMarks(step)
+                    self.center_on_rxfreq()
+                if self.bandwidth != newbw:
+                    self.bandwidth = newbw
+                    step, _ = self.determine_step_digits()
+                    self.drawTXRXMarks(step)
+
+    def show_message_box(self, message: str) -> None:
+        """Display a message box to the user."""
+        message_box = QtWidgets.QMessageBox()
+        message_box.setIcon(QtWidgets.QMessageBox.Information)
+        message_box.setText(message)
+        message_box.setWindowTitle("Information")
+        message_box.setStandardButtons(QtWidgets.QMessageBox.Ok)
+        _ = message_box.exec_()
 
     def nocat_bandchange(self) -> None:
         """Called when the bandselector dropdown changes."""
         band = self.comboBox_band.currentText()
         self.set_band(f"{band}m")
         self.update()
 
@@ -546,16 +574,19 @@
 
     def getspots(self):
         """Gets activator spots from pota.app"""
         self.time.setText(str(datetime.now(timezone.utc)).split()[1].split(".")[0][0:5])
         self.spots = self.getjson(self.potaurl)
         if self.spots:
             for spot in self.spots:
-                spot["frequency"] = float(spot.get("frequency")) / 1000
-                self.spotdb.addspot(spot)
+                try:
+                    spot["frequency"] = float(spot.get("frequency")) / 1000
+                    self.spotdb.addspot(spot)
+                except ValueError:
+                    pass
             self.update()
 
     def log_contact(self):
         """Log the contact"""
         if self.loggable is False:
             return
         try:
```

### Comparing `augratin-23.5.18/augratin/data/JetBrainsMono-Regular.ttf` & `augratin-23.5.18.1/augratin/data/JetBrainsMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `augratin-23.5.18/augratin/data/dialog.ui` & `augratin-23.5.18.1/augratin/data/dialog.ui`

 * *Files identical despite different names*

### Comparing `augratin-23.5.18/augratin/data/k6gte-augratin-128.png` & `augratin-23.5.18.1/augratin/data/k6gte-augratin-128.png`

 * *Files identical despite different names*

### Comparing `augratin-23.5.18/augratin/data/k6gte-augratin-32.png` & `augratin-23.5.18.1/augratin/data/k6gte-augratin-32.png`

 * *Files identical despite different names*

### Comparing `augratin-23.5.18/augratin/data/k6gte-augratin-64.png` & `augratin-23.5.18.1/augratin/data/k6gte-augratin-64.png`

 * *Files identical despite different names*

### Comparing `augratin-23.5.18/augratin/lib/cat_interface.py` & `augratin-23.5.18.1/augratin/lib/cat_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,18 @@
         self.port = port
         self.online = False
         if self.interface == "flrig":
             target = f"http://{host}:{port}"
             logger.debug("%s", target)
             self.server = xmlrpc.client.ServerProxy(target)
             self.online = True
+            try:
+                _ = self.server.main.get_version()
+            except ConnectionRefusedError:
+                self.online = False
         if self.interface == "rigctld":
             self.__initialize_rigctrld()
 
     def __initialize_rigctrld(self):
         try:
             self.rigctrlsocket = socket.socket()
             self.rigctrlsocket.settimeout(0.5)
```

### Comparing `augratin-23.5.18/augratin/lib/omnirig_interface.py` & `augratin-23.5.18.1/augratin/lib/omnirig_interface.py`

 * *Files identical despite different names*

### Comparing `augratin-23.5.18/augratin.egg-info/PKG-INFO` & `augratin-23.5.18.1/augratin.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: augratin
-Version: 23.5.18
+Version: 23.5.18.1
 Summary: An aid for POTA hunters
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/augratin
 Project-URL: Bug Tracker, https://github.com/mbridak/augratin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -52,15 +52,15 @@
 All contacts are stored in an ADIF file in your home directory,
 which you can then import into your normal logging program.
 
 ![screenshot](https://github.com/mbridak/augratin/raw/master/pic/screenshot.png)
 
 ## Recent changes
 
-- [23-5-18] Fix crashes related to if flrig running w/ no radio, or flrig closes.
+- [23-5-18] Fix crashes related to if flrig running w/ no radio, or flrig closes. Add dialog message window to initial startup if CAT control failed. For some reason I was missing the 17m band. Added back band selector for those who have CAT.
 - [23-5-17] Reworked bandmap display. Spots with QRT in comment are now muted. Center bandmap on RX freq when changing vfo or zooming display. Provided Non CAT control users to change bands.
 - [23-5-15] Start big code changes to impliment better bandmap.
 - [23-3-28] Merged in changes from @barryshaffer KK7JXG to add support for Omnirig on windows.
 - [23-3-7] Reduced network timeout for spot pulls from 15 to 5 seconds. Safer dictionary key access.
 - [23-2-17] Repackaged for PyPi and pip install
 
 ## Installing, Updating, Running, Removing
```

### Comparing `augratin-23.5.18/augratin.egg-info/SOURCES.txt` & `augratin-23.5.18.1/augratin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `augratin-23.5.18/pyproject.toml` & `augratin-23.5.18.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "augratin" 
-version = "23.5.18"
+version = "23.5.18.1"
 description = "An aid for POTA hunters"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
   { name="Michael Bridak", email="michael.bridak@gmail.com" },
 ]
```

