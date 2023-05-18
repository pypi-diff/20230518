# Comparing `tmp/ntvHaber-1.10.tar.gz` & `tmp/ntvHaber-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntvHaber-1.10.tar", last modified: Sun Jan 22 12:51:49 2023, max compression
+gzip compressed data, was "ntvHaber-1.30.0.tar", last modified: Thu May 18 16:21:50 2023, max compression
```

## Comparing `ntvHaber-1.10.tar` & `ntvHaber-1.30.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 12:51:49.857266 ntvHaber-1.10/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-22 12:51:28.000000 ntvHaber-1.10/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-22 12:51:28.000000 ntvHaber-1.10/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-01-22 12:51:49.857266 ntvHaber-1.10/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-01-22 12:51:28.000000 ntvHaber-1.10/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 12:51:49.853266 ntvHaber-1.10/ntvHaber/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 12:51:49.853266 ntvHaber-1.10/ntvHaber/Assets/
--rw-r--r--   0 runner    (1001) docker     (123)    12254 2023-01-22 12:51:28.000000 ntvHaber-1.10/ntvHaber/Assets/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-01-22 12:51:28.000000 ntvHaber-1.10/ntvHaber/Assets/Logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-01-22 12:51:28.000000 ntvHaber-1.10/ntvHaber/Assets/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-01-22 12:51:28.000000 ntvHaber-1.10/ntvHaber/Assets/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 12:51:49.857266 ntvHaber-1.10/ntvHaber/Assets/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-01-22 12:51:28.000000 ntvHaber-1.10/ntvHaber/Assets/icons/apple-touch-icon-192.png
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-01-22 12:51:28.000000 ntvHaber-1.10/ntvHaber/Assets/icons/icon-192.png
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-01-22 12:51:28.000000 ntvHaber-1.10/ntvHaber/Assets/icons/icon-512.png
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-01-22 12:51:28.000000 ntvHaber-1.10/ntvHaber/Assets/icons/icon-maskable-192.png
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-01-22 12:51:28.000000 ntvHaber-1.10/ntvHaber/Assets/icons/icon-maskable-512.png
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-01-22 12:51:28.000000 ntvHaber-1.10/ntvHaber/Assets/icons/loading-animation.png
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-01-22 12:51:28.000000 ntvHaber-1.10/ntvHaber/Assets/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-01-22 12:51:28.000000 ntvHaber-1.10/ntvHaber/Assets/manifest.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 12:51:49.857266 ntvHaber-1.10/ntvHaber/CLI/
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-01-22 12:51:28.000000 ntvHaber-1.10/ntvHaber/CLI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 12:51:49.857266 ntvHaber-1.10/ntvHaber/Layouts/
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-01-22 12:51:28.000000 ntvHaber-1.10/ntvHaber/Layouts/Haberler.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-01-22 12:51:28.000000 ntvHaber-1.10/ntvHaber/Layouts/KekikFlet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-01-22 12:51:28.000000 ntvHaber-1.10/ntvHaber/Layouts/Panel.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-01-22 12:51:28.000000 ntvHaber-1.10/ntvHaber/Layouts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 12:51:49.857266 ntvHaber-1.10/ntvHaber/Libs/
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-01-22 12:51:28.000000 ntvHaber-1.10/ntvHaber/Libs/NTV.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-01-22 12:51:28.000000 ntvHaber-1.10/ntvHaber/Libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-01-22 12:51:28.000000 ntvHaber-1.10/ntvHaber/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-01-22 12:51:28.000000 ntvHaber-1.10/ntvHaber/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 12:51:49.853266 ntvHaber-1.10/ntvHaber.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-01-22 12:51:49.000000 ntvHaber-1.10/ntvHaber.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-01-22 12:51:49.000000 ntvHaber-1.10/ntvHaber.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-22 12:51:49.000000 ntvHaber-1.10/ntvHaber.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-01-22 12:51:49.000000 ntvHaber-1.10/ntvHaber.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-01-22 12:51:49.000000 ntvHaber-1.10/ntvHaber.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-22 12:51:49.000000 ntvHaber-1.10/ntvHaber.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-01-22 12:51:28.000000 ntvHaber-1.10/org.kekikakademi.ntvHaber.appdata.xml
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-01-22 12:51:28.000000 ntvHaber-1.10/org.kekikakademi.ntvHaber.desktop
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-22 12:51:49.857266 ntvHaber-1.10/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-01-22 12:51:28.000000 ntvHaber-1.10/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:21:50.338291 ntvHaber-1.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-05-18 16:21:50.338291 ntvHaber-1.30.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:21:50.334291 ntvHaber-1.30.0/Shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/Shared/org.kekikakademi.ntvHaber.appdata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/Shared/org.kekikakademi.ntvHaber.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/Shared/org.kekikakademi.ntvHaber.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:21:50.334291 ntvHaber-1.30.0/ntvHaber/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:21:50.338291 ntvHaber-1.30.0/ntvHaber/Assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    12254 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/ntvHaber/Assets/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/ntvHaber/Assets/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/ntvHaber/Assets/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:21:50.338291 ntvHaber-1.30.0/ntvHaber/Assets/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/ntvHaber/Assets/icons/apple-touch-icon-192.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/ntvHaber/Assets/icons/icon-192.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/ntvHaber/Assets/icons/icon-512.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/ntvHaber/Assets/icons/icon-maskable-192.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/ntvHaber/Assets/icons/icon-maskable-512.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/ntvHaber/Assets/icons/loading-animation.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/ntvHaber/Assets/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/ntvHaber/Assets/manifest.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:21:50.338291 ntvHaber-1.30.0/ntvHaber/CLI/
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/ntvHaber/CLI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:21:50.338291 ntvHaber-1.30.0/ntvHaber/Layouts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/ntvHaber/Layouts/Haberler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/ntvHaber/Layouts/KekikFlet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/ntvHaber/Layouts/Panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/ntvHaber/Layouts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:21:50.338291 ntvHaber-1.30.0/ntvHaber/Libs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/ntvHaber/Libs/NTV.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/ntvHaber/Libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/ntvHaber/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:21:50.338291 ntvHaber-1.30.0/ntvHaber.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-05-18 16:21:50.000000 ntvHaber-1.30.0/ntvHaber.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-18 16:21:50.000000 ntvHaber-1.30.0/ntvHaber.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 16:21:50.000000 ntvHaber-1.30.0/ntvHaber.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-18 16:21:50.000000 ntvHaber-1.30.0/ntvHaber.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-18 16:21:50.000000 ntvHaber-1.30.0/ntvHaber.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-18 16:21:50.000000 ntvHaber-1.30.0/ntvHaber.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 16:21:50.338291 ntvHaber-1.30.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/setup.py
```

### Comparing `ntvHaber-1.10/LICENSE` & `ntvHaber-1.30.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.10/ntvHaber/Assets/Logo.png` & `ntvHaber-1.30.0/ntvHaber/Assets/Logo.png`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.10/ntvHaber/Assets/Logo.svg` & `ntvHaber-1.30.0/Shared/org.kekikakademi.ntvHaber.svg`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.10/ntvHaber/Assets/favicon.ico` & `ntvHaber-1.30.0/ntvHaber/Assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.10/ntvHaber/Assets/favicon.png` & `ntvHaber-1.30.0/ntvHaber/Assets/favicon.png`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.10/ntvHaber/Assets/icons/apple-touch-icon-192.png` & `ntvHaber-1.30.0/ntvHaber/Assets/icons/apple-touch-icon-192.png`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.10/ntvHaber/Assets/icons/icon-192.png` & `ntvHaber-1.30.0/ntvHaber/Assets/icons/icon-192.png`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.10/ntvHaber/Assets/icons/icon-512.png` & `ntvHaber-1.30.0/ntvHaber/Assets/icons/icon-512.png`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.10/ntvHaber/Assets/icons/icon-maskable-192.png` & `ntvHaber-1.30.0/ntvHaber/Assets/icons/icon-maskable-192.png`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.10/ntvHaber/Assets/icons/icon-maskable-512.png` & `ntvHaber-1.30.0/ntvHaber/Assets/icons/icon-maskable-512.png`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.10/ntvHaber/Assets/icons/loading-animation.png` & `ntvHaber-1.30.0/ntvHaber/Assets/icons/loading-animation.png`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.10/ntvHaber/Assets/index.html` & `ntvHaber-1.30.0/ntvHaber/Assets/index.html`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.10/ntvHaber/Assets/manifest.json` & `ntvHaber-1.30.0/ntvHaber/Assets/manifest.json`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.10/ntvHaber/CLI/__init__.py` & `ntvHaber-1.30.0/ntvHaber/CLI/__init__.py`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.10/ntvHaber/Layouts/Haberler.py` & `ntvHaber-1.30.0/ntvHaber/Layouts/Haberler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Bu araç @keyiflerolsun tarafından | @KekikAkademi için yazılmıştır.
 
-from ..CLI     import konsol
-from flet.page import Page
-from flet      import UserControl, GridView, Container, Column, Text, colors, border, ImageFit 
-from ..Libs    import sondakika_haberleri, bildirim
+from ..CLI  import konsol
+from flet   import Page, UserControl, GridView, Container, Column, Text, colors, border, ImageFit 
+from ..Libs import sondakika_haberleri, bildirim
 
 class Haberler(UserControl):
     def __init__(self, sayfa:Page, panel:Page):
         super().__init__()
         self.sayfa = sayfa
 
         self.panel    = panel
```

### Comparing `ntvHaber-1.10/ntvHaber/Layouts/KekikFlet.py` & `ntvHaber-1.30.0/ntvHaber/Layouts/KekikFlet.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # Bu araç @keyiflerolsun tarafından | @KekikAkademi için yazılmıştır.
 
-from flet.page import Page, Event
+from flet            import Page
+from flet_core.event import Event
 
 class KekikFlet:
     def __init__(self, sayfa:Page, baslik:str):
         sayfa.title                = baslik
         sayfa.horizontal_alignment = "center"
         sayfa.vertical_alignment   = "center"
         sayfa.theme_mode           = "dark"
         sayfa.scroll               = "adaptive"
         # sayfa.auto_scroll          = True
 
-        sayfa.window_max_width     = 600
+        sayfa.window_width     = 600
+        sayfa.window_max_width = 600
         # sayfa.window_skip_task_bar = True
 
         self.sayfa = sayfa
 
         def kapanirken(event:Event):
             if event.data == "close":
                 self.sayfa.window_destroy()
```

### Comparing `ntvHaber-1.10/ntvHaber/Layouts/Panel.py` & `ntvHaber-1.30.0/ntvHaber/Layouts/Panel.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # Bu araç @keyiflerolsun tarafından | @KekikAkademi için yazılmıştır.
 
-from flet.page import Page
-from flet      import UserControl, Container, Column, Row, Text, ProgressRing, colors, Divider
+from flet import Page, UserControl, Container, Column, Row, Text, ProgressRing, colors, Divider
 
 class Panel(UserControl):
     def __init__(self, sayfa:Page):
         super().__init__()
         self.sayfa = sayfa
 
         self.baslik      = Text("NTV Son Dakika Haberleri", size=22, weight="bold", color="#EF7F1A")
```

### Comparing `ntvHaber-1.10/ntvHaber/Libs/NTV.py` & `ntvHaber-1.30.0/ntvHaber/Libs/NTV.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     return haberler
 
 def sondakika_haberleri() -> list:
     konsol.log("[yellow]sondakika_haberleri() fonksiyonu çalıştırıldı...[/]")
 
     global RAMBASE
 
-    istek    = get("https://kolektifapi.kekikakademi.org/haber")
+    istek    = get("https://kolektifapi.kekikakademi.org/haber", headers={"User-Agent": "org.kekikakademi.ntvHaber"})
     haberler = istek.json()["veri"]
 
     detay_sor = []
     for haber in haberler:
         if haber["haber"] in RAMBASE:
             continue
```

### Comparing `ntvHaber-1.10/ntvHaber/Libs/__init__.py` & `ntvHaber-1.30.0/ntvHaber/Libs/__init__.py`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.10/ntvHaber/__init__.py` & `ntvHaber-1.30.0/ntvHaber/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Bu araç @keyiflerolsun tarafından | @KekikAkademi için yazılmıştır.
 
-from .CLI      import cikis_yap, hata_yakala
+from .CLI import cikis_yap, hata_yakala
 
-from flet      import FLET_APP, WEB_BROWSER
-from flet      import app as flet
-from flet.page import Page
+from flet import Page, FLET_APP, WEB_BROWSER
+from flet import app as flet
 
 import pystray
 from PIL   import Image
 from .Libs import dosya_ver
 
 from .Layouts import KekikFlet, Panel, Haberler
 from os       import name as sistem
```

### Comparing `ntvHaber-1.10/ntvHaber.egg-info/SOURCES.txt` & `ntvHaber-1.30.0/ntvHaber.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 LICENSE
 MANIFEST.in
 README.md
-org.kekikakademi.ntvHaber.appdata.xml
-org.kekikakademi.ntvHaber.desktop
 setup.py
+Shared/org.kekikakademi.ntvHaber.appdata.xml
+Shared/org.kekikakademi.ntvHaber.desktop
+Shared/org.kekikakademi.ntvHaber.svg
 ntvHaber/__init__.py
-ntvHaber/requirements.txt
 ntvHaber.egg-info/PKG-INFO
 ntvHaber.egg-info/SOURCES.txt
 ntvHaber.egg-info/dependency_links.txt
 ntvHaber.egg-info/entry_points.txt
 ntvHaber.egg-info/requires.txt
 ntvHaber.egg-info/top_level.txt
 ntvHaber/Assets/Logo.png
-ntvHaber/Assets/Logo.svg
 ntvHaber/Assets/favicon.ico
 ntvHaber/Assets/favicon.png
 ntvHaber/Assets/index.html
 ntvHaber/Assets/manifest.json
 ntvHaber/Assets/icons/apple-touch-icon-192.png
 ntvHaber/Assets/icons/icon-192.png
 ntvHaber/Assets/icons/icon-512.png
```

### Comparing `ntvHaber-1.10/org.kekikakademi.ntvHaber.appdata.xml` & `ntvHaber-1.30.0/Shared/org.kekikakademi.ntvHaber.appdata.xml`

 * *Files 13% similar despite different names*

#### Comparing `ntvHaber-1.10/org.kekikakademi.ntvHaber.appdata.xml` & `ntvHaber-1.30.0/Shared/org.kekikakademi.ntvHaber.appdata.xml`

```diff
@@ -5,33 +5,39 @@
   <project_license>GPL-3.0</project_license>
   <id type="desktop">org.kekikakademi.ntvHaber.desktop</id>
   <launchable type="desktop-id">org.kekikakademi.ntvHaber.desktop</launchable>
   <name>ntvHaber</name>
   <summary>Breaking News in Turkish from NTV.com.tr</summary>
   <summary xml:lang="tr_TR">NTV.com.tr sitesinden Son Dakika Haberleri</summary>
   <url type="homepage">https://github.com/keyiflerolsun/ntvHaber</url>
+  <url type="bugtracker">https://github.com/keyiflerolsun/ntvHaber/issues</url>
   <url type="donation">https://keyiflerolsun.me/Kahve</url>
   <developer_name>keyiflerolsun</developer_name>
   <description>
     <p>Breaking News in Turkish from NTV.com.tr</p>
     <p>An example application prepared with Python language and Flet Library.</p>
   </description>
   <description xml:lang="tr_TR">
     <p>NTV Son Dakika Haberleri</p>
     <p>https://t.me/KekikAkademi için hazırlanmıştır..</p>
   </description>
   <screenshots>
     <screenshot type="default">
-      <image>https://raw.githubusercontent.com/keyiflerolsun/ntvHaber/paketlenebilir/Resimler/SS.jpg</image>
+      <image>https://raw.githubusercontent.com/keyiflerolsun/ntvHaber/main/.github/icons/SS.png</image>
     </screenshot>
   </screenshots>
   <categories>
     <category>Education</category>
   </categories>
   <releases>
+    <release version="1.30.0" date="2023-05-23">
+      <description>
+        <p>Güncellenen Flet yolları ile uygulama yeniden derlenmiştir.</p>
+      </description>
+    </release>
     <release version="1.10" date="2023-01-22">
       <description>
         <p>Sistem bildirimleri ve sistem tepsisi ikonu..</p>
       </description>
     </release>
     <release version="1.4" date="2023-01-21">
       <description>
```

### Comparing `ntvHaber-1.10/setup.py` & `ntvHaber-1.30.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 from io         import open
 
 setup(
     # ? Genel Bilgiler
     name         = "ntvHaber",
-    version      = "1.10",
+    version      = "1.30.0",
     url          = "https://github.com/keyiflerolsun/ntvHaber",
     description  = "NTV Son Dakika Haberleri",
     keywords     = ["ntvHaber", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
 
@@ -21,21 +21,18 @@
         "Programming Language :: Python :: 3"
     ],
 
     # ? Paket Bilgileri
     packages         = ["ntvHaber"],
     python_requires  = ">=3.10",
     install_requires = [
-        "pip",
         "setuptools",
         "wheel",
         "install-freedesktop",
         "rich",
-        "pdm",
-        "pdm-pep517",
         "flet",
         "pystray",
         "Pillow",
         "notify-py",
         "requests",
         "APScheduler",
         "parsel"
@@ -47,17 +44,17 @@
             "ntvHaber = ntvHaber:basla",
         ]
     },
 
     # ? Masaüstü Paketi
     setup_requires = ["install_freedesktop"],
     data_files     = [
-        ("share/applications",                ["org.kekikakademi.ntvHaber.desktop"]),
-        ("share/appdata",                     ["org.kekikakademi.ntvHaber.appdata.xml"]),
-        ("share/icons/hicolor/scalable/apps", ["ntvHaber/Assets/Logo.svg"])
+        ("share/applications",                ["Shared/org.kekikakademi.ntvHaber.desktop"]),
+        ("share/appdata",                     ["Shared/org.kekikakademi.ntvHaber.appdata.xml"]),
+        ("share/icons/hicolor/scalable/apps", ["Shared/org.kekikakademi.ntvHaber.svg"])
     ],
 
     # ? PyPI Bilgileri
     long_description_content_type = "text/markdown",
-    long_description              = "".join(open("PyPi.md", encoding="utf-8").readlines()),
+    long_description              = "".join(open("README.md", encoding="utf-8").readlines()),
     include_package_data          = True
 )
```

