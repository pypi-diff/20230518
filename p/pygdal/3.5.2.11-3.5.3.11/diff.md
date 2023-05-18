# Comparing `tmp/pygdal-3.5.2.11.tar.gz` & `tmp/pygdal-3.5.3.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygdal-3.5.2.11.tar", last modified: Thu May 18 09:49:53 2023, max compression
+gzip compressed data, was "pygdal-3.5.3.11.tar", last modified: Thu May 18 09:50:15 2023, max compression
```

## Comparing `pygdal-3.5.2.11.tar` & `pygdal-3.5.3.11.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 jean      (1000) jean      (1000)        0 2023-05-18 09:49:53.706830 pygdal-3.5.2.11/
--rw-rw-r--   0 jean      (1000) jean      (1000)        6 2023-05-18 09:49:39.000000 pygdal-3.5.2.11/GDAL_VERSION
--rw-rw-r--   0 jean      (1000) jean      (1000)       75 2023-05-18 09:49:39.000000 pygdal-3.5.2.11/MANIFEST.in
--rw-rw-r--   0 jean      (1000) jean      (1000)     2698 2023-05-18 09:49:53.706830 pygdal-3.5.2.11/PKG-INFO
--rw-rw-r--   0 jean      (1000) jean      (1000)     1700 2023-05-18 09:49:39.000000 pygdal-3.5.2.11/README.rst
-drwxrwxr-x   0 jean      (1000) jean      (1000)        0 2023-05-18 09:49:53.706830 pygdal-3.5.2.11/extensions/
--rw-rw-r--   0 jean      (1000) jean      (1000)   210330 2023-05-18 09:49:39.000000 pygdal-3.5.2.11/extensions/gdal_array_wrap.cpp
--rw-rw-r--   0 jean      (1000) jean      (1000)  1619015 2023-05-18 09:49:39.000000 pygdal-3.5.2.11/extensions/gdal_wrap.cpp
--rw-rw-r--   0 jean      (1000) jean      (1000)   122491 2023-05-18 09:49:39.000000 pygdal-3.5.2.11/extensions/gdalconst_wrap.c
--rw-rw-r--   0 jean      (1000) jean      (1000)  1326479 2023-05-18 09:49:39.000000 pygdal-3.5.2.11/extensions/ogr_wrap.cpp
--rw-rw-r--   0 jean      (1000) jean      (1000)   721424 2023-05-18 09:49:39.000000 pygdal-3.5.2.11/extensions/osr_wrap.cpp
-drwxrwxr-x   0 jean      (1000) jean      (1000)        0 2023-05-18 09:49:53.702830 pygdal-3.5.2.11/osgeo/
--rw-rw-r--   0 jean      (1000) jean      (1000)     5418 2023-05-18 09:49:39.000000 pygdal-3.5.2.11/osgeo/__init__.py
--rw-rw-r--   0 jean      (1000) jean      (1000)   194379 2023-05-18 09:49:39.000000 pygdal-3.5.2.11/osgeo/gdal.py
--rw-rw-r--   0 jean      (1000) jean      (1000)    26574 2023-05-18 09:49:39.000000 pygdal-3.5.2.11/osgeo/gdal_array.py
--rw-rw-r--   0 jean      (1000) jean      (1000)    10262 2023-05-18 09:49:39.000000 pygdal-3.5.2.11/osgeo/gdalconst.py
--rw-rw-r--   0 jean      (1000) jean      (1000)      214 2023-05-18 09:49:39.000000 pygdal-3.5.2.11/osgeo/gdalnumeric.py
--rw-rw-r--   0 jean      (1000) jean      (1000)     9376 2023-05-18 09:49:39.000000 pygdal-3.5.2.11/osgeo/gnm.py
--rw-rw-r--   0 jean      (1000) jean      (1000)   262590 2023-05-18 09:49:39.000000 pygdal-3.5.2.11/osgeo/ogr.py
--rw-rw-r--   0 jean      (1000) jean      (1000)    52387 2023-05-18 09:49:39.000000 pygdal-3.5.2.11/osgeo/osr.py
--rw-rw-r--   0 jean      (1000) jean      (1000)      190 2023-05-18 09:49:39.000000 pygdal-3.5.2.11/osgeo/utils.py
-drwxrwxr-x   0 jean      (1000) jean      (1000)        0 2023-05-18 09:49:53.706830 pygdal-3.5.2.11/pygdal.egg-info/
--rw-rw-r--   0 jean      (1000) jean      (1000)     2698 2023-05-18 09:49:53.000000 pygdal-3.5.2.11/pygdal.egg-info/PKG-INFO
--rw-rw-r--   0 jean      (1000) jean      (1000)      518 2023-05-18 09:49:53.000000 pygdal-3.5.2.11/pygdal.egg-info/SOURCES.txt
--rw-rw-r--   0 jean      (1000) jean      (1000)        1 2023-05-18 09:49:53.000000 pygdal-3.5.2.11/pygdal.egg-info/dependency_links.txt
--rw-rw-r--   0 jean      (1000) jean      (1000)        1 2023-05-18 09:49:53.000000 pygdal-3.5.2.11/pygdal.egg-info/not-zip-safe
--rw-rw-r--   0 jean      (1000) jean      (1000)       13 2023-05-18 09:49:53.000000 pygdal-3.5.2.11/pygdal.egg-info/requires.txt
--rw-rw-r--   0 jean      (1000) jean      (1000)        6 2023-05-18 09:49:53.000000 pygdal-3.5.2.11/pygdal.egg-info/top_level.txt
--rw-rw-r--   0 jean      (1000) jean      (1000)       38 2023-05-18 09:49:53.706830 pygdal-3.5.2.11/setup.cfg
--rw-rw-r--   0 jean      (1000) jean      (1000)     7306 2023-05-18 09:49:39.000000 pygdal-3.5.2.11/setup.py
+drwxrwxr-x   0 jean      (1000) jean      (1000)        0 2023-05-18 09:50:15.151008 pygdal-3.5.3.11/
+-rw-rw-r--   0 jean      (1000) jean      (1000)        6 2023-05-18 09:50:12.000000 pygdal-3.5.3.11/GDAL_VERSION
+-rw-rw-r--   0 jean      (1000) jean      (1000)       75 2023-05-18 09:50:12.000000 pygdal-3.5.3.11/MANIFEST.in
+-rw-rw-r--   0 jean      (1000) jean      (1000)     2698 2023-05-18 09:50:15.151008 pygdal-3.5.3.11/PKG-INFO
+-rw-rw-r--   0 jean      (1000) jean      (1000)     1700 2023-05-18 09:50:12.000000 pygdal-3.5.3.11/README.rst
+drwxrwxr-x   0 jean      (1000) jean      (1000)        0 2023-05-18 09:50:15.151008 pygdal-3.5.3.11/extensions/
+-rw-rw-r--   0 jean      (1000) jean      (1000)   210330 2023-05-18 09:50:12.000000 pygdal-3.5.3.11/extensions/gdal_array_wrap.cpp
+-rw-rw-r--   0 jean      (1000) jean      (1000)  1621195 2023-05-18 09:50:12.000000 pygdal-3.5.3.11/extensions/gdal_wrap.cpp
+-rw-rw-r--   0 jean      (1000) jean      (1000)   122491 2023-05-18 09:50:12.000000 pygdal-3.5.3.11/extensions/gdalconst_wrap.c
+-rw-rw-r--   0 jean      (1000) jean      (1000)  1326479 2023-05-18 09:50:12.000000 pygdal-3.5.3.11/extensions/ogr_wrap.cpp
+-rw-rw-r--   0 jean      (1000) jean      (1000)   721424 2023-05-18 09:50:12.000000 pygdal-3.5.3.11/extensions/osr_wrap.cpp
+drwxrwxr-x   0 jean      (1000) jean      (1000)        0 2023-05-18 09:50:15.147008 pygdal-3.5.3.11/osgeo/
+-rw-rw-r--   0 jean      (1000) jean      (1000)     5418 2023-05-18 09:50:12.000000 pygdal-3.5.3.11/osgeo/__init__.py
+-rw-rw-r--   0 jean      (1000) jean      (1000)   194379 2023-05-18 09:50:12.000000 pygdal-3.5.3.11/osgeo/gdal.py
+-rw-rw-r--   0 jean      (1000) jean      (1000)    26574 2023-05-18 09:50:12.000000 pygdal-3.5.3.11/osgeo/gdal_array.py
+-rw-rw-r--   0 jean      (1000) jean      (1000)    10262 2023-05-18 09:50:12.000000 pygdal-3.5.3.11/osgeo/gdalconst.py
+-rw-rw-r--   0 jean      (1000) jean      (1000)      214 2023-05-18 09:50:12.000000 pygdal-3.5.3.11/osgeo/gdalnumeric.py
+-rw-rw-r--   0 jean      (1000) jean      (1000)     9376 2023-05-18 09:50:12.000000 pygdal-3.5.3.11/osgeo/gnm.py
+-rw-rw-r--   0 jean      (1000) jean      (1000)   262590 2023-05-18 09:50:12.000000 pygdal-3.5.3.11/osgeo/ogr.py
+-rw-rw-r--   0 jean      (1000) jean      (1000)    52387 2023-05-18 09:50:12.000000 pygdal-3.5.3.11/osgeo/osr.py
+-rw-rw-r--   0 jean      (1000) jean      (1000)      190 2023-05-18 09:50:12.000000 pygdal-3.5.3.11/osgeo/utils.py
+drwxrwxr-x   0 jean      (1000) jean      (1000)        0 2023-05-18 09:50:15.151008 pygdal-3.5.3.11/pygdal.egg-info/
+-rw-rw-r--   0 jean      (1000) jean      (1000)     2698 2023-05-18 09:50:14.000000 pygdal-3.5.3.11/pygdal.egg-info/PKG-INFO
+-rw-rw-r--   0 jean      (1000) jean      (1000)      518 2023-05-18 09:50:15.000000 pygdal-3.5.3.11/pygdal.egg-info/SOURCES.txt
+-rw-rw-r--   0 jean      (1000) jean      (1000)        1 2023-05-18 09:50:14.000000 pygdal-3.5.3.11/pygdal.egg-info/dependency_links.txt
+-rw-rw-r--   0 jean      (1000) jean      (1000)        1 2023-05-18 09:50:14.000000 pygdal-3.5.3.11/pygdal.egg-info/not-zip-safe
+-rw-rw-r--   0 jean      (1000) jean      (1000)       13 2023-05-18 09:50:14.000000 pygdal-3.5.3.11/pygdal.egg-info/requires.txt
+-rw-rw-r--   0 jean      (1000) jean      (1000)        6 2023-05-18 09:50:14.000000 pygdal-3.5.3.11/pygdal.egg-info/top_level.txt
+-rw-rw-r--   0 jean      (1000) jean      (1000)       38 2023-05-18 09:50:15.151008 pygdal-3.5.3.11/setup.cfg
+-rw-rw-r--   0 jean      (1000) jean      (1000)     7306 2023-05-18 09:50:12.000000 pygdal-3.5.3.11/setup.py
```

### Comparing `pygdal-3.5.2.11/PKG-INFO` & `pygdal-3.5.3.11/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygdal
-Version: 3.5.2.11
+Version: 3.5.3.11
 Summary: Virtualenv and setuptools friendly version of standard GDAL python bindings
 Home-page: https://github.com/nextgis/pygdal
 Author: Frank Warmerdam
 Author-email: warmerdam@pobox.com
 Maintainer: Aleksandr Dezhin
 Maintainer-email: me@dezhin.net
 License: MIT
```

### Comparing `pygdal-3.5.2.11/README.rst` & `pygdal-3.5.3.11/README.rst`

 * *Files identical despite different names*

### Comparing `pygdal-3.5.2.11/extensions/gdal_array_wrap.cpp` & `pygdal-3.5.3.11/extensions/gdal_array_wrap.cpp`

 * *Files identical despite different names*

### Comparing `pygdal-3.5.2.11/extensions/gdal_wrap.cpp` & `pygdal-3.5.3.11/extensions/gdal_wrap.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -5199,42 +5199,98 @@
 SWIGINTERN char const *GDALGroupHS_GetFullName(GDALGroupHS *self){
     return GDALGroupGetFullName(self);
   }
 SWIGINTERN char **GDALGroupHS_GetMDArrayNames(GDALGroupHS *self,char **options=0){
     return GDALGroupGetMDArrayNames( self, options );
   }
 SWIGINTERN GDALMDArrayHS *GDALGroupHS_OpenMDArray(GDALGroupHS *self,char const *name,char **options=0){
-    return GDALGroupOpenMDArray(self, name, options);
+
+    CPLErr eLastErrorType = CPLGetLastErrorType();
+
+    GDALMDArrayH hRet = GDALGroupOpenMDArray(self, name, options);
+
+    if( bUseExceptions && hRet == NULL && eLastErrorType == CE_None && CPLGetLastErrorType() == CE_None )
+        CPLError(CE_Failure, CPLE_AppDefined, "Array %s does not exist", name);
+
+    return hRet;
   }
 SWIGINTERN GDALMDArrayHS *GDALGroupHS_OpenMDArrayFromFullname(GDALGroupHS *self,char const *name,char **options=0){
-    return GDALGroupOpenMDArrayFromFullname(self, name, options);
+
+    CPLErr eLastErrorType = CPLGetLastErrorType();
+
+    GDALMDArrayH hRet = GDALGroupOpenMDArrayFromFullname(self, name, options);
+
+    if( bUseExceptions && hRet == NULL && eLastErrorType == CE_None && CPLGetLastErrorType() == CE_None )
+        CPLError(CE_Failure, CPLE_AppDefined, "Array %s does not exist", name);
+
+    return hRet;
   }
 SWIGINTERN GDALMDArrayHS *GDALGroupHS_ResolveMDArray(GDALGroupHS *self,char const *name,char const *starting_point,char **options=0){
-    return GDALGroupResolveMDArray(self, name, starting_point, options);
+
+    CPLErr eLastErrorType = CPLGetLastErrorType();
+
+    GDALMDArrayH hRet = GDALGroupResolveMDArray(self, name, starting_point, options);
+
+    if( bUseExceptions && hRet == NULL && eLastErrorType == CE_None && CPLGetLastErrorType() == CE_None )
+        CPLError(CE_Failure, CPLE_AppDefined, "Array %s does not exist", name);
+
+    return hRet;
   }
 SWIGINTERN char **GDALGroupHS_GetGroupNames(GDALGroupHS *self,char **options=0){
     return GDALGroupGetGroupNames( self, options );
   }
 SWIGINTERN GDALGroupHS *GDALGroupHS_OpenGroup(GDALGroupHS *self,char const *name,char **options=0){
-    return GDALGroupOpenGroup(self, name, options);
+
+    CPLErr eLastErrorType = CPLGetLastErrorType();
+
+    GDALGroupH hRet = GDALGroupOpenGroup(self, name, options);
+
+    if( bUseExceptions && hRet == NULL && eLastErrorType == CE_None && CPLGetLastErrorType() == CE_None )
+        CPLError(CE_Failure, CPLE_AppDefined, "Group %s does not exist", name);
+
+    return hRet;
   }
 SWIGINTERN GDALGroupHS *GDALGroupHS_OpenGroupFromFullname(GDALGroupHS *self,char const *name,char **options=0){
-    return GDALGroupOpenGroupFromFullname(self, name, options);
+
+    CPLErr eLastErrorType = CPLGetLastErrorType();
+
+    GDALGroupH hRet = GDALGroupOpenGroupFromFullname(self, name, options);
+
+    if( bUseExceptions && hRet == NULL && eLastErrorType == CE_None && CPLGetLastErrorType() == CE_None )
+        CPLError(CE_Failure, CPLE_AppDefined, "Group %s does not exist", name);
+
+    return hRet;
   }
 SWIGINTERN char **GDALGroupHS_GetVectorLayerNames(GDALGroupHS *self,char **options=0){
     return GDALGroupGetVectorLayerNames( self, options );
   }
 SWIGINTERN OGRLayerShadow *GDALGroupHS_OpenVectorLayer(GDALGroupHS *self,char const *name,char **options=0){
-    return (OGRLayerShadow*) GDALGroupOpenVectorLayer(self, name, options);
+
+    CPLErr eLastErrorType = CPLGetLastErrorType();
+
+    OGRLayerH hRet = GDALGroupOpenVectorLayer(self, name, options);
+
+    if( bUseExceptions && hRet == NULL && eLastErrorType == CE_None && CPLGetLastErrorType() == CE_None )
+        CPLError(CE_Failure, CPLE_AppDefined, "Vector layer %s does not exist", name);
+
+    return (OGRLayerShadow*) hRet;
   }
 SWIGINTERN void GDALGroupHS_GetDimensions(GDALGroupHS *self,GDALDimensionHS ***pdims,size_t *pnCount,char **options=0){
     *pdims = GDALGroupGetDimensions(self, pnCount, options);
   }
 SWIGINTERN GDALAttributeHS *GDALGroupHS_GetAttribute(GDALGroupHS *self,char const *name){
-    return GDALGroupGetAttribute(self, name);
+
+    CPLErr eLastErrorType = CPLGetLastErrorType();
+
+    GDALAttributeH hRet = GDALGroupGetAttribute(self, name);
+
+    if( bUseExceptions && hRet == NULL && eLastErrorType == CE_None && CPLGetLastErrorType() == CE_None )
+        CPLError(CE_Failure, CPLE_AppDefined, "Attribute %s does not exist", name);
+
+    return hRet;
   }
 SWIGINTERN void GDALGroupHS_GetAttributes(GDALGroupHS *self,GDALAttributeHS ***pattrs,size_t *pnCount,char **options=0){
     *pattrs = GDALGroupGetAttributes(self, pnCount, options);
   }
 SWIGINTERN char **GDALGroupHS_GetStructuralInfo(GDALGroupHS *self){
     return GDALGroupGetStructuralInfo( self );
   }
@@ -5749,15 +5805,23 @@
     if( !(GDALMDArrayAdviseReadEx( self, array_start_idx, count_internal.data(), options )) )
     {
         return CE_Failure;
     }
     return CE_None;
   }
 SWIGINTERN GDALAttributeHS *GDALMDArrayHS_GetAttribute(GDALMDArrayHS *self,char const *name){
-    return GDALMDArrayGetAttribute(self, name);
+
+    CPLErr eLastErrorType = CPLGetLastErrorType();
+
+    GDALAttributeH hRet = GDALMDArrayGetAttribute(self, name);
+
+    if( bUseExceptions && hRet == NULL && eLastErrorType == CE_None && CPLGetLastErrorType() == CE_None )
+        CPLError(CE_Failure, CPLE_AppDefined, "Attribute %s does not exist", name);
+
+    return hRet;
   }
 SWIGINTERN void GDALMDArrayHS_GetAttributes(GDALMDArrayHS *self,GDALAttributeHS ***pattrs,size_t *pnCount,char **options=0){
     *pattrs = GDALMDArrayGetAttributes(self, pnCount, options);
   }
 SWIGINTERN GDALAttributeHS *GDALMDArrayHS_CreateAttribute(GDALMDArrayHS *self,char const *name,int nDimensions,GUIntBig *dimensions,GDALExtendedDataTypeHS *data_type,char **options=0){
     return GDALMDArrayCreateAttribute(self, name, nDimensions,
                                     (const GUInt64*)dimensions,
```

### Comparing `pygdal-3.5.2.11/extensions/gdalconst_wrap.c` & `pygdal-3.5.3.11/extensions/gdalconst_wrap.c`

 * *Files identical despite different names*

### Comparing `pygdal-3.5.2.11/extensions/ogr_wrap.cpp` & `pygdal-3.5.3.11/extensions/ogr_wrap.cpp`

 * *Files identical despite different names*

### Comparing `pygdal-3.5.2.11/extensions/osr_wrap.cpp` & `pygdal-3.5.3.11/extensions/osr_wrap.cpp`

 * *Files identical despite different names*

### Comparing `pygdal-3.5.2.11/osgeo/__init__.py` & `pygdal-3.5.3.11/osgeo/__init__.py`

 * *Files identical despite different names*

### Comparing `pygdal-3.5.2.11/osgeo/gdal.py` & `pygdal-3.5.3.11/osgeo/gdal.py`

 * *Files identical despite different names*

### Comparing `pygdal-3.5.2.11/osgeo/gdal_array.py` & `pygdal-3.5.3.11/osgeo/gdal_array.py`

 * *Files identical despite different names*

### Comparing `pygdal-3.5.2.11/osgeo/gdalconst.py` & `pygdal-3.5.3.11/osgeo/gdalconst.py`

 * *Files identical despite different names*

### Comparing `pygdal-3.5.2.11/osgeo/gnm.py` & `pygdal-3.5.3.11/osgeo/gnm.py`

 * *Files identical despite different names*

### Comparing `pygdal-3.5.2.11/osgeo/ogr.py` & `pygdal-3.5.3.11/osgeo/ogr.py`

 * *Files identical despite different names*

### Comparing `pygdal-3.5.2.11/osgeo/osr.py` & `pygdal-3.5.3.11/osgeo/osr.py`

 * *Files identical despite different names*

### Comparing `pygdal-3.5.2.11/pygdal.egg-info/PKG-INFO` & `pygdal-3.5.3.11/pygdal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygdal
-Version: 3.5.2.11
+Version: 3.5.3.11
 Summary: Virtualenv and setuptools friendly version of standard GDAL python bindings
 Home-page: https://github.com/nextgis/pygdal
 Author: Frank Warmerdam
 Author-email: warmerdam@pobox.com
 Maintainer: Aleksandr Dezhin
 Maintainer-email: me@dezhin.net
 License: MIT
```

### Comparing `pygdal-3.5.2.11/pygdal.egg-info/SOURCES.txt` & `pygdal-3.5.3.11/pygdal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygdal-3.5.2.11/setup.py` & `pygdal-3.5.3.11/setup.py`

 * *Files identical despite different names*

