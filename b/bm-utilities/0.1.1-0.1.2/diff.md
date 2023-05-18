# Comparing `tmp/bm_utilities-0.1.1.tar.gz` & `tmp/bm_utilities-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bm_utilities-0.1.1.tar", last modified: Thu May 18 11:02:07 2023, max compression
+gzip compressed data, was "bm_utilities-0.1.2.tar", last modified: Thu May 18 11:08:26 2023, max compression
```

## Comparing `bm_utilities-0.1.1.tar` & `bm_utilities-0.1.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 11:02:07.076290 bm_utilities-0.1.1/
--rw-rw-rw-   0        0        0      313 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/.editorconfig
-drwxrwxrwx   0        0        0        0 2023-05-18 11:02:06.781283 bm_utilities-0.1.1/.github/
-drwxrwxrwx   0        0        0        0 2023-05-18 11:02:06.831283 bm_utilities-0.1.1/.github/ISSUE_TEMPLATE/
--rw-rw-rw-   0        0        0      537 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-rw-   0        0        0      524 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/.github/ISSUE_TEMPLATE/config.yml
--rw-rw-rw-   0        0        0      459 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxrwxrwx   0        0        0        0 2023-05-18 11:02:06.850284 bm_utilities-0.1.1/.github/workflows/
--rw-rw-rw-   0        0        0     2125 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/.github/workflows/docs-build.yml
--rw-rw-rw-   0        0        0     1041 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/.github/workflows/docs.yml
--rw-rw-rw-   0        0        0     1076 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/.github/workflows/macos.yml
--rw-rw-rw-   0        0        0     1032 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/.github/workflows/pypi.yml
--rw-rw-rw-   0        0        0     1586 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/.github/workflows/ubuntu.yml
--rw-rw-rw-   0        0        0      962 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/.github/workflows/windows.yml
--rw-rw-rw-   0        0        0     1310 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/.gitignore
--rw-rw-rw-   0        0        0     1092 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      129 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1356 2023-05-18 11:02:07.077283 bm_utilities-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      610 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 11:02:07.015283 bm_utilities-0.1.1/bm_utilities/
--rw-rw-rw-   0        0        0     5068 2023-05-18 11:00:54.000000 bm_utilities-0.1.1/bm_utilities/Address_finder.py
--rw-rw-rw-   0        0        0      136 2023-05-18 11:01:42.000000 bm_utilities-0.1.1/bm_utilities/__init__.py
--rw-rw-rw-   0        0        0     1067 2023-05-18 11:00:50.000000 bm_utilities-0.1.1/bm_utilities/bm_utilities.py
--rw-rw-rw-   0        0        0      194 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/bm_utilities/common.py
--rw-rw-rw-   0        0        0    11097 2023-05-18 08:07:28.000000 bm_utilities-0.1.1/bm_utilities/quality_gates.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:02:07.032282 bm_utilities-0.1.1/bm_utilities.egg-info/
--rw-rw-rw-   0        0        0     1356 2023-05-18 11:02:06.000000 bm_utilities-0.1.1/bm_utilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      980 2023-05-18 11:02:06.000000 bm_utilities-0.1.1/bm_utilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 11:02:06.000000 bm_utilities-0.1.1/bm_utilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-18 11:02:06.000000 bm_utilities-0.1.1/bm_utilities.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-05-18 11:02:06.000000 bm_utilities-0.1.1/bm_utilities.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-18 11:02:07.057289 bm_utilities-0.1.1/docs/
--rw-rw-rw-   0        0        0       57 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/docs/bm_utilities.md
--rw-rw-rw-   0        0        0       96 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/docs/changelog.md
--rw-rw-rw-   0        0        0       42 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/docs/common.md
--rw-rw-rw-   0        0        0     3303 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/docs/contributing.md
-drwxrwxrwx   0        0        0        0 2023-05-18 11:02:07.061282 bm_utilities-0.1.1/docs/examples/
--rw-rw-rw-   0        0        0      309 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/docs/examples/intro.ipynb
--rw-rw-rw-   0        0        0        7 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/docs/faq.md
--rw-rw-rw-   0        0        0      502 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/docs/index.md
--rw-rw-rw-   0        0        0      612 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/docs/installation.md
-drwxrwxrwx   0        0        0        0 2023-05-18 11:02:07.064282 bm_utilities-0.1.1/docs/overrides/
--rw-rw-rw-   0        0        0      285 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/docs/overrides/main.html
--rw-rw-rw-   0        0        0       79 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/docs/usage.md
--rw-rw-rw-   0        0        0     2242 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/mkdocs.yml
--rw-rw-rw-   0        0        0        0 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/requirements.txt
--rw-rw-rw-   0        0        0      148 2023-04-24 20:57:32.000000 bm_utilities-0.1.1/requirements_dev.txt
--rw-rw-rw-   0        0        0      371 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/requirements_docs.txt
--rw-rw-rw-   0        0        0      420 2023-05-18 11:02:07.079285 bm_utilities-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1771 2023-05-18 11:01:34.000000 bm_utilities-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:02:07.071287 bm_utilities-0.1.1/tests/
--rw-rw-rw-   0        0        0       43 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/tests/__init__.py
--rw-rw-rw-   0        0        0      433 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/tests/test_bm_utilities.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:26.437057 bm_utilities-0.1.2/
+-rw-rw-rw-   0        0        0      313 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/.editorconfig
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:26.177076 bm_utilities-0.1.2/.github/
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:26.230059 bm_utilities-0.1.2/.github/ISSUE_TEMPLATE/
+-rw-rw-rw-   0        0        0      537 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-rw-   0        0        0      524 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-rw-rw-   0        0        0      459 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:26.250069 bm_utilities-0.1.2/.github/workflows/
+-rw-rw-rw-   0        0        0     2125 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/.github/workflows/docs-build.yml
+-rw-rw-rw-   0        0        0     1041 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/.github/workflows/docs.yml
+-rw-rw-rw-   0        0        0     1076 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/.github/workflows/macos.yml
+-rw-rw-rw-   0        0        0     1032 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/.github/workflows/pypi.yml
+-rw-rw-rw-   0        0        0     1586 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/.github/workflows/ubuntu.yml
+-rw-rw-rw-   0        0        0      962 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/.github/workflows/windows.yml
+-rw-rw-rw-   0        0        0     1310 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/.gitignore
+-rw-rw-rw-   0        0        0     1092 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      129 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1356 2023-05-18 11:08:26.438059 bm_utilities-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      610 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:26.376057 bm_utilities-0.1.2/bm_utilities/
+-rw-rw-rw-   0        0        0     5068 2023-05-18 11:00:54.000000 bm_utilities-0.1.2/bm_utilities/Address_finder.py
+-rw-rw-rw-   0        0        0      136 2023-05-18 11:08:16.000000 bm_utilities-0.1.2/bm_utilities/__init__.py
+-rw-rw-rw-   0        0        0     1039 2023-05-18 11:07:36.000000 bm_utilities-0.1.2/bm_utilities/bm_utilities.py
+-rw-rw-rw-   0        0        0      194 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/bm_utilities/common.py
+-rw-rw-rw-   0        0        0    11097 2023-05-18 08:07:28.000000 bm_utilities-0.1.2/bm_utilities/quality_gates.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:26.395057 bm_utilities-0.1.2/bm_utilities.egg-info/
+-rw-rw-rw-   0        0        0     1356 2023-05-18 11:08:25.000000 bm_utilities-0.1.2/bm_utilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      980 2023-05-18 11:08:26.000000 bm_utilities-0.1.2/bm_utilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 11:08:25.000000 bm_utilities-0.1.2/bm_utilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-18 11:08:25.000000 bm_utilities-0.1.2/bm_utilities.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-05-18 11:08:25.000000 bm_utilities-0.1.2/bm_utilities.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:26.420060 bm_utilities-0.1.2/docs/
+-rw-rw-rw-   0        0        0       57 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/docs/bm_utilities.md
+-rw-rw-rw-   0        0        0       96 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/docs/changelog.md
+-rw-rw-rw-   0        0        0       42 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/docs/common.md
+-rw-rw-rw-   0        0        0     3303 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/docs/contributing.md
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:26.423056 bm_utilities-0.1.2/docs/examples/
+-rw-rw-rw-   0        0        0      309 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/docs/examples/intro.ipynb
+-rw-rw-rw-   0        0        0        7 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/docs/faq.md
+-rw-rw-rw-   0        0        0      502 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/docs/index.md
+-rw-rw-rw-   0        0        0      612 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/docs/installation.md
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:26.425057 bm_utilities-0.1.2/docs/overrides/
+-rw-rw-rw-   0        0        0      285 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/docs/overrides/main.html
+-rw-rw-rw-   0        0        0       79 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/docs/usage.md
+-rw-rw-rw-   0        0        0     2242 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/mkdocs.yml
+-rw-rw-rw-   0        0        0        0 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/requirements.txt
+-rw-rw-rw-   0        0        0      148 2023-04-24 20:57:32.000000 bm_utilities-0.1.2/requirements_dev.txt
+-rw-rw-rw-   0        0        0      371 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/requirements_docs.txt
+-rw-rw-rw-   0        0        0      420 2023-05-18 11:08:26.441061 bm_utilities-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1771 2023-05-18 11:08:09.000000 bm_utilities-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:26.433062 bm_utilities-0.1.2/tests/
+-rw-rw-rw-   0        0        0       43 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/tests/__init__.py
+-rw-rw-rw-   0        0        0      433 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/tests/test_bm_utilities.py
```

### Comparing `bm_utilities-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md` & `bm_utilities-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.1/.github/ISSUE_TEMPLATE/config.yml` & `bm_utilities-0.1.2/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.1/.github/workflows/docs-build.yml` & `bm_utilities-0.1.2/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.1/.github/workflows/docs.yml` & `bm_utilities-0.1.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.1/.github/workflows/macos.yml` & `bm_utilities-0.1.2/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.1/.github/workflows/pypi.yml` & `bm_utilities-0.1.2/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.1/.github/workflows/ubuntu.yml` & `bm_utilities-0.1.2/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.1/.github/workflows/windows.yml` & `bm_utilities-0.1.2/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.1/.gitignore` & `bm_utilities-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.1/LICENSE` & `bm_utilities-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.1/PKG-INFO` & `bm_utilities-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bm_utilities
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python package for bm utilities
 Home-page: https://github.com/Youssefamroo/bm_utilities
 Author: youssef amr
 Author-email: usef.amr11@gmail.com
 License: MIT license
 Keywords: bm_utilities
 Classifier: Intended Audience :: Developers
```

### Comparing `bm_utilities-0.1.1/README.md` & `bm_utilities-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.1/bm_utilities/Address_finder.py` & `bm_utilities-0.1.2/bm_utilities/Address_finder.py`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.1/bm_utilities/bm_utilities.py` & `bm_utilities-0.1.2/bm_utilities/bm_utilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from bm_utilities import Address_finder as af
 from bm_utilities import quality_gates as qg
 
 import geopandas as gpd
 import pandas as pd
-import quality_gates as qg
 
 
 def address_finder(geodf,address):
     construct = af(geodf)
     address = construct.find_address(address)
     return address
```

### Comparing `bm_utilities-0.1.1/bm_utilities/quality_gates.py` & `bm_utilities-0.1.2/bm_utilities/quality_gates.py`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.1/bm_utilities.egg-info/PKG-INFO` & `bm_utilities-0.1.2/bm_utilities.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bm-utilities
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python package for bm utilities
 Home-page: https://github.com/Youssefamroo/bm_utilities
 Author: youssef amr
 Author-email: usef.amr11@gmail.com
 License: MIT license
 Keywords: bm_utilities
 Classifier: Intended Audience :: Developers
```

### Comparing `bm_utilities-0.1.1/bm_utilities.egg-info/SOURCES.txt` & `bm_utilities-0.1.2/bm_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.1/docs/contributing.md` & `bm_utilities-0.1.2/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.1/docs/installation.md` & `bm_utilities-0.1.2/docs/installation.md`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.1/mkdocs.yml` & `bm_utilities-0.1.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.1/setup.py` & `bm_utilities-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,10 +48,10 @@
     keywords='bm_utilities',
     name='bm_utilities',
     packages=find_packages(include=['bm_utilities', 'bm_utilities.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/Youssefamroo/bm_utilities',
-    version='0.1.1',
+    version='0.1.2',
     zip_safe=False,
 )
```

