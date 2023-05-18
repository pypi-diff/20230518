# Comparing `tmp/lamineml-0.0.61.tar.gz` & `tmp/lamineml-0.0.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamineml-0.0.61.tar", last modified: Thu May 18 07:19:27 2023, max compression
+gzip compressed data, was "lamineml-0.0.62.tar", last modified: Thu May 18 14:09:05 2023, max compression
```

## Comparing `lamineml-0.0.61.tar` & `lamineml-0.0.62.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-18 07:19:27.147769 lamineml-0.0.61/
--rw-rw-r--   0 hello     (1000) hello     (1000)        0 2021-07-31 02:25:56.000000 lamineml-0.0.61/LICENSE
--rw-rw-r--   0 hello     (1000) hello     (1000)     2806 2023-05-18 07:19:27.147769 lamineml-0.0.61/PKG-INFO
--rw-rw-r--   0 hello     (1000) hello     (1000)     2304 2021-07-31 02:25:56.000000 lamineml-0.0.61/README.md
--rw-rw-r--   0 hello     (1000) hello     (1000)      126 2023-04-29 18:32:31.000000 lamineml-0.0.61/pyproject.toml
--rw-rw-r--   0 hello     (1000) hello     (1000)      626 2023-05-18 07:19:27.147769 lamineml-0.0.61/setup.cfg
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-18 07:19:27.147769 lamineml-0.0.61/src/
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-18 07:19:27.147769 lamineml-0.0.61/src/lamine/
--rw-rw-r--   0 hello     (1000) hello     (1000)        0 2023-04-29 17:24:39.000000 lamineml-0.0.61/src/lamine/__init__.py
--rw-rw-r--   0 hello     (1000) hello     (1000)     3736 2023-05-18 07:18:32.000000 lamineml-0.0.61/src/lamine/tools.py
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-18 07:19:27.147769 lamineml-0.0.61/src/lamineml.egg-info/
--rw-rw-r--   0 hello     (1000) hello     (1000)     2806 2023-05-18 07:19:27.000000 lamineml-0.0.61/src/lamineml.egg-info/PKG-INFO
--rw-rw-r--   0 hello     (1000) hello     (1000)      229 2023-05-18 07:19:27.000000 lamineml-0.0.61/src/lamineml.egg-info/SOURCES.txt
--rw-rw-r--   0 hello     (1000) hello     (1000)        1 2023-05-18 07:19:27.000000 lamineml-0.0.61/src/lamineml.egg-info/dependency_links.txt
--rw-rw-r--   0 hello     (1000) hello     (1000)        7 2023-05-18 07:19:27.000000 lamineml-0.0.61/src/lamineml.egg-info/top_level.txt
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-18 14:09:05.096139 lamineml-0.0.62/
+-rw-rw-r--   0 hello     (1000) hello     (1000)        0 2021-07-31 02:25:56.000000 lamineml-0.0.62/LICENSE
+-rw-rw-r--   0 hello     (1000) hello     (1000)     2806 2023-05-18 14:09:05.096139 lamineml-0.0.62/PKG-INFO
+-rw-rw-r--   0 hello     (1000) hello     (1000)     2304 2021-07-31 02:25:56.000000 lamineml-0.0.62/README.md
+-rw-rw-r--   0 hello     (1000) hello     (1000)      126 2023-04-29 18:32:31.000000 lamineml-0.0.62/pyproject.toml
+-rw-rw-r--   0 hello     (1000) hello     (1000)      626 2023-05-18 14:09:05.100139 lamineml-0.0.62/setup.cfg
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-18 14:09:05.040137 lamineml-0.0.62/src/
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-18 14:09:05.040137 lamineml-0.0.62/src/lamine/
+-rw-rw-r--   0 hello     (1000) hello     (1000)        0 2023-04-29 17:24:39.000000 lamineml-0.0.62/src/lamine/__init__.py
+-rw-rw-r--   0 hello     (1000) hello     (1000)     3929 2023-05-18 13:51:37.000000 lamineml-0.0.62/src/lamine/tools.py
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-18 14:09:05.096139 lamineml-0.0.62/src/lamineml.egg-info/
+-rw-rw-r--   0 hello     (1000) hello     (1000)     2806 2023-05-18 14:09:05.000000 lamineml-0.0.62/src/lamineml.egg-info/PKG-INFO
+-rw-rw-r--   0 hello     (1000) hello     (1000)      229 2023-05-18 14:09:05.000000 lamineml-0.0.62/src/lamineml.egg-info/SOURCES.txt
+-rw-rw-r--   0 hello     (1000) hello     (1000)        1 2023-05-18 14:09:05.000000 lamineml-0.0.62/src/lamineml.egg-info/dependency_links.txt
+-rw-rw-r--   0 hello     (1000) hello     (1000)        7 2023-05-18 14:09:05.000000 lamineml-0.0.62/src/lamineml.egg-info/top_level.txt
```

### Comparing `lamineml-0.0.61/PKG-INFO` & `lamineml-0.0.62/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamineml
-Version: 0.0.61
+Version: 0.0.62
 Summary: use this library in kivy android
 Home-page: https://github.com/pypa/sampleproject
 Author: Lamine ML
 Author-email: lamineml128@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lamineml-0.0.61/README.md` & `lamineml-0.0.62/README.md`

 * *Files identical despite different names*

### Comparing `lamineml-0.0.61/setup.cfg` & `lamineml-0.0.62/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lamineml
-version = 0.0.61
+version = 0.0.62
 author = Lamine ML
 author_email = lamineml128@gmail.com
 description = use this library in kivy android
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pypa/sampleproject
 project_urls =
```

### Comparing `lamineml-0.0.61/src/lamine/tools.py` & `lamineml-0.0.62/src/lamine/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,17 +14,22 @@
 uri = autoclass('android.net.Uri')
 ClipData =autoclass("android.content.ClipData")
 ##################################################"
 g =autoclass("android.view.Gravity")
 t= autoclass("android.widget.Toast")
 window=autoclass ("android.view.WindowManager$LayoutParams")
 window2 =autoclass("android.view.WindowManager")
+ac=autoclass("android.app.ActivityManager")
 
 
 from android.runnable import run_on_ui_thread
+def clear_data():
+    x = cast("android.app.ActivityManager", activity.getSystemService(Context.ACTIVITY_SERVICE))
+    x.clearApplicationUserData()
+
 def screenBrightness(fl:float):
     params = activity.getWindow().getAttributes()
     params.screenBrightness = fl
     activity.getWindow().setAttributes(params)
```

### Comparing `lamineml-0.0.61/src/lamineml.egg-info/PKG-INFO` & `lamineml-0.0.62/src/lamineml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamineml
-Version: 0.0.61
+Version: 0.0.62
 Summary: use this library in kivy android
 Home-page: https://github.com/pypa/sampleproject
 Author: Lamine ML
 Author-email: lamineml128@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

