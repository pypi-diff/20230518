# Comparing `tmp/ntvHaber-1.30.0.tar.gz` & `tmp/ntvHaber-1.30.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntvHaber-1.30.0.tar", last modified: Thu May 18 16:21:50 2023, max compression
+gzip compressed data, was "ntvHaber-1.30.1.tar", last modified: Thu May 18 16:30:47 2023, max compression
```

## Comparing `ntvHaber-1.30.0.tar` & `ntvHaber-1.30.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:21:50.338291 ntvHaber-1.30.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-05-18 16:21:50.338291 ntvHaber-1.30.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:21:50.334291 ntvHaber-1.30.0/Shared/
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/Shared/org.kekikakademi.ntvHaber.appdata.xml
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/Shared/org.kekikakademi.ntvHaber.desktop
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/Shared/org.kekikakademi.ntvHaber.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:21:50.334291 ntvHaber-1.30.0/ntvHaber/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:21:50.338291 ntvHaber-1.30.0/ntvHaber/Assets/
--rw-r--r--   0 runner    (1001) docker     (123)    12254 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/ntvHaber/Assets/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/ntvHaber/Assets/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/ntvHaber/Assets/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:21:50.338291 ntvHaber-1.30.0/ntvHaber/Assets/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/ntvHaber/Assets/icons/apple-touch-icon-192.png
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/ntvHaber/Assets/icons/icon-192.png
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/ntvHaber/Assets/icons/icon-512.png
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/ntvHaber/Assets/icons/icon-maskable-192.png
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/ntvHaber/Assets/icons/icon-maskable-512.png
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/ntvHaber/Assets/icons/loading-animation.png
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/ntvHaber/Assets/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/ntvHaber/Assets/manifest.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:21:50.338291 ntvHaber-1.30.0/ntvHaber/CLI/
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/ntvHaber/CLI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:21:50.338291 ntvHaber-1.30.0/ntvHaber/Layouts/
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/ntvHaber/Layouts/Haberler.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/ntvHaber/Layouts/KekikFlet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/ntvHaber/Layouts/Panel.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/ntvHaber/Layouts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:21:50.338291 ntvHaber-1.30.0/ntvHaber/Libs/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/ntvHaber/Libs/NTV.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/ntvHaber/Libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/ntvHaber/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:21:50.338291 ntvHaber-1.30.0/ntvHaber.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-05-18 16:21:50.000000 ntvHaber-1.30.0/ntvHaber.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-18 16:21:50.000000 ntvHaber-1.30.0/ntvHaber.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 16:21:50.000000 ntvHaber-1.30.0/ntvHaber.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-18 16:21:50.000000 ntvHaber-1.30.0/ntvHaber.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-18 16:21:50.000000 ntvHaber-1.30.0/ntvHaber.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-18 16:21:50.000000 ntvHaber-1.30.0/ntvHaber.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 16:21:50.338291 ntvHaber-1.30.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-18 16:21:24.000000 ntvHaber-1.30.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:30:47.217013 ntvHaber-1.30.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 16:30:22.000000 ntvHaber-1.30.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-18 16:30:22.000000 ntvHaber-1.30.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-05-18 16:30:47.213012 ntvHaber-1.30.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-05-18 16:30:22.000000 ntvHaber-1.30.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:30:47.213012 ntvHaber-1.30.1/Shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-18 16:30:22.000000 ntvHaber-1.30.1/Shared/org.kekikakademi.ntvHaber.appdata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-18 16:30:22.000000 ntvHaber-1.30.1/Shared/org.kekikakademi.ntvHaber.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-18 16:30:22.000000 ntvHaber-1.30.1/Shared/org.kekikakademi.ntvHaber.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:30:47.213012 ntvHaber-1.30.1/ntvHaber/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:30:47.213012 ntvHaber-1.30.1/ntvHaber/Assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    12254 2023-05-18 16:30:22.000000 ntvHaber-1.30.1/ntvHaber/Assets/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-18 16:30:22.000000 ntvHaber-1.30.1/ntvHaber/Assets/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-18 16:30:22.000000 ntvHaber-1.30.1/ntvHaber/Assets/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:30:47.213012 ntvHaber-1.30.1/ntvHaber/Assets/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-05-18 16:30:22.000000 ntvHaber-1.30.1/ntvHaber/Assets/icons/apple-touch-icon-192.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-05-18 16:30:22.000000 ntvHaber-1.30.1/ntvHaber/Assets/icons/icon-192.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-05-18 16:30:22.000000 ntvHaber-1.30.1/ntvHaber/Assets/icons/icon-512.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-05-18 16:30:22.000000 ntvHaber-1.30.1/ntvHaber/Assets/icons/icon-maskable-192.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-05-18 16:30:22.000000 ntvHaber-1.30.1/ntvHaber/Assets/icons/icon-maskable-512.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-05-18 16:30:22.000000 ntvHaber-1.30.1/ntvHaber/Assets/icons/loading-animation.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-18 16:30:22.000000 ntvHaber-1.30.1/ntvHaber/Assets/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-18 16:30:22.000000 ntvHaber-1.30.1/ntvHaber/Assets/manifest.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:30:47.213012 ntvHaber-1.30.1/ntvHaber/CLI/
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-18 16:30:22.000000 ntvHaber-1.30.1/ntvHaber/CLI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:30:47.213012 ntvHaber-1.30.1/ntvHaber/Layouts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-18 16:30:22.000000 ntvHaber-1.30.1/ntvHaber/Layouts/Haberler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-18 16:30:22.000000 ntvHaber-1.30.1/ntvHaber/Layouts/KekikFlet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-18 16:30:22.000000 ntvHaber-1.30.1/ntvHaber/Layouts/Panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-18 16:30:22.000000 ntvHaber-1.30.1/ntvHaber/Layouts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:30:47.213012 ntvHaber-1.30.1/ntvHaber/Libs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-18 16:30:22.000000 ntvHaber-1.30.1/ntvHaber/Libs/NTV.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-18 16:30:22.000000 ntvHaber-1.30.1/ntvHaber/Libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-18 16:30:22.000000 ntvHaber-1.30.1/ntvHaber/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:30:47.213012 ntvHaber-1.30.1/ntvHaber.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-05-18 16:30:47.000000 ntvHaber-1.30.1/ntvHaber.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-18 16:30:47.000000 ntvHaber-1.30.1/ntvHaber.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 16:30:47.000000 ntvHaber-1.30.1/ntvHaber.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-18 16:30:47.000000 ntvHaber-1.30.1/ntvHaber.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-18 16:30:47.000000 ntvHaber-1.30.1/ntvHaber.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-18 16:30:47.000000 ntvHaber-1.30.1/ntvHaber.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 16:30:47.217013 ntvHaber-1.30.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-18 16:30:22.000000 ntvHaber-1.30.1/setup.py
```

### Comparing `ntvHaber-1.30.0/LICENSE` & `ntvHaber-1.30.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.30.0/PKG-INFO` & `ntvHaber-1.30.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntvHaber
-Version: 1.30.0
+Version: 1.30.1
 Summary: NTV Son Dakika Haberleri
 Home-page: https://github.com/keyiflerolsun/ntvHaber
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: ntvHaber,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
@@ -112,15 +112,15 @@
 
 ```bash
 # Depoyu Çek
 git clone https://github.com/keyiflerolsun/ntvHaber.git
 cd ntvHaber
 
 # Dosyaları al
-mv Shared/* . && rm -rf Shared
+mv Shared/*.yml . && mv Shared/SRC .
 
 # Gerekli Ortamları Kur
 flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
 flatpak remote-add --if-not-exists flathub-beta https://flathub.org/beta-repo/flathub-beta.flatpakrepo
 flatpak update && flatpak upgrade
 flatpak install flathub org.freedesktop.{Platform,Sdk}//22.08
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ntvHaber Version: 1.30.0 Summary: NTV Son Dakika
+Metadata-Version: 2.1 Name: ntvHaber Version: 1.30.1 Summary: NTV Son Dakika
 Haberleri Home-page: https://github.com/keyiflerolsun/ntvHaber Author:
 keyiflerolsun Author-email: keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 ntvHaber,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE # ð° ntvHaber ![Repo Boyutu](https://img.shields.io/github/repo-size/
@@ -47,20 +47,20 @@
 icons/python.svg] Python ```bash # Depoyu Ãek https://github.com/
 keyiflerolsun/ntvHaber.git cd ntvHaber # Gerekli OrtamlarÄ± Kur pip install -
 U pip setuptools wheel twine # Paketi YÃ¼kle pip install . # ArtÄ±klarÄ±
 Temizle rm -rf build *.egg-info # ÃalÄ±ÅtÄ±r ntvHaber # Paketi KaldÄ±r pip
 uninstall ntvHaber ``` ### [https://raw.githubusercontent.com/keyiflerolsun/
 ntvHaber/main/.github/icons/flatpak.svg] FlatPak ```bash # Depoyu Ãek git
 clone https://github.com/keyiflerolsun/ntvHaber.git cd ntvHaber # DosyalarÄ± al
-mv Shared/* . && rm -rf Shared # Gerekli OrtamlarÄ± Kur flatpak remote-add --
-if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo flatpak
-remote-add --if-not-exists flathub-beta https://flathub.org/beta-repo/flathub-
-beta.flatpakrepo flatpak update && flatpak upgrade flatpak install flathub
-org.freedesktop.{Platform,Sdk}//22.08 # Paketle flatpak-builder --user --
-install --force-clean build-dir org.kekikakademi.ntvHaber.yml # ArtÄ±klarÄ±
+mv Shared/*.yml . && mv Shared/SRC . # Gerekli OrtamlarÄ± Kur flatpak remote-
+add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
+flatpak remote-add --if-not-exists flathub-beta https://flathub.org/beta-repo/
+flathub-beta.flatpakrepo flatpak update && flatpak upgrade flatpak install
+flathub org.freedesktop.{Platform,Sdk}//22.08 # Paketle flatpak-builder --user
+--install --force-clean build-dir org.kekikakademi.ntvHaber.yml # ArtÄ±klarÄ±
 Temizle rm -rf .flatpak* .vscode build-dir && find . | grep -E "
 (__pycache__|\.pyc|\.pyo$)" | xargs rm -rf # ÃalÄ±ÅtÄ±r flatpak run
 org.kekikakademi.ntvHaber # Paketi KaldÄ±r flatpak uninstall
 org.kekikakademi.ntvHaber ```  --- ## ð Telif HakkÄ± ve Lisans * *Copyright
 (C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU
 GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/
 keyiflerolsun/ntvHaber/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re
```

### Comparing `ntvHaber-1.30.0/README.md` & `ntvHaber-1.30.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
 ```bash
 # Depoyu Çek
 git clone https://github.com/keyiflerolsun/ntvHaber.git
 cd ntvHaber
 
 # Dosyaları al
-mv Shared/* . && rm -rf Shared
+mv Shared/*.yml . && mv Shared/SRC .
 
 # Gerekli Ortamları Kur
 flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
 flatpak remote-add --if-not-exists flathub-beta https://flathub.org/beta-repo/flathub-beta.flatpakrepo
 flatpak update && flatpak upgrade
 flatpak install flathub org.freedesktop.{Platform,Sdk}//22.08
```

#### html2text {}

```diff
@@ -40,20 +40,20 @@
 icons/python.svg] Python ```bash # Depoyu Ãek https://github.com/
 keyiflerolsun/ntvHaber.git cd ntvHaber # Gerekli OrtamlarÄ± Kur pip install -
 U pip setuptools wheel twine # Paketi YÃ¼kle pip install . # ArtÄ±klarÄ±
 Temizle rm -rf build *.egg-info # ÃalÄ±ÅtÄ±r ntvHaber # Paketi KaldÄ±r pip
 uninstall ntvHaber ``` ### [https://raw.githubusercontent.com/keyiflerolsun/
 ntvHaber/main/.github/icons/flatpak.svg] FlatPak ```bash # Depoyu Ãek git
 clone https://github.com/keyiflerolsun/ntvHaber.git cd ntvHaber # DosyalarÄ± al
-mv Shared/* . && rm -rf Shared # Gerekli OrtamlarÄ± Kur flatpak remote-add --
-if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo flatpak
-remote-add --if-not-exists flathub-beta https://flathub.org/beta-repo/flathub-
-beta.flatpakrepo flatpak update && flatpak upgrade flatpak install flathub
-org.freedesktop.{Platform,Sdk}//22.08 # Paketle flatpak-builder --user --
-install --force-clean build-dir org.kekikakademi.ntvHaber.yml # ArtÄ±klarÄ±
+mv Shared/*.yml . && mv Shared/SRC . # Gerekli OrtamlarÄ± Kur flatpak remote-
+add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
+flatpak remote-add --if-not-exists flathub-beta https://flathub.org/beta-repo/
+flathub-beta.flatpakrepo flatpak update && flatpak upgrade flatpak install
+flathub org.freedesktop.{Platform,Sdk}//22.08 # Paketle flatpak-builder --user
+--install --force-clean build-dir org.kekikakademi.ntvHaber.yml # ArtÄ±klarÄ±
 Temizle rm -rf .flatpak* .vscode build-dir && find . | grep -E "
 (__pycache__|\.pyc|\.pyo$)" | xargs rm -rf # ÃalÄ±ÅtÄ±r flatpak run
 org.kekikakademi.ntvHaber # Paketi KaldÄ±r flatpak uninstall
 org.kekikakademi.ntvHaber ```  --- ## ð Telif HakkÄ± ve Lisans * *Copyright
 (C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU
 GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/
 keyiflerolsun/ntvHaber/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re
```

### Comparing `ntvHaber-1.30.0/Shared/org.kekikakademi.ntvHaber.appdata.xml` & `ntvHaber-1.30.1/Shared/org.kekikakademi.ntvHaber.appdata.xml`

 * *Files 1% similar despite different names*

#### Comparing `ntvHaber-1.30.0/Shared/org.kekikakademi.ntvHaber.appdata.xml` & `ntvHaber-1.30.1/Shared/org.kekikakademi.ntvHaber.appdata.xml`

```diff
@@ -25,15 +25,15 @@
       <image>https://raw.githubusercontent.com/keyiflerolsun/ntvHaber/main/.github/icons/SS.png</image>
     </screenshot>
   </screenshots>
   <categories>
     <category>Education</category>
   </categories>
   <releases>
-    <release version="1.30.0" date="2023-05-23">
+    <release version="1.30.1" date="2023-05-23">
       <description>
         <p>Güncellenen Flet yolları ile uygulama yeniden derlenmiştir.</p>
       </description>
     </release>
     <release version="1.10" date="2023-01-22">
       <description>
         <p>Sistem bildirimleri ve sistem tepsisi ikonu..</p>
```

### Comparing `ntvHaber-1.30.0/Shared/org.kekikakademi.ntvHaber.svg` & `ntvHaber-1.30.1/Shared/org.kekikakademi.ntvHaber.svg`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.30.0/ntvHaber/Assets/Logo.png` & `ntvHaber-1.30.1/ntvHaber/Assets/Logo.png`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.30.0/ntvHaber/Assets/favicon.ico` & `ntvHaber-1.30.1/ntvHaber/Assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.30.0/ntvHaber/Assets/favicon.png` & `ntvHaber-1.30.1/ntvHaber/Assets/favicon.png`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.30.0/ntvHaber/Assets/icons/apple-touch-icon-192.png` & `ntvHaber-1.30.1/ntvHaber/Assets/icons/apple-touch-icon-192.png`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.30.0/ntvHaber/Assets/icons/icon-192.png` & `ntvHaber-1.30.1/ntvHaber/Assets/icons/icon-192.png`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.30.0/ntvHaber/Assets/icons/icon-512.png` & `ntvHaber-1.30.1/ntvHaber/Assets/icons/icon-512.png`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.30.0/ntvHaber/Assets/icons/icon-maskable-192.png` & `ntvHaber-1.30.1/ntvHaber/Assets/icons/icon-maskable-192.png`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.30.0/ntvHaber/Assets/icons/icon-maskable-512.png` & `ntvHaber-1.30.1/ntvHaber/Assets/icons/icon-maskable-512.png`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.30.0/ntvHaber/Assets/icons/loading-animation.png` & `ntvHaber-1.30.1/ntvHaber/Assets/icons/loading-animation.png`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.30.0/ntvHaber/Assets/index.html` & `ntvHaber-1.30.1/ntvHaber/Assets/index.html`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.30.0/ntvHaber/Assets/manifest.json` & `ntvHaber-1.30.1/ntvHaber/Assets/manifest.json`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.30.0/ntvHaber/CLI/__init__.py` & `ntvHaber-1.30.1/ntvHaber/CLI/__init__.py`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.30.0/ntvHaber/Layouts/Haberler.py` & `ntvHaber-1.30.1/ntvHaber/Layouts/Haberler.py`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.30.0/ntvHaber/Layouts/KekikFlet.py` & `ntvHaber-1.30.1/ntvHaber/Layouts/KekikFlet.py`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.30.0/ntvHaber/Layouts/Panel.py` & `ntvHaber-1.30.1/ntvHaber/Layouts/Panel.py`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.30.0/ntvHaber/Libs/NTV.py` & `ntvHaber-1.30.1/ntvHaber/Libs/NTV.py`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.30.0/ntvHaber/Libs/__init__.py` & `ntvHaber-1.30.1/ntvHaber/Libs/__init__.py`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.30.0/ntvHaber/__init__.py` & `ntvHaber-1.30.1/ntvHaber/__init__.py`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.30.0/ntvHaber.egg-info/PKG-INFO` & `ntvHaber-1.30.1/ntvHaber.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntvHaber
-Version: 1.30.0
+Version: 1.30.1
 Summary: NTV Son Dakika Haberleri
 Home-page: https://github.com/keyiflerolsun/ntvHaber
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: ntvHaber,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
@@ -112,15 +112,15 @@
 
 ```bash
 # Depoyu Çek
 git clone https://github.com/keyiflerolsun/ntvHaber.git
 cd ntvHaber
 
 # Dosyaları al
-mv Shared/* . && rm -rf Shared
+mv Shared/*.yml . && mv Shared/SRC .
 
 # Gerekli Ortamları Kur
 flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
 flatpak remote-add --if-not-exists flathub-beta https://flathub.org/beta-repo/flathub-beta.flatpakrepo
 flatpak update && flatpak upgrade
 flatpak install flathub org.freedesktop.{Platform,Sdk}//22.08
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ntvHaber Version: 1.30.0 Summary: NTV Son Dakika
+Metadata-Version: 2.1 Name: ntvHaber Version: 1.30.1 Summary: NTV Son Dakika
 Haberleri Home-page: https://github.com/keyiflerolsun/ntvHaber Author:
 keyiflerolsun Author-email: keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 ntvHaber,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE # ð° ntvHaber ![Repo Boyutu](https://img.shields.io/github/repo-size/
@@ -47,20 +47,20 @@
 icons/python.svg] Python ```bash # Depoyu Ãek https://github.com/
 keyiflerolsun/ntvHaber.git cd ntvHaber # Gerekli OrtamlarÄ± Kur pip install -
 U pip setuptools wheel twine # Paketi YÃ¼kle pip install . # ArtÄ±klarÄ±
 Temizle rm -rf build *.egg-info # ÃalÄ±ÅtÄ±r ntvHaber # Paketi KaldÄ±r pip
 uninstall ntvHaber ``` ### [https://raw.githubusercontent.com/keyiflerolsun/
 ntvHaber/main/.github/icons/flatpak.svg] FlatPak ```bash # Depoyu Ãek git
 clone https://github.com/keyiflerolsun/ntvHaber.git cd ntvHaber # DosyalarÄ± al
-mv Shared/* . && rm -rf Shared # Gerekli OrtamlarÄ± Kur flatpak remote-add --
-if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo flatpak
-remote-add --if-not-exists flathub-beta https://flathub.org/beta-repo/flathub-
-beta.flatpakrepo flatpak update && flatpak upgrade flatpak install flathub
-org.freedesktop.{Platform,Sdk}//22.08 # Paketle flatpak-builder --user --
-install --force-clean build-dir org.kekikakademi.ntvHaber.yml # ArtÄ±klarÄ±
+mv Shared/*.yml . && mv Shared/SRC . # Gerekli OrtamlarÄ± Kur flatpak remote-
+add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
+flatpak remote-add --if-not-exists flathub-beta https://flathub.org/beta-repo/
+flathub-beta.flatpakrepo flatpak update && flatpak upgrade flatpak install
+flathub org.freedesktop.{Platform,Sdk}//22.08 # Paketle flatpak-builder --user
+--install --force-clean build-dir org.kekikakademi.ntvHaber.yml # ArtÄ±klarÄ±
 Temizle rm -rf .flatpak* .vscode build-dir && find . | grep -E "
 (__pycache__|\.pyc|\.pyo$)" | xargs rm -rf # ÃalÄ±ÅtÄ±r flatpak run
 org.kekikakademi.ntvHaber # Paketi KaldÄ±r flatpak uninstall
 org.kekikakademi.ntvHaber ```  --- ## ð Telif HakkÄ± ve Lisans * *Copyright
 (C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU
 GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/
 keyiflerolsun/ntvHaber/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re
```

### Comparing `ntvHaber-1.30.0/ntvHaber.egg-info/SOURCES.txt` & `ntvHaber-1.30.1/ntvHaber.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ntvHaber-1.30.0/setup.py` & `ntvHaber-1.30.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 from io         import open
 
 setup(
     # ? Genel Bilgiler
     name         = "ntvHaber",
-    version      = "1.30.0",
+    version      = "1.30.1",
     url          = "https://github.com/keyiflerolsun/ntvHaber",
     description  = "NTV Son Dakika Haberleri",
     keywords     = ["ntvHaber", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
```

