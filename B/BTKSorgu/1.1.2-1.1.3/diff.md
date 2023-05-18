# Comparing `tmp/BTKSorgu-1.1.2.tar.gz` & `tmp/BTKSorgu-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BTKSorgu-1.1.2.tar", last modified: Wed May 17 23:38:07 2023, max compression
+gzip compressed data, was "BTKSorgu-1.1.3.tar", last modified: Thu May 18 19:40:51 2023, max compression
```

## Comparing `BTKSorgu-1.1.2.tar` & `BTKSorgu-1.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:38:07.367685 BTKSorgu-1.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:38:07.367685 BTKSorgu-1.1.2/BTKSorgu/
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-17 23:37:47.000000 BTKSorgu-1.1.2/BTKSorgu/Erisim_Engeli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-17 23:37:47.000000 BTKSorgu-1.1.2/BTKSorgu/KekikGUI.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-17 23:37:47.000000 BTKSorgu-1.1.2/BTKSorgu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-17 23:37:47.000000 BTKSorgu-1.1.2/BTKSorgu/arayuz.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-17 23:37:47.000000 BTKSorgu-1.1.2/BTKSorgu/konsol.py
--rw-r--r--   0 runner    (1001) docker     (123)    15717 2023-05-17 23:37:47.000000 BTKSorgu-1.1.2/BTKSorgu/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:38:07.367685 BTKSorgu-1.1.2/BTKSorgu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-05-17 23:38:07.000000 BTKSorgu-1.1.2/BTKSorgu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-17 23:38:07.000000 BTKSorgu-1.1.2/BTKSorgu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 23:38:07.000000 BTKSorgu-1.1.2/BTKSorgu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-17 23:38:07.000000 BTKSorgu-1.1.2/BTKSorgu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-17 23:38:07.000000 BTKSorgu-1.1.2/BTKSorgu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 23:38:07.000000 BTKSorgu-1.1.2/BTKSorgu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-17 23:37:47.000000 BTKSorgu-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-17 23:37:47.000000 BTKSorgu-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-05-17 23:38:07.367685 BTKSorgu-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-05-17 23:37:47.000000 BTKSorgu-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:38:07.367685 BTKSorgu-1.1.2/Shared/
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-17 23:37:47.000000 BTKSorgu-1.1.2/Shared/org.KekikAkademi.BTKSorgu.appdata.xml
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-17 23:37:47.000000 BTKSorgu-1.1.2/Shared/org.KekikAkademi.BTKSorgu.desktop
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-17 23:37:47.000000 BTKSorgu-1.1.2/Shared/org.KekikAkademi.BTKSorgu.svg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 23:38:07.367685 BTKSorgu-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-17 23:37:47.000000 BTKSorgu-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:40:51.694258 BTKSorgu-1.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:40:51.694258 BTKSorgu-1.1.3/BTKSorgu/
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-18 19:40:30.000000 BTKSorgu-1.1.3/BTKSorgu/Erisim_Engeli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-18 19:40:30.000000 BTKSorgu-1.1.3/BTKSorgu/KekikGUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-18 19:40:30.000000 BTKSorgu-1.1.3/BTKSorgu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-18 19:40:30.000000 BTKSorgu-1.1.3/BTKSorgu/arayuz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-18 19:40:30.000000 BTKSorgu-1.1.3/BTKSorgu/konsol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15717 2023-05-18 19:40:30.000000 BTKSorgu-1.1.3/BTKSorgu/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:40:51.694258 BTKSorgu-1.1.3/BTKSorgu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-05-18 19:40:51.000000 BTKSorgu-1.1.3/BTKSorgu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 19:40:51.000000 BTKSorgu-1.1.3/BTKSorgu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 19:40:51.000000 BTKSorgu-1.1.3/BTKSorgu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-18 19:40:51.000000 BTKSorgu-1.1.3/BTKSorgu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-18 19:40:51.000000 BTKSorgu-1.1.3/BTKSorgu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-18 19:40:51.000000 BTKSorgu-1.1.3/BTKSorgu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 19:40:30.000000 BTKSorgu-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-18 19:40:30.000000 BTKSorgu-1.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-05-18 19:40:51.694258 BTKSorgu-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-05-18 19:40:30.000000 BTKSorgu-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:40:51.694258 BTKSorgu-1.1.3/Shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-18 19:40:30.000000 BTKSorgu-1.1.3/Shared/org.KekikAkademi.BTKSorgu.appdata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-18 19:40:30.000000 BTKSorgu-1.1.3/Shared/org.KekikAkademi.BTKSorgu.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-18 19:40:30.000000 BTKSorgu-1.1.3/Shared/org.KekikAkademi.BTKSorgu.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 19:40:51.694258 BTKSorgu-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-18 19:40:30.000000 BTKSorgu-1.1.3/setup.py
```

### Comparing `BTKSorgu-1.1.2/BTKSorgu/Erisim_Engeli.py` & `BTKSorgu-1.1.3/BTKSorgu/Erisim_Engeli.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.1.2/BTKSorgu/KekikGUI.py` & `BTKSorgu-1.1.3/BTKSorgu/KekikGUI.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.1.2/BTKSorgu/arayuz.py` & `BTKSorgu-1.1.3/BTKSorgu/arayuz.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.1.2/BTKSorgu/konsol.py` & `BTKSorgu-1.1.3/BTKSorgu/konsol.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.1.2/BTKSorgu/logo.png` & `BTKSorgu-1.1.3/BTKSorgu/logo.png`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.1.2/BTKSorgu.egg-info/PKG-INFO` & `BTKSorgu-1.1.3/BTKSorgu.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTKSorgu
-Version: 1.1.2
+Version: 1.1.3
 Summary: Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu
 Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: BTKSorgu,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,63 +12,64 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🔍 BTKSorgu
 
-![Repo Boyutu](https://img.shields.io/github/repo-size/keyiflerolsun/BTKSorgu?logo=git&logoColor=white)
-![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/BTKSorgu&title=Görüntülenme)
+[![Repo Boyutu](https://img.shields.io/github/repo-size/keyiflerolsun/BTKSorgu?logo=git&logoColor=white)](#)
+[![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/BTKSorgu&title=Görüntülenme)](#)
 <a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/☕️-Kahve Ismarla-ffdd00" title="☕️ Kahve Ismarla" style="padding-left:5px;"></a>
 
-![Python Version](https://img.shields.io/pypi/pyversions/BTKSorgu?logo=python&logoColor=white)
-![License](https://img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white)
-![Status](https://img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white)
+[![Python Version](https://img.shields.io/pypi/pyversions/BTKSorgu?logo=python&logoColor=white)](#)
+[![License](https://img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white)](#)
+[![Status](https://img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white)](#)
 
 [![PyPI](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/project/BTKSorgu)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/project/BTKSorgu)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/project/BTKSorgu)
 
-[![PyPI Yükle](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml/badge.svg)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml)
+[![PyPI Yükleyici](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/pypiYukle.yml/badge.svg)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/pypiYukle.yml)
+[![Flatpak Yükleyici](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/flatpakYukle.yml/badge.svg)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/flatpakYukle.yml)
 
 [![FlatHub](https://img.shields.io/flathub/v/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
 [![FlatHub - Downloads](https://img.shields.io/flathub/downloads/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
 
 *Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu..*
 
-![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png)
+[![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png)](#)
 
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🚀 Kurulum
 
-### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg"> PyPi (Lib - CLI - UI)
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg"></a> PyPi (Lib - CLI - UI)
 
 ```bash
 # Yüklemek
 pip install BTKSorgu
 
 # Güncellemek
 pip install -U BTKSorgu
 ```
 
-### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/flathub.svg"> FlatHub (UI)
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/flathub.svg"></a> FlatHub (UI)
 
 ```bash
 # Yüklemek
 flatpak install flathub org.KekikAkademi.BTKSorgu
 
 # Çalıştırmak
 flatpak run org.KekikAkademi.BTKSorgu
 ```
 
 ## 📝 Kullanım
 
-### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg"> Lib
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg"></a> Lib
 
 ```python
 from BTKSorgu import BTKSorgu
 from time     import time
 
 basla = time()
 print(BTKSorgu("redtube.com"))
@@ -79,64 +80,42 @@
     # » xnxx.com, 23/02/2008 tarihli ve 410.01.02.2008-054003 sayılı Telekomünikasyon İletişim Başkanlığı kararıyla erişime engellenmiştir.
 bitir = time()
 
 print(bitir-basla)
     # » 8.352766513824463
 ```
 
-### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/iterm2.svg"> CLI
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/iterm2.svg"></a> CLI
 
 ```bash
 BTKSorgu keyiflerolsun.dev
 
 # > Bilgi Teknolojileri ve İletişim Kurumu tarafından uygulanan bir karar bulunamadı.
 ```
 
-### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/freedesktop.svg"> UI
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/freedesktop.svg"></a> UI
 
 ```bash
 BTKSorguGUI
 
 # veya
 
 flatpak run org.KekikAkademi.BTKSorgu
 ```
 
-## 🔖 Program Akış Şeması
-
-1. *Oturum Başlat,*
-2. *[https://internet2.btk.gov.tr](https://internet2.btk.gov.tr/) adresine yönlendirmeleri kabul ederek git: kurabiyeleri ye,*
-3. *Dönen kaynak kodundan doğrulama resmini indir,*
-4. *Doğrulama resmini OCR ile harflere dönüştür, boşlukları sil,*
-5. *Sorgu adresini okuduğun doğrulama koduyla birlikte post at,*
-6. *Dönen yanıtı ayrıştırıp edip geri döndür..*
-
-> Bu programın yazılma ve açık kaynak kodlu olarak paylaşılma amacı: *Tarayıcı Otomasyonlarının sebep olduğu  **gereksiz kaynak tüketimi** ve  **zaman kaybının**  önüne geçmeye teşvik etmektir…*
-
-> Tarayıcı Otomasyonu : *[Selenium IDE](https://www.selenium.dev/selenium-ide/)* **-** *[Katalon Automation Recorder](https://www.katalon.com/resources-center/blog/katalon-automation-recorder/)* **-** *[BrowserAutomationStudio](https://bablosoft.com/shop/BrowserAutomationStudio)*
-
-> Karşılaştırması : **[Selenium VS Requests](https://www.r10.net/off-topic/2751612-selenium-vs-requests.html)**
-
-## 📝 Proje İlerlemesi
-
-- ✅ **[@raifpy](https://github.com/raifpy)** *tarafından kodlanmış projenin hantal bir bileşeni itinayla `dızz 🐍`'lanmıştır..*
-- ✅ **Selenium** *bağımlılığından dolayı hantal çalışan kod yapısı tamamen ayıklanıp bütün iş* `requests`*'e yaptırılıp ciddi miktarda kaynak ve zaman tasarrufu ettirilmiştir..*
-- ✅ *Kolay erişilebilir olması ve ilham yaratması için* **pypi** *depolarına yüklenmiştir..*
-- ✅ **Tkinter** *ile basit bir arayüz tasarlanmıştır ve eğitim amacıyla Depolara yüklenmiştir..*
-
 ---
 
 <details>
     <summary style="font-weight: bold; font-size: 20px">
-      <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/buddy.svg"> <b>Manuel Derlemek</b>
+      <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/buddy.svg"></a> <b>Kendiniz Paketlemek İsterseniz</b>
       <i>(genişletmek için tıklayın!)</i>
     </summary>
     <br/>
 
-### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg"> Python
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg"></a> Python
 
 ```bash
 # Depoyu Çek
 https://github.com/keyiflerolsun/BTKSorgu.git
 cd BTKSorgu
 
 # Gerekli Ortamları Kur
@@ -152,23 +131,22 @@
 BTKSorgu     # CLI
 BTKSorguGUI  # GUI
 
 # Paketi Kaldır
 pip uninstall BTKSorgu
 ```
 
-### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/flatpak.svg"> FlatPak
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/flatpak.svg"></a> FlatPak
 
 ```bash
-# Depoyu Çek
-git clone https://github.com/keyiflerolsun/flathub.git
-cd flathub
+git clone https://github.com/keyiflerolsun/BTKSorgu.git
+cd BTKSorgu
 
-# Dala Geç
-git checkout org.KekikAkademi.BTKSorgu
+# Dosyaları al
+mv Shared/*.yml . && mv Shared/SRC .
 
 # Gerekli Ortamları Kur
 flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
 flatpak remote-add --if-not-exists flathub-beta https://flathub.org/beta-repo/flathub-beta.flatpakrepo
 flatpak update && flatpak upgrade
 flatpak install flathub org.freedesktop.{Platform,Sdk}//22.08
 
@@ -185,14 +163,36 @@
 flatpak uninstall org.KekikAkademi.BTKSorgu
 ```
 
 </details>
 
 ---
 
+## 🔖 Program Akış Şeması
+
+1. *Oturum Başlat,*
+2. *[https://internet2.btk.gov.tr](https://internet2.btk.gov.tr/) adresine yönlendirmeleri kabul ederek git: kurabiyeleri ye,*
+3. *Dönen kaynak kodundan doğrulama resmini indir,*
+4. *Doğrulama resmini OCR ile harflere dönüştür, boşlukları sil,*
+5. *Sorgu adresini okuduğun doğrulama koduyla birlikte post at,*
+6. *Dönen yanıtı ayrıştırıp edip geri döndür..*
+
+> Bu programın yazılma ve açık kaynak kodlu olarak paylaşılma amacı: *Tarayıcı Otomasyonlarının sebep olduğu  **gereksiz kaynak tüketimi** ve  **zaman kaybının**  önüne geçmeye teşvik etmektir…*
+
+> Tarayıcı Otomasyonu : *[Selenium IDE](https://www.selenium.dev/selenium-ide/)* **-** *[Katalon Automation Recorder](https://www.katalon.com/resources-center/blog/katalon-automation-recorder/)* **-** *[BrowserAutomationStudio](https://bablosoft.com/shop/BrowserAutomationStudio)*
+
+> Karşılaştırması : **[Selenium VS Requests](https://www.r10.net/off-topic/2751612-selenium-vs-requests.html)**
+
+## 📝 Proje İlerlemesi
+
+- ✅ **[@raifpy](https://github.com/raifpy)** *tarafından kodlanmış projenin hantal bir bileşeni itinayla `dızz 🐍`'lanmıştır..*
+- ✅ **Selenium** *bağımlılığından dolayı hantal çalışan kod yapısı tamamen ayıklanıp bütün iş* `requests`*'e yaptırılıp ciddi miktarda kaynak ve zaman tasarrufu ettirilmiştir..*
+- ✅ *Kolay erişilebilir olması ve ilham yaratması için* **pypi** *depolarına yüklenmiştir..*
+- ✅ **Tkinter** *ile basit bir arayüz tasarlanmıştır ve eğitim amacıyla Depolara yüklenmiştir..*
+
 ## 🌐 Telif Hakkı ve Lisans
 
 * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
 * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/BTKSorgu/blob/master/LICENSE) *Koşullarına göre lisanslanmıştır..*
 
 ## ♻️ İletişim
```

#### html2text {}

```diff
@@ -1,40 +1,43 @@
-Metadata-Version: 2.1 Name: BTKSorgu Version: 1.1.2 Summary: Hedef websitesinin
+Metadata-Version: 2.1 Name: BTKSorgu Version: 1.1.3 Summary: Hedef websitesinin
 BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
 keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
-LICENSE # ð BTKSorgu ![Repo Boyutu](https://img.shields.io/github/repo-size/
-keyiflerolsun/BTKSorgu?logo=git&logoColor=white) ![GÃ¶rÃ¼ntÃ¼lenme](https://
-hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/
-keyiflerolsun/BTKSorgu&title=GÃ¶rÃ¼ntÃ¼lenme) [https://img.shields.io/badge/
-âï¸-Kahve_Ismarla-ffdd00] ![Python Version](https://img.shields.io/pypi/
-pyversions/BTKSorgu?logo=python&logoColor=white) ![License](https://
-img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white) ![Status](https://
-img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white) [!
-[PyPI](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white)]
+LICENSE # ð BTKSorgu [![Repo Boyutu](https://img.shields.io/github/repo-
+size/keyiflerolsun/BTKSorgu?logo=git&logoColor=white)](#) [![GÃ¶rÃ¼ntÃ¼lenme]
+(https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/
+keyiflerolsun/BTKSorgu&title=GÃ¶rÃ¼ntÃ¼lenme)](#) [https://img.shields.io/
+badge/âï¸-Kahve_Ismarla-ffdd00] [![Python Version](https://img.shields.io/
+pypi/pyversions/BTKSorgu?logo=python&logoColor=white)](#) [![License](https://
+img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white)](#) [![Status](https:/
+/img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white)](#)
+[![PyPI](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white)]
 (https://pypi.org/project/BTKSorgu) [![PyPI - Downloads](https://
 img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/
 project/BTKSorgu) [![PyPI - Wheel](https://img.shields.io/pypi/wheel/
 BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/project/BTKSorgu) [![PyPI
-YÃ¼kle](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/
-KekikFlow.yml/badge.svg)](https://github.com/keyiflerolsun/BTKSorgu/actions/
-workflows/KekikFlow.yml) [![FlatHub](https://img.shields.io/flathub/v/
+YÃ¼kleyici](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/
+pypiYukle.yml/badge.svg)](https://github.com/keyiflerolsun/BTKSorgu/actions/
+workflows/pypiYukle.yml) [![Flatpak YÃ¼kleyici](https://github.com/
+keyiflerolsun/BTKSorgu/actions/workflows/flatpakYukle.yml/badge.svg)](https://
+github.com/keyiflerolsun/BTKSorgu/actions/workflows/flatpakYukle.yml) [!
+[FlatHub](https://img.shields.io/flathub/v/
 org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/
 tr/apps/org.KekikAkademi.BTKSorgu) [![FlatHub - Downloads](https://
 img.shields.io/flathub/downloads/
 org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/
 tr/apps/org.KekikAkademi.BTKSorgu) *Hedef websitesinin BTK TarafÄ±ndan EriÅim
-Engeli Sorgusu..* ![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/
-BTKSorgu/main/.github/icons/SS.png) [![ForTheBadge made-with-python](https://
-ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
-[![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-
+Engeli Sorgusu..* [![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/
+BTKSorgu/main/.github/icons/SS.png)](#) [![ForTheBadge made-with-python](https:
+//ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/
+) [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-
 with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð Kurulum ### [https:/
 /raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg]
 PyPi (Lib - CLI - UI) ```bash # YÃ¼klemek pip install BTKSorgu # GÃ¼ncellemek
 pip install -U BTKSorgu ``` ### [https://raw.githubusercontent.com/
 keyiflerolsun/BTKSorgu/main/.github/icons/flathub.svg] FlatHub (UI) ```bash #
 YÃ¼klemek flatpak install flathub org.KekikAkademi.BTKSorgu # ÃalÄ±ÅtÄ±rmak
 flatpak run org.KekikAkademi.BTKSorgu ``` ## ð KullanÄ±m ### [https://
@@ -48,59 +51,57 @@
 410.01.02.2008-054003 sayÄ±lÄ± TelekomÃ¼nikasyon Ä°letiÅim BaÅkanlÄ±ÄÄ±
 kararÄ±yla eriÅime engellenmiÅtir. bitir = time() print(bitir-basla) # Â»
 8.352766513824463 ``` ### [https://raw.githubusercontent.com/keyiflerolsun/
 BTKSorgu/main/.github/icons/iterm2.svg] CLI ```bash BTKSorgu keyiflerolsun.dev
 # > Bilgi Teknolojileri ve Ä°letiÅim Kurumu tarafÄ±ndan uygulanan bir karar
 bulunamadÄ±. ``` ### [https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/
 main/.github/icons/freedesktop.svg] UI ```bash BTKSorguGUI # veya flatpak run
-org.KekikAkademi.BTKSorgu ``` ## ð Program AkÄ±Å ÅemasÄ± 1. *Oturum
-BaÅlat,* 2. *[https://internet2.btk.gov.tr](https://internet2.btk.gov.tr/
-) adresine yÃ¶nlendirmeleri kabul ederek git: kurabiyeleri ye,* 3. *DÃ¶nen
-kaynak kodundan doÄrulama resmini indir,* 4. *DoÄrulama resmini OCR ile
-harflere dÃ¶nÃ¼ÅtÃ¼r, boÅluklarÄ± sil,* 5. *Sorgu adresini okuduÄun
-doÄrulama koduyla birlikte post at,* 6. *DÃ¶nen yanÄ±tÄ± ayrÄ±ÅtÄ±rÄ±p edip
-geri dÃ¶ndÃ¼r..* > Bu programÄ±n yazÄ±lma ve aÃ§Ä±k kaynak kodlu olarak
-paylaÅÄ±lma amacÄ±: *TarayÄ±cÄ± OtomasyonlarÄ±nÄ±n sebep olduÄu **gereksiz
-kaynak tÃ¼ketimi** ve **zaman kaybÄ±nÄ±n** Ã¶nÃ¼ne geÃ§meye teÅvik
+org.KekikAkademi.BTKSorgu ``` ---   [https://raw.githubusercontent.com/
+keyiflerolsun/BTKSorgu/main/.github/icons/buddy.svg] Kendiniz Paketlemek
+Ä°sterseniz (geniÅletmek iÃ§in tÄ±klayÄ±n!)
+### [https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/
+icons/python.svg] Python ```bash # Depoyu Ãek https://github.com/
+keyiflerolsun/BTKSorgu.git cd BTKSorgu # Gerekli OrtamlarÄ± Kur pip install -
+U pip setuptools wheel twine # Paketi YÃ¼kle pip install . # ArtÄ±klarÄ±
+Temizle rm -rf build *.egg-info # ÃalÄ±ÅtÄ±r BTKSorgu # CLI BTKSorguGUI # GUI
+# Paketi KaldÄ±r pip uninstall BTKSorgu ``` ### [https://
+raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/
+flatpak.svg] FlatPak ```bash git clone https://github.com/keyiflerolsun/
+BTKSorgu.git cd BTKSorgu # DosyalarÄ± al mv Shared/*.yml . && mv Shared/SRC . #
+Gerekli OrtamlarÄ± Kur flatpak remote-add --if-not-exists flathub https://
+flathub.org/repo/flathub.flatpakrepo flatpak remote-add --if-not-exists
+flathub-beta https://flathub.org/beta-repo/flathub-beta.flatpakrepo flatpak
+update && flatpak upgrade flatpak install flathub org.freedesktop.
+{Platform,Sdk}//22.08 # Paketle flatpak-builder --user --install --force-clean
+build-dir org.KekikAkademi.BTKSorgu.yml # ArtÄ±klarÄ± Temizle rm -rf .flatpak*
+.vscode build-dir && find . | grep -E "(__pycache__|\.pyc|\.pyo$)" | xargs rm -
+rf # ÃalÄ±ÅtÄ±r flatpak run org.KekikAkademi.BTKSorgu # Paketi KaldÄ±r
+flatpak uninstall org.KekikAkademi.BTKSorgu ```  --- ## ð Program AkÄ±Å
+ÅemasÄ± 1. *Oturum BaÅlat,* 2. *[https://internet2.btk.gov.tr](https://
+internet2.btk.gov.tr/) adresine yÃ¶nlendirmeleri kabul ederek git: kurabiyeleri
+ye,* 3. *DÃ¶nen kaynak kodundan doÄrulama resmini indir,* 4. *DoÄrulama
+resmini OCR ile harflere dÃ¶nÃ¼ÅtÃ¼r, boÅluklarÄ± sil,* 5. *Sorgu adresini
+okuduÄun doÄrulama koduyla birlikte post at,* 6. *DÃ¶nen yanÄ±tÄ±
+ayrÄ±ÅtÄ±rÄ±p edip geri dÃ¶ndÃ¼r..* > Bu programÄ±n yazÄ±lma ve aÃ§Ä±k kaynak
+kodlu olarak paylaÅÄ±lma amacÄ±: *TarayÄ±cÄ± OtomasyonlarÄ±nÄ±n sebep olduÄu
+**gereksiz kaynak tÃ¼ketimi** ve **zaman kaybÄ±nÄ±n** Ã¶nÃ¼ne geÃ§meye teÅvik
 etmektirâ¦* > TarayÄ±cÄ± Otomasyonu : *[Selenium IDE](https://
 www.selenium.dev/selenium-ide/)* **-** *[Katalon Automation Recorder](https://
 www.katalon.com/resources-center/blog/katalon-automation-recorder/)* **-** *
 [BrowserAutomationStudio](https://bablosoft.com/shop/BrowserAutomationStudio)*
 > KarÅÄ±laÅtÄ±rmasÄ± : **[Selenium VS Requests](https://www.r10.net/off-
 topic/2751612-selenium-vs-requests.html)** ## ð Proje Ä°lerlemesi - â **
 [@raifpy](https://github.com/raifpy)** *tarafÄ±ndan kodlanmÄ±Å projenin hantal
 bir bileÅeni itinayla `dÄ±zz ð`'lanmÄ±ÅtÄ±r..* - â **Selenium**
 *baÄÄ±mlÄ±lÄ±ÄÄ±ndan dolayÄ± hantal Ã§alÄ±Åan kod yapÄ±sÄ± tamamen
 ayÄ±klanÄ±p bÃ¼tÃ¼n iÅ* `requests`*'e yaptÄ±rÄ±lÄ±p ciddi miktarda kaynak ve
 zaman tasarrufu ettirilmiÅtir..* - â *Kolay eriÅilebilir olmasÄ± ve ilham
 yaratmasÄ± iÃ§in* **pypi** *depolarÄ±na yÃ¼klenmiÅtir..* - â **Tkinter**
 *ile basit bir arayÃ¼z tasarlanmÄ±ÅtÄ±r ve eÄitim amacÄ±yla Depolara
-yÃ¼klenmiÅtir..* ---   [https://raw.githubusercontent.com/keyiflerolsun/
-BTKSorgu/main/.github/icons/buddy.svg] Manuel Derlemek (geniÅletmek iÃ§in
-tÄ±klayÄ±n!)
-### [https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/
-icons/python.svg] Python ```bash # Depoyu Ãek https://github.com/
-keyiflerolsun/BTKSorgu.git cd BTKSorgu # Gerekli OrtamlarÄ± Kur pip install -
-U pip setuptools wheel twine # Paketi YÃ¼kle pip install . # ArtÄ±klarÄ±
-Temizle rm -rf build *.egg-info # ÃalÄ±ÅtÄ±r BTKSorgu # CLI BTKSorguGUI # GUI
-# Paketi KaldÄ±r pip uninstall BTKSorgu ``` ### [https://
-raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/
-flatpak.svg] FlatPak ```bash # Depoyu Ãek git clone https://github.com/
-keyiflerolsun/flathub.git cd flathub # Dala GeÃ§ git checkout
-org.KekikAkademi.BTKSorgu # Gerekli OrtamlarÄ± Kur flatpak remote-add --if-not-
-exists flathub https://flathub.org/repo/flathub.flatpakrepo flatpak remote-add
---if-not-exists flathub-beta https://flathub.org/beta-repo/flathub-
-beta.flatpakrepo flatpak update && flatpak upgrade flatpak install flathub
-org.freedesktop.{Platform,Sdk}//22.08 # Paketle flatpak-builder --user --
-install --force-clean build-dir org.KekikAkademi.BTKSorgu.yml # ArtÄ±klarÄ±
-Temizle rm -rf .flatpak* .vscode build-dir && find . | grep -E "
-(__pycache__|\.pyc|\.pyo$)" | xargs rm -rf # ÃalÄ±ÅtÄ±r flatpak run
-org.KekikAkademi.BTKSorgu # Paketi KaldÄ±r flatpak uninstall
-org.KekikAkademi.BTKSorgu ```  --- ## ð Telif HakkÄ± ve Lisans * *Copyright
-(C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU
-GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/
-keyiflerolsun/BTKSorgu/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re
-lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek
-isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun]
-(https://t.me/KekikKahve) ## ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https:/
-/KekikAkademi.org/Kahve)** *** > **[@KekikAkademi](https://t.me/KekikAkademi)**
-*iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
+yÃ¼klenmiÅtir..* ## ð Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by*
+[keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL
+PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/
+BTKSorgu/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ##
+â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek isterseniz, **Telegram**'dan
+mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ##
+ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
+*** > **[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
```

### Comparing `BTKSorgu-1.1.2/LICENSE` & `BTKSorgu-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.1.2/PKG-INFO` & `BTKSorgu-1.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTKSorgu
-Version: 1.1.2
+Version: 1.1.3
 Summary: Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu
 Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: BTKSorgu,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,63 +12,64 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🔍 BTKSorgu
 
-![Repo Boyutu](https://img.shields.io/github/repo-size/keyiflerolsun/BTKSorgu?logo=git&logoColor=white)
-![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/BTKSorgu&title=Görüntülenme)
+[![Repo Boyutu](https://img.shields.io/github/repo-size/keyiflerolsun/BTKSorgu?logo=git&logoColor=white)](#)
+[![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/BTKSorgu&title=Görüntülenme)](#)
 <a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/☕️-Kahve Ismarla-ffdd00" title="☕️ Kahve Ismarla" style="padding-left:5px;"></a>
 
-![Python Version](https://img.shields.io/pypi/pyversions/BTKSorgu?logo=python&logoColor=white)
-![License](https://img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white)
-![Status](https://img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white)
+[![Python Version](https://img.shields.io/pypi/pyversions/BTKSorgu?logo=python&logoColor=white)](#)
+[![License](https://img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white)](#)
+[![Status](https://img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white)](#)
 
 [![PyPI](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/project/BTKSorgu)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/project/BTKSorgu)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/project/BTKSorgu)
 
-[![PyPI Yükle](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml/badge.svg)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml)
+[![PyPI Yükleyici](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/pypiYukle.yml/badge.svg)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/pypiYukle.yml)
+[![Flatpak Yükleyici](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/flatpakYukle.yml/badge.svg)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/flatpakYukle.yml)
 
 [![FlatHub](https://img.shields.io/flathub/v/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
 [![FlatHub - Downloads](https://img.shields.io/flathub/downloads/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
 
 *Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu..*
 
-![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png)
+[![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png)](#)
 
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🚀 Kurulum
 
-### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg"> PyPi (Lib - CLI - UI)
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg"></a> PyPi (Lib - CLI - UI)
 
 ```bash
 # Yüklemek
 pip install BTKSorgu
 
 # Güncellemek
 pip install -U BTKSorgu
 ```
 
-### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/flathub.svg"> FlatHub (UI)
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/flathub.svg"></a> FlatHub (UI)
 
 ```bash
 # Yüklemek
 flatpak install flathub org.KekikAkademi.BTKSorgu
 
 # Çalıştırmak
 flatpak run org.KekikAkademi.BTKSorgu
 ```
 
 ## 📝 Kullanım
 
-### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg"> Lib
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg"></a> Lib
 
 ```python
 from BTKSorgu import BTKSorgu
 from time     import time
 
 basla = time()
 print(BTKSorgu("redtube.com"))
@@ -79,64 +80,42 @@
     # » xnxx.com, 23/02/2008 tarihli ve 410.01.02.2008-054003 sayılı Telekomünikasyon İletişim Başkanlığı kararıyla erişime engellenmiştir.
 bitir = time()
 
 print(bitir-basla)
     # » 8.352766513824463
 ```
 
-### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/iterm2.svg"> CLI
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/iterm2.svg"></a> CLI
 
 ```bash
 BTKSorgu keyiflerolsun.dev
 
 # > Bilgi Teknolojileri ve İletişim Kurumu tarafından uygulanan bir karar bulunamadı.
 ```
 
-### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/freedesktop.svg"> UI
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/freedesktop.svg"></a> UI
 
 ```bash
 BTKSorguGUI
 
 # veya
 
 flatpak run org.KekikAkademi.BTKSorgu
 ```
 
-## 🔖 Program Akış Şeması
-
-1. *Oturum Başlat,*
-2. *[https://internet2.btk.gov.tr](https://internet2.btk.gov.tr/) adresine yönlendirmeleri kabul ederek git: kurabiyeleri ye,*
-3. *Dönen kaynak kodundan doğrulama resmini indir,*
-4. *Doğrulama resmini OCR ile harflere dönüştür, boşlukları sil,*
-5. *Sorgu adresini okuduğun doğrulama koduyla birlikte post at,*
-6. *Dönen yanıtı ayrıştırıp edip geri döndür..*
-
-> Bu programın yazılma ve açık kaynak kodlu olarak paylaşılma amacı: *Tarayıcı Otomasyonlarının sebep olduğu  **gereksiz kaynak tüketimi** ve  **zaman kaybının**  önüne geçmeye teşvik etmektir…*
-
-> Tarayıcı Otomasyonu : *[Selenium IDE](https://www.selenium.dev/selenium-ide/)* **-** *[Katalon Automation Recorder](https://www.katalon.com/resources-center/blog/katalon-automation-recorder/)* **-** *[BrowserAutomationStudio](https://bablosoft.com/shop/BrowserAutomationStudio)*
-
-> Karşılaştırması : **[Selenium VS Requests](https://www.r10.net/off-topic/2751612-selenium-vs-requests.html)**
-
-## 📝 Proje İlerlemesi
-
-- ✅ **[@raifpy](https://github.com/raifpy)** *tarafından kodlanmış projenin hantal bir bileşeni itinayla `dızz 🐍`'lanmıştır..*
-- ✅ **Selenium** *bağımlılığından dolayı hantal çalışan kod yapısı tamamen ayıklanıp bütün iş* `requests`*'e yaptırılıp ciddi miktarda kaynak ve zaman tasarrufu ettirilmiştir..*
-- ✅ *Kolay erişilebilir olması ve ilham yaratması için* **pypi** *depolarına yüklenmiştir..*
-- ✅ **Tkinter** *ile basit bir arayüz tasarlanmıştır ve eğitim amacıyla Depolara yüklenmiştir..*
-
 ---
 
 <details>
     <summary style="font-weight: bold; font-size: 20px">
-      <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/buddy.svg"> <b>Manuel Derlemek</b>
+      <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/buddy.svg"></a> <b>Kendiniz Paketlemek İsterseniz</b>
       <i>(genişletmek için tıklayın!)</i>
     </summary>
     <br/>
 
-### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg"> Python
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg"></a> Python
 
 ```bash
 # Depoyu Çek
 https://github.com/keyiflerolsun/BTKSorgu.git
 cd BTKSorgu
 
 # Gerekli Ortamları Kur
@@ -152,23 +131,22 @@
 BTKSorgu     # CLI
 BTKSorguGUI  # GUI
 
 # Paketi Kaldır
 pip uninstall BTKSorgu
 ```
 
-### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/flatpak.svg"> FlatPak
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/flatpak.svg"></a> FlatPak
 
 ```bash
-# Depoyu Çek
-git clone https://github.com/keyiflerolsun/flathub.git
-cd flathub
+git clone https://github.com/keyiflerolsun/BTKSorgu.git
+cd BTKSorgu
 
-# Dala Geç
-git checkout org.KekikAkademi.BTKSorgu
+# Dosyaları al
+mv Shared/*.yml . && mv Shared/SRC .
 
 # Gerekli Ortamları Kur
 flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
 flatpak remote-add --if-not-exists flathub-beta https://flathub.org/beta-repo/flathub-beta.flatpakrepo
 flatpak update && flatpak upgrade
 flatpak install flathub org.freedesktop.{Platform,Sdk}//22.08
 
@@ -185,14 +163,36 @@
 flatpak uninstall org.KekikAkademi.BTKSorgu
 ```
 
 </details>
 
 ---
 
+## 🔖 Program Akış Şeması
+
+1. *Oturum Başlat,*
+2. *[https://internet2.btk.gov.tr](https://internet2.btk.gov.tr/) adresine yönlendirmeleri kabul ederek git: kurabiyeleri ye,*
+3. *Dönen kaynak kodundan doğrulama resmini indir,*
+4. *Doğrulama resmini OCR ile harflere dönüştür, boşlukları sil,*
+5. *Sorgu adresini okuduğun doğrulama koduyla birlikte post at,*
+6. *Dönen yanıtı ayrıştırıp edip geri döndür..*
+
+> Bu programın yazılma ve açık kaynak kodlu olarak paylaşılma amacı: *Tarayıcı Otomasyonlarının sebep olduğu  **gereksiz kaynak tüketimi** ve  **zaman kaybının**  önüne geçmeye teşvik etmektir…*
+
+> Tarayıcı Otomasyonu : *[Selenium IDE](https://www.selenium.dev/selenium-ide/)* **-** *[Katalon Automation Recorder](https://www.katalon.com/resources-center/blog/katalon-automation-recorder/)* **-** *[BrowserAutomationStudio](https://bablosoft.com/shop/BrowserAutomationStudio)*
+
+> Karşılaştırması : **[Selenium VS Requests](https://www.r10.net/off-topic/2751612-selenium-vs-requests.html)**
+
+## 📝 Proje İlerlemesi
+
+- ✅ **[@raifpy](https://github.com/raifpy)** *tarafından kodlanmış projenin hantal bir bileşeni itinayla `dızz 🐍`'lanmıştır..*
+- ✅ **Selenium** *bağımlılığından dolayı hantal çalışan kod yapısı tamamen ayıklanıp bütün iş* `requests`*'e yaptırılıp ciddi miktarda kaynak ve zaman tasarrufu ettirilmiştir..*
+- ✅ *Kolay erişilebilir olması ve ilham yaratması için* **pypi** *depolarına yüklenmiştir..*
+- ✅ **Tkinter** *ile basit bir arayüz tasarlanmıştır ve eğitim amacıyla Depolara yüklenmiştir..*
+
 ## 🌐 Telif Hakkı ve Lisans
 
 * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
 * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/BTKSorgu/blob/master/LICENSE) *Koşullarına göre lisanslanmıştır..*
 
 ## ♻️ İletişim
```

#### html2text {}

```diff
@@ -1,40 +1,43 @@
-Metadata-Version: 2.1 Name: BTKSorgu Version: 1.1.2 Summary: Hedef websitesinin
+Metadata-Version: 2.1 Name: BTKSorgu Version: 1.1.3 Summary: Hedef websitesinin
 BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
 keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
-LICENSE # ð BTKSorgu ![Repo Boyutu](https://img.shields.io/github/repo-size/
-keyiflerolsun/BTKSorgu?logo=git&logoColor=white) ![GÃ¶rÃ¼ntÃ¼lenme](https://
-hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/
-keyiflerolsun/BTKSorgu&title=GÃ¶rÃ¼ntÃ¼lenme) [https://img.shields.io/badge/
-âï¸-Kahve_Ismarla-ffdd00] ![Python Version](https://img.shields.io/pypi/
-pyversions/BTKSorgu?logo=python&logoColor=white) ![License](https://
-img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white) ![Status](https://
-img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white) [!
-[PyPI](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white)]
+LICENSE # ð BTKSorgu [![Repo Boyutu](https://img.shields.io/github/repo-
+size/keyiflerolsun/BTKSorgu?logo=git&logoColor=white)](#) [![GÃ¶rÃ¼ntÃ¼lenme]
+(https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/
+keyiflerolsun/BTKSorgu&title=GÃ¶rÃ¼ntÃ¼lenme)](#) [https://img.shields.io/
+badge/âï¸-Kahve_Ismarla-ffdd00] [![Python Version](https://img.shields.io/
+pypi/pyversions/BTKSorgu?logo=python&logoColor=white)](#) [![License](https://
+img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white)](#) [![Status](https:/
+/img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white)](#)
+[![PyPI](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white)]
 (https://pypi.org/project/BTKSorgu) [![PyPI - Downloads](https://
 img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/
 project/BTKSorgu) [![PyPI - Wheel](https://img.shields.io/pypi/wheel/
 BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/project/BTKSorgu) [![PyPI
-YÃ¼kle](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/
-KekikFlow.yml/badge.svg)](https://github.com/keyiflerolsun/BTKSorgu/actions/
-workflows/KekikFlow.yml) [![FlatHub](https://img.shields.io/flathub/v/
+YÃ¼kleyici](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/
+pypiYukle.yml/badge.svg)](https://github.com/keyiflerolsun/BTKSorgu/actions/
+workflows/pypiYukle.yml) [![Flatpak YÃ¼kleyici](https://github.com/
+keyiflerolsun/BTKSorgu/actions/workflows/flatpakYukle.yml/badge.svg)](https://
+github.com/keyiflerolsun/BTKSorgu/actions/workflows/flatpakYukle.yml) [!
+[FlatHub](https://img.shields.io/flathub/v/
 org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/
 tr/apps/org.KekikAkademi.BTKSorgu) [![FlatHub - Downloads](https://
 img.shields.io/flathub/downloads/
 org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/
 tr/apps/org.KekikAkademi.BTKSorgu) *Hedef websitesinin BTK TarafÄ±ndan EriÅim
-Engeli Sorgusu..* ![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/
-BTKSorgu/main/.github/icons/SS.png) [![ForTheBadge made-with-python](https://
-ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
-[![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-
+Engeli Sorgusu..* [![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/
+BTKSorgu/main/.github/icons/SS.png)](#) [![ForTheBadge made-with-python](https:
+//ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/
+) [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-
 with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð Kurulum ### [https:/
 /raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg]
 PyPi (Lib - CLI - UI) ```bash # YÃ¼klemek pip install BTKSorgu # GÃ¼ncellemek
 pip install -U BTKSorgu ``` ### [https://raw.githubusercontent.com/
 keyiflerolsun/BTKSorgu/main/.github/icons/flathub.svg] FlatHub (UI) ```bash #
 YÃ¼klemek flatpak install flathub org.KekikAkademi.BTKSorgu # ÃalÄ±ÅtÄ±rmak
 flatpak run org.KekikAkademi.BTKSorgu ``` ## ð KullanÄ±m ### [https://
@@ -48,59 +51,57 @@
 410.01.02.2008-054003 sayÄ±lÄ± TelekomÃ¼nikasyon Ä°letiÅim BaÅkanlÄ±ÄÄ±
 kararÄ±yla eriÅime engellenmiÅtir. bitir = time() print(bitir-basla) # Â»
 8.352766513824463 ``` ### [https://raw.githubusercontent.com/keyiflerolsun/
 BTKSorgu/main/.github/icons/iterm2.svg] CLI ```bash BTKSorgu keyiflerolsun.dev
 # > Bilgi Teknolojileri ve Ä°letiÅim Kurumu tarafÄ±ndan uygulanan bir karar
 bulunamadÄ±. ``` ### [https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/
 main/.github/icons/freedesktop.svg] UI ```bash BTKSorguGUI # veya flatpak run
-org.KekikAkademi.BTKSorgu ``` ## ð Program AkÄ±Å ÅemasÄ± 1. *Oturum
-BaÅlat,* 2. *[https://internet2.btk.gov.tr](https://internet2.btk.gov.tr/
-) adresine yÃ¶nlendirmeleri kabul ederek git: kurabiyeleri ye,* 3. *DÃ¶nen
-kaynak kodundan doÄrulama resmini indir,* 4. *DoÄrulama resmini OCR ile
-harflere dÃ¶nÃ¼ÅtÃ¼r, boÅluklarÄ± sil,* 5. *Sorgu adresini okuduÄun
-doÄrulama koduyla birlikte post at,* 6. *DÃ¶nen yanÄ±tÄ± ayrÄ±ÅtÄ±rÄ±p edip
-geri dÃ¶ndÃ¼r..* > Bu programÄ±n yazÄ±lma ve aÃ§Ä±k kaynak kodlu olarak
-paylaÅÄ±lma amacÄ±: *TarayÄ±cÄ± OtomasyonlarÄ±nÄ±n sebep olduÄu **gereksiz
-kaynak tÃ¼ketimi** ve **zaman kaybÄ±nÄ±n** Ã¶nÃ¼ne geÃ§meye teÅvik
+org.KekikAkademi.BTKSorgu ``` ---   [https://raw.githubusercontent.com/
+keyiflerolsun/BTKSorgu/main/.github/icons/buddy.svg] Kendiniz Paketlemek
+Ä°sterseniz (geniÅletmek iÃ§in tÄ±klayÄ±n!)
+### [https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/
+icons/python.svg] Python ```bash # Depoyu Ãek https://github.com/
+keyiflerolsun/BTKSorgu.git cd BTKSorgu # Gerekli OrtamlarÄ± Kur pip install -
+U pip setuptools wheel twine # Paketi YÃ¼kle pip install . # ArtÄ±klarÄ±
+Temizle rm -rf build *.egg-info # ÃalÄ±ÅtÄ±r BTKSorgu # CLI BTKSorguGUI # GUI
+# Paketi KaldÄ±r pip uninstall BTKSorgu ``` ### [https://
+raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/
+flatpak.svg] FlatPak ```bash git clone https://github.com/keyiflerolsun/
+BTKSorgu.git cd BTKSorgu # DosyalarÄ± al mv Shared/*.yml . && mv Shared/SRC . #
+Gerekli OrtamlarÄ± Kur flatpak remote-add --if-not-exists flathub https://
+flathub.org/repo/flathub.flatpakrepo flatpak remote-add --if-not-exists
+flathub-beta https://flathub.org/beta-repo/flathub-beta.flatpakrepo flatpak
+update && flatpak upgrade flatpak install flathub org.freedesktop.
+{Platform,Sdk}//22.08 # Paketle flatpak-builder --user --install --force-clean
+build-dir org.KekikAkademi.BTKSorgu.yml # ArtÄ±klarÄ± Temizle rm -rf .flatpak*
+.vscode build-dir && find . | grep -E "(__pycache__|\.pyc|\.pyo$)" | xargs rm -
+rf # ÃalÄ±ÅtÄ±r flatpak run org.KekikAkademi.BTKSorgu # Paketi KaldÄ±r
+flatpak uninstall org.KekikAkademi.BTKSorgu ```  --- ## ð Program AkÄ±Å
+ÅemasÄ± 1. *Oturum BaÅlat,* 2. *[https://internet2.btk.gov.tr](https://
+internet2.btk.gov.tr/) adresine yÃ¶nlendirmeleri kabul ederek git: kurabiyeleri
+ye,* 3. *DÃ¶nen kaynak kodundan doÄrulama resmini indir,* 4. *DoÄrulama
+resmini OCR ile harflere dÃ¶nÃ¼ÅtÃ¼r, boÅluklarÄ± sil,* 5. *Sorgu adresini
+okuduÄun doÄrulama koduyla birlikte post at,* 6. *DÃ¶nen yanÄ±tÄ±
+ayrÄ±ÅtÄ±rÄ±p edip geri dÃ¶ndÃ¼r..* > Bu programÄ±n yazÄ±lma ve aÃ§Ä±k kaynak
+kodlu olarak paylaÅÄ±lma amacÄ±: *TarayÄ±cÄ± OtomasyonlarÄ±nÄ±n sebep olduÄu
+**gereksiz kaynak tÃ¼ketimi** ve **zaman kaybÄ±nÄ±n** Ã¶nÃ¼ne geÃ§meye teÅvik
 etmektirâ¦* > TarayÄ±cÄ± Otomasyonu : *[Selenium IDE](https://
 www.selenium.dev/selenium-ide/)* **-** *[Katalon Automation Recorder](https://
 www.katalon.com/resources-center/blog/katalon-automation-recorder/)* **-** *
 [BrowserAutomationStudio](https://bablosoft.com/shop/BrowserAutomationStudio)*
 > KarÅÄ±laÅtÄ±rmasÄ± : **[Selenium VS Requests](https://www.r10.net/off-
 topic/2751612-selenium-vs-requests.html)** ## ð Proje Ä°lerlemesi - â **
 [@raifpy](https://github.com/raifpy)** *tarafÄ±ndan kodlanmÄ±Å projenin hantal
 bir bileÅeni itinayla `dÄ±zz ð`'lanmÄ±ÅtÄ±r..* - â **Selenium**
 *baÄÄ±mlÄ±lÄ±ÄÄ±ndan dolayÄ± hantal Ã§alÄ±Åan kod yapÄ±sÄ± tamamen
 ayÄ±klanÄ±p bÃ¼tÃ¼n iÅ* `requests`*'e yaptÄ±rÄ±lÄ±p ciddi miktarda kaynak ve
 zaman tasarrufu ettirilmiÅtir..* - â *Kolay eriÅilebilir olmasÄ± ve ilham
 yaratmasÄ± iÃ§in* **pypi** *depolarÄ±na yÃ¼klenmiÅtir..* - â **Tkinter**
 *ile basit bir arayÃ¼z tasarlanmÄ±ÅtÄ±r ve eÄitim amacÄ±yla Depolara
-yÃ¼klenmiÅtir..* ---   [https://raw.githubusercontent.com/keyiflerolsun/
-BTKSorgu/main/.github/icons/buddy.svg] Manuel Derlemek (geniÅletmek iÃ§in
-tÄ±klayÄ±n!)
-### [https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/
-icons/python.svg] Python ```bash # Depoyu Ãek https://github.com/
-keyiflerolsun/BTKSorgu.git cd BTKSorgu # Gerekli OrtamlarÄ± Kur pip install -
-U pip setuptools wheel twine # Paketi YÃ¼kle pip install . # ArtÄ±klarÄ±
-Temizle rm -rf build *.egg-info # ÃalÄ±ÅtÄ±r BTKSorgu # CLI BTKSorguGUI # GUI
-# Paketi KaldÄ±r pip uninstall BTKSorgu ``` ### [https://
-raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/
-flatpak.svg] FlatPak ```bash # Depoyu Ãek git clone https://github.com/
-keyiflerolsun/flathub.git cd flathub # Dala GeÃ§ git checkout
-org.KekikAkademi.BTKSorgu # Gerekli OrtamlarÄ± Kur flatpak remote-add --if-not-
-exists flathub https://flathub.org/repo/flathub.flatpakrepo flatpak remote-add
---if-not-exists flathub-beta https://flathub.org/beta-repo/flathub-
-beta.flatpakrepo flatpak update && flatpak upgrade flatpak install flathub
-org.freedesktop.{Platform,Sdk}//22.08 # Paketle flatpak-builder --user --
-install --force-clean build-dir org.KekikAkademi.BTKSorgu.yml # ArtÄ±klarÄ±
-Temizle rm -rf .flatpak* .vscode build-dir && find . | grep -E "
-(__pycache__|\.pyc|\.pyo$)" | xargs rm -rf # ÃalÄ±ÅtÄ±r flatpak run
-org.KekikAkademi.BTKSorgu # Paketi KaldÄ±r flatpak uninstall
-org.KekikAkademi.BTKSorgu ```  --- ## ð Telif HakkÄ± ve Lisans * *Copyright
-(C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU
-GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/
-keyiflerolsun/BTKSorgu/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re
-lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek
-isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun]
-(https://t.me/KekikKahve) ## ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https:/
-/KekikAkademi.org/Kahve)** *** > **[@KekikAkademi](https://t.me/KekikAkademi)**
-*iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
+yÃ¼klenmiÅtir..* ## ð Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by*
+[keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL
+PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/
+BTKSorgu/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ##
+â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek isterseniz, **Telegram**'dan
+mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ##
+ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
+*** > **[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
```

### Comparing `BTKSorgu-1.1.2/README.md` & `BTKSorgu-1.1.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,58 +1,59 @@
 # 🔍 BTKSorgu
 
-![Repo Boyutu](https://img.shields.io/github/repo-size/keyiflerolsun/BTKSorgu?logo=git&logoColor=white)
-![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/BTKSorgu&title=Görüntülenme)
+[![Repo Boyutu](https://img.shields.io/github/repo-size/keyiflerolsun/BTKSorgu?logo=git&logoColor=white)](#)
+[![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/BTKSorgu&title=Görüntülenme)](#)
 <a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/☕️-Kahve Ismarla-ffdd00" title="☕️ Kahve Ismarla" style="padding-left:5px;"></a>
 
-![Python Version](https://img.shields.io/pypi/pyversions/BTKSorgu?logo=python&logoColor=white)
-![License](https://img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white)
-![Status](https://img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white)
+[![Python Version](https://img.shields.io/pypi/pyversions/BTKSorgu?logo=python&logoColor=white)](#)
+[![License](https://img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white)](#)
+[![Status](https://img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white)](#)
 
 [![PyPI](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/project/BTKSorgu)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/project/BTKSorgu)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/project/BTKSorgu)
 
-[![PyPI Yükle](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml/badge.svg)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml)
+[![PyPI Yükleyici](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/pypiYukle.yml/badge.svg)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/pypiYukle.yml)
+[![Flatpak Yükleyici](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/flatpakYukle.yml/badge.svg)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/flatpakYukle.yml)
 
 [![FlatHub](https://img.shields.io/flathub/v/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
 [![FlatHub - Downloads](https://img.shields.io/flathub/downloads/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
 
 *Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu..*
 
-![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png)
+[![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png)](#)
 
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🚀 Kurulum
 
-### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg"> PyPi (Lib - CLI - UI)
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg"></a> PyPi (Lib - CLI - UI)
 
 ```bash
 # Yüklemek
 pip install BTKSorgu
 
 # Güncellemek
 pip install -U BTKSorgu
 ```
 
-### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/flathub.svg"> FlatHub (UI)
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/flathub.svg"></a> FlatHub (UI)
 
 ```bash
 # Yüklemek
 flatpak install flathub org.KekikAkademi.BTKSorgu
 
 # Çalıştırmak
 flatpak run org.KekikAkademi.BTKSorgu
 ```
 
 ## 📝 Kullanım
 
-### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg"> Lib
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg"></a> Lib
 
 ```python
 from BTKSorgu import BTKSorgu
 from time     import time
 
 basla = time()
 print(BTKSorgu("redtube.com"))
@@ -63,64 +64,42 @@
     # » xnxx.com, 23/02/2008 tarihli ve 410.01.02.2008-054003 sayılı Telekomünikasyon İletişim Başkanlığı kararıyla erişime engellenmiştir.
 bitir = time()
 
 print(bitir-basla)
     # » 8.352766513824463
 ```
 
-### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/iterm2.svg"> CLI
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/iterm2.svg"></a> CLI
 
 ```bash
 BTKSorgu keyiflerolsun.dev
 
 # > Bilgi Teknolojileri ve İletişim Kurumu tarafından uygulanan bir karar bulunamadı.
 ```
 
-### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/freedesktop.svg"> UI
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/freedesktop.svg"></a> UI
 
 ```bash
 BTKSorguGUI
 
 # veya
 
 flatpak run org.KekikAkademi.BTKSorgu
 ```
 
-## 🔖 Program Akış Şeması
-
-1. *Oturum Başlat,*
-2. *[https://internet2.btk.gov.tr](https://internet2.btk.gov.tr/) adresine yönlendirmeleri kabul ederek git: kurabiyeleri ye,*
-3. *Dönen kaynak kodundan doğrulama resmini indir,*
-4. *Doğrulama resmini OCR ile harflere dönüştür, boşlukları sil,*
-5. *Sorgu adresini okuduğun doğrulama koduyla birlikte post at,*
-6. *Dönen yanıtı ayrıştırıp edip geri döndür..*
-
-> Bu programın yazılma ve açık kaynak kodlu olarak paylaşılma amacı: *Tarayıcı Otomasyonlarının sebep olduğu  **gereksiz kaynak tüketimi** ve  **zaman kaybının**  önüne geçmeye teşvik etmektir…*
-
-> Tarayıcı Otomasyonu : *[Selenium IDE](https://www.selenium.dev/selenium-ide/)* **-** *[Katalon Automation Recorder](https://www.katalon.com/resources-center/blog/katalon-automation-recorder/)* **-** *[BrowserAutomationStudio](https://bablosoft.com/shop/BrowserAutomationStudio)*
-
-> Karşılaştırması : **[Selenium VS Requests](https://www.r10.net/off-topic/2751612-selenium-vs-requests.html)**
-
-## 📝 Proje İlerlemesi
-
-- ✅ **[@raifpy](https://github.com/raifpy)** *tarafından kodlanmış projenin hantal bir bileşeni itinayla `dızz 🐍`'lanmıştır..*
-- ✅ **Selenium** *bağımlılığından dolayı hantal çalışan kod yapısı tamamen ayıklanıp bütün iş* `requests`*'e yaptırılıp ciddi miktarda kaynak ve zaman tasarrufu ettirilmiştir..*
-- ✅ *Kolay erişilebilir olması ve ilham yaratması için* **pypi** *depolarına yüklenmiştir..*
-- ✅ **Tkinter** *ile basit bir arayüz tasarlanmıştır ve eğitim amacıyla Depolara yüklenmiştir..*
-
 ---
 
 <details>
     <summary style="font-weight: bold; font-size: 20px">
-      <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/buddy.svg"> <b>Manuel Derlemek</b>
+      <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/buddy.svg"></a> <b>Kendiniz Paketlemek İsterseniz</b>
       <i>(genişletmek için tıklayın!)</i>
     </summary>
     <br/>
 
-### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg"> Python
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg"></a> Python
 
 ```bash
 # Depoyu Çek
 https://github.com/keyiflerolsun/BTKSorgu.git
 cd BTKSorgu
 
 # Gerekli Ortamları Kur
@@ -136,23 +115,22 @@
 BTKSorgu     # CLI
 BTKSorguGUI  # GUI
 
 # Paketi Kaldır
 pip uninstall BTKSorgu
 ```
 
-### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/flatpak.svg"> FlatPak
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/flatpak.svg"></a> FlatPak
 
 ```bash
-# Depoyu Çek
-git clone https://github.com/keyiflerolsun/flathub.git
-cd flathub
+git clone https://github.com/keyiflerolsun/BTKSorgu.git
+cd BTKSorgu
 
-# Dala Geç
-git checkout org.KekikAkademi.BTKSorgu
+# Dosyaları al
+mv Shared/*.yml . && mv Shared/SRC .
 
 # Gerekli Ortamları Kur
 flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
 flatpak remote-add --if-not-exists flathub-beta https://flathub.org/beta-repo/flathub-beta.flatpakrepo
 flatpak update && flatpak upgrade
 flatpak install flathub org.freedesktop.{Platform,Sdk}//22.08
 
@@ -169,14 +147,36 @@
 flatpak uninstall org.KekikAkademi.BTKSorgu
 ```
 
 </details>
 
 ---
 
+## 🔖 Program Akış Şeması
+
+1. *Oturum Başlat,*
+2. *[https://internet2.btk.gov.tr](https://internet2.btk.gov.tr/) adresine yönlendirmeleri kabul ederek git: kurabiyeleri ye,*
+3. *Dönen kaynak kodundan doğrulama resmini indir,*
+4. *Doğrulama resmini OCR ile harflere dönüştür, boşlukları sil,*
+5. *Sorgu adresini okuduğun doğrulama koduyla birlikte post at,*
+6. *Dönen yanıtı ayrıştırıp edip geri döndür..*
+
+> Bu programın yazılma ve açık kaynak kodlu olarak paylaşılma amacı: *Tarayıcı Otomasyonlarının sebep olduğu  **gereksiz kaynak tüketimi** ve  **zaman kaybının**  önüne geçmeye teşvik etmektir…*
+
+> Tarayıcı Otomasyonu : *[Selenium IDE](https://www.selenium.dev/selenium-ide/)* **-** *[Katalon Automation Recorder](https://www.katalon.com/resources-center/blog/katalon-automation-recorder/)* **-** *[BrowserAutomationStudio](https://bablosoft.com/shop/BrowserAutomationStudio)*
+
+> Karşılaştırması : **[Selenium VS Requests](https://www.r10.net/off-topic/2751612-selenium-vs-requests.html)**
+
+## 📝 Proje İlerlemesi
+
+- ✅ **[@raifpy](https://github.com/raifpy)** *tarafından kodlanmış projenin hantal bir bileşeni itinayla `dızz 🐍`'lanmıştır..*
+- ✅ **Selenium** *bağımlılığından dolayı hantal çalışan kod yapısı tamamen ayıklanıp bütün iş* `requests`*'e yaptırılıp ciddi miktarda kaynak ve zaman tasarrufu ettirilmiştir..*
+- ✅ *Kolay erişilebilir olması ve ilham yaratması için* **pypi** *depolarına yüklenmiştir..*
+- ✅ **Tkinter** *ile basit bir arayüz tasarlanmıştır ve eğitim amacıyla Depolara yüklenmiştir..*
+
 ## 🌐 Telif Hakkı ve Lisans
 
 * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
 * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/BTKSorgu/blob/master/LICENSE) *Koşullarına göre lisanslanmıştır..*
 
 ## ♻️ İletişim
```

#### html2text {}

```diff
@@ -1,32 +1,35 @@
-# ð BTKSorgu ![Repo Boyutu](https://img.shields.io/github/repo-size/
-keyiflerolsun/BTKSorgu?logo=git&logoColor=white) ![GÃ¶rÃ¼ntÃ¼lenme](https://
-hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/
-keyiflerolsun/BTKSorgu&title=GÃ¶rÃ¼ntÃ¼lenme) [https://img.shields.io/badge/
-âï¸-Kahve_Ismarla-ffdd00] ![Python Version](https://img.shields.io/pypi/
-pyversions/BTKSorgu?logo=python&logoColor=white) ![License](https://
-img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white) ![Status](https://
-img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white) [!
-[PyPI](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white)]
+# ð BTKSorgu [![Repo Boyutu](https://img.shields.io/github/repo-size/
+keyiflerolsun/BTKSorgu?logo=git&logoColor=white)](#) [![GÃ¶rÃ¼ntÃ¼lenme](https:
+//hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/
+keyiflerolsun/BTKSorgu&title=GÃ¶rÃ¼ntÃ¼lenme)](#) [https://img.shields.io/
+badge/âï¸-Kahve_Ismarla-ffdd00] [![Python Version](https://img.shields.io/
+pypi/pyversions/BTKSorgu?logo=python&logoColor=white)](#) [![License](https://
+img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white)](#) [![Status](https:/
+/img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white)](#)
+[![PyPI](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white)]
 (https://pypi.org/project/BTKSorgu) [![PyPI - Downloads](https://
 img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/
 project/BTKSorgu) [![PyPI - Wheel](https://img.shields.io/pypi/wheel/
 BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/project/BTKSorgu) [![PyPI
-YÃ¼kle](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/
-KekikFlow.yml/badge.svg)](https://github.com/keyiflerolsun/BTKSorgu/actions/
-workflows/KekikFlow.yml) [![FlatHub](https://img.shields.io/flathub/v/
+YÃ¼kleyici](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/
+pypiYukle.yml/badge.svg)](https://github.com/keyiflerolsun/BTKSorgu/actions/
+workflows/pypiYukle.yml) [![Flatpak YÃ¼kleyici](https://github.com/
+keyiflerolsun/BTKSorgu/actions/workflows/flatpakYukle.yml/badge.svg)](https://
+github.com/keyiflerolsun/BTKSorgu/actions/workflows/flatpakYukle.yml) [!
+[FlatHub](https://img.shields.io/flathub/v/
 org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/
 tr/apps/org.KekikAkademi.BTKSorgu) [![FlatHub - Downloads](https://
 img.shields.io/flathub/downloads/
 org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/
 tr/apps/org.KekikAkademi.BTKSorgu) *Hedef websitesinin BTK TarafÄ±ndan EriÅim
-Engeli Sorgusu..* ![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/
-BTKSorgu/main/.github/icons/SS.png) [![ForTheBadge made-with-python](https://
-ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
-[![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-
+Engeli Sorgusu..* [![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/
+BTKSorgu/main/.github/icons/SS.png)](#) [![ForTheBadge made-with-python](https:
+//ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/
+) [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-
 with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð Kurulum ### [https:/
 /raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg]
 PyPi (Lib - CLI - UI) ```bash # YÃ¼klemek pip install BTKSorgu # GÃ¼ncellemek
 pip install -U BTKSorgu ``` ### [https://raw.githubusercontent.com/
 keyiflerolsun/BTKSorgu/main/.github/icons/flathub.svg] FlatHub (UI) ```bash #
 YÃ¼klemek flatpak install flathub org.KekikAkademi.BTKSorgu # ÃalÄ±ÅtÄ±rmak
 flatpak run org.KekikAkademi.BTKSorgu ``` ## ð KullanÄ±m ### [https://
@@ -40,59 +43,57 @@
 410.01.02.2008-054003 sayÄ±lÄ± TelekomÃ¼nikasyon Ä°letiÅim BaÅkanlÄ±ÄÄ±
 kararÄ±yla eriÅime engellenmiÅtir. bitir = time() print(bitir-basla) # Â»
 8.352766513824463 ``` ### [https://raw.githubusercontent.com/keyiflerolsun/
 BTKSorgu/main/.github/icons/iterm2.svg] CLI ```bash BTKSorgu keyiflerolsun.dev
 # > Bilgi Teknolojileri ve Ä°letiÅim Kurumu tarafÄ±ndan uygulanan bir karar
 bulunamadÄ±. ``` ### [https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/
 main/.github/icons/freedesktop.svg] UI ```bash BTKSorguGUI # veya flatpak run
-org.KekikAkademi.BTKSorgu ``` ## ð Program AkÄ±Å ÅemasÄ± 1. *Oturum
-BaÅlat,* 2. *[https://internet2.btk.gov.tr](https://internet2.btk.gov.tr/
-) adresine yÃ¶nlendirmeleri kabul ederek git: kurabiyeleri ye,* 3. *DÃ¶nen
-kaynak kodundan doÄrulama resmini indir,* 4. *DoÄrulama resmini OCR ile
-harflere dÃ¶nÃ¼ÅtÃ¼r, boÅluklarÄ± sil,* 5. *Sorgu adresini okuduÄun
-doÄrulama koduyla birlikte post at,* 6. *DÃ¶nen yanÄ±tÄ± ayrÄ±ÅtÄ±rÄ±p edip
-geri dÃ¶ndÃ¼r..* > Bu programÄ±n yazÄ±lma ve aÃ§Ä±k kaynak kodlu olarak
-paylaÅÄ±lma amacÄ±: *TarayÄ±cÄ± OtomasyonlarÄ±nÄ±n sebep olduÄu **gereksiz
-kaynak tÃ¼ketimi** ve **zaman kaybÄ±nÄ±n** Ã¶nÃ¼ne geÃ§meye teÅvik
+org.KekikAkademi.BTKSorgu ``` ---   [https://raw.githubusercontent.com/
+keyiflerolsun/BTKSorgu/main/.github/icons/buddy.svg] Kendiniz Paketlemek
+Ä°sterseniz (geniÅletmek iÃ§in tÄ±klayÄ±n!)
+### [https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/
+icons/python.svg] Python ```bash # Depoyu Ãek https://github.com/
+keyiflerolsun/BTKSorgu.git cd BTKSorgu # Gerekli OrtamlarÄ± Kur pip install -
+U pip setuptools wheel twine # Paketi YÃ¼kle pip install . # ArtÄ±klarÄ±
+Temizle rm -rf build *.egg-info # ÃalÄ±ÅtÄ±r BTKSorgu # CLI BTKSorguGUI # GUI
+# Paketi KaldÄ±r pip uninstall BTKSorgu ``` ### [https://
+raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/
+flatpak.svg] FlatPak ```bash git clone https://github.com/keyiflerolsun/
+BTKSorgu.git cd BTKSorgu # DosyalarÄ± al mv Shared/*.yml . && mv Shared/SRC . #
+Gerekli OrtamlarÄ± Kur flatpak remote-add --if-not-exists flathub https://
+flathub.org/repo/flathub.flatpakrepo flatpak remote-add --if-not-exists
+flathub-beta https://flathub.org/beta-repo/flathub-beta.flatpakrepo flatpak
+update && flatpak upgrade flatpak install flathub org.freedesktop.
+{Platform,Sdk}//22.08 # Paketle flatpak-builder --user --install --force-clean
+build-dir org.KekikAkademi.BTKSorgu.yml # ArtÄ±klarÄ± Temizle rm -rf .flatpak*
+.vscode build-dir && find . | grep -E "(__pycache__|\.pyc|\.pyo$)" | xargs rm -
+rf # ÃalÄ±ÅtÄ±r flatpak run org.KekikAkademi.BTKSorgu # Paketi KaldÄ±r
+flatpak uninstall org.KekikAkademi.BTKSorgu ```  --- ## ð Program AkÄ±Å
+ÅemasÄ± 1. *Oturum BaÅlat,* 2. *[https://internet2.btk.gov.tr](https://
+internet2.btk.gov.tr/) adresine yÃ¶nlendirmeleri kabul ederek git: kurabiyeleri
+ye,* 3. *DÃ¶nen kaynak kodundan doÄrulama resmini indir,* 4. *DoÄrulama
+resmini OCR ile harflere dÃ¶nÃ¼ÅtÃ¼r, boÅluklarÄ± sil,* 5. *Sorgu adresini
+okuduÄun doÄrulama koduyla birlikte post at,* 6. *DÃ¶nen yanÄ±tÄ±
+ayrÄ±ÅtÄ±rÄ±p edip geri dÃ¶ndÃ¼r..* > Bu programÄ±n yazÄ±lma ve aÃ§Ä±k kaynak
+kodlu olarak paylaÅÄ±lma amacÄ±: *TarayÄ±cÄ± OtomasyonlarÄ±nÄ±n sebep olduÄu
+**gereksiz kaynak tÃ¼ketimi** ve **zaman kaybÄ±nÄ±n** Ã¶nÃ¼ne geÃ§meye teÅvik
 etmektirâ¦* > TarayÄ±cÄ± Otomasyonu : *[Selenium IDE](https://
 www.selenium.dev/selenium-ide/)* **-** *[Katalon Automation Recorder](https://
 www.katalon.com/resources-center/blog/katalon-automation-recorder/)* **-** *
 [BrowserAutomationStudio](https://bablosoft.com/shop/BrowserAutomationStudio)*
 > KarÅÄ±laÅtÄ±rmasÄ± : **[Selenium VS Requests](https://www.r10.net/off-
 topic/2751612-selenium-vs-requests.html)** ## ð Proje Ä°lerlemesi - â **
 [@raifpy](https://github.com/raifpy)** *tarafÄ±ndan kodlanmÄ±Å projenin hantal
 bir bileÅeni itinayla `dÄ±zz ð`'lanmÄ±ÅtÄ±r..* - â **Selenium**
 *baÄÄ±mlÄ±lÄ±ÄÄ±ndan dolayÄ± hantal Ã§alÄ±Åan kod yapÄ±sÄ± tamamen
 ayÄ±klanÄ±p bÃ¼tÃ¼n iÅ* `requests`*'e yaptÄ±rÄ±lÄ±p ciddi miktarda kaynak ve
 zaman tasarrufu ettirilmiÅtir..* - â *Kolay eriÅilebilir olmasÄ± ve ilham
 yaratmasÄ± iÃ§in* **pypi** *depolarÄ±na yÃ¼klenmiÅtir..* - â **Tkinter**
 *ile basit bir arayÃ¼z tasarlanmÄ±ÅtÄ±r ve eÄitim amacÄ±yla Depolara
-yÃ¼klenmiÅtir..* ---   [https://raw.githubusercontent.com/keyiflerolsun/
-BTKSorgu/main/.github/icons/buddy.svg] Manuel Derlemek (geniÅletmek iÃ§in
-tÄ±klayÄ±n!)
-### [https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/
-icons/python.svg] Python ```bash # Depoyu Ãek https://github.com/
-keyiflerolsun/BTKSorgu.git cd BTKSorgu # Gerekli OrtamlarÄ± Kur pip install -
-U pip setuptools wheel twine # Paketi YÃ¼kle pip install . # ArtÄ±klarÄ±
-Temizle rm -rf build *.egg-info # ÃalÄ±ÅtÄ±r BTKSorgu # CLI BTKSorguGUI # GUI
-# Paketi KaldÄ±r pip uninstall BTKSorgu ``` ### [https://
-raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/
-flatpak.svg] FlatPak ```bash # Depoyu Ãek git clone https://github.com/
-keyiflerolsun/flathub.git cd flathub # Dala GeÃ§ git checkout
-org.KekikAkademi.BTKSorgu # Gerekli OrtamlarÄ± Kur flatpak remote-add --if-not-
-exists flathub https://flathub.org/repo/flathub.flatpakrepo flatpak remote-add
---if-not-exists flathub-beta https://flathub.org/beta-repo/flathub-
-beta.flatpakrepo flatpak update && flatpak upgrade flatpak install flathub
-org.freedesktop.{Platform,Sdk}//22.08 # Paketle flatpak-builder --user --
-install --force-clean build-dir org.KekikAkademi.BTKSorgu.yml # ArtÄ±klarÄ±
-Temizle rm -rf .flatpak* .vscode build-dir && find . | grep -E "
-(__pycache__|\.pyc|\.pyo$)" | xargs rm -rf # ÃalÄ±ÅtÄ±r flatpak run
-org.KekikAkademi.BTKSorgu # Paketi KaldÄ±r flatpak uninstall
-org.KekikAkademi.BTKSorgu ```  --- ## ð Telif HakkÄ± ve Lisans * *Copyright
-(C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU
-GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/
-keyiflerolsun/BTKSorgu/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re
-lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek
-isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun]
-(https://t.me/KekikKahve) ## ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https:/
-/KekikAkademi.org/Kahve)** *** > **[@KekikAkademi](https://t.me/KekikAkademi)**
-*iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
+yÃ¼klenmiÅtir..* ## ð Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by*
+[keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL
+PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/
+BTKSorgu/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ##
+â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek isterseniz, **Telegram**'dan
+mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ##
+ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
+*** > **[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
```

### Comparing `BTKSorgu-1.1.2/Shared/org.KekikAkademi.BTKSorgu.appdata.xml` & `BTKSorgu-1.1.3/Shared/org.KekikAkademi.BTKSorgu.appdata.xml`

 * *Files 7% similar despite different names*

#### Comparing `BTKSorgu-1.1.2/Shared/org.KekikAkademi.BTKSorgu.appdata.xml` & `BTKSorgu-1.1.3/Shared/org.KekikAkademi.BTKSorgu.appdata.xml`

```diff
@@ -25,17 +25,22 @@
       <image>https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png</image>
     </screenshot>
   </screenshots>
   <categories>
     <category>Education</category>
   </categories>
   <releases>
+    <release version="1.1.3" date="2023-5-18">
+      <description>
+        <p>Github aksiyonlarıyla otomatik paketlenme ve yayınlama eklendi..</p>
+      </description>
+    </release>
     <release version="1.1.2" date="2023-5-18">
       <description>
-        <p>Readme Genişletildi ve Manuel Derleme Aşamaları Eklendi..</p>
+        <p>Readme Genişletildi ve Manuel Paketleme Aşamaları Eklendi..</p>
       </description>
     </release>
     <release version="1.0.8" date="2023-5-17">
       <description>
         <p>Readme Düzenlendi..</p>
       </description>
     </release>
```

### Comparing `BTKSorgu-1.1.2/Shared/org.KekikAkademi.BTKSorgu.svg` & `BTKSorgu-1.1.3/Shared/org.KekikAkademi.BTKSorgu.svg`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.1.2/setup.py` & `BTKSorgu-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 from io         import open
 
 setup(
     # ? Genel Bilgiler
     name         = "BTKSorgu",
-    version      = "1.1.2",
+    version      = "1.1.3",
     url          = "https://github.com/keyiflerolsun/E-Fatura_Sorgu",
     description  = "Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu",
     keywords     = ["BTKSorgu", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
```

