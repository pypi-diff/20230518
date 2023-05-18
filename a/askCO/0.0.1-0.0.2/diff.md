# Comparing `tmp/askCO-0.0.1.tar.gz` & `tmp/askCO-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "askCO-0.0.1.tar", last modified: Wed May 17 02:37:01 2023, max compression
+gzip compressed data, was "askCO-0.0.2.tar", last modified: Thu May 18 02:24:02 2023, max compression
```

## Comparing `askCO-0.0.1.tar` & `askCO-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 02:37:01.610352 askCO-0.0.1/
--rw-rw-rw-   0        0        0      622 2023-05-17 02:37:01.610352 askCO-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3048 2023-05-17 02:06:05.000000 askCO-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 02:37:01.610352 askCO-0.0.1/askCO.egg-info/
--rw-rw-rw-   0        0        0      622 2023-05-17 02:37:01.000000 askCO-0.0.1/askCO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      134 2023-05-17 02:37:01.000000 askCO-0.0.1/askCO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 02:37:01.000000 askCO-0.0.1/askCO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 02:37:01.000000 askCO-0.0.1/askCO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 02:37:01.610352 askCO-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      826 2023-05-17 02:09:16.000000 askCO-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 02:24:02.791366 askCO-0.0.2/
+-rw-rw-rw-   0        0        0      622 2023-05-18 02:24:02.791366 askCO-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3048 2023-05-17 02:06:05.000000 askCO-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 02:24:02.791366 askCO-0.0.2/askCO.egg-info/
+-rw-rw-rw-   0        0        0      622 2023-05-18 02:24:02.000000 askCO-0.0.2/askCO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      134 2023-05-18 02:24:02.000000 askCO-0.0.2/askCO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 02:24:02.000000 askCO-0.0.2/askCO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 02:24:02.000000 askCO-0.0.2/askCO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 02:24:02.791366 askCO-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      826 2023-05-18 01:54:17.000000 askCO-0.0.2/setup.py
```

### Comparing `askCO-0.0.1/PKG-INFO` & `askCO-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: askCO
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python interface for Te Papa's collections API
 Author: Lucy Schrader
 Author-email: lucy@schrader.nz
 License: MIT License
 Keywords: python,museum,api
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `askCO-0.0.1/README.md` & `askCO-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `askCO-0.0.1/askCO.egg-info/PKG-INFO` & `askCO-0.0.2/askCO.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: askCO
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python interface for Te Papa's collections API
 Author: Lucy Schrader
 Author-email: lucy@schrader.nz
 License: MIT License
 Keywords: python,museum,api
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `askCO-0.0.1/setup.py` & `askCO-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
 	long_description = "Python interface to search and query records for collections objects and specimens held by Museum of New Zealand Te Papa Tongarewa."
 
 setup(
 	name="askCO",
-	version="0.0.1",
+	version="0.0.2",
 	author="Lucy Schrader",
 	author_email="lucy@schrader.nz",
 	description="Python interface for Te Papa's collections API",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	packages=find_packages(),
 	install_requires=[],
```

