# Comparing `tmp/sardem-0.9.0.tar.gz` & `tmp/sardem-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sardem-0.9.0.tar", last modified: Thu Aug  4 19:02:35 2022, max compression
+gzip compressed data, was "sardem-0.9.1.tar", last modified: Tue Aug  9 20:33:11 2022, max compression
```

## Comparing `sardem-0.9.0.tar` & `sardem-0.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 19:02:35.667777 sardem-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-08-04 19:02:34.000000 sardem-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6832 2022-08-04 19:02:35.667777 sardem-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5070 2022-08-04 19:02:34.000000 sardem-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 19:02:35.663777 sardem-0.9.0/sardem/
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-08-04 19:02:34.000000 sardem-0.9.0/sardem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5074 2022-08-04 19:02:34.000000 sardem-0.9.0/sardem/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     5426 2022-08-04 19:02:34.000000 sardem-0.9.0/sardem/conversions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3784 2022-08-04 19:02:34.000000 sardem-0.9.0/sardem/cop_dem.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 19:02:35.667777 sardem-0.9.0/sardem/cython/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-04 19:02:34.000000 sardem-0.9.0/sardem/cython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7264 2022-08-04 19:02:34.000000 sardem-0.9.0/sardem/cython/upsample.c
--rw-r--r--   0 runner    (1001) docker     (121)   116617 2022-08-04 19:02:34.000000 sardem-0.9.0/sardem/cython/upsample_cy.c
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-08-04 19:02:34.000000 sardem-0.9.0/sardem/cython/upsample_cy.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      845 2022-08-04 19:02:34.000000 sardem-0.9.0/sardem/cython/upsample_cy.pyx
--rw-r--r--   0 runner    (1001) docker     (121)    16319 2022-08-04 19:02:34.000000 sardem-0.9.0/sardem/dem.py
--rw-r--r--   0 runner    (1001) docker     (121)    15486 2022-08-04 19:02:34.000000 sardem-0.9.0/sardem/download.py
--rw-r--r--   0 runner    (1001) docker     (121)     5539 2022-08-04 19:02:34.000000 sardem-0.9.0/sardem/loading.py
--rw-r--r--   0 runner    (1001) docker     (121)     8427 2022-08-04 19:02:34.000000 sardem-0.9.0/sardem/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 19:02:35.663777 sardem-0.9.0/sardem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6832 2022-08-04 19:02:35.000000 sardem-0.9.0/sardem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      520 2022-08-04 19:02:35.000000 sardem-0.9.0/sardem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-04 19:02:35.000000 sardem-0.9.0/sardem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-08-04 19:02:35.000000 sardem-0.9.0/sardem.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-04 19:02:35.000000 sardem-0.9.0/sardem.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-08-04 19:02:35.000000 sardem-0.9.0/sardem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-08-04 19:02:35.000000 sardem-0.9.0/sardem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-04 19:02:35.667777 sardem-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1353 2022-08-04 19:02:34.000000 sardem-0.9.0/setup.py
+drwxr-xr-x   0 staniewi   (503) staff       (20)        0 2022-08-09 20:33:11.052231 sardem-0.9.1/
+-rw-r--r--   0 staniewi   (503) staff       (20)      100 2022-06-21 18:21:37.000000 sardem-0.9.1/MANIFEST.in
+-rw-r--r--   0 staniewi   (503) staff       (20)     5800 2022-08-09 20:33:11.052059 sardem-0.9.1/PKG-INFO
+-rw-r--r--   0 staniewi   (503) staff       (20)     5070 2022-06-21 18:21:37.000000 sardem-0.9.1/README.md
+drwxr-xr-x   0 staniewi   (503) staff       (20)        0 2022-08-09 20:33:11.048374 sardem-0.9.1/sardem/
+-rw-r--r--   0 staniewi   (503) staff       (20)       62 2022-06-21 18:21:37.000000 sardem-0.9.1/sardem/__init__.py
+-rw-r--r--   0 staniewi   (503) staff       (20)     5074 2022-08-04 19:00:46.000000 sardem-0.9.1/sardem/cli.py
+-rw-r--r--   0 staniewi   (503) staff       (20)     5426 2022-08-04 19:00:46.000000 sardem-0.9.1/sardem/conversions.py
+-rw-r--r--   0 staniewi   (503) staff       (20)     4803 2022-08-05 15:39:06.000000 sardem-0.9.1/sardem/cop_dem.py
+drwxr-xr-x   0 staniewi   (503) staff       (20)        0 2022-08-09 20:33:11.051640 sardem-0.9.1/sardem/cython/
+-rw-r--r--   0 staniewi   (503) staff       (20)        0 2022-06-21 18:21:37.000000 sardem-0.9.1/sardem/cython/__init__.py
+-rw-r--r--   0 staniewi   (503) staff       (20)     7264 2022-06-21 18:21:37.000000 sardem-0.9.1/sardem/cython/upsample.c
+-rw-r--r--   0 staniewi   (503) staff       (20)   116617 2022-06-21 18:21:37.000000 sardem-0.9.1/sardem/cython/upsample_cy.c
+-rw-r--r--   0 staniewi   (503) staff       (20)      241 2022-06-21 18:21:37.000000 sardem-0.9.1/sardem/cython/upsample_cy.pxd
+-rw-r--r--   0 staniewi   (503) staff       (20)      845 2022-06-21 18:21:37.000000 sardem-0.9.1/sardem/cython/upsample_cy.pyx
+-rw-r--r--   0 staniewi   (503) staff       (20)    16319 2022-08-04 19:00:46.000000 sardem-0.9.1/sardem/dem.py
+-rw-r--r--   0 staniewi   (503) staff       (20)    15486 2022-08-04 19:00:46.000000 sardem-0.9.1/sardem/download.py
+-rw-r--r--   0 staniewi   (503) staff       (20)     5539 2022-08-04 16:44:08.000000 sardem-0.9.1/sardem/loading.py
+-rw-r--r--   0 staniewi   (503) staff       (20)     8427 2022-08-04 19:00:46.000000 sardem-0.9.1/sardem/utils.py
+drwxr-xr-x   0 staniewi   (503) staff       (20)        0 2022-08-09 20:33:11.049693 sardem-0.9.1/sardem.egg-info/
+-rw-r--r--   0 staniewi   (503) staff       (20)     5800 2022-08-09 20:33:10.000000 sardem-0.9.1/sardem.egg-info/PKG-INFO
+-rw-r--r--   0 staniewi   (503) staff       (20)      520 2022-08-09 20:33:11.000000 sardem-0.9.1/sardem.egg-info/SOURCES.txt
+-rw-r--r--   0 staniewi   (503) staff       (20)        1 2022-08-09 20:33:10.000000 sardem-0.9.1/sardem.egg-info/dependency_links.txt
+-rw-r--r--   0 staniewi   (503) staff       (20)       42 2022-08-09 20:33:10.000000 sardem-0.9.1/sardem.egg-info/entry_points.txt
+-rw-r--r--   0 staniewi   (503) staff       (20)        1 2022-06-21 18:21:43.000000 sardem-0.9.1/sardem.egg-info/not-zip-safe
+-rw-r--r--   0 staniewi   (503) staff       (20)       15 2022-08-09 20:33:10.000000 sardem-0.9.1/sardem.egg-info/requires.txt
+-rw-r--r--   0 staniewi   (503) staff       (20)        7 2022-08-09 20:33:10.000000 sardem-0.9.1/sardem.egg-info/top_level.txt
+-rw-r--r--   0 staniewi   (503) staff       (20)       38 2022-08-09 20:33:11.052287 sardem-0.9.1/setup.cfg
+-rw-r--r--   0 staniewi   (503) staff       (20)     1353 2022-08-04 19:05:21.000000 sardem-0.9.1/setup.py
```

### Comparing `sardem-0.9.0/PKG-INFO` & `sardem-0.9.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,144 +1,142 @@
 Metadata-Version: 2.1
 Name: sardem
-Version: 0.9.0
+Version: 0.9.1
 Summary: Create upsampled DEMs for InSAR processing
 Home-page: https://github.com/scottstanie/sardem
 Author: Scott Staniewicz
 Author-email: scott.stanie@gmail.com
-License: UNKNOWN
-Description: 
-        # DEM creator
-        
-        Tool for making Digital Elevation Maps (DEMs) in binary data format (16-bit integers, little endian) for use in Interferometric SAR (InSAR) processing
-        
-        `sardem` creates a cropped (and possibly upsampled) digital elevation map:
-        
-        ```bash
-        usage: sardem [-h] [--bbox left bottom right top] [--geojson GEOJSON] [--xrate XRATE] [--yrate YRATE] [--output OUTPUT] [--data-source {NASA,NASA_WATER,AWS}]
-                      [--convert-to-wgs84]
-                      [left_lon] [top_lat] [dlon] [dlat]
-        ```
-        
-        ## Setup and installation
-        
-        ```bash
-        pip install sardem
-        ```
-        This creates the command line executable `sardem`
-        
-        Alternatively, you can clone to build/install:
-        
-        ```bash
-        git clone https://github.com/scottstanie/sardem
-        cd sardem
-        make
-        ```
-        which will run `pip install --upgrade .` and create the command line script.
-        
-        
-        If you use `virtualenv`
-        ```bash
-        # Optional for using virtualenv
-        virtualenv ~/envs/sardem && source ~/envs/sardem/bin/activate  # Or wherever you store your virtual envs
-        # Or if you have virtualenv wrapper: mkvirtualenv sardem
-        pip install sardem
-        ```
-        
-        
-        ## Command Line Interface
-        
-        The full options for the command line tool in `sardem/cli.py` can be found using
-        
-        ```
-        $ sardem --help
-        usage: sardem [-h] [--bbox left bottom right top] [--geojson GEOJSON] [--xrate XRATE] [--yrate YRATE] [--output OUTPUT] [--data-source {NASA,NASA_WATER,AWS}]
-                      [--convert-to-wgs84]
-                      [left_lon] [top_lat] [dlon] [dlat]
-        
-        Stiches SRTM .hgt files to make (upsampled) DEM
-        
-            Pick a lat/lon bounding box for a DEM, and it will download
-            the necessary SRTM1 tiles, stitch together, then upsample.
-        
-            Usage Examples:
-                sardem --bbox -156 18.8 -154.7 20.3  # bounding box: left  bottom  right top
-                sardem -156.0 20.2 1 2 --xrate 2 --yrate 2  # Makes a box 1 degree wide, 2 deg high
-                sardem --geojson dem_area.geojson -x 11 -y 3
-                sardem -156.0 20.2 0.5 0.5 -r 10 --data-source NASA_WATER -o my_watermask.wbd # Water mask
-        
-            Default out is elevation.dem for the final upsampled DEM.
-            Also creates elevation.dem.rsc with start lat/lon, stride, and other info.
-        
-        positional arguments:
-          left_lon              Left (western) most longitude of DEM box (degrees, west=negative)
-          top_lat               Top (northern) most latitude of DEM box (degrees)
-          dlon                  Width of DEM box (degrees)
-          dlat                  Height of DEM box (degrees)
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          --bbox left bottom right top
-                                Bounding box of area of interest  (e.g. --bbox -106.1 30.1 -103.1 33.1 ).
-          --geojson GEOJSON, -g GEOJSON
-                                Alternate to corner/dlon/dlat box specification:
-                                File containing the geojson object for DEM bounds
-          --xrate XRATE, -x XRATE
-                                Rate in x dir to upsample DEM (default=1, no upsampling)
-          --yrate YRATE, -y YRATE
-                                Rate in y dir to upsample DEM (default=1, no upsampling)
-          --output OUTPUT, -o OUTPUT
-                                Name of output dem file (default=elevation.dem for DEM, watermask.wbd for water mask)
-          --data-source {NASA,NASA_WATER,AWS}, -d {NASA,NASA_WATER,AWS}
-                                Source of SRTM data (default NASA). See README for more.
-          --convert-to-wgs84, -c
-                                Convert the DEM heights from geoid heights above EGM96 to heights above WGS84 ellipsoid
-        ```
-        
-        The code used for bilinear interpolation in the upsampling routine is in `cython/upsample.c`, and is wrapped in [cython](http://docs.cython.org/en/latest/) to allow easier installation and ability to call the function from Python.
-        The installation is handled through `pip install`, or by running `make build`.
-        
-        Functions for working with digital elevation maps (DEMs) are mostly contained in the `Downloader` and `Stitcher` classes within `sardem/dem.py` and `sardem/download.py`.
-        
-        
-        ### NASA SRTM Data access
-        
-        The default datasource is NASA's SRTM version 3 global 1 degree data.
-        See https://lpdaac.usgs.gov/dataset_discovery/measures/measures_products_table/srtmgl3s_v003 .
-        The data is valid outside of artic regions (-60 to 60 degrees latitude), and is zeros over open ocean.
-        
-        This data requires a username and password from here:
-        https://urs.earthdata.nasa.gov/users/new
-        
-        You will be prompted for a username and password when running with NASA data.
-        It will save into your ~/.netrc file for future use, which means you will not have to enter a username and password any subsequent times.
-        The entry will look like this:
-        
-        ```
-        machine urs.earthdata.nasa.gov
-            login USERNAME
-            password PASSWORD
-        ```
-        
-        If you want to avoid this entirely, you can [use Mapzen's data hosted on AWS](https://registry.opendata.aws/terrain-tiles/) by specifying
-        ```bash
-        sardem 156.0 20.0 .5 0.5 --data-source AWS
-        ```
-        
-        `--data-source NASA` is the default.
-        
-        Mapzen combines SRTM data with other sources, so the .hgt files will be slightly different (but often not noticeable)
-        
-        Warning: Mapzen notes that they are discontinuing some services, which is why NASA is the default.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: C
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Description-Content-Type: text/markdown
+
+
+# DEM creator
+
+Tool for making Digital Elevation Maps (DEMs) in binary data format (16-bit integers, little endian) for use in Interferometric SAR (InSAR) processing
+
+`sardem` creates a cropped (and possibly upsampled) digital elevation map:
+
+```bash
+usage: sardem [-h] [--bbox left bottom right top] [--geojson GEOJSON] [--xrate XRATE] [--yrate YRATE] [--output OUTPUT] [--data-source {NASA,NASA_WATER,AWS}]
+              [--convert-to-wgs84]
+              [left_lon] [top_lat] [dlon] [dlat]
+```
+
+## Setup and installation
+
+```bash
+pip install sardem
+```
+This creates the command line executable `sardem`
+
+Alternatively, you can clone to build/install:
+
+```bash
+git clone https://github.com/scottstanie/sardem
+cd sardem
+make
+```
+which will run `pip install --upgrade .` and create the command line script.
+
+
+If you use `virtualenv`
+```bash
+# Optional for using virtualenv
+virtualenv ~/envs/sardem && source ~/envs/sardem/bin/activate  # Or wherever you store your virtual envs
+# Or if you have virtualenv wrapper: mkvirtualenv sardem
+pip install sardem
+```
+
+
+## Command Line Interface
+
+The full options for the command line tool in `sardem/cli.py` can be found using
+
+```
+$ sardem --help
+usage: sardem [-h] [--bbox left bottom right top] [--geojson GEOJSON] [--xrate XRATE] [--yrate YRATE] [--output OUTPUT] [--data-source {NASA,NASA_WATER,AWS}]
+              [--convert-to-wgs84]
+              [left_lon] [top_lat] [dlon] [dlat]
+
+Stiches SRTM .hgt files to make (upsampled) DEM
+
+    Pick a lat/lon bounding box for a DEM, and it will download
+    the necessary SRTM1 tiles, stitch together, then upsample.
+
+    Usage Examples:
+        sardem --bbox -156 18.8 -154.7 20.3  # bounding box: left  bottom  right top
+        sardem -156.0 20.2 1 2 --xrate 2 --yrate 2  # Makes a box 1 degree wide, 2 deg high
+        sardem --geojson dem_area.geojson -x 11 -y 3
+        sardem -156.0 20.2 0.5 0.5 -r 10 --data-source NASA_WATER -o my_watermask.wbd # Water mask
+
+    Default out is elevation.dem for the final upsampled DEM.
+    Also creates elevation.dem.rsc with start lat/lon, stride, and other info.
+
+positional arguments:
+  left_lon              Left (western) most longitude of DEM box (degrees, west=negative)
+  top_lat               Top (northern) most latitude of DEM box (degrees)
+  dlon                  Width of DEM box (degrees)
+  dlat                  Height of DEM box (degrees)
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --bbox left bottom right top
+                        Bounding box of area of interest  (e.g. --bbox -106.1 30.1 -103.1 33.1 ).
+  --geojson GEOJSON, -g GEOJSON
+                        Alternate to corner/dlon/dlat box specification:
+                        File containing the geojson object for DEM bounds
+  --xrate XRATE, -x XRATE
+                        Rate in x dir to upsample DEM (default=1, no upsampling)
+  --yrate YRATE, -y YRATE
+                        Rate in y dir to upsample DEM (default=1, no upsampling)
+  --output OUTPUT, -o OUTPUT
+                        Name of output dem file (default=elevation.dem for DEM, watermask.wbd for water mask)
+  --data-source {NASA,NASA_WATER,AWS}, -d {NASA,NASA_WATER,AWS}
+                        Source of SRTM data (default NASA). See README for more.
+  --convert-to-wgs84, -c
+                        Convert the DEM heights from geoid heights above EGM96 to heights above WGS84 ellipsoid
+```
+
+The code used for bilinear interpolation in the upsampling routine is in `cython/upsample.c`, and is wrapped in [cython](http://docs.cython.org/en/latest/) to allow easier installation and ability to call the function from Python.
+The installation is handled through `pip install`, or by running `make build`.
+
+Functions for working with digital elevation maps (DEMs) are mostly contained in the `Downloader` and `Stitcher` classes within `sardem/dem.py` and `sardem/download.py`.
+
+
+### NASA SRTM Data access
+
+The default datasource is NASA's SRTM version 3 global 1 degree data.
+See https://lpdaac.usgs.gov/dataset_discovery/measures/measures_products_table/srtmgl3s_v003 .
+The data is valid outside of artic regions (-60 to 60 degrees latitude), and is zeros over open ocean.
+
+This data requires a username and password from here:
+https://urs.earthdata.nasa.gov/users/new
+
+You will be prompted for a username and password when running with NASA data.
+It will save into your ~/.netrc file for future use, which means you will not have to enter a username and password any subsequent times.
+The entry will look like this:
+
+```
+machine urs.earthdata.nasa.gov
+    login USERNAME
+    password PASSWORD
+```
+
+If you want to avoid this entirely, you can [use Mapzen's data hosted on AWS](https://registry.opendata.aws/terrain-tiles/) by specifying
+```bash
+sardem 156.0 20.0 .5 0.5 --data-source AWS
+```
+
+`--data-source NASA` is the default.
+
+Mapzen combines SRTM data with other sources, so the .hgt files will be slightly different (but often not noticeable)
+
+Warning: Mapzen notes that they are discontinuing some services, which is why NASA is the default.
```

### Comparing `sardem-0.9.0/README.md` & `sardem-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `sardem-0.9.0/sardem/cli.py` & `sardem-0.9.1/sardem/cli.py`

 * *Files identical despite different names*

### Comparing `sardem-0.9.0/sardem/conversions.py` & `sardem-0.9.1/sardem/conversions.py`

 * *Files identical despite different names*

### Comparing `sardem-0.9.0/sardem/cython/upsample.c` & `sardem-0.9.1/sardem/cython/upsample.c`

 * *Files identical despite different names*

### Comparing `sardem-0.9.0/sardem/cython/upsample_cy.c` & `sardem-0.9.1/sardem/cython/upsample_cy.c`

 * *Files identical despite different names*

### Comparing `sardem-0.9.0/sardem/cython/upsample_cy.pyx` & `sardem-0.9.1/sardem/cython/upsample_cy.pyx`

 * *Files identical despite different names*

### Comparing `sardem-0.9.0/sardem/dem.py` & `sardem-0.9.1/sardem/dem.py`

 * *Files identical despite different names*

### Comparing `sardem-0.9.0/sardem/download.py` & `sardem-0.9.1/sardem/download.py`

 * *Files identical despite different names*

### Comparing `sardem-0.9.0/sardem/loading.py` & `sardem-0.9.1/sardem/loading.py`

 * *Files identical despite different names*

### Comparing `sardem-0.9.0/sardem/utils.py` & `sardem-0.9.1/sardem/utils.py`

 * *Files identical despite different names*

### Comparing `sardem-0.9.0/sardem.egg-info/PKG-INFO` & `sardem-0.9.1/sardem.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,144 +1,142 @@
 Metadata-Version: 2.1
 Name: sardem
-Version: 0.9.0
+Version: 0.9.1
 Summary: Create upsampled DEMs for InSAR processing
 Home-page: https://github.com/scottstanie/sardem
 Author: Scott Staniewicz
 Author-email: scott.stanie@gmail.com
-License: UNKNOWN
-Description: 
-        # DEM creator
-        
-        Tool for making Digital Elevation Maps (DEMs) in binary data format (16-bit integers, little endian) for use in Interferometric SAR (InSAR) processing
-        
-        `sardem` creates a cropped (and possibly upsampled) digital elevation map:
-        
-        ```bash
-        usage: sardem [-h] [--bbox left bottom right top] [--geojson GEOJSON] [--xrate XRATE] [--yrate YRATE] [--output OUTPUT] [--data-source {NASA,NASA_WATER,AWS}]
-                      [--convert-to-wgs84]
-                      [left_lon] [top_lat] [dlon] [dlat]
-        ```
-        
-        ## Setup and installation
-        
-        ```bash
-        pip install sardem
-        ```
-        This creates the command line executable `sardem`
-        
-        Alternatively, you can clone to build/install:
-        
-        ```bash
-        git clone https://github.com/scottstanie/sardem
-        cd sardem
-        make
-        ```
-        which will run `pip install --upgrade .` and create the command line script.
-        
-        
-        If you use `virtualenv`
-        ```bash
-        # Optional for using virtualenv
-        virtualenv ~/envs/sardem && source ~/envs/sardem/bin/activate  # Or wherever you store your virtual envs
-        # Or if you have virtualenv wrapper: mkvirtualenv sardem
-        pip install sardem
-        ```
-        
-        
-        ## Command Line Interface
-        
-        The full options for the command line tool in `sardem/cli.py` can be found using
-        
-        ```
-        $ sardem --help
-        usage: sardem [-h] [--bbox left bottom right top] [--geojson GEOJSON] [--xrate XRATE] [--yrate YRATE] [--output OUTPUT] [--data-source {NASA,NASA_WATER,AWS}]
-                      [--convert-to-wgs84]
-                      [left_lon] [top_lat] [dlon] [dlat]
-        
-        Stiches SRTM .hgt files to make (upsampled) DEM
-        
-            Pick a lat/lon bounding box for a DEM, and it will download
-            the necessary SRTM1 tiles, stitch together, then upsample.
-        
-            Usage Examples:
-                sardem --bbox -156 18.8 -154.7 20.3  # bounding box: left  bottom  right top
-                sardem -156.0 20.2 1 2 --xrate 2 --yrate 2  # Makes a box 1 degree wide, 2 deg high
-                sardem --geojson dem_area.geojson -x 11 -y 3
-                sardem -156.0 20.2 0.5 0.5 -r 10 --data-source NASA_WATER -o my_watermask.wbd # Water mask
-        
-            Default out is elevation.dem for the final upsampled DEM.
-            Also creates elevation.dem.rsc with start lat/lon, stride, and other info.
-        
-        positional arguments:
-          left_lon              Left (western) most longitude of DEM box (degrees, west=negative)
-          top_lat               Top (northern) most latitude of DEM box (degrees)
-          dlon                  Width of DEM box (degrees)
-          dlat                  Height of DEM box (degrees)
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          --bbox left bottom right top
-                                Bounding box of area of interest  (e.g. --bbox -106.1 30.1 -103.1 33.1 ).
-          --geojson GEOJSON, -g GEOJSON
-                                Alternate to corner/dlon/dlat box specification:
-                                File containing the geojson object for DEM bounds
-          --xrate XRATE, -x XRATE
-                                Rate in x dir to upsample DEM (default=1, no upsampling)
-          --yrate YRATE, -y YRATE
-                                Rate in y dir to upsample DEM (default=1, no upsampling)
-          --output OUTPUT, -o OUTPUT
-                                Name of output dem file (default=elevation.dem for DEM, watermask.wbd for water mask)
-          --data-source {NASA,NASA_WATER,AWS}, -d {NASA,NASA_WATER,AWS}
-                                Source of SRTM data (default NASA). See README for more.
-          --convert-to-wgs84, -c
-                                Convert the DEM heights from geoid heights above EGM96 to heights above WGS84 ellipsoid
-        ```
-        
-        The code used for bilinear interpolation in the upsampling routine is in `cython/upsample.c`, and is wrapped in [cython](http://docs.cython.org/en/latest/) to allow easier installation and ability to call the function from Python.
-        The installation is handled through `pip install`, or by running `make build`.
-        
-        Functions for working with digital elevation maps (DEMs) are mostly contained in the `Downloader` and `Stitcher` classes within `sardem/dem.py` and `sardem/download.py`.
-        
-        
-        ### NASA SRTM Data access
-        
-        The default datasource is NASA's SRTM version 3 global 1 degree data.
-        See https://lpdaac.usgs.gov/dataset_discovery/measures/measures_products_table/srtmgl3s_v003 .
-        The data is valid outside of artic regions (-60 to 60 degrees latitude), and is zeros over open ocean.
-        
-        This data requires a username and password from here:
-        https://urs.earthdata.nasa.gov/users/new
-        
-        You will be prompted for a username and password when running with NASA data.
-        It will save into your ~/.netrc file for future use, which means you will not have to enter a username and password any subsequent times.
-        The entry will look like this:
-        
-        ```
-        machine urs.earthdata.nasa.gov
-            login USERNAME
-            password PASSWORD
-        ```
-        
-        If you want to avoid this entirely, you can [use Mapzen's data hosted on AWS](https://registry.opendata.aws/terrain-tiles/) by specifying
-        ```bash
-        sardem 156.0 20.0 .5 0.5 --data-source AWS
-        ```
-        
-        `--data-source NASA` is the default.
-        
-        Mapzen combines SRTM data with other sources, so the .hgt files will be slightly different (but often not noticeable)
-        
-        Warning: Mapzen notes that they are discontinuing some services, which is why NASA is the default.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: C
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Description-Content-Type: text/markdown
+
+
+# DEM creator
+
+Tool for making Digital Elevation Maps (DEMs) in binary data format (16-bit integers, little endian) for use in Interferometric SAR (InSAR) processing
+
+`sardem` creates a cropped (and possibly upsampled) digital elevation map:
+
+```bash
+usage: sardem [-h] [--bbox left bottom right top] [--geojson GEOJSON] [--xrate XRATE] [--yrate YRATE] [--output OUTPUT] [--data-source {NASA,NASA_WATER,AWS}]
+              [--convert-to-wgs84]
+              [left_lon] [top_lat] [dlon] [dlat]
+```
+
+## Setup and installation
+
+```bash
+pip install sardem
+```
+This creates the command line executable `sardem`
+
+Alternatively, you can clone to build/install:
+
+```bash
+git clone https://github.com/scottstanie/sardem
+cd sardem
+make
+```
+which will run `pip install --upgrade .` and create the command line script.
+
+
+If you use `virtualenv`
+```bash
+# Optional for using virtualenv
+virtualenv ~/envs/sardem && source ~/envs/sardem/bin/activate  # Or wherever you store your virtual envs
+# Or if you have virtualenv wrapper: mkvirtualenv sardem
+pip install sardem
+```
+
+
+## Command Line Interface
+
+The full options for the command line tool in `sardem/cli.py` can be found using
+
+```
+$ sardem --help
+usage: sardem [-h] [--bbox left bottom right top] [--geojson GEOJSON] [--xrate XRATE] [--yrate YRATE] [--output OUTPUT] [--data-source {NASA,NASA_WATER,AWS}]
+              [--convert-to-wgs84]
+              [left_lon] [top_lat] [dlon] [dlat]
+
+Stiches SRTM .hgt files to make (upsampled) DEM
+
+    Pick a lat/lon bounding box for a DEM, and it will download
+    the necessary SRTM1 tiles, stitch together, then upsample.
+
+    Usage Examples:
+        sardem --bbox -156 18.8 -154.7 20.3  # bounding box: left  bottom  right top
+        sardem -156.0 20.2 1 2 --xrate 2 --yrate 2  # Makes a box 1 degree wide, 2 deg high
+        sardem --geojson dem_area.geojson -x 11 -y 3
+        sardem -156.0 20.2 0.5 0.5 -r 10 --data-source NASA_WATER -o my_watermask.wbd # Water mask
+
+    Default out is elevation.dem for the final upsampled DEM.
+    Also creates elevation.dem.rsc with start lat/lon, stride, and other info.
+
+positional arguments:
+  left_lon              Left (western) most longitude of DEM box (degrees, west=negative)
+  top_lat               Top (northern) most latitude of DEM box (degrees)
+  dlon                  Width of DEM box (degrees)
+  dlat                  Height of DEM box (degrees)
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --bbox left bottom right top
+                        Bounding box of area of interest  (e.g. --bbox -106.1 30.1 -103.1 33.1 ).
+  --geojson GEOJSON, -g GEOJSON
+                        Alternate to corner/dlon/dlat box specification:
+                        File containing the geojson object for DEM bounds
+  --xrate XRATE, -x XRATE
+                        Rate in x dir to upsample DEM (default=1, no upsampling)
+  --yrate YRATE, -y YRATE
+                        Rate in y dir to upsample DEM (default=1, no upsampling)
+  --output OUTPUT, -o OUTPUT
+                        Name of output dem file (default=elevation.dem for DEM, watermask.wbd for water mask)
+  --data-source {NASA,NASA_WATER,AWS}, -d {NASA,NASA_WATER,AWS}
+                        Source of SRTM data (default NASA). See README for more.
+  --convert-to-wgs84, -c
+                        Convert the DEM heights from geoid heights above EGM96 to heights above WGS84 ellipsoid
+```
+
+The code used for bilinear interpolation in the upsampling routine is in `cython/upsample.c`, and is wrapped in [cython](http://docs.cython.org/en/latest/) to allow easier installation and ability to call the function from Python.
+The installation is handled through `pip install`, or by running `make build`.
+
+Functions for working with digital elevation maps (DEMs) are mostly contained in the `Downloader` and `Stitcher` classes within `sardem/dem.py` and `sardem/download.py`.
+
+
+### NASA SRTM Data access
+
+The default datasource is NASA's SRTM version 3 global 1 degree data.
+See https://lpdaac.usgs.gov/dataset_discovery/measures/measures_products_table/srtmgl3s_v003 .
+The data is valid outside of artic regions (-60 to 60 degrees latitude), and is zeros over open ocean.
+
+This data requires a username and password from here:
+https://urs.earthdata.nasa.gov/users/new
+
+You will be prompted for a username and password when running with NASA data.
+It will save into your ~/.netrc file for future use, which means you will not have to enter a username and password any subsequent times.
+The entry will look like this:
+
+```
+machine urs.earthdata.nasa.gov
+    login USERNAME
+    password PASSWORD
+```
+
+If you want to avoid this entirely, you can [use Mapzen's data hosted on AWS](https://registry.opendata.aws/terrain-tiles/) by specifying
+```bash
+sardem 156.0 20.0 .5 0.5 --data-source AWS
+```
+
+`--data-source NASA` is the default.
+
+Mapzen combines SRTM data with other sources, so the .hgt files will be slightly different (but often not noticeable)
+
+Warning: Mapzen notes that they are discontinuing some services, which is why NASA is the default.
```

### Comparing `sardem-0.9.0/sardem.egg-info/SOURCES.txt` & `sardem-0.9.1/sardem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sardem-0.9.0/setup.py` & `sardem-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sardem",
-    version="0.9.0",
+    version="0.9.1",
     author="Scott Staniewicz",
     author_email="scott.stanie@gmail.com",
     description="Create upsampled DEMs for InSAR processing",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/scottstanie/sardem",
     packages=setuptools.find_packages(),
```

