# Comparing `tmp/proventosweb-0.80.tar.gz` & `tmp/proventosweb-0.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proventosweb-0.80.tar", last modified: Thu May 18 19:04:06 2023, max compression
+gzip compressed data, was "proventosweb-0.81.tar", last modified: Thu May 18 19:09:57 2023, max compression
```

## Comparing `proventosweb-0.80.tar` & `proventosweb-0.81.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 19:04:06.447975 proventosweb-0.80/
--rw-rw-rw-   0        0        0      315 2023-05-18 19:04:06.447975 proventosweb-0.80/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-18 19:04:06.416634 proventosweb-0.80/proventosweb/
--rw-rw-rw-   0        0        0       44 2023-05-08 12:50:56.000000 proventosweb-0.80/proventosweb/__init__.py
--rw-rw-rw-   0        0        0    13109 2023-05-18 19:00:37.000000 proventosweb-0.80/proventosweb/proventosweb.py
-drwxrwxrwx   0        0        0        0 2023-05-18 19:04:06.447975 proventosweb-0.80/proventosweb.egg-info/
--rw-rw-rw-   0        0        0      315 2023-05-18 19:04:05.000000 proventosweb-0.80/proventosweb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-05-18 19:04:06.000000 proventosweb-0.80/proventosweb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 19:04:05.000000 proventosweb-0.80/proventosweb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-03 22:03:21.000000 proventosweb-0.80/proventosweb.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       35 2023-05-18 19:04:06.000000 proventosweb-0.80/proventosweb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-18 19:04:06.000000 proventosweb-0.80/proventosweb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 19:04:06.447975 proventosweb-0.80/setup.cfg
--rw-rw-rw-   0        0        0      517 2023-05-18 19:03:52.000000 proventosweb-0.80/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 19:09:57.233932 proventosweb-0.81/
+-rw-rw-rw-   0        0        0      315 2023-05-18 19:09:57.232202 proventosweb-0.81/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-18 19:09:57.200927 proventosweb-0.81/proventosweb/
+-rw-rw-rw-   0        0        0       44 2023-05-08 12:50:56.000000 proventosweb-0.81/proventosweb/__init__.py
+-rw-rw-rw-   0        0        0    14293 2023-05-18 19:08:58.000000 proventosweb-0.81/proventosweb/proventosweb.py
+drwxrwxrwx   0        0        0        0 2023-05-18 19:09:57.216572 proventosweb-0.81/proventosweb.egg-info/
+-rw-rw-rw-   0        0        0      315 2023-05-18 19:09:56.000000 proventosweb-0.81/proventosweb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-05-18 19:09:57.000000 proventosweb-0.81/proventosweb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 19:09:56.000000 proventosweb-0.81/proventosweb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-03 22:03:21.000000 proventosweb-0.81/proventosweb.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       35 2023-05-18 19:09:56.000000 proventosweb-0.81/proventosweb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-18 19:09:57.000000 proventosweb-0.81/proventosweb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 19:09:57.233932 proventosweb-0.81/setup.cfg
+-rw-rw-rw-   0        0        0      517 2023-05-18 19:09:29.000000 proventosweb-0.81/setup.py
```

### Comparing `proventosweb-0.80/proventosweb/proventosweb.py` & `proventosweb-0.81/proventosweb/proventosweb.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pandas as pd
 import json
 import requests
 from bs4 import BeautifulSoup
 import numpy as np
 import time
-
+import random
 
 def percent_str_to_float(percent_str):
     decimal_str = percent_str.replace(',', '.')
     number_str = decimal_str.strip('%')
     number = float(number_str) / 100.0
     return number
 
@@ -149,16 +149,27 @@
 
     df_concat = pd.concat(dfs, ignore_index=True)
     return df
 
 
 def provlista(acoes, testtime=0):
     session = requests.Session()
-    headers = {
-        'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.36'}
+    headers_ar = [
+        'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.36',
+        'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.124 Safari/537.36',
+        'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.124 Safari/537.36',
+        'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:88.0) Gecko/20100101 Firefox/88.0',
+        'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.114 Safari/537.36',
+        'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.101 Safari/537.36',
+        'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.77 Safari/537.36',
+        'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.77 Safari/537.36',
+        'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.57 Safari/537.36',
+        'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.57 Safari/537.36'
+    ]
+    headers = random.choice(headers_ar)
     dfprov = pd.DataFrame(columns=['Ativo', 'Tipo', 'Data COM', 'Executado', 'Valor', 'Valor Original', 'Quantia'])
     cortes = [0.25, 0.5, 0.75, 1]
     if testtime == 1:
         print('Buscando proventos de ' + str(len(acoes)) + ' ações!')
         start_time = time.time()
         longest_atv = None
         longest_time = 0
```

### Comparing `proventosweb-0.80/setup.py` & `proventosweb-0.81/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='proventosweb',
-      version='0.80',
+      version='0.81',
       description='Uma biblioteca para buscar proventos de ações na plataforma Status Invest',
       url='https://github.com/rafaelpsampaio/proventosweb',
       author='Rafael Sampaio',
       author_email='rafapsampaio@gmail.com',
       packages=['proventosweb'],
       install_requires=[
           'pandas',
```

