# Comparing `tmp/cliptry1-0.0.6.tar.gz` & `tmp/cliptry1-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliptry1-0.0.6.tar", last modified: Thu May 18 05:55:46 2023, max compression
+gzip compressed data, was "cliptry1-0.1.0.tar", last modified: Thu May 18 06:07:28 2023, max compression
```

## Comparing `cliptry1-0.0.6.tar` & `cliptry1-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 05:55:46.191794 cliptry1-0.0.6/
--rw-rw-rw-   0        0        0       25 2020-04-19 14:59:35.000000 cliptry1-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      236 2023-05-18 05:55:46.188793 cliptry1-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      106 2020-04-19 14:58:18.000000 cliptry1-0.0.6/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-18 05:55:46.167654 cliptry1-0.0.6/cliptry1.egg-info/
--rw-rw-rw-   0        0        0      236 2023-05-18 05:55:45.000000 cliptry1-0.0.6/cliptry1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2023-05-18 05:55:45.000000 cliptry1-0.0.6/cliptry1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      124 2023-05-18 05:55:45.000000 cliptry1-0.0.6/cliptry1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-05-18 05:55:45.000000 cliptry1-0.0.6/cliptry1.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-18 05:55:45.000000 cliptry1-0.0.6/cliptry1.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-18 05:55:46.181283 cliptry1-0.0.6/jaical/
--rw-rw-rw-   0        0        0      435 2023-05-18 05:54:50.000000 cliptry1-0.0.6/jaical/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-18 05:55:46.194793 cliptry1-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      512 2023-05-18 05:55:33.000000 cliptry1-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 06:07:28.796636 cliptry1-0.1.0/
+-rw-rw-rw-   0        0        0       25 2020-04-19 14:59:35.000000 cliptry1-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      236 2023-05-18 06:07:28.794635 cliptry1-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      106 2020-04-19 14:58:18.000000 cliptry1-0.1.0/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 06:07:28.774635 cliptry1-0.1.0/cliptry1.egg-info/
+-rw-rw-rw-   0        0        0      236 2023-05-18 06:07:28.000000 cliptry1-0.1.0/cliptry1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2023-05-18 06:07:28.000000 cliptry1-0.1.0/cliptry1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      124 2023-05-18 06:07:28.000000 cliptry1-0.1.0/cliptry1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-05-18 06:07:28.000000 cliptry1-0.1.0/cliptry1.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-18 06:07:28.000000 cliptry1-0.1.0/cliptry1.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 06:07:28.788635 cliptry1-0.1.0/jaical/
+-rw-rw-rw-   0        0        0      624 2023-05-18 06:06:05.000000 cliptry1-0.1.0/jaical/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-18 06:07:28.798635 cliptry1-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      512 2023-05-18 06:06:58.000000 cliptry1-0.1.0/setup.py
```

### Comparing `cliptry1-0.0.6/setup.py` & `cliptry1-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup (
   name='cliptry1',
-  version='0.0.6',
+  version='0.1.0',
   description='A very basic calculator',
   url='',  
   author='jaideep ',
   author_email='jaideepkaushal2@gmail.com',
   license='MIT', 
   keywords='calculator', 
   packages=find_packages(),
```

