# Comparing `tmp/eFatura-1.0.1.tar.gz` & `tmp/eFatura-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eFatura-1.0.1.tar", last modified: Wed May 10 14:07:50 2023, max compression
+gzip compressed data, was "eFatura-1.0.2.tar", last modified: Thu May 18 12:17:29 2023, max compression
```

## Comparing `eFatura-1.0.1.tar` & `eFatura-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:07:50.868749 eFatura-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 14:07:30.000000 eFatura-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-10 14:07:50.868749 eFatura-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-10 14:07:30.000000 eFatura-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:07:50.868749 eFatura-1.0.1/eFatura/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-10 14:07:30.000000 eFatura-1.0.1/eFatura/Oturum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-10 14:07:30.000000 eFatura-1.0.1/eFatura/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-10 14:07:30.000000 eFatura-1.0.1/eFatura/konsol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:07:50.868749 eFatura-1.0.1/eFatura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-10 14:07:50.000000 eFatura-1.0.1/eFatura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-10 14:07:50.000000 eFatura-1.0.1/eFatura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 14:07:50.000000 eFatura-1.0.1/eFatura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-10 14:07:50.000000 eFatura-1.0.1/eFatura.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-10 14:07:50.000000 eFatura-1.0.1/eFatura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-10 14:07:50.000000 eFatura-1.0.1/eFatura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 14:07:50.872749 eFatura-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-10 14:07:30.000000 eFatura-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:17:29.575943 eFatura-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-18 12:17:07.000000 eFatura-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-05-18 12:17:29.575943 eFatura-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-18 12:17:07.000000 eFatura-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:17:29.575943 eFatura-1.0.2/eFatura/
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-05-18 12:17:07.000000 eFatura-1.0.2/eFatura/KekikGUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-18 12:17:07.000000 eFatura-1.0.2/eFatura/Oturum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-18 12:17:07.000000 eFatura-1.0.2/eFatura/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-18 12:17:07.000000 eFatura-1.0.2/eFatura/arayuz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-18 12:17:07.000000 eFatura-1.0.2/eFatura/konsol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15717 2023-05-18 12:17:07.000000 eFatura-1.0.2/eFatura/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:17:29.575943 eFatura-1.0.2/eFatura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-05-18 12:17:29.000000 eFatura-1.0.2/eFatura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-18 12:17:29.000000 eFatura-1.0.2/eFatura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 12:17:29.000000 eFatura-1.0.2/eFatura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-18 12:17:29.000000 eFatura-1.0.2/eFatura.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-18 12:17:29.000000 eFatura-1.0.2/eFatura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-18 12:17:29.000000 eFatura-1.0.2/eFatura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 12:17:29.575943 eFatura-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-18 12:17:07.000000 eFatura-1.0.2/setup.py
```

### Comparing `eFatura-1.0.1/README.md` & `eFatura-1.0.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,65 +1,117 @@
-# 🔍 E-Fatura Sorgu
+# 🔍 eFatura
 
-![Repo Boyutu](https://img.shields.io/github/repo-size/keyiflerolsun/E-Fatura_Sorgu?logo=git&logoColor=white)
-![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/E-Fatura_Sorgu&title=Görüntülenme)
+![Repo Boyutu](https://img.shields.io/github/repo-size/keyiflerolsun/eFatura?logo=git&logoColor=white)
+![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/eFatura&title=Görüntülenme)
 <a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/☕️-Kahve Ismarla-ffdd00" title="☕️ Kahve Ismarla" style="padding-left:5px;"></a>
 
 ![Python Version](https://img.shields.io/pypi/pyversions/eFatura?logo=python&logoColor=white)
 ![License](https://img.shields.io/pypi/l/eFatura?logo=gnu&logoColor=white)
 ![Status](https://img.shields.io/pypi/status/eFatura?logo=windowsterminal&logoColor=white)
 
-![PyPI](https://img.shields.io/pypi/v/eFatura?logo=pypi&logoColor=white)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/eFatura?logo=pypi&logoColor=white)
-![PyPI - Wheel](https://img.shields.io/pypi/wheel/eFatura?logo=pypi&logoColor=white)
+[![PyPI](https://img.shields.io/pypi/v/eFatura?logo=pypi&logoColor=white)](https://pypi.org/project/eFatura)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/eFatura?logo=pypi&logoColor=white)](https://pypi.org/project/eFatura)
+[![PyPI - Wheel](https://img.shields.io/pypi/wheel/eFatura?logo=pypi&logoColor=white)](https://pypi.org/project/eFatura)
 
-[![Fonksiyon Testleri ve PyPI Yükle](https://github.com/keyiflerolsun/E-Fatura_Sorgu/actions/workflows/KekikFlow.yml/badge.svg)](https://github.com/keyiflerolsun/E-Fatura_Sorgu/actions/workflows/KekikFlow.yml)
+[![Fonksiyon Testleri ve PyPI Yükle](https://github.com/keyiflerolsun/eFatura/actions/workflows/KekikFlow.yml/badge.svg)](https://github.com/keyiflerolsun/eFatura/actions/workflows/KekikFlow.yml)
 
 *Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu*
 
+![eFatura](https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/SS.png)
+
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🚀 Kurulum
 
+### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/pypi.svg"> PyPi (Lib - CLI - UI)
+
 ```bash
 # Yüklemek
 pip install eFatura
 
 # Güncellemek
 pip install -U eFatura
 ```
 
 ## 📝 Kullanım
 
+### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/python.svg"> Lib
+
 ```python
 from eFatura import e_fatura
 
 print(e_fatura("11111111111")) # Vergi Numarası veya TC Kimlik Numarası
 
 >> True | False
 ```
 
+### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/iterm2.svg"> CLI
+
 ```bash
 eFatura 11111111111
+
+# » [~] 11111111111 Numarası E-Fatura Mükellefi Değildir..
+```
+
+### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/freedesktop.svg"> UI
+
+```bash
+eFaturaGUI
 ```
 
 ## 📝 Proje Sahibi
 
 - ✅ **[kmprens/CheckEinvoice](https://github.com/kmprens/CheckEinvoice)**
 
+---
+
+<details>
+    <summary style="font-weight: bold; font-size: 20px">
+      <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/buddy.svg"> <b>Manuel Derlemek</b>
+      <i>(genişletmek için tıklayın!)</i>
+    </summary>
+    <br/>
+
+### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/python.svg"> Python
+
+```bash
+# Depoyu Çek
+https://github.com/keyiflerolsun/eFatura.git
+cd eFatura
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
+eFatura     # CLI
+eFaturaGUI  # GUI
+
+# Paketi Kaldır
+pip uninstall eFatura
+```
+</details>
+
+---
+
 ## 🌐 Telif Hakkı ve Lisans
 
 * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
-* [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/E-Fatura_Sorgu/blob/master/LICENSE) *Koşullarına göre lisanslanmıştır..*
+* [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/eFatura/blob/master/LICENSE) *Koşullarına göre lisanslanmıştır..*
 
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
@@ -1,31 +1,49 @@
-# ð E-Fatura Sorgu ![Repo Boyutu](https://img.shields.io/github/repo-size/
-keyiflerolsun/E-Fatura_Sorgu?logo=git&logoColor=white) ![GÃ¶rÃ¼ntÃ¼lenme]
-(https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/
-keyiflerolsun/E-Fatura_Sorgu&title=GÃ¶rÃ¼ntÃ¼lenme) [https://img.shields.io/
-badge/âï¸-Kahve_Ismarla-ffdd00] ![Python Version](https://img.shields.io/
-pypi/pyversions/eFatura?logo=python&logoColor=white) ![License](https://
+# ð eFatura ![Repo Boyutu](https://img.shields.io/github/repo-size/
+keyiflerolsun/eFatura?logo=git&logoColor=white) ![GÃ¶rÃ¼ntÃ¼lenme](https://
+hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/
+keyiflerolsun/eFatura&title=GÃ¶rÃ¼ntÃ¼lenme) [https://img.shields.io/badge/
+âï¸-Kahve_Ismarla-ffdd00] ![Python Version](https://img.shields.io/pypi/
+pyversions/eFatura?logo=python&logoColor=white) ![License](https://
 img.shields.io/pypi/l/eFatura?logo=gnu&logoColor=white) ![Status](https://
-img.shields.io/pypi/status/eFatura?logo=windowsterminal&logoColor=white) !
-[PyPI](https://img.shields.io/pypi/v/eFatura?logo=pypi&logoColor=white) ![PyPI
-- Downloads](https://img.shields.io/pypi/dm/eFatura?logo=pypi&logoColor=white)
-![PyPI - Wheel](https://img.shields.io/pypi/wheel/
-eFatura?logo=pypi&logoColor=white) [![Fonksiyon Testleri ve PyPI YÃ¼kle](https:
-//github.com/keyiflerolsun/E-Fatura_Sorgu/actions/workflows/KekikFlow.yml/
-badge.svg)](https://github.com/keyiflerolsun/E-Fatura_Sorgu/actions/workflows/
-KekikFlow.yml) *Vergi veya TC Kimlik NumarasÄ±ndan E-Fatura MÃ¼kellefiyet
-Sorgusu* [![ForTheBadge made-with-python](https://ForTheBadge.com/images/
-badges/made-with-python.svg)](https://www.python.org/) [![ForTheBadge built-
-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://
-GitHub.com/keyiflerolsun/) ## ð Kurulum ```bash # YÃ¼klemek pip install
-eFatura # GÃ¼ncellemek pip install -U eFatura ``` ## ð KullanÄ±m ```python
-from eFatura import e_fatura print(e_fatura("11111111111")) # Vergi NumarasÄ±
-veya TC Kimlik NumarasÄ± >> True | False ``` ```bash eFatura 11111111111 ``` ##
-ð Proje Sahibi - â **[kmprens/CheckEinvoice](https://github.com/kmprens/
-CheckEinvoice)** ## ð Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by*
-[keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL
-PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/E-
-Fatura_Sorgu/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ##
-â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek isterseniz, **Telegram**'dan
-mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ##
-ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)** ##
-> **[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
+img.shields.io/pypi/status/eFatura?logo=windowsterminal&logoColor=white) [!
+[PyPI](https://img.shields.io/pypi/v/eFatura?logo=pypi&logoColor=white)](https:
+//pypi.org/project/eFatura) [![PyPI - Downloads](https://img.shields.io/pypi/
+dm/eFatura?logo=pypi&logoColor=white)](https://pypi.org/project/eFatura) [!
+[PyPI - Wheel](https://img.shields.io/pypi/wheel/
+eFatura?logo=pypi&logoColor=white)](https://pypi.org/project/eFatura) [!
+[Fonksiyon Testleri ve PyPI YÃ¼kle](https://github.com/keyiflerolsun/eFatura/
+actions/workflows/KekikFlow.yml/badge.svg)](https://github.com/keyiflerolsun/
+eFatura/actions/workflows/KekikFlow.yml) *Vergi veya TC Kimlik NumarasÄ±ndan E-
+Fatura MÃ¼kellefiyet Sorgusu* ![eFatura](https://raw.githubusercontent.com/
+keyiflerolsun/eFatura/main/.github/icons/SS.png) [![ForTheBadge made-with-
+python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://
+www.python.org/) [![ForTheBadge built-with-love](https://ForTheBadge.com/
+images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð
+Kurulum ### [https://raw.githubusercontent.com/keyiflerolsun/eFatura/
+main/.github/icons/pypi.svg] PyPi (Lib - CLI - UI) ```bash # YÃ¼klemek pip
+install eFatura # GÃ¼ncellemek pip install -U eFatura ``` ## ð KullanÄ±m ###
+[https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/
+python.svg] Lib ```python from eFatura import e_fatura print(e_fatura
+("11111111111")) # Vergi NumarasÄ± veya TC Kimlik NumarasÄ± >> True | False ```
+### [https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/
+icons/iterm2.svg] CLI ```bash eFatura 11111111111 # Â» [~] 11111111111
+NumarasÄ± E-Fatura MÃ¼kellefi DeÄildir.. ``` ### [https://
+raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/
+freedesktop.svg] UI ```bash eFaturaGUI ``` ## ð Proje Sahibi - â **
+[kmprens/CheckEinvoice](https://github.com/kmprens/CheckEinvoice)** ---
+[https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/
+buddy.svg] Manuel Derlemek (geniÅletmek iÃ§in tÄ±klayÄ±n!)
+### [https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/
+icons/python.svg] Python ```bash # Depoyu Ãek https://github.com/
+keyiflerolsun/eFatura.git cd eFatura # Gerekli OrtamlarÄ± Kur pip install -
+U pip setuptools wheel twine # Paketi YÃ¼kle pip install . # ArtÄ±klarÄ±
+Temizle rm -rf build *.egg-info # ÃalÄ±ÅtÄ±r eFatura # CLI eFaturaGUI # GUI #
+Paketi KaldÄ±r pip uninstall eFatura ```  --- ## ð Telif HakkÄ± ve Lisans *
+*Copyright (C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun)
+â¤ï¸ï¸ * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://
+github.com/keyiflerolsun/eFatura/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re
+lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek
+isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun]
+(https://t.me/KekikKahve) ## ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https:/
+/KekikAkademi.org/Kahve)** *** > **[@KekikAkademi](https://t.me/KekikAkademi)**
+*iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
```

### Comparing `eFatura-1.0.1/eFatura/Oturum.py` & `eFatura-1.0.2/eFatura/Oturum.py`

 * *Files identical despite different names*

### Comparing `eFatura-1.0.1/eFatura/__init__.py` & `eFatura-1.0.2/eFatura/__init__.py`

 * *Files identical despite different names*

### Comparing `eFatura-1.0.1/eFatura/konsol.py` & `eFatura-1.0.2/eFatura/konsol.py`

 * *Files identical despite different names*

### Comparing `eFatura-1.0.1/setup.py` & `eFatura-1.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 from io         import open
 
 setup(
     # ? Genel Bilgiler
     name         = "eFatura",
-    version      = "1.0.1",
+    version      = "1.0.2",
     url          = "https://github.com/keyiflerolsun/E-Fatura_Sorgu",
     description  = "Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu",
     keywords     = ["eFatura", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
 
@@ -27,21 +27,24 @@
     install_requires = [
         "setuptools",
         "wheel",
         "Kekik",
         "requests",
         "urllib3",
         "Pillow",
-        "pytesseract"
+        "pytesseract",
+        # "pygobject",
+        # "pygobject-stubs"
     ],
 
     # ? Konsoldan Çalıştırılabilir
     entry_points = {
         "console_scripts": [
-            "eFatura = eFatura.konsol:basla",
+            "eFatura    = eFatura.konsol:basla",
+            "eFaturaGUI = eFatura.arayuz:basla"
         ]
     },
 
     # ? PyPI Bilgileri
     long_description_content_type = "text/markdown",
     long_description              = "".join(open("README.md", encoding="utf-8").readlines()),
     include_package_data          = True
```

