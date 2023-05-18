# Comparing `tmp/template-pptx-jinja-my-0.0.1.tar.gz` & `tmp/template-pptx-jinja-my-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "template-pptx-jinja-my-0.0.1.tar", last modified: Thu May 18 09:03:03 2023, max compression
+gzip compressed data, was "template-pptx-jinja-my-0.0.2.tar", last modified: Thu May 18 09:08:27 2023, max compression
```

## Comparing `template-pptx-jinja-my-0.0.1.tar` & `template-pptx-jinja-my-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 wangguangyu   (501) staff       (20)        0 2023-05-18 09:03:03.301497 template-pptx-jinja-my-0.0.1/
--rw-r--r--   0 wangguangyu   (501) staff       (20)    35149 2023-05-18 06:21:21.000000 template-pptx-jinja-my-0.0.1/LICENSE
--rw-r--r--   0 wangguangyu   (501) staff       (20)     1036 2023-05-18 09:03:03.300840 template-pptx-jinja-my-0.0.1/PKG-INFO
--rw-r--r--   0 wangguangyu   (501) staff       (20)       38 2023-05-18 09:03:03.301611 template-pptx-jinja-my-0.0.1/setup.cfg
--rw-r--r--   0 wangguangyu   (501) staff       (20)      926 2023-05-18 08:48:59.000000 template-pptx-jinja-my-0.0.1/setup.py
-drwxr-xr-x   0 wangguangyu   (501) staff       (20)        0 2023-05-18 09:03:03.297055 template-pptx-jinja-my-0.0.1/template_pptx_jinja/
--rw-r--r--   0 wangguangyu   (501) staff       (20)        0 2023-05-18 06:21:21.000000 template-pptx-jinja-my-0.0.1/template_pptx_jinja/__init__.py
--rw-r--r--   0 wangguangyu   (501) staff       (20)      649 2023-05-18 07:18:43.000000 template-pptx-jinja-my-0.0.1/template_pptx_jinja/pictures.py
--rw-r--r--   0 wangguangyu   (501) staff       (20)     2714 2023-05-18 08:26:06.000000 template-pptx-jinja-my-0.0.1/template_pptx_jinja/render.py
-drwxr-xr-x   0 wangguangyu   (501) staff       (20)        0 2023-05-18 09:03:03.300269 template-pptx-jinja-my-0.0.1/template_pptx_jinja_my.egg-info/
--rw-r--r--   0 wangguangyu   (501) staff       (20)     1036 2023-05-18 09:03:03.000000 template-pptx-jinja-my-0.0.1/template_pptx_jinja_my.egg-info/PKG-INFO
--rw-r--r--   0 wangguangyu   (501) staff       (20)      339 2023-05-18 09:03:03.000000 template-pptx-jinja-my-0.0.1/template_pptx_jinja_my.egg-info/SOURCES.txt
--rw-r--r--   0 wangguangyu   (501) staff       (20)        1 2023-05-18 09:03:03.000000 template-pptx-jinja-my-0.0.1/template_pptx_jinja_my.egg-info/dependency_links.txt
--rw-r--r--   0 wangguangyu   (501) staff       (20)       34 2023-05-18 09:03:03.000000 template-pptx-jinja-my-0.0.1/template_pptx_jinja_my.egg-info/requires.txt
--rw-r--r--   0 wangguangyu   (501) staff       (20)       20 2023-05-18 09:03:03.000000 template-pptx-jinja-my-0.0.1/template_pptx_jinja_my.egg-info/top_level.txt
+drwxr-xr-x   0 wangguangyu   (501) staff       (20)        0 2023-05-18 09:08:27.411393 template-pptx-jinja-my-0.0.2/
+-rw-r--r--   0 wangguangyu   (501) staff       (20)    35149 2023-05-18 06:21:21.000000 template-pptx-jinja-my-0.0.2/LICENSE
+-rw-r--r--   0 wangguangyu   (501) staff       (20)     1042 2023-05-18 09:08:27.410899 template-pptx-jinja-my-0.0.2/PKG-INFO
+-rw-r--r--   0 wangguangyu   (501) staff       (20)       38 2023-05-18 09:08:27.411482 template-pptx-jinja-my-0.0.2/setup.cfg
+-rw-r--r--   0 wangguangyu   (501) staff       (20)      926 2023-05-18 09:08:15.000000 template-pptx-jinja-my-0.0.2/setup.py
+drwxr-xr-x   0 wangguangyu   (501) staff       (20)        0 2023-05-18 09:08:27.408225 template-pptx-jinja-my-0.0.2/template_pptx_jinja/
+-rw-r--r--   0 wangguangyu   (501) staff       (20)        0 2023-05-18 06:21:21.000000 template-pptx-jinja-my-0.0.2/template_pptx_jinja/__init__.py
+-rw-r--r--   0 wangguangyu   (501) staff       (20)      649 2023-05-18 07:18:43.000000 template-pptx-jinja-my-0.0.2/template_pptx_jinja/pictures.py
+-rw-r--r--   0 wangguangyu   (501) staff       (20)     2714 2023-05-18 08:26:06.000000 template-pptx-jinja-my-0.0.2/template_pptx_jinja/render.py
+drwxr-xr-x   0 wangguangyu   (501) staff       (20)        0 2023-05-18 09:08:27.410257 template-pptx-jinja-my-0.0.2/template_pptx_jinja_my.egg-info/
+-rw-r--r--   0 wangguangyu   (501) staff       (20)     1042 2023-05-18 09:08:27.000000 template-pptx-jinja-my-0.0.2/template_pptx_jinja_my.egg-info/PKG-INFO
+-rw-r--r--   0 wangguangyu   (501) staff       (20)      339 2023-05-18 09:08:27.000000 template-pptx-jinja-my-0.0.2/template_pptx_jinja_my.egg-info/SOURCES.txt
+-rw-r--r--   0 wangguangyu   (501) staff       (20)        1 2023-05-18 09:08:27.000000 template-pptx-jinja-my-0.0.2/template_pptx_jinja_my.egg-info/dependency_links.txt
+-rw-r--r--   0 wangguangyu   (501) staff       (20)       34 2023-05-18 09:08:27.000000 template-pptx-jinja-my-0.0.2/template_pptx_jinja_my.egg-info/requires.txt
+-rw-r--r--   0 wangguangyu   (501) staff       (20)       20 2023-05-18 09:08:27.000000 template-pptx-jinja-my-0.0.2/template_pptx_jinja_my.egg-info/top_level.txt
```

### Comparing `template-pptx-jinja-my-0.0.1/LICENSE` & `template-pptx-jinja-my-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `template-pptx-jinja-my-0.0.1/PKG-INFO` & `template-pptx-jinja-my-0.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: template-pptx-jinja-my
-Version: 0.0.1
+Version: 0.0.2
 Summary: PowerPoint presentation builder from template using Jinja2
 Home-page: https://github.com/macheal/template-pptx-jinja
 Author: macheal
 Author-email: xinyukc01@icloud.com
 Keywords: powerpoint,ppt,pptx,template
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Utilities
@@ -20,20 +20,20 @@
 
 You can define your own Jinja2 filters.
 
 It can also replace picture.
 
 See `example.py` for example.
 
-See the PyPI package at https://pypi.org/project/template-pptx-jinja/0.2.0
+See the PyPI package at https://pypi.org/project/template-pptx-jinja-my/0.0.1
 
 ## Install
 
 Run
 
-    pip install template-pptx-jinja
+    pip install template-pptx-jinja-my
 
 ## Dev
 
     python3 -m venv env
     source env/bin/activate
     pip install -r requirements.txt
```

### Comparing `template-pptx-jinja-my-0.0.1/setup.py` & `template-pptx-jinja-my-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def read(filename):
     with open(filename, 'r', encoding='utf-8') as myfile:
         return myfile.read()
 
 
 setup(name='template-pptx-jinja-my',
-    version="0.0.1",
+    version="0.0.2",
     description='PowerPoint presentation builder from template using Jinja2',
     long_description=read('readme.md'),
     long_description_content_type='text/markdown',
     url='https://github.com/macheal/template-pptx-jinja',
     author='macheal',
     author_email='xinyukc01@icloud.com',
     install_requires=read('requirements.txt').split(),
```

### Comparing `template-pptx-jinja-my-0.0.1/template_pptx_jinja/pictures.py` & `template-pptx-jinja-my-0.0.2/template_pptx_jinja/pictures.py`

 * *Files identical despite different names*

### Comparing `template-pptx-jinja-my-0.0.1/template_pptx_jinja/render.py` & `template-pptx-jinja-my-0.0.2/template_pptx_jinja/render.py`

 * *Files identical despite different names*

### Comparing `template-pptx-jinja-my-0.0.1/template_pptx_jinja_my.egg-info/PKG-INFO` & `template-pptx-jinja-my-0.0.2/template_pptx_jinja_my.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: template-pptx-jinja-my
-Version: 0.0.1
+Version: 0.0.2
 Summary: PowerPoint presentation builder from template using Jinja2
 Home-page: https://github.com/macheal/template-pptx-jinja
 Author: macheal
 Author-email: xinyukc01@icloud.com
 Keywords: powerpoint,ppt,pptx,template
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Utilities
@@ -20,20 +20,20 @@
 
 You can define your own Jinja2 filters.
 
 It can also replace picture.
 
 See `example.py` for example.
 
-See the PyPI package at https://pypi.org/project/template-pptx-jinja/0.2.0
+See the PyPI package at https://pypi.org/project/template-pptx-jinja-my/0.0.1
 
 ## Install
 
 Run
 
-    pip install template-pptx-jinja
+    pip install template-pptx-jinja-my
 
 ## Dev
 
     python3 -m venv env
     source env/bin/activate
     pip install -r requirements.txt
```

