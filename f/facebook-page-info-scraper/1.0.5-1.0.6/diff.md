# Comparing `tmp/facebook-page-info-scraper-1.0.5.tar.gz` & `tmp/facebook-page-info-scraper-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facebook-page-info-scraper-1.0.5.tar", last modified: Tue May 16 12:58:52 2023, max compression
+gzip compressed data, was "facebook-page-info-scraper-1.0.6.tar", last modified: Thu May 18 12:13:06 2023, max compression
```

## Comparing `facebook-page-info-scraper-1.0.5.tar` & `facebook-page-info-scraper-1.0.6.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:58:52.634785 facebook-page-info-scraper-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-16 12:58:52.634785 facebook-page-info-scraper-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-16 12:58:43.000000 facebook-page-info-scraper-1.0.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:58:52.634785 facebook-page-info-scraper-1.0.5/facebook_page_info_scraper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-16 12:58:52.000000 facebook-page-info-scraper-1.0.5/facebook_page_info_scraper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-16 12:58:52.000000 facebook-page-info-scraper-1.0.5/facebook_page_info_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 12:58:52.000000 facebook-page-info-scraper-1.0.5/facebook_page_info_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 12:58:52.000000 facebook-page-info-scraper-1.0.5/facebook_page_info_scraper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 12:58:52.000000 facebook-page-info-scraper-1.0.5/facebook_page_info_scraper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 12:58:52.634785 facebook-page-info-scraper-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-16 12:58:43.000000 facebook-page-info-scraper-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:13:06.171849 facebook-page-info-scraper-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-18 12:13:06.171849 facebook-page-info-scraper-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-18 12:12:57.000000 facebook-page-info-scraper-1.0.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:13:06.171849 facebook-page-info-scraper-1.0.6/facebook-page-info-scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 12:12:57.000000 facebook-page-info-scraper-1.0.6/facebook-page-info-scraper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19866 2023-05-18 12:12:57.000000 facebook-page-info-scraper-1.0.6/facebook-page-info-scraper/facebook-page-info-scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:13:06.171849 facebook-page-info-scraper-1.0.6/facebook_page_info_scraper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-18 12:13:06.000000 facebook-page-info-scraper-1.0.6/facebook_page_info_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-18 12:13:06.000000 facebook-page-info-scraper-1.0.6/facebook_page_info_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 12:13:06.000000 facebook-page-info-scraper-1.0.6/facebook_page_info_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-18 12:13:06.000000 facebook-page-info-scraper-1.0.6/facebook_page_info_scraper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-18 12:13:06.000000 facebook-page-info-scraper-1.0.6/facebook_page_info_scraper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 12:13:06.171849 facebook-page-info-scraper-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-18 12:12:57.000000 facebook-page-info-scraper-1.0.6/setup.py
```

### Comparing `facebook-page-info-scraper-1.0.5/PKG-INFO` & `facebook-page-info-scraper-1.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facebook-page-info-scraper
-Version: 1.0.5
+Version: 1.0.6
 Summary: A Python package capable of crawling Facebook page information
 Author: Wael hkiri
 Author-email: wael.hkiri.dev@gmail.com
 Description-Content-Type: text/x-rst
 
 ==============================
 facebook-page-info-scraper
```

### Comparing `facebook-page-info-scraper-1.0.5/README.rst` & `facebook-page-info-scraper-1.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `facebook-page-info-scraper-1.0.5/facebook_page_info_scraper.egg-info/PKG-INFO` & `facebook-page-info-scraper-1.0.6/facebook_page_info_scraper.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facebook-page-info-scraper
-Version: 1.0.5
+Version: 1.0.6
 Summary: A Python package capable of crawling Facebook page information
 Author: Wael hkiri
 Author-email: wael.hkiri.dev@gmail.com
 Description-Content-Type: text/x-rst
 
 ==============================
 facebook-page-info-scraper
```

### Comparing `facebook-page-info-scraper-1.0.5/setup.py` & `facebook-page-info-scraper-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.rst', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='facebook-page-info-scraper',
-    version='1.0.5',
+    version='1.0.6',
     author='Wael hkiri',
     author_email='wael.hkiri.dev@gmail.com',
     description='A Python package capable of crawling Facebook page information',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     packages=find_packages(),
     install_requires=[
```

