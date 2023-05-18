# Comparing `tmp/bm_utilities-0.1.2.tar.gz` & `tmp/bm_utilities-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bm_utilities-0.1.2.tar", last modified: Thu May 18 11:08:26 2023, max compression
+gzip compressed data, was "bm_utilities-0.1.3.tar", last modified: Thu May 18 11:19:22 2023, max compression
```

## Comparing `bm_utilities-0.1.2.tar` & `bm_utilities-0.1.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:26.437057 bm_utilities-0.1.2/
--rw-rw-rw-   0        0        0      313 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/.editorconfig
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:26.177076 bm_utilities-0.1.2/.github/
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:26.230059 bm_utilities-0.1.2/.github/ISSUE_TEMPLATE/
--rw-rw-rw-   0        0        0      537 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-rw-   0        0        0      524 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/.github/ISSUE_TEMPLATE/config.yml
--rw-rw-rw-   0        0        0      459 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:26.250069 bm_utilities-0.1.2/.github/workflows/
--rw-rw-rw-   0        0        0     2125 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/.github/workflows/docs-build.yml
--rw-rw-rw-   0        0        0     1041 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/.github/workflows/docs.yml
--rw-rw-rw-   0        0        0     1076 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/.github/workflows/macos.yml
--rw-rw-rw-   0        0        0     1032 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/.github/workflows/pypi.yml
--rw-rw-rw-   0        0        0     1586 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/.github/workflows/ubuntu.yml
--rw-rw-rw-   0        0        0      962 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/.github/workflows/windows.yml
--rw-rw-rw-   0        0        0     1310 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/.gitignore
--rw-rw-rw-   0        0        0     1092 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      129 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1356 2023-05-18 11:08:26.438059 bm_utilities-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      610 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:26.376057 bm_utilities-0.1.2/bm_utilities/
--rw-rw-rw-   0        0        0     5068 2023-05-18 11:00:54.000000 bm_utilities-0.1.2/bm_utilities/Address_finder.py
--rw-rw-rw-   0        0        0      136 2023-05-18 11:08:16.000000 bm_utilities-0.1.2/bm_utilities/__init__.py
--rw-rw-rw-   0        0        0     1039 2023-05-18 11:07:36.000000 bm_utilities-0.1.2/bm_utilities/bm_utilities.py
--rw-rw-rw-   0        0        0      194 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/bm_utilities/common.py
--rw-rw-rw-   0        0        0    11097 2023-05-18 08:07:28.000000 bm_utilities-0.1.2/bm_utilities/quality_gates.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:26.395057 bm_utilities-0.1.2/bm_utilities.egg-info/
--rw-rw-rw-   0        0        0     1356 2023-05-18 11:08:25.000000 bm_utilities-0.1.2/bm_utilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      980 2023-05-18 11:08:26.000000 bm_utilities-0.1.2/bm_utilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 11:08:25.000000 bm_utilities-0.1.2/bm_utilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-18 11:08:25.000000 bm_utilities-0.1.2/bm_utilities.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-05-18 11:08:25.000000 bm_utilities-0.1.2/bm_utilities.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:26.420060 bm_utilities-0.1.2/docs/
--rw-rw-rw-   0        0        0       57 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/docs/bm_utilities.md
--rw-rw-rw-   0        0        0       96 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/docs/changelog.md
--rw-rw-rw-   0        0        0       42 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/docs/common.md
--rw-rw-rw-   0        0        0     3303 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/docs/contributing.md
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:26.423056 bm_utilities-0.1.2/docs/examples/
--rw-rw-rw-   0        0        0      309 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/docs/examples/intro.ipynb
--rw-rw-rw-   0        0        0        7 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/docs/faq.md
--rw-rw-rw-   0        0        0      502 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/docs/index.md
--rw-rw-rw-   0        0        0      612 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/docs/installation.md
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:26.425057 bm_utilities-0.1.2/docs/overrides/
--rw-rw-rw-   0        0        0      285 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/docs/overrides/main.html
--rw-rw-rw-   0        0        0       79 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/docs/usage.md
--rw-rw-rw-   0        0        0     2242 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/mkdocs.yml
--rw-rw-rw-   0        0        0        0 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/requirements.txt
--rw-rw-rw-   0        0        0      148 2023-04-24 20:57:32.000000 bm_utilities-0.1.2/requirements_dev.txt
--rw-rw-rw-   0        0        0      371 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/requirements_docs.txt
--rw-rw-rw-   0        0        0      420 2023-05-18 11:08:26.441061 bm_utilities-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1771 2023-05-18 11:08:09.000000 bm_utilities-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:26.433062 bm_utilities-0.1.2/tests/
--rw-rw-rw-   0        0        0       43 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/tests/__init__.py
--rw-rw-rw-   0        0        0      433 2023-04-24 13:32:39.000000 bm_utilities-0.1.2/tests/test_bm_utilities.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:19:22.825657 bm_utilities-0.1.3/
+-rw-rw-rw-   0        0        0      313 2023-04-24 13:32:39.000000 bm_utilities-0.1.3/.editorconfig
+drwxrwxrwx   0        0        0        0 2023-05-18 11:19:22.546448 bm_utilities-0.1.3/.github/
+drwxrwxrwx   0        0        0        0 2023-05-18 11:19:22.596656 bm_utilities-0.1.3/.github/ISSUE_TEMPLATE/
+-rw-rw-rw-   0        0        0      537 2023-04-24 13:32:39.000000 bm_utilities-0.1.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-rw-   0        0        0      524 2023-04-24 13:32:39.000000 bm_utilities-0.1.3/.github/ISSUE_TEMPLATE/config.yml
+-rw-rw-rw-   0        0        0      459 2023-04-24 13:32:39.000000 bm_utilities-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md
+drwxrwxrwx   0        0        0        0 2023-05-18 11:19:22.623683 bm_utilities-0.1.3/.github/workflows/
+-rw-rw-rw-   0        0        0     2125 2023-04-24 13:32:39.000000 bm_utilities-0.1.3/.github/workflows/docs-build.yml
+-rw-rw-rw-   0        0        0     1041 2023-04-24 13:32:39.000000 bm_utilities-0.1.3/.github/workflows/docs.yml
+-rw-rw-rw-   0        0        0     1076 2023-04-24 13:32:39.000000 bm_utilities-0.1.3/.github/workflows/macos.yml
+-rw-rw-rw-   0        0        0     1032 2023-04-24 13:32:39.000000 bm_utilities-0.1.3/.github/workflows/pypi.yml
+-rw-rw-rw-   0        0        0     1586 2023-04-24 13:32:39.000000 bm_utilities-0.1.3/.github/workflows/ubuntu.yml
+-rw-rw-rw-   0        0        0      962 2023-04-24 13:32:39.000000 bm_utilities-0.1.3/.github/workflows/windows.yml
+-rw-rw-rw-   0        0        0     1310 2023-04-24 13:32:39.000000 bm_utilities-0.1.3/.gitignore
+-rw-rw-rw-   0        0        0     1092 2023-04-24 13:32:39.000000 bm_utilities-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      129 2023-04-24 13:32:39.000000 bm_utilities-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1356 2023-05-18 11:19:22.826656 bm_utilities-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      610 2023-04-24 13:32:39.000000 bm_utilities-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 11:19:22.763656 bm_utilities-0.1.3/bm_utilities/
+-rw-rw-rw-   0        0        0     5068 2023-05-18 11:00:54.000000 bm_utilities-0.1.3/bm_utilities/Address_finder.py
+-rw-rw-rw-   0        0        0      136 2023-05-18 11:19:10.000000 bm_utilities-0.1.3/bm_utilities/__init__.py
+-rw-rw-rw-   0        0        0     1053 2023-05-18 11:18:41.000000 bm_utilities-0.1.3/bm_utilities/bm_utilities.py
+-rw-rw-rw-   0        0        0      194 2023-04-24 13:32:39.000000 bm_utilities-0.1.3/bm_utilities/common.py
+-rw-rw-rw-   0        0        0    11097 2023-05-18 08:07:28.000000 bm_utilities-0.1.3/bm_utilities/quality_gates.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:19:22.784662 bm_utilities-0.1.3/bm_utilities.egg-info/
+-rw-rw-rw-   0        0        0     1356 2023-05-18 11:19:22.000000 bm_utilities-0.1.3/bm_utilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      980 2023-05-18 11:19:22.000000 bm_utilities-0.1.3/bm_utilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 11:19:22.000000 bm_utilities-0.1.3/bm_utilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-18 11:19:22.000000 bm_utilities-0.1.3/bm_utilities.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-05-18 11:19:22.000000 bm_utilities-0.1.3/bm_utilities.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 11:19:22.808659 bm_utilities-0.1.3/docs/
+-rw-rw-rw-   0        0        0       57 2023-04-24 13:32:39.000000 bm_utilities-0.1.3/docs/bm_utilities.md
+-rw-rw-rw-   0        0        0       96 2023-04-24 13:32:39.000000 bm_utilities-0.1.3/docs/changelog.md
+-rw-rw-rw-   0        0        0       42 2023-04-24 13:32:39.000000 bm_utilities-0.1.3/docs/common.md
+-rw-rw-rw-   0        0        0     3303 2023-04-24 13:32:39.000000 bm_utilities-0.1.3/docs/contributing.md
+drwxrwxrwx   0        0        0        0 2023-05-18 11:19:22.811661 bm_utilities-0.1.3/docs/examples/
+-rw-rw-rw-   0        0        0      309 2023-04-24 13:32:39.000000 bm_utilities-0.1.3/docs/examples/intro.ipynb
+-rw-rw-rw-   0        0        0        7 2023-04-24 13:32:39.000000 bm_utilities-0.1.3/docs/faq.md
+-rw-rw-rw-   0        0        0      502 2023-04-24 13:32:39.000000 bm_utilities-0.1.3/docs/index.md
+-rw-rw-rw-   0        0        0      612 2023-04-24 13:32:39.000000 bm_utilities-0.1.3/docs/installation.md
+drwxrwxrwx   0        0        0        0 2023-05-18 11:19:22.813657 bm_utilities-0.1.3/docs/overrides/
+-rw-rw-rw-   0        0        0      285 2023-04-24 13:32:39.000000 bm_utilities-0.1.3/docs/overrides/main.html
+-rw-rw-rw-   0        0        0       79 2023-04-24 13:32:39.000000 bm_utilities-0.1.3/docs/usage.md
+-rw-rw-rw-   0        0        0     2242 2023-04-24 13:32:39.000000 bm_utilities-0.1.3/mkdocs.yml
+-rw-rw-rw-   0        0        0        0 2023-04-24 13:32:39.000000 bm_utilities-0.1.3/requirements.txt
+-rw-rw-rw-   0        0        0      148 2023-04-24 20:57:32.000000 bm_utilities-0.1.3/requirements_dev.txt
+-rw-rw-rw-   0        0        0      371 2023-04-24 13:32:39.000000 bm_utilities-0.1.3/requirements_docs.txt
+-rw-rw-rw-   0        0        0      420 2023-05-18 11:19:22.828657 bm_utilities-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1771 2023-05-18 11:19:01.000000 bm_utilities-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:19:22.822668 bm_utilities-0.1.3/tests/
+-rw-rw-rw-   0        0        0       43 2023-04-24 13:32:39.000000 bm_utilities-0.1.3/tests/__init__.py
+-rw-rw-rw-   0        0        0      433 2023-04-24 13:32:39.000000 bm_utilities-0.1.3/tests/test_bm_utilities.py
```

### Comparing `bm_utilities-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md` & `bm_utilities-0.1.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.2/.github/ISSUE_TEMPLATE/config.yml` & `bm_utilities-0.1.3/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.2/.github/workflows/docs-build.yml` & `bm_utilities-0.1.3/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.2/.github/workflows/docs.yml` & `bm_utilities-0.1.3/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.2/.github/workflows/macos.yml` & `bm_utilities-0.1.3/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.2/.github/workflows/pypi.yml` & `bm_utilities-0.1.3/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.2/.github/workflows/ubuntu.yml` & `bm_utilities-0.1.3/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.2/.github/workflows/windows.yml` & `bm_utilities-0.1.3/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.2/.gitignore` & `bm_utilities-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.2/LICENSE` & `bm_utilities-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.2/PKG-INFO` & `bm_utilities-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bm_utilities
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python package for bm utilities
 Home-page: https://github.com/Youssefamroo/bm_utilities
 Author: youssef amr
 Author-email: usef.amr11@gmail.com
 License: MIT license
 Keywords: bm_utilities
 Classifier: Intended Audience :: Developers
```

### Comparing `bm_utilities-0.1.2/README.md` & `bm_utilities-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.2/bm_utilities/Address_finder.py` & `bm_utilities-0.1.3/bm_utilities/Address_finder.py`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.2/bm_utilities/bm_utilities.py` & `bm_utilities-0.1.3/bm_utilities/bm_utilities.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from bm_utilities import quality_gates as qg
 
 import geopandas as gpd
 import pandas as pd
 
 
 def address_finder(geodf,address):
-    construct = af(geodf)
+    construct = af.AddressFinder(geodf)
     address = construct.find_address(address)
     return address
 
 
 def quality_gates_check(df,config):
     my_gate = qg.QualityGates()
     df=my_gate.run_Quality_Gates(df,config)
```

### Comparing `bm_utilities-0.1.2/bm_utilities/quality_gates.py` & `bm_utilities-0.1.3/bm_utilities/quality_gates.py`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.2/bm_utilities.egg-info/PKG-INFO` & `bm_utilities-0.1.3/bm_utilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bm-utilities
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python package for bm utilities
 Home-page: https://github.com/Youssefamroo/bm_utilities
 Author: youssef amr
 Author-email: usef.amr11@gmail.com
 License: MIT license
 Keywords: bm_utilities
 Classifier: Intended Audience :: Developers
```

### Comparing `bm_utilities-0.1.2/bm_utilities.egg-info/SOURCES.txt` & `bm_utilities-0.1.3/bm_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.2/docs/contributing.md` & `bm_utilities-0.1.3/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.2/docs/installation.md` & `bm_utilities-0.1.3/docs/installation.md`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.2/mkdocs.yml` & `bm_utilities-0.1.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.2/setup.py` & `bm_utilities-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,10 +48,10 @@
     keywords='bm_utilities',
     name='bm_utilities',
     packages=find_packages(include=['bm_utilities', 'bm_utilities.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/Youssefamroo/bm_utilities',
-    version='0.1.2',
+    version='0.1.3',
     zip_safe=False,
 )
```

