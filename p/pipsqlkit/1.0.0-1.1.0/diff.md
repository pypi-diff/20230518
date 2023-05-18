# Comparing `tmp/pipsqlkit-1.0.0.tar.gz` & `tmp/pipsqlkit-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipsqlkit-1.0.0.tar", last modified: Thu May 18 20:37:49 2023, max compression
+gzip compressed data, was "pipsqlkit-1.1.0.tar", last modified: Thu May 18 20:39:54 2023, max compression
```

## Comparing `pipsqlkit-1.0.0.tar` & `pipsqlkit-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:37:49.352922 pipsqlkit-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      342 2023-05-18 20:37:49.352922 pipsqlkit-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:37:49.348922 pipsqlkit-1.0.0/pipsqlkit/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-18 20:37:49.000000 pipsqlkit-1.0.0/pipsqlkit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:37:49.348922 pipsqlkit-1.0.0/pipsqlkit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      342 2023-05-18 20:37:49.000000 pipsqlkit-1.0.0/pipsqlkit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      162 2023-05-18 20:37:49.000000 pipsqlkit-1.0.0/pipsqlkit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 20:37:49.000000 pipsqlkit-1.0.0/pipsqlkit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-18 20:37:49.000000 pipsqlkit-1.0.0/pipsqlkit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-18 20:37:49.352922 pipsqlkit-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      555 2023-05-18 20:37:49.000000 pipsqlkit-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:39:54.363489 pipsqlkit-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      342 2023-05-18 20:39:54.363489 pipsqlkit-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:39:54.363489 pipsqlkit-1.1.0/pipsqlkit/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-05-18 20:39:54.000000 pipsqlkit-1.1.0/pipsqlkit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:39:54.363489 pipsqlkit-1.1.0/pipsqlkit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      342 2023-05-18 20:39:54.000000 pipsqlkit-1.1.0/pipsqlkit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      162 2023-05-18 20:39:54.000000 pipsqlkit-1.1.0/pipsqlkit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 20:39:54.000000 pipsqlkit-1.1.0/pipsqlkit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-18 20:39:54.000000 pipsqlkit-1.1.0/pipsqlkit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-18 20:39:54.363489 pipsqlkit-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      555 2023-05-18 20:39:54.000000 pipsqlkit-1.1.0/setup.py
```

### Comparing `pipsqlkit-1.0.0/setup.py` & `pipsqlkit-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pipsqlkit",
     version=VERSION,
```

