# Comparing `tmp/pysparse-array-0.1.4.tar.gz` & `tmp/pysparse-array-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparse-array-0.1.4.tar", last modified: Tue May 16 17:50:44 2023, max compression
+gzip compressed data, was "pysparse-array-0.1.5.tar", last modified: Thu May 18 13:19:17 2023, max compression
```

## Comparing `pysparse-array-0.1.4.tar` & `pysparse-array-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-16 17:50:44.864418 pysparse-array-0.1.4/
--rw-r--r--   0 thomasfrost   (502) staff       (20)     1497 2023-05-16 17:50:07.000000 pysparse-array-0.1.4/HISTORY.md
--rw-r--r--   0 thomasfrost   (502) staff       (20)     1060 2023-05-15 14:53:09.000000 pysparse-array-0.1.4/LICENSE.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)       19 2023-05-16 11:11:47.000000 pysparse-array-0.1.4/MANIFEST.in
--rw-r--r--   0 thomasfrost   (502) staff       (20)     2289 2023-05-16 17:50:44.846358 pysparse-array-0.1.4/PKG-INFO
--rw-r--r--   0 thomasfrost   (502) staff       (20)     1584 2023-05-15 17:35:02.000000 pysparse-array-0.1.4/README.md
--rw-r--r--   0 thomasfrost   (502) staff       (20)      779 2023-05-16 15:01:18.000000 pysparse-array-0.1.4/pyproject.toml
-drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-16 17:50:44.777049 pysparse-array-0.1.4/pysparse_array.egg-info/
--rw-r--r--   0 thomasfrost   (502) staff       (20)     2289 2023-05-16 17:50:44.000000 pysparse-array-0.1.4/pysparse_array.egg-info/PKG-INFO
--rw-r--r--   0 thomasfrost   (502) staff       (20)      311 2023-05-16 17:50:44.000000 pysparse-array-0.1.4/pysparse_array.egg-info/SOURCES.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)        1 2023-05-16 17:50:44.000000 pysparse-array-0.1.4/pysparse_array.egg-info/dependency_links.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)       47 2023-05-16 17:50:44.000000 pysparse-array-0.1.4/pysparse_array.egg-info/requires.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)        7 2023-05-16 17:50:44.000000 pysparse-array-0.1.4/pysparse_array.egg-info/top_level.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)       38 2023-05-16 17:50:44.864812 pysparse-array-0.1.4/setup.cfg
--rw-r--r--   0 thomasfrost   (502) staff       (20)      708 2023-05-16 15:01:08.000000 pysparse-array-0.1.4/setup.py
-drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-16 17:50:44.841362 pysparse-array-0.1.4/sparse/
--rw-r--r--   0 thomasfrost   (502) staff       (20)      113 2023-05-16 11:47:08.000000 pysparse-array-0.1.4/sparse/__init__.py
--rw-r--r--   0 thomasfrost   (502) staff       (20)     9291 2023-05-16 17:35:44.000000 pysparse-array-0.1.4/sparse/array_api.py
--rw-r--r--   0 thomasfrost   (502) staff       (20)     6821 2023-05-16 12:54:50.000000 pysparse-array-0.1.4/sparse/core.py
+drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-18 13:19:17.676799 pysparse-array-0.1.5/
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     1680 2023-05-18 11:13:40.000000 pysparse-array-0.1.5/HISTORY.md
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     1060 2023-05-15 14:53:09.000000 pysparse-array-0.1.5/LICENSE.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)       19 2023-05-16 11:11:47.000000 pysparse-array-0.1.5/MANIFEST.in
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     5091 2023-05-18 13:19:17.638477 pysparse-array-0.1.5/PKG-INFO
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     4386 2023-05-18 13:18:38.000000 pysparse-array-0.1.5/README.md
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      779 2023-05-18 12:07:42.000000 pysparse-array-0.1.5/pyproject.toml
+drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-18 13:19:17.370822 pysparse-array-0.1.5/pysparse_array.egg-info/
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     5091 2023-05-18 13:19:17.000000 pysparse-array-0.1.5/pysparse_array.egg-info/PKG-INFO
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      311 2023-05-18 13:19:17.000000 pysparse-array-0.1.5/pysparse_array.egg-info/SOURCES.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)        1 2023-05-18 13:19:17.000000 pysparse-array-0.1.5/pysparse_array.egg-info/dependency_links.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)       47 2023-05-18 13:19:17.000000 pysparse-array-0.1.5/pysparse_array.egg-info/requires.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)        7 2023-05-18 13:19:17.000000 pysparse-array-0.1.5/pysparse_array.egg-info/top_level.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)       38 2023-05-18 13:19:17.677325 pysparse-array-0.1.5/setup.cfg
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      708 2023-05-18 12:07:54.000000 pysparse-array-0.1.5/setup.py
+drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-18 13:19:17.636387 pysparse-array-0.1.5/sparse/
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      113 2023-05-16 11:47:08.000000 pysparse-array-0.1.5/sparse/__init__.py
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     9489 2023-05-18 12:33:48.000000 pysparse-array-0.1.5/sparse/array_api.py
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     6829 2023-05-18 12:03:39.000000 pysparse-array-0.1.5/sparse/core.py
```

### Comparing `pysparse-array-0.1.4/HISTORY.md` & `pysparse-array-0.1.5/HISTORY.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,27 @@
 #Changelog
 
 All notable changes to the `PySparse` package will be documented in this file.
 
 ## [Unreleased]
 
+## [0.1.5] - 2023-05-18
+
+### Added
+- N/A
+
+### Fixed
+- N/A
+
+### Changed
+- Further optimised indexing through use of parallel find_indices search, with x2 speed-up.
+
+### Removed
+- N/A
+
 ## [0.1.4] - 2023-05-16
 
 ### Added
 - load_sparse() can now take either a single path to the parent directory of the three arrays, or individual paths to each
 - if using a single path to parent directory to load the sparse arrays, the files must be kept named as the standard 'sparse_data.npy', 'sparse_coords.npy', and 'dense_shape.npy' filenames
 
 ### Fixed
```

### Comparing `pysparse-array-0.1.4/LICENSE.txt` & `pysparse-array-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pysparse-array-0.1.4/pyproject.toml` & `pysparse-array-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "pysparse-array"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
 	{ name="Thomas Frost", email="tdgfrost@gmail.com" },
 ]
 description = "A package that enables on-the-fly encoding and decoding of large NumPy arrays as Sparse binaries."
 readme = "README.md"
 requires-python = ">=3.8.0"
 classifiers = [
```

### Comparing `pysparse-array-0.1.4/setup.py` & `pysparse-array-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme_file.read()
 
 with open('HISTORY.md') as history_file:
     HISTORY = history_file.read()
 
 setup_args = dict(
     name='pysparse-array',
-    version='0.1.4',
+    version='0.1.5',
     description='Package to encode and decode large OOM numpy arrays as Sparse binaries',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n' + HISTORY,
     packages=find_packages(),
     author='Thomas Frost',
     author_email='tdgfrost@gmail.com',
     url='https://github.com/tdgfrost/PySparse',
```

### Comparing `pysparse-array-0.1.4/sparse/array_api.py` & `pysparse-array-0.1.5/sparse/array_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import numpy as np
-from numba import njit, types
+from numba import njit, types, prange, typed
+from numpy import ndarray
+
 from .core import find_indices
 import os
 
 
-def load_sparse(data_path: str, coords_path='', shape='', mode='r'):
+def load_sparse(data_path: str, coords_path=None, shape=None):
     """
     Load a (memory-mapped) sparse array from disk
     :param data_path: path to sparse data array OR parent directory containing 'sparse_data.npy', 'sparse_coords.npy', and 'dense_shape.npy' arrays
-    :param coords_path: path to sparse coordinates array
-    :param shape: shape of the dense array, as either tuple or path to numpy array containing shape
-    :param mode: mode to open the sparse arrays in (e.g., read-only, read-write, etc.) - r/r+/w
+    :param coords_path: (optional) path to sparse coordinates array
+    :param shape: (optional) shape of the dense array, as either tuple or path to numpy array containing shape
     :return: SparseArray object
     """
     if os.path.isdir(data_path):
         coords_path = os.path.join(data_path, 'sparse_coords.npy')
         shape = os.path.join(data_path, 'dense_shape.npy')
         data_path = os.path.join(data_path, 'sparse_data.npy')
 
-    return SparseArray(data_path, coords_path, shape, mode)
+    return SparseArray(data_path, coords_path, shape, mode='r')
 
 
 class SparseArray:
     def __init__(self, data_path: str, coords_path: str, shape: str or tuple, mode='r'):
         self.data = np.load(data_path, mmap_mode=mode)
         self.data_dtype = self.data.dtype
 
@@ -116,14 +117,16 @@
         search_function = {int: self.__find_rows_int,
                            np.ndarray: self.__find_rows_ndarray}
 
         # Find the target coordinates for the given row indices
         find_coords, coords_present = search_function[type(row_idx)](self.coords, row_idx,
                                                                      maxlen=self.coords_shape[0])
 
+        find_coords = np.concatenate([np.arange(start, end+1) for start, end in find_coords if start != -1])
+
         # Assuming the row indices have non-zero data...
         if coords_present:
             # Locate the coordinates of the non-zero data in the original dense array
             target_coords = self.coords[find_coords]
 
             # Some slightly complex indexing to identify the non-zero cells of the (indexed) target array
             nonzero_row_indices_unique = np.where(np.isin(row_idx, np.unique(target_coords[:, 0])))[0]
@@ -131,30 +134,30 @@
 
             target_coords[:, 0] = -1
             target_coords[nonzero_row_indices_unique_idx, 0] = nonzero_row_indices_unique
 
             target_coords[:, 0] = np.maximum.accumulate(target_coords[:, 0], axis=0)
 
             # Re-create the dense array (of the shape requested) with all zeros
-            target_data = np.zeros((1,) + self.dense_shape[1:]) if isinstance(row_idx, int) else np.zeros(
-                (len(row_idx),) + self.dense_shape[1:])
+            target_data = np.zeros((1,) + self.dense_shape[1:], dtype=self.data_dtype) if isinstance(row_idx, int) else np.zeros(
+                (len(row_idx),) + self.dense_shape[1:], dtype=self.data_dtype)
 
             # Fill the dense array with the non-zero data at the target coordinates
             target_data[tuple(target_coords.T)] = self.data[find_coords]
         else:
             # If the row indices have no non-zero data, return an array of zeros
-            target_data = np.zeros((1,) + self.dense_shape[1:]) if isinstance(row_idx, int) else np.zeros(
-                (len(row_idx),) + self.dense_shape[1:])
+            target_data = np.zeros((1,) + self.dense_shape[1:], dtype=self.data_dtype) if isinstance(row_idx, int) else np.zeros(
+                (len(row_idx),) + self.dense_shape[1:], dtype=self.data_dtype)
 
         return target_data
 
     @staticmethod
     @njit(types.Tuple((types.int64[:], types.boolean))(types.Array(types.int32, 2, 'C', readonly=True), types.int64,
                                                        types.int64))
-    def __find_rows_int(coords: np.ndarray, row_idx: int, maxlen: int) -> types.Tuple:
+    def __find_rows_int(coords: np.ndarray, row_idx: int, maxlen: int) -> tuple[ndarray, bool]:
         """
         Efficiently search the coordinates to find the indices that match the given row index
         :param coords: numpy 2D array of coordinates
         :param row_idx: target row index (integer)
         :param maxlen: maximum length of the coordinates array
         :return: numpy array of coordinates that match the given row index
         """
@@ -163,35 +166,34 @@
         start_point, end_point = find_indices(coords, row_idx, 0, maxlen - 1)
 
         coords_present = True if start_point >= 0 else False
 
         return np.array([i for i in range(start_point, end_point + 1)]), coords_present
 
     @staticmethod
-    @njit(types.Tuple((types.int64[:], types.boolean))(types.Array(types.int32, 2, 'C', readonly=True),
-                                                       types.Array(types.int64, 1, 'A'), types.int64))
+    @njit(types.Tuple((types.ListType(types.UniTuple(types.int64, 2)), types.boolean))(types.Array(types.int32, 2, 'C', readonly=True),
+                                                                                       types.Array(types.int64, 1, 'A'), types.int64),
+          parallel=True)
     def __find_rows_ndarray(coords: np.ndarray, row_idx: np.ndarray, maxlen: int) -> (np.ndarray, bool):
         """
         Efficiently search the coordinates to find the indices that match the given row indices
         :param coords: numpy 2D array of coordinates
         :param row_idx: target row indices (numpy array)
         :param maxlen: maximum length of the coordinates array
         :return: numpy array of coordinates that match the given row indices
         """
 
-        find_coords = []
+        find_coords = typed.List([(-1, -1) for _ in range(len(row_idx))])
 
-        for row in np.sort(row_idx):
+        for row in prange(len(row_idx)):
             # Start with an efficient binary tree search algorithm for identifying the start and end indices
-            start_point, end_point = find_indices(coords, row, 0, maxlen - 1)
-            find_coords.extend([i for i in range(start_point, end_point + 1)]) if start_point >= 0 else None
-
-        coords_present = True if find_coords else False
+            start_point, end_point = find_indices(coords, row_idx[row], 0, maxlen - 1)
+            find_coords[row] = (start_point, end_point)
 
-        return np.array(find_coords), coords_present
+        return find_coords, True
 
     def __get_item(self, items) -> np.ndarray:
         """
         Get the values of the dense array at the given indices
         :param items: tuple of indices
         :return: dense numpy array values at the given indices
         """
```

### Comparing `pysparse-array-0.1.4/sparse/core.py` & `pysparse-array-0.1.5/sparse/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 from numpy.lib.format import open_memmap
 from tqdm import tqdm
 import os
-from numba import njit, types
+from numba import njit, types, prange
 
 
 """
 ============================================================
 Sparse array conversion functions
 ============================================================
 """
```

