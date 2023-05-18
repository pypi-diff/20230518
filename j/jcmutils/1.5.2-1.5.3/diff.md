# Comparing `tmp/jcmutils-1.5.2.tar.gz` & `tmp/jcmutils-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcmutils-1.5.2.tar", last modified: Thu May 18 08:26:49 2023, max compression
+gzip compressed data, was "jcmutils-1.5.3.tar", last modified: Thu May 18 08:41:29 2023, max compression
```

## Comparing `jcmutils-1.5.2.tar` & `jcmutils-1.5.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-18 08:26:49.785235 jcmutils-1.5.2/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.5.2/LICENSE
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-18 08:26:49.785235 jcmutils-1.5.2/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-05-17 04:08:25.000000 jcmutils-1.5.2/README.md
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-18 08:26:49.785235 jcmutils-1.5.2/jcmutils/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      165 2023-05-17 04:08:25.000000 jcmutils-1.5.2/jcmutils/__init__.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)    11234 2023-05-18 08:26:27.000000 jcmutils-1.5.2/jcmutils/dataset_utils.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.5.2/jcmutils/gen_sources.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-05-17 04:08:25.000000 jcmutils-1.5.2/jcmutils/logger.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     8780 2023-05-17 04:08:25.000000 jcmutils-1.5.2/jcmutils/solver.py
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-18 08:26:49.785235 jcmutils-1.5.2/jcmutils.egg-info/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-18 08:26:49.000000 jcmutils-1.5.2/jcmutils.egg-info/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      294 2023-05-18 08:26:49.000000 jcmutils-1.5.2/jcmutils.egg-info/SOURCES.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-05-18 08:26:49.000000 jcmutils-1.5.2/jcmutils.egg-info/dependency_links.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-05-18 08:26:49.000000 jcmutils-1.5.2/jcmutils.egg-info/requires.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-05-18 08:26:49.000000 jcmutils-1.5.2/jcmutils.egg-info/top_level.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-05-18 08:26:49.785235 jcmutils-1.5.2/setup.cfg
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      539 2023-05-18 08:26:36.000000 jcmutils-1.5.2/setup.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-18 08:41:29.316414 jcmutils-1.5.3/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.5.3/LICENSE
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-18 08:41:29.316414 jcmutils-1.5.3/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-05-17 04:08:25.000000 jcmutils-1.5.3/README.md
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-18 08:41:29.316414 jcmutils-1.5.3/jcmutils/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      165 2023-05-17 04:08:25.000000 jcmutils-1.5.3/jcmutils/__init__.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)    11233 2023-05-18 08:41:02.000000 jcmutils-1.5.3/jcmutils/dataset_utils.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.5.3/jcmutils/gen_sources.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-05-17 04:08:25.000000 jcmutils-1.5.3/jcmutils/logger.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     8780 2023-05-17 04:08:25.000000 jcmutils-1.5.3/jcmutils/solver.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-18 08:41:29.316414 jcmutils-1.5.3/jcmutils.egg-info/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-18 08:41:29.000000 jcmutils-1.5.3/jcmutils.egg-info/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      294 2023-05-18 08:41:29.000000 jcmutils-1.5.3/jcmutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-05-18 08:41:29.000000 jcmutils-1.5.3/jcmutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-05-18 08:41:29.000000 jcmutils-1.5.3/jcmutils.egg-info/requires.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-05-18 08:41:29.000000 jcmutils-1.5.3/jcmutils.egg-info/top_level.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-05-18 08:41:29.316414 jcmutils-1.5.3/setup.cfg
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      539 2023-05-18 08:40:39.000000 jcmutils-1.5.3/setup.py
```

### Comparing `jcmutils-1.5.2/LICENSE` & `jcmutils-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jcmutils-1.5.2/README.md` & `jcmutils-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `jcmutils-1.5.2/jcmutils/dataset_utils.py` & `jcmutils-1.5.3/jcmutils/dataset_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         gradY = cv2.Sobel(diff_img, ddepth=cv2.CV_32F, dx=0, dy=1, ksize=-1)
         
         # subtract the y-gradient from the x-gradient
         gradient = cv2.subtract(gradX, gradY)
         gradient = cv2.convertScaleAbs(gradient)
         blurred = cv2.blur(gradient, (9, 9)) 
         (_, thresh) = cv2.threshold(blurred, 60 , 255, cv2.THRESH_BINARY)
-        kernel = cv2.getStructuringElement(cv2.MORPH_RECT, ( 20, 20))
+        kernel = cv2.getStructuringElement(cv2.MORPH_RECT, (18, 18))
         closed = cv2.morphologyEx(thresh, cv2.MORPH_CLOSE, kernel)
         closed = cv2.erode(closed, None, iterations=4)
         closed = cv2.dilate(closed, None, iterations=4)
 
         # 找距离图像中心点最近的一个封闭区域
         (cnts, _) = cv2.findContours(closed.copy(), cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
         # c = sorted(cnts, key=cv2.contourArea, reverse=True)[0]
```

### Comparing `jcmutils-1.5.2/jcmutils/gen_sources.py` & `jcmutils-1.5.3/jcmutils/gen_sources.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.5.2/jcmutils/logger.py` & `jcmutils-1.5.3/jcmutils/logger.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.5.2/jcmutils/solver.py` & `jcmutils-1.5.3/jcmutils/solver.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.5.2/setup.py` & `jcmutils-1.5.3/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 
-VERSION = '1.5.2'
+VERSION = '1.5.3'
 DESCRIPTION = "A general utils for jcmsuite"
 
 setup(
     name="jcmutils",
     version=VERSION,
     author="crafter-z",
     author_email="crafterz@163.com",
```

