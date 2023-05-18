# Comparing `tmp/adv-ml-0.0.1.tar.gz` & `tmp/adv-ml-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adv-ml-0.0.1.tar", last modified: Thu May 18 08:49:33 2023, max compression
+gzip compressed data, was "adv-ml-0.0.2.tar", last modified: Thu May 18 14:34:08 2023, max compression
```

## Comparing `adv-ml-0.0.1.tar` & `adv-ml-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-05-18 08:49:33.067818 adv-ml-0.0.1/
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    35149 2023-05-17 06:04:26.000000 adv-ml-0.0.1/LICENSE
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      111 2023-04-27 10:12:58.000000 adv-ml-0.0.1/MANIFEST.in
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1207 2023-05-18 08:49:33.067818 adv-ml-0.0.1/PKG-INFO
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      195 2023-05-17 06:15:54.000000 adv-ml-0.0.1/README.md
-drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-05-18 08:49:33.067818 adv-ml-0.0.1/adv_ml/
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       22 2023-05-18 08:44:41.000000 adv-ml-0.0.1/adv_ml/__init__.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     2414 2023-05-18 08:44:41.000000 adv-ml-0.0.1/adv_ml/_modidx.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      128 2023-05-17 23:02:52.000000 adv-ml-0.0.1/adv_ml/all.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     5025 2023-05-18 08:44:41.000000 adv-ml-0.0.1/adv_ml/evasion.py
-drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-05-18 08:49:33.067818 adv-ml-0.0.1/adv_ml.egg-info/
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1207 2023-05-18 08:49:32.000000 adv-ml-0.0.1/adv_ml.egg-info/PKG-INFO
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      331 2023-05-18 08:49:32.000000 adv-ml-0.0.1/adv_ml.egg-info/SOURCES.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-05-18 08:49:32.000000 adv-ml-0.0.1/adv_ml.egg-info/dependency_links.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       55 2023-05-18 08:49:32.000000 adv-ml-0.0.1/adv_ml.egg-info/entry_points.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-05-18 08:49:32.000000 adv-ml-0.0.1/adv_ml.egg-info/not-zip-safe
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       50 2023-05-18 08:49:32.000000 adv-ml-0.0.1/adv_ml.egg-info/requires.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        7 2023-05-18 08:49:32.000000 adv-ml-0.0.1/adv_ml.egg-info/top_level.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1081 2023-05-18 08:44:31.000000 adv-ml-0.0.1/settings.ini
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       38 2023-05-18 08:49:33.067818 adv-ml-0.0.1/setup.cfg
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     2596 2023-04-27 10:12:58.000000 adv-ml-0.0.1/setup.py
+drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-05-18 14:34:08.191524 adv-ml-0.0.2/
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    35149 2023-05-17 06:04:26.000000 adv-ml-0.0.2/LICENSE
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      111 2023-04-27 10:12:58.000000 adv-ml-0.0.2/MANIFEST.in
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     4291 2023-05-18 14:34:08.191524 adv-ml-0.0.2/PKG-INFO
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     2327 2023-05-18 14:32:34.000000 adv-ml-0.0.2/README.md
+drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-05-18 14:34:08.187524 adv-ml-0.0.2/adv_ml/
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       22 2023-05-18 14:34:03.000000 adv-ml-0.0.2/adv_ml/__init__.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     6601 2023-05-18 14:34:03.000000 adv-ml-0.0.2/adv_ml/_modidx.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      162 2023-05-18 13:43:34.000000 adv-ml-0.0.2/adv_ml/all.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     2902 2023-05-18 14:34:03.000000 adv-ml-0.0.2/adv_ml/evasion.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     3396 2023-05-18 14:34:03.000000 adv-ml-0.0.2/adv_ml/input_optimization.py
+drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-05-18 14:34:08.191524 adv-ml-0.0.2/adv_ml.egg-info/
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     4291 2023-05-18 14:34:07.000000 adv-ml-0.0.2/adv_ml.egg-info/PKG-INFO
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      360 2023-05-18 14:34:08.000000 adv-ml-0.0.2/adv_ml.egg-info/SOURCES.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-05-18 14:34:07.000000 adv-ml-0.0.2/adv_ml.egg-info/dependency_links.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       55 2023-05-18 14:34:07.000000 adv-ml-0.0.2/adv_ml.egg-info/entry_points.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-05-18 08:49:32.000000 adv-ml-0.0.2/adv_ml.egg-info/not-zip-safe
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       50 2023-05-18 14:34:07.000000 adv-ml-0.0.2/adv_ml.egg-info/requires.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        7 2023-05-18 14:34:07.000000 adv-ml-0.0.2/adv_ml.egg-info/top_level.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1081 2023-05-18 14:33:18.000000 adv-ml-0.0.2/settings.ini
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       38 2023-05-18 14:34:08.191524 adv-ml-0.0.2/setup.cfg
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     2596 2023-04-27 10:12:58.000000 adv-ml-0.0.2/setup.py
```

### Comparing `adv-ml-0.0.1/LICENSE` & `adv-ml-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adv-ml-0.0.1/settings.ini` & `adv-ml-0.0.2/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = adv-ml
 lib_name = %(repo)s
-version = 0.0.1
+version = 0.0.2
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = adv_ml
```

### Comparing `adv-ml-0.0.1/setup.py` & `adv-ml-0.0.2/setup.py`

 * *Files identical despite different names*

