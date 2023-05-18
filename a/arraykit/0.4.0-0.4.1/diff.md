# Comparing `tmp/arraykit-0.4.0.tar.gz` & `tmp/arraykit-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arraykit-0.4.0.tar", last modified: Tue May 16 21:35:42 2023, max compression
+gzip compressed data, was "arraykit-0.4.1.tar", last modified: Wed May 17 23:06:51 2023, max compression
```

## Comparing `arraykit-0.4.0.tar` & `arraykit-0.4.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 21:35:42.821501 arraykit-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1779 2023-05-16 21:35:38.000000 arraykit-0.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-16 21:35:38.000000 arraykit-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1178 2023-05-16 21:35:42.821501 arraykit-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3731 2023-05-16 21:35:38.000000 arraykit-0.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 21:35:42.817501 arraykit-0.4.0/arraykit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1178 2023-05-16 21:35:42.000000 arraykit-0.4.0/arraykit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      495 2023-05-16 21:35:42.000000 arraykit-0.4.0/arraykit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-16 21:35:42.000000 arraykit-0.4.0/arraykit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-05-16 21:35:42.000000 arraykit-0.4.0/arraykit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-16 21:35:42.000000 arraykit-0.4.0/arraykit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-16 21:35:42.821501 arraykit-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2698 2023-05-16 21:35:38.000000 arraykit-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 21:35:42.817501 arraykit-0.4.0/src/
--rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-05-16 21:35:38.000000 arraykit-0.4.0/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   174826 2023-05-16 21:35:38.000000 arraykit-0.4.0/src/_arraykit.c
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 21:35:42.821501 arraykit-0.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (122)     3129 2023-05-16 21:35:38.000000 arraykit-0.4.0/test/test_array_go.py
--rw-r--r--   0 runner    (1001) docker     (122)    16629 2023-05-16 21:35:38.000000 arraykit-0.4.0/test/test_block_index.py
--rw-r--r--   0 runner    (1001) docker     (122)    49054 2023-05-16 21:35:38.000000 arraykit-0.4.0/test/test_delimited_to_arrays.py
--rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-05-16 21:35:38.000000 arraykit-0.4.0/test/test_delimited_to_arrays_integration.py
--rw-r--r--   0 runner    (1001) docker     (122)     2205 2023-05-16 21:35:38.000000 arraykit-0.4.0/test/test_delimited_to_arrays_property.py
--rw-r--r--   0 runner    (1001) docker     (122)     1957 2023-05-16 21:35:38.000000 arraykit-0.4.0/test/test_pyi.py
--rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-05-16 21:35:38.000000 arraykit-0.4.0/test/test_split_after_count.py
--rw-r--r--   0 runner    (1001) docker     (122)    28073 2023-05-16 21:35:38.000000 arraykit-0.4.0/test/test_type_discovery.py
--rw-r--r--   0 runner    (1001) docker     (122)    26140 2023-05-16 21:35:38.000000 arraykit-0.4.0/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 23:06:51.449581 arraykit-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1779 2023-05-17 23:06:45.000000 arraykit-0.4.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-17 23:06:45.000000 arraykit-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1178 2023-05-17 23:06:51.449581 arraykit-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3957 2023-05-17 23:06:45.000000 arraykit-0.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 23:06:51.449581 arraykit-0.4.1/arraykit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1178 2023-05-17 23:06:51.000000 arraykit-0.4.1/arraykit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      495 2023-05-17 23:06:51.000000 arraykit-0.4.1/arraykit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 23:06:51.000000 arraykit-0.4.1/arraykit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-05-17 23:06:51.000000 arraykit-0.4.1/arraykit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-17 23:06:51.000000 arraykit-0.4.1/arraykit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-17 23:06:51.449581 arraykit-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2698 2023-05-17 23:06:45.000000 arraykit-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 23:06:51.449581 arraykit-0.4.1/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     1379 2023-05-17 23:06:45.000000 arraykit-0.4.1/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   175735 2023-05-17 23:06:45.000000 arraykit-0.4.1/src/_arraykit.c
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 23:06:51.449581 arraykit-0.4.1/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     3129 2023-05-17 23:06:45.000000 arraykit-0.4.1/test/test_array_go.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18219 2023-05-17 23:06:45.000000 arraykit-0.4.1/test/test_block_index.py
+-rw-r--r--   0 runner    (1001) docker     (122)    49054 2023-05-17 23:06:45.000000 arraykit-0.4.1/test/test_delimited_to_arrays.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-05-17 23:06:45.000000 arraykit-0.4.1/test/test_delimited_to_arrays_integration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2205 2023-05-17 23:06:45.000000 arraykit-0.4.1/test/test_delimited_to_arrays_property.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1961 2023-05-17 23:06:45.000000 arraykit-0.4.1/test/test_pyi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-05-17 23:06:45.000000 arraykit-0.4.1/test/test_split_after_count.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28073 2023-05-17 23:06:45.000000 arraykit-0.4.1/test/test_type_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26140 2023-05-17 23:06:45.000000 arraykit-0.4.1/test/test_util.py
```

### Comparing `arraykit-0.4.0/LICENSE.txt` & `arraykit-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.0/PKG-INFO` & `arraykit-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: arraykit
-Version: 0.4.0
+Version: 0.4.1
 Summary: Array utilities for StaticFrame
 Home-page: https://github.com/static-frame/arraykit
 Author: Christopher Ariza, Brandt Bucher, Charles Burkland
 License: MIT
 Description: The ArrayKit library provides utilities for creating and transforming NumPy arrays, implementing performance-critical StaticFrame operations as Python C extensions.
         
         Code: https://github.com/static-frame/arraykit
```

### Comparing `arraykit-0.4.0/README.rst` & `arraykit-0.4.1/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -33,14 +33,23 @@
 - NumPy >= 1.18.5
 
 
 
 What is New in ArrayKit
 -------------------------
 
+0.4.1
+............
+
+Updated ``BlockIndex.register()`` to handle 0-column 2D arrays and return False.
+
+Added ``BlockIndex.rows``, ``BlockIndex.columns`` properties.
+
+Updated unset ``BlockIndex.dtype`` to return a float dtype.
+
 
 0.4.0
 ............
 
 Added ``BlockIndex``, a tool to be used by ``TypeBlocks`` for mapping realized column positions to arrays.
 
 Corrected potential issue in ``AK_CPL_resize_buffer`` that could segfault for very large offsets.
```

### Comparing `arraykit-0.4.0/arraykit.egg-info/PKG-INFO` & `arraykit-0.4.1/arraykit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: arraykit
-Version: 0.4.0
+Version: 0.4.1
 Summary: Array utilities for StaticFrame
 Home-page: https://github.com/static-frame/arraykit
 Author: Christopher Ariza, Brandt Bucher, Charles Burkland
 License: MIT
 Description: The ArrayKit library provides utilities for creating and transforming NumPy arrays, implementing performance-critical StaticFrame operations as Python C extensions.
         
         Code: https://github.com/static-frame/arraykit
```

### Comparing `arraykit-0.4.0/setup.py` & `arraykit-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import site
 import os
 import typing as tp
 from setuptools import Extension  # type: ignore
 from setuptools import setup
 from pathlib import Path
 
-AK_VERSION = '0.4.0'
+AK_VERSION = '0.4.1'
 
 def get_long_description() -> str:
     return '''The ArrayKit library provides utilities for creating and transforming NumPy arrays, implementing performance-critical StaticFrame operations as Python C extensions.
 
 Code: https://github.com/static-frame/arraykit
 
 Packages: https://pypi.org/project/arraykit
```

### Comparing `arraykit-0.4.0/src/__init__.py` & `arraykit-0.4.1/src/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pylint: disable=W0611
 # pylint: disable=E0401
 # pylint: disable=C0414
 
 from ._arraykit import __version__
 from ._arraykit import ArrayGO as ArrayGO
 from ._arraykit import BlockIndex as BlockIndex
-from ._arraykit import ErrorInitBlocks as ErrorInitBlocks
+from ._arraykit import ErrorInitTypeBlocks as ErrorInitTypeBlocks
 
 from ._arraykit import immutable_filter as immutable_filter
 from ._arraykit import mloc as mloc
 from ._arraykit import name_filter as name_filter
 from ._arraykit import shape_filter as shape_filter
 from ._arraykit import column_2d_filter as column_2d_filter
 from ._arraykit import column_1d_filter as column_1d_filter
```

### Comparing `arraykit-0.4.0/src/_arraykit.c` & `arraykit-0.4.1/src/_arraykit.c`

 * *Files 0% similar despite different names*

```diff
@@ -4110,15 +4110,15 @@
 }
 
 //------------------------------------------------------------------------------
 // BlockIndex
 //------------------------------------------------------------------------------
 
 static PyTypeObject BlockIndexType;
-static PyObject *ErrorInitBlocks;
+static PyObject *ErrorInitTypeBlocks;
 
 // NOTE: we use platform size types here, which are appropriate for the values, but might pose issues if trying to pass pickles between 32 and 64 bit machines.
 typedef struct BlockIndexRecord {
     Py_ssize_t block; // signed
     Py_ssize_t column;
 } BlockIndexRecord;
 
@@ -4773,43 +4773,47 @@
             Py_TYPE(self)->tp_name,
             self->block_count,
             self->row_count,
             self->bir_count,
             dt);
 }
 
-// Returns NULL on error, None otherwise. This checks and raises on non-array inputs, dimensions other than 1 or 2.
+// Returns NULL on error, True if the block should be reatained, False if the block has zero columns and should not be retained. This checks and raises on non-array inputs, dimensions other than 1 or 2, and mis-aligned columns.
 static PyObject *
 BlockIndex_register(BlockIndexObject *self, PyObject *value) {
     if (!PyArray_Check(value)) {
-        PyErr_Format(ErrorInitBlocks, "Found non-array block: %R", value);
+        PyErr_Format(ErrorInitTypeBlocks, "Found non-array block: %R", value);
         return NULL;
     }
     PyArrayObject *a = (PyArrayObject *)value;
     int ndim = PyArray_NDIM(a);
 
     if (ndim < 1 || ndim > 2) {
-        PyErr_Format(ErrorInitBlocks, "Array block has invalid dimensions: %i", ndim);
+        PyErr_Format(ErrorInitTypeBlocks, "Array block has invalid dimensions: %i", ndim);
         return NULL;
     }
     Py_ssize_t increment = ndim == 1 ? 1 : PyArray_DIM(a, 1);
 
     // assign alignment on first observation; otherwise take
     Py_ssize_t alignment = PyArray_DIM(a, 0);
     if (self->row_count == -1) {
         self->row_count = alignment;
     }
     else if (self->row_count != alignment) {
-        PyErr_Format(ErrorInitBlocks,
+        PyErr_Format(ErrorInitTypeBlocks,
                 "Array block has unaligned row count: found %i, expected %i",
                 alignment,
                 self->row_count);
         return NULL;
     }
 
+    if (increment == 0) {
+        Py_RETURN_FALSE;
+    }
+
     PyArray_Descr* dt = PyArray_DESCR(a); // borrowed ref
     if (self->dtype == NULL) {
         Py_INCREF((PyObject*)dt);
         self->dtype = dt;
     }
     else if (!PyDataType_ISOBJECT(self->dtype)) {
         PyArray_Descr* dtr = AK_ResolveDTypes(self->dtype, dt); // new ref
@@ -4825,15 +4829,15 @@
     Py_ssize_t bc = self->block_count;
 
     for (Py_ssize_t i = 0; i < increment; i++) {
         bir[self->bir_count] = (BlockIndexRecord){bc, i};
         self->bir_count++;
     }
     self->block_count++;
-    Py_RETURN_NONE;
+    Py_RETURN_TRUE;
 }
 
 
 static PyObject*
 BlockIndex_to_list(BlockIndexObject *self, PyObject *Py_UNUSED(unused)) {
     PyObject* list = PyList_New(self->bir_count);
     if (list == NULL) {
@@ -4938,28 +4942,44 @@
 BlockIndex_iter(BlockIndexObject* self) {
     return BIIter_new(self, 0);
 }
 
 
 static PyObject *
 BlockIndex_shape_getter(BlockIndexObject *self, void* Py_UNUSED(closure)){
+    // NOTE: this could be cached
     return Py_BuildValue("nn", self->row_count, self->bir_count);
 }
 
 static PyObject *
+BlockIndex_rows_getter(BlockIndexObject *self, void* Py_UNUSED(closure)){
+    return PyLong_FromSsize_t(self->row_count);
+}
+
+static PyObject *
+BlockIndex_columns_getter(BlockIndexObject *self, void* Py_UNUSED(closure)){
+    return PyLong_FromSsize_t(self->bir_count );
+}
+
+// Return the resolved dtype for all registered blocks. If no block have been registered, this will return a float dtype.
+static PyObject *
 BlockIndex_dtype_getter(BlockIndexObject *self, void* Py_UNUSED(closure)){
     if (self->dtype != NULL) {
         Py_INCREF(self->dtype);
         return (PyObject*)self->dtype;
     }
-    Py_RETURN_NONE;
+    // NOTE: could use NPY_DEFAULT_TYPE here; SF defines this explicitly as float64
+    return (PyObject*)PyArray_DescrFromType(NPY_FLOAT64);
 }
 
+
 static struct PyGetSetDef BlockIndex_getset[] = {
     {"shape", (getter)BlockIndex_shape_getter, NULL, NULL, NULL},
+    {"rows", (getter)BlockIndex_rows_getter, NULL, NULL, NULL},
+    {"columns", (getter)BlockIndex_columns_getter, NULL, NULL, NULL},
     {"dtype", (getter)BlockIndex_dtype_getter, NULL, NULL, NULL},
     {NULL},
 };
 
 
 static Py_ssize_t
 BlockIndex_length(BlockIndexObject *self){
@@ -5376,20 +5396,20 @@
 };
 
 PyObject *
 PyInit__arraykit(void)
 {
     import_array();
 
-    ErrorInitBlocks = PyErr_NewExceptionWithDoc(
-            "arraykit.ErrorInitBlocks",
+    ErrorInitTypeBlocks = PyErr_NewExceptionWithDoc(
+            "arraykit.ErrorInitTypeBlocks",
             "RuntimeError error in block initialization.",
             PyExc_RuntimeError,
             NULL);
-    if (ErrorInitBlocks == NULL) {
+    if (ErrorInitTypeBlocks == NULL) {
         return NULL;
     }
 
     PyObject *copy = PyImport_ImportModule("copy");
     if (copy == NULL) {
         return NULL;
     }
@@ -5407,15 +5427,15 @@
         PyType_Ready(&BIIterSeqType) ||
         PyType_Ready(&BIIterSliceType) ||
         PyType_Ready(&BIIterBooleanType) ||
         PyType_Ready(&ArrayGOType) ||
         PyModule_AddObject(m, "BlockIndex", (PyObject *) &BlockIndexType) ||
         PyModule_AddObject(m, "ArrayGO", (PyObject *) &ArrayGOType) ||
         PyModule_AddObject(m, "deepcopy", deepcopy) ||
-        PyModule_AddObject(m, "ErrorInitBlocks", ErrorInitBlocks)
+        PyModule_AddObject(m, "ErrorInitTypeBlocks", ErrorInitTypeBlocks)
     ){
         Py_DECREF(deepcopy);
         Py_XDECREF(m);
         return NULL;
     }
     return m;
 }
```

### Comparing `arraykit-0.4.0/test/test_array_go.py` & `arraykit-0.4.1/test/test_array_go.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.0/test/test_block_index.py` & `arraykit-0.4.1/test/test_block_index.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 import ctypes
 import sys
 import pickle
 
 import numpy as np
 
 from arraykit import BlockIndex
-from arraykit import ErrorInitBlocks
+from arraykit import ErrorInitTypeBlocks
 
 
 class TestUnit(unittest.TestCase):
 
     def test_block_index_init_a(self) -> None:
         bi1 = BlockIndex()
+        self.assertEqual(bi1.dtype, np.dtype(float))
         # print(bi1)
 
     def test_block_index_init_b1(self) -> None:
         with self.assertRaises(ValueError):
             _ = BlockIndex(3, 2, 10, 2)
 
     def test_block_index_init_b1(self) -> None:
@@ -48,61 +49,100 @@
         bi1 = BlockIndex()
         self.assertTrue('None' in repr(bi1))
 
     #---------------------------------------------------------------------------
 
     def test_block_index_register_a(self) -> None:
         bi1 = BlockIndex()
-        with self.assertRaises(ErrorInitBlocks):
+        with self.assertRaises(ErrorInitTypeBlocks):
             bi1.register('foo')
 
-        with self.assertRaises(ErrorInitBlocks):
+        with self.assertRaises(ErrorInitTypeBlocks):
             bi1.register(3.5)
 
     def test_block_index_register_b(self) -> None:
 
         bi1 = BlockIndex()
-        with self.assertRaises(ErrorInitBlocks):
+        with self.assertRaises(ErrorInitTypeBlocks):
             bi1.register(np.array(0))
 
-        with self.assertRaises(ErrorInitBlocks):
+        with self.assertRaises(ErrorInitTypeBlocks):
             bi1.register(np.arange(12).reshape(2,3,2))
 
 
     def test_block_index_register_c(self) -> None:
         bi1 = BlockIndex()
         bi1.register(np.array((3, 4, 5)))
         bi1.register(np.array((3, 4, 5)))
         bi1.register(np.arange(6).reshape(3,2))
         self.assertEqual(bi1.to_list(),
             [(0, 0), (1, 0), (2, 0), (2, 1)])
         self.assertEqual(bi1.shape, (3, 4))
+        self.assertEqual(bi1.rows, 3)
+        self.assertEqual(bi1.columns, 4)
 
     def test_block_index_register_d(self) -> None:
         bi1 = BlockIndex()
         bi1.register(np.arange(2))
         bi1.register(np.arange(12).reshape(2,6))
         bi1.register(np.arange(2))
         bi1.register(np.arange(12).reshape(2,6))
         self.assertEqual(bi1.to_list(),
             [(0, 0), (1, 0), (1, 1), (1, 2), (1, 3), (1, 4), (1, 5), (2, 0), (3, 0), (3, 1), (3, 2), (3, 3), (3, 4), (3, 5)]
             )
         self.assertEqual(bi1.shape, (2, 14))
+        self.assertEqual(bi1.rows, 2)
+        self.assertEqual(bi1.columns, 14)
 
     def test_block_index_register_e(self) -> None:
         bi1 = BlockIndex()
         bi1.register(np.arange(2))
-        with self.assertRaises(ErrorInitBlocks):
+        with self.assertRaises(ErrorInitTypeBlocks):
             bi1.register(np.arange(12).reshape(3,4))
 
 
     def test_block_index_register_f(self) -> None:
         bi1 = BlockIndex()
-        a1 = np.arange(20000).reshape(2, 10_000) #.reshape(2, 10_000)
+        a1 = np.arange(20000).reshape(2, 10_000)
         bi1.register(a1)
+        self.assertEqual(bi1.rows, 2)
+        self.assertEqual(bi1.columns, 10_000)
+
+
+    def test_block_index_register_g(self) -> None:
+        bi1 = BlockIndex()
+        a1 = np.array(()).reshape(4, 0)
+        self.assertFalse(bi1.register(a1))
+        self.assertEqual(bi1.shape, (4, 0))
+        # as not dtype has been registered, we will get default float
+        self.assertEqual(bi1.dtype, np.dtype(float))
+
+        a2 = np.arange(8).reshape(4, 2).astype(bool)
+        self.assertTrue(bi1.register(a2))
+        self.assertEqual(bi1.shape, (4, 2))
+        self.assertEqual(bi1.dtype, np.dtype(bool))
+
+
+    def test_block_index_register_h(self) -> None:
+        bi1 = BlockIndex()
+        a1 = np.array(()).reshape(0, 4).astype(bool)
+        self.assertTrue(bi1.register(a1))
+        self.assertEqual(bi1.shape, (0, 4))
+        self.assertEqual(bi1.dtype, np.dtype(bool))
+
+        a2 = np.array(()).reshape(0, 0).astype(float)
+        self.assertFalse(bi1.register(a2))
+        self.assertEqual(bi1.shape, (0, 4))
+        # dtype is still bool
+        self.assertEqual(bi1.dtype, np.dtype(bool))
+
+        a3 = np.array(()).reshape(0, 3).astype(int)
+        self.assertTrue(bi1.register(a3))
+        self.assertEqual(bi1.shape, (0, 7))
+        self.assertEqual(bi1.dtype, np.dtype(object))
 
 
     #---------------------------------------------------------------------------
 
     def test_block_index_to_bytes_a(self) -> None:
         bi1 = BlockIndex()
         bi1.register(np.arange(6).reshape(2,3))
@@ -187,18 +227,19 @@
         self.assertEqual(bi1[a1[1]], (1, 1))
 
     #---------------------------------------------------------------------------
     def test_block_index_getitem_a(self) -> None:
         bi1 = BlockIndex()
         bi1.register(np.arange(12).reshape(2,6))
         self.assertEqual(bi1.shape, (2, 6))
+        self.assertEqual(bi1.columns, 6)
 
         bi1.register(np.arange(4).reshape(2,2))
         self.assertEqual(bi1.shape, (2, 8))
-
+        self.assertEqual(bi1.columns, 8)
 
     def test_block_index_getitem_b(self) -> None:
         bi1 = BlockIndex()
         bi1.register(np.arange(12).reshape(2,6))
         bi1.register(np.arange(4).reshape(2,2))
 
         with self.assertRaises(TypeError):
```

### Comparing `arraykit-0.4.0/test/test_delimited_to_arrays.py` & `arraykit-0.4.1/test/test_delimited_to_arrays.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.0/test/test_delimited_to_arrays_integration.py` & `arraykit-0.4.1/test/test_delimited_to_arrays_integration.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.0/test/test_delimited_to_arrays_property.py` & `arraykit-0.4.1/test/test_delimited_to_arrays_property.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.0/test/test_pyi.py` & `arraykit-0.4.1/test/test_pyi.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         classes: tp.Dict[str: tp.List[str]] = {}
 
         for name in dir(module):
             if not cls._valid_name(name):
                 continue
             obj = getattr(module, name)
             if isinstance(obj, type): # a class
-                if name == ak.ErrorInitBlocks.__name__:
+                if name == ak.ErrorInitTypeBlocks.__name__:
                     # skip as there is Python version variability
                     continue
                 classes[name] = []
                 for part_name in dir(obj):
                     if not cls._valid_name(part_name):
                         continue
                     part_obj = getattr(obj, part_name)
```

### Comparing `arraykit-0.4.0/test/test_split_after_count.py` & `arraykit-0.4.1/test/test_split_after_count.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.0/test/test_type_discovery.py` & `arraykit-0.4.1/test/test_type_discovery.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.0/test/test_util.py` & `arraykit-0.4.1/test/test_util.py`

 * *Files identical despite different names*

