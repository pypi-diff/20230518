# Comparing `tmp/camerahub_tagger-0.5.0.tar.gz` & `tmp/camerahub_tagger-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camerahub_tagger-0.5.0.tar", max compression
+gzip compressed data, was "camerahub_tagger-0.6.0.tar", max compression
```

## Comparing `camerahub_tagger-0.5.0.tar` & `camerahub_tagger-0.6.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2908 2023-05-11 14:28:20.249401 camerahub_tagger-0.5.0/README.md
--rw-r--r--   0        0        0        0 2023-05-11 14:28:20.249401 camerahub_tagger-0.5.0/camerahub_tagger/__init__.py
--rw-r--r--   0        0        0     2628 2023-05-11 14:28:20.249401 camerahub_tagger-0.5.0/camerahub_tagger/api.py
--rw-r--r--   0        0        0     2037 2023-05-11 14:28:20.249401 camerahub_tagger-0.5.0/camerahub_tagger/config.py
--rw-r--r--   0        0        0     7204 2023-05-11 14:28:20.249401 camerahub_tagger-0.5.0/camerahub_tagger/funcs.py
--rwxr-xr-x   0        0        0     8988 2023-05-11 14:28:20.249401 camerahub_tagger-0.5.0/camerahub_tagger/main.py
--rw-r--r--   0        0        0      670 2023-05-11 14:28:41.697508 camerahub_tagger-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3676 1970-01-01 00:00:00.000000 camerahub_tagger-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     3033 2023-05-18 19:06:46.839850 camerahub_tagger-0.6.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-18 19:06:46.839850 camerahub_tagger-0.6.0/camerahub_tagger/__init__.py
+-rw-r--r--   0        0        0     2628 2023-05-18 19:06:46.839850 camerahub_tagger-0.6.0/camerahub_tagger/api.py
+-rw-r--r--   0        0        0     2037 2023-05-18 19:06:46.839850 camerahub_tagger-0.6.0/camerahub_tagger/config.py
+-rw-r--r--   0        0        0     7204 2023-05-18 19:06:46.839850 camerahub_tagger-0.6.0/camerahub_tagger/funcs.py
+-rwxr-xr-x   0        0        0     9297 2023-05-18 19:06:46.839850 camerahub_tagger-0.6.0/camerahub_tagger/main.py
+-rw-r--r--   0        0        0      670 2023-05-18 19:07:04.648115 camerahub_tagger-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3801 1970-01-01 00:00:00.000000 camerahub_tagger-0.6.0/PKG-INFO
```

### Comparing `camerahub_tagger-0.5.0/README.md` & `camerahub_tagger-0.6.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -48,14 +48,18 @@
 
 Accept all changes without confirmation
 
 ### `-d --dry-run`
 
 Don't write any tags to image files
 
+### `-d --update-only`
+
+Only update tags which have previously been written. Don't make any new Scan records in CameraHub.
+
 ### `-f --file FILE`
 
 Image file to be tagged. If not supplied, tag everything in the current directory.
 
 ### `-p --profile PROFILE`
 
 CameraHub connection profile. Default: `prod`.
@@ -87,8 +91,8 @@
 username = annieleibovitz
 password = johnandyoko
 
 [local]
 server = http://127.0.0.1:8000/api
 username = admin
 password = admin
-```
+```
```

### Comparing `camerahub_tagger-0.5.0/camerahub_tagger/api.py` & `camerahub_tagger-0.6.0/camerahub_tagger/api.py`

 * *Files identical despite different names*

### Comparing `camerahub_tagger-0.5.0/camerahub_tagger/config.py` & `camerahub_tagger-0.6.0/camerahub_tagger/config.py`

 * *Files identical despite different names*

### Comparing `camerahub_tagger-0.5.0/camerahub_tagger/funcs.py` & `camerahub_tagger-0.6.0/camerahub_tagger/funcs.py`

 * *Files identical despite different names*

### Comparing `camerahub_tagger-0.5.0/camerahub_tagger/main.py` & `camerahub_tagger-0.6.0/camerahub_tagger/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
     # Read in args
     parser = argparse.ArgumentParser()
     parser.add_argument('-r', '--recursive', help="Search for scans recursively", action='store_true')
     parser.add_argument('-a', '--auto', help="Don't prompt user to identify scans, only guess based on filename", action='store_true')
     parser.add_argument('-y', '--yes', help="Accept all changes without confirmation", action='store_true')
     parser.add_argument('-d', '--dry-run', help="Don't write any tags to image files", action='store_true')
+    parser.add_argument('-u', '--update-only', help="Only update tags which have previously been written", action='store_true')
     parser.add_argument('-c', '--clear', help="Clear existing EXIF metadata from the image file", action='store_true')
     parser.add_argument('-f', '--file', help="Image file to be tagged. If not supplied, tag everything in the current directory.", type=str)
     parser.add_argument('-p', '--profile', help="CameraHub connection profile", default='prod', type=str)
     args = parser.parse_args()
 
     # Determine path to config file
     home = os.path.expanduser("~")
@@ -118,14 +119,18 @@
         # existing = {'Exif.Image.DateTime': '2019:06:23 19:45:17', 'Exif.Image.Artist': 'TEST', 'Exif.Image.Rating': '4', ...}
 
         if existing is not None and 'Exif.Photo.ImageUniqueID' in existing and is_valid_uuid(existing['Exif.Photo.ImageUniqueID']):
             # check for presence of custom exif tag for camerahub
             # already has a uuid scan id
             print(f"{file} already has an EXIF scan ID")
             scan = existing['Exif.Photo.ImageUniqueID']
+        elif args.update_only:
+            print(f"{file} does not have an EXIF scan ID and --update-only is set, skipping")
+            unchanged.append(file)
+            continue
         else:
             # need to match it with a neg/print and generate a scan id
             print(f"{file} does not have an EXIF scan ID")
 
             # else prompt user to identify the scan
             #	guess film/frame from filename
             guess = guess_frame(file)
```

### Comparing `camerahub_tagger-0.5.0/pyproject.toml` & `camerahub_tagger-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "camerahub-tagger"
-version = "0.5.0"
+version = "0.6.0"
 description = "EXIF tagger for CameraHub"
 authors = ["Jonathan Gazeley <me@jonathangazeley.com>"]
 repository = "https://github.com/camerahub/tagger"
 homepage = "https://camerahub.info/"
 readme = ["README.md"]
 keywords = ["EXIF", "photography", "CameraHub", "metadata"]
```

### Comparing `camerahub_tagger-0.5.0/PKG-INFO` & `camerahub_tagger-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camerahub-tagger
-Version: 0.5.0
+Version: 0.6.0
 Summary: EXIF tagger for CameraHub
 Home-page: https://camerahub.info/
 Keywords: EXIF,photography,CameraHub,metadata
 Author: Jonathan Gazeley
 Author-email: me@jonathangazeley.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
@@ -69,14 +69,18 @@
 
 Accept all changes without confirmation
 
 ### `-d --dry-run`
 
 Don't write any tags to image files
 
+### `-d --update-only`
+
+Only update tags which have previously been written. Don't make any new Scan records in CameraHub.
+
 ### `-f --file FILE`
 
 Image file to be tagged. If not supplied, tag everything in the current directory.
 
 ### `-p --profile PROFILE`
 
 CameraHub connection profile. Default: `prod`.
@@ -109,7 +113,8 @@
 password = johnandyoko
 
 [local]
 server = http://127.0.0.1:8000/api
 username = admin
 password = admin
 ```
+
```

