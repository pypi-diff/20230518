# Comparing `tmp/CirclesGenderDetectorPython-0.0.1.tar.gz` & `tmp/CirclesGenderDetectorPython-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CirclesGenderDetectorPython-0.0.1.tar", last modified: Thu May 18 07:45:58 2023, max compression
+gzip compressed data, was "CirclesGenderDetectorPython-0.0.2.tar", last modified: Thu May 18 08:16:28 2023, max compression
```

## Comparing `CirclesGenderDetectorPython-0.0.1.tar` & `CirclesGenderDetectorPython-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:45:58.273113 CirclesGenderDetectorPython-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:45:58.269113 CirclesGenderDetectorPython-0.0.1/CirclesGenderDetectionPython/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 07:45:45.000000 CirclesGenderDetectorPython-0.0.1/CirclesGenderDetectionPython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-05-18 07:45:45.000000 CirclesGenderDetectorPython-0.0.1/CirclesGenderDetectionPython/gender_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-18 07:45:45.000000 CirclesGenderDetectorPython-0.0.1/CirclesGenderDetectionPython/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:45:58.269113 CirclesGenderDetectorPython-0.0.1/CirclesGenderDetectorPython.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-18 07:45:58.000000 CirclesGenderDetectorPython-0.0.1/CirclesGenderDetectorPython.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-18 07:45:58.000000 CirclesGenderDetectorPython-0.0.1/CirclesGenderDetectorPython.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 07:45:58.000000 CirclesGenderDetectorPython-0.0.1/CirclesGenderDetectorPython.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-18 07:45:58.000000 CirclesGenderDetectorPython-0.0.1/CirclesGenderDetectorPython.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-18 07:45:58.269113 CirclesGenderDetectorPython-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-18 07:45:46.000000 CirclesGenderDetectorPython-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-18 07:45:46.000000 CirclesGenderDetectorPython-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 07:45:58.273113 CirclesGenderDetectorPython-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-18 07:45:46.000000 CirclesGenderDetectorPython-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:16:28.631312 CirclesGenderDetectorPython-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:16:28.631312 CirclesGenderDetectorPython-0.0.2/CirclesGenderDetectionPython/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 08:16:13.000000 CirclesGenderDetectorPython-0.0.2/CirclesGenderDetectionPython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-05-18 08:16:14.000000 CirclesGenderDetectorPython-0.0.2/CirclesGenderDetectionPython/gender_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-18 08:16:14.000000 CirclesGenderDetectorPython-0.0.2/CirclesGenderDetectionPython/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:16:28.631312 CirclesGenderDetectorPython-0.0.2/CirclesGenderDetectorPython.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-18 08:16:28.000000 CirclesGenderDetectorPython-0.0.2/CirclesGenderDetectorPython.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-18 08:16:28.000000 CirclesGenderDetectorPython-0.0.2/CirclesGenderDetectorPython.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 08:16:28.000000 CirclesGenderDetectorPython-0.0.2/CirclesGenderDetectorPython.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-18 08:16:28.000000 CirclesGenderDetectorPython-0.0.2/CirclesGenderDetectorPython.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-18 08:16:28.631312 CirclesGenderDetectorPython-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-18 08:16:14.000000 CirclesGenderDetectorPython-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-18 08:16:14.000000 CirclesGenderDetectorPython-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 08:16:28.631312 CirclesGenderDetectorPython-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-18 08:16:14.000000 CirclesGenderDetectorPython-0.0.2/setup.py
```

### Comparing `CirclesGenderDetectorPython-0.0.1/CirclesGenderDetectionPython/gender_detection.py` & `CirclesGenderDetectorPython-0.0.2/CirclesGenderDetectionPython/gender_detection.py`

 * *Files identical despite different names*

### Comparing `CirclesGenderDetectorPython-0.0.1/README.md` & `CirclesGenderDetectorPython-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `CirclesGenderDetectorPython-0.0.1/setup.py` & `CirclesGenderDetectorPython-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 print(setuptools.find_packages())
 setuptools.setup(
      name='CirclesGenderDetectorPython',  
-     version='0.0.1',
+     version='0.0.2',
      author="Circles",
      author_email="info@circles.zone",
      description="PyPI Package for gender detection",
      long_description="This is a package for running gender detection and predicting gender",
      long_description_content_type="text/markdown",
      url="https://github.com/circles-zone/gender-detection-backend",
      packages=setuptools.find_packages(),
```

