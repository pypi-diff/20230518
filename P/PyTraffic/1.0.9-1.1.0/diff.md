# Comparing `tmp/PyTraffic-1.0.9.tar.gz` & `tmp/PyTraffic-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyTraffic-1.0.9.tar", last modified: Thu May 18 04:03:26 2023, max compression
+gzip compressed data, was "PyTraffic-1.1.0.tar", last modified: Thu May 18 05:12:52 2023, max compression
```

## Comparing `PyTraffic-1.0.9.tar` & `PyTraffic-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 04:03:26.043300 PyTraffic-1.0.9/
--rw-rw-rw-   0        0        0     2433 2023-05-18 02:54:06.000000 PyTraffic-1.0.9/CREDITS.md
--rw-rw-rw-   0        0        0     1091 2023-05-16 07:22:16.000000 PyTraffic-1.0.9/LICENSE.txt
--rw-rw-rw-   0        0        0      169 2023-05-18 04:01:46.000000 PyTraffic-1.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0     2672 2023-05-18 04:03:26.042299 PyTraffic-1.0.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-18 04:03:25.976627 PyTraffic-1.0.9/PyTraffic/
--rw-rw-rw-   0        0        0     4106 2023-05-18 03:41:27.000000 PyTraffic-1.0.9/PyTraffic/LicensePlate.py
--rw-rw-rw-   0        0        0     3197 2023-05-18 03:59:55.000000 PyTraffic-1.0.9/PyTraffic/PeopleDetection.py
--rw-rw-rw-   0        0        0     3072 2023-05-18 03:54:37.000000 PyTraffic-1.0.9/PyTraffic/VehicleDetection.py
--rw-rw-rw-   0        0        0       59 2023-05-13 05:58:41.000000 PyTraffic-1.0.9/PyTraffic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 04:03:26.033324 PyTraffic-1.0.9/PyTraffic/models/
--rw-rw-rw-   0        0        0   118802 2023-03-06 15:47:42.000000 PyTraffic-1.0.9/PyTraffic/models/haarcascade_car.xml
--rw-rw-rw-   0        0        0    78136 2023-05-13 06:54:47.000000 PyTraffic-1.0.9/PyTraffic/models/haarcascade_russian_plate_number.xml
-drwxrwxrwx   0        0        0        0 2023-05-18 04:03:26.008610 PyTraffic-1.0.9/PyTraffic.egg-info/
--rw-rw-rw-   0        0        0     2672 2023-05-18 04:03:24.000000 PyTraffic-1.0.9/PyTraffic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      415 2023-05-18 04:03:24.000000 PyTraffic-1.0.9/PyTraffic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 04:03:24.000000 PyTraffic-1.0.9/PyTraffic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-18 04:03:24.000000 PyTraffic-1.0.9/PyTraffic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-18 04:03:24.000000 PyTraffic-1.0.9/PyTraffic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2066 2023-05-18 04:00:28.000000 PyTraffic-1.0.9/README.md
--rw-rw-rw-   0        0        0       42 2023-05-18 04:03:26.044294 PyTraffic-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1149 2023-05-18 04:00:06.000000 PyTraffic-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 05:12:52.350962 PyTraffic-1.1.0/
+-rw-rw-rw-   0        0        0     2433 2023-05-18 02:54:06.000000 PyTraffic-1.1.0/CREDITS.md
+-rw-rw-rw-   0        0        0     1091 2023-05-16 07:22:16.000000 PyTraffic-1.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      169 2023-05-18 04:01:46.000000 PyTraffic-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2672 2023-05-18 05:12:52.348967 PyTraffic-1.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-18 05:12:52.318673 PyTraffic-1.1.0/PyTraffic/
+-rw-rw-rw-   0        0        0     4106 2023-05-18 03:41:27.000000 PyTraffic-1.1.0/PyTraffic/LicensePlate.py
+-rw-rw-rw-   0        0        0     3485 2023-05-18 05:10:03.000000 PyTraffic-1.1.0/PyTraffic/PeopleDetection.py
+-rw-rw-rw-   0        0        0     3072 2023-05-18 03:54:37.000000 PyTraffic-1.1.0/PyTraffic/VehicleDetection.py
+-rw-rw-rw-   0        0        0       59 2023-05-13 05:58:41.000000 PyTraffic-1.1.0/PyTraffic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 05:12:52.343994 PyTraffic-1.1.0/PyTraffic/models/
+-rw-rw-rw-   0        0        0   118802 2023-03-06 15:47:42.000000 PyTraffic-1.1.0/PyTraffic/models/haarcascade_car.xml
+-rw-rw-rw-   0        0        0    78136 2023-05-13 06:54:47.000000 PyTraffic-1.1.0/PyTraffic/models/haarcascade_russian_plate_number.xml
+drwxrwxrwx   0        0        0        0 2023-05-18 05:12:52.336626 PyTraffic-1.1.0/PyTraffic.egg-info/
+-rw-rw-rw-   0        0        0     2672 2023-05-18 05:12:52.000000 PyTraffic-1.1.0/PyTraffic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      415 2023-05-18 05:12:52.000000 PyTraffic-1.1.0/PyTraffic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 05:12:52.000000 PyTraffic-1.1.0/PyTraffic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-18 05:12:52.000000 PyTraffic-1.1.0/PyTraffic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-18 05:12:52.000000 PyTraffic-1.1.0/PyTraffic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2066 2023-05-18 05:12:10.000000 PyTraffic-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-18 05:12:52.351958 PyTraffic-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1149 2023-05-18 05:12:14.000000 PyTraffic-1.1.0/setup.py
```

### Comparing `PyTraffic-1.0.9/CREDITS.md` & `PyTraffic-1.1.0/CREDITS.md`

 * *Files identical despite different names*

### Comparing `PyTraffic-1.0.9/LICENSE.txt` & `PyTraffic-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyTraffic-1.0.9/PKG-INFO` & `PyTraffic-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTraffic
-Version: 1.0.9
+Version: 1.1.0
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
-**Version** - 1.0.9</br>
+**Version** - 1.1.0</br>
 **Description** - PyTraffic is a Python module to work on traffic-related functions and use cases.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PyTraffic](https://github.com/Anikethc/PyTraffic)</br>
 **Pypi.org URL** - [https://pypi.org/project/PyTraffic](https://pypi.org/project/PyTraffic)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pytraffic-docs](https://aniketh-chavare.gitbook.io/pytraffic-docs)
 
 ## License
```

### Comparing `PyTraffic-1.0.9/PyTraffic/LicensePlate.py` & `PyTraffic-1.1.0/PyTraffic/LicensePlate.py`

 * *Files identical despite different names*

### Comparing `PyTraffic-1.0.9/PyTraffic/PeopleDetection.py` & `PyTraffic-1.1.0/PyTraffic/PeopleDetection.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,73 +2,74 @@
 
 # Imports
 import cv2
 import mimetypes
 import os
 import imutils
 
-# Variables
-__all__ = ["detectPeople"]
-
 # Initializing the HOG Descriptor
 detector = cv2.HOGDescriptor()
 detector.setSVMDetector(cv2.HOGDescriptor_getDefaultPeopleDetector())
 
 # Function 1 - Detect
-def detect(frame):
+def detect(frame, function):
     # Set the Box Coordinates & Styles
     bounding_box_cordinates, weights =  detector.detectMultiScale(frame, winStride = (4, 4), padding = (8, 8), scale = 1.03)
 
     # Detect the People
     person = 1
 
     for x,y,w,h in bounding_box_cordinates:
         cv2.rectangle(frame, (x,y), (x+w,y+h), (0,255,0), 2)
         cv2.putText(frame, f"Person {person}", (x,y), cv2.FONT_HERSHEY_SIMPLEX, 0.5, (0,0,255), 1)
 
         person += 1
 
+        # Perform the User Function
+        if ((function is not None) and (callable(function))):
+            function()
+
     # Text on the Output
     cv2.putText(frame, f"Total People: {person-1}", (40, 40), cv2.FONT_HERSHEY_DUPLEX, 0.8, (255,0,0), 2)
 
     # Show the Output
     cv2.imshow("People Detection", frame)
     return frame
 
 # Function 2 - Detect By Video
-def detectByVideo(path):
+def detectByVideo(path, function):
     # Initializing the Video
     video = cv2.VideoCapture(path)
     check, frame = video.read()
 
     # Check if Video is Null
     if (check == False):
         raise Exception("There's something wrong with the video. Try again with another one.")
 
     # Open the Video and Send Video Data to the "detect()" Function
     while video.isOpened():
         check, frame = video.read()
 
         if (check):
             frame = imutils.resize(frame, width=min(800, frame.shape[1]))
-            frame = detect(frame)
+            frame = detect(frame, function)
 
             # Clicking "q" Closes the Video
             if (cv2.waitKey(1) == ord("q")):
                 break
         else:
             raise Exception("There's something wrong with the video. Try again with another one.")
             break
 
     # Stopping OpenCV
     video.release()
     cv2.destroyAllWindows()
 
 # Function 3 - Detect People
-def detectPeople(path, show=False):
+def detectPeople(path, show=False, function=None):
     # Check if Path Exists
     if (os.path.exists(path)):
         # Check File Type
         mimetypes.init()
 
         mimestart = mimetypes.guess_type(path)[0]
         mimestart = mimestart.split("/")[0]
@@ -80,21 +81,25 @@
             # Detecting the Humans
             (humans, _) = detector.detectMultiScale(image, winStride=(10, 10), padding=(32, 32), scale=1.1)
 
             for (x, y, w, h) in humans:
                 pad_w, pad_h = int(0.15 * w), int(0.01 * h)
                 cv2.rectangle(image, (x + pad_w, y + pad_h), (x + w - pad_w, y + h - pad_h), (0, 255, 0), 2)
 
+                # Perform the User Function
+                if ((function is not None) and (callable(function))):
+                    function()
+
             # Returning the Image
             if (show):
                 cv2.imshow("People Detection", image)
                 cv2.waitKey(0)
 
             # Returning the Count
             return len(humans)
         elif (mimestart == "video"): # Video
             # Sending the Video to the "detectByVideo()" Function
-            detectByVideo(path)
+            detectByVideo(path, function)
         else:
             raise Exception("The file provided must be an image or a video.")
     else:
         raise Exception("The image or video file path does not exist.")
```

### Comparing `PyTraffic-1.0.9/PyTraffic/VehicleDetection.py` & `PyTraffic-1.1.0/PyTraffic/VehicleDetection.py`

 * *Files identical despite different names*

### Comparing `PyTraffic-1.0.9/PyTraffic/models/haarcascade_car.xml` & `PyTraffic-1.1.0/PyTraffic/models/haarcascade_car.xml`

 * *Files identical despite different names*

### Comparing `PyTraffic-1.0.9/PyTraffic/models/haarcascade_russian_plate_number.xml` & `PyTraffic-1.1.0/PyTraffic/models/haarcascade_russian_plate_number.xml`

 * *Files identical despite different names*

### Comparing `PyTraffic-1.0.9/PyTraffic.egg-info/PKG-INFO` & `PyTraffic-1.1.0/PyTraffic.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTraffic
-Version: 1.0.9
+Version: 1.1.0
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
-**Version** - 1.0.9</br>
+**Version** - 1.1.0</br>
 **Description** - PyTraffic is a Python module to work on traffic-related functions and use cases.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PyTraffic](https://github.com/Anikethc/PyTraffic)</br>
 **Pypi.org URL** - [https://pypi.org/project/PyTraffic](https://pypi.org/project/PyTraffic)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pytraffic-docs](https://aniketh-chavare.gitbook.io/pytraffic-docs)
 
 ## License
```

### Comparing `PyTraffic-1.0.9/README.md` & `PyTraffic-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 PyTraffic is a Python module to work on traffic-related functions and use cases.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pytraffic-docs).
 
 ## Module Information
 
 **Name** - PyTraffic</br>
-**Version** - 1.0.9</br>
+**Version** - 1.1.0</br>
 **Description** - PyTraffic is a Python module to work on traffic-related functions and use cases.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PyTraffic](https://github.com/Anikethc/PyTraffic)</br>
 **Pypi.org URL** - [https://pypi.org/project/PyTraffic](https://pypi.org/project/PyTraffic)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pytraffic-docs](https://aniketh-chavare.gitbook.io/pytraffic-docs)
 
 ## License
```

### Comparing `PyTraffic-1.0.9/setup.py` & `PyTraffic-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # README.md
 with open("README.md") as readme_file:
     README = readme_file.read()
 
 # Setup Arguements
 setup_args = dict (
     name="PyTraffic",
-    version="1.0.9",
+    version="1.1.0",
     description="PyTraffic is a Python module to work on traffic-related functions and use cases.",
     long_description_content_type="text/markdown",
     long_description=README,
     license="MIT",
     packages=find_packages(),
     include_package_data=True,
     author="Aniketh Chavare",
```

