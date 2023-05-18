# Comparing `tmp/ntvHaber-1.31.tar.gz` & `tmp/ntvHaber-1.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntvHaber-1.31.tar", last modified: Thu May 18 19:10:38 2023, max compression
+gzip compressed data, was "ntvHaber-1.32.tar", last modified: Thu May 18 19:13:31 2023, max compression
```

## Comparing `ntvHaber-1.31.tar` & `ntvHaber-1.32.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:10:38.519896 ntvHaber-1.31/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 19:10:19.000000 ntvHaber-1.31/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-18 19:10:19.000000 ntvHaber-1.31/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-05-18 19:10:38.519896 ntvHaber-1.31/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-05-18 19:10:19.000000 ntvHaber-1.31/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:10:38.519896 ntvHaber-1.31/Shared/
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-05-18 19:10:19.000000 ntvHaber-1.31/Shared/org.kekikakademi.ntvHaber.appdata.xml
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-18 19:10:19.000000 ntvHaber-1.31/Shared/org.kekikakademi.ntvHaber.desktop
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-18 19:10:19.000000 ntvHaber-1.31/Shared/org.kekikakademi.ntvHaber.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:10:38.519896 ntvHaber-1.31/ntvHaber/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:10:38.519896 ntvHaber-1.31/ntvHaber/Assets/
--rw-r--r--   0 runner    (1001) docker     (123)    12254 2023-05-18 19:10:19.000000 ntvHaber-1.31/ntvHaber/Assets/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-18 19:10:19.000000 ntvHaber-1.31/ntvHaber/Assets/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-18 19:10:19.000000 ntvHaber-1.31/ntvHaber/Assets/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:10:38.519896 ntvHaber-1.31/ntvHaber/Assets/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-05-18 19:10:19.000000 ntvHaber-1.31/ntvHaber/Assets/icons/apple-touch-icon-192.png
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-05-18 19:10:19.000000 ntvHaber-1.31/ntvHaber/Assets/icons/icon-192.png
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-05-18 19:10:19.000000 ntvHaber-1.31/ntvHaber/Assets/icons/icon-512.png
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-05-18 19:10:19.000000 ntvHaber-1.31/ntvHaber/Assets/icons/icon-maskable-192.png
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-05-18 19:10:19.000000 ntvHaber-1.31/ntvHaber/Assets/icons/icon-maskable-512.png
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-05-18 19:10:19.000000 ntvHaber-1.31/ntvHaber/Assets/icons/loading-animation.png
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-18 19:10:19.000000 ntvHaber-1.31/ntvHaber/Assets/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-18 19:10:19.000000 ntvHaber-1.31/ntvHaber/Assets/manifest.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:10:38.519896 ntvHaber-1.31/ntvHaber/CLI/
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-18 19:10:19.000000 ntvHaber-1.31/ntvHaber/CLI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:10:38.519896 ntvHaber-1.31/ntvHaber/Layouts/
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-18 19:10:19.000000 ntvHaber-1.31/ntvHaber/Layouts/Haberler.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-18 19:10:19.000000 ntvHaber-1.31/ntvHaber/Layouts/KekikFlet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-18 19:10:19.000000 ntvHaber-1.31/ntvHaber/Layouts/Panel.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-18 19:10:19.000000 ntvHaber-1.31/ntvHaber/Layouts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:10:38.519896 ntvHaber-1.31/ntvHaber/Libs/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-18 19:10:19.000000 ntvHaber-1.31/ntvHaber/Libs/NTV.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-18 19:10:19.000000 ntvHaber-1.31/ntvHaber/Libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-18 19:10:19.000000 ntvHaber-1.31/ntvHaber/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:10:38.519896 ntvHaber-1.31/ntvHaber.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-05-18 19:10:38.000000 ntvHaber-1.31/ntvHaber.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-18 19:10:38.000000 ntvHaber-1.31/ntvHaber.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 19:10:38.000000 ntvHaber-1.31/ntvHaber.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-18 19:10:38.000000 ntvHaber-1.31/ntvHaber.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-18 19:10:38.000000 ntvHaber-1.31/ntvHaber.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-18 19:10:38.000000 ntvHaber-1.31/ntvHaber.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 19:10:38.519896 ntvHaber-1.31/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-18 19:10:19.000000 ntvHaber-1.31/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:13:31.857517 ntvHaber-1.32/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 19:13:11.000000 ntvHaber-1.32/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-18 19:13:11.000000 ntvHaber-1.32/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-05-18 19:13:31.857517 ntvHaber-1.32/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-05-18 19:13:11.000000 ntvHaber-1.32/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:13:31.857517 ntvHaber-1.32/Shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-05-18 19:13:11.000000 ntvHaber-1.32/Shared/org.kekikakademi.ntvHaber.appdata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-18 19:13:11.000000 ntvHaber-1.32/Shared/org.kekikakademi.ntvHaber.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-18 19:13:11.000000 ntvHaber-1.32/Shared/org.kekikakademi.ntvHaber.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:13:31.857517 ntvHaber-1.32/ntvHaber/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:13:31.857517 ntvHaber-1.32/ntvHaber/Assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    12254 2023-05-18 19:13:11.000000 ntvHaber-1.32/ntvHaber/Assets/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-18 19:13:11.000000 ntvHaber-1.32/ntvHaber/Assets/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-18 19:13:11.000000 ntvHaber-1.32/ntvHaber/Assets/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:13:31.857517 ntvHaber-1.32/ntvHaber/Assets/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-05-18 19:13:11.000000 ntvHaber-1.32/ntvHaber/Assets/icons/apple-touch-icon-192.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-05-18 19:13:11.000000 ntvHaber-1.32/ntvHaber/Assets/icons/icon-192.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-05-18 19:13:11.000000 ntvHaber-1.32/ntvHaber/Assets/icons/icon-512.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-05-18 19:13:11.000000 ntvHaber-1.32/ntvHaber/Assets/icons/icon-maskable-192.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-05-18 19:13:11.000000 ntvHaber-1.32/ntvHaber/Assets/icons/icon-maskable-512.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-05-18 19:13:11.000000 ntvHaber-1.32/ntvHaber/Assets/icons/loading-animation.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-18 19:13:11.000000 ntvHaber-1.32/ntvHaber/Assets/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-18 19:13:11.000000 ntvHaber-1.32/ntvHaber/Assets/manifest.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:13:31.857517 ntvHaber-1.32/ntvHaber/CLI/
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-18 19:13:11.000000 ntvHaber-1.32/ntvHaber/CLI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:13:31.857517 ntvHaber-1.32/ntvHaber/Layouts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-18 19:13:11.000000 ntvHaber-1.32/ntvHaber/Layouts/Haberler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-18 19:13:11.000000 ntvHaber-1.32/ntvHaber/Layouts/KekikFlet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-18 19:13:11.000000 ntvHaber-1.32/ntvHaber/Layouts/Panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-18 19:13:11.000000 ntvHaber-1.32/ntvHaber/Layouts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:13:31.857517 ntvHaber-1.32/ntvHaber/Libs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-18 19:13:11.000000 ntvHaber-1.32/ntvHaber/Libs/NTV.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-18 19:13:11.000000 ntvHaber-1.32/ntvHaber/Libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-18 19:13:11.000000 ntvHaber-1.32/ntvHaber/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:13:31.857517 ntvHaber-1.32/ntvHaber.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-05-18 19:13:31.000000 ntvHaber-1.32/ntvHaber.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-18 19:13:31.000000 ntvHaber-1.32/ntvHaber.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 19:13:31.000000 ntvHaber-1.32/ntvHaber.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-18 19:13:31.000000 ntvHaber-1.32/ntvHaber.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-18 19:13:31.000000 ntvHaber-1.32/ntvHaber.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-18 19:13:31.000000 ntvHaber-1.32/ntvHaber.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 19:13:31.857517 ntvHaber-1.32/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-18 19:13:11.000000 ntvHaber-1.32/setup.py
```

### Comparing `ntvHaber-1.31/LICENSE` & `ntvHaber-1.32/LICENSE`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.31/PKG-INFO` & `ntvHaber-1.32/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntvHaber
-Version: 1.31
+Version: 1.32
 Summary: NTV Son Dakika Haberleri
 Home-page: https://github.com/keyiflerolsun/ntvHaber
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: ntvHaber,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,14 +25,15 @@
 ![Status](https://img.shields.io/pypi/status/ntvHaber?logo=windowsterminal&logoColor=white)
 
 [![PyPI](https://img.shields.io/pypi/v/ntvHaber?logo=pypi&logoColor=white)](https://pypi.org/project/ntvHaber)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/ntvHaber?logo=pypi&logoColor=white)](https://pypi.org/project/ntvHaber)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/ntvHaber?logo=pypi&logoColor=white)](https://pypi.org/project/ntvHaber)
 
 [![PyPI Yükle](https://github.com/keyiflerolsun/ntvHaber/actions/workflows/pypiYukle.yml/badge.svg)](https://github.com/keyiflerolsun/ntvHaber/actions/workflows/pypiYukle.yml)
+[![Flatpak Yükle](https://github.com/keyiflerolsun/ntvHaber/actions/workflows/flatpakYukle.yml/badge.svg)](https://github.com/keyiflerolsun/ntvHaber/actions/workflows/flatpakYukle.yml)
 
 [![FlatHub](https://img.shields.io/flathub/v/org.kekikakademi.ntvHaber?logo=flathub&logoColor=white)](https://flathub.org/tr/apps/org.kekikakademi.ntvHaber)
 [![FlatHub - Downloads](https://img.shields.io/flathub/downloads/org.kekikakademi.ntvHaber?logo=flathub&logoColor=white)](https://flathub.org/tr/apps/org.kekikakademi.ntvHaber)
 
 **Python Yazılımların Python ve Flatpak olarak Paketlenme Örneği**
 
 _[@flet-dev](https://github.com/flet-dev) ile.._
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ntvHaber Version: 1.31 Summary: NTV Son Dakika
+Metadata-Version: 2.1 Name: ntvHaber Version: 1.32 Summary: NTV Son Dakika
 Haberleri Home-page: https://github.com/keyiflerolsun/ntvHaber Author:
 keyiflerolsun Author-email: keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 ntvHaber,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE # ð° ntvHaber ![Repo Boyutu](https://img.shields.io/github/repo-size/
@@ -16,15 +16,18 @@
 [PyPI](https://img.shields.io/pypi/v/ntvHaber?logo=pypi&logoColor=white)]
 (https://pypi.org/project/ntvHaber) [![PyPI - Downloads](https://
 img.shields.io/pypi/dm/ntvHaber?logo=pypi&logoColor=white)](https://pypi.org/
 project/ntvHaber) [![PyPI - Wheel](https://img.shields.io/pypi/wheel/
 ntvHaber?logo=pypi&logoColor=white)](https://pypi.org/project/ntvHaber) [![PyPI
 YÃ¼kle](https://github.com/keyiflerolsun/ntvHaber/actions/workflows/
 pypiYukle.yml/badge.svg)](https://github.com/keyiflerolsun/ntvHaber/actions/
-workflows/pypiYukle.yml) [![FlatHub](https://img.shields.io/flathub/v/
+workflows/pypiYukle.yml) [![Flatpak YÃ¼kle](https://github.com/keyiflerolsun/
+ntvHaber/actions/workflows/flatpakYukle.yml/badge.svg)](https://github.com/
+keyiflerolsun/ntvHaber/actions/workflows/flatpakYukle.yml) [![FlatHub](https://
+img.shields.io/flathub/v/
 org.kekikakademi.ntvHaber?logo=flathub&logoColor=white)](https://flathub.org/
 tr/apps/org.kekikakademi.ntvHaber) [![FlatHub - Downloads](https://
 img.shields.io/flathub/downloads/
 org.kekikakademi.ntvHaber?logo=flathub&logoColor=white)](https://flathub.org/
 tr/apps/org.kekikakademi.ntvHaber) **Python YazÄ±lÄ±mlarÄ±n Python ve Flatpak
 olarak Paketlenme ÃrneÄi** _[@flet-dev](https://github.com/flet-dev) ile.._ !
 [ntvHaber](https://raw.githubusercontent.com/keyiflerolsun/ntvHaber/
```

### Comparing `ntvHaber-1.31/README.md` & `ntvHaber-1.32/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 ![Status](https://img.shields.io/pypi/status/ntvHaber?logo=windowsterminal&logoColor=white)
 
 [![PyPI](https://img.shields.io/pypi/v/ntvHaber?logo=pypi&logoColor=white)](https://pypi.org/project/ntvHaber)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/ntvHaber?logo=pypi&logoColor=white)](https://pypi.org/project/ntvHaber)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/ntvHaber?logo=pypi&logoColor=white)](https://pypi.org/project/ntvHaber)
 
 [![PyPI Yükle](https://github.com/keyiflerolsun/ntvHaber/actions/workflows/pypiYukle.yml/badge.svg)](https://github.com/keyiflerolsun/ntvHaber/actions/workflows/pypiYukle.yml)
+[![Flatpak Yükle](https://github.com/keyiflerolsun/ntvHaber/actions/workflows/flatpakYukle.yml/badge.svg)](https://github.com/keyiflerolsun/ntvHaber/actions/workflows/flatpakYukle.yml)
 
 [![FlatHub](https://img.shields.io/flathub/v/org.kekikakademi.ntvHaber?logo=flathub&logoColor=white)](https://flathub.org/tr/apps/org.kekikakademi.ntvHaber)
 [![FlatHub - Downloads](https://img.shields.io/flathub/downloads/org.kekikakademi.ntvHaber?logo=flathub&logoColor=white)](https://flathub.org/tr/apps/org.kekikakademi.ntvHaber)
 
 **Python Yazılımların Python ve Flatpak olarak Paketlenme Örneği**
 
 _[@flet-dev](https://github.com/flet-dev) ile.._
```

#### html2text {}

```diff
@@ -9,15 +9,18 @@
 [PyPI](https://img.shields.io/pypi/v/ntvHaber?logo=pypi&logoColor=white)]
 (https://pypi.org/project/ntvHaber) [![PyPI - Downloads](https://
 img.shields.io/pypi/dm/ntvHaber?logo=pypi&logoColor=white)](https://pypi.org/
 project/ntvHaber) [![PyPI - Wheel](https://img.shields.io/pypi/wheel/
 ntvHaber?logo=pypi&logoColor=white)](https://pypi.org/project/ntvHaber) [![PyPI
 YÃ¼kle](https://github.com/keyiflerolsun/ntvHaber/actions/workflows/
 pypiYukle.yml/badge.svg)](https://github.com/keyiflerolsun/ntvHaber/actions/
-workflows/pypiYukle.yml) [![FlatHub](https://img.shields.io/flathub/v/
+workflows/pypiYukle.yml) [![Flatpak YÃ¼kle](https://github.com/keyiflerolsun/
+ntvHaber/actions/workflows/flatpakYukle.yml/badge.svg)](https://github.com/
+keyiflerolsun/ntvHaber/actions/workflows/flatpakYukle.yml) [![FlatHub](https://
+img.shields.io/flathub/v/
 org.kekikakademi.ntvHaber?logo=flathub&logoColor=white)](https://flathub.org/
 tr/apps/org.kekikakademi.ntvHaber) [![FlatHub - Downloads](https://
 img.shields.io/flathub/downloads/
 org.kekikakademi.ntvHaber?logo=flathub&logoColor=white)](https://flathub.org/
 tr/apps/org.kekikakademi.ntvHaber) **Python YazÄ±lÄ±mlarÄ±n Python ve Flatpak
 olarak Paketlenme ÃrneÄi** _[@flet-dev](https://github.com/flet-dev) ile.._ !
 [ntvHaber](https://raw.githubusercontent.com/keyiflerolsun/ntvHaber/
```

### Comparing `ntvHaber-1.31/Shared/org.kekikakademi.ntvHaber.appdata.xml` & `ntvHaber-1.32/Shared/org.kekikakademi.ntvHaber.appdata.xml`

 * *Files 0% similar despite different names*

#### Comparing `ntvHaber-1.31/Shared/org.kekikakademi.ntvHaber.appdata.xml` & `ntvHaber-1.32/Shared/org.kekikakademi.ntvHaber.appdata.xml`

```diff
@@ -25,15 +25,15 @@
       <image>https://raw.githubusercontent.com/keyiflerolsun/ntvHaber/main/.github/icons/SS.png</image>
     </screenshot>
   </screenshots>
   <categories>
     <category>Education</category>
   </categories>
   <releases>
-    <release version="1.31" date="2023-05-23">
+    <release version="1.32" date="2023-05-23">
       <description>
         <p>Güncellenen Flet yolları ile uygulama yeniden derlenmiştir.</p>
       </description>
     </release>
     <release version="1.10" date="2023-01-22">
       <description>
         <p>Sistem bildirimleri ve sistem tepsisi ikonu..</p>
```

### Comparing `ntvHaber-1.31/Shared/org.kekikakademi.ntvHaber.svg` & `ntvHaber-1.32/Shared/org.kekikakademi.ntvHaber.svg`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.31/ntvHaber/Assets/Logo.png` & `ntvHaber-1.32/ntvHaber/Assets/Logo.png`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.31/ntvHaber/Assets/favicon.ico` & `ntvHaber-1.32/ntvHaber/Assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.31/ntvHaber/Assets/favicon.png` & `ntvHaber-1.32/ntvHaber/Assets/favicon.png`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.31/ntvHaber/Assets/icons/apple-touch-icon-192.png` & `ntvHaber-1.32/ntvHaber/Assets/icons/apple-touch-icon-192.png`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.31/ntvHaber/Assets/icons/icon-192.png` & `ntvHaber-1.32/ntvHaber/Assets/icons/icon-192.png`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.31/ntvHaber/Assets/icons/icon-512.png` & `ntvHaber-1.32/ntvHaber/Assets/icons/icon-512.png`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.31/ntvHaber/Assets/icons/icon-maskable-192.png` & `ntvHaber-1.32/ntvHaber/Assets/icons/icon-maskable-192.png`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.31/ntvHaber/Assets/icons/icon-maskable-512.png` & `ntvHaber-1.32/ntvHaber/Assets/icons/icon-maskable-512.png`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.31/ntvHaber/Assets/icons/loading-animation.png` & `ntvHaber-1.32/ntvHaber/Assets/icons/loading-animation.png`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.31/ntvHaber/Assets/index.html` & `ntvHaber-1.32/ntvHaber/Assets/index.html`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.31/ntvHaber/Assets/manifest.json` & `ntvHaber-1.32/ntvHaber/Assets/manifest.json`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.31/ntvHaber/CLI/__init__.py` & `ntvHaber-1.32/ntvHaber/CLI/__init__.py`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.31/ntvHaber/Layouts/Haberler.py` & `ntvHaber-1.32/ntvHaber/Layouts/Haberler.py`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.31/ntvHaber/Layouts/KekikFlet.py` & `ntvHaber-1.32/ntvHaber/Layouts/KekikFlet.py`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.31/ntvHaber/Layouts/Panel.py` & `ntvHaber-1.32/ntvHaber/Layouts/Panel.py`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.31/ntvHaber/Libs/NTV.py` & `ntvHaber-1.32/ntvHaber/Libs/NTV.py`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.31/ntvHaber/Libs/__init__.py` & `ntvHaber-1.32/ntvHaber/Libs/__init__.py`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.31/ntvHaber/__init__.py` & `ntvHaber-1.32/ntvHaber/__init__.py`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.31/ntvHaber.egg-info/PKG-INFO` & `ntvHaber-1.32/ntvHaber.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntvHaber
-Version: 1.31
+Version: 1.32
 Summary: NTV Son Dakika Haberleri
 Home-page: https://github.com/keyiflerolsun/ntvHaber
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: ntvHaber,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,14 +25,15 @@
 ![Status](https://img.shields.io/pypi/status/ntvHaber?logo=windowsterminal&logoColor=white)
 
 [![PyPI](https://img.shields.io/pypi/v/ntvHaber?logo=pypi&logoColor=white)](https://pypi.org/project/ntvHaber)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/ntvHaber?logo=pypi&logoColor=white)](https://pypi.org/project/ntvHaber)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/ntvHaber?logo=pypi&logoColor=white)](https://pypi.org/project/ntvHaber)
 
 [![PyPI Yükle](https://github.com/keyiflerolsun/ntvHaber/actions/workflows/pypiYukle.yml/badge.svg)](https://github.com/keyiflerolsun/ntvHaber/actions/workflows/pypiYukle.yml)
+[![Flatpak Yükle](https://github.com/keyiflerolsun/ntvHaber/actions/workflows/flatpakYukle.yml/badge.svg)](https://github.com/keyiflerolsun/ntvHaber/actions/workflows/flatpakYukle.yml)
 
 [![FlatHub](https://img.shields.io/flathub/v/org.kekikakademi.ntvHaber?logo=flathub&logoColor=white)](https://flathub.org/tr/apps/org.kekikakademi.ntvHaber)
 [![FlatHub - Downloads](https://img.shields.io/flathub/downloads/org.kekikakademi.ntvHaber?logo=flathub&logoColor=white)](https://flathub.org/tr/apps/org.kekikakademi.ntvHaber)
 
 **Python Yazılımların Python ve Flatpak olarak Paketlenme Örneği**
 
 _[@flet-dev](https://github.com/flet-dev) ile.._
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ntvHaber Version: 1.31 Summary: NTV Son Dakika
+Metadata-Version: 2.1 Name: ntvHaber Version: 1.32 Summary: NTV Son Dakika
 Haberleri Home-page: https://github.com/keyiflerolsun/ntvHaber Author:
 keyiflerolsun Author-email: keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 ntvHaber,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE # ð° ntvHaber ![Repo Boyutu](https://img.shields.io/github/repo-size/
@@ -16,15 +16,18 @@
 [PyPI](https://img.shields.io/pypi/v/ntvHaber?logo=pypi&logoColor=white)]
 (https://pypi.org/project/ntvHaber) [![PyPI - Downloads](https://
 img.shields.io/pypi/dm/ntvHaber?logo=pypi&logoColor=white)](https://pypi.org/
 project/ntvHaber) [![PyPI - Wheel](https://img.shields.io/pypi/wheel/
 ntvHaber?logo=pypi&logoColor=white)](https://pypi.org/project/ntvHaber) [![PyPI
 YÃ¼kle](https://github.com/keyiflerolsun/ntvHaber/actions/workflows/
 pypiYukle.yml/badge.svg)](https://github.com/keyiflerolsun/ntvHaber/actions/
-workflows/pypiYukle.yml) [![FlatHub](https://img.shields.io/flathub/v/
+workflows/pypiYukle.yml) [![Flatpak YÃ¼kle](https://github.com/keyiflerolsun/
+ntvHaber/actions/workflows/flatpakYukle.yml/badge.svg)](https://github.com/
+keyiflerolsun/ntvHaber/actions/workflows/flatpakYukle.yml) [![FlatHub](https://
+img.shields.io/flathub/v/
 org.kekikakademi.ntvHaber?logo=flathub&logoColor=white)](https://flathub.org/
 tr/apps/org.kekikakademi.ntvHaber) [![FlatHub - Downloads](https://
 img.shields.io/flathub/downloads/
 org.kekikakademi.ntvHaber?logo=flathub&logoColor=white)](https://flathub.org/
 tr/apps/org.kekikakademi.ntvHaber) **Python YazÄ±lÄ±mlarÄ±n Python ve Flatpak
 olarak Paketlenme ÃrneÄi** _[@flet-dev](https://github.com/flet-dev) ile.._ !
 [ntvHaber](https://raw.githubusercontent.com/keyiflerolsun/ntvHaber/
```

### Comparing `ntvHaber-1.31/ntvHaber.egg-info/SOURCES.txt` & `ntvHaber-1.32/ntvHaber.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.31/setup.py` & `ntvHaber-1.32/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 from io         import open
 
 setup(
     # ? Genel Bilgiler
     name         = "ntvHaber",
-    version      = "1.31",
+    version      = "1.32",
     url          = "https://github.com/keyiflerolsun/ntvHaber",
     description  = "NTV Son Dakika Haberleri",
     keywords     = ["ntvHaber", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
```

