# Comparing `tmp/bm_utilities-0.1.0.tar.gz` & `tmp/bm_utilities-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bm_utilities-0.1.0.tar", last modified: Thu May 18 10:40:31 2023, max compression
+gzip compressed data, was "bm_utilities-0.1.1.tar", last modified: Thu May 18 11:02:07 2023, max compression
```

## Comparing `bm_utilities-0.1.0.tar` & `bm_utilities-0.1.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 10:40:31.367077 bm_utilities-0.1.0/
--rw-rw-rw-   0        0        0      313 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/.editorconfig
-drwxrwxrwx   0        0        0        0 2023-05-18 10:40:31.135114 bm_utilities-0.1.0/.github/
-drwxrwxrwx   0        0        0        0 2023-05-18 10:40:31.188073 bm_utilities-0.1.0/.github/ISSUE_TEMPLATE/
--rw-rw-rw-   0        0        0      537 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-rw-   0        0        0      524 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/.github/ISSUE_TEMPLATE/config.yml
--rw-rw-rw-   0        0        0      459 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxrwxrwx   0        0        0        0 2023-05-18 10:40:31.207072 bm_utilities-0.1.0/.github/workflows/
--rw-rw-rw-   0        0        0     2125 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/.github/workflows/docs-build.yml
--rw-rw-rw-   0        0        0     1041 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/.github/workflows/docs.yml
--rw-rw-rw-   0        0        0     1076 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/.github/workflows/macos.yml
--rw-rw-rw-   0        0        0     1032 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/.github/workflows/pypi.yml
--rw-rw-rw-   0        0        0     1586 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/.github/workflows/ubuntu.yml
--rw-rw-rw-   0        0        0      962 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/.github/workflows/windows.yml
--rw-rw-rw-   0        0        0     1310 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/.gitignore
--rw-rw-rw-   0        0        0     1092 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      129 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1356 2023-05-18 10:40:31.367077 bm_utilities-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      610 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 10:40:31.312073 bm_utilities-0.1.0/bm_utilities/
--rw-rw-rw-   0        0        0     4611 2023-05-18 10:03:49.000000 bm_utilities-0.1.0/bm_utilities/Address_finder.py
--rw-rw-rw-   0        0        0      136 2023-05-18 10:40:12.000000 bm_utilities-0.1.0/bm_utilities/__init__.py
--rw-rw-rw-   0        0        0     1134 2023-05-18 10:39:24.000000 bm_utilities-0.1.0/bm_utilities/bm_utilities.py
--rw-rw-rw-   0        0        0      194 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/bm_utilities/common.py
--rw-rw-rw-   0        0        0    11097 2023-05-18 08:07:28.000000 bm_utilities-0.1.0/bm_utilities/quality_gates.py
-drwxrwxrwx   0        0        0        0 2023-05-18 10:40:31.327070 bm_utilities-0.1.0/bm_utilities.egg-info/
--rw-rw-rw-   0        0        0     1356 2023-05-18 10:40:30.000000 bm_utilities-0.1.0/bm_utilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      980 2023-05-18 10:40:31.000000 bm_utilities-0.1.0/bm_utilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 10:40:30.000000 bm_utilities-0.1.0/bm_utilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-18 10:40:30.000000 bm_utilities-0.1.0/bm_utilities.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-05-18 10:40:30.000000 bm_utilities-0.1.0/bm_utilities.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-18 10:40:31.352073 bm_utilities-0.1.0/docs/
--rw-rw-rw-   0        0        0       57 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/docs/bm_utilities.md
--rw-rw-rw-   0        0        0       96 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/docs/changelog.md
--rw-rw-rw-   0        0        0       42 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/docs/common.md
--rw-rw-rw-   0        0        0     3303 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/docs/contributing.md
-drwxrwxrwx   0        0        0        0 2023-05-18 10:40:31.354067 bm_utilities-0.1.0/docs/examples/
--rw-rw-rw-   0        0        0      309 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/docs/examples/intro.ipynb
--rw-rw-rw-   0        0        0        7 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/docs/faq.md
--rw-rw-rw-   0        0        0      502 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/docs/index.md
--rw-rw-rw-   0        0        0      612 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/docs/installation.md
-drwxrwxrwx   0        0        0        0 2023-05-18 10:40:31.356069 bm_utilities-0.1.0/docs/overrides/
--rw-rw-rw-   0        0        0      285 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/docs/overrides/main.html
--rw-rw-rw-   0        0        0       79 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/docs/usage.md
--rw-rw-rw-   0        0        0     2242 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/mkdocs.yml
--rw-rw-rw-   0        0        0        0 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/requirements.txt
--rw-rw-rw-   0        0        0      148 2023-04-24 20:57:32.000000 bm_utilities-0.1.0/requirements_dev.txt
--rw-rw-rw-   0        0        0      371 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/requirements_docs.txt
--rw-rw-rw-   0        0        0      420 2023-05-18 10:40:31.369070 bm_utilities-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1771 2023-05-18 10:40:00.000000 bm_utilities-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-18 10:40:31.363075 bm_utilities-0.1.0/tests/
--rw-rw-rw-   0        0        0       43 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0      433 2023-04-24 13:32:39.000000 bm_utilities-0.1.0/tests/test_bm_utilities.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:02:07.076290 bm_utilities-0.1.1/
+-rw-rw-rw-   0        0        0      313 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/.editorconfig
+drwxrwxrwx   0        0        0        0 2023-05-18 11:02:06.781283 bm_utilities-0.1.1/.github/
+drwxrwxrwx   0        0        0        0 2023-05-18 11:02:06.831283 bm_utilities-0.1.1/.github/ISSUE_TEMPLATE/
+-rw-rw-rw-   0        0        0      537 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-rw-   0        0        0      524 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-rw-rw-   0        0        0      459 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md
+drwxrwxrwx   0        0        0        0 2023-05-18 11:02:06.850284 bm_utilities-0.1.1/.github/workflows/
+-rw-rw-rw-   0        0        0     2125 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/.github/workflows/docs-build.yml
+-rw-rw-rw-   0        0        0     1041 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/.github/workflows/docs.yml
+-rw-rw-rw-   0        0        0     1076 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/.github/workflows/macos.yml
+-rw-rw-rw-   0        0        0     1032 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/.github/workflows/pypi.yml
+-rw-rw-rw-   0        0        0     1586 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/.github/workflows/ubuntu.yml
+-rw-rw-rw-   0        0        0      962 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/.github/workflows/windows.yml
+-rw-rw-rw-   0        0        0     1310 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/.gitignore
+-rw-rw-rw-   0        0        0     1092 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      129 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1356 2023-05-18 11:02:07.077283 bm_utilities-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      610 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 11:02:07.015283 bm_utilities-0.1.1/bm_utilities/
+-rw-rw-rw-   0        0        0     5068 2023-05-18 11:00:54.000000 bm_utilities-0.1.1/bm_utilities/Address_finder.py
+-rw-rw-rw-   0        0        0      136 2023-05-18 11:01:42.000000 bm_utilities-0.1.1/bm_utilities/__init__.py
+-rw-rw-rw-   0        0        0     1067 2023-05-18 11:00:50.000000 bm_utilities-0.1.1/bm_utilities/bm_utilities.py
+-rw-rw-rw-   0        0        0      194 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/bm_utilities/common.py
+-rw-rw-rw-   0        0        0    11097 2023-05-18 08:07:28.000000 bm_utilities-0.1.1/bm_utilities/quality_gates.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:02:07.032282 bm_utilities-0.1.1/bm_utilities.egg-info/
+-rw-rw-rw-   0        0        0     1356 2023-05-18 11:02:06.000000 bm_utilities-0.1.1/bm_utilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      980 2023-05-18 11:02:06.000000 bm_utilities-0.1.1/bm_utilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 11:02:06.000000 bm_utilities-0.1.1/bm_utilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-18 11:02:06.000000 bm_utilities-0.1.1/bm_utilities.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-05-18 11:02:06.000000 bm_utilities-0.1.1/bm_utilities.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 11:02:07.057289 bm_utilities-0.1.1/docs/
+-rw-rw-rw-   0        0        0       57 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/docs/bm_utilities.md
+-rw-rw-rw-   0        0        0       96 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/docs/changelog.md
+-rw-rw-rw-   0        0        0       42 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/docs/common.md
+-rw-rw-rw-   0        0        0     3303 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/docs/contributing.md
+drwxrwxrwx   0        0        0        0 2023-05-18 11:02:07.061282 bm_utilities-0.1.1/docs/examples/
+-rw-rw-rw-   0        0        0      309 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/docs/examples/intro.ipynb
+-rw-rw-rw-   0        0        0        7 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/docs/faq.md
+-rw-rw-rw-   0        0        0      502 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/docs/index.md
+-rw-rw-rw-   0        0        0      612 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/docs/installation.md
+drwxrwxrwx   0        0        0        0 2023-05-18 11:02:07.064282 bm_utilities-0.1.1/docs/overrides/
+-rw-rw-rw-   0        0        0      285 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/docs/overrides/main.html
+-rw-rw-rw-   0        0        0       79 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/docs/usage.md
+-rw-rw-rw-   0        0        0     2242 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/mkdocs.yml
+-rw-rw-rw-   0        0        0        0 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/requirements.txt
+-rw-rw-rw-   0        0        0      148 2023-04-24 20:57:32.000000 bm_utilities-0.1.1/requirements_dev.txt
+-rw-rw-rw-   0        0        0      371 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/requirements_docs.txt
+-rw-rw-rw-   0        0        0      420 2023-05-18 11:02:07.079285 bm_utilities-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1771 2023-05-18 11:01:34.000000 bm_utilities-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:02:07.071287 bm_utilities-0.1.1/tests/
+-rw-rw-rw-   0        0        0       43 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      433 2023-04-24 13:32:39.000000 bm_utilities-0.1.1/tests/test_bm_utilities.py
```

### Comparing `bm_utilities-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md` & `bm_utilities-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.0/.github/ISSUE_TEMPLATE/config.yml` & `bm_utilities-0.1.1/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.0/.github/workflows/docs-build.yml` & `bm_utilities-0.1.1/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.0/.github/workflows/docs.yml` & `bm_utilities-0.1.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.0/.github/workflows/macos.yml` & `bm_utilities-0.1.1/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.0/.github/workflows/pypi.yml` & `bm_utilities-0.1.1/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.0/.github/workflows/ubuntu.yml` & `bm_utilities-0.1.1/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.0/.github/workflows/windows.yml` & `bm_utilities-0.1.1/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.0/.gitignore` & `bm_utilities-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.0/LICENSE` & `bm_utilities-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.0/PKG-INFO` & `bm_utilities-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bm_utilities
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package for bm utilities
 Home-page: https://github.com/Youssefamroo/bm_utilities
 Author: youssef amr
 Author-email: usef.amr11@gmail.com
 License: MIT license
 Keywords: bm_utilities
 Classifier: Intended Audience :: Developers
```

### Comparing `bm_utilities-0.1.0/README.md` & `bm_utilities-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.0/bm_utilities/Address_finder.py` & `bm_utilities-0.1.1/bm_utilities/Address_finder.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,55 +30,18 @@
     import pyarabic.araby as araby
 
 except ImportError:
     raise ImportError(
         "pyarabic needs to be installed to use this module. Use 'pip install pyarabic' to install the package. See https://deckgl.readthedocs.io/en/latest/installation.html for more details."
     )
 
-def clean_text(text,custom_stopwords=None, punctuation=None):
-        """clean data from any stopwords , punctuation and english litters
-         input:
-         if the input was list :
-         list.apply(lambda text : clean_text(text))
-         :return : clean Arabic text
-         """
-        custom_stopwords = custom_stopwords or ["رقم", "طريق", "شقة", "شقه", "القطع", "ارقام", 
-                                                    "لوحة", "لوحه", "تقسيم", "ش", "فيلا", "م","مكرر", "من", 
-                                                    "شارع", "متفرع","ورثه","ورثه ","ورثة ","ورثة ","ورثة", "والدها", "حسبى","nan","nan "]
-        punctuation = punctuation or string.punctuation
-        text = araby.strip_tashkeel(str(text))
-        text = re.sub('([@A-Za-z0-9_]+)|[^\w\s]|#|http\S+', ' ', str(text))
-        text = " ".join(word for word in text.split() if word not in custom_stopwords)
-        text = " ".join(word for word in text.split() if word not in punctuation)
-        return text
+
 
   
-def PolygonFinder(polygons, latitude, longitude):
-    # transform latitude and longitude into a point object
-    point = Point(longitude, latitude)
-
-    # compute distances between point and all polygons
-    distances = [point.distance(polygon) for polygon in polygons['geometry']]
-
-    # find index of closest polygon
-    index = np.argmin(distances)
-
-    # return information about closest polygon
-    closest_polygon = polygons.iloc[index]
-    result = {
-        'ADM3_PCODE': closest_polygon['ADM3_PCODE'],
-        'ADM2_PCODE': closest_polygon['ADM2_PCODE'],
-        'ADM1_PCODE': closest_polygon['ADM1_PCODE'],
-        'geometry': closest_polygon['geometry'],
-        'distance_polygon': distances[index],
-        'محافظة': closest_polygon['محافظة'],
-        'قسم / مركز': closest_polygon['قسم / مركز'],
-        'منطقة': closest_polygon['منطقة']
-    }
-    return result
+
     
 
 class AddressFinder:
     def __init__(self, geo_df):
       all_sub_regions = geo_df[['ADM3_AR',"ADM3_PCODE",'ADM2_AR',"ADM2_PCODE",'ADM1_AR',"ADM1_PCODE",'geometry']]
       all_sub_regions['ADM1_AR'] = all_sub_regions['ADM1_AR'].apply(lambda x : re.sub('\n','',x))
       all_sub_regions['ADM2_AR'] = all_sub_regions['ADM2_AR'].apply(lambda x : re.sub('\n','',x))
@@ -86,23 +49,69 @@
       all_sub_regions.rename(columns={
       'ADM3_AR':'منطقة',
       'ADM2_AR':'قسم / مركز',
       'ADM1_AR':'محافظة',
       },inplace=True)
       self.polygons = all_sub_regions
       self.address = []
-    
+    def clean_text(self,text,custom_stopwords=None, punctuation=None):
+        """clean data from any stopwords , punctuation and english litters
+         input:
+         if the input was list :
+         list.apply(lambda text : clean_text(text))
+         :return : clean Arabic text
+         """
+        custom_stopwords = custom_stopwords or ["رقم", "طريق", "شقة", "شقه", "القطع", "ارقام", 
+                                                    "لوحة", "لوحه", "تقسيم", "ش", "فيلا", "م","مكرر", "من", 
+                                                    "شارع", "متفرع","ورثه","ورثه ","ورثة ","ورثة ","ورثة", "والدها", "حسبى","nan","nan "]
+        punctuation = punctuation or string.punctuation
+        text = araby.strip_tashkeel(str(text))
+        text = re.sub('([@A-Za-z0-9_]+)|[^\w\s]|#|http\S+', ' ', str(text))
+        text = " ".join(word for word in text.split() if word not in custom_stopwords)
+        text = " ".join(word for word in text.split() if word not in punctuation)
+        return text
+    def PolygonFinder(self,polygons, latitude, longitude):
+        # transform latitude and longitude into a point object
+        point = Point(longitude, latitude)
+
+        # compute distances between point and all polygons
+        distances = [point.distance(polygon) for polygon in polygons['geometry']]
+        
+        # find index of closest polygon
+        index = np.argmin(distances)
+
+        # return information about closest polygon
+        closest_polygon = polygons.iloc[index]
+        result = {
+            'ADM3_PCODE': closest_polygon['ADM3_PCODE'],
+            'ADM2_PCODE': closest_polygon['ADM2_PCODE'],
+            'ADM1_PCODE': closest_polygon['ADM1_PCODE'],
+            'geometry': closest_polygon['geometry'],
+            'distance_polygon': distances[index],
+            'محافظة': closest_polygon['محافظة'],
+            'قسم / مركز': closest_polygon['قسم / مركز'],
+            'منطقة': closest_polygon['منطقة']
+        }
+        return result
     def find_address(self,data_0_100k):
         portal = GIS()
         portal
         for address_1 ,idz ,_ in zip(data_0_100k["full_address"], data_0_100k["CUSTOMER_ID"],tqdm(range(len(data_0_100k)))):
             single_line_address = " مصر "+ str(address_1)
-            single_line_address = clean_text(single_line_address)
+            single_line_address = self.clean_text(single_line_address)
             geocode_results = geocode(single_line_address)
             if len(geocode_results) != 0 :
                 country = geocode_results[0]["attributes"].get("Country",np.nan)
                 if country == 'EGY':
                     Latitude = geocode_results[0]["location"].get("y",np.NAN)
                     Longitude =  geocode_results[0]["location"].get("x",np.NAN)
                     input_data = pd.DataFrame({"Latitude":Latitude,"Longitude":Longitude,"address":address_1,"id":idz},index=[0])
-                    self.address.append(PolygonFinder(self.polygons,Latitude,Longitude))
-        return self.address
+                    self.address.append(self.PolygonFinder(self.polygons,Latitude,Longitude))
+        return self.address
+    
+'''
+geo_df = gpd.read_file(r"D:\\Task_2\\point of interst\\Reading shape files\\egy_admbnda_adm3_capmas_20170421.shp")
+address = pd.read_csv(r"D:\\Task_2\\address_finder_application\\output\\Address_Finder\\Address Finder\\test_data.csv")
+construct = AddressFinder(geo_df)
+address = construct.find_address(address)
+print(address)
+'''
```

### Comparing `bm_utilities-0.1.0/bm_utilities/bm_utilities.py` & `bm_utilities-0.1.1/bm_utilities/bm_utilities.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from bm_utilities import Address_finder as af
+from bm_utilities import quality_gates as qg
+
 import geopandas as gpd
 import pandas as pd
 import quality_gates as qg
 
 
-
-#class address_finder:
-#    def __init__(self,geo_df):
-#        self.construct = af(geo_df)
-#    def get_address(self,address):
-#        return self.construct.find_address(address)
-
-
 def address_finder(geodf,address):
     construct = af(geodf)
     address = construct.find_address(address)
     return address
 
 
 def quality_gates_check(df,config):
     my_gate = qg.QualityGates()
     df=my_gate.run_Quality_Gates(df,config)
     return df
 
 
 
 
-#print(address_finder( gpd.read_file(r"D:\\Task_2\\point of interst\\Reading shape files\\egy_admbnda_adm3_capmas_20170421.shp"),
-#                     pd.read_csv(r"D:\\Task_2\\address_finder_application\\output\\Address_Finder\\Address Finder\\test_data.csv")))
+
+'''
+geo_df = gpd.read_file(r"D:\\Task_2\\point of interst\\Reading shape files\\egy_admbnda_adm3_capmas_20170421.shp")
+address = pd.read_csv(r"D:\\Task_2\\address_finder_application\\output\\Address_Finder\\Address Finder\\test_data.csv")
+construct = AddressFinder(geo_df)
+address = construct.find_address(address)
+print(address)
+'''
 
 
 #for i in range(Branches_lat_long.shape[0]):
 #    if((Branches_lat_long[['lat']].iloc[i,:]).isna()):
 #        continue
 #    latitude = Branches_lat_long[['lat','long']].iloc[i,:]
 #    longitude = Branches_lat_long[['lat','long']].iloc[i,:]
```

### Comparing `bm_utilities-0.1.0/bm_utilities/quality_gates.py` & `bm_utilities-0.1.1/bm_utilities/quality_gates.py`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.0/bm_utilities.egg-info/PKG-INFO` & `bm_utilities-0.1.1/bm_utilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bm-utilities
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package for bm utilities
 Home-page: https://github.com/Youssefamroo/bm_utilities
 Author: youssef amr
 Author-email: usef.amr11@gmail.com
 License: MIT license
 Keywords: bm_utilities
 Classifier: Intended Audience :: Developers
```

### Comparing `bm_utilities-0.1.0/bm_utilities.egg-info/SOURCES.txt` & `bm_utilities-0.1.1/bm_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.0/docs/contributing.md` & `bm_utilities-0.1.1/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.0/docs/installation.md` & `bm_utilities-0.1.1/docs/installation.md`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.0/mkdocs.yml` & `bm_utilities-0.1.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.0/setup.py` & `bm_utilities-0.1.1/setup.py`

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
-    version='0.1.0',
+    version='0.1.1',
     zip_safe=False,
 )
```

