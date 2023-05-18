# Comparing `tmp/OmeSliCC-0.5.1.1.tar.gz` & `tmp/OmeSliCC-0.5.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OmeSliCC-0.5.1.1.tar", last modified: Thu May 18 20:45:14 2023, max compression
+gzip compressed data, was "OmeSliCC-0.5.1b0.tar", last modified: Thu May 18 20:43:10 2023, max compression
```

## Comparing `OmeSliCC-0.5.1.1.tar` & `OmeSliCC-0.5.1b0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 20:45:14.169387 OmeSliCC-0.5.1.1/
--rw-rw-rw-   0        0        0    36454 2022-09-16 15:34:35.000000 OmeSliCC-0.5.1.1/LICENSE.md
--rw-rw-rw-   0        0        0    44210 2023-05-18 20:45:14.168372 OmeSliCC-0.5.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2210 2023-03-04 11:28:54.000000 OmeSliCC-0.5.1.1/README.md
--rw-rw-rw-   0        0        0      434 2023-05-18 20:44:48.000000 OmeSliCC-0.5.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      232 2023-05-18 20:12:27.000000 OmeSliCC-0.5.1.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 20:45:14.169387 OmeSliCC-0.5.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-18 20:45:14.120375 OmeSliCC-0.5.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-18 20:45:14.154375 OmeSliCC-0.5.1.1/src/OmeSliCC/
--rw-rw-rw-   0        0        0     3141 2023-05-18 19:44:23.000000 OmeSliCC-0.5.1.1/src/OmeSliCC/BioSource.py
--rw-rw-rw-   0        0        0    12089 2023-05-18 19:44:39.000000 OmeSliCC-0.5.1.1/src/OmeSliCC/OmeSource.py
--rw-rw-rw-   0        0        0     5950 2023-05-18 19:43:38.000000 OmeSliCC-0.5.1.1/src/OmeSliCC/Omero.py
--rw-rw-rw-   0        0        0     2046 2023-05-18 19:37:19.000000 OmeSliCC-0.5.1.1/src/OmeSliCC/OmeroLabelReader.py
--rw-rw-rw-   0        0        0     4702 2023-05-18 19:45:26.000000 OmeSliCC-0.5.1.1/src/OmeSliCC/OmeroSource.py
--rw-rw-rw-   0        0        0     3335 2023-05-18 19:44:46.000000 OmeSliCC-0.5.1.1/src/OmeSliCC/PlainImageSource.py
--rw-rw-rw-   0        0        0    11964 2023-05-18 19:45:50.000000 OmeSliCC-0.5.1.1/src/OmeSliCC/TiffSource.py
--rw-rw-rw-   0        0        0     1896 2023-03-25 15:06:02.000000 OmeSliCC-0.5.1.1/src/OmeSliCC/XmlDict.py
--rw-rw-rw-   0        0        0     4718 2023-05-18 19:46:09.000000 OmeSliCC-0.5.1.1/src/OmeSliCC/ZarrSource.py
--rw-rw-rw-   0        0        0    11660 2023-05-18 19:44:05.000000 OmeSliCC-0.5.1.1/src/OmeSliCC/conversion.py
--rw-rw-rw-   0        0        0    10776 2023-05-18 19:45:10.000000 OmeSliCC-0.5.1.1/src/OmeSliCC/image_util.py
--rw-rw-rw-   0        0        0    17547 2023-05-18 19:44:55.000000 OmeSliCC-0.5.1.1/src/OmeSliCC/ome.py
--rw-rw-rw-   0        0        0     1298 2022-10-27 12:37:45.000000 OmeSliCC-0.5.1.1/src/OmeSliCC/omero_credentials.py
--rw-rw-rw-   0        0        0      225 2022-09-29 12:36:36.000000 OmeSliCC-0.5.1.1/src/OmeSliCC/parameters.py
--rw-rw-rw-   0        0        0     4970 2023-03-06 12:50:47.000000 OmeSliCC-0.5.1.1/src/OmeSliCC/util.py
-drwxrwxrwx   0        0        0        0 2023-05-18 20:45:14.164408 OmeSliCC-0.5.1.1/src/OmeSliCC.egg-info/
--rw-rw-rw-   0        0        0    44210 2023-05-18 20:45:14.000000 OmeSliCC-0.5.1.1/src/OmeSliCC.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      647 2023-05-18 20:45:14.000000 OmeSliCC-0.5.1.1/src/OmeSliCC.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 20:45:14.000000 OmeSliCC-0.5.1.1/src/OmeSliCC.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      209 2023-05-18 20:45:14.000000 OmeSliCC-0.5.1.1/src/OmeSliCC.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-18 20:45:14.000000 OmeSliCC-0.5.1.1/src/OmeSliCC.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-18 20:45:14.166379 OmeSliCC-0.5.1.1/tests/
--rw-rw-rw-   0        0        0     4482 2023-05-18 19:41:34.000000 OmeSliCC-0.5.1.1/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-05-18 20:43:10.707701 OmeSliCC-0.5.1b0/
+-rw-rw-rw-   0        0        0    36454 2022-09-16 15:34:35.000000 OmeSliCC-0.5.1b0/LICENSE.md
+-rw-rw-rw-   0        0        0    44210 2023-05-18 20:43:10.706702 OmeSliCC-0.5.1b0/PKG-INFO
+-rw-rw-rw-   0        0        0     2210 2023-03-04 11:28:54.000000 OmeSliCC-0.5.1b0/README.md
+-rw-rw-rw-   0        0        0      433 2023-05-18 20:42:46.000000 OmeSliCC-0.5.1b0/pyproject.toml
+-rw-rw-rw-   0        0        0      232 2023-05-18 20:12:27.000000 OmeSliCC-0.5.1b0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 20:43:10.707701 OmeSliCC-0.5.1b0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-18 20:43:10.665743 OmeSliCC-0.5.1b0/src/
+drwxrwxrwx   0        0        0        0 2023-05-18 20:43:10.694699 OmeSliCC-0.5.1b0/src/OmeSliCC/
+-rw-rw-rw-   0        0        0     3141 2023-05-18 19:44:23.000000 OmeSliCC-0.5.1b0/src/OmeSliCC/BioSource.py
+-rw-rw-rw-   0        0        0    12089 2023-05-18 19:44:39.000000 OmeSliCC-0.5.1b0/src/OmeSliCC/OmeSource.py
+-rw-rw-rw-   0        0        0     5950 2023-05-18 19:43:38.000000 OmeSliCC-0.5.1b0/src/OmeSliCC/Omero.py
+-rw-rw-rw-   0        0        0     2046 2023-05-18 19:37:19.000000 OmeSliCC-0.5.1b0/src/OmeSliCC/OmeroLabelReader.py
+-rw-rw-rw-   0        0        0     4702 2023-05-18 19:45:26.000000 OmeSliCC-0.5.1b0/src/OmeSliCC/OmeroSource.py
+-rw-rw-rw-   0        0        0     3335 2023-05-18 19:44:46.000000 OmeSliCC-0.5.1b0/src/OmeSliCC/PlainImageSource.py
+-rw-rw-rw-   0        0        0    11964 2023-05-18 19:45:50.000000 OmeSliCC-0.5.1b0/src/OmeSliCC/TiffSource.py
+-rw-rw-rw-   0        0        0     1896 2023-03-25 15:06:02.000000 OmeSliCC-0.5.1b0/src/OmeSliCC/XmlDict.py
+-rw-rw-rw-   0        0        0     4718 2023-05-18 19:46:09.000000 OmeSliCC-0.5.1b0/src/OmeSliCC/ZarrSource.py
+-rw-rw-rw-   0        0        0    11660 2023-05-18 19:44:05.000000 OmeSliCC-0.5.1b0/src/OmeSliCC/conversion.py
+-rw-rw-rw-   0        0        0    10776 2023-05-18 19:45:10.000000 OmeSliCC-0.5.1b0/src/OmeSliCC/image_util.py
+-rw-rw-rw-   0        0        0    17547 2023-05-18 19:44:55.000000 OmeSliCC-0.5.1b0/src/OmeSliCC/ome.py
+-rw-rw-rw-   0        0        0     1298 2022-10-27 12:37:45.000000 OmeSliCC-0.5.1b0/src/OmeSliCC/omero_credentials.py
+-rw-rw-rw-   0        0        0      225 2022-09-29 12:36:36.000000 OmeSliCC-0.5.1b0/src/OmeSliCC/parameters.py
+-rw-rw-rw-   0        0        0     4970 2023-03-06 12:50:47.000000 OmeSliCC-0.5.1b0/src/OmeSliCC/util.py
+drwxrwxrwx   0        0        0        0 2023-05-18 20:43:10.704698 OmeSliCC-0.5.1b0/src/OmeSliCC.egg-info/
+-rw-rw-rw-   0        0        0    44210 2023-05-18 20:43:10.000000 OmeSliCC-0.5.1b0/src/OmeSliCC.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      647 2023-05-18 20:43:10.000000 OmeSliCC-0.5.1b0/src/OmeSliCC.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 20:43:10.000000 OmeSliCC-0.5.1b0/src/OmeSliCC.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      209 2023-05-18 20:43:10.000000 OmeSliCC-0.5.1b0/src/OmeSliCC.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-18 20:43:10.000000 OmeSliCC-0.5.1b0/src/OmeSliCC.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 20:43:10.705703 OmeSliCC-0.5.1b0/tests/
+-rw-rw-rw-   0        0        0     4482 2023-05-18 19:41:34.000000 OmeSliCC-0.5.1b0/tests/test.py
```

### Comparing `OmeSliCC-0.5.1.1/LICENSE.md` & `OmeSliCC-0.5.1b0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `OmeSliCC-0.5.1.1/PKG-INFO` & `OmeSliCC-0.5.1b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OmeSliCC
-Version: 0.5.1.1
+Version: 0.5.1b0
 Summary: Ome(ro) Slide Image Conversion and Compression pipeline
 Author-email: Joost de Folter <folterj@gmail.com>
 License: # OmeSliCC Licence Agreement
         
         ## OmeSliCC: Ome(ro) SLide Image Conversion and Compression: Software for image conversion including handing both the images and meta-data from Omero.
         
         ©2022, The Francis Crick Institute
```

### Comparing `OmeSliCC-0.5.1.1/README.md` & `OmeSliCC-0.5.1b0/README.md`

 * *Files identical despite different names*

### Comparing `OmeSliCC-0.5.1.1/src/OmeSliCC/BioSource.py` & `OmeSliCC-0.5.1b0/src/OmeSliCC/BioSource.py`

 * *Files identical despite different names*

### Comparing `OmeSliCC-0.5.1.1/src/OmeSliCC/OmeSource.py` & `OmeSliCC-0.5.1b0/src/OmeSliCC/OmeSource.py`

 * *Files identical despite different names*

### Comparing `OmeSliCC-0.5.1.1/src/OmeSliCC/Omero.py` & `OmeSliCC-0.5.1b0/src/OmeSliCC/Omero.py`

 * *Files identical despite different names*

### Comparing `OmeSliCC-0.5.1.1/src/OmeSliCC/OmeroLabelReader.py` & `OmeSliCC-0.5.1b0/src/OmeSliCC/OmeroLabelReader.py`

 * *Files identical despite different names*

### Comparing `OmeSliCC-0.5.1.1/src/OmeSliCC/OmeroSource.py` & `OmeSliCC-0.5.1b0/src/OmeSliCC/OmeroSource.py`

 * *Files identical despite different names*

### Comparing `OmeSliCC-0.5.1.1/src/OmeSliCC/PlainImageSource.py` & `OmeSliCC-0.5.1b0/src/OmeSliCC/PlainImageSource.py`

 * *Files identical despite different names*

### Comparing `OmeSliCC-0.5.1.1/src/OmeSliCC/TiffSource.py` & `OmeSliCC-0.5.1b0/src/OmeSliCC/TiffSource.py`

 * *Files identical despite different names*

### Comparing `OmeSliCC-0.5.1.1/src/OmeSliCC/XmlDict.py` & `OmeSliCC-0.5.1b0/src/OmeSliCC/XmlDict.py`

 * *Files identical despite different names*

### Comparing `OmeSliCC-0.5.1.1/src/OmeSliCC/ZarrSource.py` & `OmeSliCC-0.5.1b0/src/OmeSliCC/ZarrSource.py`

 * *Files identical despite different names*

### Comparing `OmeSliCC-0.5.1.1/src/OmeSliCC/conversion.py` & `OmeSliCC-0.5.1b0/src/OmeSliCC/conversion.py`

 * *Files identical despite different names*

### Comparing `OmeSliCC-0.5.1.1/src/OmeSliCC/image_util.py` & `OmeSliCC-0.5.1b0/src/OmeSliCC/image_util.py`

 * *Files identical despite different names*

### Comparing `OmeSliCC-0.5.1.1/src/OmeSliCC/ome.py` & `OmeSliCC-0.5.1b0/src/OmeSliCC/ome.py`

 * *Files identical despite different names*

### Comparing `OmeSliCC-0.5.1.1/src/OmeSliCC/omero_credentials.py` & `OmeSliCC-0.5.1b0/src/OmeSliCC/omero_credentials.py`

 * *Files identical despite different names*

### Comparing `OmeSliCC-0.5.1.1/src/OmeSliCC/util.py` & `OmeSliCC-0.5.1b0/src/OmeSliCC/util.py`

 * *Files identical despite different names*

### Comparing `OmeSliCC-0.5.1.1/src/OmeSliCC.egg-info/PKG-INFO` & `OmeSliCC-0.5.1b0/src/OmeSliCC.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OmeSliCC
-Version: 0.5.1.1
+Version: 0.5.1b0
 Summary: Ome(ro) Slide Image Conversion and Compression pipeline
 Author-email: Joost de Folter <folterj@gmail.com>
 License: # OmeSliCC Licence Agreement
         
         ## OmeSliCC: Ome(ro) SLide Image Conversion and Compression: Software for image conversion including handing both the images and meta-data from Omero.
         
         ©2022, The Francis Crick Institute
```

### Comparing `OmeSliCC-0.5.1.1/src/OmeSliCC.egg-info/SOURCES.txt` & `OmeSliCC-0.5.1b0/src/OmeSliCC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OmeSliCC-0.5.1.1/tests/test.py` & `OmeSliCC-0.5.1b0/tests/test.py`

 * *Files identical despite different names*

