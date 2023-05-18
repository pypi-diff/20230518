# Comparing `tmp/sb6-0.0.1.tar.gz` & `tmp/sb6-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sb6-0.0.1.tar", last modified: Fri May 12 19:18:19 2023, max compression
+gzip compressed data, was "sb6-0.0.2.tar", last modified: Thu May 18 12:59:45 2023, max compression
```

## Comparing `sb6-0.0.1.tar` & `sb6-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:19.902412 sb6-0.0.1/
--rw-rw-rw-   0        0        0     1067 2023-04-11 12:54:43.000000 sb6-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      462 2023-05-12 19:18:19.902412 sb6-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       69 2023-05-12 01:06:50.000000 sb6-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-12 19:18:19.902412 sb6-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      769 2023-05-12 17:49:09.000000 sb6-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:19.886231 sb6-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-12 19:18:19.902412 sb6-0.0.1/src/sb6.egg-info/
--rw-rw-rw-   0        0        0      462 2023-05-12 19:18:19.000000 sb6-0.0.1/src/sb6.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      191 2023-05-12 19:18:19.000000 sb6-0.0.1/src/sb6.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 19:18:19.000000 sb6-0.0.1/src/sb6.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-12 19:18:19.000000 sb6-0.0.1/src/sb6.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-12 19:18:19.000000 sb6-0.0.1/src/sb6.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    94314 2023-05-12 19:17:01.000000 sb6-0.0.1/src/sb6.py
+drwxrwxrwx   0        0        0        0 2023-05-18 12:59:45.221224 sb6-0.0.2/
+-rw-rw-rw-   0        0        0     1067 2023-04-11 12:54:43.000000 sb6-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      462 2023-05-18 12:59:45.221224 sb6-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       69 2023-05-12 01:06:50.000000 sb6-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-18 12:59:45.221224 sb6-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      769 2023-05-18 12:56:54.000000 sb6-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 12:59:45.201588 sb6-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-18 12:59:45.221224 sb6-0.0.2/src/sb6.egg-info/
+-rw-rw-rw-   0        0        0      462 2023-05-18 12:59:45.000000 sb6-0.0.2/src/sb6.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2023-05-18 12:59:45.000000 sb6-0.0.2/src/sb6.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 12:59:45.000000 sb6-0.0.2/src/sb6.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-18 12:59:45.000000 sb6-0.0.2/src/sb6.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-18 12:59:45.000000 sb6-0.0.2/src/sb6.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0   123303 2023-05-17 19:50:11.000000 sb6-0.0.2/src/sb6.py
```

### Comparing `sb6-0.0.1/LICENSE` & `sb6-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sb6-0.0.1/setup.py` & `sb6-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sb6",
-    version="0.0.1",
+    version="0.0.2",
     description='chatbot',
     license='MIT',
     author="aiml department",
     author_email="aiml@gmail.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
```

