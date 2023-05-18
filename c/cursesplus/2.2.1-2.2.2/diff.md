# Comparing `tmp/cursesplus-2.2.1.tar.gz` & `tmp/cursesplus-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cursesplus-2.2.1.tar", last modified: Thu May 18 16:11:04 2023, max compression
+gzip compressed data, was "cursesplus-2.2.2.tar", last modified: Thu May 18 16:14:33 2023, max compression
```

## Comparing `cursesplus-2.2.1.tar` & `cursesplus-2.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-18 16:11:04.601149 cursesplus-2.2.1/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1089 2023-04-07 16:31:31.000000 cursesplus-2.2.1/LICENSE
--rw-r--r--   0 jordan    (1000) jordan    (1000)     1660 2023-05-18 16:11:04.601149 cursesplus-2.2.1/PKG-INFO
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1057 2023-05-18 16:05:26.000000 cursesplus-2.2.1/README.md
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      659 2023-05-18 16:10:15.000000 cursesplus-2.2.1/pyproject.toml
--rw-r--r--   0 jordan    (1000) jordan    (1000)       38 2023-05-18 16:11:04.601149 cursesplus-2.2.1/setup.cfg
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-18 16:11:04.591149 cursesplus-2.2.1/src/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      441 2023-05-18 15:57:38.000000 cursesplus-2.2.1/src/__cptest.py
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-18 16:11:04.591149 cursesplus-2.2.1/src/cursesplus/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      892 2023-04-07 16:31:31.000000 cursesplus-2.2.1/src/cursesplus/__init__.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)    12416 2023-05-18 16:10:09.000000 cursesplus-2.2.1/src/cursesplus/cp.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)    18476 2023-05-18 14:43:10.000000 cursesplus-2.2.1/src/cursesplus/filedialog.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     5980 2023-04-14 17:54:57.000000 cursesplus-2.2.1/src/cursesplus/messagebox.py
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-18 16:11:04.591149 cursesplus-2.2.1/src/cursesplus.egg-info/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1660 2023-05-18 16:11:04.000000 cursesplus-2.2.1/src/cursesplus.egg-info/PKG-INFO
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      306 2023-05-18 16:11:04.000000 cursesplus-2.2.1/src/cursesplus.egg-info/SOURCES.txt
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)        1 2023-05-18 16:11:04.000000 cursesplus-2.2.1/src/cursesplus.egg-info/dependency_links.txt
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)       20 2023-05-18 16:11:04.000000 cursesplus-2.2.1/src/cursesplus.egg-info/top_level.txt
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-18 16:14:33.781135 cursesplus-2.2.2/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1089 2023-04-07 16:31:31.000000 cursesplus-2.2.2/LICENSE
+-rw-r--r--   0 jordan    (1000) jordan    (1000)     1712 2023-05-18 16:14:33.781135 cursesplus-2.2.2/PKG-INFO
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1109 2023-05-18 16:14:16.000000 cursesplus-2.2.2/README.md
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      659 2023-05-18 16:14:01.000000 cursesplus-2.2.2/pyproject.toml
+-rw-r--r--   0 jordan    (1000) jordan    (1000)       38 2023-05-18 16:14:33.781135 cursesplus-2.2.2/setup.cfg
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-18 16:14:33.771135 cursesplus-2.2.2/src/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      441 2023-05-18 15:57:38.000000 cursesplus-2.2.2/src/__cptest.py
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-18 16:14:33.771135 cursesplus-2.2.2/src/cursesplus/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      892 2023-04-07 16:31:31.000000 cursesplus-2.2.2/src/cursesplus/__init__.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)    12425 2023-05-18 16:13:54.000000 cursesplus-2.2.2/src/cursesplus/cp.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)    18476 2023-05-18 14:43:10.000000 cursesplus-2.2.2/src/cursesplus/filedialog.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     5980 2023-04-14 17:54:57.000000 cursesplus-2.2.2/src/cursesplus/messagebox.py
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-18 16:14:33.781135 cursesplus-2.2.2/src/cursesplus.egg-info/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1712 2023-05-18 16:14:33.000000 cursesplus-2.2.2/src/cursesplus.egg-info/PKG-INFO
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      306 2023-05-18 16:14:33.000000 cursesplus-2.2.2/src/cursesplus.egg-info/SOURCES.txt
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)        1 2023-05-18 16:14:33.000000 cursesplus-2.2.2/src/cursesplus.egg-info/dependency_links.txt
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)       20 2023-05-18 16:14:33.000000 cursesplus-2.2.2/src/cursesplus.egg-info/top_level.txt
```

### Comparing `cursesplus-2.2.1/LICENSE` & `cursesplus-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cursesplus-2.2.1/PKG-INFO` & `cursesplus-2.2.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cursesplus
-Version: 2.2.1
+Version: 2.2.2
 Summary: An extension program to curses that offers option menus, message boxes, file dialogs and more
 Author-email: Enderbyte Programs <enderbyte09@gmail.com>
 Project-URL: Homepage, https://github.com/Enderbyte-Programs/Curses-Plus
 Project-URL: Bug Tracker, https://github.com/Enderbyte-Programs/Curses-Plus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -33,14 +33,16 @@
 
 -Add ProgressBarLocation enum-class
 
 -You can now have a small progress bar that does not clear the screen
 
 -displaymsg() will no longer clear itself.
 
+**-WARNING! This update may break progress bars.**
+
 ### Version 2.1: Files 'n' Folders
 
 -Add openfolderdialog()
 
 -Change colours
 
 -Performance improvements for all methods
```

### Comparing `cursesplus-2.2.1/README.md` & `cursesplus-2.2.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 
 -Add ProgressBarLocation enum-class
 
 -You can now have a small progress bar that does not clear the screen
 
 -displaymsg() will no longer clear itself.
 
+**-WARNING! This update may break progress bars.**
+
 ### Version 2.1: Files 'n' Folders
 
 -Add openfolderdialog()
 
 -Change colours
 
 -Performance improvements for all methods
```

### Comparing `cursesplus-2.2.1/pyproject.toml` & `cursesplus-2.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "cursesplus"
-version = "2.2.1"
+version = "2.2.2"
 authors = [{name="Enderbyte Programs",email="enderbyte09@gmail.com"},]
 description = "An extension program to curses that offers option menus, message boxes, file dialogs and more"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
```

### Comparing `cursesplus-2.2.1/src/cursesplus/__init__.py` & `cursesplus-2.2.2/src/cursesplus/__init__.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.2.1/src/cursesplus/cp.py` & `cursesplus-2.2.2/src/cursesplus/cp.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,21 +240,23 @@
     BOTTOM = 2
 
 class ProgressBar:
     def __init__(self,stdscr,max_value: int, bar_type=ProgressBarTypes.SmallProgressBar,bar_location=ProgressBarLocations.TOP,step_value=1,x_size=None,show_percent=True,show_log=None,message="Progress",waitforkeypress=False):
         """Display a Progress Bar with a log. Good for install progresses"""
         self.screen = stdscr
         if show_log is not None:
+        
             #Kept for backwards-compatibility
             self.sl = show_log
+        else:
+            self.sl = bar_type == 0
         self.max = max_value
         self.stepval = step_value
         self.sp = show_percent
-        if show_log is None:
-            self.sl = bar_type == 0
+            
         self.msg = message
         self.ACTIVE = False
         self.value = 0
         self.loglist: list[str] = []
         self.lclist: list[int] = []
         self.submsg = ""
         self.barloc = bar_location
```

### Comparing `cursesplus-2.2.1/src/cursesplus/filedialog.py` & `cursesplus-2.2.2/src/cursesplus/filedialog.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.2.1/src/cursesplus/messagebox.py` & `cursesplus-2.2.2/src/cursesplus/messagebox.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.2.1/src/cursesplus.egg-info/PKG-INFO` & `cursesplus-2.2.2/src/cursesplus.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cursesplus
-Version: 2.2.1
+Version: 2.2.2
 Summary: An extension program to curses that offers option menus, message boxes, file dialogs and more
 Author-email: Enderbyte Programs <enderbyte09@gmail.com>
 Project-URL: Homepage, https://github.com/Enderbyte-Programs/Curses-Plus
 Project-URL: Bug Tracker, https://github.com/Enderbyte-Programs/Curses-Plus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -33,14 +33,16 @@
 
 -Add ProgressBarLocation enum-class
 
 -You can now have a small progress bar that does not clear the screen
 
 -displaymsg() will no longer clear itself.
 
+**-WARNING! This update may break progress bars.**
+
 ### Version 2.1: Files 'n' Folders
 
 -Add openfolderdialog()
 
 -Change colours
 
 -Performance improvements for all methods
```

