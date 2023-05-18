# Comparing `tmp/flask_captcha2-0.0.0.tar.gz` & `tmp/flask_captcha2-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\flask_captcha2-0.0.0.tar", last modified: Thu May 18 05:10:26 2023, max compression
+gzip compressed data, was "dist\flask_captcha2-0.1.0.tar", last modified: Thu May 18 05:17:06 2023, max compression
```

## Comparing `flask_captcha2-0.0.0.tar` & `flask_captcha2-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 05:10:26.851601 flask_captcha2-0.0.0/
--rw-rw-rw-   0        0        0      571 2023-05-18 05:10:26.851601 flask_captcha2-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      102 2023-05-17 15:52:17.000000 flask_captcha2-0.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 05:10:26.849600 flask_captcha2-0.0.0/flask_captcha2.egg-info/
--rw-rw-rw-   0        0        0      571 2023-05-18 05:10:26.000000 flask_captcha2-0.0.0/flask_captcha2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-05-18 05:10:26.000000 flask_captcha2-0.0.0/flask_captcha2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 05:10:26.000000 flask_captcha2-0.0.0/flask_captcha2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-18 05:10:26.000000 flask_captcha2-0.0.0/flask_captcha2.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 05:10:26.000000 flask_captcha2-0.0.0/flask_captcha2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 05:10:26.851601 flask_captcha2-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      849 2023-05-18 05:10:24.000000 flask_captcha2-0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 05:17:06.163437 flask_captcha2-0.1.0/
+-rw-rw-rw-   0        0        0      571 2023-05-18 05:17:06.162438 flask_captcha2-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      102 2023-05-17 15:52:17.000000 flask_captcha2-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 05:17:06.155437 flask_captcha2-0.1.0/flask_captcha2/
+-rw-rw-rw-   0        0        0     3412 2023-05-17 17:21:33.000000 flask_captcha2-0.1.0/flask_captcha2/__init__.py
+-rw-rw-rw-   0        0        0      145 2023-05-18 05:15:38.000000 flask_captcha2-0.1.0/flask_captcha2/auther.py
+drwxrwxrwx   0        0        0        0 2023-05-18 05:17:06.161437 flask_captcha2-0.1.0/flask_captcha2.egg-info/
+-rw-rw-rw-   0        0        0      571 2023-05-18 05:17:06.000000 flask_captcha2-0.1.0/flask_captcha2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-05-18 05:17:06.000000 flask_captcha2-0.1.0/flask_captcha2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 05:17:06.000000 flask_captcha2-0.1.0/flask_captcha2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-18 05:17:06.000000 flask_captcha2-0.1.0/flask_captcha2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-18 05:17:06.000000 flask_captcha2-0.1.0/flask_captcha2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 05:17:06.163437 flask_captcha2-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      828 2023-05-18 05:16:59.000000 flask_captcha2-0.1.0/setup.py
```

### Comparing `flask_captcha2-0.0.0/PKG-INFO` & `flask_captcha2-0.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 1.2
 Name: flask_captcha2
-Version: 0.0.0
+Version: 0.1.0
 Summary: an light and simple flask extension for integrate google recaptcha with Flask Apps
 Home-page: https://github.com/alisharify7/flask_captcha2
 Author: Ali Sharify
 Author-email: alisharifyofficial@gmail.com
 License: MIT
 Description: # flask_captcha
         an light  and simple flask extension for integrate google recaptcha with Flask Apps
         
 Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
```

### Comparing `flask_captcha2-0.0.0/flask_captcha2.egg-info/PKG-INFO` & `flask_captcha2-0.1.0/flask_captcha2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 1.2
 Name: flask-captcha2
-Version: 0.0.0
+Version: 0.1.0
 Summary: an light and simple flask extension for integrate google recaptcha with Flask Apps
 Home-page: https://github.com/alisharify7/flask_captcha2
 Author: Ali Sharify
 Author-email: alisharifyofficial@gmail.com
 License: MIT
 Description: # flask_captcha
         an light  and simple flask extension for integrate google recaptcha with Flask Apps
         
 Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
```

### Comparing `flask_captcha2-0.0.0/setup.py` & `flask_captcha2-0.1.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 with open("./readme.md") as f:
     long_description = f.read()
 
 setup(
     name="flask_captcha2",
     version=__version__,
     description="an light and simple flask extension for integrate google recaptcha with Flask Apps",
-    packages=find_packages(where="flask_captcha2"),
+    packages=find_packages(),
     author_email="alisharifyofficial@gmail.com",
     author="Ali Sharify",
     url="https://github.com/alisharify7/flask_captcha2",
     long_description=long_description,
     classifiers=[
+        "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.10"
     ],
     license="MIT",
     install_requires=[
         "flask>=2.2.5",
         "markupsafe>=2.1.2",
         "requests>=2.30.0"
     ],
```

