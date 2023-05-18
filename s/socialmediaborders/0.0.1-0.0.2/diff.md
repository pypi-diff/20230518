# Comparing `tmp/socialmediaborders-0.0.1.tar.gz` & `tmp/socialmediaborders-0.0.2.tar.gz`

## Comparing `socialmediaborders-0.0.1.tar` & `socialmediaborders-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 socialmediaborders-0.0.1/apple_automator/Add White Borders.workflow/Contents/Info.plist
--rw-r--r--   0        0        0     9675 2020-02-02 00:00:00.000000 socialmediaborders-0.0.1/apple_automator/Add White Borders.workflow/Contents/document.wflow
--rw-r--r--   0        0        0   152153 2020-02-02 00:00:00.000000 socialmediaborders-0.0.1/apple_automator/Add White Borders.workflow/Contents/QuickLook/Preview.png
--rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 socialmediaborders-0.0.1/apple_automator/Add White Borders.workflow/Contents/QuickLook/Thumbnail.png
--rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 socialmediaborders-0.0.1/apple_automator/Add White Borders.workflow/Contents/Resources/background.color
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 socialmediaborders-0.0.1/apple_automator/Contents/Info.plist
--rw-r--r--   0        0        0    10149 2020-02-02 00:00:00.000000 socialmediaborders-0.0.1/apple_automator/Contents/document.wflow
--rw-r--r--   0        0        0   180716 2020-02-02 00:00:00.000000 socialmediaborders-0.0.1/apple_automator/Contents/QuickLook/Preview.png
--rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 socialmediaborders-0.0.1/apple_automator/Contents/QuickLook/Thumbnail.png
--rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 socialmediaborders-0.0.1/apple_automator/Contents/Resources/background.color
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 socialmediaborders-0.0.1/src/socialmediaborders/__init__.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 socialmediaborders-0.0.1/src/socialmediaborders/__main__.py
--rwxr-xr-x   0        0        0     1649 2020-02-02 00:00:00.000000 socialmediaborders-0.0.1/src/socialmediaborders/create_borders.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 socialmediaborders-0.0.1/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 socialmediaborders-0.0.1/LICENCE.txt
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 socialmediaborders-0.0.1/README.md
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 socialmediaborders-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 socialmediaborders-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 socialmediaborders-0.0.2/apple_automator/Add White Borders.workflow/Contents/Info.plist
+-rw-r--r--   0        0        0     9675 2020-02-02 00:00:00.000000 socialmediaborders-0.0.2/apple_automator/Add White Borders.workflow/Contents/document.wflow
+-rw-r--r--   0        0        0   152153 2020-02-02 00:00:00.000000 socialmediaborders-0.0.2/apple_automator/Add White Borders.workflow/Contents/QuickLook/Preview.png
+-rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 socialmediaborders-0.0.2/apple_automator/Add White Borders.workflow/Contents/QuickLook/Thumbnail.png
+-rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 socialmediaborders-0.0.2/apple_automator/Add White Borders.workflow/Contents/Resources/background.color
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 socialmediaborders-0.0.2/apple_automator/Contents/Info.plist
+-rw-r--r--   0        0        0    10149 2020-02-02 00:00:00.000000 socialmediaborders-0.0.2/apple_automator/Contents/document.wflow
+-rw-r--r--   0        0        0   180716 2020-02-02 00:00:00.000000 socialmediaborders-0.0.2/apple_automator/Contents/QuickLook/Preview.png
+-rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 socialmediaborders-0.0.2/apple_automator/Contents/QuickLook/Thumbnail.png
+-rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 socialmediaborders-0.0.2/apple_automator/Contents/Resources/background.color
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 socialmediaborders-0.0.2/src/socialmediaborders/__init__.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 socialmediaborders-0.0.2/src/socialmediaborders/__main__.py
+-rwxr-xr-x   0        0        0     1649 2020-02-02 00:00:00.000000 socialmediaborders-0.0.2/src/socialmediaborders/create_borders.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 socialmediaborders-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 socialmediaborders-0.0.2/LICENCE.txt
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 socialmediaborders-0.0.2/README.md
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 socialmediaborders-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 socialmediaborders-0.0.2/PKG-INFO
```

### Comparing `socialmediaborders-0.0.1/apple_automator/Add White Borders.workflow/Contents/Info.plist` & `socialmediaborders-0.0.2/apple_automator/Add White Borders.workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `socialmediaborders-0.0.1/apple_automator/Add White Borders.workflow/Contents/document.wflow` & `socialmediaborders-0.0.2/apple_automator/Add White Borders.workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `socialmediaborders-0.0.1/apple_automator/Add White Borders.workflow/Contents/QuickLook/Preview.png` & `socialmediaborders-0.0.2/apple_automator/Add White Borders.workflow/Contents/QuickLook/Preview.png`

 * *Files identical despite different names*

### Comparing `socialmediaborders-0.0.1/apple_automator/Add White Borders.workflow/Contents/QuickLook/Thumbnail.png` & `socialmediaborders-0.0.2/apple_automator/Add White Borders.workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `socialmediaborders-0.0.1/apple_automator/Add White Borders.workflow/Contents/Resources/background.color` & `socialmediaborders-0.0.2/apple_automator/Add White Borders.workflow/Contents/Resources/background.color`

 * *Files identical despite different names*

### Comparing `socialmediaborders-0.0.1/apple_automator/Contents/Info.plist` & `socialmediaborders-0.0.2/apple_automator/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `socialmediaborders-0.0.1/apple_automator/Contents/document.wflow` & `socialmediaborders-0.0.2/apple_automator/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `socialmediaborders-0.0.1/apple_automator/Contents/QuickLook/Preview.png` & `socialmediaborders-0.0.2/apple_automator/Contents/QuickLook/Preview.png`

 * *Files identical despite different names*

### Comparing `socialmediaborders-0.0.1/apple_automator/Contents/QuickLook/Thumbnail.png` & `socialmediaborders-0.0.2/apple_automator/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `socialmediaborders-0.0.1/apple_automator/Contents/Resources/background.color` & `socialmediaborders-0.0.2/apple_automator/Contents/Resources/background.color`

 * *Files identical despite different names*

### Comparing `socialmediaborders-0.0.1/src/socialmediaborders/__main__.py` & `socialmediaborders-0.0.2/src/socialmediaborders/__main__.py`

 * *Files identical despite different names*

### Comparing `socialmediaborders-0.0.1/src/socialmediaborders/create_borders.py` & `socialmediaborders-0.0.2/src/socialmediaborders/create_borders.py`

 * *Files identical despite different names*

### Comparing `socialmediaborders-0.0.1/LICENCE.txt` & `socialmediaborders-0.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `socialmediaborders-0.0.1/README.md` & `socialmediaborders-0.0.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Social Media Borders
 
 Adding colored borders to pictures for social media to bring them to a 1:1 format.
 
 ```
-usage: social_media_borders.py [-h] [-c COLOR] [-bp BORDERPERCENTAGE] [-o | --keepOriginal | --no-keepOriginal] path
+usage: socialmediaborders [-h] [-c COLOR] [-bp BORDERPERCENTAGE] [-k | --keepOriginal | --no-keepOriginal] path
 
 Adding colored borders to pictures for social media to bring them to a 1:1 format.
 
 positional arguments:
   path                  the path to the image
 
 optional arguments:
```

### Comparing `socialmediaborders-0.0.1/pyproject.toml` & `socialmediaborders-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 [project]
 name = "socialmediaborders"
-version = "0.0.1"
+version = "0.0.2"
 description = "Adding colored borders to pictures for social media to bring them to a 1:1 format."
 readme = "README.md"
 requires-python = ">=3.9"
-license = { file = "LICENCE.txt" }
+license = "MIT"
 authors = [{ name = "Alexander Giagoulas", email = "alexander@giagoulas.com" }]
-maintainers = [
-    { name = "Alexander Giagoulas", email = "alexander@giagoulas.com" },
-]
 classifiers = [
     "Programming Language :: Python :: 3.9",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-dependencies = ["filetype", "Pillow", "urllib3==1.26.6"]
+dependencies = ["filetype", "Pillow"]
 
 [project.urls]
 "Creator Links" = "https://giagoulas.com/links"
 
 [project.scripts]
 socialmediaborders = "socialmediaborders:__main__.main"
```

