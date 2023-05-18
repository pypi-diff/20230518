# Comparing `tmp/pygdal-3.6.3.11.tar.gz` & `tmp/pygdal-3.6.4.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygdal-3.6.3.11.tar", last modified: Thu May 18 11:14:06 2023, max compression
+gzip compressed data, was "pygdal-3.6.4.11.tar", last modified: Thu May 18 10:15:03 2023, max compression
```

## Comparing `pygdal-3.6.3.11.tar` & `pygdal-3.6.4.11.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 jean      (1000) jean      (1000)        0 2023-05-18 11:14:06.989911 pygdal-3.6.3.11/
--rw-rw-r--   0 jean      (1000) jean      (1000)        5 2023-05-18 11:14:04.000000 pygdal-3.6.3.11/GDAL_VERSION
--rw-rw-r--   0 jean      (1000) jean      (1000)       75 2023-05-18 11:14:04.000000 pygdal-3.6.3.11/MANIFEST.in
--rw-rw-r--   0 jean      (1000) jean      (1000)     2698 2023-05-18 11:14:06.989911 pygdal-3.6.3.11/PKG-INFO
--rw-rw-r--   0 jean      (1000) jean      (1000)     1700 2023-05-18 11:14:04.000000 pygdal-3.6.3.11/README.rst
-drwxrwxr-x   0 jean      (1000) jean      (1000)        0 2023-05-18 11:14:06.989911 pygdal-3.6.3.11/extensions/
--rw-rw-r--   0 jean      (1000) jean      (1000)   240623 2023-05-18 11:14:04.000000 pygdal-3.6.3.11/extensions/gdal_array_wrap.cpp
--rw-rw-r--   0 jean      (1000) jean      (1000)  1698259 2023-05-18 11:14:04.000000 pygdal-3.6.3.11/extensions/gdal_wrap.cpp
--rw-rw-r--   0 jean      (1000) jean      (1000)   125229 2023-05-18 11:14:04.000000 pygdal-3.6.3.11/extensions/gdalconst_wrap.c
--rw-rw-r--   0 jean      (1000) jean      (1000)  1307054 2023-05-18 11:14:04.000000 pygdal-3.6.3.11/extensions/ogr_wrap.cpp
--rw-rw-r--   0 jean      (1000) jean      (1000)   725967 2023-05-18 11:14:04.000000 pygdal-3.6.3.11/extensions/osr_wrap.cpp
-drwxrwxr-x   0 jean      (1000) jean      (1000)        0 2023-05-18 11:14:06.985911 pygdal-3.6.3.11/osgeo/
--rw-rw-r--   0 jean      (1000) jean      (1000)     5418 2023-05-18 11:14:04.000000 pygdal-3.6.3.11/osgeo/__init__.py
--rw-rw-r--   0 jean      (1000) jean      (1000)   208954 2023-05-18 11:14:04.000000 pygdal-3.6.3.11/osgeo/gdal.py
--rw-rw-r--   0 jean      (1000) jean      (1000)    27755 2023-05-18 11:14:04.000000 pygdal-3.6.3.11/osgeo/gdal_array.py
--rw-rw-r--   0 jean      (1000) jean      (1000)    11844 2023-05-18 11:14:04.000000 pygdal-3.6.3.11/osgeo/gdalconst.py
--rw-rw-r--   0 jean      (1000) jean      (1000)      214 2023-05-18 11:14:04.000000 pygdal-3.6.3.11/osgeo/gdalnumeric.py
--rw-rw-r--   0 jean      (1000) jean      (1000)     9892 2023-05-18 11:14:04.000000 pygdal-3.6.3.11/osgeo/gnm.py
--rw-rw-r--   0 jean      (1000) jean      (1000)   221000 2023-05-18 11:14:04.000000 pygdal-3.6.3.11/osgeo/ogr.py
--rw-rw-r--   0 jean      (1000) jean      (1000)    55075 2023-05-18 11:14:04.000000 pygdal-3.6.3.11/osgeo/osr.py
--rw-rw-r--   0 jean      (1000) jean      (1000)      190 2023-05-18 11:14:04.000000 pygdal-3.6.3.11/osgeo/utils.py
-drwxrwxr-x   0 jean      (1000) jean      (1000)        0 2023-05-18 11:14:06.989911 pygdal-3.6.3.11/pygdal.egg-info/
--rw-rw-r--   0 jean      (1000) jean      (1000)     2698 2023-05-18 11:14:06.000000 pygdal-3.6.3.11/pygdal.egg-info/PKG-INFO
--rw-rw-r--   0 jean      (1000) jean      (1000)      518 2023-05-18 11:14:06.000000 pygdal-3.6.3.11/pygdal.egg-info/SOURCES.txt
--rw-rw-r--   0 jean      (1000) jean      (1000)        1 2023-05-18 11:14:06.000000 pygdal-3.6.3.11/pygdal.egg-info/dependency_links.txt
--rw-rw-r--   0 jean      (1000) jean      (1000)        1 2023-05-18 11:14:06.000000 pygdal-3.6.3.11/pygdal.egg-info/not-zip-safe
--rw-rw-r--   0 jean      (1000) jean      (1000)       13 2023-05-18 11:14:06.000000 pygdal-3.6.3.11/pygdal.egg-info/requires.txt
--rw-rw-r--   0 jean      (1000) jean      (1000)        6 2023-05-18 11:14:06.000000 pygdal-3.6.3.11/pygdal.egg-info/top_level.txt
--rw-rw-r--   0 jean      (1000) jean      (1000)       38 2023-05-18 11:14:06.989911 pygdal-3.6.3.11/setup.cfg
--rw-rw-r--   0 jean      (1000) jean      (1000)     7306 2023-05-18 11:14:04.000000 pygdal-3.6.3.11/setup.py
+drwxrwxr-x   0 jean      (1000) jean      (1000)        0 2023-05-18 10:15:03.100536 pygdal-3.6.4.11/
+-rw-rw-r--   0 jean      (1000) jean      (1000)        5 2023-05-18 10:15:00.000000 pygdal-3.6.4.11/GDAL_VERSION
+-rw-rw-r--   0 jean      (1000) jean      (1000)       75 2023-05-18 10:15:00.000000 pygdal-3.6.4.11/MANIFEST.in
+-rw-rw-r--   0 jean      (1000) jean      (1000)     2698 2023-05-18 10:15:03.100536 pygdal-3.6.4.11/PKG-INFO
+-rw-rw-r--   0 jean      (1000) jean      (1000)     1700 2023-05-18 10:15:00.000000 pygdal-3.6.4.11/README.rst
+drwxrwxr-x   0 jean      (1000) jean      (1000)        0 2023-05-18 10:15:03.096536 pygdal-3.6.4.11/extensions/
+-rw-rw-r--   0 jean      (1000) jean      (1000)   240623 2023-05-18 10:15:00.000000 pygdal-3.6.4.11/extensions/gdal_array_wrap.cpp
+-rw-rw-r--   0 jean      (1000) jean      (1000)  1698259 2023-05-18 10:15:00.000000 pygdal-3.6.4.11/extensions/gdal_wrap.cpp
+-rw-rw-r--   0 jean      (1000) jean      (1000)   125229 2023-05-18 10:15:00.000000 pygdal-3.6.4.11/extensions/gdalconst_wrap.c
+-rw-rw-r--   0 jean      (1000) jean      (1000)  1307054 2023-05-18 10:15:00.000000 pygdal-3.6.4.11/extensions/ogr_wrap.cpp
+-rw-rw-r--   0 jean      (1000) jean      (1000)   725967 2023-05-18 10:15:00.000000 pygdal-3.6.4.11/extensions/osr_wrap.cpp
+drwxrwxr-x   0 jean      (1000) jean      (1000)        0 2023-05-18 10:15:03.092536 pygdal-3.6.4.11/osgeo/
+-rw-rw-r--   0 jean      (1000) jean      (1000)     5418 2023-05-18 10:15:00.000000 pygdal-3.6.4.11/osgeo/__init__.py
+-rw-rw-r--   0 jean      (1000) jean      (1000)   208954 2023-05-18 10:15:00.000000 pygdal-3.6.4.11/osgeo/gdal.py
+-rw-rw-r--   0 jean      (1000) jean      (1000)    27755 2023-05-18 10:15:00.000000 pygdal-3.6.4.11/osgeo/gdal_array.py
+-rw-rw-r--   0 jean      (1000) jean      (1000)    11844 2023-05-18 10:15:00.000000 pygdal-3.6.4.11/osgeo/gdalconst.py
+-rw-rw-r--   0 jean      (1000) jean      (1000)      214 2023-05-18 10:15:00.000000 pygdal-3.6.4.11/osgeo/gdalnumeric.py
+-rw-rw-r--   0 jean      (1000) jean      (1000)     9892 2023-05-18 10:15:00.000000 pygdal-3.6.4.11/osgeo/gnm.py
+-rw-rw-r--   0 jean      (1000) jean      (1000)   221000 2023-05-18 10:15:00.000000 pygdal-3.6.4.11/osgeo/ogr.py
+-rw-rw-r--   0 jean      (1000) jean      (1000)    55075 2023-05-18 10:15:00.000000 pygdal-3.6.4.11/osgeo/osr.py
+-rw-rw-r--   0 jean      (1000) jean      (1000)      190 2023-05-18 10:15:00.000000 pygdal-3.6.4.11/osgeo/utils.py
+drwxrwxr-x   0 jean      (1000) jean      (1000)        0 2023-05-18 10:15:03.100536 pygdal-3.6.4.11/pygdal.egg-info/
+-rw-rw-r--   0 jean      (1000) jean      (1000)     2698 2023-05-18 10:15:02.000000 pygdal-3.6.4.11/pygdal.egg-info/PKG-INFO
+-rw-rw-r--   0 jean      (1000) jean      (1000)      518 2023-05-18 10:15:03.000000 pygdal-3.6.4.11/pygdal.egg-info/SOURCES.txt
+-rw-rw-r--   0 jean      (1000) jean      (1000)        1 2023-05-18 10:15:02.000000 pygdal-3.6.4.11/pygdal.egg-info/dependency_links.txt
+-rw-rw-r--   0 jean      (1000) jean      (1000)        1 2023-05-18 10:15:02.000000 pygdal-3.6.4.11/pygdal.egg-info/not-zip-safe
+-rw-rw-r--   0 jean      (1000) jean      (1000)       13 2023-05-18 10:15:02.000000 pygdal-3.6.4.11/pygdal.egg-info/requires.txt
+-rw-rw-r--   0 jean      (1000) jean      (1000)        6 2023-05-18 10:15:02.000000 pygdal-3.6.4.11/pygdal.egg-info/top_level.txt
+-rw-rw-r--   0 jean      (1000) jean      (1000)       38 2023-05-18 10:15:03.100536 pygdal-3.6.4.11/setup.cfg
+-rw-rw-r--   0 jean      (1000) jean      (1000)     7306 2023-05-18 10:15:00.000000 pygdal-3.6.4.11/setup.py
```

### Comparing `pygdal-3.6.3.11/PKG-INFO` & `pygdal-3.6.4.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygdal
-Version: 3.6.3.11
+Version: 3.6.4.11
 Summary: Virtualenv and setuptools friendly version of standard GDAL python bindings
 Home-page: https://github.com/nextgis/pygdal
 Author: Frank Warmerdam
 Author-email: warmerdam@pobox.com
 Maintainer: Aleksandr Dezhin
 Maintainer-email: me@dezhin.net
 License: MIT
```

### Comparing `pygdal-3.6.3.11/README.rst` & `pygdal-3.6.4.11/README.rst`

 * *Files identical despite different names*

### Comparing `pygdal-3.6.3.11/extensions/gdal_array_wrap.cpp` & `pygdal-3.6.4.11/extensions/gdal_array_wrap.cpp`

 * *Files identical despite different names*

### Comparing `pygdal-3.6.3.11/extensions/gdal_wrap.cpp` & `pygdal-3.6.4.11/extensions/gdal_wrap.cpp`

 * *Files identical despite different names*

### Comparing `pygdal-3.6.3.11/extensions/gdalconst_wrap.c` & `pygdal-3.6.4.11/extensions/gdalconst_wrap.c`

 * *Files identical despite different names*

### Comparing `pygdal-3.6.3.11/extensions/ogr_wrap.cpp` & `pygdal-3.6.4.11/extensions/ogr_wrap.cpp`

 * *Files identical despite different names*

### Comparing `pygdal-3.6.3.11/extensions/osr_wrap.cpp` & `pygdal-3.6.4.11/extensions/osr_wrap.cpp`

 * *Files identical despite different names*

### Comparing `pygdal-3.6.3.11/osgeo/__init__.py` & `pygdal-3.6.4.11/osgeo/__init__.py`

 * *Files identical despite different names*

### Comparing `pygdal-3.6.3.11/osgeo/gdal.py` & `pygdal-3.6.4.11/osgeo/gdal.py`

 * *Files identical despite different names*

### Comparing `pygdal-3.6.3.11/osgeo/gdal_array.py` & `pygdal-3.6.4.11/osgeo/gdal_array.py`

 * *Files identical despite different names*

### Comparing `pygdal-3.6.3.11/osgeo/gdalconst.py` & `pygdal-3.6.4.11/osgeo/gdalconst.py`

 * *Files identical despite different names*

### Comparing `pygdal-3.6.3.11/osgeo/gnm.py` & `pygdal-3.6.4.11/osgeo/gnm.py`

 * *Files identical despite different names*

### Comparing `pygdal-3.6.3.11/osgeo/ogr.py` & `pygdal-3.6.4.11/osgeo/ogr.py`

 * *Files identical despite different names*

### Comparing `pygdal-3.6.3.11/osgeo/osr.py` & `pygdal-3.6.4.11/osgeo/osr.py`

 * *Files identical despite different names*

### Comparing `pygdal-3.6.3.11/pygdal.egg-info/PKG-INFO` & `pygdal-3.6.4.11/pygdal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygdal
-Version: 3.6.3.11
+Version: 3.6.4.11
 Summary: Virtualenv and setuptools friendly version of standard GDAL python bindings
 Home-page: https://github.com/nextgis/pygdal
 Author: Frank Warmerdam
 Author-email: warmerdam@pobox.com
 Maintainer: Aleksandr Dezhin
 Maintainer-email: me@dezhin.net
 License: MIT
```

### Comparing `pygdal-3.6.3.11/pygdal.egg-info/SOURCES.txt` & `pygdal-3.6.4.11/pygdal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygdal-3.6.3.11/setup.py` & `pygdal-3.6.4.11/setup.py`

 * *Files identical despite different names*

