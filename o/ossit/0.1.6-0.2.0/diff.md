# Comparing `tmp/ossit-0.1.6.tar.gz` & `tmp/ossit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ossit-0.1.6.tar", last modified: Sun May  7 22:51:11 2023, max compression
+gzip compressed data, was "ossit-0.2.0.tar", last modified: Thu May 18 17:24:19 2023, max compression
```

## Comparing `ossit-0.1.6.tar` & `ossit-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:51:11.339275 ossit-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-07 22:50:59.000000 ossit-0.1.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-07 22:51:11.339275 ossit-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-07 22:50:59.000000 ossit-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:51:11.339275 ossit-0.1.6/ossit/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-07 22:50:59.000000 ossit-0.1.6/ossit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-07 22:50:59.000000 ossit-0.1.6/ossit/api_requestor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:51:11.339275 ossit-0.1.6/ossit/api_resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 22:50:59.000000 ossit-0.1.6/ossit/api_resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-07 22:50:59.000000 ossit-0.1.6/ossit/api_resources/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-07 22:50:59.000000 ossit-0.1.6/ossit/api_resources/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-07 22:50:59.000000 ossit-0.1.6/ossit/ossit_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:51:11.339275 ossit-0.1.6/ossit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-07 22:51:11.000000 ossit-0.1.6/ossit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-07 22:51:11.000000 ossit-0.1.6/ossit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 22:51:11.000000 ossit-0.1.6/ossit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-07 22:51:11.000000 ossit-0.1.6/ossit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-07 22:50:59.000000 ossit-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-07 22:51:11.339275 ossit-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 22:50:59.000000 ossit-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:24:19.032308 ossit-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-18 17:24:08.000000 ossit-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-18 17:24:19.032308 ossit-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-05-18 17:24:08.000000 ossit-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:24:19.032308 ossit-0.2.0/ossit/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-18 17:24:08.000000 ossit-0.2.0/ossit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-18 17:24:08.000000 ossit-0.2.0/ossit/api_requestor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:24:19.032308 ossit-0.2.0/ossit/api_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-18 17:24:08.000000 ossit-0.2.0/ossit/api_resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-18 17:24:08.000000 ossit-0.2.0/ossit/api_resources/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-18 17:24:08.000000 ossit-0.2.0/ossit/api_resources/statistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-18 17:24:08.000000 ossit-0.2.0/ossit/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-18 17:24:08.000000 ossit-0.2.0/ossit/ossit_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:24:19.032308 ossit-0.2.0/ossit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-18 17:24:18.000000 ossit-0.2.0/ossit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-18 17:24:19.000000 ossit-0.2.0/ossit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 17:24:18.000000 ossit-0.2.0/ossit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 17:24:18.000000 ossit-0.2.0/ossit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-18 17:24:08.000000 ossit-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-18 17:24:19.032308 ossit-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 17:24:08.000000 ossit-0.2.0/setup.py
```

### Comparing `ossit-0.1.6/LICENSE.txt` & `ossit-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ossit-0.1.6/setup.cfg` & `ossit-0.2.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ossit
-version = 0.1.6
+version = 0.2.0
 author = Wesley Howery
 author_email = wesleyh@stratusadv.com
 description = Python Package to connect to ossit API
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
@@ -14,13 +14,13 @@
 [options]
 include_package_data = True
 packages = find:
 
 [options.packages.find]
 exclude = 
 	tests
-python_requires = >=3.6
+python_requires = >=3.9
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

