# Comparing `tmp/bm_utilities-0.0.9.tar.gz` & `tmp/bm_utilities-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bm_utilities-0.0.9.tar", last modified: Thu May 18 10:06:23 2023, max compression
+gzip compressed data, was "bm_utilities-0.1.0.tar", last modified: Thu May 18 10:40:31 2023, max compression
```

## Comparing `bm_utilities-0.0.9.tar` & `bm_utilities-0.1.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 10:06:23.900130 bm_utilities-0.0.9/
--rw-rw-rw-   0        0        0      313 2023-04-24 13:32:39.000000 bm_utilities-0.0.9/.editorconfig
-drwxrwxrwx   0        0        0        0 2023-05-18 10:06:23.538135 bm_utilities-0.0.9/.github/
-drwxrwxrwx   0        0        0        0 2023-05-18 10:06:23.587133 bm_utilities-0.0.9/.github/ISSUE_TEMPLATE/
--rw-rw-rw-   0        0        0      537 2023-04-24 13:32:39.000000 bm_utilities-0.0.9/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-rw-   0        0        0      524 2023-04-24 13:32:39.000000 bm_utilities-0.0.9/.github/ISSUE_TEMPLATE/config.yml
--rw-rw-rw-   0        0        0      459 2023-04-24 13:32:39.000000 bm_utilities-0.0.9/.github/ISSUE_TEMPLATE/feature_request.md
-drwxrwxrwx   0        0        0        0 2023-05-18 10:06:23.607130 bm_utilities-0.0.9/.github/workflows/
--rw-rw-rw-   0        0        0     2125 2023-04-24 13:32:39.000000 bm_utilities-0.0.9/.github/workflows/docs-build.yml
--rw-rw-rw-   0        0        0     1041 2023-04-24 13:32:39.000000 bm_utilities-0.0.9/.github/workflows/docs.yml
--rw-rw-rw-   0        0        0     1076 2023-04-24 13:32:39.000000 bm_utilities-0.0.9/.github/workflows/macos.yml
--rw-rw-rw-   0        0        0     1032 2023-04-24 13:32:39.000000 bm_utilities-0.0.9/.github/workflows/pypi.yml
--rw-rw-rw-   0        0        0     1586 2023-04-24 13:32:39.000000 bm_utilities-0.0.9/.github/workflows/ubuntu.yml
--rw-rw-rw-   0        0        0      962 2023-04-24 13:32:39.000000 bm_utilities-0.0.9/.github/workflows/windows.yml
--rw-rw-rw-   0        0        0     1310 2023-04-24 13:32:39.000000 bm_utilities-0.0.9/.gitignore
--rw-rw-rw-   0        0        0     1092 2023-04-24 13:32:39.000000 bm_utilities-0.0.9/LICENSE
--rw-rw-rw-   0        0        0      129 2023-04-24 13:32:39.000000 bm_utilities-0.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0     1356 2023-05-18 10:06:23.900130 bm_utilities-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      610 2023-04-24 13:32:39.000000 bm_utilities-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 10:06:23.787129 bm_utilities-0.0.9/bm_utilities/
--rw-rw-rw-   0        0        0     4611 2023-05-18 10:03:49.000000 bm_utilities-0.0.9/bm_utilities/Address_finder.py
--rw-rw-rw-   0        0        0      136 2023-05-18 10:05:51.000000 bm_utilities-0.0.9/bm_utilities/__init__.py
--rw-rw-rw-   0        0        0     1134 2023-05-18 10:04:45.000000 bm_utilities-0.0.9/bm_utilities/bm_utilities.py
--rw-rw-rw-   0        0        0      194 2023-04-24 13:32:39.000000 bm_utilities-0.0.9/bm_utilities/common.py
--rw-rw-rw-   0        0        0    11097 2023-05-18 08:07:28.000000 bm_utilities-0.0.9/bm_utilities/quality_gates.py
-drwxrwxrwx   0        0        0        0 2023-05-18 10:06:23.856130 bm_utilities-0.0.9/bm_utilities.egg-info/
--rw-rw-rw-   0        0        0     1356 2023-05-18 10:06:22.000000 bm_utilities-0.0.9/bm_utilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      980 2023-05-18 10:06:23.000000 bm_utilities-0.0.9/bm_utilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 10:06:22.000000 bm_utilities-0.0.9/bm_utilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-18 10:06:22.000000 bm_utilities-0.0.9/bm_utilities.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-05-18 10:06:22.000000 bm_utilities-0.0.9/bm_utilities.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-18 10:06:23.881129 bm_utilities-0.0.9/docs/
--rw-rw-rw-   0        0        0       57 2023-04-24 13:32:39.000000 bm_utilities-0.0.9/docs/bm_utilities.md
--rw-rw-rw-   0        0        0       96 2023-04-24 13:32:39.000000 bm_utilities-0.0.9/docs/changelog.md
--rw-rw-rw-   0        0        0       42 2023-04-24 13:32:39.000000 bm_utilities-0.0.9/docs/common.md
--rw-rw-rw-   0        0        0     3303 2023-04-24 13:32:39.000000 bm_utilities-0.0.9/docs/contributing.md
-drwxrwxrwx   0        0        0        0 2023-05-18 10:06:23.884133 bm_utilities-0.0.9/docs/examples/
--rw-rw-rw-   0        0        0      309 2023-04-24 13:32:39.000000 bm_utilities-0.0.9/docs/examples/intro.ipynb
--rw-rw-rw-   0        0        0        7 2023-04-24 13:32:39.000000 bm_utilities-0.0.9/docs/faq.md
--rw-rw-rw-   0        0        0      502 2023-04-24 13:32:39.000000 bm_utilities-0.0.9/docs/index.md
--rw-rw-rw-   0        0        0      612 2023-04-24 13:32:39.000000 bm_utilities-0.0.9/docs/installation.md
-drwxrwxrwx   0        0        0        0 2023-05-18 10:06:23.888138 bm_utilities-0.0.9/docs/overrides/
--rw-rw-rw-   0        0        0      285 2023-04-24 13:32:39.000000 bm_utilities-0.0.9/docs/overrides/main.html
--rw-rw-rw-   0        0        0       79 2023-04-24 13:32:39.000000 bm_utilities-0.0.9/docs/usage.md
--rw-rw-rw-   0        0        0     2242 2023-04-24 13:32:39.000000 bm_utilities-0.0.9/mkdocs.yml
--rw-rw-rw-   0        0        0        0 2023-04-24 13:32:39.000000 bm_utilities-0.0.9/requirements.txt
--rw-rw-rw-   0        0        0      148 2023-04-24 20:57:32.000000 bm_utilities-0.0.9/requirements_dev.txt
--rw-rw-rw-   0        0        0      371 2023-04-24 13:32:39.000000 bm_utilities-0.0.9/requirements_docs.txt
--rw-rw-rw-   0        0        0      420 2023-05-18 10:06:23.903136 bm_utilities-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1771 2023-05-18 10:05:44.000000 bm_utilities-0.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-18 10:06:23.896129 bm_utilities-0.0.9/tests/
--rw-rw-rw-   0        0        0       43 2023-04-24 13:32:39.000000 bm_utilities-0.0.9/tests/__init__.py
--rw-rw-rw-   0        0        0      433 2023-04-24 13:32:39.000000 bm_utilities-0.0.9/tests/test_bm_utilities.py
+drwxrwxrwx   0        0        0        0 2023-05-18 10:40:31.367077 bm_utilities-0.1.0/
+-rw-rw-rw-   0        0        0      313 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/.editorconfig
+drwxrwxrwx   0        0        0        0 2023-05-18 10:40:31.135114 bm_utilities-0.1.0/.github/
+drwxrwxrwx   0        0        0        0 2023-05-18 10:40:31.188073 bm_utilities-0.1.0/.github/ISSUE_TEMPLATE/
+-rw-rw-rw-   0        0        0      537 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-rw-   0        0        0      524 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-rw-rw-   0        0        0      459 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxrwxrwx   0        0        0        0 2023-05-18 10:40:31.207072 bm_utilities-0.1.0/.github/workflows/
+-rw-rw-rw-   0        0        0     2125 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/.github/workflows/docs-build.yml
+-rw-rw-rw-   0        0        0     1041 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/.github/workflows/docs.yml
+-rw-rw-rw-   0        0        0     1076 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/.github/workflows/macos.yml
+-rw-rw-rw-   0        0        0     1032 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/.github/workflows/pypi.yml
+-rw-rw-rw-   0        0        0     1586 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/.github/workflows/ubuntu.yml
+-rw-rw-rw-   0        0        0      962 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/.github/workflows/windows.yml
+-rw-rw-rw-   0        0        0     1310 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/.gitignore
+-rw-rw-rw-   0        0        0     1092 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      129 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1356 2023-05-18 10:40:31.367077 bm_utilities-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      610 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 10:40:31.312073 bm_utilities-0.1.0/bm_utilities/
+-rw-rw-rw-   0        0        0     4611 2023-05-18 10:03:49.000000 bm_utilities-0.1.0/bm_utilities/Address_finder.py
+-rw-rw-rw-   0        0        0      136 2023-05-18 10:40:12.000000 bm_utilities-0.1.0/bm_utilities/__init__.py
+-rw-rw-rw-   0        0        0     1134 2023-05-18 10:39:24.000000 bm_utilities-0.1.0/bm_utilities/bm_utilities.py
+-rw-rw-rw-   0        0        0      194 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/bm_utilities/common.py
+-rw-rw-rw-   0        0        0    11097 2023-05-18 08:07:28.000000 bm_utilities-0.1.0/bm_utilities/quality_gates.py
+drwxrwxrwx   0        0        0        0 2023-05-18 10:40:31.327070 bm_utilities-0.1.0/bm_utilities.egg-info/
+-rw-rw-rw-   0        0        0     1356 2023-05-18 10:40:30.000000 bm_utilities-0.1.0/bm_utilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      980 2023-05-18 10:40:31.000000 bm_utilities-0.1.0/bm_utilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 10:40:30.000000 bm_utilities-0.1.0/bm_utilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-18 10:40:30.000000 bm_utilities-0.1.0/bm_utilities.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-05-18 10:40:30.000000 bm_utilities-0.1.0/bm_utilities.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 10:40:31.352073 bm_utilities-0.1.0/docs/
+-rw-rw-rw-   0        0        0       57 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/docs/bm_utilities.md
+-rw-rw-rw-   0        0        0       96 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/docs/changelog.md
+-rw-rw-rw-   0        0        0       42 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/docs/common.md
+-rw-rw-rw-   0        0        0     3303 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/docs/contributing.md
+drwxrwxrwx   0        0        0        0 2023-05-18 10:40:31.354067 bm_utilities-0.1.0/docs/examples/
+-rw-rw-rw-   0        0        0      309 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/docs/examples/intro.ipynb
+-rw-rw-rw-   0        0        0        7 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/docs/faq.md
+-rw-rw-rw-   0        0        0      502 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/docs/index.md
+-rw-rw-rw-   0        0        0      612 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/docs/installation.md
+drwxrwxrwx   0        0        0        0 2023-05-18 10:40:31.356069 bm_utilities-0.1.0/docs/overrides/
+-rw-rw-rw-   0        0        0      285 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/docs/overrides/main.html
+-rw-rw-rw-   0        0        0       79 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/docs/usage.md
+-rw-rw-rw-   0        0        0     2242 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/mkdocs.yml
+-rw-rw-rw-   0        0        0        0 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/requirements.txt
+-rw-rw-rw-   0        0        0      148 2023-04-24 20:57:32.000000 bm_utilities-0.1.0/requirements_dev.txt
+-rw-rw-rw-   0        0        0      371 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/requirements_docs.txt
+-rw-rw-rw-   0        0        0      420 2023-05-18 10:40:31.369070 bm_utilities-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1771 2023-05-18 10:40:00.000000 bm_utilities-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 10:40:31.363075 bm_utilities-0.1.0/tests/
+-rw-rw-rw-   0        0        0       43 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      433 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/tests/test_bm_utilities.py
```

### Comparing `bm_utilities-0.0.9/.github/ISSUE_TEMPLATE/bug_report.md` & `bm_utilities-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.0.9/.github/ISSUE_TEMPLATE/config.yml` & `bm_utilities-0.1.0/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.0.9/.github/workflows/docs-build.yml` & `bm_utilities-0.1.0/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.0.9/.github/workflows/docs.yml` & `bm_utilities-0.1.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.0.9/.github/workflows/macos.yml` & `bm_utilities-0.1.0/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.0.9/.github/workflows/pypi.yml` & `bm_utilities-0.1.0/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.0.9/.github/workflows/ubuntu.yml` & `bm_utilities-0.1.0/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.0.9/.github/workflows/windows.yml` & `bm_utilities-0.1.0/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.0.9/.gitignore` & `bm_utilities-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.0.9/LICENSE` & `bm_utilities-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.0.9/PKG-INFO` & `bm_utilities-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bm_utilities
-Version: 0.0.9
+Version: 0.1.0
 Summary: A Python package for bm utilities
 Home-page: https://github.com/Youssefamroo/bm_utilities
 Author: youssef amr
 Author-email: usef.amr11@gmail.com
 License: MIT license
 Keywords: bm_utilities
 Classifier: Intended Audience :: Developers
```

### Comparing `bm_utilities-0.0.9/README.md` & `bm_utilities-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.0.9/bm_utilities/Address_finder.py` & `bm_utilities-0.1.0/bm_utilities/Address_finder.py`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.0.9/bm_utilities/bm_utilities.py` & `bm_utilities-0.1.0/bm_utilities/bm_utilities.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from Address_finder import AddressFinder as af
+from bm_utilities import Address_finder as af
 import geopandas as gpd
 import pandas as pd
 import quality_gates as qg
 
 
 
-class address_finder:
-    def __init__(self,geo_df):
-        self.construct = af(geo_df)
-    def get_address(self,address):
-        return self.construct.find_address(address)
+#class address_finder:
+#    def __init__(self,geo_df):
+#        self.construct = af(geo_df)
+#    def get_address(self,address):
+#        return self.construct.find_address(address)
 
 
-#def address_finder(geodf,address):
-#    construct = af(geodf)
-#    address = construct.find_address(address)
-#    return address
+def address_finder(geodf,address):
+    construct = af(geodf)
+    address = construct.find_address(address)
+    return address
 
 
 def quality_gates_check(df,config):
     my_gate = qg.QualityGates()
     df=my_gate.run_Quality_Gates(df,config)
     return df
```

### Comparing `bm_utilities-0.0.9/bm_utilities/quality_gates.py` & `bm_utilities-0.1.0/bm_utilities/quality_gates.py`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.0.9/bm_utilities.egg-info/PKG-INFO` & `bm_utilities-0.1.0/bm_utilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bm-utilities
-Version: 0.0.9
+Version: 0.1.0
 Summary: A Python package for bm utilities
 Home-page: https://github.com/Youssefamroo/bm_utilities
 Author: youssef amr
 Author-email: usef.amr11@gmail.com
 License: MIT license
 Keywords: bm_utilities
 Classifier: Intended Audience :: Developers
```

### Comparing `bm_utilities-0.0.9/bm_utilities.egg-info/SOURCES.txt` & `bm_utilities-0.1.0/bm_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.0.9/docs/contributing.md` & `bm_utilities-0.1.0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.0.9/docs/installation.md` & `bm_utilities-0.1.0/docs/installation.md`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.0.9/mkdocs.yml` & `bm_utilities-0.1.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.0.9/setup.py` & `bm_utilities-0.1.0/setup.py`

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
-    version='0.0.9',
+    version='0.1.0',
     zip_safe=False,
 )
```

