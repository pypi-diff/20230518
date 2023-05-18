# Comparing `tmp/svs_dataset_downloader-0.0.2.tar.gz` & `tmp/svs_dataset_downloader-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svs_dataset_downloader-0.0.2.tar", last modified: Sat May 13 21:27:33 2023, max compression
+gzip compressed data, was "svs_dataset_downloader-0.0.3.tar", last modified: Thu May 18 07:12:50 2023, max compression
```

## Comparing `svs_dataset_downloader-0.0.2.tar` & `svs_dataset_downloader-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 coolstorm   (501) staff       (20)        0 2023-05-13 21:27:33.401337 svs_dataset_downloader-0.0.2/
--rw-r--r--   0 coolstorm   (501) staff       (20)     1068 2023-05-13 21:17:11.000000 svs_dataset_downloader-0.0.2/LICENSE
--rw-r--r--   0 coolstorm   (501) staff       (20)      941 2023-05-13 21:27:33.401395 svs_dataset_downloader-0.0.2/PKG-INFO
--rw-r--r--   0 coolstorm   (501) staff       (20)       25 2023-05-13 21:17:11.000000 svs_dataset_downloader-0.0.2/README.md
--rw-r--r--   0 coolstorm   (501) staff       (20)       79 2023-05-13 21:27:33.401574 svs_dataset_downloader-0.0.2/setup.cfg
--rw-r--r--   0 coolstorm   (501) staff       (20)     1309 2023-05-13 21:26:39.000000 svs_dataset_downloader-0.0.2/setup.py
-drwxr-xr-x   0 coolstorm   (501) staff       (20)        0 2023-05-13 21:27:33.400639 svs_dataset_downloader-0.0.2/svs_dataset_downloader/
--rw-r--r--   0 coolstorm   (501) staff       (20)       33 2023-05-13 21:17:11.000000 svs_dataset_downloader-0.0.2/svs_dataset_downloader/__init__.py
--rw-r--r--   0 coolstorm   (501) staff       (20)     3807 2023-05-13 21:17:11.000000 svs_dataset_downloader-0.0.2/svs_dataset_downloader/downloader.py
-drwxr-xr-x   0 coolstorm   (501) staff       (20)        0 2023-05-13 21:27:33.401234 svs_dataset_downloader-0.0.2/svs_dataset_downloader.egg-info/
--rw-r--r--   0 coolstorm   (501) staff       (20)      941 2023-05-13 21:27:33.000000 svs_dataset_downloader-0.0.2/svs_dataset_downloader.egg-info/PKG-INFO
--rw-r--r--   0 coolstorm   (501) staff       (20)      337 2023-05-13 21:27:33.000000 svs_dataset_downloader-0.0.2/svs_dataset_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 coolstorm   (501) staff       (20)        1 2023-05-13 21:27:33.000000 svs_dataset_downloader-0.0.2/svs_dataset_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 coolstorm   (501) staff       (20)        9 2023-05-13 21:27:33.000000 svs_dataset_downloader-0.0.2/svs_dataset_downloader.egg-info/requires.txt
--rw-r--r--   0 coolstorm   (501) staff       (20)       23 2023-05-13 21:27:33.000000 svs_dataset_downloader-0.0.2/svs_dataset_downloader.egg-info/top_level.txt
+drwxr-xr-x   0 coolstorm   (501) staff       (20)        0 2023-05-18 07:12:50.551417 svs_dataset_downloader-0.0.3/
+-rw-r--r--   0 coolstorm   (501) staff       (20)     1068 2023-05-13 21:17:11.000000 svs_dataset_downloader-0.0.3/LICENSE
+-rw-r--r--   0 coolstorm   (501) staff       (20)     3822 2023-05-18 07:12:50.551499 svs_dataset_downloader-0.0.3/PKG-INFO
+-rw-r--r--   0 coolstorm   (501) staff       (20)     2906 2023-05-18 07:10:03.000000 svs_dataset_downloader-0.0.3/README.md
+-rw-r--r--   0 coolstorm   (501) staff       (20)       79 2023-05-18 07:12:50.551741 svs_dataset_downloader-0.0.3/setup.cfg
+-rw-r--r--   0 coolstorm   (501) staff       (20)     1309 2023-05-18 07:12:39.000000 svs_dataset_downloader-0.0.3/setup.py
+drwxr-xr-x   0 coolstorm   (501) staff       (20)        0 2023-05-18 07:12:50.550488 svs_dataset_downloader-0.0.3/svs_dataset_downloader/
+-rw-r--r--   0 coolstorm   (501) staff       (20)       33 2023-05-13 21:17:11.000000 svs_dataset_downloader-0.0.3/svs_dataset_downloader/__init__.py
+-rw-r--r--   0 coolstorm   (501) staff       (20)     3807 2023-05-13 21:32:26.000000 svs_dataset_downloader-0.0.3/svs_dataset_downloader/downloader.py
+drwxr-xr-x   0 coolstorm   (501) staff       (20)        0 2023-05-18 07:12:50.551298 svs_dataset_downloader-0.0.3/svs_dataset_downloader.egg-info/
+-rw-r--r--   0 coolstorm   (501) staff       (20)     3822 2023-05-18 07:12:50.000000 svs_dataset_downloader-0.0.3/svs_dataset_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 coolstorm   (501) staff       (20)      337 2023-05-18 07:12:50.000000 svs_dataset_downloader-0.0.3/svs_dataset_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 coolstorm   (501) staff       (20)        1 2023-05-18 07:12:50.000000 svs_dataset_downloader-0.0.3/svs_dataset_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 coolstorm   (501) staff       (20)        9 2023-05-18 07:12:50.000000 svs_dataset_downloader-0.0.3/svs_dataset_downloader.egg-info/requires.txt
+-rw-r--r--   0 coolstorm   (501) staff       (20)       23 2023-05-18 07:12:50.000000 svs_dataset_downloader-0.0.3/svs_dataset_downloader.egg-info/top_level.txt
```

### Comparing `svs_dataset_downloader-0.0.2/LICENSE` & `svs_dataset_downloader-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `svs_dataset_downloader-0.0.2/setup.py` & `svs_dataset_downloader-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Reads the content of your README.md into a variable to be used in the setup below
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='svs_dataset_downloader',
     packages=['svs_dataset_downloader'],
-    version='0.0.2',
+    version='0.0.3',
     license='MIT',
     description='Testing installation of Package',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Manas Gupta',
     author_email='manasgupta1820@gmail.com',
     url='https://github.com/Manas1820/svs-dataset-downloader',
```

### Comparing `svs_dataset_downloader-0.0.2/svs_dataset_downloader/downloader.py` & `svs_dataset_downloader-0.0.3/svs_dataset_downloader/downloader.py`

 * *Files identical despite different names*

