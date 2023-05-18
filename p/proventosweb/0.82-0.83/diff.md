# Comparing `tmp/proventosweb-0.82.tar.gz` & `tmp/proventosweb-0.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proventosweb-0.82.tar", last modified: Thu May 18 19:26:50 2023, max compression
+gzip compressed data, was "proventosweb-0.83.tar", last modified: Thu May 18 19:47:57 2023, max compression
```

## Comparing `proventosweb-0.82.tar` & `proventosweb-0.83.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 19:26:50.828626 proventosweb-0.82/
--rw-rw-rw-   0        0        0      315 2023-05-18 19:26:50.828626 proventosweb-0.82/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-18 19:26:50.797379 proventosweb-0.82/proventosweb/
--rw-rw-rw-   0        0        0       44 2023-05-08 12:50:56.000000 proventosweb-0.82/proventosweb/__init__.py
--rw-rw-rw-   0        0        0    14311 2023-05-18 19:17:51.000000 proventosweb-0.82/proventosweb/proventosweb.py
-drwxrwxrwx   0        0        0        0 2023-05-18 19:26:50.828626 proventosweb-0.82/proventosweb.egg-info/
--rw-rw-rw-   0        0        0      315 2023-05-18 19:26:50.000000 proventosweb-0.82/proventosweb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-05-18 19:26:50.000000 proventosweb-0.82/proventosweb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 19:26:50.000000 proventosweb-0.82/proventosweb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-03 22:03:21.000000 proventosweb-0.82/proventosweb.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       35 2023-05-18 19:26:50.000000 proventosweb-0.82/proventosweb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-18 19:26:50.000000 proventosweb-0.82/proventosweb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 19:26:50.828626 proventosweb-0.82/setup.cfg
--rw-rw-rw-   0        0        0      517 2023-05-18 19:18:17.000000 proventosweb-0.82/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 19:47:57.575434 proventosweb-0.83/
+-rw-rw-rw-   0        0        0      315 2023-05-18 19:47:57.575434 proventosweb-0.83/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-18 19:47:57.559760 proventosweb-0.83/proventosweb/
+-rw-rw-rw-   0        0        0       44 2023-05-08 12:50:56.000000 proventosweb-0.83/proventosweb/__init__.py
+-rw-rw-rw-   0        0        0    14336 2023-05-18 19:47:22.000000 proventosweb-0.83/proventosweb/proventosweb.py
+drwxrwxrwx   0        0        0        0 2023-05-18 19:47:57.575434 proventosweb-0.83/proventosweb.egg-info/
+-rw-rw-rw-   0        0        0      315 2023-05-18 19:47:56.000000 proventosweb-0.83/proventosweb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-05-18 19:47:57.000000 proventosweb-0.83/proventosweb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 19:47:56.000000 proventosweb-0.83/proventosweb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-03 22:03:21.000000 proventosweb-0.83/proventosweb.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       35 2023-05-18 19:47:57.000000 proventosweb-0.83/proventosweb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-18 19:47:57.000000 proventosweb-0.83/proventosweb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 19:47:57.575434 proventosweb-0.83/setup.cfg
+-rw-rw-rw-   0        0        0      517 2023-05-18 19:47:22.000000 proventosweb-0.83/setup.py
```

### Comparing `proventosweb-0.82/proventosweb/proventosweb.py` & `proventosweb-0.83/proventosweb/proventosweb.py`

 * *Files 0% similar despite different names*

```diff
@@ -266,16 +266,16 @@
         session = requests.Session()
     for tempo in tempos:
         soup, tipo2 = procurandotipo(acao, tempo, session, headers, tipos)
         if soup is not None:
             break
     dfin = None
     if soup is None:
-        print("Tipo não encontrado")
-    else:
+        print("Ação não encontrada: "+acao)
+    elif tipo2 != 'etfs':
         value = soup.find('input', {'id': 'results'}).get('value')
         if value == '[]':
             print(acao + ' sem dividendos')
             df = None
         else:
             data = json.loads(value)
             try:
```

### Comparing `proventosweb-0.82/setup.py` & `proventosweb-0.83/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='proventosweb',
-      version='0.82',
+      version='0.83',
       description='Uma biblioteca para buscar proventos de ações na plataforma Status Invest',
       url='https://github.com/rafaelpsampaio/proventosweb',
       author='Rafael Sampaio',
       author_email='rafapsampaio@gmail.com',
       packages=['proventosweb'],
       install_requires=[
           'pandas',
```

