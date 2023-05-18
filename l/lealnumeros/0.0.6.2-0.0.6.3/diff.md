# Comparing `tmp/lealnumeros-0.0.6.2.tar.gz` & `tmp/lealnumeros-0.0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lealnumeros-0.0.6.2.tar", last modified: Thu May 18 19:26:16 2023, max compression
+gzip compressed data, was "lealnumeros-0.0.6.3.tar", last modified: Thu May 18 19:30:37 2023, max compression
```

## Comparing `lealnumeros-0.0.6.2.tar` & `lealnumeros-0.0.6.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 19:26:16.210360 lealnumeros-0.0.6.2/
--rw-rw-rw-   0        0        0     1098 2023-05-18 19:18:17.000000 lealnumeros-0.0.6.2/LICENCE
--rw-rw-rw-   0        0        0     1989 2023-05-18 19:26:16.209361 lealnumeros-0.0.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     1665 2023-05-18 19:20:23.000000 lealnumeros-0.0.6.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 19:26:16.184375 lealnumeros-0.0.6.2/lealNumeros/
--rw-rw-rw-   0        0        0       32 2023-05-18 19:18:17.000000 lealnumeros-0.0.6.2/lealNumeros/__init__.py
--rw-rw-rw-   0        0        0     4650 2023-05-18 19:25:45.000000 lealnumeros-0.0.6.2/lealNumeros/main.py
-drwxrwxrwx   0        0        0        0 2023-05-18 19:26:16.208362 lealnumeros-0.0.6.2/lealnumeros.egg-info/
--rw-rw-rw-   0        0        0     1989 2023-05-18 19:26:16.000000 lealnumeros-0.0.6.2/lealnumeros.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-05-18 19:26:16.000000 lealnumeros-0.0.6.2/lealnumeros.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 19:26:16.000000 lealnumeros-0.0.6.2/lealnumeros.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-18 19:26:16.000000 lealnumeros-0.0.6.2/lealnumeros.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-18 19:26:16.000000 lealnumeros-0.0.6.2/lealnumeros.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 19:26:16.210360 lealnumeros-0.0.6.2/setup.cfg
--rw-rw-rw-   0        0        0      532 2023-05-18 19:26:10.000000 lealnumeros-0.0.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 19:30:37.888124 lealnumeros-0.0.6.3/
+-rw-rw-rw-   0        0        0     1098 2023-05-18 19:18:17.000000 lealnumeros-0.0.6.3/LICENCE
+-rw-rw-rw-   0        0        0     1989 2023-05-18 19:30:37.887131 lealnumeros-0.0.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1665 2023-05-18 19:20:23.000000 lealnumeros-0.0.6.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 19:30:37.855144 lealnumeros-0.0.6.3/lealNumeros/
+-rw-rw-rw-   0        0        0       32 2023-05-18 19:18:17.000000 lealnumeros-0.0.6.3/lealNumeros/__init__.py
+-rw-rw-rw-   0        0        0     4650 2023-05-18 19:29:01.000000 lealnumeros-0.0.6.3/lealNumeros/main.py
+drwxrwxrwx   0        0        0        0 2023-05-18 19:30:37.885127 lealnumeros-0.0.6.3/lealnumeros.egg-info/
+-rw-rw-rw-   0        0        0     1989 2023-05-18 19:30:37.000000 lealnumeros-0.0.6.3/lealnumeros.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-05-18 19:30:37.000000 lealnumeros-0.0.6.3/lealnumeros.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 19:30:37.000000 lealnumeros-0.0.6.3/lealnumeros.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-18 19:30:37.000000 lealnumeros-0.0.6.3/lealnumeros.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-18 19:30:37.000000 lealnumeros-0.0.6.3/lealnumeros.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 19:30:37.889125 lealnumeros-0.0.6.3/setup.cfg
+-rw-rw-rw-   0        0        0      532 2023-05-18 19:30:30.000000 lealnumeros-0.0.6.3/setup.py
```

### Comparing `lealnumeros-0.0.6.2/LICENCE` & `lealnumeros-0.0.6.3/LICENCE`

 * *Files identical despite different names*

### Comparing `lealnumeros-0.0.6.2/PKG-INFO` & `lealnumeros-0.0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lealnumeros
-Version: 0.0.6.2
+Version: 0.0.6.3
 Summary: Trabalhe com formatação de números de uma maneira rápido e fácil.
 Author: José Rodolfo
 Author-email: silvaleal.ctt@gmail.com
 License: MIT License
 Keywords: lealnumeros
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `lealnumeros-0.0.6.2/README.md` & `lealnumeros-0.0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `lealnumeros-0.0.6.2/lealNumeros/main.py` & `lealnumeros-0.0.6.3/lealNumeros/main.py`

 * *Files identical despite different names*

### Comparing `lealnumeros-0.0.6.2/lealnumeros.egg-info/PKG-INFO` & `lealnumeros-0.0.6.3/lealnumeros.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lealnumeros
-Version: 0.0.6.2
+Version: 0.0.6.3
 Summary: Trabalhe com formatação de números de uma maneira rápido e fácil.
 Author: José Rodolfo
 Author-email: silvaleal.ctt@gmail.com
 License: MIT License
 Keywords: lealnumeros
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `lealnumeros-0.0.6.2/setup.py` & `lealnumeros-0.0.6.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(name='lealnumeros',
-    version='0.0.6.2',
+    version='0.0.6.3',
     license='MIT License',
     author='José Rodolfo',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='silvaleal.ctt@gmail.com',
     keywords='lealnumeros',
     description=u'Trabalhe com formatação de números de uma maneira rápido e fácil.',
```

