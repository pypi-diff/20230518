# Comparing `tmp/pystripe-1.2.5.tar.gz` & `tmp/pystripe-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pystripe-1.2.5.tar", last modified: Thu May 18 17:33:32 2023, max compression
+gzip compressed data, was "dist\pystripe-1.2.6.tar", last modified: Thu May 18 17:45:33 2023, max compression
```

## Comparing `pystripe-1.2.5.tar` & `pystripe-1.2.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 17:33:32.000000 pystripe-1.2.5/
--rw-rw-rw-   0        0        0     1087 2023-04-27 18:51:02.000000 pystripe-1.2.5/LICENSE
--rw-rw-rw-   0        0        0     5302 2023-05-18 17:33:32.000000 pystripe-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     4922 2023-04-27 18:51:02.000000 pystripe-1.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 17:33:32.000000 pystripe-1.2.5/pystripe/
--rw-rw-rw-   0        0        0      327 2023-04-27 18:51:02.000000 pystripe-1.2.5/pystripe/__init__.py
--rw-rw-rw-   0        0        0    36596 2023-05-18 17:32:45.000000 pystripe-1.2.5/pystripe/core.py
--rw-rw-rw-   0        0        0    10929 2023-04-27 18:51:02.000000 pystripe-1.2.5/pystripe/lightsheet_correct.py
--rw-rw-rw-   0        0        0     1668 2023-04-27 18:51:02.000000 pystripe-1.2.5/pystripe/raw.py
-drwxrwxrwx   0        0        0        0 2023-05-18 17:33:32.000000 pystripe-1.2.5/pystripe.egg-info/
--rw-rw-rw-   0        0        0     5302 2023-05-18 17:33:31.000000 pystripe-1.2.5/pystripe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2023-05-18 17:33:32.000000 pystripe-1.2.5/pystripe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 17:33:31.000000 pystripe-1.2.5/pystripe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-18 17:33:31.000000 pystripe-1.2.5/pystripe.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      139 2023-05-18 17:33:32.000000 pystripe-1.2.5/pystripe.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-18 17:33:32.000000 pystripe-1.2.5/pystripe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 17:33:32.000000 pystripe-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0      979 2023-05-18 17:32:50.000000 pystripe-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 17:45:33.000000 pystripe-1.2.6/
+-rw-rw-rw-   0        0        0     1087 2023-04-27 18:51:02.000000 pystripe-1.2.6/LICENSE
+-rw-rw-rw-   0        0        0     5302 2023-05-18 17:45:33.000000 pystripe-1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4922 2023-04-27 18:51:02.000000 pystripe-1.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 17:45:33.000000 pystripe-1.2.6/pystripe/
+-rw-rw-rw-   0        0        0      327 2023-04-27 18:51:02.000000 pystripe-1.2.6/pystripe/__init__.py
+-rw-rw-rw-   0        0        0    36740 2023-05-18 17:44:43.000000 pystripe-1.2.6/pystripe/core.py
+-rw-rw-rw-   0        0        0    10929 2023-04-27 18:51:02.000000 pystripe-1.2.6/pystripe/lightsheet_correct.py
+-rw-rw-rw-   0        0        0     1668 2023-04-27 18:51:02.000000 pystripe-1.2.6/pystripe/raw.py
+drwxrwxrwx   0        0        0        0 2023-05-18 17:45:33.000000 pystripe-1.2.6/pystripe.egg-info/
+-rw-rw-rw-   0        0        0     5302 2023-05-18 17:45:32.000000 pystripe-1.2.6/pystripe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2023-05-18 17:45:32.000000 pystripe-1.2.6/pystripe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 17:45:32.000000 pystripe-1.2.6/pystripe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-18 17:45:32.000000 pystripe-1.2.6/pystripe.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      139 2023-05-18 17:45:32.000000 pystripe-1.2.6/pystripe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-18 17:45:32.000000 pystripe-1.2.6/pystripe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 17:45:33.000000 pystripe-1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      979 2023-05-18 17:44:48.000000 pystripe-1.2.6/setup.py
```

### Comparing `pystripe-1.2.5/LICENSE` & `pystripe-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pystripe-1.2.5/PKG-INFO` & `pystripe-1.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystripe
-Version: 1.2.5
+Version: 1.2.6
 Summary: Stripe artifact filtering for SPIM images
 Home-page: https://github.com/LifeCanvas-Technologies/pystripe
 Author: LifeCanvas Technologies
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
```

### Comparing `pystripe-1.2.5/README.md` & `pystripe-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `pystripe-1.2.5/pystripe/core.py` & `pystripe-1.2.6/pystripe/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -405,14 +405,17 @@
         coeffs_filt.append((ch_filt, cv, cd))
 
     img_log_filtered = waverec(coeffs_filt, wavelet)
     return np.exp(img_log_filtered)-1
 
 
 def apply_flat(img, flat):
+    pady, padx = [_ % 2 for _ in flat.shape]
+    if pady == 1 or padx == 1:
+        flat = np.pad(flat, ((0, pady), (0, padx)), mode="edge")
     return (img / flat).astype(img.dtype)
 
 
 def filter_streaks(img, sigma, level=0, wavelet='db3', crossover=10, threshold=-1, flat=None, dark=0):
     """Filter horizontal streaks using wavelet-FFT filter
 
     Parameters
```

### Comparing `pystripe-1.2.5/pystripe/lightsheet_correct.py` & `pystripe-1.2.6/pystripe/lightsheet_correct.py`

 * *Files identical despite different names*

### Comparing `pystripe-1.2.5/pystripe/raw.py` & `pystripe-1.2.6/pystripe/raw.py`

 * *Files identical despite different names*

### Comparing `pystripe-1.2.5/pystripe.egg-info/PKG-INFO` & `pystripe-1.2.6/pystripe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystripe
-Version: 1.2.5
+Version: 1.2.6
 Summary: Stripe artifact filtering for SPIM images
 Home-page: https://github.com/LifeCanvas-Technologies/pystripe
 Author: LifeCanvas Technologies
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
```

### Comparing `pystripe-1.2.5/setup.py` & `pystripe-1.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = "1.2.5"
+version = "1.2.6"
 
 with open("./README.md") as fd:
     long_description = fd.read()
 
 setup(
     name="pystripe",
     version=version,
```

