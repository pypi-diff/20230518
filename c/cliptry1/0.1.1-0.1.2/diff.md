# Comparing `tmp/cliptry1-0.1.1.tar.gz` & `tmp/cliptry1-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliptry1-0.1.1.tar", last modified: Thu May 18 06:26:37 2023, max compression
+gzip compressed data, was "cliptry1-0.1.2.tar", last modified: Thu May 18 06:52:10 2023, max compression
```

## Comparing `cliptry1-0.1.1.tar` & `cliptry1-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 06:26:37.442394 cliptry1-0.1.1/
--rw-rw-rw-   0        0        0       25 2020-04-19 14:59:35.000000 cliptry1-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      236 2023-05-18 06:26:37.440393 cliptry1-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      106 2020-04-19 14:58:18.000000 cliptry1-0.1.1/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-18 06:26:37.422394 cliptry1-0.1.1/cliptry1.egg-info/
--rw-rw-rw-   0        0        0      236 2023-05-18 06:26:37.000000 cliptry1-0.1.1/cliptry1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2023-05-18 06:26:37.000000 cliptry1-0.1.1/cliptry1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      124 2023-05-18 06:26:37.000000 cliptry1-0.1.1/cliptry1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-05-18 06:26:37.000000 cliptry1-0.1.1/cliptry1.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-18 06:26:37.000000 cliptry1-0.1.1/cliptry1.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-18 06:26:37.434394 cliptry1-0.1.1/jaical/
--rw-rw-rw-   0        0        0      630 2023-05-18 06:25:36.000000 cliptry1-0.1.1/jaical/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-18 06:26:37.443994 cliptry1-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-05-18 06:26:29.000000 cliptry1-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 06:52:10.180276 cliptry1-0.1.2/
+-rw-rw-rw-   0        0        0       25 2020-04-19 14:59:35.000000 cliptry1-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      236 2023-05-18 06:52:10.178251 cliptry1-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      106 2020-04-19 14:58:18.000000 cliptry1-0.1.2/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 06:52:10.161308 cliptry1-0.1.2/cliptry1.egg-info/
+-rw-rw-rw-   0        0        0      236 2023-05-18 06:52:09.000000 cliptry1-0.1.2/cliptry1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2023-05-18 06:52:09.000000 cliptry1-0.1.2/cliptry1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      124 2023-05-18 06:52:09.000000 cliptry1-0.1.2/cliptry1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-05-18 06:52:09.000000 cliptry1-0.1.2/cliptry1.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-18 06:52:09.000000 cliptry1-0.1.2/cliptry1.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 06:52:10.172406 cliptry1-0.1.2/jaical/
+-rw-rw-rw-   0        0        0      630 2023-05-18 06:25:36.000000 cliptry1-0.1.2/jaical/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-18 06:52:10.182476 cliptry1-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      526 2023-05-18 06:51:55.000000 cliptry1-0.1.2/setup.py
```

### Comparing `cliptry1-0.1.1/jaical/__init__.py` & `cliptry1-0.1.2/jaical/__init__.py`

 * *Files identical despite different names*

