# Comparing `tmp/pystripe-1.2.6.tar.gz` & `tmp/pystripe-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pystripe-1.2.6.tar", last modified: Thu May 18 17:45:33 2023, max compression
+gzip compressed data, was "dist\pystripe-1.2.7.tar", last modified: Thu May 18 18:08:01 2023, max compression
```

## Comparing `pystripe-1.2.6.tar` & `pystripe-1.2.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 17:45:33.000000 pystripe-1.2.6/
--rw-rw-rw-   0        0        0     1087 2023-04-27 18:51:02.000000 pystripe-1.2.6/LICENSE
--rw-rw-rw-   0        0        0     5302 2023-05-18 17:45:33.000000 pystripe-1.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     4922 2023-04-27 18:51:02.000000 pystripe-1.2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 17:45:33.000000 pystripe-1.2.6/pystripe/
--rw-rw-rw-   0        0        0      327 2023-04-27 18:51:02.000000 pystripe-1.2.6/pystripe/__init__.py
--rw-rw-rw-   0        0        0    36740 2023-05-18 17:44:43.000000 pystripe-1.2.6/pystripe/core.py
--rw-rw-rw-   0        0        0    10929 2023-04-27 18:51:02.000000 pystripe-1.2.6/pystripe/lightsheet_correct.py
--rw-rw-rw-   0        0        0     1668 2023-04-27 18:51:02.000000 pystripe-1.2.6/pystripe/raw.py
-drwxrwxrwx   0        0        0        0 2023-05-18 17:45:33.000000 pystripe-1.2.6/pystripe.egg-info/
--rw-rw-rw-   0        0        0     5302 2023-05-18 17:45:32.000000 pystripe-1.2.6/pystripe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2023-05-18 17:45:32.000000 pystripe-1.2.6/pystripe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 17:45:32.000000 pystripe-1.2.6/pystripe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-18 17:45:32.000000 pystripe-1.2.6/pystripe.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      139 2023-05-18 17:45:32.000000 pystripe-1.2.6/pystripe.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-18 17:45:32.000000 pystripe-1.2.6/pystripe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 17:45:33.000000 pystripe-1.2.6/setup.cfg
--rw-rw-rw-   0        0        0      979 2023-05-18 17:44:48.000000 pystripe-1.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:08:01.000000 pystripe-1.2.7/
+-rw-rw-rw-   0        0        0     1087 2023-04-27 18:51:02.000000 pystripe-1.2.7/LICENSE
+-rw-rw-rw-   0        0        0     5302 2023-05-18 18:08:01.000000 pystripe-1.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4922 2023-04-27 18:51:02.000000 pystripe-1.2.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 18:08:01.000000 pystripe-1.2.7/pystripe/
+-rw-rw-rw-   0        0        0      327 2023-04-27 18:51:02.000000 pystripe-1.2.7/pystripe/__init__.py
+-rw-rw-rw-   0        0        0    36761 2023-05-18 18:07:27.000000 pystripe-1.2.7/pystripe/core.py
+-rw-rw-rw-   0        0        0    10929 2023-04-27 18:51:02.000000 pystripe-1.2.7/pystripe/lightsheet_correct.py
+-rw-rw-rw-   0        0        0     1668 2023-04-27 18:51:02.000000 pystripe-1.2.7/pystripe/raw.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:08:01.000000 pystripe-1.2.7/pystripe.egg-info/
+-rw-rw-rw-   0        0        0     5302 2023-05-18 18:08:00.000000 pystripe-1.2.7/pystripe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2023-05-18 18:08:01.000000 pystripe-1.2.7/pystripe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 18:08:00.000000 pystripe-1.2.7/pystripe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-18 18:08:01.000000 pystripe-1.2.7/pystripe.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      139 2023-05-18 18:08:01.000000 pystripe-1.2.7/pystripe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-18 18:08:01.000000 pystripe-1.2.7/pystripe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 18:08:01.000000 pystripe-1.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      979 2023-05-18 18:07:43.000000 pystripe-1.2.7/setup.py
```

### Comparing `pystripe-1.2.6/LICENSE` & `pystripe-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pystripe-1.2.6/PKG-INFO` & `pystripe-1.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystripe
-Version: 1.2.6
+Version: 1.2.7
 Summary: Stripe artifact filtering for SPIM images
 Home-page: https://github.com/LifeCanvas-Technologies/pystripe
 Author: LifeCanvas Technologies
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
```

### Comparing `pystripe-1.2.6/README.md` & `pystripe-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `pystripe-1.2.6/pystripe/core.py` & `pystripe-1.2.7/pystripe/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -584,15 +584,15 @@
                     dtype = np.uint16
             else:
                 # Path must be to DCIMG file
                 assert str(input_path).endswith('.dcimg')
                 img = imread_dcimg(str(input_path), z_idx)
                 dtype = np.uint16
         except:
-            if i == n -1:
+            if i == n -1 and output_root_dir != None:
                 file_name = os.path.join(output_root_dir, 'destripe_log.txt')
                 if not os.path.exists(file_name):
                     error_file = open(file_name, 'w')
                     error_file.write('Error reading the following images.  Pystripe will interpolate their content.')
                     error_file.close()
                 error_file = open(file_name, 'a+')
                 error_file.write('\n{}'.format(str(input_path)))
@@ -938,15 +938,15 @@
             print('Input file was found but is not supported. Exiting...')
             return
         if args.output == '':
             output_path = Path(input_path.parent).joinpath(input_path.stem+'_destriped'+input_path.suffix)
         else:
             output_path = Path(args.output)
             assert output_path.suffix in supported_extensions
-        output_root_dir = output_path
+        output_root_dir = None
         
         read_filter_save(output_root_dir,
                          input_path,
                          output_path,
                          sigma=sigma,
                          level=args.level,
                          wavelet=args.wavelet,
```

### Comparing `pystripe-1.2.6/pystripe/lightsheet_correct.py` & `pystripe-1.2.7/pystripe/lightsheet_correct.py`

 * *Files identical despite different names*

### Comparing `pystripe-1.2.6/pystripe/raw.py` & `pystripe-1.2.7/pystripe/raw.py`

 * *Files identical despite different names*

### Comparing `pystripe-1.2.6/pystripe.egg-info/PKG-INFO` & `pystripe-1.2.7/pystripe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystripe
-Version: 1.2.6
+Version: 1.2.7
 Summary: Stripe artifact filtering for SPIM images
 Home-page: https://github.com/LifeCanvas-Technologies/pystripe
 Author: LifeCanvas Technologies
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
```

### Comparing `pystripe-1.2.6/setup.py` & `pystripe-1.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = "1.2.6"
+version = "1.2.7"
 
 with open("./README.md") as fd:
     long_description = fd.read()
 
 setup(
     name="pystripe",
     version=version,
```

