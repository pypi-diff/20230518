# Comparing `tmp/TimePrintOnPYPI-0.1.0.tar.gz` & `tmp/TimePrintOnPYPI-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TimePrintOnPYPI-0.1.0.tar", last modified: Sat May 13 09:46:54 2023, max compression
+gzip compressed data, was "TimePrintOnPYPI-1.1.0.tar", last modified: Thu May 18 18:18:48 2023, max compression
```

## Comparing `TimePrintOnPYPI-0.1.0.tar` & `TimePrintOnPYPI-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 09:46:54.134368 TimePrintOnPYPI-0.1.0/
--rw-rw-rw-   0        0        0      445 2023-05-13 09:46:54.133374 TimePrintOnPYPI-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-13 09:46:54.117776 TimePrintOnPYPI-0.1.0/TimePrint/
--rw-rw-rw-   0        0        0      347 2023-05-13 09:39:08.000000 TimePrintOnPYPI-0.1.0/TimePrint/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-13 09:46:54.132369 TimePrintOnPYPI-0.1.0/TimePrintOnPYPI.egg-info/
--rw-rw-rw-   0        0        0      445 2023-05-13 09:46:54.000000 TimePrintOnPYPI-0.1.0/TimePrintOnPYPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2023-05-13 09:46:54.000000 TimePrintOnPYPI-0.1.0/TimePrintOnPYPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 09:46:54.000000 TimePrintOnPYPI-0.1.0/TimePrintOnPYPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-13 09:46:54.000000 TimePrintOnPYPI-0.1.0/TimePrintOnPYPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-13 09:46:54.134368 TimePrintOnPYPI-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      557 2023-05-13 09:45:35.000000 TimePrintOnPYPI-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:18:48.475342 TimePrintOnPYPI-1.1.0/
+-rw-rw-rw-   0        0        0      445 2023-05-18 18:18:48.474341 TimePrintOnPYPI-1.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-18 18:18:48.453697 TimePrintOnPYPI-1.1.0/TimePrint/
+-rw-rw-rw-   0        0        0     1064 2023-05-18 18:16:21.000000 TimePrintOnPYPI-1.1.0/TimePrint/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:18:48.472337 TimePrintOnPYPI-1.1.0/TimePrintOnPYPI.egg-info/
+-rw-rw-rw-   0        0        0      445 2023-05-18 18:18:48.000000 TimePrintOnPYPI-1.1.0/TimePrintOnPYPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2023-05-18 18:18:48.000000 TimePrintOnPYPI-1.1.0/TimePrintOnPYPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 18:18:48.000000 TimePrintOnPYPI-1.1.0/TimePrintOnPYPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-18 18:18:48.000000 TimePrintOnPYPI-1.1.0/TimePrintOnPYPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 18:18:48.475342 TimePrintOnPYPI-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      557 2023-05-18 18:16:57.000000 TimePrintOnPYPI-1.1.0/setup.py
```

### Comparing `TimePrintOnPYPI-0.1.0/setup.py` & `TimePrintOnPYPI-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='TimePrintOnPYPI',
-    version='0.1.0',
+    version='1.1.0',
     description='A package for printing text with time delay between characters',
     url='https://github.com/SForces/TimePrint',
     author='Osman TUNA',
     author_email='osmntn08@gmail.com',
     license='MIT',
     packages=['TimePrint'],
     classifiers=[
```

