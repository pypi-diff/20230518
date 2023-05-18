# Comparing `tmp/proventosweb-0.81.tar.gz` & `tmp/proventosweb-0.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proventosweb-0.81.tar", last modified: Thu May 18 19:09:57 2023, max compression
+gzip compressed data, was "proventosweb-0.82.tar", last modified: Thu May 18 19:26:50 2023, max compression
```

## Comparing `proventosweb-0.81.tar` & `proventosweb-0.82.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 19:09:57.233932 proventosweb-0.81/
--rw-rw-rw-   0        0        0      315 2023-05-18 19:09:57.232202 proventosweb-0.81/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-18 19:09:57.200927 proventosweb-0.81/proventosweb/
--rw-rw-rw-   0        0        0       44 2023-05-08 12:50:56.000000 proventosweb-0.81/proventosweb/__init__.py
--rw-rw-rw-   0        0        0    14293 2023-05-18 19:08:58.000000 proventosweb-0.81/proventosweb/proventosweb.py
-drwxrwxrwx   0        0        0        0 2023-05-18 19:09:57.216572 proventosweb-0.81/proventosweb.egg-info/
--rw-rw-rw-   0        0        0      315 2023-05-18 19:09:56.000000 proventosweb-0.81/proventosweb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-05-18 19:09:57.000000 proventosweb-0.81/proventosweb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 19:09:56.000000 proventosweb-0.81/proventosweb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-03 22:03:21.000000 proventosweb-0.81/proventosweb.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       35 2023-05-18 19:09:56.000000 proventosweb-0.81/proventosweb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-18 19:09:57.000000 proventosweb-0.81/proventosweb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 19:09:57.233932 proventosweb-0.81/setup.cfg
--rw-rw-rw-   0        0        0      517 2023-05-18 19:09:29.000000 proventosweb-0.81/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 19:26:50.828626 proventosweb-0.82/
+-rw-rw-rw-   0        0        0      315 2023-05-18 19:26:50.828626 proventosweb-0.82/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-18 19:26:50.797379 proventosweb-0.82/proventosweb/
+-rw-rw-rw-   0        0        0       44 2023-05-08 12:50:56.000000 proventosweb-0.82/proventosweb/__init__.py
+-rw-rw-rw-   0        0        0    14311 2023-05-18 19:17:51.000000 proventosweb-0.82/proventosweb/proventosweb.py
+drwxrwxrwx   0        0        0        0 2023-05-18 19:26:50.828626 proventosweb-0.82/proventosweb.egg-info/
+-rw-rw-rw-   0        0        0      315 2023-05-18 19:26:50.000000 proventosweb-0.82/proventosweb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-05-18 19:26:50.000000 proventosweb-0.82/proventosweb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 19:26:50.000000 proventosweb-0.82/proventosweb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-03 22:03:21.000000 proventosweb-0.82/proventosweb.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       35 2023-05-18 19:26:50.000000 proventosweb-0.82/proventosweb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-18 19:26:50.000000 proventosweb-0.82/proventosweb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 19:26:50.828626 proventosweb-0.82/setup.cfg
+-rw-rw-rw-   0        0        0      517 2023-05-18 19:18:17.000000 proventosweb-0.82/setup.py
```

### Comparing `proventosweb-0.81/proventosweb/proventosweb.py` & `proventosweb-0.82/proventosweb/proventosweb.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,15 +233,16 @@
 
 def procurandotipo(acao, tempo, session, headers, tipos):
     tipo2 = None
     soup = None
     for tipo in tipos:
         try:
             url = 'https://statusinvest.com.br/' + tipo + '/' + acao
-            resposta = session.get(url, headers=headers, timeout=tempo)
+            resposta = session.get(url, headers={'User-Agent': headers}, timeout=tempo)
+
             if resposta.status_code == 200:
                 amostra = resposta.text
                 soup1 = BeautifulSoup(amostra, 'html.parser')
                 if soup1.find('title').text != 'OPS. . .Não encontramos o que você está procurando | Status Invest':
                     soup = soup1
                     tipo2 = tipo
                     break
```

### Comparing `proventosweb-0.81/setup.py` & `proventosweb-0.82/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='proventosweb',
-      version='0.81',
+      version='0.82',
       description='Uma biblioteca para buscar proventos de ações na plataforma Status Invest',
       url='https://github.com/rafaelpsampaio/proventosweb',
       author='Rafael Sampaio',
       author_email='rafapsampaio@gmail.com',
       packages=['proventosweb'],
       install_requires=[
           'pandas',
```

