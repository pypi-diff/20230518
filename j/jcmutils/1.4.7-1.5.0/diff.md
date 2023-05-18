# Comparing `tmp/jcmutils-1.4.7.tar.gz` & `tmp/jcmutils-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcmutils-1.4.7.tar", last modified: Wed May 17 02:00:24 2023, max compression
+gzip compressed data, was "jcmutils-1.5.0.tar", last modified: Thu May 18 06:54:32 2023, max compression
```

## Comparing `jcmutils-1.4.7.tar` & `jcmutils-1.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-17 02:00:24.714825 jcmutils-1.4.7/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.4.7/LICENSE
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-17 02:00:24.714825 jcmutils-1.4.7/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-04-15 12:55:54.000000 jcmutils-1.4.7/README.md
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-17 02:00:24.714825 jcmutils-1.4.7/jcmutils/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      165 2023-04-18 07:48:21.000000 jcmutils-1.4.7/jcmutils/__init__.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     6886 2023-05-17 02:00:03.000000 jcmutils-1.4.7/jcmutils/dataset_utils.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.4.7/jcmutils/gen_sources.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-04-15 12:55:54.000000 jcmutils-1.4.7/jcmutils/logger.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     8780 2023-05-11 10:05:05.000000 jcmutils-1.4.7/jcmutils/solver.py
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-17 02:00:24.714825 jcmutils-1.4.7/jcmutils.egg-info/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-17 02:00:24.000000 jcmutils-1.4.7/jcmutils.egg-info/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      294 2023-05-17 02:00:24.000000 jcmutils-1.4.7/jcmutils.egg-info/SOURCES.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-05-17 02:00:24.000000 jcmutils-1.4.7/jcmutils.egg-info/dependency_links.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-05-17 02:00:24.000000 jcmutils-1.4.7/jcmutils.egg-info/requires.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-05-17 02:00:24.000000 jcmutils-1.4.7/jcmutils.egg-info/top_level.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-05-17 02:00:24.714825 jcmutils-1.4.7/setup.cfg
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      539 2023-05-17 02:00:15.000000 jcmutils-1.4.7/setup.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-18 06:54:32.358915 jcmutils-1.5.0/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.5.0/LICENSE
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-18 06:54:32.358915 jcmutils-1.5.0/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-05-17 04:08:25.000000 jcmutils-1.5.0/README.md
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-18 06:54:32.354915 jcmutils-1.5.0/jcmutils/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      165 2023-05-17 04:08:25.000000 jcmutils-1.5.0/jcmutils/__init__.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)    11232 2023-05-18 06:54:08.000000 jcmutils-1.5.0/jcmutils/dataset_utils.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.5.0/jcmutils/gen_sources.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-05-17 04:08:25.000000 jcmutils-1.5.0/jcmutils/logger.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     8780 2023-05-17 04:08:25.000000 jcmutils-1.5.0/jcmutils/solver.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-18 06:54:32.358915 jcmutils-1.5.0/jcmutils.egg-info/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-18 06:54:32.000000 jcmutils-1.5.0/jcmutils.egg-info/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      294 2023-05-18 06:54:32.000000 jcmutils-1.5.0/jcmutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-05-18 06:54:32.000000 jcmutils-1.5.0/jcmutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-05-18 06:54:32.000000 jcmutils-1.5.0/jcmutils.egg-info/requires.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-05-18 06:54:32.000000 jcmutils-1.5.0/jcmutils.egg-info/top_level.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-05-18 06:54:32.358915 jcmutils-1.5.0/setup.cfg
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      539 2023-05-18 06:54:23.000000 jcmutils-1.5.0/setup.py
```

### Comparing `jcmutils-1.4.7/LICENSE` & `jcmutils-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jcmutils-1.4.7/README.md` & `jcmutils-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `jcmutils-1.4.7/jcmutils/gen_sources.py` & `jcmutils-1.5.0/jcmutils/gen_sources.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.4.7/jcmutils/logger.py` & `jcmutils-1.5.0/jcmutils/logger.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.4.7/jcmutils/solver.py` & `jcmutils-1.5.0/jcmutils/solver.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.4.7/setup.py` & `jcmutils-1.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 
-VERSION = '1.4.7'
+VERSION = '1.5.0'
 DESCRIPTION = "A general utils for jcmsuite"
 
 setup(
     name="jcmutils",
     version=VERSION,
     author="crafter-z",
     author_email="crafterz@163.com",
```

