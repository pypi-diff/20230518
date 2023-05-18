# Comparing `tmp/cursesplus-2.1.tar.gz` & `tmp/cursesplus-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cursesplus-2.1.tar", last modified: Thu May 18 14:48:04 2023, max compression
+gzip compressed data, was "cursesplus-2.2.0.tar", last modified: Thu May 18 16:06:27 2023, max compression
```

## Comparing `cursesplus-2.1.tar` & `cursesplus-2.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-18 14:48:04.831158 cursesplus-2.1/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1089 2023-04-07 16:31:31.000000 cursesplus-2.1/LICENSE
--rw-r--r--   0 jordan    (1000) jordan    (1000)     1442 2023-05-18 14:48:04.831158 cursesplus-2.1/PKG-INFO
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      841 2023-05-18 14:47:48.000000 cursesplus-2.1/README.md
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      657 2023-05-18 14:46:14.000000 cursesplus-2.1/pyproject.toml
--rw-r--r--   0 jordan    (1000) jordan    (1000)       38 2023-05-18 14:48:04.831158 cursesplus-2.1/setup.cfg
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-18 14:48:04.831158 cursesplus-2.1/src/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      288 2023-05-18 14:35:12.000000 cursesplus-2.1/src/__cptest.py
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-18 14:48:04.831158 cursesplus-2.1/src/cursesplus/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      892 2023-04-07 16:31:31.000000 cursesplus-2.1/src/cursesplus/__init__.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)    11516 2023-04-07 16:31:31.000000 cursesplus-2.1/src/cursesplus/cp.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)    18476 2023-05-18 14:43:10.000000 cursesplus-2.1/src/cursesplus/filedialog.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     5980 2023-04-14 17:54:57.000000 cursesplus-2.1/src/cursesplus/messagebox.py
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-18 14:48:04.831158 cursesplus-2.1/src/cursesplus.egg-info/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1442 2023-05-18 14:48:04.000000 cursesplus-2.1/src/cursesplus.egg-info/PKG-INFO
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      306 2023-05-18 14:48:04.000000 cursesplus-2.1/src/cursesplus.egg-info/SOURCES.txt
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)        1 2023-05-18 14:48:04.000000 cursesplus-2.1/src/cursesplus.egg-info/dependency_links.txt
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)       20 2023-05-18 14:48:04.000000 cursesplus-2.1/src/cursesplus.egg-info/top_level.txt
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-18 16:06:27.241164 cursesplus-2.2.0/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1089 2023-04-07 16:31:31.000000 cursesplus-2.2.0/LICENSE
+-rw-r--r--   0 jordan    (1000) jordan    (1000)     1660 2023-05-18 16:06:27.241164 cursesplus-2.2.0/PKG-INFO
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1057 2023-05-18 16:05:26.000000 cursesplus-2.2.0/README.md
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      659 2023-05-18 16:06:14.000000 cursesplus-2.2.0/pyproject.toml
+-rw-r--r--   0 jordan    (1000) jordan    (1000)       38 2023-05-18 16:06:27.241164 cursesplus-2.2.0/setup.cfg
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-18 16:06:27.241164 cursesplus-2.2.0/src/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      441 2023-05-18 15:57:38.000000 cursesplus-2.2.0/src/__cptest.py
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-18 16:06:27.241164 cursesplus-2.2.0/src/cursesplus/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      892 2023-04-07 16:31:31.000000 cursesplus-2.2.0/src/cursesplus/__init__.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)    12382 2023-05-18 16:05:19.000000 cursesplus-2.2.0/src/cursesplus/cp.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)    18476 2023-05-18 14:43:10.000000 cursesplus-2.2.0/src/cursesplus/filedialog.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     5980 2023-04-14 17:54:57.000000 cursesplus-2.2.0/src/cursesplus/messagebox.py
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-18 16:06:27.241164 cursesplus-2.2.0/src/cursesplus.egg-info/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1660 2023-05-18 16:06:27.000000 cursesplus-2.2.0/src/cursesplus.egg-info/PKG-INFO
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      306 2023-05-18 16:06:27.000000 cursesplus-2.2.0/src/cursesplus.egg-info/SOURCES.txt
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)        1 2023-05-18 16:06:27.000000 cursesplus-2.2.0/src/cursesplus.egg-info/dependency_links.txt
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)       20 2023-05-18 16:06:27.000000 cursesplus-2.2.0/src/cursesplus.egg-info/top_level.txt
```

### Comparing `cursesplus-2.1/LICENSE` & `cursesplus-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cursesplus-2.1/PKG-INFO` & `cursesplus-2.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cursesplus
-Version: 2.1
+Version: 2.2.0
 Summary: An extension program to curses that offers option menus, message boxes, file dialogs and more
 Author-email: Enderbyte Programs <enderbyte09@gmail.com>
 Project-URL: Homepage, https://github.com/Enderbyte-Programs/Curses-Plus
 Project-URL: Bug Tracker, https://github.com/Enderbyte-Programs/Curses-Plus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,14 +23,24 @@
 ### SPECIAL INSTRUCTIONS FOR WINDOWS
 
 For Windows you need to also install ```windows-curses``` or related program
 to provide the basic curses functionality
 
 ## What's New?
 
+### Version 2.2: Progressbar
+
+-Add ProgressBarTypes enum-class
+
+-Add ProgressBarLocation enum-class
+
+-You can now have a small progress bar that does not clear the screen
+
+-displaymsg() will no longer clear itself.
+
 ### Version 2.1: Files 'n' Folders
 
 -Add openfolderdialog()
 
 -Change colours
 
 -Performance improvements for all methods
```

### Comparing `cursesplus-2.1/pyproject.toml` & `cursesplus-2.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "cursesplus"
-version = "2.1"
+version = "2.2.0"
 authors = [{name="Enderbyte Programs",email="enderbyte09@gmail.com"},]
 description = "An extension program to curses that offers option menus, message boxes, file dialogs and more"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
```

### Comparing `cursesplus-2.1/src/cursesplus/__init__.py` & `cursesplus-2.2.0/src/cursesplus/__init__.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.1/src/cursesplus/cp.py` & `cursesplus-2.2.0/src/cursesplus/cp.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     
     for msgl in message:
         mi += 1
         stdscr.addstr(int(y//2+mi),int(x//2-len(msgl)//2),msgl)
     stdscr.addstr(y-2,0,"Press any key to dismiss this message")
     stdscr.refresh()
     stdscr.getch()
-    stdscr.erase()
+    
 
 def displaymsgnodelay(stdscr,message: list):
     """
     Display a message in a rectangle. message is a list. Each item in the list is a new line. Unlike displaymsg, the message will not need a keypress to continue. This is good for progress waiing.
     """
     stdscr.clear()
     x,y = os.get_terminal_size()
@@ -102,15 +102,15 @@
     stdscr.addstr(0,0,"Message: ")
     mi = -(len(message)/2)
     
     for msgl in message:
         mi += 1
         stdscr.addstr(int(y//2+mi),int(x//2-len(msgl)//2),msgl)
     stdscr.refresh()
-    stdscr.erase()
+    
 
 def cursesinput(stdscr,prompt: str):
     """
     Get a single line input of text from curses. To be used instead of Python standard input()
     """
     x,y = os.get_terminal_size()
     stdscr.erase()
@@ -168,15 +168,15 @@
             selected -= 1
         elif _ch == curses.KEY_DOWN and selected < len(options)-1:
             if selected >= my-6:
                 offset += 1
             selected += 1
         elif _ch == curses.KEY_BACKSPACE or _ch == 98:
             return -1
-        stdscr.erase()
+        
 def optionmenu(stdscr,options:list,title="Please choose an option and press enter") -> int:
     """Alias function to displayops()"""
     return displayops(stdscr,options,title)
 
 def askyesno_old(stdscr,title: str) -> bool:
     """Ask a yes no question provided by title."""
     result = displayops(stdscr,["Yes","No"],title)
@@ -227,49 +227,71 @@
     """Hide Cursor. Can only be called in an active curses window"""
     curses.curs_set(0)
 
 def showcursor():
     """Show cursor. Can only be called in an active curses window"""
     curses.curs_set(1)
 
+class ProgressBarTypes:
+    FullScreenProgressBar: int = 0
+    SmallProgressBar: int = 1
+class ProgressBarLocations:
+    TOP = 0
+    CENTER = 1
+    BOTTOM = 2
+
 class ProgressBar:
-    def __init__(self,stdscr,max_value: int, step_value=1,show_percent=True,show_log=False,message="Progress",waitforkeypress=False):
+    def __init__(self,stdscr,max_value: int, bar_type=ProgressBarTypes.SmallProgressBar,bar_location=ProgressBarLocations.TOP,step_value=1,x_size=None,show_percent=True,show_log=None,message="Progress",waitforkeypress=False):
         """Display a Progress Bar with a log. Good for install progresses"""
         self.screen = stdscr
+        if show_log is not None:
+            #Kept for backwards-compatibility
+            self.sl = show_log
         self.max = max_value
         self.stepval = step_value
         self.sp = show_percent
-        self.sl = show_log
+        self.sl = bar_type == 0
         self.msg = message
         self.ACTIVE = False
         self.value = 0
         self.loglist: list[str] = []
         self.lclist: list[int] = []
         self.submsg = ""
+        self.barloc = bar_location
+        if bar_type == ProgressBarTypes.FullScreenProgressBar and bar_location != ProgressBarLocations.TOP:
+            raise ValueError("Full screen progress bars may not have their locations changed.")
         self.mx, self.my = os.get_terminal_size()
         self.wfkp = waitforkeypress
     def update(self):
+        sz = self.screen.getmaxyx()[0]
+        if self.barloc == 0:
+            ydraw = 0
+        elif self.barloc == 1:
+            ydraw = sz //2-1
+        elif self.barloc == 2:
+            ydraw = sz-4
         lheight = self.my - 7
         """Redraws progress bar"""
-        self.screen.erase()
-        self.screen.addstr(0,0," "*(self.mx-1),set_colour(BLUE,WHITE))
-        self.screen.addstr(0,0,self.msg[0:self.mx-1],set_colour(BLUE,WHITE))
+        if self.sl:
+            self.screen.erase()
+        self.screen.addstr(ydraw,0," "*(self.mx-1),set_colour(BLUE,WHITE))
+        self.screen.addstr(ydraw,0,self.msg[0:self.mx-1],set_colour(BLUE,WHITE))
         #filline(self.screen,1,set_colour(GREEN,WHITE))
-        filline(self.screen,2,set_colour(RED,WHITE))
+        filline(self.screen,ydraw+2,set_colour(RED,WHITE))
         #filline(self.screen,3,set_colour(GREEN,WHITE))
-        self.screen.addstr(1,0,"-"*(self.mx-1),set_colour(RED,WHITE))
-        self.screen.addstr(3,0,"-"*(self.mx-1),set_colour(RED,WHITE))
+        self.screen.addstr(ydraw+1,0,"-"*(self.mx-1),set_colour(RED,WHITE))
+        self.screen.addstr(ydraw+3,0,"-"*(self.mx-1),set_colour(RED,WHITE))
         barfill = round((self.value/self.max)*self.mx-1)
         if not self.value > self.max:
-            self.screen.addstr(2,0," "*barfill,set_colour(GREEN,WHITE))
+            self.screen.addstr(ydraw+2,0," "*barfill,set_colour(GREEN,WHITE))
         else:
-            self.screen.addstr(2,0," "*self.mx-1,set_colour(GREEN,WHITE))
-        self.screen.addstr(3,0,self.submsg[0:self.mx-1],set_colour(RED,WHITE))
+            self.screen.addstr(ydraw+2,0," "*self.mx-1,set_colour(GREEN,WHITE))
+        self.screen.addstr(ydraw+3,0,self.submsg[0:self.mx-1],set_colour(RED,WHITE))
         if self.sp:
-            self.screen.addstr(3,self.mx-7,f"{round(self.value/self.max*100,1)} %",set_colour(RED,WHITE))
+            self.screen.addstr(ydraw+3,self.mx-7,f"{round(self.value/self.max*100,1)} %",set_colour(RED,WHITE))
         if self.sl:
             rectangle(self.screen,4,0,self.my-2,self.mx-1)
             if len(self.loglist) > lheight:
                 lx = 0
                 for val in self.loglist[len(self.loglist)-lheight:]:
                     self.screen.addstr(lx+5,1,val[0:self.mx-2],self.lclist[len(self.loglist)-lheight+lx])
                     lx += 1
```

### Comparing `cursesplus-2.1/src/cursesplus/filedialog.py` & `cursesplus-2.2.0/src/cursesplus/filedialog.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.1/src/cursesplus/messagebox.py` & `cursesplus-2.2.0/src/cursesplus/messagebox.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.1/src/cursesplus.egg-info/PKG-INFO` & `cursesplus-2.2.0/src/cursesplus.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cursesplus
-Version: 2.1
+Version: 2.2.0
 Summary: An extension program to curses that offers option menus, message boxes, file dialogs and more
 Author-email: Enderbyte Programs <enderbyte09@gmail.com>
 Project-URL: Homepage, https://github.com/Enderbyte-Programs/Curses-Plus
 Project-URL: Bug Tracker, https://github.com/Enderbyte-Programs/Curses-Plus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,14 +23,24 @@
 ### SPECIAL INSTRUCTIONS FOR WINDOWS
 
 For Windows you need to also install ```windows-curses``` or related program
 to provide the basic curses functionality
 
 ## What's New?
 
+### Version 2.2: Progressbar
+
+-Add ProgressBarTypes enum-class
+
+-Add ProgressBarLocation enum-class
+
+-You can now have a small progress bar that does not clear the screen
+
+-displaymsg() will no longer clear itself.
+
 ### Version 2.1: Files 'n' Folders
 
 -Add openfolderdialog()
 
 -Change colours
 
 -Performance improvements for all methods
```

