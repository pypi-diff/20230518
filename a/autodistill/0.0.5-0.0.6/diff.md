# Comparing `tmp/autodistill-0.0.5.tar.gz` & `tmp/autodistill-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodistill-0.0.5.tar", last modified: Mon Apr 17 15:33:34 2023, max compression
+gzip compressed data, was "autodistill-0.0.6.tar", last modified: Wed May 17 23:04:22 2023, max compression
```

## Comparing `autodistill-0.0.5.tar` & `autodistill-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:33:34.117572 autodistill-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-04-17 15:33:34.113572 autodistill-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-17 15:31:13.000000 autodistill-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:33:34.113572 autodistill-0.0.5/autodistill.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-04-17 15:33:33.000000 autodistill-0.0.5/autodistill.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-17 15:33:34.000000 autodistill-0.0.5/autodistill.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:33:33.000000 autodistill-0.0.5/autodistill.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-17 15:33:33.000000 autodistill-0.0.5/autodistill.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-17 15:33:33.000000 autodistill-0.0.5/autodistill.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 15:33:34.117572 autodistill-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-17 15:31:13.000000 autodistill-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:33:34.113572 autodistill-0.0.5/src/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-17 15:31:13.000000 autodistill-0.0.5/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-17 15:31:13.000000 autodistill-0.0.5/src/hello.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:33:34.113572 autodistill-0.0.5/test/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-17 15:31:13.000000 autodistill-0.0.5/test/test_hello.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 23:04:22.085167 autodistill-0.0.6/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4737 2023-05-17 23:04:22.085167 autodistill-0.0.6/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3397 2023-05-15 17:43:25.000000 autodistill-0.0.6/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 23:04:22.081167 autodistill-0.0.6/autodistill/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-05-17 23:03:59.000000 autodistill-0.0.6/autodistill/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 23:04:22.085167 autodistill-0.0.6/autodistill/base_models/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       57 2023-05-15 17:43:20.000000 autodistill-0.0.6/autodistill/base_models/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      444 2023-05-16 18:56:19.000000 autodistill-0.0.6/autodistill/base_models/base_model.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1758 2023-05-16 19:14:29.000000 autodistill-0.0.6/autodistill/ontology.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 23:04:22.085167 autodistill-0.0.6/autodistill/target_models/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       63 2023-05-16 19:52:06.000000 autodistill-0.0.6/autodistill/target_models/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      243 2023-05-17 21:28:59.000000 autodistill-0.0.6/autodistill/target_models/target_model.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 23:04:22.085167 autodistill-0.0.6/autodistill.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4737 2023-05-17 23:04:22.000000 autodistill-0.0.6/autodistill.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      413 2023-05-17 23:04:22.000000 autodistill-0.0.6/autodistill.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-17 23:04:22.000000 autodistill-0.0.6/autodistill.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       73 2023-05-17 23:04:22.000000 autodistill-0.0.6/autodistill.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2023-05-17 23:04:22.000000 autodistill-0.0.6/autodistill.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-17 23:04:22.085167 autodistill-0.0.6/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1211 2023-05-17 21:19:23.000000 autodistill-0.0.6/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 23:04:22.085167 autodistill-0.0.6/test/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       41 2023-05-17 21:21:04.000000 autodistill-0.0.6/test/test_hello.py
```

### Comparing `autodistill-0.0.5/setup.py` & `autodistill-0.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import setuptools
 from setuptools import find_packages
 import re
 
-with open("./src/__init__.py", 'r') as f:
+with open("./autodistill/__init__.py", 'r') as f:
     content = f.read()
     # from https://www.py4u.net/discuss/139845
     version = re.search(r'__version__\s*=\s*[\'"]([^\'"]*)[\'"]', content).group(1)
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fh:
     install_requires = fh.read().split('\n')
 
 setuptools.setup(
     name="autodistill",  
     version=version,
-    author="jacobsolawetz",
+    author="Roboflow",
     author_email="jacob@roboflow.com",
     description="Automatically distill large foundational models into smaller, in-domain models for deployment",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/roboflow/autodistill",
+    url="https://github.com/autodistill/autodistill",
     install_requires=install_requires,
     packages=find_packages(exclude=("tests",)),
     extras_require={
         "dev": ["flake8", "black==22.3.0", "isort", "twine", "pytest", "wheel"],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
```

