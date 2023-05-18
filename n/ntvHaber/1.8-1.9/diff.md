# Comparing `tmp/ntvHaber-1.8.tar.gz` & `tmp/ntvHaber-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntvHaber-1.8.tar", last modified: Sun Jan 22 00:58:51 2023, max compression
+gzip compressed data, was "ntvHaber-1.9.tar", last modified: Sun Jan 22 02:27:03 2023, max compression
```

## Comparing `ntvHaber-1.8.tar` & `ntvHaber-1.9.tar`

### file list

```diff
@@ -1,44 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 00:58:51.753083 ntvHaber-1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-22 00:58:33.000000 ntvHaber-1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-22 00:58:33.000000 ntvHaber-1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-01-22 00:58:51.753083 ntvHaber-1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-01-22 00:58:33.000000 ntvHaber-1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 00:58:51.753083 ntvHaber-1.8/ntvHaber/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 00:58:51.753083 ntvHaber-1.8/ntvHaber/Assets/
--rw-r--r--   0 runner    (1001) docker     (123)    12254 2023-01-22 00:58:33.000000 ntvHaber-1.8/ntvHaber/Assets/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-01-22 00:58:33.000000 ntvHaber-1.8/ntvHaber/Assets/Logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-01-22 00:58:33.000000 ntvHaber-1.8/ntvHaber/Assets/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-01-22 00:58:33.000000 ntvHaber-1.8/ntvHaber/Assets/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 00:58:51.753083 ntvHaber-1.8/ntvHaber/Assets/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-01-22 00:58:33.000000 ntvHaber-1.8/ntvHaber/Assets/icons/apple-touch-icon-192.png
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-01-22 00:58:33.000000 ntvHaber-1.8/ntvHaber/Assets/icons/icon-192.png
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-01-22 00:58:33.000000 ntvHaber-1.8/ntvHaber/Assets/icons/icon-512.png
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-01-22 00:58:33.000000 ntvHaber-1.8/ntvHaber/Assets/icons/icon-maskable-192.png
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-01-22 00:58:33.000000 ntvHaber-1.8/ntvHaber/Assets/icons/icon-maskable-512.png
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-01-22 00:58:33.000000 ntvHaber-1.8/ntvHaber/Assets/icons/loading-animation.png
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-01-22 00:58:33.000000 ntvHaber-1.8/ntvHaber/Assets/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-01-22 00:58:33.000000 ntvHaber-1.8/ntvHaber/Assets/manifest.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 00:58:51.753083 ntvHaber-1.8/ntvHaber/CLI/
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-01-22 00:58:33.000000 ntvHaber-1.8/ntvHaber/CLI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 00:58:51.753083 ntvHaber-1.8/ntvHaber/Layouts/
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-01-22 00:58:33.000000 ntvHaber-1.8/ntvHaber/Layouts/Haberler.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-01-22 00:58:33.000000 ntvHaber-1.8/ntvHaber/Layouts/KekikFlet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-01-22 00:58:33.000000 ntvHaber-1.8/ntvHaber/Layouts/Panel.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-01-22 00:58:33.000000 ntvHaber-1.8/ntvHaber/Layouts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 00:58:51.753083 ntvHaber-1.8/ntvHaber/Libs/
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-01-22 00:58:33.000000 ntvHaber-1.8/ntvHaber/Libs/NTV.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-01-22 00:58:33.000000 ntvHaber-1.8/ntvHaber/Libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-01-22 00:58:33.000000 ntvHaber-1.8/ntvHaber/Libs/dosya_ver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-01-22 00:58:33.000000 ntvHaber-1.8/ntvHaber/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-01-22 00:58:33.000000 ntvHaber-1.8/ntvHaber/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 00:58:51.753083 ntvHaber-1.8/ntvHaber.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-01-22 00:58:51.000000 ntvHaber-1.8/ntvHaber.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-01-22 00:58:51.000000 ntvHaber-1.8/ntvHaber.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-22 00:58:51.000000 ntvHaber-1.8/ntvHaber.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-01-22 00:58:51.000000 ntvHaber-1.8/ntvHaber.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-01-22 00:58:51.000000 ntvHaber-1.8/ntvHaber.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-22 00:58:51.000000 ntvHaber-1.8/ntvHaber.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-01-22 00:58:33.000000 ntvHaber-1.8/org.kekikakademi.ntvHaber.appdata.xml
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-01-22 00:58:33.000000 ntvHaber-1.8/org.kekikakademi.ntvHaber.desktop
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-22 00:58:51.753083 ntvHaber-1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-01-22 00:58:33.000000 ntvHaber-1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 02:27:03.755395 ntvHaber-1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-22 02:26:45.000000 ntvHaber-1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-22 02:26:45.000000 ntvHaber-1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-01-22 02:27:03.755395 ntvHaber-1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-01-22 02:26:45.000000 ntvHaber-1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 02:27:03.755395 ntvHaber-1.9/ntvHaber/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 02:27:03.755395 ntvHaber-1.9/ntvHaber/Assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    12254 2023-01-22 02:26:45.000000 ntvHaber-1.9/ntvHaber/Assets/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-01-22 02:26:45.000000 ntvHaber-1.9/ntvHaber/Assets/Logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-01-22 02:26:45.000000 ntvHaber-1.9/ntvHaber/Assets/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-01-22 02:26:45.000000 ntvHaber-1.9/ntvHaber/Assets/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 02:27:03.755395 ntvHaber-1.9/ntvHaber/Assets/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-01-22 02:26:45.000000 ntvHaber-1.9/ntvHaber/Assets/icons/apple-touch-icon-192.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-01-22 02:26:45.000000 ntvHaber-1.9/ntvHaber/Assets/icons/icon-192.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-01-22 02:26:45.000000 ntvHaber-1.9/ntvHaber/Assets/icons/icon-512.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-01-22 02:26:45.000000 ntvHaber-1.9/ntvHaber/Assets/icons/icon-maskable-192.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-01-22 02:26:45.000000 ntvHaber-1.9/ntvHaber/Assets/icons/icon-maskable-512.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-01-22 02:26:45.000000 ntvHaber-1.9/ntvHaber/Assets/icons/loading-animation.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-01-22 02:26:45.000000 ntvHaber-1.9/ntvHaber/Assets/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-01-22 02:26:45.000000 ntvHaber-1.9/ntvHaber/Assets/manifest.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 02:27:03.755395 ntvHaber-1.9/ntvHaber/CLI/
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-01-22 02:26:45.000000 ntvHaber-1.9/ntvHaber/CLI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 02:27:03.755395 ntvHaber-1.9/ntvHaber/Layouts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-01-22 02:26:45.000000 ntvHaber-1.9/ntvHaber/Layouts/Haberler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-01-22 02:26:45.000000 ntvHaber-1.9/ntvHaber/Layouts/KekikFlet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-01-22 02:26:45.000000 ntvHaber-1.9/ntvHaber/Layouts/Panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-01-22 02:26:45.000000 ntvHaber-1.9/ntvHaber/Layouts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 02:27:03.755395 ntvHaber-1.9/ntvHaber/Libs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-01-22 02:26:45.000000 ntvHaber-1.9/ntvHaber/Libs/NTV.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-01-22 02:26:45.000000 ntvHaber-1.9/ntvHaber/Libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-01-22 02:26:45.000000 ntvHaber-1.9/ntvHaber/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-01-22 02:26:45.000000 ntvHaber-1.9/ntvHaber/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 02:27:03.755395 ntvHaber-1.9/ntvHaber.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-01-22 02:27:03.000000 ntvHaber-1.9/ntvHaber.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-01-22 02:27:03.000000 ntvHaber-1.9/ntvHaber.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-22 02:27:03.000000 ntvHaber-1.9/ntvHaber.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-01-22 02:27:03.000000 ntvHaber-1.9/ntvHaber.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-01-22 02:27:03.000000 ntvHaber-1.9/ntvHaber.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-22 02:27:03.000000 ntvHaber-1.9/ntvHaber.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-01-22 02:26:45.000000 ntvHaber-1.9/org.kekikakademi.ntvHaber.appdata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-01-22 02:26:45.000000 ntvHaber-1.9/org.kekikakademi.ntvHaber.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-22 02:27:03.755395 ntvHaber-1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-01-22 02:26:45.000000 ntvHaber-1.9/setup.py
```

### Comparing `ntvHaber-1.8/LICENSE` & `ntvHaber-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.8/PKG-INFO` & `ntvHaber-1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntvHaber
-Version: 1.8
+Version: 1.9
 Summary: NTV Son Dakika Haberleri
 Home-page: https://github.com/keyiflerolsun/ntvHaber
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: ntvHaber,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ntvHaber Version: 1.8 Summary: NTV Son Dakika
+Metadata-Version: 2.1 Name: ntvHaber Version: 1.9 Summary: NTV Son Dakika
 Haberleri Home-page: https://github.com/keyiflerolsun/ntvHaber Author:
 keyiflerolsun Author-email: keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 ntvHaber,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE # ð° ntvHaber ![Repo Boyutu](https://img.shields.io/github/repo-size/
```

### Comparing `ntvHaber-1.8/README.md` & `ntvHaber-1.9/README.md`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.8/ntvHaber/Assets/Logo.png` & `ntvHaber-1.9/ntvHaber/Assets/Logo.png`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.8/ntvHaber/Assets/Logo.svg` & `ntvHaber-1.9/ntvHaber/Assets/Logo.svg`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.8/ntvHaber/Assets/favicon.ico` & `ntvHaber-1.9/ntvHaber/Assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.8/ntvHaber/Assets/favicon.png` & `ntvHaber-1.9/ntvHaber/Assets/favicon.png`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.8/ntvHaber/Assets/icons/apple-touch-icon-192.png` & `ntvHaber-1.9/ntvHaber/Assets/icons/apple-touch-icon-192.png`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.8/ntvHaber/Assets/icons/icon-192.png` & `ntvHaber-1.9/ntvHaber/Assets/icons/icon-192.png`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.8/ntvHaber/Assets/icons/icon-512.png` & `ntvHaber-1.9/ntvHaber/Assets/icons/icon-512.png`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.8/ntvHaber/Assets/icons/icon-maskable-192.png` & `ntvHaber-1.9/ntvHaber/Assets/icons/icon-maskable-192.png`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.8/ntvHaber/Assets/icons/icon-maskable-512.png` & `ntvHaber-1.9/ntvHaber/Assets/icons/icon-maskable-512.png`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.8/ntvHaber/Assets/icons/loading-animation.png` & `ntvHaber-1.9/ntvHaber/Assets/icons/loading-animation.png`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.8/ntvHaber/Assets/index.html` & `ntvHaber-1.9/ntvHaber/Assets/index.html`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.8/ntvHaber/Assets/manifest.json` & `ntvHaber-1.9/ntvHaber/Assets/manifest.json`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.8/ntvHaber/CLI/__init__.py` & `ntvHaber-1.9/ntvHaber/CLI/__init__.py`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.8/ntvHaber/Layouts/Haberler.py` & `ntvHaber-1.9/ntvHaber/Layouts/Haberler.py`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.8/ntvHaber/Layouts/KekikFlet.py` & `ntvHaber-1.9/ntvHaber/Layouts/KekikFlet.py`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.8/ntvHaber/Layouts/Panel.py` & `ntvHaber-1.9/ntvHaber/Layouts/Panel.py`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.8/ntvHaber/Libs/NTV.py` & `ntvHaber-1.9/ntvHaber/Libs/NTV.py`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.8/ntvHaber/__init__.py` & `ntvHaber-1.9/ntvHaber/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from .CLI      import cikis_yap, hata_yakala
 
 from flet      import FLET_APP, WEB_BROWSER
 from flet      import app as flet
 from flet.page import Page
 
 import pystray
-from PIL             import Image
-from .Libs.dosya_ver import get_resource
+from PIL   import Image
+from .Libs import dosya_ver
 
 from .Layouts import KekikFlet, Panel, Haberler
 from os       import name as sistem
 from .Libs    import zamanlayici
 
 ZAMANLA = False
 
@@ -37,15 +37,15 @@
 
     def __gizle():
         sayfa.window_minimized = True
         sayfa.update()
 
     simge_durum = pystray.Icon(
         name  = sayfa.title,
-        icon  = Image.open(get_resource("Assets/Logo.png")),
+        icon  = Image.open(dosya_ver("Assets/Logo.png", 2)),
         title = sayfa.title,
         menu  = pystray.Menu(
             pystray.MenuItem("Göster", __goster),
             pystray.MenuItem("Gizle", __gizle),            
             pystray.MenuItem("Kapat", sayfa.window_destroy)
         )
     )
```

### Comparing `ntvHaber-1.8/ntvHaber.egg-info/PKG-INFO` & `ntvHaber-1.9/ntvHaber.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntvHaber
-Version: 1.8
+Version: 1.9
 Summary: NTV Son Dakika Haberleri
 Home-page: https://github.com/keyiflerolsun/ntvHaber
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: ntvHaber,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ntvHaber Version: 1.8 Summary: NTV Son Dakika
+Metadata-Version: 2.1 Name: ntvHaber Version: 1.9 Summary: NTV Son Dakika
 Haberleri Home-page: https://github.com/keyiflerolsun/ntvHaber Author:
 keyiflerolsun Author-email: keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 ntvHaber,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE # ð° ntvHaber ![Repo Boyutu](https://img.shields.io/github/repo-size/
```

### Comparing `ntvHaber-1.8/ntvHaber.egg-info/SOURCES.txt` & `ntvHaber-1.9/ntvHaber.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -26,9 +26,8 @@
 ntvHaber/Assets/icons/loading-animation.png
 ntvHaber/CLI/__init__.py
 ntvHaber/Layouts/Haberler.py
 ntvHaber/Layouts/KekikFlet.py
 ntvHaber/Layouts/Panel.py
 ntvHaber/Layouts/__init__.py
 ntvHaber/Libs/NTV.py
-ntvHaber/Libs/__init__.py
-ntvHaber/Libs/dosya_ver.py
+ntvHaber/Libs/__init__.py
```

### Comparing `ntvHaber-1.8/org.kekikakademi.ntvHaber.appdata.xml` & `ntvHaber-1.9/org.kekikakademi.ntvHaber.appdata.xml`

 * *Files 0% similar despite different names*

#### Comparing `ntvHaber-1.8/org.kekikakademi.ntvHaber.appdata.xml` & `ntvHaber-1.9/org.kekikakademi.ntvHaber.appdata.xml`

```diff
@@ -24,15 +24,15 @@
       <image>https://raw.githubusercontent.com/keyiflerolsun/ntvHaber/paketlenebilir/Resimler/SS.jpg</image>
     </screenshot>
   </screenshots>
   <categories>
     <category>Education</category>
   </categories>
   <releases>
-    <release version="1.8" date="2023-01-22">
+    <release version="1.9" date="2023-01-22">
       <description>
         <p>Sistem bildirimleri ve sistem tepsisi ikonu..</p>
       </description>
     </release>
     <release version="1.4" date="2023-01-21">
       <description>
         <p>GridView Kullanımı</p>
```

### Comparing `ntvHaber-1.8/setup.py` & `ntvHaber-1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 from io         import open
 
 setup(
     # ? Genel Bilgiler
     name         = "ntvHaber",
-    version      = "1.8",
+    version      = "1.9",
     url          = "https://github.com/keyiflerolsun/ntvHaber",
     description  = "NTV Son Dakika Haberleri",
     keywords     = ["ntvHaber", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
```

