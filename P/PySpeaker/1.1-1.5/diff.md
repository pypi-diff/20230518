# Comparing `tmp/PySpeaker-1.1.tar.gz` & `tmp/PySpeaker-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySpeaker-1.1.tar", last modified: Thu May 18 14:38:40 2023, max compression
+gzip compressed data, was "PySpeaker-1.5.tar", last modified: Thu May 18 15:17:27 2023, max compression
```

## Comparing `PySpeaker-1.1.tar` & `PySpeaker-1.5.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 14:38:40.259764 PySpeaker-1.1/
--rw-rw-rw-   0        0        0     1091 2023-02-23 09:47:52.000000 PySpeaker-1.1/LICENSE.txt
--rw-rw-rw-   0        0        0      212 2023-05-18 14:38:40.257762 PySpeaker-1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-18 14:38:40.254764 PySpeaker-1.1/PySpeaker.egg-info/
--rw-rw-rw-   0        0        0      212 2023-05-18 14:38:40.000000 PySpeaker-1.1/PySpeaker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2023-05-18 14:38:40.000000 PySpeaker-1.1/PySpeaker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 14:38:40.000000 PySpeaker-1.1/PySpeaker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-05-18 14:38:40.000000 PySpeaker-1.1/PySpeaker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-18 14:38:40.000000 PySpeaker-1.1/PySpeaker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      329 2023-05-18 11:26:55.000000 PySpeaker-1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-18 14:38:40.259764 PySpeaker-1.1/setup.cfg
--rw-rw-rw-   0        0        0      651 2023-05-18 14:38:31.000000 PySpeaker-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 15:17:27.258566 PySpeaker-1.5/
+-rw-rw-rw-   0        0        0     1091 2023-02-23 09:47:52.000000 PySpeaker-1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      212 2023-05-18 15:17:27.255046 PySpeaker-1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-18 15:17:27.248084 PySpeaker-1.5/PySpeaker.egg-info/
+-rw-rw-rw-   0        0        0      212 2023-05-18 15:17:27.000000 PySpeaker-1.5/PySpeaker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2023-05-18 15:17:27.000000 PySpeaker-1.5/PySpeaker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 15:17:27.000000 PySpeaker-1.5/PySpeaker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-05-18 15:17:27.000000 PySpeaker-1.5/PySpeaker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-18 15:17:27.000000 PySpeaker-1.5/PySpeaker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      329 2023-05-18 11:26:55.000000 PySpeaker-1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 15:17:27.252045 PySpeaker-1.5/pyspeaker/
+-rw-rw-rw-   0        0        0      776 2023-05-18 11:45:12.000000 PySpeaker-1.5/pyspeaker/Audio.py
+-rw-rw-rw-   0        0        0       42 2023-05-18 15:17:27.259530 PySpeaker-1.5/setup.cfg
+-rw-rw-rw-   0        0        0      622 2023-05-18 15:16:41.000000 PySpeaker-1.5/setup.py
```

### Comparing `PySpeaker-1.1/LICENSE.txt` & `PySpeaker-1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PySpeaker-1.1/setup.py` & `PySpeaker-1.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from setuptools import find_packages, setup
 
 setup(
 name = "PySpeaker",
 author = "Akshat Sabharwal",
-version = "1.1",
-packages=find_packages(),
-py_modules=['pyspeaker'],
+version = "1.5",
+packages=["pyspeaker"],
 author_email = "akshatsabharwal35@gmail.com",
 description = """A module for controlling the Speakers of the device
 Methods
 
 get_volume: Returns the current volume of the device's speakers
 set_volume: Sets the volume of the device's speakers to the given volume level.
 rangify: Interpolates or maps the given volume range of the speakers to the user-specified range.""",
```

