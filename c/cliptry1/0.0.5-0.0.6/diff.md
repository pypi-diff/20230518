# Comparing `tmp/cliptry1-0.0.5.tar.gz` & `tmp/cliptry1-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliptry1-0.0.5.tar", last modified: Wed May 17 13:09:43 2023, max compression
+gzip compressed data, was "cliptry1-0.0.6.tar", last modified: Thu May 18 05:55:46 2023, max compression
```

## Comparing `cliptry1-0.0.5.tar` & `cliptry1-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 13:09:43.360218 cliptry1-0.0.5/
--rw-rw-rw-   0        0        0       25 2020-04-19 14:59:35.000000 cliptry1-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      236 2023-05-17 13:09:43.356219 cliptry1-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      106 2020-04-19 14:58:18.000000 cliptry1-0.0.5/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-17 13:09:43.334289 cliptry1-0.0.5/cliptry1.egg-info/
--rw-rw-rw-   0        0        0      236 2023-05-17 13:09:42.000000 cliptry1-0.0.5/cliptry1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2023-05-17 13:09:43.000000 cliptry1-0.0.5/cliptry1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      124 2023-05-17 13:09:42.000000 cliptry1-0.0.5/cliptry1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-05-17 13:09:42.000000 cliptry1-0.0.5/cliptry1.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-17 13:09:42.000000 cliptry1-0.0.5/cliptry1.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-17 13:09:43.349218 cliptry1-0.0.5/jaical/
--rw-rw-rw-   0        0        0      466 2023-05-17 13:02:57.000000 cliptry1-0.0.5/jaical/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-17 13:09:43.363220 cliptry1-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      512 2023-05-17 13:09:27.000000 cliptry1-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 05:55:46.191794 cliptry1-0.0.6/
+-rw-rw-rw-   0        0        0       25 2020-04-19 14:59:35.000000 cliptry1-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      236 2023-05-18 05:55:46.188793 cliptry1-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      106 2020-04-19 14:58:18.000000 cliptry1-0.0.6/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 05:55:46.167654 cliptry1-0.0.6/cliptry1.egg-info/
+-rw-rw-rw-   0        0        0      236 2023-05-18 05:55:45.000000 cliptry1-0.0.6/cliptry1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2023-05-18 05:55:45.000000 cliptry1-0.0.6/cliptry1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      124 2023-05-18 05:55:45.000000 cliptry1-0.0.6/cliptry1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-05-18 05:55:45.000000 cliptry1-0.0.6/cliptry1.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-18 05:55:45.000000 cliptry1-0.0.6/cliptry1.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 05:55:46.181283 cliptry1-0.0.6/jaical/
+-rw-rw-rw-   0        0        0      435 2023-05-18 05:54:50.000000 cliptry1-0.0.6/jaical/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-18 05:55:46.194793 cliptry1-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      512 2023-05-18 05:55:33.000000 cliptry1-0.0.6/setup.py
```

### Comparing `cliptry1-0.0.5/setup.py` & `cliptry1-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup (
   name='cliptry1',
-  version='0.0.5',
+  version='0.0.6',
   description='A very basic calculator',
   url='',  
   author='jaideep ',
   author_email='jaideepkaushal2@gmail.com',
   license='MIT', 
   keywords='calculator', 
   packages=find_packages(),
```

