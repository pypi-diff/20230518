# Comparing `tmp/interactivenlp-0.0.2.tar.gz` & `tmp/interactivenlp-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interactivenlp-0.0.2.tar", last modified: Thu May 18 20:29:30 2023, max compression
+gzip compressed data, was "interactivenlp-0.0.3.tar", last modified: Thu May 18 20:33:55 2023, max compression
```

## Comparing `interactivenlp-0.0.2.tar` & `interactivenlp-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 20:29:30.400629 interactivenlp-0.0.2/
--rw-rw-rw-   0        0        0     1090 2023-05-18 19:27:11.000000 interactivenlp-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      358 2023-05-18 20:29:30.398605 interactivenlp-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       64 2023-05-18 19:26:55.000000 interactivenlp-0.0.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-18 20:29:30.369975 interactivenlp-0.0.2/interactivenlp/
--rw-rw-rw-   0        0        0      281 2023-05-18 19:31:08.000000 interactivenlp-0.0.2/interactivenlp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 20:29:30.397636 interactivenlp-0.0.2/interactivenlp.egg-info/
--rw-rw-rw-   0        0        0      358 2023-05-18 20:29:30.000000 interactivenlp-0.0.2/interactivenlp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-05-18 20:29:30.000000 interactivenlp-0.0.2/interactivenlp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 20:29:30.000000 interactivenlp-0.0.2/interactivenlp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-18 20:29:30.000000 interactivenlp-0.0.2/interactivenlp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-18 20:29:30.000000 interactivenlp-0.0.2/interactivenlp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 20:29:30.400629 interactivenlp-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      616 2023-05-18 20:27:05.000000 interactivenlp-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 20:33:55.854048 interactivenlp-0.0.3/
+-rw-rw-rw-   0        0        0     1090 2023-05-18 19:27:11.000000 interactivenlp-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      358 2023-05-18 20:33:55.852043 interactivenlp-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       64 2023-05-18 19:26:55.000000 interactivenlp-0.0.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-18 20:33:55.821173 interactivenlp-0.0.3/interactivenlp/
+-rw-rw-rw-   0        0        0      281 2023-05-18 19:31:08.000000 interactivenlp-0.0.3/interactivenlp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 20:33:55.849045 interactivenlp-0.0.3/interactivenlp/typedef/
+-rw-rw-rw-   0        0        0        0 2023-05-18 20:33:03.000000 interactivenlp-0.0.3/interactivenlp/typedef/__init__.py
+-rw-rw-rw-   0        0        0     1106 2023-05-18 18:21:43.000000 interactivenlp-0.0.3/interactivenlp/typedef/block.py
+-rw-rw-rw-   0        0        0      189 2023-05-18 18:21:40.000000 interactivenlp-0.0.3/interactivenlp/typedef/interactive.py
+-rw-rw-rw-   0        0        0      159 2023-05-18 01:03:52.000000 interactivenlp-0.0.3/interactivenlp/typedef/rss.py
+drwxrwxrwx   0        0        0        0 2023-05-18 20:33:55.851048 interactivenlp-0.0.3/interactivenlp/web/
+-rw-rw-rw-   0        0        0        0 2023-05-18 20:33:14.000000 interactivenlp-0.0.3/interactivenlp/web/__init__.py
+-rw-rw-rw-   0        0        0      967 2023-05-18 18:18:03.000000 interactivenlp-0.0.3/interactivenlp/web/server.py
+drwxrwxrwx   0        0        0        0 2023-05-18 20:33:55.835214 interactivenlp-0.0.3/interactivenlp.egg-info/
+-rw-rw-rw-   0        0        0      358 2023-05-18 20:33:55.000000 interactivenlp-0.0.3/interactivenlp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      438 2023-05-18 20:33:55.000000 interactivenlp-0.0.3/interactivenlp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 20:33:55.000000 interactivenlp-0.0.3/interactivenlp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-18 20:33:55.000000 interactivenlp-0.0.3/interactivenlp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-18 20:33:55.000000 interactivenlp-0.0.3/interactivenlp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 20:33:55.854048 interactivenlp-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      616 2023-05-18 20:33:51.000000 interactivenlp-0.0.3/setup.py
```

### Comparing `interactivenlp-0.0.2/LICENSE` & `interactivenlp-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `interactivenlp-0.0.2/setup.py` & `interactivenlp-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages
 
 with open('README.rst', "r") as f:
     long_description = f.read()
 
 setup(
     name='interactivenlp',
-    version='0.0.2',
+    version='0.0.3',
     description='Interactive NLP',
     long_description=long_description,
     author="Chunxu Yang",
     author_email="chunxuyang@ucla.edu",
     install_requires=[
         'flask',
         'flask-cors',
```

