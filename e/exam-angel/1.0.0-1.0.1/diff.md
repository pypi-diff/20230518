# Comparing `tmp/exam_angel-1.0.0.tar.gz` & `tmp/exam_angel-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exam_angel-1.0.0.tar", last modified: Thu Apr 20 12:33:27 2023, max compression
+gzip compressed data, was "exam_angel-1.0.1.tar", last modified: Thu May 18 20:44:09 2023, max compression
```

## Comparing `exam_angel-1.0.0.tar` & `exam_angel-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 12:33:27.068221 exam_angel-1.0.0/
--rw-rw-rw-   0        0        0     1048 2021-11-29 01:46:00.000000 exam_angel-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0       37 2021-11-29 01:46:00.000000 exam_angel-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0      247 2023-04-20 12:33:27.067223 exam_angel-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0        4 2023-04-20 12:22:53.000000 exam_angel-1.0.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-20 12:33:27.052265 exam_angel-1.0.0/exam_angel/
--rw-rw-rw-   0        0        0      210 2023-04-20 12:18:47.000000 exam_angel-1.0.0/exam_angel/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 12:33:27.065230 exam_angel-1.0.0/exam_angel.egg-info/
--rw-rw-rw-   0        0        0      247 2023-04-20 12:33:26.000000 exam_angel-1.0.0/exam_angel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-04-20 12:33:26.000000 exam_angel-1.0.0/exam_angel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 12:33:26.000000 exam_angel-1.0.0/exam_angel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-20 12:24:03.000000 exam_angel-1.0.0/exam_angel.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       24 2023-04-20 12:33:26.000000 exam_angel-1.0.0/exam_angel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-20 12:33:26.000000 exam_angel-1.0.0/exam_angel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 12:33:27.068221 exam_angel-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      358 2023-04-20 12:29:37.000000 exam_angel-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 20:44:09.107843 exam_angel-1.0.1/
+-rw-rw-rw-   0        0        0     1048 2021-11-29 01:46:00.000000 exam_angel-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       37 2021-11-29 01:46:00.000000 exam_angel-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      247 2023-05-18 20:44:09.105847 exam_angel-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0        4 2023-04-20 12:22:53.000000 exam_angel-1.0.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-18 20:44:09.050992 exam_angel-1.0.1/exam_angel/
+-rw-rw-rw-   0        0        0    16040 2023-05-18 20:32:12.000000 exam_angel-1.0.1/exam_angel/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 20:44:09.102855 exam_angel-1.0.1/exam_angel.egg-info/
+-rw-rw-rw-   0        0        0      247 2023-05-18 20:44:08.000000 exam_angel-1.0.1/exam_angel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-05-18 20:44:08.000000 exam_angel-1.0.1/exam_angel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 20:44:08.000000 exam_angel-1.0.1/exam_angel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-18 20:44:08.000000 exam_angel-1.0.1/exam_angel.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       24 2023-05-18 20:44:08.000000 exam_angel-1.0.1/exam_angel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-18 20:44:08.000000 exam_angel-1.0.1/exam_angel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 20:44:09.107843 exam_angel-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      358 2023-05-18 20:41:13.000000 exam_angel-1.0.1/setup.py
+-rw-rw-rw-   0        0        0      185 2023-05-18 20:34:38.000000 exam_angel-1.0.1/test.py
```

### Comparing `exam_angel-1.0.0/LICENSE.txt` & `exam_angel-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

