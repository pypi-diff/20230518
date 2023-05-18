# Comparing `tmp/imageTable-0.1.1.tar.gz` & `tmp/imageTable-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imageTable-0.1.1.tar", last modified: Thu May 18 01:10:49 2023, max compression
+gzip compressed data, was "imageTable-0.1.2.tar", last modified: Thu May 18 01:15:10 2023, max compression
```

## Comparing `imageTable-0.1.1.tar` & `imageTable-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-18 01:10:49.979932 imageTable-0.1.1/
--rw-r--r--   0 kevin      (501) staff       (20)      210 2023-05-18 01:10:49.978484 imageTable-0.1.1/PKG-INFO
--rw-r--r--   0 kevin      (501) staff       (20)       38 2023-05-18 01:10:49.980137 imageTable-0.1.1/setup.cfg
--rw-r--r--   0 kevin      (501) staff       (20)      685 2023-05-18 01:09:56.000000 imageTable-0.1.1/setup.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-18 01:10:49.972013 imageTable-0.1.1/src/
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-18 01:10:49.974703 imageTable-0.1.1/src/imageTable/
--rw-rw-r--   0 kevin      (501) staff       (20)       70 2023-03-29 00:08:52.000000 imageTable-0.1.1/src/imageTable/__init__.py
--rwxr--r--   0 kevin      (501) staff       (20)     1201 2023-05-18 01:05:01.000000 imageTable-0.1.1/src/imageTable/image2csv.py
--rwxr-xr-x   0 kevin      (501) staff       (20)     4592 2023-05-17 23:08:13.000000 imageTable-0.1.1/src/imageTable/imageTable.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-18 01:10:49.977714 imageTable-0.1.1/src/imageTable.egg-info/
--rw-r--r--   0 kevin      (501) staff       (20)      210 2023-05-18 01:10:49.000000 imageTable-0.1.1/src/imageTable.egg-info/PKG-INFO
--rw-r--r--   0 kevin      (501) staff       (20)      281 2023-05-18 01:10:49.000000 imageTable-0.1.1/src/imageTable.egg-info/SOURCES.txt
--rw-r--r--   0 kevin      (501) staff       (20)        1 2023-05-18 01:10:49.000000 imageTable-0.1.1/src/imageTable.egg-info/dependency_links.txt
--rw-r--r--   0 kevin      (501) staff       (20)       44 2023-05-18 01:10:49.000000 imageTable-0.1.1/src/imageTable.egg-info/requires.txt
--rw-r--r--   0 kevin      (501) staff       (20)       11 2023-05-18 01:10:49.000000 imageTable-0.1.1/src/imageTable.egg-info/top_level.txt
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-18 01:15:10.748750 imageTable-0.1.2/
+-rw-r--r--   0 kevin      (501) staff       (20)      210 2023-05-18 01:15:10.748181 imageTable-0.1.2/PKG-INFO
+-rw-r--r--   0 kevin      (501) staff       (20)       38 2023-05-18 01:15:10.749111 imageTable-0.1.2/setup.cfg
+-rw-r--r--   0 kevin      (501) staff       (20)      685 2023-05-18 01:14:51.000000 imageTable-0.1.2/setup.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-18 01:15:10.741109 imageTable-0.1.2/src/
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-18 01:15:10.744330 imageTable-0.1.2/src/imageTable/
+-rw-rw-r--   0 kevin      (501) staff       (20)       70 2023-05-18 01:14:23.000000 imageTable-0.1.2/src/imageTable/__init__.py
+-rwxr--r--   0 kevin      (501) staff       (20)     1201 2023-05-18 01:05:01.000000 imageTable-0.1.2/src/imageTable/image2csv.py
+-rwxr-xr-x   0 kevin      (501) staff       (20)     4592 2023-05-17 23:08:13.000000 imageTable-0.1.2/src/imageTable/imageTable.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-18 01:15:10.747392 imageTable-0.1.2/src/imageTable.egg-info/
+-rw-r--r--   0 kevin      (501) staff       (20)      210 2023-05-18 01:15:10.000000 imageTable-0.1.2/src/imageTable.egg-info/PKG-INFO
+-rw-r--r--   0 kevin      (501) staff       (20)      281 2023-05-18 01:15:10.000000 imageTable-0.1.2/src/imageTable.egg-info/SOURCES.txt
+-rw-r--r--   0 kevin      (501) staff       (20)        1 2023-05-18 01:15:10.000000 imageTable-0.1.2/src/imageTable.egg-info/dependency_links.txt
+-rw-r--r--   0 kevin      (501) staff       (20)       44 2023-05-18 01:15:10.000000 imageTable-0.1.2/src/imageTable.egg-info/requires.txt
+-rw-r--r--   0 kevin      (501) staff       (20)       11 2023-05-18 01:15:10.000000 imageTable-0.1.2/src/imageTable.egg-info/top_level.txt
```

### Comparing `imageTable-0.1.1/setup.py` & `imageTable-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from warnings import warn
 
 if sys.version_info.major != 3:
     raise RuntimeError('imageTable requires Python 3')
 
 
 setup(name='imageTable',
-      version='0.1.1',
+      version='0.1.2',
       description='manipulation of czi and ims files',
       author='',
       author_email='',
       package_dir={'': 'src'},
       packages=['imageTable'],
       install_requires=[
           'numpy',
```

### Comparing `imageTable-0.1.1/src/imageTable/image2csv.py` & `imageTable-0.1.2/src/imageTable/image2csv.py`

 * *Files identical despite different names*

### Comparing `imageTable-0.1.1/src/imageTable/imageTable.py` & `imageTable-0.1.2/src/imageTable/imageTable.py`

 * *Files identical despite different names*

