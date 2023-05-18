# Comparing `tmp/syngenta_digital_adapt-0.0.0.tar.gz` & `tmp/syngenta_digital_adapt-0.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syngenta_digital_adapt-0.0.0.tar", last modified: Wed May 17 19:18:36 2023, max compression
+gzip compressed data, was "dist/syngenta_digital_adapt-0.0.0b1.tar", last modified: Thu May 18 14:48:29 2023, max compression
```

## Comparing `syngenta_digital_adapt-0.0.0.tar` & `syngenta_digital_adapt-0.0.0b1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 dbankhead   (501) staff       (20)        0 2023-05-17 19:18:36.131545 syngenta_digital_adapt-0.0.0/
--rw-r--r--   0 dbankhead   (501) staff       (20)     1065 2023-05-17 18:56:35.000000 syngenta_digital_adapt-0.0.0/LICENSE
--rw-r--r--   0 dbankhead   (501) staff       (20)      859 2023-05-17 19:18:36.131410 syngenta_digital_adapt-0.0.0/PKG-INFO
--rw-r--r--   0 dbankhead   (501) staff       (20)       58 2023-05-17 18:56:35.000000 syngenta_digital_adapt-0.0.0/README.md
--rw-r--r--   0 dbankhead   (501) staff       (20)       38 2023-05-17 19:18:36.131580 syngenta_digital_adapt-0.0.0/setup.cfg
--rw-r--r--   0 dbankhead   (501) staff       (20)     1229 2023-05-17 19:13:05.000000 syngenta_digital_adapt-0.0.0/setup.py
-drwxr-xr-x   0 dbankhead   (501) staff       (20)        0 2023-05-17 19:18:36.131252 syngenta_digital_adapt-0.0.0/syngenta_digital_adapt.egg-info/
--rw-r--r--   0 dbankhead   (501) staff       (20)      859 2023-05-17 19:18:36.000000 syngenta_digital_adapt-0.0.0/syngenta_digital_adapt.egg-info/PKG-INFO
--rw-r--r--   0 dbankhead   (501) staff       (20)      255 2023-05-17 19:18:36.000000 syngenta_digital_adapt-0.0.0/syngenta_digital_adapt.egg-info/SOURCES.txt
--rw-r--r--   0 dbankhead   (501) staff       (20)        1 2023-05-17 19:18:36.000000 syngenta_digital_adapt-0.0.0/syngenta_digital_adapt.egg-info/dependency_links.txt
--rw-r--r--   0 dbankhead   (501) staff       (20)       83 2023-05-17 19:18:36.000000 syngenta_digital_adapt-0.0.0/syngenta_digital_adapt.egg-info/requires.txt
--rw-r--r--   0 dbankhead   (501) staff       (20)        1 2023-05-17 19:18:36.000000 syngenta_digital_adapt-0.0.0/syngenta_digital_adapt.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-18 14:48:29.866221 syngenta_digital_adapt-0.0.0b1/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1065 2023-05-18 14:48:24.000000 syngenta_digital_adapt-0.0.0b1/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      861 2023-05-18 14:48:29.866221 syngenta_digital_adapt-0.0.0b1/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       58 2023-05-18 14:48:24.000000 syngenta_digital_adapt-0.0.0b1/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-05-18 14:48:29.866221 syngenta_digital_adapt-0.0.0b1/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1229 2023-05-18 14:48:24.000000 syngenta_digital_adapt-0.0.0b1/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-18 14:48:29.866221 syngenta_digital_adapt-0.0.0b1/syngenta_digital_adapt.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      861 2023-05-18 14:48:29.000000 syngenta_digital_adapt-0.0.0b1/syngenta_digital_adapt.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      255 2023-05-18 14:48:29.000000 syngenta_digital_adapt-0.0.0b1/syngenta_digital_adapt.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-05-18 14:48:29.000000 syngenta_digital_adapt-0.0.0b1/syngenta_digital_adapt.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       83 2023-05-18 14:48:29.000000 syngenta_digital_adapt-0.0.0b1/syngenta_digital_adapt.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-05-18 14:48:29.000000 syngenta_digital_adapt-0.0.0b1/syngenta_digital_adapt.egg-info/top_level.txt
```

### Comparing `syngenta_digital_adapt-0.0.0/LICENSE` & `syngenta_digital_adapt-0.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `syngenta_digital_adapt-0.0.0/PKG-INFO` & `syngenta_digital_adapt-0.0.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngenta_digital_adapt
-Version: 0.0.0
+Version: 0.0.0b1
 Summary: Syngenta's ADAPT-based implementation in Python
 Home-page: https://github.com/syngenta-digital/package-python-adapt.git
 Author: Demetrius Bankhead, DevOps Engineer, Syngenta Digital
 Author-email: demetrius.bankhead@syngenta.com
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
```

### Comparing `syngenta_digital_adapt-0.0.0/setup.py` & `syngenta_digital_adapt-0.0.0b1/setup.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_adapt-0.0.0/syngenta_digital_adapt.egg-info/PKG-INFO` & `syngenta_digital_adapt-0.0.0b1/syngenta_digital_adapt.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngenta-digital-adapt
-Version: 0.0.0
+Version: 0.0.0b1
 Summary: Syngenta's ADAPT-based implementation in Python
 Home-page: https://github.com/syngenta-digital/package-python-adapt.git
 Author: Demetrius Bankhead, DevOps Engineer, Syngenta Digital
 Author-email: demetrius.bankhead@syngenta.com
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
```

