# Comparing `tmp/pystripe-1.2.3.tar.gz` & `tmp/pystripe-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pystripe-1.2.3.tar", last modified: Thu Apr 27 18:52:20 2023, max compression
+gzip compressed data, was "dist\pystripe-1.2.4.tar", last modified: Thu May 18 17:30:09 2023, max compression
```

## Comparing `pystripe-1.2.3.tar` & `pystripe-1.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 18:52:20.000000 pystripe-1.2.3/
--rw-rw-rw-   0        0        0     1087 2023-04-27 18:51:02.000000 pystripe-1.2.3/LICENSE
--rw-rw-rw-   0        0        0     5302 2023-04-27 18:52:20.000000 pystripe-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     4922 2023-04-27 18:51:02.000000 pystripe-1.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 18:52:20.000000 pystripe-1.2.3/pystripe/
--rw-rw-rw-   0        0        0      327 2023-04-27 18:51:02.000000 pystripe-1.2.3/pystripe/__init__.py
--rw-rw-rw-   0        0        0    36593 2023-04-27 18:51:02.000000 pystripe-1.2.3/pystripe/core.py
--rw-rw-rw-   0        0        0    10929 2023-04-27 18:51:02.000000 pystripe-1.2.3/pystripe/lightsheet_correct.py
--rw-rw-rw-   0        0        0     1668 2023-04-27 18:51:02.000000 pystripe-1.2.3/pystripe/raw.py
-drwxrwxrwx   0        0        0        0 2023-04-27 18:52:20.000000 pystripe-1.2.3/pystripe.egg-info/
--rw-rw-rw-   0        0        0     5302 2023-04-27 18:52:19.000000 pystripe-1.2.3/pystripe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2023-04-27 18:52:20.000000 pystripe-1.2.3/pystripe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 18:52:19.000000 pystripe-1.2.3/pystripe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-27 18:52:19.000000 pystripe-1.2.3/pystripe.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      139 2023-04-27 18:52:19.000000 pystripe-1.2.3/pystripe.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-27 18:52:19.000000 pystripe-1.2.3/pystripe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 18:52:20.000000 pystripe-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0      979 2023-04-27 18:51:02.000000 pystripe-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 17:30:09.000000 pystripe-1.2.4/
+-rw-rw-rw-   0        0        0     1087 2023-04-27 18:51:02.000000 pystripe-1.2.4/LICENSE
+-rw-rw-rw-   0        0        0     5302 2023-05-18 17:30:09.000000 pystripe-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4922 2023-04-27 18:51:02.000000 pystripe-1.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 17:30:09.000000 pystripe-1.2.4/pystripe/
+-rw-rw-rw-   0        0        0      327 2023-04-27 18:51:02.000000 pystripe-1.2.4/pystripe/__init__.py
+-rw-rw-rw-   0        0        0    36595 2023-05-18 17:08:13.000000 pystripe-1.2.4/pystripe/core.py
+-rw-rw-rw-   0        0        0    10929 2023-04-27 18:51:02.000000 pystripe-1.2.4/pystripe/lightsheet_correct.py
+-rw-rw-rw-   0        0        0     1668 2023-04-27 18:51:02.000000 pystripe-1.2.4/pystripe/raw.py
+drwxrwxrwx   0        0        0        0 2023-05-18 17:30:09.000000 pystripe-1.2.4/pystripe.egg-info/
+-rw-rw-rw-   0        0        0     5302 2023-05-18 17:30:08.000000 pystripe-1.2.4/pystripe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2023-05-18 17:30:09.000000 pystripe-1.2.4/pystripe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 17:30:08.000000 pystripe-1.2.4/pystripe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-18 17:30:09.000000 pystripe-1.2.4/pystripe.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      139 2023-05-18 17:30:09.000000 pystripe-1.2.4/pystripe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-18 17:30:09.000000 pystripe-1.2.4/pystripe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 17:30:09.000000 pystripe-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      979 2023-05-18 17:28:44.000000 pystripe-1.2.4/setup.py
```

### Comparing `pystripe-1.2.3/LICENSE` & `pystripe-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pystripe-1.2.3/PKG-INFO` & `pystripe-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystripe
-Version: 1.2.3
+Version: 1.2.4
 Summary: Stripe artifact filtering for SPIM images
 Home-page: https://github.com/LifeCanvas-Technologies/pystripe
 Author: LifeCanvas Technologies
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
```

### Comparing `pystripe-1.2.3/README.md` & `pystripe-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pystripe-1.2.3/pystripe/core.py` & `pystripe-1.2.4/pystripe/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -868,15 +868,15 @@
     parser.add_argument("--rotate", "-r", help="Rotate output images 90 degrees counter-clockwise", action='store_true')
     parser.add_argument("--lightsheet", help="Use the lightsheet method", action="store_true")
     parser.add_argument("--artifact-length", help="Look for minimum in lightsheet direction over this length", default=150, type=int)
     parser.add_argument("--background-window-size", help="Size of window in x and y for background estimation", default=200, type=int)
     parser.add_argument("--percentile", help="The percentile at which to measure the background", type=float, default=.25)
     parser.add_argument("--lightsheet-vs-background", help="The background is multiplied by this weight when comparing lightsheet against background", type=float, default=2.0)
     parser.add_argument("--dont-convert-16bit", help="Is the output converted to 16-bit .tiff or not", action="store_true")
-    parser.add_argument("--output_format", "-of", help="Desired format output for the images", type=str, required=False, default=None)
+    parser.add_argument("--output_format", "-of", help="Desired format output for the images", type=str, required=False, default="tiff")
     args = parser.parse_args()
     return args
 
 
 def interpolate(image_path, input_path, output_path):
     # print('Interpolate:\nimage_path: {}\ninput_path: {}\noutput_path: {}\n'.format(image_path, input_path, output_path))
     rel_path = Path(image_path).relative_to(input_path)
```

### Comparing `pystripe-1.2.3/pystripe/lightsheet_correct.py` & `pystripe-1.2.4/pystripe/lightsheet_correct.py`

 * *Files identical despite different names*

### Comparing `pystripe-1.2.3/pystripe/raw.py` & `pystripe-1.2.4/pystripe/raw.py`

 * *Files identical despite different names*

### Comparing `pystripe-1.2.3/pystripe.egg-info/PKG-INFO` & `pystripe-1.2.4/pystripe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystripe
-Version: 1.2.3
+Version: 1.2.4
 Summary: Stripe artifact filtering for SPIM images
 Home-page: https://github.com/LifeCanvas-Technologies/pystripe
 Author: LifeCanvas Technologies
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
```

### Comparing `pystripe-1.2.3/setup.py` & `pystripe-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = "1.2.3"
+version = "1.2.4"
 
 with open("./README.md") as fd:
     long_description = fd.read()
 
 setup(
     name="pystripe",
     version=version,
```

