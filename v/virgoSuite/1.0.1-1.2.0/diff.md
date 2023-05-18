# Comparing `tmp/virgoSuite-1.0.1.tar.gz` & `tmp/virgoSuite-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virgoSuite-1.0.1.tar", last modified: Mon May 15 17:16:56 2023, max compression
+gzip compressed data, was "virgoSuite-1.2.0.tar", last modified: Thu May 18 21:53:11 2023, max compression
```

## Comparing `virgoSuite-1.0.1.tar` & `virgoSuite-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:16:56.384766 virgoSuite-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-15 17:16:39.000000 virgoSuite-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-15 17:16:56.384766 virgoSuite-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-15 17:16:39.000000 virgoSuite-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 17:16:56.384766 virgoSuite-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-15 17:16:39.000000 virgoSuite-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:16:56.384766 virgoSuite-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:16:56.384766 virgoSuite-1.0.1/src/virgoSuite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 17:16:39.000000 virgoSuite-1.0.1/src/virgoSuite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24577 2023-05-15 17:16:39.000000 virgoSuite-1.0.1/src/virgoSuite/sfdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:16:56.384766 virgoSuite-1.0.1/src/virgoSuite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-15 17:16:56.000000 virgoSuite-1.0.1/src/virgoSuite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-15 17:16:56.000000 virgoSuite-1.0.1/src/virgoSuite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 17:16:56.000000 virgoSuite-1.0.1/src/virgoSuite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-15 17:16:56.000000 virgoSuite-1.0.1/src/virgoSuite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-15 17:16:56.000000 virgoSuite-1.0.1/src/virgoSuite.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:53:11.348264 virgoSuite-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-18 21:52:46.000000 virgoSuite-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-18 21:53:11.348264 virgoSuite-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-18 21:52:46.000000 virgoSuite-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 21:53:11.348264 virgoSuite-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-18 21:52:46.000000 virgoSuite-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:53:11.344264 virgoSuite-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:53:11.344264 virgoSuite-1.2.0/src/virgoSuite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:52:46.000000 virgoSuite-1.2.0/src/virgoSuite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24735 2023-05-18 21:52:46.000000 virgoSuite-1.2.0/src/virgoSuite/sfdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22319 2023-05-18 21:52:46.000000 virgoSuite-1.2.0/src/virgoSuite/sfdbV2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:53:11.348264 virgoSuite-1.2.0/src/virgoSuite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-18 21:53:11.000000 virgoSuite-1.2.0/src/virgoSuite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-18 21:53:11.000000 virgoSuite-1.2.0/src/virgoSuite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 21:53:11.000000 virgoSuite-1.2.0/src/virgoSuite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-18 21:53:11.000000 virgoSuite-1.2.0/src/virgoSuite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-18 21:53:11.000000 virgoSuite-1.2.0/src/virgoSuite.egg-info/top_level.txt
```

### Comparing `virgoSuite-1.0.1/LICENSE` & `virgoSuite-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `virgoSuite-1.0.1/setup.py` & `virgoSuite-1.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,15 +32,13 @@
     ],
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     install_requires=[
         "numpy",
         "scipy",
         "matplotlib",
-        "xarray",
         "pandas",
+        "h5py",
+        "dask",
         "astropy",
-        "zarr",
-        "tqdm",
-        "requests",
     ],
 )
```

### Comparing `virgoSuite-1.0.1/src/virgoSuite/sfdb.py` & `virgoSuite-1.2.0/src/virgoSuite/sfdb.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,24 +17,26 @@
 # http://grwavsf.roma1.infn.it/snag/Snag2_UG.pdf
 
 import numpy as np
 import pandas
 import astropy.time
 import xarray
 import zarr
+from dask import delayed
 
 import os
 
 from fnmatch import fnmatch
 from pathlib import Path
 from typing import TextIO
 
 import matplotlib.pyplot as plt
 from tqdm.contrib.telegram import tqdm, trange
 import string
+from dask.diagnostics import ProgressBar
 
 
 import random
 import string
 
 
 def get_random_string(length: int) -> str:
@@ -88,24 +90,24 @@
         return None
     elif n_elements == 1:
         out_variable = data_array[0]
     else:
         out_variable = data_array
 
     if (dt == "int") or (dt == "int32"):
-        return out_variable.astype("int64")
+        return out_variable.astype("int32")
     elif dt in ["float32", "double", "float", "float64", "single"]:
-        return out_variable.astype("double")
+        return out_variable.astype("float32")
 
 
 # =============================================================================
 # =============================================================================
 
 
-def read_block(fid: TextIO) -> list:
+def read_block(fid: TextIO) -> tuple[dict, np.ndarray, np.ndarray, np.ndarray]:
     """
     Read a block of FFTs
 
     `Snag <http://grwavsf.roma1.infn.it/snag/>`_ inspired function to read a
     block of FFTs from a SFDB file. The function will look for a list of values
     inside the file and will return them in an handy packed version.
 
@@ -213,21 +215,21 @@
     count = fread(fid, 1, "double")  # count
 
     if count is None:
         return None, None, None, None
 
     det = fread(fid, 1, "int32")  # detector
     if det == 0:
-        detector = "N"
+        detector = "Nautilus"
     elif det == 1:
-        detector = "V"
+        detector = "Virgo"
     elif det == 2:
-        detector = "H"
+        detector = "Hanford"
     elif det == 3:
-        detector = "L"
+        detector = "Livingston"
 
     gps_seconds = fread(fid, 1, "int32")  # gps_sec
     gps_nanoseconds = fread(fid, 1, "int32")  # gps_nsec
     gps_time = gps_seconds + gps_nanoseconds * 1e-9
 
     fft_lenght = fread(fid, 1, "double")  # tbase
     starting_fft_sample_index = fread(fid, 1, "int32")  # firstfrind
@@ -385,49 +387,46 @@
     )
     fft_data = _[0::2] + 1j * _[1::2]
 
     # Here is important to specify to export data as float, otherwise the
     # precision will not be enough
     return (
         header,
-        periodogram.astype("float64"),
-        autoregressive_spectrum.astype("float64"),
-        fft_data.astype("complex128"),
+        periodogram.astype("float32"),
+        autoregressive_spectrum.astype("float32"),
+        fft_data.astype("complex64"),
     )
 
 
 # =============================================================================
 # =============================================================================
 
 
 def load_file_sfdb(
     path_to_sfdb: str,
+    # -----Telegram Bot Notifications------
     telegram_notification: bool = False,
     token: str = "",
     chat_id: str = "",
-) -> pandas.DataFrame:
+    # -------------------------------------
+) -> list[xarray.Dataset]:
     """
     SFDB to netCDF4
 
     Contert SFDB files into netCDF4.
     netCDF4 is like hdf5 but hadles multidimensional data with more ease.
 
     Parameters
-    **********
-        path_to_sfdb : str
-            path to the file.
-        save_path : str
-            path to save folder
+    ----------
+    path_to_sfdb : str
+        path to the file.
+    save_path : str
+        path to save folder
 
     """
-
-    # SFDB files come with several attributes.
-    # We want to separate attributes, metadata and data to ensure readability
-    # and ease of use.
-
     with open(path_to_sfdb) as fid:
         if telegram_notification:
             _range = trange(
                 200,
                 token=token,
                 chat_id=chat_id,
             )
@@ -632,18 +631,18 @@
 # =============================================================================
 
 
 def convert_sfdb(
     path_to_sfdb: str,
     output_path: str,
     output_database_format: list = "all",
-    compression: bool = False,
     telegram_notifications: bool = False,
     token: str = "",
     chat_id: str = "",
+    compression: bool = False,
 ) -> None:
     # First we check whether a directory or a file are provided
     is_a_File = os.path.isfile(path_to_sfdb)
     is_a_directory = os.path.isdir(path_to_sfdb)
     if (not is_a_File) and (not is_a_directory):
         raise TypeError("Please check the path to the sfdb database.")
 
@@ -670,14 +669,15 @@
         file_list = [path_to_sfdb]
     elif is_a_directory:
         file_list = list_sfdb_in_directory(path_to_sfdb)
     if len(file_list) == 1:
         print(f"{len(file_list)} files was found.")
     elif len(file_list) > 1:
         print(f"{len(file_list)} files were found.")
+
     print(f"Starting conversion...")
 
     if telegram_notifications:
         file_list = tqdm(file_list, token=token, chat_id=chat_id)
 
     for file in file_list:
         print(f"Processing : {file}")
@@ -702,47 +702,50 @@
                 (save_format == "zarr")
                 or (save_format == "Zarr")
                 or (save_format == "ZARR")
             ):
                 print("Support for zarr has been haulted.")
                 print("Skipping.")
                 """
+
                 save_path = output_path + f"/DATABASE/zarr/fft_data.zarr"
                 save_path = zarr.storage.NestedDirectoryStore(
-                    path=save_path,
-                    dimension_separator="/",
+                    path=save_path, dimension_separator="/"
                 )
                 data.to_zarr(
                     save_path,
                     mode="w",
                 )
 
                 save_path = output_path + f"/DATABASE/zarr/spectrum.zarr"
                 save_path = zarr.storage.NestedDirectoryStore(
-                    path=save_path,
-                    dimension_separator="/",
+                    path=save_path, dimension_separator="/"
                 )
                 spectrum.to_zarr(
                     save_path,
                     mode="w",
                 )"""
 
             elif (
                 (save_format == "netCDF4")
                 or (save_format == "CDF4")
                 or (save_format == "netcdf")
             ):
                 print("Saving to netCDF4...")
+                # encoding = {"gzip": True, "complevel": 9}
+                # encoding = {"gzip": True, "compression_opts": 9}  # h5py
+
                 save_path = output_path + f"/DATABASE/netcdf/{run}/{calibration}/FFT/"
                 Path(save_path).mkdir(parents=True, exist_ok=True)
                 data.to_netcdf(
                     save_path + f"{get_random_string(15)}.netCDF4",
                     mode="w",
                     engine="netcdf4",
                 )
+
                 save_path = (
                     output_path + f"/DATABASE/netcdf/{run}/{calibration}/SPECTRUM/"
                 )
                 Path(save_path).mkdir(parents=True, exist_ok=True)
                 spectrum.to_netcdf(
                     save_path + f"{get_random_string(15)}.netCDF4",
                     mode="w",
```

