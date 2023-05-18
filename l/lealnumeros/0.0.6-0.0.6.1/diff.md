# Comparing `tmp/lealnumeros-0.0.6.tar.gz` & `tmp/lealnumeros-0.0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lealnumeros-0.0.6.tar", last modified: Thu May 18 19:21:17 2023, max compression
+gzip compressed data, was "lealnumeros-0.0.6.1.tar", last modified: Thu May 18 19:23:25 2023, max compression
```

## Comparing `lealnumeros-0.0.6.tar` & `lealnumeros-0.0.6.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 19:21:17.742123 lealnumeros-0.0.6/
--rw-rw-rw-   0        0        0     1098 2023-05-18 19:18:17.000000 lealnumeros-0.0.6/LICENCE
--rw-rw-rw-   0        0        0     1987 2023-05-18 19:21:17.740126 lealnumeros-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1665 2023-05-18 19:20:23.000000 lealnumeros-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 19:21:17.701315 lealnumeros-0.0.6/lealNumeros/
--rw-rw-rw-   0        0        0       32 2023-05-18 19:18:17.000000 lealnumeros-0.0.6/lealNumeros/__init__.py
--rw-rw-rw-   0        0        0     4650 2023-05-18 19:18:17.000000 lealnumeros-0.0.6/lealNumeros/main.py
-drwxrwxrwx   0        0        0        0 2023-05-18 19:21:17.738120 lealnumeros-0.0.6/lealnumeros.egg-info/
--rw-rw-rw-   0        0        0     1987 2023-05-18 19:21:17.000000 lealnumeros-0.0.6/lealnumeros.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-05-18 19:21:17.000000 lealnumeros-0.0.6/lealnumeros.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 19:21:17.000000 lealnumeros-0.0.6/lealnumeros.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-18 19:21:17.000000 lealnumeros-0.0.6/lealnumeros.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-18 19:21:17.000000 lealnumeros-0.0.6/lealnumeros.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 19:21:17.742123 lealnumeros-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      517 2023-05-18 19:18:58.000000 lealnumeros-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 19:23:25.239568 lealnumeros-0.0.6.1/
+-rw-rw-rw-   0        0        0     1098 2023-05-18 19:18:17.000000 lealnumeros-0.0.6.1/LICENCE
+-rw-rw-rw-   0        0        0     1989 2023-05-18 19:23:25.238567 lealnumeros-0.0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1665 2023-05-18 19:20:23.000000 lealnumeros-0.0.6.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 19:23:25.200590 lealnumeros-0.0.6.1/lealNumeros/
+-rw-rw-rw-   0        0        0       32 2023-05-18 19:18:17.000000 lealnumeros-0.0.6.1/lealNumeros/__init__.py
+-rw-rw-rw-   0        0        0     4650 2023-05-18 19:18:17.000000 lealnumeros-0.0.6.1/lealNumeros/main.py
+drwxrwxrwx   0        0        0        0 2023-05-18 19:23:25.236570 lealnumeros-0.0.6.1/lealnumeros.egg-info/
+-rw-rw-rw-   0        0        0     1989 2023-05-18 19:23:25.000000 lealnumeros-0.0.6.1/lealnumeros.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-05-18 19:23:25.000000 lealnumeros-0.0.6.1/lealnumeros.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 19:23:25.000000 lealnumeros-0.0.6.1/lealnumeros.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-18 19:23:25.000000 lealnumeros-0.0.6.1/lealnumeros.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-18 19:23:25.000000 lealnumeros-0.0.6.1/lealnumeros.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 19:23:25.240567 lealnumeros-0.0.6.1/setup.cfg
+-rw-rw-rw-   0        0        0      532 2023-05-18 19:23:07.000000 lealnumeros-0.0.6.1/setup.py
```

### Comparing `lealnumeros-0.0.6/LICENCE` & `lealnumeros-0.0.6.1/LICENCE`

 * *Files identical despite different names*

### Comparing `lealnumeros-0.0.6/PKG-INFO` & `lealnumeros-0.0.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lealnumeros
-Version: 0.0.6
+Version: 0.0.6.1
 Summary: Trabalhe com formatação de números de uma maneira rápido e fácil.
 Author: José Rodolfo
 Author-email: silvaleal.ctt@gmail.com
 License: MIT License
 Keywords: lealnumeros
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `lealnumeros-0.0.6/README.md` & `lealnumeros-0.0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `lealnumeros-0.0.6/lealNumeros/main.py` & `lealnumeros-0.0.6.1/lealNumeros/main.py`

 * *Files identical despite different names*

### Comparing `lealnumeros-0.0.6/lealnumeros.egg-info/PKG-INFO` & `lealnumeros-0.0.6.1/lealnumeros.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lealnumeros
-Version: 0.0.6
+Version: 0.0.6.1
 Summary: Trabalhe com formatação de números de uma maneira rápido e fácil.
 Author: José Rodolfo
 Author-email: silvaleal.ctt@gmail.com
 License: MIT License
 Keywords: lealnumeros
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `lealnumeros-0.0.6/setup.py` & `lealnumeros-0.0.6.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(name='lealnumeros',
-    version='0.0.6',
+    version='0.0.6.1',
     license='MIT License',
     author='José Rodolfo',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='silvaleal.ctt@gmail.com',
     keywords='lealnumeros',
     description=u'Trabalhe com formatação de números de uma maneira rápido e fácil.',
     packages=['lealNumeros'],
-    install_requires=['num2words'],)
+    install_requires=['num2words', 'translate'],)
```

