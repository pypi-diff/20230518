# Comparing `tmp/PyTraffic-1.1.0.tar.gz` & `tmp/PyTraffic-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyTraffic-1.1.0.tar", last modified: Thu May 18 05:12:52 2023, max compression
+gzip compressed data, was "PyTraffic-1.1.1.tar", last modified: Thu May 18 06:02:43 2023, max compression
```

## Comparing `PyTraffic-1.1.0.tar` & `PyTraffic-1.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 05:12:52.350962 PyTraffic-1.1.0/
--rw-rw-rw-   0        0        0     2433 2023-05-18 02:54:06.000000 PyTraffic-1.1.0/CREDITS.md
--rw-rw-rw-   0        0        0     1091 2023-05-16 07:22:16.000000 PyTraffic-1.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0      169 2023-05-18 04:01:46.000000 PyTraffic-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2672 2023-05-18 05:12:52.348967 PyTraffic-1.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-18 05:12:52.318673 PyTraffic-1.1.0/PyTraffic/
--rw-rw-rw-   0        0        0     4106 2023-05-18 03:41:27.000000 PyTraffic-1.1.0/PyTraffic/LicensePlate.py
--rw-rw-rw-   0        0        0     3485 2023-05-18 05:10:03.000000 PyTraffic-1.1.0/PyTraffic/PeopleDetection.py
--rw-rw-rw-   0        0        0     3072 2023-05-18 03:54:37.000000 PyTraffic-1.1.0/PyTraffic/VehicleDetection.py
--rw-rw-rw-   0        0        0       59 2023-05-13 05:58:41.000000 PyTraffic-1.1.0/PyTraffic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 05:12:52.343994 PyTraffic-1.1.0/PyTraffic/models/
--rw-rw-rw-   0        0        0   118802 2023-03-06 15:47:42.000000 PyTraffic-1.1.0/PyTraffic/models/haarcascade_car.xml
--rw-rw-rw-   0        0        0    78136 2023-05-13 06:54:47.000000 PyTraffic-1.1.0/PyTraffic/models/haarcascade_russian_plate_number.xml
-drwxrwxrwx   0        0        0        0 2023-05-18 05:12:52.336626 PyTraffic-1.1.0/PyTraffic.egg-info/
--rw-rw-rw-   0        0        0     2672 2023-05-18 05:12:52.000000 PyTraffic-1.1.0/PyTraffic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      415 2023-05-18 05:12:52.000000 PyTraffic-1.1.0/PyTraffic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 05:12:52.000000 PyTraffic-1.1.0/PyTraffic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-18 05:12:52.000000 PyTraffic-1.1.0/PyTraffic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-18 05:12:52.000000 PyTraffic-1.1.0/PyTraffic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2066 2023-05-18 05:12:10.000000 PyTraffic-1.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-18 05:12:52.351958 PyTraffic-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1149 2023-05-18 05:12:14.000000 PyTraffic-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 06:02:43.538675 PyTraffic-1.1.1/
+-rw-rw-rw-   0        0        0     2705 2023-05-18 06:01:40.000000 PyTraffic-1.1.1/CREDITS.md
+-rw-rw-rw-   0        0        0     1091 2023-05-16 07:22:16.000000 PyTraffic-1.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      169 2023-05-18 04:01:46.000000 PyTraffic-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2672 2023-05-18 06:02:43.537715 PyTraffic-1.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-18 06:02:43.506759 PyTraffic-1.1.1/PyTraffic/
+-rw-rw-rw-   0        0        0     4106 2023-05-18 03:41:27.000000 PyTraffic-1.1.1/PyTraffic/LicensePlate.py
+-rw-rw-rw-   0        0        0     3485 2023-05-18 05:10:03.000000 PyTraffic-1.1.1/PyTraffic/PeopleDetection.py
+-rw-rw-rw-   0        0        0     3072 2023-05-18 03:54:37.000000 PyTraffic-1.1.1/PyTraffic/VehicleDetection.py
+-rw-rw-rw-   0        0        0       59 2023-05-13 05:58:41.000000 PyTraffic-1.1.1/PyTraffic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 06:02:43.533688 PyTraffic-1.1.1/PyTraffic/models/
+-rw-rw-rw-   0        0        0   118802 2023-03-06 15:47:42.000000 PyTraffic-1.1.1/PyTraffic/models/haarcascade_car.xml
+-rw-rw-rw-   0        0        0    78136 2023-05-13 06:54:47.000000 PyTraffic-1.1.1/PyTraffic/models/haarcascade_russian_plate_number.xml
+drwxrwxrwx   0        0        0        0 2023-05-18 06:02:43.524711 PyTraffic-1.1.1/PyTraffic.egg-info/
+-rw-rw-rw-   0        0        0     2672 2023-05-18 06:02:43.000000 PyTraffic-1.1.1/PyTraffic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      415 2023-05-18 06:02:43.000000 PyTraffic-1.1.1/PyTraffic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 06:02:43.000000 PyTraffic-1.1.1/PyTraffic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-18 06:02:43.000000 PyTraffic-1.1.1/PyTraffic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-18 06:02:43.000000 PyTraffic-1.1.1/PyTraffic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2066 2023-05-18 06:01:45.000000 PyTraffic-1.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-18 06:02:43.539672 PyTraffic-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1149 2023-05-18 06:01:48.000000 PyTraffic-1.1.1/setup.py
```

### Comparing `PyTraffic-1.1.0/CREDITS.md` & `PyTraffic-1.1.1/CREDITS.md`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,19 @@
 **Link:** Visit [here](https://www.codingninjas.com/codestudio/library/vehicle-detection-using-opencv).<br>
 
 **Name:** How to detect humans in an image in OpenCV Python?<br>
 **Used For:** PeopleDetection (Sub-Module)<br>
 **Author:** Shahid Akhtar Khan<br>
 **Link:** Visit [here](https://www.tutorialspoint.com/how-to-detect-humans-in-an-image-in-opencv-python).<br>
 
+**Name:** Python Project – Real-time Human Detection & Counting<br>
+**Used For:** PeopleDetection (Sub-Module)<br>
+**Author:** Data-Flair.training<br>
+**Link:** Visit [here](https://data-flair.training/blogs/python-project-real-time-human-detection-counting).<br>
+
 ## <u><i>Python Modules</i></u>
 
 **Module:** opencv-python<br>
 **Used For:** LicensePlate and VehicleDetection (Sub-Modules)<br>
 **Author:** OpenCV<br>
 **Link:** Visit [here](https://github.com/opencv/opencv-python).<br>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `PyTraffic-1.1.0/LICENSE.txt` & `PyTraffic-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyTraffic-1.1.0/PKG-INFO` & `PyTraffic-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTraffic
-Version: 1.1.0
+Version: 1.1.1
 Summary: PyTraffic is a Python module to work on traffic-related functions and use cases.
 Home-page: https://github.com/Anikethc/PyTraffic
 Download-URL: https://pypi.org/project/PyTraffic
 Author: Aniketh Chavare
 Author-email: anikethchavare@outlook.com
 License: MIT
 Keywords: Traffic,Traffic Density,Traffic Density Estimation,License Plates,License Plate Detection,License Plate Recognition,Vehicles,Vehicle Detection
@@ -18,15 +18,15 @@
 PyTraffic is a Python module to work on traffic-related functions and use cases.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pytraffic-docs).
 
 ## Module Information
 
 **Name** - PyTraffic</br>
-**Version** - 1.1.0</br>
+**Version** - 1.1.1</br>
 **Description** - PyTraffic is a Python module to work on traffic-related functions and use cases.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PyTraffic](https://github.com/Anikethc/PyTraffic)</br>
 **Pypi.org URL** - [https://pypi.org/project/PyTraffic](https://pypi.org/project/PyTraffic)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pytraffic-docs](https://aniketh-chavare.gitbook.io/pytraffic-docs)
 
 ## License
```

### Comparing `PyTraffic-1.1.0/PyTraffic/LicensePlate.py` & `PyTraffic-1.1.1/PyTraffic/LicensePlate.py`

 * *Files identical despite different names*

### Comparing `PyTraffic-1.1.0/PyTraffic/PeopleDetection.py` & `PyTraffic-1.1.1/PyTraffic/PeopleDetection.py`

 * *Files identical despite different names*

### Comparing `PyTraffic-1.1.0/PyTraffic/VehicleDetection.py` & `PyTraffic-1.1.1/PyTraffic/VehicleDetection.py`

 * *Files identical despite different names*

### Comparing `PyTraffic-1.1.0/PyTraffic/models/haarcascade_car.xml` & `PyTraffic-1.1.1/PyTraffic/models/haarcascade_car.xml`

 * *Files identical despite different names*

### Comparing `PyTraffic-1.1.0/PyTraffic/models/haarcascade_russian_plate_number.xml` & `PyTraffic-1.1.1/PyTraffic/models/haarcascade_russian_plate_number.xml`

 * *Files identical despite different names*

### Comparing `PyTraffic-1.1.0/PyTraffic.egg-info/PKG-INFO` & `PyTraffic-1.1.1/PyTraffic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTraffic
-Version: 1.1.0
+Version: 1.1.1
 Summary: PyTraffic is a Python module to work on traffic-related functions and use cases.
 Home-page: https://github.com/Anikethc/PyTraffic
 Download-URL: https://pypi.org/project/PyTraffic
 Author: Aniketh Chavare
 Author-email: anikethchavare@outlook.com
 License: MIT
 Keywords: Traffic,Traffic Density,Traffic Density Estimation,License Plates,License Plate Detection,License Plate Recognition,Vehicles,Vehicle Detection
@@ -18,15 +18,15 @@
 PyTraffic is a Python module to work on traffic-related functions and use cases.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pytraffic-docs).
 
 ## Module Information
 
 **Name** - PyTraffic</br>
-**Version** - 1.1.0</br>
+**Version** - 1.1.1</br>
 **Description** - PyTraffic is a Python module to work on traffic-related functions and use cases.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PyTraffic](https://github.com/Anikethc/PyTraffic)</br>
 **Pypi.org URL** - [https://pypi.org/project/PyTraffic](https://pypi.org/project/PyTraffic)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pytraffic-docs](https://aniketh-chavare.gitbook.io/pytraffic-docs)
 
 ## License
```

### Comparing `PyTraffic-1.1.0/README.md` & `PyTraffic-1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 PyTraffic is a Python module to work on traffic-related functions and use cases.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pytraffic-docs).
 
 ## Module Information
 
 **Name** - PyTraffic</br>
-**Version** - 1.1.0</br>
+**Version** - 1.1.1</br>
 **Description** - PyTraffic is a Python module to work on traffic-related functions and use cases.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PyTraffic](https://github.com/Anikethc/PyTraffic)</br>
 **Pypi.org URL** - [https://pypi.org/project/PyTraffic](https://pypi.org/project/PyTraffic)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pytraffic-docs](https://aniketh-chavare.gitbook.io/pytraffic-docs)
 
 ## License
```

### Comparing `PyTraffic-1.1.0/setup.py` & `PyTraffic-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # README.md
 with open("README.md") as readme_file:
     README = readme_file.read()
 
 # Setup Arguements
 setup_args = dict (
     name="PyTraffic",
-    version="1.1.0",
+    version="1.1.1",
     description="PyTraffic is a Python module to work on traffic-related functions and use cases.",
     long_description_content_type="text/markdown",
     long_description=README,
     license="MIT",
     packages=find_packages(),
     include_package_data=True,
     author="Aniketh Chavare",
```

