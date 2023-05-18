# Comparing `tmp/proventosweb-0.70.tar.gz` & `tmp/proventosweb-0.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proventosweb-0.70.tar", last modified: Thu May 18 18:55:15 2023, max compression
+gzip compressed data, was "proventosweb-0.80.tar", last modified: Thu May 18 19:04:06 2023, max compression
```

## Comparing `proventosweb-0.70.tar` & `proventosweb-0.80.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 18:55:15.135430 proventosweb-0.70/
--rw-rw-rw-   0        0        0      315 2023-05-18 18:55:15.135430 proventosweb-0.70/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-18 18:55:15.103105 proventosweb-0.70/proventosweb/
--rw-rw-rw-   0        0        0       44 2023-05-08 12:50:56.000000 proventosweb-0.70/proventosweb/__init__.py
--rw-rw-rw-   0        0        0    12842 2023-05-18 18:48:39.000000 proventosweb-0.70/proventosweb/proventosweb.py
-drwxrwxrwx   0        0        0        0 2023-05-18 18:55:15.121372 proventosweb-0.70/proventosweb.egg-info/
--rw-rw-rw-   0        0        0      315 2023-05-18 18:55:14.000000 proventosweb-0.70/proventosweb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-05-18 18:55:14.000000 proventosweb-0.70/proventosweb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 18:55:14.000000 proventosweb-0.70/proventosweb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-03 22:03:21.000000 proventosweb-0.70/proventosweb.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       35 2023-05-18 18:55:14.000000 proventosweb-0.70/proventosweb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-18 18:55:14.000000 proventosweb-0.70/proventosweb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 18:55:15.135430 proventosweb-0.70/setup.cfg
--rw-rw-rw-   0        0        0      517 2023-05-18 18:48:57.000000 proventosweb-0.70/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 19:04:06.447975 proventosweb-0.80/
+-rw-rw-rw-   0        0        0      315 2023-05-18 19:04:06.447975 proventosweb-0.80/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-18 19:04:06.416634 proventosweb-0.80/proventosweb/
+-rw-rw-rw-   0        0        0       44 2023-05-08 12:50:56.000000 proventosweb-0.80/proventosweb/__init__.py
+-rw-rw-rw-   0        0        0    13109 2023-05-18 19:00:37.000000 proventosweb-0.80/proventosweb/proventosweb.py
+drwxrwxrwx   0        0        0        0 2023-05-18 19:04:06.447975 proventosweb-0.80/proventosweb.egg-info/
+-rw-rw-rw-   0        0        0      315 2023-05-18 19:04:05.000000 proventosweb-0.80/proventosweb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-05-18 19:04:06.000000 proventosweb-0.80/proventosweb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 19:04:05.000000 proventosweb-0.80/proventosweb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-03 22:03:21.000000 proventosweb-0.80/proventosweb.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       35 2023-05-18 19:04:06.000000 proventosweb-0.80/proventosweb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-18 19:04:06.000000 proventosweb-0.80/proventosweb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 19:04:06.447975 proventosweb-0.80/setup.cfg
+-rw-rw-rw-   0        0        0      517 2023-05-18 19:03:52.000000 proventosweb-0.80/setup.py
```

### Comparing `proventosweb-0.70/proventosweb/proventosweb.py` & `proventosweb-0.80/proventosweb/proventosweb.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,18 +47,21 @@
     else:
         dfcons = pd.concat([dfp, dfb, dfbo, dfs], ignore_index=True)
         dfcons['Data COM'] = pd.to_datetime(dfcons['Data COM'], dayfirst=True).dt.date
         dfcons['Executado'] = dfcons['Executado'].replace('-', None)
         dfcons['Executado'] = pd.to_datetime(dfcons['Executado'], dayfirst=True).dt.date
         if sub is not None and not sub.empty:
             dfcons['Quantia'] = dfcons['Quantia'].replace({np.nan: None})
+            dfcons['Quantia'] = dfcons['Quantia'].replace({pd.NA: None})
         if prov is not None and not prov.empty:
             dfcons['Valor Original'] = dfcons['Valor Original'].replace({pd.NA: None})
+            dfcons['Valor Original'] = dfcons['Valor Original'].replace({np.nan: None})
         if boni is not None and not prov.empty:
             dfcons['Proporção'] = dfcons['Proporção'].replace({pd.NA: None})
+            dfcons['Proporção'] = dfcons['Proporção'].replace({np.nan: None})
         dfcons.sort_values(by=['Tipo', 'Data COM'])
     return dfcons
 
 
 def dobramento(strings):
     data = []
     for string in strings:
@@ -236,19 +239,19 @@
     return soup, tipo2
 
 
 def eventos(acao, session=0, headers=0):
     acao = acao.upper()
     tempos = [x / 10 for x in range(3, 10)]
     if acao[-2:] == '34':
-        tipos = ['bdrs', 'acoes', 'fundos-imobiliarios', 'fiinfras', 'fiagros', 'etfs']
+        tipos = ['bdrs', 'acoes', 'fundos-imobiliarios', 'fiinfras', 'fiagros','fips', 'etfs']
     elif acao[-2:] == '11':
-        tipos = ['fundos-imobiliarios', 'acoes', 'fiinfras', 'fiagros', 'etfs', 'bdrs']
+        tipos = ['fundos-imobiliarios', 'acoes', 'fiinfras', 'fiagros','fips', 'etfs', 'bdrs']
     else:
-        tipos = ['acoes', 'fundos-imobiliarios', 'fiinfras', 'fiagros', 'etfs', 'bdrs']
+        tipos = ['acoes', 'fundos-imobiliarios', 'fiinfras', 'fiagros', 'etfs','fips', 'bdrs']
     if session == 0:
         headers = {
             'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.36'}
         session = requests.Session()
     for tempo in tempos:
         soup, tipo2 = procurandotipo(acao, tempo, session, headers, tipos)
         if soup is not None:
```

### Comparing `proventosweb-0.70/setup.py` & `proventosweb-0.80/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='proventosweb',
-      version='0.70',
+      version='0.80',
       description='Uma biblioteca para buscar proventos de ações na plataforma Status Invest',
       url='https://github.com/rafaelpsampaio/proventosweb',
       author='Rafael Sampaio',
       author_email='rafapsampaio@gmail.com',
       packages=['proventosweb'],
       install_requires=[
           'pandas',
```

