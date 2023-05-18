# Comparing `tmp/satyampy-0.1.2.tar.gz` & `tmp/satyampy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satyampy-0.1.2.tar", last modified: Thu May 18 07:51:59 2023, max compression
+gzip compressed data, was "satyampy-0.1.3.tar", last modified: Thu May 18 08:08:18 2023, max compression
```

## Comparing `satyampy-0.1.2.tar` & `satyampy-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 satyam    (1000) satyam    (1000)        0 2023-05-18 07:51:59.281021 satyampy-0.1.2/
--rw-rw-r--   0 satyam    (1000) satyam    (1000)      133 2023-05-18 07:51:59.281021 satyampy-0.1.2/PKG-INFO
-drwxrwxr-x   0 satyam    (1000) satyam    (1000)        0 2023-05-18 07:51:59.281021 satyampy-0.1.2/satyampy/
--rw-rw-r--   0 satyam    (1000) satyam    (1000)       22 2023-05-18 07:50:08.000000 satyampy-0.1.2/satyampy/__init__.py
--rw-rw-r--   0 satyam    (1000) satyam    (1000)      344 2023-05-18 07:19:38.000000 satyampy-0.1.2/satyampy/__main__.py
-drwxrwxr-x   0 satyam    (1000) satyam    (1000)        0 2023-05-18 07:51:59.281021 satyampy-0.1.2/satyampy.egg-info/
--rw-rw-r--   0 satyam    (1000) satyam    (1000)      133 2023-05-18 07:51:59.000000 satyampy-0.1.2/satyampy.egg-info/PKG-INFO
--rw-rw-r--   0 satyam    (1000) satyam    (1000)      269 2023-05-18 07:51:59.000000 satyampy-0.1.2/satyampy.egg-info/SOURCES.txt
--rw-rw-r--   0 satyam    (1000) satyam    (1000)        1 2023-05-18 07:51:59.000000 satyampy-0.1.2/satyampy.egg-info/dependency_links.txt
--rw-rw-r--   0 satyam    (1000) satyam    (1000)       53 2023-05-18 07:51:59.000000 satyampy-0.1.2/satyampy.egg-info/entry_points.txt
--rw-rw-r--   0 satyam    (1000) satyam    (1000)       14 2023-05-18 07:51:59.000000 satyampy-0.1.2/satyampy.egg-info/top_level.txt
--rw-rw-r--   0 satyam    (1000) satyam    (1000)       38 2023-05-18 07:51:59.285021 satyampy-0.1.2/setup.cfg
--rw-rw-r--   0 satyam    (1000) satyam    (1000)      239 2023-05-18 07:50:14.000000 satyampy-0.1.2/setup.py
-drwxrwxr-x   0 satyam    (1000) satyam    (1000)        0 2023-05-18 07:51:59.281021 satyampy-0.1.2/test/
--rw-rw-r--   0 satyam    (1000) satyam    (1000)        0 2023-05-18 07:26:00.000000 satyampy-0.1.2/test/__init__.py
--rw-rw-r--   0 satyam    (1000) satyam    (1000)       68 2023-05-18 07:28:50.000000 satyampy-0.1.2/test/conftest.py
--rw-rw-r--   0 satyam    (1000) satyam    (1000)      421 2023-05-18 07:30:42.000000 satyampy-0.1.2/test/test_satyampy.py
+drwxrwxr-x   0 satyam    (1000) satyam    (1000)        0 2023-05-18 08:08:18.860364 satyampy-0.1.3/
+-rw-rw-r--   0 satyam    (1000) satyam    (1000)      156 2023-05-18 08:08:18.860364 satyampy-0.1.3/PKG-INFO
+drwxrwxr-x   0 satyam    (1000) satyam    (1000)        0 2023-05-18 08:08:18.860364 satyampy-0.1.3/satyampy/
+-rw-rw-r--   0 satyam    (1000) satyam    (1000)       22 2023-05-18 08:08:00.000000 satyampy-0.1.3/satyampy/__init__.py
+-rw-rw-r--   0 satyam    (1000) satyam    (1000)      344 2023-05-18 07:19:38.000000 satyampy-0.1.3/satyampy/__main__.py
+drwxrwxr-x   0 satyam    (1000) satyam    (1000)        0 2023-05-18 08:08:18.860364 satyampy-0.1.3/satyampy.egg-info/
+-rw-rw-r--   0 satyam    (1000) satyam    (1000)      156 2023-05-18 08:08:18.000000 satyampy-0.1.3/satyampy.egg-info/PKG-INFO
+-rw-rw-r--   0 satyam    (1000) satyam    (1000)      269 2023-05-18 08:08:18.000000 satyampy-0.1.3/satyampy.egg-info/SOURCES.txt
+-rw-rw-r--   0 satyam    (1000) satyam    (1000)        1 2023-05-18 08:08:18.000000 satyampy-0.1.3/satyampy.egg-info/dependency_links.txt
+-rw-rw-r--   0 satyam    (1000) satyam    (1000)       53 2023-05-18 08:08:18.000000 satyampy-0.1.3/satyampy.egg-info/entry_points.txt
+-rw-rw-r--   0 satyam    (1000) satyam    (1000)       14 2023-05-18 08:08:18.000000 satyampy-0.1.3/satyampy.egg-info/top_level.txt
+-rw-rw-r--   0 satyam    (1000) satyam    (1000)       38 2023-05-18 08:08:18.860364 satyampy-0.1.3/setup.cfg
+-rw-rw-r--   0 satyam    (1000) satyam    (1000)      293 2023-05-18 08:07:46.000000 satyampy-0.1.3/setup.py
+drwxrwxr-x   0 satyam    (1000) satyam    (1000)        0 2023-05-18 08:08:18.860364 satyampy-0.1.3/test/
+-rw-rw-r--   0 satyam    (1000) satyam    (1000)        0 2023-05-18 07:26:00.000000 satyampy-0.1.3/test/__init__.py
+-rw-rw-r--   0 satyam    (1000) satyam    (1000)       68 2023-05-18 07:28:50.000000 satyampy-0.1.3/test/conftest.py
+-rw-rw-r--   0 satyam    (1000) satyam    (1000)      139 2023-05-18 07:56:33.000000 satyampy-0.1.3/test/test_satyampy.py
```

