# Comparing `tmp/bioumlsim-0.1.6.tar.gz` & `tmp/bioumlsim-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioumlsim-0.1.6.tar", last modified: Wed May 17 17:34:39 2023, max compression
+gzip compressed data, was "bioumlsim-0.2.0.tar", last modified: Wed May 17 19:01:07 2023, max compression
```

## Comparing `bioumlsim-0.1.6.tar` & `bioumlsim-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 17:34:39.038100 bioumlsim-0.1.6/
--rw-rw-rw-   0        0        0     1088 2023-05-17 07:27:39.000000 bioumlsim-0.1.6/LICENSE
--rw-rw-rw-   0        0        0      771 2023-05-17 17:34:39.039068 bioumlsim-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0       60 2023-05-17 07:27:39.000000 bioumlsim-0.1.6/README.md
--rw-rw-rw-   0        0        0      185 2023-05-17 10:21:02.000000 bioumlsim-0.1.6/pyproject.toml
--rw-rw-rw-   0        0        0      790 2023-05-17 17:34:39.040069 bioumlsim-0.1.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-17 17:34:39.018069 bioumlsim-0.1.6/src/
--rw-rw-rw-   0        0        0        0 2023-05-17 07:30:52.000000 bioumlsim-0.1.6/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 17:34:39.037104 bioumlsim-0.1.6/src/bioumlsim.egg-info/
--rw-rw-rw-   0        0        0      771 2023-05-17 17:34:38.000000 bioumlsim-0.1.6/src/bioumlsim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-05-17 17:34:38.000000 bioumlsim-0.1.6/src/bioumlsim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 17:34:38.000000 bioumlsim-0.1.6/src/bioumlsim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-17 10:19:31.000000 bioumlsim-0.1.6/src/bioumlsim.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       14 2023-05-17 17:34:38.000000 bioumlsim-0.1.6/src/bioumlsim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-05-17 17:34:38.000000 bioumlsim-0.1.6/src/bioumlsim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1316 2023-05-17 17:32:55.000000 bioumlsim-0.1.6/src/bioumlsim.py
--rw-rw-rw-   0        0        0      166 2023-05-17 17:19:08.000000 bioumlsim-0.1.6/src/test.py
+drwxrwxrwx   0        0        0        0 2023-05-17 19:01:07.951435 bioumlsim-0.2.0/
+-rw-rw-rw-   0        0        0     1088 2023-05-17 07:27:39.000000 bioumlsim-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      771 2023-05-17 19:01:07.952405 bioumlsim-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2023-05-17 07:27:39.000000 bioumlsim-0.2.0/README.md
+-rw-rw-rw-   0        0        0      185 2023-05-17 10:21:02.000000 bioumlsim-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0      790 2023-05-17 19:01:07.953402 bioumlsim-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-17 19:01:07.929402 bioumlsim-0.2.0/src/
+-rw-rw-rw-   0        0        0        0 2023-05-17 07:30:52.000000 bioumlsim-0.2.0/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 19:01:07.951435 bioumlsim-0.2.0/src/bioumlsim.egg-info/
+-rw-rw-rw-   0        0        0      771 2023-05-17 19:01:07.000000 bioumlsim-0.2.0/src/bioumlsim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-05-17 19:01:07.000000 bioumlsim-0.2.0/src/bioumlsim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 19:01:07.000000 bioumlsim-0.2.0/src/bioumlsim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-17 10:19:31.000000 bioumlsim-0.2.0/src/bioumlsim.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       14 2023-05-17 19:01:07.000000 bioumlsim-0.2.0/src/bioumlsim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-05-17 19:01:07.000000 bioumlsim-0.2.0/src/bioumlsim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2351 2023-05-17 18:45:43.000000 bioumlsim-0.2.0/src/bioumlsim.py
+-rw-rw-rw-   0        0        0      377 2023-05-17 18:41:47.000000 bioumlsim-0.2.0/src/test.py
```

### Comparing `bioumlsim-0.1.6/LICENSE` & `bioumlsim-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.1.6/PKG-INFO` & `bioumlsim-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioumlsim
-Version: 0.1.6
+Version: 0.2.0
 Summary: Python interface for simulation with BioUML
 Home-page: https://www.biouml.org/
 Author: Ilya Kiselev, Biosoft.ru
 Author-email: 4x3cut0r@gmail.com
 Project-URL: Bug Tracker, https://github.com/Biosoft-ru/bioumlsim/issues
 Project-URL: Source Code, https://github.com/Biosoft-ru/bioumlsim
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bioumlsim-0.1.6/setup.cfg` & `bioumlsim-0.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 696f 756d 6c73 696d 0d0a 7665   = bioumlsim..ve
-00000020: 7273 696f 6e20 3d20 302e 312e 360d 0a61  rsion = 0.1.6..a
+00000020: 7273 696f 6e20 3d20 302e 322e 300d 0a61  rsion = 0.2.0..a
 00000030: 7574 686f 7220 3d20 496c 7961 204b 6973  uthor = Ilya Kis
 00000040: 656c 6576 2c20 4269 6f73 6f66 742e 7275  elev, Biosoft.ru
 00000050: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000060: 2034 7833 6375 7430 7240 676d 6169 6c2e   4x3cut0r@gmail.
 00000070: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 00000080: 203d 2050 7974 686f 6e20 696e 7465 7266   = Python interf
 00000090: 6163 6520 666f 7220 7369 6d75 6c61 7469  ace for simulati
```

### Comparing `bioumlsim-0.1.6/src/bioumlsim.egg-info/PKG-INFO` & `bioumlsim-0.2.0/src/bioumlsim.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioumlsim
-Version: 0.1.6
+Version: 0.2.0
 Summary: Python interface for simulation with BioUML
 Home-page: https://www.biouml.org/
 Author: Ilya Kiselev, Biosoft.ru
 Author-email: 4x3cut0r@gmail.com
 Project-URL: Bug Tracker, https://github.com/Biosoft-ru/bioumlsim/issues
 Project-URL: Source Code, https://github.com/Biosoft-ru/bioumlsim
 Classifier: Programming Language :: Python :: 3
```

