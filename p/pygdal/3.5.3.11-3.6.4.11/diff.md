# Comparing `tmp/pygdal-3.5.3.11.tar.gz` & `tmp/pygdal-3.6.4.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygdal-3.5.3.11.tar", last modified: Thu May 18 09:50:15 2023, max compression
+gzip compressed data, was "pygdal-3.6.4.11.tar", last modified: Thu May 18 10:15:03 2023, max compression
```

## Comparing `pygdal-3.5.3.11.tar` & `pygdal-3.6.4.11.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 jean      (1000) jean      (1000)        0 2023-05-18 09:50:15.151008 pygdal-3.5.3.11/
--rw-rw-r--   0 jean      (1000) jean      (1000)        6 2023-05-18 09:50:12.000000 pygdal-3.5.3.11/GDAL_VERSION
--rw-rw-r--   0 jean      (1000) jean      (1000)       75 2023-05-18 09:50:12.000000 pygdal-3.5.3.11/MANIFEST.in
--rw-rw-r--   0 jean      (1000) jean      (1000)     2698 2023-05-18 09:50:15.151008 pygdal-3.5.3.11/PKG-INFO
--rw-rw-r--   0 jean      (1000) jean      (1000)     1700 2023-05-18 09:50:12.000000 pygdal-3.5.3.11/README.rst
-drwxrwxr-x   0 jean      (1000) jean      (1000)        0 2023-05-18 09:50:15.151008 pygdal-3.5.3.11/extensions/
--rw-rw-r--   0 jean      (1000) jean      (1000)   210330 2023-05-18 09:50:12.000000 pygdal-3.5.3.11/extensions/gdal_array_wrap.cpp
--rw-rw-r--   0 jean      (1000) jean      (1000)  1621195 2023-05-18 09:50:12.000000 pygdal-3.5.3.11/extensions/gdal_wrap.cpp
--rw-rw-r--   0 jean      (1000) jean      (1000)   122491 2023-05-18 09:50:12.000000 pygdal-3.5.3.11/extensions/gdalconst_wrap.c
--rw-rw-r--   0 jean      (1000) jean      (1000)  1326479 2023-05-18 09:50:12.000000 pygdal-3.5.3.11/extensions/ogr_wrap.cpp
--rw-rw-r--   0 jean      (1000) jean      (1000)   721424 2023-05-18 09:50:12.000000 pygdal-3.5.3.11/extensions/osr_wrap.cpp
-drwxrwxr-x   0 jean      (1000) jean      (1000)        0 2023-05-18 09:50:15.147008 pygdal-3.5.3.11/osgeo/
--rw-rw-r--   0 jean      (1000) jean      (1000)     5418 2023-05-18 09:50:12.000000 pygdal-3.5.3.11/osgeo/__init__.py
--rw-rw-r--   0 jean      (1000) jean      (1000)   194379 2023-05-18 09:50:12.000000 pygdal-3.5.3.11/osgeo/gdal.py
--rw-rw-r--   0 jean      (1000) jean      (1000)    26574 2023-05-18 09:50:12.000000 pygdal-3.5.3.11/osgeo/gdal_array.py
--rw-rw-r--   0 jean      (1000) jean      (1000)    10262 2023-05-18 09:50:12.000000 pygdal-3.5.3.11/osgeo/gdalconst.py
--rw-rw-r--   0 jean      (1000) jean      (1000)      214 2023-05-18 09:50:12.000000 pygdal-3.5.3.11/osgeo/gdalnumeric.py
--rw-rw-r--   0 jean      (1000) jean      (1000)     9376 2023-05-18 09:50:12.000000 pygdal-3.5.3.11/osgeo/gnm.py
--rw-rw-r--   0 jean      (1000) jean      (1000)   262590 2023-05-18 09:50:12.000000 pygdal-3.5.3.11/osgeo/ogr.py
--rw-rw-r--   0 jean      (1000) jean      (1000)    52387 2023-05-18 09:50:12.000000 pygdal-3.5.3.11/osgeo/osr.py
--rw-rw-r--   0 jean      (1000) jean      (1000)      190 2023-05-18 09:50:12.000000 pygdal-3.5.3.11/osgeo/utils.py
-drwxrwxr-x   0 jean      (1000) jean      (1000)        0 2023-05-18 09:50:15.151008 pygdal-3.5.3.11/pygdal.egg-info/
--rw-rw-r--   0 jean      (1000) jean      (1000)     2698 2023-05-18 09:50:14.000000 pygdal-3.5.3.11/pygdal.egg-info/PKG-INFO
--rw-rw-r--   0 jean      (1000) jean      (1000)      518 2023-05-18 09:50:15.000000 pygdal-3.5.3.11/pygdal.egg-info/SOURCES.txt
--rw-rw-r--   0 jean      (1000) jean      (1000)        1 2023-05-18 09:50:14.000000 pygdal-3.5.3.11/pygdal.egg-info/dependency_links.txt
--rw-rw-r--   0 jean      (1000) jean      (1000)        1 2023-05-18 09:50:14.000000 pygdal-3.5.3.11/pygdal.egg-info/not-zip-safe
--rw-rw-r--   0 jean      (1000) jean      (1000)       13 2023-05-18 09:50:14.000000 pygdal-3.5.3.11/pygdal.egg-info/requires.txt
--rw-rw-r--   0 jean      (1000) jean      (1000)        6 2023-05-18 09:50:14.000000 pygdal-3.5.3.11/pygdal.egg-info/top_level.txt
--rw-rw-r--   0 jean      (1000) jean      (1000)       38 2023-05-18 09:50:15.151008 pygdal-3.5.3.11/setup.cfg
--rw-rw-r--   0 jean      (1000) jean      (1000)     7306 2023-05-18 09:50:12.000000 pygdal-3.5.3.11/setup.py
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

### Comparing `pygdal-3.5.3.11/PKG-INFO` & `pygdal-3.6.4.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygdal
-Version: 3.5.3.11
+Version: 3.6.4.11
 Summary: Virtualenv and setuptools friendly version of standard GDAL python bindings
 Home-page: https://github.com/nextgis/pygdal
 Author: Frank Warmerdam
 Author-email: warmerdam@pobox.com
 Maintainer: Aleksandr Dezhin
 Maintainer-email: me@dezhin.net
 License: MIT
```

### Comparing `pygdal-3.5.3.11/README.rst` & `pygdal-3.6.4.11/README.rst`

 * *Files identical despite different names*

### Comparing `pygdal-3.5.3.11/extensions/gdal_array_wrap.cpp` & `pygdal-3.6.4.11/extensions/gdal_array_wrap.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -3230,83 +3230,82 @@
             pszLastErrorMessage);
     }
 }
 
 
 #include <vector>
 #include "gdal_priv.h"
+#include "ogr_recordbatch.h"
+
 #ifdef _DEBUG
 #undef _DEBUG
 #include "Python.h"
+#include "datetime.h"
 #define _DEBUG
 #else
 #include "Python.h"
+#include "datetime.h"
 #endif
 #define NPY_NO_DEPRECATED_API NPY_1_7_API_VERSION
 #include "numpy/arrayobject.h"
 
 #ifdef DEBUG
 typedef struct GDALRasterBandHS GDALRasterBandShadow;
 typedef struct GDALDatasetHS GDALDatasetShadow;
 typedef struct RasterAttributeTableHS GDALRasterAttributeTableShadow;
 #else
 typedef void GDALRasterBandShadow;
 typedef void GDALDatasetShadow;
 typedef void GDALRasterAttributeTableShadow;
 #endif
 
+// Declaration from memmultidim.h
+std::shared_ptr<GDALMDArray> CPL_DLL MEMGroupCreateMDArray(GDALGroup* poGroup,
+                                                   const std::string& osName,
+                                                   const std::vector<std::shared_ptr<GDALDimension>>& aoDimensions,
+                                                   const GDALExtendedDataType& oDataType,
+                                                   void* pData,
+                                                   CSLConstList papszOptions);
+
+
 CPL_C_START
 
 GDALRasterBandH CPL_DLL MEMCreateRasterBandEx( GDALDataset *, int, GByte *,
                                                GDALDataType, GSpacing, GSpacing, int );
 CPL_C_END
 
 typedef char retStringAndCPLFree;
 
 class NUMPYDataset : public GDALDataset
 {
     PyArrayObject *psArray;
 
     int           bValidGeoTransform;
     double	  adfGeoTransform[6];
-    char	  *pszProjection;
+    OGRSpatialReference m_oSRS{};
 
     int           nGCPCount;
     GDAL_GCP      *pasGCPList;
-    char          *pszGCPProjection;
+    OGRSpatialReference m_oGCPSRS{};;
 
   public:
                  NUMPYDataset();
                  ~NUMPYDataset();
 
-    virtual const char *_GetProjectionRef(void) override;
-    const OGRSpatialReference* GetSpatialRef() const override {
-        return GetSpatialRefFromOldGetProjectionRef();
-    }
-    virtual CPLErr _SetProjection( const char * ) override;
-    CPLErr SetSpatialRef(const OGRSpatialReference* poSRS) override {
-        return OldSetProjectionFromSetSpatialRef(poSRS);
-    }
+    const OGRSpatialReference* GetSpatialRef() const override;
+    CPLErr SetSpatialRef(const OGRSpatialReference* poSRS) override;
 
     virtual CPLErr GetGeoTransform( double * ) override;
     virtual CPLErr SetGeoTransform( double * ) override;
 
     virtual int    GetGCPCount() override;
-    virtual const char *_GetGCPProjection() override;
-    const OGRSpatialReference* GetGCPSpatialRef() const override {
-        return GetGCPSpatialRefFromOldGetGCPProjection();
-    }
+    const OGRSpatialReference* GetGCPSpatialRef() const override;
     virtual const GDAL_GCP *GetGCPs() override;
-    virtual CPLErr _SetGCPs( int nGCPCount, const GDAL_GCP *pasGCPList,
-                            const char *pszGCPProjection ) override;
-    using GDALDataset::SetGCPs;
     CPLErr SetGCPs( int nGCPCount, const GDAL_GCP *pasGCPList,
-                    const OGRSpatialReference* poSRS ) override {
-        return OldSetGCPsFromNew(nGCPCount, pasGCPList, poSRS);
-    }
+                    const OGRSpatialReference* poSRS ) override;
 
     static GDALDataset *Open( PyArrayObject *psArray, bool binterleave = true );
     static GDALDataset *Open( GDALOpenInfo * );
 };
 
 
 /************************************************************************/
@@ -3339,38 +3338,33 @@
 /*                            NUMPYDataset()                            */
 /************************************************************************/
 
 NUMPYDataset::NUMPYDataset()
 
 {
     psArray = NULL;
-    pszProjection = CPLStrdup("");
     bValidGeoTransform = FALSE;
     adfGeoTransform[0] = 0.0;
     adfGeoTransform[1] = 1.0;
     adfGeoTransform[2] = 0.0;
     adfGeoTransform[3] = 0.0;
     adfGeoTransform[4] = 0.0;
     adfGeoTransform[5] = 1.0;
 
     nGCPCount = 0;
     pasGCPList = NULL;
-    pszGCPProjection = CPLStrdup("");
 }
 
 /************************************************************************/
 /*                            ~NUMPYDataset()                            */
 /************************************************************************/
 
 NUMPYDataset::~NUMPYDataset()
 
 {
-    CPLFree( pszProjection );
-
-    CPLFree( pszGCPProjection );
     if( nGCPCount > 0 )
     {
         GDALDeinitGCPs( nGCPCount, pasGCPList );
         CPLFree( pasGCPList );
     }
 
     FlushCache(true);
@@ -3380,32 +3374,33 @@
 
     Py_DECREF( psArray );
 
     SWIG_PYTHON_THREAD_END_BLOCK;
 }
 
 /************************************************************************/
-/*                          GetProjectionRef()                          */
+/*                          GetSpatialRef()                             */
 /************************************************************************/
 
-const char *NUMPYDataset::_GetProjectionRef()
+const OGRSpatialReference *NUMPYDataset::GetSpatialRef() const
 
 {
-    return( pszProjection );
+    return m_oSRS.IsEmpty() ? nullptr:  &m_oSRS;
 }
 
 /************************************************************************/
-/*                           SetProjection()                            */
+/*                           SetSpatialRef()                            */
 /************************************************************************/
 
-CPLErr NUMPYDataset::_SetProjection( const char * pszNewProjection )
+CPLErr NUMPYDataset::SetSpatialRef( const OGRSpatialReference* poSRS )
 
 {
-    CPLFree( pszProjection );
-    pszProjection = CPLStrdup( pszNewProjection );
+    m_oSRS.Clear();
+    if( poSRS )
+        m_oSRS = *poSRS;
 
     return CE_None;
 }
 
 /************************************************************************/
 /*                          GetGeoTransform()                           */
 /************************************************************************/
@@ -3439,21 +3434,21 @@
 int NUMPYDataset::GetGCPCount()
 
 {
     return nGCPCount;
 }
 
 /************************************************************************/
-/*                          GetGCPProjection()                          */
+/*                          GetGCPSpatialRef()                          */
 /************************************************************************/
 
-const char *NUMPYDataset::_GetGCPProjection()
+const OGRSpatialReference *NUMPYDataset::GetGCPSpatialRef() const
 
 {
-    return pszGCPProjection;
+    return m_oGCPSRS.IsEmpty() ? nullptr:  &m_oGCPSRS;
 }
 
 /************************************************************************/
 /*                               GetGCPs()                              */
 /************************************************************************/
 
 const GDAL_GCP *NUMPYDataset::GetGCPs()
@@ -3462,27 +3457,28 @@
     return pasGCPList;
 }
 
 /************************************************************************/
 /*                              SetGCPs()                               */
 /************************************************************************/
 
-CPLErr NUMPYDataset::_SetGCPs( int nGCPCount, const GDAL_GCP *pasGCPList,
-                              const char *pszGCPProjection )
+CPLErr NUMPYDataset::SetGCPs( int nGCPCount, const GDAL_GCP *pasGCPList,
+                              const OGRSpatialReference* poSRS )
 
 {
-    CPLFree( this->pszGCPProjection );
+    m_oGCPSRS.Clear();
+    if( poSRS )
+        m_oGCPSRS = *poSRS;
+
     if( this->nGCPCount > 0 )
     {
         GDALDeinitGCPs( this->nGCPCount, this->pasGCPList );
         CPLFree( this->pasGCPList );
     }
 
-    this->pszGCPProjection = CPLStrdup(pszGCPProjection);
-
     this->nGCPCount = nGCPCount;
 
     this->pasGCPList = GDALDuplicateGCPs( nGCPCount, pasGCPList );
 
     return CE_None;
 }
 
@@ -3762,24 +3758,19 @@
         apoDims.push_back(poDim);
         if( i > 0 )
             strides += ',';
         strides += CPLSPrintf(CPL_FRMT_GIB,
                               static_cast<GIntBig>(PyArray_STRIDES(psArray)[i]));
     }
     CPLStringList aosOptions;
-    char szDataPointer[128] = { '\0' };
-    int nChars = CPLPrintPointer( szDataPointer,
-                                  PyArray_DATA(psArray),
-                                  sizeof(szDataPointer) );
-    szDataPointer[nChars] = 0;
-    aosOptions.SetNameValue("DATAPOINTER", szDataPointer);
     aosOptions.SetNameValue("STRIDES", strides.c_str());
-    auto mdArray = poGroup->CreateMDArray("array",
+    auto mdArray = MEMGroupCreateMDArray(poGroup.get(), "array",
                                       apoDims,
                                       GDALExtendedDataType::Create(eType),
+                                      PyArray_DATA(psArray),
                                       aosOptions.List());
     if( !mdArray )
     {
         delete poMEMDS;
         return nullptr;
     }
 
@@ -3950,15 +3941,15 @@
 PyProgressProxy( double dfComplete, const char *pszMessage, void *pData )
 
 {
     PyProgressData *psInfo = (PyProgressData *) pData;
     PyObject *psArgs, *psResult;
     int      bContinue = TRUE;
 
-    if( psInfo->nLastReported == (int) (100.0 * dfComplete) )
+    if( dfComplete > 0 && psInfo->nLastReported == (int) (100.0 * dfComplete) )
         return TRUE;
 
     if( psInfo->psPyCallback == NULL || psInfo->psPyCallback == Py_None )
         return TRUE;
 
     psInfo->nLastReported = (int) (100.0 * dfComplete);
 
@@ -4312,14 +4303,696 @@
                                 buffer_datatype,
                                 PyArray_DATA(psArray),
                                 NULL, 0) ? CE_None : CE_Failure;
     }
   }
 
 
+typedef void* VoidPtrAsLong;
+
+/* Internal method used by ogr.Layer.GetNextRecordBatchAsNumpy() */
+PyObject* _RecordBatchAsNumpy(VoidPtrAsLong recordBatchPtr,
+                              VoidPtrAsLong schemaPtr,
+                              PyObject* pointerArrayKeeper)
+{
+    const struct ArrowSchema* schema = (const struct ArrowSchema* )schemaPtr;
+    const struct ArrowArray* array = (const struct ArrowArray* )recordBatchPtr;
+    if( strcmp(schema->format, "+s") != 0 )
+    {
+      CPLError(CE_Failure, CPLE_AppDefined, "schema->format != '+s'");
+      Py_RETURN_NONE;
+    }
+    if( schema->n_children != array->n_children )
+    {
+      CPLError(CE_Failure, CPLE_AppDefined,
+               "schema->n_children(=%d) != array->n_children(=%d)",
+               static_cast<int>(schema->n_children),
+               static_cast<int>(array->n_children));
+      Py_RETURN_NONE;
+    }
+    PyObject *dict = PyDict_New();
+    for( int iField = 0; iField < array->n_children; iField++ )
+    {
+        const struct ArrowArray* arrayField = array->children[iField];
+        const struct ArrowSchema* schemaField = schema->children[iField];
+        npy_intp dims = arrayField->length;
+        const char* arrowType = schemaField->format;
+        int typenum = -1;
+        int sizeOfType = 0;
+        const struct
+        {
+            char        arrowType;
+            int         numpyType;
+            int         sizeOfType;
+        } MapArrowTypeToNumpyType[] = {
+            { 'b', NPY_BOOL,    1 },
+            { 'C', NPY_UINT8,   1 },
+            { 'c', NPY_INT8,    1 },
+            { 'S', NPY_UINT16,  2 },
+            { 's', NPY_INT16,   2 },
+            { 'I', NPY_UINT32,  4 },
+            { 'i', NPY_INT32,   4 },
+            { 'L', NPY_UINT64,  8 },
+            { 'l', NPY_INT64,   8 },
+            { 'e', NPY_FLOAT16, 2 },
+            { 'f', NPY_FLOAT32, 4 },
+            { 'g', NPY_FLOAT64, 8 },
+        };
+        const size_t nEltsInMapArrowTypeToNumpyType =
+            sizeof(MapArrowTypeToNumpyType) / sizeof(MapArrowTypeToNumpyType[0]);
+        const bool bIsList = (arrowType[0] == '+' &&
+                              arrowType[1] == 'l' &&
+                              arrowType[2] == '\0' &&
+                              schemaField->n_children == 1);
+        const bool bIsFixedSizeList = (arrowType[0] == '+' &&
+                                       arrowType[1] == 'w' &&
+                                       arrowType[2] == ':' &&
+                                       schemaField->n_children == 1);
+        for( size_t j = 0; j < nEltsInMapArrowTypeToNumpyType; ++j )
+        {
+            if( arrowType[0] == MapArrowTypeToNumpyType[j].arrowType &&
+                arrowType[1] == '\0' )
+            {
+                typenum = MapArrowTypeToNumpyType[j].numpyType;
+                break;
+            }
+            else if( (bIsList || bIsFixedSizeList) &&
+                     schemaField->children[0]->format[0] == MapArrowTypeToNumpyType[j].arrowType &&
+                     schemaField->children[0]->format[1] == '\0' )
+            {
+                typenum = MapArrowTypeToNumpyType[j].numpyType;
+                sizeOfType = MapArrowTypeToNumpyType[j].sizeOfType;
+                break;
+            }
+        }
+
+        PyObject* numpyArray = NULL;
+        if( typenum != -1 && !bIsList && schemaField->n_children == 0 )
+        {
+            if( arrayField->n_buffers != 2 )
+            {
+                CPLError(CE_Failure, CPLE_AppDefined,
+                         "Field %s: arrayField->n_buffers != 2",
+                         schemaField->name);
+                Py_DECREF(dict);
+                Py_RETURN_NONE;
+            }
+            if( typenum == NPY_BOOL )
+            {
+                numpyArray = PyArray_SimpleNew(1, &dims, NPY_BOOL);
+                for( npy_intp j = 0; j < dims; j++ )
+                {
+                    size_t srcOffset = static_cast<size_t>(arrayField->offset + j);
+                    uint8_t val = (((uint8_t*)arrayField->buffers[1])[srcOffset/8] >> (srcOffset % 8)) & 1;
+                    *(uint8_t*)PyArray_GETPTR1((PyArrayObject *) numpyArray, j) = val;
+                }
+            }
+            else
+            {
+                numpyArray = PyArray_SimpleNewFromData(1, &dims, typenum,
+                                            (char*)arrayField->buffers[1] + static_cast<size_t>(arrayField->offset) * sizeOfType);
+
+                /* Keep a reference to the owner object */
+#if NPY_API_VERSION >= 0x00000007
+                PyArray_SetBaseObject((PyArrayObject *) numpyArray, pointerArrayKeeper);
+#else
+                PyArray_BASE((PyArrayObject *) numpyArray) = pointerArrayKeeper;
+#endif
+                Py_INCREF(pointerArrayKeeper);
+            }
+        }
+        else if( typenum != -1 && bIsList )
+        {
+            if( arrayField->n_buffers != 2 )
+            {
+                CPLError(CE_Failure, CPLE_AppDefined,
+                         "Field %s: arrayField->n_buffers != 2",
+                         schemaField->name);
+                Py_DECREF(dict);
+                Py_RETURN_NONE;
+            }
+            if( arrayField->n_children != 1 )
+            {
+                CPLError(CE_Failure, CPLE_AppDefined,
+                         "Field %s: arrayField->n_children != 1",
+                         schemaField->name);
+                Py_DECREF(dict);
+                Py_RETURN_NONE;
+            }
+            if( arrayField->children[0]->n_buffers != 2 )
+            {
+                CPLError(CE_Failure, CPLE_AppDefined,
+                         "Field %s: arrayField->children[0]->n_buffers != 2",
+                         schemaField->name);
+                Py_DECREF(dict);
+                Py_RETURN_NONE;
+            }
+            const int32_t* offsets = (const int32_t*)arrayField->buffers[1] + arrayField->offset;
+            numpyArray = PyArray_SimpleNew(1, &dims, NPY_OBJECT);
+            for( npy_intp j = 0; j < dims; j++ )
+            {
+                npy_intp nvalues = offsets[j+1] - offsets[j];
+                PyObject* subObj;
+                if( typenum == NPY_BOOL )
+                {
+                    subObj = PyArray_SimpleNew(1, &nvalues, NPY_BOOL);
+                    for( npy_intp k = 0; k < nvalues; k++ )
+                    {
+                        size_t srcOffset = static_cast<size_t>(arrayField->children[0]->offset + offsets[j] + k);
+                        uint8_t val = (((uint8_t*)arrayField->children[0]->buffers[1])[srcOffset / 8]  >> (srcOffset % 8)) & 1;
+                        *(uint8_t*)PyArray_GETPTR1((PyArrayObject *) subObj, k) = val;
+                    }
+                }
+                else
+                {
+                    subObj = PyArray_SimpleNewFromData(
+                        1, &nvalues, typenum,
+                        (char*)arrayField->children[0]->buffers[1] + (static_cast<size_t>(arrayField->children[0]->offset) + offsets[j]) * sizeOfType);
+                    /* Keep a reference to the owner object */
+#if NPY_API_VERSION >= 0x00000007
+                    PyArray_SetBaseObject((PyArrayObject *) subObj, pointerArrayKeeper);
+#else
+                    PyArray_BASE((PyArrayObject *) subObj) = pointerArrayKeeper;
+#endif
+                    Py_INCREF(pointerArrayKeeper);
+                }
+                memcpy(PyArray_GETPTR1((PyArrayObject *) numpyArray, j),
+                       &subObj,
+                       sizeof(PyObject*));
+            }
+        }
+        else if( typenum != -1 && bIsFixedSizeList )
+        {
+            if( arrayField->n_buffers != 1 )
+            {
+                CPLError(CE_Failure, CPLE_AppDefined,
+                         "Field %s: arrayField->n_buffers != 1",
+                         schemaField->name);
+                Py_DECREF(dict);
+                Py_RETURN_NONE;
+            }
+            if( arrayField->n_children != 1 )
+            {
+                CPLError(CE_Failure, CPLE_AppDefined,
+                         "Field %s: arrayField->n_children != 1",
+                         schemaField->name);
+                Py_DECREF(dict);
+                Py_RETURN_NONE;
+            }
+            if( arrayField->children[0]->n_buffers != 2 )
+            {
+                CPLError(CE_Failure, CPLE_AppDefined,
+                         "Field %s: arrayField->children[0]->n_buffers != 2",
+                         schemaField->name);
+                Py_DECREF(dict);
+                Py_RETURN_NONE;
+            }
+            const int nLength = atoi(arrowType + strlen("+w:"));
+            numpyArray = PyArray_SimpleNew(1, &dims, NPY_OBJECT);
+            for( npy_intp j = 0; j < dims; j++ )
+            {
+                PyObject* subObj;
+                npy_intp nvalues = nLength;
+                if( typenum == NPY_BOOL )
+                {
+                    subObj = PyArray_SimpleNew(1, &nvalues, NPY_BOOL);
+                    for( npy_intp k = 0; k < nvalues; k++ )
+                    {
+                        size_t srcOffset = static_cast<size_t>(arrayField->children[0]->offset + j * nLength + k);
+                        uint8_t val = (((uint8_t*)arrayField->children[0]->buffers[1])[srcOffset / 8]  >> (srcOffset % 8)) & 1;
+                        *(uint8_t*)PyArray_GETPTR1((PyArrayObject *) subObj, k) = val;
+                    }
+                }
+                else
+                {
+                    subObj = PyArray_SimpleNewFromData(
+                        1, &nvalues, typenum,
+                        (char*)arrayField->children[0]->buffers[1] + static_cast<size_t>(arrayField->children[0]->offset) + j * nLength * sizeOfType);
+                    /* Keep a reference to the owner object */
+#if NPY_API_VERSION >= 0x00000007
+                    PyArray_SetBaseObject((PyArrayObject *) subObj, pointerArrayKeeper);
+#else
+                    PyArray_BASE((PyArrayObject *) subObj) = pointerArrayKeeper;
+#endif
+                    Py_INCREF(pointerArrayKeeper);
+                }
+                memcpy(PyArray_GETPTR1((PyArrayObject *) numpyArray, j),
+                       &subObj,
+                       sizeof(PyObject*));
+            }
+        }
+        else if( (arrowType[0] == 'u' || /* string */
+                  arrowType[0] == 'z'    /* binary */) && arrowType[1] == '\0' &&
+                  schemaField->n_children == 0 )
+        {
+            if( arrayField->n_buffers != 3 )
+            {
+                CPLError(CE_Failure, CPLE_AppDefined,
+                         "Field %s: arrayField->n_buffers != 3",
+                         schemaField->name);
+                Py_DECREF(dict);
+                Py_RETURN_NONE;
+            }
+            const int32_t* offsets = (const int32_t*)arrayField->buffers[1] + static_cast<size_t>(arrayField->offset);
+            // numpy can't deal with zero length strings
+            int32_t maxLength = 1;
+            int32_t minLength = 0x7FFFFFFF;
+            for( npy_intp j = 0; j < dims; j++ )
+            {
+                const int32_t nLength = offsets[j+1] - offsets[j];
+                if( nLength < minLength )
+                    minLength = nLength;
+                if( nLength > maxLength )
+                    maxLength = nLength;
+            }
+
+            if( arrowType[0] == 'z' && (minLength == 0 || minLength != maxLength) )
+            {
+                const uint8_t* panNotNulls =
+                     arrayField->null_count == 0 ? NULL :
+                    (const uint8_t*)arrayField->buffers[0];
+                numpyArray = PyArray_SimpleNew(1, &dims, NPY_OBJECT);
+                for( npy_intp j = 0; j < dims; j++ )
+                {
+                    PyObject* subObj;
+                    size_t srcOffset = static_cast<size_t>(arrayField->offset + j);
+                    if( panNotNulls && (panNotNulls[srcOffset / 8] & (1 << (srcOffset%8))) == 0 )
+                    {
+                        subObj = Py_None;
+                        Py_INCREF(subObj);
+                    }
+                    else
+                    {
+                        const int32_t nLength = offsets[j+1] - offsets[j];
+                        subObj = PyBytes_FromStringAndSize(
+                            ((const char*)arrayField->buffers[2]) + offsets[j],
+                            nLength);
+                    }
+                    memcpy(PyArray_GETPTR1((PyArrayObject *) numpyArray, j),
+                           &subObj,
+                           sizeof(PyObject*));
+                }
+            }
+            else
+            {
+                // create the dtype string
+                PyObject *pDTypeString = PyUnicode_FromFormat("%c%u",
+                    arrowType[0] == 'u' ? 'S' : 'V', maxLength);
+                // out type description object
+                PyArray_Descr *pDescr = NULL;
+                PyArray_DescrConverter(pDTypeString, &pDescr);
+                Py_DECREF(pDTypeString);
+
+                if( minLength == maxLength )
+                {
+                    numpyArray = PyArray_NewFromDescr(
+                        &PyArray_Type, pDescr, 1, &dims, NULL,
+                        (char*)arrayField->buffers[2] + offsets[0], 0, NULL);
+
+                    /* Keep a reference to the owner object */
+#if NPY_API_VERSION >= 0x00000007
+                    PyArray_SetBaseObject((PyArrayObject *) numpyArray, pointerArrayKeeper);
+#else
+                    PyArray_BASE((PyArrayObject *) numpyArray) = pointerArrayKeeper;
+#endif
+                    Py_INCREF(pointerArrayKeeper);
+                }
+                else
+                {
+                    // create array
+                    numpyArray = PyArray_SimpleNewFromDescr(1, &dims, pDescr);
+                    for( npy_intp j = 0; j < dims; j++ )
+                    {
+                        const int32_t nLength = offsets[j+1] - offsets[j];
+                        if( nLength > 0 )
+                        {
+                            memcpy(PyArray_GETPTR1((PyArrayObject *) numpyArray, j),
+                                   ((const char*)arrayField->buffers[2]) + offsets[j],
+                                   nLength);
+                        }
+                        if( nLength < maxLength )
+                        {
+                            memset(((char*)PyArray_GETPTR1((PyArrayObject *) numpyArray, j)) + nLength,
+                                   0,
+                                   maxLength - nLength);
+                        }
+                    }
+                }
+            }
+        }
+        else if( arrowType[0] == 'w' && arrowType[1] == ':' &&
+                 schemaField->n_children == 0 )
+        {
+            // Fixed width binary
+            if( arrayField->n_buffers != 2 )
+            {
+                CPLError(CE_Failure, CPLE_AppDefined,
+                         "field %s:arrayField->n_buffers != 2",
+                         schemaField->name);
+                Py_DECREF(dict);
+                Py_RETURN_NONE;
+            }
+            const int nLength = atoi(arrowType + strlen("w:"));
+            numpyArray = PyArray_SimpleNew(1, &dims, NPY_OBJECT);
+            for( npy_intp j = 0; j < dims; j++ )
+            {
+                PyObject* subObj = PyBytes_FromStringAndSize(
+                        ((const char*)arrayField->buffers[1]) + static_cast<size_t>(arrayField->offset) + j * nLength,
+                        nLength);
+                memcpy(PyArray_GETPTR1((PyArrayObject *) numpyArray, j),
+                       &subObj,
+                       sizeof(PyObject*));
+            }
+        }
+        else if( bIsList &&
+                 schemaField->children[0]->format[0] == 'u' &&
+                 schemaField->children[0]->format[1] == '\0' )
+        {
+            // List of strings
+            if( arrayField->n_buffers != 2 )
+            {
+                CPLError(CE_Failure, CPLE_AppDefined,
+                         "Field %s: arrayField->n_buffers != 2",
+                         schemaField->name);
+                Py_DECREF(dict);
+                Py_RETURN_NONE;
+            }
+            if( arrayField->n_children != 1 )
+            {
+                CPLError(CE_Failure, CPLE_AppDefined,
+                         "Field %s: arrayField->n_children != 1",
+                         schemaField->name);
+                Py_DECREF(dict);
+                Py_RETURN_NONE;
+            }
+            if( arrayField->children[0]->n_buffers != 3 )
+            {
+                CPLError(CE_Failure, CPLE_AppDefined,
+                         "Field %s: arrayField->children[0]->n_buffers != 3",
+                         schemaField->name);
+                Py_DECREF(dict);
+                Py_RETURN_NONE;
+            }
+            const int32_t* offsets = (const int32_t*)arrayField->buffers[1] + static_cast<size_t>(arrayField->offset);
+            const int32_t* offsetsToBytes = (const int32_t*)arrayField->children[0]->buffers[1] + static_cast<size_t>(arrayField->children[0]->offset);
+            const char* bytes = (const char*)arrayField->children[0]->buffers[2] + static_cast<size_t>(arrayField->children[0]->offset);
+            numpyArray = PyArray_SimpleNew(1, &dims, NPY_OBJECT);
+            for( npy_intp j = 0; j < dims; j++ )
+            {
+                npy_intp nStrings = offsets[j+1] - offsets[j];
+                int32_t maxLength = 1;
+                for( npy_intp k = 0; k < nStrings; k++ )
+                {
+                    const int32_t nLength = offsetsToBytes[offsets[j] + k + 1] - offsetsToBytes[offsets[j] + k];
+                    if( nLength > maxLength )
+                        maxLength = nLength;
+                }
+
+                // create the dtype string
+                PyObject *pDTypeString = PyUnicode_FromFormat("S%d", maxLength);
+                // out type description object
+                PyArray_Descr *pDescr = NULL;
+                PyArray_DescrConverter(pDTypeString, &pDescr);
+                Py_DECREF(pDTypeString);
+
+                PyObject* subArray = PyArray_SimpleNewFromDescr(1, &nStrings, pDescr);
+                for( npy_intp k = 0; k < nStrings; k++ )
+                {
+                    const int32_t nLength = offsetsToBytes[offsets[j] + k + 1] - offsetsToBytes[offsets[j] + k];
+                    if( nLength > 0 )
+                    {
+                        memcpy(PyArray_GETPTR1((PyArrayObject *) subArray, k),
+                               bytes + offsetsToBytes[offsets[j] + k],
+                               nLength);
+                    }
+                    if( nLength < maxLength )
+                    {
+                        memset(((char*)PyArray_GETPTR1((PyArrayObject *) subArray, k)) + nLength,
+                               0,
+                               maxLength - nLength);
+                    }
+                }
+
+                memcpy(PyArray_GETPTR1((PyArrayObject *) numpyArray, j),
+                       &subArray,
+                       sizeof(PyObject*));
+            }
+        }
+        else if( bIsFixedSizeList &&
+                 schemaField->children[0]->format[0] == 'u' &&
+                 schemaField->children[0]->format[1] == '\0' )
+        {
+            // Fixed size list of strings
+            const int nStrings = atoi(arrowType + strlen("+w:"));
+            if( arrayField->n_buffers != 1 )
+            {
+                CPLError(CE_Failure, CPLE_AppDefined,
+                         "Field %s: arrayField->n_buffers != 1",
+                         schemaField->name);
+                Py_DECREF(dict);
+                Py_RETURN_NONE;
+            }
+            if( arrayField->n_children != 1 )
+            {
+                CPLError(CE_Failure, CPLE_AppDefined,
+                         "Field %s: arrayField->n_children != 1",
+                         schemaField->name);
+                Py_DECREF(dict);
+                Py_RETURN_NONE;
+            }
+            if( arrayField->children[0]->n_buffers != 3 )
+            {
+                CPLError(CE_Failure, CPLE_AppDefined,
+                         "Field %s: arrayField->children[0]->n_buffers != 3",
+                         schemaField->name);
+                Py_DECREF(dict);
+                Py_RETURN_NONE;
+            }
+            const int32_t* offsetsToBytes = (const int32_t*)arrayField->children[0]->buffers[1] + static_cast<size_t>(arrayField->children[0]->offset);
+            const char* bytes = (const char*)arrayField->children[0]->buffers[2] + static_cast<size_t>(arrayField->children[0]->offset);
+            numpyArray = PyArray_SimpleNew(1, &dims, NPY_OBJECT);
+            for( npy_intp j = 0; j < dims; j++ )
+            {
+                int32_t maxLength = 1;
+                for( int k = 0; k < nStrings; k++ )
+                {
+                    const int32_t nLength = offsetsToBytes[j * nStrings + k + 1] - offsetsToBytes[j * nStrings + k];
+                    if( nLength > maxLength )
+                        maxLength = nLength;
+                }
+
+                // create the dtype string
+                PyObject *pDTypeString = PyUnicode_FromFormat("S%u", maxLength);
+                // out type description object
+                PyArray_Descr *pDescr = NULL;
+                PyArray_DescrConverter(pDTypeString, &pDescr);
+                Py_DECREF(pDTypeString);
+
+                npy_intp nStringsNpyIntp = nStrings;
+                PyObject* subArray = PyArray_SimpleNewFromDescr(1, &nStringsNpyIntp, pDescr);
+                for( int k = 0; k < nStrings; k++ )
+                {
+                    const int32_t nLength = offsetsToBytes[j * nStrings + k + 1] - offsetsToBytes[j * nStrings + k];
+                    if( nLength > 0 )
+                    {
+                        memcpy(PyArray_GETPTR1((PyArrayObject *) subArray, k),
+                               bytes + offsetsToBytes[j * nStrings + k],
+                               nLength);
+                    }
+                    if( nLength < maxLength )
+                    {
+                        memset(((char*)PyArray_GETPTR1((PyArrayObject *) subArray, k)) + nLength,
+                               0,
+                               maxLength - nLength);
+                    }
+                }
+
+                memcpy(PyArray_GETPTR1((PyArrayObject *) numpyArray, j),
+                       &subArray,
+                       sizeof(PyObject*));
+            }
+        }
+        else if( strcmp(arrowType, "tdD") == 0 &&
+                 schemaField->n_children == 0 )
+        {
+            // Date(32) in days since Epoch
+            if( arrayField->n_buffers != 2 )
+            {
+                CPLError(CE_Failure, CPLE_AppDefined,
+                         "Field %s: arrayField->n_buffers != 2",
+                         schemaField->name);
+                Py_DECREF(dict);
+                Py_RETURN_NONE;
+            }
+
+            // create the dtype string
+            PyObject *pDTypeString = PyUnicode_FromString("datetime64[D]");
+            // out type description object
+            PyArray_Descr *pDescr = NULL;
+            PyArray_DescrConverter(pDTypeString, &pDescr);
+            Py_DECREF(pDTypeString);
+            CPLAssert(pDescr);
+
+            // create array
+            numpyArray = PyArray_SimpleNewFromDescr(1, &dims, pDescr);
+            for( npy_intp j = 0; j < dims; j++ )
+            {
+                *(int64_t*)PyArray_GETPTR1((PyArrayObject *) numpyArray, j) =
+                    ((int*)arrayField->buffers[1])[j + static_cast<size_t>(arrayField->offset)];
+            }
+        }
+        else if( strcmp(arrowType, "ttm") == 0 &&
+                 schemaField->n_children == 0 )
+        {
+            // Time(32) in milliseconds
+            if( arrayField->n_buffers != 2 )
+            {
+                CPLError(CE_Failure, CPLE_AppDefined,
+                         "Field %s: arrayField->n_buffers != 2",
+                         schemaField->name);
+                Py_DECREF(dict);
+                Py_RETURN_NONE;
+            }
+#if 0
+            // create the dtype string
+            PyObject *pDTypeString = PyUnicode_FromString("datetime64[ms]");
+            // out type description object
+            PyArray_Descr *pDescr = NULL;
+            PyArray_DescrConverter(pDTypeString, &pDescr);
+            Py_DECREF(pDTypeString);
+            CPLAssert(pDescr);
+
+            // create array
+            numpyArray = PyArray_SimpleNewFromDescr(1, &dims, pDescr);
+            for( npy_intp j = 0; j < dims; j++ )
+            {
+                *(int64_t*)PyArray_GETPTR1((PyArrayObject *) numpyArray, j) =
+                    ((int*)arrayField->buffers[1])[j + static_cast<size_t>(arrayField->offset)];
+            }
+#else
+            // create array
+            numpyArray = PyArray_SimpleNew(1, &dims, NPY_OBJECT);
+            for( npy_intp j = 0; j < dims; j++ )
+            {
+                int timeMs = ((int*)arrayField->buffers[1])[j + static_cast<size_t>(arrayField->offset)];
+                PyObject* subObj = PyTime_FromTime((timeMs / 1000) / 3600,
+                                                   ((timeMs / 1000) % 3600) / 60,
+                                                   ((timeMs / 1000) % 3600) % 60,
+                                                   (timeMs % 1000) * 1000);
+                memcpy(PyArray_GETPTR1((PyArrayObject *) numpyArray, j),
+                       &subObj,
+                       sizeof(PyObject*));
+            }
+#endif
+        }
+        else if( strcmp(arrowType, "ttu") == 0 &&
+                 schemaField->n_children == 0 )
+        {
+            // Time(64) in microseconds
+            if( arrayField->n_buffers != 2 )
+            {
+                CPLError(CE_Failure, CPLE_AppDefined,
+                         "Field %s: arrayField->n_buffers != 2",
+                         schemaField->name);
+                Py_DECREF(dict);
+                Py_RETURN_NONE;
+            }
+
+            // create array
+            numpyArray = PyArray_SimpleNew(1, &dims, NPY_OBJECT);
+            for( npy_intp j = 0; j < dims; j++ )
+            {
+                const int64_t timeUs = ((int64_t*)arrayField->buffers[1])[j + static_cast<size_t>(arrayField->offset)];
+                PyObject* subObj = PyTime_FromTime(static_cast<int>((timeUs / 1000000) / 3600),
+                                                   static_cast<int>(((timeUs / 1000000) % 3600) / 60),
+                                                   static_cast<int>(((timeUs / 1000000) % 3600) % 60),
+                                                   static_cast<int>(timeUs % 1000000));
+                memcpy(PyArray_GETPTR1((PyArrayObject *) numpyArray, j),
+                       &subObj,
+                       sizeof(PyObject*));
+            }
+        }
+        else if( (strncmp(arrowType, "tsm:", 4) == 0 || // DateTime in milliseconds
+                  strncmp(arrowType, "tsu:", 4) == 0) &&  // DateTime in microseconds
+                 schemaField->n_children == 0 )
+        {
+            // DateTime(64) in milliseconds
+            if( arrayField->n_buffers != 2 )
+            {
+                CPLError(CE_Failure, CPLE_AppDefined,
+                         "Field %s: arrayField->n_buffers != 2",
+                         schemaField->name);
+                Py_DECREF(dict);
+                Py_RETURN_NONE;
+            }
+
+            // create the dtype string
+            PyObject *pDTypeString = PyUnicode_FromString(
+                strncmp(arrowType, "tsm:", 4) == 0 ? "datetime64[ms]" :
+                                                     "datetime64[us]");
+            // out type description object
+            PyArray_Descr *pDescr = NULL;
+            PyArray_DescrConverter(pDTypeString, &pDescr);
+            Py_DECREF(pDTypeString);
+            CPLAssert(pDescr);
+
+            // create array
+            numpyArray = PyArray_NewFromDescr(
+                        &PyArray_Type, pDescr, 1, &dims, NULL,
+                        (int64_t*)arrayField->buffers[1] + static_cast<size_t>(arrayField->offset), 0, NULL);
+
+            /* Keep a reference to the owner object */
+#if NPY_API_VERSION >= 0x00000007
+            PyArray_SetBaseObject((PyArrayObject *) numpyArray, pointerArrayKeeper);
+#else
+            PyArray_BASE((PyArrayObject *) numpyArray) = pointerArrayKeeper;
+#endif
+            Py_INCREF(pointerArrayKeeper);
+        }
+        else
+        {
+            CPLError(CE_Warning, CPLE_AppDefined,
+                     "Field %s: Unhandled arrow type: %s",
+                     schemaField->name,
+                     arrowType);
+        }
+
+        if( numpyArray )
+        {
+            const uint8_t* panNotNulls = (const uint8_t*)arrayField->buffers[0];
+            if( panNotNulls && arrayField->null_count != 0 )
+            {
+                PyObject* maskArray = PyArray_SimpleNew(1, &dims, NPY_BOOL);
+                for( npy_intp j = 0; j < dims; j++ )
+                {
+                    size_t srcOffset = static_cast<size_t>(arrayField->offset + j);
+                    // Inverse convention between arrow not-null bitmap, where
+                    // 1 means valid, and numpy masks where 1 means invalid
+                    *(char*)PyArray_GETPTR1((PyArrayObject *) maskArray, j) =
+                        ((panNotNulls[srcOffset / 8] & (1 << (srcOffset%8))) == 0) ? 1 : 0;
+                }
+                PyObject *subdict = PyDict_New();
+                PyDict_SetItemString( subdict, "mask", maskArray );
+                PyDict_SetItemString( subdict, "data", numpyArray );
+                PyDict_SetItemString( dict, schemaField->name, subdict);
+                Py_DECREF(maskArray);
+                Py_DECREF(subdict);
+            }
+            else
+            {
+                PyDict_SetItemString( dict, schemaField->name, numpyArray );
+            }
+            Py_DECREF(numpyArray);
+        }
+    }
+    return dict;
+}
+
+
+
     void VirtualMemGetArray(CPLVirtualMemShadow* virtualmem, CPLVirtualMemShadow** pvirtualmem, int numpytypemap)
     {
         *pvirtualmem = virtualmem;
     }
 
 
   // need different functions for read and write
@@ -5560,14 +6233,38 @@
       free((void*) arg7);
     }
   }
   return NULL;
 }
 
 
+SWIGINTERN PyObject *_wrap__RecordBatchAsNumpy(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0;
+  VoidPtrAsLong arg1 = (VoidPtrAsLong) 0 ;
+  VoidPtrAsLong arg2 = (VoidPtrAsLong) 0 ;
+  PyObject *arg3 = (PyObject *) 0 ;
+  PyObject *swig_obj[3] ;
+  PyObject *result = 0 ;
+  
+  if (!SWIG_Python_UnpackTuple(args, "_RecordBatchAsNumpy", 3, 3, swig_obj)) SWIG_fail;
+  {
+    arg1 = PyLong_AsVoidPtr(swig_obj[0]);
+  }
+  {
+    arg2 = PyLong_AsVoidPtr(swig_obj[1]);
+  }
+  arg3 = swig_obj[2];
+  result = (PyObject *)_RecordBatchAsNumpy(arg1,arg2,arg3);
+  resultobj = result;
+  return resultobj;
+fail:
+  return NULL;
+}
+
+
 SWIGINTERN PyObject *_wrap_VirtualMemGetArray(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
   CPLVirtualMemShadow *arg1 = (CPLVirtualMemShadow *) 0 ;
   CPLVirtualMemShadow **arg2 = (CPLVirtualMemShadow **) 0 ;
   int arg3 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
@@ -5891,14 +6588,15 @@
 	 { "TermProgress_nocb", (PyCFunction)(void(*)(void))_wrap_TermProgress_nocb, METH_VARARGS|METH_KEYWORDS, "TermProgress_nocb(double dfProgress, char const * pszMessage=None, void * pData=None) -> int"},
 	 { "OpenNumPyArray", _wrap_OpenNumPyArray, METH_VARARGS, "OpenNumPyArray(PyArrayObject * psArray, bool binterleave) -> Dataset"},
 	 { "OpenMultiDimensionalNumPyArray", _wrap_OpenMultiDimensionalNumPyArray, METH_O, "OpenMultiDimensionalNumPyArray(PyArrayObject * psArray) -> Dataset"},
 	 { "GetArrayFilename", _wrap_GetArrayFilename, METH_O, "GetArrayFilename(PyArrayObject * psArray) -> retStringAndCPLFree *"},
 	 { "BandRasterIONumPy", (PyCFunction)(void(*)(void))_wrap_BandRasterIONumPy, METH_VARARGS|METH_KEYWORDS, "BandRasterIONumPy(Band band, int bWrite, double xoff, double yoff, double xsize, double ysize, PyArrayObject * psArray, GDALDataType buf_type, GDALRIOResampleAlg resample_alg, GDALProgressFunc callback=0, void * callback_data=None) -> CPLErr"},
 	 { "DatasetIONumPy", (PyCFunction)(void(*)(void))_wrap_DatasetIONumPy, METH_VARARGS|METH_KEYWORDS, "DatasetIONumPy(Dataset ds, int bWrite, double xoff, double yoff, double xsize, double ysize, PyArrayObject * psArray, GDALDataType buf_type, GDALRIOResampleAlg resample_alg, GDALProgressFunc callback=0, void * callback_data=None, bool binterleave=True, int band_list=0) -> CPLErr"},
 	 { "MDArrayIONumPy", _wrap_MDArrayIONumPy, METH_VARARGS, "MDArrayIONumPy(bool bWrite, GDALMDArrayHS * mdarray, PyArrayObject * psArray, int nDims1, int nDims3, GDALExtendedDataTypeHS * buffer_datatype) -> CPLErr"},
+	 { "_RecordBatchAsNumpy", _wrap__RecordBatchAsNumpy, METH_VARARGS, "_RecordBatchAsNumpy(VoidPtrAsLong recordBatchPtr, VoidPtrAsLong schemaPtr, PyObject * pointerArrayKeeper) -> PyObject *"},
 	 { "VirtualMemGetArray", _wrap_VirtualMemGetArray, METH_O, "VirtualMemGetArray(VirtualMem virtualmem)"},
 	 { "RATValuesIONumPyWrite", (PyCFunction)(void(*)(void))_wrap_RATValuesIONumPyWrite, METH_VARARGS|METH_KEYWORDS, "RATValuesIONumPyWrite(RasterAttributeTable poRAT, int nField, int nStart, PyArrayObject * psArray) -> CPLErr"},
 	 { "RATValuesIONumPyRead", (PyCFunction)(void(*)(void))_wrap_RATValuesIONumPyRead, METH_VARARGS|METH_KEYWORDS, "RATValuesIONumPyRead(RasterAttributeTable poRAT, int nField, int nStart, int nLength) -> PyObject *"},
 	 { NULL, NULL, 0, NULL }
 };
 
 static PyMethodDef SwigMethods_proxydocs[] = {
@@ -6716,14 +7414,15 @@
   SwigPyBuiltin_AddPublicSymbol(public_interface, swig_const_table[i].name);
 #endif
   
   SWIG_InstallConstants(d,swig_const_table);
   
   
   import_array();
+  PyDateTime_IMPORT;
   GDALRegister_NUMPY();
   
   
   
   /* Initialize threading */
   SWIG_PYTHON_INITIALIZE_THREADS;
 #if PY_VERSION_HEX >= 0x03000000
```

### Comparing `pygdal-3.5.3.11/extensions/gdal_wrap.cpp` & `pygdal-3.6.4.11/extensions/gdal_wrap.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -2720,58 +2720,59 @@
 #define SWIGTYPE_p_GDALMultiDimInfoOptions swig_types[23]
 #define SWIGTYPE_p_GDALMultiDimTranslateOptions swig_types[24]
 #define SWIGTYPE_p_GDALNearblackOptions swig_types[25]
 #define SWIGTYPE_p_GDALProgressFunc swig_types[26]
 #define SWIGTYPE_p_GDALRasterAttributeTableShadow swig_types[27]
 #define SWIGTYPE_p_GDALRasterBandShadow swig_types[28]
 #define SWIGTYPE_p_GDALRasterizeOptions swig_types[29]
-#define SWIGTYPE_p_GDALTransformerInfoShadow swig_types[30]
-#define SWIGTYPE_p_GDALTranslateOptions swig_types[31]
-#define SWIGTYPE_p_GDALVectorTranslateOptions swig_types[32]
-#define SWIGTYPE_p_GDALViewshedMode swig_types[33]
-#define SWIGTYPE_p_GDALViewshedOutputType swig_types[34]
-#define SWIGTYPE_p_GDALWarpAppOptions swig_types[35]
-#define SWIGTYPE_p_GDAL_GCP swig_types[36]
-#define SWIGTYPE_p_GIntBig swig_types[37]
-#define SWIGTYPE_p_GUIntBig swig_types[38]
-#define SWIGTYPE_p_OGRFeatureShadow swig_types[39]
-#define SWIGTYPE_p_OGRFieldDomainShadow swig_types[40]
-#define SWIGTYPE_p_OGRGeometryShadow swig_types[41]
-#define SWIGTYPE_p_OGRLayerShadow swig_types[42]
-#define SWIGTYPE_p_OGRStyleTableShadow swig_types[43]
-#define SWIGTYPE_p_OSRSpatialReferenceShadow swig_types[44]
-#define SWIGTYPE_p_StatBuf swig_types[45]
-#define SWIGTYPE_p_Statistics swig_types[46]
-#define SWIGTYPE_p_VSIDIR swig_types[47]
-#define SWIGTYPE_p_VSILFILE swig_types[48]
-#define SWIGTYPE_p_char swig_types[49]
-#define SWIGTYPE_p_double swig_types[50]
-#define SWIGTYPE_p_f_double_p_q_const__char_p_void__int swig_types[51]
-#define SWIGTYPE_p_int swig_types[52]
-#define SWIGTYPE_p_p_GByte swig_types[53]
-#define SWIGTYPE_p_p_GDALDatasetShadow swig_types[54]
-#define SWIGTYPE_p_p_GDALDimensionHS swig_types[55]
-#define SWIGTYPE_p_p_GDALEDTComponentHS swig_types[56]
-#define SWIGTYPE_p_p_GDALRasterBandShadow swig_types[57]
-#define SWIGTYPE_p_p_GDAL_GCP swig_types[58]
-#define SWIGTYPE_p_p_GUIntBig swig_types[59]
-#define SWIGTYPE_p_p_OGRLayerShadow swig_types[60]
-#define SWIGTYPE_p_p_OSRSpatialReferenceShadow swig_types[61]
-#define SWIGTYPE_p_p_char swig_types[62]
-#define SWIGTYPE_p_p_double swig_types[63]
-#define SWIGTYPE_p_p_int swig_types[64]
-#define SWIGTYPE_p_p_p_GDALAttributeHS swig_types[65]
-#define SWIGTYPE_p_p_p_GDALDimensionHS swig_types[66]
-#define SWIGTYPE_p_p_p_GDALEDTComponentHS swig_types[67]
-#define SWIGTYPE_p_p_p_GDALMDArrayHS swig_types[68]
-#define SWIGTYPE_p_p_void swig_types[69]
-#define SWIGTYPE_p_size_t swig_types[70]
-#define SWIGTYPE_p_vsi_l_offset swig_types[71]
-static swig_type_info *swig_types[73];
-static swig_module_info swig_module = {swig_types, 72, 0, 0, 0, 0};
+#define SWIGTYPE_p_GDALRelationshipShadow swig_types[30]
+#define SWIGTYPE_p_GDALTransformerInfoShadow swig_types[31]
+#define SWIGTYPE_p_GDALTranslateOptions swig_types[32]
+#define SWIGTYPE_p_GDALVectorTranslateOptions swig_types[33]
+#define SWIGTYPE_p_GDALViewshedMode swig_types[34]
+#define SWIGTYPE_p_GDALViewshedOutputType swig_types[35]
+#define SWIGTYPE_p_GDALWarpAppOptions swig_types[36]
+#define SWIGTYPE_p_GDAL_GCP swig_types[37]
+#define SWIGTYPE_p_GIntBig swig_types[38]
+#define SWIGTYPE_p_GUIntBig swig_types[39]
+#define SWIGTYPE_p_OGRFeatureShadow swig_types[40]
+#define SWIGTYPE_p_OGRFieldDomainShadow swig_types[41]
+#define SWIGTYPE_p_OGRGeometryShadow swig_types[42]
+#define SWIGTYPE_p_OGRLayerShadow swig_types[43]
+#define SWIGTYPE_p_OGRStyleTableShadow swig_types[44]
+#define SWIGTYPE_p_OSRSpatialReferenceShadow swig_types[45]
+#define SWIGTYPE_p_StatBuf swig_types[46]
+#define SWIGTYPE_p_Statistics swig_types[47]
+#define SWIGTYPE_p_VSIDIR swig_types[48]
+#define SWIGTYPE_p_VSILFILE swig_types[49]
+#define SWIGTYPE_p_char swig_types[50]
+#define SWIGTYPE_p_double swig_types[51]
+#define SWIGTYPE_p_f_double_p_q_const__char_p_void__int swig_types[52]
+#define SWIGTYPE_p_int swig_types[53]
+#define SWIGTYPE_p_p_GByte swig_types[54]
+#define SWIGTYPE_p_p_GDALDatasetShadow swig_types[55]
+#define SWIGTYPE_p_p_GDALDimensionHS swig_types[56]
+#define SWIGTYPE_p_p_GDALEDTComponentHS swig_types[57]
+#define SWIGTYPE_p_p_GDALRasterBandShadow swig_types[58]
+#define SWIGTYPE_p_p_GDAL_GCP swig_types[59]
+#define SWIGTYPE_p_p_GUIntBig swig_types[60]
+#define SWIGTYPE_p_p_OGRLayerShadow swig_types[61]
+#define SWIGTYPE_p_p_OSRSpatialReferenceShadow swig_types[62]
+#define SWIGTYPE_p_p_char swig_types[63]
+#define SWIGTYPE_p_p_double swig_types[64]
+#define SWIGTYPE_p_p_int swig_types[65]
+#define SWIGTYPE_p_p_p_GDALAttributeHS swig_types[66]
+#define SWIGTYPE_p_p_p_GDALDimensionHS swig_types[67]
+#define SWIGTYPE_p_p_p_GDALEDTComponentHS swig_types[68]
+#define SWIGTYPE_p_p_p_GDALMDArrayHS swig_types[69]
+#define SWIGTYPE_p_p_void swig_types[70]
+#define SWIGTYPE_p_size_t swig_types[71]
+#define SWIGTYPE_p_vsi_l_offset swig_types[72]
+static swig_type_info *swig_types[74];
+static swig_module_info swig_module = {swig_types, 73, 0, 0, 0, 0};
 #define SWIG_TypeQuery(name) SWIG_TypeQueryModule(&swig_module, &swig_module, name)
 #define SWIG_MangledTypeQuery(name) SWIG_MangledTypeQueryModule(&swig_module, &swig_module, name)
 
 /* -------- TYPES TABLE (END) -------- */
 
 #ifdef SWIG_TypeQuery
 # undef SWIG_TypeQuery
@@ -2895,14 +2896,15 @@
 typedef void GDALDriverShadow;
 typedef void GDALDatasetShadow;
 typedef void GDALRasterBandShadow;
 typedef void GDALColorTableShadow;
 typedef void GDALRasterAttributeTableShadow;
 typedef void GDALTransformerInfoShadow;
 typedef void GDALAsyncReaderShadow;
+typedef void GDALRelationshipShadow;
 
 typedef GDALExtendedDataTypeHS GDALExtendedDataTypeHS;
 typedef GDALEDTComponentHS GDALEDTComponentHS;
 typedef GDALGroupHS GDALGroupHS;
 typedef GDALMDArrayHS GDALMDArrayHS;
 typedef GDALAttributeHS GDALAttributeHS;
 typedef GDALDimensionHS GDALDimensionHS;
@@ -3638,15 +3640,15 @@
 PyProgressProxy( double dfComplete, const char *pszMessage, void *pData )
 
 {
     PyProgressData *psInfo = (PyProgressData *) pData;
     PyObject *psArgs, *psResult;
     int      bContinue = TRUE;
 
-    if( psInfo->nLastReported == (int) (100.0 * dfComplete) )
+    if( dfComplete > 0 && psInfo->nLastReported == (int) (100.0 * dfComplete) )
         return TRUE;
 
     if( psInfo->psPyCallback == NULL || psInfo->psPyCallback == Py_None )
         return TRUE;
 
     psInfo->nLastReported = (int) (100.0 * dfComplete);
 
@@ -4009,23 +4011,37 @@
 }
 const char *wrapper_CPLGetThreadLocalConfigOption( const char * pszKey, const char * pszDefault = NULL )
 {
     return CPLGetThreadLocalConfigOption( pszKey, pszDefault );
 }
 
 
+void wrapper_VSISetCredential( const char* pszPathPrefix, const char * pszKey, const char * pszValue )
+{
+    VSISetPathSpecificOption(pszPathPrefix, pszKey, pszValue);
+}
+
 const char *wrapper_VSIGetCredential( const char* pszPathPrefix, const char * pszKey, const char * pszDefault = NULL )
 {
-    return VSIGetCredential( pszPathPrefix, pszKey, pszDefault );
+    return VSIGetPathSpecificOption( pszPathPrefix, pszKey, pszDefault );
+}
+
+const char *wrapper_VSIGetPathSpecificOption( const char* pszPathPrefix, const char * pszKey, const char * pszDefault = NULL )
+{
+    return VSIGetPathSpecificOption( pszPathPrefix, pszKey, pszDefault );
 }
 
 
 void wrapper_VSIClearCredentials(const char * pszPathPrefix = NULL)
 {
-    VSIClearCredentials( pszPathPrefix );
+    VSIClearPathSpecificOptions( pszPathPrefix );
+}
+void wrapper_VSIClearPathSpecificOptions(const char * pszPathPrefix = NULL)
+{
+    VSIClearPathSpecificOptions( pszPathPrefix );
 }
 
 
 void wrapper_VSIFileFromMemBuffer( const char* utf8_path, GIntBig nBytes, const char *pabyData)
 {
     const size_t nSize = static_cast<size_t>(nBytes);
     void* pabyDataDup = VSIMalloc(nSize);
@@ -4693,24 +4709,25 @@
         return NULL;
     }
     Py_DECREF(o);
   }
   return ret;
 }
 
-SWIGINTERN int GDALDatasetShadow_BuildOverviews(GDALDatasetShadow *self,char const *resampling="NEAREST",int overviewlist=0,int *pOverviews=0,GDALProgressFunc callback=NULL,void *callback_data=NULL){
+SWIGINTERN int GDALDatasetShadow_BuildOverviews(GDALDatasetShadow *self,char const *resampling="NEAREST",int overviewlist=0,int *pOverviews=0,GDALProgressFunc callback=NULL,void *callback_data=NULL,char **options=NULL){
 
-    return GDALBuildOverviews(  self,
+    return GDALBuildOverviewsEx(  self,
                                 resampling ? resampling : "NEAREST",
                                 overviewlist,
                                 pOverviews,
                                 0,
                                 0,
                                 callback,
-                                callback_data);
+                                callback_data,
+                                options);
   }
 SWIGINTERN int GDALDatasetShadow_GetGCPCount(GDALDatasetShadow *self){
     return GDALGetGCPCount( self );
   }
 SWIGINTERN char const *GDALDatasetShadow_GetGCPProjection(GDALDatasetShadow *self){
     return GDALGetGCPProjection( self );
   }
@@ -5086,14 +5103,29 @@
   }
 SWIGINTERN bool GDALDatasetShadow_DeleteFieldDomain(GDALDatasetShadow *self,char const *name){
       return GDALDatasetDeleteFieldDomain(self, name, NULL);
   }
 SWIGINTERN bool GDALDatasetShadow_UpdateFieldDomain(GDALDatasetShadow *self,OGRFieldDomainShadow *fieldDomain){
       return GDALDatasetUpdateFieldDomain(self, (OGRFieldDomainH)fieldDomain, NULL);
   }
+SWIGINTERN char **GDALDatasetShadow_GetRelationshipNames(GDALDatasetShadow *self,char **options=0){
+    return GDALDatasetGetRelationshipNames(self, options);
+  }
+SWIGINTERN GDALRelationshipShadow *GDALDatasetShadow_GetRelationship(GDALDatasetShadow *self,char const *name){
+    return (GDALRelationshipShadow*) GDALDatasetGetRelationship(self, name);
+  }
+SWIGINTERN bool GDALDatasetShadow_AddRelationship(GDALDatasetShadow *self,GDALRelationshipShadow *relationship){
+      return GDALDatasetAddRelationship(self, (GDALRelationshipH)relationship, NULL);
+  }
+SWIGINTERN bool GDALDatasetShadow_DeleteRelationship(GDALDatasetShadow *self,char const *name){
+      return GDALDatasetDeleteRelationship(self, name, NULL);
+  }
+SWIGINTERN bool GDALDatasetShadow_UpdateRelationship(GDALDatasetShadow *self,GDALRelationshipShadow *relationship){
+      return GDALDatasetUpdateRelationship(self, (GDALRelationshipH)relationship, NULL);
+  }
 SWIGINTERN CPLErr GDALDatasetShadow_ReadRaster1(GDALDatasetShadow *self,double xoff,double yoff,double xsize,double ysize,void **buf,int *buf_xsize=0,int *buf_ysize=0,GDALDataType *buf_type=0,int band_list=0,int *pband_list=0,GIntBig *buf_pixel_space=0,GIntBig *buf_line_space=0,GIntBig *buf_band_space=0,GDALRIOResampleAlg resample_alg=GRIORA_NearestNeighbour,GDALProgressFunc callback=NULL,void *callback_data=NULL,void *inputOutputBuf=NULL){
     *buf = NULL;
 
     int nxsize = (buf_xsize==0) ? xsize : *buf_xsize;
     int nysize = (buf_ysize==0) ? ysize : *buf_ysize;
     GDALDataType ntype;
     if ( buf_type != 0 ) {
@@ -6355,15 +6387,15 @@
     if (min) *min = 0;
     if (max) *max = 0;
     if (mean) *mean = 0;
     if (stddev) *stddev = -1; /* This is the only way to recognize from Python if GetRasterStatistics() has updated the values */
     return GDALGetRasterStatistics( self, approx_ok, force,
 				    min, max, mean, stddev );
   }
-SWIGINTERN CPLErr GDALRasterBandShadow_ComputeStatistics(GDALRasterBandShadow *self,bool approx_ok,double *min=NULL,double *max=NULL,double *mean=NULL,double *stddev=NULL,GDALProgressFunc callback=NULL,void *callback_data=NULL){
+SWIGINTERN CPLErr GDALRasterBandShadow_ComputeStatistics(GDALRasterBandShadow *self,bool approx_ok,double *min,double *max,double *mean,double *stddev,GDALProgressFunc callback=NULL,void *callback_data=NULL){
     return GDALComputeRasterStatistics( self, approx_ok, min, max, mean, stddev, callback, callback_data );
   }
 SWIGINTERN CPLErr GDALRasterBandShadow_SetStatistics(GDALRasterBandShadow *self,double min,double max,double mean,double stddev){
     return GDALSetRasterStatistics( self, min, max, mean, stddev );
   }
 SWIGINTERN int GDALRasterBandShadow_GetOverviewCount(GDALRasterBandShadow *self){
     return GDALGetOverviewCount(self);
@@ -6372,16 +6404,22 @@
     return (GDALRasterBandShadow*) GDALGetOverview( self, i );
   }
 SWIGINTERN int GDALRasterBandShadow_Checksum(GDALRasterBandShadow *self,int xoff=0,int yoff=0,int *xsize=0,int *ysize=0){
     int nxsize = (xsize!=0) ? *xsize : GDALGetRasterBandXSize( self );
     int nysize = (ysize!=0) ? *ysize : GDALGetRasterBandYSize( self );
     return GDALChecksumImage( self, xoff, yoff, nxsize, nysize );
   }
-SWIGINTERN void GDALRasterBandShadow_ComputeRasterMinMax(GDALRasterBandShadow *self,double argout[2],int approx_ok=0){
-    GDALComputeRasterMinMax( self, approx_ok, argout );
+SWIGINTERN void GDALRasterBandShadow_ComputeRasterMinMax(GDALRasterBandShadow *self,double argout[2],int *isvalid,bool approx_ok=false,bool can_return_none=false){
+    *isvalid = GDALComputeRasterMinMax( self, approx_ok, argout ) == CE_None;
+    if( !can_return_none && !*isvalid )
+    {
+        *isvalid = true;
+        argout[0] = CPLAtof("nan");
+        argout[1] = CPLAtof("nan");
+    }
   }
 SWIGINTERN void GDALRasterBandShadow_ComputeBandStats(GDALRasterBandShadow *self,double argout[2],int samplestep=1){
     GDALComputeBandStats( self, samplestep, argout+0, argout+1,
                           NULL, NULL );
   }
 SWIGINTERN CPLErr GDALRasterBandShadow_Fill(GDALRasterBandShadow *self,double real_fill,double imag_fill=0.0){
     return GDALFillRaster( self, real_fill, imag_fill );
@@ -6743,14 +6781,90 @@
     }
 SWIGINTERN void GDALRasterAttributeTableShadow_SetTableType(GDALRasterAttributeTableShadow *self,GDALRATTableType eTableType){
         GDALRATSetTableType( self, eTableType );
     }
 SWIGINTERN GDALRATTableType GDALRasterAttributeTableShadow_GetTableType(GDALRasterAttributeTableShadow *self){
         return GDALRATGetTableType( self );
     }
+SWIGINTERN GDALRelationshipShadow *new_GDALRelationshipShadow(char const *name,char const *leftTableName,char const *rightTableName,GDALRelationshipCardinality cardinality){
+        return (GDALRelationshipShadow*)
+        GDALRelationshipCreate(name,
+                               leftTableName,
+                               rightTableName,
+                               cardinality);
+    }
+SWIGINTERN void delete_GDALRelationshipShadow(GDALRelationshipShadow *self){
+        GDALDestroyRelationship(self);
+    }
+SWIGINTERN char const *GDALRelationshipShadow_GetName(GDALRelationshipShadow *self){
+        return GDALRelationshipGetName( self );
+    }
+SWIGINTERN GDALRelationshipCardinality GDALRelationshipShadow_GetCardinality(GDALRelationshipShadow *self){
+        return GDALRelationshipGetCardinality( self );
+    }
+SWIGINTERN char const *GDALRelationshipShadow_GetLeftTableName(GDALRelationshipShadow *self){
+        return GDALRelationshipGetLeftTableName( self );
+    }
+SWIGINTERN char const *GDALRelationshipShadow_GetRightTableName(GDALRelationshipShadow *self){
+        return GDALRelationshipGetRightTableName( self );
+    }
+SWIGINTERN char const *GDALRelationshipShadow_GetMappingTableName(GDALRelationshipShadow *self){
+        return GDALRelationshipGetMappingTableName( self );
+    }
+SWIGINTERN void GDALRelationshipShadow_SetMappingTableName(GDALRelationshipShadow *self,char const *pszName){
+        GDALRelationshipSetMappingTableName( self, pszName );
+    }
+SWIGINTERN char **GDALRelationshipShadow_GetLeftTableFields(GDALRelationshipShadow *self){
+           return GDALRelationshipGetLeftTableFields(self);
+        }
+SWIGINTERN char **GDALRelationshipShadow_GetRightTableFields(GDALRelationshipShadow *self){
+            return GDALRelationshipGetRightTableFields(self);
+        }
+SWIGINTERN void GDALRelationshipShadow_SetLeftTableFields(GDALRelationshipShadow *self,char **pFields){
+            GDALRelationshipSetLeftTableFields(self, pFields);
+        }
+SWIGINTERN void GDALRelationshipShadow_SetRightTableFields(GDALRelationshipShadow *self,char **pFields){
+            GDALRelationshipSetRightTableFields(self, pFields);
+        }
+SWIGINTERN char **GDALRelationshipShadow_GetLeftMappingTableFields(GDALRelationshipShadow *self){
+            return GDALRelationshipGetLeftMappingTableFields(self);
+        }
+SWIGINTERN char **GDALRelationshipShadow_GetRightMappingTableFields(GDALRelationshipShadow *self){
+            return GDALRelationshipGetRightMappingTableFields(self);
+        }
+SWIGINTERN void GDALRelationshipShadow_SetLeftMappingTableFields(GDALRelationshipShadow *self,char **pFields){
+          GDALRelationshipSetLeftMappingTableFields(self, pFields);
+      }
+SWIGINTERN void GDALRelationshipShadow_SetRightMappingTableFields(GDALRelationshipShadow *self,char **pFields){
+          GDALRelationshipSetRightMappingTableFields(self, pFields);
+      }
+SWIGINTERN GDALRelationshipType GDALRelationshipShadow_GetType(GDALRelationshipShadow *self){
+        return GDALRelationshipGetType( self );
+    }
+SWIGINTERN void GDALRelationshipShadow_SetType(GDALRelationshipShadow *self,GDALRelationshipType type){
+      return GDALRelationshipSetType( self, type );
+    }
+SWIGINTERN char const *GDALRelationshipShadow_GetForwardPathLabel(GDALRelationshipShadow *self){
+        return GDALRelationshipGetForwardPathLabel( self );
+    }
+SWIGINTERN void GDALRelationshipShadow_SetForwardPathLabel(GDALRelationshipShadow *self,char const *pszLabel){
+        GDALRelationshipSetForwardPathLabel( self, pszLabel );
+    }
+SWIGINTERN char const *GDALRelationshipShadow_GetBackwardPathLabel(GDALRelationshipShadow *self){
+        return GDALRelationshipGetBackwardPathLabel( self );
+    }
+SWIGINTERN void GDALRelationshipShadow_SetBackwardPathLabel(GDALRelationshipShadow *self,char const *pszLabel){
+        GDALRelationshipSetBackwardPathLabel( self, pszLabel );
+    }
+SWIGINTERN char const *GDALRelationshipShadow_GetRelatedTableType(GDALRelationshipShadow *self){
+        return GDALRelationshipGetRelatedTableType( self );
+    }
+SWIGINTERN void GDALRelationshipShadow_SetRelatedTableType(GDALRelationshipShadow *self,char const *pszType){
+        GDALRelationshipSetRelatedTableType( self, pszType );
+    }
 
 #include "gdalgrid.h"
 
 #ifdef DEBUG
 typedef struct OGRLayerHS OGRLayerShadow;
 typedef struct OGRGeometryHS OGRGeometryShadow;
 #else
@@ -10500,14 +10614,88 @@
 fail:
   if (alloc1 == SWIG_NEWOBJ) delete[] buf1;
   if (alloc2 == SWIG_NEWOBJ) delete[] buf2;
   return NULL;
 }
 
 
+SWIGINTERN PyObject *_wrap_SetPathSpecificOption(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  char *arg1 = (char *) 0 ;
+  char *arg2 = (char *) 0 ;
+  char *arg3 = (char *) 0 ;
+  int res1 ;
+  char *buf1 = 0 ;
+  int alloc1 = 0 ;
+  int res2 ;
+  char *buf2 = 0 ;
+  int alloc2 = 0 ;
+  int res3 ;
+  char *buf3 = 0 ;
+  int alloc3 = 0 ;
+  PyObject *swig_obj[3] ;
+  
+  if (!SWIG_Python_UnpackTuple(args, "SetPathSpecificOption", 3, 3, swig_obj)) SWIG_fail;
+  res1 = SWIG_AsCharPtrAndSize(swig_obj[0], &buf1, NULL, &alloc1);
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "SetPathSpecificOption" "', argument " "1"" of type '" "char const *""'");
+  }
+  arg1 = reinterpret_cast< char * >(buf1);
+  res2 = SWIG_AsCharPtrAndSize(swig_obj[1], &buf2, NULL, &alloc2);
+  if (!SWIG_IsOK(res2)) {
+    SWIG_exception_fail(SWIG_ArgError(res2), "in method '" "SetPathSpecificOption" "', argument " "2"" of type '" "char const *""'");
+  }
+  arg2 = reinterpret_cast< char * >(buf2);
+  res3 = SWIG_AsCharPtrAndSize(swig_obj[2], &buf3, NULL, &alloc3);
+  if (!SWIG_IsOK(res3)) {
+    SWIG_exception_fail(SWIG_ArgError(res3), "in method '" "SetPathSpecificOption" "', argument " "3"" of type '" "char const *""'");
+  }
+  arg3 = reinterpret_cast< char * >(buf3);
+  {
+    if (!arg1) {
+      SWIG_exception(SWIG_ValueError,"Received a NULL pointer.");
+    }
+  }
+  {
+    if (!arg2) {
+      SWIG_exception(SWIG_ValueError,"Received a NULL pointer.");
+    }
+  }
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      VSISetPathSpecificOption((char const *)arg1,(char const *)arg2,(char const *)arg3);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  resultobj = SWIG_Py_Void();
+  if (alloc1 == SWIG_NEWOBJ) delete[] buf1;
+  if (alloc2 == SWIG_NEWOBJ) delete[] buf2;
+  if (alloc3 == SWIG_NEWOBJ) delete[] buf3;
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  if (alloc1 == SWIG_NEWOBJ) delete[] buf1;
+  if (alloc2 == SWIG_NEWOBJ) delete[] buf2;
+  if (alloc3 == SWIG_NEWOBJ) delete[] buf3;
+  return NULL;
+}
+
+
 SWIGINTERN PyObject *_wrap_SetCredential(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
   char *arg1 = (char *) 0 ;
   char *arg2 = (char *) 0 ;
   char *arg3 = (char *) 0 ;
   int res1 ;
   char *buf1 = 0 ;
@@ -10548,15 +10736,15 @@
   }
   {
     if ( bUseExceptions ) {
       ClearErrorState();
     }
     {
       SWIG_PYTHON_THREAD_BEGIN_ALLOW;
-      VSISetCredential((char const *)arg1,(char const *)arg2,(char const *)arg3);
+      wrapper_VSISetCredential((char const *)arg1,(char const *)arg2,(char const *)arg3);
       SWIG_PYTHON_THREAD_END_ALLOW;
     }
 #ifndef SED_HACKS
     if ( bUseExceptions ) {
       CPLErr eclass = CPLGetLastErrorType();
       if ( eclass == CE_Failure || eclass == CE_Fatal ) {
         SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
@@ -10651,14 +10839,91 @@
   if (alloc1 == SWIG_NEWOBJ) delete[] buf1;
   if (alloc2 == SWIG_NEWOBJ) delete[] buf2;
   if (alloc3 == SWIG_NEWOBJ) delete[] buf3;
   return NULL;
 }
 
 
+SWIGINTERN PyObject *_wrap_GetPathSpecificOption(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  char *arg1 = (char *) 0 ;
+  char *arg2 = (char *) 0 ;
+  char *arg3 = (char *) NULL ;
+  int res1 ;
+  char *buf1 = 0 ;
+  int alloc1 = 0 ;
+  int res2 ;
+  char *buf2 = 0 ;
+  int alloc2 = 0 ;
+  int res3 ;
+  char *buf3 = 0 ;
+  int alloc3 = 0 ;
+  PyObject *swig_obj[3] ;
+  char *result = 0 ;
+  
+  if (!SWIG_Python_UnpackTuple(args, "GetPathSpecificOption", 2, 3, swig_obj)) SWIG_fail;
+  res1 = SWIG_AsCharPtrAndSize(swig_obj[0], &buf1, NULL, &alloc1);
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "GetPathSpecificOption" "', argument " "1"" of type '" "char const *""'");
+  }
+  arg1 = reinterpret_cast< char * >(buf1);
+  res2 = SWIG_AsCharPtrAndSize(swig_obj[1], &buf2, NULL, &alloc2);
+  if (!SWIG_IsOK(res2)) {
+    SWIG_exception_fail(SWIG_ArgError(res2), "in method '" "GetPathSpecificOption" "', argument " "2"" of type '" "char const *""'");
+  }
+  arg2 = reinterpret_cast< char * >(buf2);
+  if (swig_obj[2]) {
+    res3 = SWIG_AsCharPtrAndSize(swig_obj[2], &buf3, NULL, &alloc3);
+    if (!SWIG_IsOK(res3)) {
+      SWIG_exception_fail(SWIG_ArgError(res3), "in method '" "GetPathSpecificOption" "', argument " "3"" of type '" "char const *""'");
+    }
+    arg3 = reinterpret_cast< char * >(buf3);
+  }
+  {
+    if (!arg1) {
+      SWIG_exception(SWIG_ValueError,"Received a NULL pointer.");
+    }
+  }
+  {
+    if (!arg2) {
+      SWIG_exception(SWIG_ValueError,"Received a NULL pointer.");
+    }
+  }
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      result = (char *)wrapper_VSIGetPathSpecificOption((char const *)arg1,(char const *)arg2,(char const *)arg3);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  resultobj = SWIG_FromCharPtr((const char *)result);
+  if (alloc1 == SWIG_NEWOBJ) delete[] buf1;
+  if (alloc2 == SWIG_NEWOBJ) delete[] buf2;
+  if (alloc3 == SWIG_NEWOBJ) delete[] buf3;
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  if (alloc1 == SWIG_NEWOBJ) delete[] buf1;
+  if (alloc2 == SWIG_NEWOBJ) delete[] buf2;
+  if (alloc3 == SWIG_NEWOBJ) delete[] buf3;
+  return NULL;
+}
+
+
 SWIGINTERN PyObject *_wrap_ClearCredentials(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
   char *arg1 = (char *) NULL ;
   int res1 ;
   char *buf1 = 0 ;
   int alloc1 = 0 ;
   PyObject *swig_obj[1] ;
@@ -10695,14 +10960,58 @@
   return resultobj;
 fail:
   if (alloc1 == SWIG_NEWOBJ) delete[] buf1;
   return NULL;
 }
 
 
+SWIGINTERN PyObject *_wrap_ClearPathSpecificOptions(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  char *arg1 = (char *) NULL ;
+  int res1 ;
+  char *buf1 = 0 ;
+  int alloc1 = 0 ;
+  PyObject *swig_obj[1] ;
+  
+  if (!SWIG_Python_UnpackTuple(args, "ClearPathSpecificOptions", 0, 1, swig_obj)) SWIG_fail;
+  if (swig_obj[0]) {
+    res1 = SWIG_AsCharPtrAndSize(swig_obj[0], &buf1, NULL, &alloc1);
+    if (!SWIG_IsOK(res1)) {
+      SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ClearPathSpecificOptions" "', argument " "1"" of type '" "char const *""'");
+    }
+    arg1 = reinterpret_cast< char * >(buf1);
+  }
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      wrapper_VSIClearPathSpecificOptions((char const *)arg1);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  resultobj = SWIG_Py_Void();
+  if (alloc1 == SWIG_NEWOBJ) delete[] buf1;
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  if (alloc1 == SWIG_NEWOBJ) delete[] buf1;
+  return NULL;
+}
+
+
 SWIGINTERN PyObject *_wrap_CPLBinaryToHex(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
   int arg1 ;
   GByte *arg2 = (GByte *) 0 ;
   int alloc1 = 0 ;
   bool viewIsValid1 = false ;
   Py_buffer view1 ;
@@ -13582,14 +13891,78 @@
     /* %typemap(freearg) (const char *utf8_path) */
     GDALPythonFreeCStr(arg1, bToFree1);
   }
   return NULL;
 }
 
 
+SWIGINTERN PyObject *_wrap_GetNumCPUs(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  int result;
+  
+  if (!SWIG_Python_UnpackTuple(args, "GetNumCPUs", 0, 0, 0)) SWIG_fail;
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      result = (int)CPLGetNumCPUs();
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  resultobj = SWIG_From_int(static_cast< int >(result));
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  return NULL;
+}
+
+
+SWIGINTERN PyObject *_wrap_GetUsablePhysicalRAM(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  GIntBig result;
+  
+  if (!SWIG_Python_UnpackTuple(args, "GetUsablePhysicalRAM", 0, 0, 0)) SWIG_fail;
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      result = CPLGetUsablePhysicalRAM();
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  {
+    resultobj = PyLong_FromLongLong(result);
+  }
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  return NULL;
+}
+
+
 SWIGINTERN PyObject *_wrap_MajorObject_GetDescription(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
   GDALMajorObjectShadow *arg1 = (GDALMajorObjectShadow *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   PyObject *swig_obj[1] ;
   char *result = 0 ;
@@ -18305,37 +18678,39 @@
   PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
   GDALDatasetShadow *arg1 = (GDALDatasetShadow *) 0 ;
   char *arg2 = (char *) "NEAREST" ;
   int arg3 = (int) 0 ;
   int *arg4 = (int *) 0 ;
   GDALProgressFunc arg5 = (GDALProgressFunc) NULL ;
   void *arg6 = (void *) NULL ;
+  char **arg7 = (char **) NULL ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   int res2 ;
   char *buf2 = 0 ;
   int alloc2 = 0 ;
   PyObject * obj0 = 0 ;
   PyObject * obj1 = 0 ;
   PyObject * obj2 = 0 ;
   PyObject * obj3 = 0 ;
   PyObject * obj4 = 0 ;
+  PyObject * obj5 = 0 ;
   char * kwnames[] = {
-    (char *)"self",  (char *)"resampling",  (char *)"overviewlist",  (char *)"callback",  (char *)"callback_data",  NULL 
+    (char *)"self",  (char *)"resampling",  (char *)"overviewlist",  (char *)"callback",  (char *)"callback_data",  (char *)"options",  NULL 
   };
   int result;
   
   /* %typemap(arginit) ( const char* callback_data=NULL)  */
   PyProgressData *psProgressInfo;
   psProgressInfo = (PyProgressData *) CPLCalloc(1,sizeof(PyProgressData));
   psProgressInfo->nLastReported = -1;
   psProgressInfo->psPyCallback = NULL;
   psProgressInfo->psPyCallbackData = NULL;
   arg6 = psProgressInfo;
-  if (!PyArg_ParseTupleAndKeywords(args, kwargs, "O|OOOO:Dataset_BuildOverviews", kwnames, &obj0, &obj1, &obj2, &obj3, &obj4)) SWIG_fail;
+  if (!PyArg_ParseTupleAndKeywords(args, kwargs, "O|OOOOO:Dataset_BuildOverviews", kwnames, &obj0, &obj1, &obj2, &obj3, &obj4, &obj5)) SWIG_fail;
   res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_GDALDatasetShadow, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "Dataset_BuildOverviews" "', argument " "1"" of type '" "GDALDatasetShadow *""'"); 
   }
   arg1 = reinterpret_cast< GDALDatasetShadow * >(argp1);
   if (obj1) {
     res2 = SWIG_AsCharPtrAndSize(obj1, &buf2, NULL, &alloc2);
@@ -18393,21 +18768,32 @@
   }
   if (obj4) {
     {
       /* %typemap(in) ( void* callback_data=NULL)  */
       psProgressInfo->psPyCallbackData = obj4 ;
     }
   }
+  if (obj5) {
+    {
+      /* %typemap(in) char **options */
+      int bErr = FALSE;
+      arg7 = CSLFromPySequence(obj5, &bErr);
+      if( bErr )
+      {
+        SWIG_fail;
+      }
+    }
+  }
   {
     if ( bUseExceptions ) {
       ClearErrorState();
     }
     {
       SWIG_PYTHON_THREAD_BEGIN_ALLOW;
-      result = (int)GDALDatasetShadow_BuildOverviews(arg1,(char const *)arg2,arg3,arg4,arg5,arg6);
+      result = (int)GDALDatasetShadow_BuildOverviews(arg1,(char const *)arg2,arg3,arg4,arg5,arg6,arg7);
       SWIG_PYTHON_THREAD_END_ALLOW;
     }
 #ifndef SED_HACKS
     if ( bUseExceptions ) {
       CPLErr eclass = CPLGetLastErrorType();
       if ( eclass == CE_Failure || eclass == CE_Fatal ) {
         SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
@@ -18423,28 +18809,36 @@
   }
   {
     /* %typemap(freearg) ( void* callback_data=NULL)  */
     
     CPLFree(psProgressInfo);
     
   }
+  {
+    /* %typemap(freearg) char **options */
+    CSLDestroy( arg7 );
+  }
   if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
   return resultobj;
 fail:
   if (alloc2 == SWIG_NEWOBJ) delete[] buf2;
   {
     /* %typemap(freearg) (int nList, int* pList) */
     free(arg4);
   }
   {
     /* %typemap(freearg) ( void* callback_data=NULL)  */
     
     CPLFree(psProgressInfo);
     
   }
+  {
+    /* %typemap(freearg) char **options */
+    CSLDestroy( arg7 );
+  }
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_Dataset_GetGCPCount(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
   GDALDatasetShadow *arg1 = (GDALDatasetShadow *) 0 ;
@@ -21590,14 +21984,308 @@
   if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
   return resultobj;
 fail:
   return NULL;
 }
 
 
+SWIGINTERN PyObject *_wrap_Dataset_GetRelationshipNames(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  GDALDatasetShadow *arg1 = (GDALDatasetShadow *) 0 ;
+  char **arg2 = (char **) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  PyObject *swig_obj[2] ;
+  char **result = 0 ;
+  
+  if (!SWIG_Python_UnpackTuple(args, "Dataset_GetRelationshipNames", 1, 2, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_GDALDatasetShadow, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "Dataset_GetRelationshipNames" "', argument " "1"" of type '" "GDALDatasetShadow *""'"); 
+  }
+  arg1 = reinterpret_cast< GDALDatasetShadow * >(argp1);
+  if (swig_obj[1]) {
+    {
+      /* %typemap(in) char **options */
+      int bErr = FALSE;
+      arg2 = CSLFromPySequence(swig_obj[1], &bErr);
+      if( bErr )
+      {
+        SWIG_fail;
+      }
+    }
+  }
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      result = (char **)GDALDatasetShadow_GetRelationshipNames(arg1,arg2);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  {
+    /* %typemap(out) char **CSL -> ( string ) */
+    char **stringarray = result;
+    if ( stringarray == NULL ) {
+      resultobj = Py_None;
+      Py_INCREF( resultobj );
+    }
+    else {
+      int len = CSLCount( stringarray );
+      resultobj = PyList_New( len );
+      for ( int i = 0; i < len; ++i ) {
+        PyObject *o = GDALPythonObjectFromCStr( stringarray[i] );
+        PyList_SetItem(resultobj, i, o );
+      }
+    }
+    CSLDestroy(result);
+  }
+  {
+    /* %typemap(freearg) char **options */
+    CSLDestroy( arg2 );
+  }
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  {
+    /* %typemap(freearg) char **options */
+    CSLDestroy( arg2 );
+  }
+  return NULL;
+}
+
+
+SWIGINTERN PyObject *_wrap_Dataset_GetRelationship(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  GDALDatasetShadow *arg1 = (GDALDatasetShadow *) 0 ;
+  char *arg2 = (char *) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  int res2 ;
+  char *buf2 = 0 ;
+  int alloc2 = 0 ;
+  PyObject *swig_obj[2] ;
+  GDALRelationshipShadow *result = 0 ;
+  
+  if (!SWIG_Python_UnpackTuple(args, "Dataset_GetRelationship", 2, 2, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_GDALDatasetShadow, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "Dataset_GetRelationship" "', argument " "1"" of type '" "GDALDatasetShadow *""'"); 
+  }
+  arg1 = reinterpret_cast< GDALDatasetShadow * >(argp1);
+  res2 = SWIG_AsCharPtrAndSize(swig_obj[1], &buf2, NULL, &alloc2);
+  if (!SWIG_IsOK(res2)) {
+    SWIG_exception_fail(SWIG_ArgError(res2), "in method '" "Dataset_GetRelationship" "', argument " "2"" of type '" "char const *""'");
+  }
+  arg2 = reinterpret_cast< char * >(buf2);
+  {
+    if (!arg2) {
+      SWIG_exception(SWIG_ValueError,"Received a NULL pointer.");
+    }
+  }
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      result = (GDALRelationshipShadow *)GDALDatasetShadow_GetRelationship(arg1,(char const *)arg2);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  resultobj = SWIG_NewPointerObj(SWIG_as_voidptr(result), SWIGTYPE_p_GDALRelationshipShadow, 0 |  0 );
+  if (alloc2 == SWIG_NEWOBJ) delete[] buf2;
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  if (alloc2 == SWIG_NEWOBJ) delete[] buf2;
+  return NULL;
+}
+
+
+SWIGINTERN PyObject *_wrap_Dataset_AddRelationship(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  GDALDatasetShadow *arg1 = (GDALDatasetShadow *) 0 ;
+  GDALRelationshipShadow *arg2 = (GDALRelationshipShadow *) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  void *argp2 = 0 ;
+  int res2 = 0 ;
+  PyObject *swig_obj[2] ;
+  bool result;
+  
+  if (!SWIG_Python_UnpackTuple(args, "Dataset_AddRelationship", 2, 2, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_GDALDatasetShadow, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "Dataset_AddRelationship" "', argument " "1"" of type '" "GDALDatasetShadow *""'"); 
+  }
+  arg1 = reinterpret_cast< GDALDatasetShadow * >(argp1);
+  res2 = SWIG_ConvertPtr(swig_obj[1], &argp2,SWIGTYPE_p_GDALRelationshipShadow, 0 |  0 );
+  if (!SWIG_IsOK(res2)) {
+    SWIG_exception_fail(SWIG_ArgError(res2), "in method '" "Dataset_AddRelationship" "', argument " "2"" of type '" "GDALRelationshipShadow *""'"); 
+  }
+  arg2 = reinterpret_cast< GDALRelationshipShadow * >(argp2);
+  {
+    if (!arg2) {
+      SWIG_exception(SWIG_ValueError,"Received a NULL pointer.");
+    }
+  }
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      result = (bool)GDALDatasetShadow_AddRelationship(arg1,arg2);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  resultobj = SWIG_From_bool(static_cast< bool >(result));
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  return NULL;
+}
+
+
+SWIGINTERN PyObject *_wrap_Dataset_DeleteRelationship(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  GDALDatasetShadow *arg1 = (GDALDatasetShadow *) 0 ;
+  char *arg2 = (char *) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  int res2 ;
+  char *buf2 = 0 ;
+  int alloc2 = 0 ;
+  PyObject *swig_obj[2] ;
+  bool result;
+  
+  if (!SWIG_Python_UnpackTuple(args, "Dataset_DeleteRelationship", 2, 2, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_GDALDatasetShadow, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "Dataset_DeleteRelationship" "', argument " "1"" of type '" "GDALDatasetShadow *""'"); 
+  }
+  arg1 = reinterpret_cast< GDALDatasetShadow * >(argp1);
+  res2 = SWIG_AsCharPtrAndSize(swig_obj[1], &buf2, NULL, &alloc2);
+  if (!SWIG_IsOK(res2)) {
+    SWIG_exception_fail(SWIG_ArgError(res2), "in method '" "Dataset_DeleteRelationship" "', argument " "2"" of type '" "char const *""'");
+  }
+  arg2 = reinterpret_cast< char * >(buf2);
+  {
+    if (!arg2) {
+      SWIG_exception(SWIG_ValueError,"Received a NULL pointer.");
+    }
+  }
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      result = (bool)GDALDatasetShadow_DeleteRelationship(arg1,(char const *)arg2);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  resultobj = SWIG_From_bool(static_cast< bool >(result));
+  if (alloc2 == SWIG_NEWOBJ) delete[] buf2;
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  if (alloc2 == SWIG_NEWOBJ) delete[] buf2;
+  return NULL;
+}
+
+
+SWIGINTERN PyObject *_wrap_Dataset_UpdateRelationship(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  GDALDatasetShadow *arg1 = (GDALDatasetShadow *) 0 ;
+  GDALRelationshipShadow *arg2 = (GDALRelationshipShadow *) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  void *argp2 = 0 ;
+  int res2 = 0 ;
+  PyObject *swig_obj[2] ;
+  bool result;
+  
+  if (!SWIG_Python_UnpackTuple(args, "Dataset_UpdateRelationship", 2, 2, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_GDALDatasetShadow, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "Dataset_UpdateRelationship" "', argument " "1"" of type '" "GDALDatasetShadow *""'"); 
+  }
+  arg1 = reinterpret_cast< GDALDatasetShadow * >(argp1);
+  res2 = SWIG_ConvertPtr(swig_obj[1], &argp2,SWIGTYPE_p_GDALRelationshipShadow, 0 |  0 );
+  if (!SWIG_IsOK(res2)) {
+    SWIG_exception_fail(SWIG_ArgError(res2), "in method '" "Dataset_UpdateRelationship" "', argument " "2"" of type '" "GDALRelationshipShadow *""'"); 
+  }
+  arg2 = reinterpret_cast< GDALRelationshipShadow * >(argp2);
+  {
+    if (!arg2) {
+      SWIG_exception(SWIG_ValueError,"Received a NULL pointer.");
+    }
+  }
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      result = (bool)GDALDatasetShadow_UpdateRelationship(arg1,arg2);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  resultobj = SWIG_From_bool(static_cast< bool >(result));
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  return NULL;
+}
+
+
 SWIGINTERN PyObject *_wrap_Dataset_ReadRaster1(PyObject *SWIGUNUSEDPARM(self), PyObject *args, PyObject *kwargs) {
   PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
   GDALDatasetShadow *arg1 = (GDALDatasetShadow *) 0 ;
   double arg2 ;
   double arg3 ;
   double arg4 ;
   double arg5 ;
@@ -31148,103 +31836,109 @@
   if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
   return resultobj;
 fail:
   return NULL;
 }
 
 
-SWIGINTERN PyObject *_wrap_Band_ComputeStatistics(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+SWIGINTERN PyObject *_wrap_Band_ComputeStatistics(PyObject *SWIGUNUSEDPARM(self), PyObject *args, PyObject *kwargs) {
   PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
   GDALRasterBandShadow *arg1 = (GDALRasterBandShadow *) 0 ;
   bool arg2 ;
-  double *arg3 = (double *) NULL ;
-  double *arg4 = (double *) NULL ;
-  double *arg5 = (double *) NULL ;
-  double *arg6 = (double *) NULL ;
+  double *arg3 = (double *) 0 ;
+  double *arg4 = (double *) 0 ;
+  double *arg5 = (double *) 0 ;
+  double *arg6 = (double *) 0 ;
   GDALProgressFunc arg7 = (GDALProgressFunc) NULL ;
   void *arg8 = (void *) NULL ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   bool val2 ;
   int ecode2 = 0 ;
   double temp3 ;
   int res3 = SWIG_TMPOBJ ;
   double temp4 ;
   int res4 = SWIG_TMPOBJ ;
   double temp5 ;
   int res5 = SWIG_TMPOBJ ;
   double temp6 ;
   int res6 = SWIG_TMPOBJ ;
-  PyObject *swig_obj[4] ;
+  PyObject * obj0 = 0 ;
+  PyObject * obj1 = 0 ;
+  PyObject * obj2 = 0 ;
+  PyObject * obj3 = 0 ;
+  char * kwnames[] = {
+    (char *)"self",  (char *)"approx_ok",  (char *)"callback",  (char *)"callback_data",  NULL 
+  };
   CPLErr result;
   
   /* %typemap(arginit) ( const char* callback_data=NULL)  */
   PyProgressData *psProgressInfo;
   psProgressInfo = (PyProgressData *) CPLCalloc(1,sizeof(PyProgressData));
   psProgressInfo->nLastReported = -1;
   psProgressInfo->psPyCallback = NULL;
   psProgressInfo->psPyCallbackData = NULL;
   arg8 = psProgressInfo;
   arg3 = &temp3;
   arg4 = &temp4;
   arg5 = &temp5;
   arg6 = &temp6;
-  if (!SWIG_Python_UnpackTuple(args, "Band_ComputeStatistics", 2, 4, swig_obj)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_GDALRasterBandShadow, 0 |  0 );
+  if (!PyArg_ParseTupleAndKeywords(args, kwargs, "OO|OO:Band_ComputeStatistics", kwnames, &obj0, &obj1, &obj2, &obj3)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_GDALRasterBandShadow, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "Band_ComputeStatistics" "', argument " "1"" of type '" "GDALRasterBandShadow *""'"); 
   }
   arg1 = reinterpret_cast< GDALRasterBandShadow * >(argp1);
-  ecode2 = SWIG_AsVal_bool(swig_obj[1], &val2);
+  ecode2 = SWIG_AsVal_bool(obj1, &val2);
   if (!SWIG_IsOK(ecode2)) {
     SWIG_exception_fail(SWIG_ArgError(ecode2), "in method '" "Band_ComputeStatistics" "', argument " "2"" of type '" "bool""'");
   } 
   arg2 = static_cast< bool >(val2);
-  if (swig_obj[2]) {
+  if (obj2) {
     {
       /* %typemap(in) (GDALProgressFunc callback = NULL) */
       /* callback_func typemap */
       
       /* In some cases 0 is passed instead of None. */
       /* See https://github.com/OSGeo/gdal/pull/219 */
-      if ( PyLong_Check(swig_obj[2]) || PyInt_Check(swig_obj[2]) )
+      if ( PyLong_Check(obj2) || PyInt_Check(obj2) )
       {
-        if( PyLong_AsLong(swig_obj[2]) == 0 )
+        if( PyLong_AsLong(obj2) == 0 )
         {
-          swig_obj[2] = Py_None;
+          obj2 = Py_None;
         }
       }
       
-      if (swig_obj[2] && swig_obj[2] != Py_None ) {
+      if (obj2 && obj2 != Py_None ) {
         void* cbfunction = NULL;
-        CPL_IGNORE_RET_VAL(SWIG_ConvertPtr( swig_obj[2],
+        CPL_IGNORE_RET_VAL(SWIG_ConvertPtr( obj2,
             (void**)&cbfunction,
             SWIGTYPE_p_f_double_p_q_const__char_p_void__int,
             SWIG_POINTER_EXCEPTION | 0 ));
         
         if ( cbfunction == GDALTermProgress ) {
           arg7 = GDALTermProgress;
         } else {
-          if (!PyCallable_Check(swig_obj[2])) {
+          if (!PyCallable_Check(obj2)) {
             PyErr_SetString( PyExc_RuntimeError,
               "Object given is not a Python function" );
             SWIG_fail;
           }
-          psProgressInfo->psPyCallback = swig_obj[2];
+          psProgressInfo->psPyCallback = obj2;
           arg7 = PyProgressProxy;
         }
         
       }
       
     }
   }
-  if (swig_obj[3]) {
+  if (obj3) {
     {
       /* %typemap(in) ( void* callback_data=NULL)  */
-      psProgressInfo->psPyCallbackData = swig_obj[3] ;
+      psProgressInfo->psPyCallbackData = obj3 ;
     }
   }
   {
     if ( bUseExceptions ) {
       ClearErrorState();
     }
     {
@@ -31565,67 +32259,91 @@
   if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
   return resultobj;
 fail:
   return NULL;
 }
 
 
-SWIGINTERN PyObject *_wrap_Band_ComputeRasterMinMax(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+SWIGINTERN PyObject *_wrap_Band_ComputeRasterMinMax(PyObject *SWIGUNUSEDPARM(self), PyObject *args, PyObject *kwargs) {
   PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
   GDALRasterBandShadow *arg1 = (GDALRasterBandShadow *) 0 ;
   double *arg2 ;
-  int arg3 = (int) 0 ;
+  int *arg3 = (int *) 0 ;
+  bool arg4 = (bool) false ;
+  bool arg5 = (bool) false ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   double argout2[2] ;
-  int val3 ;
-  int ecode3 = 0 ;
-  PyObject *swig_obj[2] ;
+  int isvalid2 ;
+  bool val4 ;
+  int ecode4 = 0 ;
+  bool val5 ;
+  int ecode5 = 0 ;
+  PyObject * obj0 = 0 ;
+  PyObject * obj1 = 0 ;
+  PyObject * obj2 = 0 ;
+  char * kwnames[] = {
+    (char *)"self",  (char *)"approx_ok",  (char *)"can_return_none",  NULL 
+  };
   
   {
-    /* %typemap(in,numinputs=0) (double argout2[ANY]) */
-    memset(argout2, 0, sizeof(argout2));
+    /* %typemap(in,numinputs=0) (double argout2[2], int* isvalid2) */
     arg2 = argout2;
+    arg3 = &isvalid2;
   }
-  if (!SWIG_Python_UnpackTuple(args, "Band_ComputeRasterMinMax", 1, 2, swig_obj)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_GDALRasterBandShadow, 0 |  0 );
+  if (!PyArg_ParseTupleAndKeywords(args, kwargs, "O|OO:Band_ComputeRasterMinMax", kwnames, &obj0, &obj1, &obj2)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_GDALRasterBandShadow, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "Band_ComputeRasterMinMax" "', argument " "1"" of type '" "GDALRasterBandShadow *""'"); 
   }
   arg1 = reinterpret_cast< GDALRasterBandShadow * >(argp1);
-  if (swig_obj[1]) {
-    ecode3 = SWIG_AsVal_int(swig_obj[1], &val3);
-    if (!SWIG_IsOK(ecode3)) {
-      SWIG_exception_fail(SWIG_ArgError(ecode3), "in method '" "Band_ComputeRasterMinMax" "', argument " "3"" of type '" "int""'");
+  if (obj1) {
+    ecode4 = SWIG_AsVal_bool(obj1, &val4);
+    if (!SWIG_IsOK(ecode4)) {
+      SWIG_exception_fail(SWIG_ArgError(ecode4), "in method '" "Band_ComputeRasterMinMax" "', argument " "4"" of type '" "bool""'");
     } 
-    arg3 = static_cast< int >(val3);
+    arg4 = static_cast< bool >(val4);
+  }
+  if (obj2) {
+    ecode5 = SWIG_AsVal_bool(obj2, &val5);
+    if (!SWIG_IsOK(ecode5)) {
+      SWIG_exception_fail(SWIG_ArgError(ecode5), "in method '" "Band_ComputeRasterMinMax" "', argument " "5"" of type '" "bool""'");
+    } 
+    arg5 = static_cast< bool >(val5);
   }
   {
     if ( bUseExceptions ) {
       ClearErrorState();
     }
     {
       SWIG_PYTHON_THREAD_BEGIN_ALLOW;
-      GDALRasterBandShadow_ComputeRasterMinMax(arg1,arg2,arg3);
+      GDALRasterBandShadow_ComputeRasterMinMax(arg1,arg2,arg3,arg4,arg5);
       SWIG_PYTHON_THREAD_END_ALLOW;
     }
 #ifndef SED_HACKS
     if ( bUseExceptions ) {
       CPLErr eclass = CPLGetLastErrorType();
       if ( eclass == CE_Failure || eclass == CE_Fatal ) {
         SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
       }
     }
 #endif
   }
   resultobj = SWIG_Py_Void();
   {
-    /* %typemap(argout) (double argout[ANY]) */
-    PyObject *out = CreateTupleFromDoubleArray( arg2, 2 );
-    resultobj = t_output_helper(resultobj,out);
+    /* %typemap(argout) (double argout[2], int* isvalid)  */
+    PyObject *r;
+    if ( !*arg3 ) {
+      Py_INCREF(Py_None);
+      r = Py_None;
+    }
+    else {
+      r = CreateTupleFromDoubleArray(arg2, 2);
+    }
+    resultobj = t_output_helper(resultobj,r);
   }
   if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
   return resultobj;
 fail:
   return NULL;
 }
 
@@ -35890,14 +36608,1287 @@
   return SWIG_Py_Void();
 }
 
 SWIGINTERN PyObject *RasterAttributeTable_swiginit(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   return SWIG_Python_InitShadowInstance(args);
 }
 
+SWIGINTERN PyObject *_wrap_new_Relationship(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  char *arg1 = (char *) 0 ;
+  char *arg2 = (char *) 0 ;
+  char *arg3 = (char *) 0 ;
+  GDALRelationshipCardinality arg4 ;
+  int res1 ;
+  char *buf1 = 0 ;
+  int alloc1 = 0 ;
+  int res2 ;
+  char *buf2 = 0 ;
+  int alloc2 = 0 ;
+  int res3 ;
+  char *buf3 = 0 ;
+  int alloc3 = 0 ;
+  int val4 ;
+  int ecode4 = 0 ;
+  PyObject *swig_obj[4] ;
+  GDALRelationshipShadow *result = 0 ;
+  
+  if (!SWIG_Python_UnpackTuple(args, "new_Relationship", 4, 4, swig_obj)) SWIG_fail;
+  res1 = SWIG_AsCharPtrAndSize(swig_obj[0], &buf1, NULL, &alloc1);
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "new_Relationship" "', argument " "1"" of type '" "char const *""'");
+  }
+  arg1 = reinterpret_cast< char * >(buf1);
+  res2 = SWIG_AsCharPtrAndSize(swig_obj[1], &buf2, NULL, &alloc2);
+  if (!SWIG_IsOK(res2)) {
+    SWIG_exception_fail(SWIG_ArgError(res2), "in method '" "new_Relationship" "', argument " "2"" of type '" "char const *""'");
+  }
+  arg2 = reinterpret_cast< char * >(buf2);
+  res3 = SWIG_AsCharPtrAndSize(swig_obj[2], &buf3, NULL, &alloc3);
+  if (!SWIG_IsOK(res3)) {
+    SWIG_exception_fail(SWIG_ArgError(res3), "in method '" "new_Relationship" "', argument " "3"" of type '" "char const *""'");
+  }
+  arg3 = reinterpret_cast< char * >(buf3);
+  ecode4 = SWIG_AsVal_int(swig_obj[3], &val4);
+  if (!SWIG_IsOK(ecode4)) {
+    SWIG_exception_fail(SWIG_ArgError(ecode4), "in method '" "new_Relationship" "', argument " "4"" of type '" "GDALRelationshipCardinality""'");
+  } 
+  arg4 = static_cast< GDALRelationshipCardinality >(val4);
+  {
+    if (!arg1) {
+      SWIG_exception(SWIG_ValueError,"Received a NULL pointer.");
+    }
+  }
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      result = (GDALRelationshipShadow *)new_GDALRelationshipShadow((char const *)arg1,(char const *)arg2,(char const *)arg3,arg4);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  resultobj = SWIG_NewPointerObj(SWIG_as_voidptr(result), SWIGTYPE_p_GDALRelationshipShadow, SWIG_POINTER_NEW |  0 );
+  if (alloc1 == SWIG_NEWOBJ) delete[] buf1;
+  if (alloc2 == SWIG_NEWOBJ) delete[] buf2;
+  if (alloc3 == SWIG_NEWOBJ) delete[] buf3;
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  if (alloc1 == SWIG_NEWOBJ) delete[] buf1;
+  if (alloc2 == SWIG_NEWOBJ) delete[] buf2;
+  if (alloc3 == SWIG_NEWOBJ) delete[] buf3;
+  return NULL;
+}
+
+
+SWIGINTERN PyObject *_wrap_delete_Relationship(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  GDALRelationshipShadow *arg1 = (GDALRelationshipShadow *) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  PyObject *swig_obj[1] ;
+  
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_GDALRelationshipShadow, SWIG_POINTER_DISOWN |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "delete_Relationship" "', argument " "1"" of type '" "GDALRelationshipShadow *""'"); 
+  }
+  arg1 = reinterpret_cast< GDALRelationshipShadow * >(argp1);
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      delete_GDALRelationshipShadow(arg1);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  resultobj = SWIG_Py_Void();
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  return NULL;
+}
+
+
+SWIGINTERN PyObject *_wrap_Relationship_GetName(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  GDALRelationshipShadow *arg1 = (GDALRelationshipShadow *) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  PyObject *swig_obj[1] ;
+  char *result = 0 ;
+  
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_GDALRelationshipShadow, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "Relationship_GetName" "', argument " "1"" of type '" "GDALRelationshipShadow *""'"); 
+  }
+  arg1 = reinterpret_cast< GDALRelationshipShadow * >(argp1);
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      result = (char *)GDALRelationshipShadow_GetName(arg1);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  resultobj = SWIG_FromCharPtr((const char *)result);
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  return NULL;
+}
+
+
+SWIGINTERN PyObject *_wrap_Relationship_GetCardinality(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  GDALRelationshipShadow *arg1 = (GDALRelationshipShadow *) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  PyObject *swig_obj[1] ;
+  GDALRelationshipCardinality result;
+  
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_GDALRelationshipShadow, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "Relationship_GetCardinality" "', argument " "1"" of type '" "GDALRelationshipShadow *""'"); 
+  }
+  arg1 = reinterpret_cast< GDALRelationshipShadow * >(argp1);
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      result = (GDALRelationshipCardinality)GDALRelationshipShadow_GetCardinality(arg1);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  resultobj = SWIG_From_int(static_cast< int >(result));
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  return NULL;
+}
+
+
+SWIGINTERN PyObject *_wrap_Relationship_GetLeftTableName(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  GDALRelationshipShadow *arg1 = (GDALRelationshipShadow *) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  PyObject *swig_obj[1] ;
+  char *result = 0 ;
+  
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_GDALRelationshipShadow, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "Relationship_GetLeftTableName" "', argument " "1"" of type '" "GDALRelationshipShadow *""'"); 
+  }
+  arg1 = reinterpret_cast< GDALRelationshipShadow * >(argp1);
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      result = (char *)GDALRelationshipShadow_GetLeftTableName(arg1);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  resultobj = SWIG_FromCharPtr((const char *)result);
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  return NULL;
+}
+
+
+SWIGINTERN PyObject *_wrap_Relationship_GetRightTableName(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  GDALRelationshipShadow *arg1 = (GDALRelationshipShadow *) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  PyObject *swig_obj[1] ;
+  char *result = 0 ;
+  
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_GDALRelationshipShadow, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "Relationship_GetRightTableName" "', argument " "1"" of type '" "GDALRelationshipShadow *""'"); 
+  }
+  arg1 = reinterpret_cast< GDALRelationshipShadow * >(argp1);
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      result = (char *)GDALRelationshipShadow_GetRightTableName(arg1);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  resultobj = SWIG_FromCharPtr((const char *)result);
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  return NULL;
+}
+
+
+SWIGINTERN PyObject *_wrap_Relationship_GetMappingTableName(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  GDALRelationshipShadow *arg1 = (GDALRelationshipShadow *) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  PyObject *swig_obj[1] ;
+  char *result = 0 ;
+  
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_GDALRelationshipShadow, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "Relationship_GetMappingTableName" "', argument " "1"" of type '" "GDALRelationshipShadow *""'"); 
+  }
+  arg1 = reinterpret_cast< GDALRelationshipShadow * >(argp1);
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      result = (char *)GDALRelationshipShadow_GetMappingTableName(arg1);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  resultobj = SWIG_FromCharPtr((const char *)result);
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  return NULL;
+}
+
+
+SWIGINTERN PyObject *_wrap_Relationship_SetMappingTableName(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  GDALRelationshipShadow *arg1 = (GDALRelationshipShadow *) 0 ;
+  char *arg2 = (char *) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  PyObject *str2 = 0 ;
+  int bToFree2 = 0 ;
+  PyObject *swig_obj[2] ;
+  
+  if (!SWIG_Python_UnpackTuple(args, "Relationship_SetMappingTableName", 2, 2, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_GDALRelationshipShadow, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "Relationship_SetMappingTableName" "', argument " "1"" of type '" "GDALRelationshipShadow *""'"); 
+  }
+  arg1 = reinterpret_cast< GDALRelationshipShadow * >(argp1);
+  {
+    /* %typemap(in) (tostring argin) */
+    str2 = PyObject_Str( swig_obj[1] );
+    if ( str2 == 0 ) {
+      PyErr_SetString( PyExc_RuntimeError, "Unable to format argument as string");
+      SWIG_fail;
+    }
+    
+    arg2 = GDALPythonObjectToCStr(str2, &bToFree2);
+  }
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      GDALRelationshipShadow_SetMappingTableName(arg1,(char const *)arg2);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  resultobj = SWIG_Py_Void();
+  {
+    /* %typemap(freearg) (tostring argin) */
+    if ( str2 != NULL)
+    {
+      Py_DECREF(str2);
+    }
+    GDALPythonFreeCStr(arg2, bToFree2);
+  }
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  {
+    /* %typemap(freearg) (tostring argin) */
+    if ( str2 != NULL)
+    {
+      Py_DECREF(str2);
+    }
+    GDALPythonFreeCStr(arg2, bToFree2);
+  }
+  return NULL;
+}
+
+
+SWIGINTERN PyObject *_wrap_Relationship_GetLeftTableFields(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  GDALRelationshipShadow *arg1 = (GDALRelationshipShadow *) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  PyObject *swig_obj[1] ;
+  char **result = 0 ;
+  
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_GDALRelationshipShadow, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "Relationship_GetLeftTableFields" "', argument " "1"" of type '" "GDALRelationshipShadow *""'"); 
+  }
+  arg1 = reinterpret_cast< GDALRelationshipShadow * >(argp1);
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      result = (char **)GDALRelationshipShadow_GetLeftTableFields(arg1);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  {
+    /* %typemap(out) char **CSL -> ( string ) */
+    char **stringarray = result;
+    if ( stringarray == NULL ) {
+      resultobj = Py_None;
+      Py_INCREF( resultobj );
+    }
+    else {
+      int len = CSLCount( stringarray );
+      resultobj = PyList_New( len );
+      for ( int i = 0; i < len; ++i ) {
+        PyObject *o = GDALPythonObjectFromCStr( stringarray[i] );
+        PyList_SetItem(resultobj, i, o );
+      }
+    }
+    CSLDestroy(result);
+  }
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  return NULL;
+}
+
+
+SWIGINTERN PyObject *_wrap_Relationship_GetRightTableFields(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  GDALRelationshipShadow *arg1 = (GDALRelationshipShadow *) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  PyObject *swig_obj[1] ;
+  char **result = 0 ;
+  
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_GDALRelationshipShadow, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "Relationship_GetRightTableFields" "', argument " "1"" of type '" "GDALRelationshipShadow *""'"); 
+  }
+  arg1 = reinterpret_cast< GDALRelationshipShadow * >(argp1);
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      result = (char **)GDALRelationshipShadow_GetRightTableFields(arg1);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  {
+    /* %typemap(out) char **CSL -> ( string ) */
+    char **stringarray = result;
+    if ( stringarray == NULL ) {
+      resultobj = Py_None;
+      Py_INCREF( resultobj );
+    }
+    else {
+      int len = CSLCount( stringarray );
+      resultobj = PyList_New( len );
+      for ( int i = 0; i < len; ++i ) {
+        PyObject *o = GDALPythonObjectFromCStr( stringarray[i] );
+        PyList_SetItem(resultobj, i, o );
+      }
+    }
+    CSLDestroy(result);
+  }
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  return NULL;
+}
+
+
+SWIGINTERN PyObject *_wrap_Relationship_SetLeftTableFields(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  GDALRelationshipShadow *arg1 = (GDALRelationshipShadow *) 0 ;
+  char **arg2 = (char **) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  PyObject *swig_obj[2] ;
+  
+  if (!SWIG_Python_UnpackTuple(args, "Relationship_SetLeftTableFields", 2, 2, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_GDALRelationshipShadow, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "Relationship_SetLeftTableFields" "', argument " "1"" of type '" "GDALRelationshipShadow *""'"); 
+  }
+  arg1 = reinterpret_cast< GDALRelationshipShadow * >(argp1);
+  {
+    /* %typemap(in) char **options */
+    int bErr = FALSE;
+    arg2 = CSLFromPySequence(swig_obj[1], &bErr);
+    if( bErr )
+    {
+      SWIG_fail;
+    }
+  }
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      GDALRelationshipShadow_SetLeftTableFields(arg1,arg2);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  resultobj = SWIG_Py_Void();
+  {
+    /* %typemap(freearg) char **options */
+    CSLDestroy( arg2 );
+  }
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  {
+    /* %typemap(freearg) char **options */
+    CSLDestroy( arg2 );
+  }
+  return NULL;
+}
+
+
+SWIGINTERN PyObject *_wrap_Relationship_SetRightTableFields(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  GDALRelationshipShadow *arg1 = (GDALRelationshipShadow *) 0 ;
+  char **arg2 = (char **) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  PyObject *swig_obj[2] ;
+  
+  if (!SWIG_Python_UnpackTuple(args, "Relationship_SetRightTableFields", 2, 2, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_GDALRelationshipShadow, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "Relationship_SetRightTableFields" "', argument " "1"" of type '" "GDALRelationshipShadow *""'"); 
+  }
+  arg1 = reinterpret_cast< GDALRelationshipShadow * >(argp1);
+  {
+    /* %typemap(in) char **options */
+    int bErr = FALSE;
+    arg2 = CSLFromPySequence(swig_obj[1], &bErr);
+    if( bErr )
+    {
+      SWIG_fail;
+    }
+  }
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      GDALRelationshipShadow_SetRightTableFields(arg1,arg2);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  resultobj = SWIG_Py_Void();
+  {
+    /* %typemap(freearg) char **options */
+    CSLDestroy( arg2 );
+  }
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  {
+    /* %typemap(freearg) char **options */
+    CSLDestroy( arg2 );
+  }
+  return NULL;
+}
+
+
+SWIGINTERN PyObject *_wrap_Relationship_GetLeftMappingTableFields(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  GDALRelationshipShadow *arg1 = (GDALRelationshipShadow *) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  PyObject *swig_obj[1] ;
+  char **result = 0 ;
+  
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_GDALRelationshipShadow, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "Relationship_GetLeftMappingTableFields" "', argument " "1"" of type '" "GDALRelationshipShadow *""'"); 
+  }
+  arg1 = reinterpret_cast< GDALRelationshipShadow * >(argp1);
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      result = (char **)GDALRelationshipShadow_GetLeftMappingTableFields(arg1);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  {
+    /* %typemap(out) char **CSL -> ( string ) */
+    char **stringarray = result;
+    if ( stringarray == NULL ) {
+      resultobj = Py_None;
+      Py_INCREF( resultobj );
+    }
+    else {
+      int len = CSLCount( stringarray );
+      resultobj = PyList_New( len );
+      for ( int i = 0; i < len; ++i ) {
+        PyObject *o = GDALPythonObjectFromCStr( stringarray[i] );
+        PyList_SetItem(resultobj, i, o );
+      }
+    }
+    CSLDestroy(result);
+  }
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  return NULL;
+}
+
+
+SWIGINTERN PyObject *_wrap_Relationship_GetRightMappingTableFields(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  GDALRelationshipShadow *arg1 = (GDALRelationshipShadow *) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  PyObject *swig_obj[1] ;
+  char **result = 0 ;
+  
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_GDALRelationshipShadow, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "Relationship_GetRightMappingTableFields" "', argument " "1"" of type '" "GDALRelationshipShadow *""'"); 
+  }
+  arg1 = reinterpret_cast< GDALRelationshipShadow * >(argp1);
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      result = (char **)GDALRelationshipShadow_GetRightMappingTableFields(arg1);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  {
+    /* %typemap(out) char **CSL -> ( string ) */
+    char **stringarray = result;
+    if ( stringarray == NULL ) {
+      resultobj = Py_None;
+      Py_INCREF( resultobj );
+    }
+    else {
+      int len = CSLCount( stringarray );
+      resultobj = PyList_New( len );
+      for ( int i = 0; i < len; ++i ) {
+        PyObject *o = GDALPythonObjectFromCStr( stringarray[i] );
+        PyList_SetItem(resultobj, i, o );
+      }
+    }
+    CSLDestroy(result);
+  }
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  return NULL;
+}
+
+
+SWIGINTERN PyObject *_wrap_Relationship_SetLeftMappingTableFields(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  GDALRelationshipShadow *arg1 = (GDALRelationshipShadow *) 0 ;
+  char **arg2 = (char **) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  PyObject *swig_obj[2] ;
+  
+  if (!SWIG_Python_UnpackTuple(args, "Relationship_SetLeftMappingTableFields", 2, 2, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_GDALRelationshipShadow, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "Relationship_SetLeftMappingTableFields" "', argument " "1"" of type '" "GDALRelationshipShadow *""'"); 
+  }
+  arg1 = reinterpret_cast< GDALRelationshipShadow * >(argp1);
+  {
+    /* %typemap(in) char **options */
+    int bErr = FALSE;
+    arg2 = CSLFromPySequence(swig_obj[1], &bErr);
+    if( bErr )
+    {
+      SWIG_fail;
+    }
+  }
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      GDALRelationshipShadow_SetLeftMappingTableFields(arg1,arg2);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  resultobj = SWIG_Py_Void();
+  {
+    /* %typemap(freearg) char **options */
+    CSLDestroy( arg2 );
+  }
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  {
+    /* %typemap(freearg) char **options */
+    CSLDestroy( arg2 );
+  }
+  return NULL;
+}
+
+
+SWIGINTERN PyObject *_wrap_Relationship_SetRightMappingTableFields(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  GDALRelationshipShadow *arg1 = (GDALRelationshipShadow *) 0 ;
+  char **arg2 = (char **) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  PyObject *swig_obj[2] ;
+  
+  if (!SWIG_Python_UnpackTuple(args, "Relationship_SetRightMappingTableFields", 2, 2, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_GDALRelationshipShadow, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "Relationship_SetRightMappingTableFields" "', argument " "1"" of type '" "GDALRelationshipShadow *""'"); 
+  }
+  arg1 = reinterpret_cast< GDALRelationshipShadow * >(argp1);
+  {
+    /* %typemap(in) char **options */
+    int bErr = FALSE;
+    arg2 = CSLFromPySequence(swig_obj[1], &bErr);
+    if( bErr )
+    {
+      SWIG_fail;
+    }
+  }
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      GDALRelationshipShadow_SetRightMappingTableFields(arg1,arg2);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  resultobj = SWIG_Py_Void();
+  {
+    /* %typemap(freearg) char **options */
+    CSLDestroy( arg2 );
+  }
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  {
+    /* %typemap(freearg) char **options */
+    CSLDestroy( arg2 );
+  }
+  return NULL;
+}
+
+
+SWIGINTERN PyObject *_wrap_Relationship_GetType(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  GDALRelationshipShadow *arg1 = (GDALRelationshipShadow *) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  PyObject *swig_obj[1] ;
+  GDALRelationshipType result;
+  
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_GDALRelationshipShadow, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "Relationship_GetType" "', argument " "1"" of type '" "GDALRelationshipShadow *""'"); 
+  }
+  arg1 = reinterpret_cast< GDALRelationshipShadow * >(argp1);
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      result = (GDALRelationshipType)GDALRelationshipShadow_GetType(arg1);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  resultobj = SWIG_From_int(static_cast< int >(result));
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  return NULL;
+}
+
+
+SWIGINTERN PyObject *_wrap_Relationship_SetType(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  GDALRelationshipShadow *arg1 = (GDALRelationshipShadow *) 0 ;
+  GDALRelationshipType arg2 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  int val2 ;
+  int ecode2 = 0 ;
+  PyObject *swig_obj[2] ;
+  
+  if (!SWIG_Python_UnpackTuple(args, "Relationship_SetType", 2, 2, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_GDALRelationshipShadow, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "Relationship_SetType" "', argument " "1"" of type '" "GDALRelationshipShadow *""'"); 
+  }
+  arg1 = reinterpret_cast< GDALRelationshipShadow * >(argp1);
+  ecode2 = SWIG_AsVal_int(swig_obj[1], &val2);
+  if (!SWIG_IsOK(ecode2)) {
+    SWIG_exception_fail(SWIG_ArgError(ecode2), "in method '" "Relationship_SetType" "', argument " "2"" of type '" "GDALRelationshipType""'");
+  } 
+  arg2 = static_cast< GDALRelationshipType >(val2);
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      GDALRelationshipShadow_SetType(arg1,arg2);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  resultobj = SWIG_Py_Void();
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  return NULL;
+}
+
+
+SWIGINTERN PyObject *_wrap_Relationship_GetForwardPathLabel(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  GDALRelationshipShadow *arg1 = (GDALRelationshipShadow *) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  PyObject *swig_obj[1] ;
+  char *result = 0 ;
+  
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_GDALRelationshipShadow, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "Relationship_GetForwardPathLabel" "', argument " "1"" of type '" "GDALRelationshipShadow *""'"); 
+  }
+  arg1 = reinterpret_cast< GDALRelationshipShadow * >(argp1);
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      result = (char *)GDALRelationshipShadow_GetForwardPathLabel(arg1);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  resultobj = SWIG_FromCharPtr((const char *)result);
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  return NULL;
+}
+
+
+SWIGINTERN PyObject *_wrap_Relationship_SetForwardPathLabel(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  GDALRelationshipShadow *arg1 = (GDALRelationshipShadow *) 0 ;
+  char *arg2 = (char *) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  PyObject *str2 = 0 ;
+  int bToFree2 = 0 ;
+  PyObject *swig_obj[2] ;
+  
+  if (!SWIG_Python_UnpackTuple(args, "Relationship_SetForwardPathLabel", 2, 2, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_GDALRelationshipShadow, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "Relationship_SetForwardPathLabel" "', argument " "1"" of type '" "GDALRelationshipShadow *""'"); 
+  }
+  arg1 = reinterpret_cast< GDALRelationshipShadow * >(argp1);
+  {
+    /* %typemap(in) (tostring argin) */
+    str2 = PyObject_Str( swig_obj[1] );
+    if ( str2 == 0 ) {
+      PyErr_SetString( PyExc_RuntimeError, "Unable to format argument as string");
+      SWIG_fail;
+    }
+    
+    arg2 = GDALPythonObjectToCStr(str2, &bToFree2);
+  }
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      GDALRelationshipShadow_SetForwardPathLabel(arg1,(char const *)arg2);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  resultobj = SWIG_Py_Void();
+  {
+    /* %typemap(freearg) (tostring argin) */
+    if ( str2 != NULL)
+    {
+      Py_DECREF(str2);
+    }
+    GDALPythonFreeCStr(arg2, bToFree2);
+  }
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  {
+    /* %typemap(freearg) (tostring argin) */
+    if ( str2 != NULL)
+    {
+      Py_DECREF(str2);
+    }
+    GDALPythonFreeCStr(arg2, bToFree2);
+  }
+  return NULL;
+}
+
+
+SWIGINTERN PyObject *_wrap_Relationship_GetBackwardPathLabel(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  GDALRelationshipShadow *arg1 = (GDALRelationshipShadow *) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  PyObject *swig_obj[1] ;
+  char *result = 0 ;
+  
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_GDALRelationshipShadow, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "Relationship_GetBackwardPathLabel" "', argument " "1"" of type '" "GDALRelationshipShadow *""'"); 
+  }
+  arg1 = reinterpret_cast< GDALRelationshipShadow * >(argp1);
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      result = (char *)GDALRelationshipShadow_GetBackwardPathLabel(arg1);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  resultobj = SWIG_FromCharPtr((const char *)result);
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  return NULL;
+}
+
+
+SWIGINTERN PyObject *_wrap_Relationship_SetBackwardPathLabel(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  GDALRelationshipShadow *arg1 = (GDALRelationshipShadow *) 0 ;
+  char *arg2 = (char *) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  PyObject *str2 = 0 ;
+  int bToFree2 = 0 ;
+  PyObject *swig_obj[2] ;
+  
+  if (!SWIG_Python_UnpackTuple(args, "Relationship_SetBackwardPathLabel", 2, 2, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_GDALRelationshipShadow, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "Relationship_SetBackwardPathLabel" "', argument " "1"" of type '" "GDALRelationshipShadow *""'"); 
+  }
+  arg1 = reinterpret_cast< GDALRelationshipShadow * >(argp1);
+  {
+    /* %typemap(in) (tostring argin) */
+    str2 = PyObject_Str( swig_obj[1] );
+    if ( str2 == 0 ) {
+      PyErr_SetString( PyExc_RuntimeError, "Unable to format argument as string");
+      SWIG_fail;
+    }
+    
+    arg2 = GDALPythonObjectToCStr(str2, &bToFree2);
+  }
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      GDALRelationshipShadow_SetBackwardPathLabel(arg1,(char const *)arg2);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  resultobj = SWIG_Py_Void();
+  {
+    /* %typemap(freearg) (tostring argin) */
+    if ( str2 != NULL)
+    {
+      Py_DECREF(str2);
+    }
+    GDALPythonFreeCStr(arg2, bToFree2);
+  }
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  {
+    /* %typemap(freearg) (tostring argin) */
+    if ( str2 != NULL)
+    {
+      Py_DECREF(str2);
+    }
+    GDALPythonFreeCStr(arg2, bToFree2);
+  }
+  return NULL;
+}
+
+
+SWIGINTERN PyObject *_wrap_Relationship_GetRelatedTableType(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  GDALRelationshipShadow *arg1 = (GDALRelationshipShadow *) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  PyObject *swig_obj[1] ;
+  char *result = 0 ;
+  
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_GDALRelationshipShadow, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "Relationship_GetRelatedTableType" "', argument " "1"" of type '" "GDALRelationshipShadow *""'"); 
+  }
+  arg1 = reinterpret_cast< GDALRelationshipShadow * >(argp1);
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      result = (char *)GDALRelationshipShadow_GetRelatedTableType(arg1);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  resultobj = SWIG_FromCharPtr((const char *)result);
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  return NULL;
+}
+
+
+SWIGINTERN PyObject *_wrap_Relationship_SetRelatedTableType(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  GDALRelationshipShadow *arg1 = (GDALRelationshipShadow *) 0 ;
+  char *arg2 = (char *) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  PyObject *str2 = 0 ;
+  int bToFree2 = 0 ;
+  PyObject *swig_obj[2] ;
+  
+  if (!SWIG_Python_UnpackTuple(args, "Relationship_SetRelatedTableType", 2, 2, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_GDALRelationshipShadow, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "Relationship_SetRelatedTableType" "', argument " "1"" of type '" "GDALRelationshipShadow *""'"); 
+  }
+  arg1 = reinterpret_cast< GDALRelationshipShadow * >(argp1);
+  {
+    /* %typemap(in) (tostring argin) */
+    str2 = PyObject_Str( swig_obj[1] );
+    if ( str2 == 0 ) {
+      PyErr_SetString( PyExc_RuntimeError, "Unable to format argument as string");
+      SWIG_fail;
+    }
+    
+    arg2 = GDALPythonObjectToCStr(str2, &bToFree2);
+  }
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      GDALRelationshipShadow_SetRelatedTableType(arg1,(char const *)arg2);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  resultobj = SWIG_Py_Void();
+  {
+    /* %typemap(freearg) (tostring argin) */
+    if ( str2 != NULL)
+    {
+      Py_DECREF(str2);
+    }
+    GDALPythonFreeCStr(arg2, bToFree2);
+  }
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  {
+    /* %typemap(freearg) (tostring argin) */
+    if ( str2 != NULL)
+    {
+      Py_DECREF(str2);
+    }
+    GDALPythonFreeCStr(arg2, bToFree2);
+  }
+  return NULL;
+}
+
+
+SWIGINTERN PyObject *Relationship_swigregister(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *obj;
+  if (!SWIG_Python_UnpackTuple(args, "swigregister", 1, 1, &obj)) return NULL;
+  SWIG_TypeNewClientData(SWIGTYPE_p_GDALRelationshipShadow, SWIG_NewClientData(obj));
+  return SWIG_Py_Void();
+}
+
+SWIGINTERN PyObject *Relationship_swiginit(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  return SWIG_Python_InitShadowInstance(args);
+}
+
 SWIGINTERN PyObject *_wrap_TermProgress_nocb(PyObject *SWIGUNUSEDPARM(self), PyObject *args, PyObject *kwargs) {
   PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
   double arg1 ;
   char *arg2 = (char *) NULL ;
   void *arg3 = (void *) NULL ;
   double val1 ;
   int ecode1 = 0 ;
@@ -44617,17 +46608,20 @@
 	 { "DirEntry_swiginit", DirEntry_swiginit, METH_VARARGS, NULL},
 	 { "GetNextDirEntry", _wrap_GetNextDirEntry, METH_O, "GetNextDirEntry(VSIDIR * dir) -> DirEntry"},
 	 { "CloseDir", _wrap_CloseDir, METH_O, "CloseDir(VSIDIR * dir)"},
 	 { "SetConfigOption", _wrap_SetConfigOption, METH_VARARGS, "SetConfigOption(char const * pszKey, char const * pszValue)"},
 	 { "SetThreadLocalConfigOption", _wrap_SetThreadLocalConfigOption, METH_VARARGS, "SetThreadLocalConfigOption(char const * pszKey, char const * pszValue)"},
 	 { "GetConfigOption", _wrap_GetConfigOption, METH_VARARGS, "GetConfigOption(char const * pszKey, char const * pszDefault=None) -> char const *"},
 	 { "GetThreadLocalConfigOption", _wrap_GetThreadLocalConfigOption, METH_VARARGS, "GetThreadLocalConfigOption(char const * pszKey, char const * pszDefault=None) -> char const *"},
+	 { "SetPathSpecificOption", _wrap_SetPathSpecificOption, METH_VARARGS, "SetPathSpecificOption(char const * pszPathPrefix, char const * pszKey, char const * pszValue)"},
 	 { "SetCredential", _wrap_SetCredential, METH_VARARGS, "SetCredential(char const * pszPathPrefix, char const * pszKey, char const * pszValue)"},
 	 { "GetCredential", _wrap_GetCredential, METH_VARARGS, "GetCredential(char const * pszPathPrefix, char const * pszKey, char const * pszDefault=None) -> char const *"},
+	 { "GetPathSpecificOption", _wrap_GetPathSpecificOption, METH_VARARGS, "GetPathSpecificOption(char const * pszPathPrefix, char const * pszKey, char const * pszDefault=None) -> char const *"},
 	 { "ClearCredentials", _wrap_ClearCredentials, METH_VARARGS, "ClearCredentials(char const * pszPathPrefix=None)"},
+	 { "ClearPathSpecificOptions", _wrap_ClearPathSpecificOptions, METH_VARARGS, "ClearPathSpecificOptions(char const * pszPathPrefix=None)"},
 	 { "CPLBinaryToHex", _wrap_CPLBinaryToHex, METH_O, "CPLBinaryToHex(int nBytes) -> retStringAndCPLFree *"},
 	 { "CPLHexToBinary", _wrap_CPLHexToBinary, METH_VARARGS, "CPLHexToBinary(char const * pszHex, int * pnBytes) -> GByte *"},
 	 { "FileFromMemBuffer", _wrap_FileFromMemBuffer, METH_VARARGS, "FileFromMemBuffer(char const * utf8_path, GIntBig nBytes)"},
 	 { "Unlink", _wrap_Unlink, METH_O, "Unlink(char const * utf8_path) -> VSI_RETVAL"},
 	 { "UnlinkBatch", _wrap_UnlinkBatch, METH_O, "UnlinkBatch(char ** files) -> bool"},
 	 { "HasThreadSupport", _wrap_HasThreadSupport, METH_NOARGS, "HasThreadSupport() -> int"},
 	 { "Mkdir", _wrap_Mkdir, METH_VARARGS, "Mkdir(char const * utf8_path, int mode) -> VSI_RETVAL"},
@@ -44665,14 +46659,16 @@
 	 { "VSIFGetRangeStatusL", _wrap_VSIFGetRangeStatusL, METH_VARARGS, "VSIFGetRangeStatusL(VSILFILE fp, GIntBig offset, GIntBig length) -> int"},
 	 { "VSIFWriteL", _wrap_VSIFWriteL, METH_VARARGS, "VSIFWriteL(int nLen, int size, int memb, VSILFILE fp) -> int"},
 	 { "VSICurlClearCache", _wrap_VSICurlClearCache, METH_NOARGS, "VSICurlClearCache()"},
 	 { "VSICurlPartialClearCache", _wrap_VSICurlPartialClearCache, METH_O, "VSICurlPartialClearCache(char const * utf8_path)"},
 	 { "NetworkStatsReset", _wrap_NetworkStatsReset, METH_NOARGS, "NetworkStatsReset()"},
 	 { "NetworkStatsGetAsSerializedJSON", _wrap_NetworkStatsGetAsSerializedJSON, METH_VARARGS, "NetworkStatsGetAsSerializedJSON(char ** options=None) -> retStringAndCPLFree *"},
 	 { "ParseCommandLine", _wrap_ParseCommandLine, METH_O, "ParseCommandLine(char const * utf8_path) -> char **"},
+	 { "GetNumCPUs", _wrap_GetNumCPUs, METH_NOARGS, "GetNumCPUs() -> int"},
+	 { "GetUsablePhysicalRAM", _wrap_GetUsablePhysicalRAM, METH_NOARGS, "GetUsablePhysicalRAM() -> GIntBig"},
 	 { "MajorObject_GetDescription", _wrap_MajorObject_GetDescription, METH_O, "MajorObject_GetDescription(MajorObject self) -> char const *"},
 	 { "MajorObject_SetDescription", _wrap_MajorObject_SetDescription, METH_VARARGS, "MajorObject_SetDescription(MajorObject self, char const * pszNewDesc)"},
 	 { "MajorObject_GetMetadataDomainList", _wrap_MajorObject_GetMetadataDomainList, METH_O, "MajorObject_GetMetadataDomainList(MajorObject self) -> char **"},
 	 { "MajorObject_GetMetadata_Dict", _wrap_MajorObject_GetMetadata_Dict, METH_VARARGS, "MajorObject_GetMetadata_Dict(MajorObject self, char const * pszDomain=\"\") -> char **"},
 	 { "MajorObject_GetMetadata_List", _wrap_MajorObject_GetMetadata_List, METH_VARARGS, "MajorObject_GetMetadata_List(MajorObject self, char const * pszDomain=\"\") -> char **"},
 	 { "MajorObject_SetMetadata", _wrap_MajorObject_SetMetadata, METH_VARARGS, "\n"
 		"MajorObject_SetMetadata(MajorObject self, char ** papszMetadata, char const * pszDomain=\"\") -> CPLErr\n"
@@ -44755,15 +46751,15 @@
 	 { "Dataset_GetProjection", _wrap_Dataset_GetProjection, METH_O, "Dataset_GetProjection(Dataset self) -> char const *"},
 	 { "Dataset_GetProjectionRef", _wrap_Dataset_GetProjectionRef, METH_O, "Dataset_GetProjectionRef(Dataset self) -> char const *"},
 	 { "Dataset_GetSpatialRef", _wrap_Dataset_GetSpatialRef, METH_O, "Dataset_GetSpatialRef(Dataset self) -> SpatialReference"},
 	 { "Dataset_SetProjection", _wrap_Dataset_SetProjection, METH_VARARGS, "Dataset_SetProjection(Dataset self, char const * prj) -> CPLErr"},
 	 { "Dataset_SetSpatialRef", _wrap_Dataset_SetSpatialRef, METH_VARARGS, "Dataset_SetSpatialRef(Dataset self, SpatialReference srs) -> CPLErr"},
 	 { "Dataset_GetGeoTransform", (PyCFunction)(void(*)(void))_wrap_Dataset_GetGeoTransform, METH_VARARGS|METH_KEYWORDS, "Dataset_GetGeoTransform(Dataset self, int * can_return_null=None)"},
 	 { "Dataset_SetGeoTransform", _wrap_Dataset_SetGeoTransform, METH_VARARGS, "Dataset_SetGeoTransform(Dataset self, double [6] argin) -> CPLErr"},
-	 { "Dataset_BuildOverviews", (PyCFunction)(void(*)(void))_wrap_Dataset_BuildOverviews, METH_VARARGS|METH_KEYWORDS, "Dataset_BuildOverviews(Dataset self, char const * resampling=\"NEAREST\", int overviewlist=0, GDALProgressFunc callback=0, void * callback_data=None) -> int"},
+	 { "Dataset_BuildOverviews", (PyCFunction)(void(*)(void))_wrap_Dataset_BuildOverviews, METH_VARARGS|METH_KEYWORDS, "Dataset_BuildOverviews(Dataset self, char const * resampling=\"NEAREST\", int overviewlist=0, GDALProgressFunc callback=0, void * callback_data=None, char ** options=None) -> int"},
 	 { "Dataset_GetGCPCount", _wrap_Dataset_GetGCPCount, METH_O, "Dataset_GetGCPCount(Dataset self) -> int"},
 	 { "Dataset_GetGCPProjection", _wrap_Dataset_GetGCPProjection, METH_O, "Dataset_GetGCPProjection(Dataset self) -> char const *"},
 	 { "Dataset_GetGCPSpatialRef", _wrap_Dataset_GetGCPSpatialRef, METH_O, "Dataset_GetGCPSpatialRef(Dataset self) -> SpatialReference"},
 	 { "Dataset_GetGCPs", _wrap_Dataset_GetGCPs, METH_O, "Dataset_GetGCPs(Dataset self)"},
 	 { "Dataset__SetGCPs", _wrap_Dataset__SetGCPs, METH_VARARGS, "Dataset__SetGCPs(Dataset self, int nGCPs, char const * pszGCPProjection) -> CPLErr"},
 	 { "Dataset__SetGCPs2", _wrap_Dataset__SetGCPs2, METH_VARARGS, "Dataset__SetGCPs2(Dataset self, int nGCPs, SpatialReference hSRS) -> CPLErr"},
 	 { "Dataset_FlushCache", _wrap_Dataset_FlushCache, METH_O, "Dataset_FlushCache(Dataset self)"},
@@ -44796,14 +46792,19 @@
 	 { "Dataset_RollbackTransaction", _wrap_Dataset_RollbackTransaction, METH_O, "Dataset_RollbackTransaction(Dataset self) -> OGRErr"},
 	 { "Dataset_ClearStatistics", _wrap_Dataset_ClearStatistics, METH_O, "Dataset_ClearStatistics(Dataset self)"},
 	 { "Dataset_GetFieldDomainNames", _wrap_Dataset_GetFieldDomainNames, METH_VARARGS, "Dataset_GetFieldDomainNames(Dataset self, char ** options=None) -> char **"},
 	 { "Dataset_GetFieldDomain", _wrap_Dataset_GetFieldDomain, METH_VARARGS, "Dataset_GetFieldDomain(Dataset self, char const * name) -> FieldDomain"},
 	 { "Dataset_AddFieldDomain", _wrap_Dataset_AddFieldDomain, METH_VARARGS, "Dataset_AddFieldDomain(Dataset self, FieldDomain fieldDomain) -> bool"},
 	 { "Dataset_DeleteFieldDomain", _wrap_Dataset_DeleteFieldDomain, METH_VARARGS, "Dataset_DeleteFieldDomain(Dataset self, char const * name) -> bool"},
 	 { "Dataset_UpdateFieldDomain", _wrap_Dataset_UpdateFieldDomain, METH_VARARGS, "Dataset_UpdateFieldDomain(Dataset self, FieldDomain fieldDomain) -> bool"},
+	 { "Dataset_GetRelationshipNames", _wrap_Dataset_GetRelationshipNames, METH_VARARGS, "Dataset_GetRelationshipNames(Dataset self, char ** options=None) -> char **"},
+	 { "Dataset_GetRelationship", _wrap_Dataset_GetRelationship, METH_VARARGS, "Dataset_GetRelationship(Dataset self, char const * name) -> Relationship"},
+	 { "Dataset_AddRelationship", _wrap_Dataset_AddRelationship, METH_VARARGS, "Dataset_AddRelationship(Dataset self, Relationship relationship) -> bool"},
+	 { "Dataset_DeleteRelationship", _wrap_Dataset_DeleteRelationship, METH_VARARGS, "Dataset_DeleteRelationship(Dataset self, char const * name) -> bool"},
+	 { "Dataset_UpdateRelationship", _wrap_Dataset_UpdateRelationship, METH_VARARGS, "Dataset_UpdateRelationship(Dataset self, Relationship relationship) -> bool"},
 	 { "Dataset_ReadRaster1", (PyCFunction)(void(*)(void))_wrap_Dataset_ReadRaster1, METH_VARARGS|METH_KEYWORDS, "Dataset_ReadRaster1(Dataset self, double xoff, double yoff, double xsize, double ysize, int * buf_xsize=None, int * buf_ysize=None, GDALDataType * buf_type=None, int band_list=0, GIntBig * buf_pixel_space=None, GIntBig * buf_line_space=None, GIntBig * buf_band_space=None, GDALRIOResampleAlg resample_alg=GRIORA_NearestNeighbour, GDALProgressFunc callback=0, void * callback_data=None, void * inputOutputBuf=None) -> CPLErr"},
 	 { "Dataset_swigregister", Dataset_swigregister, METH_O, NULL},
 	 { "delete_Group", _wrap_delete_Group, METH_O, "delete_Group(Group self)"},
 	 { "Group_GetName", _wrap_Group_GetName, METH_O, "Group_GetName(Group self) -> char const *"},
 	 { "Group_GetFullName", _wrap_Group_GetFullName, METH_O, "Group_GetFullName(Group self) -> char const *"},
 	 { "Group_GetMDArrayNames", _wrap_Group_GetMDArrayNames, METH_VARARGS, "Group_GetMDArrayNames(Group self, char ** options=None) -> char **"},
 	 { "Group_OpenMDArray", _wrap_Group_OpenMDArray, METH_VARARGS, "Group_OpenMDArray(Group self, char const * name, char ** options=None) -> MDArray"},
@@ -44956,20 +46957,20 @@
 	 { "Band_GetMinimum", _wrap_Band_GetMinimum, METH_O, "Band_GetMinimum(Band self)"},
 	 { "Band_GetMaximum", _wrap_Band_GetMaximum, METH_O, "Band_GetMaximum(Band self)"},
 	 { "Band_GetOffset", _wrap_Band_GetOffset, METH_O, "Band_GetOffset(Band self)"},
 	 { "Band_GetScale", _wrap_Band_GetScale, METH_O, "Band_GetScale(Band self)"},
 	 { "Band_SetOffset", _wrap_Band_SetOffset, METH_VARARGS, "Band_SetOffset(Band self, double val) -> CPLErr"},
 	 { "Band_SetScale", _wrap_Band_SetScale, METH_VARARGS, "Band_SetScale(Band self, double val) -> CPLErr"},
 	 { "Band_GetStatistics", _wrap_Band_GetStatistics, METH_VARARGS, "Band_GetStatistics(Band self, int approx_ok, int force) -> CPLErr"},
-	 { "Band_ComputeStatistics", _wrap_Band_ComputeStatistics, METH_VARARGS, "Band_ComputeStatistics(Band self, bool approx_ok, GDALProgressFunc callback=0, void * callback_data=None) -> CPLErr"},
+	 { "Band_ComputeStatistics", (PyCFunction)(void(*)(void))_wrap_Band_ComputeStatistics, METH_VARARGS|METH_KEYWORDS, "Band_ComputeStatistics(Band self, bool approx_ok, GDALProgressFunc callback=0, void * callback_data=None) -> CPLErr"},
 	 { "Band_SetStatistics", _wrap_Band_SetStatistics, METH_VARARGS, "Band_SetStatistics(Band self, double min, double max, double mean, double stddev) -> CPLErr"},
 	 { "Band_GetOverviewCount", _wrap_Band_GetOverviewCount, METH_O, "Band_GetOverviewCount(Band self) -> int"},
 	 { "Band_GetOverview", _wrap_Band_GetOverview, METH_VARARGS, "Band_GetOverview(Band self, int i) -> Band"},
 	 { "Band_Checksum", (PyCFunction)(void(*)(void))_wrap_Band_Checksum, METH_VARARGS|METH_KEYWORDS, "Band_Checksum(Band self, int xoff=0, int yoff=0, int * xsize=None, int * ysize=None) -> int"},
-	 { "Band_ComputeRasterMinMax", _wrap_Band_ComputeRasterMinMax, METH_VARARGS, "Band_ComputeRasterMinMax(Band self, int approx_ok=0)"},
+	 { "Band_ComputeRasterMinMax", (PyCFunction)(void(*)(void))_wrap_Band_ComputeRasterMinMax, METH_VARARGS|METH_KEYWORDS, "Band_ComputeRasterMinMax(Band self, bool approx_ok=False, bool can_return_none=False)"},
 	 { "Band_ComputeBandStats", _wrap_Band_ComputeBandStats, METH_VARARGS, "Band_ComputeBandStats(Band self, int samplestep=1)"},
 	 { "Band_Fill", _wrap_Band_Fill, METH_VARARGS, "Band_Fill(Band self, double real_fill, double imag_fill=0.0) -> CPLErr"},
 	 { "Band_WriteRaster", (PyCFunction)(void(*)(void))_wrap_Band_WriteRaster, METH_VARARGS|METH_KEYWORDS, "Band_WriteRaster(Band self, int xoff, int yoff, int xsize, int ysize, GIntBig buf_len, int * buf_xsize=None, int * buf_ysize=None, GDALDataType * buf_type=None, GIntBig * buf_pixel_space=None, GIntBig * buf_line_space=None) -> CPLErr"},
 	 { "Band_FlushCache", _wrap_Band_FlushCache, METH_O, "Band_FlushCache(Band self)"},
 	 { "Band_GetRasterColorTable", _wrap_Band_GetRasterColorTable, METH_O, "Band_GetRasterColorTable(Band self) -> ColorTable"},
 	 { "Band_GetColorTable", _wrap_Band_GetColorTable, METH_O, "Band_GetColorTable(Band self) -> ColorTable"},
 	 { "Band_SetRasterColorTable", _wrap_Band_SetRasterColorTable, METH_VARARGS, "Band_SetRasterColorTable(Band self, ColorTable arg) -> int"},
@@ -45028,14 +47029,40 @@
 	 { "RasterAttributeTable_GetRowOfValue", _wrap_RasterAttributeTable_GetRowOfValue, METH_VARARGS, "RasterAttributeTable_GetRowOfValue(RasterAttributeTable self, double dfValue) -> int"},
 	 { "RasterAttributeTable_ChangesAreWrittenToFile", _wrap_RasterAttributeTable_ChangesAreWrittenToFile, METH_O, "RasterAttributeTable_ChangesAreWrittenToFile(RasterAttributeTable self) -> int"},
 	 { "RasterAttributeTable_DumpReadable", _wrap_RasterAttributeTable_DumpReadable, METH_O, "RasterAttributeTable_DumpReadable(RasterAttributeTable self)"},
 	 { "RasterAttributeTable_SetTableType", _wrap_RasterAttributeTable_SetTableType, METH_VARARGS, "RasterAttributeTable_SetTableType(RasterAttributeTable self, GDALRATTableType eTableType)"},
 	 { "RasterAttributeTable_GetTableType", _wrap_RasterAttributeTable_GetTableType, METH_O, "RasterAttributeTable_GetTableType(RasterAttributeTable self) -> GDALRATTableType"},
 	 { "RasterAttributeTable_swigregister", RasterAttributeTable_swigregister, METH_O, NULL},
 	 { "RasterAttributeTable_swiginit", RasterAttributeTable_swiginit, METH_VARARGS, NULL},
+	 { "new_Relationship", _wrap_new_Relationship, METH_VARARGS, "new_Relationship(char const * name, char const * leftTableName, char const * rightTableName, GDALRelationshipCardinality cardinality) -> Relationship"},
+	 { "delete_Relationship", _wrap_delete_Relationship, METH_O, "delete_Relationship(Relationship self)"},
+	 { "Relationship_GetName", _wrap_Relationship_GetName, METH_O, "Relationship_GetName(Relationship self) -> char const *"},
+	 { "Relationship_GetCardinality", _wrap_Relationship_GetCardinality, METH_O, "Relationship_GetCardinality(Relationship self) -> GDALRelationshipCardinality"},
+	 { "Relationship_GetLeftTableName", _wrap_Relationship_GetLeftTableName, METH_O, "Relationship_GetLeftTableName(Relationship self) -> char const *"},
+	 { "Relationship_GetRightTableName", _wrap_Relationship_GetRightTableName, METH_O, "Relationship_GetRightTableName(Relationship self) -> char const *"},
+	 { "Relationship_GetMappingTableName", _wrap_Relationship_GetMappingTableName, METH_O, "Relationship_GetMappingTableName(Relationship self) -> char const *"},
+	 { "Relationship_SetMappingTableName", _wrap_Relationship_SetMappingTableName, METH_VARARGS, "Relationship_SetMappingTableName(Relationship self, char const * pszName)"},
+	 { "Relationship_GetLeftTableFields", _wrap_Relationship_GetLeftTableFields, METH_O, "Relationship_GetLeftTableFields(Relationship self) -> char **"},
+	 { "Relationship_GetRightTableFields", _wrap_Relationship_GetRightTableFields, METH_O, "Relationship_GetRightTableFields(Relationship self) -> char **"},
+	 { "Relationship_SetLeftTableFields", _wrap_Relationship_SetLeftTableFields, METH_VARARGS, "Relationship_SetLeftTableFields(Relationship self, char ** pFields)"},
+	 { "Relationship_SetRightTableFields", _wrap_Relationship_SetRightTableFields, METH_VARARGS, "Relationship_SetRightTableFields(Relationship self, char ** pFields)"},
+	 { "Relationship_GetLeftMappingTableFields", _wrap_Relationship_GetLeftMappingTableFields, METH_O, "Relationship_GetLeftMappingTableFields(Relationship self) -> char **"},
+	 { "Relationship_GetRightMappingTableFields", _wrap_Relationship_GetRightMappingTableFields, METH_O, "Relationship_GetRightMappingTableFields(Relationship self) -> char **"},
+	 { "Relationship_SetLeftMappingTableFields", _wrap_Relationship_SetLeftMappingTableFields, METH_VARARGS, "Relationship_SetLeftMappingTableFields(Relationship self, char ** pFields)"},
+	 { "Relationship_SetRightMappingTableFields", _wrap_Relationship_SetRightMappingTableFields, METH_VARARGS, "Relationship_SetRightMappingTableFields(Relationship self, char ** pFields)"},
+	 { "Relationship_GetType", _wrap_Relationship_GetType, METH_O, "Relationship_GetType(Relationship self) -> GDALRelationshipType"},
+	 { "Relationship_SetType", _wrap_Relationship_SetType, METH_VARARGS, "Relationship_SetType(Relationship self, GDALRelationshipType type)"},
+	 { "Relationship_GetForwardPathLabel", _wrap_Relationship_GetForwardPathLabel, METH_O, "Relationship_GetForwardPathLabel(Relationship self) -> char const *"},
+	 { "Relationship_SetForwardPathLabel", _wrap_Relationship_SetForwardPathLabel, METH_VARARGS, "Relationship_SetForwardPathLabel(Relationship self, char const * pszLabel)"},
+	 { "Relationship_GetBackwardPathLabel", _wrap_Relationship_GetBackwardPathLabel, METH_O, "Relationship_GetBackwardPathLabel(Relationship self) -> char const *"},
+	 { "Relationship_SetBackwardPathLabel", _wrap_Relationship_SetBackwardPathLabel, METH_VARARGS, "Relationship_SetBackwardPathLabel(Relationship self, char const * pszLabel)"},
+	 { "Relationship_GetRelatedTableType", _wrap_Relationship_GetRelatedTableType, METH_O, "Relationship_GetRelatedTableType(Relationship self) -> char const *"},
+	 { "Relationship_SetRelatedTableType", _wrap_Relationship_SetRelatedTableType, METH_VARARGS, "Relationship_SetRelatedTableType(Relationship self, char const * pszType)"},
+	 { "Relationship_swigregister", Relationship_swigregister, METH_O, NULL},
+	 { "Relationship_swiginit", Relationship_swiginit, METH_VARARGS, NULL},
 	 { "TermProgress_nocb", (PyCFunction)(void(*)(void))_wrap_TermProgress_nocb, METH_VARARGS|METH_KEYWORDS, "TermProgress_nocb(double dfProgress, char const * pszMessage=None, void * pData=None) -> int"},
 	 { "ComputeMedianCutPCT", (PyCFunction)(void(*)(void))_wrap_ComputeMedianCutPCT, METH_VARARGS|METH_KEYWORDS, "ComputeMedianCutPCT(Band red, Band green, Band blue, int num_colors, ColorTable colors, GDALProgressFunc callback=0, void * callback_data=None) -> int"},
 	 { "DitherRGB2PCT", (PyCFunction)(void(*)(void))_wrap_DitherRGB2PCT, METH_VARARGS|METH_KEYWORDS, "DitherRGB2PCT(Band red, Band green, Band blue, Band target, ColorTable colors, GDALProgressFunc callback=0, void * callback_data=None) -> int"},
 	 { "ReprojectImage", (PyCFunction)(void(*)(void))_wrap_ReprojectImage, METH_VARARGS|METH_KEYWORDS, "ReprojectImage(Dataset src_ds, Dataset dst_ds, char const * src_wkt=None, char const * dst_wkt=None, GDALResampleAlg eResampleAlg=GRA_NearestNeighbour, double WarpMemoryLimit=0.0, double maxerror=0.0, GDALProgressFunc callback=0, void * callback_data=None, char ** options=None) -> CPLErr"},
 	 { "ComputeProximity", (PyCFunction)(void(*)(void))_wrap_ComputeProximity, METH_VARARGS|METH_KEYWORDS, "ComputeProximity(Band srcBand, Band proximityBand, char ** options=None, GDALProgressFunc callback=0, void * callback_data=None) -> int"},
 	 { "RasterizeLayer", (PyCFunction)(void(*)(void))_wrap_RasterizeLayer, METH_VARARGS|METH_KEYWORDS, "RasterizeLayer(Dataset dataset, int bands, Layer layer, void * pfnTransformer=None, void * pTransformArg=None, int burn_values=0, char ** options=None, GDALProgressFunc callback=0, void * callback_data=None) -> int"},
 	 { "Polygonize", (PyCFunction)(void(*)(void))_wrap_Polygonize, METH_VARARGS|METH_KEYWORDS, "Polygonize(Band srcBand, Band maskBand, Layer outLayer, int iPixValField, char ** options=None, GDALProgressFunc callback=0, void * callback_data=None) -> int"},
@@ -45198,14 +47225,15 @@
 static swig_type_info _swigt__p_GDALMultiDimInfoOptions = {"_p_GDALMultiDimInfoOptions", "GDALMultiDimInfoOptions *", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_GDALMultiDimTranslateOptions = {"_p_GDALMultiDimTranslateOptions", "GDALMultiDimTranslateOptions *", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_GDALNearblackOptions = {"_p_GDALNearblackOptions", "GDALNearblackOptions *", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_GDALProgressFunc = {"_p_GDALProgressFunc", "GDALProgressFunc *", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_GDALRasterAttributeTableShadow = {"_p_GDALRasterAttributeTableShadow", "GDALRasterAttributeTableShadow *", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_GDALRasterBandShadow = {"_p_GDALRasterBandShadow", "GDALRasterBandShadow *", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_GDALRasterizeOptions = {"_p_GDALRasterizeOptions", "GDALRasterizeOptions *", 0, 0, (void*)0, 0};
+static swig_type_info _swigt__p_GDALRelationshipShadow = {"_p_GDALRelationshipShadow", "GDALRelationshipShadow *", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_GDALTransformerInfoShadow = {"_p_GDALTransformerInfoShadow", "GDALTransformerInfoShadow *", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_GDALTranslateOptions = {"_p_GDALTranslateOptions", "GDALTranslateOptions *", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_GDALVectorTranslateOptions = {"_p_GDALVectorTranslateOptions", "GDALVectorTranslateOptions *", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_GDALViewshedMode = {"_p_GDALViewshedMode", "enum GDALViewshedMode *|GDALViewshedMode *", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_GDALViewshedOutputType = {"_p_GDALViewshedOutputType", "enum GDALViewshedOutputType *|GDALViewshedOutputType *", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_GDALWarpAppOptions = {"_p_GDALWarpAppOptions", "GDALWarpAppOptions *", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_GDAL_GCP = {"_p_GDAL_GCP", "GDAL_GCP *", 0, 0, (void*)0, 0};
@@ -45220,15 +47248,15 @@
 static swig_type_info _swigt__p_StatBuf = {"_p_StatBuf", "StatBuf *", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_Statistics = {"_p_Statistics", "Statistics *", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_VSIDIR = {"_p_VSIDIR", "VSIDIR *", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_VSILFILE = {"_p_VSILFILE", "VSILFILE *", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_char = {"_p_char", "char *|retStringAndCPLFree *", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_double = {"_p_double", "double *", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_f_double_p_q_const__char_p_void__int = {"_p_f_double_p_q_const__char_p_void__int", "int (*)(double,char const *,void *)", 0, 0, (void*)0, 0};
-static swig_type_info _swigt__p_int = {"_p_int", "OGRFieldSubType *|OGRFieldDomainType *|GDALRATFieldType *|OGRFieldType *|RETURN_NONE *|int *|GDALAccess *|OSRAxisMappingStrategy *|OGRwkbByteOrder *|CPLErr *|GDALRWFlag *|OGRJustification *|GDALRATFieldUsage *|GDALTileOrganization *|OGRAxisOrientation *|GDALPaletteInterp *|GDALColorInterp *|GDALRIOResampleAlg *|GDALResampleAlg *|OGRErr *|OGRwkbGeometryType *|GDALDataType *|GDALAsyncStatusType *|GDALRATTableType *|OGRFieldDomainMergePolicy *|OGRFieldDomainSplitPolicy *", 0, 0, (void*)0, 0};
+static swig_type_info _swigt__p_int = {"_p_int", "OGRFieldSubType *|OGRFieldDomainType *|GDALRATFieldType *|OGRFieldType *|RETURN_NONE *|GDALRelationshipType *|int *|GDALAccess *|OSRAxisMappingStrategy *|OGRwkbByteOrder *|CPLErr *|GDALRWFlag *|OGRJustification *|GDALRATFieldUsage *|GDALTileOrganization *|OGRAxisOrientation *|GDALPaletteInterp *|GDALColorInterp *|GDALRIOResampleAlg *|GDALResampleAlg *|OGRErr *|OGRwkbGeometryType *|GDALDataType *|GDALAsyncStatusType *|GDALRATTableType *|GDALRelationshipCardinality *|OGRFieldDomainMergePolicy *|OGRFieldDomainSplitPolicy *", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_p_GByte = {"_p_p_GByte", "GByte **", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_p_GDALDatasetShadow = {"_p_p_GDALDatasetShadow", "GDALDatasetShadow **", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_p_GDALDimensionHS = {"_p_p_GDALDimensionHS", "GDALDimensionHS **", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_p_GDALEDTComponentHS = {"_p_p_GDALEDTComponentHS", "GDALEDTComponentHS **", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_p_GDALRasterBandShadow = {"_p_p_GDALRasterBandShadow", "GDALRasterBandShadow **", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_p_GDAL_GCP = {"_p_p_GDAL_GCP", "GDAL_GCP **", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_p_GUIntBig = {"_p_p_GUIntBig", "GUIntBig **", 0, 0, (void*)0, 0};
@@ -45272,14 +47300,15 @@
   &_swigt__p_GDALMultiDimInfoOptions,
   &_swigt__p_GDALMultiDimTranslateOptions,
   &_swigt__p_GDALNearblackOptions,
   &_swigt__p_GDALProgressFunc,
   &_swigt__p_GDALRasterAttributeTableShadow,
   &_swigt__p_GDALRasterBandShadow,
   &_swigt__p_GDALRasterizeOptions,
+  &_swigt__p_GDALRelationshipShadow,
   &_swigt__p_GDALTransformerInfoShadow,
   &_swigt__p_GDALTranslateOptions,
   &_swigt__p_GDALVectorTranslateOptions,
   &_swigt__p_GDALViewshedMode,
   &_swigt__p_GDALViewshedOutputType,
   &_swigt__p_GDALWarpAppOptions,
   &_swigt__p_GDAL_GCP,
@@ -45346,14 +47375,15 @@
 static swig_cast_info _swigc__p_GDALMultiDimInfoOptions[] = {  {&_swigt__p_GDALMultiDimInfoOptions, 0, 0, 0},{0, 0, 0, 0}};
 static swig_cast_info _swigc__p_GDALMultiDimTranslateOptions[] = {  {&_swigt__p_GDALMultiDimTranslateOptions, 0, 0, 0},{0, 0, 0, 0}};
 static swig_cast_info _swigc__p_GDALNearblackOptions[] = {  {&_swigt__p_GDALNearblackOptions, 0, 0, 0},{0, 0, 0, 0}};
 static swig_cast_info _swigc__p_GDALProgressFunc[] = {  {&_swigt__p_GDALProgressFunc, 0, 0, 0},{0, 0, 0, 0}};
 static swig_cast_info _swigc__p_GDALRasterAttributeTableShadow[] = {  {&_swigt__p_GDALRasterAttributeTableShadow, 0, 0, 0},{0, 0, 0, 0}};
 static swig_cast_info _swigc__p_GDALRasterBandShadow[] = {  {&_swigt__p_GDALRasterBandShadow, 0, 0, 0},{0, 0, 0, 0}};
 static swig_cast_info _swigc__p_GDALRasterizeOptions[] = {  {&_swigt__p_GDALRasterizeOptions, 0, 0, 0},{0, 0, 0, 0}};
+static swig_cast_info _swigc__p_GDALRelationshipShadow[] = {  {&_swigt__p_GDALRelationshipShadow, 0, 0, 0},{0, 0, 0, 0}};
 static swig_cast_info _swigc__p_GDALTransformerInfoShadow[] = {  {&_swigt__p_GDALTransformerInfoShadow, 0, 0, 0},{0, 0, 0, 0}};
 static swig_cast_info _swigc__p_GDALTranslateOptions[] = {  {&_swigt__p_GDALTranslateOptions, 0, 0, 0},{0, 0, 0, 0}};
 static swig_cast_info _swigc__p_GDALVectorTranslateOptions[] = {  {&_swigt__p_GDALVectorTranslateOptions, 0, 0, 0},{0, 0, 0, 0}};
 static swig_cast_info _swigc__p_GDALViewshedMode[] = {  {&_swigt__p_GDALViewshedMode, 0, 0, 0},{0, 0, 0, 0}};
 static swig_cast_info _swigc__p_GDALViewshedOutputType[] = {  {&_swigt__p_GDALViewshedOutputType, 0, 0, 0},{0, 0, 0, 0}};
 static swig_cast_info _swigc__p_GDALWarpAppOptions[] = {  {&_swigt__p_GDALWarpAppOptions, 0, 0, 0},{0, 0, 0, 0}};
 static swig_cast_info _swigc__p_GDAL_GCP[] = {  {&_swigt__p_GDAL_GCP, 0, 0, 0},{0, 0, 0, 0}};
@@ -45420,14 +47450,15 @@
   _swigc__p_GDALMultiDimInfoOptions,
   _swigc__p_GDALMultiDimTranslateOptions,
   _swigc__p_GDALNearblackOptions,
   _swigc__p_GDALProgressFunc,
   _swigc__p_GDALRasterAttributeTableShadow,
   _swigc__p_GDALRasterBandShadow,
   _swigc__p_GDALRasterizeOptions,
+  _swigc__p_GDALRelationshipShadow,
   _swigc__p_GDALTransformerInfoShadow,
   _swigc__p_GDALTranslateOptions,
   _swigc__p_GDALVectorTranslateOptions,
   _swigc__p_GDALViewshedMode,
   _swigc__p_GDALViewshedOutputType,
   _swigc__p_GDALWarpAppOptions,
   _swigc__p_GDAL_GCP,
```

### Comparing `pygdal-3.5.3.11/extensions/gdalconst_wrap.c` & `pygdal-3.6.4.11/extensions/gdalconst_wrap.c`

 * *Files 2% similar despite different names*

```diff
@@ -3623,47 +3623,68 @@
   SWIG_Python_SetConstant(d, "DMD_CONNECTION_PREFIX",SWIG_FromCharPtr(GDAL_DMD_CONNECTION_PREFIX));
   SWIG_Python_SetConstant(d, "DMD_EXTENSIONS",SWIG_FromCharPtr(GDAL_DMD_EXTENSIONS));
   SWIG_Python_SetConstant(d, "DMD_CREATIONOPTIONLIST",SWIG_FromCharPtr(GDAL_DMD_CREATIONOPTIONLIST));
   SWIG_Python_SetConstant(d, "DMD_MULTIDIM_DATASET_CREATIONOPTIONLIST",SWIG_FromCharPtr(GDAL_DMD_MULTIDIM_DATASET_CREATIONOPTIONLIST));
   SWIG_Python_SetConstant(d, "DMD_MULTIDIM_GROUP_CREATIONOPTIONLIST",SWIG_FromCharPtr(GDAL_DMD_MULTIDIM_GROUP_CREATIONOPTIONLIST));
   SWIG_Python_SetConstant(d, "DMD_MULTIDIM_DIMENSION_CREATIONOPTIONLIST",SWIG_FromCharPtr(GDAL_DMD_MULTIDIM_DIMENSION_CREATIONOPTIONLIST));
   SWIG_Python_SetConstant(d, "DMD_MULTIDIM_ARRAY_CREATIONOPTIONLIST",SWIG_FromCharPtr(GDAL_DMD_MULTIDIM_ARRAY_CREATIONOPTIONLIST));
+  SWIG_Python_SetConstant(d, "DMD_MULTIDIM_ARRAY_OPENOPTIONLIST",SWIG_FromCharPtr(GDAL_DMD_MULTIDIM_ARRAY_OPENOPTIONLIST));
   SWIG_Python_SetConstant(d, "DMD_MULTIDIM_ATTRIBUTE_CREATIONOPTIONLIST",SWIG_FromCharPtr(GDAL_DMD_MULTIDIM_ATTRIBUTE_CREATIONOPTIONLIST));
   SWIG_Python_SetConstant(d, "DMD_OPENOPTIONLIST",SWIG_FromCharPtr(GDAL_DMD_OPENOPTIONLIST));
   SWIG_Python_SetConstant(d, "DMD_CREATIONDATATYPES",SWIG_FromCharPtr(GDAL_DMD_CREATIONDATATYPES));
   SWIG_Python_SetConstant(d, "DMD_CREATIONFIELDDATATYPES",SWIG_FromCharPtr(GDAL_DMD_CREATIONFIELDDATATYPES));
   SWIG_Python_SetConstant(d, "DMD_CREATIONFIELDDATASUBTYPES",SWIG_FromCharPtr(GDAL_DMD_CREATIONFIELDDATASUBTYPES));
   SWIG_Python_SetConstant(d, "DMD_SUBDATASETS",SWIG_FromCharPtr(GDAL_DMD_SUBDATASETS));
   SWIG_Python_SetConstant(d, "DMD_CREATION_FIELD_DOMAIN_TYPES",SWIG_FromCharPtr(GDAL_DMD_CREATION_FIELD_DOMAIN_TYPES));
+  SWIG_Python_SetConstant(d, "DMD_ALTER_GEOM_FIELD_DEFN_FLAGS",SWIG_FromCharPtr(GDAL_DMD_ALTER_GEOM_FIELD_DEFN_FLAGS));
+  SWIG_Python_SetConstant(d, "DMD_SUPPORTED_SQL_DIALECTS",SWIG_FromCharPtr(GDAL_DMD_SUPPORTED_SQL_DIALECTS));
   SWIG_Python_SetConstant(d, "DCAP_OPEN",SWIG_FromCharPtr(GDAL_DCAP_OPEN));
   SWIG_Python_SetConstant(d, "DCAP_CREATE",SWIG_FromCharPtr(GDAL_DCAP_CREATE));
   SWIG_Python_SetConstant(d, "DCAP_CREATE_MULTIDIMENSIONAL",SWIG_FromCharPtr(GDAL_DCAP_CREATE_MULTIDIMENSIONAL));
   SWIG_Python_SetConstant(d, "DCAP_CREATECOPY",SWIG_FromCharPtr(GDAL_DCAP_CREATECOPY));
   SWIG_Python_SetConstant(d, "DCAP_CREATECOPY_MULTIDIMENSIONAL",SWIG_FromCharPtr(GDAL_DCAP_CREATECOPY_MULTIDIMENSIONAL));
   SWIG_Python_SetConstant(d, "DCAP_MULTIDIM_RASTER",SWIG_FromCharPtr(GDAL_DCAP_MULTIDIM_RASTER));
   SWIG_Python_SetConstant(d, "DCAP_SUBCREATECOPY",SWIG_FromCharPtr(GDAL_DCAP_SUBCREATECOPY));
   SWIG_Python_SetConstant(d, "DCAP_VIRTUALIO",SWIG_FromCharPtr(GDAL_DCAP_VIRTUALIO));
   SWIG_Python_SetConstant(d, "DCAP_RASTER",SWIG_FromCharPtr(GDAL_DCAP_RASTER));
   SWIG_Python_SetConstant(d, "DCAP_VECTOR",SWIG_FromCharPtr(GDAL_DCAP_VECTOR));
   SWIG_Python_SetConstant(d, "DCAP_GNM",SWIG_FromCharPtr(GDAL_DCAP_GNM));
+  SWIG_Python_SetConstant(d, "DCAP_CREATE_LAYER",SWIG_FromCharPtr(GDAL_DCAP_CREATE_LAYER));
+  SWIG_Python_SetConstant(d, "DCAP_DELETE_LAYER",SWIG_FromCharPtr(GDAL_DCAP_DELETE_LAYER));
+  SWIG_Python_SetConstant(d, "DCAP_CREATE_FIELD",SWIG_FromCharPtr(GDAL_DCAP_CREATE_FIELD));
+  SWIG_Python_SetConstant(d, "DCAP_DELETE_FIELD",SWIG_FromCharPtr(GDAL_DCAP_DELETE_FIELD));
+  SWIG_Python_SetConstant(d, "DCAP_REORDER_FIELDS",SWIG_FromCharPtr(GDAL_DCAP_REORDER_FIELDS));
+  SWIG_Python_SetConstant(d, "DMD_ALTER_FIELD_DEFN_FLAGS",SWIG_FromCharPtr(GDAL_DMD_ALTER_FIELD_DEFN_FLAGS));
   SWIG_Python_SetConstant(d, "DCAP_NOTNULL_FIELDS",SWIG_FromCharPtr(GDAL_DCAP_NOTNULL_FIELDS));
   SWIG_Python_SetConstant(d, "DCAP_UNIQUE_FIELDS",SWIG_FromCharPtr(GDAL_DCAP_UNIQUE_FIELDS));
   SWIG_Python_SetConstant(d, "DCAP_DEFAULT_FIELDS",SWIG_FromCharPtr(GDAL_DCAP_DEFAULT_FIELDS));
   SWIG_Python_SetConstant(d, "DCAP_NOTNULL_GEOMFIELDS",SWIG_FromCharPtr(GDAL_DCAP_NOTNULL_GEOMFIELDS));
   SWIG_Python_SetConstant(d, "DCAP_NONSPATIAL",SWIG_FromCharPtr(GDAL_DCAP_NONSPATIAL));
+  SWIG_Python_SetConstant(d, "DCAP_CURVE_GEOMETRIES",SWIG_FromCharPtr(GDAL_DCAP_CURVE_GEOMETRIES));
+  SWIG_Python_SetConstant(d, "DCAP_MEASURED_GEOMETRIES",SWIG_FromCharPtr(GDAL_DCAP_MEASURED_GEOMETRIES));
+  SWIG_Python_SetConstant(d, "DCAP_Z_GEOMETRIES",SWIG_FromCharPtr(GDAL_DCAP_Z_GEOMETRIES));
+  SWIG_Python_SetConstant(d, "DMD_GEOMETRY_FLAGS",SWIG_FromCharPtr(GDAL_DMD_GEOMETRY_FLAGS));
   SWIG_Python_SetConstant(d, "DCAP_FEATURE_STYLES",SWIG_FromCharPtr(GDAL_DCAP_FEATURE_STYLES));
   SWIG_Python_SetConstant(d, "DCAP_COORDINATE_EPOCH",SWIG_FromCharPtr(GDAL_DCAP_COORDINATE_EPOCH));
   SWIG_Python_SetConstant(d, "DCAP_MULTIPLE_VECTOR_LAYERS",SWIG_FromCharPtr(GDAL_DCAP_MULTIPLE_VECTOR_LAYERS));
   SWIG_Python_SetConstant(d, "DCAP_FIELD_DOMAINS",SWIG_FromCharPtr(GDAL_DCAP_FIELD_DOMAINS));
+  SWIG_Python_SetConstant(d, "DCAP_RELATIONSHIPS",SWIG_FromCharPtr(GDAL_DCAP_RELATIONSHIPS));
+  SWIG_Python_SetConstant(d, "GDAL_DCAP_CREATE_RELATIONSHIP",SWIG_FromCharPtr(GDAL_DCAP_CREATE_RELATIONSHIP));
+  SWIG_Python_SetConstant(d, "GDAL_DCAP_DELETE_RELATIONSHIP",SWIG_FromCharPtr(GDAL_DCAP_DELETE_RELATIONSHIP));
+  SWIG_Python_SetConstant(d, "GDAL_DCAP_UPDATE_RELATIONSHIP",SWIG_FromCharPtr(GDAL_DCAP_UPDATE_RELATIONSHIP));
+  SWIG_Python_SetConstant(d, "GDAL_DMD_RELATIONSHIP_FLAGS",SWIG_FromCharPtr(GDAL_DMD_RELATIONSHIP_FLAGS));
   SWIG_Python_SetConstant(d, "DCAP_RENAME_LAYERS",SWIG_FromCharPtr(GDAL_DCAP_RENAME_LAYERS));
   SWIG_Python_SetConstant(d, "DIM_TYPE_HORIZONTAL_X",SWIG_FromCharPtr(GDAL_DIM_TYPE_HORIZONTAL_X));
   SWIG_Python_SetConstant(d, "DIM_TYPE_HORIZONTAL_Y",SWIG_FromCharPtr(GDAL_DIM_TYPE_HORIZONTAL_Y));
   SWIG_Python_SetConstant(d, "DIM_TYPE_VERTICAL",SWIG_FromCharPtr(GDAL_DIM_TYPE_VERTICAL));
   SWIG_Python_SetConstant(d, "DIM_TYPE_TEMPORAL",SWIG_FromCharPtr(GDAL_DIM_TYPE_TEMPORAL));
   SWIG_Python_SetConstant(d, "DIM_TYPE_PARAMETRIC",SWIG_FromCharPtr(GDAL_DIM_TYPE_PARAMETRIC));
+  SWIG_Python_SetConstant(d, "GDsCAddRelationship",SWIG_FromCharPtr("AddRelationship"));
+  SWIG_Python_SetConstant(d, "GDsCDeleteRelationship",SWIG_FromCharPtr("DeleteRelationship"));
+  SWIG_Python_SetConstant(d, "GDsCUpdateRelationship",SWIG_FromCharPtr("UpdateRelationship"));
   SWIG_Python_SetConstant(d, "CPLES_BackslashQuotable",SWIG_From_int((int)(CPLES_BackslashQuotable)));
   SWIG_Python_SetConstant(d, "CPLES_XML",SWIG_From_int((int)(CPLES_XML)));
   SWIG_Python_SetConstant(d, "CPLES_XML_BUT_QUOTES",SWIG_From_int((int)(CPLES_XML_BUT_QUOTES)));
   SWIG_Python_SetConstant(d, "CPLES_URL",SWIG_From_int((int)(CPLES_URL)));
   SWIG_Python_SetConstant(d, "CPLES_SQL",SWIG_From_int((int)(CPLES_SQL)));
   SWIG_Python_SetConstant(d, "CPLES_SQLI",SWIG_From_int((int)(CPLES_SQLI)));
   SWIG_Python_SetConstant(d, "CPLES_CSV",SWIG_From_int((int)(CPLES_CSV)));
@@ -3701,14 +3722,21 @@
   SWIG_Python_SetConstant(d, "GARIO_PENDING",SWIG_From_int((int)(GARIO_PENDING)));
   SWIG_Python_SetConstant(d, "GARIO_UPDATE",SWIG_From_int((int)(GARIO_UPDATE)));
   SWIG_Python_SetConstant(d, "GARIO_ERROR",SWIG_From_int((int)(GARIO_ERROR)));
   SWIG_Python_SetConstant(d, "GARIO_COMPLETE",SWIG_From_int((int)(GARIO_COMPLETE)));
   SWIG_Python_SetConstant(d, "GTO_TIP",SWIG_From_int((int)(GTO_TIP)));
   SWIG_Python_SetConstant(d, "GTO_BIT",SWIG_From_int((int)(GTO_BIT)));
   SWIG_Python_SetConstant(d, "GTO_BSQ",SWIG_From_int((int)(GTO_BSQ)));
+  SWIG_Python_SetConstant(d, "GRC_ONE_TO_ONE",SWIG_From_int((int)(GRC_ONE_TO_ONE)));
+  SWIG_Python_SetConstant(d, "GRC_ONE_TO_MANY",SWIG_From_int((int)(GRC_ONE_TO_MANY)));
+  SWIG_Python_SetConstant(d, "GRC_MANY_TO_ONE",SWIG_From_int((int)(GRC_MANY_TO_ONE)));
+  SWIG_Python_SetConstant(d, "GRC_MANY_TO_MANY",SWIG_From_int((int)(GRC_MANY_TO_MANY)));
+  SWIG_Python_SetConstant(d, "GRT_COMPOSITE",SWIG_From_int((int)(GRT_COMPOSITE)));
+  SWIG_Python_SetConstant(d, "GRT_ASSOCIATION",SWIG_From_int((int)(GRT_ASSOCIATION)));
+  SWIG_Python_SetConstant(d, "GRT_AGGREGATION",SWIG_From_int((int)(GRT_AGGREGATION)));
   
   /* Initialize threading */
   SWIG_PYTHON_INITIALIZE_THREADS;
 #if PY_VERSION_HEX >= 0x03000000
   return m;
 #else
   return;
```

### Comparing `pygdal-3.5.3.11/extensions/ogr_wrap.cpp` & `pygdal-3.6.4.11/extensions/ogr_wrap.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -2690,44 +2690,48 @@
 
 
   #define SWIG_exception(code, msg) do { SWIG_Error(code, msg); SWIG_fail;; } while(0) 
 
 
 /* -------- TYPES TABLE (BEGIN) -------- */
 
-#define SWIGTYPE_p_GDALMajorObjectShadow swig_types[0]
-#define SWIGTYPE_p_GDALProgressFunc swig_types[1]
-#define SWIGTYPE_p_GIntBig swig_types[2]
-#define SWIGTYPE_p_OGRCodedValue swig_types[3]
-#define SWIGTYPE_p_OGRDataSourceShadow swig_types[4]
-#define SWIGTYPE_p_OGRDriverShadow swig_types[5]
-#define SWIGTYPE_p_OGRFeatureDefnShadow swig_types[6]
-#define SWIGTYPE_p_OGRFeatureShadow swig_types[7]
-#define SWIGTYPE_p_OGRFieldDefnShadow swig_types[8]
-#define SWIGTYPE_p_OGRFieldDomainShadow swig_types[9]
-#define SWIGTYPE_p_OGRGeomFieldDefnShadow swig_types[10]
-#define SWIGTYPE_p_OGRGeomTransformerShadow swig_types[11]
-#define SWIGTYPE_p_OGRGeometryShadow swig_types[12]
-#define SWIGTYPE_p_OGRLayerShadow swig_types[13]
-#define SWIGTYPE_p_OGRPreparedGeometryShadow swig_types[14]
-#define SWIGTYPE_p_OGRStyleTableShadow swig_types[15]
-#define SWIGTYPE_p_OSRCoordinateTransformationShadow swig_types[16]
-#define SWIGTYPE_p_OSRSpatialReferenceShadow swig_types[17]
-#define SWIGTYPE_p_char swig_types[18]
-#define SWIGTYPE_p_double swig_types[19]
-#define SWIGTYPE_p_f_double_p_q_const__char_p_void__int swig_types[20]
-#define SWIGTYPE_p_float swig_types[21]
-#define SWIGTYPE_p_int swig_types[22]
-#define SWIGTYPE_p_p_GIntBig swig_types[23]
-#define SWIGTYPE_p_p_char swig_types[24]
-#define SWIGTYPE_p_p_double swig_types[25]
-#define SWIGTYPE_p_p_int swig_types[26]
-#define SWIGTYPE_p_size_t swig_types[27]
-static swig_type_info *swig_types[29];
-static swig_module_info swig_module = {swig_types, 28, 0, 0, 0, 0};
+#define SWIGTYPE_p_ArrowArray swig_types[0]
+#define SWIGTYPE_p_ArrowArrayStream swig_types[1]
+#define SWIGTYPE_p_ArrowSchema swig_types[2]
+#define SWIGTYPE_p_GDALMajorObjectShadow swig_types[3]
+#define SWIGTYPE_p_GDALProgressFunc swig_types[4]
+#define SWIGTYPE_p_GIntBig swig_types[5]
+#define SWIGTYPE_p_OGRCodedValue swig_types[6]
+#define SWIGTYPE_p_OGRDataSourceShadow swig_types[7]
+#define SWIGTYPE_p_OGRDriverShadow swig_types[8]
+#define SWIGTYPE_p_OGRFeatureDefnShadow swig_types[9]
+#define SWIGTYPE_p_OGRFeatureShadow swig_types[10]
+#define SWIGTYPE_p_OGRFieldDefnShadow swig_types[11]
+#define SWIGTYPE_p_OGRFieldDomainShadow swig_types[12]
+#define SWIGTYPE_p_OGRGeomFieldDefnShadow swig_types[13]
+#define SWIGTYPE_p_OGRGeomTransformerShadow swig_types[14]
+#define SWIGTYPE_p_OGRGeometryShadow swig_types[15]
+#define SWIGTYPE_p_OGRLayerShadow swig_types[16]
+#define SWIGTYPE_p_OGRPreparedGeometryShadow swig_types[17]
+#define SWIGTYPE_p_OGRStyleTableShadow swig_types[18]
+#define SWIGTYPE_p_OSRCoordinateTransformationShadow swig_types[19]
+#define SWIGTYPE_p_OSRSpatialReferenceShadow swig_types[20]
+#define SWIGTYPE_p_char swig_types[21]
+#define SWIGTYPE_p_double swig_types[22]
+#define SWIGTYPE_p_f_double_p_q_const__char_p_void__int swig_types[23]
+#define SWIGTYPE_p_float swig_types[24]
+#define SWIGTYPE_p_int swig_types[25]
+#define SWIGTYPE_p_p_GIntBig swig_types[26]
+#define SWIGTYPE_p_p_OGRGeometryTypeCounter swig_types[27]
+#define SWIGTYPE_p_p_char swig_types[28]
+#define SWIGTYPE_p_p_double swig_types[29]
+#define SWIGTYPE_p_p_int swig_types[30]
+#define SWIGTYPE_p_size_t swig_types[31]
+static swig_type_info *swig_types[33];
+static swig_module_info swig_module = {swig_types, 32, 0, 0, 0, 0};
 #define SWIG_TypeQuery(name) SWIG_TypeQueryModule(&swig_module, &swig_module, name)
 #define SWIG_MangledTypeQuery(name) SWIG_MangledTypeQueryModule(&swig_module, &swig_module, name)
 
 /* -------- TYPES TABLE (END) -------- */
 
 #ifdef SWIG_TypeQuery
 # undef SWIG_TypeQuery
@@ -2823,28 +2827,32 @@
       _obj = obj;
       return *this;      
     }
   };
 }
 
 
+typedef void* VoidPtrAsLong;
+
+
 typedef char retStringAndCPLFree;
 
 
 #include <iostream>
 using namespace std;
 
 #define CPL_SUPRESS_CPLUSPLUS
 
 #include "gdal.h"
 #include "ogr_api.h"
 #include "ogr_core.h"
 #include "cpl_port.h"
 #include "cpl_string.h"
 #include "ogr_srs_api.h"
+#include "ogr_recordbatch.h"
 
 #define FIELD_INDEX_ERROR_TMPL "Invalid field index: '%i'"
 #define FIELD_NAME_ERROR_TMPL "Invalid field name: '%s'"
 
 typedef void GDALMajorObjectShadow;
 
 #ifdef DEBUG
@@ -3161,15 +3169,15 @@
 PyProgressProxy( double dfComplete, const char *pszMessage, void *pData )
 
 {
     PyProgressData *psInfo = (PyProgressData *) pData;
     PyObject *psArgs, *psResult;
     int      bContinue = TRUE;
 
-    if( psInfo->nLastReported == (int) (100.0 * dfComplete) )
+    if( dfComplete > 0 && psInfo->nLastReported == (int) (100.0 * dfComplete) )
         return TRUE;
 
     if( psInfo->psPyCallback == NULL || psInfo->psPyCallback == Py_None )
         return TRUE;
 
     psInfo->nLastReported = (int) (100.0 * dfComplete);
 
@@ -3778,14 +3786,68 @@
   }
 SWIGINTERN OGRErr OGRDataSourceShadow_CommitTransaction(OGRDataSourceShadow *self){
     return GDALDatasetCommitTransaction(self);
   }
 SWIGINTERN OGRErr OGRDataSourceShadow_RollbackTransaction(OGRDataSourceShadow *self){
     return GDALDatasetRollbackTransaction(self);
   }
+SWIGINTERN void delete_ArrowArray(ArrowArray *self){
+    if( self->release )
+      self->release(self);
+    free(self);
+  }
+SWIGINTERN VoidPtrAsLong ArrowArray__getPtr(ArrowArray *self){
+    return self;
+  }
+SWIGINTERN GIntBig ArrowArray_GetChildrenCount(ArrowArray *self){
+    return self->n_children;
+  }
+SWIGINTERN GIntBig ArrowArray_GetLength(ArrowArray *self){
+    return self->length;
+  }
+SWIGINTERN void delete_ArrowSchema(ArrowSchema *self){
+    if( self->release )
+      self->release(self);
+    free(self);
+  }
+SWIGINTERN VoidPtrAsLong ArrowSchema__getPtr(ArrowSchema *self){
+    return self;
+  }
+SWIGINTERN GIntBig ArrowSchema_GetChildrenCount(ArrowSchema *self){
+    return self->n_children;
+  }
+SWIGINTERN void delete_ArrowArrayStream(ArrowArrayStream *self){
+    if( self->release )
+      self->release(self);
+    free(self);
+  }
+SWIGINTERN ArrowSchema *ArrowArrayStream_GetSchema(ArrowArrayStream *self){
+      struct ArrowSchema* schema = (struct ArrowSchema* )malloc(sizeof(struct ArrowSchema));
+      if( self->get_schema(self, schema) == 0 )
+      {
+          return schema;
+      }
+      else
+      {
+          free(schema);
+          return NULL;
+      }
+  }
+SWIGINTERN ArrowArray *ArrowArrayStream_GetNextRecordBatch(ArrowArrayStream *self,char **options=NULL){
+      struct ArrowArray* array = (struct ArrowArray* )malloc(sizeof(struct ArrowArray));
+      if( self->get_next(self, array) == 0 && array->release != NULL )
+      {
+          return array;
+      }
+      else
+      {
+          free(array);
+          return NULL;
+      }
+  }
 SWIGINTERN OGRErr OGRLayerShadow_Rename(OGRLayerShadow *self,char const *new_name){
     return OGR_L_Rename( self, new_name);
   }
 SWIGINTERN int OGRLayerShadow_GetRefCount(OGRLayerShadow *self){
     return OGR_L_GetRefCount(self);
   }
 SWIGINTERN void OGRLayerShadow_SetSpatialFilter__SWIG_0(OGRLayerShadow *self,OGRGeometryShadow *filter){
@@ -3832,14 +3894,17 @@
   }
 SWIGINTERN OGRErr OGRLayerShadow_SetFeature(OGRLayerShadow *self,OGRFeatureShadow *feature){
     return OGR_L_SetFeature(self, feature);
   }
 SWIGINTERN OGRErr OGRLayerShadow_CreateFeature(OGRLayerShadow *self,OGRFeatureShadow *feature){
     return OGR_L_CreateFeature(self, feature);
   }
+SWIGINTERN OGRErr OGRLayerShadow_UpsertFeature(OGRLayerShadow *self,OGRFeatureShadow *feature){
+    return OGR_L_UpsertFeature(self, feature);
+  }
 SWIGINTERN OGRErr OGRLayerShadow_DeleteFeature(OGRLayerShadow *self,GIntBig fid){
     return OGR_L_DeleteFeature(self, fid);
   }
 SWIGINTERN OGRErr OGRLayerShadow_SyncToDisk(OGRLayerShadow *self){
     return OGR_L_SyncToDisk(self);
   }
 SWIGINTERN OGRFeatureDefnShadow *OGRLayerShadow_GetLayerDefn(OGRLayerShadow *self){
@@ -3908,14 +3973,17 @@
       return 6;
     }
     return OGR_L_ReorderFields(self, pList);
   }
 SWIGINTERN OGRErr OGRLayerShadow_AlterFieldDefn(OGRLayerShadow *self,int iField,OGRFieldDefnShadow *field_def,int nFlags){
     return OGR_L_AlterFieldDefn(self, iField, field_def, nFlags);
   }
+SWIGINTERN OGRErr OGRLayerShadow_AlterGeomFieldDefn(OGRLayerShadow *self,int iGeomField,OGRGeomFieldDefnShadow const *field_def,int nFlags){
+    return OGR_L_AlterGeomFieldDefn(self, iGeomField, const_cast<OGRGeomFieldDefnShadow*>(field_def), nFlags);
+  }
 SWIGINTERN OGRErr OGRLayerShadow_CreateGeomField(OGRLayerShadow *self,OGRGeomFieldDefnShadow *field_def,int approx_ok=1){
     return OGR_L_CreateGeomField(self, field_def, approx_ok);
   }
 SWIGINTERN OGRErr OGRLayerShadow_StartTransaction(OGRLayerShadow *self){
     return OGR_L_StartTransaction(self);
   }
 SWIGINTERN OGRErr OGRLayerShadow_CommitTransaction(OGRLayerShadow *self){
@@ -3963,14 +4031,27 @@
 SWIGINTERN OGRStyleTableShadow *OGRLayerShadow_GetStyleTable(OGRLayerShadow *self){
     return (OGRStyleTableShadow*) OGR_L_GetStyleTable(self);
   }
 SWIGINTERN void OGRLayerShadow_SetStyleTable(OGRLayerShadow *self,OGRStyleTableShadow *table){
     if( table != NULL )
         OGR_L_SetStyleTable(self, (OGRStyleTableH) table);
   }
+SWIGINTERN ArrowArrayStream *OGRLayerShadow_GetArrowStream(OGRLayerShadow *self,char **options=NULL){
+      struct ArrowArrayStream* stream = (struct ArrowArrayStream* )malloc(sizeof(struct ArrowArrayStream));
+      if( OGR_L_GetArrowStream(self, stream, options) )
+          return stream;
+      else
+      {
+          free(stream);
+          return NULL;
+      }
+  }
+SWIGINTERN void OGRLayerShadow_GetGeometryTypes(OGRLayerShadow *self,OGRGeometryTypeCounter **ppRet,int *pnEntryCount,int geom_field=0,int flags=0,GDALProgressFunc callback=NULL,void *callback_data=NULL){
+        *ppRet = OGR_L_GetGeometryTypes(self, geom_field, flags, pnEntryCount, callback, callback_data);
+    }
 SWIGINTERN void delete_OGRFeatureShadow(OGRFeatureShadow *self){
     OGR_F_Destroy(self);
   }
 SWIGINTERN OGRFeatureShadow *new_OGRFeatureShadow(OGRFeatureDefnShadow *feature_def){
       return (OGRFeatureShadow*) OGR_F_Create( feature_def );
   }
 SWIGINTERN OGRFeatureDefnShadow *OGRFeatureShadow_GetDefnRef(OGRFeatureShadow *self){
@@ -5195,14 +5276,31 @@
   }
 SWIGINTERN OGRGeometryShadow *OGRGeometryShadow_GetBoundary(OGRGeometryShadow *self){
     return (OGRGeometryShadow*) OGR_G_Boundary(self);
   }
 SWIGINTERN OGRGeometryShadow *OGRGeometryShadow_ConvexHull(OGRGeometryShadow *self){
     return (OGRGeometryShadow*) OGR_G_ConvexHull(self);
   }
+
+SWIGINTERN int
+SWIG_AsVal_bool (PyObject *obj, bool *val)
+{
+  int r;
+  if (!PyBool_Check(obj))
+    return SWIG_ERROR;
+  r = PyObject_IsTrue(obj);
+  if (r == -1)
+    return SWIG_ERROR;
+  if (val) *val = r ? true : false;
+  return SWIG_OK;
+}
+
+SWIGINTERN OGRGeometryShadow *OGRGeometryShadow_ConcaveHull(OGRGeometryShadow *self,double ratio,bool allowHoles){
+    return (OGRGeometryShadow*) OGR_G_ConcaveHull(self, ratio, allowHoles);
+  }
 SWIGINTERN OGRGeometryShadow *OGRGeometryShadow_MakeValid(OGRGeometryShadow *self,char **options=NULL){
     return (OGRGeometryShadow*) OGR_G_MakeValidEx(self, options);
   }
 SWIGINTERN OGRGeometryShadow *OGRGeometryShadow_Normalize(OGRGeometryShadow *self){
     return (OGRGeometryShadow*) OGR_G_Normalize(self);
   }
 SWIGINTERN OGRGeometryShadow *OGRGeometryShadow_RemoveLowerDimensionSubGeoms(OGRGeometryShadow *self){
@@ -5539,28 +5637,14 @@
                                                             &sMin,
                                                             minIsInclusive,
                                                             &sMax,
                                                             maxIsInclusive );
 }
 
 
-SWIGINTERN int
-SWIG_AsVal_bool (PyObject *obj, bool *val)
-{
-  int r;
-  if (!PyBool_Check(obj))
-    return SWIG_ERROR;
-  r = PyObject_IsTrue(obj);
-  if (r == -1)
-    return SWIG_ERROR;
-  if (val) *val = r ? true : false;
-  return SWIG_OK;
-}
-
-
 static
 OGRFieldDomainShadow* CreateGlobFieldDomain( const char *name,
                                              const char* description,
                                              OGRFieldType type,
                                              OGRFieldSubType subtype,
                                              const char* glob ) {
   return (OGRFieldDomainShadow*) OGR_GlobFldDomain_Create( name,
@@ -8767,14 +8851,471 @@
 SWIGINTERN PyObject *DataSource_swigregister(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *obj;
   if (!SWIG_Python_UnpackTuple(args, "swigregister", 1, 1, &obj)) return NULL;
   SWIG_TypeNewClientData(SWIGTYPE_p_OGRDataSourceShadow, SWIG_NewClientData(obj));
   return SWIG_Py_Void();
 }
 
+SWIGINTERN PyObject *_wrap_delete_ArrowArray(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  ArrowArray *arg1 = (ArrowArray *) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  PyObject *swig_obj[1] ;
+  
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ArrowArray, SWIG_POINTER_DISOWN |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "delete_ArrowArray" "', argument " "1"" of type '" "ArrowArray *""'"); 
+  }
+  arg1 = reinterpret_cast< ArrowArray * >(argp1);
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      delete_ArrowArray(arg1);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  resultobj = SWIG_Py_Void();
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  return NULL;
+}
+
+
+SWIGINTERN PyObject *_wrap_ArrowArray__getPtr(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  ArrowArray *arg1 = (ArrowArray *) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  PyObject *swig_obj[1] ;
+  VoidPtrAsLong result;
+  
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ArrowArray, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ArrowArray__getPtr" "', argument " "1"" of type '" "ArrowArray *""'"); 
+  }
+  arg1 = reinterpret_cast< ArrowArray * >(argp1);
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      result = (VoidPtrAsLong)ArrowArray__getPtr(arg1);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  {
+    resultobj = PyLong_FromVoidPtr(result);
+  }
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  return NULL;
+}
+
+
+SWIGINTERN PyObject *_wrap_ArrowArray_GetChildrenCount(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  ArrowArray *arg1 = (ArrowArray *) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  PyObject *swig_obj[1] ;
+  GIntBig result;
+  
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ArrowArray, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ArrowArray_GetChildrenCount" "', argument " "1"" of type '" "ArrowArray *""'"); 
+  }
+  arg1 = reinterpret_cast< ArrowArray * >(argp1);
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      result = ArrowArray_GetChildrenCount(arg1);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  {
+    resultobj = PyLong_FromLongLong(result);
+  }
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  return NULL;
+}
+
+
+SWIGINTERN PyObject *_wrap_ArrowArray_GetLength(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  ArrowArray *arg1 = (ArrowArray *) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  PyObject *swig_obj[1] ;
+  GIntBig result;
+  
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ArrowArray, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ArrowArray_GetLength" "', argument " "1"" of type '" "ArrowArray *""'"); 
+  }
+  arg1 = reinterpret_cast< ArrowArray * >(argp1);
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      result = ArrowArray_GetLength(arg1);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  {
+    resultobj = PyLong_FromLongLong(result);
+  }
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  return NULL;
+}
+
+
+SWIGINTERN PyObject *ArrowArray_swigregister(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *obj;
+  if (!SWIG_Python_UnpackTuple(args, "swigregister", 1, 1, &obj)) return NULL;
+  SWIG_TypeNewClientData(SWIGTYPE_p_ArrowArray, SWIG_NewClientData(obj));
+  return SWIG_Py_Void();
+}
+
+SWIGINTERN PyObject *_wrap_delete_ArrowSchema(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  ArrowSchema *arg1 = (ArrowSchema *) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  PyObject *swig_obj[1] ;
+  
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ArrowSchema, SWIG_POINTER_DISOWN |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "delete_ArrowSchema" "', argument " "1"" of type '" "ArrowSchema *""'"); 
+  }
+  arg1 = reinterpret_cast< ArrowSchema * >(argp1);
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      delete_ArrowSchema(arg1);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  resultobj = SWIG_Py_Void();
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  return NULL;
+}
+
+
+SWIGINTERN PyObject *_wrap_ArrowSchema__getPtr(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  ArrowSchema *arg1 = (ArrowSchema *) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  PyObject *swig_obj[1] ;
+  VoidPtrAsLong result;
+  
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ArrowSchema, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ArrowSchema__getPtr" "', argument " "1"" of type '" "ArrowSchema *""'"); 
+  }
+  arg1 = reinterpret_cast< ArrowSchema * >(argp1);
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      result = (VoidPtrAsLong)ArrowSchema__getPtr(arg1);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  {
+    resultobj = PyLong_FromVoidPtr(result);
+  }
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  return NULL;
+}
+
+
+SWIGINTERN PyObject *_wrap_ArrowSchema_GetChildrenCount(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  ArrowSchema *arg1 = (ArrowSchema *) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  PyObject *swig_obj[1] ;
+  GIntBig result;
+  
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ArrowSchema, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ArrowSchema_GetChildrenCount" "', argument " "1"" of type '" "ArrowSchema *""'"); 
+  }
+  arg1 = reinterpret_cast< ArrowSchema * >(argp1);
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      result = ArrowSchema_GetChildrenCount(arg1);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  {
+    resultobj = PyLong_FromLongLong(result);
+  }
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  return NULL;
+}
+
+
+SWIGINTERN PyObject *ArrowSchema_swigregister(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *obj;
+  if (!SWIG_Python_UnpackTuple(args, "swigregister", 1, 1, &obj)) return NULL;
+  SWIG_TypeNewClientData(SWIGTYPE_p_ArrowSchema, SWIG_NewClientData(obj));
+  return SWIG_Py_Void();
+}
+
+SWIGINTERN PyObject *_wrap_delete_ArrowArrayStream(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  ArrowArrayStream *arg1 = (ArrowArrayStream *) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  PyObject *swig_obj[1] ;
+  
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ArrowArrayStream, SWIG_POINTER_DISOWN |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "delete_ArrowArrayStream" "', argument " "1"" of type '" "ArrowArrayStream *""'"); 
+  }
+  arg1 = reinterpret_cast< ArrowArrayStream * >(argp1);
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      delete_ArrowArrayStream(arg1);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  resultobj = SWIG_Py_Void();
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  return NULL;
+}
+
+
+SWIGINTERN PyObject *_wrap_ArrowArrayStream_GetSchema(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  ArrowArrayStream *arg1 = (ArrowArrayStream *) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  PyObject *swig_obj[1] ;
+  ArrowSchema *result = 0 ;
+  
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ArrowArrayStream, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ArrowArrayStream_GetSchema" "', argument " "1"" of type '" "ArrowArrayStream *""'"); 
+  }
+  arg1 = reinterpret_cast< ArrowArrayStream * >(argp1);
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      result = (ArrowSchema *)ArrowArrayStream_GetSchema(arg1);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  resultobj = SWIG_NewPointerObj(SWIG_as_voidptr(result), SWIGTYPE_p_ArrowSchema, SWIG_POINTER_OWN |  0 );
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  return NULL;
+}
+
+
+SWIGINTERN PyObject *_wrap_ArrowArrayStream_GetNextRecordBatch(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  ArrowArrayStream *arg1 = (ArrowArrayStream *) 0 ;
+  char **arg2 = (char **) NULL ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  PyObject *swig_obj[2] ;
+  ArrowArray *result = 0 ;
+  
+  if (!SWIG_Python_UnpackTuple(args, "ArrowArrayStream_GetNextRecordBatch", 1, 2, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ArrowArrayStream, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ArrowArrayStream_GetNextRecordBatch" "', argument " "1"" of type '" "ArrowArrayStream *""'"); 
+  }
+  arg1 = reinterpret_cast< ArrowArrayStream * >(argp1);
+  if (swig_obj[1]) {
+    {
+      /* %typemap(in) char **options */
+      int bErr = FALSE;
+      arg2 = CSLFromPySequence(swig_obj[1], &bErr);
+      if( bErr )
+      {
+        SWIG_fail;
+      }
+    }
+  }
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      result = (ArrowArray *)ArrowArrayStream_GetNextRecordBatch(arg1,arg2);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  resultobj = SWIG_NewPointerObj(SWIG_as_voidptr(result), SWIGTYPE_p_ArrowArray, SWIG_POINTER_OWN |  0 );
+  {
+    /* %typemap(freearg) char **options */
+    CSLDestroy( arg2 );
+  }
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  {
+    /* %typemap(freearg) char **options */
+    CSLDestroy( arg2 );
+  }
+  return NULL;
+}
+
+
+SWIGINTERN PyObject *ArrowArrayStream_swigregister(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *obj;
+  if (!SWIG_Python_UnpackTuple(args, "swigregister", 1, 1, &obj)) return NULL;
+  SWIG_TypeNewClientData(SWIGTYPE_p_ArrowArrayStream, SWIG_NewClientData(obj));
+  return SWIG_Py_Void();
+}
+
 SWIGINTERN PyObject *_wrap_Layer_Rename(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
   OGRLayerShadow *arg1 = (OGRLayerShadow *) 0 ;
   char *arg2 = (char *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   int res2 ;
@@ -9865,14 +10406,83 @@
   if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
   return resultobj;
 fail:
   return NULL;
 }
 
 
+SWIGINTERN PyObject *_wrap_Layer_UpsertFeature(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  OGRLayerShadow *arg1 = (OGRLayerShadow *) 0 ;
+  OGRFeatureShadow *arg2 = (OGRFeatureShadow *) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  void *argp2 = 0 ;
+  int res2 = 0 ;
+  PyObject *swig_obj[2] ;
+  OGRErr result;
+  
+  if (!SWIG_Python_UnpackTuple(args, "Layer_UpsertFeature", 2, 2, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_OGRLayerShadow, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "Layer_UpsertFeature" "', argument " "1"" of type '" "OGRLayerShadow *""'"); 
+  }
+  arg1 = reinterpret_cast< OGRLayerShadow * >(argp1);
+  res2 = SWIG_ConvertPtr(swig_obj[1], &argp2,SWIGTYPE_p_OGRFeatureShadow, 0 |  0 );
+  if (!SWIG_IsOK(res2)) {
+    SWIG_exception_fail(SWIG_ArgError(res2), "in method '" "Layer_UpsertFeature" "', argument " "2"" of type '" "OGRFeatureShadow *""'"); 
+  }
+  arg2 = reinterpret_cast< OGRFeatureShadow * >(argp2);
+  {
+    if (!arg2) {
+      SWIG_exception(SWIG_ValueError,"Received a NULL pointer.");
+    }
+  }
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      result = (OGRErr)OGRLayerShadow_UpsertFeature(arg1,arg2);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  {
+    /* %typemap(out) OGRErr */
+    if ( result != 0 && bUseExceptions) {
+      const char* pszMessage = CPLGetLastErrorMsg();
+      if( pszMessage[0] != '\0' )
+      PyErr_SetString( PyExc_RuntimeError, pszMessage );
+      else
+      PyErr_SetString( PyExc_RuntimeError, OGRErrMessages(result) );
+      SWIG_fail;
+    }
+  }
+  {
+    /* %typemap(ret) OGRErr */
+    if ( ReturnSame(resultobj == Py_None || resultobj == 0) ) {
+      resultobj = PyInt_FromLong( result );
+    }
+  }
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  return NULL;
+}
+
+
 SWIGINTERN PyObject *_wrap_Layer_DeleteFeature(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
   OGRLayerShadow *arg1 = (OGRLayerShadow *) 0 ;
   GIntBig arg2 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   PyObject *swig_obj[2] ;
@@ -10089,15 +10699,15 @@
   double *arg2 ;
   int *arg3 = (int *) NULL ;
   int arg4 = (int) 1 ;
   int arg5 = (int) 0 ;
   int arg6 = (int) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
-  double argout2[6] ;
+  double argout2[4] ;
   int isvalid2 ;
   int val4 ;
   int ecode4 = 0 ;
   int val5 ;
   int ecode5 = 0 ;
   int val6 ;
   int ecode6 = 0 ;
@@ -10106,15 +10716,15 @@
   PyObject * obj2 = 0 ;
   PyObject * obj3 = 0 ;
   char * kwnames[] = {
     (char *)"self",  (char *)"force",  (char *)"can_return_null",  (char *)"geom_field",  NULL 
   };
   
   {
-    /* %typemap(in) (double argout2[4], int* isvalid2) */
+    /* %typemap(in,numinputs=0) (double argout2[4], int* isvalid2) */
     arg2 = argout2;
     arg3 = &isvalid2;
   }
   if (!PyArg_ParseTupleAndKeywords(args, kwargs, "O|OOO:Layer_GetExtent", kwnames, &obj0, &obj1, &obj2, &obj3)) SWIG_fail;
   res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_OGRLayerShadow, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "Layer_GetExtent" "', argument " "1"" of type '" "OGRLayerShadow *""'"); 
@@ -10609,14 +11219,99 @@
   if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
   return resultobj;
 fail:
   return NULL;
 }
 
 
+SWIGINTERN PyObject *_wrap_Layer_AlterGeomFieldDefn(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  OGRLayerShadow *arg1 = (OGRLayerShadow *) 0 ;
+  int arg2 ;
+  OGRGeomFieldDefnShadow *arg3 = (OGRGeomFieldDefnShadow *) 0 ;
+  int arg4 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  int val2 ;
+  int ecode2 = 0 ;
+  void *argp3 = 0 ;
+  int res3 = 0 ;
+  int val4 ;
+  int ecode4 = 0 ;
+  PyObject *swig_obj[4] ;
+  OGRErr result;
+  
+  if (!SWIG_Python_UnpackTuple(args, "Layer_AlterGeomFieldDefn", 4, 4, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_OGRLayerShadow, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "Layer_AlterGeomFieldDefn" "', argument " "1"" of type '" "OGRLayerShadow *""'"); 
+  }
+  arg1 = reinterpret_cast< OGRLayerShadow * >(argp1);
+  ecode2 = SWIG_AsVal_int(swig_obj[1], &val2);
+  if (!SWIG_IsOK(ecode2)) {
+    SWIG_exception_fail(SWIG_ArgError(ecode2), "in method '" "Layer_AlterGeomFieldDefn" "', argument " "2"" of type '" "int""'");
+  } 
+  arg2 = static_cast< int >(val2);
+  res3 = SWIG_ConvertPtr(swig_obj[2], &argp3,SWIGTYPE_p_OGRGeomFieldDefnShadow, 0 |  0 );
+  if (!SWIG_IsOK(res3)) {
+    SWIG_exception_fail(SWIG_ArgError(res3), "in method '" "Layer_AlterGeomFieldDefn" "', argument " "3"" of type '" "OGRGeomFieldDefnShadow const *""'"); 
+  }
+  arg3 = reinterpret_cast< OGRGeomFieldDefnShadow * >(argp3);
+  ecode4 = SWIG_AsVal_int(swig_obj[3], &val4);
+  if (!SWIG_IsOK(ecode4)) {
+    SWIG_exception_fail(SWIG_ArgError(ecode4), "in method '" "Layer_AlterGeomFieldDefn" "', argument " "4"" of type '" "int""'");
+  } 
+  arg4 = static_cast< int >(val4);
+  {
+    if (!arg3) {
+      SWIG_exception(SWIG_ValueError,"Received a NULL pointer.");
+    }
+  }
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      result = (OGRErr)OGRLayerShadow_AlterGeomFieldDefn(arg1,arg2,(OGRGeomFieldDefnShadow const *)arg3,arg4);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  {
+    /* %typemap(out) OGRErr */
+    if ( result != 0 && bUseExceptions) {
+      const char* pszMessage = CPLGetLastErrorMsg();
+      if( pszMessage[0] != '\0' )
+      PyErr_SetString( PyExc_RuntimeError, pszMessage );
+      else
+      PyErr_SetString( PyExc_RuntimeError, OGRErrMessages(result) );
+      SWIG_fail;
+    }
+  }
+  {
+    /* %typemap(ret) OGRErr */
+    if ( ReturnSame(resultobj == Py_None || resultobj == 0) ) {
+      resultobj = PyInt_FromLong( result );
+    }
+  }
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  return NULL;
+}
+
+
 SWIGINTERN PyObject *_wrap_Layer_CreateGeomField(PyObject *SWIGUNUSEDPARM(self), PyObject *args, PyObject *kwargs) {
   PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
   OGRLayerShadow *arg1 = (OGRLayerShadow *) 0 ;
   OGRGeomFieldDefnShadow *arg2 = (OGRGeomFieldDefnShadow *) 0 ;
   int arg3 = (int) 1 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
@@ -12324,14 +13019,242 @@
   if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
   return resultobj;
 fail:
   return NULL;
 }
 
 
+SWIGINTERN PyObject *_wrap_Layer_GetArrowStream(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  OGRLayerShadow *arg1 = (OGRLayerShadow *) 0 ;
+  char **arg2 = (char **) NULL ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  PyObject *swig_obj[2] ;
+  ArrowArrayStream *result = 0 ;
+  
+  if (!SWIG_Python_UnpackTuple(args, "Layer_GetArrowStream", 1, 2, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_OGRLayerShadow, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "Layer_GetArrowStream" "', argument " "1"" of type '" "OGRLayerShadow *""'"); 
+  }
+  arg1 = reinterpret_cast< OGRLayerShadow * >(argp1);
+  if (swig_obj[1]) {
+    {
+      /* %typemap(in) char **options */
+      int bErr = FALSE;
+      arg2 = CSLFromPySequence(swig_obj[1], &bErr);
+      if( bErr )
+      {
+        SWIG_fail;
+      }
+    }
+  }
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      result = (ArrowArrayStream *)OGRLayerShadow_GetArrowStream(arg1,arg2);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  resultobj = SWIG_NewPointerObj(SWIG_as_voidptr(result), SWIGTYPE_p_ArrowArrayStream, SWIG_POINTER_OWN |  0 );
+  {
+    /* %typemap(freearg) char **options */
+    CSLDestroy( arg2 );
+  }
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  {
+    /* %typemap(freearg) char **options */
+    CSLDestroy( arg2 );
+  }
+  return NULL;
+}
+
+
+SWIGINTERN PyObject *_wrap_Layer_GetGeometryTypes(PyObject *SWIGUNUSEDPARM(self), PyObject *args, PyObject *kwargs) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  OGRLayerShadow *arg1 = (OGRLayerShadow *) 0 ;
+  OGRGeometryTypeCounter **arg2 = (OGRGeometryTypeCounter **) 0 ;
+  int *arg3 = (int *) 0 ;
+  int arg4 = (int) 0 ;
+  int arg5 = (int) 0 ;
+  GDALProgressFunc arg6 = (GDALProgressFunc) NULL ;
+  void *arg7 = (void *) NULL ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  OGRGeometryTypeCounter *pRet2 = NULL ;
+  int nEntryCount2 = 0 ;
+  int val4 ;
+  int ecode4 = 0 ;
+  int val5 ;
+  int ecode5 = 0 ;
+  PyObject * obj0 = 0 ;
+  PyObject * obj1 = 0 ;
+  PyObject * obj2 = 0 ;
+  PyObject * obj3 = 0 ;
+  PyObject * obj4 = 0 ;
+  char * kwnames[] = {
+    (char *)"self",  (char *)"geom_field",  (char *)"flags",  (char *)"callback",  (char *)"callback_data",  NULL 
+  };
+  
+  /* %typemap(arginit) ( const char* callback_data=NULL)  */
+  PyProgressData *psProgressInfo;
+  psProgressInfo = (PyProgressData *) CPLCalloc(1,sizeof(PyProgressData));
+  psProgressInfo->nLastReported = -1;
+  psProgressInfo->psPyCallback = NULL;
+  psProgressInfo->psPyCallbackData = NULL;
+  arg7 = psProgressInfo;
+  {
+    /* %typemap(in,numinputs=0) (OGRGeometryTypeCounter** ppRet, int* pnEntryCount) */
+    arg2 = &pRet2;
+    arg3 = &nEntryCount2;
+  }
+  if (!PyArg_ParseTupleAndKeywords(args, kwargs, "O|OOOO:Layer_GetGeometryTypes", kwnames, &obj0, &obj1, &obj2, &obj3, &obj4)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_OGRLayerShadow, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "Layer_GetGeometryTypes" "', argument " "1"" of type '" "OGRLayerShadow *""'"); 
+  }
+  arg1 = reinterpret_cast< OGRLayerShadow * >(argp1);
+  if (obj1) {
+    ecode4 = SWIG_AsVal_int(obj1, &val4);
+    if (!SWIG_IsOK(ecode4)) {
+      SWIG_exception_fail(SWIG_ArgError(ecode4), "in method '" "Layer_GetGeometryTypes" "', argument " "4"" of type '" "int""'");
+    } 
+    arg4 = static_cast< int >(val4);
+  }
+  if (obj2) {
+    ecode5 = SWIG_AsVal_int(obj2, &val5);
+    if (!SWIG_IsOK(ecode5)) {
+      SWIG_exception_fail(SWIG_ArgError(ecode5), "in method '" "Layer_GetGeometryTypes" "', argument " "5"" of type '" "int""'");
+    } 
+    arg5 = static_cast< int >(val5);
+  }
+  if (obj3) {
+    {
+      /* %typemap(in) (GDALProgressFunc callback = NULL) */
+      /* callback_func typemap */
+      
+      /* In some cases 0 is passed instead of None. */
+      /* See https://github.com/OSGeo/gdal/pull/219 */
+      if ( PyLong_Check(obj3) || PyInt_Check(obj3) )
+      {
+        if( PyLong_AsLong(obj3) == 0 )
+        {
+          obj3 = Py_None;
+        }
+      }
+      
+      if (obj3 && obj3 != Py_None ) {
+        void* cbfunction = NULL;
+        CPL_IGNORE_RET_VAL(SWIG_ConvertPtr( obj3,
+            (void**)&cbfunction,
+            SWIGTYPE_p_f_double_p_q_const__char_p_void__int,
+            SWIG_POINTER_EXCEPTION | 0 ));
+        
+        if ( cbfunction == GDALTermProgress ) {
+          arg6 = GDALTermProgress;
+        } else {
+          if (!PyCallable_Check(obj3)) {
+            PyErr_SetString( PyExc_RuntimeError,
+              "Object given is not a Python function" );
+            SWIG_fail;
+          }
+          psProgressInfo->psPyCallback = obj3;
+          arg6 = PyProgressProxy;
+        }
+        
+      }
+      
+    }
+  }
+  if (obj4) {
+    {
+      /* %typemap(in) ( void* callback_data=NULL)  */
+      psProgressInfo->psPyCallbackData = obj4 ;
+    }
+  }
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      OGRLayerShadow_GetGeometryTypes(arg1,arg2,arg3,arg4,arg5,arg6,arg7);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  resultobj = SWIG_Py_Void();
+  {
+    /* %typemap(argout)  (OGRGeometryTypeCounter** ppRet, int* pnEntryCount) */
+    Py_DECREF(resultobj);
+    int nEntryCount = *(arg3);
+    OGRGeometryTypeCounter* pRet = *(arg2);
+    if( pRet == NULL )
+    {
+      PyErr_SetString( PyExc_RuntimeError, CPLGetLastErrorMsg() );
+      SWIG_fail;
+    }
+    resultobj = PyDict_New();
+    for(int i = 0; i < nEntryCount; ++ i)
+    {
+      PyObject *key = PyInt_FromLong( (int)(pRet[i].eGeomType) );
+      PyObject *val = PyLong_FromLongLong( pRet[i].nCount );
+      PyDict_SetItem(resultobj, key, val );
+      Py_DECREF(key);
+      Py_DECREF(val);
+    }
+  }
+  {
+    /* %typemap(freearg)  (OGRGeometryTypeCounter** ppRet, int* pnEntryCount) */
+    VSIFree(*arg2);
+  }
+  {
+    /* %typemap(freearg) ( void* callback_data=NULL)  */
+    
+    CPLFree(psProgressInfo);
+    
+  }
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  {
+    /* %typemap(freearg)  (OGRGeometryTypeCounter** ppRet, int* pnEntryCount) */
+    VSIFree(*arg2);
+  }
+  {
+    /* %typemap(freearg) ( void* callback_data=NULL)  */
+    
+    CPLFree(psProgressInfo);
+    
+  }
+  return NULL;
+}
+
+
 SWIGINTERN PyObject *Layer_swigregister(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *obj;
   if (!SWIG_Python_UnpackTuple(args, "swigregister", 1, 1, &obj)) return NULL;
   SWIG_TypeNewClientData(SWIGTYPE_p_OGRLayerShadow, SWIG_NewClientData(obj));
   return SWIG_Py_Void();
 }
 
@@ -24871,14 +25794,70 @@
   if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
   return resultobj;
 fail:
   return NULL;
 }
 
 
+SWIGINTERN PyObject *_wrap_Geometry_ConcaveHull(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  OGRGeometryShadow *arg1 = (OGRGeometryShadow *) 0 ;
+  double arg2 ;
+  bool arg3 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  double val2 ;
+  int ecode2 = 0 ;
+  bool val3 ;
+  int ecode3 = 0 ;
+  PyObject *swig_obj[3] ;
+  OGRGeometryShadow *result = 0 ;
+  
+  if (!SWIG_Python_UnpackTuple(args, "Geometry_ConcaveHull", 3, 3, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_OGRGeometryShadow, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "Geometry_ConcaveHull" "', argument " "1"" of type '" "OGRGeometryShadow *""'"); 
+  }
+  arg1 = reinterpret_cast< OGRGeometryShadow * >(argp1);
+  ecode2 = SWIG_AsVal_double(swig_obj[1], &val2);
+  if (!SWIG_IsOK(ecode2)) {
+    SWIG_exception_fail(SWIG_ArgError(ecode2), "in method '" "Geometry_ConcaveHull" "', argument " "2"" of type '" "double""'");
+  } 
+  arg2 = static_cast< double >(val2);
+  ecode3 = SWIG_AsVal_bool(swig_obj[2], &val3);
+  if (!SWIG_IsOK(ecode3)) {
+    SWIG_exception_fail(SWIG_ArgError(ecode3), "in method '" "Geometry_ConcaveHull" "', argument " "3"" of type '" "bool""'");
+  } 
+  arg3 = static_cast< bool >(val3);
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    {
+      SWIG_PYTHON_THREAD_BEGIN_ALLOW;
+      result = (OGRGeometryShadow *)OGRGeometryShadow_ConcaveHull(arg1,arg2,arg3);
+      SWIG_PYTHON_THREAD_END_ALLOW;
+    }
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  resultobj = SWIG_NewPointerObj(SWIG_as_voidptr(result), SWIGTYPE_p_OGRGeometryShadow, SWIG_POINTER_OWN |  0 );
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  return NULL;
+}
+
+
 SWIGINTERN PyObject *_wrap_Geometry_MakeValid(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
   OGRGeometryShadow *arg1 = (OGRGeometryShadow *) 0 ;
   char **arg2 = (char **) NULL ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   PyObject *swig_obj[2] ;
@@ -30281,195 +31260,197 @@
 		"int\n"
 		"OGR_DS_GetLayerCount(OGRDataSourceH hDS)\n"
 		"\n"
 		"Get the number of layers in this data source.\n"
 		"\n"
 		"Deprecated Use GDALDatasetGetLayerCount() in GDAL 2.0\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hDS:\n"
+		"    handle to the data source from which to get the number of\n"
+		"    layers.\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    layer count.\n"
 		"\n"
-		"hDS:  handle to the data source from which to get the number of\n"
-		"layers.\n"
-		"\n"
-		"layer count. \n"
 		""},
 	 { "DataSource_GetDriver", _wrap_DataSource_GetDriver, METH_O, "\n"
 		"DataSource_GetDriver(DataSource self) -> Driver\n"
 		"OGRSFDriverH\n"
 		"OGR_DS_GetDriver(OGRDataSourceH hDS)\n"
 		"\n"
 		"Returns the driver that the dataset was opened with.\n"
 		"\n"
 		"NOTE: Starting with GDAL 2.0, it is NOT safe to cast the returned\n"
-		"handle to OGRSFDriver*. If a C++ object is needed, the handle should\n"
-		"be cast to GDALDriver*.\n"
+		"handle to OGRSFDriver\\*. If a C++ object is needed, the handle should\n"
+		"be cast to GDALDriver\\*.\n"
 		"\n"
 		"Deprecated Use GDALGetDatasetDriver() in GDAL 2.0\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hDS:\n"
+		"    handle to the datasource\n"
 		"\n"
-		"hDS:  handle to the datasource\n"
+		"Returns\n"
+		"--------\n"
+		"OGRSFDriverH:\n"
+		"    NULL if driver info is not available, or pointer to a driver owned by\n"
+		"    the OGRSFDriverManager.\n"
 		"\n"
-		"NULL if driver info is not available, or pointer to a driver owned by\n"
-		"the OGRSFDriverManager. \n"
 		""},
 	 { "DataSource_GetName", _wrap_DataSource_GetName, METH_O, "\n"
 		"DataSource_GetName(DataSource self) -> char const *\n"
-		"const char*\n"
+		"const char\\*\n"
 		"OGR_DS_GetName(OGRDataSourceH hDS)\n"
 		"\n"
 		"Returns the name of the data source.\n"
 		"\n"
 		"This string should be sufficient to open the data source if passed to\n"
 		"the same OGRSFDriver that this data source was opened with, but it\n"
 		"need not be exactly the same string that was used to open the data\n"
 		"source. Normally this is a filename.\n"
 		"\n"
 		"Deprecated Use GDALGetDescription() in GDAL 2.0\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
-		"\n"
-		"hDS:  handle to the data source to get the name from.\n"
-		"\n"
-		"pointer to an internal name string which should not be modified or\n"
-		"freed by the caller. \n"
-		""},
-	 { "DataSource_DeleteLayer", _wrap_DataSource_DeleteLayer, METH_VARARGS, "\n"
-		"DataSource_DeleteLayer(DataSource self, int index) -> OGRErr\n"
-		"OGRErr\n"
-		"OGR_DS_DeleteLayer(OGRDataSourceH hDS, int iLayer)\n"
-		"\n"
-		"Delete the indicated layer from the datasource.\n"
-		"\n"
-		"If this method is supported the ODsCDeleteLayer capability will test\n"
-		"TRUE on the OGRDataSource.\n"
-		"\n"
-		"Deprecated Use GDALDatasetDeleteLayer() in GDAL 2.0\n"
-		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hDS:\n"
+		"    handle to the data source to get the name from.\n"
 		"\n"
-		"hDS:  handle to the datasource\n"
-		"\n"
-		"iLayer:  the index of the layer to delete.\n"
+		"Returns\n"
+		"--------\n"
+		"str:\n"
+		"    pointer to an internal name string which should not be modified or\n"
+		"    freed by the caller.\n"
 		"\n"
-		"OGRERR_NONE on success, or OGRERR_UNSUPPORTED_OPERATION if deleting\n"
-		"layers is not supported for this datasource. \n"
 		""},
+	 { "DataSource_DeleteLayer", _wrap_DataSource_DeleteLayer, METH_VARARGS, "DataSource_DeleteLayer(DataSource self, int index) -> OGRErr"},
 	 { "DataSource_SyncToDisk", _wrap_DataSource_SyncToDisk, METH_O, "\n"
 		"DataSource_SyncToDisk(DataSource self) -> OGRErr\n"
 		"OGRErr\n"
 		"OGR_DS_SyncToDisk(OGRDataSourceH hDS)\n"
 		"\n"
 		"Flush pending changes to disk.\n"
 		"\n"
 		"See GDALDataset::FlushCache() \n"
 		""},
 	 { "DataSource_FlushCache", _wrap_DataSource_FlushCache, METH_O, "DataSource_FlushCache(DataSource self)"},
 	 { "DataSource_CreateLayer", (PyCFunction)(void(*)(void))_wrap_DataSource_CreateLayer, METH_VARARGS|METH_KEYWORDS, "\n"
 		"DataSource_CreateLayer(DataSource self, char const * name, SpatialReference srs=None, OGRwkbGeometryType geom_type=wkbUnknown, char ** options=None) -> Layer\n"
 		"OGRLayerH\n"
-		"OGR_DS_CreateLayer(OGRDataSourceH hDS, const char *pszName,\n"
+		"OGR_DS_CreateLayer(OGRDataSourceH hDS, const char \\*pszName,\n"
 		"OGRSpatialReferenceH hSpatialRef, OGRwkbGeometryType eType, char\n"
-		"**papszOptions)\n"
+		"\\*\\*papszOptions)\n"
 		"\n"
 		"This function attempts to create a new layer on the data source with\n"
 		"the indicated name, coordinate system, geometry type.\n"
 		"\n"
 		"The papszOptions argument can be used to control driver specific\n"
 		"creation options. These options are normally documented in the format\n"
 		"specific documentation.\n"
 		"\n"
 		"Deprecated Use GDALDatasetCreateLayer() in GDAL 2.0\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hDS:\n"
+		"    The dataset handle.pszName:  the name for the new layer. This should ideally not match\n"
+		"    any existing layer on the datasource.\n"
+		"hSpatialRef:\n"
+		"    handle to the coordinate system to use for the new\n"
+		"    layer, or NULL if no coordinate system is available. The driver might\n"
+		"    only increase the reference counter of the object to take ownership,\n"
+		"    and not make a full copy, so do not use OSRDestroySpatialReference(),\n"
+		"    but OSRRelease() instead when you are done with the object.\n"
+		"eType:\n"
+		"    the geometry type for the layer. Use wkbUnknown if there are\n"
+		"    no constraints on the types geometry to be written.\n"
+		"papszOptions:\n"
+		"    a StringList of name=value options. Options are driver\n"
+		"    specific, and driver information can be found at the following\n"
+		"    url:http://www.gdal.org/ogr_formats.html\n"
+		"\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"OGRLayerH:\n"
+		"    NULL is returned on failure, or a new OGRLayer handle on success.\n"
 		"\n"
-		"hDS:  The dataset handle.\n"
-		"\n"
-		"pszName:  the name for the new layer. This should ideally not match\n"
-		"any existing layer on the datasource.\n"
-		"\n"
-		"hSpatialRef:  handle to the coordinate system to use for the new\n"
-		"layer, or NULL if no coordinate system is available. The driver might\n"
-		"only increase the reference counter of the object to take ownership,\n"
-		"and not make a full copy, so do not use OSRDestroySpatialReference(),\n"
-		"but OSRRelease() instead when you are done with the object.\n"
-		"\n"
-		"eType:  the geometry type for the layer. Use wkbUnknown if there are\n"
-		"no constraints on the types geometry to be written.\n"
-		"\n"
-		"papszOptions:  a StringList of name=value options. Options are driver\n"
-		"specific, and driver information can be found at the following\n"
-		"url:http://www.gdal.org/ogr_formats.html\n"
-		"\n"
-		"NULL is returned on failure, or a new OGRLayer handle on success.\n"
-		"Example: \n"
 		""},
 	 { "DataSource_CopyLayer", (PyCFunction)(void(*)(void))_wrap_DataSource_CopyLayer, METH_VARARGS|METH_KEYWORDS, "\n"
 		"DataSource_CopyLayer(DataSource self, Layer src_layer, char const * new_name, char ** options=None) -> Layer\n"
 		"OGRLayerH\n"
 		"OGR_DS_CopyLayer(OGRDataSourceH hDS, OGRLayerH hSrcLayer, const char\n"
-		"*pszNewName, char **papszOptions)\n"
+		"\\*pszNewName, char \\*\\*papszOptions)\n"
 		"\n"
 		"Duplicate an existing layer.\n"
 		"\n"
 		"This function creates a new layer, duplicate the field definitions of\n"
 		"the source layer and then duplicate each features of the source layer.\n"
 		"The papszOptions argument can be used to control driver specific\n"
 		"creation options. These options are normally documented in the format\n"
 		"specific documentation. The source layer may come from another\n"
 		"dataset.\n"
 		"\n"
 		"Deprecated Use GDALDatasetCopyLayer() in GDAL 2.0\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hDS:\n"
+		"    handle to the data source where to create the new layer\n"
+		"hSrcLayer:\n"
+		"    handle to the source layer.\n"
+		"pszNewName:\n"
+		"    the name of the layer to create.\n"
+		"papszOptions:\n"
+		"    a StringList of name=value options. Options are driver\n"
+		"    specific.\n"
+		"\n"
+		"Returns\n"
+		"-------\n"
+		"OGRLayerH:\n"
+		"    a handle to the layer, or NULL if an error occurs.\n"
 		"\n"
-		"hDS:  handle to the data source where to create the new layer\n"
-		"\n"
-		"hSrcLayer:  handle to the source layer.\n"
-		"\n"
-		"pszNewName:  the name of the layer to create.\n"
-		"\n"
-		"papszOptions:  a StringList of name=value options. Options are driver\n"
-		"specific.\n"
-		"\n"
-		"a handle to the layer, or NULL if an error occurs. \n"
 		""},
 	 { "DataSource_GetLayerByIndex", _wrap_DataSource_GetLayerByIndex, METH_VARARGS, "DataSource_GetLayerByIndex(DataSource self, int index=0) -> Layer"},
 	 { "DataSource_GetLayerByName", _wrap_DataSource_GetLayerByName, METH_VARARGS, "\n"
 		"DataSource_GetLayerByName(DataSource self, char const * layer_name) -> Layer\n"
 		"OGRLayerH\n"
-		"OGR_DS_GetLayerByName(OGRDataSourceH hDS, const char *pszLayerName)\n"
+		"OGR_DS_GetLayerByName(OGRDataSourceH hDS, const char \\*pszLayerName)\n"
 		"\n"
 		"Fetch a layer by name.\n"
 		"\n"
 		"The returned layer remains owned by the OGRDataSource and should not\n"
 		"be deleted by the application.\n"
 		"\n"
 		"Deprecated Use GDALDatasetGetLayerByName() in GDAL 2.0\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hDS:\n"
+		"    handle to the data source from which to get the layer.\n"
+		"pszLayerName:\n"
+		"    Layer the layer name of the layer to fetch.\n"
 		"\n"
-		"hDS:  handle to the data source from which to get the layer.\n"
 		"\n"
-		"pszLayerName:  Layer the layer name of the layer to fetch.\n"
+		"Returns\n"
+		"--------\n"
+		"OGRLayerH:\n"
+		"    a handle to the layer, or NULL if the layer is not found or an error\n"
+		"    occurs.\n"
 		"\n"
-		"a handle to the layer, or NULL if the layer is not found or an error\n"
-		"occurs. \n"
 		""},
 	 { "DataSource_TestCapability", _wrap_DataSource_TestCapability, METH_VARARGS, "\n"
 		"DataSource_TestCapability(DataSource self, char const * cap) -> bool\n"
 		"int\n"
-		"OGR_DS_TestCapability(OGRDataSourceH hDS, const char *pszCapability)\n"
+		"OGR_DS_TestCapability(OGRDataSourceH hDS, const char \\*pszCapability)\n"
 		"\n"
 		"Test if capability is available.\n"
 		"\n"
 		"One of the following data source capability names can be passed into\n"
 		"this function, and a TRUE or FALSE value will be returned indicating\n"
 		"whether or not the capability is available for this object.\n"
 		"\n"
@@ -30485,28 +31466,32 @@
 		"declared in layers of that dataset.\n"
 		"\n"
 		"The #define macro forms of the capability names should be used in\n"
 		"preference to the strings themselves to avoid misspelling.\n"
 		"\n"
 		"Deprecated Use GDALDatasetTestCapability() in GDAL 2.0\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hDS:\n"
+		"    handle to the data source against which to test the capability.\n"
+		"pszCapability:\n"
+		"    the capability to test.\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    TRUE if capability available otherwise FALSE.\n"
 		"\n"
-		"hDS:  handle to the data source against which to test the capability.\n"
-		"\n"
-		"pszCapability:  the capability to test.\n"
-		"\n"
-		"TRUE if capability available otherwise FALSE. \n"
 		""},
 	 { "DataSource_ExecuteSQL", (PyCFunction)(void(*)(void))_wrap_DataSource_ExecuteSQL, METH_VARARGS|METH_KEYWORDS, "\n"
 		"DataSource_ExecuteSQL(DataSource self, char const * statement, Geometry spatialFilter=None, char const * dialect=\"\") -> Layer\n"
 		"OGRLayerH\n"
-		"OGR_DS_ExecuteSQL(OGRDataSourceH hDS, const char *pszStatement,\n"
-		"OGRGeometryH hSpatialFilter, const char *pszDialect)\n"
+		"OGR_DS_ExecuteSQL(OGRDataSourceH hDS, const char \\*pszStatement,\n"
+		"OGRGeometryH hSpatialFilter, const char \\*pszDialect)\n"
 		"\n"
 		"Execute an SQL statement against the data store.\n"
 		"\n"
 		"The result of an SQL query is either NULL for statements that are in\n"
 		"error, or that have no results set, or an OGRLayer handle representing\n"
 		"a results set from the query. Note that this OGRLayer is in addition\n"
 		"to the layers in the data store and must be destroyed with\n"
@@ -30517,31 +31502,35 @@
 		"review theOGR SQL document. Some drivers (i.e. Oracle and PostGIS)\n"
 		"pass the SQL directly through to the underlying RDBMS.\n"
 		"\n"
 		"TheSQLITE dialect can also be used.\n"
 		"\n"
 		"Deprecated Use GDALDatasetExecuteSQL() in GDAL 2.0\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hDS:\n"
+		"    handle to the data source on which the SQL query is executed.\n"
+		"pszStatement:\n"
+		"    the SQL statement to execute.\n"
+		"hSpatialFilter:\n"
+		"    handle to a geometry which represents a spatial\n"
+		"    filter. Can be NULL.\n"
+		"pszDialect:\n"
+		"    allows control of the statement dialect. If set to NULL,\n"
+		"    the OGR SQL engine will be used, except for RDBMS drivers that will\n"
+		"    use their dedicated SQL engine, unless OGRSQL is explicitly passed as\n"
+		"    the dialect. The SQLITE dialect can also be used.\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"OGRLayerH:\n"
+		"    a handle to a OGRLayer containing the results of the query. Deallocate\n"
+		"    with OGR_DS_ReleaseResultSet().\n"
 		"\n"
-		"hDS:  handle to the data source on which the SQL query is executed.\n"
-		"\n"
-		"pszStatement:  the SQL statement to execute.\n"
-		"\n"
-		"hSpatialFilter:  handle to a geometry which represents a spatial\n"
-		"filter. Can be NULL.\n"
-		"\n"
-		"pszDialect:  allows control of the statement dialect. If set to NULL,\n"
-		"the OGR SQL engine will be used, except for RDBMS drivers that will\n"
-		"use their dedicated SQL engine, unless OGRSQL is explicitly passed as\n"
-		"the dialect. The SQLITE dialect can also be used.\n"
-		"\n"
-		"a handle to a OGRLayer containing the results of the query. Deallocate\n"
-		"with OGR_DS_ReleaseResultSet(). \n"
 		""},
 	 { "DataSource_AbortSQL", _wrap_DataSource_AbortSQL, METH_O, "DataSource_AbortSQL(DataSource self) -> OGRErr"},
 	 { "DataSource_ReleaseResultSet", _wrap_DataSource_ReleaseResultSet, METH_VARARGS, "\n"
 		"DataSource_ReleaseResultSet(DataSource self, Layer layer)\n"
 		"void\n"
 		"OGR_DS_ReleaseResultSet(OGRDataSourceH hDS, OGRLayerH hLayer)\n"
 		"\n"
@@ -30550,20 +31539,20 @@
 		"This function should only be used to deallocate OGRLayers resulting\n"
 		"from an OGR_DS_ExecuteSQL() call on the same OGRDataSource. Failure to\n"
 		"deallocate a results set before destroying the OGRDataSource may cause\n"
 		"errors.\n"
 		"\n"
 		"Deprecated Use GDALDatasetReleaseResultSet() in GDAL 2.0\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
-		"\n"
-		"hDS:  a handle to the data source on which was executed an SQL query.\n"
-		"\n"
-		"hLayer:  handle to the result of a previous OGR_DS_ExecuteSQL() call.\n"
+		"hDS:\n"
+		"    a handle to the data source on which was executed an SQL query.\n"
+		"hLayer:\n"
+		"    handle to the result of a previous OGR_DS_ExecuteSQL() call.\n"
 		"\n"
 		""},
 	 { "DataSource_GetStyleTable", _wrap_DataSource_GetStyleTable, METH_O, "\n"
 		"DataSource_GetStyleTable(DataSource self) -> StyleTable\n"
 		"OGRStyleTableH\n"
 		"OGR_DS_GetStyleTable(OGRDataSourceH hDS)\n"
 		"\n"
@@ -30576,1587 +31565,916 @@
 		"\n"
 		"Set style table. \n"
 		""},
 	 { "DataSource_StartTransaction", (PyCFunction)(void(*)(void))_wrap_DataSource_StartTransaction, METH_VARARGS|METH_KEYWORDS, "DataSource_StartTransaction(DataSource self, int force=FALSE) -> OGRErr"},
 	 { "DataSource_CommitTransaction", _wrap_DataSource_CommitTransaction, METH_O, "DataSource_CommitTransaction(DataSource self) -> OGRErr"},
 	 { "DataSource_RollbackTransaction", _wrap_DataSource_RollbackTransaction, METH_O, "DataSource_RollbackTransaction(DataSource self) -> OGRErr"},
 	 { "DataSource_swigregister", DataSource_swigregister, METH_O, NULL},
+	 { "delete_ArrowArray", _wrap_delete_ArrowArray, METH_O, "delete_ArrowArray(ArrowArray self)"},
+	 { "ArrowArray__getPtr", _wrap_ArrowArray__getPtr, METH_O, "ArrowArray__getPtr(ArrowArray self) -> VoidPtrAsLong"},
+	 { "ArrowArray_GetChildrenCount", _wrap_ArrowArray_GetChildrenCount, METH_O, "ArrowArray_GetChildrenCount(ArrowArray self) -> GIntBig"},
+	 { "ArrowArray_GetLength", _wrap_ArrowArray_GetLength, METH_O, "ArrowArray_GetLength(ArrowArray self) -> GIntBig"},
+	 { "ArrowArray_swigregister", ArrowArray_swigregister, METH_O, NULL},
+	 { "delete_ArrowSchema", _wrap_delete_ArrowSchema, METH_O, "delete_ArrowSchema(ArrowSchema self)"},
+	 { "ArrowSchema__getPtr", _wrap_ArrowSchema__getPtr, METH_O, "ArrowSchema__getPtr(ArrowSchema self) -> VoidPtrAsLong"},
+	 { "ArrowSchema_GetChildrenCount", _wrap_ArrowSchema_GetChildrenCount, METH_O, "ArrowSchema_GetChildrenCount(ArrowSchema self) -> GIntBig"},
+	 { "ArrowSchema_swigregister", ArrowSchema_swigregister, METH_O, NULL},
+	 { "delete_ArrowArrayStream", _wrap_delete_ArrowArrayStream, METH_O, "delete_ArrowArrayStream(ArrowArrayStream self)"},
+	 { "ArrowArrayStream_GetSchema", _wrap_ArrowArrayStream_GetSchema, METH_O, "ArrowArrayStream_GetSchema(ArrowArrayStream self) -> ArrowSchema"},
+	 { "ArrowArrayStream_GetNextRecordBatch", _wrap_ArrowArrayStream_GetNextRecordBatch, METH_VARARGS, "ArrowArrayStream_GetNextRecordBatch(ArrowArrayStream self, char ** options=None) -> ArrowArray"},
+	 { "ArrowArrayStream_swigregister", ArrowArrayStream_swigregister, METH_O, NULL},
 	 { "Layer_Rename", _wrap_Layer_Rename, METH_VARARGS, "Layer_Rename(Layer self, char const * new_name) -> OGRErr"},
 	 { "Layer_GetRefCount", _wrap_Layer_GetRefCount, METH_O, "\n"
 		"Layer_GetRefCount(Layer self) -> int\n"
-		"int OGR_L_GetRefCount(OGRLayerH\n"
-		"hLayer) \n"
+		"\n"
+		"For more details: :cpp:func:`OGR_L_GetRefCount`\n"
+		"\n"
 		""},
 	 { "Layer_SetSpatialFilter", _wrap_Layer_SetSpatialFilter, METH_VARARGS, "\n"
 		"Layer_SetSpatialFilter(Layer self, Geometry filter)\n"
 		"Layer_SetSpatialFilter(Layer self, int iGeomField, Geometry filter)\n"
-		"void\n"
-		"OGR_L_SetSpatialFilter(OGRLayerH hLayer, OGRGeometryH hGeom)\n"
 		"\n"
 		"Set a new spatial filter.\n"
 		"\n"
-		"This function set the geometry to be used as a spatial filter when\n"
-		"fetching features via the OGR_L_GetNextFeature() function. Only\n"
-		"features that geometrically intersect the filter geometry will be\n"
-		"returned.\n"
-		"\n"
-		"Currently this test is may be inaccurately implemented, but it is\n"
-		"guaranteed that all features whose envelope (as returned by\n"
-		"OGR_G_GetEnvelope()) overlaps the envelope of the spatial filter will\n"
-		"be returned. This can result in more shapes being returned that should\n"
-		"strictly be the case.\n"
-		"\n"
-		"Starting with GDAL 2.3, features with null or empty geometries will\n"
-		"never be considered as matching a spatial filter.\n"
-		"\n"
-		"This function makes an internal copy of the passed geometry. The\n"
-		"passed geometry remains the responsibility of the caller, and may be\n"
-		"safely destroyed.\n"
-		"\n"
-		"For the time being the passed filter geometry should be in the same\n"
-		"SRS as the layer (as returned by OGR_L_GetSpatialRef()). In the future\n"
-		"this may be generalized.\n"
+		"For more details:\n"
 		"\n"
-		"This function is the same as the C++ method\n"
-		"OGRLayer::SetSpatialFilter.\n"
+		"- :cpp:func:`OGR_L_SetSpatialFilter`\n"
+		"- :cpp:func:`OGR_L_SetSpatialFilterEx`\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"iGeomField: int, optional\n"
+		"    index of the geometry field on which the spatial filter operates.\n"
+		"filter: Geometry\n"
+		"    The geometry to use as a filtering region. None may\n"
+		"    be passed indicating that the current spatial filter should be\n"
+		"    cleared, but no new one instituted.\n"
 		"\n"
-		"hLayer:  handle to the layer on which to set the spatial filter.\n"
-		"\n"
-		"hGeom:  handle to the geometry to use as a filtering region. NULL may\n"
-		"be passed indicating that the current spatial filter should be\n"
-		"cleared, but no new one instituted. \n"
 		""},
 	 { "Layer_SetSpatialFilterRect", _wrap_Layer_SetSpatialFilterRect, METH_VARARGS, "\n"
 		"Layer_SetSpatialFilterRect(Layer self, double minx, double miny, double maxx, double maxy)\n"
 		"Layer_SetSpatialFilterRect(Layer self, int iGeomField, double minx, double miny, double maxx, double maxy)\n"
-		"void\n"
-		"OGR_L_SetSpatialFilterRect(OGRLayerH hLayer, double dfMinX, double\n"
-		"dfMinY, double dfMaxX, double dfMaxY)\n"
 		"\n"
 		"Set a new rectangular spatial filter.\n"
 		"\n"
-		"This method set rectangle to be used as a spatial filter when fetching\n"
-		"features via the OGR_L_GetNextFeature() method. Only features that\n"
-		"geometrically intersect the given rectangle will be returned.\n"
-		"\n"
-		"The x/y values should be in the same coordinate system as the layer as\n"
-		"a whole (as returned by OGRLayer::GetSpatialRef()). Internally this\n"
-		"method is normally implemented as creating a 5 vertex closed\n"
-		"rectangular polygon and passing it to OGRLayer::SetSpatialFilter(). It\n"
-		"exists as a convenience.\n"
+		"For more details:\n"
 		"\n"
-		"The only way to clear a spatial filter set with this method is to call\n"
-		"OGRLayer::SetSpatialFilter(NULL).\n"
+		"- :cpp:func:`OGR_L_SetSpatialFilterRect`\n"
+		"- :cpp:func:`OGR_L_SetSpatialFilterRectEx`\n"
 		"\n"
-		"This method is the same as the C++ method\n"
-		"OGRLayer::SetSpatialFilterRect().\n"
-		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"iGeomField: int, optional\n"
+		"    index of the geometry field on which the spatial filter operates.\n"
+		"minx: float\n"
+		"    the minimum X coordinate for the rectangular region.\n"
+		"miny: float\n"
+		"    the minimum Y coordinate for the rectangular region.\n"
+		"maxx: float\n"
+		"    the maximum X coordinate for the rectangular region.\n"
+		"maxy: float\n"
+		"    the maximum Y coordinate for the rectangular region.\n"
 		"\n"
-		"hLayer:  handle to the layer on which to set the spatial filter.\n"
-		"\n"
-		"dfMinX:  the minimum X coordinate for the rectangular region.\n"
-		"\n"
-		"dfMinY:  the minimum Y coordinate for the rectangular region.\n"
-		"\n"
-		"dfMaxX:  the maximum X coordinate for the rectangular region.\n"
-		"\n"
-		"dfMaxY:  the maximum Y coordinate for the rectangular region. \n"
 		""},
 	 { "Layer_GetSpatialFilter", _wrap_Layer_GetSpatialFilter, METH_O, "\n"
 		"Layer_GetSpatialFilter(Layer self) -> Geometry\n"
-		"OGRGeometryH\n"
-		"OGR_L_GetSpatialFilter(OGRLayerH hLayer)\n"
 		"\n"
 		"This function returns the current spatial filter for this layer.\n"
 		"\n"
-		"The returned pointer is to an internally owned object, and should not\n"
-		"be altered or deleted by the caller.\n"
+		"For more details: :cpp:func:`OGR_L_GetSpatialFilter`\n"
 		"\n"
-		"This function is the same as the C++ method\n"
-		"OGRLayer::GetSpatialFilter().\n"
-		"\n"
-		"Parameters:\n"
-		"-----------\n"
+		"Returns\n"
+		"--------\n"
+		"Geometry:\n"
+		"    The spatial filter geometry.\n"
 		"\n"
-		"hLayer:  handle to the layer to get the spatial filter from.\n"
-		"\n"
-		"a handle to the spatial filter geometry. \n"
 		""},
 	 { "Layer_SetAttributeFilter", _wrap_Layer_SetAttributeFilter, METH_VARARGS, "\n"
 		"Layer_SetAttributeFilter(Layer self, char * filter_string) -> OGRErr\n"
-		"OGRErr\n"
-		"OGR_L_SetAttributeFilter(OGRLayerH hLayer, const char *pszQuery)\n"
 		"\n"
 		"Set a new attribute query.\n"
 		"\n"
-		"This function sets the attribute query string to be used when fetching\n"
-		"features via the OGR_L_GetNextFeature() function. Only features for\n"
-		"which the query evaluates as true will be returned.\n"
-		"\n"
-		"The query string should be in the format of an SQL WHERE clause. For\n"
-		"instance \"population > 1000000 and population < 5000000\" where\n"
-		"population is an attribute in the layer. The query format is a\n"
-		"restricted form of SQL WHERE clause as defined\n"
-		"\"eq_format=restricted_where\" about half way through this document:\n"
-		"\n"
-		"http://ogdi.sourceforge.net/prop/6.2.CapabilitiesMetadata.html\n"
+		"For more details: :cpp:func:`OGR_L_SetAttributeFilter`\n"
 		"\n"
-		"Note that installing a query string will generally result in resetting\n"
-		"the current reading position (ala OGR_L_ResetReading()).\n"
-		"\n"
-		"This function is the same as the C++ method\n"
-		"OGRLayer::SetAttributeFilter().\n"
-		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"filter_string: str\n"
+		"    query in restricted SQL WHERE format, or None to clear the\n"
+		"    current query.\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    :py:const:`osgeo.ogr.OGRERR_NONE` if successfully installed,\n"
+		"    or an error code if the query expression is in error,\n"
+		"    or some other failure occurs.\n"
 		"\n"
-		"hLayer:  handle to the layer on which attribute query will be\n"
-		"executed.\n"
-		"\n"
-		"pszQuery:  query in restricted SQL WHERE format, or NULL to clear the\n"
-		"current query.\n"
-		"\n"
-		"OGRERR_NONE if successfully installed, or an error code if the query\n"
-		"expression is in error, or some other failure occurs. \n"
 		""},
 	 { "Layer_ResetReading", _wrap_Layer_ResetReading, METH_O, "\n"
 		"Layer_ResetReading(Layer self)\n"
-		"void\n"
-		"OGR_L_ResetReading(OGRLayerH hLayer)\n"
 		"\n"
 		"Reset feature reading to start on the first feature.\n"
 		"\n"
-		"This affects GetNextFeature().\n"
+		"For more details: :cpp:func:`OGR_L_ResetReading`\n"
 		"\n"
-		"This function is the same as the C++ method OGRLayer::ResetReading().\n"
-		"\n"
-		"Parameters:\n"
-		"-----------\n"
-		"\n"
-		"hLayer:  handle to the layer on which features are read. \n"
 		""},
 	 { "Layer_GetName", _wrap_Layer_GetName, METH_O, "\n"
 		"Layer_GetName(Layer self) -> char const *\n"
-		"const char* OGR_L_GetName(OGRLayerH\n"
-		"hLayer)\n"
 		"\n"
 		"Return the layer name.\n"
 		"\n"
-		"This returns the same content as\n"
-		"OGR_FD_GetName(OGR_L_GetLayerDefn(hLayer)), but for a few drivers,\n"
-		"calling OGR_L_GetName() directly can avoid lengthy layer definition\n"
-		"initialization.\n"
-		"\n"
-		"This function is the same as the C++ method OGRLayer::GetName().\n"
-		"\n"
-		"Parameters:\n"
-		"-----------\n"
-		"\n"
-		"hLayer:  handle to the layer.\n"
+		"For more details: :cpp:func:`OGR_L_GetName`\n"
 		"\n"
-		"the layer name (must not been freed)\n"
+		"Returns\n"
+		"--------\n"
+		"str:\n"
+		"    The layer name\n"
 		"\n"
-		"OGR 1.8.0 \n"
 		""},
 	 { "Layer_GetGeomType", _wrap_Layer_GetGeomType, METH_O, "\n"
 		"Layer_GetGeomType(Layer self) -> OGRwkbGeometryType\n"
-		"OGRwkbGeometryType\n"
-		"OGR_L_GetGeomType(OGRLayerH hLayer)\n"
 		"\n"
 		"Return the layer geometry type.\n"
 		"\n"
-		"This returns the same result as\n"
-		"OGR_FD_GetGeomType(OGR_L_GetLayerDefn(hLayer)), but for a few drivers,\n"
-		"calling OGR_L_GetGeomType() directly can avoid lengthy layer\n"
-		"definition initialization.\n"
-		"\n"
-		"For layers with multiple geometry fields, this method only returns the\n"
-		"geometry type of the first geometry column. For other columns, use\n"
-		"OGR_GFld_GetType(OGR_FD_GetGeomFieldDefn(OGR_L_GetLayerDefn(hLayer),\n"
-		"i)). For layers without any geometry field, this method returns\n"
-		"wkbNone.\n"
-		"\n"
-		"This function is the same as the C++ method OGRLayer::GetGeomType().\n"
-		"\n"
-		"Parameters:\n"
-		"-----------\n"
-		"\n"
-		"hLayer:  handle to the layer.\n"
+		"For more details: :cpp:func:`OGR_L_GetGeomType`\n"
 		"\n"
-		"the geometry type\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    The geometry type code. The types can be found with\n"
+		"    'osgeo.ogr.wkb' prefix. For example :py:const:`osgeo.ogr.wkbPolygon`.\n"
 		"\n"
-		"OGR 1.8.0 \n"
 		""},
 	 { "Layer_GetGeometryColumn", _wrap_Layer_GetGeometryColumn, METH_O, "\n"
 		"Layer_GetGeometryColumn(Layer self) -> char const *\n"
-		"const char*\n"
-		"OGR_L_GetGeometryColumn(OGRLayerH hLayer)\n"
 		"\n"
 		"This method returns the name of the underlying database column being\n"
-		"used as the geometry column, or \"\" if not supported.\n"
+		"used as the geometry column, or '' if not supported.\n"
 		"\n"
-		"For layers with multiple geometry fields, this method only returns the\n"
-		"geometry type of the first geometry column. For other columns, use OGR\n"
-		"_GFld_GetNameRef(OGR_FD_GetGeomFieldDefn(OGR_L_GetLayerDefn(hLayer),\n"
-		"i)).\n"
+		"For more details: :cpp:func:`OGR_L_GetGeometryColumn`\n"
 		"\n"
-		"This method is the same as the C++ method\n"
-		"OGRLayer::GetGeometryColumn()\n"
-		"\n"
-		"Parameters:\n"
-		"-----------\n"
+		"Returns\n"
+		"--------\n"
+		"str:\n"
+		"    geometry column name.\n"
 		"\n"
-		"hLayer:  handle to the layer\n"
-		"\n"
-		"geometry column name. \n"
 		""},
 	 { "Layer_GetFIDColumn", _wrap_Layer_GetFIDColumn, METH_O, "\n"
 		"Layer_GetFIDColumn(Layer self) -> char const *\n"
-		"const char*\n"
-		"OGR_L_GetFIDColumn(OGRLayerH hLayer)\n"
 		"\n"
 		"This method returns the name of the underlying database column being\n"
-		"used as the FID column, or \"\" if not supported.\n"
-		"\n"
-		"This method is the same as the C++ method OGRLayer::GetFIDColumn()\n"
+		"used as the FID column, or '' if not supported.\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
+		"For more details: :cpp:func:`OGR_L_GetFIDColumn`\n"
 		"\n"
-		"hLayer:  handle to the layer\n"
+		"Returns\n"
+		"--------\n"
+		"str:\n"
+		"    fid column name.\n"
 		"\n"
-		"fid column name. \n"
 		""},
 	 { "Layer_GetFeature", _wrap_Layer_GetFeature, METH_VARARGS, "\n"
 		"Layer_GetFeature(Layer self, GIntBig fid) -> Feature\n"
-		"OGRFeatureH\n"
-		"OGR_L_GetFeature(OGRLayerH hLayer, GIntBig nFeatureId)\n"
 		"\n"
 		"Fetch a feature by its identifier.\n"
 		"\n"
-		"This function will attempt to read the identified feature. The nFID\n"
-		"value cannot be OGRNullFID. Success or failure of this operation is\n"
-		"unaffected by the spatial or attribute filters (and specialized\n"
-		"implementations in drivers should make sure that they do not take into\n"
-		"account spatial or attribute filters).\n"
+		"For more details: :cpp:func:`OGR_L_GetFeature`\n"
 		"\n"
-		"If this function returns a non-NULL feature, it is guaranteed that its\n"
-		"feature id ( OGR_F_GetFID()) will be the same as nFID.\n"
+		"Use :py:func:`TestCapability` with (:py:const:`osgeo.ogr.OLCRandomRead`)\n"
+		"to establish if this layer supports efficient random access reading via\n"
+		":py:func:`GetFeature`; However, the call should always work if the feature exists.\n"
 		"\n"
-		"Use OGR_L_TestCapability(OLCRandomRead) to establish if this layer\n"
-		"supports efficient random access reading via OGR_L_GetFeature();\n"
-		"however, the call should always work if the feature exists as a\n"
-		"fallback implementation just scans all the features in the layer\n"
-		"looking for the desired feature.\n"
+		"Sequential reads (with :py:func:`GetNextFeature`) are generally\n"
+		"considered interrupted by a :py:func:`GetFeature` call.\n"
 		"\n"
-		"Sequential reads (with OGR_L_GetNextFeature()) are generally\n"
-		"considered interrupted by a OGR_L_GetFeature() call.\n"
-		"\n"
-		"The returned feature should be free with OGR_F_Destroy().\n"
-		"\n"
-		"This function is the same as the C++ method OGRLayer::GetFeature( ).\n"
-		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"fid: int\n"
+		"    The feature id of the feature to read.\n"
 		"\n"
-		"hLayer:  handle to the layer that owned the feature.\n"
+		"Returns\n"
+		"--------\n"
+		"Feature:\n"
+		"    A new feature now owned by the caller, or None on failure.\n"
+		"    The returned feature should be deleted with :py:func:`Destroy`.\n"
 		"\n"
-		"nFeatureId:  the feature id of the feature to read.\n"
-		"\n"
-		"a handle to a feature now owned by the caller, or NULL on failure. \n"
 		""},
 	 { "Layer_GetNextFeature", _wrap_Layer_GetNextFeature, METH_O, "\n"
 		"Layer_GetNextFeature(Layer self) -> Feature\n"
-		"OGRFeatureH\n"
-		"OGR_L_GetNextFeature(OGRLayerH hLayer)\n"
 		"\n"
 		"Fetch the next available feature from this layer.\n"
 		"\n"
-		"The returned feature becomes the responsibility of the caller to\n"
-		"delete with OGR_F_Destroy(). It is critical that all features\n"
-		"associated with an OGRLayer (more specifically an OGRFeatureDefn) be\n"
-		"deleted before that layer/datasource is deleted.\n"
-		"\n"
-		"Only features matching the current spatial filter (set with\n"
-		"SetSpatialFilter()) will be returned.\n"
-		"\n"
-		"This function implements sequential access to the features of a layer.\n"
-		"The OGR_L_ResetReading() function can be used to start at the\n"
-		"beginning again.\n"
-		"\n"
-		"Features returned by OGR_GetNextFeature() may or may not be affected\n"
-		"by concurrent modifications depending on drivers. A guaranteed way of\n"
-		"seeing modifications in effect is to call OGR_L_ResetReading() on\n"
-		"layers where OGR_GetNextFeature() has been called, before reading\n"
-		"again. Structural changes in layers (field addition, deletion, ...)\n"
-		"when a read is in progress may or may not be possible depending on\n"
-		"drivers. If a transaction is committed/aborted, the current sequential\n"
-		"reading may or may not be valid after that operation and a call to\n"
-		"OGR_L_ResetReading() might be needed.\n"
-		"\n"
-		"This function is the same as the C++ method\n"
-		"OGRLayer::GetNextFeature().\n"
-		"\n"
-		"Parameters:\n"
-		"-----------\n"
+		"For more details: :cpp:func:`OGR_L_GetNextFeature`\n"
 		"\n"
-		"hLayer:  handle to the layer from which feature are read.\n"
+		"Returns\n"
+		"--------\n"
+		"Feature:\n"
+		"    A feature or None if no more features are available.\n"
 		"\n"
-		"a handle to a feature, or NULL if no more features are available. \n"
 		""},
 	 { "Layer_SetNextByIndex", _wrap_Layer_SetNextByIndex, METH_VARARGS, "\n"
 		"Layer_SetNextByIndex(Layer self, GIntBig new_index) -> OGRErr\n"
-		"OGRErr\n"
-		"OGR_L_SetNextByIndex(OGRLayerH hLayer, GIntBig nIndex)\n"
 		"\n"
 		"Move read cursor to the nIndex'th feature in the current resultset.\n"
 		"\n"
-		"This method allows positioning of a layer such that the\n"
-		"GetNextFeature() call will read the requested feature, where nIndex is\n"
-		"an absolute index into the current result set. So, setting it to 3\n"
-		"would mean the next feature read with GetNextFeature() would have been\n"
-		"the 4th feature to have been read if sequential reading took place\n"
-		"from the beginning of the layer, including accounting for spatial and\n"
-		"attribute filters.\n"
-		"\n"
-		"Only in rare circumstances is SetNextByIndex() efficiently\n"
-		"implemented. In all other cases the default implementation which calls\n"
-		"ResetReading() and then calls GetNextFeature() nIndex times is used.\n"
-		"To determine if fast seeking is available on the current layer use the\n"
-		"TestCapability() method with a value of OLCFastSetNextByIndex.\n"
+		"For more details: :cpp:func:`OGR_L_SetNextByIndex`\n"
 		"\n"
-		"This method is the same as the C++ method OGRLayer::SetNextByIndex()\n"
-		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"new_index: int\n"
+		"    The index indicating how many steps into the result set to seek.\n"
 		"\n"
-		"hLayer:  handle to the layer\n"
-		"\n"
-		"nIndex:  the index indicating how many steps into the result set to\n"
-		"seek.\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    :py:const:`osgeo.ogr.OGRERR_NONE` on success or an error code.\n"
 		"\n"
-		"OGRERR_NONE on success or an error code. \n"
 		""},
 	 { "Layer_SetFeature", _wrap_Layer_SetFeature, METH_VARARGS, "\n"
 		"Layer_SetFeature(Layer self, Feature feature) -> OGRErr\n"
-		"OGRErr OGR_L_SetFeature(OGRLayerH\n"
-		"hLayer, OGRFeatureH hFeat)\n"
 		"\n"
 		"Rewrite an existing feature.\n"
 		"\n"
-		"This function will write a feature to the layer, based on the feature\n"
-		"id within the OGRFeature.\n"
-		"\n"
-		"Use OGR_L_TestCapability(OLCRandomWrite) to establish if this layer\n"
-		"supports random access writing via OGR_L_SetFeature().\n"
+		"For more details: :cpp:func:`OGR_L_SetFeature`\n"
 		"\n"
-		"This function is the same as the C++ method OGRLayer::SetFeature().\n"
+		"To set a feature, but create it if it doesn't exist see :py:meth:`.Layer.UpsertFeature`.\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"feature: Feature\n"
+		"    The feature to write.\n"
 		"\n"
-		"hLayer:  handle to the layer to write the feature.\n"
-		"\n"
-		"hFeat:  the feature to write.\n"
-		"\n"
-		"OGRERR_NONE if the operation works, otherwise an appropriate error\n"
-		"code (e.g OGRERR_NON_EXISTING_FEATURE if the feature does not exist).\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    :py:const:`osgeo.ogr.OGRERR_NONE` if the operation works,\n"
+		"    otherwise an appropriate error code\n"
+		"    (e.g :py:const:`osgeo.ogr.OGRERR_NON_EXISTING_FEATURE` if the\n"
+		"    feature does not exist).\n"
 		"\n"
 		""},
 	 { "Layer_CreateFeature", _wrap_Layer_CreateFeature, METH_VARARGS, "\n"
 		"Layer_CreateFeature(Layer self, Feature feature) -> OGRErr\n"
-		"OGRErr\n"
-		"OGR_L_CreateFeature(OGRLayerH hLayer, OGRFeatureH hFeat)\n"
 		"\n"
 		"Create and write a new feature within a layer.\n"
 		"\n"
-		"The passed feature is written to the layer as a new feature, rather\n"
-		"than overwriting an existing one. If the feature has a feature id\n"
-		"other than OGRNullFID, then the native implementation may use that as\n"
-		"the feature id of the new feature, but not necessarily. Upon\n"
-		"successful return the passed feature will have been updated with the\n"
-		"new feature id.\n"
+		"For more details: :cpp:func:`OGR_L_CreateFeature`\n"
 		"\n"
-		"This function is the same as the C++ method OGRLayer::CreateFeature().\n"
+		"To create a feature, but set it if it exists see :py:meth:`.Layer.UpsertFeature`.\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"feature: Feature\n"
+		"    The feature to write to disk.\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    :py:const:`osgeo.ogr.OGRERR_NONE` on success.\n"
+		"\n"
+		""},
+	 { "Layer_UpsertFeature", _wrap_Layer_UpsertFeature, METH_VARARGS, "\n"
+		"Layer_UpsertFeature(Layer self, Feature feature) -> OGRErr\n"
 		"\n"
-		"hLayer:  handle to the layer to write the feature to.\n"
+		"Rewrite an existing feature or create a new feature within a layer.\n"
 		"\n"
-		"hFeat:  the handle of the feature to write to disk.\n"
+		"For more details: :cpp:func:`OGR_L_UpsertFeature`\n"
+		"\n"
+		"Parameters\n"
+		"-----------\n"
+		"feature: Feature\n"
+		"    The feature to write to disk.\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    :py:const:`osgeo.ogr.OGRERR_NONE` on success.\n"
 		"\n"
-		"OGRERR_NONE on success. \n"
 		""},
 	 { "Layer_DeleteFeature", _wrap_Layer_DeleteFeature, METH_VARARGS, "\n"
 		"Layer_DeleteFeature(Layer self, GIntBig fid) -> OGRErr\n"
-		"OGRErr\n"
-		"OGR_L_DeleteFeature(OGRLayerH hLayer, GIntBig nFID)\n"
 		"\n"
 		"Delete feature from layer.\n"
 		"\n"
-		"The feature with the indicated feature id is deleted from the layer if\n"
-		"supported by the driver. Most drivers do not support feature deletion,\n"
-		"and will return OGRERR_UNSUPPORTED_OPERATION. The\n"
-		"OGR_L_TestCapability() function may be called with OLCDeleteFeature to\n"
-		"check if the driver supports feature deletion.\n"
-		"\n"
-		"This method is the same as the C++ method OGRLayer::DeleteFeature().\n"
+		"For more details: :cpp:func:`OGR_L_DeleteFeature`\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"fid: int\n"
+		"    The feature id to be deleted from the layer\n"
 		"\n"
-		"hLayer:  handle to the layer\n"
-		"\n"
-		"nFID:  the feature id to be deleted from the layer\n"
-		"\n"
-		"OGRERR_NONE if the operation works, otherwise an appropriate error\n"
-		"code (e.g OGRERR_NON_EXISTING_FEATURE if the feature does not exist).\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    :py:const:`osgeo.ogr.OGRERR_NONE` if the operation works,\n"
+		"    otherwise an appropriate error code\n"
+		"    (e.g :py:const:`osgeo.ogr.OGRERR_NON_EXISTING_FEATURE`)\n"
+		"    if the feature does not exist.\n"
 		"\n"
 		""},
 	 { "Layer_SyncToDisk", _wrap_Layer_SyncToDisk, METH_O, "\n"
 		"Layer_SyncToDisk(Layer self) -> OGRErr\n"
-		"OGRErr OGR_L_SyncToDisk(OGRLayerH\n"
-		"hLayer)\n"
 		"\n"
 		"Flush pending changes to disk.\n"
 		"\n"
-		"This call is intended to force the layer to flush any pending writes\n"
-		"to disk, and leave the disk file in a consistent state. It would not\n"
-		"normally have any effect on read-only datasources.\n"
-		"\n"
-		"Some layers do not implement this method, and will still return\n"
-		"OGRERR_NONE. The default implementation just returns OGRERR_NONE. An\n"
-		"error is only returned if an error occurs while attempting to flush to\n"
-		"disk.\n"
-		"\n"
-		"In any event, you should always close any opened datasource with\n"
-		"OGR_DS_Destroy() that will ensure all data is correctly flushed.\n"
-		"\n"
-		"This method is the same as the C++ method OGRLayer::SyncToDisk()\n"
-		"\n"
-		"Parameters:\n"
-		"-----------\n"
+		"For more details: :cpp:func:`OGR_L_SyncToDisk`\n"
 		"\n"
-		"hLayer:  handle to the layer\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    :py:const:`osgeo.ogr.OGRERR_NONE` if no error occurs\n"
+		"    (even if nothing is done) or an error code.\n"
 		"\n"
-		"OGRERR_NONE if no error occurs (even if nothing is done) or an error\n"
-		"code. \n"
 		""},
 	 { "Layer_GetLayerDefn", _wrap_Layer_GetLayerDefn, METH_O, "\n"
 		"Layer_GetLayerDefn(Layer self) -> FeatureDefn\n"
-		"OGRFeatureDefnH\n"
-		"OGR_L_GetLayerDefn(OGRLayerH hLayer)\n"
 		"\n"
 		"Fetch the schema information for this layer.\n"
 		"\n"
-		"The returned handle to the OGRFeatureDefn is owned by the OGRLayer,\n"
-		"and should not be modified or freed by the application. It\n"
-		"encapsulates the attribute schema of the features of the layer.\n"
+		"For more details: :cpp:func:`OGR_L_GetLayerDefn`\n"
 		"\n"
-		"This function is the same as the C++ method OGRLayer::GetLayerDefn().\n"
+		"Returns\n"
+		"--------\n"
+		"FeatureDefn:\n"
+		"    The feature definition.\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
-		"\n"
-		"hLayer:  handle to the layer to get the schema information.\n"
-		"\n"
-		"a handle to the feature definition. \n"
 		""},
 	 { "Layer_GetFeatureCount", (PyCFunction)(void(*)(void))_wrap_Layer_GetFeatureCount, METH_VARARGS|METH_KEYWORDS, "\n"
 		"Layer_GetFeatureCount(Layer self, int force=1) -> GIntBig\n"
-		"GIntBig\n"
-		"OGR_L_GetFeatureCount(OGRLayerH hLayer, int bForce)\n"
 		"\n"
 		"Fetch the feature count in this layer.\n"
 		"\n"
-		"Returns the number of features in the layer. For dynamic databases the\n"
-		"count may not be exact. If bForce is FALSE, and it would be expensive\n"
-		"to establish the feature count a value of -1 may be returned\n"
-		"indicating that the count isn't know. If bForce is TRUE some\n"
-		"implementations will actually scan the entire layer once to count\n"
-		"objects.\n"
-		"\n"
-		"The returned count takes the spatial filter into account.\n"
-		"\n"
-		"Note that some implementations of this method may alter the read\n"
-		"cursor of the layer.\n"
-		"\n"
-		"This function is the same as the CPP OGRLayer::GetFeatureCount().\n"
-		"\n"
-		"Note: since GDAL 2.0, this method returns a GIntBig (previously a int)\n"
+		"For more details: :cpp:func:`OGR_L_GetFeatureCount`\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"force: int\n"
+		"    Flag indicating whether the count should be computed even if\n"
+		"    it is expensive.\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    Feature count, -1 if count not known.\n"
 		"\n"
-		"hLayer:  handle to the layer that owned the features.\n"
-		"\n"
-		"bForce:  Flag indicating whether the count should be computed even if\n"
-		"it is expensive.\n"
-		"\n"
-		"feature count, -1 if count not known. \n"
 		""},
 	 { "Layer_GetExtent", (PyCFunction)(void(*)(void))_wrap_Layer_GetExtent, METH_VARARGS|METH_KEYWORDS, "\n"
 		"Layer_GetExtent(Layer self, int force=1, int can_return_null=0, int geom_field=0)\n"
-		"OGRErr OGR_L_GetExtent(OGRLayerH\n"
-		"hLayer, OGREnvelope *psExtent, int bForce)\n"
 		"\n"
 		"Fetch the extent of this layer.\n"
 		"\n"
-		"Returns the extent (MBR) of the data in the layer. If bForce is FALSE,\n"
-		"and it would be expensive to establish the extent then OGRERR_FAILURE\n"
-		"will be returned indicating that the extent isn't know. If bForce is\n"
-		"TRUE then some implementations will actually scan the entire layer\n"
-		"once to compute the MBR of all the features in the layer.\n"
-		"\n"
-		"Depending on the drivers, the returned extent may or may not take the\n"
-		"spatial filter into account. So it is safer to call OGR_L_GetExtent()\n"
-		"without setting a spatial filter.\n"
+		"For more details:\n"
 		"\n"
-		"Layers without any geometry may return OGRERR_FAILURE just indicating\n"
-		"that no meaningful extents could be collected.\n"
+		"- :cpp:func:`OGR_L_GetExtent`\n"
+		"- :cpp:func:`OGR_L_GetExtentEx`\n"
 		"\n"
-		"Note that some implementations of this method may alter the read\n"
-		"cursor of the layer.\n"
+		".. warning:: Check the return order of the bounds.\n"
 		"\n"
-		"This function is the same as the C++ method OGRLayer::GetExtent().\n"
-		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"force: int, default=False\n"
+		"    Flag indicating whether the extent should be computed even if\n"
+		"    it is expensive.\n"
+		"can_return_null: int, default=False\n"
+		"    Whether None can be returned in the response.\n"
+		"geom_field: int, default=0\n"
+		"    Ithe index of the geometry field on which to compute the extent.\n"
+		"    Can be iterated over using :py:func:`range` and :py:func:`GetGeomFieldCount`.\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"minx: float\n"
+		"maxx: float\n"
+		"miny: float\n"
+		"maxy: float\n"
 		"\n"
-		"hLayer:  handle to the layer from which to get extent.\n"
-		"\n"
-		"psExtent:  the structure in which the extent value will be returned.\n"
-		"\n"
-		"bForce:  Flag indicating whether the extent should be computed even if\n"
-		"it is expensive.\n"
-		"\n"
-		"OGRERR_NONE on success, OGRERR_FAILURE if extent not known. \n"
 		""},
 	 { "Layer_TestCapability", _wrap_Layer_TestCapability, METH_VARARGS, "\n"
 		"Layer_TestCapability(Layer self, char const * cap) -> bool\n"
-		"int\n"
-		"OGR_L_TestCapability(OGRLayerH hLayer, const char *pszCap)\n"
 		"\n"
 		"Test if this layer supported the named capability.\n"
 		"\n"
-		"The capability codes that can be tested are represented as strings,\n"
-		"but #defined constants exists to ensure correct spelling. Specific\n"
-		"layer types may implement class specific capabilities, but this can't\n"
-		"generally be discovered by the caller.\n"
-		"\n"
-		"OLCRandomRead / \"RandomRead\": TRUE if the GetFeature() method is\n"
-		"implemented in an optimized way for this layer, as opposed to the\n"
-		"default implementation using ResetReading() and GetNextFeature() to\n"
-		"find the requested feature id.\n"
-		"\n"
-		"OLCSequentialWrite / \"SequentialWrite\": TRUE if the CreateFeature()\n"
-		"method works for this layer. Note this means that this particular\n"
-		"layer is writable. The same OGRLayer class may returned FALSE for\n"
-		"other layer instances that are effectively read-only.\n"
-		"\n"
-		"OLCRandomWrite / \"RandomWrite\": TRUE if the SetFeature() method is\n"
-		"operational on this layer. Note this means that this particular layer\n"
-		"is writable. The same OGRLayer class may returned FALSE for other\n"
-		"layer instances that are effectively read-only.\n"
-		"\n"
-		"OLCFastSpatialFilter / \"FastSpatialFilter\": TRUE if this layer\n"
-		"implements spatial filtering efficiently. Layers that effectively read\n"
-		"all features, and test them with the OGRFeature intersection methods\n"
-		"should return FALSE. This can be used as a clue by the application\n"
-		"whether it should build and maintain its own spatial index for\n"
-		"features in this layer.\n"
-		"\n"
-		"OLCFastFeatureCount / \"FastFeatureCount\": TRUE if this layer can\n"
-		"return a feature count (via OGR_L_GetFeatureCount()) efficiently, i.e.\n"
-		"without counting the features. In some cases this will return TRUE\n"
-		"until a spatial filter is installed after which it will return FALSE.\n"
-		"\n"
-		"OLCFastGetExtent / \"FastGetExtent\": TRUE if this layer can return\n"
-		"its data extent (via OGR_L_GetExtent()) efficiently, i.e. without\n"
-		"scanning all the features. In some cases this will return TRUE until a\n"
-		"spatial filter is installed after which it will return FALSE.\n"
-		"\n"
-		"OLCFastSetNextByIndex / \"FastSetNextByIndex\": TRUE if this layer can\n"
-		"perform the SetNextByIndex() call efficiently, otherwise FALSE.\n"
-		"\n"
-		"OLCCreateField / \"CreateField\": TRUE if this layer can create new\n"
-		"fields on the current layer using CreateField(), otherwise FALSE.\n"
-		"\n"
-		"OLCCreateGeomField / \"CreateGeomField\": (GDAL >= 1.11) TRUE if this\n"
-		"layer can create new geometry fields on the current layer using\n"
-		"CreateGeomField(), otherwise FALSE.\n"
-		"\n"
-		"OLCDeleteField / \"DeleteField\": TRUE if this layer can delete\n"
-		"existing fields on the current layer using DeleteField(), otherwise\n"
-		"FALSE.\n"
-		"\n"
-		"OLCReorderFields / \"ReorderFields\": TRUE if this layer can reorder\n"
-		"existing fields on the current layer using ReorderField() or\n"
-		"ReorderFields(), otherwise FALSE.\n"
-		"\n"
-		"OLCAlterFieldDefn / \"AlterFieldDefn\": TRUE if this layer can alter\n"
-		"the definition of an existing field on the current layer using\n"
-		"AlterFieldDefn(), otherwise FALSE.\n"
-		"\n"
-		"OLCDeleteFeature / \"DeleteFeature\": TRUE if the DeleteFeature()\n"
-		"method is supported on this layer, otherwise FALSE.\n"
-		"\n"
-		"OLCStringsAsUTF8 / \"StringsAsUTF8\": TRUE if values of OFTString\n"
-		"fields are assured to be in UTF-8 format. If FALSE the encoding of\n"
-		"fields is uncertain, though it might still be UTF-8.\n"
-		"\n"
-		"OLCTransactions / \"Transactions\": TRUE if the StartTransaction(),\n"
-		"CommitTransaction() and RollbackTransaction() methods work in a\n"
-		"meaningful way, otherwise FALSE.\n"
+		"For more details: :cpp:func:`OGR_L_TestCapability`\n"
 		"\n"
-		"OLCCurveGeometries / \"CurveGeometries\": TRUE if this layer supports\n"
-		"writing curve geometries or may return such geometries. (GDAL 2.0).\n"
-		"\n"
-		"This function is the same as the C++ method\n"
-		"OGRLayer::TestCapability().\n"
-		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"cap: str\n"
+		"    The name of the capability to test. These can\n"
+		"    be found in the `osgeo.ogr` namespace. For example,\n"
+		"    :py:const:`osgeo.ogr.OLCRandomRead`.\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    True if the layer has the requested capability, or False otherwise.\n"
+		"    Will return False for any unrecognized capabilities.\n"
 		"\n"
-		"hLayer:  handle to the layer to get the capability from.\n"
-		"\n"
-		"pszCap:  the name of the capability to test.\n"
-		"\n"
-		"TRUE if the layer has the requested capability, or FALSE otherwise.\n"
-		"OGRLayers will return FALSE for any unrecognized capabilities. \n"
 		""},
 	 { "Layer_CreateField", (PyCFunction)(void(*)(void))_wrap_Layer_CreateField, METH_VARARGS|METH_KEYWORDS, "\n"
 		"Layer_CreateField(Layer self, FieldDefn field_def, int approx_ok=1) -> OGRErr\n"
-		"OGRErr\n"
-		"OGR_L_CreateField(OGRLayerH hLayer, OGRFieldDefnH hField, int\n"
-		"bApproxOK)\n"
 		"\n"
 		"Create a new field on a layer.\n"
 		"\n"
-		"You must use this to create new fields on a real layer. Internally the\n"
-		"OGRFeatureDefn for the layer will be updated to reflect the new field.\n"
-		"Applications should never modify the OGRFeatureDefn used by a layer\n"
-		"directly.\n"
-		"\n"
-		"This function should not be called while there are feature objects in\n"
-		"existence that were obtained or created with the previous layer\n"
-		"definition.\n"
-		"\n"
-		"Not all drivers support this function. You can query a layer to check\n"
-		"if it supports it with the OLCCreateField capability. Some drivers may\n"
-		"only support this method while there are still no features in the\n"
-		"layer. When it is supported, the existing features of the backing\n"
-		"file/database should be updated accordingly.\n"
+		"For more details: :cpp:func:`OGR_L_CreateField`\n"
 		"\n"
-		"Drivers may or may not support not-null constraints. If they support\n"
-		"creating fields with not-null constraints, this is generally before\n"
-		"creating any feature to the layer.\n"
-		"\n"
-		"This function is the same as the C++ method OGRLayer::CreateField().\n"
-		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"field_def: FieldDefn\n"
+		"    The field definition to write to disk.\n"
+		"approx_ok: bool, default=True\n"
+		"    If True, the field may be created in a slightly different\n"
+		"    form depending on the limitations of the format driver.\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    :py:const:`osgeo.ogr.OGRERR_NONE` on success.\n"
 		"\n"
-		"hLayer:  handle to the layer to write the field definition.\n"
-		"\n"
-		"hField:  handle of the field definition to write to disk.\n"
-		"\n"
-		"bApproxOK:  If TRUE, the field may be created in a slightly different\n"
-		"form depending on the limitations of the format driver.\n"
-		"\n"
-		"OGRERR_NONE on success. \n"
 		""},
 	 { "Layer_DeleteField", _wrap_Layer_DeleteField, METH_VARARGS, "\n"
 		"Layer_DeleteField(Layer self, int iField) -> OGRErr\n"
-		"OGRErr\n"
-		"OGR_L_DeleteField(OGRLayerH hLayer, int iField)\n"
 		"\n"
 		"Delete an existing field on a layer.\n"
 		"\n"
-		"You must use this to delete existing fields on a real layer.\n"
-		"Internally the OGRFeatureDefn for the layer will be updated to reflect\n"
-		"the deleted field. Applications should never modify the OGRFeatureDefn\n"
-		"used by a layer directly.\n"
-		"\n"
-		"This function should not be called while there are feature objects in\n"
-		"existence that were obtained or created with the previous layer\n"
-		"definition.\n"
+		"For more details: :cpp:func:`OGR_L_DeleteField`\n"
 		"\n"
-		"Not all drivers support this function. You can query a layer to check\n"
-		"if it supports it with the OLCDeleteField capability. Some drivers may\n"
-		"only support this method while there are still no features in the\n"
-		"layer. When it is supported, the existing features of the backing\n"
-		"file/database should be updated accordingly.\n"
-		"\n"
-		"This function is the same as the C++ method OGRLayer::DeleteField().\n"
-		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"iField: int\n"
+		"    index of the field to delete.\n"
 		"\n"
-		"hLayer:  handle to the layer.\n"
-		"\n"
-		"iField:  index of the field to delete.\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    :py:const:`osgeo.ogr.OGRERR_NONE` on success.\n"
 		"\n"
-		"OGRERR_NONE on success.\n"
-		"\n"
-		"OGR 1.9.0 \n"
 		""},
 	 { "Layer_ReorderField", _wrap_Layer_ReorderField, METH_VARARGS, "\n"
 		"Layer_ReorderField(Layer self, int iOldFieldPos, int iNewFieldPos) -> OGRErr\n"
-		"OGRErr\n"
-		"OGR_L_ReorderField(OGRLayerH hLayer, int iOldFieldPos, int\n"
-		"iNewFieldPos)\n"
 		"\n"
 		"Reorder an existing field on a layer.\n"
 		"\n"
-		"This function is a convenience wrapper of OGR_L_ReorderFields()\n"
-		"dedicated to move a single field.\n"
-		"\n"
-		"You must use this to reorder existing fields on a real layer.\n"
-		"Internally the OGRFeatureDefn for the layer will be updated to reflect\n"
-		"the reordering of the fields. Applications should never modify the\n"
-		"OGRFeatureDefn used by a layer directly.\n"
-		"\n"
-		"This function should not be called while there are feature objects in\n"
-		"existence that were obtained or created with the previous layer\n"
-		"definition.\n"
-		"\n"
-		"The field definition that was at initial position iOldFieldPos will be\n"
-		"moved at position iNewFieldPos, and elements between will be shuffled\n"
-		"accordingly.\n"
-		"\n"
-		"For example, let suppose the fields were \"0\",\"1\",\"2\",\"3\",\"4\"\n"
-		"initially. ReorderField(1, 3) will reorder them as\n"
-		"\"0\",\"2\",\"3\",\"1\",\"4\".\n"
+		"For more details: :cpp:func:`OGR_L_ReorderField`\n"
 		"\n"
-		"Not all drivers support this function. You can query a layer to check\n"
-		"if it supports it with the OLCReorderFields capability. Some drivers\n"
-		"may only support this method while there are still no features in the\n"
-		"layer. When it is supported, the existing features of the backing\n"
-		"file/database should be updated accordingly.\n"
-		"\n"
-		"This function is the same as the C++ method OGRLayer::ReorderField().\n"
-		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"iOldFieldPos: int\n"
+		"    previous position of the field to move. Must be in the\n"
+		"    range [0,GetFieldCount()-1].\n"
+		"iNewFieldPos: int\n"
+		"    new position of the field to move. Must be in the range\n"
+		"    [0,GetFieldCount()-1].\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    :py:const:`osgeo.ogr.OGRERR_NONE` on success.\n"
 		"\n"
-		"hLayer:  handle to the layer.\n"
-		"\n"
-		"iOldFieldPos:  previous position of the field to move. Must be in the\n"
-		"range [0,GetFieldCount()-1].\n"
-		"\n"
-		"iNewFieldPos:  new position of the field to move. Must be in the range\n"
-		"[0,GetFieldCount()-1].\n"
-		"\n"
-		"OGRERR_NONE on success.\n"
-		"\n"
-		"OGR 1.9.0 \n"
 		""},
 	 { "Layer_ReorderFields", _wrap_Layer_ReorderFields, METH_VARARGS, "\n"
 		"Layer_ReorderFields(Layer self, int nList) -> OGRErr\n"
-		"OGRErr\n"
-		"OGR_L_ReorderFields(OGRLayerH hLayer, int *panMap)\n"
 		"\n"
 		"Reorder all the fields of a layer.\n"
 		"\n"
-		"You must use this to reorder existing fields on a real layer.\n"
-		"Internally the OGRFeatureDefn for the layer will be updated to reflect\n"
-		"the reordering of the fields. Applications should never modify the\n"
-		"OGRFeatureDefn used by a layer directly.\n"
-		"\n"
-		"This function should not be called while there are feature objects in\n"
-		"existence that were obtained or created with the previous layer\n"
-		"definition.\n"
-		"\n"
-		"panMap is such that,for each field definition at position i after\n"
-		"reordering, its position before reordering was panMap[i].\n"
-		"\n"
-		"For example, let suppose the fields were \"0\",\"1\",\"2\",\"3\",\"4\"\n"
-		"initially. ReorderFields([0,2,3,1,4]) will reorder them as\n"
-		"\"0\",\"2\",\"3\",\"1\",\"4\".\n"
-		"\n"
-		"Not all drivers support this function. You can query a layer to check\n"
-		"if it supports it with the OLCReorderFields capability. Some drivers\n"
-		"may only support this method while there are still no features in the\n"
-		"layer. When it is supported, the existing features of the backing\n"
-		"file/database should be updated accordingly.\n"
-		"\n"
-		"This function is the same as the C++ method OGRLayer::ReorderFields().\n"
+		"For more details: :cpp:func:`OGR_L_ReorderFields`\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"nList: list[int]\n"
+		"    A list of GetLayerDefn().GetFieldCount()\n"
+		"    elements which is a permutation of\n"
+		"    [0, GetLayerDefn().GetFieldCount()-1].\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    :py:const:`osgeo.ogr.OGRERR_NONE` on success.\n"
 		"\n"
-		"hLayer:  handle to the layer.\n"
-		"\n"
-		"panMap:  an array of GetLayerDefn()-> OGRFeatureDefn::GetFieldCount()\n"
-		"elements which is a permutation of [0, GetLayerDefn()->\n"
-		"OGRFeatureDefn::GetFieldCount()-1].\n"
-		"\n"
-		"OGRERR_NONE on success.\n"
-		"\n"
-		"OGR 1.9.0 \n"
 		""},
 	 { "Layer_AlterFieldDefn", _wrap_Layer_AlterFieldDefn, METH_VARARGS, "\n"
 		"Layer_AlterFieldDefn(Layer self, int iField, FieldDefn field_def, int nFlags) -> OGRErr\n"
-		"OGRErr\n"
-		"OGR_L_AlterFieldDefn(OGRLayerH hLayer, int iField, OGRFieldDefnH\n"
-		"hNewFieldDefn, int nFlags)\n"
 		"\n"
 		"Alter the definition of an existing field on a layer.\n"
 		"\n"
-		"You must use this to alter the definition of an existing field of a\n"
-		"real layer. Internally the OGRFeatureDefn for the layer will be\n"
-		"updated to reflect the altered field. Applications should never modify\n"
-		"the OGRFeatureDefn used by a layer directly.\n"
-		"\n"
-		"This function should not be called while there are feature objects in\n"
-		"existence that were obtained or created with the previous layer\n"
-		"definition.\n"
-		"\n"
-		"Not all drivers support this function. You can query a layer to check\n"
-		"if it supports it with the OLCAlterFieldDefn capability. Some drivers\n"
-		"may only support this method while there are still no features in the\n"
-		"layer. When it is supported, the existing features of the backing\n"
-		"file/database should be updated accordingly. Some drivers might also\n"
-		"not support all update flags.\n"
+		"For more details: :cpp:func:`OGR_L_AlterFieldDefn`\n"
 		"\n"
-		"This function is the same as the C++ method\n"
-		"OGRLayer::AlterFieldDefn().\n"
-		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"iField: int\n"
+		"    index of the field whose definition must be altered.\n"
+		"field_def: FieldDefn\n"
+		"    new field definition\n"
+		"nFlags: int\n"
+		"    Combination of\n"
+		"    :py:const:`osgeo.ogr.ALTER_NAME_FLAG`,\n"
+		"    :py:const:`osgeo.ogr.ALTER_TYPE_FLAG`,\n"
+		"    :py:const:`osgeo.ogr.ALTER_WIDTH_PRECISION_FLAG`,\n"
+		"    :py:const:`osgeo.ogr.ALTER_NULLABLE_FLAG` and\n"
+		"    :py:const:`osgeo.ogr.ALTER_DEFAULT_FLAG`\n"
+		"    to indicate which of the name and/or type and/or width and precision\n"
+		"    fields and/or nullability from the new field definition must be taken\n"
+		"    into account.\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    :py:const:`osgeo.ogr.OGRERR_NONE` on success.\n"
 		"\n"
-		"hLayer:  handle to the layer.\n"
-		"\n"
-		"iField:  index of the field whose definition must be altered.\n"
-		"\n"
-		"hNewFieldDefn:  new field definition\n"
-		"\n"
-		"nFlags:  combination of ALTER_NAME_FLAG, ALTER_TYPE_FLAG,\n"
-		"ALTER_WIDTH_PRECISION_FLAG, ALTER_NULLABLE_FLAG and ALTER_DEFAULT_FLAG\n"
-		"to indicate which of the name and/or type and/or width and precision\n"
-		"fields and/or nullability from the new field definition must be taken\n"
-		"into account.\n"
-		"\n"
-		"OGRERR_NONE on success.\n"
-		"\n"
-		"OGR 1.9.0 \n"
 		""},
+	 { "Layer_AlterGeomFieldDefn", _wrap_Layer_AlterGeomFieldDefn, METH_VARARGS, "Layer_AlterGeomFieldDefn(Layer self, int iGeomField, GeomFieldDefn field_def, int nFlags) -> OGRErr"},
 	 { "Layer_CreateGeomField", (PyCFunction)(void(*)(void))_wrap_Layer_CreateGeomField, METH_VARARGS|METH_KEYWORDS, "\n"
 		"Layer_CreateGeomField(Layer self, GeomFieldDefn field_def, int approx_ok=1) -> OGRErr\n"
-		"OGRErr\n"
-		"OGR_L_CreateGeomField(OGRLayerH hLayer, OGRGeomFieldDefnH hField, int\n"
-		"bApproxOK)\n"
 		"\n"
 		"Create a new geometry field on a layer.\n"
 		"\n"
-		"You must use this to create new geometry fields on a real layer.\n"
-		"Internally the OGRFeatureDefn for the layer will be updated to reflect\n"
-		"the new field. Applications should never modify the OGRFeatureDefn\n"
-		"used by a layer directly.\n"
-		"\n"
-		"This function should not be called while there are feature objects in\n"
-		"existence that were obtained or created with the previous layer\n"
-		"definition.\n"
+		"For more details: :cpp:func:`OGR_L_CreateGeomField`\n"
 		"\n"
-		"Not all drivers support this function. You can query a layer to check\n"
-		"if it supports it with the OLCCreateField capability. Some drivers may\n"
-		"only support this method while there are still no features in the\n"
-		"layer. When it is supported, the existing features of the backing\n"
-		"file/database should be updated accordingly.\n"
-		"\n"
-		"Drivers may or may not support not-null constraints. If they support\n"
-		"creating fields with not-null constraints, this is generally before\n"
-		"creating any feature to the layer.\n"
-		"\n"
-		"This function is the same as the C++ method OGRLayer::CreateField().\n"
-		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"field_def: GeomFieldDefn\n"
+		"    The geometry field definition to write to disk.\n"
+		"approx_ok: bool, default=True\n"
+		"    If True, the field may be created in a slightly different\n"
+		"    form depending on the limitations of the format driver.\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    :py:const:`osgeo.ogr.OGRERR_NONE` on success.\n"
 		"\n"
-		"hLayer:  handle to the layer to write the field definition.\n"
-		"\n"
-		"hField:  handle of the geometry field definition to write to disk.\n"
-		"\n"
-		"bApproxOK:  If TRUE, the field may be created in a slightly different\n"
-		"form depending on the limitations of the format driver.\n"
-		"\n"
-		"OGRERR_NONE on success.\n"
-		"\n"
-		"OGR 1.11 \n"
 		""},
 	 { "Layer_StartTransaction", _wrap_Layer_StartTransaction, METH_O, "\n"
 		"Layer_StartTransaction(Layer self) -> OGRErr\n"
-		"OGRErr\n"
-		"OGR_L_StartTransaction(OGRLayerH hLayer)\n"
-		"\n"
-		"For datasources which support transactions, StartTransaction creates a\n"
-		"transaction.\n"
 		"\n"
-		"If starting the transaction fails, will return OGRERR_FAILURE.\n"
-		"Datasources which do not support transactions will always return\n"
-		"OGRERR_NONE.\n"
-		"\n"
-		"Note: as of GDAL 2.0, use of this API is discouraged when the dataset\n"
-		"offers dataset level transaction with GDALDataset::StartTransaction().\n"
-		"The reason is that most drivers can only offer transactions at dataset\n"
-		"level, and not layer level. Very few drivers really support\n"
-		"transactions at layer scope.\n"
+		"For datasources which support transactions, this creates a transaction.\n"
 		"\n"
-		"This function is the same as the C++ method\n"
-		"OGRLayer::StartTransaction().\n"
-		"\n"
-		"Parameters:\n"
-		"-----------\n"
+		"For more details: :cpp:func:`OGR_L_StartTransaction`\n"
 		"\n"
-		"hLayer:  handle to the layer\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    :py:const:`osgeo.ogr.OGRERR_NONE` on success.\n"
 		"\n"
-		"OGRERR_NONE on success. \n"
 		""},
 	 { "Layer_CommitTransaction", _wrap_Layer_CommitTransaction, METH_O, "\n"
 		"Layer_CommitTransaction(Layer self) -> OGRErr\n"
-		"OGRErr\n"
-		"OGR_L_CommitTransaction(OGRLayerH hLayer)\n"
-		"\n"
-		"For datasources which support transactions, CommitTransaction commits\n"
-		"a transaction.\n"
 		"\n"
-		"If no transaction is active, or the commit fails, will return\n"
-		"OGRERR_FAILURE. Datasources which do not support transactions will\n"
-		"always return OGRERR_NONE.\n"
+		"For datasources which support transactions, this commits a transaction.\n"
 		"\n"
-		"This function is the same as the C++ method\n"
-		"OGRLayer::CommitTransaction().\n"
+		"For more details: :cpp:func:`OGR_L_CommitTransaction`\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    :py:const:`osgeo.ogr.OGRERR_NONE` on success.\n"
 		"\n"
-		"hLayer:  handle to the layer\n"
-		"\n"
-		"OGRERR_NONE on success. \n"
 		""},
 	 { "Layer_RollbackTransaction", _wrap_Layer_RollbackTransaction, METH_O, "\n"
 		"Layer_RollbackTransaction(Layer self) -> OGRErr\n"
-		"OGRErr\n"
-		"OGR_L_RollbackTransaction(OGRLayerH hLayer)\n"
 		"\n"
-		"For datasources which support transactions, RollbackTransaction will\n"
-		"roll back a datasource to its state before the start of the current\n"
-		"transaction.\n"
-		"\n"
-		"If no transaction is active, or the rollback fails, will return\n"
-		"OGRERR_FAILURE. Datasources which do not support transactions will\n"
-		"always return OGRERR_NONE.\n"
+		"Roll back a datasource to its state before the start of the current transaction.\n"
 		"\n"
-		"This function is the same as the C++ method\n"
-		"OGRLayer::RollbackTransaction().\n"
+		"For more details: :cpp:func:`OGR_L_RollbackTransaction`\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
-		"\n"
-		"hLayer:  handle to the layer\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    :py:const:`osgeo.ogr.OGRERR_NONE` on success.\n"
 		"\n"
-		"OGRERR_NONE on success. \n"
 		""},
 	 { "Layer_FindFieldIndex", _wrap_Layer_FindFieldIndex, METH_VARARGS, "\n"
 		"Layer_FindFieldIndex(Layer self, char const * pszFieldName, int bExactMatch) -> int\n"
-		"int\n"
-		"OGR_L_FindFieldIndex(OGRLayerH hLayer, const char *pszFieldName, int\n"
-		"bExactMatch)\n"
 		"\n"
 		"Find the index of field in a layer.\n"
 		"\n"
-		"The returned number is the index of the field in the layers, or -1 if\n"
-		"the field doesn't exist.\n"
+		"For more details: :cpp:func:`OGR_L_FindFieldIndex`\n"
 		"\n"
-		"If bExactMatch is set to FALSE and the field doesn't exists in the\n"
-		"given form the driver might apply some changes to make it match, like\n"
-		"those it might do if the layer was created (eg. like LAUNDER in the\n"
-		"OCI driver).\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    field index, or -1 if the field doesn't exist\n"
 		"\n"
-		"This method is the same as the C++ method OGRLayer::FindFieldIndex().\n"
-		"\n"
-		"field index, or -1 if the field doesn't exist \n"
 		""},
 	 { "Layer_GetSpatialRef", _wrap_Layer_GetSpatialRef, METH_O, "\n"
 		"Layer_GetSpatialRef(Layer self) -> SpatialReference\n"
-		"OGRSpatialReferenceH\n"
-		"OGR_L_GetSpatialRef(OGRLayerH hLayer)\n"
 		"\n"
 		"Fetch the spatial reference system for this layer.\n"
 		"\n"
-		"The returned object is owned by the OGRLayer and should not be\n"
-		"modified or freed by the application.\n"
-		"\n"
-		"This function is the same as the C++ method OGRLayer::GetSpatialRef().\n"
+		"For more details: :cpp:func:`OGR_L_GetSpatialRef`\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
+		"Returns\n"
+		"--------\n"
+		"SpatialReference:\n"
+		"    spatial reference, or None if there isn't one.\n"
 		"\n"
-		"hLayer:  handle to the layer to get the spatial reference from.\n"
-		"\n"
-		"spatial reference, or NULL if there isn't one. \n"
 		""},
 	 { "Layer_GetFeaturesRead", _wrap_Layer_GetFeaturesRead, METH_O, "\n"
 		"Layer_GetFeaturesRead(Layer self) -> GIntBig\n"
-		"GIntBig\n"
-		"OGR_L_GetFeaturesRead(OGRLayerH hLayer) \n"
+		"\n"
+		"For more details: :cpp:func:`OGR_L_GetFeaturesRead`\n"
+		"\n"
 		""},
 	 { "Layer_SetIgnoredFields", _wrap_Layer_SetIgnoredFields, METH_VARARGS, "\n"
 		"Layer_SetIgnoredFields(Layer self, char const ** options) -> OGRErr\n"
-		"OGRErr\n"
-		"OGR_L_SetIgnoredFields(OGRLayerH hLayer, const char **papszFields)\n"
 		"\n"
 		"Set which fields can be omitted when retrieving features from the\n"
 		"layer.\n"
 		"\n"
-		"If the driver supports this functionality (testable using\n"
-		"OLCIgnoreFields capability), it will not fetch the specified fields in\n"
-		"subsequent calls to GetFeature() / GetNextFeature() and thus save some\n"
-		"processing time and/or bandwidth.\n"
-		"\n"
-		"Besides field names of the layers, the following special fields can be\n"
-		"passed: \"OGR_GEOMETRY\" to ignore geometry and \"OGR_STYLE\" to\n"
-		"ignore layer style.\n"
-		"\n"
-		"By default, no fields are ignored.\n"
+		"For more details: :cpp:func:`OGR_L_SetIgnoredFields`\n"
 		"\n"
-		"This method is the same as the C++ method OGRLayer::SetIgnoredFields()\n"
-		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"options: list[str]\n"
+		"    A list of field names.\n"
+		"    If an empty list is passed, the ignored list is cleared.\n"
+		"\n"
+		"Returns\n"
+		"-------\n"
+		"int:\n"
+		"    :py:const:`osgeo.ogr.OGRERR_NONE` if all field names have been resolved\n"
+		"    (even if the driver does not support this method)\n"
 		"\n"
-		"hLayer:  handle to the layer\n"
-		"\n"
-		"papszFields:  an array of field names terminated by NULL item. If NULL\n"
-		"is passed, the ignored list is cleared.\n"
-		"\n"
-		"OGRERR_NONE if all field names have been resolved (even if the driver\n"
-		"does not support this method) \n"
 		""},
 	 { "Layer_Intersection", (PyCFunction)(void(*)(void))_wrap_Layer_Intersection, METH_VARARGS|METH_KEYWORDS, "\n"
 		"Layer_Intersection(Layer self, Layer method_layer, Layer result_layer, char ** options=None, GDALProgressFunc callback=0, void * callback_data=None) -> OGRErr\n"
-		"OGRErr\n"
-		"OGR_L_Intersection(OGRLayerH pLayerInput, OGRLayerH pLayerMethod,\n"
-		"OGRLayerH pLayerResult, char **papszOptions, GDALProgressFunc\n"
-		"pfnProgress, void *pProgressArg)\n"
 		"\n"
 		"Intersection of two layers.\n"
 		"\n"
-		"The result layer contains features whose geometries represent areas\n"
-		"that are common between features in the input layer and in the method\n"
-		"layer. The features in the result layer have attributes from both\n"
-		"input and method layers. The schema of the result layer can be set by\n"
-		"the user or, if it is empty, is initialized to contain all fields in\n"
-		"the input and method layers.\n"
-		"\n"
-		"If the schema of the result is set by user and contains fields that\n"
-		"have the same name as a field in input and in method layer, then the\n"
-		"attribute in the result feature will get the value from the feature of\n"
-		"the method layer.\n"
-		"\n"
-		"For best performance use the minimum amount of features in the method\n"
-		"layer and copy it into a memory layer.\n"
+		"For more details: :cpp:func:`OGR_L_Intersection`\n"
 		"\n"
-		"This method relies on GEOS support. Do not use unless the GEOS support\n"
-		"is compiled in.  The recognized list of options is :\n"
-		"SKIP_FAILURES=YES/NO. Set it to YES to go on, even when a feature\n"
-		"could not be inserted or a GEOS call failed.\n"
-		"\n"
-		"PROMOTE_TO_MULTI=YES/NO. Set it to YES to convert Polygons into\n"
-		"MultiPolygons, or LineStrings to MultiLineStrings.\n"
-		"\n"
-		"INPUT_PREFIX=string. Set a prefix for the field names that will be\n"
-		"created from the fields of the input layer.\n"
-		"\n"
-		"METHOD_PREFIX=string. Set a prefix for the field names that will be\n"
-		"created from the fields of the method layer.\n"
-		"\n"
-		"USE_PREPARED_GEOMETRIES=YES/NO. Set to NO to not use prepared\n"
-		"geometries to pretest intersection of features of method layer with\n"
-		"features of this layer.\n"
-		"\n"
-		"PRETEST_CONTAINMENT=YES/NO. Set to YES to pretest the containment of\n"
-		"features of method layer within the features of this layer. This will\n"
-		"speed up the method significantly in some cases. Requires that the\n"
-		"prepared geometries are in effect.\n"
-		"\n"
-		"KEEP_LOWER_DIMENSION_GEOMETRIES=YES/NO. Set to NO to skip result\n"
-		"features with lower dimension geometry that would otherwise be added\n"
-		"to the result layer. The default is to add but only if the result\n"
-		"layer has an unknown geometry type.\n"
-		"\n"
-		"This function is the same as the C++ method OGRLayer::Intersection().\n"
-		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"method_layer: Layer\n"
+		"    the method layer. Should not be None.\n"
+		"result_layer: Layer\n"
+		"    the layer where the features resulting from the\n"
+		"    operation are inserted. Should not be None.\n"
+		"options: list[str], optional\n"
+		"    List of options (empty list is allowed). For example [\"PROMOTE_TO_MULTI=YES\"].\n"
+		"callback: Callable, optional\n"
+		"    a GDALProgressFunc() compatible callback function for\n"
+		"    reporting progress or None.\n"
+		"callback_data:\n"
+		"    Argument to be passed to 'callback'. May be None.\n"
+		"\n"
+		"Returns\n"
+		"-------\n"
+		"int:\n"
+		"    An error code if there was an error or the execution was interrupted,\n"
+		"    :py:const:`osgeo.ogr.OGRERR_NONE` otherwise.\n"
 		"\n"
-		"pLayerInput:  the input layer. Should not be NULL.\n"
-		"\n"
-		"pLayerMethod:  the method layer. Should not be NULL.\n"
-		"\n"
-		"pLayerResult:  the layer where the features resulting from the\n"
-		"operation are inserted. Should not be NULL. See above the note about\n"
-		"the schema.\n"
-		"\n"
-		"papszOptions:  NULL terminated list of options (may be NULL).\n"
-		"\n"
-		"pfnProgress:  a GDALProgressFunc() compatible callback function for\n"
-		"reporting progress or NULL.\n"
-		"\n"
-		"pProgressArg:  argument to be passed to pfnProgress. May be NULL.\n"
-		"\n"
-		"an error code if there was an error or the execution was interrupted,\n"
-		"OGRERR_NONE otherwise.\n"
-		"\n"
-		"The first geometry field is always used.\n"
-		"\n"
-		"OGR 1.10 \n"
 		""},
 	 { "Layer_Union", (PyCFunction)(void(*)(void))_wrap_Layer_Union, METH_VARARGS|METH_KEYWORDS, "\n"
 		"Layer_Union(Layer self, Layer method_layer, Layer result_layer, char ** options=None, GDALProgressFunc callback=0, void * callback_data=None) -> OGRErr\n"
-		"OGRErr OGR_L_Union(OGRLayerH\n"
-		"pLayerInput, OGRLayerH pLayerMethod, OGRLayerH pLayerResult, char\n"
-		"**papszOptions, GDALProgressFunc pfnProgress, void *pProgressArg)\n"
 		"\n"
 		"Union of two layers.\n"
 		"\n"
-		"The result layer contains features whose geometries represent areas\n"
-		"that are in either in the input layer, in the method layer, or in\n"
-		"both. The features in the result layer have attributes from both input\n"
-		"and method layers. For features which represent areas that are only in\n"
-		"the input or in the method layer the respective attributes have\n"
-		"undefined values. The schema of the result layer can be set by the\n"
-		"user or, if it is empty, is initialized to contain all fields in the\n"
-		"input and method layers.\n"
-		"\n"
-		"If the schema of the result is set by user and contains fields that\n"
-		"have the same name as a field in input and in method layer, then the\n"
-		"attribute in the result feature will get the value from the feature of\n"
-		"the method layer (even if it is undefined).\n"
-		"\n"
-		"For best performance use the minimum amount of features in the method\n"
-		"layer and copy it into a memory layer.\n"
-		"\n"
-		"This method relies on GEOS support. Do not use unless the GEOS support\n"
-		"is compiled in.  The recognized list of options is :\n"
-		"SKIP_FAILURES=YES/NO. Set it to YES to go on, even when a feature\n"
-		"could not be inserted or a GEOS call failed.\n"
+		"For more details: :cpp:func:`OGR_L_Union`\n"
 		"\n"
-		"PROMOTE_TO_MULTI=YES/NO. Set it to YES to convert Polygons into\n"
-		"MultiPolygons, or LineStrings to MultiLineStrings.\n"
-		"\n"
-		"INPUT_PREFIX=string. Set a prefix for the field names that will be\n"
-		"created from the fields of the input layer.\n"
-		"\n"
-		"METHOD_PREFIX=string. Set a prefix for the field names that will be\n"
-		"created from the fields of the method layer.\n"
-		"\n"
-		"USE_PREPARED_GEOMETRIES=YES/NO. Set to NO to not use prepared\n"
-		"geometries to pretest intersection of features of method layer with\n"
-		"features of this layer.\n"
-		"\n"
-		"KEEP_LOWER_DIMENSION_GEOMETRIES=YES/NO. Set to NO to skip result\n"
-		"features with lower dimension geometry that would otherwise be added\n"
-		"to the result layer. The default is to add but only if the result\n"
-		"layer has an unknown geometry type.\n"
-		"\n"
-		"This function is the same as the C++ method OGRLayer::Union().\n"
+		"The first geometry field is always used.\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"method_layer: Layer\n"
+		"    the method layer. Should not be None.\n"
+		"result_layer: Layer\n"
+		"    the layer where the features resulting from the\n"
+		"    operation are inserted. Should not be None.\n"
+		"options: list[str], optional\n"
+		"    List of options (empty list is allowed). For example [\"PROMOTE_TO_MULTI=YES\"].\n"
+		"callback: Callable, optional\n"
+		"    a GDALProgressFunc() compatible callback function for\n"
+		"    reporting progress or None.\n"
+		"callback_data:\n"
+		"    Argument to be passed to 'callback'. May be None.\n"
+		"\n"
+		"Returns\n"
+		"-------\n"
+		"int:\n"
+		"    An error code if there was an error or the execution was interrupted,\n"
+		"    :py:const:`osgeo.ogr.OGRERR_NONE` otherwise.\n"
 		"\n"
-		"pLayerInput:  the input layer. Should not be NULL.\n"
-		"\n"
-		"pLayerMethod:  the method layer. Should not be NULL.\n"
-		"\n"
-		"pLayerResult:  the layer where the features resulting from the\n"
-		"operation are inserted. Should not be NULL. See above the note about\n"
-		"the schema.\n"
-		"\n"
-		"papszOptions:  NULL terminated list of options (may be NULL).\n"
-		"\n"
-		"pfnProgress:  a GDALProgressFunc() compatible callback function for\n"
-		"reporting progress or NULL.\n"
-		"\n"
-		"pProgressArg:  argument to be passed to pfnProgress. May be NULL.\n"
-		"\n"
-		"an error code if there was an error or the execution was interrupted,\n"
-		"OGRERR_NONE otherwise.\n"
-		"\n"
-		"The first geometry field is always used.\n"
-		"\n"
-		"OGR 1.10 \n"
 		""},
 	 { "Layer_SymDifference", (PyCFunction)(void(*)(void))_wrap_Layer_SymDifference, METH_VARARGS|METH_KEYWORDS, "\n"
 		"Layer_SymDifference(Layer self, Layer method_layer, Layer result_layer, char ** options=None, GDALProgressFunc callback=0, void * callback_data=None) -> OGRErr\n"
-		"OGRErr\n"
-		"OGR_L_SymDifference(OGRLayerH pLayerInput, OGRLayerH pLayerMethod,\n"
-		"OGRLayerH pLayerResult, char **papszOptions, GDALProgressFunc\n"
-		"pfnProgress, void *pProgressArg)\n"
 		"\n"
 		"Symmetrical difference of two layers.\n"
 		"\n"
-		"The result layer contains features whose geometries represent areas\n"
-		"that are in either in the input layer or in the method layer but not\n"
-		"in both. The features in the result layer have attributes from both\n"
-		"input and method layers. For features which represent areas that are\n"
-		"only in the input or in the method layer the respective attributes\n"
-		"have undefined values. The schema of the result layer can be set by\n"
-		"the user or, if it is empty, is initialized to contain all fields in\n"
-		"the input and method layers.\n"
-		"\n"
-		"If the schema of the result is set by user and contains fields that\n"
-		"have the same name as a field in input and in method layer, then the\n"
-		"attribute in the result feature will get the value from the feature of\n"
-		"the method layer (even if it is undefined).\n"
-		"\n"
-		"For best performance use the minimum amount of features in the method\n"
-		"layer and copy it into a memory layer.\n"
-		"\n"
-		"This method relies on GEOS support. Do not use unless the GEOS support\n"
-		"is compiled in.  The recognized list of options is :\n"
-		"SKIP_FAILURES=YES/NO. Set it to YES to go on, even when a feature\n"
-		"could not be inserted or a GEOS call failed.\n"
+		"For more details: :cpp:func:`OGR_L_SymDifference`\n"
 		"\n"
-		"PROMOTE_TO_MULTI=YES/NO. Set it to YES to convert Polygons into\n"
-		"MultiPolygons, or LineStrings to MultiLineStrings.\n"
-		"\n"
-		"INPUT_PREFIX=string. Set a prefix for the field names that will be\n"
-		"created from the fields of the input layer.\n"
-		"\n"
-		"METHOD_PREFIX=string. Set a prefix for the field names that will be\n"
-		"created from the fields of the method layer.\n"
-		"\n"
-		"This function is the same as the C++ method OGRLayer::SymDifference().\n"
-		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"method_layer: Layer\n"
+		"    the method layer. Should not be None.\n"
+		"result_layer: Layer\n"
+		"    the layer where the features resulting from the\n"
+		"    operation are inserted. Should not be None.\n"
+		"options: list[str], optional\n"
+		"    List of options (empty list is allowed). For example [\"PROMOTE_TO_MULTI=YES\"].\n"
+		"callback: Callable, optional\n"
+		"    a GDALProgressFunc() compatible callback function for\n"
+		"    reporting progress or None.\n"
+		"callback_data:\n"
+		"    Argument to be passed to 'callback'. May be None.\n"
+		"\n"
+		"Returns\n"
+		"-------\n"
+		"int:\n"
+		"    An error code if there was an error or the execution was interrupted,\n"
+		"    :py:const:`osgeo.ogr.OGRERR_NONE` otherwise.\n"
 		"\n"
-		"pLayerInput:  the input layer. Should not be NULL.\n"
-		"\n"
-		"pLayerMethod:  the method layer. Should not be NULL.\n"
-		"\n"
-		"pLayerResult:  the layer where the features resulting from the\n"
-		"operation are inserted. Should not be NULL. See above the note about\n"
-		"the schema.\n"
-		"\n"
-		"papszOptions:  NULL terminated list of options (may be NULL).\n"
-		"\n"
-		"pfnProgress:  a GDALProgressFunc() compatible callback function for\n"
-		"reporting progress or NULL.\n"
-		"\n"
-		"pProgressArg:  argument to be passed to pfnProgress. May be NULL.\n"
-		"\n"
-		"an error code if there was an error or the execution was interrupted,\n"
-		"OGRERR_NONE otherwise.\n"
-		"\n"
-		"The first geometry field is always used.\n"
-		"\n"
-		"OGR 1.10 \n"
 		""},
 	 { "Layer_Identity", (PyCFunction)(void(*)(void))_wrap_Layer_Identity, METH_VARARGS|METH_KEYWORDS, "\n"
 		"Layer_Identity(Layer self, Layer method_layer, Layer result_layer, char ** options=None, GDALProgressFunc callback=0, void * callback_data=None) -> OGRErr\n"
-		"OGRErr OGR_L_Identity(OGRLayerH\n"
-		"pLayerInput, OGRLayerH pLayerMethod, OGRLayerH pLayerResult, char\n"
-		"**papszOptions, GDALProgressFunc pfnProgress, void *pProgressArg)\n"
-		"\n"
-		"Identify the features of this layer with the ones from the identity\n"
-		"layer.\n"
-		"\n"
-		"The result layer contains features whose geometries represent areas\n"
-		"that are in the input layer. The features in the result layer have\n"
-		"attributes from both input and method layers. The schema of the result\n"
-		"layer can be set by the user or, if it is empty, is initialized to\n"
-		"contain all fields in input and method layers.\n"
-		"\n"
-		"If the schema of the result is set by user and contains fields that\n"
-		"have the same name as a field in input and in method layer, then the\n"
-		"attribute in the result feature will get the value from the feature of\n"
-		"the method layer (even if it is undefined).\n"
-		"\n"
-		"For best performance use the minimum amount of features in the method\n"
-		"layer and copy it into a memory layer.\n"
-		"\n"
-		"This method relies on GEOS support. Do not use unless the GEOS support\n"
-		"is compiled in.  The recognized list of options is :\n"
-		"SKIP_FAILURES=YES/NO. Set it to YES to go on, even when a feature\n"
-		"could not be inserted or a GEOS call failed.\n"
 		"\n"
-		"PROMOTE_TO_MULTI=YES/NO. Set it to YES to convert Polygons into\n"
-		"MultiPolygons, or LineStrings to MultiLineStrings.\n"
+		"Identify the features of this layer with the ones from the identity layer.\n"
 		"\n"
-		"INPUT_PREFIX=string. Set a prefix for the field names that will be\n"
-		"created from the fields of the input layer.\n"
+		"For more details: :cpp:func:`OGR_L_Identity`\n"
 		"\n"
-		"METHOD_PREFIX=string. Set a prefix for the field names that will be\n"
-		"created from the fields of the method layer.\n"
-		"\n"
-		"USE_PREPARED_GEOMETRIES=YES/NO. Set to NO to not use prepared\n"
-		"geometries to pretest intersection of features of method layer with\n"
-		"features of this layer.\n"
-		"\n"
-		"KEEP_LOWER_DIMENSION_GEOMETRIES=YES/NO. Set to NO to skip result\n"
-		"features with lower dimension geometry that would otherwise be added\n"
-		"to the result layer. The default is to add but only if the result\n"
-		"layer has an unknown geometry type.\n"
-		"\n"
-		"This function is the same as the C++ method OGRLayer::Identity().\n"
-		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"method_layer: Layer\n"
+		"    the method layer. Should not be None.\n"
+		"result_layer: Layer\n"
+		"    the layer where the features resulting from the\n"
+		"    operation are inserted. Should not be None.\n"
+		"options: list[str], optional\n"
+		"    List of options (empty list is allowed). For example [\"PROMOTE_TO_MULTI=YES\"].\n"
+		"callback: Callable, optional\n"
+		"    a GDALProgressFunc() compatible callback function for\n"
+		"    reporting progress or None.\n"
+		"callback_data:\n"
+		"    Argument to be passed to 'callback'. May be None.\n"
+		"\n"
+		"Returns\n"
+		"-------\n"
+		"int:\n"
+		"    An error code if there was an error or the execution was interrupted,\n"
+		"    :py:const:`osgeo.ogr.OGRERR_NONE` otherwise.\n"
 		"\n"
-		"pLayerInput:  the input layer. Should not be NULL.\n"
-		"\n"
-		"pLayerMethod:  the method layer. Should not be NULL.\n"
-		"\n"
-		"pLayerResult:  the layer where the features resulting from the\n"
-		"operation are inserted. Should not be NULL. See above the note about\n"
-		"the schema.\n"
-		"\n"
-		"papszOptions:  NULL terminated list of options (may be NULL).\n"
-		"\n"
-		"pfnProgress:  a GDALProgressFunc() compatible callback function for\n"
-		"reporting progress or NULL.\n"
-		"\n"
-		"pProgressArg:  argument to be passed to pfnProgress. May be NULL.\n"
-		"\n"
-		"an error code if there was an error or the execution was interrupted,\n"
-		"OGRERR_NONE otherwise.\n"
-		"\n"
-		"The first geometry field is always used.\n"
-		"\n"
-		"OGR 1.10 \n"
 		""},
 	 { "Layer_Update", (PyCFunction)(void(*)(void))_wrap_Layer_Update, METH_VARARGS|METH_KEYWORDS, "\n"
 		"Layer_Update(Layer self, Layer method_layer, Layer result_layer, char ** options=None, GDALProgressFunc callback=0, void * callback_data=None) -> OGRErr\n"
-		"OGRErr OGR_L_Update(OGRLayerH\n"
-		"pLayerInput, OGRLayerH pLayerMethod, OGRLayerH pLayerResult, char\n"
-		"**papszOptions, GDALProgressFunc pfnProgress, void *pProgressArg)\n"
 		"\n"
 		"Update this layer with features from the update layer.\n"
 		"\n"
-		"The result layer contains features whose geometries represent areas\n"
-		"that are either in the input layer or in the method layer. The\n"
-		"features in the result layer have areas of the features of the method\n"
-		"layer or those ares of the features of the input layer that are not\n"
-		"covered by the method layer. The features of the result layer get\n"
-		"their attributes from the input layer. The schema of the result layer\n"
-		"can be set by the user or, if it is empty, is initialized to contain\n"
-		"all fields in the input layer.\n"
-		"\n"
-		"If the schema of the result is set by user and contains fields that\n"
-		"have the same name as a field in the method layer, then the attribute\n"
-		"in the result feature the originates from the method layer will get\n"
-		"the value from the feature of the method layer.\n"
-		"\n"
-		"For best performance use the minimum amount of features in the method\n"
-		"layer and copy it into a memory layer.\n"
-		"\n"
-		"This method relies on GEOS support. Do not use unless the GEOS support\n"
-		"is compiled in.  The recognized list of options is :\n"
-		"SKIP_FAILURES=YES/NO. Set it to YES to go on, even when a feature\n"
-		"could not be inserted or a GEOS call failed.\n"
-		"\n"
-		"PROMOTE_TO_MULTI=YES/NO. Set it to YES to convert Polygons into\n"
-		"MultiPolygons, or LineStrings to MultiLineStrings.\n"
-		"\n"
-		"INPUT_PREFIX=string. Set a prefix for the field names that will be\n"
-		"created from the fields of the input layer.\n"
+		"For more details: :cpp:func:`OGR_L_Update`\n"
 		"\n"
-		"METHOD_PREFIX=string. Set a prefix for the field names that will be\n"
-		"created from the fields of the method layer.\n"
-		"\n"
-		"This function is the same as the C++ method OGRLayer::Update().\n"
-		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"method_layer: Layer\n"
+		"    the method layer. Should not be None.\n"
+		"result_layer: Layer\n"
+		"    the layer where the features resulting from the\n"
+		"    operation are inserted. Should not be None.\n"
+		"options: list[str], optional\n"
+		"    List of options (empty list is allowed). For example [\"PROMOTE_TO_MULTI=YES\"].\n"
+		"callback: Callable, optional\n"
+		"    a GDALProgressFunc() compatible callback function for\n"
+		"    reporting progress or None.\n"
+		"callback_data:\n"
+		"    Argument to be passed to 'callback'. May be None.\n"
+		"\n"
+		"Returns\n"
+		"-------\n"
+		"int:\n"
+		"    An error code if there was an error or the execution was interrupted,\n"
+		"    :py:const:`osgeo.ogr.OGRERR_NONE` otherwise.\n"
 		"\n"
-		"pLayerInput:  the input layer. Should not be NULL.\n"
-		"\n"
-		"pLayerMethod:  the method layer. Should not be NULL.\n"
-		"\n"
-		"pLayerResult:  the layer where the features resulting from the\n"
-		"operation are inserted. Should not be NULL. See above the note about\n"
-		"the schema.\n"
-		"\n"
-		"papszOptions:  NULL terminated list of options (may be NULL).\n"
-		"\n"
-		"pfnProgress:  a GDALProgressFunc() compatible callback function for\n"
-		"reporting progress or NULL.\n"
-		"\n"
-		"pProgressArg:  argument to be passed to pfnProgress. May be NULL.\n"
-		"\n"
-		"an error code if there was an error or the execution was interrupted,\n"
-		"OGRERR_NONE otherwise.\n"
-		"\n"
-		"The first geometry field is always used.\n"
-		"\n"
-		"OGR 1.10 \n"
 		""},
 	 { "Layer_Clip", (PyCFunction)(void(*)(void))_wrap_Layer_Clip, METH_VARARGS|METH_KEYWORDS, "\n"
 		"Layer_Clip(Layer self, Layer method_layer, Layer result_layer, char ** options=None, GDALProgressFunc callback=0, void * callback_data=None) -> OGRErr\n"
-		"OGRErr OGR_L_Clip(OGRLayerH pLayerInput,\n"
-		"OGRLayerH pLayerMethod, OGRLayerH pLayerResult, char **papszOptions,\n"
-		"GDALProgressFunc pfnProgress, void *pProgressArg)\n"
 		"\n"
 		"Clip off areas that are not covered by the method layer.\n"
 		"\n"
-		"The result layer contains features whose geometries represent areas\n"
-		"that are in the input layer and in the method layer. The features in\n"
-		"the result layer have the (possibly clipped) areas of features in the\n"
-		"input layer and the attributes from the same features. The schema of\n"
-		"the result layer can be set by the user or, if it is empty, is\n"
-		"initialized to contain all fields in the input layer.\n"
-		"\n"
-		"For best performance use the minimum amount of features in the method\n"
-		"layer and copy it into a memory layer.\n"
-		"\n"
-		"This method relies on GEOS support. Do not use unless the GEOS support\n"
-		"is compiled in.  The recognized list of options is :\n"
-		"SKIP_FAILURES=YES/NO. Set it to YES to go on, even when a feature\n"
-		"could not be inserted or a GEOS call failed.\n"
+		"For more details: :cpp:func:`OGR_L_Clip`\n"
 		"\n"
-		"PROMOTE_TO_MULTI=YES/NO. Set it to YES to convert Polygons into\n"
-		"MultiPolygons, or LineStrings to MultiLineStrings.\n"
-		"\n"
-		"INPUT_PREFIX=string. Set a prefix for the field names that will be\n"
-		"created from the fields of the input layer.\n"
-		"\n"
-		"METHOD_PREFIX=string. Set a prefix for the field names that will be\n"
-		"created from the fields of the method layer.\n"
-		"\n"
-		"This function is the same as the C++ method OGRLayer::Clip().\n"
-		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"method_layer: Layer\n"
+		"    the method layer. Should not be None.\n"
+		"result_layer: Layer\n"
+		"    the layer where the features resulting from the\n"
+		"    operation are inserted. Should not be None.\n"
+		"options: list[str], optional\n"
+		"    List of options (empty list is allowed). For example [\"PROMOTE_TO_MULTI=YES\"].\n"
+		"callback: Callable, optional\n"
+		"    a GDALProgressFunc() compatible callback function for\n"
+		"    reporting progress or None.\n"
+		"callback_data:\n"
+		"    Argument to be passed to 'callback'. May be None.\n"
+		"\n"
+		"Returns\n"
+		"-------\n"
+		"int:\n"
+		"    An error code if there was an error or the execution was interrupted,\n"
+		"    :py:const:`osgeo.ogr.OGRERR_NONE` otherwise.\n"
 		"\n"
-		"pLayerInput:  the input layer. Should not be NULL.\n"
-		"\n"
-		"pLayerMethod:  the method layer. Should not be NULL.\n"
-		"\n"
-		"pLayerResult:  the layer where the features resulting from the\n"
-		"operation are inserted. Should not be NULL. See above the note about\n"
-		"the schema.\n"
-		"\n"
-		"papszOptions:  NULL terminated list of options (may be NULL).\n"
-		"\n"
-		"pfnProgress:  a GDALProgressFunc() compatible callback function for\n"
-		"reporting progress or NULL.\n"
-		"\n"
-		"pProgressArg:  argument to be passed to pfnProgress. May be NULL.\n"
-		"\n"
-		"an error code if there was an error or the execution was interrupted,\n"
-		"OGRERR_NONE otherwise.\n"
-		"\n"
-		"The first geometry field is always used.\n"
-		"\n"
-		"OGR 1.10 \n"
 		""},
 	 { "Layer_Erase", (PyCFunction)(void(*)(void))_wrap_Layer_Erase, METH_VARARGS|METH_KEYWORDS, "\n"
 		"Layer_Erase(Layer self, Layer method_layer, Layer result_layer, char ** options=None, GDALProgressFunc callback=0, void * callback_data=None) -> OGRErr\n"
-		"OGRErr OGR_L_Erase(OGRLayerH\n"
-		"pLayerInput, OGRLayerH pLayerMethod, OGRLayerH pLayerResult, char\n"
-		"**papszOptions, GDALProgressFunc pfnProgress, void *pProgressArg)\n"
 		"\n"
 		"Remove areas that are covered by the method layer.\n"
 		"\n"
-		"The result layer contains features whose geometries represent areas\n"
-		"that are in the input layer but not in the method layer. The features\n"
-		"in the result layer have attributes from the input layer. The schema\n"
-		"of the result layer can be set by the user or, if it is empty, is\n"
-		"initialized to contain all fields in the input layer.\n"
-		"\n"
-		"For best performance use the minimum amount of features in the method\n"
-		"layer and copy it into a memory layer.\n"
-		"\n"
-		"This method relies on GEOS support. Do not use unless the GEOS support\n"
-		"is compiled in.  The recognized list of options is :\n"
-		"SKIP_FAILURES=YES/NO. Set it to YES to go on, even when a feature\n"
-		"could not be inserted or a GEOS call failed.\n"
-		"\n"
-		"PROMOTE_TO_MULTI=YES/NO. Set it to YES to convert Polygons into\n"
-		"MultiPolygons, or LineStrings to MultiLineStrings.\n"
-		"\n"
-		"INPUT_PREFIX=string. Set a prefix for the field names that will be\n"
-		"created from the fields of the input layer.\n"
-		"\n"
-		"METHOD_PREFIX=string. Set a prefix for the field names that will be\n"
-		"created from the fields of the method layer.\n"
-		"\n"
-		"This function is the same as the C++ method OGRLayer::Erase().\n"
+		"For more details: :cpp:func:`OGR_L_Erase`\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"method_layer: Layer\n"
+		"    the method layer. Should not be None.\n"
+		"result_layer: Layer\n"
+		"    the layer where the features resulting from the\n"
+		"    operation are inserted. Should not be None.\n"
+		"options: list[str], optional\n"
+		"    List of options (empty list is allowed). For example [\"PROMOTE_TO_MULTI=YES\"].\n"
+		"callback: Callable, optional\n"
+		"    a GDALProgressFunc() compatible callback function for\n"
+		"    reporting progress or None.\n"
+		"callback_data:\n"
+		"    Argument to be passed to 'callback'. May be None.\n"
+		"\n"
+		"Returns\n"
+		"-------\n"
+		"int:\n"
+		"    An error code if there was an error or the execution was interrupted,\n"
+		"    :py:const:`osgeo.ogr.OGRERR_NONE` otherwise.\n"
 		"\n"
-		"pLayerInput:  the input layer. Should not be NULL.\n"
-		"\n"
-		"pLayerMethod:  the method layer. Should not be NULL.\n"
-		"\n"
-		"pLayerResult:  the layer where the features resulting from the\n"
-		"operation are inserted. Should not be NULL. See above the note about\n"
-		"the schema.\n"
-		"\n"
-		"papszOptions:  NULL terminated list of options (may be NULL).\n"
-		"\n"
-		"pfnProgress:  a GDALProgressFunc() compatible callback function for\n"
-		"reporting progress or NULL.\n"
-		"\n"
-		"pProgressArg:  argument to be passed to pfnProgress. May be NULL.\n"
-		"\n"
-		"an error code if there was an error or the execution was interrupted,\n"
-		"OGRERR_NONE otherwise.\n"
-		"\n"
-		"The first geometry field is always used.\n"
-		"\n"
-		"OGR 1.10 \n"
 		""},
 	 { "Layer_GetStyleTable", _wrap_Layer_GetStyleTable, METH_O, "\n"
 		"Layer_GetStyleTable(Layer self) -> StyleTable\n"
-		"OGRStyleTableH\n"
-		"OGR_L_GetStyleTable(OGRLayerH hLayer)\n"
 		"\n"
-		"Get style table. \n"
+		"Get style table.\n"
+		"\n"
+		"For more details: :cpp:func:`OGR_L_GetStyleTable`\n"
+		"\n"
 		""},
 	 { "Layer_SetStyleTable", _wrap_Layer_SetStyleTable, METH_VARARGS, "\n"
 		"Layer_SetStyleTable(Layer self, StyleTable table)\n"
-		"void\n"
-		"OGR_L_SetStyleTable(OGRLayerH hLayer, OGRStyleTableH hStyleTable)\n"
 		"\n"
-		"Set style table. \n"
+		"Set style table.\n"
+		"\n"
+		"For more details: :cpp:func:`OGR_L_SetStyleTable`\n"
+		"\n"
+		""},
+	 { "Layer_GetArrowStream", _wrap_Layer_GetArrowStream, METH_VARARGS, "Layer_GetArrowStream(Layer self, char ** options=None) -> ArrowArrayStream"},
+	 { "Layer_GetGeometryTypes", (PyCFunction)(void(*)(void))_wrap_Layer_GetGeometryTypes, METH_VARARGS|METH_KEYWORDS, "\n"
+		"Layer_GetGeometryTypes(Layer self, int geom_field=0, int flags=0, GDALProgressFunc callback=0, void * callback_data=None)\n"
+		"\n"
+		"Get actual geometry types found in features.\n"
+		"\n"
+		"For more details: :cpp:func:`OGR_L_GetGeometryTypes`\n"
+		"\n"
+		"Parameters\n"
+		"-----------\n"
+		"geom_field: int, optional\n"
+		"    index of the geometry field\n"
+		"flags: int, optional\n"
+		"    0, or a combination of :py:const:`osgeo.ogr.GGT_COUNT_NOT_NEEDED`,\n"
+		"    :py:const:`osgeo.ogr.GGT_STOP_IF_MIXED` and\n"
+		"    :py:const:`osgeo.ogr.GGT_GEOMCOLLECTIONZ_TINZ`\n"
+		"callback: Callable, optional\n"
+		"    a GDALProgressFunc() compatible callback function for\n"
+		"    cancellation or None.\n"
+		"callback_data:\n"
+		"    Argument to be passed to 'callback'. May be None.\n"
+		"\n"
+		"Returns\n"
+		"-------\n"
+		"dict:\n"
+		"    A dictionary whose keys are :py:const:`osgeo.ogr.wkbXXXX` constants and\n"
+		"    values the corresponding number of geometries of that type in the layer.\n"
+		"\n"
 		""},
 	 { "Layer_swigregister", Layer_swigregister, METH_O, NULL},
 	 { "delete_Feature", _wrap_delete_Feature, METH_O, "delete_Feature(Feature self)"},
 	 { "new_Feature", (PyCFunction)(void(*)(void))_wrap_new_Feature, METH_VARARGS|METH_KEYWORDS, "new_Feature(FeatureDefn feature_def) -> Feature"},
 	 { "Feature_GetDefnRef", _wrap_Feature_GetDefnRef, METH_O, "\n"
 		"Feature_GetDefnRef(Feature self) -> FeatureDefn\n"
-		"OGRFeatureDefnH\n"
-		"OGR_F_GetDefnRef(OGRFeatureH hFeat)\n"
+		"\n"
+		"OGRFeatureDefnH OGR_F_GetDefnRef(OGRFeatureH hFeat)\n"
 		"\n"
 		"Fetch feature definition.\n"
 		"\n"
 		"This function is the same as the C++ method OGRFeature::GetDefnRef().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature to get the feature definition from.\n"
 		"\n"
-		"hFeat:  handle to the feature to get the feature definition from.\n"
+		"Returns\n"
+		"--------\n"
+		"OGRFeatureDefnH:\n"
+		"    a handle to the feature definition object on which feature depends.\n"
 		"\n"
-		"a handle to the feature definition object on which feature depends. \n"
 		""},
 	 { "Feature_SetGeometry", _wrap_Feature_SetGeometry, METH_VARARGS, "\n"
 		"Feature_SetGeometry(Feature self, Geometry geom) -> OGRErr\n"
-		"OGRErr\n"
-		"OGR_F_SetGeometry(OGRFeatureH hFeat, OGRGeometryH hGeom)\n"
+		"\n"
+		"OGRErr OGR_F_SetGeometry(OGRFeatureH hFeat, OGRGeometryH hGeom)\n"
 		"\n"
 		"Set feature geometry.\n"
 		"\n"
 		"This function updates the features geometry, and operate exactly as\n"
 		"SetGeometryDirectly(), except that this function does not assume\n"
 		"ownership of the passed geometry, but instead makes a copy of it.\n"
 		"\n"
@@ -32164,29 +32482,33 @@
 		"\n"
 		"This method has only an effect on the in-memory feature object. If\n"
 		"this object comes from a layer and the modifications must be\n"
 		"serialized back to the datasource, OGR_L_SetFeature() must be used\n"
 		"afterwards. Or if this is a new feature, OGR_L_CreateFeature() must be\n"
 		"used afterwards.\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature on which new geometry is applied to.\n"
+		"hGeom:\n"
+		"    handle to the new geometry to apply to feature.\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"OGRErr:\n"
+		"    OGRERR_NONE if successful, or OGR_UNSUPPORTED_GEOMETRY_TYPE if the\n"
+		"    geometry type is illegal for the OGRFeatureDefn (checking not yet\n"
+		"    implemented).\n"
 		"\n"
-		"hFeat:  handle to the feature on which new geometry is applied to.\n"
-		"\n"
-		"hGeom:  handle to the new geometry to apply to feature.\n"
-		"\n"
-		"OGRERR_NONE if successful, or OGR_UNSUPPORTED_GEOMETRY_TYPE if the\n"
-		"geometry type is illegal for the OGRFeatureDefn (checking not yet\n"
-		"implemented). \n"
 		""},
 	 { "Feature_SetGeometryDirectly", _wrap_Feature_SetGeometryDirectly, METH_VARARGS, "\n"
 		"Feature_SetGeometryDirectly(Feature self, Geometry geom) -> OGRErr\n"
-		"OGRErr\n"
-		"OGR_F_SetGeometryDirectly(OGRFeatureH hFeat, OGRGeometryH hGeom)\n"
+		"\n"
+		"OGRErr OGR_F_SetGeometryDirectly(OGRFeatureH hFeat, OGRGeometryH hGeom)\n"
 		"\n"
 		"Set feature geometry.\n"
 		"\n"
 		"This function updates the features geometry, and operate exactly as\n"
 		"SetGeometry(), except that this function assumes ownership of the\n"
 		"passed geometry (even in case of failure of that function).\n"
 		"\n"
@@ -32195,43 +32517,47 @@
 		"\n"
 		"This method has only an effect on the in-memory feature object. If\n"
 		"this object comes from a layer and the modifications must be\n"
 		"serialized back to the datasource, OGR_L_SetFeature() must be used\n"
 		"afterwards. Or if this is a new feature, OGR_L_CreateFeature() must be\n"
 		"used afterwards.\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature on which to apply the geometry.\n"
+		"hGeom:\n"
+		"    handle to the new geometry to apply to feature.\n"
 		"\n"
-		"hFeat:  handle to the feature on which to apply the geometry.\n"
 		"\n"
-		"hGeom:  handle to the new geometry to apply to feature.\n"
+		"Returns\n"
+		"--------\n"
+		"OGRErr:\n"
+		"    OGRERR_NONE if successful, or OGR_UNSUPPORTED_GEOMETRY_TYPE if the\n"
+		"    geometry type is illegal for the OGRFeatureDefn (checking not yet\n"
+		"    implemented).\n"
 		"\n"
-		"OGRERR_NONE if successful, or OGR_UNSUPPORTED_GEOMETRY_TYPE if the\n"
-		"geometry type is illegal for the OGRFeatureDefn (checking not yet\n"
-		"implemented). \n"
 		""},
 	 { "Feature_GetGeometryRef", _wrap_Feature_GetGeometryRef, METH_O, "\n"
 		"Feature_GetGeometryRef(Feature self) -> Geometry\n"
-		"OGRGeometryH\n"
-		"OGR_F_GetGeometryRef(OGRFeatureH hFeat)\n"
 		"\n"
-		"Fetch a handle to feature geometry.\n"
+		"Return the feature geometry\n"
 		"\n"
-		"This function is essentially the same as the C++ method\n"
-		"OGRFeature::GetGeometryRef() (the only difference is that this C\n"
-		"function honours OGRGetNonLinearGeometriesEnabledFlag())\n"
+		"The lifetime of the returned geometry is bound to the one of its belonging\n"
+		"feature.\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
+		"For more details: :cpp:func:`OGR_F_GetGeometryRef`\n"
 		"\n"
-		"hFeat:  handle to the feature to get geometry from.\n"
+		"The geometry() method is also available as an alias of GetGeometryRef()\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"Geometry:\n"
+		"    the geometry, or None.\n"
 		"\n"
-		"a handle to internal feature geometry. This object should not be\n"
-		"modified. \n"
 		""},
 	 { "Feature_SetGeomField", _wrap_Feature_SetGeomField, METH_VARARGS, "\n"
 		"Feature_SetGeomField(Feature self, int iField, Geometry geom) -> OGRErr\n"
 		"Feature_SetGeomField(Feature self, char const * field_name, Geometry geom) -> OGRErr\n"
 		"OGRErr\n"
 		"OGR_F_SetGeomField(OGRFeatureH hFeat, int iField, OGRGeometryH hGeom)\n"
 		"\n"
@@ -32239,604 +32565,701 @@
 		"\n"
 		"This function updates the features geometry, and operate exactly as\n"
 		"SetGeometryDirectly(), except that this function does not assume\n"
 		"ownership of the passed geometry, but instead makes a copy of it.\n"
 		"\n"
 		"This function is the same as the C++ OGRFeature::SetGeomField().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature on which new geometry is applied to.\n"
+		"iField:\n"
+		"    geometry field to set.\n"
+		"hGeom:\n"
+		"    handle to the new geometry to apply to feature.\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"OGRErr:\n"
+		"    OGRERR_NONE if successful, or OGR_UNSUPPORTED_GEOMETRY_TYPE if the\n"
+		"    geometry type is illegal for the OGRFeatureDefn (checking not yet\n"
+		"    implemented).\n"
 		"\n"
-		"hFeat:  handle to the feature on which new geometry is applied to.\n"
-		"\n"
-		"iField:  geometry field to set.\n"
-		"\n"
-		"hGeom:  handle to the new geometry to apply to feature.\n"
-		"\n"
-		"OGRERR_NONE if successful, or OGR_UNSUPPORTED_GEOMETRY_TYPE if the\n"
-		"geometry type is illegal for the OGRFeatureDefn (checking not yet\n"
-		"implemented). \n"
 		""},
 	 { "Feature_SetGeomFieldDirectly", _wrap_Feature_SetGeomFieldDirectly, METH_VARARGS, "\n"
 		"Feature_SetGeomFieldDirectly(Feature self, int iField, Geometry geom) -> OGRErr\n"
 		"Feature_SetGeomFieldDirectly(Feature self, char const * field_name, Geometry geom) -> OGRErr\n"
-		"OGRErr\n"
-		"OGR_F_SetGeomFieldDirectly(OGRFeatureH hFeat, int iField, OGRGeometryH\n"
-		"hGeom)\n"
+		"\n"
+		"OGRErr OGR_F_SetGeomFieldDirectly(OGRFeatureH hFeat, int iField, OGRGeometryH hGeom)\n"
 		"\n"
 		"Set feature geometry of a specified geometry field.\n"
 		"\n"
 		"This function updates the features geometry, and operate exactly as\n"
 		"SetGeomField(), except that this function assumes ownership of the\n"
 		"passed geometry (even in case of failure of that function).\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFeature::SetGeomFieldDirectly.\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
-		"\n"
-		"hFeat:  handle to the feature on which to apply the geometry.\n"
-		"\n"
-		"iField:  geometry field to set.\n"
-		"\n"
-		"hGeom:  handle to the new geometry to apply to feature.\n"
+		".. versionadded:: 1.11\n"
 		"\n"
-		"OGRERR_NONE if successful, or OGRERR_FAILURE if the index is invalid,\n"
-		"or OGR_UNSUPPORTED_GEOMETRY_TYPE if the geometry type is illegal for\n"
-		"the OGRFeatureDefn (checking not yet implemented).\n"
+		"Parameters\n"
+		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature on which to apply the geometry.\n"
+		"iField:\n"
+		"    geometry field to set.\n"
+		"hGeom:\n"
+		"    handle to the new geometry to apply to feature.\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"OGRErr:\n"
+		"    OGRERR_NONE if successful, or OGRERR_FAILURE if the index is invalid,\n"
+		"    or OGR_UNSUPPORTED_GEOMETRY_TYPE if the geometry type is illegal for\n"
+		"    the OGRFeatureDefn (checking not yet implemented).\n"
 		"\n"
-		"GDAL 1.11 \n"
 		""},
 	 { "Feature_GetGeomFieldRef", _wrap_Feature_GetGeomFieldRef, METH_VARARGS, "\n"
 		"Feature_GetGeomFieldRef(Feature self, int iField) -> Geometry\n"
 		"Feature_GetGeomFieldRef(Feature self, char const * field_name) -> Geometry\n"
 		"OGRGeometryH\n"
 		"OGR_F_GetGeomFieldRef(OGRFeatureH hFeat, int iField)\n"
 		"\n"
 		"Fetch a handle to feature geometry.\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFeature::GetGeomFieldRef().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
-		"\n"
-		"hFeat:  handle to the feature to get geometry from.\n"
-		"\n"
-		"iField:  geometry field to get.\n"
+		"hFeat:\n"
+		"    handle to the feature to get geometry from.\n"
+		"iField:\n"
+		"    geometry field to get.\n"
 		"\n"
 		"a handle to internal feature geometry. This object should not be\n"
 		"modified.\n"
 		"\n"
 		"GDAL 1.11 \n"
 		""},
 	 { "Feature_Clone", _wrap_Feature_Clone, METH_O, "\n"
 		"Feature_Clone(Feature self) -> Feature\n"
-		"OGRFeatureH OGR_F_Clone(OGRFeatureH\n"
-		"hFeat)\n"
+		"\n"
+		"OGRFeatureH OGR_F_Clone(OGRFeatureH hFeat)\n"
 		"\n"
 		"Duplicate feature.\n"
 		"\n"
 		"The newly created feature is owned by the caller, and will have its\n"
 		"own reference to the OGRFeatureDefn.\n"
 		"\n"
 		"This function is the same as the C++ method OGRFeature::Clone().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature to clone.\n"
 		"\n"
-		"hFeat:  handle to the feature to clone.\n"
+		"Returns\n"
+		"--------\n"
+		"OGRFeatureH:\n"
+		"    a handle to the new feature, exactly matching this feature.\n"
 		"\n"
-		"a handle to the new feature, exactly matching this feature. \n"
 		""},
 	 { "Feature_Equal", _wrap_Feature_Equal, METH_VARARGS, "\n"
 		"Feature_Equal(Feature self, Feature feature) -> bool\n"
 		"int OGR_F_Equal(OGRFeatureH hFeat,\n"
 		"OGRFeatureH hOtherFeat)\n"
 		"\n"
 		"Test if two features are the same.\n"
 		"\n"
 		"Two features are considered equal if the share them (handle equality)\n"
 		"same OGRFeatureDefn, have the same field values, and the same geometry\n"
 		"(as tested by OGR_G_Equal()) as well as the same feature id.\n"
 		"\n"
 		"This function is the same as the C++ method OGRFeature::Equal().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hFeat:\n"
+		"    handle to one of the feature.\n"
+		"hOtherFeat:\n"
+		"    handle to the other feature to test this one against.\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    TRUE if they are equal, otherwise FALSE.\n"
 		"\n"
-		"hFeat:  handle to one of the feature.\n"
-		"\n"
-		"hOtherFeat:  handle to the other feature to test this one against.\n"
-		"\n"
-		"TRUE if they are equal, otherwise FALSE. \n"
 		""},
 	 { "Feature_GetFieldCount", _wrap_Feature_GetFieldCount, METH_O, "\n"
 		"Feature_GetFieldCount(Feature self) -> int\n"
-		"int\n"
-		"OGR_F_GetFieldCount(OGRFeatureH hFeat)\n"
+		"\n"
+		"int OGR_F_GetFieldCount(OGRFeatureH hFeat)\n"
 		"\n"
 		"Fetch number of fields on this feature This will always be the same as\n"
 		"the field count for the OGRFeatureDefn.\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFeature::GetFieldCount().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature to get the fields count from.\n"
 		"\n"
-		"hFeat:  handle to the feature to get the fields count from.\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    count of fields.\n"
 		"\n"
-		"count of fields. \n"
 		""},
 	 { "Feature_GetFieldDefnRef", _wrap_Feature_GetFieldDefnRef, METH_VARARGS, "\n"
 		"Feature_GetFieldDefnRef(Feature self, int id) -> FieldDefn\n"
 		"Feature_GetFieldDefnRef(Feature self, char const * field_name) -> FieldDefn\n"
-		"OGRFieldDefnH\n"
-		"OGR_F_GetFieldDefnRef(OGRFeatureH hFeat, int i)\n"
+		"\n"
+		"OGRFieldDefnH OGR_F_GetFieldDefnRef(OGRFeatureH hFeat, int i)\n"
 		"\n"
 		"Fetch definition for this field.\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFeature::GetFieldDefnRef().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature on which the field is found.\n"
+		"i:\n"
+		"    the field to fetch, from 0 to GetFieldCount()-1.\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"OGRFieldDefnH:\n"
+		"    a handle to the field definition (from the OGRFeatureDefn). This is an\n"
+		"    internal reference, and should not be deleted or modified.\n"
 		"\n"
-		"hFeat:  handle to the feature on which the field is found.\n"
-		"\n"
-		"i:  the field to fetch, from 0 to GetFieldCount()-1.\n"
-		"\n"
-		"a handle to the field definition (from the OGRFeatureDefn). This is an\n"
-		"internal reference, and should not be deleted or modified. \n"
 		""},
 	 { "Feature_GetGeomFieldCount", _wrap_Feature_GetGeomFieldCount, METH_O, "\n"
 		"Feature_GetGeomFieldCount(Feature self) -> int\n"
-		"int\n"
-		"OGR_F_GetGeomFieldCount(OGRFeatureH hFeat)\n"
+		"\n"
+		"int OGR_F_GetGeomFieldCount(OGRFeatureH hFeat)\n"
 		"\n"
 		"Fetch number of geometry fields on this feature This will always be\n"
 		"the same as the geometry field count for the OGRFeatureDefn.\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFeature::GetGeomFieldCount().\n"
 		"\n"
-		"Parameters:\n"
+		".. versionadded:: 1.11\n"
+		"\n"
+		"Parameters\n"
 		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature to get the geometry fields count from.\n"
 		"\n"
-		"hFeat:  handle to the feature to get the geometry fields count from.\n"
 		"\n"
-		"count of geometry fields.\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    count of geometry fields.\n"
 		"\n"
-		"GDAL 1.11 \n"
 		""},
 	 { "Feature_GetGeomFieldDefnRef", _wrap_Feature_GetGeomFieldDefnRef, METH_VARARGS, "\n"
 		"Feature_GetGeomFieldDefnRef(Feature self, int id) -> GeomFieldDefn\n"
 		"Feature_GetGeomFieldDefnRef(Feature self, char const * field_name) -> GeomFieldDefn\n"
-		"OGRGeomFieldDefnH\n"
-		"OGR_F_GetGeomFieldDefnRef(OGRFeatureH hFeat, int i)\n"
+		"\n"
+		"OGRGeomFieldDefnH OGR_F_GetGeomFieldDefnRef(OGRFeatureH hFeat, int i)\n"
 		"\n"
 		"Fetch definition for this geometry field.\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFeature::GetGeomFieldDefnRef().\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
+		".. versionadded:: 1.11\n"
 		"\n"
-		"hFeat:  handle to the feature on which the field is found.\n"
+		"Parameters\n"
+		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature on which the field is found.\n"
+		"i:\n"
+		"    the field to fetch, from 0 to GetGeomFieldCount()-1.\n"
 		"\n"
-		"i:  the field to fetch, from 0 to GetGeomFieldCount()-1.\n"
 		"\n"
-		"a handle to the field definition (from the OGRFeatureDefn). This is an\n"
-		"internal reference, and should not be deleted or modified.\n"
+		"Returns\n"
+		"--------\n"
+		"OGRGeomFieldDefnH:\n"
+		"    a handle to the field definition (from the OGRFeatureDefn). This is an\n"
+		"    internal reference, and should not be deleted or modified.\n"
 		"\n"
-		"GDAL 1.11 \n"
 		""},
 	 { "Feature_GetFieldAsString", _wrap_Feature_GetFieldAsString, METH_VARARGS, "\n"
 		"Feature_GetFieldAsString(Feature self, int id) -> char const\n"
 		"Feature_GetFieldAsString(Feature self, char const * field_name) -> char const *\n"
-		"const char*\n"
-		"OGR_F_GetFieldAsString(OGRFeatureH hFeat, int iField)\n"
+		"\n"
+		"const char\\* OGR_F_GetFieldAsString(OGRFeatureH hFeat, int iField)\n"
 		"\n"
 		"Fetch field value as a string.\n"
 		"\n"
 		"OFTReal and OFTInteger fields will be translated to string using\n"
 		"sprintf(), but not necessarily using the established formatting rules.\n"
 		"Other field types, or errors will result in a return value of zero.\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFeature::GetFieldAsString().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature that owned the field.\n"
+		"iField:\n"
+		"    the field to fetch, from 0 to GetFieldCount()-1.\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"str:\n"
+		"    the field value. This string is internal, and should not be modified,\n"
+		"    or freed. Its lifetime may be very brief.\n"
 		"\n"
-		"hFeat:  handle to the feature that owned the field.\n"
-		"\n"
-		"iField:  the field to fetch, from 0 to GetFieldCount()-1.\n"
-		"\n"
-		"the field value. This string is internal, and should not be modified,\n"
-		"or freed. Its lifetime may be very brief. \n"
 		""},
 	 { "Feature_GetFieldAsInteger", _wrap_Feature_GetFieldAsInteger, METH_VARARGS, "\n"
 		"Feature_GetFieldAsInteger(Feature self, int id) -> int\n"
 		"Feature_GetFieldAsInteger(Feature self, char const * field_name) -> int\n"
-		"int\n"
-		"OGR_F_GetFieldAsInteger(OGRFeatureH hFeat, int iField)\n"
+		"\n"
+		"int OGR_F_GetFieldAsInteger(OGRFeatureH hFeat, int iField)\n"
 		"\n"
 		"Fetch field value as integer.\n"
 		"\n"
 		"OFTString features will be translated using atoi(). OFTReal fields\n"
 		"will be cast to integer. Other field types, or errors will result in a\n"
 		"return value of zero.\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFeature::GetFieldAsInteger().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature that owned the field.\n"
+		"iField:\n"
+		"    the field to fetch, from 0 to GetFieldCount()-1.\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    the field value.\n"
 		"\n"
-		"hFeat:  handle to the feature that owned the field.\n"
-		"\n"
-		"iField:  the field to fetch, from 0 to GetFieldCount()-1.\n"
-		"\n"
-		"the field value. \n"
 		""},
 	 { "Feature_GetFieldAsInteger64", _wrap_Feature_GetFieldAsInteger64, METH_VARARGS, "\n"
 		"Feature_GetFieldAsInteger64(Feature self, int id) -> GIntBig\n"
 		"Feature_GetFieldAsInteger64(Feature self, char const * field_name) -> GIntBig\n"
-		"GIntBig\n"
-		"OGR_F_GetFieldAsInteger64(OGRFeatureH hFeat, int iField)\n"
+		"\n"
+		"GIntBig OGR_F_GetFieldAsInteger64(OGRFeatureH hFeat, int iField)\n"
 		"\n"
 		"Fetch field value as integer 64 bit.\n"
 		"\n"
 		"OFTInteger are promoted to 64 bit. OFTString features will be\n"
 		"translated using CPLAtoGIntBig(). OFTReal fields will be cast to\n"
 		"integer. Other field types, or errors will result in a return value of\n"
 		"zero.\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFeature::GetFieldAsInteger64().\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
+		".. versionadded:: 2.0\n"
 		"\n"
-		"hFeat:  handle to the feature that owned the field.\n"
-		"\n"
-		"iField:  the field to fetch, from 0 to GetFieldCount()-1.\n"
-		"\n"
-		"the field value.\n"
+		"Parameters\n"
+		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature that owned the field.\n"
+		"iField:\n"
+		"    the field to fetch, from 0 to GetFieldCount()-1.\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    the field value.\n"
 		"\n"
-		"GDAL 2.0 \n"
 		""},
 	 { "Feature_GetFieldAsDouble", _wrap_Feature_GetFieldAsDouble, METH_VARARGS, "\n"
 		"Feature_GetFieldAsDouble(Feature self, int id) -> double\n"
 		"Feature_GetFieldAsDouble(Feature self, char const * field_name) -> double\n"
-		"double\n"
-		"OGR_F_GetFieldAsDouble(OGRFeatureH hFeat, int iField)\n"
+		"\n"
+		"double OGR_F_GetFieldAsDouble(OGRFeatureH hFeat, int iField)\n"
 		"\n"
 		"Fetch field value as a double.\n"
 		"\n"
 		"OFTString features will be translated using CPLAtof(). OFTInteger\n"
 		"fields will be cast to double. Other field types, or errors will\n"
 		"result in a return value of zero.\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFeature::GetFieldAsDouble().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature that owned the field.\n"
+		"iField:\n"
+		"    the field to fetch, from 0 to GetFieldCount()-1.\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"float:\n"
+		"    the field value.\n"
 		"\n"
-		"hFeat:  handle to the feature that owned the field.\n"
-		"\n"
-		"iField:  the field to fetch, from 0 to GetFieldCount()-1.\n"
-		"\n"
-		"the field value. \n"
 		""},
 	 { "Feature_GetFieldAsDateTime", _wrap_Feature_GetFieldAsDateTime, METH_VARARGS, "\n"
 		"Feature_GetFieldAsDateTime(Feature self, int id)\n"
 		"Feature_GetFieldAsDateTime(Feature self, char const * field_name)\n"
 		"int\n"
-		"OGR_F_GetFieldAsDateTime(OGRFeatureH hFeat, int iField, int *pnYear,\n"
-		"int *pnMonth, int *pnDay, int *pnHour, int *pnMinute, int *pnSecond,\n"
-		"int *pnTZFlag)\n"
+		"OGR_F_GetFieldAsDateTime(OGRFeatureH hFeat, int iField, int \\*pnYear,\n"
+		"int \\*pnMonth, int \\*pnDay, int \\*pnHour, int \\*pnMinute, int \\*pnSecond,\n"
+		"int \\*pnTZFlag)\n"
 		"\n"
 		"Fetch field value as date and time.\n"
 		"\n"
 		"Currently this method only works for OFTDate, OFTTime and OFTDateTime\n"
 		"fields.\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFeature::GetFieldAsDateTime().\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
-		"\n"
-		"hFeat:  handle to the feature that owned the field.\n"
-		"\n"
-		"iField:  the field to fetch, from 0 to GetFieldCount()-1.\n"
+		".. note:: Use OGR_F_GetFieldAsDateTimeEx() for second with millisecond accuracy.\n"
 		"\n"
-		"pnYear:  (including century)\n"
-		"\n"
-		"pnMonth:  (1-12)\n"
-		"\n"
-		"pnDay:  (1-31)\n"
-		"\n"
-		"pnHour:  (0-23)\n"
-		"\n"
-		"pnMinute:  (0-59)\n"
-		"\n"
-		"pnSecond:  (0-59)\n"
-		"\n"
-		"pnTZFlag:  (0=unknown, 1=localtime, 100=GMT, see data model for\n"
+		"Parameters\n"
+		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature that owned the field.\n"
+		"iField:\n"
+		"    the field to fetch, from 0 to GetFieldCount()-1.\n"
+		"pnYear:\n"
+		"    (including century)\n"
+		"pnMonth:\n"
+		"    (1-12)\n"
+		"pnDay:\n"
+		"    (1-31)\n"
+		"pnHour:\n"
+		"    (0-23)\n"
+		"pnMinute:\n"
+		"    (0-59)\n"
+		"pnSecond:\n"
+		"    (0-59)\n"
+		"pnTZFlag:\n"
+		"    (0=unknown, 1=localtime, 100=GMT, see data model for\n"
 		"details)\n"
 		"\n"
-		"TRUE on success or FALSE on failure.\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    TRUE on success or FALSE on failure.\n"
 		"\n"
-		"See:  Use OGR_F_GetFieldAsDateTimeEx() for second with millisecond\n"
-		"accuracy. \n"
 		""},
 	 { "Feature_GetFieldAsIntegerList", _wrap_Feature_GetFieldAsIntegerList, METH_VARARGS, "\n"
 		"Feature_GetFieldAsIntegerList(Feature self, int id)\n"
 		"Feature_GetFieldAsIntegerList(Feature self, char const * field_name)\n"
-		"const int*\n"
-		"OGR_F_GetFieldAsIntegerList(OGRFeatureH hFeat, int iField, int\n"
-		"*pnCount)\n"
+		"\n"
+		"const int\\* OGR_F_GetFieldAsIntegerList(OGRFeatureH hFeat, int iField, int\n"
+		"\\*pnCount)\n"
 		"\n"
 		"Fetch field value as a list of integers.\n"
 		"\n"
 		"Currently this function only works for OFTIntegerList fields.\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFeature::GetFieldAsIntegerList().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature that owned the field.\n"
+		"iField:\n"
+		"    the field to fetch, from 0 to GetFieldCount()-1.\n"
+		"pnCount:\n"
+		"    an integer to put the list count (number of integers) into.\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"list[int]:\n"
+		"    the field value. This list is internal, and should not be modified, or\n"
+		"    freed. Its lifetime may be very brief. If \\*pnCount is zero on return\n"
+		"    the returned pointer may be NULL or non-NULL.\n"
 		"\n"
-		"hFeat:  handle to the feature that owned the field.\n"
-		"\n"
-		"iField:  the field to fetch, from 0 to GetFieldCount()-1.\n"
-		"\n"
-		"pnCount:  an integer to put the list count (number of integers) into.\n"
-		"\n"
-		"the field value. This list is internal, and should not be modified, or\n"
-		"freed. Its lifetime may be very brief. If *pnCount is zero on return\n"
-		"the returned pointer may be NULL or non-NULL. \n"
 		""},
 	 { "Feature_GetFieldAsInteger64List", _wrap_Feature_GetFieldAsInteger64List, METH_VARARGS, "\n"
 		"Feature_GetFieldAsInteger64List(Feature self, int id)\n"
-		"const GIntBig*\n"
+		"const GIntBig\\*\n"
 		"OGR_F_GetFieldAsInteger64List(OGRFeatureH hFeat, int iField, int\n"
-		"*pnCount)\n"
+		"\\*pnCount)\n"
 		"\n"
 		"Fetch field value as a list of 64 bit integers.\n"
 		"\n"
 		"Currently this function only works for OFTInteger64List fields.\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFeature::GetFieldAsInteger64List().\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
+		".. versionadded:: 2.0\n"
 		"\n"
-		"hFeat:  handle to the feature that owned the field.\n"
-		"\n"
-		"iField:  the field to fetch, from 0 to GetFieldCount()-1.\n"
-		"\n"
-		"pnCount:  an integer to put the list count (number of integers) into.\n"
-		"\n"
-		"the field value. This list is internal, and should not be modified, or\n"
-		"freed. Its lifetime may be very brief. If *pnCount is zero on return\n"
-		"the returned pointer may be NULL or non-NULL.\n"
+		"Parameters\n"
+		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature that owned the field.\n"
+		"iField:\n"
+		"    the field to fetch, from 0 to GetFieldCount()-1.\n"
+		"pnCount:\n"
+		"    an integer to put the list count (number of integers) into.\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"list[int]:\n"
+		"    the field value. This list is internal, and should not be modified, or\n"
+		"    freed. Its lifetime may be very brief. If \\*pnCount is zero on return\n"
+		"    the returned pointer may be NULL or non-NULL.\n"
 		"\n"
-		"GDAL 2.0 \n"
 		""},
 	 { "Feature_GetFieldAsDoubleList", _wrap_Feature_GetFieldAsDoubleList, METH_VARARGS, "\n"
 		"Feature_GetFieldAsDoubleList(Feature self, int id)\n"
 		"Feature_GetFieldAsDoubleList(Feature self, char const * field_name)\n"
-		"const double*\n"
+		"const double\\*\n"
 		"OGR_F_GetFieldAsDoubleList(OGRFeatureH hFeat, int iField, int\n"
-		"*pnCount)\n"
+		"\\*pnCount)\n"
 		"\n"
 		"Fetch field value as a list of doubles.\n"
 		"\n"
 		"Currently this function only works for OFTRealList fields.\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFeature::GetFieldAsDoubleList().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature that owned the field.\n"
+		"iField:\n"
+		"    the field to fetch, from 0 to GetFieldCount()-1.\n"
+		"pnCount:\n"
+		"    an integer to put the list count (number of doubles) into.\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"list[float]:\n"
+		"    the field value. This list is internal, and should not be modified, or\n"
+		"    freed. Its lifetime may be very brief. If \\*pnCount is zero on return\n"
+		"    the returned pointer may be NULL or non-NULL.\n"
 		"\n"
-		"hFeat:  handle to the feature that owned the field.\n"
-		"\n"
-		"iField:  the field to fetch, from 0 to GetFieldCount()-1.\n"
-		"\n"
-		"pnCount:  an integer to put the list count (number of doubles) into.\n"
-		"\n"
-		"the field value. This list is internal, and should not be modified, or\n"
-		"freed. Its lifetime may be very brief. If *pnCount is zero on return\n"
-		"the returned pointer may be NULL or non-NULL. \n"
 		""},
 	 { "Feature_GetFieldAsStringList", _wrap_Feature_GetFieldAsStringList, METH_VARARGS, "\n"
 		"Feature_GetFieldAsStringList(Feature self, int id) -> char **\n"
-		"char**\n"
+		"char\\*\\*\n"
 		"OGR_F_GetFieldAsStringList(OGRFeatureH hFeat, int iField)\n"
 		"\n"
 		"Fetch field value as a list of strings.\n"
 		"\n"
 		"Currently this method only works for OFTStringList fields.\n"
 		"\n"
 		"The returned list is terminated by a NULL pointer. The number of\n"
 		"elements can also be calculated using CSLCount().\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFeature::GetFieldAsStringList().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature that owned the field.\n"
+		"iField:\n"
+		"    the field to fetch, from 0 to GetFieldCount()-1.\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"list[str]:\n"
+		"    the field value. This list is internal, and should not be modified, or\n"
+		"    freed. Its lifetime may be very brief.\n"
 		"\n"
-		"hFeat:  handle to the feature that owned the field.\n"
-		"\n"
-		"iField:  the field to fetch, from 0 to GetFieldCount()-1.\n"
-		"\n"
-		"the field value. This list is internal, and should not be modified, or\n"
-		"freed. Its lifetime may be very brief. \n"
 		""},
 	 { "Feature_GetFieldAsBinary", _wrap_Feature_GetFieldAsBinary, METH_VARARGS, "\n"
 		"Feature_GetFieldAsBinary(Feature self, int id) -> OGRErr\n"
 		"Feature_GetFieldAsBinary(Feature self, char const * field_name) -> OGRErr\n"
-		"GByte*\n"
-		"OGR_F_GetFieldAsBinary(OGRFeatureH hFeat, int iField, int *pnBytes)\n"
+		"GByte\\*\n"
+		"OGR_F_GetFieldAsBinary(OGRFeatureH hFeat, int iField, int \\*pnBytes)\n"
 		"\n"
 		"Fetch field value as binary.\n"
 		"\n"
 		"This method only works for OFTBinary and OFTString fields.\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFeature::GetFieldAsBinary().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature that owned the field.\n"
+		"iField:\n"
+		"    the field to fetch, from 0 to GetFieldCount()-1.\n"
+		"pnBytes:\n"
+		"    location to place count of bytes returned.\n"
 		"\n"
-		"hFeat:  handle to the feature that owned the field.\n"
-		"\n"
-		"iField:  the field to fetch, from 0 to GetFieldCount()-1.\n"
 		"\n"
-		"pnBytes:  location to place count of bytes returned.\n"
+		"Returns\n"
+		"--------\n"
+		"list:\n"
+		"    the field value. This list is internal, and should not be modified, or\n"
+		"    freed. Its lifetime may be very brief.\n"
 		"\n"
-		"the field value. This list is internal, and should not be modified, or\n"
-		"freed. Its lifetime may be very brief. \n"
 		""},
 	 { "Feature_IsFieldSet", _wrap_Feature_IsFieldSet, METH_VARARGS, "\n"
 		"Feature_IsFieldSet(Feature self, int id) -> bool\n"
 		"Feature_IsFieldSet(Feature self, char const * field_name) -> bool\n"
-		"int OGR_F_IsFieldSet(OGRFeatureH\n"
-		"hFeat, int iField)\n"
+		"\n"
+		"int OGR_F_IsFieldSet(OGRFeatureH hFeat, int iField)\n"
 		"\n"
 		"Test if a field has ever been assigned a value or not.\n"
 		"\n"
 		"This function is the same as the C++ method OGRFeature::IsFieldSet().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature on which the field is.\n"
+		"iField:\n"
+		"    the field to test.\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    TRUE if the field has been set, otherwise false.\n"
 		"\n"
-		"hFeat:  handle to the feature on which the field is.\n"
-		"\n"
-		"iField:  the field to test.\n"
-		"\n"
-		"TRUE if the field has been set, otherwise false. \n"
 		""},
 	 { "Feature_IsFieldNull", _wrap_Feature_IsFieldNull, METH_VARARGS, "\n"
 		"Feature_IsFieldNull(Feature self, int id) -> bool\n"
 		"Feature_IsFieldNull(Feature self, char const * field_name) -> bool\n"
-		"int OGR_F_IsFieldNull(OGRFeatureH\n"
-		"hFeat, int iField)\n"
+		"\n"
+		"int OGR_F_IsFieldNull(OGRFeatureH hFeat, int iField)\n"
 		"\n"
 		"Test if a field is null.\n"
 		"\n"
 		"This function is the same as the C++ method OGRFeature::IsFieldNull().\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
-		"\n"
-		"hFeat:  handle to the feature on which the field is.\n"
-		"\n"
-		"iField:  the field to test.\n"
+		".. versionadded:: 2.2\n"
 		"\n"
-		"TRUE if the field is null, otherwise false.\n"
+		"Parameters\n"
+		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature on which the field is.\n"
+		"iField:\n"
+		"    the field to test.\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    TRUE if the field is null, otherwise false.\n"
 		"\n"
-		"GDAL 2.2 \n"
 		""},
 	 { "Feature_IsFieldSetAndNotNull", _wrap_Feature_IsFieldSetAndNotNull, METH_VARARGS, "\n"
 		"Feature_IsFieldSetAndNotNull(Feature self, int id) -> bool\n"
 		"Feature_IsFieldSetAndNotNull(Feature self, char const * field_name) -> bool\n"
-		"int\n"
-		"OGR_F_IsFieldSetAndNotNull(OGRFeatureH hFeat, int iField)\n"
+		"\n"
+		"int OGR_F_IsFieldSetAndNotNull(OGRFeatureH hFeat, int iField)\n"
 		"\n"
 		"Test if a field is set and not null.\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFeature::IsFieldSetAndNotNull().\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
-		"\n"
-		"hFeat:  handle to the feature on which the field is.\n"
-		"\n"
-		"iField:  the field to test.\n"
+		".. versionadded:: 2.2\n"
 		"\n"
-		"TRUE if the field is set and not null, otherwise false.\n"
+		"Parameters\n"
+		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature on which the field is.\n"
+		"iField:\n"
+		"    the field to test.\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    TRUE if the field is set and not null, otherwise false.\n"
 		"\n"
-		"GDAL 2.2 \n"
 		""},
 	 { "Feature_GetFieldIndex", _wrap_Feature_GetFieldIndex, METH_VARARGS, "\n"
 		"Feature_GetFieldIndex(Feature self, char const * field_name) -> int\n"
-		"int\n"
-		"OGR_F_GetFieldIndex(OGRFeatureH hFeat, const char *pszName)\n"
+		"\n"
+		"int OGR_F_GetFieldIndex(OGRFeatureH hFeat, const char \\*pszName)\n"
 		"\n"
 		"Fetch the field index given field name.\n"
 		"\n"
 		"This is a cover for the OGRFeatureDefn::GetFieldIndex() method.\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFeature::GetFieldIndex().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature on which the field is found.\n"
+		"pszName:\n"
+		"    the name of the field to search for.\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    the field index, or -1 if no matching field is found.\n"
 		"\n"
-		"hFeat:  handle to the feature on which the field is found.\n"
-		"\n"
-		"pszName:  the name of the field to search for.\n"
-		"\n"
-		"the field index, or -1 if no matching field is found. \n"
 		""},
 	 { "Feature_GetGeomFieldIndex", _wrap_Feature_GetGeomFieldIndex, METH_VARARGS, "\n"
 		"Feature_GetGeomFieldIndex(Feature self, char const * field_name) -> int\n"
-		"int\n"
-		"OGR_F_GetGeomFieldIndex(OGRFeatureH hFeat, const char *pszName)\n"
+		"\n"
+		"int OGR_F_GetGeomFieldIndex(OGRFeatureH hFeat, const char \\*pszName)\n"
 		"\n"
 		"Fetch the geometry field index given geometry field name.\n"
 		"\n"
 		"This is a cover for the OGRFeatureDefn::GetGeomFieldIndex() method.\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFeature::GetGeomFieldIndex().\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
+		".. versionadded:: 1.11\n"
 		"\n"
-		"hFeat:  handle to the feature on which the geometry field is found.\n"
+		"Parameters\n"
+		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature on which the geometry field is found.\n"
+		"pszName:\n"
+		"    the name of the geometry field to search for.\n"
 		"\n"
-		"pszName:  the name of the geometry field to search for.\n"
 		"\n"
-		"the geometry field index, or -1 if no matching geometry field is\n"
-		"found.\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    the geometry field index, or -1 if no matching geometry field is found.\n"
 		"\n"
-		"GDAL 1.11 \n"
 		""},
 	 { "Feature_GetFID", _wrap_Feature_GetFID, METH_O, "\n"
 		"Feature_GetFID(Feature self) -> GIntBig\n"
 		"GIntBig OGR_F_GetFID(OGRFeatureH\n"
 		"hFeat)\n"
 		"\n"
 		"Get feature identifier.\n"
 		"\n"
 		"This function is the same as the C++ method OGRFeature::GetFID().\n"
 		"Note: since GDAL 2.0, this method returns a GIntBig (previously a\n"
 		"long)\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
-		"\n"
-		"hFeat:  handle to the feature from which to get the feature\n"
+		"hFeat:\n"
+		"    handle to the feature from which to get the feature\n"
 		"identifier.\n"
 		"\n"
-		"feature id or OGRNullFID if none has been assigned. \n"
+		"Returns\n"
+		"-------\n"
+		"int:\n"
+		"    feature id or OGRNullFID if none has been assigned.\n"
+		"\n"
 		""},
 	 { "Feature_SetFID", _wrap_Feature_SetFID, METH_VARARGS, "\n"
 		"Feature_SetFID(Feature self, GIntBig fid) -> OGRErr\n"
 		"OGRErr OGR_F_SetFID(OGRFeatureH hFeat,\n"
 		"GIntBig nFID)\n"
 		"\n"
 		"Set the feature identifier.\n"
@@ -32844,80 +33267,87 @@
 		"For specific types of features this operation may fail on illegal\n"
 		"features ids. Generally it always succeeds. Feature ids should be\n"
 		"greater than or equal to zero, with the exception of OGRNullFID (-1)\n"
 		"indicating that the feature id is unknown.\n"
 		"\n"
 		"This function is the same as the C++ method OGRFeature::SetFID().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature to set the feature id to.\n"
+		"nFID:\n"
+		"    the new feature identifier value to assign.\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"OGRErr:\n"
+		"    On success OGRERR_NONE, or on failure some other value.\n"
 		"\n"
-		"hFeat:  handle to the feature to set the feature id to.\n"
-		"\n"
-		"nFID:  the new feature identifier value to assign.\n"
-		"\n"
-		"On success OGRERR_NONE, or on failure some other value. \n"
 		""},
 	 { "Feature_DumpReadable", _wrap_Feature_DumpReadable, METH_O, "\n"
 		"Feature_DumpReadable(Feature self)\n"
 		"void\n"
-		"OGR_F_DumpReadable(OGRFeatureH hFeat, FILE *fpOut)\n"
+		"OGR_F_DumpReadable(OGRFeatureH hFeat, FILE \\*fpOut)\n"
 		"\n"
 		"Dump this feature in a human readable form.\n"
 		"\n"
 		"This dumps the attributes, and geometry; however, it doesn't\n"
 		"definition information (other than field types and names), nor does it\n"
 		"report the geometry spatial reference system.\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFeature::DumpReadable().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature to dump.\n"
+		"fpOut:\n"
+		"    the stream to write to, such as strout.\n"
 		"\n"
-		"hFeat:  handle to the feature to dump.\n"
-		"\n"
-		"fpOut:  the stream to write to, such as strout. \n"
 		""},
 	 { "Feature_UnsetField", _wrap_Feature_UnsetField, METH_VARARGS, "\n"
 		"Feature_UnsetField(Feature self, int id)\n"
 		"Feature_UnsetField(Feature self, char const * field_name)\n"
-		"void OGR_F_UnsetField(OGRFeatureH\n"
-		"hFeat, int iField)\n"
+		"\n"
+		"void OGR_F_UnsetField(OGRFeatureH hFeat, int iField)\n"
 		"\n"
 		"Clear a field, marking it as unset.\n"
 		"\n"
 		"This function is the same as the C++ method OGRFeature::UnsetField().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature on which the field is.\n"
+		"iField:\n"
+		"    the field to unset.\n"
 		"\n"
-		"hFeat:  handle to the feature on which the field is.\n"
-		"\n"
-		"iField:  the field to unset. \n"
 		""},
 	 { "Feature_SetFieldNull", _wrap_Feature_SetFieldNull, METH_VARARGS, "\n"
 		"Feature_SetFieldNull(Feature self, int id)\n"
 		"Feature_SetFieldNull(Feature self, char const * field_name)\n"
-		"void\n"
-		"OGR_F_SetFieldNull(OGRFeatureH hFeat, int iField)\n"
+		"\n"
+		"void OGR_F_SetFieldNull(OGRFeatureH hFeat, int iField)\n"
 		"\n"
 		"Clear a field, marking it as null.\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFeature::SetFieldNull().\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
-		"\n"
-		"hFeat:  handle to the feature on which the field is.\n"
+		".. versionadded:: 2.2\n"
 		"\n"
-		"iField:  the field to set to null.\n"
+		"Parameters\n"
+		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature on which the field is.\n"
+		"iField:\n"
+		"    the field to set to null.\n"
 		"\n"
-		"GDAL 2.2 \n"
 		""},
 	 { "Feature_SetFieldInteger64", _wrap_Feature_SetFieldInteger64, METH_VARARGS, "\n"
 		"Feature_SetFieldInteger64(Feature self, int id, GIntBig value)\n"
 		"void\n"
 		"OGR_F_SetFieldInteger64(OGRFeatureH hFeat, int iField, GIntBig nValue)\n"
 		"\n"
 		"Set field to 64 bit integer value.\n"
@@ -32931,124 +33361,128 @@
 		"\n"
 		"This method has only an effect on the in-memory feature object. If\n"
 		"this object comes from a layer and the modifications must be\n"
 		"serialized back to the datasource, OGR_L_SetFeature() must be used\n"
 		"afterwards. Or if this is a new feature, OGR_L_CreateFeature() must be\n"
 		"used afterwards.\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
-		"\n"
-		"hFeat:  handle to the feature that owned the field.\n"
-		"\n"
-		"iField:  the field to fetch, from 0 to GetFieldCount()-1.\n"
+		".. versionadded:: 2.0\n"
 		"\n"
-		"nValue:  the value to assign.\n"
+		"Parameters\n"
+		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature that owned the field.\n"
+		"iField:\n"
+		"    the field to fetch, from 0 to GetFieldCount()-1.\n"
+		"nValue:\n"
+		"    the value to assign.\n"
 		"\n"
-		"GDAL 2.0 \n"
 		""},
 	 { "Feature_SetField", _wrap_Feature_SetField, METH_VARARGS, "\n"
 		"Feature_SetField(Feature self, int id, char const * value)\n"
 		"Feature_SetField(Feature self, char const * field_name, char const * value)\n"
 		"Feature_SetField(Feature self, int id, double value)\n"
 		"Feature_SetField(Feature self, char const * field_name, double value)\n"
 		"Feature_SetField(Feature self, int id, int year, int month, int day, int hour, int minute, float second, int tzflag)\n"
 		"Feature_SetField(Feature self, char const * field_name, int year, int month, int day, int hour, int minute, float second, int tzflag)\n"
 		""},
 	 { "Feature_SetFieldIntegerList", _wrap_Feature_SetFieldIntegerList, METH_VARARGS, "\n"
 		"Feature_SetFieldIntegerList(Feature self, int id, int nList)\n"
 		"void\n"
 		"OGR_F_SetFieldIntegerList(OGRFeatureH hFeat, int iField, int nCount,\n"
-		"const int *panValues)\n"
+		"const int \\*panValues)\n"
 		"\n"
 		"Set field to list of integers value.\n"
 		"\n"
 		"This function currently on has an effect of OFTIntegerList,\n"
 		"OFTInteger64List and OFTRealList fields.\n"
 		"\n"
 		"This function is the same as the C++ method OGRFeature::SetField().\n"
 		"\n"
 		"This method has only an effect on the in-memory feature object. If\n"
 		"this object comes from a layer and the modifications must be\n"
 		"serialized back to the datasource, OGR_L_SetFeature() must be used\n"
 		"afterwards. Or if this is a new feature, OGR_L_CreateFeature() must be\n"
 		"used afterwards.\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature that owned the field.\n"
+		"iField:\n"
+		"    the field to set, from 0 to GetFieldCount()-1.\n"
+		"nCount:\n"
+		"    the number of values in the list being assigned.\n"
+		"panValues:\n"
+		"    the values to assign.\n"
 		"\n"
-		"hFeat:  handle to the feature that owned the field.\n"
-		"\n"
-		"iField:  the field to set, from 0 to GetFieldCount()-1.\n"
-		"\n"
-		"nCount:  the number of values in the list being assigned.\n"
-		"\n"
-		"panValues:  the values to assign. \n"
 		""},
 	 { "Feature_SetFieldInteger64List", _wrap_Feature_SetFieldInteger64List, METH_VARARGS, "\n"
 		"Feature_SetFieldInteger64List(Feature self, int id, int nList)\n"
 		"void\n"
 		"OGR_F_SetFieldInteger64List(OGRFeatureH hFeat, int iField, int nCount,\n"
-		"const GIntBig *panValues)\n"
+		"const GIntBig \\*panValues)\n"
 		"\n"
 		"Set field to list of 64 bit integers value.\n"
 		"\n"
 		"This function currently on has an effect of OFTIntegerList,\n"
 		"OFTInteger64List and OFTRealList fields.\n"
 		"\n"
 		"This function is the same as the C++ method OGRFeature::SetField().\n"
 		"\n"
 		"This method has only an effect on the in-memory feature object. If\n"
 		"this object comes from a layer and the modifications must be\n"
 		"serialized back to the datasource, OGR_L_SetFeature() must be used\n"
 		"afterwards. Or if this is a new feature, OGR_L_CreateFeature() must be\n"
 		"used afterwards.\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
-		"\n"
-		"hFeat:  handle to the feature that owned the field.\n"
-		"\n"
-		"iField:  the field to set, from 0 to GetFieldCount()-1.\n"
+		".. versionadded:: 2.0\n"
 		"\n"
-		"nCount:  the number of values in the list being assigned.\n"
-		"\n"
-		"panValues:  the values to assign.\n"
+		"Parameters\n"
+		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature that owned the field.\n"
+		"iField:\n"
+		"    the field to set, from 0 to GetFieldCount()-1.\n"
+		"nCount:\n"
+		"    the number of values in the list being assigned.\n"
+		"panValues:\n"
+		"    the values to assign.\n"
 		"\n"
-		"GDAL 2.0 \n"
 		""},
 	 { "Feature_SetFieldDoubleList", _wrap_Feature_SetFieldDoubleList, METH_VARARGS, "\n"
 		"Feature_SetFieldDoubleList(Feature self, int id, int nList)\n"
 		"void\n"
 		"OGR_F_SetFieldDoubleList(OGRFeatureH hFeat, int iField, int nCount,\n"
-		"const double *padfValues)\n"
+		"const double \\*padfValues)\n"
 		"\n"
 		"Set field to list of doubles value.\n"
 		"\n"
 		"This function currently on has an effect of OFTIntegerList,\n"
 		"OFTInteger64List, OFTRealList fields.\n"
 		"\n"
 		"This function is the same as the C++ method OGRFeature::SetField().\n"
 		"\n"
 		"This method has only an effect on the in-memory feature object. If\n"
 		"this object comes from a layer and the modifications must be\n"
 		"serialized back to the datasource, OGR_L_SetFeature() must be used\n"
 		"afterwards. Or if this is a new feature, OGR_L_CreateFeature() must be\n"
 		"used afterwards.\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature that owned the field.\n"
+		"iField:\n"
+		"    the field to set, from 0 to GetFieldCount()-1.\n"
+		"nCount:\n"
+		"    the number of values in the list being assigned.\n"
+		"padfValues:\n"
+		"    the values to assign.\n"
 		"\n"
-		"hFeat:  handle to the feature that owned the field.\n"
-		"\n"
-		"iField:  the field to set, from 0 to GetFieldCount()-1.\n"
-		"\n"
-		"nCount:  the number of values in the list being assigned.\n"
-		"\n"
-		"padfValues:  the values to assign. \n"
 		""},
 	 { "Feature_SetFieldStringList", _wrap_Feature_SetFieldStringList, METH_VARARGS, "\n"
 		"Feature_SetFieldStringList(Feature self, int id, char ** pList)\n"
 		"void\n"
 		"OGR_F_SetFieldStringList(OGRFeatureH hFeat, int iField, CSLConstList\n"
 		"papszValues)\n"
 		"\n"
@@ -33060,23 +33494,24 @@
 		"\n"
 		"This method has only an effect on the in-memory feature object. If\n"
 		"this object comes from a layer and the modifications must be\n"
 		"serialized back to the datasource, OGR_L_SetFeature() must be used\n"
 		"afterwards. Or if this is a new feature, OGR_L_CreateFeature() must be\n"
 		"used afterwards.\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature that owned the field.\n"
+		"iField:\n"
+		"    the field to set, from 0 to GetFieldCount()-1.\n"
+		"papszValues:\n"
+		"    the values to assign. List of NUL-terminated string,\n"
+		"ending with a NULL pointer.\n"
 		"\n"
-		"hFeat:  handle to the feature that owned the field.\n"
-		"\n"
-		"iField:  the field to set, from 0 to GetFieldCount()-1.\n"
-		"\n"
-		"papszValues:  the values to assign. List of NUL-terminated string,\n"
-		"ending with a NULL pointer. \n"
 		""},
 	 { "Feature_SetFieldBinaryFromHexString", _wrap_Feature_SetFieldBinaryFromHexString, METH_VARARGS, "\n"
 		"Feature_SetFieldBinaryFromHexString(Feature self, int id, char const * pszValue)\n"
 		"Feature_SetFieldBinaryFromHexString(Feature self, char const * field_name, char const * pszValue)\n"
 		""},
 	 { "Feature_SetFrom", (PyCFunction)(void(*)(void))_wrap_Feature_SetFrom, METH_VARARGS|METH_KEYWORDS, "\n"
 		"Feature_SetFrom(Feature self, Feature other, int forgiving=1) -> OGRErr\n"
@@ -33084,114 +33519,126 @@
 		"hFeat, OGRFeatureH hOtherFeat, int bForgiving)\n"
 		"\n"
 		"Set one feature from another.\n"
 		"\n"
 		"Overwrite the contents of this feature from the geometry and\n"
 		"attributes of another. The hOtherFeature does not need to have the\n"
 		"same OGRFeatureDefn. Field values are copied by corresponding field\n"
-		"names. Field types do not have to exactly match. OGR_F_SetField*()\n"
+		"names. Field types do not have to exactly match. OGR_F_SetField\\*()\n"
 		"function conversion rules will be applied as needed.\n"
 		"\n"
 		"This function is the same as the C++ method OGRFeature::SetFrom().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature to set to.\n"
+		"hOtherFeat:\n"
+		"    handle to the feature from which geometry, and field\n"
+		"    values will be copied.\n"
+		"bForgiving:\n"
+		"    TRUE if the operation should continue despite lacking\n"
+		"    output fields matching some of the source fields.\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"OGRErr:\n"
+		"    OGRERR_NONE if the operation succeeds, even if some values are not\n"
+		"    transferred, otherwise an error code.\n"
 		"\n"
-		"hFeat:  handle to the feature to set to.\n"
-		"\n"
-		"hOtherFeat:  handle to the feature from which geometry, and field\n"
-		"values will be copied.\n"
-		"\n"
-		"bForgiving:  TRUE if the operation should continue despite lacking\n"
-		"output fields matching some of the source fields.\n"
-		"\n"
-		"OGRERR_NONE if the operation succeeds, even if some values are not\n"
-		"transferred, otherwise an error code. \n"
 		""},
 	 { "Feature_SetFromWithMap", _wrap_Feature_SetFromWithMap, METH_VARARGS, "\n"
 		"Feature_SetFromWithMap(Feature self, Feature other, int forgiving, int nList) -> OGRErr\n"
 		"OGRErr\n"
 		"OGR_F_SetFromWithMap(OGRFeatureH hFeat, OGRFeatureH hOtherFeat, int\n"
-		"bForgiving, const int *panMap)\n"
+		"bForgiving, const int \\*panMap)\n"
 		"\n"
 		"Set one feature from another.\n"
 		"\n"
 		"Overwrite the contents of this feature from the geometry and\n"
 		"attributes of another. The hOtherFeature does not need to have the\n"
 		"same OGRFeatureDefn. Field values are copied according to the provided\n"
 		"indices map. Field types do not have to exactly match.\n"
-		"OGR_F_SetField*() function conversion rules will be applied as needed.\n"
+		"OGR_F_SetField\\*() function conversion rules will be applied as needed.\n"
 		"This is more efficient than OGR_F_SetFrom() in that this doesn't\n"
 		"lookup the fields by their names. Particularly useful when the field\n"
 		"names don't match.\n"
 		"\n"
 		"This function is the same as the C++ method OGRFeature::SetFrom().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature to set to.\n"
+		"hOtherFeat:\n"
+		"    handle to the feature from which geometry, and field\n"
+		"    values will be copied.\n"
+		"panMap:\n"
+		"    Array of the indices of the destination feature's fields\n"
+		"    stored at the corresponding index of the source feature's fields. A\n"
+		"    value of -1 should be used to ignore the source's field. The array\n"
+		"    should not be NULL and be as long as the number of fields in the\n"
+		"    source feature.\n"
+		"bForgiving:\n"
+		"    TRUE if the operation should continue despite lacking\n"
+		"    output fields matching some of the source fields.\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"OGRErr:\n"
+		"    OGRERR_NONE if the operation succeeds, even if some values are not\n"
+		"    transferred, otherwise an error code.\n"
 		"\n"
-		"hFeat:  handle to the feature to set to.\n"
-		"\n"
-		"hOtherFeat:  handle to the feature from which geometry, and field\n"
-		"values will be copied.\n"
-		"\n"
-		"panMap:  Array of the indices of the destination feature's fields\n"
-		"stored at the corresponding index of the source feature's fields. A\n"
-		"value of -1 should be used to ignore the source's field. The array\n"
-		"should not be NULL and be as long as the number of fields in the\n"
-		"source feature.\n"
-		"\n"
-		"bForgiving:  TRUE if the operation should continue despite lacking\n"
-		"output fields matching some of the source fields.\n"
-		"\n"
-		"OGRERR_NONE if the operation succeeds, even if some values are not\n"
-		"transferred, otherwise an error code. \n"
 		""},
 	 { "Feature_GetStyleString", _wrap_Feature_GetStyleString, METH_O, "\n"
 		"Feature_GetStyleString(Feature self) -> char const *\n"
-		"const char*\n"
+		"const char\\*\n"
 		"OGR_F_GetStyleString(OGRFeatureH hFeat)\n"
 		"\n"
 		"Fetch style string for this feature.\n"
 		"\n"
 		"Set the OGR Feature Style Specification for details on the format of\n"
 		"this string, and ogr_featurestyle.h for services available to parse\n"
 		"it.\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFeature::GetStyleString().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature to get the style from.\n"
 		"\n"
-		"hFeat:  handle to the feature to get the style from.\n"
+		"Returns\n"
+		"--------\n"
+		"str:\n"
+		"    a reference to a representation in string format, or NULL if there\n"
+		"    isn't one.\n"
 		"\n"
-		"a reference to a representation in string format, or NULL if there\n"
-		"isn't one. \n"
 		""},
 	 { "Feature_SetStyleString", _wrap_Feature_SetStyleString, METH_VARARGS, "\n"
 		"Feature_SetStyleString(Feature self, char const * the_string)\n"
 		"void\n"
-		"OGR_F_SetStyleString(OGRFeatureH hFeat, const char *pszStyle)\n"
+		"OGR_F_SetStyleString(OGRFeatureH hFeat, const char \\*pszStyle)\n"
 		"\n"
 		"Set feature style string.\n"
 		"\n"
 		"This method operate exactly as OGR_F_SetStyleStringDirectly() except\n"
 		"that it does not assume ownership of the passed string, but instead\n"
 		"makes a copy of it.\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFeature::SetStyleString().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
-		"\n"
-		"hFeat:  handle to the feature to set style to.\n"
-		"\n"
-		"pszStyle:  the style string to apply to this feature, cannot be NULL.\n"
+		"hFeat:\n"
+		"    handle to the feature to set style to.\n"
+		"pszStyle:\n"
+		"    the style string to apply to this feature, cannot be NULL.\n"
 		"\n"
 		""},
 	 { "Feature_GetFieldType", _wrap_Feature_GetFieldType, METH_VARARGS, "\n"
 		"Feature_GetFieldType(Feature self, int id) -> OGRFieldType\n"
 		"Feature_GetFieldType(Feature self, char const * field_name) -> OGRFieldType\n"
 		""},
 	 { "Feature_Validate", _wrap_Feature_Validate, METH_VARARGS, "\n"
@@ -33207,55 +33654,60 @@
 		"must be interpreted as the number of UTF-8 characters. Some drivers\n"
 		"might interpret the width as the number of bytes instead. So this test\n"
 		"is rather conservative (if it fails, then it will fail for all\n"
 		"interpretations).\n"
 		"\n"
 		"This function is the same as the C++ method OGRFeature::Validate().\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
-		"\n"
-		"hFeat:  handle to the feature to validate.\n"
+		".. versionadded:: 2.0\n"
 		"\n"
-		"nValidateFlags:  OGR_F_VAL_ALL or combination of OGR_F_VAL_NULL,\n"
-		"OGR_F_VAL_GEOM_TYPE, OGR_F_VAL_WIDTH and\n"
-		"OGR_F_VAL_ALLOW_NULL_WHEN_DEFAULT with '|' operator\n"
-		"\n"
-		"bEmitError:  TRUE if a CPLError() must be emitted when a check fails\n"
-		"\n"
-		"TRUE if all enabled validation tests pass.\n"
+		"Parameters\n"
+		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature to validate.\n"
+		"nValidateFlags:\n"
+		"    OGR_F_VAL_ALL or combination of OGR_F_VAL_NULL,\n"
+		"    OGR_F_VAL_GEOM_TYPE, OGR_F_VAL_WIDTH and\n"
+		"    OGR_F_VAL_ALLOW_NULL_WHEN_DEFAULT with '|' operator\n"
+		"bEmitError:\n"
+		"    TRUE if a CPLError() must be emitted when a check fails\n"
+		"\n"
+		"Returns\n"
+		"-------\n"
+		"int:\n"
+		"    TRUE if all enabled validation tests pass.\n"
 		"\n"
-		"GDAL 2.0 \n"
 		""},
 	 { "Feature_FillUnsetWithDefault", _wrap_Feature_FillUnsetWithDefault, METH_VARARGS, "\n"
 		"Feature_FillUnsetWithDefault(Feature self, int bNotNullableOnly=FALSE, char ** options=None)\n"
 		"void\n"
 		"OGR_F_FillUnsetWithDefault(OGRFeatureH hFeat, int bNotNullableOnly,\n"
-		"char **papszOptions)\n"
+		"char \\*\\*papszOptions)\n"
 		"\n"
 		"Fill unset fields with default values that might be defined.\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFeature::FillUnsetWithDefault().\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
-		"\n"
-		"hFeat:  handle to the feature.\n"
+		".. versionadded:: 2.0\n"
 		"\n"
-		"bNotNullableOnly:  if we should fill only unset fields with a not-null\n"
-		"constraint.\n"
-		"\n"
-		"papszOptions:  unused currently. Must be set to NULL.\n"
+		"Parameters\n"
+		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature.\n"
+		"bNotNullableOnly:\n"
+		"    if we should fill only unset fields with a not-null\n"
+		"    constraint.\n"
+		"papszOptions:\n"
+		"    unused currently. Must be set to NULL.\n"
 		"\n"
-		"GDAL 2.0 \n"
 		""},
 	 { "Feature_GetNativeData", _wrap_Feature_GetNativeData, METH_O, "\n"
 		"Feature_GetNativeData(Feature self) -> char const *\n"
-		"const char*\n"
+		"const char\\*\n"
 		"OGR_F_GetNativeData(OGRFeatureH hFeat)\n"
 		"\n"
 		"Returns the native data for the feature.\n"
 		"\n"
 		"The native data is the representation in a \"natural\" form that comes\n"
 		"from the driver that created this feature, or that is aimed at an\n"
 		"output driver. The native data may be in different format, which is\n"
@@ -33270,119 +33722,121 @@
 		"may be useful in round-tripping scenarios where some characteristics\n"
 		"of the underlying format are not captured otherwise by the OGR\n"
 		"abstraction.\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFeature::GetNativeData().\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
-		"\n"
-		"hFeat:  handle to the feature.\n"
+		".. note:: See https://trac.osgeo.org/gdal/wiki/rfc60_improved_roundtripping_in_ogr\n"
 		"\n"
-		"a string with the native data, or NULL if there is none.\n"
+		".. versionadded:: 2.1\n"
 		"\n"
-		"GDAL 2.1\n"
+		"Parameters\n"
+		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature.\n"
 		"\n"
-		"See:\n"
-		"https://trac.osgeo.org/gdal/wiki/rfc60_improved_roundtripping_in_ogr\n"
+		"Returns\n"
+		"-------\n"
+		"str:\n"
+		"    a string with the native data, or NULL if there is none.\n"
 		"\n"
 		""},
 	 { "Feature_GetNativeMediaType", _wrap_Feature_GetNativeMediaType, METH_O, "\n"
 		"Feature_GetNativeMediaType(Feature self) -> char const *\n"
-		"const char*\n"
+		"const char\\*\n"
 		"OGR_F_GetNativeMediaType(OGRFeatureH hFeat)\n"
 		"\n"
 		"Returns the native media type for the feature.\n"
 		"\n"
 		"The native media type is the identifier for the format of the native\n"
 		"data. It follows the IANA RFC 2045\n"
 		"(seehttps://en.wikipedia.org/wiki/Media_type), e.g.\n"
 		"\"application/vnd.geo+json\" for JSon.\n"
 		"\n"
 		"This function is the same as the C function\n"
 		"OGR_F_GetNativeMediaType().\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
+		".. note:: See https://trac.osgeo.org/gdal/wiki/rfc60_improved_roundtripping_in_ogr\n"
 		"\n"
-		"hFeat:  handle to the feature.\n"
+		".. versionadded:: 2.1\n"
 		"\n"
-		"a string with the native media type, or NULL if there is none.\n"
+		"Parameters\n"
+		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature.\n"
 		"\n"
-		"GDAL 2.1\n"
 		"\n"
-		"See:\n"
-		"https://trac.osgeo.org/gdal/wiki/rfc60_improved_roundtripping_in_ogr\n"
+		"Returns\n"
+		"--------\n"
+		"str:\n"
+		"    a string with the native media type, or NULL if there is none.\n"
 		"\n"
 		""},
 	 { "Feature_SetNativeData", _wrap_Feature_SetNativeData, METH_VARARGS, "\n"
 		"Feature_SetNativeData(Feature self, char const * nativeData)\n"
 		"void\n"
-		"OGR_F_SetNativeData(OGRFeatureH hFeat, const char *pszNativeData)\n"
+		"OGR_F_SetNativeData(OGRFeatureH hFeat, const char \\*pszNativeData)\n"
 		"\n"
 		"Sets the native data for the feature.\n"
 		"\n"
 		"The native data is the representation in a \"natural\" form that comes\n"
 		"from the driver that created this feature, or that is aimed at an\n"
 		"output driver. The native data may be in different format, which is\n"
 		"indicated by OGR_F_GetNativeMediaType().\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFeature::SetNativeData().\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
-		"\n"
-		"hFeat:  handle to the feature.\n"
-		"\n"
-		"pszNativeData:  a string with the native data, or NULL if there is\n"
-		"none.\n"
+		".. note:: See https://trac.osgeo.org/gdal/wiki/rfc60_improved_roundtripping_in_ogr\n"
 		"\n"
-		"GDAL 2.1\n"
+		".. versionadded:: 2.1\n"
 		"\n"
-		"See:\n"
-		"https://trac.osgeo.org/gdal/wiki/rfc60_improved_roundtripping_in_ogr\n"
+		"Parameters\n"
+		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature.\n"
+		"pszNativeData:\n"
+		"    a string with the native data, or NULL if there is none.\n"
 		"\n"
 		""},
 	 { "Feature_SetNativeMediaType", _wrap_Feature_SetNativeMediaType, METH_VARARGS, "\n"
 		"Feature_SetNativeMediaType(Feature self, char const * nativeMediaType)\n"
 		"void\n"
 		"OGR_F_SetNativeMediaType(OGRFeatureH hFeat, const char\n"
-		"*pszNativeMediaType)\n"
+		"\\*pszNativeMediaType)\n"
 		"\n"
 		"Sets the native media type for the feature.\n"
 		"\n"
 		"The native media type is the identifier for the format of the native\n"
 		"data. It follows the IANA RFC 2045\n"
 		"(seehttps://en.wikipedia.org/wiki/Media_type), e.g.\n"
 		"\"application/vnd.geo+json\" for JSon.\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFeature::SetNativeMediaType().\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
-		"\n"
-		"hFeat:  handle to the feature.\n"
+		".. note:: See https://trac.osgeo.org/gdal/wiki/rfc60_improved_roundtripping_in_ogr\n"
 		"\n"
-		"pszNativeMediaType:  a string with the native media type, or NULL if\n"
-		"there is none.\n"
+		".. versionadded:: 2.1\n"
 		"\n"
-		"GDAL 2.1\n"
 		"\n"
-		"See:\n"
-		"https://trac.osgeo.org/gdal/wiki/rfc60_improved_roundtripping_in_ogr\n"
+		"Parameters\n"
+		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature.\n"
+		"pszNativeMediaType:\n"
+		"    a string with the native media type, or NULL if there is none.\n"
 		"\n"
 		""},
 	 { "Feature_SetFieldString", _wrap_Feature_SetFieldString, METH_VARARGS, "\n"
 		"Feature_SetFieldString(Feature self, int id, char const * value)\n"
 		"void\n"
 		"OGR_F_SetFieldString(OGRFeatureH hFeat, int iField, const char\n"
-		"*pszValue)\n"
+		"\\*pszValue)\n"
 		"\n"
 		"Set field to string value.\n"
 		"\n"
 		"OFTInteger fields will be set based on an atoi() conversion of the\n"
 		"string. OFTInteger64 fields will be set based on an CPLAtoGIntBig()\n"
 		"conversion of the string. OFTReal fields will be set based on an\n"
 		"CPLAtof() conversion of the string. Other field types may be\n"
@@ -33392,103 +33846,117 @@
 		"\n"
 		"This method has only an effect on the in-memory feature object. If\n"
 		"this object comes from a layer and the modifications must be\n"
 		"serialized back to the datasource, OGR_L_SetFeature() must be used\n"
 		"afterwards. Or if this is a new feature, OGR_L_CreateFeature() must be\n"
 		"used afterwards.\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hFeat:\n"
+		"    handle to the feature that owned the field.\n"
+		"iField:\n"
+		"    the field to fetch, from 0 to GetFieldCount()-1.\n"
+		"pszValue:\n"
+		"    the value to assign.\n"
 		"\n"
-		"hFeat:  handle to the feature that owned the field.\n"
-		"\n"
-		"iField:  the field to fetch, from 0 to GetFieldCount()-1.\n"
-		"\n"
-		"pszValue:  the value to assign. \n"
 		""},
 	 { "Feature_swigregister", Feature_swigregister, METH_O, NULL},
 	 { "Feature_swiginit", Feature_swiginit, METH_VARARGS, NULL},
 	 { "delete_FeatureDefn", _wrap_delete_FeatureDefn, METH_O, "delete_FeatureDefn(FeatureDefn self)"},
 	 { "new_FeatureDefn", (PyCFunction)(void(*)(void))_wrap_new_FeatureDefn, METH_VARARGS|METH_KEYWORDS, "new_FeatureDefn(char const * name_null_ok=None) -> FeatureDefn"},
 	 { "FeatureDefn_GetName", _wrap_FeatureDefn_GetName, METH_O, "\n"
 		"FeatureDefn_GetName(FeatureDefn self) -> char const *\n"
-		"const char*\n"
+		"const char\\*\n"
 		"OGR_FD_GetName(OGRFeatureDefnH hDefn)\n"
 		"\n"
 		"Get name of the OGRFeatureDefn passed as an argument.\n"
 		"\n"
 		"This function is the same as the C++ method OGRFeatureDefn::GetName().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hDefn:\n"
+		"    handle to the feature definition to get the name from.\n"
 		"\n"
-		"hDefn:  handle to the feature definition to get the name from.\n"
-		"\n"
-		"the name. This name is internal and should not be modified, or freed.\n"
+		"Returns\n"
+		"--------\n"
+		"str:\n"
+		"    the name. This name is internal and should not be modified, or freed.\n"
 		"\n"
 		""},
 	 { "FeatureDefn_GetFieldCount", _wrap_FeatureDefn_GetFieldCount, METH_O, "\n"
 		"FeatureDefn_GetFieldCount(FeatureDefn self) -> int\n"
 		"int\n"
 		"OGR_FD_GetFieldCount(OGRFeatureDefnH hDefn)\n"
 		"\n"
 		"Fetch number of fields on the passed feature definition.\n"
 		"\n"
 		"This function is the same as the C++ OGRFeatureDefn::GetFieldCount().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hDefn:\n"
+		"    handle to the feature definition to get the fields count from.\n"
 		"\n"
-		"hDefn:  handle to the feature definition to get the fields count from.\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    count of fields.\n"
 		"\n"
-		"count of fields. \n"
 		""},
 	 { "FeatureDefn_GetFieldDefn", _wrap_FeatureDefn_GetFieldDefn, METH_VARARGS, "\n"
 		"FeatureDefn_GetFieldDefn(FeatureDefn self, int i) -> FieldDefn\n"
 		"OGRFieldDefnH\n"
 		"OGR_FD_GetFieldDefn(OGRFeatureDefnH hDefn, int iField)\n"
 		"\n"
 		"Fetch field definition of the passed feature definition.\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFeatureDefn::GetFieldDefn().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
-		"\n"
-		"hDefn:  handle to the feature definition to get the field definition\n"
-		"from.\n"
-		"\n"
-		"iField:  the field to fetch, between 0 and GetFieldCount()-1.\n"
-		"\n"
-		"a handle to an internal field definition object or NULL if invalid\n"
-		"index. This object should not be modified or freed by the application.\n"
+		"hDefn:\n"
+		"    handle to the feature definition to get the field definition from.\n"
+		"iField:\n"
+		"    the field to fetch, between 0 and GetFieldCount()-1.\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"OGRFieldDefnH:\n"
+		"    a handle to an internal field definition object or NULL if invalid\n"
+		"    index. This object should not be modified or freed by the application.\n"
 		"\n"
 		""},
 	 { "FeatureDefn_GetFieldIndex", _wrap_FeatureDefn_GetFieldIndex, METH_VARARGS, "\n"
 		"FeatureDefn_GetFieldIndex(FeatureDefn self, char const * field_name) -> int\n"
 		"int\n"
-		"OGR_FD_GetFieldIndex(OGRFeatureDefnH hDefn, const char *pszFieldName)\n"
+		"OGR_FD_GetFieldIndex(OGRFeatureDefnH hDefn, const char \\*pszFieldName)\n"
 		"\n"
 		"Find field by name.\n"
 		"\n"
 		"The field index of the first field matching the passed field name\n"
 		"(case insensitively) is returned.\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFeatureDefn::GetFieldIndex.\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hDefn:\n"
+		"    handle to the feature definition to get field index from.\n"
+		"pszFieldName:\n"
+		"    the field name to search for.\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    the field index, or -1 if no match found.\n"
 		"\n"
-		"hDefn:  handle to the feature definition to get field index from.\n"
-		"\n"
-		"pszFieldName:  the field name to search for.\n"
-		"\n"
-		"the field index, or -1 if no match found. \n"
 		""},
 	 { "FeatureDefn_AddFieldDefn", _wrap_FeatureDefn_AddFieldDefn, METH_VARARGS, "\n"
 		"FeatureDefn_AddFieldDefn(FeatureDefn self, FieldDefn defn)\n"
 		"void\n"
 		"OGR_FD_AddFieldDefn(OGRFeatureDefnH hDefn, OGRFieldDefnH hNewField)\n"
 		"\n"
 		"Add a new field definition to the passed feature definition.\n"
@@ -33499,87 +33967,97 @@
 		"This function should only be called while there are no OGRFeature\n"
 		"objects in existence based on this OGRFeatureDefn. The OGRFieldDefn\n"
 		"passed in is copied, and remains the responsibility of the caller.\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFeatureDefn::AddFieldDefn().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hDefn:\n"
+		"    handle to the feature definition to add the field definition to.\n"
+		"hNewField:\n"
+		"    handle to the new field definition.\n"
 		"\n"
-		"hDefn:  handle to the feature definition to add the field definition\n"
-		"to.\n"
-		"\n"
-		"hNewField:  handle to the new field definition. \n"
 		""},
 	 { "FeatureDefn_GetGeomFieldCount", _wrap_FeatureDefn_GetGeomFieldCount, METH_O, "\n"
 		"FeatureDefn_GetGeomFieldCount(FeatureDefn self) -> int\n"
 		"int\n"
 		"OGR_FD_GetGeomFieldCount(OGRFeatureDefnH hDefn)\n"
 		"\n"
 		"Fetch number of geometry fields on the passed feature definition.\n"
 		"\n"
 		"This function is the same as the C++\n"
 		"OGRFeatureDefn::GetGeomFieldCount().\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
+		".. versionadded:: 1.11\n"
 		"\n"
-		"hDefn:  handle to the feature definition to get the fields count from.\n"
+		"Parameters\n"
+		"-----------\n"
+		"hDefn:\n"
+		"    handle to the feature definition to get the fields count from.\n"
 		"\n"
-		"count of geometry fields.\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    count of geometry fields.\n"
 		"\n"
-		"GDAL 1.11 \n"
 		""},
 	 { "FeatureDefn_GetGeomFieldDefn", _wrap_FeatureDefn_GetGeomFieldDefn, METH_VARARGS, "\n"
 		"FeatureDefn_GetGeomFieldDefn(FeatureDefn self, int i) -> GeomFieldDefn\n"
 		"OGRGeomFieldDefnH\n"
 		"OGR_FD_GetGeomFieldDefn(OGRFeatureDefnH hDefn, int iGeomField)\n"
 		"\n"
 		"Fetch geometry field definition of the passed feature definition.\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFeatureDefn::GetGeomFieldDefn().\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
+		".. versionadded:: 1.11\n"
 		"\n"
-		"hDefn:  handle to the feature definition to get the field definition\n"
-		"from.\n"
-		"\n"
-		"iGeomField:  the geometry field to fetch, between 0 and\n"
-		"GetGeomFieldCount() - 1.\n"
-		"\n"
-		"a handle to an internal field definition object or NULL if invalid\n"
-		"index. This object should not be modified or freed by the application.\n"
+		"Parameters\n"
+		"-----------\n"
+		"hDefn:\n"
+		"    handle to the feature definition to get the field definition from.\n"
+		"iGeomField:\n"
+		"    the geometry field to fetch, between 0 and GetGeomFieldCount() - 1.\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"OGRGeomFieldDefnH:\n"
+		"    a handle to an internal field definition object or NULL if invalid\n"
+		"    index. This object should not be modified or freed by the application.\n"
 		"\n"
-		"GDAL 1.11 \n"
 		""},
 	 { "FeatureDefn_GetGeomFieldIndex", _wrap_FeatureDefn_GetGeomFieldIndex, METH_VARARGS, "\n"
 		"FeatureDefn_GetGeomFieldIndex(FeatureDefn self, char const * field_name) -> int\n"
 		"int\n"
 		"OGR_FD_GetGeomFieldIndex(OGRFeatureDefnH hDefn, const char\n"
-		"*pszGeomFieldName)\n"
+		"\\*pszGeomFieldName)\n"
 		"\n"
 		"Find geometry field by name.\n"
 		"\n"
 		"The geometry field index of the first geometry field matching the\n"
 		"passed field name (case insensitively) is returned.\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFeatureDefn::GetGeomFieldIndex.\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hDefn:\n"
+		"    handle to the feature definition to get field index from.\n"
+		"pszGeomFieldName:\n"
+		"    the geometry field name to search for.\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    the geometry field index, or -1 if no match found.\n"
 		"\n"
-		"hDefn:  handle to the feature definition to get field index from.\n"
-		"\n"
-		"pszGeomFieldName:  the geometry field name to search for.\n"
-		"\n"
-		"the geometry field index, or -1 if no match found. \n"
 		""},
 	 { "FeatureDefn_AddGeomFieldDefn", _wrap_FeatureDefn_AddGeomFieldDefn, METH_VARARGS, "\n"
 		"FeatureDefn_AddGeomFieldDefn(FeatureDefn self, GeomFieldDefn defn)\n"
 		"void\n"
 		"OGR_FD_AddGeomFieldDefn(OGRFeatureDefnH hDefn, OGRGeomFieldDefnH\n"
 		"hNewGeomField)\n"
 		"\n"
@@ -33592,23 +34070,24 @@
 		"objects in existence based on this OGRFeatureDefn. The\n"
 		"OGRGeomFieldDefn passed in is copied, and remains the responsibility\n"
 		"of the caller.\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFeatureDefn::AddGeomFieldDefn().\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
-		"\n"
-		"hDefn:  handle to the feature definition to add the geometry field\n"
-		"definition to.\n"
+		".. versionadded:: 1.11\n"
 		"\n"
-		"hNewGeomField:  handle to the new field definition.\n"
+		"Parameters\n"
+		"-----------\n"
+		"hDefn:\n"
+		"    handle to the feature definition to add the geometry field\n"
+		"    definition to.\n"
+		"hNewGeomField:\n"
+		"    handle to the new field definition.\n"
 		"\n"
-		"GDAL 1.11 \n"
 		""},
 	 { "FeatureDefn_DeleteGeomFieldDefn", _wrap_FeatureDefn_DeleteGeomFieldDefn, METH_VARARGS, "\n"
 		"FeatureDefn_DeleteGeomFieldDefn(FeatureDefn self, int idx) -> OGRErr\n"
 		"OGRErr\n"
 		"OGR_FD_DeleteGeomFieldDefn(OGRFeatureDefnH hDefn, int iGeomField)\n"
 		"\n"
 		"Delete an existing geometry field definition.\n"
@@ -33619,45 +34098,52 @@
 		"\n"
 		"This method should only be called while there are no OGRFeature\n"
 		"objects in existence based on this OGRFeatureDefn.\n"
 		"\n"
 		"This method is the same as the C++ method\n"
 		"OGRFeatureDefn::DeleteGeomFieldDefn().\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
-		"\n"
-		"hDefn:  handle to the feature definition.\n"
+		".. versionadded:: 1.11\n"
 		"\n"
-		"iGeomField:  the index of the geometry field definition.\n"
-		"\n"
-		"OGRERR_NONE in case of success.\n"
+		"Parameters\n"
+		"-----------\n"
+		"hDefn:\n"
+		"    handle to the feature definition.\n"
+		"iGeomField:\n"
+		"    the index of the geometry field definition.\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"OGRErr:\n"
+		"    OGRERR_NONE in case of success.\n"
 		"\n"
-		"GDAL 1.11 \n"
 		""},
 	 { "FeatureDefn_GetGeomType", _wrap_FeatureDefn_GetGeomType, METH_O, "\n"
 		"FeatureDefn_GetGeomType(FeatureDefn self) -> OGRwkbGeometryType\n"
 		"OGRwkbGeometryType\n"
 		"OGR_FD_GetGeomType(OGRFeatureDefnH hDefn)\n"
 		"\n"
 		"Fetch the geometry base type of the passed feature definition.\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFeatureDefn::GetGeomType().\n"
 		"\n"
 		"Starting with GDAL 1.11, this method returns\n"
 		"GetGeomFieldDefn(0)->GetType().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hDefn:\n"
+		"    handle to the feature definition to get the geometry type from.\n"
 		"\n"
-		"hDefn:  handle to the feature definition to get the geometry type\n"
-		"from.\n"
+		"Returns\n"
+		"--------\n"
+		"OGRwkbGeometryType:\n"
+		"    the base type for all geometry related to this definition.\n"
 		"\n"
-		"the base type for all geometry related to this definition. \n"
 		""},
 	 { "FeatureDefn_SetGeomType", _wrap_FeatureDefn_SetGeomType, METH_VARARGS, "\n"
 		"FeatureDefn_SetGeomType(FeatureDefn self, OGRwkbGeometryType geom_type)\n"
 		"void\n"
 		"OGR_FD_SetGeomType(OGRFeatureDefnH hDefn, OGRwkbGeometryType eType)\n"
 		"\n"
 		"Assign the base geometry type for the passed layer (the same as the\n"
@@ -33670,179 +34156,196 @@
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFeatureDefn::SetGeomType().\n"
 		"\n"
 		"Starting with GDAL 1.11, this method calls\n"
 		"GetGeomFieldDefn(0)->SetType().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hDefn:\n"
+		"    handle to the layer or feature definition to set the geometry type to.\n"
+		"eType:\n"
+		"    the new type to assign.\n"
 		"\n"
-		"hDefn:  handle to the layer or feature definition to set the geometry\n"
-		"type to.\n"
-		"\n"
-		"eType:  the new type to assign. \n"
 		""},
 	 { "FeatureDefn_GetReferenceCount", _wrap_FeatureDefn_GetReferenceCount, METH_O, "\n"
 		"FeatureDefn_GetReferenceCount(FeatureDefn self) -> int\n"
 		"int\n"
 		"OGR_FD_GetReferenceCount(OGRFeatureDefnH hDefn)\n"
 		"\n"
 		"Fetch current reference count.\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFeatureDefn::GetReferenceCount().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hDefn:\n"
+		"    handle to the feature definition on witch OGRFeature are based on.\n"
 		"\n"
-		"hDefn:  handle to the feature definition on witch OGRFeature are based\n"
-		"on.\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    the current reference count.\n"
 		"\n"
-		"the current reference count. \n"
 		""},
 	 { "FeatureDefn_IsGeometryIgnored", _wrap_FeatureDefn_IsGeometryIgnored, METH_O, "\n"
 		"FeatureDefn_IsGeometryIgnored(FeatureDefn self) -> int\n"
 		"int\n"
 		"OGR_FD_IsGeometryIgnored(OGRFeatureDefnH hDefn)\n"
 		"\n"
 		"Determine whether the geometry can be omitted when fetching features.\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFeatureDefn::IsGeometryIgnored().\n"
 		"\n"
 		"Starting with GDAL 1.11, this method returns\n"
 		"GetGeomFieldDefn(0)->IsIgnored().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hDefn:\n"
+		"    handle to the feature definition on witch OGRFeature are based on.\n"
 		"\n"
-		"hDefn:  handle to the feature definition on witch OGRFeature are based\n"
-		"on.\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    ignore state\n"
 		"\n"
-		"ignore state \n"
 		""},
 	 { "FeatureDefn_SetGeometryIgnored", _wrap_FeatureDefn_SetGeometryIgnored, METH_VARARGS, "\n"
 		"FeatureDefn_SetGeometryIgnored(FeatureDefn self, int bIgnored)\n"
 		"void\n"
 		"OGR_FD_SetGeometryIgnored(OGRFeatureDefnH hDefn, int bIgnore)\n"
 		"\n"
 		"Set whether the geometry can be omitted when fetching features.\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFeatureDefn::SetGeometryIgnored().\n"
 		"\n"
 		"Starting with GDAL 1.11, this method calls\n"
 		"GetGeomFieldDefn(0)->SetIgnored().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hDefn:\n"
+		"    handle to the feature definition on witch OGRFeature are based on.\n"
+		"bIgnore:\n"
+		"    ignore state\n"
 		"\n"
-		"hDefn:  handle to the feature definition on witch OGRFeature are based\n"
-		"on.\n"
-		"\n"
-		"bIgnore:  ignore state \n"
 		""},
 	 { "FeatureDefn_IsStyleIgnored", _wrap_FeatureDefn_IsStyleIgnored, METH_O, "\n"
 		"FeatureDefn_IsStyleIgnored(FeatureDefn self) -> int\n"
 		"int\n"
 		"OGR_FD_IsStyleIgnored(OGRFeatureDefnH hDefn)\n"
 		"\n"
 		"Determine whether the style can be omitted when fetching features.\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFeatureDefn::IsStyleIgnored().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hDefn:\n"
+		"    handle to the feature definition on which OGRFeature are based on.\n"
 		"\n"
-		"hDefn:  handle to the feature definition on which OGRFeature are based\n"
-		"on.\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    ignore state\n"
 		"\n"
-		"ignore state \n"
 		""},
 	 { "FeatureDefn_SetStyleIgnored", _wrap_FeatureDefn_SetStyleIgnored, METH_VARARGS, "\n"
 		"FeatureDefn_SetStyleIgnored(FeatureDefn self, int bIgnored)\n"
 		"void\n"
 		"OGR_FD_SetStyleIgnored(OGRFeatureDefnH hDefn, int bIgnore)\n"
 		"\n"
 		"Set whether the style can be omitted when fetching features.\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFeatureDefn::SetStyleIgnored().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hDefn:\n"
+		"    handle to the feature definition on witch OGRFeature are based on.\n"
+		"bIgnore:\n"
+		"    ignore state\n"
 		"\n"
-		"hDefn:  handle to the feature definition on witch OGRFeature are based\n"
-		"on.\n"
-		"\n"
-		"bIgnore:  ignore state \n"
 		""},
 	 { "FeatureDefn_IsSame", _wrap_FeatureDefn_IsSame, METH_VARARGS, "\n"
 		"FeatureDefn_IsSame(FeatureDefn self, FeatureDefn other_defn) -> int\n"
 		"int OGR_FD_IsSame(OGRFeatureDefnH\n"
 		"hFDefn, OGRFeatureDefnH hOtherFDefn)\n"
 		"\n"
 		"Test if the feature definition is identical to the other one.\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
-		"\n"
-		"hFDefn:  handle to the feature definition on witch OGRFeature are\n"
-		"based on.\n"
-		"\n"
-		"hOtherFDefn:  handle to the other feature definition to compare to.\n"
+		".. versionadded:: 1.11\n"
 		"\n"
-		"TRUE if the feature definition is identical to the other one.\n"
+		"Parameters\n"
+		"-----------\n"
+		"hFDefn:\n"
+		"    handle to the feature definition on witch OGRFeature are based on.\n"
+		"hOtherFDefn:\n"
+		"    handle to the other feature definition to compare to.\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    TRUE if the feature definition is identical to the other one.\n"
 		"\n"
-		"OGR 1.11 \n"
 		""},
 	 { "FeatureDefn_swigregister", FeatureDefn_swigregister, METH_O, NULL},
 	 { "FeatureDefn_swiginit", FeatureDefn_swiginit, METH_VARARGS, NULL},
 	 { "delete_FieldDefn", _wrap_delete_FieldDefn, METH_O, "delete_FieldDefn(FieldDefn self)"},
 	 { "new_FieldDefn", (PyCFunction)(void(*)(void))_wrap_new_FieldDefn, METH_VARARGS|METH_KEYWORDS, "new_FieldDefn(char const * name_null_ok=\"unnamed\", OGRFieldType field_type=OFTString) -> FieldDefn"},
 	 { "FieldDefn_GetName", _wrap_FieldDefn_GetName, METH_O, "FieldDefn_GetName(FieldDefn self) -> char const *"},
 	 { "FieldDefn_GetNameRef", _wrap_FieldDefn_GetNameRef, METH_O, "\n"
 		"FieldDefn_GetNameRef(FieldDefn self) -> char const *\n"
-		"const char*\n"
+		"const char\\*\n"
 		"OGR_Fld_GetNameRef(OGRFieldDefnH hDefn)\n"
 		"\n"
 		"Fetch name of this field.\n"
 		"\n"
 		"This function is the same as the CPP method\n"
 		"OGRFieldDefn::GetNameRef().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hDefn:\n"
+		"    handle to the field definition.\n"
 		"\n"
-		"hDefn:  handle to the field definition.\n"
+		"Returns\n"
+		"--------\n"
+		"str:\n"
+		"    the name of the field definition.\n"
 		"\n"
-		"the name of the field definition. \n"
 		""},
 	 { "FieldDefn_SetName", _wrap_FieldDefn_SetName, METH_VARARGS, "\n"
 		"FieldDefn_SetName(FieldDefn self, char const * name)\n"
 		"void OGR_Fld_SetName(OGRFieldDefnH\n"
-		"hDefn, const char *pszName)\n"
+		"hDefn, const char \\*pszName)\n"
 		"\n"
 		"Reset the name of this field.\n"
 		"\n"
 		"This function is the same as the CPP method OGRFieldDefn::SetName().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hDefn:\n"
+		"    handle to the field definition to apply the new name to.\n"
+		"pszName:\n"
+		"    the new name to apply.\n"
 		"\n"
-		"hDefn:  handle to the field definition to apply the new name to.\n"
-		"\n"
-		"pszName:  the new name to apply. \n"
 		""},
 	 { "FieldDefn_GetAlternativeName", _wrap_FieldDefn_GetAlternativeName, METH_O, "FieldDefn_GetAlternativeName(FieldDefn self) -> char const *"},
 	 { "FieldDefn_GetAlternativeNameRef", _wrap_FieldDefn_GetAlternativeNameRef, METH_O, "\n"
 		"FieldDefn_GetAlternativeNameRef(FieldDefn self) -> char const *\n"
-		"const char*\n"
+		"const char\\*\n"
 		"OGR_Fld_GetAlternativeNameRef(OGRFieldDefnH hDefn)\n"
 		"\n"
 		"Fetch the alternative name (or \"alias\") for this field.\n"
 		"\n"
 		"The alternative name is an optional attribute for a field which can\n"
 		"provide a more user-friendly, descriptive name of a field which is not\n"
 		"subject to the usual naming constraints defined by the data provider.\n"
@@ -33850,269 +34353,304 @@
 		"This is a metadata style attribute only: the alternative name cannot\n"
 		"be used in place of the actual field name during SQL queries or other\n"
 		"field name dependent API calls.\n"
 		"\n"
 		"This function is the same as the CPP method\n"
 		"OGRFieldDefn::GetAlternativeNameRef().\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
+		".. versionadded:: 3.2\n"
 		"\n"
-		"hDefn:  handle to the field definition.\n"
+		"Parameters\n"
+		"-----------\n"
+		"hDefn:\n"
+		"    handle to the field definition.\n"
 		"\n"
-		"the alternative name of the field definition.\n"
+		"Returns\n"
+		"--------\n"
+		"str:\n"
+		"    the alternative name of the field definition.\n"
 		"\n"
-		"GDAL 3.2 \n"
 		""},
 	 { "FieldDefn_SetAlternativeName", _wrap_FieldDefn_SetAlternativeName, METH_VARARGS, "\n"
 		"FieldDefn_SetAlternativeName(FieldDefn self, char const * alternativeName)\n"
 		"void\n"
 		"OGR_Fld_SetAlternativeName(OGRFieldDefnH hDefn, const char\n"
-		"*pszAlternativeName)\n"
+		"\\*pszAlternativeName)\n"
 		"\n"
 		"Reset the alternative name (or \"alias\") for this field.\n"
 		"\n"
 		"The alternative name is an optional attribute for a field which can\n"
 		"provide a more user-friendly, descriptive name of a field which is not\n"
 		"subject to the usual naming constraints defined by the data provider.\n"
 		"\n"
 		"This is a metadata style attribute only: the alternative name cannot\n"
 		"be used in place of the actual field name during SQL queries or other\n"
 		"field name dependent API calls.\n"
 		"\n"
 		"This function is the same as the CPP method\n"
 		"OGRFieldDefn::SetAlternativeName().\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
-		"\n"
-		"hDefn:  handle to the field definition to apply the new alternative\n"
-		"name to.\n"
+		".. versionadded:: 3.2\n"
 		"\n"
-		"pszAlternativeName:  the new alternative name to apply.\n"
+		"Parameters\n"
+		"-----------\n"
+		"hDefn:\n"
+		"    handle to the field definition to apply the new alternative name to.\n"
+		"pszAlternativeName:\n"
+		"    the new alternative name to apply.\n"
 		"\n"
-		"GDAL 3.2 \n"
 		""},
 	 { "FieldDefn_GetType", _wrap_FieldDefn_GetType, METH_O, "\n"
 		"FieldDefn_GetType(FieldDefn self) -> OGRFieldType\n"
 		"OGRFieldType\n"
 		"OGR_Fld_GetType(OGRFieldDefnH hDefn)\n"
 		"\n"
 		"Fetch type of this field.\n"
 		"\n"
 		"This function is the same as the CPP method OGRFieldDefn::GetType().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hDefn:\n"
+		"    handle to the field definition to get type from.\n"
 		"\n"
-		"hDefn:  handle to the field definition to get type from.\n"
+		"Returns\n"
+		"--------\n"
+		"OGRFieldType:\n"
+		"    field type.\n"
 		"\n"
-		"field type. \n"
 		""},
 	 { "FieldDefn_SetType", _wrap_FieldDefn_SetType, METH_VARARGS, "\n"
 		"FieldDefn_SetType(FieldDefn self, OGRFieldType type)\n"
 		"void OGR_Fld_SetType(OGRFieldDefnH\n"
 		"hDefn, OGRFieldType eType)\n"
 		"\n"
 		"Set the type of this field.\n"
 		"\n"
 		"This should never be done to an OGRFieldDefn that is already part of\n"
 		"an OGRFeatureDefn.\n"
 		"\n"
 		"This function is the same as the CPP method OGRFieldDefn::SetType().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hDefn:\n"
+		"    handle to the field definition to set type to.\n"
+		"eType:\n"
+		"    the new field type.\n"
 		"\n"
-		"hDefn:  handle to the field definition to set type to.\n"
-		"\n"
-		"eType:  the new field type. \n"
 		""},
 	 { "FieldDefn_GetSubType", _wrap_FieldDefn_GetSubType, METH_O, "\n"
 		"FieldDefn_GetSubType(FieldDefn self) -> OGRFieldSubType\n"
 		"OGRFieldSubType\n"
 		"OGR_Fld_GetSubType(OGRFieldDefnH hDefn)\n"
 		"\n"
 		"Fetch subtype of this field.\n"
 		"\n"
 		"This function is the same as the CPP method\n"
 		"OGRFieldDefn::GetSubType().\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
+		".. versionadded:: 2.0\n"
 		"\n"
-		"hDefn:  handle to the field definition to get subtype from.\n"
+		"Parameters\n"
+		"-----------\n"
+		"hDefn:\n"
+		"    handle to the field definition to get subtype from.\n"
 		"\n"
-		"field subtype.\n"
+		"Returns\n"
+		"--------\n"
+		"OGRFieldSubType:\n"
+		"    field subtype.\n"
 		"\n"
-		"GDAL 2.0 \n"
 		""},
 	 { "FieldDefn_SetSubType", _wrap_FieldDefn_SetSubType, METH_VARARGS, "\n"
 		"FieldDefn_SetSubType(FieldDefn self, OGRFieldSubType type)\n"
 		"void\n"
 		"OGR_Fld_SetSubType(OGRFieldDefnH hDefn, OGRFieldSubType eSubType)\n"
 		"\n"
 		"Set the subtype of this field.\n"
 		"\n"
 		"This should never be done to an OGRFieldDefn that is already part of\n"
 		"an OGRFeatureDefn.\n"
 		"\n"
 		"This function is the same as the CPP method\n"
 		"OGRFieldDefn::SetSubType().\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
-		"\n"
-		"hDefn:  handle to the field definition to set type to.\n"
+		".. versionadded:: 2.0\n"
 		"\n"
-		"eSubType:  the new field subtype.\n"
+		"Parameters\n"
+		"-----------\n"
+		"hDefn:\n"
+		"    handle to the field definition to set type to.\n"
+		"eSubType:\n"
+		"    the new field subtype.\n"
 		"\n"
-		"GDAL 2.0 \n"
 		""},
 	 { "FieldDefn_GetJustify", _wrap_FieldDefn_GetJustify, METH_O, "\n"
 		"FieldDefn_GetJustify(FieldDefn self) -> OGRJustification\n"
 		"OGRJustification\n"
 		"OGR_Fld_GetJustify(OGRFieldDefnH hDefn)\n"
 		"\n"
 		"Get the justification for this field.\n"
 		"\n"
 		"This function is the same as the CPP method\n"
 		"OGRFieldDefn::GetJustify().\n"
 		"\n"
 		"Note: no driver is know to use the concept of field justification.\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hDefn:\n"
+		"    handle to the field definition to get justification from.\n"
 		"\n"
-		"hDefn:  handle to the field definition to get justification from.\n"
+		"Returns\n"
+		"--------\n"
+		"OGRJustification:\n"
+		"    the justification.\n"
 		"\n"
-		"the justification. \n"
 		""},
 	 { "FieldDefn_SetJustify", _wrap_FieldDefn_SetJustify, METH_VARARGS, "\n"
 		"FieldDefn_SetJustify(FieldDefn self, OGRJustification justify)\n"
 		"void\n"
 		"OGR_Fld_SetJustify(OGRFieldDefnH hDefn, OGRJustification eJustify)\n"
 		"\n"
 		"Set the justification for this field.\n"
 		"\n"
 		"Note: no driver is know to use the concept of field justification.\n"
 		"\n"
 		"This function is the same as the CPP method\n"
 		"OGRFieldDefn::SetJustify().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hDefn:\n"
+		"    handle to the field definition to set justification to.\n"
+		"eJustify:\n"
+		"    the new justification.\n"
 		"\n"
-		"hDefn:  handle to the field definition to set justification to.\n"
-		"\n"
-		"eJustify:  the new justification. \n"
 		""},
 	 { "FieldDefn_GetWidth", _wrap_FieldDefn_GetWidth, METH_O, "\n"
 		"FieldDefn_GetWidth(FieldDefn self) -> int\n"
 		"int OGR_Fld_GetWidth(OGRFieldDefnH\n"
 		"hDefn)\n"
 		"\n"
 		"Get the formatting width for this field.\n"
 		"\n"
 		"This function is the same as the CPP method OGRFieldDefn::GetWidth().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hDefn:\n"
+		"    handle to the field definition to get width from.\n"
+		"\n"
 		"\n"
-		"hDefn:  handle to the field definition to get width from.\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    the width, zero means no specified width.\n"
 		"\n"
-		"the width, zero means no specified width. \n"
 		""},
 	 { "FieldDefn_SetWidth", _wrap_FieldDefn_SetWidth, METH_VARARGS, "\n"
 		"FieldDefn_SetWidth(FieldDefn self, int width)\n"
 		"void OGR_Fld_SetWidth(OGRFieldDefnH\n"
 		"hDefn, int nNewWidth)\n"
 		"\n"
 		"Set the formatting width for this field in characters.\n"
 		"\n"
 		"This function is the same as the CPP method OGRFieldDefn::SetWidth().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hDefn:\n"
+		"    handle to the field definition to set width to.\n"
+		"nNewWidth:\n"
+		"    the new width.\n"
 		"\n"
-		"hDefn:  handle to the field definition to set width to.\n"
-		"\n"
-		"nNewWidth:  the new width. \n"
 		""},
 	 { "FieldDefn_GetPrecision", _wrap_FieldDefn_GetPrecision, METH_O, "\n"
 		"FieldDefn_GetPrecision(FieldDefn self) -> int\n"
 		"int\n"
 		"OGR_Fld_GetPrecision(OGRFieldDefnH hDefn)\n"
 		"\n"
 		"Get the formatting precision for this field.\n"
 		"\n"
 		"This should normally be zero for fields of types other than OFTReal.\n"
 		"\n"
 		"This function is the same as the CPP method\n"
 		"OGRFieldDefn::GetPrecision().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hDefn:\n"
+		"    handle to the field definition to get precision from.\n"
 		"\n"
-		"hDefn:  handle to the field definition to get precision from.\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    the precision.\n"
 		"\n"
-		"the precision. \n"
 		""},
 	 { "FieldDefn_SetPrecision", _wrap_FieldDefn_SetPrecision, METH_VARARGS, "\n"
 		"FieldDefn_SetPrecision(FieldDefn self, int precision)\n"
 		"void\n"
 		"OGR_Fld_SetPrecision(OGRFieldDefnH hDefn, int nPrecision)\n"
 		"\n"
 		"Set the formatting precision for this field in characters.\n"
 		"\n"
 		"This should normally be zero for fields of types other than OFTReal.\n"
 		"\n"
 		"This function is the same as the CPP method\n"
 		"OGRFieldDefn::SetPrecision().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hDefn:\n"
+		"    handle to the field definition to set precision to.\n"
+		"nPrecision:\n"
+		"    the new precision.\n"
 		"\n"
-		"hDefn:  handle to the field definition to set precision to.\n"
-		"\n"
-		"nPrecision:  the new precision. \n"
 		""},
 	 { "FieldDefn_GetTypeName", _wrap_FieldDefn_GetTypeName, METH_O, "FieldDefn_GetTypeName(FieldDefn self) -> char const *"},
 	 { "FieldDefn_GetFieldTypeName", _wrap_FieldDefn_GetFieldTypeName, METH_VARARGS, "FieldDefn_GetFieldTypeName(FieldDefn self, OGRFieldType type) -> char const *"},
 	 { "FieldDefn_IsIgnored", _wrap_FieldDefn_IsIgnored, METH_O, "\n"
 		"FieldDefn_IsIgnored(FieldDefn self) -> int\n"
 		"int OGR_Fld_IsIgnored(OGRFieldDefnH\n"
 		"hDefn)\n"
 		"\n"
 		"Return whether this field should be omitted when fetching features.\n"
 		"\n"
 		"This method is the same as the C++ method OGRFieldDefn::IsIgnored().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hDefn:\n"
+		"    handle to the field definition\n"
 		"\n"
-		"hDefn:  handle to the field definition\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    ignore state\n"
 		"\n"
-		"ignore state \n"
 		""},
 	 { "FieldDefn_SetIgnored", _wrap_FieldDefn_SetIgnored, METH_VARARGS, "\n"
 		"FieldDefn_SetIgnored(FieldDefn self, int bIgnored)\n"
 		"void\n"
 		"OGR_Fld_SetIgnored(OGRFieldDefnH hDefn, int ignore)\n"
 		"\n"
 		"Set whether this field should be omitted when fetching features.\n"
 		"\n"
 		"This method is the same as the C++ method OGRFieldDefn::SetIgnored().\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"hDefn:\n"
+		"    handle to the field definition\n"
+		"ignore:\n"
+		"    ignore state\n"
 		"\n"
-		"hDefn:  handle to the field definition\n"
-		"\n"
-		"ignore:  ignore state \n"
 		""},
 	 { "FieldDefn_IsNullable", _wrap_FieldDefn_IsNullable, METH_O, "\n"
 		"FieldDefn_IsNullable(FieldDefn self) -> int\n"
 		"int\n"
 		"OGR_Fld_IsNullable(OGRFieldDefnH hDefn)\n"
 		"\n"
 		"Return whether this field can receive null values.\n"
@@ -34122,22 +34660,27 @@
 		"Even if this method returns FALSE (i.e not-nullable field), it doesn't\n"
 		"mean that OGRFeature::IsFieldSet() will necessary return TRUE, as\n"
 		"fields can be temporary unset and null/not-null validation is usually\n"
 		"done when OGRLayer::CreateFeature()/SetFeature() is called.\n"
 		"\n"
 		"This method is the same as the C++ method OGRFieldDefn::IsNullable().\n"
 		"\n"
-		"Parameters:\n"
+		".. versionadded:: 2.0\n"
+		"\n"
+		"Parameters\n"
 		"-----------\n"
+		"hDefn:\n"
+		"    handle to the field definition\n"
 		"\n"
-		"hDefn:  handle to the field definition\n"
 		"\n"
-		"TRUE if the field is authorized to be null.\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    TRUE if the field is authorized to be null.\n"
 		"\n"
-		"GDAL 2.0 \n"
 		""},
 	 { "FieldDefn_SetNullable", _wrap_FieldDefn_SetNullable, METH_VARARGS, "\n"
 		"FieldDefn_SetNullable(FieldDefn self, int bNullable)\n"
 		"void\n"
 		"OGR_Fld_SetNullable(OGRFieldDefnH hDefn, int bNullableIn)\n"
 		"\n"
 		"Set whether this field can receive null values.\n"
@@ -34146,42 +34689,48 @@
 		"with FALSE to set a not-null constraint.\n"
 		"\n"
 		"Drivers that support writing not-null constraint will advertise the\n"
 		"GDAL_DCAP_NOTNULL_FIELDS driver metadata item.\n"
 		"\n"
 		"This method is the same as the C++ method OGRFieldDefn::SetNullable().\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
-		"\n"
-		"hDefn:  handle to the field definition\n"
+		".. versionadded:: 2.0\n"
 		"\n"
-		"bNullableIn:  FALSE if the field must have a not-null constraint.\n"
+		"Parameters\n"
+		"-----------\n"
+		"hDefn:\n"
+		"    handle to the field definition\n"
+		"bNullableIn:\n"
+		"    FALSE if the field must have a not-null constraint.\n"
 		"\n"
-		"GDAL 2.0 \n"
 		""},
 	 { "FieldDefn_IsUnique", _wrap_FieldDefn_IsUnique, METH_O, "\n"
 		"FieldDefn_IsUnique(FieldDefn self) -> int\n"
 		"int OGR_Fld_IsUnique(OGRFieldDefnH\n"
 		"hDefn)\n"
 		"\n"
 		"Return whether this field has a unique constraint.\n"
 		"\n"
 		"By default, fields have no unique constraint.\n"
 		"\n"
 		"This method is the same as the C++ method OGRFieldDefn::IsUnique().\n"
 		"\n"
-		"Parameters:\n"
+		".. versionadded:: 3.2\n"
+		"\n"
+		"Parameters\n"
 		"-----------\n"
+		"hDefn:\n"
+		"    handle to the field definition\n"
 		"\n"
-		"hDefn:  handle to the field definition\n"
 		"\n"
-		"TRUE if the field has a unique constraint.\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    TRUE if the field has a unique constraint.\n"
 		"\n"
-		"GDAL 3.2 \n"
 		""},
 	 { "FieldDefn_SetUnique", _wrap_FieldDefn_SetUnique, METH_VARARGS, "\n"
 		"FieldDefn_SetUnique(FieldDefn self, int bUnique)\n"
 		"void\n"
 		"OGR_Fld_SetUnique(OGRFieldDefnH hDefn, int bUniqueIn)\n"
 		"\n"
 		"Set whether this field has a unique constraint.\n"
@@ -34191,46 +34740,51 @@
 		"\n"
 		"Drivers that support writing unique constraint will advertise the\n"
 		"GDAL_DCAP_UNIQUE_FIELDS driver metadata item. field can receive null\n"
 		"values.\n"
 		"\n"
 		"This method is the same as the C++ method OGRFieldDefn::SetUnique().\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
-		"\n"
-		"hDefn:  handle to the field definition\n"
+		".. versionadded:: 3.2\n"
 		"\n"
-		"bUniqueIn:  TRUE if the field must have a unique constraint.\n"
+		"Parameters\n"
+		"-----------\n"
+		"hDefn:\n"
+		"    handle to the field definition\n"
+		"bUniqueIn:\n"
+		"    TRUE if the field must have a unique constraint.\n"
 		"\n"
-		"GDAL 3.2 \n"
 		""},
 	 { "FieldDefn_GetDefault", _wrap_FieldDefn_GetDefault, METH_O, "\n"
 		"FieldDefn_GetDefault(FieldDefn self) -> char const *\n"
-		"const char*\n"
+		"const char\\*\n"
 		"OGR_Fld_GetDefault(OGRFieldDefnH hDefn)\n"
 		"\n"
 		"Get default field value.\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFieldDefn::GetDefault().\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
+		".. versionadded:: 2.0\n"
 		"\n"
-		"hDefn:  handle to the field definition.\n"
+		"Parameters\n"
+		"-----------\n"
+		"hDefn:\n"
+		"    handle to the field definition.\n"
 		"\n"
-		"default field value or NULL.\n"
+		"Returns\n"
+		"--------\n"
+		"str:\n"
+		"    default field value or NULL.\n"
 		"\n"
-		"GDAL 2.0 \n"
 		""},
 	 { "FieldDefn_SetDefault", _wrap_FieldDefn_SetDefault, METH_VARARGS, "\n"
 		"FieldDefn_SetDefault(FieldDefn self, char const * pszValue)\n"
 		"void\n"
-		"OGR_Fld_SetDefault(OGRFieldDefnH hDefn, const char *pszDefault)\n"
+		"OGR_Fld_SetDefault(OGRFieldDefnH hDefn, const char \\*pszDefault)\n"
 		"\n"
 		"Set default field value.\n"
 		"\n"
 		"The default field value is taken into account by drivers (generally\n"
 		"those with a SQL interface) that support it at field creation time.\n"
 		"OGR will generally not automatically set the default field value to\n"
 		"null fields by itself when calling OGRFeature::CreateFeature() /\n"
@@ -34247,22 +34801,23 @@
 		"\n"
 		"Drivers that support writing DEFAULT clauses will advertise the\n"
 		"GDAL_DCAP_DEFAULT_FIELDS driver metadata item.\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFieldDefn::SetDefault().\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
+		".. versionadded:: 2.0\n"
 		"\n"
-		"hDefn:  handle to the field definition.\n"
-		"\n"
-		"pszDefault:  new default field value or NULL pointer.\n"
+		"Parameters\n"
+		"-----------\n"
+		"hDefn:\n"
+		"    handle to the field definition.\n"
+		"pszDefault:\n"
+		"    new default field value or NULL pointer.\n"
 		"\n"
-		"GDAL 2.0 \n"
 		""},
 	 { "FieldDefn_IsDefaultDriverSpecific", _wrap_FieldDefn_IsDefaultDriverSpecific, METH_O, "\n"
 		"FieldDefn_IsDefaultDriverSpecific(FieldDefn self) -> int\n"
 		"int\n"
 		"OGR_Fld_IsDefaultDriverSpecific(OGRFieldDefnH hDefn)\n"
 		"\n"
 		"Returns whether the default value is driver specific.\n"
@@ -34271,67 +34826,77 @@
 		"value, a literal value enclosed between single quote characters,\n"
 		"CURRENT_TIMESTAMP, CURRENT_TIME, CURRENT_DATE or datetime literal\n"
 		"value.\n"
 		"\n"
 		"This function is the same as the C++ method\n"
 		"OGRFieldDefn::IsDefaultDriverSpecific().\n"
 		"\n"
-		"Parameters:\n"
+		".. versionadded:: 2.0\n"
+		"\n"
+		"Parameters\n"
 		"-----------\n"
+		"hDefn:\n"
+		"    handle to the field definition\n"
 		"\n"
-		"hDefn:  handle to the field definition\n"
 		"\n"
-		"TRUE if the default value is driver specific.\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    TRUE if the default value is driver specific.\n"
 		"\n"
-		"GDAL 2.0 \n"
 		""},
 	 { "FieldDefn_GetDomainName", _wrap_FieldDefn_GetDomainName, METH_O, "\n"
 		"FieldDefn_GetDomainName(FieldDefn self) -> char const *\n"
-		"const char*\n"
+		"const char\\*\n"
 		"OGR_Fld_GetDomainName(OGRFieldDefnH hDefn)\n"
 		"\n"
 		"Return the name of the field domain for this field.\n"
 		"\n"
 		"By default, none (empty string) is returned.\n"
 		"\n"
 		"Field domains ( OGRFieldDomain class) are attached at the GDALDataset\n"
 		"level and should be retrieved with GDALDatasetGetFieldDomain().\n"
 		"\n"
 		"This method is the same as the C++ method\n"
 		"OGRFieldDefn::GetDomainName().\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
+		".. versionadded:: 3.3\n"
 		"\n"
-		"hDefn:  handle to the field definition\n"
+		"Parameters\n"
+		"-----------\n"
+		"hDefn:\n"
+		"    handle to the field definition\n"
 		"\n"
-		"the field domain name, or an empty string if there is none.\n"
+		"Returns\n"
+		"--------\n"
+		"str:\n"
+		"    the field domain name, or an empty string if there is none.\n"
 		"\n"
-		"GDAL 3.3 \n"
 		""},
 	 { "FieldDefn_SetDomainName", _wrap_FieldDefn_SetDomainName, METH_VARARGS, "\n"
 		"FieldDefn_SetDomainName(FieldDefn self, char const * name)\n"
 		"void\n"
-		"OGR_Fld_SetDomainName(OGRFieldDefnH hDefn, const char *pszFieldName)\n"
+		"OGR_Fld_SetDomainName(OGRFieldDefnH hDefn, const char \\*pszFieldName)\n"
 		"\n"
 		"Set the name of the field domain for this field.\n"
 		"\n"
 		"Field domains ( OGRFieldDomain) are attached at the GDALDataset level.\n"
 		"\n"
 		"This method is the same as the C++ method\n"
 		"OGRFieldDefn::SetDomainName().\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
-		"\n"
-		"hDefn:  handle to the field definition\n"
+		".. versionadded:: 3.3\n"
 		"\n"
-		"pszFieldName:  Field domain name.\n"
+		"Parameters\n"
+		"-----------\n"
+		"hDefn:\n"
+		"    handle to the field definition\n"
+		"pszFieldName:\n"
+		"    Field domain name.\n"
 		"\n"
-		"GDAL 3.3 \n"
 		""},
 	 { "FieldDefn_swigregister", FieldDefn_swigregister, METH_O, NULL},
 	 { "FieldDefn_swiginit", FieldDefn_swiginit, METH_VARARGS, NULL},
 	 { "delete_GeomFieldDefn", _wrap_delete_GeomFieldDefn, METH_O, "delete_GeomFieldDefn(GeomFieldDefn self)"},
 	 { "new_GeomFieldDefn", (PyCFunction)(void(*)(void))_wrap_new_GeomFieldDefn, METH_VARARGS|METH_KEYWORDS, "new_GeomFieldDefn(char const * name_null_ok=\"\", OGRwkbGeometryType field_type=wkbUnknown) -> GeomFieldDefn"},
 	 { "GeomFieldDefn_GetName", _wrap_GeomFieldDefn_GetName, METH_O, "GeomFieldDefn_GetName(GeomFieldDefn self) -> char const *"},
 	 { "GeomFieldDefn_GetNameRef", _wrap_GeomFieldDefn_GetNameRef, METH_O, "GeomFieldDefn_GetNameRef(GeomFieldDefn self) -> char const *"},
@@ -34359,202 +34924,127 @@
 	 { "ForceToMultiPoint", _wrap_ForceToMultiPoint, METH_O, "ForceToMultiPoint(Geometry geom_in) -> Geometry"},
 	 { "ForceToMultiLineString", _wrap_ForceToMultiLineString, METH_O, "ForceToMultiLineString(Geometry geom_in) -> Geometry"},
 	 { "ForceTo", _wrap_ForceTo, METH_VARARGS, "ForceTo(Geometry geom_in, OGRwkbGeometryType eTargetType, char ** options=None) -> Geometry"},
 	 { "delete_Geometry", _wrap_delete_Geometry, METH_O, "delete_Geometry(Geometry self)"},
 	 { "new_Geometry", (PyCFunction)(void(*)(void))_wrap_new_Geometry, METH_VARARGS|METH_KEYWORDS, "new_Geometry(OGRwkbGeometryType type=wkbUnknown, char * wkt=None, int wkb=0, char * gml=None) -> Geometry"},
 	 { "Geometry_ExportToWkt", _wrap_Geometry_ExportToWkt, METH_O, "\n"
 		"Geometry_ExportToWkt(Geometry self) -> OGRErr\n"
-		"OGRErr\n"
-		"OGR_G_ExportToWkt(OGRGeometryH hGeom, char **ppszSrcText)\n"
 		"\n"
 		"Convert a geometry into well known text format.\n"
 		"\n"
-		"This function relates to the SFCOM IWks::ExportToWKT() method.\n"
+		"For more details: :cpp:func:`OGR_G_ExportToWkt`\n"
 		"\n"
-		"For backward compatibility purposes, it exports the Old-style 99-402\n"
-		"extended dimension (Z) WKB types for types Point, LineString, Polygon,\n"
-		"MultiPoint, MultiLineString, MultiPolygon and GeometryCollection. For\n"
-		"other geometry types, it is equivalent to OGR_G_ExportToIsoWkt().\n"
+		"Returns\n"
+		"--------\n"
+		"str\n"
 		"\n"
-		"This function is the same as the CPP method\n"
-		"OGRGeometry::exportToWkt().\n"
-		"\n"
-		"Parameters:\n"
-		"-----------\n"
-		"\n"
-		"hGeom:  handle on the geometry to convert to a text format from.\n"
-		"\n"
-		"ppszSrcText:  a text buffer is allocated by the program, and assigned\n"
-		"to the passed pointer. After use, *ppszDstText should be freed with\n"
-		"CPLFree().\n"
-		"\n"
-		"Currently OGRERR_NONE is always returned. \n"
 		""},
 	 { "Geometry_ExportToIsoWkt", _wrap_Geometry_ExportToIsoWkt, METH_O, "\n"
 		"Geometry_ExportToIsoWkt(Geometry self) -> OGRErr\n"
-		"OGRErr\n"
-		"OGR_G_ExportToIsoWkt(OGRGeometryH hGeom, char **ppszSrcText)\n"
 		"\n"
 		"Convert a geometry into SFSQL 1.2 / ISO SQL/MM Part 3 well known text\n"
 		"format.\n"
 		"\n"
-		"This function relates to the SFCOM IWks::ExportToWKT() method. It\n"
-		"exports the SFSQL 1.2 and ISO SQL/MM Part 3 extended dimension (Z&M)\n"
-		"WKB types.\n"
-		"\n"
-		"This function is the same as the CPP method\n"
-		"OGRGeometry::exportToWkt(wkbVariantIso).\n"
-		"\n"
-		"Parameters:\n"
-		"-----------\n"
-		"\n"
-		"hGeom:  handle on the geometry to convert to a text format from.\n"
+		"For more details: :cpp:func:`OGR_G_ExportToIsoWkt`\n"
 		"\n"
-		"ppszSrcText:  a text buffer is allocated by the program, and assigned\n"
-		"to the passed pointer. After use, *ppszDstText should be freed with\n"
-		"CPLFree().\n"
+		".. versionadded:: 2.0\n"
 		"\n"
-		"Currently OGRERR_NONE is always returned.\n"
+		"Returns\n"
+		"--------\n"
+		"str\n"
 		"\n"
-		"GDAL 2.0 \n"
 		""},
 	 { "Geometry_ExportToWkb", (PyCFunction)(void(*)(void))_wrap_Geometry_ExportToWkb, METH_VARARGS|METH_KEYWORDS, "\n"
 		"Geometry_ExportToWkb(Geometry self, OGRwkbByteOrder byte_order=wkbNDR) -> OGRErr\n"
-		"OGRErr\n"
-		"OGR_G_ExportToWkb(OGRGeometryH hGeom, OGRwkbByteOrder eOrder, unsigned\n"
-		"char *pabyDstBuffer)\n"
 		"\n"
 		"Convert a geometry well known binary format.\n"
 		"\n"
-		"This function relates to the SFCOM IWks::ExportToWKB() method.\n"
-		"\n"
-		"For backward compatibility purposes, it exports the Old-style 99-402\n"
-		"extended dimension (Z) WKB types for types Point, LineString, Polygon,\n"
-		"MultiPoint, MultiLineString, MultiPolygon and GeometryCollection. For\n"
-		"other geometry types, it is equivalent to OGR_G_ExportToIsoWkb().\n"
-		"\n"
-		"This function is the same as the CPP method\n"
-		"OGRGeometry::exportToWkb(OGRwkbByteOrder, unsigned char *,\n"
-		"OGRwkbVariant) with eWkbVariant = wkbVariantOldOgc.\n"
+		"For more details: :cpp:func:`OGR_G_ExportToWkb`\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"byte_order: osgeo.ogr.wkbXDR | osgeo.ogr.wkbNDR, default=osgeo.ogr.wkbNDR\n"
+		"    One of wkbXDR or wkbNDR indicating MSB or LSB byte order respectively.\n"
 		"\n"
-		"hGeom:  handle on the geometry to convert to a well know binary data\n"
-		"from.\n"
+		"Returns\n"
+		"--------\n"
+		"bytes\n"
 		"\n"
-		"eOrder:  One of wkbXDR or wkbNDR indicating MSB or LSB byte order\n"
-		"respectively.\n"
-		"\n"
-		"pabyDstBuffer:  a buffer into which the binary representation is\n"
-		"written. This buffer must be at least OGR_G_WkbSize() byte in size.\n"
-		"\n"
-		"Currently OGRERR_NONE is always returned. \n"
 		""},
 	 { "Geometry_ExportToIsoWkb", (PyCFunction)(void(*)(void))_wrap_Geometry_ExportToIsoWkb, METH_VARARGS|METH_KEYWORDS, "\n"
 		"Geometry_ExportToIsoWkb(Geometry self, OGRwkbByteOrder byte_order=wkbNDR) -> OGRErr\n"
-		"OGRErr\n"
-		"OGR_G_ExportToIsoWkb(OGRGeometryH hGeom, OGRwkbByteOrder eOrder,\n"
-		"unsigned char *pabyDstBuffer)\n"
 		"\n"
 		"Convert a geometry into SFSQL 1.2 / ISO SQL/MM Part 3 well known\n"
 		"binary format.\n"
 		"\n"
-		"This function relates to the SFCOM IWks::ExportToWKB() method. It\n"
-		"exports the SFSQL 1.2 and ISO SQL/MM Part 3 extended dimension (Z&M)\n"
-		"WKB types.\n"
+		"For more details: :cpp:func:`OGR_G_ExportToIsoWkb`\n"
 		"\n"
-		"This function is the same as the CPP method\n"
-		"OGRGeometry::exportToWkb(OGRwkbByteOrder, unsigned char *,\n"
-		"OGRwkbVariant) with eWkbVariant = wkbVariantIso.\n"
+		".. versionadded:: 2.0\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"byte_order: osgeo.ogr.wkbXDR | osgeo.ogr.wkbNDR, default=osgeo.ogr.wkbNDR\n"
+		"    One of wkbXDR or wkbNDR indicating MSB or LSB byte order respectively.\n"
 		"\n"
-		"hGeom:  handle on the geometry to convert to a well know binary data\n"
-		"from.\n"
-		"\n"
-		"eOrder:  One of wkbXDR or wkbNDR indicating MSB or LSB byte order\n"
-		"respectively.\n"
-		"\n"
-		"pabyDstBuffer:  a buffer into which the binary representation is\n"
-		"written. This buffer must be at least OGR_G_WkbSize() byte in size.\n"
+		"Returns\n"
+		"--------\n"
+		"bytes\n"
 		"\n"
-		"Currently OGRERR_NONE is always returned.\n"
-		"\n"
-		"GDAL 2.0 \n"
 		""},
 	 { "Geometry_ExportToGML", (PyCFunction)(void(*)(void))_wrap_Geometry_ExportToGML, METH_VARARGS|METH_KEYWORDS, "Geometry_ExportToGML(Geometry self, char ** options=None) -> retStringAndCPLFree *"},
 	 { "Geometry_ExportToKML", _wrap_Geometry_ExportToKML, METH_VARARGS, "Geometry_ExportToKML(Geometry self, char const * altitude_mode=None) -> retStringAndCPLFree *"},
 	 { "Geometry_ExportToJson", (PyCFunction)(void(*)(void))_wrap_Geometry_ExportToJson, METH_VARARGS|METH_KEYWORDS, "Geometry_ExportToJson(Geometry self, char ** options=None) -> retStringAndCPLFree *"},
 	 { "Geometry_AddPoint", (PyCFunction)(void(*)(void))_wrap_Geometry_AddPoint, METH_VARARGS|METH_KEYWORDS, "Geometry_AddPoint(Geometry self, double x, double y, double z=0)"},
 	 { "Geometry_AddPointM", (PyCFunction)(void(*)(void))_wrap_Geometry_AddPointM, METH_VARARGS|METH_KEYWORDS, "Geometry_AddPointM(Geometry self, double x, double y, double m)"},
 	 { "Geometry_AddPointZM", (PyCFunction)(void(*)(void))_wrap_Geometry_AddPointZM, METH_VARARGS|METH_KEYWORDS, "Geometry_AddPointZM(Geometry self, double x, double y, double z, double m)"},
 	 { "Geometry_AddPoint_2D", _wrap_Geometry_AddPoint_2D, METH_VARARGS, "Geometry_AddPoint_2D(Geometry self, double x, double y)"},
 	 { "Geometry_AddGeometryDirectly", _wrap_Geometry_AddGeometryDirectly, METH_VARARGS, "Geometry_AddGeometryDirectly(Geometry self, Geometry other_disown) -> OGRErr"},
 	 { "Geometry_AddGeometry", _wrap_Geometry_AddGeometry, METH_VARARGS, "Geometry_AddGeometry(Geometry self, Geometry other) -> OGRErr"},
 	 { "Geometry_RemoveGeometry", _wrap_Geometry_RemoveGeometry, METH_VARARGS, "Geometry_RemoveGeometry(Geometry self, int iSubGeom) -> OGRErr"},
 	 { "Geometry_Clone", _wrap_Geometry_Clone, METH_O, "\n"
 		"Geometry_Clone(Geometry self) -> Geometry\n"
-		"OGRGeometryH OGR_G_Clone(OGRGeometryH\n"
-		"hGeom)\n"
 		"\n"
 		"Make a copy of this object.\n"
 		"\n"
-		"This function relates to the SFCOM IGeometry::clone() method.\n"
-		"\n"
-		"This function is the same as the CPP method OGRGeometry::clone().\n"
+		"For more details: :cpp:func:`OGR_G_Clone`\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
+		"Returns\n"
+		"--------\n"
+		"Geometry:\n"
+		"    The copy of the geometry with the same spatial reference system\n"
+		"    as the original.\n"
 		"\n"
-		"hGeom:  handle on the geometry to clone from.\n"
-		"\n"
-		"a handle on the copy of the geometry with the spatial reference system\n"
-		"as the original. \n"
 		""},
 	 { "Geometry_GetGeometryType", _wrap_Geometry_GetGeometryType, METH_O, "\n"
 		"Geometry_GetGeometryType(Geometry self) -> OGRwkbGeometryType\n"
-		"OGRwkbGeometryType\n"
-		"OGR_G_GetGeometryType(OGRGeometryH hGeom)\n"
 		"\n"
 		"Fetch geometry type.\n"
 		"\n"
-		"Note that the geometry type may include the 2.5D flag. To get a 2D\n"
-		"flattened version of the geometry type apply the wkbFlatten() macro to\n"
-		"the return result.\n"
-		"\n"
-		"This function is the same as the CPP method\n"
-		"OGRGeometry::getGeometryType().\n"
-		"\n"
-		"Parameters:\n"
-		"-----------\n"
+		"For more details: :cpp:func:`OGR_G_GetGeometryType`\n"
 		"\n"
-		"hGeom:  handle on the geometry to get type from.\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    The geometry type code. The types can be found with\n"
+		"    'osgeo.ogr.wkb' prefix. For example :py:const:`osgeo.ogr.wkbPolygon`.\n"
 		"\n"
-		"the geometry type code. \n"
 		""},
 	 { "Geometry_GetGeometryName", _wrap_Geometry_GetGeometryName, METH_O, "\n"
 		"Geometry_GetGeometryName(Geometry self) -> char const *\n"
-		"const char*\n"
-		"OGR_G_GetGeometryName(OGRGeometryH hGeom)\n"
 		"\n"
 		"Fetch WKT name for geometry type.\n"
 		"\n"
-		"There is no SFCOM analog to this function.\n"
+		"For more details: :cpp:func:`OGR_G_GetGeometryName`\n"
 		"\n"
-		"This function is the same as the CPP method\n"
-		"OGRGeometry::getGeometryName().\n"
-		"\n"
-		"Parameters:\n"
-		"-----------\n"
+		"geometry to get name from.\n"
 		"\n"
-		"hGeom:  handle on the geometry to get name from.\n"
+		"Returns\n"
+		"--------\n"
+		"str\n"
 		"\n"
-		"name used for this geometry type in well known text format. \n"
 		""},
 	 { "Geometry_Length", _wrap_Geometry_Length, METH_O, "Geometry_Length(Geometry self) -> double"},
 	 { "Geometry_Area", _wrap_Geometry_Area, METH_O, "Geometry_Area(Geometry self) -> double"},
 	 { "Geometry_GetArea", _wrap_Geometry_GetArea, METH_O, "Geometry_GetArea(Geometry self) -> double"},
 	 { "Geometry_GetPointCount", _wrap_Geometry_GetPointCount, METH_O, "Geometry_GetPointCount(Geometry self) -> int"},
 	 { "Geometry_GetPoints", (PyCFunction)(void(*)(void))_wrap_Geometry_GetPoints, METH_VARARGS|METH_KEYWORDS, "Geometry_GetPoints(Geometry self, int nCoordDimension=0)"},
 	 { "Geometry_GetX", (PyCFunction)(void(*)(void))_wrap_Geometry_GetX, METH_VARARGS|METH_KEYWORDS, "Geometry_GetX(Geometry self, int point=0) -> double"},
@@ -34567,1283 +35057,830 @@
 	 { "Geometry_GetGeometryCount", _wrap_Geometry_GetGeometryCount, METH_O, "Geometry_GetGeometryCount(Geometry self) -> int"},
 	 { "Geometry_SetPoint", (PyCFunction)(void(*)(void))_wrap_Geometry_SetPoint, METH_VARARGS|METH_KEYWORDS, "Geometry_SetPoint(Geometry self, int point, double x, double y, double z=0)"},
 	 { "Geometry_SetPointM", (PyCFunction)(void(*)(void))_wrap_Geometry_SetPointM, METH_VARARGS|METH_KEYWORDS, "Geometry_SetPointM(Geometry self, int point, double x, double y, double m)"},
 	 { "Geometry_SetPointZM", (PyCFunction)(void(*)(void))_wrap_Geometry_SetPointZM, METH_VARARGS|METH_KEYWORDS, "Geometry_SetPointZM(Geometry self, int point, double x, double y, double z, double m)"},
 	 { "Geometry_SetPoint_2D", (PyCFunction)(void(*)(void))_wrap_Geometry_SetPoint_2D, METH_VARARGS|METH_KEYWORDS, "Geometry_SetPoint_2D(Geometry self, int point, double x, double y)"},
 	 { "Geometry_SwapXY", _wrap_Geometry_SwapXY, METH_O, "\n"
 		"Geometry_SwapXY(Geometry self)\n"
-		"void OGR_G_SwapXY(OGRGeometryH hGeom)\n"
 		"\n"
 		"Swap x and y coordinates.\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
+		"For more details: :cpp:func:`OGR_G_SwapXY`\n"
+		"\n"
+		".. versionadded:: 2.3.0\n"
 		"\n"
-		"hGeom:  geometry.\n"
 		"\n"
-		"OGR 2.3.0 \n"
 		""},
 	 { "Geometry_GetGeometryRef", _wrap_Geometry_GetGeometryRef, METH_VARARGS, "Geometry_GetGeometryRef(Geometry self, int geom) -> Geometry"},
 	 { "Geometry_Simplify", _wrap_Geometry_Simplify, METH_VARARGS, "\n"
 		"Geometry_Simplify(Geometry self, double tolerance) -> Geometry\n"
-		"OGRGeometryH\n"
-		"OGR_G_Simplify(OGRGeometryH hThis, double dTolerance)\n"
 		"\n"
 		"Compute a simplified geometry.\n"
 		"\n"
-		"This function is the same as the C++ method OGRGeometry::Simplify().\n"
+		"For more details: :cpp:func:`OGR_G_Simplify`\n"
 		"\n"
-		"This function is built on the GEOS library, check it for the\n"
-		"definition of the geometry operation. If OGR is built without the GEOS\n"
-		"library, this function will always fail, issuing a CPLE_NotSupported\n"
-		"error.\n"
-		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"tolerance: float\n"
+		"    The distance tolerance for the simplification.\n"
 		"\n"
-		"hThis:  the geometry.\n"
-		"\n"
-		"dTolerance:  the distance tolerance for the simplification.\n"
+		"Returns\n"
+		"--------\n"
+		"Geometry:\n"
+		"    The simplified geometry or None if an error occurs.\n"
 		"\n"
-		"the simplified geometry or NULL if an error occurs.\n"
-		"\n"
-		"OGR 1.8.0 \n"
 		""},
 	 { "Geometry_SimplifyPreserveTopology", _wrap_Geometry_SimplifyPreserveTopology, METH_VARARGS, "\n"
 		"Geometry_SimplifyPreserveTopology(Geometry self, double tolerance) -> Geometry\n"
-		"OGRGeometryH\n"
-		"OGR_G_SimplifyPreserveTopology(OGRGeometryH hThis, double dTolerance)\n"
 		"\n"
 		"Simplify the geometry while preserving topology.\n"
 		"\n"
-		"This function is the same as the C++ method\n"
-		"OGRGeometry::SimplifyPreserveTopology().\n"
-		"\n"
-		"This function is built on the GEOS library, check it for the\n"
-		"definition of the geometry operation. If OGR is built without the GEOS\n"
-		"library, this function will always fail, issuing a CPLE_NotSupported\n"
-		"error.\n"
+		"For more details: :cpp:func:`OGR_G_SimplifyPreserveTopology`\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"tolerance: float\n"
+		"    The distance tolerance for the simplification.\n"
 		"\n"
-		"hThis:  the geometry.\n"
-		"\n"
-		"dTolerance:  the distance tolerance for the simplification.\n"
+		"Returns\n"
+		"--------\n"
+		"Geometry:\n"
+		"    The simplified geometry or None if an error occurs.\n"
 		"\n"
-		"the simplified geometry or NULL if an error occurs.\n"
-		"\n"
-		"OGR 1.9.0 \n"
 		""},
 	 { "Geometry_DelaunayTriangulation", (PyCFunction)(void(*)(void))_wrap_Geometry_DelaunayTriangulation, METH_VARARGS|METH_KEYWORDS, "\n"
 		"Geometry_DelaunayTriangulation(Geometry self, double dfTolerance=0.0, int bOnlyEdges=FALSE) -> Geometry\n"
-		"OGRGeometryH\n"
-		"OGR_G_DelaunayTriangulation(OGRGeometryH hThis, double dfTolerance,\n"
-		"int bOnlyEdges)\n"
 		"\n"
 		"Return a Delaunay triangulation of the vertices of the geometry.\n"
 		"\n"
-		"This function is the same as the C++ method\n"
-		"OGRGeometry::DelaunayTriangulation().\n"
+		"For more details: :cpp:func:`OGR_G_DelaunayTriangulation`\n"
 		"\n"
-		"This function is built on the GEOS library, v3.4 or above. If OGR is\n"
-		"built without the GEOS library, this function will always fail,\n"
-		"issuing a CPLE_NotSupported error.\n"
+		".. versionadded:: 2.1\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"dfTolerance: float\n"
+		"    optional snapping tolerance to use for improved robustness\n"
+		"bOnlyEdges: bool\n"
+		"    If True, will return a MULTILINESTRING, otherwise it will\n"
+		"    return a GEOMETRYCOLLECTION containing triangular POLYGONs.\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"Geometry:\n"
+		"    The geometry resulting from the Delaunay triangulation or None if an\n"
+		"    error occurs.\n"
 		"\n"
-		"hThis:  the geometry.\n"
-		"\n"
-		"dfTolerance:  optional snapping tolerance to use for improved\n"
-		"robustness\n"
-		"\n"
-		"bOnlyEdges:  if TRUE, will return a MULTILINESTRING, otherwise it will\n"
-		"return a GEOMETRYCOLLECTION containing triangular POLYGONs.\n"
-		"\n"
-		"the geometry resulting from the Delaunay triangulation or NULL if an\n"
-		"error occurs.\n"
-		"\n"
-		"OGR 2.1 \n"
 		""},
 	 { "Geometry_Polygonize", _wrap_Geometry_Polygonize, METH_O, "\n"
 		"Geometry_Polygonize(Geometry self) -> Geometry\n"
-		"OGRGeometryH\n"
-		"OGR_G_Polygonize(OGRGeometryH hTarget)\n"
 		"\n"
 		"Polygonizes a set of sparse edges.\n"
 		"\n"
-		"A new geometry object is created and returned containing a collection\n"
-		"of reassembled Polygons: NULL will be returned if the input collection\n"
-		"doesn't corresponds to a MultiLinestring, or when reassembling Edges\n"
-		"into Polygons is impossible due to topological inconsistencies.\n"
-		"\n"
-		"This function is the same as the C++ method OGRGeometry::Polygonize().\n"
-		"\n"
-		"This function is built on the GEOS library, check it for the\n"
-		"definition of the geometry operation. If OGR is built without the GEOS\n"
-		"library, this function will always fail, issuing a CPLE_NotSupported\n"
-		"error.\n"
-		"\n"
-		"Parameters:\n"
-		"-----------\n"
-		"\n"
-		"hTarget:  The Geometry to be polygonized.\n"
+		"For more details: :cpp:func:`OGR_G_Polygonize`\n"
 		"\n"
-		"a handle to a newly allocated geometry now owned by the caller, or\n"
-		"NULL on failure.\n"
+		"Returns\n"
+		"--------\n"
+		"Geometry:\n"
+		"    A new geometry or None on failure.\n"
 		"\n"
-		"OGR 1.9.0 \n"
 		""},
 	 { "Geometry_Boundary", _wrap_Geometry_Boundary, METH_O, "\n"
 		"Geometry_Boundary(Geometry self) -> Geometry\n"
-		"OGRGeometryH\n"
-		"OGR_G_Boundary(OGRGeometryH hTarget)\n"
 		"\n"
 		"Compute boundary.\n"
 		"\n"
-		"A new geometry object is created and returned containing the boundary\n"
-		"of the geometry on which the method is invoked.\n"
-		"\n"
-		"This function is the same as the C++ method OGR_G_Boundary().\n"
-		"\n"
-		"This function is built on the GEOS library, check it for the\n"
-		"definition of the geometry operation. If OGR is built without the GEOS\n"
-		"library, this function will always fail, issuing a CPLE_NotSupported\n"
-		"error.\n"
-		"\n"
-		"Parameters:\n"
-		"-----------\n"
-		"\n"
-		"hTarget:  The Geometry to calculate the boundary of.\n"
+		"For more details: :cpp:func:`OGR_G_Boundary`\n"
 		"\n"
-		"a handle to a newly allocated geometry now owned by the caller, or\n"
-		"NULL on failure.\n"
+		"Returns\n"
+		"--------\n"
+		"Geometry:\n"
+		"    A new geometry or None on failure.\n"
 		"\n"
-		"OGR 1.8.0 \n"
 		""},
 	 { "Geometry_GetBoundary", _wrap_Geometry_GetBoundary, METH_O, "\n"
 		"Geometry_GetBoundary(Geometry self) -> Geometry\n"
-		"OGRGeometryH\n"
-		"OGR_G_GetBoundary(OGRGeometryH hTarget)\n"
 		"\n"
 		"Compute boundary (deprecated)\n"
 		"\n"
-		"Deprecated\n"
+		"For more details: :cpp:func:`OGR_G_GetBoundary`\n"
+		"\n"
+		"..warning:: Deprecated\n"
+		"\n"
+		"See: :cpp:func:`OGR_G_Boundary`\n"
 		"\n"
-		"See:   OGR_G_Boundary() \n"
 		""},
 	 { "Geometry_ConvexHull", _wrap_Geometry_ConvexHull, METH_O, "\n"
 		"Geometry_ConvexHull(Geometry self) -> Geometry\n"
-		"OGRGeometryH\n"
-		"OGR_G_ConvexHull(OGRGeometryH hTarget)\n"
 		"\n"
 		"Compute convex hull.\n"
 		"\n"
-		"A new geometry object is created and returned containing the convex\n"
-		"hull of the geometry on which the method is invoked.\n"
+		"For more details: :cpp:func:`OGR_G_ConvexHull`\n"
 		"\n"
-		"This function is the same as the C++ method OGRGeometry::ConvexHull().\n"
-		"\n"
-		"This function is built on the GEOS library, check it for the\n"
-		"definition of the geometry operation. If OGR is built without the GEOS\n"
-		"library, this function will always fail, issuing a CPLE_NotSupported\n"
-		"error.\n"
-		"\n"
-		"Parameters:\n"
-		"-----------\n"
+		"Returns\n"
+		"--------\n"
+		"Geometry:\n"
+		"    a handle to A newly allocated geometry now owned by the caller, or\n"
+		"    None on failure.\n"
 		"\n"
-		"hTarget:  The Geometry to calculate the convex hull of.\n"
-		"\n"
-		"a handle to a newly allocated geometry now owned by the caller, or\n"
-		"NULL on failure. \n"
 		""},
+	 { "Geometry_ConcaveHull", _wrap_Geometry_ConcaveHull, METH_VARARGS, "Geometry_ConcaveHull(Geometry self, double ratio, bool allowHoles) -> Geometry"},
 	 { "Geometry_MakeValid", _wrap_Geometry_MakeValid, METH_VARARGS, "\n"
 		"Geometry_MakeValid(Geometry self, char ** options=None) -> Geometry\n"
-		"OGRGeometryH\n"
-		"OGR_G_MakeValid(OGRGeometryH hGeom)\n"
 		"\n"
 		"Attempts to make an invalid geometry valid without losing vertices.\n"
 		"\n"
-		"Already-valid geometries are cloned without further intervention.\n"
-		"\n"
-		"This function is the same as the C++ method OGRGeometry::MakeValid().\n"
+		"For more details: :cpp:func:`OGR_G_MakeValidEx`\n"
 		"\n"
-		"This function is built on the GEOS >= 3.8 library, check it for the\n"
-		"definition of the geometry operation. If OGR is built without the GEOS\n"
-		">= 3.8 library, this function will return a clone of the input\n"
-		"geometry if it is valid, or NULL if it is invalid\n"
+		".. versionadded:: 3.0\n"
+		".. versionadded:: 3.4 options\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"options: list[str], optional\n"
+		"    papszOptions to be passed in. For example: [\"METHOD=STRUCTURE\"].\n"
 		"\n"
-		"hGeom:  The Geometry to make valid.\n"
+		"Returns\n"
+		"--------\n"
+		"Geometry:\n"
+		"    A newly allocated geometry now owned by the caller, or None on\n"
+		"    failure.\n"
 		"\n"
-		"a newly allocated geometry now owned by the caller, or NULL on\n"
-		"failure.\n"
-		"\n"
-		"GDAL 3.0 \n"
 		""},
 	 { "Geometry_Normalize", _wrap_Geometry_Normalize, METH_O, "\n"
 		"Geometry_Normalize(Geometry self) -> Geometry\n"
-		"OGRGeometryH\n"
-		"OGR_G_Normalize(OGRGeometryH hGeom)\n"
 		"\n"
 		"Attempts to bring geometry into normalized/canonical form.\n"
 		"\n"
-		"This function is the same as the C++ method OGRGeometry::Normalize().\n"
+		"For more details: :cpp:func:`OGR_G_Normalize`\n"
 		"\n"
-		"This function is built on the GEOS library; check it for the\n"
-		"definition of the geometry operation. If OGR is built without the GEOS\n"
-		"library, this function will always fail, issuing a CPLE_NotSupported\n"
-		"error.\n"
+		".. versionadded:: 3.3\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
+		"Returns\n"
+		"--------\n"
+		"Geometry:\n"
+		"    A newly allocated geometry now owned by the caller, or None on\n"
+		"    failure.\n"
 		"\n"
-		"hGeom:  The Geometry to normalize.\n"
-		"\n"
-		"a newly allocated geometry now owned by the caller, or NULL on\n"
-		"failure.\n"
-		"\n"
-		"GDAL 3.3 \n"
 		""},
 	 { "Geometry_RemoveLowerDimensionSubGeoms", _wrap_Geometry_RemoveLowerDimensionSubGeoms, METH_O, "Geometry_RemoveLowerDimensionSubGeoms(Geometry self) -> Geometry"},
 	 { "Geometry_Buffer", (PyCFunction)(void(*)(void))_wrap_Geometry_Buffer, METH_VARARGS|METH_KEYWORDS, "\n"
 		"Geometry_Buffer(Geometry self, double distance, int quadsecs=30) -> Geometry\n"
-		"OGRGeometryH OGR_G_Buffer(OGRGeometryH\n"
-		"hTarget, double dfDist, int nQuadSegs)\n"
 		"\n"
 		"Compute buffer of geometry.\n"
 		"\n"
-		"Builds a new geometry containing the buffer region around the geometry\n"
-		"on which it is invoked. The buffer is a polygon containing the region\n"
-		"within the buffer distance of the original geometry.\n"
-		"\n"
-		"Some buffer sections are properly described as curves, but are\n"
-		"converted to approximate polygons. The nQuadSegs parameter can be used\n"
-		"to control how many segments should be used to define a 90 degree\n"
-		"curve - a quadrant of a circle. A value of 30 is a reasonable default.\n"
-		"Large values result in large numbers of vertices in the resulting\n"
-		"buffer geometry while small numbers reduce the accuracy of the result.\n"
+		"For more details: :cpp:func:`OGR_G_Buffer`\n"
 		"\n"
-		"This function is the same as the C++ method OGRGeometry::Buffer().\n"
-		"\n"
-		"This function is built on the GEOS library, check it for the\n"
-		"definition of the geometry operation. If OGR is built without the GEOS\n"
-		"library, this function will always fail, issuing a CPLE_NotSupported\n"
-		"error.\n"
-		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"distance: float\n"
+		"    The buffer distance to be applied. Should be expressed into\n"
+		"    the same unit as the coordinates of the geometry.\n"
+		"quadsecs: int, default=30\n"
+		"    The number of segments used to approximate a 90 degree\n"
+		"    (quadrant) of curvature.\n"
+		"\n"
+		"Returns\n"
+		"--------\n"
+		"Geometry:\n"
+		"    The newly created geometry or None if an error occurs.\n"
 		"\n"
-		"hTarget:  the geometry.\n"
-		"\n"
-		"dfDist:  the buffer distance to be applied. Should be expressed into\n"
-		"the same unit as the coordinates of the geometry.\n"
-		"\n"
-		"nQuadSegs:  the number of segments used to approximate a 90 degree\n"
-		"(quadrant) of curvature.\n"
-		"\n"
-		"the newly created geometry, or NULL if an error occurs. \n"
 		""},
 	 { "Geometry_Intersection", _wrap_Geometry_Intersection, METH_VARARGS, "\n"
 		"Geometry_Intersection(Geometry self, Geometry other) -> Geometry\n"
-		"OGRGeometryH\n"
-		"OGR_G_Intersection(OGRGeometryH hThis, OGRGeometryH hOther)\n"
 		"\n"
 		"Compute intersection.\n"
 		"\n"
-		"Generates a new geometry which is the region of intersection of the\n"
-		"two geometries operated on. The OGR_G_Intersects() function can be\n"
-		"used to test if two geometries intersect.\n"
-		"\n"
-		"Geometry validity is not checked. In case you are unsure of the\n"
-		"validity of the input geometries, call IsValid() before, otherwise the\n"
-		"result might be wrong.\n"
-		"\n"
-		"This function is the same as the C++ method\n"
-		"OGRGeometry::Intersection().\n"
-		"\n"
-		"This function is built on the GEOS library, check it for the\n"
-		"definition of the geometry operation. If OGR is built without the GEOS\n"
-		"library, this function will always fail, issuing a CPLE_NotSupported\n"
-		"error.\n"
+		"For more details: :cpp:func:`OGR_G_Intersection`\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"other: Geometry\n"
+		"    The other geometry.\n"
 		"\n"
-		"hThis:  the geometry.\n"
+		"Returns\n"
+		"--------\n"
+		"Geometry:\n"
+		"    A new geometry representing the intersection or None if there is no\n"
+		"    intersection or an error occurs.\n"
 		"\n"
-		"hOther:  the other geometry.\n"
-		"\n"
-		"a new geometry representing the intersection or NULL if there is no\n"
-		"intersection or an error occurs. \n"
 		""},
 	 { "Geometry_Union", _wrap_Geometry_Union, METH_VARARGS, "\n"
 		"Geometry_Union(Geometry self, Geometry other) -> Geometry\n"
-		"OGRGeometryH OGR_G_Union(OGRGeometryH\n"
-		"hThis, OGRGeometryH hOther)\n"
 		"\n"
 		"Compute union.\n"
 		"\n"
-		"Generates a new geometry which is the region of union of the two\n"
-		"geometries operated on.\n"
-		"\n"
-		"Geometry validity is not checked. In case you are unsure of the\n"
-		"validity of the input geometries, call IsValid() before, otherwise the\n"
-		"result might be wrong.\n"
-		"\n"
-		"This function is the same as the C++ method OGRGeometry::Union().\n"
-		"\n"
-		"This function is built on the GEOS library, check it for the\n"
-		"definition of the geometry operation. If OGR is built without the GEOS\n"
-		"library, this function will always fail, issuing a CPLE_NotSupported\n"
-		"error.\n"
+		"For more details: :cpp:func:`OGR_G_Union`\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"other: Geometry\n"
+		"    The other geometry.\n"
 		"\n"
-		"hThis:  the geometry.\n"
+		"Returns\n"
+		"--------\n"
+		"Geometry:\n"
+		"    A new geometry representing the union or None if an error occurs.\n"
 		"\n"
-		"hOther:  the other geometry.\n"
-		"\n"
-		"a new geometry representing the union or NULL if an error occurs. \n"
 		""},
 	 { "Geometry_UnionCascaded", _wrap_Geometry_UnionCascaded, METH_O, "\n"
 		"Geometry_UnionCascaded(Geometry self) -> Geometry\n"
-		"OGRGeometryH\n"
-		"OGR_G_UnionCascaded(OGRGeometryH hThis)\n"
 		"\n"
 		"Compute union using cascading.\n"
 		"\n"
-		"Geometry validity is not checked. In case you are unsure of the\n"
-		"validity of the input geometries, call IsValid() before, otherwise the\n"
-		"result might be wrong.\n"
+		"For more deails: :cpp:func:`OGR_G_UnionCascaded`\n"
 		"\n"
-		"This function is the same as the C++ method\n"
-		"OGRGeometry::UnionCascaded().\n"
+		"Returns\n"
+		"--------\n"
+		"Geometry:\n"
+		"    A new geometry representing the union or None if an error occurs.\n"
 		"\n"
-		"This function is built on the GEOS library, check it for the\n"
-		"definition of the geometry operation. If OGR is built without the GEOS\n"
-		"library, this function will always fail, issuing a CPLE_NotSupported\n"
-		"error.\n"
-		"\n"
-		"Parameters:\n"
-		"-----------\n"
-		"\n"
-		"hThis:  the geometry.\n"
-		"\n"
-		"a new geometry representing the union or NULL if an error occurs. \n"
 		""},
 	 { "Geometry_Difference", _wrap_Geometry_Difference, METH_VARARGS, "\n"
 		"Geometry_Difference(Geometry self, Geometry other) -> Geometry\n"
-		"OGRGeometryH\n"
-		"OGR_G_Difference(OGRGeometryH hThis, OGRGeometryH hOther)\n"
 		"\n"
 		"Compute difference.\n"
 		"\n"
-		"Generates a new geometry which is the region of this geometry with the\n"
-		"region of the other geometry removed.\n"
-		"\n"
-		"Geometry validity is not checked. In case you are unsure of the\n"
-		"validity of the input geometries, call IsValid() before, otherwise the\n"
-		"result might be wrong.\n"
+		"For more details: :cpp:func:`OGR_G_Difference`\n"
 		"\n"
-		"This function is the same as the C++ method OGRGeometry::Difference().\n"
-		"\n"
-		"This function is built on the GEOS library, check it for the\n"
-		"definition of the geometry operation. If OGR is built without the GEOS\n"
-		"library, this function will always fail, issuing a CPLE_NotSupported\n"
-		"error.\n"
-		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"other: Geometry\n"
+		"    The other geometry.\n"
 		"\n"
-		"hThis:  the geometry.\n"
-		"\n"
-		"hOther:  the other geometry.\n"
+		"Returns\n"
+		"--------\n"
+		"Geometry:\n"
+		"    A new geometry representing the difference or None if the difference\n"
+		"    is empty or an error occurs.\n"
 		"\n"
-		"a new geometry representing the difference or NULL if the difference\n"
-		"is empty or an error occurs. \n"
 		""},
 	 { "Geometry_SymDifference", _wrap_Geometry_SymDifference, METH_VARARGS, "\n"
 		"Geometry_SymDifference(Geometry self, Geometry other) -> Geometry\n"
-		"OGRGeometryH\n"
-		"OGR_G_SymDifference(OGRGeometryH hThis, OGRGeometryH hOther)\n"
 		"\n"
 		"Compute symmetric difference.\n"
 		"\n"
-		"Generates a new geometry which is the symmetric difference of this\n"
-		"geometry and the other geometry.\n"
-		"\n"
-		"Geometry validity is not checked. In case you are unsure of the\n"
-		"validity of the input geometries, call IsValid() before, otherwise the\n"
-		"result might be wrong.\n"
-		"\n"
-		"This function is the same as the C++ method\n"
-		"OGRGeometry::SymmetricDifference().\n"
-		"\n"
-		"This function is built on the GEOS library, check it for the\n"
-		"definition of the geometry operation. If OGR is built without the GEOS\n"
-		"library, this function will always fail, issuing a CPLE_NotSupported\n"
-		"error.\n"
+		"For more details: :cpp:func:`OGR_G_SymDifference`\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"other:\n"
+		"    the other geometry.\n"
 		"\n"
-		"hThis:  the geometry.\n"
-		"\n"
-		"hOther:  the other geometry.\n"
+		"Returns\n"
+		"--------\n"
+		"Geometry:\n"
+		"    A new geometry representing the symmetric difference or None if the\n"
+		"    difference is empty or an error occurs.\n"
 		"\n"
-		"a new geometry representing the symmetric difference or NULL if the\n"
-		"difference is empty or an error occurs.\n"
-		"\n"
-		"OGR 1.8.0 \n"
 		""},
 	 { "Geometry_SymmetricDifference", _wrap_Geometry_SymmetricDifference, METH_VARARGS, "\n"
 		"Geometry_SymmetricDifference(Geometry self, Geometry other) -> Geometry\n"
-		"OGRGeometryH\n"
-		"OGR_G_SymmetricDifference(OGRGeometryH hThis, OGRGeometryH hOther)\n"
 		"\n"
 		"Compute symmetric difference (deprecated)\n"
 		"\n"
-		"Deprecated\n"
+		"For more details: :cpp:func:`OGR_G_SymmetricDifference`\n"
+		"\n"
+		".. warning:: Deprecated\n"
+		"\n"
 		"\n"
-		"See:  OGR_G_SymmetricDifference() \n"
 		""},
 	 { "Geometry_Distance", _wrap_Geometry_Distance, METH_VARARGS, "\n"
 		"Geometry_Distance(Geometry self, Geometry other) -> double\n"
-		"double OGR_G_Distance(OGRGeometryH\n"
-		"hFirst, OGRGeometryH hOther)\n"
 		"\n"
 		"Compute distance between two geometries.\n"
 		"\n"
-		"Returns the shortest distance between the two geometries. The distance\n"
-		"is expressed into the same unit as the coordinates of the geometries.\n"
-		"\n"
-		"This function is the same as the C++ method OGRGeometry::Distance().\n"
+		"For more details: :cpp:func:`OGR_G_Distance`\n"
 		"\n"
-		"This function is built on the GEOS library, check it for the\n"
-		"definition of the geometry operation. If OGR is built without the GEOS\n"
-		"library, this function will always fail, issuing a CPLE_NotSupported\n"
-		"error.\n"
-		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"other: Geometry\n"
+		"    The other geometry to compare against.\n"
 		"\n"
-		"hFirst:  the first geometry to compare against.\n"
-		"\n"
-		"hOther:  the other geometry to compare against.\n"
+		"Returns\n"
+		"--------\n"
+		"float:\n"
+		"    The distance between the geometries or -1 if an error occurs.\n"
 		"\n"
-		"the distance between the geometries or -1 if an error occurs. \n"
 		""},
 	 { "Geometry_Distance3D", _wrap_Geometry_Distance3D, METH_VARARGS, "\n"
 		"Geometry_Distance3D(Geometry self, Geometry other) -> double\n"
-		"double\n"
-		"OGR_G_Distance3D(OGRGeometryH hFirst, OGRGeometryH hOther)\n"
 		"\n"
 		"Returns the 3D distance between two geometries.\n"
 		"\n"
-		"The distance is expressed into the same unit as the coordinates of the\n"
-		"geometries.\n"
+		"For more details: :cpp:func:`OGR_G_Distance3D`\n"
 		"\n"
-		"This method is built on the SFCGAL library, check it for the\n"
-		"definition of the geometry operation. If OGR is built without the\n"
-		"SFCGAL library, this method will always return -1.0\n"
+		".. versionadded:: 2.2\n"
 		"\n"
-		"This function is the same as the C++ method OGRGeometry::Distance3D().\n"
-		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"other: Geometry\n"
+		"    The other geometry to compare against.\n"
 		"\n"
-		"hFirst:  the first geometry to compare against.\n"
-		"\n"
-		"hOther:  the other geometry to compare against.\n"
-		"\n"
-		"distance between the two geometries\n"
+		"Returns\n"
+		"--------\n"
+		"float:\n"
+		"    The distance between the geometries or -1 if an error occurs.\n"
 		"\n"
-		"GDAL 2.2\n"
-		"\n"
-		"the distance between the geometries or -1 if an error occurs. \n"
 		""},
 	 { "Geometry_Empty", _wrap_Geometry_Empty, METH_O, "\n"
 		"Geometry_Empty(Geometry self)\n"
-		"void OGR_G_Empty(OGRGeometryH hGeom)\n"
 		"\n"
 		"Clear geometry information.\n"
 		"\n"
-		"This restores the geometry to its initial state after construction,\n"
-		"and before assignment of actual geometry.\n"
-		"\n"
-		"This function relates to the SFCOM IGeometry::Empty() method.\n"
-		"\n"
-		"This function is the same as the CPP method OGRGeometry::empty().\n"
+		"For more details: :cpp:func:`OGR_G_Empty`\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
-		"\n"
-		"hGeom:  handle on the geometry to empty. \n"
 		""},
 	 { "Geometry_IsEmpty", _wrap_Geometry_IsEmpty, METH_O, "\n"
 		"Geometry_IsEmpty(Geometry self) -> bool\n"
-		"int OGR_G_IsEmpty(OGRGeometryH hGeom)\n"
 		"\n"
 		"Test if the geometry is empty.\n"
 		"\n"
-		"This method is the same as the CPP method OGRGeometry::IsEmpty().\n"
+		"For more details: :cpp:func:`OGR_G_IsEmpty`\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    True if the geometry has no points, otherwise False.\n"
 		"\n"
-		"hGeom:  The Geometry to test.\n"
-		"\n"
-		"TRUE if the geometry has no points, otherwise FALSE. \n"
 		""},
 	 { "Geometry_IsValid", _wrap_Geometry_IsValid, METH_O, "\n"
 		"Geometry_IsValid(Geometry self) -> bool\n"
-		"int OGR_G_IsValid(OGRGeometryH hGeom)\n"
 		"\n"
 		"Test if the geometry is valid.\n"
 		"\n"
-		"This function is the same as the C++ method OGRGeometry::IsValid().\n"
-		"\n"
-		"This function is built on the GEOS library, check it for the\n"
-		"definition of the geometry operation. If OGR is built without the GEOS\n"
-		"library, this function will always return FALSE.\n"
-		"\n"
-		"Parameters:\n"
-		"-----------\n"
+		"For more details: :cpp:func:`OGR_G_IsValid`\n"
 		"\n"
-		"hGeom:  The Geometry to test.\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    True if the geometry has no points, otherwise False.\n"
 		"\n"
-		"TRUE if the geometry has no points, otherwise FALSE. \n"
 		""},
 	 { "Geometry_IsSimple", _wrap_Geometry_IsSimple, METH_O, "\n"
 		"Geometry_IsSimple(Geometry self) -> bool\n"
-		"int OGR_G_IsSimple(OGRGeometryH\n"
-		"hGeom)\n"
-		"\n"
-		"Returns TRUE if the geometry is simple.\n"
-		"\n"
-		"Returns TRUE if the geometry has no anomalous geometric points, such\n"
-		"as self intersection or self tangency. The description of each\n"
-		"instantiable geometric class will include the specific conditions that\n"
-		"cause an instance of that class to be classified as not simple.\n"
 		"\n"
-		"This function is the same as the C++ method OGRGeometry::IsSimple()\n"
-		"method.\n"
+		"Returns True if the geometry is simple.\n"
 		"\n"
-		"If OGR is built without the GEOS library, this function will always\n"
-		"return FALSE.\n"
+		"For more details: :cpp:func:`OGR_G_IsSimple`\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
-		"\n"
-		"hGeom:  The Geometry to test.\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    True if object is simple, otherwise False.\n"
 		"\n"
-		"TRUE if object is simple, otherwise FALSE. \n"
 		""},
 	 { "Geometry_IsRing", _wrap_Geometry_IsRing, METH_O, "\n"
 		"Geometry_IsRing(Geometry self) -> bool\n"
-		"int OGR_G_IsRing(OGRGeometryH hGeom)\n"
 		"\n"
 		"Test if the geometry is a ring.\n"
 		"\n"
-		"This function is the same as the C++ method OGRGeometry::IsRing().\n"
-		"\n"
-		"This function is built on the GEOS library, check it for the\n"
-		"definition of the geometry operation. If OGR is built without the GEOS\n"
-		"library, this function will always return FALSE.\n"
+		"For more details: :cpp:func:`OGR_G_IsRing`\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
-		"\n"
-		"hGeom:  The Geometry to test.\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    True if the geometry has no points, otherwise False.\n"
 		"\n"
-		"TRUE if the geometry has no points, otherwise FALSE. \n"
 		""},
 	 { "Geometry_Intersects", _wrap_Geometry_Intersects, METH_VARARGS, "\n"
 		"Geometry_Intersects(Geometry self, Geometry other) -> bool\n"
-		"int OGR_G_Intersects(OGRGeometryH\n"
-		"hGeom, OGRGeometryH hOtherGeom)\n"
-		"\n"
-		"Do these features intersect?\n"
 		"\n"
-		"Determines whether two geometries intersect. If GEOS is enabled, then\n"
-		"this is done in rigorous fashion otherwise TRUE is returned if the\n"
-		"envelopes (bounding boxes) of the two geometries overlap.\n"
+		"Determines whether two geometries intersect.\n"
 		"\n"
-		"This function is the same as the CPP method OGRGeometry::Intersects.\n"
+		"For more details: :cpp:func:`OGR_G_Intersects`\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"other: Geometry\n"
+		"    The other geometry to test against.\n"
 		"\n"
-		"hGeom:  handle on the first geometry.\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    True if the geometries intersect, otherwise False.\n"
 		"\n"
-		"hOtherGeom:  handle on the other geometry to test against.\n"
-		"\n"
-		"TRUE if the geometries intersect, otherwise FALSE. \n"
 		""},
 	 { "Geometry_Intersect", _wrap_Geometry_Intersect, METH_VARARGS, "Geometry_Intersect(Geometry self, Geometry other) -> bool"},
 	 { "Geometry_Equals", _wrap_Geometry_Equals, METH_VARARGS, "\n"
 		"Geometry_Equals(Geometry self, Geometry other) -> bool\n"
-		"int OGR_G_Equals(OGRGeometryH hGeom,\n"
-		"OGRGeometryH hOther)\n"
-		"\n"
-		"Returns TRUE if two geometries are equivalent.\n"
 		"\n"
-		"This operation implements the SQL/MM ST_OrderingEquals() operation.\n"
+		"Returns True if two geometries are equivalent.\n"
 		"\n"
-		"The comparison is done in a structural way, that is to say that the\n"
-		"geometry types must be identical, as well as the number and ordering\n"
-		"of sub-geometries and vertices. Or equivalently, two geometries are\n"
-		"considered equal by this method if their WKT/WKB representation is\n"
-		"equal. Note: this must be distinguished for equality in a spatial way\n"
-		"(which is the purpose of the ST_Equals() operation).\n"
+		"For more details: :cpp:func:`OGR_G_Equals`\n"
 		"\n"
-		"This function is the same as the CPP method OGRGeometry::Equals()\n"
-		"method.\n"
-		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"other: Geometry\n"
+		"    The other geometry to test against.\n"
 		"\n"
-		"hGeom:  handle on the first geometry.\n"
-		"\n"
-		"hOther:  handle on the other geometry to test against.\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    True if equivalent or False otherwise.\n"
 		"\n"
-		"TRUE if equivalent or FALSE otherwise. \n"
 		""},
 	 { "Geometry_Equal", _wrap_Geometry_Equal, METH_VARARGS, "Geometry_Equal(Geometry self, Geometry other) -> bool"},
 	 { "Geometry_Disjoint", _wrap_Geometry_Disjoint, METH_VARARGS, "\n"
 		"Geometry_Disjoint(Geometry self, Geometry other) -> bool\n"
-		"int OGR_G_Disjoint(OGRGeometryH\n"
-		"hThis, OGRGeometryH hOther)\n"
 		"\n"
 		"Test for disjointness.\n"
 		"\n"
-		"Tests if this geometry and the other geometry are disjoint.\n"
-		"\n"
-		"Geometry validity is not checked. In case you are unsure of the\n"
-		"validity of the input geometries, call IsValid() before, otherwise the\n"
-		"result might be wrong.\n"
-		"\n"
-		"This function is the same as the C++ method OGRGeometry::Disjoint().\n"
-		"\n"
-		"This function is built on the GEOS library, check it for the\n"
-		"definition of the geometry operation. If OGR is built without the GEOS\n"
-		"library, this function will always fail, issuing a CPLE_NotSupported\n"
-		"error.\n"
+		"For more details: :cpp:func:`OGR_G_Disjoint`\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"other: Geometry\n"
+		"    The other geometry to compare.\n"
 		"\n"
-		"hThis:  the geometry to compare.\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    True if they are disjoint, otherwise False.\n"
 		"\n"
-		"hOther:  the other geometry to compare.\n"
-		"\n"
-		"TRUE if they are disjoint, otherwise FALSE. \n"
 		""},
 	 { "Geometry_Touches", _wrap_Geometry_Touches, METH_VARARGS, "\n"
 		"Geometry_Touches(Geometry self, Geometry other) -> bool\n"
-		"int OGR_G_Touches(OGRGeometryH hThis,\n"
-		"OGRGeometryH hOther)\n"
 		"\n"
 		"Test for touching.\n"
 		"\n"
-		"Tests if this geometry and the other geometry are touching.\n"
-		"\n"
-		"Geometry validity is not checked. In case you are unsure of the\n"
-		"validity of the input geometries, call IsValid() before, otherwise the\n"
-		"result might be wrong.\n"
-		"\n"
-		"This function is the same as the C++ method OGRGeometry::Touches().\n"
+		"For more details: :cpp:func:`OGR_G_Touches`\n"
 		"\n"
-		"This function is built on the GEOS library, check it for the\n"
-		"definition of the geometry operation. If OGR is built without the GEOS\n"
-		"library, this function will always fail, issuing a CPLE_NotSupported\n"
-		"error.\n"
-		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"other:\n"
+		"    the other geometry to compare.\n"
 		"\n"
-		"hThis:  the geometry to compare.\n"
-		"\n"
-		"hOther:  the other geometry to compare.\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    True if they are touching, otherwise False.\n"
 		"\n"
-		"TRUE if they are touching, otherwise FALSE. \n"
 		""},
 	 { "Geometry_Crosses", _wrap_Geometry_Crosses, METH_VARARGS, "\n"
 		"Geometry_Crosses(Geometry self, Geometry other) -> bool\n"
-		"int OGR_G_Crosses(OGRGeometryH hThis,\n"
-		"OGRGeometryH hOther)\n"
 		"\n"
 		"Test for crossing.\n"
 		"\n"
-		"Tests if this geometry and the other geometry are crossing.\n"
-		"\n"
-		"Geometry validity is not checked. In case you are unsure of the\n"
-		"validity of the input geometries, call IsValid() before, otherwise the\n"
-		"result might be wrong.\n"
+		"For more details: :cpp:func:`OGR_G_Crosses`\n"
 		"\n"
-		"This function is the same as the C++ method OGRGeometry::Crosses().\n"
-		"\n"
-		"This function is built on the GEOS library, check it for the\n"
-		"definition of the geometry operation. If OGR is built without the GEOS\n"
-		"library, this function will always fail, issuing a CPLE_NotSupported\n"
-		"error.\n"
-		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"other: Geometry\n"
+		"    the other geometry to compare.\n"
 		"\n"
-		"hThis:  the geometry to compare.\n"
-		"\n"
-		"hOther:  the other geometry to compare.\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    True if they are crossing, otherwise False.\n"
 		"\n"
-		"TRUE if they are crossing, otherwise FALSE. \n"
 		""},
 	 { "Geometry_Within", _wrap_Geometry_Within, METH_VARARGS, "\n"
 		"Geometry_Within(Geometry self, Geometry other) -> bool\n"
-		"int OGR_G_Within(OGRGeometryH hThis,\n"
-		"OGRGeometryH hOther)\n"
 		"\n"
 		"Test for containment.\n"
 		"\n"
-		"Tests if this geometry is within the other geometry.\n"
-		"\n"
-		"Geometry validity is not checked. In case you are unsure of the\n"
-		"validity of the input geometries, call IsValid() before, otherwise the\n"
-		"result might be wrong.\n"
-		"\n"
-		"This function is the same as the C++ method OGRGeometry::Within().\n"
-		"\n"
-		"This function is built on the GEOS library, check it for the\n"
-		"definition of the geometry operation. If OGR is built without the GEOS\n"
-		"library, this function will always fail, issuing a CPLE_NotSupported\n"
-		"error.\n"
+		"For more details: :cpp:func:`OGR_G_Within`\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"other: Geometry\n"
+		"    the other geometry to compare.\n"
 		"\n"
-		"hThis:  the geometry to compare.\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    True if this is within other, otherwise False.\n"
 		"\n"
-		"hOther:  the other geometry to compare.\n"
-		"\n"
-		"TRUE if hThis is within hOther, otherwise FALSE. \n"
 		""},
 	 { "Geometry_Contains", _wrap_Geometry_Contains, METH_VARARGS, "\n"
 		"Geometry_Contains(Geometry self, Geometry other) -> bool\n"
-		"int OGR_G_Contains(OGRGeometryH\n"
-		"hThis, OGRGeometryH hOther)\n"
 		"\n"
 		"Test for containment.\n"
 		"\n"
-		"Tests if this geometry contains the other geometry.\n"
-		"\n"
-		"Geometry validity is not checked. In case you are unsure of the\n"
-		"validity of the input geometries, call IsValid() before, otherwise the\n"
-		"result might be wrong.\n"
-		"\n"
-		"This function is the same as the C++ method OGRGeometry::Contains().\n"
+		"For more details: :cpp:func:`OGR_G_Contains`\n"
 		"\n"
-		"This function is built on the GEOS library, check it for the\n"
-		"definition of the geometry operation. If OGR is built without the GEOS\n"
-		"library, this function will always fail, issuing a CPLE_NotSupported\n"
-		"error.\n"
-		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"other: Geometry\n"
+		"    the other geometry to compare.\n"
 		"\n"
-		"hThis:  the geometry to compare.\n"
-		"\n"
-		"hOther:  the other geometry to compare.\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    True if this contains the other geometry, otherwise False.\n"
 		"\n"
-		"TRUE if hThis contains hOther geometry, otherwise FALSE. \n"
 		""},
 	 { "Geometry_Overlaps", _wrap_Geometry_Overlaps, METH_VARARGS, "\n"
 		"Geometry_Overlaps(Geometry self, Geometry other) -> bool\n"
-		"int OGR_G_Overlaps(OGRGeometryH\n"
-		"hThis, OGRGeometryH hOther)\n"
 		"\n"
 		"Test for overlap.\n"
 		"\n"
-		"Tests if this geometry and the other geometry overlap, that is their\n"
-		"intersection has a non-zero area.\n"
-		"\n"
-		"Geometry validity is not checked. In case you are unsure of the\n"
-		"validity of the input geometries, call IsValid() before, otherwise the\n"
-		"result might be wrong.\n"
+		"For more details: :cpp:func:`OGR_G_Overlaps`\n"
 		"\n"
-		"This function is the same as the C++ method OGRGeometry::Overlaps().\n"
-		"\n"
-		"This function is built on the GEOS library, check it for the\n"
-		"definition of the geometry operation. If OGR is built without the GEOS\n"
-		"library, this function will always fail, issuing a CPLE_NotSupported\n"
-		"error.\n"
-		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"other: Geometry\n"
+		"    the other geometry to compare.\n"
 		"\n"
-		"hThis:  the geometry to compare.\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    True if they are overlapping, otherwise False.\n"
 		"\n"
-		"hOther:  the other geometry to compare.\n"
-		"\n"
-		"TRUE if they are overlapping, otherwise FALSE. \n"
 		""},
 	 { "Geometry_TransformTo", _wrap_Geometry_TransformTo, METH_VARARGS, "\n"
 		"Geometry_TransformTo(Geometry self, SpatialReference reference) -> OGRErr\n"
-		"OGRErr\n"
-		"OGR_G_TransformTo(OGRGeometryH hGeom, OGRSpatialReferenceH hSRS)\n"
 		"\n"
 		"Transform geometry to new spatial reference system.\n"
 		"\n"
-		"This function will transform the coordinates of a geometry from their\n"
-		"current spatial reference system to a new target spatial reference\n"
-		"system. Normally this means reprojecting the vectors, but it could\n"
-		"include datum shifts, and changes of units.\n"
-		"\n"
-		"This function will only work if the geometry already has an assigned\n"
-		"spatial reference system, and if it is transformable to the target\n"
-		"coordinate system.\n"
-		"\n"
-		"Because this function requires internal creation and initialization of\n"
-		"an OGRCoordinateTransformation object it is significantly more\n"
-		"expensive to use this function to transform many geometries than it is\n"
-		"to create the OGRCoordinateTransformation in advance, and call\n"
-		"transform() with that transformation. This function exists primarily\n"
-		"for convenience when only transforming a single geometry.\n"
-		"\n"
-		"This function is the same as the CPP method OGRGeometry::transformTo.\n"
+		"For more details: :cpp:func:`OGR_G_TransformTo`\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"reference: SpatialReference\n"
+		"   The spatial reference system to apply.\n"
 		"\n"
-		"hGeom:  handle on the geometry to apply the transform to.\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    :py:const:`osgeo.ogr.OGRERR_NONE` on success, or an error code.\n"
 		"\n"
-		"hSRS:  handle on the spatial reference system to apply.\n"
-		"\n"
-		"OGRERR_NONE on success, or an error code. \n"
 		""},
 	 { "Geometry_GetSpatialReference", _wrap_Geometry_GetSpatialReference, METH_O, "\n"
 		"Geometry_GetSpatialReference(Geometry self) -> SpatialReference\n"
-		"OGRSpatialReferenceH\n"
-		"OGR_G_GetSpatialReference(OGRGeometryH hGeom)\n"
-		"\n"
-		"Returns spatial reference system for geometry.\n"
 		"\n"
-		"This function relates to the SFCOM IGeometry::get_SpatialReference()\n"
-		"method.\n"
+		"For more details: :cpp:func:`OGR_G_GetSpatialReference`\n"
 		"\n"
-		"This function is the same as the CPP method\n"
-		"OGRGeometry::getSpatialReference().\n"
-		"\n"
-		"Parameters:\n"
-		"-----------\n"
+		"Returns spatial reference system for geometry.\n"
 		"\n"
-		"hGeom:  handle on the geometry to get spatial reference from.\n"
+		"Returns\n"
+		"--------\n"
+		"SpatialReference\n"
 		"\n"
-		"a reference to the spatial reference geometry. \n"
 		""},
 	 { "Geometry_AssignSpatialReference", _wrap_Geometry_AssignSpatialReference, METH_VARARGS, "\n"
 		"Geometry_AssignSpatialReference(Geometry self, SpatialReference reference)\n"
-		"void\n"
-		"OGR_G_AssignSpatialReference(OGRGeometryH hGeom, OGRSpatialReferenceH\n"
-		"hSRS)\n"
 		"\n"
 		"Assign spatial reference to this object.\n"
 		"\n"
-		"Any existing spatial reference is replaced, but under no circumstances\n"
-		"does this result in the object being reprojected. It is just changing\n"
-		"the interpretation of the existing geometry. Note that assigning a\n"
-		"spatial reference increments the reference count on the\n"
-		"OGRSpatialReference, but does not copy it.\n"
-		"\n"
-		"Starting with GDAL 2.3, this will also assign the spatial reference to\n"
-		"potential sub-geometries of the geometry ( OGRGeometryCollection,\n"
-		"OGRCurvePolygon/OGRPolygon, OGRCompoundCurve, OGRPolyhedralSurface and\n"
-		"their derived classes).\n"
-		"\n"
-		"This is similar to the SFCOM IGeometry::put_SpatialReference() method.\n"
+		"For more details: :cpp:func:`OGR_G_AssignSpatialReference`\n"
 		"\n"
-		"This function is the same as the CPP method\n"
-		"OGRGeometry::assignSpatialReference.\n"
-		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"reference: SpatialReference\n"
+		"    The new spatial reference system to apply.\n"
 		"\n"
-		"hGeom:  handle on the geometry to apply the new spatial reference\n"
-		"system.\n"
-		"\n"
-		"hSRS:  handle on the new spatial reference system to apply. \n"
 		""},
 	 { "Geometry_CloseRings", _wrap_Geometry_CloseRings, METH_O, "\n"
 		"Geometry_CloseRings(Geometry self)\n"
-		"void OGR_G_CloseRings(OGRGeometryH\n"
-		"hGeom)\n"
 		"\n"
 		"Force rings to be closed.\n"
 		"\n"
-		"If this geometry, or any contained geometries has polygon rings that\n"
-		"are not closed, they will be closed by adding the starting point at\n"
-		"the end.\n"
+		"For more details: :cpp:func:`OGR_G_CloseRings`\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
-		"\n"
-		"hGeom:  handle to the geometry. \n"
 		""},
 	 { "Geometry_FlattenTo2D", _wrap_Geometry_FlattenTo2D, METH_O, "\n"
 		"Geometry_FlattenTo2D(Geometry self)\n"
-		"void\n"
-		"OGR_G_FlattenTo2D(OGRGeometryH hGeom)\n"
 		"\n"
 		"Convert geometry to strictly 2D.\n"
 		"\n"
-		"In a sense this converts all Z coordinates to 0.0.\n"
-		"\n"
-		"This function is the same as the CPP method\n"
-		"OGRGeometry::flattenTo2D().\n"
-		"\n"
-		"Parameters:\n"
-		"-----------\n"
+		"For more details: :cpp:func:`OGR_G_FlattenTo2D`\n"
 		"\n"
-		"hGeom:  handle on the geometry to convert. \n"
 		""},
 	 { "Geometry_Segmentize", _wrap_Geometry_Segmentize, METH_VARARGS, "\n"
 		"Geometry_Segmentize(Geometry self, double dfMaxLength)\n"
-		"void OGR_G_Segmentize(OGRGeometryH\n"
-		"hGeom, double dfMaxLength)\n"
 		"\n"
 		"Modify the geometry such it has no segment longer then the given\n"
 		"distance.\n"
 		"\n"
-		"Interpolated points will have Z and M values (if needed) set to 0.\n"
-		"Distance computation is performed in 2d only.\n"
-		"\n"
-		"This function is the same as the CPP method OGRGeometry::segmentize().\n"
+		"For more details: :cpp:func:`OGR_G_Segmentize`\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"dfMaxLength: float\n"
+		"    the maximum distance between 2 points after segmentization\n"
 		"\n"
-		"hGeom:  handle on the geometry to segmentize\n"
-		"\n"
-		"dfMaxLength:  the maximum distance between 2 points after\n"
-		"segmentization \n"
 		""},
 	 { "Geometry_GetEnvelope", _wrap_Geometry_GetEnvelope, METH_O, "\n"
 		"Geometry_GetEnvelope(Geometry self)\n"
-		"void\n"
-		"OGR_G_GetEnvelope(OGRGeometryH hGeom, OGREnvelope *psEnvelope)\n"
 		"\n"
 		"Computes and returns the bounding envelope for this geometry in the\n"
 		"passed psEnvelope structure.\n"
 		"\n"
-		"This function is the same as the CPP method\n"
-		"OGRGeometry::getEnvelope().\n"
+		"For more details: :cpp:func:`OGR_G_GetEnvelope`\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
+		".. warning:: Check the return order of the bounds.\n"
 		"\n"
-		"hGeom:  handle of the geometry to get envelope from.\n"
+		"Returns\n"
+		"--------\n"
+		"minx: float\n"
+		"maxx: float\n"
+		"miny: float\n"
+		"maxy: float\n"
 		"\n"
-		"psEnvelope:  the structure in which to place the results. \n"
 		""},
 	 { "Geometry_GetEnvelope3D", _wrap_Geometry_GetEnvelope3D, METH_O, "\n"
 		"Geometry_GetEnvelope3D(Geometry self)\n"
-		"void\n"
-		"OGR_G_GetEnvelope3D(OGRGeometryH hGeom, OGREnvelope3D *psEnvelope)\n"
 		"\n"
 		"Computes and returns the bounding envelope (3D) for this geometry in\n"
 		"the passed psEnvelope structure.\n"
 		"\n"
-		"This function is the same as the CPP method\n"
-		"OGRGeometry::getEnvelope().\n"
-		"\n"
-		"Parameters:\n"
-		"-----------\n"
+		"For more details: :cpp:func:`OGR_G_GetEnvelope3D`\n"
 		"\n"
-		"hGeom:  handle of the geometry to get envelope from.\n"
+		".. warning:: Check the return order of the bounds.\n"
 		"\n"
-		"psEnvelope:  the structure in which to place the results.\n"
+		"Returns\n"
+		"--------\n"
+		"minx: float\n"
+		"maxx: float\n"
+		"miny: float\n"
+		"maxy: float\n"
+		"minz: float\n"
+		"maxz: float\n"
 		"\n"
-		"OGR 1.9.0 \n"
 		""},
 	 { "Geometry_Centroid", _wrap_Geometry_Centroid, METH_O, "\n"
 		"Geometry_Centroid(Geometry self) -> Geometry\n"
-		"int OGR_G_Centroid(OGRGeometryH\n"
-		"hGeom, OGRGeometryH hCentroidPoint)\n"
 		"\n"
 		"Compute the geometry centroid.\n"
 		"\n"
-		"The centroid location is applied to the passed in OGRPoint object. The\n"
-		"centroid is not necessarily within the geometry.\n"
+		"For more details: :cpp:func:`OGR_G_Centroid`\n"
 		"\n"
-		"This method relates to the SFCOM ISurface::get_Centroid() method\n"
-		"however the current implementation based on GEOS can operate on other\n"
-		"geometry types such as multipoint, linestring, geometrycollection such\n"
-		"as multipolygons. OGC SF SQL 1.1 defines the operation for surfaces\n"
-		"(polygons). SQL/MM-Part 3 defines the operation for surfaces and\n"
-		"multisurfaces (multipolygons).\n"
-		"\n"
-		"This function is the same as the C++ method OGRGeometry::Centroid().\n"
-		"\n"
-		"This function is built on the GEOS library, check it for the\n"
-		"definition of the geometry operation. If OGR is built without the GEOS\n"
-		"library, this function will always fail, issuing a CPLE_NotSupported\n"
-		"error.\n"
+		"Returns\n"
+		"--------\n"
+		"Geometry\n"
 		"\n"
-		"OGRERR_NONE on success or OGRERR_FAILURE on error. \n"
 		""},
 	 { "Geometry_PointOnSurface", _wrap_Geometry_PointOnSurface, METH_O, "\n"
 		"Geometry_PointOnSurface(Geometry self) -> Geometry\n"
-		"OGRGeometryH\n"
-		"OGR_G_PointOnSurface(OGRGeometryH hGeom)\n"
 		"\n"
 		"Returns a point guaranteed to lie on the surface.\n"
 		"\n"
-		"This method relates to the SFCOM ISurface::get_PointOnSurface() method\n"
-		"however the current implementation based on GEOS can operate on other\n"
-		"geometry types than the types that are supported by SQL/MM-Part 3 :\n"
-		"surfaces (polygons) and multisurfaces (multipolygons).\n"
-		"\n"
-		"This method is built on the GEOS library, check it for the definition\n"
-		"of the geometry operation. If OGR is built without the GEOS library,\n"
-		"this method will always fail, issuing a CPLE_NotSupported error.\n"
+		"For more details: :cpp:func:`OGR_G_PointOnSurface`\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
+		"Returns\n"
+		"--------\n"
+		"Geometry:\n"
+		"    A point guaranteed to lie on the surface or None if an error occurred.\n"
 		"\n"
-		"hGeom:  the geometry to operate on.\n"
-		"\n"
-		"a point guaranteed to lie on the surface or NULL if an error occurred.\n"
-		"\n"
-		"OGR 1.10 \n"
 		""},
 	 { "Geometry_WkbSize", _wrap_Geometry_WkbSize, METH_O, "\n"
 		"Geometry_WkbSize(Geometry self) -> size_t\n"
-		"int OGR_G_WkbSize(OGRGeometryH hGeom)\n"
 		"\n"
 		"Returns size of related binary representation.\n"
 		"\n"
-		"This function returns the exact number of bytes required to hold the\n"
-		"well known binary representation of this geometry object. Its\n"
-		"computation may be slightly expensive for complex geometries.\n"
-		"\n"
-		"This function relates to the SFCOM IWks::WkbSize() method.\n"
-		"\n"
-		"This function is the same as the CPP method OGRGeometry::WkbSize().\n"
-		"\n"
-		"Use OGR_G_WkbSizeEx() if called on huge geometries (> 2 GB serialized)\n"
-		"\n"
-		"Parameters:\n"
-		"-----------\n"
+		"For more details: :cpp:func:`OGR_G_WkbSize`\n"
 		"\n"
-		"hGeom:  handle on the geometry to get the binary size from.\n"
+		"Returns\n"
+		"--------\n"
+		"int\n"
 		"\n"
-		"size of binary representation in bytes. \n"
 		""},
 	 { "Geometry_GetCoordinateDimension", _wrap_Geometry_GetCoordinateDimension, METH_O, "\n"
 		"Geometry_GetCoordinateDimension(Geometry self) -> int\n"
-		"int\n"
-		"OGR_G_GetCoordinateDimension(OGRGeometryH hGeom)\n"
 		"\n"
 		"Get the dimension of the coordinates in this geometry.\n"
 		"\n"
-		"This function is the same as the CPP method\n"
-		"OGRGeometry::getCoordinateDimension().\n"
-		"\n"
-		"Parameters:\n"
-		"-----------\n"
+		"For more details: :cpp:func:`OGR_G_GetCoordinateDimension`\n"
 		"\n"
-		"hGeom:  handle on the geometry to get the dimension of the coordinates\n"
-		"from.\n"
+		".. warning:: Deprecated. Use :py:func:`CoordinateDimension`,\n"
+		"    :py:func:`Is3D`, or :py:func:`IsMeasured`.\n"
 		"\n"
-		"Deprecated use OGR_G_CoordinateDimension(), OGR_G_Is3D(), or\n"
-		"OGR_G_IsMeasured().\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    This will return 2 or 3.\n"
 		"\n"
-		"this will return 2 or 3. \n"
 		""},
 	 { "Geometry_CoordinateDimension", _wrap_Geometry_CoordinateDimension, METH_O, "\n"
 		"Geometry_CoordinateDimension(Geometry self) -> int\n"
-		"int\n"
-		"OGR_G_CoordinateDimension(OGRGeometryH hGeom)\n"
 		"\n"
 		"Get the dimension of the coordinates in this geometry.\n"
 		"\n"
-		"This function is the same as the CPP method\n"
-		"OGRGeometry::CoordinateDimension().\n"
-		"\n"
-		"Parameters:\n"
-		"-----------\n"
+		"For more details: :cpp:func:`OGR_G_CoordinateDimension`\n"
 		"\n"
-		"hGeom:  handle on the geometry to get the dimension of the coordinates\n"
-		"from.\n"
+		".. versionadded:: 2.1\n"
 		"\n"
-		"this will return 2 for XY, 3 for XYZ and XYM, and 4 for XYZM data.\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    This will return 2 for XY, 3 for XYZ and XYM, and 4 for XYZM data.\n"
 		"\n"
-		"GDAL 2.1 \n"
 		""},
 	 { "Geometry_Is3D", _wrap_Geometry_Is3D, METH_O, "\n"
 		"Geometry_Is3D(Geometry self) -> int\n"
-		"int OGR_G_Is3D(OGRGeometryH hGeom)\n"
 		"\n"
 		"See whether this geometry has Z coordinates.\n"
 		"\n"
-		"This function is the same as the CPP method OGRGeometry::Is3D().\n"
+		"For more details: :cpp:func:`OGR_G_Is3D`\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
-		"\n"
-		"hGeom:  handle on the geometry to check whether it has Z coordinates.\n"
+		".. versionadded:: 2.1\n"
 		"\n"
-		"TRUE if the geometry has Z coordinates.\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    True if the geometry has Z coordinates.\n"
 		"\n"
-		"GDAL 2.1 \n"
 		""},
 	 { "Geometry_IsMeasured", _wrap_Geometry_IsMeasured, METH_O, "\n"
 		"Geometry_IsMeasured(Geometry self) -> int\n"
-		"int OGR_G_IsMeasured(OGRGeometryH\n"
-		"hGeom)\n"
 		"\n"
 		"See whether this geometry is measured.\n"
 		"\n"
-		"This function is the same as the CPP method OGRGeometry::IsMeasured().\n"
+		"For more details: :cpp:func:`OGR_G_IsMeasured`\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
+		".. versionadded:: 2.1\n"
 		"\n"
-		"hGeom:  handle on the geometry to check whether it is measured.\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    True if the geometry has M coordinates.\n"
 		"\n"
-		"TRUE if the geometry has M coordinates.\n"
-		"\n"
-		"GDAL 2.1 \n"
 		""},
 	 { "Geometry_SetCoordinateDimension", _wrap_Geometry_SetCoordinateDimension, METH_VARARGS, "\n"
 		"Geometry_SetCoordinateDimension(Geometry self, int dimension)\n"
-		"void\n"
-		"OGR_G_SetCoordinateDimension(OGRGeometryH hGeom, int nNewDimension)\n"
 		"\n"
 		"Set the coordinate dimension.\n"
 		"\n"
-		"This method sets the explicit coordinate dimension. Setting the\n"
-		"coordinate dimension of a geometry to 2 should zero out any existing Z\n"
-		"values. Setting the dimension of a geometry collection, a compound\n"
-		"curve, a polygon, etc. will affect the children geometries. This will\n"
-		"also remove the M dimension if present before this call.\n"
+		"For more details: :cpp:func:`OGR_G_SetCoordinateDimension`\n"
 		"\n"
-		"Deprecated use OGR_G_Set3D() or OGR_G_SetMeasured().\n"
+		".. warning:: Deprecated. Use :py:func:`Set3D` or :py:func:`SetMeasured`.\n"
 		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"dimension: int\n"
+		"    New coordinate dimension value, either 2 or 3.\n"
 		"\n"
-		"hGeom:  handle on the geometry to set the dimension of the\n"
-		"coordinates.\n"
-		"\n"
-		"nNewDimension:  New coordinate dimension value, either 2 or 3. \n"
 		""},
 	 { "Geometry_Set3D", _wrap_Geometry_Set3D, METH_VARARGS, "\n"
 		"Geometry_Set3D(Geometry self, int b3D)\n"
-		"void OGR_G_Set3D(OGRGeometryH hGeom,\n"
-		"int bIs3D)\n"
 		"\n"
 		"Add or remove the Z coordinate dimension.\n"
 		"\n"
-		"This method adds or removes the explicit Z coordinate dimension.\n"
-		"Removing the Z coordinate dimension of a geometry will remove any\n"
-		"existing Z values. Adding the Z dimension to a geometry collection, a\n"
-		"compound curve, a polygon, etc. will affect the children geometries.\n"
+		"For more details: :cpp:func:`OGR_G_Set3D`\n"
 		"\n"
-		"Parameters:\n"
-		"-----------\n"
-		"\n"
-		"hGeom:  handle on the geometry to set or unset the Z dimension.\n"
+		".. versionadded:: 2.1\n"
 		"\n"
-		"bIs3D:  Should the geometry have a Z dimension, either TRUE or FALSE.\n"
+		"Parameters\n"
+		"-----------\n"
+		"bIs3D: bool\n"
+		"    Should the geometry have a Z dimension, either True or False.\n"
 		"\n"
-		"GDAL 2.1 \n"
 		""},
 	 { "Geometry_SetMeasured", _wrap_Geometry_SetMeasured, METH_VARARGS, "\n"
 		"Geometry_SetMeasured(Geometry self, int bMeasured)\n"
-		"void\n"
-		"OGR_G_SetMeasured(OGRGeometryH hGeom, int bIsMeasured)\n"
 		"\n"
 		"Add or remove the M coordinate dimension.\n"
 		"\n"
-		"This method adds or removes the explicit M coordinate dimension.\n"
-		"Removing the M coordinate dimension of a geometry will remove any\n"
-		"existing M values. Adding the M dimension to a geometry collection, a\n"
-		"compound curve, a polygon, etc. will affect the children geometries.\n"
-		"\n"
-		"Parameters:\n"
-		"-----------\n"
+		"For more details: :cpp:func:`OGR_G_SetMeasured`\n"
 		"\n"
-		"hGeom:  handle on the geometry to set or unset the M dimension.\n"
+		".. versionadded:: 2.1\n"
 		"\n"
-		"bIsMeasured:  Should the geometry have a M dimension, either TRUE or\n"
-		"FALSE.\n"
+		"Parameters\n"
+		"-----------\n"
+		"bIsMeasured: bool\n"
+		"    Should the geometry have a M dimension, either True or False.\n"
 		"\n"
-		"GDAL 2.1 \n"
 		""},
 	 { "Geometry_GetDimension", _wrap_Geometry_GetDimension, METH_O, "\n"
 		"Geometry_GetDimension(Geometry self) -> int\n"
-		"int\n"
-		"OGR_G_GetDimension(OGRGeometryH hGeom)\n"
 		"\n"
 		"Get the dimension of this geometry.\n"
 		"\n"
-		"This function corresponds to the SFCOM IGeometry::GetDimension()\n"
-		"method. It indicates the dimension of the geometry, but does not\n"
-		"indicate the dimension of the underlying space (as indicated by\n"
-		"OGR_G_GetCoordinateDimension() function).\n"
-		"\n"
-		"This function is the same as the CPP method\n"
-		"OGRGeometry::getDimension().\n"
-		"\n"
-		"Parameters:\n"
-		"-----------\n"
+		"For more details: :cpp:func:`OGR_G_GetDimension`\n"
 		"\n"
-		"hGeom:  handle on the geometry to get the dimension from.\n"
+		"Returns\n"
+		"--------\n"
+		"int:\n"
+		"    0 for points, 1 for lines, and 2 for surfaces.\n"
 		"\n"
-		"0 for points, 1 for lines and 2 for surfaces. \n"
 		""},
 	 { "Geometry_HasCurveGeometry", _wrap_Geometry_HasCurveGeometry, METH_VARARGS, "Geometry_HasCurveGeometry(Geometry self, int bLookForCircular=FALSE) -> int"},
 	 { "Geometry_GetLinearGeometry", (PyCFunction)(void(*)(void))_wrap_Geometry_GetLinearGeometry, METH_VARARGS|METH_KEYWORDS, "Geometry_GetLinearGeometry(Geometry self, double dfMaxAngleStepSizeDegrees=0.0, char ** options=None) -> Geometry"},
 	 { "Geometry_GetCurveGeometry", (PyCFunction)(void(*)(void))_wrap_Geometry_GetCurveGeometry, METH_VARARGS|METH_KEYWORDS, "Geometry_GetCurveGeometry(Geometry self, char ** options=None) -> Geometry"},
 	 { "Geometry_Value", _wrap_Geometry_Value, METH_VARARGS, "Geometry_Value(Geometry self, double dfDistance) -> Geometry"},
 	 { "Geometry_Transform", _wrap_Geometry_Transform, METH_VARARGS, "\n"
 		"Geometry_Transform(Geometry self, CoordinateTransformation trans) -> OGRErr\n"
 		"Geometry_Transform(Geometry self, GeomTransformer transformer) -> Geometry\n"
-		"OGRErr OGR_G_Transform(OGRGeometryH\n"
-		"hGeom, OGRCoordinateTransformationH hTransform)\n"
 		"\n"
 		"Apply arbitrary coordinate transformation to geometry.\n"
 		"\n"
-		"This function will transform the coordinates of a geometry from their\n"
-		"current spatial reference system to a new target spatial reference\n"
-		"system. Normally this means reprojecting the vectors, but it could\n"
-		"include datum shifts, and changes of units.\n"
+		"For more details: :cpp:func:`OGR_G_Transform`\n"
 		"\n"
-		"Note that this function does not require that the geometry already\n"
-		"have a spatial reference system. It will be assumed that they can be\n"
-		"treated as having the source spatial reference system of the\n"
-		"OGRCoordinateTransformation object, and the actual SRS of the geometry\n"
-		"will be ignored. On successful completion the output\n"
-		"OGRSpatialReference of the OGRCoordinateTransformation will be\n"
-		"assigned to the geometry.\n"
-		"\n"
-		"This function is the same as the CPP method OGRGeometry::transform.\n"
-		"\n"
-		"Parameters:\n"
+		"Parameters\n"
 		"-----------\n"
+		"trans: CoordinateTransform\n"
+		"    The transformation to apply.\n"
 		"\n"
-		"hGeom:  handle on the geometry to apply the transform to.\n"
-		"\n"
-		"hTransform:  handle on the transformation to apply.\n"
+		"Returns\n"
+		"--------\n"
+		"Geometry:\n"
+		"    The transformed geometry.\n"
 		"\n"
-		"OGRERR_NONE on success or an error code. \n"
 		""},
 	 { "Geometry_CreatePreparedGeometry", _wrap_Geometry_CreatePreparedGeometry, METH_O, "Geometry_CreatePreparedGeometry(Geometry self) -> PreparedGeometry"},
 	 { "Geometry_swigregister", Geometry_swigregister, METH_O, NULL},
 	 { "Geometry_swiginit", Geometry_swiginit, METH_VARARGS, NULL},
 	 { "delete_PreparedGeometry", _wrap_delete_PreparedGeometry, METH_O, "delete_PreparedGeometry(PreparedGeometry self)"},
 	 { "PreparedGeometry_Intersects", _wrap_PreparedGeometry_Intersects, METH_VARARGS, "PreparedGeometry_Intersects(PreparedGeometry self, Geometry otherGeom) -> bool"},
 	 { "PreparedGeometry_Contains", _wrap_PreparedGeometry_Contains, METH_VARARGS, "PreparedGeometry_Contains(PreparedGeometry self, Geometry otherGeom) -> bool"},
@@ -35917,14 +35954,17 @@
 }
 static void *_p_OGRLayerShadowTo_p_GDALMajorObjectShadow(void *x, int *SWIGUNUSEDPARM(newmemory)) {
     return (void *)((GDALMajorObjectShadow *)  ((OGRLayerShadow *) x));
 }
 static void *_p_OGRDataSourceShadowTo_p_GDALMajorObjectShadow(void *x, int *SWIGUNUSEDPARM(newmemory)) {
     return (void *)((GDALMajorObjectShadow *)  ((OGRDataSourceShadow *) x));
 }
+static swig_type_info _swigt__p_ArrowArray = {"_p_ArrowArray", "ArrowArray *", 0, 0, (void*)0, 0};
+static swig_type_info _swigt__p_ArrowArrayStream = {"_p_ArrowArrayStream", "ArrowArrayStream *", 0, 0, (void*)0, 0};
+static swig_type_info _swigt__p_ArrowSchema = {"_p_ArrowSchema", "ArrowSchema *", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_GDALMajorObjectShadow = {"_p_GDALMajorObjectShadow", "GDALMajorObjectShadow *", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_GDALProgressFunc = {"_p_GDALProgressFunc", "GDALProgressFunc *", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_GIntBig = {"_p_GIntBig", "GIntBig *", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_OGRCodedValue = {"_p_OGRCodedValue", "OGRCodedValue *", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_OGRDataSourceShadow = {"_p_OGRDataSourceShadow", "OGRDataSourceShadow *", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_OGRDriverShadow = {"_p_OGRDriverShadow", "OGRDriverShadow *", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_OGRFeatureDefnShadow = {"_p_OGRFeatureDefnShadow", "OGRFeatureDefnShadow *", 0, 0, (void*)0, 0};
@@ -35941,20 +35981,24 @@
 static swig_type_info _swigt__p_OSRSpatialReferenceShadow = {"_p_OSRSpatialReferenceShadow", "OSRSpatialReferenceShadow *", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_char = {"_p_char", "char *|retStringAndCPLFree *", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_double = {"_p_double", "double *", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_f_double_p_q_const__char_p_void__int = {"_p_f_double_p_q_const__char_p_void__int", "int (*)(double,char const *,void *)", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_float = {"_p_float", "float *", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_int = {"_p_int", "OGRFieldSubType *|OSRAxisMappingStrategy *|OGRFieldDomainType *|OGRFieldType *|CPLErr *|int *|OGRwkbGeometryType *|OGRJustification *|OGRAxisOrientation *|OGRFieldDomainSplitPolicy *|OGRFieldDomainMergePolicy *|OGRwkbByteOrder *|OGRErr *", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_p_GIntBig = {"_p_p_GIntBig", "GIntBig **", 0, 0, (void*)0, 0};
+static swig_type_info _swigt__p_p_OGRGeometryTypeCounter = {"_p_p_OGRGeometryTypeCounter", "OGRGeometryTypeCounter **", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_p_char = {"_p_p_char", "char **", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_p_double = {"_p_p_double", "double **", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_p_int = {"_p_p_int", "int **", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_size_t = {"_p_size_t", "size_t *", 0, 0, (void*)0, 0};
 
 static swig_type_info *swig_type_initial[] = {
+  &_swigt__p_ArrowArray,
+  &_swigt__p_ArrowArrayStream,
+  &_swigt__p_ArrowSchema,
   &_swigt__p_GDALMajorObjectShadow,
   &_swigt__p_GDALProgressFunc,
   &_swigt__p_GIntBig,
   &_swigt__p_OGRCodedValue,
   &_swigt__p_OGRDataSourceShadow,
   &_swigt__p_OGRDriverShadow,
   &_swigt__p_OGRFeatureDefnShadow,
@@ -35971,20 +36015,24 @@
   &_swigt__p_OSRSpatialReferenceShadow,
   &_swigt__p_char,
   &_swigt__p_double,
   &_swigt__p_f_double_p_q_const__char_p_void__int,
   &_swigt__p_float,
   &_swigt__p_int,
   &_swigt__p_p_GIntBig,
+  &_swigt__p_p_OGRGeometryTypeCounter,
   &_swigt__p_p_char,
   &_swigt__p_p_double,
   &_swigt__p_p_int,
   &_swigt__p_size_t,
 };
 
+static swig_cast_info _swigc__p_ArrowArray[] = {  {&_swigt__p_ArrowArray, 0, 0, 0},{0, 0, 0, 0}};
+static swig_cast_info _swigc__p_ArrowArrayStream[] = {  {&_swigt__p_ArrowArrayStream, 0, 0, 0},{0, 0, 0, 0}};
+static swig_cast_info _swigc__p_ArrowSchema[] = {  {&_swigt__p_ArrowSchema, 0, 0, 0},{0, 0, 0, 0}};
 static swig_cast_info _swigc__p_GDALMajorObjectShadow[] = {  {&_swigt__p_GDALMajorObjectShadow, 0, 0, 0},  {&_swigt__p_OGRDriverShadow, _p_OGRDriverShadowTo_p_GDALMajorObjectShadow, 0, 0},  {&_swigt__p_OGRLayerShadow, _p_OGRLayerShadowTo_p_GDALMajorObjectShadow, 0, 0},  {&_swigt__p_OGRDataSourceShadow, _p_OGRDataSourceShadowTo_p_GDALMajorObjectShadow, 0, 0},{0, 0, 0, 0}};
 static swig_cast_info _swigc__p_GDALProgressFunc[] = {  {&_swigt__p_GDALProgressFunc, 0, 0, 0},{0, 0, 0, 0}};
 static swig_cast_info _swigc__p_GIntBig[] = {  {&_swigt__p_GIntBig, 0, 0, 0},{0, 0, 0, 0}};
 static swig_cast_info _swigc__p_OGRCodedValue[] = {  {&_swigt__p_OGRCodedValue, 0, 0, 0},{0, 0, 0, 0}};
 static swig_cast_info _swigc__p_OGRDataSourceShadow[] = {  {&_swigt__p_OGRDataSourceShadow, 0, 0, 0},{0, 0, 0, 0}};
 static swig_cast_info _swigc__p_OGRDriverShadow[] = {  {&_swigt__p_OGRDriverShadow, 0, 0, 0},{0, 0, 0, 0}};
 static swig_cast_info _swigc__p_OGRFeatureDefnShadow[] = {  {&_swigt__p_OGRFeatureDefnShadow, 0, 0, 0},{0, 0, 0, 0}};
@@ -36001,20 +36049,24 @@
 static swig_cast_info _swigc__p_OSRSpatialReferenceShadow[] = {  {&_swigt__p_OSRSpatialReferenceShadow, 0, 0, 0},{0, 0, 0, 0}};
 static swig_cast_info _swigc__p_char[] = {  {&_swigt__p_char, 0, 0, 0},{0, 0, 0, 0}};
 static swig_cast_info _swigc__p_double[] = {  {&_swigt__p_double, 0, 0, 0},{0, 0, 0, 0}};
 static swig_cast_info _swigc__p_f_double_p_q_const__char_p_void__int[] = {  {&_swigt__p_f_double_p_q_const__char_p_void__int, 0, 0, 0},{0, 0, 0, 0}};
 static swig_cast_info _swigc__p_float[] = {  {&_swigt__p_float, 0, 0, 0},{0, 0, 0, 0}};
 static swig_cast_info _swigc__p_int[] = {  {&_swigt__p_int, 0, 0, 0},{0, 0, 0, 0}};
 static swig_cast_info _swigc__p_p_GIntBig[] = {  {&_swigt__p_p_GIntBig, 0, 0, 0},{0, 0, 0, 0}};
+static swig_cast_info _swigc__p_p_OGRGeometryTypeCounter[] = {  {&_swigt__p_p_OGRGeometryTypeCounter, 0, 0, 0},{0, 0, 0, 0}};
 static swig_cast_info _swigc__p_p_char[] = {  {&_swigt__p_p_char, 0, 0, 0},{0, 0, 0, 0}};
 static swig_cast_info _swigc__p_p_double[] = {  {&_swigt__p_p_double, 0, 0, 0},{0, 0, 0, 0}};
 static swig_cast_info _swigc__p_p_int[] = {  {&_swigt__p_p_int, 0, 0, 0},{0, 0, 0, 0}};
 static swig_cast_info _swigc__p_size_t[] = {  {&_swigt__p_size_t, 0, 0, 0},{0, 0, 0, 0}};
 
 static swig_cast_info *swig_cast_initial[] = {
+  _swigc__p_ArrowArray,
+  _swigc__p_ArrowArrayStream,
+  _swigc__p_ArrowSchema,
   _swigc__p_GDALMajorObjectShadow,
   _swigc__p_GDALProgressFunc,
   _swigc__p_GIntBig,
   _swigc__p_OGRCodedValue,
   _swigc__p_OGRDataSourceShadow,
   _swigc__p_OGRDriverShadow,
   _swigc__p_OGRFeatureDefnShadow,
@@ -36031,14 +36083,15 @@
   _swigc__p_OSRSpatialReferenceShadow,
   _swigc__p_char,
   _swigc__p_double,
   _swigc__p_f_double_p_q_const__char_p_void__int,
   _swigc__p_float,
   _swigc__p_int,
   _swigc__p_p_GIntBig,
+  _swigc__p_p_OGRGeometryTypeCounter,
   _swigc__p_p_char,
   _swigc__p_p_double,
   _swigc__p_p_int,
   _swigc__p_size_t,
 };
 
 
@@ -36888,45 +36941,59 @@
   SWIG_Python_SetConstant(d, "ALTER_WIDTH_PRECISION_FLAG",SWIG_From_int(static_cast< int >(4)));
   SWIG_Python_SetConstant(d, "ALTER_NULLABLE_FLAG",SWIG_From_int(static_cast< int >(8)));
   SWIG_Python_SetConstant(d, "ALTER__FLAG",SWIG_From_int(static_cast< int >(8)));
   SWIG_Python_SetConstant(d, "ALTER_DEFAULT_FLAG",SWIG_From_int(static_cast< int >(16)));
   SWIG_Python_SetConstant(d, "ALTER_UNIQUE_FLAG",SWIG_From_int(static_cast< int >(32)));
   SWIG_Python_SetConstant(d, "ALTER_DOMAIN_FLAG",SWIG_From_int(static_cast< int >(64)));
   SWIG_Python_SetConstant(d, "ALTER_ALL_FLAG",SWIG_From_int(static_cast< int >(1+2+4+8+16+32+64)));
+  SWIG_Python_SetConstant(d, "ALTER_GEOM_FIELD_DEFN_NAME_FLAG",SWIG_From_int(static_cast< int >(4096)));
+  SWIG_Python_SetConstant(d, "ALTER_GEOM_FIELD_DEFN_TYPE_FLAG",SWIG_From_int(static_cast< int >(8192)));
+  SWIG_Python_SetConstant(d, "ALTER_GEOM_FIELD_DEFN_NULLABLE_FLAG",SWIG_From_int(static_cast< int >(16384)));
+  SWIG_Python_SetConstant(d, "ALTER_GEOM_FIELD_DEFN_SRS_FLAG",SWIG_From_int(static_cast< int >(32768)));
+  SWIG_Python_SetConstant(d, "ALTER_GEOM_FIELD_DEFN_SRS_COORD_EPOCH_FLAG",SWIG_From_int(static_cast< int >(65536)));
+  SWIG_Python_SetConstant(d, "ALTER_GEOM_FIELD_DEFN_ALL_FLAG",SWIG_From_int(static_cast< int >(4096+8192+16384+32768+65536)));
   SWIG_Python_SetConstant(d, "F_VAL_NULL",SWIG_From_int(static_cast< int >(0x00000001)));
   SWIG_Python_SetConstant(d, "F_VAL_GEOM_TYPE",SWIG_From_int(static_cast< int >(0x00000002)));
   SWIG_Python_SetConstant(d, "F_VAL_WIDTH",SWIG_From_int(static_cast< int >(0x00000004)));
   SWIG_Python_SetConstant(d, "F_VAL_ALLOW_NULL_WHEN_DEFAULT",SWIG_From_int(static_cast< int >(0x00000008)));
   SWIG_Python_SetConstant(d, "F_VAL_ALL",SWIG_From_int(static_cast< int >(0xFFFFFFFF)));
+  SWIG_Python_SetConstant(d, "GGT_COUNT_NOT_NEEDED",SWIG_From_int(static_cast< int >(0x1)));
+  SWIG_Python_SetConstant(d, "GGT_STOP_IF_MIXED",SWIG_From_int(static_cast< int >(0x2)));
+  SWIG_Python_SetConstant(d, "GGT_GEOMCOLLECTIONZ_TINZ",SWIG_From_int(static_cast< int >(0x4)));
   SWIG_Python_SetConstant(d, "OLCRandomRead",SWIG_FromCharPtr("RandomRead"));
   SWIG_Python_SetConstant(d, "OLCSequentialWrite",SWIG_FromCharPtr("SequentialWrite"));
   SWIG_Python_SetConstant(d, "OLCRandomWrite",SWIG_FromCharPtr("RandomWrite"));
   SWIG_Python_SetConstant(d, "OLCFastSpatialFilter",SWIG_FromCharPtr("FastSpatialFilter"));
   SWIG_Python_SetConstant(d, "OLCFastFeatureCount",SWIG_FromCharPtr("FastFeatureCount"));
   SWIG_Python_SetConstant(d, "OLCFastGetExtent",SWIG_FromCharPtr("FastGetExtent"));
   SWIG_Python_SetConstant(d, "OLCCreateField",SWIG_FromCharPtr("CreateField"));
   SWIG_Python_SetConstant(d, "OLCDeleteField",SWIG_FromCharPtr("DeleteField"));
   SWIG_Python_SetConstant(d, "OLCReorderFields",SWIG_FromCharPtr("ReorderFields"));
   SWIG_Python_SetConstant(d, "OLCAlterFieldDefn",SWIG_FromCharPtr("AlterFieldDefn"));
+  SWIG_Python_SetConstant(d, "OLCAlterGeomFieldDefn",SWIG_FromCharPtr("AlterGeomFieldDefn"));
   SWIG_Python_SetConstant(d, "OLCTransactions",SWIG_FromCharPtr("Transactions"));
   SWIG_Python_SetConstant(d, "OLCDeleteFeature",SWIG_FromCharPtr("DeleteFeature"));
+  SWIG_Python_SetConstant(d, "OLCUpsertFeature",SWIG_FromCharPtr("UpsertFeature"));
   SWIG_Python_SetConstant(d, "OLCFastSetNextByIndex",SWIG_FromCharPtr("FastSetNextByIndex"));
   SWIG_Python_SetConstant(d, "OLCStringsAsUTF8",SWIG_FromCharPtr("StringsAsUTF8"));
   SWIG_Python_SetConstant(d, "OLCIgnoreFields",SWIG_FromCharPtr("IgnoreFields"));
   SWIG_Python_SetConstant(d, "OLCCreateGeomField",SWIG_FromCharPtr("CreateGeomField"));
   SWIG_Python_SetConstant(d, "OLCCurveGeometries",SWIG_FromCharPtr("CurveGeometries"));
   SWIG_Python_SetConstant(d, "OLCMeasuredGeometries",SWIG_FromCharPtr("MeasuredGeometries"));
+  SWIG_Python_SetConstant(d, "OLCZGeometries",SWIG_FromCharPtr("ZGeometries"));
   SWIG_Python_SetConstant(d, "OLCRename",SWIG_FromCharPtr("Rename"));
+  SWIG_Python_SetConstant(d, "OLCFastGetArrowStream",SWIG_FromCharPtr("FastGetArrowStream"));
   SWIG_Python_SetConstant(d, "ODsCCreateLayer",SWIG_FromCharPtr("CreateLayer"));
   SWIG_Python_SetConstant(d, "ODsCDeleteLayer",SWIG_FromCharPtr("DeleteLayer"));
   SWIG_Python_SetConstant(d, "ODsCCreateGeomFieldAfterCreateLayer",SWIG_FromCharPtr("CreateGeomFieldAfterCreateLayer"));
   SWIG_Python_SetConstant(d, "ODsCCurveGeometries",SWIG_FromCharPtr("CurveGeometries"));
   SWIG_Python_SetConstant(d, "ODsCTransactions",SWIG_FromCharPtr("Transactions"));
   SWIG_Python_SetConstant(d, "ODsCEmulatedTransactions",SWIG_FromCharPtr("EmulatedTransactions"));
   SWIG_Python_SetConstant(d, "ODsCMeasuredGeometries",SWIG_FromCharPtr("MeasuredGeometries"));
+  SWIG_Python_SetConstant(d, "ODsCZGeometries",SWIG_FromCharPtr("ZGeometries"));
   SWIG_Python_SetConstant(d, "ODsCRandomLayerRead",SWIG_FromCharPtr("RandomLayerRead"));
   SWIG_Python_SetConstant(d, "ODsCRandomLayerWrite",SWIG_FromCharPtr("RandomLayerWrite "));
   SWIG_Python_SetConstant(d, "ODsCAddFieldDomain",SWIG_FromCharPtr("AddFieldDomain"));
   SWIG_Python_SetConstant(d, "ODsCDeleteFieldDomain",SWIG_FromCharPtr("DeleteFieldDomain"));
   SWIG_Python_SetConstant(d, "ODsCUpdateFieldDomain",SWIG_FromCharPtr("UpdateFieldDomain"));
   SWIG_Python_SetConstant(d, "ODrCCreateDataSource",SWIG_FromCharPtr("CreateDataSource"));
   SWIG_Python_SetConstant(d, "ODrCDeleteDataSource",SWIG_FromCharPtr("DeleteDataSource"));
```

### Comparing `pygdal-3.5.3.11/extensions/osr_wrap.cpp` & `pygdal-3.6.4.11/extensions/osr_wrap.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -4041,14 +4041,17 @@
   }
 SWIGINTERN OSRSpatialReferenceShadow *OSRSpatialReferenceShadow_CloneGeogCS(OSRSpatialReferenceShadow *self){
     return (OSRSpatialReferenceShadow*) OSRCloneGeogCS(self);
   }
 SWIGINTERN OSRSpatialReferenceShadow *OSRSpatialReferenceShadow_Clone(OSRSpatialReferenceShadow *self){
     return (OSRSpatialReferenceShadow*) OSRClone(self);
   }
+SWIGINTERN OGRErr OSRSpatialReferenceShadow_StripVertical(OSRSpatialReferenceShadow *self){
+    return OSRStripVertical(self);
+  }
 SWIGINTERN OGRErr OSRSpatialReferenceShadow_Validate(OSRSpatialReferenceShadow *self){
     return OSRValidate(self);
   }
 SWIGINTERN OGRErr OSRSpatialReferenceShadow_MorphToESRI(OSRSpatialReferenceShadow *self){
     return OSRMorphToESRI(self);
   }
 SWIGINTERN OGRErr OSRSpatialReferenceShadow_MorphFromESRI(OSRSpatialReferenceShadow *self){
@@ -4070,47 +4073,50 @@
     OCTDestroyCoordinateTransformationOptions( self );
   }
 SWIGINTERN bool OGRCoordinateTransformationOptions_SetAreaOfInterest(OGRCoordinateTransformationOptions *self,double westLongitudeDeg,double southLatitudeDeg,double eastLongitudeDeg,double northLatitudeDeg){
     return OCTCoordinateTransformationOptionsSetAreaOfInterest(self,
         westLongitudeDeg, southLatitudeDeg,
         eastLongitudeDeg, northLatitudeDeg);
   }
-SWIGINTERN bool OGRCoordinateTransformationOptions_SetOperation(OGRCoordinateTransformationOptions *self,char const *operation){
-    return OCTCoordinateTransformationOptionsSetOperation(self, operation, false);
-  }
-SWIGINTERN bool OGRCoordinateTransformationOptions_SetDesiredAccuracy(OGRCoordinateTransformationOptions *self,double accuracy){
-    return OCTCoordinateTransformationOptionsSetDesiredAccuracy(self, accuracy);
-  }
 
 SWIGINTERN int
 SWIG_AsVal_bool (PyObject *obj, bool *val)
 {
   int r;
   if (!PyBool_Check(obj))
     return SWIG_ERROR;
   r = PyObject_IsTrue(obj);
   if (r == -1)
     return SWIG_ERROR;
   if (val) *val = r ? true : false;
   return SWIG_OK;
 }
 
+SWIGINTERN bool OGRCoordinateTransformationOptions_SetOperation(OGRCoordinateTransformationOptions *self,char const *operation,bool inverseCT=false){
+    return OCTCoordinateTransformationOptionsSetOperation(self, operation, inverseCT);
+  }
+SWIGINTERN bool OGRCoordinateTransformationOptions_SetDesiredAccuracy(OGRCoordinateTransformationOptions *self,double accuracy){
+    return OCTCoordinateTransformationOptionsSetDesiredAccuracy(self, accuracy);
+  }
 SWIGINTERN bool OGRCoordinateTransformationOptions_SetBallparkAllowed(OGRCoordinateTransformationOptions *self,bool allowBallpark){
     return OCTCoordinateTransformationOptionsSetBallparkAllowed(self, allowBallpark);
   }
 SWIGINTERN OSRCoordinateTransformationShadow *new_OSRCoordinateTransformationShadow__SWIG_0(OSRSpatialReferenceShadow *src,OSRSpatialReferenceShadow *dst){
     return (OSRCoordinateTransformationShadow*) OCTNewCoordinateTransformation(src, dst);
   }
 SWIGINTERN OSRCoordinateTransformationShadow *new_OSRCoordinateTransformationShadow__SWIG_1(OSRSpatialReferenceShadow *src,OSRSpatialReferenceShadow *dst,OGRCoordinateTransformationOptions *options){
     return (OSRCoordinateTransformationShadow*)
         options ? OCTNewCoordinateTransformationEx( src, dst, options ) : OCTNewCoordinateTransformation(src, dst);
   }
 SWIGINTERN void delete_OSRCoordinateTransformationShadow(OSRCoordinateTransformationShadow *self){
     OCTDestroyCoordinateTransformation( self );
   }
+SWIGINTERN OSRCoordinateTransformationShadow *OSRCoordinateTransformationShadow_GetInverse(OSRCoordinateTransformationShadow *self){
+    return OCTGetInverse(self);
+  }
 SWIGINTERN void OSRCoordinateTransformationShadow_TransformPoint__SWIG_0(OSRCoordinateTransformationShadow *self,double inout[3]){
     if (self == NULL)
         return;
     OCTTransform( self, 1, &inout[0], &inout[1], &inout[2] );
   }
 SWIGINTERN void OSRCoordinateTransformationShadow_TransformPoint__SWIG_1(OSRCoordinateTransformationShadow *self,double inout[4]){
     if (self == NULL)
@@ -14692,14 +14698,67 @@
   if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
   return resultobj;
 fail:
   return NULL;
 }
 
 
+SWIGINTERN PyObject *_wrap_SpatialReference_StripVertical(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  OSRSpatialReferenceShadow *arg1 = (OSRSpatialReferenceShadow *) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  PyObject *swig_obj[1] ;
+  OGRErr result;
+  
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_OSRSpatialReferenceShadow, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "SpatialReference_StripVertical" "', argument " "1"" of type '" "OSRSpatialReferenceShadow *""'"); 
+  }
+  arg1 = reinterpret_cast< OSRSpatialReferenceShadow * >(argp1);
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    result = (OGRErr)OSRSpatialReferenceShadow_StripVertical(arg1);
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  {
+    /* %typemap(out) OGRErr */
+    if ( result != 0 && bUseExceptions) {
+      const char* pszMessage = CPLGetLastErrorMsg();
+      if( pszMessage[0] != '\0' )
+      PyErr_SetString( PyExc_RuntimeError, pszMessage );
+      else
+      PyErr_SetString( PyExc_RuntimeError, OGRErrMessages(result) );
+      SWIG_fail;
+    }
+  }
+  {
+    /* %typemap(ret) OGRErr */
+    if ( ReturnSame(resultobj == Py_None || resultobj == 0) ) {
+      resultobj = PyInt_FromLong( result );
+    }
+  }
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  return NULL;
+}
+
+
 SWIGINTERN PyObject *_wrap_SpatialReference_Validate(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
   OSRSpatialReferenceShadow *arg1 = (OSRSpatialReferenceShadow *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   PyObject *swig_obj[1] ;
   OGRErr result;
@@ -15194,38 +15253,48 @@
 }
 
 
 SWIGINTERN PyObject *_wrap_CoordinateTransformationOptions_SetOperation(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
   OGRCoordinateTransformationOptions *arg1 = (OGRCoordinateTransformationOptions *) 0 ;
   char *arg2 = (char *) 0 ;
+  bool arg3 = (bool) false ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   int res2 ;
   char *buf2 = 0 ;
   int alloc2 = 0 ;
-  PyObject *swig_obj[2] ;
+  bool val3 ;
+  int ecode3 = 0 ;
+  PyObject *swig_obj[3] ;
   bool result;
   
-  if (!SWIG_Python_UnpackTuple(args, "CoordinateTransformationOptions_SetOperation", 2, 2, swig_obj)) SWIG_fail;
+  if (!SWIG_Python_UnpackTuple(args, "CoordinateTransformationOptions_SetOperation", 2, 3, swig_obj)) SWIG_fail;
   res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_OGRCoordinateTransformationOptions, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "CoordinateTransformationOptions_SetOperation" "', argument " "1"" of type '" "OGRCoordinateTransformationOptions *""'"); 
   }
   arg1 = reinterpret_cast< OGRCoordinateTransformationOptions * >(argp1);
   res2 = SWIG_AsCharPtrAndSize(swig_obj[1], &buf2, NULL, &alloc2);
   if (!SWIG_IsOK(res2)) {
     SWIG_exception_fail(SWIG_ArgError(res2), "in method '" "CoordinateTransformationOptions_SetOperation" "', argument " "2"" of type '" "char const *""'");
   }
   arg2 = reinterpret_cast< char * >(buf2);
+  if (swig_obj[2]) {
+    ecode3 = SWIG_AsVal_bool(swig_obj[2], &val3);
+    if (!SWIG_IsOK(ecode3)) {
+      SWIG_exception_fail(SWIG_ArgError(ecode3), "in method '" "CoordinateTransformationOptions_SetOperation" "', argument " "3"" of type '" "bool""'");
+    } 
+    arg3 = static_cast< bool >(val3);
+  }
   {
     if ( bUseExceptions ) {
       ClearErrorState();
     }
-    result = (bool)OGRCoordinateTransformationOptions_SetOperation(arg1,(char const *)arg2);
+    result = (bool)OGRCoordinateTransformationOptions_SetOperation(arg1,(char const *)arg2,arg3);
 #ifndef SED_HACKS
     if ( bUseExceptions ) {
       CPLErr eclass = CPLGetLastErrorType();
       if ( eclass == CE_Failure || eclass == CE_Fatal ) {
         SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
       }
     }
@@ -15517,14 +15586,51 @@
   if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
   return resultobj;
 fail:
   return NULL;
 }
 
 
+SWIGINTERN PyObject *_wrap_CoordinateTransformation_GetInverse(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
+  OSRCoordinateTransformationShadow *arg1 = (OSRCoordinateTransformationShadow *) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  PyObject *swig_obj[1] ;
+  OSRCoordinateTransformationShadow *result = 0 ;
+  
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_OSRCoordinateTransformationShadow, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "CoordinateTransformation_GetInverse" "', argument " "1"" of type '" "OSRCoordinateTransformationShadow *""'"); 
+  }
+  arg1 = reinterpret_cast< OSRCoordinateTransformationShadow * >(argp1);
+  {
+    if ( bUseExceptions ) {
+      ClearErrorState();
+    }
+    result = (OSRCoordinateTransformationShadow *)OSRCoordinateTransformationShadow_GetInverse(arg1);
+#ifndef SED_HACKS
+    if ( bUseExceptions ) {
+      CPLErr eclass = CPLGetLastErrorType();
+      if ( eclass == CE_Failure || eclass == CE_Fatal ) {
+        SWIG_exception( SWIG_RuntimeError, CPLGetLastErrorMsg() );
+      }
+    }
+#endif
+  }
+  resultobj = SWIG_NewPointerObj(SWIG_as_voidptr(result), SWIGTYPE_p_OSRCoordinateTransformationShadow, SWIG_POINTER_OWN |  0 );
+  if ( ReturnSame(bLocalUseExceptionsCode) ) { CPLErr eclass = CPLGetLastErrorType(); if ( eclass == CE_Failure || eclass == CE_Fatal ) { Py_XDECREF(resultobj); SWIG_Error( SWIG_RuntimeError, CPLGetLastErrorMsg() ); return NULL; } }
+  return resultobj;
+fail:
+  return NULL;
+}
+
+
 SWIGINTERN PyObject *_wrap_CoordinateTransformation_TransformPoint__SWIG_0(PyObject *SWIGUNUSEDPARM(self), Py_ssize_t nobjs, PyObject **swig_obj) {
   PyObject *resultobj = 0; int bLocalUseExceptionsCode = bUseExceptions;
   OSRCoordinateTransformationShadow *arg1 = (OSRCoordinateTransformationShadow *) 0 ;
   double *arg2 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   double argin2[3] ;
@@ -18030,35 +18136,37 @@
 	 { "SpatialReference_ExportToProj4", _wrap_SpatialReference_ExportToProj4, METH_O, "SpatialReference_ExportToProj4(SpatialReference self) -> OGRErr"},
 	 { "SpatialReference_ExportToPCI", _wrap_SpatialReference_ExportToPCI, METH_O, "SpatialReference_ExportToPCI(SpatialReference self) -> OGRErr"},
 	 { "SpatialReference_ExportToUSGS", _wrap_SpatialReference_ExportToUSGS, METH_O, "SpatialReference_ExportToUSGS(SpatialReference self) -> OGRErr"},
 	 { "SpatialReference_ExportToXML", _wrap_SpatialReference_ExportToXML, METH_VARARGS, "SpatialReference_ExportToXML(SpatialReference self, char const * dialect=\"\") -> OGRErr"},
 	 { "SpatialReference_ExportToMICoordSys", _wrap_SpatialReference_ExportToMICoordSys, METH_O, "SpatialReference_ExportToMICoordSys(SpatialReference self) -> OGRErr"},
 	 { "SpatialReference_CloneGeogCS", _wrap_SpatialReference_CloneGeogCS, METH_O, "SpatialReference_CloneGeogCS(SpatialReference self) -> SpatialReference"},
 	 { "SpatialReference_Clone", _wrap_SpatialReference_Clone, METH_O, "SpatialReference_Clone(SpatialReference self) -> SpatialReference"},
+	 { "SpatialReference_StripVertical", _wrap_SpatialReference_StripVertical, METH_O, "SpatialReference_StripVertical(SpatialReference self) -> OGRErr"},
 	 { "SpatialReference_Validate", _wrap_SpatialReference_Validate, METH_O, "SpatialReference_Validate(SpatialReference self) -> OGRErr"},
 	 { "SpatialReference_MorphToESRI", _wrap_SpatialReference_MorphToESRI, METH_O, "SpatialReference_MorphToESRI(SpatialReference self) -> OGRErr"},
 	 { "SpatialReference_MorphFromESRI", _wrap_SpatialReference_MorphFromESRI, METH_O, "SpatialReference_MorphFromESRI(SpatialReference self) -> OGRErr"},
 	 { "SpatialReference_ConvertToOtherProjection", _wrap_SpatialReference_ConvertToOtherProjection, METH_VARARGS, "SpatialReference_ConvertToOtherProjection(SpatialReference self, char const * other_projection, char ** options=None) -> SpatialReference"},
 	 { "SpatialReference_PromoteTo3D", _wrap_SpatialReference_PromoteTo3D, METH_VARARGS, "SpatialReference_PromoteTo3D(SpatialReference self, char const * name=None) -> OGRErr"},
 	 { "SpatialReference_DemoteTo2D", _wrap_SpatialReference_DemoteTo2D, METH_VARARGS, "SpatialReference_DemoteTo2D(SpatialReference self, char const * name=None) -> OGRErr"},
 	 { "SpatialReference_swigregister", SpatialReference_swigregister, METH_O, NULL},
 	 { "SpatialReference_swiginit", SpatialReference_swiginit, METH_VARARGS, NULL},
 	 { "new_CoordinateTransformationOptions", _wrap_new_CoordinateTransformationOptions, METH_NOARGS, "new_CoordinateTransformationOptions() -> CoordinateTransformationOptions"},
 	 { "delete_CoordinateTransformationOptions", _wrap_delete_CoordinateTransformationOptions, METH_O, "delete_CoordinateTransformationOptions(CoordinateTransformationOptions self)"},
 	 { "CoordinateTransformationOptions_SetAreaOfInterest", _wrap_CoordinateTransformationOptions_SetAreaOfInterest, METH_VARARGS, "CoordinateTransformationOptions_SetAreaOfInterest(CoordinateTransformationOptions self, double westLongitudeDeg, double southLatitudeDeg, double eastLongitudeDeg, double northLatitudeDeg) -> bool"},
-	 { "CoordinateTransformationOptions_SetOperation", _wrap_CoordinateTransformationOptions_SetOperation, METH_VARARGS, "CoordinateTransformationOptions_SetOperation(CoordinateTransformationOptions self, char const * operation) -> bool"},
+	 { "CoordinateTransformationOptions_SetOperation", _wrap_CoordinateTransformationOptions_SetOperation, METH_VARARGS, "CoordinateTransformationOptions_SetOperation(CoordinateTransformationOptions self, char const * operation, bool inverseCT=False) -> bool"},
 	 { "CoordinateTransformationOptions_SetDesiredAccuracy", _wrap_CoordinateTransformationOptions_SetDesiredAccuracy, METH_VARARGS, "CoordinateTransformationOptions_SetDesiredAccuracy(CoordinateTransformationOptions self, double accuracy) -> bool"},
 	 { "CoordinateTransformationOptions_SetBallparkAllowed", _wrap_CoordinateTransformationOptions_SetBallparkAllowed, METH_VARARGS, "CoordinateTransformationOptions_SetBallparkAllowed(CoordinateTransformationOptions self, bool allowBallpark) -> bool"},
 	 { "CoordinateTransformationOptions_swigregister", CoordinateTransformationOptions_swigregister, METH_O, NULL},
 	 { "CoordinateTransformationOptions_swiginit", CoordinateTransformationOptions_swiginit, METH_VARARGS, NULL},
 	 { "new_CoordinateTransformation", _wrap_new_CoordinateTransformation, METH_VARARGS, "\n"
 		"CoordinateTransformation(SpatialReference src, SpatialReference dst)\n"
 		"new_CoordinateTransformation(SpatialReference src, SpatialReference dst, CoordinateTransformationOptions options) -> CoordinateTransformation\n"
 		""},
 	 { "delete_CoordinateTransformation", _wrap_delete_CoordinateTransformation, METH_O, "delete_CoordinateTransformation(CoordinateTransformation self)"},
+	 { "CoordinateTransformation_GetInverse", _wrap_CoordinateTransformation_GetInverse, METH_O, "CoordinateTransformation_GetInverse(CoordinateTransformation self) -> CoordinateTransformation"},
 	 { "CoordinateTransformation_TransformPoint", _wrap_CoordinateTransformation_TransformPoint, METH_VARARGS, "\n"
 		"CoordinateTransformation_TransformPoint(CoordinateTransformation self, double [3] inout)\n"
 		"CoordinateTransformation_TransformPoint(CoordinateTransformation self, double [4] inout)\n"
 		"CoordinateTransformation_TransformPoint(CoordinateTransformation self, double x, double y, double z=0.0)\n"
 		"CoordinateTransformation_TransformPoint(CoordinateTransformation self, double x, double y, double z, double t)\n"
 		""},
 	 { "CoordinateTransformation_TransformPointWithErrorCode", _wrap_CoordinateTransformation_TransformPointWithErrorCode, METH_VARARGS, "CoordinateTransformation_TransformPointWithErrorCode(CoordinateTransformation self, double x, double y, double z, double t)"},
```

### Comparing `pygdal-3.5.3.11/osgeo/__init__.py` & `pygdal-3.6.4.11/osgeo/__init__.py`

 * *Files identical despite different names*

### Comparing `pygdal-3.5.3.11/osgeo/gdal.py` & `pygdal-3.6.4.11/osgeo/gdal.py`

 * *Files 18% similar despite different names*

```diff
@@ -146,31 +146,31 @@
           if not entry:
               break
           yield entry
   finally:
       CloseDir(dir)
 
 
-def GetUseExceptions(*args):
+def GetUseExceptions(*args) -> "int":
     r"""GetUseExceptions() -> int"""
     return _gdal.GetUseExceptions(*args)
 
-def UseExceptions(*args):
+def UseExceptions(*args) -> "void":
     r"""UseExceptions()"""
     return _gdal.UseExceptions(*args)
 
-def DontUseExceptions(*args):
+def DontUseExceptions(*args) -> "void":
     r"""DontUseExceptions()"""
     return _gdal.DontUseExceptions(*args)
 
-def VSIFReadL(*args):
+def VSIFReadL(*args) -> "void **":
     r"""VSIFReadL(unsigned int nMembSize, unsigned int nMembCount, VSILFILE fp) -> unsigned int"""
     return _gdal.VSIFReadL(*args)
 
-def VSIGetMemFileBuffer_unsafe(*args):
+def VSIGetMemFileBuffer_unsafe(*args) -> "vsi_l_offset *":
     r"""VSIGetMemFileBuffer_unsafe(char const * utf8_path)"""
     return _gdal.VSIGetMemFileBuffer_unsafe(*args)
 
 
 def InfoOptions(options=None, format='text', deserialize=True,
          computeMinMax=False, reportHistograms=False, reportProj4=False,
          stats=False, approxStats=False, computeChecksum=False,
@@ -224,21 +224,25 @@
         if extraMDDomains is not None:
             for mdd in extraMDDomains:
                 new_options += ['-mdd', mdd]
 
     return (GDALInfoOptions(new_options), format, deserialize)
 
 def Info(ds, **kwargs):
-    """ Return information on a dataset.
-        Arguments are :
-          ds --- a Dataset object or a filename
-        Keyword arguments are :
-          options --- return of gdal.InfoOptions(), string or array of strings
-          other keywords arguments of gdal.InfoOptions()
-        If options is provided as a gdal.InfoOptions() object, other keywords are ignored. """
+    """Return information on a dataset.
+
+    Parameters
+    ----------
+    ds:
+        a Dataset object or a filename
+    kwargs:
+        options: return of gdal.InfoOptions(), string or array of strings
+        other keywords arguments of gdal.InfoOptions().
+        If options is provided as a gdal.InfoOptions() object, other keywords are ignored.
+    """
     if 'options' not in kwargs or isinstance(kwargs['options'], (list, str)):
         (opts, format, deserialize) = InfoOptions(**kwargs)
     else:
         (opts, format, deserialize) = kwargs['options']
     if isinstance(ds, str):
         ds = Open(ds)
     ret = InfoInternal(ds, opts)
@@ -267,21 +271,25 @@
         if arrayoptions:
             for option in arrayoptions:
                 new_options += ['-arrayoption', option]
 
     return GDALMultiDimInfoOptions(new_options), as_text
 
 def MultiDimInfo(ds, **kwargs):
-    """ Return information on a dataset.
-        Arguments are :
-          ds --- a Dataset object or a filename
-        Keyword arguments are :
-          options --- return of gdal.MultiDimInfoOptions(), string or array of strings
-          other keywords arguments of gdal.MultiDimInfoOptions()
-        If options is provided as a gdal.MultiDimInfoOptions() object, other keywords are ignored. """
+    """Return information on a dataset.
+
+    Parameters
+    ----------
+    ds:
+        a Dataset object or a filename
+    kwargs:
+        options: return of gdal.MultiDimInfoOptions(), string or array of strings
+        other keywords arguments of gdal.MultiDimInfoOptions().
+        If options is provided as a gdal.MultiDimInfoOptions() object, other keywords are ignored.
+    """
     if 'options' not in kwargs or isinstance(kwargs['options'], (list, str)):
         opts, as_text = MultiDimInfoOptions(**kwargs)
     else:
         opts = kwargs['options']
         as_text = True
     if isinstance(ds, str):
         ds = OpenEx(ds, OF_VERBOSE_ERROR | OF_MULTIDIM_RASTER)
@@ -313,49 +321,86 @@
               xRes = 0.0, yRes = 0.0,
               creationOptions=None, srcWin=None, projWin=None, projWinSRS=None, strict = False,
               unscale = False, scaleParams=None, exponents=None,
               outputBounds=None, metadataOptions=None,
               outputSRS=None, nogcp=False, GCPs=None,
               noData=None, rgbExpand=None,
               stats = False, rat = True, xmp = True, resampleAlg=None,
+              overviewLevel = 'AUTO',
               callback=None, callback_data=None):
-    """ Create a TranslateOptions() object that can be passed to gdal.Translate()
-        Keyword arguments are :
-          options --- can be be an array of strings, a string or let empty and filled from other keywords.
-          format --- output format ("GTiff", etc...)
-          outputType --- output type (gdalconst.GDT_Byte, etc...)
-          bandList --- array of band numbers (index start at 1)
-          maskBand --- mask band to generate or not ("none", "auto", "mask", 1, ...)
-          width --- width of the output raster in pixel
-          height --- height of the output raster in pixel
-          widthPct --- width of the output raster in percentage (100 = original width)
-          heightPct --- height of the output raster in percentage (100 = original height)
-          xRes --- output horizontal resolution
-          yRes --- output vertical resolution
-          creationOptions --- list of creation options
-          srcWin --- subwindow in pixels to extract: [left_x, top_y, width, height]
-          projWin --- subwindow in projected coordinates to extract: [ulx, uly, lrx, lry]
-          projWinSRS --- SRS in which projWin is expressed
-          strict --- strict mode
-          unscale --- unscale values with scale and offset metadata
-          scaleParams --- list of scale parameters, each of the form [src_min,src_max] or [src_min,src_max,dst_min,dst_max]
-          exponents --- list of exponentiation parameters
-          outputBounds --- assigned output bounds: [ulx, uly, lrx, lry]
-          metadataOptions --- list of metadata options
-          outputSRS --- assigned output SRS
-          nogcp --- ignore GCP in the raster
-          GCPs --- list of GCPs
-          noData --- nodata value (or "none" to unset it)
-          rgbExpand --- Color palette expansion mode: "gray", "rgb", "rgba"
-          stats --- whether to calculate statistics
-          rat --- whether to write source RAT
-          xmp --- whether to copy XMP metadata
-          resampleAlg --- resampling mode
-          callback --- callback method
-          callback_data --- user data for callback
+    """Create a TranslateOptions() object that can be passed to gdal.Translate()
+
+    Parameters
+    ----------
+    options:
+        can be be an array of strings, a string or let empty and filled from other keywords.
+    format:
+        output format ("GTiff", etc...)
+    outputType:
+        output type (gdalconst.GDT_Byte, etc...)
+    bandList:
+        array of band numbers (index start at 1)
+    maskBand:
+        mask band to generate or not ("none", "auto", "mask", 1, ...)
+    width:
+        width of the output raster in pixel
+    height:
+        height of the output raster in pixel
+    widthPct:
+        width of the output raster in percentage (100 = original width)
+    heightPct:
+        height of the output raster in percentage (100 = original height)
+    xRes:
+        output horizontal resolution
+    yRes:
+        output vertical resolution
+    creationOptions:
+        list of creation options
+    srcWin:
+        subwindow in pixels to extract: [left_x, top_y, width, height]
+    projWin:
+        subwindow in projected coordinates to extract: [ulx, uly, lrx, lry]
+    projWinSRS:
+        SRS in which projWin is expressed
+    strict:
+        strict mode
+    unscale:
+        unscale values with scale and offset metadata
+    scaleParams:
+        list of scale parameters, each of the form [src_min,src_max] or [src_min,src_max,dst_min,dst_max]
+    exponents:
+        list of exponentiation parameters
+    outputBounds:
+        assigned output bounds: [ulx, uly, lrx, lry]
+    metadataOptions:
+        list of metadata options
+    outputSRS:
+        assigned output SRS
+    nogcp:
+        ignore GCP in the raster
+    GCPs:
+        list of GCPs
+    noData:
+        nodata value (or "none" to unset it)
+    rgbExpand:
+        Color palette expansion mode: "gray", "rgb", "rgba"
+    stats:
+        whether to calculate statistics
+    rat:
+        whether to write source RAT
+    xmp:
+        whether to copy XMP metadata
+    resampleAlg:
+        resampling mode
+    overviewLevel:
+        To specify which overview level of source files must be used
+    callback:
+        callback method
+    callback_data:
+        user data for callback
     """
 
 # Only used for tests
     return_option_list = options == '__RETURN_OPTION_LIST__'
     if return_option_list:
         options = []
     else:
@@ -431,28 +476,46 @@
             if resampleAlg in mapGRIORAMethodToString:
                 new_options += ['-r', mapGRIORAMethodToString[resampleAlg]]
             else:
                 new_options += ['-r', str(resampleAlg)]
         if xRes != 0 and yRes != 0:
             new_options += ['-tr', _strHighPrec(xRes), _strHighPrec(yRes)]
 
+        if overviewLevel is None or isinstance(overviewLevel, str):
+            pass
+        elif isinstance(overviewLevel, int):
+            if overviewLevel < 0:
+                overviewLevel = 'AUTO' + str(overviewLevel)
+            else:
+                overviewLevel = str(overviewLevel)
+        else:
+            overviewLevel = None
+
+        if overviewLevel is not None and overviewLevel != 'AUTO':
+            new_options += ['-ovr', overviewLevel]
+
     if return_option_list:
         return new_options
 
     return (GDALTranslateOptions(new_options), callback, callback_data)
 
 def Translate(destName, srcDS, **kwargs):
-    """ Convert a dataset.
-        Arguments are :
-          destName --- Output dataset name
-          srcDS --- a Dataset object or a filename
-        Keyword arguments are :
-          options --- return of gdal.TranslateOptions(), string or array of strings
-          other keywords arguments of gdal.TranslateOptions()
-        If options is provided as a gdal.TranslateOptions() object, other keywords are ignored. """
+    """Convert a dataset.
+
+    Parameters
+    ----------
+    destName:
+        Output dataset name
+    srcDS:
+        a Dataset object or a filename
+    kwargs:
+        options: return of gdal.TranslateOptions(), string or array of strings
+        other keywords arguments of gdal.TranslateOptions().
+        If options is provided as a gdal.TranslateOptions() object, other keywords are ignored.
+    """
 
     if 'options' not in kwargs or isinstance(kwargs['options'], (list, str)):
         (opts, callback, callback_data) = TranslateOptions(**kwargs)
     else:
         (opts, callback, callback_data) = kwargs['options']
     if isinstance(srcDS, str):
         srcDS = Open(srcDS)
@@ -474,56 +537,100 @@
          tps = False, rpc = False, geoloc = False, polynomialOrder=None,
          transformerOptions=None, cutlineDSName=None,
          cutlineLayer=None, cutlineWhere=None, cutlineSQL=None, cutlineBlend=None, cropToCutline = False,
          copyMetadata = True, metadataConflictValue=None,
          setColorInterpretation = False,
          overviewLevel = 'AUTO',
          callback=None, callback_data=None):
-    """ Create a WarpOptions() object that can be passed to gdal.Warp()
-        Keyword arguments are :
-          options --- can be be an array of strings, a string or let empty and filled from other keywords.
-          format --- output format ("GTiff", etc...)
-          outputBounds --- output bounds as (minX, minY, maxX, maxY) in target SRS
-          outputBoundsSRS --- SRS in which output bounds are expressed, in the case they are not expressed in dstSRS
-          xRes, yRes --- output resolution in target SRS
-          targetAlignedPixels --- whether to force output bounds to be multiple of output resolution
-          width --- width of the output raster in pixel
-          height --- height of the output raster in pixel
-          srcSRS --- source SRS
-          dstSRS --- output SRS
-          coordinateOperation -- coordinate operation as a PROJ string or WKT string
-          srcAlpha --- whether to force the last band of the input dataset to be considered as an alpha band
-          dstAlpha --- whether to force the creation of an output alpha band
-          outputType --- output type (gdalconst.GDT_Byte, etc...)
-          workingType --- working type (gdalconst.GDT_Byte, etc...)
-          warpOptions --- list of warping options
-          errorThreshold --- error threshold for approximation transformer (in pixels)
-          warpMemoryLimit --- size of working buffer in MB
-          resampleAlg --- resampling mode
-          creationOptions --- list of creation options
-          srcNodata --- source nodata value(s)
-          dstNodata --- output nodata value(s)
-          multithread --- whether to multithread computation and I/O operations
-          tps --- whether to use Thin Plate Spline GCP transformer
-          rpc --- whether to use RPC transformer
-          geoloc --- whether to use GeoLocation array transformer
-          polynomialOrder --- order of polynomial GCP interpolation
-          transformerOptions --- list of transformer options
-          cutlineDSName --- cutline dataset name
-          cutlineLayer --- cutline layer name
-          cutlineWhere --- cutline WHERE clause
-          cutlineSQL --- cutline SQL statement
-          cutlineBlend --- cutline blend distance in pixels
-          cropToCutline --- whether to use cutline extent for output bounds
-          copyMetadata --- whether to copy source metadata
-          metadataConflictValue --- metadata data conflict value
-          setColorInterpretation --- whether to force color interpretation of input bands to output bands
-          overviewLevel --- To specify which overview level of source files must be used
-          callback --- callback method
-          callback_data --- user data for callback
+    """Create a WarpOptions() object that can be passed to gdal.Warp()
+
+    Parameters
+    ----------
+    options:
+        can be be an array of strings, a string or let empty and filled from other keywords.
+    format:
+        output format ("GTiff", etc...)
+    outputBounds:
+        output bounds as (minX, minY, maxX, maxY) in target SRS
+    outputBoundsSRS:
+        SRS in which output bounds are expressed, in the case they are not expressed in dstSRS
+    xRes:
+        output resolution in target SRS
+    yRes:
+        output resolution in target SRS
+    targetAlignedPixels:
+        whether to force output bounds to be multiple of output resolution
+    width:
+        width of the output raster in pixel
+    height:
+        height of the output raster in pixel
+    srcSRS:
+        source SRS
+    dstSRS:
+        output SRS
+    coordinateOperation:
+        coordinate operation as a PROJ string or WKT string
+    srcAlpha:
+        whether to force the last band of the input dataset to be considered as an alpha band
+    dstAlpha:
+        whether to force the creation of an output alpha band
+    outputType:
+        output type (gdalconst.GDT_Byte, etc...)
+    workingType:
+        working type (gdalconst.GDT_Byte, etc...)
+    warpOptions:
+        list of warping options
+    errorThreshold:
+        error threshold for approximation transformer (in pixels)
+    warpMemoryLimit:
+        size of working buffer in MB
+    resampleAlg:
+        resampling mode
+    creationOptions:
+        list of creation options
+    srcNodata:
+        source nodata value(s)
+    dstNodata:
+        output nodata value(s)
+    multithread:
+        whether to multithread computation and I/O operations
+    tps:
+        whether to use Thin Plate Spline GCP transformer
+    rpc:
+        whether to use RPC transformer
+    geoloc:
+        whether to use GeoLocation array transformer
+    polynomialOrder:
+        order of polynomial GCP interpolation
+    transformerOptions:
+        list of transformer options
+    cutlineDSName:
+        cutline dataset name
+    cutlineLayer:
+        cutline layer name
+    cutlineWhere:
+        cutline WHERE clause
+    cutlineSQL:
+        cutline SQL statement
+    cutlineBlend:
+        cutline blend distance in pixels
+    cropToCutline:
+        whether to use cutline extent for output bounds
+    copyMetadata:
+        whether to copy source metadata
+    metadataConflictValue:
+        metadata data conflict value
+    setColorInterpretation:
+        whether to force color interpretation of input bands to output bands
+    overviewLevel:
+        To specify which overview level of source files must be used
+    callback:
+        callback method
+    callback_data:
+        user data for callback
     """
 
 # Only used for tests
     return_option_list = options == '__RETURN_OPTION_LIST__'
     if return_option_list:
         options = []
     else:
@@ -643,22 +750,27 @@
 
     if return_option_list:
         return new_options
 
     return (GDALWarpAppOptions(new_options), callback, callback_data)
 
 def Warp(destNameOrDestDS, srcDSOrSrcDSTab, **kwargs):
-    """ Warp one or several datasets.
-        Arguments are :
-          destNameOrDestDS --- Output dataset name or object
-          srcDSOrSrcDSTab --- an array of Dataset objects or filenames, or a Dataset object or a filename
-        Keyword arguments are :
-          options --- return of gdal.WarpOptions(), string or array of strings
-          other keywords arguments of gdal.WarpOptions()
-        If options is provided as a gdal.WarpOptions() object, other keywords are ignored. """
+    """Warp one or several datasets.
+
+    Parameters
+    ----------
+    destNameOrDestDS:
+        Output dataset name or object
+    srcDSOrSrcDSTab:
+        an array of Dataset objects or filenames, or a Dataset object or a filename
+    kwargs:
+        options: return of gdal.WarpOptions(), string or array of strings,
+        other keywords arguments of gdal.WarpOptions().
+        If options is provided as a gdal.WarpOptions() object, other keywords are ignored.
+    """
 
     if 'options' not in kwargs or isinstance(kwargs['options'], (list, str)):
         (opts, callback, callback_data) = WarpOptions(**kwargs)
     else:
         (opts, callback, callback_data) = kwargs['options']
     if isinstance(srcDSOrSrcDSTab, str):
         srcDSTab = [Open(srcDSOrSrcDSTab)]
@@ -696,46 +808,78 @@
          segmentizeMaxDist= None,
          makeValid=False,
          zField=None,
          resolveDomains=False,
          skipFailures=False,
          limit=None,
          callback=None, callback_data=None):
-    """ Create a VectorTranslateOptions() object that can be passed to gdal.VectorTranslate()
-        Keyword arguments are :
-          options --- can be be an array of strings, a string or let empty and filled from other keywords.
-          format --- output format ("ESRI Shapefile", etc...)
-          accessMode --- None for creation, 'update', 'append', 'overwrite'
-          srcSRS --- source SRS
-          dstSRS --- output SRS (with reprojection if reproject = True)
-          coordinateOperation -- coordinate operation as a PROJ string or WKT string
-          reproject --- whether to do reprojection
-          SQLStatement --- SQL statement to apply to the source dataset
-          SQLDialect --- SQL dialect ('OGRSQL', 'SQLITE', ...)
-          where --- WHERE clause to apply to source layer(s)
-          selectFields --- list of fields to select
-          addFields --- whether to add new fields found in source layers (to be used with accessMode == 'append')
-          forceNullable --- whether to drop NOT NULL constraints on newly created fields
-          emptyStrAsNull --- whether to treat empty string values as NULL
-          spatFilter --- spatial filter as (minX, minY, maxX, maxY) bounding box
-          spatSRS --- SRS in which the spatFilter is expressed. If not specified, it is assumed to be the one of the layer(s)
-          datasetCreationOptions --- list of dataset creation options
-          layerCreationOptions --- list of layer creation options
-          layers --- list of layers to convert
-          layerName --- output layer name
-          geometryType --- output layer geometry type ('POINT', ....)
-          dim --- output dimension ('XY', 'XYZ', 'XYM', 'XYZM', 'layer_dim')
-          segmentizeMaxDist --- maximum distance between consecutive nodes of a line geometry
-          makeValid --- run MakeValid() on geometries
-          zField --- name of field to use to set the Z component of geometries
-          resolveDomains --- whether to create an additional field for each field associated with a coded field domain.
-          skipFailures --- whether to skip failures
-          limit -- maximum number of features to read per layer
-          callback --- callback method
-          callback_data --- user data for callback
+    """Create a VectorTranslateOptions() object that can be passed to gdal.VectorTranslate()
+
+    Parameters
+    ----------
+    options:
+        can be be an array of strings, a string or let empty and filled from other keywords.
+    format:
+        format ("ESRI Shapefile", etc...)
+    accessMode:
+        None for creation, 'update', 'append', 'upsert', 'overwrite'
+    srcSRS:
+        source SRS
+    dstSRS:
+        output SRS (with reprojection if reproject = True)
+    coordinateOperation:
+        coordinate operation as a PROJ string or WKT string
+    reproject:
+        whether to do reprojection
+    SQLStatement:
+        SQL statement to apply to the source dataset
+    SQLDialect:
+        SQL dialect ('OGRSQL', 'SQLITE', ...)
+    where:
+        WHERE clause to apply to source layer(s)
+    selectFields:
+        list of fields to select
+    addFields:
+        whether to add new fields found in source layers (to be used with accessMode == 'append' or 'upsert')
+    forceNullable:
+        whether to drop NOT NULL constraints on newly created fields
+    emptyStrAsNull:
+        whether to treat empty string values as NULL
+    spatFilter:
+        spatial filter as (minX, minY, maxX, maxY) bounding box
+    spatSRS:
+        SRS in which the spatFilter is expressed. If not specified, it is assumed to be the one of the layer(s)
+    datasetCreationOptions:
+        list of dataset creation options
+    layerCreationOptions:
+        list of layer creation options
+    layers:
+        list of layers to convert
+    layerName:
+        output layer name
+    geometryType:
+        output layer geometry type ('POINT', ....)
+    dim:
+        output dimension ('XY', 'XYZ', 'XYM', 'XYZM', 'layer_dim')
+    segmentizeMaxDist:
+        maximum distance between consecutive nodes of a line geometry
+    makeValid:
+        run MakeValid() on geometries
+    zField:
+        name of field to use to set the Z component of geometries
+    resolveDomains:
+        whether to create an additional field for each field associated with a coded field domain.
+    skipFailures:
+        whether to skip failures
+    limit:
+        maximum number of features to read per layer
+    callback:
+        callback method
+    callback_data:
+        user data for callback
     """
     options = [] if options is None else options
 
     if isinstance(options, str):
         new_options = ParseCommandLine(options)
     else:
         new_options = options
@@ -759,14 +903,16 @@
         if accessMode is not None:
             if accessMode == 'update':
                 new_options += ['-update']
             elif accessMode == 'append':
                 new_options += ['-append']
             elif accessMode == 'overwrite':
                 new_options += ['-overwrite']
+            elif accessMode == 'upsert':
+                new_options += ['-upsert']
             else:
                 raise Exception('unhandled accessMode')
         if addFields:
             new_options += ['-addfields']
         if forceNullable:
             new_options += ['-forceNullable']
         if emptyStrAsNull:
@@ -818,22 +964,28 @@
             new_options += ['-limit', str(limit)]
     if callback is not None:
         new_options += ['-progress']
 
     return (GDALVectorTranslateOptions(new_options), callback, callback_data)
 
 def VectorTranslate(destNameOrDestDS, srcDS, **kwargs):
-    """ Convert one vector dataset
-        Arguments are :
-          destNameOrDestDS --- Output dataset name or object
-          srcDS --- a Dataset object or a filename
-        Keyword arguments are :
-          options --- return of gdal.VectorTranslateOptions(), string or array of strings
-          other keywords arguments of gdal.VectorTranslateOptions()
-        If options is provided as a gdal.VectorTranslateOptions() object, other keywords are ignored. """
+    """Convert one vector dataset
+
+    Parameters
+    ----------
+    destNameOrDestDS:
+        Output dataset name or object
+    srcDS:
+        a Dataset object or a filename
+    kwargs:
+        options: return of gdal.VectorTranslateOptions(), string or array of strings,
+        other keywords arguments of gdal.VectorTranslateOptions().
+        If options is provided as a gdal.VectorTranslateOptions() object,
+        other keywords are ignored.
+    """
 
     if 'options' not in kwargs or isinstance(kwargs['options'], (list, str)):
         (opts, callback, callback_data) = VectorTranslateOptions(**kwargs)
     else:
         (opts, callback, callback_data) = kwargs['options']
     if isinstance(srcDS, str):
         srcDS = OpenEx(srcDS, gdalconst.OF_VECTOR)
@@ -846,37 +998,60 @@
 def DEMProcessingOptions(options=None, colorFilename=None, format=None,
               creationOptions=None, computeEdges=False, alg=None, band=1,
               zFactor=None, scale=None, azimuth=None, altitude=None,
               combined=False, multiDirectional=False, igor=False,
               slopeFormat=None, trigonometric=False, zeroForFlat=False,
               addAlpha=None, colorSelection=None,
               callback=None, callback_data=None):
-    """ Create a DEMProcessingOptions() object that can be passed to gdal.DEMProcessing()
-        Keyword arguments are :
-          options --- can be be an array of strings, a string or let empty and filled from other keywords.
-          colorFilename --- (mandatory for "color-relief") name of file that contains palette definition for the "color-relief" processing.
-          format --- output format ("GTiff", etc...)
-          creationOptions --- list of creation options
-          computeEdges --- whether to compute values at raster edges.
-          alg --- 'Horn' (default) or 'ZevenbergenThorne' for hillshade, slope or aspect. 'Wilson' (default) or 'Riley' for TRI
-          band --- source band number to use
-          zFactor --- (hillshade only) vertical exaggeration used to pre-multiply the elevations.
-          scale --- ratio of vertical units to horizontal.
-          azimuth --- (hillshade only) azimuth of the light, in degrees. 0 if it comes from the top of the raster, 90 from the east, ... The default value, 315, should rarely be changed as it is the value generally used to generate shaded maps.
-          altitude ---(hillshade only) altitude of the light, in degrees. 90 if the light comes from above the DEM, 0 if it is raking light.
-          combined --- (hillshade only) whether to compute combined shading, a combination of slope and oblique shading. Only one of combined, multiDirectional and igor can be specified.
-          multiDirectional --- (hillshade only) whether to compute multi-directional shading. Only one of combined, multiDirectional and igor can be specified.
-          igor --- (hillshade only) whether to use Igor's hillshading from Maperitive.  Only one of combined, multiDirectional and igor can be specified.
-          slopeformat --- (slope only) "degree" or "percent".
-          trigonometric --- (aspect only) whether to return trigonometric angle instead of azimuth. Thus 0deg means East, 90deg North, 180deg West, 270deg South.
-          zeroForFlat --- (aspect only) whether to return 0 for flat areas with slope=0, instead of -9999.
-          addAlpha --- adds an alpha band to the output file (only for processing = 'color-relief')
-          colorSelection --- (color-relief only) Determines how color entries are selected from an input value. Can be "nearest_color_entry", "exact_color_entry" or "linear_interpolation". Defaults to "linear_interpolation"
-          callback --- callback method
-          callback_data --- user data for callback
+    """Create a DEMProcessingOptions() object that can be passed to gdal.DEMProcessing()
+
+    Parameters
+    ----------
+    options:
+        can be be an array of strings, a string or let empty and filled from other keywords.
+    colorFilename:
+        (mandatory for "color-relief") name of file that contains palette definition for the "color-relief" processing.
+    format:
+        output format ("GTiff", etc...)
+    creationOptions:
+        list of creation options
+    computeEdges:
+        whether to compute values at raster edges.
+    alg:
+        'Horn' (default) or 'ZevenbergenThorne' for hillshade, slope or aspect. 'Wilson' (default) or 'Riley' for TRI
+    band:
+        source band number to use
+    zFactor:
+        (hillshade only) vertical exaggeration used to pre-multiply the elevations.
+    scale:
+        ratio of vertical units to horizontal.
+    azimuth:
+        (hillshade only) azimuth of the light, in degrees. 0 if it comes from the top of the raster, 90 from the east, ... The default value, 315, should rarely be changed as it is the value generally used to generate shaded maps.
+    altitude:
+        (hillshade only) altitude of the light, in degrees. 90 if the light comes from above the DEM, 0 if it is raking light.
+    combined:
+        (hillshade only) whether to compute combined shading, a combination of slope and oblique shading. Only one of combined, multiDirectional and igor can be specified.
+    multiDirectional:
+        (hillshade only) whether to compute multi-directional shading. Only one of combined, multiDirectional and igor can be specified.
+    igor:
+        (hillshade only) whether to use Igor's hillshading from Maperitive.  Only one of combined, multiDirectional and igor can be specified.
+    slopeformat:
+        (slope only) "degree" or "percent".
+    trigonometric:
+        (aspect only) whether to return trigonometric angle instead of azimuth. Thus 0deg means East, 90deg North, 180deg West, 270deg South.
+    zeroForFlat:
+        (aspect only) whether to return 0 for flat areas with slope=0, instead of -9999.
+    addAlpha:
+        adds an alpha band to the output file (only for processing = 'color-relief')
+    colorSelection:
+        (color-relief only) Determines how color entries are selected from an input value. Can be "nearest_color_entry", "exact_color_entry" or "linear_interpolation". Defaults to "linear_interpolation"
+    callback:
+        callback method
+    callback_data:
+        user data for callback
     """
     options = [] if options is None else options
 
     if isinstance(options, str):
         new_options = ParseCommandLine(options)
     else:
         new_options = options
@@ -921,23 +1096,30 @@
                 raise ValueError("Unsupported value for colorSelection")
         if addAlpha:
             new_options += ['-alpha']
 
     return (GDALDEMProcessingOptions(new_options), colorFilename, callback, callback_data)
 
 def DEMProcessing(destName, srcDS, processing, **kwargs):
-    """ Apply a DEM processing.
-        Arguments are :
-          destName --- Output dataset name
-          srcDS --- a Dataset object or a filename
-          processing --- one of "hillshade", "slope", "aspect", "color-relief", "TRI", "TPI", "Roughness"
-        Keyword arguments are :
-          options --- return of gdal.DEMProcessingOptions(), string or array of strings
-          other keywords arguments of gdal.DEMProcessingOptions()
-        If options is provided as a gdal.DEMProcessingOptions() object, other keywords are ignored. """
+    """Apply a DEM processing.
+
+    Parameters
+    ----------
+    destName:
+        Output dataset name
+    srcDS:
+        a Dataset object or a filename
+    processing:
+        one of "hillshade", "slope", "aspect", "color-relief", "TRI", "TPI", "Roughness"
+    kwargs:
+        options: return of gdal.DEMProcessingOptions(), string or array of strings,
+        other keywords arguments of gdal.DEMProcessingOptions().
+        If options is provided as a gdal.DEMProcessingOptions() object,
+        other keywords are ignored.
+    """
 
     if 'options' not in kwargs or isinstance(kwargs['options'], (list, str)):
         (opts, colorFilename, callback, callback_data) = DEMProcessingOptions(**kwargs)
     else:
         (opts, colorFilename, callback, callback_data) = kwargs['options']
     if isinstance(srcDS, str):
         srcDS = Open(srcDS)
@@ -945,27 +1127,40 @@
     return DEMProcessingInternal(destName, srcDS, processing, colorFilename, opts, callback, callback_data)
 
 
 def NearblackOptions(options=None, format=None,
          creationOptions=None, white = False, colors=None,
          maxNonBlack=None, nearDist=None, setAlpha = False, setMask = False,
          callback=None, callback_data=None):
-    """ Create a NearblackOptions() object that can be passed to gdal.Nearblack()
-        Keyword arguments are :
-          options --- can be be an array of strings, a string or let empty and filled from other keywords.
-          format --- output format ("GTiff", etc...)
-          creationOptions --- list of creation options
-          white --- whether to search for nearly white (255) pixels instead of nearly black pixels.
-          colors --- list of colors  to search for, e.g. ((0,0,0),(255,255,255)). The pixels that are considered as the collar are set to 0
-          maxNonBlack --- number of non-black (or other searched colors specified with white / colors) pixels that can be encountered before the giving up search inwards. Defaults to 2.
-          nearDist --- select how far from black, white or custom colors the pixel values can be and still considered near black, white or custom color.  Defaults to 15.
-          setAlpha --- adds an alpha band to the output file.
-          setMask --- adds a mask band to the output file.
-          callback --- callback method
-          callback_data --- user data for callback
+    """Create a NearblackOptions() object that can be passed to gdal.Nearblack()
+
+    Parameters
+    ----------
+    options:
+        can be be an array of strings, a string or let empty and filled from other keywords.
+    format:
+        output format ("GTiff", etc...)
+    creationOptions:
+        list of creation options
+    white:
+        whether to search for nearly white (255) pixels instead of nearly black pixels.
+    colors:
+        list of colors  to search for, e.g. ((0,0,0),(255,255,255)). The pixels that are considered as the collar are set to 0
+    maxNonBlack:
+        number of non-black (or other searched colors specified with white / colors) pixels that can be encountered before the giving up search inwards. Defaults to 2.
+    nearDist:
+        select how far from black, white or custom colors the pixel values can be and still considered near black, white or custom color.  Defaults to 15.
+    setAlpha:
+        adds an alpha band to the output file.
+    setMask:
+        adds a mask band to the output file.
+    callback:
+        callback method
+    callback_data:
+        user data for callback
     """
     options = [] if options is None else options
 
     if isinstance(options, str):
         new_options = ParseCommandLine(options)
     else:
         new_options = options
@@ -992,22 +1187,27 @@
             new_options += ['-setalpha']
         if setMask:
             new_options += ['-setmask']
 
     return (GDALNearblackOptions(new_options), callback, callback_data)
 
 def Nearblack(destNameOrDestDS, srcDS, **kwargs):
-    """ Convert nearly black/white borders to exact value.
-        Arguments are :
-          destNameOrDestDS --- Output dataset name or object
-          srcDS --- a Dataset object or a filename
-        Keyword arguments are :
-          options --- return of gdal.NearblackOptions(), string or array of strings
-          other keywords arguments of gdal.NearblackOptions()
-        If options is provided as a gdal.NearblackOptions() object, other keywords are ignored. """
+    """Convert nearly black/white borders to exact value.
+
+    Parameters
+    ----------
+    destNameOrDestDS:
+        Output dataset name or object
+    srcDS:
+        a Dataset object or a filename
+    kwargs:
+        options: return of gdal.NearblackOptions(), string or array of strings,
+        other keywords arguments of gdal.NearblackOptions().
+        If options is provided as a gdal.NearblackOptions() object, other keywords are ignored.
+    """
 
     if 'options' not in kwargs or isinstance(kwargs['options'], (list, str)):
         (opts, callback, callback_data) = NearblackOptions(**kwargs)
     else:
         (opts, callback, callback_data) = kwargs['options']
     if isinstance(srcDS, str):
         srcDS = OpenEx(srcDS)
@@ -1031,34 +1231,61 @@
               where=None,
               spatFilter=None,
               zfield=None,
               z_increase=None,
               z_multiply=None,
               callback=None, callback_data=None):
     """ Create a GridOptions() object that can be passed to gdal.Grid()
-        Keyword arguments are :
-          options --- can be be an array of strings, a string or let empty and filled from other keywords.
-          format --- output format ("GTiff", etc...)
-          outputType --- output type (gdalconst.GDT_Byte, etc...)
-          width --- width of the output raster in pixel
-          height --- height of the output raster in pixel
-          creationOptions --- list of creation options
-          outputBounds --- assigned output bounds: [ulx, uly, lrx, lry]
-          outputSRS --- assigned output SRS
-          noData --- nodata value
-          algorithm --- e.g "invdist:power=2.0:smoothing=0.0:radius1=0.0:radius2=0.0:angle=0.0:max_points=0:min_points=0:nodata=0.0"
-          layers --- list of layers to convert
-          SQLStatement --- SQL statement to apply to the source dataset
-          where --- WHERE clause to apply to source layer(s)
-          spatFilter --- spatial filter as (minX, minY, maxX, maxY) bounding box
-          zfield --- Identifies an attribute field on the features to be used to get a Z value from. This value overrides Z value read from feature geometry record.
-          z_increase --- Addition to the attribute field on the features to be used to get a Z value from. The addition should be the same unit as Z value. The result value will be Z value + Z increase value. The default value is 0.
-          z_multiply - Multiplication ratio for Z field. This can be used for shift from e.g. foot to meters or from  elevation to deep. The result value will be (Z value + Z increase value) * Z multiply value.  The default value is 1.
-          callback --- callback method
-          callback_data --- user data for callback
+
+    Parameters
+    ----------
+    options:
+        can be be an array of strings, a string or let empty and filled from other keywords.
+    format:
+        output format ("GTiff", etc...)
+    outputType:
+        output type (gdalconst.GDT_Byte, etc...)
+    width:
+        width of the output raster in pixel
+    height:
+        height of the output raster in pixel
+    creationOptions:
+        list of creation options
+    outputBounds:
+        assigned output bounds:
+        [ulx, uly, lrx, lry]
+    outputSRS:
+        assigned output SRS
+    noData:
+        nodata value
+    algorithm:
+        e.g "invdist:power=2.0:smoothing=0.0:radius1=0.0:radius2=0.0:angle=0.0:max_points=0:min_points=0:nodata=0.0"
+    layers:
+        list of layers to convert
+    SQLStatement:
+        SQL statement to apply to the source dataset
+    where:
+        WHERE clause to apply to source layer(s)
+    spatFilter:
+        spatial filter as (minX, minY, maxX, maxY) bounding box
+    zfield:
+        Identifies an attribute field on the features to be used to get a Z value from.
+        This value overrides Z value read from feature geometry record.
+    z_increase:
+        Addition to the attribute field on the features to be used to get a Z value from.
+        The addition should be the same unit as Z value. The result value will be
+        Z value + Z increase value. The default value is 0.
+    z_multiply:
+        Multiplication ratio for Z field. This can be used for shift from e.g. foot to meters
+        or from  elevation to deep. The result value will be
+        (Z value + Z increase value) * Z multiply value. The default value is 1.
+    callback:
+        callback method
+    callback_data:
+        user data for callback
     """
     options = [] if options is None else options
 
     if isinstance(options, str):
         new_options = ParseCommandLine(options)
     else:
         new_options = options
@@ -1096,21 +1323,26 @@
         if spatFilter is not None:
             new_options += ['-spat', str(spatFilter[0]), str(spatFilter[1]), str(spatFilter[2]), str(spatFilter[3])]
 
     return (GDALGridOptions(new_options), callback, callback_data)
 
 def Grid(destName, srcDS, **kwargs):
     """ Create raster from the scattered data.
-        Arguments are :
-          destName --- Output dataset name
-          srcDS --- a Dataset object or a filename
-        Keyword arguments are :
-          options --- return of gdal.GridOptions(), string or array of strings
-          other keywords arguments of gdal.GridOptions()
-        If options is provided as a gdal.GridOptions() object, other keywords are ignored. """
+
+    Parameters
+    ----------
+    destName:
+        Output dataset name
+    srcDS:
+        a Dataset object or a filename
+    kwargs:
+        options: return of gdal.GridOptions(), string or array of strings,
+        other keywords arguments of gdal.GridOptions()
+        If options is provided as a gdal.GridOptions() object, other keywords are ignored.
+    """
 
     if 'options' not in kwargs or isinstance(kwargs['options'], (list, str)):
         (opts, callback, callback_data) = GridOptions(**kwargs)
     else:
         (opts, callback, callback_data) = kwargs['options']
     if isinstance(srcDS, str):
         srcDS = OpenEx(srcDS, gdalconst.OF_VECTOR)
@@ -1125,43 +1357,83 @@
          width=None, height=None,
          xRes=None, yRes=None, targetAlignedPixels=False,
          bands=None, inverse=False, allTouched=False,
          burnValues=None, attribute=None, useZ=False, layers=None,
          SQLStatement=None, SQLDialect=None, where=None, optim=None,
          add=None,
          callback=None, callback_data=None):
-    """ Create a RasterizeOptions() object that can be passed to gdal.Rasterize()
-        Keyword arguments are :
-          options --- can be be an array of strings, a string or let empty and filled from other keywords.
-          format --- output format ("GTiff", etc...)
-          outputType --- output type (gdalconst.GDT_Byte, etc...)
-          creationOptions --- list of creation options
-          outputBounds --- assigned output bounds: [minx, miny, maxx, maxy]
-          outputSRS --- assigned output SRS
-          transformerOptions --- list of transformer options
-          width --- width of the output raster in pixel
-          height --- height of the output raster in pixel
-          xRes, yRes --- output resolution in target SRS
-          targetAlignedPixels --- whether to force output bounds to be multiple of output resolution
-          noData --- nodata value
-          initValues --- Value or list of values to pre-initialize the output image bands with.  However, it is not marked as the nodata value in the output file.  If only one value is given, the same value is used in all the bands.
-          bands --- list of output bands to burn values into
-          inverse --- whether to invert rasterization, i.e. burn the fixed burn value, or the burn value associated  with the first feature into all parts of the image not inside the provided a polygon.
-          allTouched -- whether to enable the ALL_TOUCHED rasterization option so that all pixels touched by lines or polygons will be updated, not just those on the line render path, or whose center point is within the polygon.
-          burnValues -- list of fixed values to burn into each band for all objects. Excusive with attribute.
-          attribute --- identifies an attribute field on the features to be used for a burn-in value. The value will be burned into all output bands. Excusive with burnValues.
-          useZ --- whether to indicate that a burn value should be extracted from the "Z" values of the feature. These values are added to the burn value given by burnValues or attribute if provided. As of now, only points and lines are drawn in 3D.
-          layers --- list of layers from the datasource that will be used for input features.
-          SQLStatement --- SQL statement to apply to the source dataset
-          SQLDialect --- SQL dialect ('OGRSQL', 'SQLITE', ...)
-          where --- WHERE clause to apply to source layer(s)
-          optim --- optimization mode ('RASTER', 'VECTOR')
-          add --- set to True to use additive mode instead of replace when burning values
-          callback --- callback method
-          callback_data --- user data for callback
+    """Create a RasterizeOptions() object that can be passed to gdal.Rasterize()
+
+    Parameters
+    ----------
+    options:
+        can be be an array of strings, a string or let empty and filled from other keywords.
+    format:
+        output format ("GTiff", etc...)
+    outputType:
+        output type (gdalconst.GDT_Byte, etc...)
+    creationOptions:
+        list of creation options
+    outputBounds:
+        assigned output bounds:
+        [minx, miny, maxx, maxy]
+    outputSRS:
+        assigned output SRS
+    transformerOptions:
+        list of transformer options
+    width:
+        width of the output raster in pixel
+    height:
+        height of the output raster in pixel
+    xRes, yRes:
+        output resolution in target SRS
+    targetAlignedPixels:
+        whether to force output bounds to be multiple of output resolution
+    noData:
+        nodata value
+    initValues:
+        Value or list of values to pre-initialize the output image bands with.
+         However, it is not marked as the nodata value in the output file.
+          If only one value is given, the same value is used in all the bands.
+    bands:
+        list of output bands to burn values into
+    inverse:
+        whether to invert rasterization, i.e. burn the fixed burn value, or the
+        burn value associated with the first feature into all parts of the image
+        not inside the provided a polygon.
+    allTouched:
+        whether to enable the ALL_TOUCHED rasterization option so that all pixels
+        touched by lines or polygons will be updated, not just those on the line
+        render path, or whose center point is within the polygon.
+    burnValues:
+        list of fixed values to burn into each band for all objects.
+        Excusive with attribute.
+    attribute:
+        identifies an attribute field on the features to be used for a burn-in value.
+        The value will be burned into all output bands. Excusive with burnValues.
+    useZ:
+        whether to indicate that a burn value should be extracted from the "Z" values
+        of the feature. These values are added to the burn value given by burnValues
+        or attribute if provided. As of now, only points and lines are drawn in 3D.
+    layers:
+        list of layers from the datasource that will be used for input features.
+    SQLStatement:
+        SQL statement to apply to the source dataset
+    SQLDialect:
+        SQL dialect ('OGRSQL', 'SQLITE', ...)
+    where:
+        WHERE clause to apply to source layer(s)
+    optim:
+        optimization mode ('RASTER', 'VECTOR')
+    add:
+        set to True to use additive mode instead of replace when burning values
+    callback:
+        callback method
+    callback_data:
+        user data for callback
     """
     options = [] if options is None else options
 
     if isinstance(options, str):
         new_options = ParseCommandLine(options)
     else:
         new_options = options
@@ -1228,22 +1500,27 @@
             new_options += ['-optim', str(optim)]
         if add:
             new_options += ['-add']
 
     return (GDALRasterizeOptions(new_options), callback, callback_data)
 
 def Rasterize(destNameOrDestDS, srcDS, **kwargs):
-    """ Burns vector geometries into a raster
-        Arguments are :
-          destNameOrDestDS --- Output dataset name or object
-          srcDS --- a Dataset object or a filename
-        Keyword arguments are :
-          options --- return of gdal.RasterizeOptions(), string or array of strings
-          other keywords arguments of gdal.RasterizeOptions()
-        If options is provided as a gdal.RasterizeOptions() object, other keywords are ignored. """
+    """Burns vector geometries into a raster
+
+    Parameters
+    ----------
+    destNameOrDestDS:
+        Output dataset name or object
+    srcDS:
+        a Dataset object or a filename
+    kwargs:
+        options: return of gdal.RasterizeOptions(), string or array of strings,
+        other keywords arguments of gdal.RasterizeOptions()
+        If options is provided as a gdal.RasterizeOptions() object, other keywords are ignored.
+    """
 
     if 'options' not in kwargs or isinstance(kwargs['options'], (list, str)):
         (opts, callback, callback_data) = RasterizeOptions(**kwargs)
     else:
         (opts, callback, callback_data) = kwargs['options']
     if isinstance(srcDS, str):
         srcDS = OpenEx(srcDS, gdalconst.OF_VECTOR)
@@ -1253,46 +1530,69 @@
     else:
         return wrapper_GDALRasterizeDestDS(destNameOrDestDS, srcDS, opts, callback, callback_data)
 
 
 def BuildVRTOptions(options=None,
                     resolution=None,
                     outputBounds=None,
-                    xRes=None, yRes=None,
+                    xRes=None,
+                    yRes=None,
                     targetAlignedPixels=None,
                     separate=None,
                     bandList=None,
                     addAlpha=None,
                     resampleAlg=None,
                     outputSRS=None,
                     allowProjectionDifference=None,
                     srcNodata=None,
                     VRTNodata=None,
                     hideNodata=None,
                     strict=False,
                     callback=None, callback_data=None):
-    """ Create a BuildVRTOptions() object that can be passed to gdal.BuildVRT()
-        Keyword arguments are :
-          options --- can be be an array of strings, a string or let empty and filled from other keywords..
-          resolution --- 'highest', 'lowest', 'average', 'user'.
-          outputBounds --- output bounds as (minX, minY, maxX, maxY) in target SRS.
-          xRes, yRes --- output resolution in target SRS.
-          targetAlignedPixels --- whether to force output bounds to be multiple of output resolution.
-          separate --- whether each source file goes into a separate stacked band in the VRT band.
-          bandList --- array of band numbers (index start at 1).
-          addAlpha --- whether to add an alpha mask band to the VRT when the source raster have none.
-          resampleAlg --- resampling mode.
-          outputSRS --- assigned output SRS.
-          allowProjectionDifference --- whether to accept input datasets have not the same projection. Note: they will *not* be reprojected.
-          srcNodata --- source nodata value(s).
-          VRTNodata --- nodata values at the VRT band level.
-          hideNodata --- whether to make the VRT band not report the NoData value.
-          strict --- set to True if warnings should be failures
-          callback --- callback method.
-          callback_data --- user data for callback.
+    """Create a BuildVRTOptions() object that can be passed to gdal.BuildVRT()
+
+    Parameters
+    ----------
+    options:l
+        can be be an array of strings, a string or let empty and filled from other keywords.
+    resolution:
+        'highest', 'lowest', 'average', 'user'.
+    outputBounds:l
+        output bounds as (minX, minY, maxX, maxY) in target SRS.
+    xRes:
+        output resolution in target SRS.
+    yRes:
+        output resolution in target SRS.
+    targetAlignedPixels:
+        whether to force output bounds to be multiple of output resolution.
+    separate:
+        whether each source file goes into a separate stacked band in the VRT band.
+    bandList:
+        array of band numbers (index start at 1).
+    addAlpha:
+        whether to add an alpha mask band to the VRT when the source raster have none.
+    resampleAlg:
+        resampling mode.
+    outputSRS:
+        assigned output SRS.
+    allowProjectionDifference:
+        whether to accept input datasets have not the same projection.
+        Note: they will *not* be reprojected.
+    srcNodata:
+        source nodata value(s).
+    VRTNodata:
+        nodata values at the VRT band level.
+    hideNodata:
+        whether to make the VRT band not report the NoData value.
+    strict:
+        set to True if warnings should be failures
+    callback:
+        callback method.
+    callback_data:
+        user data for callback.
     """
 
 # Only used for tests
     return_option_list = options == '__RETURN_OPTION_LIST__'
     if return_option_list:
         options = []
     else:
@@ -1337,23 +1637,28 @@
 
     if return_option_list:
         return new_options
 
     return (GDALBuildVRTOptions(new_options), callback, callback_data)
 
 def BuildVRT(destName, srcDSOrSrcDSTab, **kwargs):
-    """ Build a VRT from a list of datasets.
-        Arguments are :
-          destName --- Output dataset name
-          srcDSOrSrcDSTab --- an array of Dataset objects or filenames, or a Dataset object or a filename
-        Keyword arguments are :
-          options --- return of gdal.BuildVRTOptions(), string or array of strings
-          other keywords arguments of gdal.BuildVRTOptions()
-        If options is provided as a gdal.BuildVRTOptions() object, other keywords are ignored. """
+    """Build a VRT from a list of datasets.
 
+    Parameters
+    ----------
+    destName:
+        Output dataset name.
+    srcDSOrSrcDSTab:
+        An array of Dataset objects or filenames, or a Dataset object or a filename.
+    kwargs:
+        options: return of gdal.BuildVRTOptions(), string or array of strings,
+        other keywords arguments of gdal.BuildVRTOptions().
+        If options is provided as a gdal.BuildVRTOptions() object,
+        other keywords are ignored.
+    """
     if 'options' not in kwargs or isinstance(kwargs['options'], (list, str)):
         (opts, callback, callback_data) = BuildVRTOptions(**kwargs)
     else:
         (opts, callback, callback_data) = kwargs['options']
 
     srcDSTab = []
     srcDSNamesTab = []
@@ -1375,25 +1680,40 @@
     else:
         return BuildVRTInternalNames(destName, srcDSNamesTab, opts, callback, callback_data)
 
 
 def MultiDimTranslateOptions(options=None, format=None, creationOptions=None,
          arraySpecs=None, groupSpecs=None, subsetSpecs=None, scaleAxesSpecs=None,
          callback=None, callback_data=None):
-    """ Create a MultiDimTranslateOptions() object that can be passed to gdal.MultiDimTranslate()
-        Keyword arguments are :
-          options --- can be be an array of strings, a string or let empty and filled from other keywords.
-          format --- output format ("GTiff", etc...)
-          creationOptions --- list of creation options
-          arraySpecs -- list of array specifications, each of them being an array name or "name={src_array_name},dstname={dst_name},transpose=[1,0],view=[:,::-1]"
-          groupSpecs -- list of group specifications, each of them being a group name or "name={src_array_name},dstname={dst_name},recursive=no"
-          subsetSpecs -- list of subset specifications, each of them being like "{dim_name}({min_val},{max_val})" or "{dim_name}({slice_va})"
-          scaleAxesSpecs -- list of dimension scaling specifications, each of them being like "{dim_name}({scale_factor})"
-          callback --- callback method
-          callback_data --- user data for callback
+    """Create a MultiDimTranslateOptions() object that can be passed to gdal.MultiDimTranslate()
+
+    Parameters
+    ----------
+    options:
+        can be be an array of strings, a string or let empty and filled from other keywords.
+    format:
+        output format ("GTiff", etc...)
+    creationOptions:
+        list of creation options
+    arraySpecs:
+        list of array specifications, each of them being an array name or
+        "name={src_array_name},dstname={dst_name},transpose=[1,0],view=[:,::-1]"
+    groupSpecs:
+        list of group specifications, each of them being a group name or
+        "name={src_array_name},dstname={dst_name},recursive=no"
+    subsetSpecs:
+        list of subset specifications, each of them being like
+        "{dim_name}({min_val},{max_val})" or "{dim_name}({slice_va})"
+    scaleAxesSpecs:
+        list of dimension scaling specifications, each of them being like
+        "{dim_name}({scale_factor})"
+    callback:
+        callback method
+    callback_data:
+        user data for callback
     """
     options = [] if options is None else options
 
     if isinstance(options, str):
         new_options = ParseCommandLine(options)
     else:
         new_options = options
@@ -1414,22 +1734,28 @@
         if scaleAxesSpecs is not None:
             for s in scaleAxesSpecs:
                 new_options += ['-scaleaxes', s]
 
     return (GDALMultiDimTranslateOptions(new_options), callback, callback_data)
 
 def MultiDimTranslate(destName, srcDSOrSrcDSTab, **kwargs):
-    """ MultiDimTranslate one or several datasets.
-        Arguments are :
-          destName --- Output dataset name
-          srcDSOrSrcDSTab --- an array of Dataset objects or filenames, or a Dataset object or a filename
-        Keyword arguments are :
-          options --- return of gdal.MultiDimTranslateOptions(), string or array of strings
-          other keywords arguments of gdal.MultiDimTranslateOptions()
-        If options is provided as a gdal.MultiDimTranslateOptions() object, other keywords are ignored. """
+    """MultiDimTranslate one or several datasets.
+
+    Parameters
+    ----------
+    destName:
+        Output dataset name
+    srcDSOrSrcDSTab:
+        an array of Dataset objects or filenames, or a Dataset object or a filename
+    kwargs:
+        options: return of gdal.MultiDimTranslateOptions(), string or array of strings
+        other keywords arguments of gdal.MultiDimTranslateOptions().
+        If options is provided as a gdal.MultiDimTranslateOptions() object,
+        other keywords are ignored.
+    """
 
     if 'options' not in kwargs or isinstance(kwargs['options'], (list, str)):
         (opts, callback, callback_data) = MultiDimTranslateOptions(**kwargs)
     else:
         (opts, callback, callback_data) = kwargs['options']
     if isinstance(srcDSOrSrcDSTab, str):
         srcDSTab = [OpenEx(srcDSOrSrcDSTab, OF_VERBOSE_ERROR | OF_RASTER | OF_MULTIDIM_RASTER)]
@@ -1495,115 +1821,115 @@
 
     from warnings import warn
     warn('ApplyVerticalShiftGrid() will be removed in GDAL 4.0', DeprecationWarning)
     return _ApplyVerticalShiftGrid(*args, **kwargs)
 
 
 
-def Debug(*args):
+def Debug(*args) -> "void":
     r"""Debug(char const * msg_class, char const * message)"""
     return _gdal.Debug(*args)
 
-def SetErrorHandler(*args):
+def SetErrorHandler(*args) -> "CPLErr":
     r"""SetErrorHandler(CPLErrorHandler pfnErrorHandler=0) -> CPLErr"""
     return _gdal.SetErrorHandler(*args)
 
-def SetCurrentErrorHandlerCatchDebug(*args):
+def SetCurrentErrorHandlerCatchDebug(*args) -> "void":
     r"""SetCurrentErrorHandlerCatchDebug(int bCatchDebug)"""
     return _gdal.SetCurrentErrorHandlerCatchDebug(*args)
 
-def PushErrorHandler(*args):
+def PushErrorHandler(*args) -> "CPLErr":
     r"""PushErrorHandler(CPLErrorHandler pfnErrorHandler=0) -> CPLErr"""
     return _gdal.PushErrorHandler(*args)
 
-def PopErrorHandler(*args):
+def PopErrorHandler(*args) -> "void":
     r"""PopErrorHandler()"""
     return _gdal.PopErrorHandler(*args)
 
-def Error(*args):
+def Error(*args) -> "void":
     r"""Error(CPLErr msg_class=CE_Failure, int err_code=0, char const * msg="error")"""
     return _gdal.Error(*args)
 
-def GOA2GetAuthorizationURL(*args):
+def GOA2GetAuthorizationURL(*args) -> "retStringAndCPLFree *":
     r"""GOA2GetAuthorizationURL(char const * pszScope) -> retStringAndCPLFree *"""
     return _gdal.GOA2GetAuthorizationURL(*args)
 
-def GOA2GetRefreshToken(*args):
+def GOA2GetRefreshToken(*args) -> "retStringAndCPLFree *":
     r"""GOA2GetRefreshToken(char const * pszAuthToken, char const * pszScope) -> retStringAndCPLFree *"""
     return _gdal.GOA2GetRefreshToken(*args)
 
-def GOA2GetAccessToken(*args):
+def GOA2GetAccessToken(*args) -> "retStringAndCPLFree *":
     r"""GOA2GetAccessToken(char const * pszRefreshToken, char const * pszScope) -> retStringAndCPLFree *"""
     return _gdal.GOA2GetAccessToken(*args)
 
-def ErrorReset(*args):
+def ErrorReset(*args) -> "void":
     r"""ErrorReset()"""
     return _gdal.ErrorReset(*args)
 
-def wrapper_EscapeString(*args, **kwargs):
+def wrapper_EscapeString(*args, **kwargs) -> "retStringAndCPLFree *":
     r"""wrapper_EscapeString(int len, int scheme=CPLES_SQL) -> retStringAndCPLFree *"""
     return _gdal.wrapper_EscapeString(*args, **kwargs)
 
-def EscapeBinary(*args, **kwargs):
+def EscapeBinary(*args, **kwargs) -> "char **":
     r"""EscapeBinary(int len, int scheme=CPLES_SQL)"""
     return _gdal.EscapeBinary(*args, **kwargs)
 
-def GetLastErrorNo(*args):
+def GetLastErrorNo(*args) -> "int":
     r"""GetLastErrorNo() -> int"""
     return _gdal.GetLastErrorNo(*args)
 
-def GetLastErrorType(*args):
+def GetLastErrorType(*args) -> "int":
     r"""GetLastErrorType() -> int"""
     return _gdal.GetLastErrorType(*args)
 
-def GetLastErrorMsg(*args):
+def GetLastErrorMsg(*args) -> "char const *":
     r"""GetLastErrorMsg() -> char const *"""
     return _gdal.GetLastErrorMsg(*args)
 
-def GetErrorCounter(*args):
+def GetErrorCounter(*args) -> "unsigned int":
     r"""GetErrorCounter() -> unsigned int"""
     return _gdal.GetErrorCounter(*args)
 
-def VSIGetLastErrorNo(*args):
+def VSIGetLastErrorNo(*args) -> "int":
     r"""VSIGetLastErrorNo() -> int"""
     return _gdal.VSIGetLastErrorNo(*args)
 
-def VSIGetLastErrorMsg(*args):
+def VSIGetLastErrorMsg(*args) -> "char const *":
     r"""VSIGetLastErrorMsg() -> char const *"""
     return _gdal.VSIGetLastErrorMsg(*args)
 
-def VSIErrorReset(*args):
+def VSIErrorReset(*args) -> "void":
     r"""VSIErrorReset()"""
     return _gdal.VSIErrorReset(*args)
 
-def PushFinderLocation(*args):
+def PushFinderLocation(*args) -> "void":
     r"""PushFinderLocation(char const * utf8_path)"""
     return _gdal.PushFinderLocation(*args)
 
-def PopFinderLocation(*args):
+def PopFinderLocation(*args) -> "void":
     r"""PopFinderLocation()"""
     return _gdal.PopFinderLocation(*args)
 
-def FinderClean(*args):
+def FinderClean(*args) -> "void":
     r"""FinderClean()"""
     return _gdal.FinderClean(*args)
 
-def FindFile(*args):
+def FindFile(*args) -> "char const *":
     r"""FindFile(char const * pszClass, char const * utf8_path) -> char const *"""
     return _gdal.FindFile(*args)
 
-def ReadDir(*args):
+def ReadDir(*args) -> "char **":
     r"""ReadDir(char const * utf8_path, int nMaxFiles=0) -> char **"""
     return _gdal.ReadDir(*args)
 
-def ReadDirRecursive(*args):
+def ReadDirRecursive(*args) -> "char **":
     r"""ReadDirRecursive(char const * utf8_path) -> char **"""
     return _gdal.ReadDirRecursive(*args)
 
-def OpenDir(*args):
+def OpenDir(*args) -> "VSIDIR *":
     r"""OpenDir(char const * utf8_path, int nRecurseDepth=-1, char ** options=None) -> VSIDIR *"""
     return _gdal.OpenDir(*args)
 class DirEntry(object):
     r"""Proxy of C++ DirEntry class."""
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
@@ -1617,123 +1943,135 @@
     extra = property(_gdal.DirEntry_extra_get, doc=r"""extra : p.p.char""")
 
     def __init__(self, *args):
         r"""__init__(DirEntry self, DirEntry entryIn) -> DirEntry"""
         _gdal.DirEntry_swiginit(self, _gdal.new_DirEntry(*args))
     __swig_destroy__ = _gdal.delete_DirEntry
 
-    def IsDirectory(self, *args):
+    def IsDirectory(self, *args) -> "bool":
         r"""IsDirectory(DirEntry self) -> bool"""
         return _gdal.DirEntry_IsDirectory(self, *args)
 
 # Register DirEntry in _gdal:
 _gdal.DirEntry_swigregister(DirEntry)
 
 
-def GetNextDirEntry(*args):
+def GetNextDirEntry(*args) -> "DirEntry *":
     r"""GetNextDirEntry(VSIDIR * dir) -> DirEntry"""
     return _gdal.GetNextDirEntry(*args)
 
-def CloseDir(*args):
+def CloseDir(*args) -> "void":
     r"""CloseDir(VSIDIR * dir)"""
     return _gdal.CloseDir(*args)
 
-def SetConfigOption(*args):
+def SetConfigOption(*args) -> "void":
     r"""SetConfigOption(char const * pszKey, char const * pszValue)"""
     return _gdal.SetConfigOption(*args)
 
-def SetThreadLocalConfigOption(*args):
+def SetThreadLocalConfigOption(*args) -> "void":
     r"""SetThreadLocalConfigOption(char const * pszKey, char const * pszValue)"""
     return _gdal.SetThreadLocalConfigOption(*args)
 
-def GetConfigOption(*args):
+def GetConfigOption(*args) -> "char const *":
     r"""GetConfigOption(char const * pszKey, char const * pszDefault=None) -> char const *"""
     return _gdal.GetConfigOption(*args)
 
-def GetThreadLocalConfigOption(*args):
+def GetThreadLocalConfigOption(*args) -> "char const *":
     r"""GetThreadLocalConfigOption(char const * pszKey, char const * pszDefault=None) -> char const *"""
     return _gdal.GetThreadLocalConfigOption(*args)
 
-def SetCredential(*args):
+def SetPathSpecificOption(*args) -> "void":
+    r"""SetPathSpecificOption(char const * pszPathPrefix, char const * pszKey, char const * pszValue)"""
+    return _gdal.SetPathSpecificOption(*args)
+
+def SetCredential(*args) -> "void":
     r"""SetCredential(char const * pszPathPrefix, char const * pszKey, char const * pszValue)"""
     return _gdal.SetCredential(*args)
 
-def GetCredential(*args):
+def GetCredential(*args) -> "char const *":
     r"""GetCredential(char const * pszPathPrefix, char const * pszKey, char const * pszDefault=None) -> char const *"""
     return _gdal.GetCredential(*args)
 
-def ClearCredentials(*args):
+def GetPathSpecificOption(*args) -> "char const *":
+    r"""GetPathSpecificOption(char const * pszPathPrefix, char const * pszKey, char const * pszDefault=None) -> char const *"""
+    return _gdal.GetPathSpecificOption(*args)
+
+def ClearCredentials(*args) -> "void":
     r"""ClearCredentials(char const * pszPathPrefix=None)"""
     return _gdal.ClearCredentials(*args)
 
-def CPLBinaryToHex(*args):
+def ClearPathSpecificOptions(*args) -> "void":
+    r"""ClearPathSpecificOptions(char const * pszPathPrefix=None)"""
+    return _gdal.ClearPathSpecificOptions(*args)
+
+def CPLBinaryToHex(*args) -> "retStringAndCPLFree *":
     r"""CPLBinaryToHex(int nBytes) -> retStringAndCPLFree *"""
     return _gdal.CPLBinaryToHex(*args)
 
-def CPLHexToBinary(*args):
+def CPLHexToBinary(*args) -> "GByte *":
     r"""CPLHexToBinary(char const * pszHex, int * pnBytes) -> GByte *"""
     return _gdal.CPLHexToBinary(*args)
 
-def FileFromMemBuffer(*args):
+def FileFromMemBuffer(*args) -> "void":
     r"""FileFromMemBuffer(char const * utf8_path, GIntBig nBytes)"""
     return _gdal.FileFromMemBuffer(*args)
 
-def Unlink(*args):
+def Unlink(*args) -> "VSI_RETVAL":
     r"""Unlink(char const * utf8_path) -> VSI_RETVAL"""
     return _gdal.Unlink(*args)
 
-def UnlinkBatch(*args):
+def UnlinkBatch(*args) -> "bool":
     r"""UnlinkBatch(char ** files) -> bool"""
     return _gdal.UnlinkBatch(*args)
 
-def HasThreadSupport(*args):
+def HasThreadSupport(*args) -> "int":
     r"""HasThreadSupport() -> int"""
     return _gdal.HasThreadSupport(*args)
 
-def Mkdir(*args):
+def Mkdir(*args) -> "VSI_RETVAL":
     r"""Mkdir(char const * utf8_path, int mode) -> VSI_RETVAL"""
     return _gdal.Mkdir(*args)
 
-def Rmdir(*args):
+def Rmdir(*args) -> "VSI_RETVAL":
     r"""Rmdir(char const * utf8_path) -> VSI_RETVAL"""
     return _gdal.Rmdir(*args)
 
-def MkdirRecursive(*args):
+def MkdirRecursive(*args) -> "VSI_RETVAL":
     r"""MkdirRecursive(char const * utf8_path, int mode) -> VSI_RETVAL"""
     return _gdal.MkdirRecursive(*args)
 
-def RmdirRecursive(*args):
+def RmdirRecursive(*args) -> "VSI_RETVAL":
     r"""RmdirRecursive(char const * utf8_path) -> VSI_RETVAL"""
     return _gdal.RmdirRecursive(*args)
 
-def Rename(*args):
+def Rename(*args) -> "VSI_RETVAL":
     r"""Rename(char const * pszOld, char const * pszNew) -> VSI_RETVAL"""
     return _gdal.Rename(*args)
 
-def Sync(*args, **kwargs):
+def Sync(*args, **kwargs) -> "bool":
     r"""Sync(char const * pszSource, char const * pszTarget, char ** options=None, GDALProgressFunc callback=0, void * callback_data=None) -> bool"""
     return _gdal.Sync(*args, **kwargs)
 
-def AbortPendingUploads(*args):
+def AbortPendingUploads(*args) -> "bool":
     r"""AbortPendingUploads(char const * utf8_path) -> bool"""
     return _gdal.AbortPendingUploads(*args)
 
-def GetActualURL(*args):
+def GetActualURL(*args) -> "char const *":
     r"""GetActualURL(char const * utf8_path) -> char const *"""
     return _gdal.GetActualURL(*args)
 
-def GetSignedURL(*args):
+def GetSignedURL(*args) -> "retStringAndCPLFree *":
     r"""GetSignedURL(char const * utf8_path, char ** options=None) -> retStringAndCPLFree *"""
     return _gdal.GetSignedURL(*args)
 
-def GetFileSystemsPrefixes(*args):
+def GetFileSystemsPrefixes(*args) -> "char **":
     r"""GetFileSystemsPrefixes() -> char **"""
     return _gdal.GetFileSystemsPrefixes(*args)
 
-def GetFileSystemOptions(*args):
+def GetFileSystemOptions(*args) -> "char const *":
     r"""GetFileSystemOptions(char const * utf8_path) -> char const *"""
     return _gdal.GetFileSystemOptions(*args)
 class VSILFILE(object):
     r"""Proxy of C++ VSILFILE class."""
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
 
@@ -1764,144 +2102,152 @@
     mtime = property(_gdal.StatBuf_mtime_get, doc=r"""mtime : GIntBig""")
 
     def __init__(self, *args):
         r"""__init__(StatBuf self, StatBuf psStatBuf) -> StatBuf"""
         _gdal.StatBuf_swiginit(self, _gdal.new_StatBuf(*args))
     __swig_destroy__ = _gdal.delete_StatBuf
 
-    def IsDirectory(self, *args):
+    def IsDirectory(self, *args) -> "int":
         r"""IsDirectory(StatBuf self) -> int"""
         return _gdal.StatBuf_IsDirectory(self, *args)
 
 # Register StatBuf in _gdal:
 _gdal.StatBuf_swigregister(StatBuf)
 
 
-def VSIStatL(*args):
+def VSIStatL(*args) -> "StatBuf *":
     r"""VSIStatL(char const * utf8_path, int nFlags=0) -> int"""
     return _gdal.VSIStatL(*args)
 
-def GetFileMetadata(*args):
+def GetFileMetadata(*args) -> "char **":
     r"""GetFileMetadata(char const * utf8_path, char const * domain, char ** options=None) -> char **"""
     return _gdal.GetFileMetadata(*args)
 
-def SetFileMetadata(*args):
+def SetFileMetadata(*args) -> "bool":
     r"""SetFileMetadata(char const * utf8_path, char ** metadata, char const * domain, char ** options=None) -> bool"""
     return _gdal.SetFileMetadata(*args)
 
-def VSIFOpenL(*args):
+def VSIFOpenL(*args) -> "VSILFILE *":
     r"""VSIFOpenL(char const * utf8_path, char const * pszMode) -> VSILFILE"""
     return _gdal.VSIFOpenL(*args)
 
-def VSIFOpenExL(*args):
+def VSIFOpenExL(*args) -> "VSILFILE *":
     r"""VSIFOpenExL(char const * utf8_path, char const * pszMode, int bSetError=FALSE, char ** options=None) -> VSILFILE"""
     return _gdal.VSIFOpenExL(*args)
 
-def VSIFEofL(*args):
+def VSIFEofL(*args) -> "int":
     r"""VSIFEofL(VSILFILE fp) -> int"""
     return _gdal.VSIFEofL(*args)
 
-def VSIFFlushL(*args):
+def VSIFFlushL(*args) -> "int":
     r"""VSIFFlushL(VSILFILE fp) -> int"""
     return _gdal.VSIFFlushL(*args)
 
-def VSIFCloseL(*args):
+def VSIFCloseL(*args) -> "VSI_RETVAL":
     r"""VSIFCloseL(VSILFILE fp) -> VSI_RETVAL"""
     return _gdal.VSIFCloseL(*args)
 
-def VSIFSeekL(*args):
+def VSIFSeekL(*args) -> "int":
     r"""VSIFSeekL(VSILFILE fp, GIntBig offset, int whence) -> int"""
     return _gdal.VSIFSeekL(*args)
 
-def VSIFTellL(*args):
+def VSIFTellL(*args) -> "GIntBig":
     r"""VSIFTellL(VSILFILE fp) -> GIntBig"""
     return _gdal.VSIFTellL(*args)
 
-def VSIFTruncateL(*args):
+def VSIFTruncateL(*args) -> "int":
     r"""VSIFTruncateL(VSILFILE fp, GIntBig length) -> int"""
     return _gdal.VSIFTruncateL(*args)
 
-def VSISupportsSparseFiles(*args):
+def VSISupportsSparseFiles(*args) -> "int":
     r"""VSISupportsSparseFiles(char const * utf8_path) -> int"""
     return _gdal.VSISupportsSparseFiles(*args)
 VSI_RANGE_STATUS_UNKNOWN = _gdal.VSI_RANGE_STATUS_UNKNOWN
 
 VSI_RANGE_STATUS_DATA = _gdal.VSI_RANGE_STATUS_DATA
 
 VSI_RANGE_STATUS_HOLE = _gdal.VSI_RANGE_STATUS_HOLE
 
 
-def VSIFGetRangeStatusL(*args):
+def VSIFGetRangeStatusL(*args) -> "int":
     r"""VSIFGetRangeStatusL(VSILFILE fp, GIntBig offset, GIntBig length) -> int"""
     return _gdal.VSIFGetRangeStatusL(*args)
 
-def VSIFWriteL(*args):
+def VSIFWriteL(*args) -> "int":
     r"""VSIFWriteL(int nLen, int size, int memb, VSILFILE fp) -> int"""
     return _gdal.VSIFWriteL(*args)
 
-def VSICurlClearCache(*args):
+def VSICurlClearCache(*args) -> "void":
     r"""VSICurlClearCache()"""
     return _gdal.VSICurlClearCache(*args)
 
-def VSICurlPartialClearCache(*args):
+def VSICurlPartialClearCache(*args) -> "void":
     r"""VSICurlPartialClearCache(char const * utf8_path)"""
     return _gdal.VSICurlPartialClearCache(*args)
 
-def NetworkStatsReset(*args):
+def NetworkStatsReset(*args) -> "void":
     r"""NetworkStatsReset()"""
     return _gdal.NetworkStatsReset(*args)
 
-def NetworkStatsGetAsSerializedJSON(*args):
+def NetworkStatsGetAsSerializedJSON(*args) -> "retStringAndCPLFree *":
     r"""NetworkStatsGetAsSerializedJSON(char ** options=None) -> retStringAndCPLFree *"""
     return _gdal.NetworkStatsGetAsSerializedJSON(*args)
 
-def ParseCommandLine(*args):
+def ParseCommandLine(*args) -> "char **":
     r"""ParseCommandLine(char const * utf8_path) -> char **"""
     return _gdal.ParseCommandLine(*args)
+
+def GetNumCPUs(*args) -> "int":
+    r"""GetNumCPUs() -> int"""
+    return _gdal.GetNumCPUs(*args)
+
+def GetUsablePhysicalRAM(*args) -> "GIntBig":
+    r"""GetUsablePhysicalRAM() -> GIntBig"""
+    return _gdal.GetUsablePhysicalRAM(*args)
 class MajorObject(object):
     r"""Proxy of C++ GDALMajorObjectShadow class."""
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
 
     def __init__(self, *args, **kwargs):
         raise AttributeError("No constructor defined")
     __repr__ = _swig_repr
 
-    def GetDescription(self, *args):
+    def GetDescription(self, *args) -> "char const *":
         r"""GetDescription(MajorObject self) -> char const *"""
         return _gdal.MajorObject_GetDescription(self, *args)
 
-    def SetDescription(self, *args):
+    def SetDescription(self, *args) -> "void":
         r"""SetDescription(MajorObject self, char const * pszNewDesc)"""
         return _gdal.MajorObject_SetDescription(self, *args)
 
-    def GetMetadataDomainList(self, *args):
+    def GetMetadataDomainList(self, *args) -> "char **":
         r"""GetMetadataDomainList(MajorObject self) -> char **"""
         return _gdal.MajorObject_GetMetadataDomainList(self, *args)
 
-    def GetMetadata_Dict(self, *args):
+    def GetMetadata_Dict(self, *args) -> "char **":
         r"""GetMetadata_Dict(MajorObject self, char const * pszDomain="") -> char **"""
         return _gdal.MajorObject_GetMetadata_Dict(self, *args)
 
-    def GetMetadata_List(self, *args):
+    def GetMetadata_List(self, *args) -> "char **":
         r"""GetMetadata_List(MajorObject self, char const * pszDomain="") -> char **"""
         return _gdal.MajorObject_GetMetadata_List(self, *args)
 
-    def SetMetadata(self, *args):
+    def SetMetadata(self, *args) -> "CPLErr":
         r"""
         SetMetadata(MajorObject self, char ** papszMetadata, char const * pszDomain="") -> CPLErr
         SetMetadata(MajorObject self, char * pszMetadataString, char const * pszDomain="") -> CPLErr
         """
         return _gdal.MajorObject_SetMetadata(self, *args)
 
-    def GetMetadataItem(self, *args):
+    def GetMetadataItem(self, *args) -> "char const *":
         r"""GetMetadataItem(MajorObject self, char const * pszName, char const * pszDomain="") -> char const *"""
         return _gdal.MajorObject_GetMetadataItem(self, *args)
 
-    def SetMetadataItem(self, *args):
+    def SetMetadataItem(self, *args) -> "CPLErr":
         r"""SetMetadataItem(MajorObject self, char const * pszName, char const * pszValue, char const * pszDomain="") -> CPLErr"""
         return _gdal.MajorObject_SetMetadataItem(self, *args)
 
     def GetMetadata(self, domain=''):
       if domain and domain[:4] == 'xml:':
         return self.GetMetadata_List(domain)
       return self.GetMetadata_Dict(domain)
@@ -1918,43 +2264,43 @@
     def __init__(self, *args, **kwargs):
         raise AttributeError("No constructor defined")
     __repr__ = _swig_repr
     ShortName = property(_gdal.Driver_ShortName_get, doc=r"""ShortName : p.q(const).char""")
     LongName = property(_gdal.Driver_LongName_get, doc=r"""LongName : p.q(const).char""")
     HelpTopic = property(_gdal.Driver_HelpTopic_get, doc=r"""HelpTopic : p.q(const).char""")
 
-    def Create(self, *args, **kwargs):
+    def Create(self, *args, **kwargs) -> "GDALDatasetShadow *":
         r"""Create(Driver self, char const * utf8_path, int xsize, int ysize, int bands=1, GDALDataType eType=GDT_Byte, char ** options=None) -> Dataset"""
         return _gdal.Driver_Create(self, *args, **kwargs)
 
-    def CreateMultiDimensional(self, *args, **kwargs):
+    def CreateMultiDimensional(self, *args, **kwargs) -> "GDALDatasetShadow *":
         r"""CreateMultiDimensional(Driver self, char const * utf8_path, char ** root_group_options=None, char ** options=None) -> Dataset"""
         return _gdal.Driver_CreateMultiDimensional(self, *args, **kwargs)
 
-    def CreateCopy(self, *args, **kwargs):
+    def CreateCopy(self, *args, **kwargs) -> "GDALDatasetShadow *":
         r"""CreateCopy(Driver self, char const * utf8_path, Dataset src, int strict=1, char ** options=None, GDALProgressFunc callback=0, void * callback_data=None) -> Dataset"""
         return _gdal.Driver_CreateCopy(self, *args, **kwargs)
 
-    def Delete(self, *args):
+    def Delete(self, *args) -> "CPLErr":
         r"""Delete(Driver self, char const * utf8_path) -> CPLErr"""
         return _gdal.Driver_Delete(self, *args)
 
-    def Rename(self, *args):
+    def Rename(self, *args) -> "CPLErr":
         r"""Rename(Driver self, char const * newName, char const * oldName) -> CPLErr"""
         return _gdal.Driver_Rename(self, *args)
 
-    def CopyFiles(self, *args):
+    def CopyFiles(self, *args) -> "CPLErr":
         r"""CopyFiles(Driver self, char const * newName, char const * oldName) -> CPLErr"""
         return _gdal.Driver_CopyFiles(self, *args)
 
-    def Register(self, *args):
+    def Register(self, *args) -> "int":
         r"""Register(Driver self) -> int"""
         return _gdal.Driver_Register(self, *args)
 
-    def Deregister(self, *args):
+    def Deregister(self, *args) -> "void":
         r"""Deregister(Driver self)"""
         return _gdal.Driver_Deregister(self, *args)
 
 # Register Driver in _gdal:
 _gdal.Driver_swigregister(Driver)
 
 from . import ogr
@@ -1996,108 +2342,109 @@
     def __str__(self):
       str = '%s (%.2fP,%.2fL) -> (%.7fE,%.7fN,%.2f) %s '\
             % (self.Id, self.GCPPixel, self.GCPLine,
                self.GCPX, self.GCPY, self.GCPZ, self.Info )
       return str
 
     def serialize(self, with_Z=0):
-      base = [gdalconst.CXT_Element,'GCP']
-      base.append([gdalconst.CXT_Attribute,'Id',[gdalconst.CXT_Text,self.Id]])
+      base = [gdalconst.CXT_Element, 'GCP']
+      base.append([gdalconst.CXT_Attribute, 'Id', [gdalconst.CXT_Text, self.Id]])
       pixval = '%0.15E' % self.GCPPixel
       lineval = '%0.15E' % self.GCPLine
       xval = '%0.15E' % self.GCPX
       yval = '%0.15E' % self.GCPY
       zval = '%0.15E' % self.GCPZ
-      base.append([gdalconst.CXT_Attribute,'Pixel',[gdalconst.CXT_Text,pixval]])
-      base.append([gdalconst.CXT_Attribute,'Line',[gdalconst.CXT_Text,lineval]])
-      base.append([gdalconst.CXT_Attribute,'X',[gdalconst.CXT_Text,xval]])
-      base.append([gdalconst.CXT_Attribute,'Y',[gdalconst.CXT_Text,yval]])
+      base.append([gdalconst.CXT_Attribute, 'Pixel', [gdalconst.CXT_Text, pixval]])
+      base.append([gdalconst.CXT_Attribute, 'Line', [gdalconst.CXT_Text, lineval]])
+      base.append([gdalconst.CXT_Attribute, 'X', [gdalconst.CXT_Text, xval]])
+      base.append([gdalconst.CXT_Attribute, 'Y', [gdalconst.CXT_Text, yval]])
       if with_Z:
-          base.append([gdalconst.CXT_Attribute,'Z',[gdalconst.CXT_Text,zval]])
+          base.append([gdalconst.CXT_Attribute, 'Z', [gdalconst.CXT_Text, zval]])
       return base
 
 
+
 # Register GCP in _gdal:
 _gdal.GCP_swigregister(GCP)
 
 
-def GDAL_GCP_GCPX_get(*args):
+def GDAL_GCP_GCPX_get(*args) -> "double":
     r"""GDAL_GCP_GCPX_get(GCP gcp) -> double"""
     return _gdal.GDAL_GCP_GCPX_get(*args)
 
-def GDAL_GCP_GCPX_set(*args):
+def GDAL_GCP_GCPX_set(*args) -> "void":
     r"""GDAL_GCP_GCPX_set(GCP gcp, double dfGCPX)"""
     return _gdal.GDAL_GCP_GCPX_set(*args)
 
-def GDAL_GCP_GCPY_get(*args):
+def GDAL_GCP_GCPY_get(*args) -> "double":
     r"""GDAL_GCP_GCPY_get(GCP gcp) -> double"""
     return _gdal.GDAL_GCP_GCPY_get(*args)
 
-def GDAL_GCP_GCPY_set(*args):
+def GDAL_GCP_GCPY_set(*args) -> "void":
     r"""GDAL_GCP_GCPY_set(GCP gcp, double dfGCPY)"""
     return _gdal.GDAL_GCP_GCPY_set(*args)
 
-def GDAL_GCP_GCPZ_get(*args):
+def GDAL_GCP_GCPZ_get(*args) -> "double":
     r"""GDAL_GCP_GCPZ_get(GCP gcp) -> double"""
     return _gdal.GDAL_GCP_GCPZ_get(*args)
 
-def GDAL_GCP_GCPZ_set(*args):
+def GDAL_GCP_GCPZ_set(*args) -> "void":
     r"""GDAL_GCP_GCPZ_set(GCP gcp, double dfGCPZ)"""
     return _gdal.GDAL_GCP_GCPZ_set(*args)
 
-def GDAL_GCP_GCPPixel_get(*args):
+def GDAL_GCP_GCPPixel_get(*args) -> "double":
     r"""GDAL_GCP_GCPPixel_get(GCP gcp) -> double"""
     return _gdal.GDAL_GCP_GCPPixel_get(*args)
 
-def GDAL_GCP_GCPPixel_set(*args):
+def GDAL_GCP_GCPPixel_set(*args) -> "void":
     r"""GDAL_GCP_GCPPixel_set(GCP gcp, double dfGCPPixel)"""
     return _gdal.GDAL_GCP_GCPPixel_set(*args)
 
-def GDAL_GCP_GCPLine_get(*args):
+def GDAL_GCP_GCPLine_get(*args) -> "double":
     r"""GDAL_GCP_GCPLine_get(GCP gcp) -> double"""
     return _gdal.GDAL_GCP_GCPLine_get(*args)
 
-def GDAL_GCP_GCPLine_set(*args):
+def GDAL_GCP_GCPLine_set(*args) -> "void":
     r"""GDAL_GCP_GCPLine_set(GCP gcp, double dfGCPLine)"""
     return _gdal.GDAL_GCP_GCPLine_set(*args)
 
-def GDAL_GCP_Info_get(*args):
+def GDAL_GCP_Info_get(*args) -> "char const *":
     r"""GDAL_GCP_Info_get(GCP gcp) -> char const *"""
     return _gdal.GDAL_GCP_Info_get(*args)
 
-def GDAL_GCP_Info_set(*args):
+def GDAL_GCP_Info_set(*args) -> "void":
     r"""GDAL_GCP_Info_set(GCP gcp, char const * pszInfo)"""
     return _gdal.GDAL_GCP_Info_set(*args)
 
-def GDAL_GCP_Id_get(*args):
+def GDAL_GCP_Id_get(*args) -> "char const *":
     r"""GDAL_GCP_Id_get(GCP gcp) -> char const *"""
     return _gdal.GDAL_GCP_Id_get(*args)
 
-def GDAL_GCP_Id_set(*args):
+def GDAL_GCP_Id_set(*args) -> "void":
     r"""GDAL_GCP_Id_set(GCP gcp, char const * pszId)"""
     return _gdal.GDAL_GCP_Id_set(*args)
 
-def GCPsToGeoTransform(*args):
+def GCPsToGeoTransform(*args) -> "double [ANY]":
     r"""GCPsToGeoTransform(int nGCPs, int bApproxOK=1) -> RETURN_NONE"""
     return _gdal.GCPsToGeoTransform(*args)
 class VirtualMem(object):
     r"""Proxy of C++ CPLVirtualMemShadow class."""
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
 
     def __init__(self, *args, **kwargs):
         raise AttributeError("No constructor defined")
     __repr__ = _swig_repr
     __swig_destroy__ = _gdal.delete_VirtualMem
 
-    def GetAddr(self, *args):
+    def GetAddr(self, *args) -> "void":
         r"""GetAddr(VirtualMem self)"""
         return _gdal.VirtualMem_GetAddr(self, *args)
 
-    def Pin(self, *args):
+    def Pin(self, *args) -> "void":
         r"""Pin(VirtualMem self, size_t start_offset=0, size_t nsize=0, int bWriteOp=0)"""
         return _gdal.VirtualMem_Pin(self, *args)
 
 # Register VirtualMem in _gdal:
 _gdal.VirtualMem_swigregister(VirtualMem)
 
 class AsyncReader(object):
@@ -2106,27 +2453,27 @@
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
 
     def __init__(self, *args, **kwargs):
         raise AttributeError("No constructor defined")
     __repr__ = _swig_repr
     __swig_destroy__ = _gdal.delete_AsyncReader
 
-    def GetNextUpdatedRegion(self, *args):
+    def GetNextUpdatedRegion(self, *args) -> "GDALAsyncStatusType":
         r"""GetNextUpdatedRegion(AsyncReader self, double timeout) -> GDALAsyncStatusType"""
         return _gdal.AsyncReader_GetNextUpdatedRegion(self, *args)
 
-    def GetBuffer(self, *args):
+    def GetBuffer(self, *args) -> "void":
         r"""GetBuffer(AsyncReader self)"""
         return _gdal.AsyncReader_GetBuffer(self, *args)
 
-    def LockBuffer(self, *args):
+    def LockBuffer(self, *args) -> "int":
         r"""LockBuffer(AsyncReader self, double timeout) -> int"""
         return _gdal.AsyncReader_LockBuffer(self, *args)
 
-    def UnlockBuffer(self, *args):
+    def UnlockBuffer(self, *args) -> "void":
         r"""UnlockBuffer(AsyncReader self)"""
         return _gdal.AsyncReader_UnlockBuffer(self, *args)
 
 # Register AsyncReader in _gdal:
 _gdal.AsyncReader_swigregister(AsyncReader)
 
 class Dataset(MajorObject):
@@ -2138,219 +2485,239 @@
         raise AttributeError("No constructor defined")
     __repr__ = _swig_repr
     RasterXSize = property(_gdal.Dataset_RasterXSize_get, doc=r"""RasterXSize : int""")
     RasterYSize = property(_gdal.Dataset_RasterYSize_get, doc=r"""RasterYSize : int""")
     RasterCount = property(_gdal.Dataset_RasterCount_get, doc=r"""RasterCount : int""")
     __swig_destroy__ = _gdal.delete_Dataset
 
-    def GetDriver(self, *args):
+    def GetDriver(self, *args) -> "GDALDriverShadow *":
         r"""GetDriver(Dataset self) -> Driver"""
         return _gdal.Dataset_GetDriver(self, *args)
 
-    def GetRasterBand(self, *args):
+    def GetRasterBand(self, *args) -> "GDALRasterBandShadow *":
         r"""GetRasterBand(Dataset self, int nBand) -> Band"""
         return _gdal.Dataset_GetRasterBand(self, *args)
 
-    def GetRootGroup(self, *args):
+    def GetRootGroup(self, *args) -> "GDALGroupHS *":
         r"""GetRootGroup(Dataset self) -> Group"""
         return _gdal.Dataset_GetRootGroup(self, *args)
 
-    def GetProjection(self, *args):
+    def GetProjection(self, *args) -> "char const *":
         r"""GetProjection(Dataset self) -> char const *"""
         return _gdal.Dataset_GetProjection(self, *args)
 
-    def GetProjectionRef(self, *args):
+    def GetProjectionRef(self, *args) -> "char const *":
         r"""GetProjectionRef(Dataset self) -> char const *"""
         return _gdal.Dataset_GetProjectionRef(self, *args)
 
-    def GetSpatialRef(self, *args):
+    def GetSpatialRef(self, *args) -> "OSRSpatialReferenceShadow *":
         r"""GetSpatialRef(Dataset self) -> SpatialReference"""
         return _gdal.Dataset_GetSpatialRef(self, *args)
 
-    def SetProjection(self, *args):
+    def SetProjection(self, *args) -> "CPLErr":
         r"""SetProjection(Dataset self, char const * prj) -> CPLErr"""
         return _gdal.Dataset_SetProjection(self, *args)
 
-    def SetSpatialRef(self, *args):
+    def SetSpatialRef(self, *args) -> "CPLErr":
         r"""SetSpatialRef(Dataset self, SpatialReference srs) -> CPLErr"""
         return _gdal.Dataset_SetSpatialRef(self, *args)
 
-    def GetGeoTransform(self, *args, **kwargs):
+    def GetGeoTransform(self, *args, **kwargs) -> "void":
         r"""GetGeoTransform(Dataset self, int * can_return_null=None)"""
         return _gdal.Dataset_GetGeoTransform(self, *args, **kwargs)
 
-    def SetGeoTransform(self, *args):
+    def SetGeoTransform(self, *args) -> "CPLErr":
         r"""SetGeoTransform(Dataset self, double [6] argin) -> CPLErr"""
         return _gdal.Dataset_SetGeoTransform(self, *args)
 
-    def BuildOverviews(self, *args, **kwargs):
-        r"""BuildOverviews(Dataset self, char const * resampling="NEAREST", int overviewlist=0, GDALProgressFunc callback=0, void * callback_data=None) -> int"""
+    def BuildOverviews(self, *args, **kwargs) -> "int":
+        r"""BuildOverviews(Dataset self, char const * resampling="NEAREST", int overviewlist=0, GDALProgressFunc callback=0, void * callback_data=None, char ** options=None) -> int"""
         return _gdal.Dataset_BuildOverviews(self, *args, **kwargs)
 
-    def GetGCPCount(self, *args):
+    def GetGCPCount(self, *args) -> "int":
         r"""GetGCPCount(Dataset self) -> int"""
         return _gdal.Dataset_GetGCPCount(self, *args)
 
-    def GetGCPProjection(self, *args):
+    def GetGCPProjection(self, *args) -> "char const *":
         r"""GetGCPProjection(Dataset self) -> char const *"""
         return _gdal.Dataset_GetGCPProjection(self, *args)
 
-    def GetGCPSpatialRef(self, *args):
+    def GetGCPSpatialRef(self, *args) -> "OSRSpatialReferenceShadow *":
         r"""GetGCPSpatialRef(Dataset self) -> SpatialReference"""
         return _gdal.Dataset_GetGCPSpatialRef(self, *args)
 
-    def GetGCPs(self, *args):
+    def GetGCPs(self, *args) -> "void":
         r"""GetGCPs(Dataset self)"""
         return _gdal.Dataset_GetGCPs(self, *args)
 
-    def _SetGCPs(self, *args):
+    def _SetGCPs(self, *args) -> "CPLErr":
         r"""_SetGCPs(Dataset self, int nGCPs, char const * pszGCPProjection) -> CPLErr"""
         return _gdal.Dataset__SetGCPs(self, *args)
 
-    def _SetGCPs2(self, *args):
+    def _SetGCPs2(self, *args) -> "CPLErr":
         r"""_SetGCPs2(Dataset self, int nGCPs, SpatialReference hSRS) -> CPLErr"""
         return _gdal.Dataset__SetGCPs2(self, *args)
 
-    def FlushCache(self, *args):
+    def FlushCache(self, *args) -> "void":
         r"""FlushCache(Dataset self)"""
         return _gdal.Dataset_FlushCache(self, *args)
 
-    def AddBand(self, *args, **kwargs):
+    def AddBand(self, *args, **kwargs) -> "CPLErr":
         r"""AddBand(Dataset self, GDALDataType datatype=GDT_Byte, char ** options=None) -> CPLErr"""
         return _gdal.Dataset_AddBand(self, *args, **kwargs)
 
-    def CreateMaskBand(self, *args):
+    def CreateMaskBand(self, *args) -> "CPLErr":
         r"""CreateMaskBand(Dataset self, int nFlags) -> CPLErr"""
         return _gdal.Dataset_CreateMaskBand(self, *args)
 
-    def GetFileList(self, *args):
+    def GetFileList(self, *args) -> "char **":
         r"""GetFileList(Dataset self) -> char **"""
         return _gdal.Dataset_GetFileList(self, *args)
 
-    def WriteRaster(self, *args, **kwargs):
+    def WriteRaster(self, *args, **kwargs) -> "CPLErr":
         r"""WriteRaster(Dataset self, int xoff, int yoff, int xsize, int ysize, GIntBig buf_len, int * buf_xsize=None, int * buf_ysize=None, GDALDataType * buf_type=None, int band_list=0, GIntBig * buf_pixel_space=None, GIntBig * buf_line_space=None, GIntBig * buf_band_space=None) -> CPLErr"""
         return _gdal.Dataset_WriteRaster(self, *args, **kwargs)
 
-    def AdviseRead(self, *args):
+    def AdviseRead(self, *args) -> "CPLErr":
         r"""AdviseRead(Dataset self, int xoff, int yoff, int xsize, int ysize, int * buf_xsize=None, int * buf_ysize=None, GDALDataType * buf_type=None, int band_list=0, char ** options=None) -> CPLErr"""
         return _gdal.Dataset_AdviseRead(self, *args)
 
-    def BeginAsyncReader(self, *args, **kwargs):
+    def BeginAsyncReader(self, *args, **kwargs) -> "GDALAsyncReaderShadow *":
         r"""BeginAsyncReader(Dataset self, int xOff, int yOff, int xSize, int ySize, int buf_len, int buf_xsize, int buf_ysize, GDALDataType bufType=(GDALDataType) 0, int band_list=0, int nPixelSpace=0, int nLineSpace=0, int nBandSpace=0, char ** options=None) -> AsyncReader"""
         return _gdal.Dataset_BeginAsyncReader(self, *args, **kwargs)
 
-    def EndAsyncReader(self, *args):
+    def EndAsyncReader(self, *args) -> "void":
         r"""EndAsyncReader(Dataset self, AsyncReader ario)"""
         return _gdal.Dataset_EndAsyncReader(self, *args)
 
-    def GetVirtualMem(self, *args, **kwargs):
+    def GetVirtualMem(self, *args, **kwargs) -> "CPLVirtualMemShadow *":
         r"""GetVirtualMem(Dataset self, GDALRWFlag eRWFlag, int nXOff, int nYOff, int nXSize, int nYSize, int nBufXSize, int nBufYSize, GDALDataType eBufType, int band_list, int bIsBandSequential, size_t nCacheSize, size_t nPageSizeHint, char ** options=None) -> VirtualMem"""
         return _gdal.Dataset_GetVirtualMem(self, *args, **kwargs)
 
-    def GetTiledVirtualMem(self, *args, **kwargs):
+    def GetTiledVirtualMem(self, *args, **kwargs) -> "CPLVirtualMemShadow *":
         r"""GetTiledVirtualMem(Dataset self, GDALRWFlag eRWFlag, int nXOff, int nYOff, int nXSize, int nYSize, int nTileXSize, int nTileYSize, GDALDataType eBufType, int band_list, GDALTileOrganization eTileOrganization, size_t nCacheSize, char ** options=None) -> VirtualMem"""
         return _gdal.Dataset_GetTiledVirtualMem(self, *args, **kwargs)
 
-    def CreateLayer(self, *args, **kwargs):
+    def CreateLayer(self, *args, **kwargs) -> "OGRLayerShadow *":
         r"""CreateLayer(Dataset self, char const * name, SpatialReference srs=None, OGRwkbGeometryType geom_type=wkbUnknown, char ** options=None) -> Layer"""
         return _gdal.Dataset_CreateLayer(self, *args, **kwargs)
 
-    def CopyLayer(self, *args, **kwargs):
+    def CopyLayer(self, *args, **kwargs) -> "OGRLayerShadow *":
         r"""CopyLayer(Dataset self, Layer src_layer, char const * new_name, char ** options=None) -> Layer"""
         return _gdal.Dataset_CopyLayer(self, *args, **kwargs)
 
-    def DeleteLayer(self, *args):
+    def DeleteLayer(self, *args) -> "OGRErr":
         r"""DeleteLayer(Dataset self, int index) -> OGRErr"""
         return _gdal.Dataset_DeleteLayer(self, *args)
 
-    def GetLayerCount(self, *args):
+    def GetLayerCount(self, *args) -> "int":
         r"""GetLayerCount(Dataset self) -> int"""
         return _gdal.Dataset_GetLayerCount(self, *args)
 
-    def IsLayerPrivate(self, *args):
+    def IsLayerPrivate(self, *args) -> "bool":
         r"""IsLayerPrivate(Dataset self, int index) -> bool"""
         return _gdal.Dataset_IsLayerPrivate(self, *args)
 
-    def GetLayerByIndex(self, *args):
+    def GetLayerByIndex(self, *args) -> "OGRLayerShadow *":
         r"""GetLayerByIndex(Dataset self, int index=0) -> Layer"""
         return _gdal.Dataset_GetLayerByIndex(self, *args)
 
-    def GetLayerByName(self, *args):
+    def GetLayerByName(self, *args) -> "OGRLayerShadow *":
         r"""GetLayerByName(Dataset self, char const * layer_name) -> Layer"""
         return _gdal.Dataset_GetLayerByName(self, *args)
 
-    def ResetReading(self, *args):
+    def ResetReading(self, *args) -> "void":
         r"""ResetReading(Dataset self)"""
         return _gdal.Dataset_ResetReading(self, *args)
 
-    def GetNextFeature(self, *args, **kwargs):
+    def GetNextFeature(self, *args, **kwargs) -> "OGRFeatureShadow *":
         r"""GetNextFeature(Dataset self, bool include_layer=True, bool include_pct=False, GDALProgressFunc callback=0, void * callback_data=None) -> Feature"""
         return _gdal.Dataset_GetNextFeature(self, *args, **kwargs)
 
-    def TestCapability(self, *args):
+    def TestCapability(self, *args) -> "bool":
         r"""TestCapability(Dataset self, char const * cap) -> bool"""
         return _gdal.Dataset_TestCapability(self, *args)
 
-    def ExecuteSQL(self, *args, **kwargs):
+    def ExecuteSQL(self, *args, **kwargs) -> "OGRLayerShadow *":
         r"""ExecuteSQL(Dataset self, char const * statement, Geometry spatialFilter=None, char const * dialect="") -> Layer"""
         return _gdal.Dataset_ExecuteSQL(self, *args, **kwargs)
 
-    def ReleaseResultSet(self, *args):
+    def ReleaseResultSet(self, *args) -> "void":
         r"""ReleaseResultSet(Dataset self, Layer layer)"""
         return _gdal.Dataset_ReleaseResultSet(self, *args)
 
-    def GetStyleTable(self, *args):
+    def GetStyleTable(self, *args) -> "OGRStyleTableShadow *":
         r"""GetStyleTable(Dataset self) -> StyleTable"""
         return _gdal.Dataset_GetStyleTable(self, *args)
 
-    def SetStyleTable(self, *args):
+    def SetStyleTable(self, *args) -> "void":
         r"""SetStyleTable(Dataset self, StyleTable table)"""
         return _gdal.Dataset_SetStyleTable(self, *args)
 
-    def AbortSQL(self, *args):
+    def AbortSQL(self, *args) -> "OGRErr":
         r"""AbortSQL(Dataset self) -> OGRErr"""
         return _gdal.Dataset_AbortSQL(self, *args)
 
-    def StartTransaction(self, *args, **kwargs):
+    def StartTransaction(self, *args, **kwargs) -> "OGRErr":
         r"""StartTransaction(Dataset self, int force=FALSE) -> OGRErr"""
         return _gdal.Dataset_StartTransaction(self, *args, **kwargs)
 
-    def CommitTransaction(self, *args):
+    def CommitTransaction(self, *args) -> "OGRErr":
         r"""CommitTransaction(Dataset self) -> OGRErr"""
         return _gdal.Dataset_CommitTransaction(self, *args)
 
-    def RollbackTransaction(self, *args):
+    def RollbackTransaction(self, *args) -> "OGRErr":
         r"""RollbackTransaction(Dataset self) -> OGRErr"""
         return _gdal.Dataset_RollbackTransaction(self, *args)
 
-    def ClearStatistics(self, *args):
+    def ClearStatistics(self, *args) -> "void":
         r"""ClearStatistics(Dataset self)"""
         return _gdal.Dataset_ClearStatistics(self, *args)
 
-    def GetFieldDomainNames(self, *args):
+    def GetFieldDomainNames(self, *args) -> "char **":
         r"""GetFieldDomainNames(Dataset self, char ** options=None) -> char **"""
         return _gdal.Dataset_GetFieldDomainNames(self, *args)
 
-    def GetFieldDomain(self, *args):
+    def GetFieldDomain(self, *args) -> "OGRFieldDomainShadow *":
         r"""GetFieldDomain(Dataset self, char const * name) -> FieldDomain"""
         return _gdal.Dataset_GetFieldDomain(self, *args)
 
-    def AddFieldDomain(self, *args):
+    def AddFieldDomain(self, *args) -> "bool":
         r"""AddFieldDomain(Dataset self, FieldDomain fieldDomain) -> bool"""
         return _gdal.Dataset_AddFieldDomain(self, *args)
 
-    def DeleteFieldDomain(self, *args):
+    def DeleteFieldDomain(self, *args) -> "bool":
         r"""DeleteFieldDomain(Dataset self, char const * name) -> bool"""
         return _gdal.Dataset_DeleteFieldDomain(self, *args)
 
-    def UpdateFieldDomain(self, *args):
+    def UpdateFieldDomain(self, *args) -> "bool":
         r"""UpdateFieldDomain(Dataset self, FieldDomain fieldDomain) -> bool"""
         return _gdal.Dataset_UpdateFieldDomain(self, *args)
 
-    def ReadRaster1(self, *args, **kwargs):
+    def GetRelationshipNames(self, *args) -> "char **":
+        r"""GetRelationshipNames(Dataset self, char ** options=None) -> char **"""
+        return _gdal.Dataset_GetRelationshipNames(self, *args)
+
+    def GetRelationship(self, *args) -> "GDALRelationshipShadow *":
+        r"""GetRelationship(Dataset self, char const * name) -> Relationship"""
+        return _gdal.Dataset_GetRelationship(self, *args)
+
+    def AddRelationship(self, *args) -> "bool":
+        r"""AddRelationship(Dataset self, Relationship relationship) -> bool"""
+        return _gdal.Dataset_AddRelationship(self, *args)
+
+    def DeleteRelationship(self, *args) -> "bool":
+        r"""DeleteRelationship(Dataset self, char const * name) -> bool"""
+        return _gdal.Dataset_DeleteRelationship(self, *args)
+
+    def UpdateRelationship(self, *args) -> "bool":
+        r"""UpdateRelationship(Dataset self, Relationship relationship) -> bool"""
+        return _gdal.Dataset_UpdateRelationship(self, *args)
+
+    def ReadRaster1(self, *args, **kwargs) -> "CPLErr":
         r"""ReadRaster1(Dataset self, double xoff, double yoff, double xsize, double ysize, int * buf_xsize=None, int * buf_ysize=None, GDALDataType * buf_type=None, int band_list=0, GIntBig * buf_pixel_space=None, GIntBig * buf_line_space=None, GIntBig * buf_band_space=None, GDALRIOResampleAlg resample_alg=GRIORA_NearestNeighbour, GDALProgressFunc callback=0, void * callback_data=None, void * inputOutputBuf=None) -> CPLErr"""
         return _gdal.Dataset_ReadRaster1(self, *args, **kwargs)
 
 
     def ReadAsArray(self, xoff=0, yoff=0, xsize=None, ysize=None, buf_obj=None,
                     buf_xsize=None, buf_ysize=None, buf_type=None,
                     resample_alg=gdalconst.GRIORA_NearestNeighbour,
@@ -2496,17 +2863,17 @@
         if ysize is None:
             ysize = self.RasterYSize
         if datatype is None:
             datatype = self.GetRasterBand(1).DataType
         if band_list is None:
             band_list = list(range(1, self.RasterCount + 1))
         if options is None:
-            virtualmem = self.GetTiledVirtualMem(eAccess,xoff,yoff,xsize,ysize,tilexsize,tileysize,datatype,band_list,tile_organization,cache_size)
+            virtualmem = self.GetTiledVirtualMem(eAccess, xoff, yoff, xsize, ysize, tilexsize, tileysize, datatype, band_list, tile_organization, cache_size)
         else:
-            virtualmem = self.GetTiledVirtualMem(eAccess,xoff,yoff,xsize,ysize,tilexsize,tileysize,datatype,band_list,tile_organization,cache_size, options)
+            virtualmem = self.GetTiledVirtualMem(eAccess, xoff, yoff, xsize, ysize, tilexsize, tileysize, datatype, band_list, tile_organization, cache_size, options)
         return gdal_array.VirtualMemGetArray( virtualmem )
 
     def GetSubDatasets(self):
         sd_list = []
 
         sd = self.GetMetadata('SUBDATASETS')
         if sd is None:
@@ -2588,87 +2955,87 @@
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
 
     def __init__(self, *args, **kwargs):
         raise AttributeError("No constructor defined")
     __repr__ = _swig_repr
     __swig_destroy__ = _gdal.delete_Group
 
-    def GetName(self, *args):
+    def GetName(self, *args) -> "char const *":
         r"""GetName(Group self) -> char const *"""
         return _gdal.Group_GetName(self, *args)
 
-    def GetFullName(self, *args):
+    def GetFullName(self, *args) -> "char const *":
         r"""GetFullName(Group self) -> char const *"""
         return _gdal.Group_GetFullName(self, *args)
 
-    def GetMDArrayNames(self, *args):
+    def GetMDArrayNames(self, *args) -> "char **":
         r"""GetMDArrayNames(Group self, char ** options=None) -> char **"""
         return _gdal.Group_GetMDArrayNames(self, *args)
 
-    def OpenMDArray(self, *args):
+    def OpenMDArray(self, *args) -> "GDALMDArrayHS *":
         r"""OpenMDArray(Group self, char const * name, char ** options=None) -> MDArray"""
         return _gdal.Group_OpenMDArray(self, *args)
 
-    def OpenMDArrayFromFullname(self, *args):
+    def OpenMDArrayFromFullname(self, *args) -> "GDALMDArrayHS *":
         r"""OpenMDArrayFromFullname(Group self, char const * name, char ** options=None) -> MDArray"""
         return _gdal.Group_OpenMDArrayFromFullname(self, *args)
 
-    def ResolveMDArray(self, *args):
+    def ResolveMDArray(self, *args) -> "GDALMDArrayHS *":
         r"""ResolveMDArray(Group self, char const * name, char const * starting_point, char ** options=None) -> MDArray"""
         return _gdal.Group_ResolveMDArray(self, *args)
 
-    def GetGroupNames(self, *args):
+    def GetGroupNames(self, *args) -> "char **":
         r"""GetGroupNames(Group self, char ** options=None) -> char **"""
         return _gdal.Group_GetGroupNames(self, *args)
 
-    def OpenGroup(self, *args):
+    def OpenGroup(self, *args) -> "GDALGroupHS *":
         r"""OpenGroup(Group self, char const * name, char ** options=None) -> Group"""
         return _gdal.Group_OpenGroup(self, *args)
 
-    def OpenGroupFromFullname(self, *args):
+    def OpenGroupFromFullname(self, *args) -> "GDALGroupHS *":
         r"""OpenGroupFromFullname(Group self, char const * name, char ** options=None) -> Group"""
         return _gdal.Group_OpenGroupFromFullname(self, *args)
 
-    def GetVectorLayerNames(self, *args):
+    def GetVectorLayerNames(self, *args) -> "char **":
         r"""GetVectorLayerNames(Group self, char ** options=None) -> char **"""
         return _gdal.Group_GetVectorLayerNames(self, *args)
 
-    def OpenVectorLayer(self, *args):
+    def OpenVectorLayer(self, *args) -> "OGRLayerShadow *":
         r"""OpenVectorLayer(Group self, char const * name, char ** options=None) -> Layer"""
         return _gdal.Group_OpenVectorLayer(self, *args)
 
-    def GetDimensions(self, *args):
+    def GetDimensions(self, *args) -> "void":
         r"""GetDimensions(Group self, char ** options=None)"""
         return _gdal.Group_GetDimensions(self, *args)
 
-    def GetAttribute(self, *args):
+    def GetAttribute(self, *args) -> "GDALAttributeHS *":
         r"""GetAttribute(Group self, char const * name) -> Attribute"""
         return _gdal.Group_GetAttribute(self, *args)
 
-    def GetAttributes(self, *args):
+    def GetAttributes(self, *args) -> "void":
         r"""GetAttributes(Group self, char ** options=None)"""
         return _gdal.Group_GetAttributes(self, *args)
 
-    def GetStructuralInfo(self, *args):
+    def GetStructuralInfo(self, *args) -> "char **":
         r"""GetStructuralInfo(Group self) -> char **"""
         return _gdal.Group_GetStructuralInfo(self, *args)
 
-    def CreateGroup(self, *args):
+    def CreateGroup(self, *args) -> "GDALGroupHS *":
         r"""CreateGroup(Group self, char const * name, char ** options=None) -> Group"""
         return _gdal.Group_CreateGroup(self, *args)
 
-    def CreateDimension(self, *args):
+    def CreateDimension(self, *args) -> "GDALDimensionHS *":
         r"""CreateDimension(Group self, char const * name, char const * type, char const * direction, unsigned long long size, char ** options=None) -> Dimension"""
         return _gdal.Group_CreateDimension(self, *args)
 
-    def CreateMDArray(self, *args):
+    def CreateMDArray(self, *args) -> "GDALMDArrayHS *":
         r"""CreateMDArray(Group self, char const * name, int nDimensions, ExtendedDataType data_type, char ** options=None) -> MDArray"""
         return _gdal.Group_CreateMDArray(self, *args)
 
-    def CreateAttribute(self, *args):
+    def CreateAttribute(self, *args) -> "GDALAttributeHS *":
         r"""CreateAttribute(Group self, char const * name, int nDimensions, ExtendedDataType data_type, char ** options=None) -> Attribute"""
         return _gdal.Group_CreateAttribute(self, *args)
 
 # Register Group in _gdal:
 _gdal.Group_swigregister(Group)
 
 class Statistics(object):
@@ -2696,199 +3063,199 @@
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
 
     def __init__(self, *args, **kwargs):
         raise AttributeError("No constructor defined")
     __repr__ = _swig_repr
     __swig_destroy__ = _gdal.delete_MDArray
 
-    def GetName(self, *args):
+    def GetName(self, *args) -> "char const *":
         r"""GetName(MDArray self) -> char const *"""
         return _gdal.MDArray_GetName(self, *args)
 
-    def GetFullName(self, *args):
+    def GetFullName(self, *args) -> "char const *":
         r"""GetFullName(MDArray self) -> char const *"""
         return _gdal.MDArray_GetFullName(self, *args)
 
-    def GetTotalElementsCount(self, *args):
+    def GetTotalElementsCount(self, *args) -> "unsigned long long":
         r"""GetTotalElementsCount(MDArray self) -> unsigned long long"""
         return _gdal.MDArray_GetTotalElementsCount(self, *args)
 
-    def GetDimensionCount(self, *args):
+    def GetDimensionCount(self, *args) -> "size_t":
         r"""GetDimensionCount(MDArray self) -> size_t"""
         return _gdal.MDArray_GetDimensionCount(self, *args)
 
-    def GetDimensions(self, *args):
+    def GetDimensions(self, *args) -> "void":
         r"""GetDimensions(MDArray self)"""
         return _gdal.MDArray_GetDimensions(self, *args)
 
-    def GetCoordinateVariables(self, *args):
+    def GetCoordinateVariables(self, *args) -> "void":
         r"""GetCoordinateVariables(MDArray self)"""
         return _gdal.MDArray_GetCoordinateVariables(self, *args)
 
-    def GetBlockSize(self, *args):
+    def GetBlockSize(self, *args) -> "void":
         r"""GetBlockSize(MDArray self)"""
         return _gdal.MDArray_GetBlockSize(self, *args)
 
-    def GetProcessingChunkSize(self, *args):
+    def GetProcessingChunkSize(self, *args) -> "void":
         r"""GetProcessingChunkSize(MDArray self, size_t nMaxChunkMemory)"""
         return _gdal.MDArray_GetProcessingChunkSize(self, *args)
 
-    def GetDataType(self, *args):
+    def GetDataType(self, *args) -> "GDALExtendedDataTypeHS *":
         r"""GetDataType(MDArray self) -> ExtendedDataType"""
         return _gdal.MDArray_GetDataType(self, *args)
 
-    def GetStructuralInfo(self, *args):
+    def GetStructuralInfo(self, *args) -> "char **":
         r"""GetStructuralInfo(MDArray self) -> char **"""
         return _gdal.MDArray_GetStructuralInfo(self, *args)
 
-    def Read(self, *args):
+    def Read(self, *args) -> "CPLErr":
         r"""Read(MDArray self, int nDims1, int nDims2, int nDims3, int nDims4, ExtendedDataType buffer_datatype) -> CPLErr"""
         return _gdal.MDArray_Read(self, *args)
 
-    def WriteStringArray(self, *args):
+    def WriteStringArray(self, *args) -> "CPLErr":
         r"""WriteStringArray(MDArray self, int nDims1, int nDims2, int nDims3, ExtendedDataType buffer_datatype, char ** options) -> CPLErr"""
         return _gdal.MDArray_WriteStringArray(self, *args)
 
-    def Write(self, *args):
+    def Write(self, *args) -> "CPLErr":
         r"""Write(MDArray self, int nDims1, int nDims2, int nDims3, int nDims4, ExtendedDataType buffer_datatype, GIntBig buf_len) -> CPLErr"""
         return _gdal.MDArray_Write(self, *args)
 
-    def AdviseRead(self, *args):
+    def AdviseRead(self, *args) -> "CPLErr":
         r"""AdviseRead(MDArray self, int nDims1, int nDims2, char ** options=None) -> CPLErr"""
         return _gdal.MDArray_AdviseRead(self, *args)
 
-    def GetAttribute(self, *args):
+    def GetAttribute(self, *args) -> "GDALAttributeHS *":
         r"""GetAttribute(MDArray self, char const * name) -> Attribute"""
         return _gdal.MDArray_GetAttribute(self, *args)
 
-    def GetAttributes(self, *args):
+    def GetAttributes(self, *args) -> "void":
         r"""GetAttributes(MDArray self, char ** options=None)"""
         return _gdal.MDArray_GetAttributes(self, *args)
 
-    def CreateAttribute(self, *args):
+    def CreateAttribute(self, *args) -> "GDALAttributeHS *":
         r"""CreateAttribute(MDArray self, char const * name, int nDimensions, ExtendedDataType data_type, char ** options=None) -> Attribute"""
         return _gdal.MDArray_CreateAttribute(self, *args)
 
-    def GetNoDataValueAsRaw(self, *args):
+    def GetNoDataValueAsRaw(self, *args) -> "CPLErr":
         r"""GetNoDataValueAsRaw(MDArray self) -> CPLErr"""
         return _gdal.MDArray_GetNoDataValueAsRaw(self, *args)
 
-    def GetNoDataValueAsDouble(self, *args):
+    def GetNoDataValueAsDouble(self, *args) -> "void":
         r"""GetNoDataValueAsDouble(MDArray self)"""
         return _gdal.MDArray_GetNoDataValueAsDouble(self, *args)
 
-    def GetNoDataValueAsInt64(self, *args):
+    def GetNoDataValueAsInt64(self, *args) -> "void":
         r"""GetNoDataValueAsInt64(MDArray self)"""
         return _gdal.MDArray_GetNoDataValueAsInt64(self, *args)
 
-    def GetNoDataValueAsUInt64(self, *args):
+    def GetNoDataValueAsUInt64(self, *args) -> "void":
         r"""GetNoDataValueAsUInt64(MDArray self)"""
         return _gdal.MDArray_GetNoDataValueAsUInt64(self, *args)
 
-    def GetNoDataValueAsString(self, *args):
+    def GetNoDataValueAsString(self, *args) -> "retStringAndCPLFree *":
         r"""GetNoDataValueAsString(MDArray self) -> retStringAndCPLFree *"""
         return _gdal.MDArray_GetNoDataValueAsString(self, *args)
 
-    def SetNoDataValueDouble(self, *args):
+    def SetNoDataValueDouble(self, *args) -> "CPLErr":
         r"""SetNoDataValueDouble(MDArray self, double d) -> CPLErr"""
         return _gdal.MDArray_SetNoDataValueDouble(self, *args)
 
-    def SetNoDataValueInt64(self, *args):
+    def SetNoDataValueInt64(self, *args) -> "CPLErr":
         r"""SetNoDataValueInt64(MDArray self, GIntBig v) -> CPLErr"""
         return _gdal.MDArray_SetNoDataValueInt64(self, *args)
 
-    def SetNoDataValueUInt64(self, *args):
+    def SetNoDataValueUInt64(self, *args) -> "CPLErr":
         r"""SetNoDataValueUInt64(MDArray self, GUIntBig v) -> CPLErr"""
         return _gdal.MDArray_SetNoDataValueUInt64(self, *args)
 
-    def SetNoDataValueString(self, *args):
+    def SetNoDataValueString(self, *args) -> "CPLErr":
         r"""SetNoDataValueString(MDArray self, char const * nodata) -> CPLErr"""
         return _gdal.MDArray_SetNoDataValueString(self, *args)
 
-    def SetNoDataValueRaw(self, *args):
+    def SetNoDataValueRaw(self, *args) -> "CPLErr":
         r"""SetNoDataValueRaw(MDArray self, GIntBig nLen) -> CPLErr"""
         return _gdal.MDArray_SetNoDataValueRaw(self, *args)
 
-    def DeleteNoDataValue(self, *args):
+    def DeleteNoDataValue(self, *args) -> "CPLErr":
         r"""DeleteNoDataValue(MDArray self) -> CPLErr"""
         return _gdal.MDArray_DeleteNoDataValue(self, *args)
 
-    def GetOffset(self, *args):
+    def GetOffset(self, *args) -> "void":
         r"""GetOffset(MDArray self)"""
         return _gdal.MDArray_GetOffset(self, *args)
 
-    def GetOffsetStorageType(self, *args):
+    def GetOffsetStorageType(self, *args) -> "GDALDataType":
         r"""GetOffsetStorageType(MDArray self) -> GDALDataType"""
         return _gdal.MDArray_GetOffsetStorageType(self, *args)
 
-    def GetScale(self, *args):
+    def GetScale(self, *args) -> "void":
         r"""GetScale(MDArray self)"""
         return _gdal.MDArray_GetScale(self, *args)
 
-    def GetScaleStorageType(self, *args):
+    def GetScaleStorageType(self, *args) -> "GDALDataType":
         r"""GetScaleStorageType(MDArray self) -> GDALDataType"""
         return _gdal.MDArray_GetScaleStorageType(self, *args)
 
-    def SetOffset(self, *args, **kwargs):
+    def SetOffset(self, *args, **kwargs) -> "CPLErr":
         r"""SetOffset(MDArray self, double val, GDALDataType storageType=GDT_Unknown) -> CPLErr"""
         return _gdal.MDArray_SetOffset(self, *args, **kwargs)
 
-    def SetScale(self, *args, **kwargs):
+    def SetScale(self, *args, **kwargs) -> "CPLErr":
         r"""SetScale(MDArray self, double val, GDALDataType storageType=GDT_Unknown) -> CPLErr"""
         return _gdal.MDArray_SetScale(self, *args, **kwargs)
 
-    def SetUnit(self, *args):
+    def SetUnit(self, *args) -> "CPLErr":
         r"""SetUnit(MDArray self, char const * unit) -> CPLErr"""
         return _gdal.MDArray_SetUnit(self, *args)
 
-    def GetUnit(self, *args):
+    def GetUnit(self, *args) -> "char const *":
         r"""GetUnit(MDArray self) -> char const *"""
         return _gdal.MDArray_GetUnit(self, *args)
 
-    def SetSpatialRef(self, *args):
+    def SetSpatialRef(self, *args) -> "OGRErr":
         r"""SetSpatialRef(MDArray self, SpatialReference srs) -> OGRErr"""
         return _gdal.MDArray_SetSpatialRef(self, *args)
 
-    def GetSpatialRef(self, *args):
+    def GetSpatialRef(self, *args) -> "OSRSpatialReferenceShadow *":
         r"""GetSpatialRef(MDArray self) -> SpatialReference"""
         return _gdal.MDArray_GetSpatialRef(self, *args)
 
-    def GetView(self, *args):
+    def GetView(self, *args) -> "GDALMDArrayHS *":
         r"""GetView(MDArray self, char const * viewExpr) -> MDArray"""
         return _gdal.MDArray_GetView(self, *args)
 
-    def Transpose(self, *args):
+    def Transpose(self, *args) -> "GDALMDArrayHS *":
         r"""Transpose(MDArray self, int nList) -> MDArray"""
         return _gdal.MDArray_Transpose(self, *args)
 
-    def GetUnscaled(self, *args):
+    def GetUnscaled(self, *args) -> "GDALMDArrayHS *":
         r"""GetUnscaled(MDArray self) -> MDArray"""
         return _gdal.MDArray_GetUnscaled(self, *args)
 
-    def GetMask(self, *args):
+    def GetMask(self, *args) -> "GDALMDArrayHS *":
         r"""GetMask(MDArray self, char ** options=None) -> MDArray"""
         return _gdal.MDArray_GetMask(self, *args)
 
-    def AsClassicDataset(self, *args):
+    def AsClassicDataset(self, *args) -> "GDALDatasetShadow *":
         r"""AsClassicDataset(MDArray self, size_t iXDim, size_t iYDim) -> Dataset"""
         return _gdal.MDArray_AsClassicDataset(self, *args)
 
-    def GetStatistics(self, *args, **kwargs):
+    def GetStatistics(self, *args, **kwargs) -> "Statistics *":
         r"""GetStatistics(MDArray self, bool approx_ok=FALSE, bool force=TRUE, GDALProgressFunc callback=0, void * callback_data=None) -> Statistics"""
         return _gdal.MDArray_GetStatistics(self, *args, **kwargs)
 
-    def ComputeStatistics(self, *args, **kwargs):
+    def ComputeStatistics(self, *args, **kwargs) -> "Statistics *":
         r"""ComputeStatistics(MDArray self, bool approx_ok=FALSE, GDALProgressFunc callback=0, void * callback_data=None) -> Statistics"""
         return _gdal.MDArray_ComputeStatistics(self, *args, **kwargs)
 
-    def GetResampled(self, *args):
+    def GetResampled(self, *args) -> "GDALMDArrayHS *":
         r"""GetResampled(MDArray self, int nDimensions, GDALRIOResampleAlg resample_alg, OSRSpatialReferenceShadow ** srs, char ** options=None) -> MDArray"""
         return _gdal.MDArray_GetResampled(self, *args)
 
-    def Cache(self, *args):
+    def Cache(self, *args) -> "bool":
         r"""Cache(MDArray self, char ** options=None) -> bool"""
         return _gdal.MDArray_Cache(self, *args)
 
     def Read(self,
              array_start_idx = None,
              count = None,
              array_step = None,
@@ -2975,23 +3342,23 @@
            count is None and buffer_stride is None and buffer_datatype is None:
             return self.WriteArray(buffer, array_start_idx=array_start_idx, array_step=array_step)
 
     # Special case for buffer of type array and 1D arrays
         if dimCount == 1 and type(buffer).__name__ == 'array' and \
            count is None and buffer_stride is None and buffer_datatype is None:
             map_typecode_itemsize_to_gdal = {
-               ('B',1): GDT_Byte,
-               ('h',2): GDT_Int16,
-               ('H',2): GDT_UInt16,
-               ('i',4): GDT_Int32,
-               ('I',4): GDT_UInt32,
-               ('l',4): GDT_Int32,
-    # ('l',8): GDT_Int64,
-    # ('q',8): GDT_Int64,
-    # ('Q',8): GDT_UInt64,
+               ('B', 1): GDT_Byte,
+               ('h', 2): GDT_Int16,
+               ('H', 2): GDT_UInt16,
+               ('i', 4): GDT_Int32,
+               ('I', 4): GDT_UInt32,
+               ('l', 4): GDT_Int32,
+    # ('l', 8): GDT_Int64,
+    # ('q', 8): GDT_Int64,
+    # ('Q', 8): GDT_UInt64,
                ('f', 4): GDT_Float32,
                ('d', 8): GDT_Float64
             }
             key = (buffer.typecode, buffer.itemsize)
             if key not in map_typecode_itemsize_to_gdal:
                 raise Exception("unhandled type for buffer of type array")
             buffer_datatype = ExtendedDataType.Create(map_typecode_itemsize_to_gdal[key])
@@ -3074,14 +3441,15 @@
       shp = ()
       for dim in self.GetDimensions():
         shp += (dim.GetSize(),)
       return shp
 
     shape = property(fget=GetShape, doc='Returns the shape of the array.')
 
+
     def GetNoDataValue(self):
       """GetNoDataValue(MDArray self) -> value """
 
       dt = self.GetDataType()
       if dt.GetClass() == GEDTC_NUMERIC and dt.GetNumericDataType() == gdalconst.GDT_Int64:
           return _gdal.MDArray_GetNoDataValueAsInt64(self)
 
@@ -3100,101 +3468,100 @@
 
       if dt.GetClass() == GEDTC_NUMERIC and dt.GetNumericDataType() == gdalconst.GDT_UInt64:
           return _gdal.MDArray_SetNoDataValueUInt64(self, value)
 
       return _gdal.MDArray_SetNoDataValueDouble(self, value)
 
 
-
 # Register MDArray in _gdal:
 _gdal.MDArray_swigregister(MDArray)
 
 class Attribute(object):
     r"""Proxy of C++ GDALAttributeHS class."""
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
 
     def __init__(self, *args, **kwargs):
         raise AttributeError("No constructor defined")
     __repr__ = _swig_repr
     __swig_destroy__ = _gdal.delete_Attribute
 
-    def GetName(self, *args):
+    def GetName(self, *args) -> "char const *":
         r"""GetName(Attribute self) -> char const *"""
         return _gdal.Attribute_GetName(self, *args)
 
-    def GetFullName(self, *args):
+    def GetFullName(self, *args) -> "char const *":
         r"""GetFullName(Attribute self) -> char const *"""
         return _gdal.Attribute_GetFullName(self, *args)
 
-    def GetTotalElementsCount(self, *args):
+    def GetTotalElementsCount(self, *args) -> "unsigned long long":
         r"""GetTotalElementsCount(Attribute self) -> unsigned long long"""
         return _gdal.Attribute_GetTotalElementsCount(self, *args)
 
-    def GetDimensionCount(self, *args):
+    def GetDimensionCount(self, *args) -> "size_t":
         r"""GetDimensionCount(Attribute self) -> size_t"""
         return _gdal.Attribute_GetDimensionCount(self, *args)
 
-    def GetDimensionsSize(self, *args):
+    def GetDimensionsSize(self, *args) -> "void":
         r"""GetDimensionsSize(Attribute self)"""
         return _gdal.Attribute_GetDimensionsSize(self, *args)
 
-    def GetDataType(self, *args):
+    def GetDataType(self, *args) -> "GDALExtendedDataTypeHS *":
         r"""GetDataType(Attribute self) -> ExtendedDataType"""
         return _gdal.Attribute_GetDataType(self, *args)
 
-    def ReadAsRaw(self, *args):
+    def ReadAsRaw(self, *args) -> "CPLErr":
         r"""ReadAsRaw(Attribute self) -> CPLErr"""
         return _gdal.Attribute_ReadAsRaw(self, *args)
 
-    def ReadAsString(self, *args):
+    def ReadAsString(self, *args) -> "char const *":
         r"""ReadAsString(Attribute self) -> char const *"""
         return _gdal.Attribute_ReadAsString(self, *args)
 
-    def ReadAsInt(self, *args):
+    def ReadAsInt(self, *args) -> "int":
         r"""ReadAsInt(Attribute self) -> int"""
         return _gdal.Attribute_ReadAsInt(self, *args)
 
-    def ReadAsDouble(self, *args):
+    def ReadAsDouble(self, *args) -> "double":
         r"""ReadAsDouble(Attribute self) -> double"""
         return _gdal.Attribute_ReadAsDouble(self, *args)
 
-    def ReadAsStringArray(self, *args):
+    def ReadAsStringArray(self, *args) -> "char **":
         r"""ReadAsStringArray(Attribute self) -> char **"""
         return _gdal.Attribute_ReadAsStringArray(self, *args)
 
-    def ReadAsIntArray(self, *args):
+    def ReadAsIntArray(self, *args) -> "void":
         r"""ReadAsIntArray(Attribute self)"""
         return _gdal.Attribute_ReadAsIntArray(self, *args)
 
-    def ReadAsDoubleArray(self, *args):
+    def ReadAsDoubleArray(self, *args) -> "void":
         r"""ReadAsDoubleArray(Attribute self)"""
         return _gdal.Attribute_ReadAsDoubleArray(self, *args)
 
-    def WriteRaw(self, *args):
+    def WriteRaw(self, *args) -> "CPLErr":
         r"""WriteRaw(Attribute self, GIntBig nLen) -> CPLErr"""
         return _gdal.Attribute_WriteRaw(self, *args)
 
-    def WriteString(self, *args):
+    def WriteString(self, *args) -> "CPLErr":
         r"""WriteString(Attribute self, char const * val) -> CPLErr"""
         return _gdal.Attribute_WriteString(self, *args)
 
-    def WriteStringArray(self, *args):
+    def WriteStringArray(self, *args) -> "CPLErr":
         r"""WriteStringArray(Attribute self, char ** vals) -> CPLErr"""
         return _gdal.Attribute_WriteStringArray(self, *args)
 
-    def WriteInt(self, *args):
+    def WriteInt(self, *args) -> "CPLErr":
         r"""WriteInt(Attribute self, int val) -> CPLErr"""
         return _gdal.Attribute_WriteInt(self, *args)
 
-    def WriteDouble(self, *args):
+    def WriteDouble(self, *args) -> "CPLErr":
         r"""WriteDouble(Attribute self, double val) -> CPLErr"""
         return _gdal.Attribute_WriteDouble(self, *args)
 
-    def WriteDoubleArray(self, *args):
+    def WriteDoubleArray(self, *args) -> "CPLErr":
         r"""WriteDoubleArray(Attribute self, int nList) -> CPLErr"""
         return _gdal.Attribute_WriteDoubleArray(self, *args)
 
 
     def Read(self):
       """ Read an attribute and return it with the most appropriate type """
       dt = self.GetDataType()
@@ -3259,39 +3626,39 @@
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
 
     def __init__(self, *args, **kwargs):
         raise AttributeError("No constructor defined")
     __repr__ = _swig_repr
     __swig_destroy__ = _gdal.delete_Dimension
 
-    def GetName(self, *args):
+    def GetName(self, *args) -> "char const *":
         r"""GetName(Dimension self) -> char const *"""
         return _gdal.Dimension_GetName(self, *args)
 
-    def GetFullName(self, *args):
+    def GetFullName(self, *args) -> "char const *":
         r"""GetFullName(Dimension self) -> char const *"""
         return _gdal.Dimension_GetFullName(self, *args)
 
-    def GetType(self, *args):
+    def GetType(self, *args) -> "char const *":
         r"""GetType(Dimension self) -> char const *"""
         return _gdal.Dimension_GetType(self, *args)
 
-    def GetDirection(self, *args):
+    def GetDirection(self, *args) -> "char const *":
         r"""GetDirection(Dimension self) -> char const *"""
         return _gdal.Dimension_GetDirection(self, *args)
 
-    def GetSize(self, *args):
+    def GetSize(self, *args) -> "unsigned long long":
         r"""GetSize(Dimension self) -> unsigned long long"""
         return _gdal.Dimension_GetSize(self, *args)
 
-    def GetIndexingVariable(self, *args):
+    def GetIndexingVariable(self, *args) -> "GDALMDArrayHS *":
         r"""GetIndexingVariable(Dimension self) -> MDArray"""
         return _gdal.Dimension_GetIndexingVariable(self, *args)
 
-    def SetIndexingVariable(self, *args):
+    def SetIndexingVariable(self, *args) -> "bool":
         r"""SetIndexingVariable(Dimension self, MDArray array) -> bool"""
         return _gdal.Dimension_SetIndexingVariable(self, *args)
 
 # Register Dimension in _gdal:
 _gdal.Dimension_swigregister(Dimension)
 
 GEDTC_NUMERIC = _gdal.GEDTC_NUMERIC
@@ -3307,118 +3674,118 @@
 
     def __init__(self, *args, **kwargs):
         raise AttributeError("No constructor defined")
     __repr__ = _swig_repr
     __swig_destroy__ = _gdal.delete_ExtendedDataType
 
     @staticmethod
-    def Create(*args):
+    def Create(*args) -> "GDALExtendedDataTypeHS *":
         r"""Create(GDALDataType dt) -> ExtendedDataType"""
         return _gdal.ExtendedDataType_Create(*args)
 
     @staticmethod
-    def CreateString(*args):
+    def CreateString(*args) -> "GDALExtendedDataTypeHS *":
         r"""CreateString(size_t nMaxStringLength=0, GDALExtendedDataTypeSubType eSubType=GEDTST_NONE) -> ExtendedDataType"""
         return _gdal.ExtendedDataType_CreateString(*args)
 
     @staticmethod
-    def CreateCompound(*args):
+    def CreateCompound(*args) -> "GDALExtendedDataTypeHS *":
         r"""CreateCompound(char const * name, size_t nTotalSize, int nComps) -> ExtendedDataType"""
         return _gdal.ExtendedDataType_CreateCompound(*args)
 
-    def GetName(self, *args):
+    def GetName(self, *args) -> "char const *":
         r"""GetName(ExtendedDataType self) -> char const *"""
         return _gdal.ExtendedDataType_GetName(self, *args)
 
-    def GetClass(self, *args):
+    def GetClass(self, *args) -> "GDALExtendedDataTypeClass":
         r"""GetClass(ExtendedDataType self) -> GDALExtendedDataTypeClass"""
         return _gdal.ExtendedDataType_GetClass(self, *args)
 
-    def GetNumericDataType(self, *args):
+    def GetNumericDataType(self, *args) -> "GDALDataType":
         r"""GetNumericDataType(ExtendedDataType self) -> GDALDataType"""
         return _gdal.ExtendedDataType_GetNumericDataType(self, *args)
 
-    def GetSize(self, *args):
+    def GetSize(self, *args) -> "size_t":
         r"""GetSize(ExtendedDataType self) -> size_t"""
         return _gdal.ExtendedDataType_GetSize(self, *args)
 
-    def GetMaxStringLength(self, *args):
+    def GetMaxStringLength(self, *args) -> "size_t":
         r"""GetMaxStringLength(ExtendedDataType self) -> size_t"""
         return _gdal.ExtendedDataType_GetMaxStringLength(self, *args)
 
-    def GetSubType(self, *args):
+    def GetSubType(self, *args) -> "GDALExtendedDataTypeSubType":
         r"""GetSubType(ExtendedDataType self) -> GDALExtendedDataTypeSubType"""
         return _gdal.ExtendedDataType_GetSubType(self, *args)
 
-    def GetComponents(self, *args):
+    def GetComponents(self, *args) -> "void":
         r"""GetComponents(ExtendedDataType self)"""
         return _gdal.ExtendedDataType_GetComponents(self, *args)
 
-    def CanConvertTo(self, *args):
+    def CanConvertTo(self, *args) -> "bool":
         r"""CanConvertTo(ExtendedDataType self, ExtendedDataType other) -> bool"""
         return _gdal.ExtendedDataType_CanConvertTo(self, *args)
 
-    def Equals(self, *args):
+    def Equals(self, *args) -> "bool":
         r"""Equals(ExtendedDataType self, ExtendedDataType other) -> bool"""
         return _gdal.ExtendedDataType_Equals(self, *args)
 
 
     def __eq__(self, other):
       return self.Equals(other)
 
     def __ne__(self, other):
       return not self.__eq__(other)
 
 
 # Register ExtendedDataType in _gdal:
 _gdal.ExtendedDataType_swigregister(ExtendedDataType)
 
-def ExtendedDataType_Create(*args):
+def ExtendedDataType_Create(*args) -> "GDALExtendedDataTypeHS *":
     r"""ExtendedDataType_Create(GDALDataType dt) -> ExtendedDataType"""
     return _gdal.ExtendedDataType_Create(*args)
 
-def ExtendedDataType_CreateString(*args):
+def ExtendedDataType_CreateString(*args) -> "GDALExtendedDataTypeHS *":
     r"""ExtendedDataType_CreateString(size_t nMaxStringLength=0, GDALExtendedDataTypeSubType eSubType=GEDTST_NONE) -> ExtendedDataType"""
     return _gdal.ExtendedDataType_CreateString(*args)
 
-def ExtendedDataType_CreateCompound(*args):
+def ExtendedDataType_CreateCompound(*args) -> "GDALExtendedDataTypeHS *":
     r"""ExtendedDataType_CreateCompound(char const * name, size_t nTotalSize, int nComps) -> ExtendedDataType"""
     return _gdal.ExtendedDataType_CreateCompound(*args)
 
 class EDTComponent(object):
     r"""Proxy of C++ GDALEDTComponentHS class."""
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
 
     def __init__(self, *args, **kwargs):
         raise AttributeError("No constructor defined")
     __repr__ = _swig_repr
     __swig_destroy__ = _gdal.delete_EDTComponent
 
     @staticmethod
-    def Create(*args):
+    def Create(*args) -> "GDALEDTComponentHS *":
         r"""Create(char const * name, size_t offset, ExtendedDataType type) -> EDTComponent"""
         return _gdal.EDTComponent_Create(*args)
 
-    def GetName(self, *args):
+    def GetName(self, *args) -> "char const *":
         r"""GetName(EDTComponent self) -> char const *"""
         return _gdal.EDTComponent_GetName(self, *args)
 
-    def GetOffset(self, *args):
+    def GetOffset(self, *args) -> "size_t":
         r"""GetOffset(EDTComponent self) -> size_t"""
         return _gdal.EDTComponent_GetOffset(self, *args)
 
-    def GetType(self, *args):
+    def GetType(self, *args) -> "GDALExtendedDataTypeHS *":
         r"""GetType(EDTComponent self) -> ExtendedDataType"""
         return _gdal.EDTComponent_GetType(self, *args)
 
 # Register EDTComponent in _gdal:
 _gdal.EDTComponent_swigregister(EDTComponent)
 
-def EDTComponent_Create(*args):
+def EDTComponent_Create(*args) -> "GDALEDTComponentHS *":
     r"""EDTComponent_Create(char const * name, size_t offset, ExtendedDataType type) -> EDTComponent"""
     return _gdal.EDTComponent_Create(*args)
 
 class Band(MajorObject):
     r"""Proxy of C++ GDALRasterBandShadow class."""
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
@@ -3426,272 +3793,310 @@
     def __init__(self, *args, **kwargs):
         raise AttributeError("No constructor defined")
     __repr__ = _swig_repr
     XSize = property(_gdal.Band_XSize_get, doc=r"""XSize : int""")
     YSize = property(_gdal.Band_YSize_get, doc=r"""YSize : int""")
     DataType = property(_gdal.Band_DataType_get, doc=r"""DataType : GDALDataType""")
 
-    def GetDataset(self, *args):
+    def GetDataset(self, *args) -> "GDALDatasetShadow *":
         r"""GetDataset(Band self) -> Dataset"""
         return _gdal.Band_GetDataset(self, *args)
 
-    def GetBand(self, *args):
+    def GetBand(self, *args) -> "int":
         r"""GetBand(Band self) -> int"""
         return _gdal.Band_GetBand(self, *args)
 
-    def GetBlockSize(self, *args):
+    def GetBlockSize(self, *args) -> "void":
         r"""GetBlockSize(Band self)"""
         return _gdal.Band_GetBlockSize(self, *args)
 
-    def GetActualBlockSize(self, *args):
+    def GetActualBlockSize(self, *args) -> "void":
         r"""GetActualBlockSize(Band self, int nXBlockOff, int nYBlockOff)"""
         return _gdal.Band_GetActualBlockSize(self, *args)
 
-    def GetColorInterpretation(self, *args):
+    def GetColorInterpretation(self, *args) -> "GDALColorInterp":
         r"""GetColorInterpretation(Band self) -> GDALColorInterp"""
         return _gdal.Band_GetColorInterpretation(self, *args)
 
-    def GetRasterColorInterpretation(self, *args):
+    def GetRasterColorInterpretation(self, *args) -> "GDALColorInterp":
         r"""GetRasterColorInterpretation(Band self) -> GDALColorInterp"""
         return _gdal.Band_GetRasterColorInterpretation(self, *args)
 
-    def SetColorInterpretation(self, *args):
+    def SetColorInterpretation(self, *args) -> "CPLErr":
         r"""SetColorInterpretation(Band self, GDALColorInterp val) -> CPLErr"""
         return _gdal.Band_SetColorInterpretation(self, *args)
 
-    def SetRasterColorInterpretation(self, *args):
+    def SetRasterColorInterpretation(self, *args) -> "CPLErr":
         r"""SetRasterColorInterpretation(Band self, GDALColorInterp val) -> CPLErr"""
         return _gdal.Band_SetRasterColorInterpretation(self, *args)
 
-    def GetNoDataValue(self, *args):
-        r"""GetNoDataValue(Band self)"""
-        return _gdal.Band_GetNoDataValue(self, *args)
+    def GetNoDataValue(self):
+        """GetNoDataValue(Band self) -> value """
+
+        if self.DataType == gdalconst.GDT_Int64:
+            return _gdal.Band_GetNoDataValueAsInt64(self)
+
+        if self.DataType == gdalconst.GDT_UInt64:
+            return _gdal.Band_GetNoDataValueAsUInt64(self)
+
+        return _gdal.Band_GetNoDataValue(self)
+
 
-    def GetNoDataValueAsInt64(self, *args):
+
+    def GetNoDataValueAsInt64(self, *args) -> "void":
         r"""GetNoDataValueAsInt64(Band self)"""
         return _gdal.Band_GetNoDataValueAsInt64(self, *args)
 
-    def GetNoDataValueAsUInt64(self, *args):
+    def GetNoDataValueAsUInt64(self, *args) -> "void":
         r"""GetNoDataValueAsUInt64(Band self)"""
         return _gdal.Band_GetNoDataValueAsUInt64(self, *args)
 
-    def SetNoDataValue(self, *args):
-        r"""SetNoDataValue(Band self, double d) -> CPLErr"""
-        return _gdal.Band_SetNoDataValue(self, *args)
+    def SetNoDataValue(self, value) -> "CPLErr":
+        """SetNoDataValue(Band self, value) -> CPLErr"""
+
+        if self.DataType == gdalconst.GDT_Int64:
+            return _gdal.Band_SetNoDataValueAsInt64(self, value)
+
+        if self.DataType == gdalconst.GDT_UInt64:
+            return _gdal.Band_SetNoDataValueAsUInt64(self, value)
 
-    def SetNoDataValueAsInt64(self, *args):
+        return _gdal.Band_SetNoDataValue(self, value)
+
+
+
+    def SetNoDataValueAsInt64(self, *args) -> "CPLErr":
         r"""SetNoDataValueAsInt64(Band self, GIntBig v) -> CPLErr"""
         return _gdal.Band_SetNoDataValueAsInt64(self, *args)
 
-    def SetNoDataValueAsUInt64(self, *args):
+    def SetNoDataValueAsUInt64(self, *args) -> "CPLErr":
         r"""SetNoDataValueAsUInt64(Band self, GUIntBig v) -> CPLErr"""
         return _gdal.Band_SetNoDataValueAsUInt64(self, *args)
 
-    def DeleteNoDataValue(self, *args):
+    def DeleteNoDataValue(self, *args) -> "CPLErr":
         r"""DeleteNoDataValue(Band self) -> CPLErr"""
         return _gdal.Band_DeleteNoDataValue(self, *args)
 
-    def GetUnitType(self, *args):
+    def GetUnitType(self, *args) -> "char const *":
         r"""GetUnitType(Band self) -> char const *"""
         return _gdal.Band_GetUnitType(self, *args)
 
-    def SetUnitType(self, *args):
+    def SetUnitType(self, *args) -> "CPLErr":
         r"""SetUnitType(Band self, char const * val) -> CPLErr"""
         return _gdal.Band_SetUnitType(self, *args)
 
-    def GetRasterCategoryNames(self, *args):
+    def GetRasterCategoryNames(self, *args) -> "char **":
         r"""GetRasterCategoryNames(Band self) -> char **"""
         return _gdal.Band_GetRasterCategoryNames(self, *args)
 
-    def SetRasterCategoryNames(self, *args):
+    def SetRasterCategoryNames(self, *args) -> "CPLErr":
         r"""SetRasterCategoryNames(Band self, char ** names) -> CPLErr"""
         return _gdal.Band_SetRasterCategoryNames(self, *args)
 
-    def GetMinimum(self, *args):
+    def GetMinimum(self, *args) -> "void":
         r"""GetMinimum(Band self)"""
         return _gdal.Band_GetMinimum(self, *args)
 
-    def GetMaximum(self, *args):
+    def GetMaximum(self, *args) -> "void":
         r"""GetMaximum(Band self)"""
         return _gdal.Band_GetMaximum(self, *args)
 
-    def GetOffset(self, *args):
+    def GetOffset(self, *args) -> "void":
         r"""GetOffset(Band self)"""
         return _gdal.Band_GetOffset(self, *args)
 
-    def GetScale(self, *args):
+    def GetScale(self, *args) -> "void":
         r"""GetScale(Band self)"""
         return _gdal.Band_GetScale(self, *args)
 
-    def SetOffset(self, *args):
+    def SetOffset(self, *args) -> "CPLErr":
         r"""SetOffset(Band self, double val) -> CPLErr"""
         return _gdal.Band_SetOffset(self, *args)
 
-    def SetScale(self, *args):
+    def SetScale(self, *args) -> "CPLErr":
         r"""SetScale(Band self, double val) -> CPLErr"""
         return _gdal.Band_SetScale(self, *args)
 
-    def GetStatistics(self, *args):
+    def GetStatistics(self, *args) -> "CPLErr":
         r"""GetStatistics(Band self, int approx_ok, int force) -> CPLErr"""
         return _gdal.Band_GetStatistics(self, *args)
 
-    def ComputeStatistics(self, *args):
-        r"""ComputeStatistics(Band self, bool approx_ok, GDALProgressFunc callback=0, void * callback_data=None) -> CPLErr"""
-        return _gdal.Band_ComputeStatistics(self, *args)
+    def ComputeStatistics(self, *args, **kwargs) -> "CPLErr":
+        """ComputeStatistics(Band self, bool approx_ok, callback=None, callback_data=None) -> CPLErr"""
+
+        if len(args) == 1:
+            kwargs["approx_ok"] = args[0]
+            args = ()
+
+        if "approx_ok" in kwargs:
+    # Compatibility with older signature that used int for approx_ok
+            if kwargs["approx_ok"] == 0:
+                kwargs["approx_ok"] = False
+            elif kwargs["approx_ok"] == 1:
+                kwargs["approx_ok"] = True
+            elif isinstance(kwargs["approx_ok"], int):
+                raise Exception("approx_ok value should be 0/1/False/True")
+
+        return _gdal.Band_ComputeStatistics(self, *args, **kwargs)
+
+
 
-    def SetStatistics(self, *args):
+    def SetStatistics(self, *args) -> "CPLErr":
         r"""SetStatistics(Band self, double min, double max, double mean, double stddev) -> CPLErr"""
         return _gdal.Band_SetStatistics(self, *args)
 
-    def GetOverviewCount(self, *args):
+    def GetOverviewCount(self, *args) -> "int":
         r"""GetOverviewCount(Band self) -> int"""
         return _gdal.Band_GetOverviewCount(self, *args)
 
-    def GetOverview(self, *args):
+    def GetOverview(self, *args) -> "GDALRasterBandShadow *":
         r"""GetOverview(Band self, int i) -> Band"""
         return _gdal.Band_GetOverview(self, *args)
 
-    def Checksum(self, *args, **kwargs):
+    def Checksum(self, *args, **kwargs) -> "int":
         r"""Checksum(Band self, int xoff=0, int yoff=0, int * xsize=None, int * ysize=None) -> int"""
         return _gdal.Band_Checksum(self, *args, **kwargs)
 
-    def ComputeRasterMinMax(self, *args):
-        r"""ComputeRasterMinMax(Band self, int approx_ok=0)"""
-        return _gdal.Band_ComputeRasterMinMax(self, *args)
+    def ComputeRasterMinMax(self, *args, **kwargs):
+        """ComputeRasterMinMax(Band self, bool approx_ok=False, bool can_return_none=False) -> (min, max) or None"""
 
-    def ComputeBandStats(self, *args):
+        if len(args) == 1:
+            kwargs["approx_ok"] = args[0]
+            args = ()
+
+        if "approx_ok" in kwargs:
+    # Compatibility with older signature that used int for approx_ok
+            if kwargs["approx_ok"] == 0:
+                kwargs["approx_ok"] = False
+            elif kwargs["approx_ok"] == 1:
+                kwargs["approx_ok"] = True
+            elif isinstance(kwargs["approx_ok"], int):
+                raise Exception("approx_ok value should be 0/1/False/True")
+
+    # can_return_null is used in other methods
+        if "can_return_null" in kwargs:
+            kwargs["can_return_none"] = kwargs["can_return_null"];
+            del kwargs["can_return_null"]
+
+        return _gdal.Band_ComputeRasterMinMax(self, *args, **kwargs)
+
+
+
+    def ComputeBandStats(self, *args) -> "void":
         r"""ComputeBandStats(Band self, int samplestep=1)"""
         return _gdal.Band_ComputeBandStats(self, *args)
 
-    def Fill(self, *args):
+    def Fill(self, *args) -> "CPLErr":
         r"""Fill(Band self, double real_fill, double imag_fill=0.0) -> CPLErr"""
         return _gdal.Band_Fill(self, *args)
 
-    def WriteRaster(self, *args, **kwargs):
+    def WriteRaster(self, *args, **kwargs) -> "CPLErr":
         r"""WriteRaster(Band self, int xoff, int yoff, int xsize, int ysize, GIntBig buf_len, int * buf_xsize=None, int * buf_ysize=None, GDALDataType * buf_type=None, GIntBig * buf_pixel_space=None, GIntBig * buf_line_space=None) -> CPLErr"""
         return _gdal.Band_WriteRaster(self, *args, **kwargs)
 
-    def FlushCache(self, *args):
+    def FlushCache(self, *args) -> "void":
         r"""FlushCache(Band self)"""
         return _gdal.Band_FlushCache(self, *args)
 
-    def GetRasterColorTable(self, *args):
+    def GetRasterColorTable(self, *args) -> "GDALColorTableShadow *":
         r"""GetRasterColorTable(Band self) -> ColorTable"""
         return _gdal.Band_GetRasterColorTable(self, *args)
 
-    def GetColorTable(self, *args):
+    def GetColorTable(self, *args) -> "GDALColorTableShadow *":
         r"""GetColorTable(Band self) -> ColorTable"""
         return _gdal.Band_GetColorTable(self, *args)
 
-    def SetRasterColorTable(self, *args):
+    def SetRasterColorTable(self, *args) -> "int":
         r"""SetRasterColorTable(Band self, ColorTable arg) -> int"""
         return _gdal.Band_SetRasterColorTable(self, *args)
 
-    def SetColorTable(self, *args):
+    def SetColorTable(self, *args) -> "int":
         r"""SetColorTable(Band self, ColorTable arg) -> int"""
         return _gdal.Band_SetColorTable(self, *args)
 
-    def GetDefaultRAT(self, *args):
+    def GetDefaultRAT(self, *args) -> "GDALRasterAttributeTableShadow *":
         r"""GetDefaultRAT(Band self) -> RasterAttributeTable"""
         return _gdal.Band_GetDefaultRAT(self, *args)
 
-    def SetDefaultRAT(self, *args):
+    def SetDefaultRAT(self, *args) -> "int":
         r"""SetDefaultRAT(Band self, RasterAttributeTable table) -> int"""
         return _gdal.Band_SetDefaultRAT(self, *args)
 
-    def GetMaskBand(self, *args):
+    def GetMaskBand(self, *args) -> "GDALRasterBandShadow *":
         r"""GetMaskBand(Band self) -> Band"""
         return _gdal.Band_GetMaskBand(self, *args)
 
-    def GetMaskFlags(self, *args):
+    def GetMaskFlags(self, *args) -> "int":
         r"""GetMaskFlags(Band self) -> int"""
         return _gdal.Band_GetMaskFlags(self, *args)
 
-    def CreateMaskBand(self, *args):
+    def CreateMaskBand(self, *args) -> "CPLErr":
         r"""CreateMaskBand(Band self, int nFlags) -> CPLErr"""
         return _gdal.Band_CreateMaskBand(self, *args)
 
-    def IsMaskBand(self, *args):
+    def IsMaskBand(self, *args) -> "bool":
         r"""IsMaskBand(Band self) -> bool"""
         return _gdal.Band_IsMaskBand(self, *args)
 
-    def GetHistogram(self, *args, **kwargs):
+    def GetHistogram(self, *args, **kwargs) -> "CPLErr":
         r"""GetHistogram(Band self, double min=-0.5, double max=255.5, int buckets=256, int include_out_of_range=0, int approx_ok=1, GDALProgressFunc callback=0, void * callback_data=None) -> CPLErr"""
         return _gdal.Band_GetHistogram(self, *args, **kwargs)
 
-    def GetDefaultHistogram(self, *args, **kwargs):
+    def GetDefaultHistogram(self, *args, **kwargs) -> "CPLErr":
         r"""GetDefaultHistogram(Band self, double * min_ret=None, double * max_ret=None, int * buckets_ret=None, GUIntBig ** ppanHistogram=None, int force=1, GDALProgressFunc callback=0, void * callback_data=None) -> CPLErr"""
         return _gdal.Band_GetDefaultHistogram(self, *args, **kwargs)
 
-    def SetDefaultHistogram(self, *args):
+    def SetDefaultHistogram(self, *args) -> "CPLErr":
         r"""SetDefaultHistogram(Band self, double min, double max, int buckets_in) -> CPLErr"""
         return _gdal.Band_SetDefaultHistogram(self, *args)
 
-    def HasArbitraryOverviews(self, *args):
+    def HasArbitraryOverviews(self, *args) -> "bool":
         r"""HasArbitraryOverviews(Band self) -> bool"""
         return _gdal.Band_HasArbitraryOverviews(self, *args)
 
-    def GetCategoryNames(self, *args):
+    def GetCategoryNames(self, *args) -> "char **":
         r"""GetCategoryNames(Band self) -> char **"""
         return _gdal.Band_GetCategoryNames(self, *args)
 
-    def SetCategoryNames(self, *args):
+    def SetCategoryNames(self, *args) -> "CPLErr":
         r"""SetCategoryNames(Band self, char ** papszCategoryNames) -> CPLErr"""
         return _gdal.Band_SetCategoryNames(self, *args)
 
-    def GetVirtualMem(self, *args, **kwargs):
+    def GetVirtualMem(self, *args, **kwargs) -> "CPLVirtualMemShadow *":
         r"""GetVirtualMem(Band self, GDALRWFlag eRWFlag, int nXOff, int nYOff, int nXSize, int nYSize, int nBufXSize, int nBufYSize, GDALDataType eBufType, size_t nCacheSize, size_t nPageSizeHint, char ** options=None) -> VirtualMem"""
         return _gdal.Band_GetVirtualMem(self, *args, **kwargs)
 
-    def GetVirtualMemAuto(self, *args, **kwargs):
+    def GetVirtualMemAuto(self, *args, **kwargs) -> "CPLVirtualMemShadow *":
         r"""GetVirtualMemAuto(Band self, GDALRWFlag eRWFlag, char ** options=None) -> VirtualMem"""
         return _gdal.Band_GetVirtualMemAuto(self, *args, **kwargs)
 
-    def GetTiledVirtualMem(self, *args, **kwargs):
+    def GetTiledVirtualMem(self, *args, **kwargs) -> "CPLVirtualMemShadow *":
         r"""GetTiledVirtualMem(Band self, GDALRWFlag eRWFlag, int nXOff, int nYOff, int nXSize, int nYSize, int nTileXSize, int nTileYSize, GDALDataType eBufType, size_t nCacheSize, char ** options=None) -> VirtualMem"""
         return _gdal.Band_GetTiledVirtualMem(self, *args, **kwargs)
 
-    def GetDataCoverageStatus(self, *args):
+    def GetDataCoverageStatus(self, *args) -> "int":
         r"""GetDataCoverageStatus(Band self, int nXOff, int nYOff, int nXSize, int nYSize, int nMaskFlagStop=0) -> int"""
         return _gdal.Band_GetDataCoverageStatus(self, *args)
 
-    def AdviseRead(self, *args):
+    def AdviseRead(self, *args) -> "CPLErr":
         r"""AdviseRead(Band self, int xoff, int yoff, int xsize, int ysize, int * buf_xsize=None, int * buf_ysize=None, GDALDataType * buf_type=None, char ** options=None) -> CPLErr"""
         return _gdal.Band_AdviseRead(self, *args)
 
-    def AsMDArray(self, *args):
+    def AsMDArray(self, *args) -> "GDALMDArrayHS *":
         r"""AsMDArray(Band self) -> MDArray"""
         return _gdal.Band_AsMDArray(self, *args)
 
-    def ReadRaster1(self, *args, **kwargs):
+    def ReadRaster1(self, *args, **kwargs) -> "CPLErr":
         r"""ReadRaster1(Band self, double xoff, double yoff, double xsize, double ysize, int * buf_xsize=None, int * buf_ysize=None, GDALDataType * buf_type=None, GIntBig * buf_pixel_space=None, GIntBig * buf_line_space=None, GDALRIOResampleAlg resample_alg=GRIORA_NearestNeighbour, GDALProgressFunc callback=0, void * callback_data=None, void * inputOutputBuf=None) -> CPLErr"""
         return _gdal.Band_ReadRaster1(self, *args, **kwargs)
 
-    def ReadBlock(self, *args, **kwargs):
+    def ReadBlock(self, *args, **kwargs) -> "CPLErr":
         r"""ReadBlock(Band self, int xoff, int yoff, void * buf_obj=None) -> CPLErr"""
         return _gdal.Band_ReadBlock(self, *args, **kwargs)
 
 
-    def ComputeStatistics(self, *args):
-      """ComputeStatistics(Band self, bool approx_ok, GDALProgressFunc callback=0, void * callback_data=None) -> CPLErr"""
-
-    # For backward compatibility. New SWIG has stricter typing and really
-    # enforces bool
-      approx_ok = args[0]
-      if approx_ok == 0:
-          approx_ok = False
-      elif approx_ok == 1:
-          approx_ok = True
-      new_args = [approx_ok]
-      for arg in args[1:]:
-          new_args.append( arg )
-
-      return _gdal.Band_ComputeStatistics(self, *new_args)
-
-
     def ReadRaster(self, xoff=0, yoff=0, xsize=None, ysize=None,
                    buf_xsize=None, buf_ysize=None, buf_type=None,
                    buf_pixel_space=None, buf_line_space=None,
                    resample_alg=gdalconst.GRIORA_NearestNeighbour,
                    callback=None,
                    callback_data=None,
                    buf_obj=None):
@@ -3793,15 +4198,15 @@
              Any reference to the array must be dropped before the last reference to the
              related dataset is also dropped.
           """
           from osgeo import gdal_array
           if options is None:
               virtualmem = self.GetVirtualMemAuto(eAccess)
           else:
-              virtualmem = self.GetVirtualMemAuto(eAccess,options)
+              virtualmem = self.GetVirtualMemAuto(eAccess, options)
           return gdal_array.VirtualMemGetArray( virtualmem )
 
     def GetTiledVirtualMemArray(self, eAccess=gdalconst.GF_Read, xoff=0, yoff=0,
                              xsize=None, ysize=None, tilexsize=256, tileysize=256,
                              datatype=None,
                              cache_size = 10 * 1024 * 1024, options=None):
           """Return a NumPy array for the band, seen as a virtual memory mapping with
@@ -3814,42 +4219,19 @@
           if xsize is None:
               xsize = self.XSize
           if ysize is None:
               ysize = self.YSize
           if datatype is None:
               datatype = self.DataType
           if options is None:
-              virtualmem = self.GetTiledVirtualMem(eAccess,xoff,yoff,xsize,ysize,tilexsize,tileysize,datatype,cache_size)
+              virtualmem = self.GetTiledVirtualMem(eAccess, xoff, yoff, xsize, ysize, tilexsize, tileysize, datatype, cache_size)
           else:
-              virtualmem = self.GetTiledVirtualMem(eAccess,xoff,yoff,xsize,ysize,tilexsize,tileysize,datatype,cache_size,options)
+              virtualmem = self.GetTiledVirtualMem(eAccess, xoff, yoff, xsize, ysize, tilexsize, tileysize, datatype, cache_size, options)
           return gdal_array.VirtualMemGetArray( virtualmem )
 
-    def GetNoDataValue(self):
-      """GetNoDataValue(Band self) -> value """
-
-      if self.DataType == gdalconst.GDT_Int64:
-          return _gdal.Band_GetNoDataValueAsInt64(self)
-
-      if self.DataType == gdalconst.GDT_UInt64:
-          return _gdal.Band_GetNoDataValueAsUInt64(self)
-
-      return _gdal.Band_GetNoDataValue(self)
-
-
-    def SetNoDataValue(self, value):
-      """SetNoDataValue(Band self, value) -> CPLErr"""
-
-      if self.DataType == gdalconst.GDT_Int64:
-          return _gdal.Band_SetNoDataValueAsInt64(self, value)
-
-      if self.DataType == gdalconst.GDT_UInt64:
-          return _gdal.Band_SetNoDataValueAsUInt64(self, value)
-
-      return _gdal.Band_SetNoDataValue(self, value)
-
 
 
 # Register Band in _gdal:
 _gdal.Band_swigregister(Band)
 
 class ColorTable(object):
     r"""Proxy of C++ GDALColorTableShadow class."""
@@ -3858,39 +4240,39 @@
     __repr__ = _swig_repr
 
     def __init__(self, *args, **kwargs):
         r"""__init__(ColorTable self, GDALPaletteInterp palette=GPI_RGB) -> ColorTable"""
         _gdal.ColorTable_swiginit(self, _gdal.new_ColorTable(*args, **kwargs))
     __swig_destroy__ = _gdal.delete_ColorTable
 
-    def Clone(self, *args):
+    def Clone(self, *args) -> "GDALColorTableShadow *":
         r"""Clone(ColorTable self) -> ColorTable"""
         return _gdal.ColorTable_Clone(self, *args)
 
-    def GetPaletteInterpretation(self, *args):
+    def GetPaletteInterpretation(self, *args) -> "GDALPaletteInterp":
         r"""GetPaletteInterpretation(ColorTable self) -> GDALPaletteInterp"""
         return _gdal.ColorTable_GetPaletteInterpretation(self, *args)
 
-    def GetCount(self, *args):
+    def GetCount(self, *args) -> "int":
         r"""GetCount(ColorTable self) -> int"""
         return _gdal.ColorTable_GetCount(self, *args)
 
-    def GetColorEntry(self, *args):
+    def GetColorEntry(self, *args) -> "GDALColorEntry *":
         r"""GetColorEntry(ColorTable self, int entry) -> ColorEntry"""
         return _gdal.ColorTable_GetColorEntry(self, *args)
 
-    def GetColorEntryAsRGB(self, *args):
+    def GetColorEntryAsRGB(self, *args) -> "int":
         r"""GetColorEntryAsRGB(ColorTable self, int entry, ColorEntry centry) -> int"""
         return _gdal.ColorTable_GetColorEntryAsRGB(self, *args)
 
-    def SetColorEntry(self, *args):
+    def SetColorEntry(self, *args) -> "void":
         r"""SetColorEntry(ColorTable self, int entry, ColorEntry centry)"""
         return _gdal.ColorTable_SetColorEntry(self, *args)
 
-    def CreateColorRamp(self, *args):
+    def CreateColorRamp(self, *args) -> "void":
         r"""CreateColorRamp(ColorTable self, int nStartIndex, ColorEntry startcolor, int nEndIndex, ColorEntry endcolor)"""
         return _gdal.ColorTable_CreateColorRamp(self, *args)
 
 # Register ColorTable in _gdal:
 _gdal.ColorTable_swigregister(ColorTable)
 
 class RasterAttributeTable(object):
@@ -3900,99 +4282,99 @@
     __repr__ = _swig_repr
 
     def __init__(self, *args):
         r"""__init__(RasterAttributeTable self) -> RasterAttributeTable"""
         _gdal.RasterAttributeTable_swiginit(self, _gdal.new_RasterAttributeTable(*args))
     __swig_destroy__ = _gdal.delete_RasterAttributeTable
 
-    def Clone(self, *args):
+    def Clone(self, *args) -> "GDALRasterAttributeTableShadow *":
         r"""Clone(RasterAttributeTable self) -> RasterAttributeTable"""
         return _gdal.RasterAttributeTable_Clone(self, *args)
 
-    def GetColumnCount(self, *args):
+    def GetColumnCount(self, *args) -> "int":
         r"""GetColumnCount(RasterAttributeTable self) -> int"""
         return _gdal.RasterAttributeTable_GetColumnCount(self, *args)
 
-    def GetNameOfCol(self, *args):
+    def GetNameOfCol(self, *args) -> "char const *":
         r"""GetNameOfCol(RasterAttributeTable self, int iCol) -> char const *"""
         return _gdal.RasterAttributeTable_GetNameOfCol(self, *args)
 
-    def GetUsageOfCol(self, *args):
+    def GetUsageOfCol(self, *args) -> "GDALRATFieldUsage":
         r"""GetUsageOfCol(RasterAttributeTable self, int iCol) -> GDALRATFieldUsage"""
         return _gdal.RasterAttributeTable_GetUsageOfCol(self, *args)
 
-    def GetTypeOfCol(self, *args):
+    def GetTypeOfCol(self, *args) -> "GDALRATFieldType":
         r"""GetTypeOfCol(RasterAttributeTable self, int iCol) -> GDALRATFieldType"""
         return _gdal.RasterAttributeTable_GetTypeOfCol(self, *args)
 
-    def GetColOfUsage(self, *args):
+    def GetColOfUsage(self, *args) -> "int":
         r"""GetColOfUsage(RasterAttributeTable self, GDALRATFieldUsage eUsage) -> int"""
         return _gdal.RasterAttributeTable_GetColOfUsage(self, *args)
 
-    def GetRowCount(self, *args):
+    def GetRowCount(self, *args) -> "int":
         r"""GetRowCount(RasterAttributeTable self) -> int"""
         return _gdal.RasterAttributeTable_GetRowCount(self, *args)
 
-    def GetValueAsString(self, *args):
+    def GetValueAsString(self, *args) -> "char const *":
         r"""GetValueAsString(RasterAttributeTable self, int iRow, int iCol) -> char const *"""
         return _gdal.RasterAttributeTable_GetValueAsString(self, *args)
 
-    def GetValueAsInt(self, *args):
+    def GetValueAsInt(self, *args) -> "int":
         r"""GetValueAsInt(RasterAttributeTable self, int iRow, int iCol) -> int"""
         return _gdal.RasterAttributeTable_GetValueAsInt(self, *args)
 
-    def GetValueAsDouble(self, *args):
+    def GetValueAsDouble(self, *args) -> "double":
         r"""GetValueAsDouble(RasterAttributeTable self, int iRow, int iCol) -> double"""
         return _gdal.RasterAttributeTable_GetValueAsDouble(self, *args)
 
-    def SetValueAsString(self, *args):
+    def SetValueAsString(self, *args) -> "void":
         r"""SetValueAsString(RasterAttributeTable self, int iRow, int iCol, char const * pszValue)"""
         return _gdal.RasterAttributeTable_SetValueAsString(self, *args)
 
-    def SetValueAsInt(self, *args):
+    def SetValueAsInt(self, *args) -> "void":
         r"""SetValueAsInt(RasterAttributeTable self, int iRow, int iCol, int nValue)"""
         return _gdal.RasterAttributeTable_SetValueAsInt(self, *args)
 
-    def SetValueAsDouble(self, *args):
+    def SetValueAsDouble(self, *args) -> "void":
         r"""SetValueAsDouble(RasterAttributeTable self, int iRow, int iCol, double dfValue)"""
         return _gdal.RasterAttributeTable_SetValueAsDouble(self, *args)
 
-    def SetRowCount(self, *args):
+    def SetRowCount(self, *args) -> "void":
         r"""SetRowCount(RasterAttributeTable self, int nCount)"""
         return _gdal.RasterAttributeTable_SetRowCount(self, *args)
 
-    def CreateColumn(self, *args):
+    def CreateColumn(self, *args) -> "int":
         r"""CreateColumn(RasterAttributeTable self, char const * pszName, GDALRATFieldType eType, GDALRATFieldUsage eUsage) -> int"""
         return _gdal.RasterAttributeTable_CreateColumn(self, *args)
 
-    def GetLinearBinning(self, *args):
+    def GetLinearBinning(self, *args) -> "bool":
         r"""GetLinearBinning(RasterAttributeTable self) -> bool"""
         return _gdal.RasterAttributeTable_GetLinearBinning(self, *args)
 
-    def SetLinearBinning(self, *args):
+    def SetLinearBinning(self, *args) -> "int":
         r"""SetLinearBinning(RasterAttributeTable self, double dfRow0Min, double dfBinSize) -> int"""
         return _gdal.RasterAttributeTable_SetLinearBinning(self, *args)
 
-    def GetRowOfValue(self, *args):
+    def GetRowOfValue(self, *args) -> "int":
         r"""GetRowOfValue(RasterAttributeTable self, double dfValue) -> int"""
         return _gdal.RasterAttributeTable_GetRowOfValue(self, *args)
 
-    def ChangesAreWrittenToFile(self, *args):
+    def ChangesAreWrittenToFile(self, *args) -> "int":
         r"""ChangesAreWrittenToFile(RasterAttributeTable self) -> int"""
         return _gdal.RasterAttributeTable_ChangesAreWrittenToFile(self, *args)
 
-    def DumpReadable(self, *args):
+    def DumpReadable(self, *args) -> "void":
         r"""DumpReadable(RasterAttributeTable self)"""
         return _gdal.RasterAttributeTable_DumpReadable(self, *args)
 
-    def SetTableType(self, *args):
+    def SetTableType(self, *args) -> "void":
         r"""SetTableType(RasterAttributeTable self, GDALRATTableType eTableType)"""
         return _gdal.RasterAttributeTable_SetTableType(self, *args)
 
-    def GetTableType(self, *args):
+    def GetTableType(self, *args) -> "GDALRATTableType":
         r"""GetTableType(RasterAttributeTable self) -> GDALRATTableType"""
         return _gdal.RasterAttributeTable_GetTableType(self, *args)
 
     def WriteArray(self, array, field, start=0):
         from osgeo import gdal_array
 
         return gdal_array.RATWriteArray(self, array, field, start)
@@ -4002,70 +4384,172 @@
 
         return gdal_array.RATReadArray(self, field, start, length)
 
 
 # Register RasterAttributeTable in _gdal:
 _gdal.RasterAttributeTable_swigregister(RasterAttributeTable)
 
+class Relationship(object):
+    r"""Proxy of C++ GDALRelationshipShadow class."""
+
+    thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
+    __repr__ = _swig_repr
+
+    def __init__(self, *args):
+        r"""__init__(Relationship self, char const * name, char const * leftTableName, char const * rightTableName, GDALRelationshipCardinality cardinality) -> Relationship"""
+        _gdal.Relationship_swiginit(self, _gdal.new_Relationship(*args))
+    __swig_destroy__ = _gdal.delete_Relationship
+
+    def GetName(self, *args) -> "char const *":
+        r"""GetName(Relationship self) -> char const *"""
+        return _gdal.Relationship_GetName(self, *args)
+
+    def GetCardinality(self, *args) -> "GDALRelationshipCardinality":
+        r"""GetCardinality(Relationship self) -> GDALRelationshipCardinality"""
+        return _gdal.Relationship_GetCardinality(self, *args)
+
+    def GetLeftTableName(self, *args) -> "char const *":
+        r"""GetLeftTableName(Relationship self) -> char const *"""
+        return _gdal.Relationship_GetLeftTableName(self, *args)
+
+    def GetRightTableName(self, *args) -> "char const *":
+        r"""GetRightTableName(Relationship self) -> char const *"""
+        return _gdal.Relationship_GetRightTableName(self, *args)
+
+    def GetMappingTableName(self, *args) -> "char const *":
+        r"""GetMappingTableName(Relationship self) -> char const *"""
+        return _gdal.Relationship_GetMappingTableName(self, *args)
+
+    def SetMappingTableName(self, *args) -> "void":
+        r"""SetMappingTableName(Relationship self, char const * pszName)"""
+        return _gdal.Relationship_SetMappingTableName(self, *args)
+
+    def GetLeftTableFields(self, *args) -> "char **":
+        r"""GetLeftTableFields(Relationship self) -> char **"""
+        return _gdal.Relationship_GetLeftTableFields(self, *args)
+
+    def GetRightTableFields(self, *args) -> "char **":
+        r"""GetRightTableFields(Relationship self) -> char **"""
+        return _gdal.Relationship_GetRightTableFields(self, *args)
+
+    def SetLeftTableFields(self, *args) -> "void":
+        r"""SetLeftTableFields(Relationship self, char ** pFields)"""
+        return _gdal.Relationship_SetLeftTableFields(self, *args)
+
+    def SetRightTableFields(self, *args) -> "void":
+        r"""SetRightTableFields(Relationship self, char ** pFields)"""
+        return _gdal.Relationship_SetRightTableFields(self, *args)
+
+    def GetLeftMappingTableFields(self, *args) -> "char **":
+        r"""GetLeftMappingTableFields(Relationship self) -> char **"""
+        return _gdal.Relationship_GetLeftMappingTableFields(self, *args)
+
+    def GetRightMappingTableFields(self, *args) -> "char **":
+        r"""GetRightMappingTableFields(Relationship self) -> char **"""
+        return _gdal.Relationship_GetRightMappingTableFields(self, *args)
+
+    def SetLeftMappingTableFields(self, *args) -> "void":
+        r"""SetLeftMappingTableFields(Relationship self, char ** pFields)"""
+        return _gdal.Relationship_SetLeftMappingTableFields(self, *args)
+
+    def SetRightMappingTableFields(self, *args) -> "void":
+        r"""SetRightMappingTableFields(Relationship self, char ** pFields)"""
+        return _gdal.Relationship_SetRightMappingTableFields(self, *args)
+
+    def GetType(self, *args) -> "GDALRelationshipType":
+        r"""GetType(Relationship self) -> GDALRelationshipType"""
+        return _gdal.Relationship_GetType(self, *args)
+
+    def SetType(self, *args) -> "void":
+        r"""SetType(Relationship self, GDALRelationshipType type)"""
+        return _gdal.Relationship_SetType(self, *args)
+
+    def GetForwardPathLabel(self, *args) -> "char const *":
+        r"""GetForwardPathLabel(Relationship self) -> char const *"""
+        return _gdal.Relationship_GetForwardPathLabel(self, *args)
+
+    def SetForwardPathLabel(self, *args) -> "void":
+        r"""SetForwardPathLabel(Relationship self, char const * pszLabel)"""
+        return _gdal.Relationship_SetForwardPathLabel(self, *args)
+
+    def GetBackwardPathLabel(self, *args) -> "char const *":
+        r"""GetBackwardPathLabel(Relationship self) -> char const *"""
+        return _gdal.Relationship_GetBackwardPathLabel(self, *args)
+
+    def SetBackwardPathLabel(self, *args) -> "void":
+        r"""SetBackwardPathLabel(Relationship self, char const * pszLabel)"""
+        return _gdal.Relationship_SetBackwardPathLabel(self, *args)
+
+    def GetRelatedTableType(self, *args) -> "char const *":
+        r"""GetRelatedTableType(Relationship self) -> char const *"""
+        return _gdal.Relationship_GetRelatedTableType(self, *args)
+
+    def SetRelatedTableType(self, *args) -> "void":
+        r"""SetRelatedTableType(Relationship self, char const * pszType)"""
+        return _gdal.Relationship_SetRelatedTableType(self, *args)
+
+# Register Relationship in _gdal:
+_gdal.Relationship_swigregister(Relationship)
+
 
-def TermProgress_nocb(*args, **kwargs):
+def TermProgress_nocb(*args, **kwargs) -> "int":
     r"""TermProgress_nocb(double dfProgress, char const * pszMessage=None, void * pData=None) -> int"""
     return _gdal.TermProgress_nocb(*args, **kwargs)
 TermProgress = _gdal.TermProgress
 
 
-def ComputeMedianCutPCT(*args, **kwargs):
+def ComputeMedianCutPCT(*args, **kwargs) -> "int":
     r"""ComputeMedianCutPCT(Band red, Band green, Band blue, int num_colors, ColorTable colors, GDALProgressFunc callback=0, void * callback_data=None) -> int"""
     return _gdal.ComputeMedianCutPCT(*args, **kwargs)
 
-def DitherRGB2PCT(*args, **kwargs):
+def DitherRGB2PCT(*args, **kwargs) -> "int":
     r"""DitherRGB2PCT(Band red, Band green, Band blue, Band target, ColorTable colors, GDALProgressFunc callback=0, void * callback_data=None) -> int"""
     return _gdal.DitherRGB2PCT(*args, **kwargs)
 
-def ReprojectImage(*args, **kwargs):
+def ReprojectImage(*args, **kwargs) -> "CPLErr":
     r"""ReprojectImage(Dataset src_ds, Dataset dst_ds, char const * src_wkt=None, char const * dst_wkt=None, GDALResampleAlg eResampleAlg=GRA_NearestNeighbour, double WarpMemoryLimit=0.0, double maxerror=0.0, GDALProgressFunc callback=0, void * callback_data=None, char ** options=None) -> CPLErr"""
     return _gdal.ReprojectImage(*args, **kwargs)
 
-def ComputeProximity(*args, **kwargs):
+def ComputeProximity(*args, **kwargs) -> "int":
     r"""ComputeProximity(Band srcBand, Band proximityBand, char ** options=None, GDALProgressFunc callback=0, void * callback_data=None) -> int"""
     return _gdal.ComputeProximity(*args, **kwargs)
 
-def RasterizeLayer(*args, **kwargs):
+def RasterizeLayer(*args, **kwargs) -> "int":
     r"""RasterizeLayer(Dataset dataset, int bands, Layer layer, void * pfnTransformer=None, void * pTransformArg=None, int burn_values=0, char ** options=None, GDALProgressFunc callback=0, void * callback_data=None) -> int"""
     return _gdal.RasterizeLayer(*args, **kwargs)
 
-def Polygonize(*args, **kwargs):
+def Polygonize(*args, **kwargs) -> "int":
     r"""Polygonize(Band srcBand, Band maskBand, Layer outLayer, int iPixValField, char ** options=None, GDALProgressFunc callback=0, void * callback_data=None) -> int"""
     return _gdal.Polygonize(*args, **kwargs)
 
-def FPolygonize(*args, **kwargs):
+def FPolygonize(*args, **kwargs) -> "int":
     r"""FPolygonize(Band srcBand, Band maskBand, Layer outLayer, int iPixValField, char ** options=None, GDALProgressFunc callback=0, void * callback_data=None) -> int"""
     return _gdal.FPolygonize(*args, **kwargs)
 
-def FillNodata(*args, **kwargs):
+def FillNodata(*args, **kwargs) -> "int":
     r"""FillNodata(Band targetBand, Band maskBand, double maxSearchDist, int smoothingIterations, char ** options=None, GDALProgressFunc callback=0, void * callback_data=None) -> int"""
     return _gdal.FillNodata(*args, **kwargs)
 
-def SieveFilter(*args, **kwargs):
+def SieveFilter(*args, **kwargs) -> "int":
     r"""SieveFilter(Band srcBand, Band maskBand, Band dstBand, int threshold, int connectedness=4, char ** options=None, GDALProgressFunc callback=0, void * callback_data=None) -> int"""
     return _gdal.SieveFilter(*args, **kwargs)
 
-def RegenerateOverviews(*args, **kwargs):
+def RegenerateOverviews(*args, **kwargs) -> "int":
     r"""RegenerateOverviews(Band srcBand, int overviewBandCount, char const * resampling="average", GDALProgressFunc callback=0, void * callback_data=None) -> int"""
     return _gdal.RegenerateOverviews(*args, **kwargs)
 
-def RegenerateOverview(*args, **kwargs):
+def RegenerateOverview(*args, **kwargs) -> "int":
     r"""RegenerateOverview(Band srcBand, Band overviewBand, char const * resampling="average", GDALProgressFunc callback=0, void * callback_data=None) -> int"""
     return _gdal.RegenerateOverview(*args, **kwargs)
 
-def ContourGenerate(*args, **kwargs):
+def ContourGenerate(*args, **kwargs) -> "int":
     r"""ContourGenerate(Band srcBand, double contourInterval, double contourBase, int fixedLevelCount, int useNoData, double noDataValue, Layer dstLayer, int idField, int elevField, GDALProgressFunc callback=0, void * callback_data=None) -> int"""
     return _gdal.ContourGenerate(*args, **kwargs)
 
-def ContourGenerateEx(*args, **kwargs):
+def ContourGenerateEx(*args, **kwargs) -> "int":
     r"""ContourGenerateEx(Band srcBand, Layer dstLayer, char ** options=None, GDALProgressFunc callback=0, void * callback_data=None) -> int"""
     return _gdal.ContourGenerateEx(*args, **kwargs)
 GVM_Diagonal = _gdal.GVM_Diagonal
 
 GVM_Edge = _gdal.GVM_Edge
 
 GVM_Max = _gdal.GVM_Max
@@ -4075,183 +4559,183 @@
 GVOT_NORMAL = _gdal.GVOT_NORMAL
 
 GVOT_MIN_TARGET_HEIGHT_FROM_DEM = _gdal.GVOT_MIN_TARGET_HEIGHT_FROM_DEM
 
 GVOT_MIN_TARGET_HEIGHT_FROM_GROUND = _gdal.GVOT_MIN_TARGET_HEIGHT_FROM_GROUND
 
 
-def ViewshedGenerate(*args, **kwargs):
+def ViewshedGenerate(*args, **kwargs) -> "GDALDatasetShadow *":
     r"""ViewshedGenerate(Band srcBand, char const * driverName, char const * targetRasterName, char ** creationOptions, double observerX, double observerY, double observerHeight, double targetHeight, double visibleVal, double invisibleVal, double outOfRangeVal, double noDataVal, double dfCurvCoeff, GDALViewshedMode mode, double maxDistance, GDALProgressFunc callback=0, void * callback_data=None, GDALViewshedOutputType heightMode=GVOT_NORMAL, char ** options=None) -> Dataset"""
     return _gdal.ViewshedGenerate(*args, **kwargs)
 
-def AutoCreateWarpedVRT(*args):
+def AutoCreateWarpedVRT(*args) -> "GDALDatasetShadow *":
     r"""AutoCreateWarpedVRT(Dataset src_ds, char const * src_wkt=None, char const * dst_wkt=None, GDALResampleAlg eResampleAlg=GRA_NearestNeighbour, double maxerror=0.0) -> Dataset"""
     return _gdal.AutoCreateWarpedVRT(*args)
 
-def CreatePansharpenedVRT(*args):
+def CreatePansharpenedVRT(*args) -> "GDALDatasetShadow *":
     r"""CreatePansharpenedVRT(char const * pszXML, Band panchroBand, int nInputSpectralBands) -> Dataset"""
     return _gdal.CreatePansharpenedVRT(*args)
 class GDALTransformerInfoShadow(object):
     r"""Proxy of C++ GDALTransformerInfoShadow class."""
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
 
     def __init__(self, *args, **kwargs):
         raise AttributeError("No constructor defined")
     __repr__ = _swig_repr
     __swig_destroy__ = _gdal.delete_GDALTransformerInfoShadow
 
-    def TransformPoint(self, *args):
+    def TransformPoint(self, *args) -> "int":
         r"""
         TransformPoint(GDALTransformerInfoShadow self, int bDstToSrc, double [3] inout) -> int
         TransformPoint(GDALTransformerInfoShadow self, int bDstToSrc, double x, double y, double z=0.0) -> int
         """
         return _gdal.GDALTransformerInfoShadow_TransformPoint(self, *args)
 
-    def TransformPoints(self, *args):
+    def TransformPoints(self, *args) -> "int":
         r"""TransformPoints(GDALTransformerInfoShadow self, int bDstToSrc, int nCount) -> int"""
         return _gdal.GDALTransformerInfoShadow_TransformPoints(self, *args)
 
-    def TransformGeolocations(self, *args, **kwargs):
+    def TransformGeolocations(self, *args, **kwargs) -> "int":
         r"""TransformGeolocations(GDALTransformerInfoShadow self, Band xBand, Band yBand, Band zBand, GDALProgressFunc callback=0, void * callback_data=None, char ** options=None) -> int"""
         return _gdal.GDALTransformerInfoShadow_TransformGeolocations(self, *args, **kwargs)
 
 # Register GDALTransformerInfoShadow in _gdal:
 _gdal.GDALTransformerInfoShadow_swigregister(GDALTransformerInfoShadow)
 
 
-def Transformer(*args):
+def Transformer(*args) -> "GDALTransformerInfoShadow *":
     r"""Transformer(Dataset src, Dataset dst, char ** options) -> GDALTransformerInfoShadow"""
     return _gdal.Transformer(*args)
 
-def _ApplyVerticalShiftGrid(*args, **kwargs):
+def _ApplyVerticalShiftGrid(*args, **kwargs) -> "GDALDatasetShadow *":
     r"""_ApplyVerticalShiftGrid(Dataset src_ds, Dataset grid_ds, bool inverse=False, double srcUnitToMeter=1.0, double dstUnitToMeter=1.0, char ** options=None) -> Dataset"""
     return _gdal._ApplyVerticalShiftGrid(*args, **kwargs)
 
-def ApplyGeoTransform(*args):
+def ApplyGeoTransform(*args) -> "double *, double *":
     r"""ApplyGeoTransform(double [6] padfGeoTransform, double dfPixel, double dfLine)"""
     return _gdal.ApplyGeoTransform(*args)
 
-def InvGeoTransform(*args):
+def InvGeoTransform(*args) -> "double [6]":
     r"""InvGeoTransform(double [6] gt_in) -> RETURN_NONE"""
     return _gdal.InvGeoTransform(*args)
 
-def VersionInfo(*args):
+def VersionInfo(*args) -> "char const *":
     r"""VersionInfo(char const * request="VERSION_NUM") -> char const *"""
     return _gdal.VersionInfo(*args)
 
-def AllRegister(*args):
+def AllRegister(*args) -> "void":
     r"""AllRegister()"""
     return _gdal.AllRegister(*args)
 
-def GDALDestroyDriverManager(*args):
+def GDALDestroyDriverManager(*args) -> "void":
     r"""GDALDestroyDriverManager()"""
     return _gdal.GDALDestroyDriverManager(*args)
 
-def GetCacheMax(*args):
+def GetCacheMax(*args) -> "GIntBig":
     r"""GetCacheMax() -> GIntBig"""
     return _gdal.GetCacheMax(*args)
 
-def GetCacheUsed(*args):
+def GetCacheUsed(*args) -> "GIntBig":
     r"""GetCacheUsed() -> GIntBig"""
     return _gdal.GetCacheUsed(*args)
 
-def SetCacheMax(*args):
+def SetCacheMax(*args) -> "void":
     r"""SetCacheMax(GIntBig nBytes)"""
     return _gdal.SetCacheMax(*args)
 
-def GetDataTypeSize(*args):
+def GetDataTypeSize(*args) -> "int":
     r"""GetDataTypeSize(GDALDataType eDataType) -> int"""
     return _gdal.GetDataTypeSize(*args)
 
-def DataTypeIsComplex(*args):
+def DataTypeIsComplex(*args) -> "int":
     r"""DataTypeIsComplex(GDALDataType eDataType) -> int"""
     return _gdal.DataTypeIsComplex(*args)
 
-def GetDataTypeName(*args):
+def GetDataTypeName(*args) -> "char const *":
     r"""GetDataTypeName(GDALDataType eDataType) -> char const *"""
     return _gdal.GetDataTypeName(*args)
 
-def GetDataTypeByName(*args):
+def GetDataTypeByName(*args) -> "GDALDataType":
     r"""GetDataTypeByName(char const * pszDataTypeName) -> GDALDataType"""
     return _gdal.GetDataTypeByName(*args)
 
-def DataTypeUnion(*args):
+def DataTypeUnion(*args) -> "GDALDataType":
     r"""DataTypeUnion(GDALDataType a, GDALDataType b) -> GDALDataType"""
     return _gdal.DataTypeUnion(*args)
 
-def GetColorInterpretationName(*args):
+def GetColorInterpretationName(*args) -> "char const *":
     r"""GetColorInterpretationName(GDALColorInterp eColorInterp) -> char const *"""
     return _gdal.GetColorInterpretationName(*args)
 
-def GetPaletteInterpretationName(*args):
+def GetPaletteInterpretationName(*args) -> "char const *":
     r"""GetPaletteInterpretationName(GDALPaletteInterp ePaletteInterp) -> char const *"""
     return _gdal.GetPaletteInterpretationName(*args)
 
-def DecToDMS(*args):
+def DecToDMS(*args) -> "char const *":
     r"""DecToDMS(double arg1, char const * arg2, int arg3=2) -> char const *"""
     return _gdal.DecToDMS(*args)
 
-def PackedDMSToDec(*args):
+def PackedDMSToDec(*args) -> "double":
     r"""PackedDMSToDec(double dfPacked) -> double"""
     return _gdal.PackedDMSToDec(*args)
 
-def DecToPackedDMS(*args):
+def DecToPackedDMS(*args) -> "double":
     r"""DecToPackedDMS(double dfDec) -> double"""
     return _gdal.DecToPackedDMS(*args)
 
-def ParseXMLString(*args):
+def ParseXMLString(*args) -> "CPLXMLNode *":
     r"""ParseXMLString(char * pszXMLString) -> CPLXMLNode *"""
     return _gdal.ParseXMLString(*args)
 
-def SerializeXMLTree(*args):
+def SerializeXMLTree(*args) -> "retStringAndCPLFree *":
     r"""SerializeXMLTree(CPLXMLNode * xmlnode) -> retStringAndCPLFree *"""
     return _gdal.SerializeXMLTree(*args)
 
-def GetJPEG2000Structure(*args):
+def GetJPEG2000Structure(*args) -> "CPLXMLNode *":
     r"""GetJPEG2000Structure(char const * pszFilename, char ** options=None) -> CPLXMLNode *"""
     return _gdal.GetJPEG2000Structure(*args)
 
-def GetJPEG2000StructureAsString(*args):
+def GetJPEG2000StructureAsString(*args) -> "retStringAndCPLFree *":
     r"""GetJPEG2000StructureAsString(char const * pszFilename, char ** options=None) -> retStringAndCPLFree *"""
     return _gdal.GetJPEG2000StructureAsString(*args)
 
-def GetDriverCount(*args):
+def GetDriverCount(*args) -> "int":
     r"""GetDriverCount() -> int"""
     return _gdal.GetDriverCount(*args)
 
-def GetDriverByName(*args):
+def GetDriverByName(*args) -> "GDALDriverShadow *":
     r"""GetDriverByName(char const * name) -> Driver"""
     return _gdal.GetDriverByName(*args)
 
-def GetDriver(*args):
+def GetDriver(*args) -> "GDALDriverShadow *":
     r"""GetDriver(int i) -> Driver"""
     return _gdal.GetDriver(*args)
 
-def Open(*args):
+def Open(*args) -> "GDALDatasetShadow *":
     r"""Open(char const * utf8_path, GDALAccess eAccess=GA_ReadOnly) -> Dataset"""
     return _gdal.Open(*args)
 
-def OpenEx(*args, **kwargs):
+def OpenEx(*args, **kwargs) -> "GDALDatasetShadow *":
     r"""OpenEx(char const * utf8_path, unsigned int nOpenFlags=0, char ** allowed_drivers=None, char ** open_options=None, char ** sibling_files=None) -> Dataset"""
     return _gdal.OpenEx(*args, **kwargs)
 
-def OpenShared(*args):
+def OpenShared(*args) -> "GDALDatasetShadow *":
     r"""OpenShared(char const * utf8_path, GDALAccess eAccess=GA_ReadOnly) -> Dataset"""
     return _gdal.OpenShared(*args)
 
-def IdentifyDriver(*args):
+def IdentifyDriver(*args) -> "GDALDriverShadow *":
     r"""IdentifyDriver(char const * utf8_path, char ** papszSiblings=None) -> Driver"""
     return _gdal.IdentifyDriver(*args)
 
-def IdentifyDriverEx(*args, **kwargs):
+def IdentifyDriverEx(*args, **kwargs) -> "GDALDriverShadow *":
     r"""IdentifyDriverEx(char const * utf8_path, unsigned int nIdentifyFlags=0, char ** allowed_drivers=None, char ** sibling_files=None) -> Driver"""
     return _gdal.IdentifyDriverEx(*args, **kwargs)
 
-def GeneralCmdLineProcessor(*args):
+def GeneralCmdLineProcessor(*args) -> "char **":
     r"""GeneralCmdLineProcessor(char ** papszArgv, int nOptions=0) -> char **"""
     return _gdal.GeneralCmdLineProcessor(*args)
 
 __version__ = _gdal.VersionInfo("RELEASE_NAME")
 
 class GDALInfoOptions(object):
     r"""Proxy of C++ GDALInfoOptions class."""
@@ -4264,15 +4748,15 @@
         _gdal.GDALInfoOptions_swiginit(self, _gdal.new_GDALInfoOptions(*args))
     __swig_destroy__ = _gdal.delete_GDALInfoOptions
 
 # Register GDALInfoOptions in _gdal:
 _gdal.GDALInfoOptions_swigregister(GDALInfoOptions)
 
 
-def InfoInternal(*args):
+def InfoInternal(*args) -> "retStringAndCPLFree *":
     r"""InfoInternal(Dataset hDataset, GDALInfoOptions infoOptions) -> retStringAndCPLFree *"""
     return _gdal.InfoInternal(*args)
 class GDALMultiDimInfoOptions(object):
     r"""Proxy of C++ GDALMultiDimInfoOptions class."""
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
@@ -4282,15 +4766,15 @@
         _gdal.GDALMultiDimInfoOptions_swiginit(self, _gdal.new_GDALMultiDimInfoOptions(*args))
     __swig_destroy__ = _gdal.delete_GDALMultiDimInfoOptions
 
 # Register GDALMultiDimInfoOptions in _gdal:
 _gdal.GDALMultiDimInfoOptions_swigregister(GDALMultiDimInfoOptions)
 
 
-def MultiDimInfoInternal(*args):
+def MultiDimInfoInternal(*args) -> "retStringAndCPLFree *":
     r"""MultiDimInfoInternal(Dataset hDataset, GDALMultiDimInfoOptions infoOptions) -> retStringAndCPLFree *"""
     return _gdal.MultiDimInfoInternal(*args)
 class GDALTranslateOptions(object):
     r"""Proxy of C++ GDALTranslateOptions class."""
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
@@ -4300,15 +4784,15 @@
         _gdal.GDALTranslateOptions_swiginit(self, _gdal.new_GDALTranslateOptions(*args))
     __swig_destroy__ = _gdal.delete_GDALTranslateOptions
 
 # Register GDALTranslateOptions in _gdal:
 _gdal.GDALTranslateOptions_swigregister(GDALTranslateOptions)
 
 
-def TranslateInternal(*args):
+def TranslateInternal(*args) -> "GDALDatasetShadow *":
     r"""TranslateInternal(char const * dest, Dataset dataset, GDALTranslateOptions translateOptions, GDALProgressFunc callback=0, void * callback_data=None) -> Dataset"""
     return _gdal.TranslateInternal(*args)
 class GDALWarpAppOptions(object):
     r"""Proxy of C++ GDALWarpAppOptions class."""
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
@@ -4318,19 +4802,19 @@
         _gdal.GDALWarpAppOptions_swiginit(self, _gdal.new_GDALWarpAppOptions(*args))
     __swig_destroy__ = _gdal.delete_GDALWarpAppOptions
 
 # Register GDALWarpAppOptions in _gdal:
 _gdal.GDALWarpAppOptions_swigregister(GDALWarpAppOptions)
 
 
-def wrapper_GDALWarpDestDS(*args):
+def wrapper_GDALWarpDestDS(*args) -> "int":
     r"""wrapper_GDALWarpDestDS(Dataset dstDS, int object_list_count, GDALWarpAppOptions warpAppOptions, GDALProgressFunc callback=0, void * callback_data=None) -> int"""
     return _gdal.wrapper_GDALWarpDestDS(*args)
 
-def wrapper_GDALWarpDestName(*args):
+def wrapper_GDALWarpDestName(*args) -> "GDALDatasetShadow *":
     r"""wrapper_GDALWarpDestName(char const * dest, int object_list_count, GDALWarpAppOptions warpAppOptions, GDALProgressFunc callback=0, void * callback_data=None) -> Dataset"""
     return _gdal.wrapper_GDALWarpDestName(*args)
 class GDALVectorTranslateOptions(object):
     r"""Proxy of C++ GDALVectorTranslateOptions class."""
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
@@ -4340,19 +4824,19 @@
         _gdal.GDALVectorTranslateOptions_swiginit(self, _gdal.new_GDALVectorTranslateOptions(*args))
     __swig_destroy__ = _gdal.delete_GDALVectorTranslateOptions
 
 # Register GDALVectorTranslateOptions in _gdal:
 _gdal.GDALVectorTranslateOptions_swigregister(GDALVectorTranslateOptions)
 
 
-def wrapper_GDALVectorTranslateDestDS(*args):
+def wrapper_GDALVectorTranslateDestDS(*args) -> "int":
     r"""wrapper_GDALVectorTranslateDestDS(Dataset dstDS, Dataset srcDS, GDALVectorTranslateOptions options, GDALProgressFunc callback=0, void * callback_data=None) -> int"""
     return _gdal.wrapper_GDALVectorTranslateDestDS(*args)
 
-def wrapper_GDALVectorTranslateDestName(*args):
+def wrapper_GDALVectorTranslateDestName(*args) -> "GDALDatasetShadow *":
     r"""wrapper_GDALVectorTranslateDestName(char const * dest, Dataset srcDS, GDALVectorTranslateOptions options, GDALProgressFunc callback=0, void * callback_data=None) -> Dataset"""
     return _gdal.wrapper_GDALVectorTranslateDestName(*args)
 class GDALDEMProcessingOptions(object):
     r"""Proxy of C++ GDALDEMProcessingOptions class."""
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
@@ -4362,15 +4846,15 @@
         _gdal.GDALDEMProcessingOptions_swiginit(self, _gdal.new_GDALDEMProcessingOptions(*args))
     __swig_destroy__ = _gdal.delete_GDALDEMProcessingOptions
 
 # Register GDALDEMProcessingOptions in _gdal:
 _gdal.GDALDEMProcessingOptions_swigregister(GDALDEMProcessingOptions)
 
 
-def DEMProcessingInternal(*args):
+def DEMProcessingInternal(*args) -> "GDALDatasetShadow *":
     r"""DEMProcessingInternal(char const * dest, Dataset dataset, char const * pszProcessing, char const * pszColorFilename, GDALDEMProcessingOptions options, GDALProgressFunc callback=0, void * callback_data=None) -> Dataset"""
     return _gdal.DEMProcessingInternal(*args)
 class GDALNearblackOptions(object):
     r"""Proxy of C++ GDALNearblackOptions class."""
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
@@ -4380,19 +4864,19 @@
         _gdal.GDALNearblackOptions_swiginit(self, _gdal.new_GDALNearblackOptions(*args))
     __swig_destroy__ = _gdal.delete_GDALNearblackOptions
 
 # Register GDALNearblackOptions in _gdal:
 _gdal.GDALNearblackOptions_swigregister(GDALNearblackOptions)
 
 
-def wrapper_GDALNearblackDestDS(*args):
+def wrapper_GDALNearblackDestDS(*args) -> "int":
     r"""wrapper_GDALNearblackDestDS(Dataset dstDS, Dataset srcDS, GDALNearblackOptions options, GDALProgressFunc callback=0, void * callback_data=None) -> int"""
     return _gdal.wrapper_GDALNearblackDestDS(*args)
 
-def wrapper_GDALNearblackDestName(*args):
+def wrapper_GDALNearblackDestName(*args) -> "GDALDatasetShadow *":
     r"""wrapper_GDALNearblackDestName(char const * dest, Dataset srcDS, GDALNearblackOptions options, GDALProgressFunc callback=0, void * callback_data=None) -> Dataset"""
     return _gdal.wrapper_GDALNearblackDestName(*args)
 class GDALGridOptions(object):
     r"""Proxy of C++ GDALGridOptions class."""
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
@@ -4402,15 +4886,15 @@
         _gdal.GDALGridOptions_swiginit(self, _gdal.new_GDALGridOptions(*args))
     __swig_destroy__ = _gdal.delete_GDALGridOptions
 
 # Register GDALGridOptions in _gdal:
 _gdal.GDALGridOptions_swigregister(GDALGridOptions)
 
 
-def GridInternal(*args):
+def GridInternal(*args) -> "GDALDatasetShadow *":
     r"""GridInternal(char const * dest, Dataset dataset, GDALGridOptions options, GDALProgressFunc callback=0, void * callback_data=None) -> Dataset"""
     return _gdal.GridInternal(*args)
 class GDALRasterizeOptions(object):
     r"""Proxy of C++ GDALRasterizeOptions class."""
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
@@ -4420,19 +4904,19 @@
         _gdal.GDALRasterizeOptions_swiginit(self, _gdal.new_GDALRasterizeOptions(*args))
     __swig_destroy__ = _gdal.delete_GDALRasterizeOptions
 
 # Register GDALRasterizeOptions in _gdal:
 _gdal.GDALRasterizeOptions_swigregister(GDALRasterizeOptions)
 
 
-def wrapper_GDALRasterizeDestDS(*args):
+def wrapper_GDALRasterizeDestDS(*args) -> "int":
     r"""wrapper_GDALRasterizeDestDS(Dataset dstDS, Dataset srcDS, GDALRasterizeOptions options, GDALProgressFunc callback=0, void * callback_data=None) -> int"""
     return _gdal.wrapper_GDALRasterizeDestDS(*args)
 
-def wrapper_GDALRasterizeDestName(*args):
+def wrapper_GDALRasterizeDestName(*args) -> "GDALDatasetShadow *":
     r"""wrapper_GDALRasterizeDestName(char const * dest, Dataset srcDS, GDALRasterizeOptions options, GDALProgressFunc callback=0, void * callback_data=None) -> Dataset"""
     return _gdal.wrapper_GDALRasterizeDestName(*args)
 class GDALBuildVRTOptions(object):
     r"""Proxy of C++ GDALBuildVRTOptions class."""
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
@@ -4442,19 +4926,19 @@
         _gdal.GDALBuildVRTOptions_swiginit(self, _gdal.new_GDALBuildVRTOptions(*args))
     __swig_destroy__ = _gdal.delete_GDALBuildVRTOptions
 
 # Register GDALBuildVRTOptions in _gdal:
 _gdal.GDALBuildVRTOptions_swigregister(GDALBuildVRTOptions)
 
 
-def BuildVRTInternalObjects(*args):
+def BuildVRTInternalObjects(*args) -> "GDALDatasetShadow *":
     r"""BuildVRTInternalObjects(char const * dest, int object_list_count, GDALBuildVRTOptions options, GDALProgressFunc callback=0, void * callback_data=None) -> Dataset"""
     return _gdal.BuildVRTInternalObjects(*args)
 
-def BuildVRTInternalNames(*args):
+def BuildVRTInternalNames(*args) -> "GDALDatasetShadow *":
     r"""BuildVRTInternalNames(char const * dest, char ** source_filenames, GDALBuildVRTOptions options, GDALProgressFunc callback=0, void * callback_data=None) -> Dataset"""
     return _gdal.BuildVRTInternalNames(*args)
 class GDALMultiDimTranslateOptions(object):
     r"""Proxy of C++ GDALMultiDimTranslateOptions class."""
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
@@ -4464,12 +4948,12 @@
         _gdal.GDALMultiDimTranslateOptions_swiginit(self, _gdal.new_GDALMultiDimTranslateOptions(*args))
     __swig_destroy__ = _gdal.delete_GDALMultiDimTranslateOptions
 
 # Register GDALMultiDimTranslateOptions in _gdal:
 _gdal.GDALMultiDimTranslateOptions_swigregister(GDALMultiDimTranslateOptions)
 
 
-def wrapper_GDALMultiDimTranslateDestName(*args):
+def wrapper_GDALMultiDimTranslateDestName(*args) -> "GDALDatasetShadow *":
     r"""wrapper_GDALMultiDimTranslateDestName(char const * dest, int object_list_count, GDALMultiDimTranslateOptions multiDimTranslateOptions, GDALProgressFunc callback=0, void * callback_data=None) -> Dataset"""
     return _gdal.wrapper_GDALMultiDimTranslateDestName(*args)
```

### Comparing `pygdal-3.5.3.11/osgeo/gdal_array.py` & `pygdal-3.6.4.11/osgeo/gdal_array.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,69 +68,73 @@
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
 
     def __init__(self, *args, **kwargs):
         raise AttributeError("No constructor defined")
     __repr__ = _swig_repr
     __swig_destroy__ = _gdal_array.delete_VirtualMem
 
-    def GetAddr(self):
+    def GetAddr(self) -> "void":
         r"""GetAddr(VirtualMem self)"""
         return _gdal_array.VirtualMem_GetAddr(self)
 
-    def Pin(self, start_offset=0, nsize=0, bWriteOp=0):
+    def Pin(self, start_offset: "size_t"=0, nsize: "size_t"=0, bWriteOp: "int"=0) -> "void":
         r"""Pin(VirtualMem self, size_t start_offset=0, size_t nsize=0, int bWriteOp=0)"""
         return _gdal_array.VirtualMem_Pin(self, start_offset, nsize, bWriteOp)
 
 # Register VirtualMem in _gdal_array:
 _gdal_array.VirtualMem_swigregister(VirtualMem)
 
 
-def _StoreLastException():
+def _StoreLastException() -> "void":
     r"""_StoreLastException()"""
     return _gdal_array._StoreLastException()
 
-def TermProgress_nocb(dfProgress, pszMessage=None, pData=None):
+def TermProgress_nocb(dfProgress: "double", pszMessage: "char const *"=None, pData: "void *"=None) -> "int":
     r"""TermProgress_nocb(double dfProgress, char const * pszMessage=None, void * pData=None) -> int"""
     return _gdal_array.TermProgress_nocb(dfProgress, pszMessage, pData)
 TermProgress = _gdal_array.TermProgress
 
 
-def OpenNumPyArray(psArray, binterleave):
+def OpenNumPyArray(psArray: "PyArrayObject *", binterleave: "bool") -> "GDALDatasetShadow *":
     r"""OpenNumPyArray(PyArrayObject * psArray, bool binterleave) -> Dataset"""
     return _gdal_array.OpenNumPyArray(psArray, binterleave)
 
-def OpenMultiDimensionalNumPyArray(psArray):
+def OpenMultiDimensionalNumPyArray(psArray: "PyArrayObject *") -> "GDALDatasetShadow *":
     r"""OpenMultiDimensionalNumPyArray(PyArrayObject * psArray) -> Dataset"""
     return _gdal_array.OpenMultiDimensionalNumPyArray(psArray)
 
-def GetArrayFilename(psArray):
+def GetArrayFilename(psArray: "PyArrayObject *") -> "retStringAndCPLFree *":
     r"""GetArrayFilename(PyArrayObject * psArray) -> retStringAndCPLFree *"""
     return _gdal_array.GetArrayFilename(psArray)
 
-def BandRasterIONumPy(band, bWrite, xoff, yoff, xsize, ysize, psArray, buf_type, resample_alg, callback=0, callback_data=None):
+def BandRasterIONumPy(band: "Band", bWrite: "int", xoff: "double", yoff: "double", xsize: "double", ysize: "double", psArray: "PyArrayObject *", buf_type: "GDALDataType", resample_alg: "GDALRIOResampleAlg", callback: "GDALProgressFunc"=0, callback_data: "void *"=None) -> "CPLErr":
     r"""BandRasterIONumPy(Band band, int bWrite, double xoff, double yoff, double xsize, double ysize, PyArrayObject * psArray, GDALDataType buf_type, GDALRIOResampleAlg resample_alg, GDALProgressFunc callback=0, void * callback_data=None) -> CPLErr"""
     return _gdal_array.BandRasterIONumPy(band, bWrite, xoff, yoff, xsize, ysize, psArray, buf_type, resample_alg, callback, callback_data)
 
-def DatasetIONumPy(ds, bWrite, xoff, yoff, xsize, ysize, psArray, buf_type, resample_alg, callback=0, callback_data=None, binterleave=True, band_list=0):
+def DatasetIONumPy(ds: "Dataset", bWrite: "int", xoff: "double", yoff: "double", xsize: "double", ysize: "double", psArray: "PyArrayObject *", buf_type: "GDALDataType", resample_alg: "GDALRIOResampleAlg", callback: "GDALProgressFunc"=0, callback_data: "void *"=None, binterleave: "bool"=True, band_list: "int"=0) -> "CPLErr":
     r"""DatasetIONumPy(Dataset ds, int bWrite, double xoff, double yoff, double xsize, double ysize, PyArrayObject * psArray, GDALDataType buf_type, GDALRIOResampleAlg resample_alg, GDALProgressFunc callback=0, void * callback_data=None, bool binterleave=True, int band_list=0) -> CPLErr"""
     return _gdal_array.DatasetIONumPy(ds, bWrite, xoff, yoff, xsize, ysize, psArray, buf_type, resample_alg, callback, callback_data, binterleave, band_list)
 
-def MDArrayIONumPy(bWrite, mdarray, psArray, nDims1, nDims3, buffer_datatype):
+def MDArrayIONumPy(bWrite: "bool", mdarray: "GDALMDArrayHS *", psArray: "PyArrayObject *", nDims1: "int", nDims3: "int", buffer_datatype: "GDALExtendedDataTypeHS *") -> "CPLErr":
     r"""MDArrayIONumPy(bool bWrite, GDALMDArrayHS * mdarray, PyArrayObject * psArray, int nDims1, int nDims3, GDALExtendedDataTypeHS * buffer_datatype) -> CPLErr"""
     return _gdal_array.MDArrayIONumPy(bWrite, mdarray, psArray, nDims1, nDims3, buffer_datatype)
 
-def VirtualMemGetArray(virtualmem):
+def _RecordBatchAsNumpy(recordBatchPtr: "VoidPtrAsLong", schemaPtr: "VoidPtrAsLong", pointerArrayKeeper: "PyObject *") -> "PyObject *":
+    r"""_RecordBatchAsNumpy(VoidPtrAsLong recordBatchPtr, VoidPtrAsLong schemaPtr, PyObject * pointerArrayKeeper) -> PyObject *"""
+    return _gdal_array._RecordBatchAsNumpy(recordBatchPtr, schemaPtr, pointerArrayKeeper)
+
+def VirtualMemGetArray(virtualmem: "VirtualMem") -> "int":
     r"""VirtualMemGetArray(VirtualMem virtualmem)"""
     return _gdal_array.VirtualMemGetArray(virtualmem)
 
-def RATValuesIONumPyWrite(poRAT, nField, nStart, psArray):
+def RATValuesIONumPyWrite(poRAT: "RasterAttributeTable", nField: "int", nStart: "int", psArray: "PyArrayObject *") -> "CPLErr":
     r"""RATValuesIONumPyWrite(RasterAttributeTable poRAT, int nField, int nStart, PyArrayObject * psArray) -> CPLErr"""
     return _gdal_array.RATValuesIONumPyWrite(poRAT, nField, nStart, psArray)
 
-def RATValuesIONumPyRead(poRAT, nField, nStart, nLength):
+def RATValuesIONumPyRead(poRAT: "RasterAttributeTable", nField: "int", nStart: "int", nLength: "int") -> "PyObject *":
     r"""RATValuesIONumPyRead(RasterAttributeTable poRAT, int nField, int nStart, int nLength) -> PyObject *"""
     return _gdal_array.RATValuesIONumPyRead(poRAT, nField, nStart, nLength)
 
 import numpy
 
 from osgeo import gdalconst
 from osgeo import gdal
```

### Comparing `pygdal-3.5.3.11/osgeo/gdalconst.py` & `pygdal-3.6.4.11/osgeo/gdalconst.py`

 * *Files 8% similar despite different names*

```diff
@@ -167,47 +167,68 @@
 DMD_CONNECTION_PREFIX = _gdalconst.DMD_CONNECTION_PREFIX
 DMD_EXTENSIONS = _gdalconst.DMD_EXTENSIONS
 DMD_CREATIONOPTIONLIST = _gdalconst.DMD_CREATIONOPTIONLIST
 DMD_MULTIDIM_DATASET_CREATIONOPTIONLIST = _gdalconst.DMD_MULTIDIM_DATASET_CREATIONOPTIONLIST
 DMD_MULTIDIM_GROUP_CREATIONOPTIONLIST = _gdalconst.DMD_MULTIDIM_GROUP_CREATIONOPTIONLIST
 DMD_MULTIDIM_DIMENSION_CREATIONOPTIONLIST = _gdalconst.DMD_MULTIDIM_DIMENSION_CREATIONOPTIONLIST
 DMD_MULTIDIM_ARRAY_CREATIONOPTIONLIST = _gdalconst.DMD_MULTIDIM_ARRAY_CREATIONOPTIONLIST
+DMD_MULTIDIM_ARRAY_OPENOPTIONLIST = _gdalconst.DMD_MULTIDIM_ARRAY_OPENOPTIONLIST
 DMD_MULTIDIM_ATTRIBUTE_CREATIONOPTIONLIST = _gdalconst.DMD_MULTIDIM_ATTRIBUTE_CREATIONOPTIONLIST
 DMD_OPENOPTIONLIST = _gdalconst.DMD_OPENOPTIONLIST
 DMD_CREATIONDATATYPES = _gdalconst.DMD_CREATIONDATATYPES
 DMD_CREATIONFIELDDATATYPES = _gdalconst.DMD_CREATIONFIELDDATATYPES
 DMD_CREATIONFIELDDATASUBTYPES = _gdalconst.DMD_CREATIONFIELDDATASUBTYPES
 DMD_SUBDATASETS = _gdalconst.DMD_SUBDATASETS
 DMD_CREATION_FIELD_DOMAIN_TYPES = _gdalconst.DMD_CREATION_FIELD_DOMAIN_TYPES
+DMD_ALTER_GEOM_FIELD_DEFN_FLAGS = _gdalconst.DMD_ALTER_GEOM_FIELD_DEFN_FLAGS
+DMD_SUPPORTED_SQL_DIALECTS = _gdalconst.DMD_SUPPORTED_SQL_DIALECTS
 DCAP_OPEN = _gdalconst.DCAP_OPEN
 DCAP_CREATE = _gdalconst.DCAP_CREATE
 DCAP_CREATE_MULTIDIMENSIONAL = _gdalconst.DCAP_CREATE_MULTIDIMENSIONAL
 DCAP_CREATECOPY = _gdalconst.DCAP_CREATECOPY
 DCAP_CREATECOPY_MULTIDIMENSIONAL = _gdalconst.DCAP_CREATECOPY_MULTIDIMENSIONAL
 DCAP_MULTIDIM_RASTER = _gdalconst.DCAP_MULTIDIM_RASTER
 DCAP_SUBCREATECOPY = _gdalconst.DCAP_SUBCREATECOPY
 DCAP_VIRTUALIO = _gdalconst.DCAP_VIRTUALIO
 DCAP_RASTER = _gdalconst.DCAP_RASTER
 DCAP_VECTOR = _gdalconst.DCAP_VECTOR
 DCAP_GNM = _gdalconst.DCAP_GNM
+DCAP_CREATE_LAYER = _gdalconst.DCAP_CREATE_LAYER
+DCAP_DELETE_LAYER = _gdalconst.DCAP_DELETE_LAYER
+DCAP_CREATE_FIELD = _gdalconst.DCAP_CREATE_FIELD
+DCAP_DELETE_FIELD = _gdalconst.DCAP_DELETE_FIELD
+DCAP_REORDER_FIELDS = _gdalconst.DCAP_REORDER_FIELDS
+DMD_ALTER_FIELD_DEFN_FLAGS = _gdalconst.DMD_ALTER_FIELD_DEFN_FLAGS
 DCAP_NOTNULL_FIELDS = _gdalconst.DCAP_NOTNULL_FIELDS
 DCAP_UNIQUE_FIELDS = _gdalconst.DCAP_UNIQUE_FIELDS
 DCAP_DEFAULT_FIELDS = _gdalconst.DCAP_DEFAULT_FIELDS
 DCAP_NOTNULL_GEOMFIELDS = _gdalconst.DCAP_NOTNULL_GEOMFIELDS
 DCAP_NONSPATIAL = _gdalconst.DCAP_NONSPATIAL
+DCAP_CURVE_GEOMETRIES = _gdalconst.DCAP_CURVE_GEOMETRIES
+DCAP_MEASURED_GEOMETRIES = _gdalconst.DCAP_MEASURED_GEOMETRIES
+DCAP_Z_GEOMETRIES = _gdalconst.DCAP_Z_GEOMETRIES
+DMD_GEOMETRY_FLAGS = _gdalconst.DMD_GEOMETRY_FLAGS
 DCAP_FEATURE_STYLES = _gdalconst.DCAP_FEATURE_STYLES
 DCAP_COORDINATE_EPOCH = _gdalconst.DCAP_COORDINATE_EPOCH
 DCAP_MULTIPLE_VECTOR_LAYERS = _gdalconst.DCAP_MULTIPLE_VECTOR_LAYERS
 DCAP_FIELD_DOMAINS = _gdalconst.DCAP_FIELD_DOMAINS
+DCAP_RELATIONSHIPS = _gdalconst.DCAP_RELATIONSHIPS
+GDAL_DCAP_CREATE_RELATIONSHIP = _gdalconst.GDAL_DCAP_CREATE_RELATIONSHIP
+GDAL_DCAP_DELETE_RELATIONSHIP = _gdalconst.GDAL_DCAP_DELETE_RELATIONSHIP
+GDAL_DCAP_UPDATE_RELATIONSHIP = _gdalconst.GDAL_DCAP_UPDATE_RELATIONSHIP
+GDAL_DMD_RELATIONSHIP_FLAGS = _gdalconst.GDAL_DMD_RELATIONSHIP_FLAGS
 DCAP_RENAME_LAYERS = _gdalconst.DCAP_RENAME_LAYERS
 DIM_TYPE_HORIZONTAL_X = _gdalconst.DIM_TYPE_HORIZONTAL_X
 DIM_TYPE_HORIZONTAL_Y = _gdalconst.DIM_TYPE_HORIZONTAL_Y
 DIM_TYPE_VERTICAL = _gdalconst.DIM_TYPE_VERTICAL
 DIM_TYPE_TEMPORAL = _gdalconst.DIM_TYPE_TEMPORAL
 DIM_TYPE_PARAMETRIC = _gdalconst.DIM_TYPE_PARAMETRIC
+GDsCAddRelationship = _gdalconst.GDsCAddRelationship
+GDsCDeleteRelationship = _gdalconst.GDsCDeleteRelationship
+GDsCUpdateRelationship = _gdalconst.GDsCUpdateRelationship
 CPLES_BackslashQuotable = _gdalconst.CPLES_BackslashQuotable
 CPLES_XML = _gdalconst.CPLES_XML
 CPLES_XML_BUT_QUOTES = _gdalconst.CPLES_XML_BUT_QUOTES
 CPLES_URL = _gdalconst.CPLES_URL
 CPLES_SQL = _gdalconst.CPLES_SQL
 CPLES_SQLI = _gdalconst.CPLES_SQLI
 CPLES_CSV = _gdalconst.CPLES_CSV
@@ -245,9 +266,16 @@
 GARIO_PENDING = _gdalconst.GARIO_PENDING
 GARIO_UPDATE = _gdalconst.GARIO_UPDATE
 GARIO_ERROR = _gdalconst.GARIO_ERROR
 GARIO_COMPLETE = _gdalconst.GARIO_COMPLETE
 GTO_TIP = _gdalconst.GTO_TIP
 GTO_BIT = _gdalconst.GTO_BIT
 GTO_BSQ = _gdalconst.GTO_BSQ
+GRC_ONE_TO_ONE = _gdalconst.GRC_ONE_TO_ONE
+GRC_ONE_TO_MANY = _gdalconst.GRC_ONE_TO_MANY
+GRC_MANY_TO_ONE = _gdalconst.GRC_MANY_TO_ONE
+GRC_MANY_TO_MANY = _gdalconst.GRC_MANY_TO_MANY
+GRT_COMPOSITE = _gdalconst.GRT_COMPOSITE
+GRT_ASSOCIATION = _gdalconst.GRT_ASSOCIATION
+GRT_AGGREGATION = _gdalconst.GRT_AGGREGATION
```

### Comparing `pygdal-3.5.3.11/osgeo/gnm.py` & `pygdal-3.6.4.11/osgeo/gnm.py`

 * *Files 14% similar despite different names*

```diff
@@ -58,23 +58,23 @@
 
 class _SwigNonDynamicMeta(type):
     """Meta class to enforce nondynamic attributes (no new attributes) for a class"""
     __setattr__ = _swig_setattr_nondynamic_class_variable(type.__setattr__)
 
 
 
-def GetUseExceptions(*args):
+def GetUseExceptions(*args) -> "int":
     r"""GetUseExceptions() -> int"""
     return _gnm.GetUseExceptions(*args)
 
-def UseExceptions(*args):
+def UseExceptions(*args) -> "void":
     r"""UseExceptions()"""
     return _gnm.UseExceptions(*args)
 
-def DontUseExceptions(*args):
+def DontUseExceptions(*args) -> "void":
     r"""DontUseExceptions()"""
     return _gnm.DontUseExceptions(*args)
 from . import ogr
 from . import osr
 GATDijkstraShortestPath = _gnm.GATDijkstraShortestPath
 
 GATKShortestPath = _gnm.GATKShortestPath
@@ -84,104 +84,104 @@
 GNM_EDGE_DIR_BOTH = _gnm.GNM_EDGE_DIR_BOTH
 
 GNM_EDGE_DIR_SRCTOTGT = _gnm.GNM_EDGE_DIR_SRCTOTGT
 
 GNM_EDGE_DIR_TGTTOSRC = _gnm.GNM_EDGE_DIR_TGTTOSRC
 
 
-def CastToNetwork(*args):
+def CastToNetwork(*args) -> "GNMNetworkShadow *":
     r"""CastToNetwork(MajorObject base) -> Network"""
     return _gnm.CastToNetwork(*args)
 
-def CastToGenericNetwork(*args):
+def CastToGenericNetwork(*args) -> "GNMGenericNetworkShadow *":
     r"""CastToGenericNetwork(MajorObject base) -> GenericNetwork"""
     return _gnm.CastToGenericNetwork(*args)
 class Network(ogr.MajorObject):
     r"""Proxy of C++ GNMNetworkShadow class."""
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
 
     def __init__(self, *args, **kwargs):
         raise AttributeError("No constructor defined")
     __repr__ = _swig_repr
     __swig_destroy__ = _gnm.delete_Network
 
-    def ReleaseResultSet(self, *args):
+    def ReleaseResultSet(self, *args) -> "void":
         r"""ReleaseResultSet(Network self, Layer layer)"""
         return _gnm.Network_ReleaseResultSet(self, *args)
 
-    def GetVersion(self, *args):
+    def GetVersion(self, *args) -> "int":
         r"""GetVersion(Network self) -> int"""
         return _gnm.Network_GetVersion(self, *args)
 
-    def GetName(self, *args):
+    def GetName(self, *args) -> "char const *":
         r"""GetName(Network self) -> char const *"""
         return _gnm.Network_GetName(self, *args)
 
-    def GetFeatureByGlobalFID(self, *args):
+    def GetFeatureByGlobalFID(self, *args) -> "OGRFeatureShadow *":
         r"""GetFeatureByGlobalFID(Network self, GIntBig GFID) -> Feature"""
         return _gnm.Network_GetFeatureByGlobalFID(self, *args)
 
-    def GetPath(self, *args, **kwargs):
+    def GetPath(self, *args, **kwargs) -> "OGRLayerShadow *":
         r"""GetPath(Network self, GIntBig nStartFID, GIntBig nEndFID, GNMGraphAlgorithmType eAlgorithm, char ** options=None) -> Layer"""
         return _gnm.Network_GetPath(self, *args, **kwargs)
 
-    def DisconnectAll(self, *args):
+    def DisconnectAll(self, *args) -> "CPLErr":
         r"""DisconnectAll(Network self) -> CPLErr"""
         return _gnm.Network_DisconnectAll(self, *args)
 
-    def GetProjection(self, *args):
+    def GetProjection(self, *args) -> "char const *":
         r"""GetProjection(Network self) -> char const *"""
         return _gnm.Network_GetProjection(self, *args)
 
-    def GetProjectionRef(self, *args):
+    def GetProjectionRef(self, *args) -> "char const *":
         r"""GetProjectionRef(Network self) -> char const *"""
         return _gnm.Network_GetProjectionRef(self, *args)
 
-    def GetFileList(self, *args):
+    def GetFileList(self, *args) -> "char **":
         r"""GetFileList(Network self) -> char **"""
         return _gnm.Network_GetFileList(self, *args)
 
-    def CreateLayer(self, *args, **kwargs):
+    def CreateLayer(self, *args, **kwargs) -> "OGRLayerShadow *":
         r"""CreateLayer(Network self, char const * name, SpatialReference srs=None, OGRwkbGeometryType geom_type=wkbUnknown, char ** options=None) -> Layer"""
         return _gnm.Network_CreateLayer(self, *args, **kwargs)
 
-    def CopyLayer(self, *args, **kwargs):
+    def CopyLayer(self, *args, **kwargs) -> "OGRLayerShadow *":
         r"""CopyLayer(Network self, Layer src_layer, char const * new_name, char ** options=None) -> Layer"""
         return _gnm.Network_CopyLayer(self, *args, **kwargs)
 
-    def DeleteLayer(self, *args):
+    def DeleteLayer(self, *args) -> "OGRErr":
         r"""DeleteLayer(Network self, int index) -> OGRErr"""
         return _gnm.Network_DeleteLayer(self, *args)
 
-    def GetLayerCount(self, *args):
+    def GetLayerCount(self, *args) -> "int":
         r"""GetLayerCount(Network self) -> int"""
         return _gnm.Network_GetLayerCount(self, *args)
 
-    def GetLayerByIndex(self, *args):
+    def GetLayerByIndex(self, *args) -> "OGRLayerShadow *":
         r"""GetLayerByIndex(Network self, int index=0) -> Layer"""
         return _gnm.Network_GetLayerByIndex(self, *args)
 
-    def GetLayerByName(self, *args):
+    def GetLayerByName(self, *args) -> "OGRLayerShadow *":
         r"""GetLayerByName(Network self, char const * layer_name) -> Layer"""
         return _gnm.Network_GetLayerByName(self, *args)
 
-    def TestCapability(self, *args):
+    def TestCapability(self, *args) -> "bool":
         r"""TestCapability(Network self, char const * cap) -> bool"""
         return _gnm.Network_TestCapability(self, *args)
 
-    def StartTransaction(self, *args, **kwargs):
+    def StartTransaction(self, *args, **kwargs) -> "OGRErr":
         r"""StartTransaction(Network self, int force=FALSE) -> OGRErr"""
         return _gnm.Network_StartTransaction(self, *args, **kwargs)
 
-    def CommitTransaction(self, *args):
+    def CommitTransaction(self, *args) -> "OGRErr":
         r"""CommitTransaction(Network self) -> OGRErr"""
         return _gnm.Network_CommitTransaction(self, *args)
 
-    def RollbackTransaction(self, *args):
+    def RollbackTransaction(self, *args) -> "OGRErr":
         r"""RollbackTransaction(Network self) -> OGRErr"""
         return _gnm.Network_RollbackTransaction(self, *args)
 
 # Register Network in _gnm:
 _gnm.Network_swigregister(Network)
 
 class GenericNetwork(Network):
@@ -190,55 +190,55 @@
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
 
     def __init__(self, *args, **kwargs):
         raise AttributeError("No constructor defined")
     __repr__ = _swig_repr
     __swig_destroy__ = _gnm.delete_GenericNetwork
 
-    def ConnectFeatures(self, *args):
+    def ConnectFeatures(self, *args) -> "CPLErr":
         r"""ConnectFeatures(GenericNetwork self, GIntBig nSrcFID, GIntBig nTgtFID, GIntBig nConFID, double dfCost, double dfInvCost, GNMDirection eDir) -> CPLErr"""
         return _gnm.GenericNetwork_ConnectFeatures(self, *args)
 
-    def DisconnectFeatures(self, *args):
+    def DisconnectFeatures(self, *args) -> "CPLErr":
         r"""DisconnectFeatures(GenericNetwork self, GIntBig nSrcFID, GIntBig nTgtFID, GIntBig nConFID) -> CPLErr"""
         return _gnm.GenericNetwork_DisconnectFeatures(self, *args)
 
-    def DisconnectFeaturesWithId(self, *args):
+    def DisconnectFeaturesWithId(self, *args) -> "CPLErr":
         r"""DisconnectFeaturesWithId(GenericNetwork self, GIntBig nFID) -> CPLErr"""
         return _gnm.GenericNetwork_DisconnectFeaturesWithId(self, *args)
 
-    def ReconnectFeatures(self, *args):
+    def ReconnectFeatures(self, *args) -> "CPLErr":
         r"""ReconnectFeatures(GenericNetwork self, GIntBig nSrcFID, GIntBig nTgtFID, GIntBig nConFID, double dfCost, double dfInvCost, GNMDirection eDir) -> CPLErr"""
         return _gnm.GenericNetwork_ReconnectFeatures(self, *args)
 
-    def CreateRule(self, *args):
+    def CreateRule(self, *args) -> "CPLErr":
         r"""CreateRule(GenericNetwork self, char const * pszRuleStr) -> CPLErr"""
         return _gnm.GenericNetwork_CreateRule(self, *args)
 
-    def DeleteAllRules(self, *args):
+    def DeleteAllRules(self, *args) -> "CPLErr":
         r"""DeleteAllRules(GenericNetwork self) -> CPLErr"""
         return _gnm.GenericNetwork_DeleteAllRules(self, *args)
 
-    def DeleteRule(self, *args):
+    def DeleteRule(self, *args) -> "CPLErr":
         r"""DeleteRule(GenericNetwork self, char const * pszRuleStr) -> CPLErr"""
         return _gnm.GenericNetwork_DeleteRule(self, *args)
 
-    def GetRules(self, *args):
+    def GetRules(self, *args) -> "char **":
         r"""GetRules(GenericNetwork self) -> char **"""
         return _gnm.GenericNetwork_GetRules(self, *args)
 
-    def ConnectPointsByLines(self, *args, **kwargs):
+    def ConnectPointsByLines(self, *args, **kwargs) -> "CPLErr":
         r"""ConnectPointsByLines(GenericNetwork self, char ** papszLayerList, double dfTolerance, double dfCost, double dfInvCost, GNMDirection eDir) -> CPLErr"""
         return _gnm.GenericNetwork_ConnectPointsByLines(self, *args, **kwargs)
 
-    def ChangeBlockState(self, *args):
+    def ChangeBlockState(self, *args) -> "CPLErr":
         r"""ChangeBlockState(GenericNetwork self, GIntBig nFID, bool bIsBlock) -> CPLErr"""
         return _gnm.GenericNetwork_ChangeBlockState(self, *args)
 
-    def ChangeAllBlockState(self, *args):
+    def ChangeAllBlockState(self, *args) -> "CPLErr":
         r"""ChangeAllBlockState(GenericNetwork self, bool bIsBlock=False) -> CPLErr"""
         return _gnm.GenericNetwork_ChangeAllBlockState(self, *args)
 
 # Register GenericNetwork in _gnm:
 _gnm.GenericNetwork_swigregister(GenericNetwork)
```

### Comparing `pygdal-3.5.3.11/osgeo/osr.py` & `pygdal-3.6.4.11/osgeo/osr.py`

 * *Files 7% similar despite different names*

```diff
@@ -250,31 +250,31 @@
 PROJ_ERR_COORD_TRANSFM_OUTSIDE_GRID = _osr.PROJ_ERR_COORD_TRANSFM_OUTSIDE_GRID
 PROJ_ERR_COORD_TRANSFM_GRID_AT_NODATA = _osr.PROJ_ERR_COORD_TRANSFM_GRID_AT_NODATA
 PROJ_ERR_OTHER = _osr.PROJ_ERR_OTHER
 PROJ_ERR_OTHER_API_MISUSE = _osr.PROJ_ERR_OTHER_API_MISUSE
 PROJ_ERR_OTHER_NO_INVERSE_OP = _osr.PROJ_ERR_OTHER_NO_INVERSE_OP
 PROJ_ERR_OTHER_NETWORK_ERROR = _osr.PROJ_ERR_OTHER_NETWORK_ERROR
 
-def GetUseExceptions(*args):
+def GetUseExceptions(*args) -> "int":
     r"""GetUseExceptions() -> int"""
     return _osr.GetUseExceptions(*args)
 
-def UseExceptions(*args):
+def UseExceptions(*args) -> "void":
     r"""UseExceptions()"""
     return _osr.UseExceptions(*args)
 
-def DontUseExceptions(*args):
+def DontUseExceptions(*args) -> "void":
     r"""DontUseExceptions()"""
     return _osr.DontUseExceptions(*args)
 
-def GetWellKnownGeogCSAsWKT(*args):
+def GetWellKnownGeogCSAsWKT(*args) -> "char **":
     r"""GetWellKnownGeogCSAsWKT(char const * name) -> OGRErr"""
     return _osr.GetWellKnownGeogCSAsWKT(*args)
 
-def GetUserInputAsWKT(*args):
+def GetUserInputAsWKT(*args) -> "char **":
     r"""GetUserInputAsWKT(char const * name) -> OGRErr"""
     return _osr.GetUserInputAsWKT(*args)
 class AreaOfUse(object):
     r"""Proxy of C++ OSRAreaOfUse class."""
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
@@ -289,581 +289,585 @@
         _osr.AreaOfUse_swiginit(self, _osr.new_AreaOfUse(*args))
     __swig_destroy__ = _osr.delete_AreaOfUse
 
 # Register AreaOfUse in _osr:
 _osr.AreaOfUse_swigregister(AreaOfUse)
 
 
-def OSRAreaOfUse_west_lon_degree_get(*args):
+def OSRAreaOfUse_west_lon_degree_get(*args) -> "double":
     r"""OSRAreaOfUse_west_lon_degree_get(AreaOfUse area) -> double"""
     return _osr.OSRAreaOfUse_west_lon_degree_get(*args)
 
-def OSRAreaOfUse_south_lat_degree_get(*args):
+def OSRAreaOfUse_south_lat_degree_get(*args) -> "double":
     r"""OSRAreaOfUse_south_lat_degree_get(AreaOfUse area) -> double"""
     return _osr.OSRAreaOfUse_south_lat_degree_get(*args)
 
-def OSRAreaOfUse_east_lon_degree_get(*args):
+def OSRAreaOfUse_east_lon_degree_get(*args) -> "double":
     r"""OSRAreaOfUse_east_lon_degree_get(AreaOfUse area) -> double"""
     return _osr.OSRAreaOfUse_east_lon_degree_get(*args)
 
-def OSRAreaOfUse_north_lat_degree_get(*args):
+def OSRAreaOfUse_north_lat_degree_get(*args) -> "double":
     r"""OSRAreaOfUse_north_lat_degree_get(AreaOfUse area) -> double"""
     return _osr.OSRAreaOfUse_north_lat_degree_get(*args)
 
-def OSRAreaOfUse_name_get(*args):
+def OSRAreaOfUse_name_get(*args) -> "char const *":
     r"""OSRAreaOfUse_name_get(AreaOfUse area) -> char const *"""
     return _osr.OSRAreaOfUse_name_get(*args)
 class SpatialReference(object):
     r"""Proxy of C++ OSRSpatialReferenceShadow class."""
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
 
     def __init__(self, *args, **kwargs):
         r"""__init__(SpatialReference self, char const * wkt="") -> SpatialReference"""
         _osr.SpatialReference_swiginit(self, _osr.new_SpatialReference(*args, **kwargs))
     __swig_destroy__ = _osr.delete_SpatialReference
 
-    def __str__(self, *args):
+    def __str__(self, *args) -> "retStringAndCPLFree *":
         r"""__str__(SpatialReference self) -> retStringAndCPLFree *"""
         return _osr.SpatialReference___str__(self, *args)
 
-    def GetName(self, *args):
+    def GetName(self, *args) -> "char const *":
         r"""GetName(SpatialReference self) -> char const *"""
         return _osr.SpatialReference_GetName(self, *args)
 
-    def IsSame(self, *args, **kwargs):
+    def IsSame(self, *args, **kwargs) -> "int":
         r"""IsSame(SpatialReference self, SpatialReference rhs, char ** options=None) -> int"""
         return _osr.SpatialReference_IsSame(self, *args, **kwargs)
 
-    def IsSameGeogCS(self, *args):
+    def IsSameGeogCS(self, *args) -> "int":
         r"""IsSameGeogCS(SpatialReference self, SpatialReference rhs) -> int"""
         return _osr.SpatialReference_IsSameGeogCS(self, *args)
 
-    def IsSameVertCS(self, *args):
+    def IsSameVertCS(self, *args) -> "int":
         r"""IsSameVertCS(SpatialReference self, SpatialReference rhs) -> int"""
         return _osr.SpatialReference_IsSameVertCS(self, *args)
 
-    def IsGeographic(self, *args):
+    def IsGeographic(self, *args) -> "int":
         r"""IsGeographic(SpatialReference self) -> int"""
         return _osr.SpatialReference_IsGeographic(self, *args)
 
-    def IsDerivedGeographic(self, *args):
+    def IsDerivedGeographic(self, *args) -> "int":
         r"""IsDerivedGeographic(SpatialReference self) -> int"""
         return _osr.SpatialReference_IsDerivedGeographic(self, *args)
 
-    def IsProjected(self, *args):
+    def IsProjected(self, *args) -> "int":
         r"""IsProjected(SpatialReference self) -> int"""
         return _osr.SpatialReference_IsProjected(self, *args)
 
-    def IsCompound(self, *args):
+    def IsCompound(self, *args) -> "int":
         r"""IsCompound(SpatialReference self) -> int"""
         return _osr.SpatialReference_IsCompound(self, *args)
 
-    def IsGeocentric(self, *args):
+    def IsGeocentric(self, *args) -> "int":
         r"""IsGeocentric(SpatialReference self) -> int"""
         return _osr.SpatialReference_IsGeocentric(self, *args)
 
-    def IsLocal(self, *args):
+    def IsLocal(self, *args) -> "int":
         r"""IsLocal(SpatialReference self) -> int"""
         return _osr.SpatialReference_IsLocal(self, *args)
 
-    def IsVertical(self, *args):
+    def IsVertical(self, *args) -> "int":
         r"""IsVertical(SpatialReference self) -> int"""
         return _osr.SpatialReference_IsVertical(self, *args)
 
-    def IsDynamic(self, *args):
+    def IsDynamic(self, *args) -> "bool":
         r"""IsDynamic(SpatialReference self) -> bool"""
         return _osr.SpatialReference_IsDynamic(self, *args)
 
-    def GetCoordinateEpoch(self, *args):
+    def GetCoordinateEpoch(self, *args) -> "double":
         r"""GetCoordinateEpoch(SpatialReference self) -> double"""
         return _osr.SpatialReference_GetCoordinateEpoch(self, *args)
 
-    def SetCoordinateEpoch(self, *args):
+    def SetCoordinateEpoch(self, *args) -> "void":
         r"""SetCoordinateEpoch(SpatialReference self, double coordinateEpoch)"""
         return _osr.SpatialReference_SetCoordinateEpoch(self, *args)
 
-    def EPSGTreatsAsLatLong(self, *args):
+    def EPSGTreatsAsLatLong(self, *args) -> "int":
         r"""EPSGTreatsAsLatLong(SpatialReference self) -> int"""
         return _osr.SpatialReference_EPSGTreatsAsLatLong(self, *args)
 
-    def EPSGTreatsAsNorthingEasting(self, *args):
+    def EPSGTreatsAsNorthingEasting(self, *args) -> "int":
         r"""EPSGTreatsAsNorthingEasting(SpatialReference self) -> int"""
         return _osr.SpatialReference_EPSGTreatsAsNorthingEasting(self, *args)
 
-    def SetAuthority(self, *args):
+    def SetAuthority(self, *args) -> "OGRErr":
         r"""SetAuthority(SpatialReference self, char const * pszTargetKey, char const * pszAuthority, int nCode) -> OGRErr"""
         return _osr.SpatialReference_SetAuthority(self, *args)
 
-    def GetAttrValue(self, *args):
+    def GetAttrValue(self, *args) -> "char const *":
         r"""GetAttrValue(SpatialReference self, char const * name, int child=0) -> char const *"""
         return _osr.SpatialReference_GetAttrValue(self, *args)
 
-    def SetAttrValue(self, *args):
+    def SetAttrValue(self, *args) -> "OGRErr":
         r"""SetAttrValue(SpatialReference self, char const * name, char const * value) -> OGRErr"""
         return _osr.SpatialReference_SetAttrValue(self, *args)
 
-    def SetAngularUnits(self, *args):
+    def SetAngularUnits(self, *args) -> "OGRErr":
         r"""SetAngularUnits(SpatialReference self, char const * name, double to_radians) -> OGRErr"""
         return _osr.SpatialReference_SetAngularUnits(self, *args)
 
-    def GetAngularUnits(self, *args):
+    def GetAngularUnits(self, *args) -> "double":
         r"""GetAngularUnits(SpatialReference self) -> double"""
         return _osr.SpatialReference_GetAngularUnits(self, *args)
 
-    def GetAngularUnitsName(self, *args):
+    def GetAngularUnitsName(self, *args) -> "char const *":
         r"""GetAngularUnitsName(SpatialReference self) -> char const *"""
         return _osr.SpatialReference_GetAngularUnitsName(self, *args)
 
-    def SetTargetLinearUnits(self, *args):
+    def SetTargetLinearUnits(self, *args) -> "OGRErr":
         r"""SetTargetLinearUnits(SpatialReference self, char const * target, char const * name, double to_meters) -> OGRErr"""
         return _osr.SpatialReference_SetTargetLinearUnits(self, *args)
 
-    def SetLinearUnits(self, *args):
+    def SetLinearUnits(self, *args) -> "OGRErr":
         r"""SetLinearUnits(SpatialReference self, char const * name, double to_meters) -> OGRErr"""
         return _osr.SpatialReference_SetLinearUnits(self, *args)
 
-    def SetLinearUnitsAndUpdateParameters(self, *args):
+    def SetLinearUnitsAndUpdateParameters(self, *args) -> "OGRErr":
         r"""SetLinearUnitsAndUpdateParameters(SpatialReference self, char const * name, double to_meters) -> OGRErr"""
         return _osr.SpatialReference_SetLinearUnitsAndUpdateParameters(self, *args)
 
-    def GetTargetLinearUnits(self, *args):
+    def GetTargetLinearUnits(self, *args) -> "double":
         r"""GetTargetLinearUnits(SpatialReference self, char const * target_key) -> double"""
         return _osr.SpatialReference_GetTargetLinearUnits(self, *args)
 
-    def GetLinearUnits(self, *args):
+    def GetLinearUnits(self, *args) -> "double":
         r"""GetLinearUnits(SpatialReference self) -> double"""
         return _osr.SpatialReference_GetLinearUnits(self, *args)
 
-    def GetLinearUnitsName(self, *args):
+    def GetLinearUnitsName(self, *args) -> "char const *":
         r"""GetLinearUnitsName(SpatialReference self) -> char const *"""
         return _osr.SpatialReference_GetLinearUnitsName(self, *args)
 
-    def GetAuthorityCode(self, *args):
+    def GetAuthorityCode(self, *args) -> "char const *":
         r"""GetAuthorityCode(SpatialReference self, char const * target_key) -> char const *"""
         return _osr.SpatialReference_GetAuthorityCode(self, *args)
 
-    def GetAuthorityName(self, *args):
+    def GetAuthorityName(self, *args) -> "char const *":
         r"""GetAuthorityName(SpatialReference self, char const * target_key) -> char const *"""
         return _osr.SpatialReference_GetAuthorityName(self, *args)
 
-    def GetAreaOfUse(self, *args):
+    def GetAreaOfUse(self, *args) -> "OSRAreaOfUse *":
         r"""GetAreaOfUse(SpatialReference self) -> AreaOfUse"""
         return _osr.SpatialReference_GetAreaOfUse(self, *args)
 
-    def GetAxisName(self, *args):
+    def GetAxisName(self, *args) -> "char const *":
         r"""GetAxisName(SpatialReference self, char const * target_key, int iAxis) -> char const *"""
         return _osr.SpatialReference_GetAxisName(self, *args)
 
-    def GetAxesCount(self, *args):
+    def GetAxesCount(self, *args) -> "int":
         r"""GetAxesCount(SpatialReference self) -> int"""
         return _osr.SpatialReference_GetAxesCount(self, *args)
 
-    def GetAxisOrientation(self, *args):
+    def GetAxisOrientation(self, *args) -> "OGRAxisOrientation":
         r"""GetAxisOrientation(SpatialReference self, char const * target_key, int iAxis) -> OGRAxisOrientation"""
         return _osr.SpatialReference_GetAxisOrientation(self, *args)
 
-    def GetAxisMappingStrategy(self, *args):
+    def GetAxisMappingStrategy(self, *args) -> "OSRAxisMappingStrategy":
         r"""GetAxisMappingStrategy(SpatialReference self) -> OSRAxisMappingStrategy"""
         return _osr.SpatialReference_GetAxisMappingStrategy(self, *args)
 
-    def SetAxisMappingStrategy(self, *args):
+    def SetAxisMappingStrategy(self, *args) -> "void":
         r"""SetAxisMappingStrategy(SpatialReference self, OSRAxisMappingStrategy strategy)"""
         return _osr.SpatialReference_SetAxisMappingStrategy(self, *args)
 
-    def GetDataAxisToSRSAxisMapping(self, *args):
+    def GetDataAxisToSRSAxisMapping(self, *args) -> "void":
         r"""GetDataAxisToSRSAxisMapping(SpatialReference self)"""
         return _osr.SpatialReference_GetDataAxisToSRSAxisMapping(self, *args)
 
-    def SetDataAxisToSRSAxisMapping(self, *args):
+    def SetDataAxisToSRSAxisMapping(self, *args) -> "OGRErr":
         r"""SetDataAxisToSRSAxisMapping(SpatialReference self, int nList) -> OGRErr"""
         return _osr.SpatialReference_SetDataAxisToSRSAxisMapping(self, *args)
 
-    def SetUTM(self, *args):
+    def SetUTM(self, *args) -> "OGRErr":
         r"""SetUTM(SpatialReference self, int zone, int north=1) -> OGRErr"""
         return _osr.SpatialReference_SetUTM(self, *args)
 
-    def GetUTMZone(self, *args):
+    def GetUTMZone(self, *args) -> "int":
         r"""GetUTMZone(SpatialReference self) -> int"""
         return _osr.SpatialReference_GetUTMZone(self, *args)
 
-    def SetStatePlane(self, *args):
+    def SetStatePlane(self, *args) -> "OGRErr":
         r"""SetStatePlane(SpatialReference self, int zone, int is_nad83=1, char const * unitsname="", double units=0.0) -> OGRErr"""
         return _osr.SpatialReference_SetStatePlane(self, *args)
 
-    def AutoIdentifyEPSG(self, *args):
+    def AutoIdentifyEPSG(self, *args) -> "OGRErr":
         r"""AutoIdentifyEPSG(SpatialReference self) -> OGRErr"""
         return _osr.SpatialReference_AutoIdentifyEPSG(self, *args)
 
-    def FindMatches(self, *args):
+    def FindMatches(self, *args) -> "void":
         r"""FindMatches(SpatialReference self, char ** options=None)"""
         return _osr.SpatialReference_FindMatches(self, *args)
 
-    def SetProjection(self, *args):
+    def SetProjection(self, *args) -> "OGRErr":
         r"""SetProjection(SpatialReference self, char const * arg) -> OGRErr"""
         return _osr.SpatialReference_SetProjection(self, *args)
 
-    def SetProjParm(self, *args):
+    def SetProjParm(self, *args) -> "OGRErr":
         r"""SetProjParm(SpatialReference self, char const * name, double val) -> OGRErr"""
         return _osr.SpatialReference_SetProjParm(self, *args)
 
-    def GetProjParm(self, *args):
+    def GetProjParm(self, *args) -> "double":
         r"""GetProjParm(SpatialReference self, char const * name, double default_val=0.0) -> double"""
         return _osr.SpatialReference_GetProjParm(self, *args)
 
-    def SetNormProjParm(self, *args):
+    def SetNormProjParm(self, *args) -> "OGRErr":
         r"""SetNormProjParm(SpatialReference self, char const * name, double val) -> OGRErr"""
         return _osr.SpatialReference_SetNormProjParm(self, *args)
 
-    def GetNormProjParm(self, *args):
+    def GetNormProjParm(self, *args) -> "double":
         r"""GetNormProjParm(SpatialReference self, char const * name, double default_val=0.0) -> double"""
         return _osr.SpatialReference_GetNormProjParm(self, *args)
 
-    def GetSemiMajor(self, *args):
+    def GetSemiMajor(self, *args) -> "double":
         r"""GetSemiMajor(SpatialReference self) -> double"""
         return _osr.SpatialReference_GetSemiMajor(self, *args)
 
-    def GetSemiMinor(self, *args):
+    def GetSemiMinor(self, *args) -> "double":
         r"""GetSemiMinor(SpatialReference self) -> double"""
         return _osr.SpatialReference_GetSemiMinor(self, *args)
 
-    def GetInvFlattening(self, *args):
+    def GetInvFlattening(self, *args) -> "double":
         r"""GetInvFlattening(SpatialReference self) -> double"""
         return _osr.SpatialReference_GetInvFlattening(self, *args)
 
-    def SetACEA(self, *args, **kwargs):
+    def SetACEA(self, *args, **kwargs) -> "OGRErr":
         r"""SetACEA(SpatialReference self, double stdp1, double stdp2, double clat, double clong, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetACEA(self, *args, **kwargs)
 
-    def SetAE(self, *args, **kwargs):
+    def SetAE(self, *args, **kwargs) -> "OGRErr":
         r"""SetAE(SpatialReference self, double clat, double clong, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetAE(self, *args, **kwargs)
 
-    def SetBonne(self, *args, **kwargs):
+    def SetBonne(self, *args, **kwargs) -> "OGRErr":
         r"""SetBonne(SpatialReference self, double stdp, double cm, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetBonne(self, *args, **kwargs)
 
-    def SetCEA(self, *args, **kwargs):
+    def SetCEA(self, *args, **kwargs) -> "OGRErr":
         r"""SetCEA(SpatialReference self, double stdp1, double cm, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetCEA(self, *args, **kwargs)
 
-    def SetCS(self, *args, **kwargs):
+    def SetCS(self, *args, **kwargs) -> "OGRErr":
         r"""SetCS(SpatialReference self, double clat, double clong, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetCS(self, *args, **kwargs)
 
-    def SetEC(self, *args, **kwargs):
+    def SetEC(self, *args, **kwargs) -> "OGRErr":
         r"""SetEC(SpatialReference self, double stdp1, double stdp2, double clat, double clong, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetEC(self, *args, **kwargs)
 
-    def SetEckertIV(self, *args, **kwargs):
+    def SetEckertIV(self, *args, **kwargs) -> "OGRErr":
         r"""SetEckertIV(SpatialReference self, double cm, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetEckertIV(self, *args, **kwargs)
 
-    def SetEckertVI(self, *args, **kwargs):
+    def SetEckertVI(self, *args, **kwargs) -> "OGRErr":
         r"""SetEckertVI(SpatialReference self, double cm, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetEckertVI(self, *args, **kwargs)
 
-    def SetEquirectangular(self, *args, **kwargs):
+    def SetEquirectangular(self, *args, **kwargs) -> "OGRErr":
         r"""SetEquirectangular(SpatialReference self, double clat, double clong, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetEquirectangular(self, *args, **kwargs)
 
-    def SetEquirectangular2(self, *args, **kwargs):
+    def SetEquirectangular2(self, *args, **kwargs) -> "OGRErr":
         r"""SetEquirectangular2(SpatialReference self, double clat, double clong, double pseudostdparallellat, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetEquirectangular2(self, *args, **kwargs)
 
-    def SetGaussSchreiberTMercator(self, *args, **kwargs):
+    def SetGaussSchreiberTMercator(self, *args, **kwargs) -> "OGRErr":
         r"""SetGaussSchreiberTMercator(SpatialReference self, double clat, double clong, double sc, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetGaussSchreiberTMercator(self, *args, **kwargs)
 
-    def SetGS(self, *args, **kwargs):
+    def SetGS(self, *args, **kwargs) -> "OGRErr":
         r"""SetGS(SpatialReference self, double cm, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetGS(self, *args, **kwargs)
 
-    def SetGH(self, *args, **kwargs):
+    def SetGH(self, *args, **kwargs) -> "OGRErr":
         r"""SetGH(SpatialReference self, double cm, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetGH(self, *args, **kwargs)
 
-    def SetIGH(self, *args):
+    def SetIGH(self, *args) -> "OGRErr":
         r"""SetIGH(SpatialReference self) -> OGRErr"""
         return _osr.SpatialReference_SetIGH(self, *args)
 
-    def SetGEOS(self, *args, **kwargs):
+    def SetGEOS(self, *args, **kwargs) -> "OGRErr":
         r"""SetGEOS(SpatialReference self, double cm, double satelliteheight, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetGEOS(self, *args, **kwargs)
 
-    def SetGnomonic(self, *args, **kwargs):
+    def SetGnomonic(self, *args, **kwargs) -> "OGRErr":
         r"""SetGnomonic(SpatialReference self, double clat, double clong, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetGnomonic(self, *args, **kwargs)
 
-    def SetHOM(self, *args, **kwargs):
+    def SetHOM(self, *args, **kwargs) -> "OGRErr":
         r"""SetHOM(SpatialReference self, double clat, double clong, double azimuth, double recttoskew, double scale, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetHOM(self, *args, **kwargs)
 
-    def SetHOM2PNO(self, *args, **kwargs):
+    def SetHOM2PNO(self, *args, **kwargs) -> "OGRErr":
         r"""SetHOM2PNO(SpatialReference self, double clat, double dfLat1, double dfLong1, double dfLat2, double dfLong2, double scale, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetHOM2PNO(self, *args, **kwargs)
 
-    def SetKrovak(self, *args, **kwargs):
+    def SetKrovak(self, *args, **kwargs) -> "OGRErr":
         r"""SetKrovak(SpatialReference self, double clat, double clong, double azimuth, double pseudostdparallellat, double scale, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetKrovak(self, *args, **kwargs)
 
-    def SetLAEA(self, *args, **kwargs):
+    def SetLAEA(self, *args, **kwargs) -> "OGRErr":
         r"""SetLAEA(SpatialReference self, double clat, double clong, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetLAEA(self, *args, **kwargs)
 
-    def SetLCC(self, *args, **kwargs):
+    def SetLCC(self, *args, **kwargs) -> "OGRErr":
         r"""SetLCC(SpatialReference self, double stdp1, double stdp2, double clat, double clong, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetLCC(self, *args, **kwargs)
 
-    def SetLCC1SP(self, *args, **kwargs):
+    def SetLCC1SP(self, *args, **kwargs) -> "OGRErr":
         r"""SetLCC1SP(SpatialReference self, double clat, double clong, double scale, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetLCC1SP(self, *args, **kwargs)
 
-    def SetLCCB(self, *args, **kwargs):
+    def SetLCCB(self, *args, **kwargs) -> "OGRErr":
         r"""SetLCCB(SpatialReference self, double stdp1, double stdp2, double clat, double clong, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetLCCB(self, *args, **kwargs)
 
-    def SetMC(self, *args, **kwargs):
+    def SetMC(self, *args, **kwargs) -> "OGRErr":
         r"""SetMC(SpatialReference self, double clat, double clong, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetMC(self, *args, **kwargs)
 
-    def SetMercator(self, *args, **kwargs):
+    def SetMercator(self, *args, **kwargs) -> "OGRErr":
         r"""SetMercator(SpatialReference self, double clat, double clong, double scale, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetMercator(self, *args, **kwargs)
 
-    def SetMercator2SP(self, *args, **kwargs):
+    def SetMercator2SP(self, *args, **kwargs) -> "OGRErr":
         r"""SetMercator2SP(SpatialReference self, double stdp1, double clat, double clong, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetMercator2SP(self, *args, **kwargs)
 
-    def SetMollweide(self, *args, **kwargs):
+    def SetMollweide(self, *args, **kwargs) -> "OGRErr":
         r"""SetMollweide(SpatialReference self, double cm, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetMollweide(self, *args, **kwargs)
 
-    def SetNZMG(self, *args, **kwargs):
+    def SetNZMG(self, *args, **kwargs) -> "OGRErr":
         r"""SetNZMG(SpatialReference self, double clat, double clong, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetNZMG(self, *args, **kwargs)
 
-    def SetOS(self, *args, **kwargs):
+    def SetOS(self, *args, **kwargs) -> "OGRErr":
         r"""SetOS(SpatialReference self, double dfOriginLat, double dfCMeridian, double scale, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetOS(self, *args, **kwargs)
 
-    def SetOrthographic(self, *args, **kwargs):
+    def SetOrthographic(self, *args, **kwargs) -> "OGRErr":
         r"""SetOrthographic(SpatialReference self, double clat, double clong, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetOrthographic(self, *args, **kwargs)
 
-    def SetPolyconic(self, *args, **kwargs):
+    def SetPolyconic(self, *args, **kwargs) -> "OGRErr":
         r"""SetPolyconic(SpatialReference self, double clat, double clong, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetPolyconic(self, *args, **kwargs)
 
-    def SetPS(self, *args, **kwargs):
+    def SetPS(self, *args, **kwargs) -> "OGRErr":
         r"""SetPS(SpatialReference self, double clat, double clong, double scale, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetPS(self, *args, **kwargs)
 
-    def SetRobinson(self, *args, **kwargs):
+    def SetRobinson(self, *args, **kwargs) -> "OGRErr":
         r"""SetRobinson(SpatialReference self, double clong, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetRobinson(self, *args, **kwargs)
 
-    def SetSinusoidal(self, *args, **kwargs):
+    def SetSinusoidal(self, *args, **kwargs) -> "OGRErr":
         r"""SetSinusoidal(SpatialReference self, double clong, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetSinusoidal(self, *args, **kwargs)
 
-    def SetStereographic(self, *args, **kwargs):
+    def SetStereographic(self, *args, **kwargs) -> "OGRErr":
         r"""SetStereographic(SpatialReference self, double clat, double clong, double scale, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetStereographic(self, *args, **kwargs)
 
-    def SetSOC(self, *args, **kwargs):
+    def SetSOC(self, *args, **kwargs) -> "OGRErr":
         r"""SetSOC(SpatialReference self, double latitudeoforigin, double cm, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetSOC(self, *args, **kwargs)
 
-    def SetTM(self, *args, **kwargs):
+    def SetTM(self, *args, **kwargs) -> "OGRErr":
         r"""SetTM(SpatialReference self, double clat, double clong, double scale, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetTM(self, *args, **kwargs)
 
-    def SetTMVariant(self, *args, **kwargs):
+    def SetTMVariant(self, *args, **kwargs) -> "OGRErr":
         r"""SetTMVariant(SpatialReference self, char const * pszVariantName, double clat, double clong, double scale, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetTMVariant(self, *args, **kwargs)
 
-    def SetTMG(self, *args, **kwargs):
+    def SetTMG(self, *args, **kwargs) -> "OGRErr":
         r"""SetTMG(SpatialReference self, double clat, double clong, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetTMG(self, *args, **kwargs)
 
-    def SetTMSO(self, *args, **kwargs):
+    def SetTMSO(self, *args, **kwargs) -> "OGRErr":
         r"""SetTMSO(SpatialReference self, double clat, double clong, double scale, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetTMSO(self, *args, **kwargs)
 
-    def SetVDG(self, *args, **kwargs):
+    def SetVDG(self, *args, **kwargs) -> "OGRErr":
         r"""SetVDG(SpatialReference self, double clong, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetVDG(self, *args, **kwargs)
 
-    def SetVerticalPerspective(self, *args, **kwargs):
+    def SetVerticalPerspective(self, *args, **kwargs) -> "OGRErr":
         r"""SetVerticalPerspective(SpatialReference self, double topoOriginLat, double topoOriginLon, double topoOriginHeight, double viewPointHeight, double fe, double fn) -> OGRErr"""
         return _osr.SpatialReference_SetVerticalPerspective(self, *args, **kwargs)
 
-    def SetWellKnownGeogCS(self, *args):
+    def SetWellKnownGeogCS(self, *args) -> "OGRErr":
         r"""SetWellKnownGeogCS(SpatialReference self, char const * name) -> OGRErr"""
         return _osr.SpatialReference_SetWellKnownGeogCS(self, *args)
 
-    def SetFromUserInput(self, *args):
+    def SetFromUserInput(self, *args) -> "OGRErr":
         r"""SetFromUserInput(SpatialReference self, char const * name) -> OGRErr"""
         return _osr.SpatialReference_SetFromUserInput(self, *args)
 
-    def CopyGeogCSFrom(self, *args):
+    def CopyGeogCSFrom(self, *args) -> "OGRErr":
         r"""CopyGeogCSFrom(SpatialReference self, SpatialReference rhs) -> OGRErr"""
         return _osr.SpatialReference_CopyGeogCSFrom(self, *args)
 
-    def SetTOWGS84(self, *args):
+    def SetTOWGS84(self, *args) -> "OGRErr":
         r"""SetTOWGS84(SpatialReference self, double p1, double p2, double p3, double p4=0.0, double p5=0.0, double p6=0.0, double p7=0.0) -> OGRErr"""
         return _osr.SpatialReference_SetTOWGS84(self, *args)
 
-    def HasTOWGS84(self, *args):
+    def HasTOWGS84(self, *args) -> "bool":
         r"""HasTOWGS84(SpatialReference self) -> bool"""
         return _osr.SpatialReference_HasTOWGS84(self, *args)
 
-    def GetTOWGS84(self, *args):
+    def GetTOWGS84(self, *args) -> "OGRErr":
         r"""GetTOWGS84(SpatialReference self) -> OGRErr"""
         return _osr.SpatialReference_GetTOWGS84(self, *args)
 
-    def AddGuessedTOWGS84(self, *args):
+    def AddGuessedTOWGS84(self, *args) -> "OGRErr":
         r"""AddGuessedTOWGS84(SpatialReference self) -> OGRErr"""
         return _osr.SpatialReference_AddGuessedTOWGS84(self, *args)
 
-    def SetLocalCS(self, *args):
+    def SetLocalCS(self, *args) -> "OGRErr":
         r"""SetLocalCS(SpatialReference self, char const * pszName) -> OGRErr"""
         return _osr.SpatialReference_SetLocalCS(self, *args)
 
-    def SetGeogCS(self, *args):
+    def SetGeogCS(self, *args) -> "OGRErr":
         r"""SetGeogCS(SpatialReference self, char const * pszGeogName, char const * pszDatumName, char const * pszEllipsoidName, double dfSemiMajor, double dfInvFlattening, char const * pszPMName="Greenwich", double dfPMOffset=0.0, char const * pszUnits="degree", double dfConvertToRadians=0.0174532925199433) -> OGRErr"""
         return _osr.SpatialReference_SetGeogCS(self, *args)
 
-    def SetProjCS(self, *args):
+    def SetProjCS(self, *args) -> "OGRErr":
         r"""SetProjCS(SpatialReference self, char const * name="unnamed") -> OGRErr"""
         return _osr.SpatialReference_SetProjCS(self, *args)
 
-    def SetGeocCS(self, *args):
+    def SetGeocCS(self, *args) -> "OGRErr":
         r"""SetGeocCS(SpatialReference self, char const * name="unnamed") -> OGRErr"""
         return _osr.SpatialReference_SetGeocCS(self, *args)
 
-    def SetVertCS(self, *args):
+    def SetVertCS(self, *args) -> "OGRErr":
         r"""SetVertCS(SpatialReference self, char const * VertCSName="unnamed", char const * VertDatumName="unnamed", int VertDatumType=0) -> OGRErr"""
         return _osr.SpatialReference_SetVertCS(self, *args)
 
-    def SetCompoundCS(self, *args):
+    def SetCompoundCS(self, *args) -> "OGRErr":
         r"""SetCompoundCS(SpatialReference self, char const * name, SpatialReference horizcs, SpatialReference vertcs) -> OGRErr"""
         return _osr.SpatialReference_SetCompoundCS(self, *args)
 
-    def ImportFromWkt(self, *args):
+    def ImportFromWkt(self, *args) -> "OGRErr":
         r"""ImportFromWkt(SpatialReference self, char ** ppszInput) -> OGRErr"""
         return _osr.SpatialReference_ImportFromWkt(self, *args)
 
-    def ImportFromProj4(self, *args):
+    def ImportFromProj4(self, *args) -> "OGRErr":
         r"""ImportFromProj4(SpatialReference self, char * ppszInput) -> OGRErr"""
         return _osr.SpatialReference_ImportFromProj4(self, *args)
 
-    def ImportFromUrl(self, *args):
+    def ImportFromUrl(self, *args) -> "OGRErr":
         r"""ImportFromUrl(SpatialReference self, char * url) -> OGRErr"""
         return _osr.SpatialReference_ImportFromUrl(self, *args)
 
-    def ImportFromESRI(self, *args):
+    def ImportFromESRI(self, *args) -> "OGRErr":
         r"""ImportFromESRI(SpatialReference self, char ** ppszInput) -> OGRErr"""
         return _osr.SpatialReference_ImportFromESRI(self, *args)
 
-    def ImportFromEPSG(self, *args):
+    def ImportFromEPSG(self, *args) -> "OGRErr":
         r"""ImportFromEPSG(SpatialReference self, int arg) -> OGRErr"""
         return _osr.SpatialReference_ImportFromEPSG(self, *args)
 
-    def ImportFromEPSGA(self, *args):
+    def ImportFromEPSGA(self, *args) -> "OGRErr":
         r"""ImportFromEPSGA(SpatialReference self, int arg) -> OGRErr"""
         return _osr.SpatialReference_ImportFromEPSGA(self, *args)
 
-    def ImportFromPCI(self, *args):
+    def ImportFromPCI(self, *args) -> "OGRErr":
         r"""ImportFromPCI(SpatialReference self, char const * proj, char const * units="METRE", double [17] argin=0) -> OGRErr"""
         return _osr.SpatialReference_ImportFromPCI(self, *args)
 
-    def ImportFromUSGS(self, *args):
+    def ImportFromUSGS(self, *args) -> "OGRErr":
         r"""ImportFromUSGS(SpatialReference self, long proj_code, long zone=0, double [15] argin=0, long datum_code=0) -> OGRErr"""
         return _osr.SpatialReference_ImportFromUSGS(self, *args)
 
-    def ImportFromXML(self, *args):
+    def ImportFromXML(self, *args) -> "OGRErr":
         r"""ImportFromXML(SpatialReference self, char const * xmlString) -> OGRErr"""
         return _osr.SpatialReference_ImportFromXML(self, *args)
 
-    def ImportFromERM(self, *args):
+    def ImportFromERM(self, *args) -> "OGRErr":
         r"""ImportFromERM(SpatialReference self, char const * proj, char const * datum, char const * units) -> OGRErr"""
         return _osr.SpatialReference_ImportFromERM(self, *args)
 
-    def ImportFromMICoordSys(self, *args):
+    def ImportFromMICoordSys(self, *args) -> "OGRErr":
         r"""ImportFromMICoordSys(SpatialReference self, char const * pszCoordSys) -> OGRErr"""
         return _osr.SpatialReference_ImportFromMICoordSys(self, *args)
 
-    def ImportFromOzi(self, *args):
+    def ImportFromOzi(self, *args) -> "OGRErr":
         r"""ImportFromOzi(SpatialReference self, char const *const * papszLines) -> OGRErr"""
         return _osr.SpatialReference_ImportFromOzi(self, *args)
 
-    def ExportToWkt(self, *args):
+    def ExportToWkt(self, *args) -> "OGRErr":
         r"""ExportToWkt(SpatialReference self, char ** options=None) -> OGRErr"""
         return _osr.SpatialReference_ExportToWkt(self, *args)
 
-    def ExportToPrettyWkt(self, *args):
+    def ExportToPrettyWkt(self, *args) -> "OGRErr":
         r"""ExportToPrettyWkt(SpatialReference self, int simplify=0) -> OGRErr"""
         return _osr.SpatialReference_ExportToPrettyWkt(self, *args)
 
-    def ExportToPROJJSON(self, *args):
+    def ExportToPROJJSON(self, *args) -> "OGRErr":
         r"""ExportToPROJJSON(SpatialReference self, char ** options=None) -> OGRErr"""
         return _osr.SpatialReference_ExportToPROJJSON(self, *args)
 
-    def ExportToProj4(self, *args):
+    def ExportToProj4(self, *args) -> "OGRErr":
         r"""ExportToProj4(SpatialReference self) -> OGRErr"""
         return _osr.SpatialReference_ExportToProj4(self, *args)
 
-    def ExportToPCI(self, *args):
+    def ExportToPCI(self, *args) -> "OGRErr":
         r"""ExportToPCI(SpatialReference self) -> OGRErr"""
         return _osr.SpatialReference_ExportToPCI(self, *args)
 
-    def ExportToUSGS(self, *args):
+    def ExportToUSGS(self, *args) -> "OGRErr":
         r"""ExportToUSGS(SpatialReference self) -> OGRErr"""
         return _osr.SpatialReference_ExportToUSGS(self, *args)
 
-    def ExportToXML(self, *args):
+    def ExportToXML(self, *args) -> "OGRErr":
         r"""ExportToXML(SpatialReference self, char const * dialect="") -> OGRErr"""
         return _osr.SpatialReference_ExportToXML(self, *args)
 
-    def ExportToMICoordSys(self, *args):
+    def ExportToMICoordSys(self, *args) -> "OGRErr":
         r"""ExportToMICoordSys(SpatialReference self) -> OGRErr"""
         return _osr.SpatialReference_ExportToMICoordSys(self, *args)
 
-    def CloneGeogCS(self, *args):
+    def CloneGeogCS(self, *args) -> "OSRSpatialReferenceShadow *":
         r"""CloneGeogCS(SpatialReference self) -> SpatialReference"""
         return _osr.SpatialReference_CloneGeogCS(self, *args)
 
-    def Clone(self, *args):
+    def Clone(self, *args) -> "OSRSpatialReferenceShadow *":
         r"""Clone(SpatialReference self) -> SpatialReference"""
         return _osr.SpatialReference_Clone(self, *args)
 
-    def Validate(self, *args):
+    def StripVertical(self, *args) -> "OGRErr":
+        r"""StripVertical(SpatialReference self) -> OGRErr"""
+        return _osr.SpatialReference_StripVertical(self, *args)
+
+    def Validate(self, *args) -> "OGRErr":
         r"""Validate(SpatialReference self) -> OGRErr"""
         return _osr.SpatialReference_Validate(self, *args)
 
-    def MorphToESRI(self, *args):
+    def MorphToESRI(self, *args) -> "OGRErr":
         r"""MorphToESRI(SpatialReference self) -> OGRErr"""
         return _osr.SpatialReference_MorphToESRI(self, *args)
 
-    def MorphFromESRI(self, *args):
+    def MorphFromESRI(self, *args) -> "OGRErr":
         r"""MorphFromESRI(SpatialReference self) -> OGRErr"""
         return _osr.SpatialReference_MorphFromESRI(self, *args)
 
-    def ConvertToOtherProjection(self, *args):
+    def ConvertToOtherProjection(self, *args) -> "OSRSpatialReferenceShadow *":
         r"""ConvertToOtherProjection(SpatialReference self, char const * other_projection, char ** options=None) -> SpatialReference"""
         return _osr.SpatialReference_ConvertToOtherProjection(self, *args)
 
-    def PromoteTo3D(self, *args):
+    def PromoteTo3D(self, *args) -> "OGRErr":
         r"""PromoteTo3D(SpatialReference self, char const * name=None) -> OGRErr"""
         return _osr.SpatialReference_PromoteTo3D(self, *args)
 
-    def DemoteTo2D(self, *args):
+    def DemoteTo2D(self, *args) -> "OGRErr":
         r"""DemoteTo2D(SpatialReference self, char const * name=None) -> OGRErr"""
         return _osr.SpatialReference_DemoteTo2D(self, *args)
 
 
     def __init__(self, *args, **kwargs):
         """__init__(OSRSpatialReferenceShadow self, char const * wkt) -> SpatialReference"""
         oldval = _osr.GetUseExceptions()
@@ -891,27 +895,27 @@
     __repr__ = _swig_repr
 
     def __init__(self, *args):
         r"""__init__(CoordinateTransformationOptions self) -> CoordinateTransformationOptions"""
         _osr.CoordinateTransformationOptions_swiginit(self, _osr.new_CoordinateTransformationOptions(*args))
     __swig_destroy__ = _osr.delete_CoordinateTransformationOptions
 
-    def SetAreaOfInterest(self, *args):
+    def SetAreaOfInterest(self, *args) -> "bool":
         r"""SetAreaOfInterest(CoordinateTransformationOptions self, double westLongitudeDeg, double southLatitudeDeg, double eastLongitudeDeg, double northLatitudeDeg) -> bool"""
         return _osr.CoordinateTransformationOptions_SetAreaOfInterest(self, *args)
 
-    def SetOperation(self, *args):
-        r"""SetOperation(CoordinateTransformationOptions self, char const * operation) -> bool"""
+    def SetOperation(self, *args) -> "bool":
+        r"""SetOperation(CoordinateTransformationOptions self, char const * operation, bool inverseCT=False) -> bool"""
         return _osr.CoordinateTransformationOptions_SetOperation(self, *args)
 
-    def SetDesiredAccuracy(self, *args):
+    def SetDesiredAccuracy(self, *args) -> "bool":
         r"""SetDesiredAccuracy(CoordinateTransformationOptions self, double accuracy) -> bool"""
         return _osr.CoordinateTransformationOptions_SetDesiredAccuracy(self, *args)
 
-    def SetBallparkAllowed(self, *args):
+    def SetBallparkAllowed(self, *args) -> "bool":
         r"""SetBallparkAllowed(CoordinateTransformationOptions self, bool allowBallpark) -> bool"""
         return _osr.CoordinateTransformationOptions_SetBallparkAllowed(self, *args)
 
 # Register CoordinateTransformationOptions in _osr:
 _osr.CoordinateTransformationOptions_swigregister(CoordinateTransformationOptions)
 
 class CoordinateTransformation(object):
@@ -924,40 +928,44 @@
         r"""
         __init__(CoordinateTransformation self, SpatialReference src, SpatialReference dst) -> CoordinateTransformation
         __init__(CoordinateTransformation self, SpatialReference src, SpatialReference dst, CoordinateTransformationOptions options) -> CoordinateTransformation
         """
         _osr.CoordinateTransformation_swiginit(self, _osr.new_CoordinateTransformation(*args))
     __swig_destroy__ = _osr.delete_CoordinateTransformation
 
-    def TransformPoint(self, *args):
+    def GetInverse(self, *args) -> "OSRCoordinateTransformationShadow *":
+        r"""GetInverse(CoordinateTransformation self) -> CoordinateTransformation"""
+        return _osr.CoordinateTransformation_GetInverse(self, *args)
+
+    def TransformPoint(self, *args) -> "void":
         r"""
         TransformPoint(CoordinateTransformation self, double [3] inout)
         TransformPoint(CoordinateTransformation self, double [4] inout)
         TransformPoint(CoordinateTransformation self, double x, double y, double z=0.0)
         TransformPoint(CoordinateTransformation self, double x, double y, double z, double t)
         """
         return _osr.CoordinateTransformation_TransformPoint(self, *args)
 
-    def TransformPointWithErrorCode(self, *args):
+    def TransformPointWithErrorCode(self, *args) -> "void":
         r"""TransformPointWithErrorCode(CoordinateTransformation self, double x, double y, double z, double t)"""
         return _osr.CoordinateTransformation_TransformPointWithErrorCode(self, *args)
 
-    def TransformPoints(self, *args):
+    def TransformPoints(self, *args) -> "void":
         r"""TransformPoints(CoordinateTransformation self, int nCount)"""
         return _osr.CoordinateTransformation_TransformPoints(self, *args)
 
-    def TransformBounds(self, *args):
+    def TransformBounds(self, *args) -> "void":
         r"""TransformBounds(CoordinateTransformation self, double minx, double miny, double maxx, double maxy, int densify_pts)"""
         return _osr.CoordinateTransformation_TransformBounds(self, *args)
 
 # Register CoordinateTransformation in _osr:
 _osr.CoordinateTransformation_swigregister(CoordinateTransformation)
 
 
-def CreateCoordinateTransformation(*args):
+def CreateCoordinateTransformation(*args) -> "OSRCoordinateTransformationShadow *":
     r"""CreateCoordinateTransformation(SpatialReference src, SpatialReference dst, CoordinateTransformationOptions options=None) -> CoordinateTransformation"""
     return _osr.CreateCoordinateTransformation(*args)
 OSR_CRS_TYPE_GEOGRAPHIC_2D = _osr.OSR_CRS_TYPE_GEOGRAPHIC_2D
 
 OSR_CRS_TYPE_GEOGRAPHIC_3D = _osr.OSR_CRS_TYPE_GEOGRAPHIC_3D
 
 OSR_CRS_TYPE_GEOCENTRIC = _osr.OSR_CRS_TYPE_GEOCENTRIC
@@ -993,104 +1001,104 @@
         _osr.CRSInfo_swiginit(self, _osr.new_CRSInfo(*args))
     __swig_destroy__ = _osr.delete_CRSInfo
 
 # Register CRSInfo in _osr:
 _osr.CRSInfo_swigregister(CRSInfo)
 
 
-def OSRCRSInfo_auth_name_get(*args):
+def OSRCRSInfo_auth_name_get(*args) -> "char const *":
     r"""OSRCRSInfo_auth_name_get(CRSInfo crsInfo) -> char const *"""
     return _osr.OSRCRSInfo_auth_name_get(*args)
 
-def OSRCRSInfo_code_get(*args):
+def OSRCRSInfo_code_get(*args) -> "char const *":
     r"""OSRCRSInfo_code_get(CRSInfo crsInfo) -> char const *"""
     return _osr.OSRCRSInfo_code_get(*args)
 
-def OSRCRSInfo_name_get(*args):
+def OSRCRSInfo_name_get(*args) -> "char const *":
     r"""OSRCRSInfo_name_get(CRSInfo crsInfo) -> char const *"""
     return _osr.OSRCRSInfo_name_get(*args)
 
-def OSRCRSInfo_type_get(*args):
+def OSRCRSInfo_type_get(*args) -> "OSRCRSType":
     r"""OSRCRSInfo_type_get(CRSInfo crsInfo) -> OSRCRSType"""
     return _osr.OSRCRSInfo_type_get(*args)
 
-def OSRCRSInfo_deprecated_get(*args):
+def OSRCRSInfo_deprecated_get(*args) -> "bool":
     r"""OSRCRSInfo_deprecated_get(CRSInfo crsInfo) -> bool"""
     return _osr.OSRCRSInfo_deprecated_get(*args)
 
-def OSRCRSInfo_bbox_valid_get(*args):
+def OSRCRSInfo_bbox_valid_get(*args) -> "bool":
     r"""OSRCRSInfo_bbox_valid_get(CRSInfo crsInfo) -> bool"""
     return _osr.OSRCRSInfo_bbox_valid_get(*args)
 
-def OSRCRSInfo_west_lon_degree_get(*args):
+def OSRCRSInfo_west_lon_degree_get(*args) -> "double":
     r"""OSRCRSInfo_west_lon_degree_get(CRSInfo crsInfo) -> double"""
     return _osr.OSRCRSInfo_west_lon_degree_get(*args)
 
-def OSRCRSInfo_south_lat_degree_get(*args):
+def OSRCRSInfo_south_lat_degree_get(*args) -> "double":
     r"""OSRCRSInfo_south_lat_degree_get(CRSInfo crsInfo) -> double"""
     return _osr.OSRCRSInfo_south_lat_degree_get(*args)
 
-def OSRCRSInfo_east_lon_degree_get(*args):
+def OSRCRSInfo_east_lon_degree_get(*args) -> "double":
     r"""OSRCRSInfo_east_lon_degree_get(CRSInfo crsInfo) -> double"""
     return _osr.OSRCRSInfo_east_lon_degree_get(*args)
 
-def OSRCRSInfo_north_lat_degree_get(*args):
+def OSRCRSInfo_north_lat_degree_get(*args) -> "double":
     r"""OSRCRSInfo_north_lat_degree_get(CRSInfo crsInfo) -> double"""
     return _osr.OSRCRSInfo_north_lat_degree_get(*args)
 
-def OSRCRSInfo_area_name_get(*args):
+def OSRCRSInfo_area_name_get(*args) -> "char const *":
     r"""OSRCRSInfo_area_name_get(CRSInfo crsInfo) -> char const *"""
     return _osr.OSRCRSInfo_area_name_get(*args)
 
-def OSRCRSInfo_projection_method_get(*args):
+def OSRCRSInfo_projection_method_get(*args) -> "char const *":
     r"""OSRCRSInfo_projection_method_get(CRSInfo crsInfo) -> char const *"""
     return _osr.OSRCRSInfo_projection_method_get(*args)
 
-def GetCRSInfoListFromDatabase(*args):
+def GetCRSInfoListFromDatabase(*args) -> "int *":
     r"""GetCRSInfoListFromDatabase(char const * authName)"""
     return _osr.GetCRSInfoListFromDatabase(*args)
 
-def SetPROJSearchPath(*args):
+def SetPROJSearchPath(*args) -> "void":
     r"""SetPROJSearchPath(char const * utf8_path)"""
     return _osr.SetPROJSearchPath(*args)
 
-def SetPROJSearchPaths(*args):
+def SetPROJSearchPaths(*args) -> "void":
     r"""SetPROJSearchPaths(char ** paths)"""
     return _osr.SetPROJSearchPaths(*args)
 
-def GetPROJSearchPaths(*args):
+def GetPROJSearchPaths(*args) -> "char **":
     r"""GetPROJSearchPaths() -> char **"""
     return _osr.GetPROJSearchPaths(*args)
 
-def GetPROJVersionMajor(*args):
+def GetPROJVersionMajor(*args) -> "int":
     r"""GetPROJVersionMajor() -> int"""
     return _osr.GetPROJVersionMajor(*args)
 
-def GetPROJVersionMinor(*args):
+def GetPROJVersionMinor(*args) -> "int":
     r"""GetPROJVersionMinor() -> int"""
     return _osr.GetPROJVersionMinor(*args)
 
-def GetPROJVersionMicro(*args):
+def GetPROJVersionMicro(*args) -> "int":
     r"""GetPROJVersionMicro() -> int"""
     return _osr.GetPROJVersionMicro(*args)
 
-def GetPROJEnableNetwork(*args):
+def GetPROJEnableNetwork(*args) -> "bool":
     r"""GetPROJEnableNetwork() -> bool"""
     return _osr.GetPROJEnableNetwork(*args)
 
-def SetPROJEnableNetwork(*args):
+def SetPROJEnableNetwork(*args) -> "void":
     r"""SetPROJEnableNetwork(bool enabled)"""
     return _osr.SetPROJEnableNetwork(*args)
 
-def SetPROJAuxDbPath(*args):
+def SetPROJAuxDbPath(*args) -> "void":
     r"""SetPROJAuxDbPath(char const * utf8_path)"""
     return _osr.SetPROJAuxDbPath(*args)
 
-def SetPROJAuxDbPaths(*args):
+def SetPROJAuxDbPaths(*args) -> "void":
     r"""SetPROJAuxDbPaths(char ** paths)"""
     return _osr.SetPROJAuxDbPaths(*args)
 
-def GetPROJAuxDbPaths(*args):
+def GetPROJAuxDbPaths(*args) -> "char **":
     r"""GetPROJAuxDbPaths() -> char **"""
     return _osr.GetPROJAuxDbPaths(*args)
```

### Comparing `pygdal-3.5.3.11/pygdal.egg-info/PKG-INFO` & `pygdal-3.6.4.11/pygdal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygdal
-Version: 3.5.3.11
+Version: 3.6.4.11
 Summary: Virtualenv and setuptools friendly version of standard GDAL python bindings
 Home-page: https://github.com/nextgis/pygdal
 Author: Frank Warmerdam
 Author-email: warmerdam@pobox.com
 Maintainer: Aleksandr Dezhin
 Maintainer-email: me@dezhin.net
 License: MIT
```

### Comparing `pygdal-3.5.3.11/pygdal.egg-info/SOURCES.txt` & `pygdal-3.6.4.11/pygdal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygdal-3.5.3.11/setup.py` & `pygdal-3.6.4.11/setup.py`

 * *Files identical despite different names*

