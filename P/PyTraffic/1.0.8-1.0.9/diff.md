# Comparing `tmp/PyTraffic-1.0.8.tar.gz` & `tmp/PyTraffic-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyTraffic-1.0.8.tar", last modified: Tue May 16 09:55:35 2023, max compression
+gzip compressed data, was "PyTraffic-1.0.9.tar", last modified: Thu May 18 04:03:26 2023, max compression
```

## Comparing `PyTraffic-1.0.8.tar` & `PyTraffic-1.0.9.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 09:55:35.563603 PyTraffic-1.0.8/
--rw-rw-rw-   0        0        0     1091 2023-05-16 07:22:16.000000 PyTraffic-1.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0      149 2023-05-16 06:43:09.000000 PyTraffic-1.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     4831 2023-05-16 09:55:35.561611 PyTraffic-1.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-16 09:55:35.515731 PyTraffic-1.0.8/PyTraffic/
--rw-rw-rw-   0        0        0     3645 2023-05-16 09:29:42.000000 PyTraffic-1.0.8/PyTraffic/LicensePlate.py
--rw-rw-rw-   0        0        0     3039 2023-05-16 09:44:23.000000 PyTraffic-1.0.8/PyTraffic/VehicleDetection.py
--rw-rw-rw-   0        0        0       59 2023-05-13 05:58:41.000000 PyTraffic-1.0.8/PyTraffic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:55:35.536675 PyTraffic-1.0.8/PyTraffic/models/
--rw-rw-rw-   0        0        0   118802 2023-03-06 15:47:42.000000 PyTraffic-1.0.8/PyTraffic/models/haarcascade_car.xml
--rw-rw-rw-   0        0        0    78136 2023-05-13 06:54:47.000000 PyTraffic-1.0.8/PyTraffic/models/haarcascade_russian_plate_number.xml
-drwxrwxrwx   0        0        0        0 2023-05-16 09:55:35.530691 PyTraffic-1.0.8/PyTraffic.egg-info/
--rw-rw-rw-   0        0        0     4831 2023-05-16 09:55:34.000000 PyTraffic-1.0.8/PyTraffic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      375 2023-05-16 09:55:34.000000 PyTraffic-1.0.8/PyTraffic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 09:55:34.000000 PyTraffic-1.0.8/PyTraffic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-16 09:55:34.000000 PyTraffic-1.0.8/PyTraffic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-16 09:55:34.000000 PyTraffic-1.0.8/PyTraffic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4253 2023-05-16 09:52:27.000000 PyTraffic-1.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-05-16 09:55:35.563603 PyTraffic-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1063 2023-05-16 09:52:40.000000 PyTraffic-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 04:03:26.043300 PyTraffic-1.0.9/
+-rw-rw-rw-   0        0        0     2433 2023-05-18 02:54:06.000000 PyTraffic-1.0.9/CREDITS.md
+-rw-rw-rw-   0        0        0     1091 2023-05-16 07:22:16.000000 PyTraffic-1.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      169 2023-05-18 04:01:46.000000 PyTraffic-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2672 2023-05-18 04:03:26.042299 PyTraffic-1.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-18 04:03:25.976627 PyTraffic-1.0.9/PyTraffic/
+-rw-rw-rw-   0        0        0     4106 2023-05-18 03:41:27.000000 PyTraffic-1.0.9/PyTraffic/LicensePlate.py
+-rw-rw-rw-   0        0        0     3197 2023-05-18 03:59:55.000000 PyTraffic-1.0.9/PyTraffic/PeopleDetection.py
+-rw-rw-rw-   0        0        0     3072 2023-05-18 03:54:37.000000 PyTraffic-1.0.9/PyTraffic/VehicleDetection.py
+-rw-rw-rw-   0        0        0       59 2023-05-13 05:58:41.000000 PyTraffic-1.0.9/PyTraffic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 04:03:26.033324 PyTraffic-1.0.9/PyTraffic/models/
+-rw-rw-rw-   0        0        0   118802 2023-03-06 15:47:42.000000 PyTraffic-1.0.9/PyTraffic/models/haarcascade_car.xml
+-rw-rw-rw-   0        0        0    78136 2023-05-13 06:54:47.000000 PyTraffic-1.0.9/PyTraffic/models/haarcascade_russian_plate_number.xml
+drwxrwxrwx   0        0        0        0 2023-05-18 04:03:26.008610 PyTraffic-1.0.9/PyTraffic.egg-info/
+-rw-rw-rw-   0        0        0     2672 2023-05-18 04:03:24.000000 PyTraffic-1.0.9/PyTraffic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      415 2023-05-18 04:03:24.000000 PyTraffic-1.0.9/PyTraffic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 04:03:24.000000 PyTraffic-1.0.9/PyTraffic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-18 04:03:24.000000 PyTraffic-1.0.9/PyTraffic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-18 04:03:24.000000 PyTraffic-1.0.9/PyTraffic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2066 2023-05-18 04:00:28.000000 PyTraffic-1.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-18 04:03:26.044294 PyTraffic-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1149 2023-05-18 04:00:06.000000 PyTraffic-1.0.9/setup.py
```

### Comparing `PyTraffic-1.0.8/LICENSE.txt` & `PyTraffic-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyTraffic-1.0.8/PyTraffic/LicensePlate.py` & `PyTraffic-1.0.9/PyTraffic/LicensePlate.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,101 +2,108 @@
 
 # Imports
 import os
 import cv2
 import imutils
 import numpy as np
 import pytesseract
+import mimetypes
 
-# Function 1 - Show License Plate
-def showLicensePlate(imagePath):
-    # Set Directory
-    directory = os.path.dirname(os.path.realpath(__file__))
-    directory = directory.replace(os.sep, "/")
+# Set Directory
+directory = os.path.dirname(os.path.realpath(__file__))
+directory = directory.replace(os.sep, "/")
 
-    # Check if Path Exists
-    if (os.path.exists(imagePath)):
-        # Reading the Image
-        img = cv2.imread(imagePath)
-
-        # Converting the Images to Grayscale
-        gray = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
-        cascade = cv2.CascadeClassifier(directory + "/models/haarcascade_russian_plate_number.xml")
-
-        # Finding the Plates
-        plates = cascade.detectMultiScale(gray, 1.2, 5)
-        print("Number of Detected License Plates:", len(plates))
-
-        # Displaying Each License Plate
-        for (x,y,w,h) in plates:
-            cv2.rectangle(img, (x,y), (x+w, y+h), (0,255,0), 2)
-            gray_plates = gray[y:y+h, x:x+w]
-            color_plates = img[y:y+h, x:x+w]
-
-            cv2.imshow("Vehicle Image", img)
-            cv2.imshow("Number Plate", gray_plates)
-            cv2.waitKey(0)
-    else:
-        raise Exception("The image file path does not exist.")
+# Variables
+cascade = cv2.CascadeClassifier(directory + "/models/haarcascade_russian_plate_number.xml")
 
-# Function 2 - Get License Plate Number
-def getLicensePlateNumber(imagePath, tesseractPath):
+# Function 1 - Get License Plate
+def getLicensePlate(imagePath, tesseractPath, show=False):
     # Check if Path Exists
     if (os.path.exists(imagePath)):
         # Check for Tesseract
         if (os.path.exists(tesseractPath)):
-            # Connecting to Tesseract
-            pytesseract.pytesseract.tesseract_cmd = tesseractPath
-
-            # Reading the Image
-            img = cv2.imread(imagePath, cv2.IMREAD_COLOR)
-            img = cv2.resize(img, (600,400))
-
-            # Converting the Image to Grayscale
-            gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY) 
-            gray = cv2.bilateralFilter(gray, 13, 15, 15) 
-
-            # Finding & Counting Contours
-            edged = cv2.Canny(gray, 30, 200) 
-            contours = cv2.findContours(edged.copy(), cv2.RETR_TREE, cv2.CHAIN_APPROX_SIMPLE)
-            contours = imutils.grab_contours(contours)
-            contours = sorted(contours, key = cv2.contourArea, reverse = True)[:10]
-            screenCnt = None
-
-            for c in contours:
-                peri = cv2.arcLength(c, True)
-                approx = cv2.approxPolyDP(c, 0.018 * peri, True)
-
-                if len(approx) == 4:
-                    screenCnt = approx
-                    break
+            # Check File Type
+            mimetypes.init()
 
-            if screenCnt is None:
-                detected = 0
-            else:
-                detected = 1
+            mimestart = mimetypes.guess_type(imagePath)[0]
+            mimestart = mimestart.split("/")[0]
 
-            if detected == 1:
-                cv2.drawContours(img, [screenCnt], -1, (0, 0, 255), 3)
+            if (mimestart == "image"): # Image:
+                # Connecting to Tesseract
+                pytesseract.pytesseract.tesseract_cmd = tesseractPath
+
+                # Reading the Image
+                img = cv2.imread(imagePath, cv2.IMREAD_COLOR)
+                img = cv2.resize(img, (600,400))
+
+                # Converting the Image to Grayscale
+                gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY) 
+                gray = cv2.bilateralFilter(gray, 13, 15, 15) 
+
+                # Finding & Counting Contours
+                edged = cv2.Canny(gray, 30, 200) 
+                contours = cv2.findContours(edged.copy(), cv2.RETR_TREE, cv2.CHAIN_APPROX_SIMPLE)
+                contours = imutils.grab_contours(contours)
+                contours = sorted(contours, key = cv2.contourArea, reverse = True)[:10]
+                screenCnt = None
+
+                for c in contours:
+                    peri = cv2.arcLength(c, True)
+                    approx = cv2.approxPolyDP(c, 0.018 * peri, True)
+
+                    if len(approx) == 4:
+                        screenCnt = approx
+                        break
+
+                if screenCnt is None:
+                    detected = 0
+                else:
+                    detected = 1
+
+                if detected == 1:
+                    cv2.drawContours(img, [screenCnt], -1, (0, 0, 255), 3)
+
+                mask = np.zeros(gray.shape, np.uint8)
+                new_image = cv2.drawContours(mask, [screenCnt], 0,255, -1,)
+                new_image = cv2.bitwise_and(img, img, mask=mask)
+
+                (x, y) = np.where(mask == 255)
+                (topx, topy) = (np.min(x), np.min(y))
+                (bottomx, bottomy) = (np.max(x), np.max(y))
+                Cropped = gray[topx:bottomx+1, topy:bottomy+1]
+
+                # License Plate Number
+                text = pytesseract.image_to_string(Cropped, config="--psm 11")
+
+                # Stopping OpenCV
+                cv2.waitKey(0)
+                cv2.destroyAllWindows()
+
+                # Check for "show" Argument
+                if (show):
+                    # Reading the Image
+                    img = cv2.imread(imagePath)
+
+                    # Converting the Images to Grayscale
+                    gray = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
+
+                    # Finding the Plates
+                    plates = cascade.detectMultiScale(gray, 1.2, 5)
+
+                    # Displaying Each License Plate
+                    for (x,y,w,h) in plates:
+                        cv2.rectangle(img, (x,y), (x+w, y+h), (0,255,0), 2)
+                        gray_plates = gray[y:y+h, x:x+w]
+                        color_plates = img[y:y+h, x:x+w]
+
+                        cv2.imshow("Vehicle Image", img)
+                        cv2.imshow("Number Plate", gray_plates)
+                        cv2.waitKey(0)
 
-            mask = np.zeros(gray.shape,np.uint8)
-            new_image = cv2.drawContours(mask,[screenCnt],0,255,-1,)
-            new_image = cv2.bitwise_and(img,img,mask=mask)
-
-            (x, y) = np.where(mask == 255)
-            (topx, topy) = (np.min(x), np.min(y))
-            (bottomx, bottomy) = (np.max(x), np.max(y))
-            Cropped = gray[topx:bottomx+1, topy:bottomy+1]
-
-            # License Plate Number
-            text = pytesseract.image_to_string(Cropped, config="--psm 11")
-
-            # Close OpenCV
-            cv2.waitKey(0)
-            cv2.destroyAllWindows()
-
-            # Return the License Plate Number
-            return text
+                # Return the License Plate Number
+                return text
+            else:
+                raise Exception("The file provided must be an image.")
         else:
             raise Exception("The 'tesseract.exe' file path does not exist. Make sure Tesseract-OCR is installed and the path given exists.")
     else:
         raise Exception("The image file path does not exist.")
```

### Comparing `PyTraffic-1.0.8/PyTraffic/VehicleDetection.py` & `PyTraffic-1.0.9/PyTraffic/VehicleDetection.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 directory = directory.replace(os.sep, "/")
 
 # Variables
 car_cascade = cv2.CascadeClassifier(directory + "/models/haarcascade_car.xml")
 
 # Function 1 - Detect Cars
 def detectCars(path, show=False):
+    # Check if Path Exists
     if (os.path.exists(path)):
         # Check File Type
         mimetypes.init()
 
         mimestart = mimetypes.guess_type(path)[0]
         mimestart = mimestart.split("/")[0]
 
@@ -68,29 +69,29 @@
             # Opening the Video
             video = cv2.VideoCapture(path)
 
             # Opening the Video and Processing
             while video.isOpened():
                 time.sleep(.05)
 
-                # Read First Frame
+                # Reading the First Frame
                 ret, frame = video.read()
                 gray = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)
 
                 # Identifying the Cars
                 cars = car_cascade.detectMultiScale(gray, 1.4, 2)
 
                 for (x,y,w,h) in cars:
                     cv2.rectangle(frame, (x, y), (x+w, y+h), (0, 255, 255), 2)
                     cv2.imshow("Vehicle Detection - Cars", frame)
 
-                # Clicking 'q' Closes the Video
+                # Clicking "q" Closes the Video
                 if cv2.waitKey(1) == ord("q"):
                     break
 
-            # Closing the Video
+            # Stopping OpenCV
             video.release()
             cv2.destroyAllWindows()
         else:
             raise Exception("The file provided must be an image or a video.")
     else:
         raise Exception("The image or video file path does not exist.")
```

### Comparing `PyTraffic-1.0.8/PyTraffic/models/haarcascade_car.xml` & `PyTraffic-1.0.9/PyTraffic/models/haarcascade_car.xml`

 * *Files identical despite different names*

### Comparing `PyTraffic-1.0.8/PyTraffic/models/haarcascade_russian_plate_number.xml` & `PyTraffic-1.0.9/PyTraffic/models/haarcascade_russian_plate_number.xml`

 * *Files identical despite different names*

