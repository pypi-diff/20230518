# Comparing `tmp/BTKSorgu-1.0.8.tar.gz` & `tmp/BTKSorgu-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BTKSorgu-1.0.8.tar", last modified: Wed May 17 19:05:41 2023, max compression
+gzip compressed data, was "BTKSorgu-1.0.9.tar", last modified: Wed May 17 22:53:15 2023, max compression
```

## Comparing `BTKSorgu-1.0.8.tar` & `BTKSorgu-1.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:05:41.723685 BTKSorgu-1.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:05:41.719685 BTKSorgu-1.0.8/BTKSorgu/
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-17 19:05:21.000000 BTKSorgu-1.0.8/BTKSorgu/Erisim_Engeli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-17 19:05:21.000000 BTKSorgu-1.0.8/BTKSorgu/KekikGUI.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-17 19:05:21.000000 BTKSorgu-1.0.8/BTKSorgu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-17 19:05:21.000000 BTKSorgu-1.0.8/BTKSorgu/arayuz.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-17 19:05:21.000000 BTKSorgu-1.0.8/BTKSorgu/konsol.py
--rw-r--r--   0 runner    (1001) docker     (123)    15717 2023-05-17 19:05:21.000000 BTKSorgu-1.0.8/BTKSorgu/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:05:41.723685 BTKSorgu-1.0.8/BTKSorgu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-05-17 19:05:41.000000 BTKSorgu-1.0.8/BTKSorgu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-17 19:05:41.000000 BTKSorgu-1.0.8/BTKSorgu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 19:05:41.000000 BTKSorgu-1.0.8/BTKSorgu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-17 19:05:41.000000 BTKSorgu-1.0.8/BTKSorgu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-17 19:05:41.000000 BTKSorgu-1.0.8/BTKSorgu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 19:05:41.000000 BTKSorgu-1.0.8/BTKSorgu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-17 19:05:21.000000 BTKSorgu-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-17 19:05:21.000000 BTKSorgu-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-05-17 19:05:41.723685 BTKSorgu-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-05-17 19:05:21.000000 BTKSorgu-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:05:41.723685 BTKSorgu-1.0.8/Shared/
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-17 19:05:21.000000 BTKSorgu-1.0.8/Shared/org.KekikAkademi.BTKSorgu.appdata.xml
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-17 19:05:21.000000 BTKSorgu-1.0.8/Shared/org.KekikAkademi.BTKSorgu.desktop
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-17 19:05:21.000000 BTKSorgu-1.0.8/Shared/org.KekikAkademi.BTKSorgu.svg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 19:05:41.723685 BTKSorgu-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-17 19:05:21.000000 BTKSorgu-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:53:15.168375 BTKSorgu-1.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:53:15.168375 BTKSorgu-1.0.9/BTKSorgu/
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-17 22:52:55.000000 BTKSorgu-1.0.9/BTKSorgu/Erisim_Engeli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-17 22:52:55.000000 BTKSorgu-1.0.9/BTKSorgu/KekikGUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-17 22:52:55.000000 BTKSorgu-1.0.9/BTKSorgu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-17 22:52:55.000000 BTKSorgu-1.0.9/BTKSorgu/arayuz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-17 22:52:55.000000 BTKSorgu-1.0.9/BTKSorgu/konsol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15717 2023-05-17 22:52:55.000000 BTKSorgu-1.0.9/BTKSorgu/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:53:15.168375 BTKSorgu-1.0.9/BTKSorgu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-05-17 22:53:15.000000 BTKSorgu-1.0.9/BTKSorgu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-17 22:53:15.000000 BTKSorgu-1.0.9/BTKSorgu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 22:53:15.000000 BTKSorgu-1.0.9/BTKSorgu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-17 22:53:15.000000 BTKSorgu-1.0.9/BTKSorgu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-17 22:53:15.000000 BTKSorgu-1.0.9/BTKSorgu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 22:53:15.000000 BTKSorgu-1.0.9/BTKSorgu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-17 22:52:55.000000 BTKSorgu-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-17 22:52:55.000000 BTKSorgu-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-05-17 22:53:15.168375 BTKSorgu-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-05-17 22:52:55.000000 BTKSorgu-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:53:15.168375 BTKSorgu-1.0.9/Shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-17 22:52:55.000000 BTKSorgu-1.0.9/Shared/org.KekikAkademi.BTKSorgu.appdata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-17 22:52:55.000000 BTKSorgu-1.0.9/Shared/org.KekikAkademi.BTKSorgu.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-17 22:52:55.000000 BTKSorgu-1.0.9/Shared/org.KekikAkademi.BTKSorgu.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 22:53:15.168375 BTKSorgu-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-17 22:52:55.000000 BTKSorgu-1.0.9/setup.py
```

### Comparing `BTKSorgu-1.0.8/BTKSorgu/Erisim_Engeli.py` & `BTKSorgu-1.0.9/BTKSorgu/Erisim_Engeli.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.8/BTKSorgu/KekikGUI.py` & `BTKSorgu-1.0.9/BTKSorgu/KekikGUI.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.8/BTKSorgu/arayuz.py` & `BTKSorgu-1.0.9/BTKSorgu/arayuz.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.8/BTKSorgu/konsol.py` & `BTKSorgu-1.0.9/BTKSorgu/konsol.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.8/BTKSorgu/logo.png` & `BTKSorgu-1.0.9/BTKSorgu/logo.png`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.8/BTKSorgu.egg-info/PKG-INFO` & `BTKSorgu-1.0.9/BTKSorgu.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTKSorgu
-Version: 1.0.8
+Version: 1.0.9
 Summary: Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu
 Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: BTKSorgu,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
@@ -38,37 +38,37 @@
 ![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png)
 
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🚀 Kurulum
 
-### <img width="14" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg"> PyPi (Lib - CLI - UI)
+### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg"> PyPi (Lib - CLI - UI)
 
 ```bash
 # Yüklemek
 pip install BTKSorgu
 
 # Güncellemek
 pip install -U BTKSorgu
 ```
 
-### <img width="14" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/flatpak.svg"> FlatHub (UI)
+### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/flathub.svg"> FlatHub (UI)
 
 ```bash
 # Yüklemek
-flatpak install flathub org.kekikakademi.ntvHaber
+flatpak install flathub org.KekikAkademi.BTKSorgu
 
 # Çalıştırmak
-flatpak run org.kekikakademi.ntvHaber
+flatpak run org.KekikAkademi.BTKSorgu
 ```
 
 ## 📝 Kullanım
 
-### <img width="14" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg"> Lib
+### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg"> Lib
 
 ```python
 from BTKSorgu import BTKSorgu
 from time     import time
 
 basla = time()
 print(BTKSorgu("redtube.com"))
@@ -79,29 +79,30 @@
     # » xnxx.com, 23/02/2008 tarihli ve 410.01.02.2008-054003 sayılı Telekomünikasyon İletişim Başkanlığı kararıyla erişime engellenmiştir.
 bitir = time()
 
 print(bitir-basla)
     # » 8.352766513824463
 ```
 
-### <img width="14" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/iterm2.svg"> CLI
+### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/iterm2.svg"> CLI
 
 ```bash
 BTKSorgu keyiflerolsun.dev
 
 # > Bilgi Teknolojileri ve İletişim Kurumu tarafından uygulanan bir karar bulunamadı.
 ```
 
-### <img width="14" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/freedesktop.svg"> UI
+### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/freedesktop.svg"> UI
 
 ```bash
 BTKSorguGUI
 
 # veya
-flatpak run org.kekikakademi.ntvHaber
+
+flatpak run org.KekikAkademi.BTKSorgu
 ```
 
 ## 🔖 Program Akış Şeması
 
 1. *Oturum Başlat,*
 2. *[https://internet2.btk.gov.tr](https://internet2.btk.gov.tr/) adresine yönlendirmeleri kabul ederek git: kurabiyeleri ye,*
 3. *Dönen kaynak kodundan doğrulama resmini indir,*
@@ -109,32 +110,98 @@
 5. *Sorgu adresini okuduğun doğrulama koduyla birlikte post at,*
 6. *Dönen yanıtı ayrıştırıp edip geri döndür..*
 
 > Bu programın yazılma ve açık kaynak kodlu olarak paylaşılma amacı: *Tarayıcı Otomasyonlarının sebep olduğu  **gereksiz kaynak tüketimi** ve  **zaman kaybının**  önüne geçmeye teşvik etmektir…*
 
 > Tarayıcı Otomasyonu : *[Selenium IDE](https://www.selenium.dev/selenium-ide/)* **-** *[Katalon Automation Recorder](https://www.katalon.com/resources-center/blog/katalon-automation-recorder/)* **-** *[BrowserAutomationStudio](https://bablosoft.com/shop/BrowserAutomationStudio)*
 
-> Karşılaştırması : **[Selenium VS Requests](https://www.r10.net/off-topic/2751412-selenium-vs-requests.html)**
+> Karşılaştırması : **[Selenium VS Requests](https://www.r10.net/off-topic/2751612-selenium-vs-requests.html)**
 
 ## 📝 Proje İlerlemesi
 
 - ✅ **[@raifpy](https://github.com/raifpy)** *tarafından kodlanmış projenin hantal bir bileşeni itinayla `dızz 🐍`'lanmıştır..*
 - ✅ **Selenium** *bağımlılığından dolayı hantal çalışan kod yapısı tamamen ayıklanıp bütün iş* `requests`*'e yaptırılıp ciddi miktarda kaynak ve zaman tasarrufu ettirilmiştir..*
 - ✅ *Kolay erişilebilir olması ve ilham yaratması için* **pypi** *depolarına yüklenmiştir..*
 - ✅ **Tkinter** *ile basit bir arayüz tasarlanmıştır ve eğitim amacıyla Depolara yüklenmiştir..*
 
+---
+
+<details>
+    <summary style="font-weight: bold; font-size: 20px">
+      <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/buddy.svg"> <b>Manuel Derlemek</b>
+      <i>(genişletmek için tıklayın!)</i>
+    </summary>
+    <br/>
+
+### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg"> Python
+
+```bash
+# Depoyu Çek
+https://github.com/keyiflerolsun/BTKSorgu.git
+cd BTKSorgu
+
+# Gerekli Ortamları Kur
+pip install -U pip setuptools wheel twine
+
+# Paketi Yükle
+pip install .
+
+# Artıkları Temizle
+rm -rf build *.egg-info
+
+# Çalıştır
+BTKSorgu     # CLI
+BTKSorguGUI  # GUI
+
+# Paketi Kaldır
+pip uninstall BTKSorgu
+```
+
+### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/flatpak.svg"> FlatPak
+
+```bash
+# Depoyu Çek
+git clone https://github.com/keyiflerolsun/flathub.git
+cd flathub
+
+# Dala Geç
+git checkout org.KekikAkademi.BTKSorgu
+
+# Gerekli Ortamları Kur
+flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
+flatpak remote-add --if-not-exists flathub-beta https://flathub.org/beta-repo/flathub-beta.flatpakrepo
+flatpak update && flatpak upgrade
+flatpak install flathub org.freedesktop.{Platform,Sdk}//22.08
+
+# Paketle
+flatpak-builder --user --install --force-clean build-dir org.KekikAkademi.BTKSorgu.yml
+
+# Artıkları Temizle
+rm -rf .flatpak* .vscode build-dir && find . | grep -E "(__pycache__|\.pyc|\.pyo$)" | xargs rm -rf
+
+# Çalıştır
+flatpak run org.KekikAkademi.BTKSorgu
+
+# Paketi Kaldır
+flatpak uninstall org.KekikAkademi.BTKSorgu
+```
+
+</details>
+
+---
+
 ## 🌐 Telif Hakkı ve Lisans
 
 * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
 * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/BTKSorgu/blob/master/LICENSE) *Koşullarına göre lisanslanmıştır..*
 
 ## ♻️ İletişim
 
 *Benimle iletişime geçmek isterseniz, **Telegram**'dan mesaj göndermekten çekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve)
 
 ## 💸 Bağış Yap
 
 **[☕️ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
 
-##
+***
 
 > **[@KekikAkademi](https://t.me/KekikAkademi)** *için yazılmıştır..*
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: BTKSorgu Version: 1.0.8 Summary: Hedef websitesinin
+Metadata-Version: 2.1 Name: BTKSorgu Version: 1.0.9 Summary: Hedef websitesinin
 BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
 keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
@@ -31,54 +31,76 @@
 BTKSorgu/main/.github/icons/SS.png) [![ForTheBadge made-with-python](https://
 ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-
 with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð Kurulum ### [https:/
 /raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg]
 PyPi (Lib - CLI - UI) ```bash # YÃ¼klemek pip install BTKSorgu # GÃ¼ncellemek
 pip install -U BTKSorgu ``` ### [https://raw.githubusercontent.com/
-keyiflerolsun/BTKSorgu/main/.github/icons/flatpak.svg] FlatHub (UI) ```bash #
-YÃ¼klemek flatpak install flathub org.kekikakademi.ntvHaber # ÃalÄ±ÅtÄ±rmak
-flatpak run org.kekikakademi.ntvHaber ``` ## ð KullanÄ±m ### [https://
+keyiflerolsun/BTKSorgu/main/.github/icons/flathub.svg] FlatHub (UI) ```bash #
+YÃ¼klemek flatpak install flathub org.KekikAkademi.BTKSorgu # ÃalÄ±ÅtÄ±rmak
+flatpak run org.KekikAkademi.BTKSorgu ``` ## ð KullanÄ±m ### [https://
 raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg]
 Lib ```python from BTKSorgu import BTKSorgu from time import time basla = time
 () print(BTKSorgu("redtube.com")) # Â» redtube.com, 30/01/2008 tarihli ve
 410.01.02.2008-028105 sayÄ±lÄ± TelekomÃ¼nikasyon Ä°letiÅim BaÅkanlÄ±ÄÄ±
 kararÄ±yla eriÅime engellenmiÅtir. print(BTKSorgu("kekikakademi.org")) # Â»
 Bilgi Teknolojileri ve Ä°letiÅim Kurumu tarafÄ±ndan uygulanan bir karar
 bulunamadÄ±. print(BTKSorgu("xnxx.com")) # Â» xnxx.com, 23/02/2008 tarihli ve
 410.01.02.2008-054003 sayÄ±lÄ± TelekomÃ¼nikasyon Ä°letiÅim BaÅkanlÄ±ÄÄ±
 kararÄ±yla eriÅime engellenmiÅtir. bitir = time() print(bitir-basla) # Â»
 8.352766513824463 ``` ### [https://raw.githubusercontent.com/keyiflerolsun/
 BTKSorgu/main/.github/icons/iterm2.svg] CLI ```bash BTKSorgu keyiflerolsun.dev
 # > Bilgi Teknolojileri ve Ä°letiÅim Kurumu tarafÄ±ndan uygulanan bir karar
 bulunamadÄ±. ``` ### [https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/
 main/.github/icons/freedesktop.svg] UI ```bash BTKSorguGUI # veya flatpak run
-org.kekikakademi.ntvHaber ``` ## ð Program AkÄ±Å ÅemasÄ± 1. *Oturum
+org.KekikAkademi.BTKSorgu ``` ## ð Program AkÄ±Å ÅemasÄ± 1. *Oturum
 BaÅlat,* 2. *[https://internet2.btk.gov.tr](https://internet2.btk.gov.tr/
 ) adresine yÃ¶nlendirmeleri kabul ederek git: kurabiyeleri ye,* 3. *DÃ¶nen
 kaynak kodundan doÄrulama resmini indir,* 4. *DoÄrulama resmini OCR ile
 harflere dÃ¶nÃ¼ÅtÃ¼r, boÅluklarÄ± sil,* 5. *Sorgu adresini okuduÄun
 doÄrulama koduyla birlikte post at,* 6. *DÃ¶nen yanÄ±tÄ± ayrÄ±ÅtÄ±rÄ±p edip
 geri dÃ¶ndÃ¼r..* > Bu programÄ±n yazÄ±lma ve aÃ§Ä±k kaynak kodlu olarak
 paylaÅÄ±lma amacÄ±: *TarayÄ±cÄ± OtomasyonlarÄ±nÄ±n sebep olduÄu **gereksiz
 kaynak tÃ¼ketimi** ve **zaman kaybÄ±nÄ±n** Ã¶nÃ¼ne geÃ§meye teÅvik
 etmektirâ¦* > TarayÄ±cÄ± Otomasyonu : *[Selenium IDE](https://
 www.selenium.dev/selenium-ide/)* **-** *[Katalon Automation Recorder](https://
 www.katalon.com/resources-center/blog/katalon-automation-recorder/)* **-** *
 [BrowserAutomationStudio](https://bablosoft.com/shop/BrowserAutomationStudio)*
 > KarÅÄ±laÅtÄ±rmasÄ± : **[Selenium VS Requests](https://www.r10.net/off-
-topic/2751412-selenium-vs-requests.html)** ## ð Proje Ä°lerlemesi - â **
+topic/2751612-selenium-vs-requests.html)** ## ð Proje Ä°lerlemesi - â **
 [@raifpy](https://github.com/raifpy)** *tarafÄ±ndan kodlanmÄ±Å projenin hantal
 bir bileÅeni itinayla `dÄ±zz ð`'lanmÄ±ÅtÄ±r..* - â **Selenium**
 *baÄÄ±mlÄ±lÄ±ÄÄ±ndan dolayÄ± hantal Ã§alÄ±Åan kod yapÄ±sÄ± tamamen
 ayÄ±klanÄ±p bÃ¼tÃ¼n iÅ* `requests`*'e yaptÄ±rÄ±lÄ±p ciddi miktarda kaynak ve
 zaman tasarrufu ettirilmiÅtir..* - â *Kolay eriÅilebilir olmasÄ± ve ilham
 yaratmasÄ± iÃ§in* **pypi** *depolarÄ±na yÃ¼klenmiÅtir..* - â **Tkinter**
 *ile basit bir arayÃ¼z tasarlanmÄ±ÅtÄ±r ve eÄitim amacÄ±yla Depolara
-yÃ¼klenmiÅtir..* ## ð Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by*
-[keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL
-PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/
-BTKSorgu/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ##
-â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek isterseniz, **Telegram**'dan
-mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ##
-ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)** ##
-> **[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
+yÃ¼klenmiÅtir..* ---   [https://raw.githubusercontent.com/keyiflerolsun/
+BTKSorgu/main/.github/icons/buddy.svg] Manuel Derlemek (geniÅletmek iÃ§in
+tÄ±klayÄ±n!)
+### [https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/
+icons/python.svg] Python ```bash # Depoyu Ãek https://github.com/
+keyiflerolsun/BTKSorgu.git cd BTKSorgu # Gerekli OrtamlarÄ± Kur pip install -
+U pip setuptools wheel twine # Paketi YÃ¼kle pip install . # ArtÄ±klarÄ±
+Temizle rm -rf build *.egg-info # ÃalÄ±ÅtÄ±r BTKSorgu # CLI BTKSorguGUI # GUI
+# Paketi KaldÄ±r pip uninstall BTKSorgu ``` ### [https://
+raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/
+flatpak.svg] FlatPak ```bash # Depoyu Ãek git clone https://github.com/
+keyiflerolsun/flathub.git cd flathub # Dala GeÃ§ git checkout
+org.KekikAkademi.BTKSorgu # Gerekli OrtamlarÄ± Kur flatpak remote-add --if-not-
+exists flathub https://flathub.org/repo/flathub.flatpakrepo flatpak remote-add
+--if-not-exists flathub-beta https://flathub.org/beta-repo/flathub-
+beta.flatpakrepo flatpak update && flatpak upgrade flatpak install flathub
+org.freedesktop.{Platform,Sdk}//22.08 # Paketle flatpak-builder --user --
+install --force-clean build-dir org.KekikAkademi.BTKSorgu.yml # ArtÄ±klarÄ±
+Temizle rm -rf .flatpak* .vscode build-dir && find . | grep -E "
+(__pycache__|\.pyc|\.pyo$)" | xargs rm -rf # ÃalÄ±ÅtÄ±r flatpak run
+org.KekikAkademi.BTKSorgu # Paketi KaldÄ±r flatpak uninstall
+org.KekikAkademi.BTKSorgu ```  --- ## ð Telif HakkÄ± ve Lisans * *Copyright
+(C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU
+GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/
+keyiflerolsun/BTKSorgu/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re
+lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek
+isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun]
+(https://t.me/KekikKahve) ## ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https:/
+/KekikAkademi.org/Kahve)** *** > **[@KekikAkademi](https://t.me/KekikAkademi)**
+*iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
```

### Comparing `BTKSorgu-1.0.8/LICENSE` & `BTKSorgu-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.8/PKG-INFO` & `BTKSorgu-1.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTKSorgu
-Version: 1.0.8
+Version: 1.0.9
 Summary: Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu
 Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: BTKSorgu,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
@@ -38,37 +38,37 @@
 ![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png)
 
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🚀 Kurulum
 
-### <img width="14" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg"> PyPi (Lib - CLI - UI)
+### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg"> PyPi (Lib - CLI - UI)
 
 ```bash
 # Yüklemek
 pip install BTKSorgu
 
 # Güncellemek
 pip install -U BTKSorgu
 ```
 
-### <img width="14" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/flatpak.svg"> FlatHub (UI)
+### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/flathub.svg"> FlatHub (UI)
 
 ```bash
 # Yüklemek
-flatpak install flathub org.kekikakademi.ntvHaber
+flatpak install flathub org.KekikAkademi.BTKSorgu
 
 # Çalıştırmak
-flatpak run org.kekikakademi.ntvHaber
+flatpak run org.KekikAkademi.BTKSorgu
 ```
 
 ## 📝 Kullanım
 
-### <img width="14" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg"> Lib
+### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg"> Lib
 
 ```python
 from BTKSorgu import BTKSorgu
 from time     import time
 
 basla = time()
 print(BTKSorgu("redtube.com"))
@@ -79,29 +79,30 @@
     # » xnxx.com, 23/02/2008 tarihli ve 410.01.02.2008-054003 sayılı Telekomünikasyon İletişim Başkanlığı kararıyla erişime engellenmiştir.
 bitir = time()
 
 print(bitir-basla)
     # » 8.352766513824463
 ```
 
-### <img width="14" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/iterm2.svg"> CLI
+### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/iterm2.svg"> CLI
 
 ```bash
 BTKSorgu keyiflerolsun.dev
 
 # > Bilgi Teknolojileri ve İletişim Kurumu tarafından uygulanan bir karar bulunamadı.
 ```
 
-### <img width="14" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/freedesktop.svg"> UI
+### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/freedesktop.svg"> UI
 
 ```bash
 BTKSorguGUI
 
 # veya
-flatpak run org.kekikakademi.ntvHaber
+
+flatpak run org.KekikAkademi.BTKSorgu
 ```
 
 ## 🔖 Program Akış Şeması
 
 1. *Oturum Başlat,*
 2. *[https://internet2.btk.gov.tr](https://internet2.btk.gov.tr/) adresine yönlendirmeleri kabul ederek git: kurabiyeleri ye,*
 3. *Dönen kaynak kodundan doğrulama resmini indir,*
@@ -109,32 +110,98 @@
 5. *Sorgu adresini okuduğun doğrulama koduyla birlikte post at,*
 6. *Dönen yanıtı ayrıştırıp edip geri döndür..*
 
 > Bu programın yazılma ve açık kaynak kodlu olarak paylaşılma amacı: *Tarayıcı Otomasyonlarının sebep olduğu  **gereksiz kaynak tüketimi** ve  **zaman kaybının**  önüne geçmeye teşvik etmektir…*
 
 > Tarayıcı Otomasyonu : *[Selenium IDE](https://www.selenium.dev/selenium-ide/)* **-** *[Katalon Automation Recorder](https://www.katalon.com/resources-center/blog/katalon-automation-recorder/)* **-** *[BrowserAutomationStudio](https://bablosoft.com/shop/BrowserAutomationStudio)*
 
-> Karşılaştırması : **[Selenium VS Requests](https://www.r10.net/off-topic/2751412-selenium-vs-requests.html)**
+> Karşılaştırması : **[Selenium VS Requests](https://www.r10.net/off-topic/2751612-selenium-vs-requests.html)**
 
 ## 📝 Proje İlerlemesi
 
 - ✅ **[@raifpy](https://github.com/raifpy)** *tarafından kodlanmış projenin hantal bir bileşeni itinayla `dızz 🐍`'lanmıştır..*
 - ✅ **Selenium** *bağımlılığından dolayı hantal çalışan kod yapısı tamamen ayıklanıp bütün iş* `requests`*'e yaptırılıp ciddi miktarda kaynak ve zaman tasarrufu ettirilmiştir..*
 - ✅ *Kolay erişilebilir olması ve ilham yaratması için* **pypi** *depolarına yüklenmiştir..*
 - ✅ **Tkinter** *ile basit bir arayüz tasarlanmıştır ve eğitim amacıyla Depolara yüklenmiştir..*
 
+---
+
+<details>
+    <summary style="font-weight: bold; font-size: 20px">
+      <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/buddy.svg"> <b>Manuel Derlemek</b>
+      <i>(genişletmek için tıklayın!)</i>
+    </summary>
+    <br/>
+
+### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg"> Python
+
+```bash
+# Depoyu Çek
+https://github.com/keyiflerolsun/BTKSorgu.git
+cd BTKSorgu
+
+# Gerekli Ortamları Kur
+pip install -U pip setuptools wheel twine
+
+# Paketi Yükle
+pip install .
+
+# Artıkları Temizle
+rm -rf build *.egg-info
+
+# Çalıştır
+BTKSorgu     # CLI
+BTKSorguGUI  # GUI
+
+# Paketi Kaldır
+pip uninstall BTKSorgu
+```
+
+### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/flatpak.svg"> FlatPak
+
+```bash
+# Depoyu Çek
+git clone https://github.com/keyiflerolsun/flathub.git
+cd flathub
+
+# Dala Geç
+git checkout org.KekikAkademi.BTKSorgu
+
+# Gerekli Ortamları Kur
+flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
+flatpak remote-add --if-not-exists flathub-beta https://flathub.org/beta-repo/flathub-beta.flatpakrepo
+flatpak update && flatpak upgrade
+flatpak install flathub org.freedesktop.{Platform,Sdk}//22.08
+
+# Paketle
+flatpak-builder --user --install --force-clean build-dir org.KekikAkademi.BTKSorgu.yml
+
+# Artıkları Temizle
+rm -rf .flatpak* .vscode build-dir && find . | grep -E "(__pycache__|\.pyc|\.pyo$)" | xargs rm -rf
+
+# Çalıştır
+flatpak run org.KekikAkademi.BTKSorgu
+
+# Paketi Kaldır
+flatpak uninstall org.KekikAkademi.BTKSorgu
+```
+
+</details>
+
+---
+
 ## 🌐 Telif Hakkı ve Lisans
 
 * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
 * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/BTKSorgu/blob/master/LICENSE) *Koşullarına göre lisanslanmıştır..*
 
 ## ♻️ İletişim
 
 *Benimle iletişime geçmek isterseniz, **Telegram**'dan mesaj göndermekten çekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve)
 
 ## 💸 Bağış Yap
 
 **[☕️ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
 
-##
+***
 
 > **[@KekikAkademi](https://t.me/KekikAkademi)** *için yazılmıştır..*
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: BTKSorgu Version: 1.0.8 Summary: Hedef websitesinin
+Metadata-Version: 2.1 Name: BTKSorgu Version: 1.0.9 Summary: Hedef websitesinin
 BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
 keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
@@ -31,54 +31,76 @@
 BTKSorgu/main/.github/icons/SS.png) [![ForTheBadge made-with-python](https://
 ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-
 with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð Kurulum ### [https:/
 /raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg]
 PyPi (Lib - CLI - UI) ```bash # YÃ¼klemek pip install BTKSorgu # GÃ¼ncellemek
 pip install -U BTKSorgu ``` ### [https://raw.githubusercontent.com/
-keyiflerolsun/BTKSorgu/main/.github/icons/flatpak.svg] FlatHub (UI) ```bash #
-YÃ¼klemek flatpak install flathub org.kekikakademi.ntvHaber # ÃalÄ±ÅtÄ±rmak
-flatpak run org.kekikakademi.ntvHaber ``` ## ð KullanÄ±m ### [https://
+keyiflerolsun/BTKSorgu/main/.github/icons/flathub.svg] FlatHub (UI) ```bash #
+YÃ¼klemek flatpak install flathub org.KekikAkademi.BTKSorgu # ÃalÄ±ÅtÄ±rmak
+flatpak run org.KekikAkademi.BTKSorgu ``` ## ð KullanÄ±m ### [https://
 raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg]
 Lib ```python from BTKSorgu import BTKSorgu from time import time basla = time
 () print(BTKSorgu("redtube.com")) # Â» redtube.com, 30/01/2008 tarihli ve
 410.01.02.2008-028105 sayÄ±lÄ± TelekomÃ¼nikasyon Ä°letiÅim BaÅkanlÄ±ÄÄ±
 kararÄ±yla eriÅime engellenmiÅtir. print(BTKSorgu("kekikakademi.org")) # Â»
 Bilgi Teknolojileri ve Ä°letiÅim Kurumu tarafÄ±ndan uygulanan bir karar
 bulunamadÄ±. print(BTKSorgu("xnxx.com")) # Â» xnxx.com, 23/02/2008 tarihli ve
 410.01.02.2008-054003 sayÄ±lÄ± TelekomÃ¼nikasyon Ä°letiÅim BaÅkanlÄ±ÄÄ±
 kararÄ±yla eriÅime engellenmiÅtir. bitir = time() print(bitir-basla) # Â»
 8.352766513824463 ``` ### [https://raw.githubusercontent.com/keyiflerolsun/
 BTKSorgu/main/.github/icons/iterm2.svg] CLI ```bash BTKSorgu keyiflerolsun.dev
 # > Bilgi Teknolojileri ve Ä°letiÅim Kurumu tarafÄ±ndan uygulanan bir karar
 bulunamadÄ±. ``` ### [https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/
 main/.github/icons/freedesktop.svg] UI ```bash BTKSorguGUI # veya flatpak run
-org.kekikakademi.ntvHaber ``` ## ð Program AkÄ±Å ÅemasÄ± 1. *Oturum
+org.KekikAkademi.BTKSorgu ``` ## ð Program AkÄ±Å ÅemasÄ± 1. *Oturum
 BaÅlat,* 2. *[https://internet2.btk.gov.tr](https://internet2.btk.gov.tr/
 ) adresine yÃ¶nlendirmeleri kabul ederek git: kurabiyeleri ye,* 3. *DÃ¶nen
 kaynak kodundan doÄrulama resmini indir,* 4. *DoÄrulama resmini OCR ile
 harflere dÃ¶nÃ¼ÅtÃ¼r, boÅluklarÄ± sil,* 5. *Sorgu adresini okuduÄun
 doÄrulama koduyla birlikte post at,* 6. *DÃ¶nen yanÄ±tÄ± ayrÄ±ÅtÄ±rÄ±p edip
 geri dÃ¶ndÃ¼r..* > Bu programÄ±n yazÄ±lma ve aÃ§Ä±k kaynak kodlu olarak
 paylaÅÄ±lma amacÄ±: *TarayÄ±cÄ± OtomasyonlarÄ±nÄ±n sebep olduÄu **gereksiz
 kaynak tÃ¼ketimi** ve **zaman kaybÄ±nÄ±n** Ã¶nÃ¼ne geÃ§meye teÅvik
 etmektirâ¦* > TarayÄ±cÄ± Otomasyonu : *[Selenium IDE](https://
 www.selenium.dev/selenium-ide/)* **-** *[Katalon Automation Recorder](https://
 www.katalon.com/resources-center/blog/katalon-automation-recorder/)* **-** *
 [BrowserAutomationStudio](https://bablosoft.com/shop/BrowserAutomationStudio)*
 > KarÅÄ±laÅtÄ±rmasÄ± : **[Selenium VS Requests](https://www.r10.net/off-
-topic/2751412-selenium-vs-requests.html)** ## ð Proje Ä°lerlemesi - â **
+topic/2751612-selenium-vs-requests.html)** ## ð Proje Ä°lerlemesi - â **
 [@raifpy](https://github.com/raifpy)** *tarafÄ±ndan kodlanmÄ±Å projenin hantal
 bir bileÅeni itinayla `dÄ±zz ð`'lanmÄ±ÅtÄ±r..* - â **Selenium**
 *baÄÄ±mlÄ±lÄ±ÄÄ±ndan dolayÄ± hantal Ã§alÄ±Åan kod yapÄ±sÄ± tamamen
 ayÄ±klanÄ±p bÃ¼tÃ¼n iÅ* `requests`*'e yaptÄ±rÄ±lÄ±p ciddi miktarda kaynak ve
 zaman tasarrufu ettirilmiÅtir..* - â *Kolay eriÅilebilir olmasÄ± ve ilham
 yaratmasÄ± iÃ§in* **pypi** *depolarÄ±na yÃ¼klenmiÅtir..* - â **Tkinter**
 *ile basit bir arayÃ¼z tasarlanmÄ±ÅtÄ±r ve eÄitim amacÄ±yla Depolara
-yÃ¼klenmiÅtir..* ## ð Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by*
-[keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL
-PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/
-BTKSorgu/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ##
-â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek isterseniz, **Telegram**'dan
-mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ##
-ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)** ##
-> **[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
+yÃ¼klenmiÅtir..* ---   [https://raw.githubusercontent.com/keyiflerolsun/
+BTKSorgu/main/.github/icons/buddy.svg] Manuel Derlemek (geniÅletmek iÃ§in
+tÄ±klayÄ±n!)
+### [https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/
+icons/python.svg] Python ```bash # Depoyu Ãek https://github.com/
+keyiflerolsun/BTKSorgu.git cd BTKSorgu # Gerekli OrtamlarÄ± Kur pip install -
+U pip setuptools wheel twine # Paketi YÃ¼kle pip install . # ArtÄ±klarÄ±
+Temizle rm -rf build *.egg-info # ÃalÄ±ÅtÄ±r BTKSorgu # CLI BTKSorguGUI # GUI
+# Paketi KaldÄ±r pip uninstall BTKSorgu ``` ### [https://
+raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/
+flatpak.svg] FlatPak ```bash # Depoyu Ãek git clone https://github.com/
+keyiflerolsun/flathub.git cd flathub # Dala GeÃ§ git checkout
+org.KekikAkademi.BTKSorgu # Gerekli OrtamlarÄ± Kur flatpak remote-add --if-not-
+exists flathub https://flathub.org/repo/flathub.flatpakrepo flatpak remote-add
+--if-not-exists flathub-beta https://flathub.org/beta-repo/flathub-
+beta.flatpakrepo flatpak update && flatpak upgrade flatpak install flathub
+org.freedesktop.{Platform,Sdk}//22.08 # Paketle flatpak-builder --user --
+install --force-clean build-dir org.KekikAkademi.BTKSorgu.yml # ArtÄ±klarÄ±
+Temizle rm -rf .flatpak* .vscode build-dir && find . | grep -E "
+(__pycache__|\.pyc|\.pyo$)" | xargs rm -rf # ÃalÄ±ÅtÄ±r flatpak run
+org.KekikAkademi.BTKSorgu # Paketi KaldÄ±r flatpak uninstall
+org.KekikAkademi.BTKSorgu ```  --- ## ð Telif HakkÄ± ve Lisans * *Copyright
+(C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU
+GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/
+keyiflerolsun/BTKSorgu/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re
+lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek
+isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun]
+(https://t.me/KekikKahve) ## ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https:/
+/KekikAkademi.org/Kahve)** *** > **[@KekikAkademi](https://t.me/KekikAkademi)**
+*iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
```

### Comparing `BTKSorgu-1.0.8/README.md` & `BTKSorgu-1.0.9/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -22,37 +22,37 @@
 ![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png)
 
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🚀 Kurulum
 
-### <img width="14" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg"> PyPi (Lib - CLI - UI)
+### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg"> PyPi (Lib - CLI - UI)
 
 ```bash
 # Yüklemek
 pip install BTKSorgu
 
 # Güncellemek
 pip install -U BTKSorgu
 ```
 
-### <img width="14" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/flatpak.svg"> FlatHub (UI)
+### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/flathub.svg"> FlatHub (UI)
 
 ```bash
 # Yüklemek
-flatpak install flathub org.kekikakademi.ntvHaber
+flatpak install flathub org.KekikAkademi.BTKSorgu
 
 # Çalıştırmak
-flatpak run org.kekikakademi.ntvHaber
+flatpak run org.KekikAkademi.BTKSorgu
 ```
 
 ## 📝 Kullanım
 
-### <img width="14" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg"> Lib
+### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg"> Lib
 
 ```python
 from BTKSorgu import BTKSorgu
 from time     import time
 
 basla = time()
 print(BTKSorgu("redtube.com"))
@@ -63,29 +63,30 @@
     # » xnxx.com, 23/02/2008 tarihli ve 410.01.02.2008-054003 sayılı Telekomünikasyon İletişim Başkanlığı kararıyla erişime engellenmiştir.
 bitir = time()
 
 print(bitir-basla)
     # » 8.352766513824463
 ```
 
-### <img width="14" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/iterm2.svg"> CLI
+### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/iterm2.svg"> CLI
 
 ```bash
 BTKSorgu keyiflerolsun.dev
 
 # > Bilgi Teknolojileri ve İletişim Kurumu tarafından uygulanan bir karar bulunamadı.
 ```
 
-### <img width="14" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/freedesktop.svg"> UI
+### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/freedesktop.svg"> UI
 
 ```bash
 BTKSorguGUI
 
 # veya
-flatpak run org.kekikakademi.ntvHaber
+
+flatpak run org.KekikAkademi.BTKSorgu
 ```
 
 ## 🔖 Program Akış Şeması
 
 1. *Oturum Başlat,*
 2. *[https://internet2.btk.gov.tr](https://internet2.btk.gov.tr/) adresine yönlendirmeleri kabul ederek git: kurabiyeleri ye,*
 3. *Dönen kaynak kodundan doğrulama resmini indir,*
@@ -93,32 +94,98 @@
 5. *Sorgu adresini okuduğun doğrulama koduyla birlikte post at,*
 6. *Dönen yanıtı ayrıştırıp edip geri döndür..*
 
 > Bu programın yazılma ve açık kaynak kodlu olarak paylaşılma amacı: *Tarayıcı Otomasyonlarının sebep olduğu  **gereksiz kaynak tüketimi** ve  **zaman kaybının**  önüne geçmeye teşvik etmektir…*
 
 > Tarayıcı Otomasyonu : *[Selenium IDE](https://www.selenium.dev/selenium-ide/)* **-** *[Katalon Automation Recorder](https://www.katalon.com/resources-center/blog/katalon-automation-recorder/)* **-** *[BrowserAutomationStudio](https://bablosoft.com/shop/BrowserAutomationStudio)*
 
-> Karşılaştırması : **[Selenium VS Requests](https://www.r10.net/off-topic/2751412-selenium-vs-requests.html)**
+> Karşılaştırması : **[Selenium VS Requests](https://www.r10.net/off-topic/2751612-selenium-vs-requests.html)**
 
 ## 📝 Proje İlerlemesi
 
 - ✅ **[@raifpy](https://github.com/raifpy)** *tarafından kodlanmış projenin hantal bir bileşeni itinayla `dızz 🐍`'lanmıştır..*
 - ✅ **Selenium** *bağımlılığından dolayı hantal çalışan kod yapısı tamamen ayıklanıp bütün iş* `requests`*'e yaptırılıp ciddi miktarda kaynak ve zaman tasarrufu ettirilmiştir..*
 - ✅ *Kolay erişilebilir olması ve ilham yaratması için* **pypi** *depolarına yüklenmiştir..*
 - ✅ **Tkinter** *ile basit bir arayüz tasarlanmıştır ve eğitim amacıyla Depolara yüklenmiştir..*
 
+---
+
+<details>
+    <summary style="font-weight: bold; font-size: 20px">
+      <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/buddy.svg"> <b>Manuel Derlemek</b>
+      <i>(genişletmek için tıklayın!)</i>
+    </summary>
+    <br/>
+
+### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg"> Python
+
+```bash
+# Depoyu Çek
+https://github.com/keyiflerolsun/BTKSorgu.git
+cd BTKSorgu
+
+# Gerekli Ortamları Kur
+pip install -U pip setuptools wheel twine
+
+# Paketi Yükle
+pip install .
+
+# Artıkları Temizle
+rm -rf build *.egg-info
+
+# Çalıştır
+BTKSorgu     # CLI
+BTKSorguGUI  # GUI
+
+# Paketi Kaldır
+pip uninstall BTKSorgu
+```
+
+### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/flatpak.svg"> FlatPak
+
+```bash
+# Depoyu Çek
+git clone https://github.com/keyiflerolsun/flathub.git
+cd flathub
+
+# Dala Geç
+git checkout org.KekikAkademi.BTKSorgu
+
+# Gerekli Ortamları Kur
+flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
+flatpak remote-add --if-not-exists flathub-beta https://flathub.org/beta-repo/flathub-beta.flatpakrepo
+flatpak update && flatpak upgrade
+flatpak install flathub org.freedesktop.{Platform,Sdk}//22.08
+
+# Paketle
+flatpak-builder --user --install --force-clean build-dir org.KekikAkademi.BTKSorgu.yml
+
+# Artıkları Temizle
+rm -rf .flatpak* .vscode build-dir && find . | grep -E "(__pycache__|\.pyc|\.pyo$)" | xargs rm -rf
+
+# Çalıştır
+flatpak run org.KekikAkademi.BTKSorgu
+
+# Paketi Kaldır
+flatpak uninstall org.KekikAkademi.BTKSorgu
+```
+
+</details>
+
+---
+
 ## 🌐 Telif Hakkı ve Lisans
 
 * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
 * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/BTKSorgu/blob/master/LICENSE) *Koşullarına göre lisanslanmıştır..*
 
 ## ♻️ İletişim
 
 *Benimle iletişime geçmek isterseniz, **Telegram**'dan mesaj göndermekten çekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve)
 
 ## 💸 Bağış Yap
 
 **[☕️ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
 
-##
+***
 
-> **[@KekikAkademi](https://t.me/KekikAkademi)** *için yazılmıştır..*
+> **[@KekikAkademi](https://t.me/KekikAkademi)** *için yazılmıştır..*
```

#### html2text {}

```diff
@@ -23,54 +23,76 @@
 BTKSorgu/main/.github/icons/SS.png) [![ForTheBadge made-with-python](https://
 ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-
 with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð Kurulum ### [https:/
 /raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg]
 PyPi (Lib - CLI - UI) ```bash # YÃ¼klemek pip install BTKSorgu # GÃ¼ncellemek
 pip install -U BTKSorgu ``` ### [https://raw.githubusercontent.com/
-keyiflerolsun/BTKSorgu/main/.github/icons/flatpak.svg] FlatHub (UI) ```bash #
-YÃ¼klemek flatpak install flathub org.kekikakademi.ntvHaber # ÃalÄ±ÅtÄ±rmak
-flatpak run org.kekikakademi.ntvHaber ``` ## ð KullanÄ±m ### [https://
+keyiflerolsun/BTKSorgu/main/.github/icons/flathub.svg] FlatHub (UI) ```bash #
+YÃ¼klemek flatpak install flathub org.KekikAkademi.BTKSorgu # ÃalÄ±ÅtÄ±rmak
+flatpak run org.KekikAkademi.BTKSorgu ``` ## ð KullanÄ±m ### [https://
 raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg]
 Lib ```python from BTKSorgu import BTKSorgu from time import time basla = time
 () print(BTKSorgu("redtube.com")) # Â» redtube.com, 30/01/2008 tarihli ve
 410.01.02.2008-028105 sayÄ±lÄ± TelekomÃ¼nikasyon Ä°letiÅim BaÅkanlÄ±ÄÄ±
 kararÄ±yla eriÅime engellenmiÅtir. print(BTKSorgu("kekikakademi.org")) # Â»
 Bilgi Teknolojileri ve Ä°letiÅim Kurumu tarafÄ±ndan uygulanan bir karar
 bulunamadÄ±. print(BTKSorgu("xnxx.com")) # Â» xnxx.com, 23/02/2008 tarihli ve
 410.01.02.2008-054003 sayÄ±lÄ± TelekomÃ¼nikasyon Ä°letiÅim BaÅkanlÄ±ÄÄ±
 kararÄ±yla eriÅime engellenmiÅtir. bitir = time() print(bitir-basla) # Â»
 8.352766513824463 ``` ### [https://raw.githubusercontent.com/keyiflerolsun/
 BTKSorgu/main/.github/icons/iterm2.svg] CLI ```bash BTKSorgu keyiflerolsun.dev
 # > Bilgi Teknolojileri ve Ä°letiÅim Kurumu tarafÄ±ndan uygulanan bir karar
 bulunamadÄ±. ``` ### [https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/
 main/.github/icons/freedesktop.svg] UI ```bash BTKSorguGUI # veya flatpak run
-org.kekikakademi.ntvHaber ``` ## ð Program AkÄ±Å ÅemasÄ± 1. *Oturum
+org.KekikAkademi.BTKSorgu ``` ## ð Program AkÄ±Å ÅemasÄ± 1. *Oturum
 BaÅlat,* 2. *[https://internet2.btk.gov.tr](https://internet2.btk.gov.tr/
 ) adresine yÃ¶nlendirmeleri kabul ederek git: kurabiyeleri ye,* 3. *DÃ¶nen
 kaynak kodundan doÄrulama resmini indir,* 4. *DoÄrulama resmini OCR ile
 harflere dÃ¶nÃ¼ÅtÃ¼r, boÅluklarÄ± sil,* 5. *Sorgu adresini okuduÄun
 doÄrulama koduyla birlikte post at,* 6. *DÃ¶nen yanÄ±tÄ± ayrÄ±ÅtÄ±rÄ±p edip
 geri dÃ¶ndÃ¼r..* > Bu programÄ±n yazÄ±lma ve aÃ§Ä±k kaynak kodlu olarak
 paylaÅÄ±lma amacÄ±: *TarayÄ±cÄ± OtomasyonlarÄ±nÄ±n sebep olduÄu **gereksiz
 kaynak tÃ¼ketimi** ve **zaman kaybÄ±nÄ±n** Ã¶nÃ¼ne geÃ§meye teÅvik
 etmektirâ¦* > TarayÄ±cÄ± Otomasyonu : *[Selenium IDE](https://
 www.selenium.dev/selenium-ide/)* **-** *[Katalon Automation Recorder](https://
 www.katalon.com/resources-center/blog/katalon-automation-recorder/)* **-** *
 [BrowserAutomationStudio](https://bablosoft.com/shop/BrowserAutomationStudio)*
 > KarÅÄ±laÅtÄ±rmasÄ± : **[Selenium VS Requests](https://www.r10.net/off-
-topic/2751412-selenium-vs-requests.html)** ## ð Proje Ä°lerlemesi - â **
+topic/2751612-selenium-vs-requests.html)** ## ð Proje Ä°lerlemesi - â **
 [@raifpy](https://github.com/raifpy)** *tarafÄ±ndan kodlanmÄ±Å projenin hantal
 bir bileÅeni itinayla `dÄ±zz ð`'lanmÄ±ÅtÄ±r..* - â **Selenium**
 *baÄÄ±mlÄ±lÄ±ÄÄ±ndan dolayÄ± hantal Ã§alÄ±Åan kod yapÄ±sÄ± tamamen
 ayÄ±klanÄ±p bÃ¼tÃ¼n iÅ* `requests`*'e yaptÄ±rÄ±lÄ±p ciddi miktarda kaynak ve
 zaman tasarrufu ettirilmiÅtir..* - â *Kolay eriÅilebilir olmasÄ± ve ilham
 yaratmasÄ± iÃ§in* **pypi** *depolarÄ±na yÃ¼klenmiÅtir..* - â **Tkinter**
 *ile basit bir arayÃ¼z tasarlanmÄ±ÅtÄ±r ve eÄitim amacÄ±yla Depolara
-yÃ¼klenmiÅtir..* ## ð Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by*
-[keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL
-PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/
-BTKSorgu/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ##
-â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek isterseniz, **Telegram**'dan
-mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ##
-ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)** ##
-> **[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
+yÃ¼klenmiÅtir..* ---   [https://raw.githubusercontent.com/keyiflerolsun/
+BTKSorgu/main/.github/icons/buddy.svg] Manuel Derlemek (geniÅletmek iÃ§in
+tÄ±klayÄ±n!)
+### [https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/
+icons/python.svg] Python ```bash # Depoyu Ãek https://github.com/
+keyiflerolsun/BTKSorgu.git cd BTKSorgu # Gerekli OrtamlarÄ± Kur pip install -
+U pip setuptools wheel twine # Paketi YÃ¼kle pip install . # ArtÄ±klarÄ±
+Temizle rm -rf build *.egg-info # ÃalÄ±ÅtÄ±r BTKSorgu # CLI BTKSorguGUI # GUI
+# Paketi KaldÄ±r pip uninstall BTKSorgu ``` ### [https://
+raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/
+flatpak.svg] FlatPak ```bash # Depoyu Ãek git clone https://github.com/
+keyiflerolsun/flathub.git cd flathub # Dala GeÃ§ git checkout
+org.KekikAkademi.BTKSorgu # Gerekli OrtamlarÄ± Kur flatpak remote-add --if-not-
+exists flathub https://flathub.org/repo/flathub.flatpakrepo flatpak remote-add
+--if-not-exists flathub-beta https://flathub.org/beta-repo/flathub-
+beta.flatpakrepo flatpak update && flatpak upgrade flatpak install flathub
+org.freedesktop.{Platform,Sdk}//22.08 # Paketle flatpak-builder --user --
+install --force-clean build-dir org.KekikAkademi.BTKSorgu.yml # ArtÄ±klarÄ±
+Temizle rm -rf .flatpak* .vscode build-dir && find . | grep -E "
+(__pycache__|\.pyc|\.pyo$)" | xargs rm -rf # ÃalÄ±ÅtÄ±r flatpak run
+org.KekikAkademi.BTKSorgu # Paketi KaldÄ±r flatpak uninstall
+org.KekikAkademi.BTKSorgu ```  --- ## ð Telif HakkÄ± ve Lisans * *Copyright
+(C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU
+GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/
+keyiflerolsun/BTKSorgu/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re
+lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek
+isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun]
+(https://t.me/KekikKahve) ## ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https:/
+/KekikAkademi.org/Kahve)** *** > **[@KekikAkademi](https://t.me/KekikAkademi)**
+*iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
```

### Comparing `BTKSorgu-1.0.8/Shared/org.KekikAkademi.BTKSorgu.appdata.xml` & `BTKSorgu-1.0.9/Shared/org.KekikAkademi.BTKSorgu.appdata.xml`

 * *Files 6% similar despite different names*

#### Comparing `BTKSorgu-1.0.8/Shared/org.KekikAkademi.BTKSorgu.appdata.xml` & `BTKSorgu-1.0.9/Shared/org.KekikAkademi.BTKSorgu.appdata.xml`

```diff
@@ -25,14 +25,19 @@
       <image>https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png</image>
     </screenshot>
   </screenshots>
   <categories>
     <category>Education</category>
   </categories>
   <releases>
+    <release version="1.0.8" date="2023-5-18">
+      <description>
+        <p>Readme Genişletildi ve Manuel Derleme Aşamaları Eklendi..</p>
+      </description>
+    </release>
     <release version="1.0.8" date="2023-5-17">
       <description>
         <p>Readme Düzenlendi..</p>
       </description>
     </release>
     <release version="1.0.5" date="2023-5-17">
       <description>
```

### Comparing `BTKSorgu-1.0.8/Shared/org.KekikAkademi.BTKSorgu.svg` & `BTKSorgu-1.0.9/Shared/org.KekikAkademi.BTKSorgu.svg`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.8/setup.py` & `BTKSorgu-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 from io         import open
 
 setup(
     # ? Genel Bilgiler
     name         = "BTKSorgu",
-    version      = "1.0.8",
+    version      = "1.0.9",
     url          = "https://github.com/keyiflerolsun/E-Fatura_Sorgu",
     description  = "Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu",
     keywords     = ["BTKSorgu", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
```

