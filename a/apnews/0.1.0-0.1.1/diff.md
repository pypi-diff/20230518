# Comparing `tmp/apnews-0.1.0.tar.gz` & `tmp/apnews-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apnews-0.1.0.tar", last modified: Thu May 18 06:40:03 2023, max compression
+gzip compressed data, was "apnews-0.1.1.tar", last modified: Thu May 18 07:03:34 2023, max compression
```

## Comparing `apnews-0.1.0.tar` & `apnews-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 spence    (1000) spence    (1000)        0 2023-05-18 06:40:03.019994 apnews-0.1.0/
--rw-r--r--   0 spence    (1000) spence    (1000)     1074 2023-05-16 08:48:48.000000 apnews-0.1.0/LICENSE
--rw-r--r--   0 spence    (1000) spence    (1000)      610 2023-05-18 06:40:03.019994 apnews-0.1.0/PKG-INFO
--rw-r--r--   0 spence    (1000) spence    (1000)      106 2023-05-16 08:48:48.000000 apnews-0.1.0/README.md
-drwxr-xr-x   0 spence    (1000) spence    (1000)        0 2023-05-18 06:40:03.018994 apnews-0.1.0/apnews/
--rw-r--r--   0 spence    (1000) spence    (1000)       21 2023-05-18 06:24:55.000000 apnews-0.1.0/apnews/__init__.py
--rw-r--r--   0 spence    (1000) spence    (1000)     1892 2023-05-18 06:30:25.000000 apnews-0.1.0/apnews/client.py
-drwxr-xr-x   0 spence    (1000) spence    (1000)        0 2023-05-18 06:40:03.019994 apnews-0.1.0/apnews.egg-info/
--rw-r--r--   0 spence    (1000) spence    (1000)      610 2023-05-18 06:40:03.000000 apnews-0.1.0/apnews.egg-info/PKG-INFO
--rw-r--r--   0 spence    (1000) spence    (1000)      211 2023-05-18 06:40:03.000000 apnews-0.1.0/apnews.egg-info/SOURCES.txt
--rw-r--r--   0 spence    (1000) spence    (1000)        1 2023-05-18 06:40:03.000000 apnews-0.1.0/apnews.egg-info/dependency_links.txt
--rw-r--r--   0 spence    (1000) spence    (1000)       24 2023-05-18 06:40:03.000000 apnews-0.1.0/apnews.egg-info/requires.txt
--rw-r--r--   0 spence    (1000) spence    (1000)        7 2023-05-18 06:40:03.000000 apnews-0.1.0/apnews.egg-info/top_level.txt
--rw-r--r--   0 spence    (1000) spence    (1000)       38 2023-05-18 06:40:03.019994 apnews-0.1.0/setup.cfg
--rw-r--r--   0 spence    (1000) spence    (1000)      732 2023-05-18 06:39:47.000000 apnews-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:03:34.496792 apnews-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-18 07:03:20.000000 apnews-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-18 07:03:34.496792 apnews-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-18 07:03:20.000000 apnews-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:03:34.496792 apnews-0.1.1/apnews/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-18 07:03:20.000000 apnews-0.1.1/apnews/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-18 07:03:20.000000 apnews-0.1.1/apnews/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:03:34.496792 apnews-0.1.1/apnews.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-18 07:03:34.000000 apnews-0.1.1/apnews.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-18 07:03:34.000000 apnews-0.1.1/apnews.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 07:03:34.000000 apnews-0.1.1/apnews.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-18 07:03:34.000000 apnews-0.1.1/apnews.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-18 07:03:34.000000 apnews-0.1.1/apnews.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 07:03:34.496792 apnews-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-18 07:03:20.000000 apnews-0.1.1/setup.py
```

### Comparing `apnews-0.1.0/LICENSE` & `apnews-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `apnews-0.1.0/apnews/client.py` & `apnews-0.1.1/apnews/client.py`

 * *Files identical despite different names*

### Comparing `apnews-0.1.0/setup.py` & `apnews-0.1.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 from setuptools import setup, find_packages
+from os import path
+
+this_directory = path.abspath(path.dirname(__file__))
+with open(path.join(this_directory, 'README.md')) as f:
+    long_description = f.read()
 
 setup(
     name="apnews",
-    version="0.1.0",
+    version="0.1.1",
     description="A simple web scraper for Associated Press",
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     author="Spencer Churchill",
     author_email="spence@duck.com",
     url="https://github.com/splch/py-apnews",
     packages=find_packages(),
     install_requires=[
         "requests",
         "beautifulsoup4"
```

