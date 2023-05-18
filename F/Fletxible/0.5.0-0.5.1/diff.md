# Comparing `tmp/Fletxible-0.5.0.tar.gz` & `tmp/Fletxible-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fletxible-0.5.0.tar", last modified: Wed May 17 16:18:12 2023, max compression
+gzip compressed data, was "Fletxible-0.5.1.tar", last modified: Thu May 18 15:53:22 2023, max compression
```

## Comparing `Fletxible-0.5.0.tar` & `Fletxible-0.5.1.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-17 16:18:12.601059 Fletxible-0.5.0/
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-17 16:18:12.597604 Fletxible-0.5.0/Fletxible.egg-info/
--rw-r--r--   0 ahmad      (501) staff       (20)      830 2023-05-17 16:18:12.000000 Fletxible-0.5.0/Fletxible.egg-info/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)      360 2023-05-17 16:18:12.000000 Fletxible-0.5.0/Fletxible.egg-info/SOURCES.txt
--rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-05-17 16:18:12.000000 Fletxible-0.5.0/Fletxible.egg-info/dependency_links.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       50 2023-05-17 16:18:12.000000 Fletxible-0.5.0/Fletxible.egg-info/entry_points.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       37 2023-05-17 16:18:12.000000 Fletxible-0.5.0/Fletxible.egg-info/requires.txt
--rw-r--r--   0 ahmad      (501) staff       (20)        6 2023-05-17 16:18:12.000000 Fletxible-0.5.0/Fletxible.egg-info/top_level.txt
--rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-04-29 15:25:05.000000 Fletxible-0.5.0/LICENSE
--rw-r--r--   0 ahmad      (501) staff       (20)      830 2023-05-17 16:18:12.600829 Fletxible-0.5.0/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)     4106 2023-05-01 16:06:19.000000 Fletxible-0.5.0/README.md
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-17 16:18:12.599946 Fletxible-0.5.0/logic/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-01 13:39:08.000000 Fletxible-0.5.0/logic/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     2251 2023-05-17 15:53:13.000000 Fletxible-0.5.0/logic/cli.py
--rw-r--r--   0 ahmad      (501) staff       (20)     7170 2023-05-17 15:50:13.000000 Fletxible-0.5.0/logic/controls.py
--rw-r--r--   0 ahmad      (501) staff       (20)      868 2023-05-17 15:48:21.000000 Fletxible-0.5.0/logic/main.py
--rw-r--r--   0 ahmad      (501) staff       (20)     6505 2023-05-16 19:07:50.000000 Fletxible-0.5.0/logic/script.py
--rw-r--r--   0 ahmad      (501) staff       (20)      908 2023-05-17 15:50:39.000000 Fletxible-0.5.0/logic/styles.py
--rw-r--r--   0 ahmad      (501) staff       (20)     4736 2023-05-17 15:57:08.000000 Fletxible-0.5.0/logic/utilities.py
--rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-05-17 16:18:12.601127 Fletxible-0.5.0/setup.cfg
--rw-r--r--   0 ahmad      (501) staff       (20)     1110 2023-05-17 16:17:33.000000 Fletxible-0.5.0/setup.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-17 16:18:12.600378 Fletxible-0.5.0/tests/
--rw-r--r--   0 ahmad      (501) staff       (20)        5 2023-05-01 14:25:50.000000 Fletxible-0.5.0/tests/test_route.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-18 15:53:22.880722 Fletxible-0.5.1/
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-18 15:53:22.875948 Fletxible-0.5.1/Fletxible.egg-info/
+-rw-r--r--   0 ahmad      (501) staff       (20)      830 2023-05-18 15:53:22.000000 Fletxible-0.5.1/Fletxible.egg-info/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)      391 2023-05-18 15:53:22.000000 Fletxible-0.5.1/Fletxible.egg-info/SOURCES.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-05-18 15:53:22.000000 Fletxible-0.5.1/Fletxible.egg-info/dependency_links.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       50 2023-05-18 15:53:22.000000 Fletxible-0.5.1/Fletxible.egg-info/entry_points.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       37 2023-05-18 15:53:22.000000 Fletxible-0.5.1/Fletxible.egg-info/requires.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)        6 2023-05-18 15:53:22.000000 Fletxible-0.5.1/Fletxible.egg-info/top_level.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-04-29 15:25:05.000000 Fletxible-0.5.1/LICENSE
+-rw-r--r--   0 ahmad      (501) staff       (20)      830 2023-05-18 15:53:22.880470 Fletxible-0.5.1/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)     4106 2023-05-01 16:06:19.000000 Fletxible-0.5.1/README.md
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-18 15:53:22.879326 Fletxible-0.5.1/logic/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-01 13:39:08.000000 Fletxible-0.5.1/logic/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     2251 2023-05-17 15:53:13.000000 Fletxible-0.5.1/logic/cli.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     7170 2023-05-17 15:50:13.000000 Fletxible-0.5.1/logic/controls.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      891 2023-05-18 14:26:31.000000 Fletxible-0.5.1/logic/main.py
+-rw-r--r--   0 ahmad      (501) staff       (20)       68 2023-05-18 15:36:10.000000 Fletxible-0.5.1/logic/mapped.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      335 2023-05-18 15:36:10.000000 Fletxible-0.5.1/logic/route.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     6505 2023-05-16 19:07:50.000000 Fletxible-0.5.1/logic/script.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      908 2023-05-17 15:50:39.000000 Fletxible-0.5.1/logic/styles.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     5929 2023-05-18 15:36:06.000000 Fletxible-0.5.1/logic/utilities.py
+-rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-05-18 15:53:22.880794 Fletxible-0.5.1/setup.cfg
+-rw-r--r--   0 ahmad      (501) staff       (20)     1110 2023-05-18 15:52:37.000000 Fletxible-0.5.1/setup.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-18 15:53:22.879823 Fletxible-0.5.1/tests/
+-rw-r--r--   0 ahmad      (501) staff       (20)        5 2023-05-01 14:25:50.000000 Fletxible-0.5.1/tests/test_route.py
```

### Comparing `Fletxible-0.5.0/Fletxible.egg-info/PKG-INFO` & `Fletxible-0.5.1/Fletxible.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fletxible
-Version: 0.5.0
+Version: 0.5.1
 Summary: Web Boilerplate for Flet Library
 Home-page: https://github.com/LineIndent/fletxible
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 Keywords: python web template,web application,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Fletxible-0.5.0/LICENSE` & `Fletxible-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.0/PKG-INFO` & `Fletxible-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fletxible
-Version: 0.5.0
+Version: 0.5.1
 Summary: Web Boilerplate for Flet Library
 Home-page: https://github.com/LineIndent/fletxible
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 Keywords: python web template,web application,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Fletxible-0.5.0/README.md` & `Fletxible-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.0/logic/cli.py` & `Fletxible-0.5.1/logic/cli.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.0/logic/controls.py` & `Fletxible-0.5.1/logic/controls.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.0/logic/main.py` & `Fletxible-0.5.1/logic/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,12 +26,13 @@
 
         else:
             for nav in page.views[-1].controls[:]:
                 nav.content.show_navigation()
 
     # Page events ...
     page.on_resize = resize_event
+    resize_event(None)
     page.update()
 
 
 if __name__ == "__main__":
     ft.flet.app(target=main)
```

### Comparing `Fletxible-0.5.0/logic/script.py` & `Fletxible-0.5.1/logic/script.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.0/logic/styles.py` & `Fletxible-0.5.1/logic/styles.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.0/logic/utilities.py` & `Fletxible-0.5.1/logic/utilities.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     for file in os.listdir("pages"):
         # Set the path of the file to loop over folders and only include files
         path = os.path.join("pages", file)
 
         # If the path is NOT a folder, continue ...
         if not os.path.isdir(path):
             filename = os.path.splitext(file)[0]
-            string = f"ft.Text(size=13, weight='bold', spans=[ft.TextSpan('{filename}', on_click=lambda e: route(e, '/{filename}'))]),"
+            string = f"ft.Text(size=13, weight='bold', spans=[ft.TextSpan('{filename.capitalize()}', on_click=lambda e: route(e, '/{filename}'))]),"
             route_list.append(string)
 
     return route_list
 
 
 def set_app_route_method():
     string = """from script import route_keys
@@ -43,14 +43,24 @@
         #
         self.stack = ft.Stack(expand=True)
 
         #
         self.row = ft.Row(expand=True, spacing=2)
 
         #
+        self.drawer = ft.Container(
+            expand=True,
+            width=0,
+            bgcolor="#23262d",
+            animate=ft.Animation(550, "ease"),
+            content=ft.Column(expand=True),
+            shadow=None,
+        )
+        
+        #
         self.left_panel = ft.Container(
             expand=1,
             padding=ft.padding.only(top=65),
             content=ft.Column(
                 expand=True,
                 alignment="start",
                 controls=[],
@@ -88,22 +98,24 @@
                 
                 # end #
             ],
         )
 
         #
         self.nav_mobile = ft.IconButton(
-            icon=ft.icons.MENU_SHARP, visible=False, icon_size=14, icon_color="white"
+            icon=ft.icons.MENU_SHARP, visible=False, icon_size=14, icon_color="white",
+            on_click=lambda e: self.show_drawer(e),
+
         )
 
         #
         self.header = ft.Container(
             bgcolor="#34373e",
             height=60,
-            padding=ft.padding.only(left=20, right=20),
+            padding=ft.padding.only(left=60, right=60),
             shadow=ft.BoxShadow(
                 spread_radius=2,
                 blur_radius=4,
                 color=ft.colors.with_opacity(0.25, "black"),
                 offset=ft.Offset(2, 2),
             ),
             content=ft.Row(
@@ -116,38 +128,70 @@
                     self.nav,
                     self.nav_mobile,
                 ],
             ),
         )
         super().__init__()
 
+    def show_drawer(self, e):
+        if self.drawer.width != 220:
+            self.drawer.width = 220
+            self.drawer.shadow = ft.BoxShadow(
+                blur_radius=15,
+                spread_radius=8,
+                color=ft.colors.with_opacity(0.25, "black"),
+                offset=(4, 4),
+            )
+
+        else:
+            self.drawer.width = 0
+            self.drawer.shadow = None
+
+        self.drawer.update()
+
     def hide_navigation(self):
         self.nav.visible = False
         self.nav.update()
+        
+        self.left_panel.visible = False
+        self.left_panel.update()
+
+        self.right_panel.visible = False
+        self.right_panel.update()
 
         self.nav_mobile.visible = True
         self.nav_mobile.update()
 
     def show_navigation(self):
+        self.drawer.width = 0
+        self.drawer.shadow = None
+        self.drawer.update()
+        
         self.nav.visible = True
         self.nav.update()
+        
+        self.left_panel.visible = True
+        self.left_panel.update()
+
+        self.right_panel.visible = True
+        self.right_panel.update()
 
         self.nav_mobile.visible = False
         self.nav_mobile.update()
 
     def build(self):
         #
         self.row.controls = [
             self.left_panel,
             self.middle_panel,
             self.right_panel,
         ]
 
         #
-        self.stack.controls = [self.row, self.header]
+        self.stack.controls = [self.row, self.header, self.drawer]
 
         #
         return self.stack
 
 
 class View(ft.View):
     def __init__(
```

### Comparing `Fletxible-0.5.0/setup.py` & `Fletxible-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="Fletxible",
-    version="0.5.0",
+    version="0.5.1",
     author="S. Ahmad P. Hakimi",
     author_email="pourhakimi@pm.me",
     description="Web Boilerplate for Flet Library",
     long_description="Fletxible is a Python web boilerplate project designed to provide a solid foundation for building web applications with Python and Flet. The project comes pre-configured with a range of tools and features to make it easy for developers to get started building their applications, without the need to spend time setting up infrastructure or configuring tools.",
     long_description_content_type="text/markdown",
     url="https://github.com/LineIndent/fletxible",
     packages=["logic"],
```

