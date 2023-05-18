# Comparing `tmp/PySpeaker-2.0.tar.gz` & `tmp/pyspeaker-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySpeaker-2.0.tar", last modified: Thu May 18 15:31:32 2023, max compression
+gzip compressed data, was "pyspeaker-3.0.tar", last modified: Thu May 18 16:15:39 2023, max compression
```

## Comparing `PySpeaker-2.0.tar` & `pyspeaker-3.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 15:31:32.975412 PySpeaker-2.0/
--rw-rw-rw-   0        0        0     1091 2023-02-23 09:47:52.000000 PySpeaker-2.0/LICENSE.txt
--rw-rw-rw-   0        0        0      212 2023-05-18 15:31:32.973412 PySpeaker-2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-18 15:31:32.965886 PySpeaker-2.0/PySpeaker.egg-info/
--rw-rw-rw-   0        0        0      212 2023-05-18 15:31:32.000000 PySpeaker-2.0/PySpeaker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2023-05-18 15:31:32.000000 PySpeaker-2.0/PySpeaker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 15:31:32.000000 PySpeaker-2.0/PySpeaker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-05-18 15:31:32.000000 PySpeaker-2.0/PySpeaker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-18 15:31:32.000000 PySpeaker-2.0/PySpeaker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      329 2023-05-18 11:26:55.000000 PySpeaker-2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 15:31:32.970059 PySpeaker-2.0/pyspeaker/
--rw-rw-rw-   0        0        0      776 2023-05-18 11:45:12.000000 PySpeaker-2.0/pyspeaker/Audio.py
--rw-rw-rw-   0        0        0       42 2023-05-18 15:31:32.975412 PySpeaker-2.0/setup.cfg
--rw-rw-rw-   0        0        0      641 2023-05-18 15:31:26.000000 PySpeaker-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 16:15:39.417851 pyspeaker-3.0/
+-rw-rw-rw-   0        0        0     1091 2023-02-23 09:47:52.000000 pyspeaker-3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      212 2023-05-18 16:15:39.415856 pyspeaker-3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2023-05-18 11:26:55.000000 pyspeaker-3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 16:15:39.387943 pyspeaker-3.0/app/
+drwxrwxrwx   0        0        0        0 2023-05-18 16:15:39.398847 pyspeaker-3.0/app/pyspeaker/
+-rw-rw-rw-   0        0        0      776 2023-05-18 11:45:12.000000 pyspeaker-3.0/app/pyspeaker/Audio.py
+drwxrwxrwx   0        0        0        0 2023-05-18 16:15:39.412851 pyspeaker-3.0/app/pyspeaker.egg-info/
+-rw-rw-rw-   0        0        0      212 2023-05-18 16:15:39.000000 pyspeaker-3.0/app/pyspeaker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-05-18 16:15:39.000000 pyspeaker-3.0/app/pyspeaker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 16:15:39.000000 pyspeaker-3.0/app/pyspeaker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-05-18 16:15:39.000000 pyspeaker-3.0/app/pyspeaker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-18 16:15:39.000000 pyspeaker-3.0/app/pyspeaker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 16:15:39.417851 pyspeaker-3.0/setup.cfg
+-rw-rw-rw-   0        0        0      660 2023-05-18 16:14:53.000000 pyspeaker-3.0/setup.py
```

### Comparing `PySpeaker-2.0/LICENSE.txt` & `pyspeaker-3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PySpeaker-2.0/pyspeaker/Audio.py` & `pyspeaker-3.0/app/pyspeaker/Audio.py`

 * *Files identical despite different names*

