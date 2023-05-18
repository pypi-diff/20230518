# Comparing `tmp/pyspeaker-3.0.tar.gz` & `tmp/pyspeaker-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspeaker-3.0.tar", last modified: Thu May 18 16:15:39 2023, max compression
+gzip compressed data, was "pyspeaker-4.0.tar", last modified: Thu May 18 16:48:20 2023, max compression
```

## Comparing `pyspeaker-3.0.tar` & `pyspeaker-4.0.tar`

### file list

```diff
@@ -1,15 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 16:15:39.417851 pyspeaker-3.0/
--rw-rw-rw-   0        0        0     1091 2023-02-23 09:47:52.000000 pyspeaker-3.0/LICENSE.txt
--rw-rw-rw-   0        0        0      212 2023-05-18 16:15:39.415856 pyspeaker-3.0/PKG-INFO
--rw-rw-rw-   0        0        0      329 2023-05-18 11:26:55.000000 pyspeaker-3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 16:15:39.387943 pyspeaker-3.0/app/
-drwxrwxrwx   0        0        0        0 2023-05-18 16:15:39.398847 pyspeaker-3.0/app/pyspeaker/
--rw-rw-rw-   0        0        0      776 2023-05-18 11:45:12.000000 pyspeaker-3.0/app/pyspeaker/Audio.py
-drwxrwxrwx   0        0        0        0 2023-05-18 16:15:39.412851 pyspeaker-3.0/app/pyspeaker.egg-info/
--rw-rw-rw-   0        0        0      212 2023-05-18 16:15:39.000000 pyspeaker-3.0/app/pyspeaker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-05-18 16:15:39.000000 pyspeaker-3.0/app/pyspeaker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 16:15:39.000000 pyspeaker-3.0/app/pyspeaker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-05-18 16:15:39.000000 pyspeaker-3.0/app/pyspeaker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-18 16:15:39.000000 pyspeaker-3.0/app/pyspeaker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 16:15:39.417851 pyspeaker-3.0/setup.cfg
--rw-rw-rw-   0        0        0      660 2023-05-18 16:14:53.000000 pyspeaker-3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 16:48:20.538233 pyspeaker-4.0/
+-rw-rw-rw-   0        0        0     1091 2023-02-23 09:47:52.000000 pyspeaker-4.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      212 2023-05-18 16:48:20.537217 pyspeaker-4.0/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2023-05-18 11:26:55.000000 pyspeaker-4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 16:48:20.501103 pyspeaker-4.0/app/
+drwxrwxrwx   0        0        0        0 2023-05-18 16:48:20.532996 pyspeaker-4.0/app/pyspeaker.egg-info/
+-rw-rw-rw-   0        0        0      212 2023-05-18 16:48:20.000000 pyspeaker-4.0/app/pyspeaker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2023-05-18 16:48:20.000000 pyspeaker-4.0/app/pyspeaker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 16:48:20.000000 pyspeaker-4.0/app/pyspeaker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-05-18 16:48:20.000000 pyspeaker-4.0/app/pyspeaker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-18 16:48:20.000000 pyspeaker-4.0/app/pyspeaker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 16:48:20.539641 pyspeaker-4.0/setup.cfg
+-rw-rw-rw-   0        0        0      650 2023-05-18 16:48:09.000000 pyspeaker-4.0/setup.py
```

### Comparing `pyspeaker-3.0/LICENSE.txt` & `pyspeaker-4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyspeaker-3.0/setup.py` & `pyspeaker-4.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import find_packages, setup
 
 setup(
 name = "pyspeaker",
 author = "Akshat Sabharwal",
-version = "3.0",
+version = "4.0",
 package_dir={"": "app"},
-package=find_packages(where="app"),
+py_modules=["Audio"],
 author_email = "akshatsabharwal35@gmail.com",
 description = """A module for controlling the Speakers of the device
-Methods
+\bMethods\b
 
 get_volume: Returns the current volume of the device's speakers
 set_volume: Sets the volume of the device's speakers to the given volume level.
 rangify: Interpolates or maps the given volume range of the speakers to the user-specified range.""",
 install_requires = [
     'pycaw',
     'ctypes-callable',
```

