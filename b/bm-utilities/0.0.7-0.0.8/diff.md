# Comparing `tmp/bm_utilities-0.0.7.tar.gz` & `tmp/bm_utilities-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bm_utilities-0.0.7.tar", last modified: Mon May 15 12:30:26 2023, max compression
+gzip compressed data, was "bm_utilities-0.0.8.tar", last modified: Thu May 18 08:12:58 2023, max compression
```

## Comparing `bm_utilities-0.0.7.tar` & `bm_utilities-0.0.8.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 12:30:26.643794 bm_utilities-0.0.7/
--rw-rw-rw-   0        0        0      313 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/.editorconfig
-drwxrwxrwx   0        0        0        0 2023-05-15 12:30:26.491794 bm_utilities-0.0.7/.github/
-drwxrwxrwx   0        0        0        0 2023-05-15 12:30:26.530241 bm_utilities-0.0.7/.github/ISSUE_TEMPLATE/
--rw-rw-rw-   0        0        0      537 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-rw-   0        0        0      524 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/.github/ISSUE_TEMPLATE/config.yml
--rw-rw-rw-   0        0        0      459 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/.github/ISSUE_TEMPLATE/feature_request.md
-drwxrwxrwx   0        0        0        0 2023-05-15 12:30:26.544733 bm_utilities-0.0.7/.github/workflows/
--rw-rw-rw-   0        0        0     2125 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/.github/workflows/docs-build.yml
--rw-rw-rw-   0        0        0     1041 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/.github/workflows/docs.yml
--rw-rw-rw-   0        0        0     1076 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/.github/workflows/macos.yml
--rw-rw-rw-   0        0        0     1032 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/.github/workflows/pypi.yml
--rw-rw-rw-   0        0        0     1586 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/.github/workflows/ubuntu.yml
--rw-rw-rw-   0        0        0      962 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/.github/workflows/windows.yml
--rw-rw-rw-   0        0        0     1310 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/.gitignore
--rw-rw-rw-   0        0        0     1092 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      129 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1356 2023-05-15 12:30:26.644796 bm_utilities-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      610 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 12:30:26.595713 bm_utilities-0.0.7/bm_utilities/
--rw-rw-rw-   0        0        0     4605 2023-05-15 12:10:28.000000 bm_utilities-0.0.7/bm_utilities/Address_finder.py
--rw-rw-rw-   0        0        0      136 2023-05-15 12:30:20.000000 bm_utilities-0.0.7/bm_utilities/__init__.py
--rw-rw-rw-   0        0        0      231 2023-05-15 12:28:50.000000 bm_utilities-0.0.7/bm_utilities/bm_utilities.py
--rw-rw-rw-   0        0        0      194 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/bm_utilities/common.py
-drwxrwxrwx   0        0        0        0 2023-05-15 12:30:26.609534 bm_utilities-0.0.7/bm_utilities.egg-info/
--rw-rw-rw-   0        0        0     1356 2023-05-15 12:30:26.000000 bm_utilities-0.0.7/bm_utilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      950 2023-05-15 12:30:26.000000 bm_utilities-0.0.7/bm_utilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 12:30:26.000000 bm_utilities-0.0.7/bm_utilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-25 12:05:59.000000 bm_utilities-0.0.7/bm_utilities.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-05-15 12:30:26.000000 bm_utilities-0.0.7/bm_utilities.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-15 12:30:26.630797 bm_utilities-0.0.7/docs/
--rw-rw-rw-   0        0        0       57 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/docs/bm_utilities.md
--rw-rw-rw-   0        0        0       96 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/docs/changelog.md
--rw-rw-rw-   0        0        0       42 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/docs/common.md
--rw-rw-rw-   0        0        0     3303 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/docs/contributing.md
-drwxrwxrwx   0        0        0        0 2023-05-15 12:30:26.632796 bm_utilities-0.0.7/docs/examples/
--rw-rw-rw-   0        0        0      309 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/docs/examples/intro.ipynb
--rw-rw-rw-   0        0        0        7 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/docs/faq.md
--rw-rw-rw-   0        0        0      502 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/docs/index.md
--rw-rw-rw-   0        0        0      612 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/docs/installation.md
-drwxrwxrwx   0        0        0        0 2023-05-15 12:30:26.634805 bm_utilities-0.0.7/docs/overrides/
--rw-rw-rw-   0        0        0      285 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/docs/overrides/main.html
--rw-rw-rw-   0        0        0       79 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/docs/usage.md
--rw-rw-rw-   0        0        0     2242 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/mkdocs.yml
--rw-rw-rw-   0        0        0        0 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/requirements.txt
--rw-rw-rw-   0        0        0      148 2023-04-24 20:57:32.000000 bm_utilities-0.0.7/requirements_dev.txt
--rw-rw-rw-   0        0        0      371 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/requirements_docs.txt
--rw-rw-rw-   0        0        0      420 2023-05-15 12:30:26.645795 bm_utilities-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1771 2023-05-15 12:30:14.000000 bm_utilities-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-15 12:30:26.640798 bm_utilities-0.0.7/tests/
--rw-rw-rw-   0        0        0       43 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/tests/__init__.py
--rw-rw-rw-   0        0        0      433 2023-04-24 13:32:39.000000 bm_utilities-0.0.7/tests/test_bm_utilities.py
+drwxrwxrwx   0        0        0        0 2023-05-18 08:12:58.383741 bm_utilities-0.0.8/
+-rw-rw-rw-   0        0        0      313 2023-04-24 13:32:39.000000 bm_utilities-0.0.8/.editorconfig
+drwxrwxrwx   0        0        0        0 2023-05-18 08:12:58.177659 bm_utilities-0.0.8/.github/
+drwxrwxrwx   0        0        0        0 2023-05-18 08:12:58.220665 bm_utilities-0.0.8/.github/ISSUE_TEMPLATE/
+-rw-rw-rw-   0        0        0      537 2023-04-24 13:32:39.000000 bm_utilities-0.0.8/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-rw-   0        0        0      524 2023-04-24 13:32:39.000000 bm_utilities-0.0.8/.github/ISSUE_TEMPLATE/config.yml
+-rw-rw-rw-   0        0        0      459 2023-04-24 13:32:39.000000 bm_utilities-0.0.8/.github/ISSUE_TEMPLATE/feature_request.md
+drwxrwxrwx   0        0        0        0 2023-05-18 08:12:58.236659 bm_utilities-0.0.8/.github/workflows/
+-rw-rw-rw-   0        0        0     2125 2023-04-24 13:32:39.000000 bm_utilities-0.0.8/.github/workflows/docs-build.yml
+-rw-rw-rw-   0        0        0     1041 2023-04-24 13:32:39.000000 bm_utilities-0.0.8/.github/workflows/docs.yml
+-rw-rw-rw-   0        0        0     1076 2023-04-24 13:32:39.000000 bm_utilities-0.0.8/.github/workflows/macos.yml
+-rw-rw-rw-   0        0        0     1032 2023-04-24 13:32:39.000000 bm_utilities-0.0.8/.github/workflows/pypi.yml
+-rw-rw-rw-   0        0        0     1586 2023-04-24 13:32:39.000000 bm_utilities-0.0.8/.github/workflows/ubuntu.yml
+-rw-rw-rw-   0        0        0      962 2023-04-24 13:32:39.000000 bm_utilities-0.0.8/.github/workflows/windows.yml
+-rw-rw-rw-   0        0        0     1310 2023-04-24 13:32:39.000000 bm_utilities-0.0.8/.gitignore
+-rw-rw-rw-   0        0        0     1092 2023-04-24 13:32:39.000000 bm_utilities-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      129 2023-04-24 13:32:39.000000 bm_utilities-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     1356 2023-05-18 08:12:58.383741 bm_utilities-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      610 2023-04-24 13:32:39.000000 bm_utilities-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 08:12:58.326743 bm_utilities-0.0.8/bm_utilities/
+-rw-rw-rw-   0        0        0     4608 2023-05-18 07:55:38.000000 bm_utilities-0.0.8/bm_utilities/Address_finder.py
+-rw-rw-rw-   0        0        0      136 2023-05-18 08:12:43.000000 bm_utilities-0.0.8/bm_utilities/__init__.py
+-rw-rw-rw-   0        0        0      935 2023-05-18 08:10:32.000000 bm_utilities-0.0.8/bm_utilities/bm_utilities.py
+-rw-rw-rw-   0        0        0      194 2023-04-24 13:32:39.000000 bm_utilities-0.0.8/bm_utilities/common.py
+-rw-rw-rw-   0        0        0    11097 2023-05-18 08:07:28.000000 bm_utilities-0.0.8/bm_utilities/quality_gates.py
+drwxrwxrwx   0        0        0        0 2023-05-18 08:12:58.342744 bm_utilities-0.0.8/bm_utilities.egg-info/
+-rw-rw-rw-   0        0        0     1356 2023-05-18 08:12:57.000000 bm_utilities-0.0.8/bm_utilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      980 2023-05-18 08:12:58.000000 bm_utilities-0.0.8/bm_utilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 08:12:57.000000 bm_utilities-0.0.8/bm_utilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-18 08:12:57.000000 bm_utilities-0.0.8/bm_utilities.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-05-18 08:12:57.000000 bm_utilities-0.0.8/bm_utilities.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 08:12:58.367747 bm_utilities-0.0.8/docs/
+-rw-rw-rw-   0        0        0       57 2023-04-24 13:32:39.000000 bm_utilities-0.0.8/docs/bm_utilities.md
+-rw-rw-rw-   0        0        0       96 2023-04-24 13:32:39.000000 bm_utilities-0.0.8/docs/changelog.md
+-rw-rw-rw-   0        0        0       42 2023-04-24 13:32:39.000000 bm_utilities-0.0.8/docs/common.md
+-rw-rw-rw-   0        0        0     3303 2023-04-24 13:32:39.000000 bm_utilities-0.0.8/docs/contributing.md
+drwxrwxrwx   0        0        0        0 2023-05-18 08:12:58.371744 bm_utilities-0.0.8/docs/examples/
+-rw-rw-rw-   0        0        0      309 2023-04-24 13:32:39.000000 bm_utilities-0.0.8/docs/examples/intro.ipynb
+-rw-rw-rw-   0        0        0        7 2023-04-24 13:32:39.000000 bm_utilities-0.0.8/docs/faq.md
+-rw-rw-rw-   0        0        0      502 2023-04-24 13:32:39.000000 bm_utilities-0.0.8/docs/index.md
+-rw-rw-rw-   0        0        0      612 2023-04-24 13:32:39.000000 bm_utilities-0.0.8/docs/installation.md
+drwxrwxrwx   0        0        0        0 2023-05-18 08:12:58.374743 bm_utilities-0.0.8/docs/overrides/
+-rw-rw-rw-   0        0        0      285 2023-04-24 13:32:39.000000 bm_utilities-0.0.8/docs/overrides/main.html
+-rw-rw-rw-   0        0        0       79 2023-04-24 13:32:39.000000 bm_utilities-0.0.8/docs/usage.md
+-rw-rw-rw-   0        0        0     2242 2023-04-24 13:32:39.000000 bm_utilities-0.0.8/mkdocs.yml
+-rw-rw-rw-   0        0        0        0 2023-04-24 13:32:39.000000 bm_utilities-0.0.8/requirements.txt
+-rw-rw-rw-   0        0        0      148 2023-04-24 20:57:32.000000 bm_utilities-0.0.8/requirements_dev.txt
+-rw-rw-rw-   0        0        0      371 2023-04-24 13:32:39.000000 bm_utilities-0.0.8/requirements_docs.txt
+-rw-rw-rw-   0        0        0      420 2023-05-18 08:12:58.385743 bm_utilities-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1771 2023-05-18 08:12:48.000000 bm_utilities-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 08:12:58.380746 bm_utilities-0.0.8/tests/
+-rw-rw-rw-   0        0        0       43 2023-04-24 13:32:39.000000 bm_utilities-0.0.8/tests/__init__.py
+-rw-rw-rw-   0        0        0      433 2023-04-24 13:32:39.000000 bm_utilities-0.0.8/tests/test_bm_utilities.py
```

### Comparing `bm_utilities-0.0.7/.github/ISSUE_TEMPLATE/bug_report.md` & `bm_utilities-0.0.8/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.0.7/.github/ISSUE_TEMPLATE/config.yml` & `bm_utilities-0.0.8/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.0.7/.github/workflows/docs-build.yml` & `bm_utilities-0.0.8/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.0.7/.github/workflows/docs.yml` & `bm_utilities-0.0.8/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.0.7/.github/workflows/macos.yml` & `bm_utilities-0.0.8/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.0.7/.github/workflows/pypi.yml` & `bm_utilities-0.0.8/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.0.7/.github/workflows/ubuntu.yml` & `bm_utilities-0.0.8/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.0.7/.github/workflows/windows.yml` & `bm_utilities-0.0.8/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.0.7/.gitignore` & `bm_utilities-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.0.7/LICENSE` & `bm_utilities-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.0.7/PKG-INFO` & `bm_utilities-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bm_utilities
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Python package for bm utilities
 Home-page: https://github.com/Youssefamroo/bm_utilities
 Author: youssef amr
 Author-email: usef.amr11@gmail.com
 License: MIT license
 Keywords: bm_utilities
 Classifier: Intended Audience :: Developers
```

### Comparing `bm_utilities-0.0.7/README.md` & `bm_utilities-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.0.7/bm_utilities/Address_finder.py` & `bm_utilities-0.0.8/bm_utilities/Address_finder.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     import pyarabic.araby as araby
 
 except ImportError:
     raise ImportError(
         "pyarabic needs to be installed to use this module. Use 'pip install pyarabic' to install the package. See https://deckgl.readthedocs.io/en/latest/installation.html for more details."
     )
 
-def clean_text(custom_stopwords=None, punctuation=None):
+def clean_text(text,custom_stopwords=None, punctuation=None):
         """clean data from any stopwords , punctuation and english litters
          input:
          if the input was list :
          list.apply(lambda text : clean_text(text))
          :return : clean Arabic text
          """
         custom_stopwords = custom_stopwords or ["رقم", "طريق", "شقة", "شقه", "القطع", "ارقام", 
@@ -96,14 +96,13 @@
         portal
         for address_1 ,idz ,_ in zip(data_0_100k["full_address"], data_0_100k["CUSTOMER_ID"],tqdm(range(len(data_0_100k)))):
             single_line_address = " مصر "+ str(address_1)
             single_line_address = clean_text(single_line_address)
             geocode_results = geocode(single_line_address)
             if len(geocode_results) != 0 :
                 country = geocode_results[0]["attributes"].get("Country",np.nan)
-
                 if country == 'EGY':
                     Latitude = geocode_results[0]["location"].get("y",np.NAN)
                     Longitude =  geocode_results[0]["location"].get("x",np.NAN)
                     input_data = pd.DataFrame({"Latitude":Latitude,"Longitude":Longitude,"address":address_1,"id":idz},index=[0])
                     self.address.append(PolygonFinder(self.polygons,Latitude,Longitude))
         return self.address
```

### Comparing `bm_utilities-0.0.7/bm_utilities.egg-info/PKG-INFO` & `bm_utilities-0.0.8/bm_utilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bm-utilities
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Python package for bm utilities
 Home-page: https://github.com/Youssefamroo/bm_utilities
 Author: youssef amr
 Author-email: usef.amr11@gmail.com
 License: MIT license
 Keywords: bm_utilities
 Classifier: Intended Audience :: Developers
```

### Comparing `bm_utilities-0.0.7/bm_utilities.egg-info/SOURCES.txt` & `bm_utilities-0.0.8/bm_utilities.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 .github/workflows/pypi.yml
 .github/workflows/ubuntu.yml
 .github/workflows/windows.yml
 bm_utilities/Address_finder.py
 bm_utilities/__init__.py
 bm_utilities/bm_utilities.py
 bm_utilities/common.py
+bm_utilities/quality_gates.py
 bm_utilities.egg-info/PKG-INFO
 bm_utilities.egg-info/SOURCES.txt
 bm_utilities.egg-info/dependency_links.txt
 bm_utilities.egg-info/not-zip-safe
 bm_utilities.egg-info/top_level.txt
 docs/bm_utilities.md
 docs/changelog.md
```

### Comparing `bm_utilities-0.0.7/docs/contributing.md` & `bm_utilities-0.0.8/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.0.7/docs/installation.md` & `bm_utilities-0.0.8/docs/installation.md`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.0.7/mkdocs.yml` & `bm_utilities-0.0.8/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.0.7/setup.py` & `bm_utilities-0.0.8/setup.py`

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
-    version='0.0.7',
+    version='0.0.8',
     zip_safe=False,
 )
```

