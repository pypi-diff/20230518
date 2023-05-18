# Comparing `tmp/quantready_base-0.1.0.tar.gz` & `tmp/quantready_base-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantready_base-0.1.0.tar", max compression
+gzip compressed data, was "quantready_base-0.2.0.tar", max compression
```

## Comparing `quantready_base-0.1.0.tar` & `quantready_base-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1080 2023-05-17 12:29:01.545385 quantready_base-0.1.0/LICENSE
--rw-r--r--   0        0        0     4412 2023-05-18 03:11:37.387731 quantready_base-0.1.0/README.md
--rw-r--r--   0        0        0     1006 2023-05-18 01:36:28.336317 quantready_base-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       81 2023-05-18 02:40:42.504458 quantready_base-0.1.0/quantready_base/__init__.py
--rw-r--r--   0        0        0      120 2023-05-18 01:16:48.958226 quantready_base-0.1.0/quantready_base/__main__.py
--rw-r--r--   0        0        0      828 2023-05-18 02:09:34.146470 quantready_base-0.1.0/quantready_base/cli.py
--rw-r--r--   0        0        0      843 2023-05-18 02:50:29.419957 quantready_base-0.1.0/quantready_base/config.py
--rw-r--r--   0        0        0     5270 1970-01-01 00:00:00.000000 quantready_base-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-05-18 04:33:23.095029 quantready_base-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4599 2023-05-18 04:33:23.095029 quantready_base-0.2.0/README.md
+-rw-r--r--   0        0        0     1006 2023-05-18 04:33:23.095029 quantready_base-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       81 2023-05-18 04:33:23.095029 quantready_base-0.2.0/quantready_base/__init__.py
+-rw-r--r--   0        0        0      120 2023-05-18 04:33:23.095029 quantready_base-0.2.0/quantready_base/__main__.py
+-rw-r--r--   0        0        0      828 2023-05-18 04:33:23.095029 quantready_base-0.2.0/quantready_base/cli.py
+-rw-r--r--   0        0        0      843 2023-05-18 04:33:23.095029 quantready_base-0.2.0/quantready_base/config.py
+-rw-r--r--   0        0        0     5457 1970-01-01 00:00:00.000000 quantready_base-0.2.0/PKG-INFO
```

### Comparing `quantready_base-0.1.0/LICENSE` & `quantready_base-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quantready_base-0.1.0/README.md` & `quantready_base-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 * ✔️ [poetry](https://python-poetry.org/) for dependency management
 * ✔️ [pre-commit](https://pre-commit.com/) hooks for code formatting, linting, and testing
 * ✔️ [unittest](https://docs.python.org/3/library/unittest.html) for testing
 * ✔️ [gitleaks](https://gitleaks.io/) for secrets scanning
 
 Deployment:
 
-* 🔲 [github actions](https://github.com/actions) for CI/CD
+* ✔️ [github actions](https://github.com/actions) for CI/CD
 * ✔️ [docker](https://docker.com) for building containers
-* 🔲 [twine](https://twine.readthedocs.io/en/latest/) for publishing to pypi or private repositories
+* ✔️ [twine](https://twine.readthedocs.io/en/latest/) for publishing to pypi or private repositories
 * 🔲 [gcloud](https://cloud.google.com/sdk/gcloud) for publishing to private repositories
 
 ## 📦 Installation
 
 There are two ways to install:
 
 ### 1. Install using `quantready` cli
@@ -99,24 +99,26 @@
 ```
 
 ### Publish to pypi
 
 ```bash
 # Build the package
 poetry build
-twine upload dist/*
-
+poetry run twine upload dist/*
 ```
 
+Get `PYPI_API_TOKEN` from <https://pypi.org/manage/account/token/>
+And set it as a github secret <https://github.com/><username>/<repo>/settings/secrets/actions
+
 ### Publish to private repository
 
 ```bash
 # Build the package
 poetry build
-twine upload --repository-url https://pypi.yourdomain.com dist/*
+poetry run twine upload --repository-url https://pypi.yourdomain.com dist/*
 
 ```
 
 ## 📝 License
 
 This project is licensed under the terms of the [MIT license](/LICENSE).
```

### Comparing `quantready_base-0.1.0/pyproject.toml` & `quantready_base-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quantready-base"
-version = "0.1.0"
+version = "0.2.0"
 description = "Publish public or private python libraries - using the modern python stack"
 authors = ["Sean Kruzel <sean@closedloop.tech>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "quantready_base" }]
 
 [tool.poetry.dependencies]
```

### Comparing `quantready_base-0.1.0/quantready_base/cli.py` & `quantready_base-0.2.0/quantready_base/cli.py`

 * *Files identical despite different names*

### Comparing `quantready_base-0.1.0/quantready_base/config.py` & `quantready_base-0.2.0/quantready_base/config.py`

 * *Files identical despite different names*

### Comparing `quantready_base-0.1.0/PKG-INFO` & `quantready_base-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantready-base
-Version: 0.1.0
+Version: 0.2.0
 Summary: Publish public or private python libraries - using the modern python stack
 License: MIT
 Author: Sean Kruzel
 Author-email: sean@closedloop.tech
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -32,17 +32,17 @@
 * ✔️ [poetry](https://python-poetry.org/) for dependency management
 * ✔️ [pre-commit](https://pre-commit.com/) hooks for code formatting, linting, and testing
 * ✔️ [unittest](https://docs.python.org/3/library/unittest.html) for testing
 * ✔️ [gitleaks](https://gitleaks.io/) for secrets scanning
 
 Deployment:
 
-* 🔲 [github actions](https://github.com/actions) for CI/CD
+* ✔️ [github actions](https://github.com/actions) for CI/CD
 * ✔️ [docker](https://docker.com) for building containers
-* 🔲 [twine](https://twine.readthedocs.io/en/latest/) for publishing to pypi or private repositories
+* ✔️ [twine](https://twine.readthedocs.io/en/latest/) for publishing to pypi or private repositories
 * 🔲 [gcloud](https://cloud.google.com/sdk/gcloud) for publishing to private repositories
 
 ## 📦 Installation
 
 There are two ways to install:
 
 ### 1. Install using `quantready` cli
@@ -122,24 +122,26 @@
 ```
 
 ### Publish to pypi
 
 ```bash
 # Build the package
 poetry build
-twine upload dist/*
-
+poetry run twine upload dist/*
 ```
 
+Get `PYPI_API_TOKEN` from <https://pypi.org/manage/account/token/>
+And set it as a github secret <https://github.com/><username>/<repo>/settings/secrets/actions
+
 ### Publish to private repository
 
 ```bash
 # Build the package
 poetry build
-twine upload --repository-url https://pypi.yourdomain.com dist/*
+poetry run twine upload --repository-url https://pypi.yourdomain.com dist/*
 
 ```
 
 ## 📝 License
 
 This project is licensed under the terms of the [MIT license](/LICENSE).
```

