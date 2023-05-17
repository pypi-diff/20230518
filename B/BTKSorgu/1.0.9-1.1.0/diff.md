# Comparing `tmp/BTKSorgu-1.0.9.tar.gz` & `tmp/BTKSorgu-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BTKSorgu-1.0.9.tar", last modified: Wed May 17 22:53:15 2023, max compression
+gzip compressed data, was "BTKSorgu-1.1.0.tar", last modified: Wed May 17 23:29:42 2023, max compression
```

## Comparing `BTKSorgu-1.0.9.tar` & `BTKSorgu-1.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:53:15.168375 BTKSorgu-1.0.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:53:15.168375 BTKSorgu-1.0.9/BTKSorgu/
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-17 22:52:55.000000 BTKSorgu-1.0.9/BTKSorgu/Erisim_Engeli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-17 22:52:55.000000 BTKSorgu-1.0.9/BTKSorgu/KekikGUI.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-17 22:52:55.000000 BTKSorgu-1.0.9/BTKSorgu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-17 22:52:55.000000 BTKSorgu-1.0.9/BTKSorgu/arayuz.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-17 22:52:55.000000 BTKSorgu-1.0.9/BTKSorgu/konsol.py
--rw-r--r--   0 runner    (1001) docker     (123)    15717 2023-05-17 22:52:55.000000 BTKSorgu-1.0.9/BTKSorgu/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:53:15.168375 BTKSorgu-1.0.9/BTKSorgu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-05-17 22:53:15.000000 BTKSorgu-1.0.9/BTKSorgu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-17 22:53:15.000000 BTKSorgu-1.0.9/BTKSorgu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 22:53:15.000000 BTKSorgu-1.0.9/BTKSorgu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-17 22:53:15.000000 BTKSorgu-1.0.9/BTKSorgu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-17 22:53:15.000000 BTKSorgu-1.0.9/BTKSorgu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 22:53:15.000000 BTKSorgu-1.0.9/BTKSorgu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-17 22:52:55.000000 BTKSorgu-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-17 22:52:55.000000 BTKSorgu-1.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-05-17 22:53:15.168375 BTKSorgu-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-05-17 22:52:55.000000 BTKSorgu-1.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:53:15.168375 BTKSorgu-1.0.9/Shared/
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-17 22:52:55.000000 BTKSorgu-1.0.9/Shared/org.KekikAkademi.BTKSorgu.appdata.xml
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-17 22:52:55.000000 BTKSorgu-1.0.9/Shared/org.KekikAkademi.BTKSorgu.desktop
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-17 22:52:55.000000 BTKSorgu-1.0.9/Shared/org.KekikAkademi.BTKSorgu.svg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 22:53:15.168375 BTKSorgu-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-17 22:52:55.000000 BTKSorgu-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:29:42.706414 BTKSorgu-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:29:42.706414 BTKSorgu-1.1.0/BTKSorgu/
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-17 23:29:22.000000 BTKSorgu-1.1.0/BTKSorgu/Erisim_Engeli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-17 23:29:22.000000 BTKSorgu-1.1.0/BTKSorgu/KekikGUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-17 23:29:22.000000 BTKSorgu-1.1.0/BTKSorgu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-17 23:29:22.000000 BTKSorgu-1.1.0/BTKSorgu/arayuz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-17 23:29:22.000000 BTKSorgu-1.1.0/BTKSorgu/konsol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15717 2023-05-17 23:29:22.000000 BTKSorgu-1.1.0/BTKSorgu/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:29:42.706414 BTKSorgu-1.1.0/BTKSorgu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-05-17 23:29:42.000000 BTKSorgu-1.1.0/BTKSorgu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-17 23:29:42.000000 BTKSorgu-1.1.0/BTKSorgu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 23:29:42.000000 BTKSorgu-1.1.0/BTKSorgu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-17 23:29:42.000000 BTKSorgu-1.1.0/BTKSorgu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-17 23:29:42.000000 BTKSorgu-1.1.0/BTKSorgu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 23:29:42.000000 BTKSorgu-1.1.0/BTKSorgu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-17 23:29:22.000000 BTKSorgu-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-17 23:29:22.000000 BTKSorgu-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-05-17 23:29:42.706414 BTKSorgu-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-05-17 23:29:22.000000 BTKSorgu-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:29:42.706414 BTKSorgu-1.1.0/Shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-17 23:29:22.000000 BTKSorgu-1.1.0/Shared/org.KekikAkademi.BTKSorgu.appdata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-17 23:29:22.000000 BTKSorgu-1.1.0/Shared/org.KekikAkademi.BTKSorgu.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-17 23:29:22.000000 BTKSorgu-1.1.0/Shared/org.KekikAkademi.BTKSorgu.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 23:29:42.706414 BTKSorgu-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-17 23:29:22.000000 BTKSorgu-1.1.0/setup.py
```

### Comparing `BTKSorgu-1.0.9/BTKSorgu/Erisim_Engeli.py` & `BTKSorgu-1.1.0/BTKSorgu/Erisim_Engeli.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.9/BTKSorgu/KekikGUI.py` & `BTKSorgu-1.1.0/BTKSorgu/KekikGUI.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.9/BTKSorgu/arayuz.py` & `BTKSorgu-1.1.0/BTKSorgu/arayuz.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.9/BTKSorgu/konsol.py` & `BTKSorgu-1.1.0/BTKSorgu/konsol.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.9/BTKSorgu/logo.png` & `BTKSorgu-1.1.0/BTKSorgu/logo.png`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.9/BTKSorgu.egg-info/PKG-INFO` & `BTKSorgu-1.1.0/BTKSorgu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTKSorgu
-Version: 1.0.9
+Version: 1.1.0
 Summary: Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu
 Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: BTKSorgu,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: BTKSorgu Version: 1.0.9 Summary: Hedef websitesinin
+Metadata-Version: 2.1 Name: BTKSorgu Version: 1.1.0 Summary: Hedef websitesinin
 BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
 keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
```

### Comparing `BTKSorgu-1.0.9/LICENSE` & `BTKSorgu-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.9/PKG-INFO` & `BTKSorgu-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTKSorgu
-Version: 1.0.9
+Version: 1.1.0
 Summary: Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu
 Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: BTKSorgu,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: BTKSorgu Version: 1.0.9 Summary: Hedef websitesinin
+Metadata-Version: 2.1 Name: BTKSorgu Version: 1.1.0 Summary: Hedef websitesinin
 BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
 keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
```

### Comparing `BTKSorgu-1.0.9/README.md` & `BTKSorgu-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.9/Shared/org.KekikAkademi.BTKSorgu.appdata.xml` & `BTKSorgu-1.1.0/Shared/org.KekikAkademi.BTKSorgu.appdata.xml`

 * *Files 0% similar despite different names*

#### Comparing `BTKSorgu-1.0.9/Shared/org.KekikAkademi.BTKSorgu.appdata.xml` & `BTKSorgu-1.1.0/Shared/org.KekikAkademi.BTKSorgu.appdata.xml`

```diff
@@ -25,15 +25,15 @@
       <image>https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png</image>
     </screenshot>
   </screenshots>
   <categories>
     <category>Education</category>
   </categories>
   <releases>
-    <release version="1.0.8" date="2023-5-18">
+    <release version="1.1.0" date="2023-5-18">
       <description>
         <p>Readme Genişletildi ve Manuel Derleme Aşamaları Eklendi..</p>
       </description>
     </release>
     <release version="1.0.8" date="2023-5-17">
       <description>
         <p>Readme Düzenlendi..</p>
```

### Comparing `BTKSorgu-1.0.9/Shared/org.KekikAkademi.BTKSorgu.svg` & `BTKSorgu-1.1.0/Shared/org.KekikAkademi.BTKSorgu.svg`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.9/setup.py` & `BTKSorgu-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 from io         import open
 
 setup(
     # ? Genel Bilgiler
     name         = "BTKSorgu",
-    version      = "1.0.9",
+    version      = "1.1.0",
     url          = "https://github.com/keyiflerolsun/E-Fatura_Sorgu",
     description  = "Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu",
     keywords     = ["BTKSorgu", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
```

