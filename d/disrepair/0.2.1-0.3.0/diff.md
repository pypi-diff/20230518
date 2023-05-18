# Comparing `tmp/disrepair-0.2.1.tar.gz` & `tmp/disrepair-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disrepair-0.2.1.tar", max compression
+gzip compressed data, was "disrepair-0.3.0.tar", max compression
```

## Comparing `disrepair-0.2.1.tar` & `disrepair-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0    35149 2022-08-28 11:02:12.292950 disrepair-0.2.1/LICENSE
--rw-r--r--   0        0        0      748 2022-08-29 10:00:32.111557 disrepair-0.2.1/README.md
--rw-r--r--   0        0        0       48 2022-08-29 09:56:12.665107 disrepair-0.2.1/disrepair/__init__.py
--rw-r--r--   0        0        0       29 2022-08-28 12:00:28.971959 disrepair-0.2.1/disrepair/__main__.py
--rwxr-xr-x   0        0        0    11299 2022-08-29 09:44:08.954816 disrepair-0.2.1/disrepair/check.py
--rw-r--r--   0        0        0      835 2022-08-29 09:56:34.595662 disrepair-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1644 2022-08-29 10:01:11.375914 disrepair-0.2.1/setup.py
--rw-r--r--   0        0        0     1797 2022-08-29 10:01:11.376725 disrepair-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-18 16:01:10.205656 disrepair-0.3.0/LICENSE
+-rw-r--r--   0        0        0      748 2023-05-18 16:01:10.205656 disrepair-0.3.0/README.md
+-rw-r--r--   0        0        0       48 2023-05-18 16:01:10.205656 disrepair-0.3.0/disrepair/__init__.py
+-rw-r--r--   0        0        0       29 2023-05-18 16:01:10.205656 disrepair-0.3.0/disrepair/__main__.py
+-rwxr-xr-x   0        0        0    11512 2023-05-18 16:25:13.177083 disrepair-0.3.0/disrepair/check.py
+-rw-r--r--   0        0        0      855 2023-05-18 16:13:09.739589 disrepair-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1881 1970-01-01 00:00:00.000000 disrepair-0.3.0/PKG-INFO
```

### Comparing `disrepair-0.2.1/LICENSE` & `disrepair-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `disrepair-0.2.1/README.md` & `disrepair-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `disrepair-0.2.1/disrepair/check.py` & `disrepair-0.3.0/disrepair/check.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 import os.path
 
 import click
 import requests
 from packaging.version import InvalidVersion, Version
-from pypi_simple import PyPISimple, UnsupportedContentTypeError, UnsupportedRepoVersionError
+from pypi_simple import PyPISimple, UnsupportedContentTypeError, UnsupportedRepoVersionError, NoSuchProjectError
 from requirements.requirement import Requirement
 from rich.console import Console
 
 JSON_REPO = 'https://pypi.org/pypi'
 SIMPLE_REPO = "https://pypi.org/simple"
 
 
@@ -145,14 +145,18 @@
                 page = client.get_project_page(name, timeout=5)
             except requests.RequestException:
                 raise CheckFailed("Connection error")
             except UnsupportedRepoVersionError:
                 raise CheckFailed("Unsupported repo version")
             except UnsupportedContentTypeError:
                 raise CheckFailed("Unsupported content type")
+            except NoSuchProjectError:
+                raise CheckFailed("Package not found")
+            except Exception as exc:
+                raise CheckFailed(f"Unexpected error: {exc}")
 
             if page is None:
                 raise CheckFailed("Package not found")
 
             if not page.packages:
                 raise CheckFailed("Package not found")
```

### Comparing `disrepair-0.2.1/pyproject.toml` & `disrepair-0.3.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "disrepair"
-version = "0.2.1"
+version = "0.3.0"
 description = "Checks for out-of-date Python packages in requirements files"
 authors = ["David Bell <dave@evad.io>"]
 
 license = "GPL3"
 readme = "README.md"
 homepage = "https://github.com/divad/disrepair"
 repository = "https://github.com/divad/disrepair"
@@ -22,14 +22,15 @@
 python = "^3.7"
 click = ">=8.0"
 requests = ">=2.0"
 packaging = ">=21.0"
 pypi-simple = ">=0.8.0"
 requirements-parser = ">=0.5.0"
 rich = ">=12.0"
+setuptools = ">=60"
 
 [tool.poetry.scripts]
 disrepair = 'disrepair:check'
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `disrepair-0.2.1/PKG-INFO` & `disrepair-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: disrepair
-Version: 0.2.1
+Version: 0.3.0
 Summary: Checks for out-of-date Python packages in requirements files
 Home-page: https://github.com/divad/disrepair
 License: GPL3
 Author: David Bell
 Author-email: dave@evad.io
 Requires-Python: >=3.7,<4.0
 Classifier: Environment :: Console
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Dist: click (>=8.0)
 Requires-Dist: packaging (>=21.0)
 Requires-Dist: pypi-simple (>=0.8.0)
 Requires-Dist: requests (>=2.0)
 Requires-Dist: requirements-parser (>=0.5.0)
 Requires-Dist: rich (>=12.0)
+Requires-Dist: setuptools (>=60)
 Project-URL: Repository, https://github.com/divad/disrepair
 Description-Content-Type: text/markdown
 
 # disrepair
 Checks for out-of-date Python packages in requirements files
 
 ## Install
```

