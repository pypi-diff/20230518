# Comparing `tmp/LasBuildSeg-0.1.12.tar.gz` & `tmp/LasBuildSeg-0.1.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LasBuildSeg-0.1.12.tar", last modified: Wed May 17 19:19:37 2023, max compression
+gzip compressed data, was "LasBuildSeg-0.1.13.tar", last modified: Wed May 17 20:11:15 2023, max compression
```

## Comparing `LasBuildSeg-0.1.12.tar` & `LasBuildSeg-0.1.13.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 19:19:37.063806 LasBuildSeg-0.1.12/
--rw-rw-rw-   0        0        0      107 2023-05-17 19:14:54.000000 LasBuildSeg-0.1.12/CHANGELOG.txt
--rw-rw-rw-   0        0        0    18092 2023-05-10 06:27:14.000000 LasBuildSeg-0.1.12/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-05-17 19:19:36.913309 LasBuildSeg-0.1.12/LasBuildSeg/
-drwxrwxrwx   0        0        0        0 2023-05-17 19:19:37.056830 LasBuildSeg-0.1.12/LasBuildSeg/.ipynb_checkpoints/
--rw-rw-rw-   0        0        0    11872 2023-05-10 09:29:06.000000 LasBuildSeg-0.1.12/LasBuildSeg/.ipynb_checkpoints/LasBuildSeg-checkpoint.py
--rw-rw-rw-   0        0        0    14489 2023-05-17 19:17:14.000000 LasBuildSeg-0.1.12/LasBuildSeg/LasBuildSeg.py
--rw-rw-rw-   0        0        0      518 2023-05-17 08:50:32.000000 LasBuildSeg-0.1.12/LasBuildSeg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 19:19:37.001016 LasBuildSeg-0.1.12/LasBuildSeg.egg-info/
--rw-rw-rw-   0        0        0     2372 2023-05-17 19:19:35.000000 LasBuildSeg-0.1.12/LasBuildSeg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2023-05-17 19:19:36.000000 LasBuildSeg-0.1.12/LasBuildSeg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 19:19:35.000000 LasBuildSeg-0.1.12/LasBuildSeg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2023-05-17 19:19:35.000000 LasBuildSeg-0.1.12/LasBuildSeg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-17 19:19:35.000000 LasBuildSeg-0.1.12/LasBuildSeg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       51 2023-05-10 09:31:40.000000 LasBuildSeg-0.1.12/MANIFEST.in
--rw-rw-rw-   0        0        0     2372 2023-05-17 19:19:37.060816 LasBuildSeg-0.1.12/PKG-INFO
--rw-rw-rw-   0        0        0     1440 2023-05-17 09:56:57.000000 LasBuildSeg-0.1.12/README.md
--rw-rw-rw-   0        0        0     1496 2023-05-17 19:14:58.000000 LasBuildSeg-0.1.12/Setup.py
--rw-rw-rw-   0        0        0      123 2023-05-17 11:16:46.000000 LasBuildSeg-0.1.12/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 19:19:37.063806 LasBuildSeg-0.1.12/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-17 20:11:15.149426 LasBuildSeg-0.1.13/
+-rw-rw-rw-   0        0        0      107 2023-05-17 20:07:57.000000 LasBuildSeg-0.1.13/CHANGELOG.txt
+-rw-rw-rw-   0        0        0    18092 2023-05-10 06:27:14.000000 LasBuildSeg-0.1.13/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 20:11:15.095611 LasBuildSeg-0.1.13/LasBuildSeg/
+drwxrwxrwx   0        0        0        0 2023-05-17 20:11:15.140456 LasBuildSeg-0.1.13/LasBuildSeg/.ipynb_checkpoints/
+-rw-rw-rw-   0        0        0    11872 2023-05-10 09:29:06.000000 LasBuildSeg-0.1.13/LasBuildSeg/.ipynb_checkpoints/LasBuildSeg-checkpoint.py
+-rw-rw-rw-   0        0        0    14634 2023-05-17 20:07:44.000000 LasBuildSeg-0.1.13/LasBuildSeg/LasBuildSeg.py
+-rw-rw-rw-   0        0        0      518 2023-05-17 08:50:32.000000 LasBuildSeg-0.1.13/LasBuildSeg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 20:11:15.137465 LasBuildSeg-0.1.13/LasBuildSeg.egg-info/
+-rw-rw-rw-   0        0        0     2448 2023-05-17 20:11:13.000000 LasBuildSeg-0.1.13/LasBuildSeg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2023-05-17 20:11:14.000000 LasBuildSeg-0.1.13/LasBuildSeg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 20:11:13.000000 LasBuildSeg-0.1.13/LasBuildSeg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2023-05-17 20:11:13.000000 LasBuildSeg-0.1.13/LasBuildSeg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-17 20:11:13.000000 LasBuildSeg-0.1.13/LasBuildSeg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       51 2023-05-10 09:31:40.000000 LasBuildSeg-0.1.13/MANIFEST.in
+-rw-rw-rw-   0        0        0     2448 2023-05-17 20:11:15.145460 LasBuildSeg-0.1.13/PKG-INFO
+-rw-rw-rw-   0        0        0     1516 2023-05-17 20:10:13.000000 LasBuildSeg-0.1.13/README.md
+-rw-rw-rw-   0        0        0     1496 2023-05-17 20:08:01.000000 LasBuildSeg-0.1.13/Setup.py
+-rw-rw-rw-   0        0        0      123 2023-05-17 11:16:46.000000 LasBuildSeg-0.1.13/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 20:11:15.149426 LasBuildSeg-0.1.13/setup.cfg
```

### Comparing `LasBuildSeg-0.1.12/LICENSE.txt` & `LasBuildSeg-0.1.13/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `LasBuildSeg-0.1.12/LasBuildSeg/.ipynb_checkpoints/LasBuildSeg-checkpoint.py` & `LasBuildSeg-0.1.13/LasBuildSeg/.ipynb_checkpoints/LasBuildSeg-checkpoint.py`

 * *Files identical despite different names*

### Comparing `LasBuildSeg-0.1.12/LasBuildSeg/LasBuildSeg.py` & `LasBuildSeg-0.1.13/LasBuildSeg/LasBuildSeg.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,22 +83,26 @@
     las_file_dtm = laspy.read('updated_file.las')
 
     # Create a Pyproj CRS object for the input EPSG code
     input_crs = pyproj.CRS.from_epsg(input_epsg) 
 
     points = np.vstack((las_file_dtm.x, las_file_dtm.y, las_file_dtm.z)).T
     
-
+    # Extract the x, y, and z coordinates from the LAS file
+    xdtm = las_file_dtm.x
+    ydtm = las_file_dtm.y
+     
+    # Calculate the grid bounds based on the x and y coordinates
+    min_x = np.floor(min(xdtm))
+    max_x = np.ceil(max(xdtm))
+    min_y = np.floor(min(ydtm))
+    max_y = np.ceil(max(ydtm))
     # Classify ground points in lidar data class 2
     ground_points = points[las_file_dtm.classification == 2]
 
-    # Determine the bounds of the point cloud
-    min_x, max_x = np.min(points[:,0]), np.max(points[:,0])
-    min_y, max_y = np.min(points[:,1]), np.max(points[:,1])
-
     # Calculate the size of the output raster
     width = int(np.ceil((max_x - min_x) / resolution))
     height = int(np.ceil((max_y - min_y) / resolution))
 
     # Create the output raster profile
     profile = {
         'driver': 'GTiff',
```

### Comparing `LasBuildSeg-0.1.12/LasBuildSeg/__init__.py` & `LasBuildSeg-0.1.13/LasBuildSeg/__init__.py`

 * *Files identical despite different names*

### Comparing `LasBuildSeg-0.1.12/LasBuildSeg.egg-info/PKG-INFO` & `LasBuildSeg-0.1.13/LasBuildSeg.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LasBuildSeg
-Version: 0.1.12
+Version: 0.1.13
 Summary: Building Footrprint Extraction from Aerial LiDAR data
 Home-page: 
 Author: MertcanErdem
 Author-email: merak908@gmail.com
 License: GNU General Public License v2.0
 Keywords: Building,Lidar
 Classifier: Development Status :: 5 - Production/Stable
@@ -27,17 +27,19 @@
 ```python
 import LasBuildSeg as lasb
 import numpy as np
 
 input_laz = '<input>.laz'
 epsg_code = <epsg_code>
 dsm_resolution = <resolution>
+scale=<lazfilescale>
+method=<interpoaltion method>
 
-lasb.generate_dsm(input_laz, epsg_code, dsm_resolution)
-lasb.generate_dtm(input_laz, epsg_code , dsm_resolution)
+Lasb.generate_dsm(input_laz, epsg_code, dsm_resolution,intermethod)
+Lasb.generate_dtm(input_laz, epsg_code, dsm_resolution,intermethod)
 lasb.generate_ndhm('dtm.tif', 'dsm.tif')
 
 img, profile = lasb.read_geotiff('ndhm.tif')
 lasb.DSM_Transform('dsm.tif')
 
 dem, _ = lasb.read_geotiff('dsm3857.tif')
 img_8bit = lasb.to_8bit(img)
```

### Comparing `LasBuildSeg-0.1.12/PKG-INFO` & `LasBuildSeg-0.1.13/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LasBuildSeg
-Version: 0.1.12
+Version: 0.1.13
 Summary: Building Footrprint Extraction from Aerial LiDAR data
 Home-page: 
 Author: MertcanErdem
 Author-email: merak908@gmail.com
 License: GNU General Public License v2.0
 Keywords: Building,Lidar
 Classifier: Development Status :: 5 - Production/Stable
@@ -27,17 +27,19 @@
 ```python
 import LasBuildSeg as lasb
 import numpy as np
 
 input_laz = '<input>.laz'
 epsg_code = <epsg_code>
 dsm_resolution = <resolution>
+scale=<lazfilescale>
+method=<interpoaltion method>
 
-lasb.generate_dsm(input_laz, epsg_code, dsm_resolution)
-lasb.generate_dtm(input_laz, epsg_code , dsm_resolution)
+Lasb.generate_dsm(input_laz, epsg_code, dsm_resolution,intermethod)
+Lasb.generate_dtm(input_laz, epsg_code, dsm_resolution,intermethod)
 lasb.generate_ndhm('dtm.tif', 'dsm.tif')
 
 img, profile = lasb.read_geotiff('ndhm.tif')
 lasb.DSM_Transform('dsm.tif')
 
 dem, _ = lasb.read_geotiff('dsm3857.tif')
 img_8bit = lasb.to_8bit(img)
```

### Comparing `LasBuildSeg-0.1.12/README.md` & `LasBuildSeg-0.1.13/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 ```python
 import LasBuildSeg as lasb
 import numpy as np
 
 input_laz = '<input>.laz'
 epsg_code = <epsg_code>
 dsm_resolution = <resolution>
+scale=<lazfilescale>
+method=<interpoaltion method>
 
-lasb.generate_dsm(input_laz, epsg_code, dsm_resolution)
-lasb.generate_dtm(input_laz, epsg_code , dsm_resolution)
+Lasb.generate_dsm(input_laz, epsg_code, dsm_resolution,intermethod)
+Lasb.generate_dtm(input_laz, epsg_code, dsm_resolution,intermethod)
 lasb.generate_ndhm('dtm.tif', 'dsm.tif')
 
 img, profile = lasb.read_geotiff('ndhm.tif')
 lasb.DSM_Transform('dsm.tif')
 
 dem, _ = lasb.read_geotiff('dsm3857.tif')
 img_8bit = lasb.to_8bit(img)
```

### Comparing `LasBuildSeg-0.1.12/Setup.py` & `LasBuildSeg-0.1.13/Setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     INSTALL_REQUIRES = []
 else:
     with open("requirements.txt") as f:
         INSTALL_REQUIRES = [line.strip() for line in f.readlines()]
         
 setup(
   name='LasBuildSeg',
-  version='0.1.12',
+  version='0.1.13',
   description='Building Footrprint Extraction from Aerial LiDAR data',
   long_description=long_description,
   long_description_content_type='text/markdown',  
   url='',  
   author='MertcanErdem',
   author_email='merak908@gmail.com',
   license='GNU General Public License v2.0',
```

