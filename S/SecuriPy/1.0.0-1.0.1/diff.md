# Comparing `tmp/SecuriPy-1.0.0.tar.gz` & `tmp/SecuriPy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SecuriPy-1.0.0.tar", last modified: Thu May 18 11:39:59 2023, max compression
+gzip compressed data, was "SecuriPy-1.0.1.tar", last modified: Thu May 18 13:13:37 2023, max compression
```

## Comparing `SecuriPy-1.0.0.tar` & `SecuriPy-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 11:39:59.719635 SecuriPy-1.0.0/
--rw-rw-rw-   0        0        0     3700 2023-05-18 11:39:59.715745 SecuriPy-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2925 2023-05-18 11:39:07.000000 SecuriPy-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 11:39:59.645355 SecuriPy-1.0.0/SecuriPy.egg-info/
--rw-rw-rw-   0        0        0     3700 2023-05-18 11:39:59.000000 SecuriPy-1.0.0/SecuriPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-05-18 11:39:59.000000 SecuriPy-1.0.0/SecuriPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 11:39:59.000000 SecuriPy-1.0.0/SecuriPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-18 11:39:59.000000 SecuriPy-1.0.0/SecuriPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1531 2023-05-17 17:44:10.000000 SecuriPy-1.0.0/SecuriPy.py
--rw-rw-rw-   0        0        0     1058 2023-05-18 11:38:55.000000 SecuriPy-1.0.0/build.py
--rw-rw-rw-   0        0        0       86 2023-05-18 06:16:12.000000 SecuriPy-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-18 11:39:59.720646 SecuriPy-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1058 2023-05-18 11:39:20.000000 SecuriPy-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 13:13:37.775586 SecuriPy-1.0.1/
+-rw-rw-rw-   0        0        0     3700 2023-05-18 13:13:37.775586 SecuriPy-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2925 2023-05-18 11:39:07.000000 SecuriPy-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 13:13:37.772074 SecuriPy-1.0.1/SecuriPy.egg-info/
+-rw-rw-rw-   0        0        0     3700 2023-05-18 13:13:37.000000 SecuriPy-1.0.1/SecuriPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-05-18 13:13:37.000000 SecuriPy-1.0.1/SecuriPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 13:13:37.000000 SecuriPy-1.0.1/SecuriPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-18 13:13:37.000000 SecuriPy-1.0.1/SecuriPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1531 2023-05-17 17:44:10.000000 SecuriPy-1.0.1/SecuriPy.py
+-rw-rw-rw-   0        0        0     1058 2023-05-18 13:13:10.000000 SecuriPy-1.0.1/build.py
+-rw-rw-rw-   0        0        0       86 2023-05-18 06:16:12.000000 SecuriPy-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-18 13:13:37.775586 SecuriPy-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1058 2023-05-18 13:13:17.000000 SecuriPy-1.0.1/setup.py
```

### Comparing `SecuriPy-1.0.0/PKG-INFO` & `SecuriPy-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SecuriPy
-Version: 1.0.0
+Version: 1.0.1
 Summary: Encrypter and Decrypter of Readable messages Using Python
 Home-page: https://github.com/Anupam1707/SecuriPy
 Author: Anupam Kanoongo
 Author-email: programmer.tiak@gmail.com
 License: MIT
 Project-URL: Source Code, https://raw.githubusercontent.com/Anupam1707/SecuriPy/main/SecuriPy.py
 Project-URL: Documentation, https://github.com/Anupam1707/SecuriPy/#readme
```

### Comparing `SecuriPy-1.0.0/README.md` & `SecuriPy-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `SecuriPy-1.0.0/SecuriPy.egg-info/PKG-INFO` & `SecuriPy-1.0.1/SecuriPy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SecuriPy
-Version: 1.0.0
+Version: 1.0.1
 Summary: Encrypter and Decrypter of Readable messages Using Python
 Home-page: https://github.com/Anupam1707/SecuriPy
 Author: Anupam Kanoongo
 Author-email: programmer.tiak@gmail.com
 License: MIT
 Project-URL: Source Code, https://raw.githubusercontent.com/Anupam1707/SecuriPy/main/SecuriPy.py
 Project-URL: Documentation, https://github.com/Anupam1707/SecuriPy/#readme
```

### Comparing `SecuriPy-1.0.0/SecuriPy.py` & `SecuriPy-1.0.1/SecuriPy.py`

 * *Files identical despite different names*

### Comparing `SecuriPy-1.0.0/build.py` & `SecuriPy-1.0.1/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SecuriPy",
-    version="1.0.0",
+    version="1.0.1",
     author="Anupam Kanoongo",
     author_email="programmer.tiak@gmail.com",
     description="Encrypter and Decrypter of Readable messages Using Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Anupam1707/SecuriPy",
     project_urls={
```

### Comparing `SecuriPy-1.0.0/setup.py` & `SecuriPy-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SecuriPy",
-    version="1.0.0",
+    version="1.0.1",
     author="Anupam Kanoongo",
     author_email="programmer.tiak@gmail.com",
     description="Encrypter and Decrypter of Readable messages Using Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Anupam1707/SecuriPy",
     project_urls={
```

