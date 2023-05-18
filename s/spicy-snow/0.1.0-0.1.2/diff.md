# Comparing `tmp/spicy-snow-0.1.0.tar.gz` & `tmp/spicy-snow-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spicy-snow-0.1.0.tar", last modified: Wed May 17 18:49:46 2023, max compression
+gzip compressed data, was "spicy-snow-0.1.2.tar", last modified: Wed May 17 19:21:37 2023, max compression
```

## Comparing `spicy-snow-0.1.0.tar` & `spicy-snow-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:49:46.611893 spicy-snow-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-17 18:49:32.000000 spicy-snow-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-05-17 18:49:46.611893 spicy-snow-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-05-17 18:49:32.000000 spicy-snow-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-17 18:49:32.000000 spicy-snow-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 18:49:46.611893 spicy-snow-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-05-17 18:49:33.000000 spicy-snow-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:49:46.611893 spicy-snow-0.1.0/spicy_snow/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-17 18:49:32.000000 spicy-snow-0.1.0/spicy_snow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-05-17 18:49:32.000000 spicy-snow-0.1.0/spicy_snow/retrieval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:49:46.611893 spicy-snow-0.1.0/spicy_snow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-05-17 18:49:46.000000 spicy-snow-0.1.0/spicy_snow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-17 18:49:46.000000 spicy-snow-0.1.0/spicy_snow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 18:49:46.000000 spicy-snow-0.1.0/spicy_snow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-17 18:49:46.000000 spicy-snow-0.1.0/spicy_snow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-17 18:49:46.000000 spicy-snow-0.1.0/spicy_snow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:49:46.611893 spicy-snow-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-17 18:49:32.000000 spicy-snow-0.1.0/tests/test_IO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-05-17 18:49:32.000000 spicy-snow-0.1.0/tests/test_downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)    11456 2023-05-17 18:49:32.000000 spicy-snow-0.1.0/tests/test_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    22511 2023-05-17 18:49:32.000000 spicy-snow-0.1.0/tests/test_snow_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    23142 2023-05-17 18:49:32.000000 spicy-snow-0.1.0/tests/test_wetsnow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:37.403977 spicy-snow-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-17 19:21:19.000000 spicy-snow-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-05-17 19:21:37.403977 spicy-snow-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-05-17 19:21:19.000000 spicy-snow-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-17 19:21:19.000000 spicy-snow-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 19:21:37.403977 spicy-snow-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-05-17 19:21:20.000000 spicy-snow-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:37.399977 spicy-snow-0.1.2/spicy_snow/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-17 19:21:19.000000 spicy-snow-0.1.2/spicy_snow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-05-17 19:21:19.000000 spicy-snow-0.1.2/spicy_snow/retrieval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:37.403977 spicy-snow-0.1.2/spicy_snow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-05-17 19:21:37.000000 spicy-snow-0.1.2/spicy_snow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-17 19:21:37.000000 spicy-snow-0.1.2/spicy_snow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 19:21:37.000000 spicy-snow-0.1.2/spicy_snow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-17 19:21:37.000000 spicy-snow-0.1.2/spicy_snow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-17 19:21:37.000000 spicy-snow-0.1.2/spicy_snow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:37.403977 spicy-snow-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-17 19:21:19.000000 spicy-snow-0.1.2/tests/test_IO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-05-17 19:21:20.000000 spicy-snow-0.1.2/tests/test_downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11456 2023-05-17 19:21:20.000000 spicy-snow-0.1.2/tests/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22511 2023-05-17 19:21:20.000000 spicy-snow-0.1.2/tests/test_snow_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23142 2023-05-17 19:21:20.000000 spicy-snow-0.1.2/tests/test_wetsnow.py
```

### Comparing `spicy-snow-0.1.0/LICENSE` & `spicy-snow-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spicy-snow-0.1.0/PKG-INFO` & `spicy-snow-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spicy-snow
-Version: 0.1.0
+Version: 0.1.2
 Summary: Snow Depth Retrievals from Sentinel-1 Backscatter.
 Home-page: https://github.com/SnowEx/spicy-snow
 Author: Zach Keskinen
 Author-email: zachkeskinen@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -33,18 +33,15 @@
 Lievens et al 2021 - https://tc.copernicus.org/articles/16/159/2022/
 
 <img src="https://github.com/SnowEx/spicy-snow/blob/main/title-img.png" width="800">
 
 ## Example Installation
 
 ```sh
-# pip install to come! Please just add this directory to your path for now.
-# see https://stackoverflow.com/questions/32715261/how-to-add-folder-to-search-path-for-a-given-anaconda-environment
-# for instructions - be sure to conda install conda-build before running command.
-pip install c_snow
+pip install spicy-snow
 ```
 
 ## Example usage:
 
 ```python
 from pathlib import Path
 
@@ -54,14 +51,15 @@
 
 from spicy_snow.retrieval import retrieve_snow_depth
 from spicy_snow.IO.user_dates import get_input_dates
 
 # change to your minimum longitude, min lat, max long, max lat
 area = shapely.geometry.box(-113.2, 43, -113, 43.4)
 
+# this will be where your results are saved
 out_nc = Path('~/Desktop/spicy-test/test.nc').expanduser()
 
 # this will generate a tuple of dates from the previous August 1st to this date
 dates = get_input_dates('2021-04-01') # run on all s1 images from (2020-08-01, 2021-04-01) in this example
 
 spicy_ds = retrieve_snow_depth(area = area, dates = dates, 
                                work_dir = Path('~/Desktop/spicy-test/').expanduser(),
```

### Comparing `spicy-snow-0.1.0/README.md` & `spicy-snow-0.1.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -14,18 +14,15 @@
 Lievens et al 2021 - https://tc.copernicus.org/articles/16/159/2022/
 
 <img src="https://github.com/SnowEx/spicy-snow/blob/main/title-img.png" width="800">
 
 ## Example Installation
 
 ```sh
-# pip install to come! Please just add this directory to your path for now.
-# see https://stackoverflow.com/questions/32715261/how-to-add-folder-to-search-path-for-a-given-anaconda-environment
-# for instructions - be sure to conda install conda-build before running command.
-pip install c_snow
+pip install spicy-snow
 ```
 
 ## Example usage:
 
 ```python
 from pathlib import Path
 
@@ -35,14 +32,15 @@
 
 from spicy_snow.retrieval import retrieve_snow_depth
 from spicy_snow.IO.user_dates import get_input_dates
 
 # change to your minimum longitude, min lat, max long, max lat
 area = shapely.geometry.box(-113.2, 43, -113, 43.4)
 
+# this will be where your results are saved
 out_nc = Path('~/Desktop/spicy-test/test.nc').expanduser()
 
 # this will generate a tuple of dates from the previous August 1st to this date
 dates = get_input_dates('2021-04-01') # run on all s1 images from (2020-08-01, 2021-04-01) in this example
 
 spicy_ds = retrieve_snow_depth(area = area, dates = dates, 
                                work_dir = Path('~/Desktop/spicy-test/').expanduser(),
```

### Comparing `spicy-snow-0.1.0/setup.py` & `spicy-snow-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 
         sys.exit()
 
 
 # Where the magic happens:
 setup(
     name=NAME,
-    version='0.1.0', # change to value if not using github auto upload
+    version='0.1.2', # change to value if not using github auto upload
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
```

### Comparing `spicy-snow-0.1.0/spicy_snow/retrieval.py` & `spicy-snow-0.1.2/spicy_snow/retrieval.py`

 * *Files identical despite different names*

### Comparing `spicy-snow-0.1.0/spicy_snow.egg-info/PKG-INFO` & `spicy-snow-0.1.2/spicy_snow.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spicy-snow
-Version: 0.1.0
+Version: 0.1.2
 Summary: Snow Depth Retrievals from Sentinel-1 Backscatter.
 Home-page: https://github.com/SnowEx/spicy-snow
 Author: Zach Keskinen
 Author-email: zachkeskinen@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -33,18 +33,15 @@
 Lievens et al 2021 - https://tc.copernicus.org/articles/16/159/2022/
 
 <img src="https://github.com/SnowEx/spicy-snow/blob/main/title-img.png" width="800">
 
 ## Example Installation
 
 ```sh
-# pip install to come! Please just add this directory to your path for now.
-# see https://stackoverflow.com/questions/32715261/how-to-add-folder-to-search-path-for-a-given-anaconda-environment
-# for instructions - be sure to conda install conda-build before running command.
-pip install c_snow
+pip install spicy-snow
 ```
 
 ## Example usage:
 
 ```python
 from pathlib import Path
 
@@ -54,14 +51,15 @@
 
 from spicy_snow.retrieval import retrieve_snow_depth
 from spicy_snow.IO.user_dates import get_input_dates
 
 # change to your minimum longitude, min lat, max long, max lat
 area = shapely.geometry.box(-113.2, 43, -113, 43.4)
 
+# this will be where your results are saved
 out_nc = Path('~/Desktop/spicy-test/test.nc').expanduser()
 
 # this will generate a tuple of dates from the previous August 1st to this date
 dates = get_input_dates('2021-04-01') # run on all s1 images from (2020-08-01, 2021-04-01) in this example
 
 spicy_ds = retrieve_snow_depth(area = area, dates = dates, 
                                work_dir = Path('~/Desktop/spicy-test/').expanduser(),
```

### Comparing `spicy-snow-0.1.0/tests/test_IO.py` & `spicy-snow-0.1.2/tests/test_IO.py`

 * *Files identical despite different names*

### Comparing `spicy-snow-0.1.0/tests/test_downloads.py` & `spicy-snow-0.1.2/tests/test_downloads.py`

 * *Files identical despite different names*

### Comparing `spicy-snow-0.1.0/tests/test_preprocessing.py` & `spicy-snow-0.1.2/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `spicy-snow-0.1.0/tests/test_snow_index.py` & `spicy-snow-0.1.2/tests/test_snow_index.py`

 * *Files identical despite different names*

### Comparing `spicy-snow-0.1.0/tests/test_wetsnow.py` & `spicy-snow-0.1.2/tests/test_wetsnow.py`

 * *Files identical despite different names*

