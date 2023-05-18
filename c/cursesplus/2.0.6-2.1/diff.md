# Comparing `tmp/cursesplus-2.0.6.tar.gz` & `tmp/cursesplus-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cursesplus-2.0.6.tar", last modified: Sun May  7 14:59:44 2023, max compression
+gzip compressed data, was "cursesplus-2.1.tar", last modified: Thu May 18 14:48:04 2023, max compression
```

## Comparing `cursesplus-2.0.6.tar` & `cursesplus-2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-07 14:59:44.654817 cursesplus-2.0.6/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1089 2023-04-07 16:31:31.000000 cursesplus-2.0.6/LICENSE
--rw-r--r--   0 jordan    (1000) jordan    (1000)     1667 2023-05-07 14:59:44.654817 cursesplus-2.0.6/PKG-INFO
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1064 2023-05-07 14:40:15.000000 cursesplus-2.0.6/README.md
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      659 2023-05-07 14:52:44.000000 cursesplus-2.0.6/pyproject.toml
--rw-r--r--   0 jordan    (1000) jordan    (1000)       38 2023-05-07 14:59:44.654817 cursesplus-2.0.6/setup.cfg
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-07 14:59:44.654817 cursesplus-2.0.6/src/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      283 2023-05-06 21:59:53.000000 cursesplus-2.0.6/src/__cptest.py
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-07 14:59:44.654817 cursesplus-2.0.6/src/cursesplus/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      892 2023-04-07 16:31:31.000000 cursesplus-2.0.6/src/cursesplus/__init__.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)    11516 2023-04-07 16:31:31.000000 cursesplus-2.0.6/src/cursesplus/cp.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)    13264 2023-05-07 14:59:27.000000 cursesplus-2.0.6/src/cursesplus/filedialog.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     5980 2023-04-14 17:54:57.000000 cursesplus-2.0.6/src/cursesplus/messagebox.py
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-07 14:59:44.654817 cursesplus-2.0.6/src/cursesplus.egg-info/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1667 2023-05-07 14:59:44.000000 cursesplus-2.0.6/src/cursesplus.egg-info/PKG-INFO
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      306 2023-05-07 14:59:44.000000 cursesplus-2.0.6/src/cursesplus.egg-info/SOURCES.txt
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)        1 2023-05-07 14:59:44.000000 cursesplus-2.0.6/src/cursesplus.egg-info/dependency_links.txt
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)       20 2023-05-07 14:59:44.000000 cursesplus-2.0.6/src/cursesplus.egg-info/top_level.txt
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-18 14:48:04.831158 cursesplus-2.1/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1089 2023-04-07 16:31:31.000000 cursesplus-2.1/LICENSE
+-rw-r--r--   0 jordan    (1000) jordan    (1000)     1442 2023-05-18 14:48:04.831158 cursesplus-2.1/PKG-INFO
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      841 2023-05-18 14:47:48.000000 cursesplus-2.1/README.md
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      657 2023-05-18 14:46:14.000000 cursesplus-2.1/pyproject.toml
+-rw-r--r--   0 jordan    (1000) jordan    (1000)       38 2023-05-18 14:48:04.831158 cursesplus-2.1/setup.cfg
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-18 14:48:04.831158 cursesplus-2.1/src/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      288 2023-05-18 14:35:12.000000 cursesplus-2.1/src/__cptest.py
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-18 14:48:04.831158 cursesplus-2.1/src/cursesplus/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      892 2023-04-07 16:31:31.000000 cursesplus-2.1/src/cursesplus/__init__.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)    11516 2023-04-07 16:31:31.000000 cursesplus-2.1/src/cursesplus/cp.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)    18476 2023-05-18 14:43:10.000000 cursesplus-2.1/src/cursesplus/filedialog.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     5980 2023-04-14 17:54:57.000000 cursesplus-2.1/src/cursesplus/messagebox.py
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-18 14:48:04.831158 cursesplus-2.1/src/cursesplus.egg-info/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1442 2023-05-18 14:48:04.000000 cursesplus-2.1/src/cursesplus.egg-info/PKG-INFO
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      306 2023-05-18 14:48:04.000000 cursesplus-2.1/src/cursesplus.egg-info/SOURCES.txt
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)        1 2023-05-18 14:48:04.000000 cursesplus-2.1/src/cursesplus.egg-info/dependency_links.txt
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)       20 2023-05-18 14:48:04.000000 cursesplus-2.1/src/cursesplus.egg-info/top_level.txt
```

### Comparing `cursesplus-2.0.6/LICENSE` & `cursesplus-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cursesplus-2.0.6/PKG-INFO` & `cursesplus-2.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cursesplus
-Version: 2.0.6
+Version: 2.1
 Summary: An extension program to curses that offers option menus, message boxes, file dialogs and more
 Author-email: Enderbyte Programs <enderbyte09@gmail.com>
 Project-URL: Homepage, https://github.com/Enderbyte-Programs/Curses-Plus
 Project-URL: Bug Tracker, https://github.com/Enderbyte-Programs/Curses-Plus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,39 +21,32 @@
 on Windows
 
 ### SPECIAL INSTRUCTIONS FOR WINDOWS
 
 For Windows you need to also install ```windows-curses``` or related program
 to provide the basic curses functionality
 
-### System requirements
-
-**A computer running any of the following OSes:**
-
-Microsoft Windows 7
-Microsoft Windows 8
-Microsoft Windows 8.1
-Microsoft Windows 10
-Microsoft Windows 11
-Any modern distro of Linux that supports Python3
-
-**Python Version 3.6 or newer**
-
 ## What's New?
 
-### Version 2.0.5
+### Version 2.1: Files 'n' Folders
 
-Fix small bug in Manjaro Konsole
+-Add openfolderdialog()
 
-### Version 2.0.4
+-Change colours
 
-More features added to filedialog
+-Performance improvements for all methods
 
 ### Version 2.0: Incompatible api changes
 
 -askyesno now MUST be messagebox.askyesno
+
 -Rewrite colour system. load_colours() is now nonexistent.
+
 -Now use set_colour(background,foreground). A set of colour constants are defined in the cp class.
 
 ## Uses
 
 curses-plus offers many utilities to make writing TUI applications easy. (TUI stands for Terminal User Interface)
+
+## Documentation
+
+TODO
```

### Comparing `cursesplus-2.0.6/README.md` & `cursesplus-2.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -7,39 +7,32 @@
 on Windows
 
 ### SPECIAL INSTRUCTIONS FOR WINDOWS
 
 For Windows you need to also install ```windows-curses``` or related program
 to provide the basic curses functionality
 
-### System requirements
-
-**A computer running any of the following OSes:**
-
-Microsoft Windows 7
-Microsoft Windows 8
-Microsoft Windows 8.1
-Microsoft Windows 10
-Microsoft Windows 11
-Any modern distro of Linux that supports Python3
-
-**Python Version 3.6 or newer**
-
 ## What's New?
 
-### Version 2.0.5
+### Version 2.1: Files 'n' Folders
 
-Fix small bug in Manjaro Konsole
+-Add openfolderdialog()
 
-### Version 2.0.4
+-Change colours
 
-More features added to filedialog
+-Performance improvements for all methods
 
 ### Version 2.0: Incompatible api changes
 
 -askyesno now MUST be messagebox.askyesno
+
 -Rewrite colour system. load_colours() is now nonexistent.
+
 -Now use set_colour(background,foreground). A set of colour constants are defined in the cp class.
 
 ## Uses
 
-curses-plus offers many utilities to make writing TUI applications easy. (TUI stands for Terminal User Interface)
+curses-plus offers many utilities to make writing TUI applications easy. (TUI stands for Terminal User Interface)
+
+## Documentation
+
+TODO
```

### Comparing `cursesplus-2.0.6/pyproject.toml` & `cursesplus-2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "cursesplus"
-version = "2.0.6"
+version = "2.1"
 authors = [{name="Enderbyte Programs",email="enderbyte09@gmail.com"},]
 description = "An extension program to curses that offers option menus, message boxes, file dialogs and more"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
```

### Comparing `cursesplus-2.0.6/src/cursesplus/__init__.py` & `cursesplus-2.1/src/cursesplus/__init__.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.0.6/src/cursesplus/cp.py` & `cursesplus-2.1/src/cursesplus/cp.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.0.6/src/cursesplus/filedialog.py` & `cursesplus-2.1/src/cursesplus/filedialog.py`

 * *Files 13% similar despite different names*

```diff
@@ -138,23 +138,25 @@
             refresh = True
         elif ch == cp.curses.KEY_ENTER or ch == 10 or ch == 13:
             if masterlist[selected].isdir:
                 directory = masterlist[selected].path
                 selected = 0
                 refresh = True
                 yoffset = 0
+                directory = directory.replace("//","/")
             else:
                 return masterlist[selected].path
         elif ch == cp.curses.KEY_SLEFT or ch == 98:
             directory = "/".join(directory.split("/")[0:-1])
             selected = 0
             yoffset = 0
             refresh = True
             if directory == "":
                 directory = "/"
+            directory = directory.replace("//","/")
         elif ch == 114:
             refresh = True#Refresh files list
         elif ch == 108:
             npath = cp.cursesinput(stdscr,"Please enter new path").replace("\n","")
             if os.path.isdir(npath):
                 directory = npath
                 selected = 0
@@ -163,14 +165,130 @@
             else:
                 messagebox.showwarning(stdscr,["Path does not exist"])
         elif ch == 104:
             cp.displaymsg(stdscr,["List of Keybinds","Down Arrow: Scroll down","Up Arrow: Scroll up","Left Arrow: Scroll left","Right Arrow: Scroll right","Shift-left arrow: Move up to parent Directory","Enter: Open/select","F: Change filter","L: Change location"])
 
         #masterlist.clear()
 
+def openfolderdialog(stdscr,title: str = "Please choose a folder",directory: str = os.getcwd()) -> str:
+    """Start a filedialog to open a file. title is the prompt the use recieves. filter is the file filter. The filter syntax is the same as TK syntax. The first
+    filter provided is the main filter. 
+    Filter Syntax: 
+    [[GLOB,NAME],[GLOB,NAME]]
+    Glob is a pattern to match for files (like *.txt)
+    Name is a file type like (Text Files)
+    
+    directory is the directory that the dialog opens to
+
+    RETURNS the full file path chosen
+    """
+    xoffset: int = 0
+    yoffset: int = 0
+    selected: int = 0
+    refresh: bool = False
+    masterlist: list = list[Fileobj]
+    directories = [directory+"/"+l for l in os.listdir(directory) if os.path.isdir(directory+"/"+l)]
+    directories.sort()
+    #displaymsg(stdscr,directories+files)
+    masterlist = [Fileobj(f) for f in directories]
+    while True:
+        
+        mx,my = os.get_terminal_size()
+        MAXNL = mx - 33
+        stdscr.clear()
+        cp.rectangle(stdscr,2,0,my-2,mx-1)
+        cp.filline(stdscr,0,cp.set_color(cp.BLUE,cp.WHITE))
+        cp.filline(stdscr,1,cp.set_color(cp.GREEN,cp.WHITE))
+        cp.filline(stdscr,my-2,cp.set_color(cp.WHITE,cp.BLACK))
+        cp.filline(stdscr,my-1,cp.set_color(cp.RED,cp.WHITE))
+        topline = "Name"+" "*(MAXNL-4)+"|"+"Size     "+"|Date Modified"
+        topline = topline+(mx-2-len(topline))*" "
+        if refresh:
+            masterlist: list = list[Fileobj]
+            directories = [directory+"/"+l for l in os.listdir(directory) if os.path.isdir(directory+"/"+l)]
+            directories.sort()
+            masterlist = [Fileobj(f) for f in directories]
+        stdscr.addstr(0,0,title+"|H for Help|Press Shift-Left Arrow to move up directory"[0:mx],cp.set_colour(cp.BLUE,cp.WHITE))
+        stdscr.addstr(1,0,directory[xoffset:xoffset+mx],cp.set_colour(cp.GREEN,cp.WHITE))
+        stdscr.addstr(my-2,0,f"[{len(masterlist)} objects found]"[0:mx],cp.set_colour(cp.WHITE,cp.BLACK))
+        stdscr.addstr(2,1,topline[0:mx-1])
+        
+        try:
+            stdscr.addstr(my-1,0,masterlist[selected].path[xoffset:xoffset+mx],cp.set_colour(cp.RED,cp.WHITE))
+        except:
+            pass
+        ind = yoffset#Track position in list
+        indx = 0#track position in iter
+        for fileobjects in masterlist[yoffset:yoffset+my-5]:
+            wstr = fileobjects.strippedpath[xoffset:xoffset+MAXNL]
+            wstr += " "*(MAXNL-len(wstr)+1)
+            wstr += fileobjects.sizestr
+            wstr += " "*(10-len(fileobjects.sizestr))
+            wstr += fileobjects.date
+            if selected == ind:
+                stdscr.addstr(3+indx,1,wstr,cp.set_colour(cp.BLACK,cp.GREEN))
+            elif fileobjects.isdir:
+                stdscr.addstr(3+indx,1,wstr,cp.set_colour(cp.BLACK,cp.YELLOW))
+            else:
+                stdscr.addstr(3+indx,1,wstr)
+            ind += 1
+            indx += 1#Inc both
+
+        
+        stdscr.refresh()
+        ch = stdscr.getch()
+        refresh = False
+        if ch == cp.curses.KEY_LEFT and xoffset > 0:
+            xoffset -= 1
+        elif ch == cp.curses.KEY_RIGHT:
+            xoffset += 1
+        elif ch == cp.curses.KEY_UP and selected > 0:
+            selected -= 1
+            if selected < yoffset:
+                yoffset -= 1
+        elif ch == cp.curses.KEY_DOWN and selected < len(masterlist)-1:
+            if selected - yoffset > my - 7:
+                yoffset += 1
+            selected += 1
+        elif ch == cp.curses.KEY_ENTER or ch == 10 or ch == 13:
+            if masterlist[selected].isdir:
+                directory = masterlist[selected].path
+                selected = 0
+                refresh = True
+                yoffset = 0
+                directory = directory.replace("//","/")
+            else:
+                return masterlist[selected].path
+        elif ch == 115:
+            return masterlist[selected].path
+        elif ch == cp.curses.KEY_SLEFT or ch == 98:
+            directory = "/".join(directory.split("/")[0:-1])
+            selected = 0
+            yoffset = 0
+            refresh = True
+            if directory == "":
+                directory = "/"
+            
+            directory = directory.replace("//","/")
+        elif ch == 114:
+            refresh = True#Refresh files list
+        elif ch == 108:
+            npath = cp.cursesinput(stdscr,"Please enter new path").replace("\n","")
+            if os.path.isdir(npath):
+                directory = npath
+                selected = 0
+                yoffset = 0
+                refresh = True
+            else:
+                messagebox.showwarning(stdscr,["Path does not exist"])
+        elif ch == 104:
+            cp.displaymsg(stdscr,["List of Keybinds","Down Arrow: Scroll down","Up Arrow: Scroll up","Left Arrow: Scroll left","Right Arrow: Scroll right","Shift-left arrow: Move up to parent Directory","Enter: Open","S: Choose folder","L: Change location"])
+
+        #masterlist.clear()
+
 def openfilesdialog(stdscr,title: str = "Please choose a file",filter: str = [["*","All Files"]],directory: str = os.getcwd()) -> list:
     """Start a filedialog to select multiple files. title is the prompt the user recieves. filter is the file filter. The filter syntax is the same as TK syntax. The first
     filter provided is the main filter. 
     Filter Syntax: 
     [[GLOB,NAME],[GLOB,NAME]]
     Glob is a pattern to match for files (like *.txt)
     Name is a file type like (Text Files)
@@ -265,14 +383,15 @@
             update = True
         elif ch == cp.curses.KEY_ENTER or ch == 10 or ch == 13:
             if masterlist[selected].isdir:
                 directory = masterlist[selected].path
                 selected = 0
                 yoffset = 0
                 update = True
+                directory = directory.replace("//","/")
             else:
                 chosen.clear()
                 chosen.append(masterlist[selected].path)
         elif ch == 115:
             #s for add to selection
             if not masterlist[selected].isdir:
                 if masterlist[selected].path in chosen:
@@ -282,14 +401,15 @@
         elif ch == cp.curses.KEY_SLEFT or ch == 98:
             directory = "/".join(directory.split("/")[0:-1])
             selected = 0
             yoffset = 0
             update = True
             if directory == "":
                 directory = "/"
+            directory = directory.replace("//","/")
         elif ch == 114:
             update = True#Refresh files list
         elif ch == 100 or cp.curses.keyname(ch).decode() == "^X":
             return [c for c in chosen if os.path.isfile(c) and c.replace(" ","") != ""]#Only return files that still exist
         elif ch == 99:
             chosen.clear()
         elif ch == 108:
```

### Comparing `cursesplus-2.0.6/src/cursesplus/messagebox.py` & `cursesplus-2.1/src/cursesplus/messagebox.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.0.6/src/cursesplus.egg-info/PKG-INFO` & `cursesplus-2.1/src/cursesplus.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cursesplus
-Version: 2.0.6
+Version: 2.1
 Summary: An extension program to curses that offers option menus, message boxes, file dialogs and more
 Author-email: Enderbyte Programs <enderbyte09@gmail.com>
 Project-URL: Homepage, https://github.com/Enderbyte-Programs/Curses-Plus
 Project-URL: Bug Tracker, https://github.com/Enderbyte-Programs/Curses-Plus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,39 +21,32 @@
 on Windows
 
 ### SPECIAL INSTRUCTIONS FOR WINDOWS
 
 For Windows you need to also install ```windows-curses``` or related program
 to provide the basic curses functionality
 
-### System requirements
-
-**A computer running any of the following OSes:**
-
-Microsoft Windows 7
-Microsoft Windows 8
-Microsoft Windows 8.1
-Microsoft Windows 10
-Microsoft Windows 11
-Any modern distro of Linux that supports Python3
-
-**Python Version 3.6 or newer**
-
 ## What's New?
 
-### Version 2.0.5
+### Version 2.1: Files 'n' Folders
 
-Fix small bug in Manjaro Konsole
+-Add openfolderdialog()
 
-### Version 2.0.4
+-Change colours
 
-More features added to filedialog
+-Performance improvements for all methods
 
 ### Version 2.0: Incompatible api changes
 
 -askyesno now MUST be messagebox.askyesno
+
 -Rewrite colour system. load_colours() is now nonexistent.
+
 -Now use set_colour(background,foreground). A set of colour constants are defined in the cp class.
 
 ## Uses
 
 curses-plus offers many utilities to make writing TUI applications easy. (TUI stands for Terminal User Interface)
+
+## Documentation
+
+TODO
```

