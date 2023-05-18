# Comparing `tmp/pypura-0.1.1.tar.gz` & `tmp/pypura-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypura-0.1.1.tar", max compression
+gzip compressed data, was "pypura-0.1.2.tar", max compression
```

## Comparing `pypura-0.1.1.tar` & `pypura-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1071 2023-05-16 21:33:19.526089 pypura-0.1.1/LICENSE
--rw-r--r--   0        0        0       76 2023-05-16 18:55:48.661213 pypura-0.1.1/README.md
--rw-r--r--   0        0        0      631 2023-05-17 21:30:10.586520 pypura-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      251 2023-05-17 21:30:10.597215 pypura-0.1.1/pypura/__init__.py
--rw-r--r--   0        0        0      612 2023-05-17 19:03:02.323743 pypura-0.1.1/pypura/const.py
--rw-r--r--   0        0        0      200 2023-05-16 22:52:50.516386 pypura-0.1.1/pypura/exceptions.py
--rw-r--r--   0        0        0     5620 2023-05-17 19:32:48.277789 pypura-0.1.1/pypura/pura.py
--rw-r--r--   0        0        0        0 2023-05-17 06:46:31.898658 pypura-0.1.1/pypura/py.typed
--rw-r--r--   0        0        0      717 2023-05-17 19:03:43.405261 pypura-0.1.1/pypura/utils.py
--rw-r--r--   0        0        0      773 1970-01-01 00:00:00.000000 pypura-0.1.1/setup.py
--rw-r--r--   0        0        0      689 1970-01-01 00:00:00.000000 pypura-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-16 21:33:19.526089 pypura-0.1.2/LICENSE
+-rw-r--r--   0        0        0       76 2023-05-16 18:55:48.661213 pypura-0.1.2/README.md
+-rw-r--r--   0        0        0      631 2023-05-18 02:11:16.605364 pypura-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      251 2023-05-18 02:11:25.600975 pypura-0.1.2/pypura/__init__.py
+-rw-r--r--   0        0        0     1447 2023-05-18 02:10:28.055646 pypura-0.1.2/pypura/const.py
+-rw-r--r--   0        0        0      200 2023-05-16 22:52:50.516386 pypura-0.1.2/pypura/exceptions.py
+-rw-r--r--   0        0        0     5620 2023-05-17 19:32:48.277789 pypura-0.1.2/pypura/pura.py
+-rw-r--r--   0        0        0        0 2023-05-17 06:46:31.898658 pypura-0.1.2/pypura/py.typed
+-rw-r--r--   0        0        0      717 2023-05-17 19:03:43.405261 pypura-0.1.2/pypura/utils.py
+-rw-r--r--   0        0        0      773 1970-01-01 00:00:00.000000 pypura-0.1.2/setup.py
+-rw-r--r--   0        0        0      689 1970-01-01 00:00:00.000000 pypura-0.1.2/PKG-INFO
```

### Comparing `pypura-0.1.1/LICENSE` & `pypura-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pypura-0.1.1/pyproject.toml` & `pypura-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pypura"
-version = "0.1.1"
+version = "0.1.2"
 description = "Python package for interacting with Pura smart fragrance diffuser"
 authors = ["Nathan Spencer <natekspencer@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 include = ["pypura/py.typed"]
 
 [tool.poetry.dependencies]
```

### Comparing `pypura-0.1.1/pypura/pura.py` & `pypura-0.1.2/pypura/pura.py`

 * *Files identical despite different names*

### Comparing `pypura-0.1.1/pypura/utils.py` & `pypura-0.1.2/pypura/utils.py`

 * *Files identical despite different names*

### Comparing `pypura-0.1.1/setup.py` & `pypura-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['boto3>=1.26.135,<2.0.0', 'pycognito>=2022.12.0,<2023.0.0']
 
 setup_kwargs = {
     'name': 'pypura',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Python package for interacting with Pura smart fragrance diffuser',
     'long_description': '# pypura\nPython package for interacting with Pura smart fragrance diffusers\n',
     'author': 'Nathan Spencer',
     'author_email': 'natekspencer@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pypura-0.1.1/PKG-INFO` & `pypura-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypura
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python package for interacting with Pura smart fragrance diffuser
 License: MIT
 Author: Nathan Spencer
 Author-email: natekspencer@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

