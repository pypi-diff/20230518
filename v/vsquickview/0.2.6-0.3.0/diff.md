# Comparing `tmp/vsquickview-0.2.6.tar.gz` & `tmp/vsquickview-0.3.0.tar.gz`

## Comparing `vsquickview-0.2.6.tar` & `vsquickview-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 vsquickview-0.2.6/vsquickview/__init__.py
--rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 vsquickview-0.2.6/vsquickview/colourbars.py
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 vsquickview-0.2.6/vsquickview/fakevsquickview.py
--rw-r--r--   0        0        0    14624 2020-02-02 00:00:00.000000 vsquickview-0.2.6/vsquickview/vsquickview.py
--rw-r--r--   0        0        0    14341 2020-02-02 00:00:00.000000 vsquickview-0.2.6/vsquickview/vsquickview.qml
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 vsquickview-0.2.6/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 vsquickview-0.2.6/LICENSE
--rw-r--r--   0        0        0     5919 2020-02-02 00:00:00.000000 vsquickview-0.2.6/README.md
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 vsquickview-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     6772 2020-02-02 00:00:00.000000 vsquickview-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 vsquickview-0.3.0/vsquickview/__init__.py
+-rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 vsquickview-0.3.0/vsquickview/colourbars.py
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 vsquickview-0.3.0/vsquickview/fakevsquickview.py
+-rw-r--r--   0        0        0    14624 2020-02-02 00:00:00.000000 vsquickview-0.3.0/vsquickview/vsquickview.py
+-rw-r--r--   0        0        0    14341 2020-02-02 00:00:00.000000 vsquickview-0.3.0/vsquickview/vsquickview.qml
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 vsquickview-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 vsquickview-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5919 2020-02-02 00:00:00.000000 vsquickview-0.3.0/README.md
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 vsquickview-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6772 2020-02-02 00:00:00.000000 vsquickview-0.3.0/PKG-INFO
```

### Comparing `vsquickview-0.2.6/vsquickview/__init__.py` & `vsquickview-0.3.0/vsquickview/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,8 +41,8 @@
                                  SetIndex, \
                                  SetPreviewGroup, \
                                  ClearPreviewGroup, \
                                  PreviewGroup, \
                                  Show, \
                                  Hide
 
-__version__ = "0.2.6"
+__version__ = "0.3.0"
```

### Comparing `vsquickview-0.2.6/vsquickview/colourbars.py` & `vsquickview-0.3.0/vsquickview/colourbars.py`

 * *Files identical despite different names*

### Comparing `vsquickview-0.2.6/vsquickview/fakevsquickview.py` & `vsquickview-0.3.0/vsquickview/fakevsquickview.py`

 * *Files identical despite different names*

### Comparing `vsquickview-0.2.6/vsquickview/vsquickview.py` & `vsquickview-0.3.0/vsquickview/vsquickview.py`

 * *Files identical despite different names*

### Comparing `vsquickview-0.2.6/vsquickview/vsquickview.qml` & `vsquickview-0.3.0/vsquickview/vsquickview.qml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -278,29 +278,29 @@
                 if(event.modifiers === Qt.AltModifier) {
                     altPressed = true
                 }
             }
 
             else if(event.key === Qt.Key_Right) {
                 if(event.modifiers === Qt.ShiftModifier) {
-                    backend.nextPreviewGroupFrame()
+                    backend.nextTwelveFrames()
                 }
                 else if(event.modifiers === Qt.ControlModifier) {
-                    backend.nextTwelveFrames()
+                    backend.nextPreviewGroupFrame()
                 }
                 else {
                     backend.nextFrame()
                 }
             }
             else if(event.key === Qt.Key_Left) {
                 if(event.modifiers === Qt.ShiftModifier) {
-                    backend.prevPreviewGroupFrame()
+                    backend.prevTwelveFrames()
                 }
                 else if(event.modifiers === Qt.ControlModifier) {
-                    backend.prevTwelveFrames()
+                    backend.prevPreviewGroupFrame()
                 }
                 else {
                     backend.prevFrame()
                 }
             }
 
             else if(event.key === Qt.Key_G) {
```

### Comparing `vsquickview-0.2.6/LICENSE` & `vsquickview-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vsquickview-0.2.6/README.md` & `vsquickview-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `vsquickview-0.2.6/pyproject.toml` & `vsquickview-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vsquickview-0.2.6/PKG-INFO` & `vsquickview-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsquickview
-Version: 0.2.6
+Version: 0.3.0
 Summary: VapourSynth preview script
 Project-URL: Documentation, https://github.com/Akatmks/vsquickview
 Project-URL: Issues, https://github.com/Akatmks/vsquickview/issues
 Project-URL: Source, https://github.com/Akatmks/vsquickview
 Author-email: Akatsumekusa <Akatsumekusa@protonmail.com>
 License-Expression: MIT
 License-File: LICENSE
```

