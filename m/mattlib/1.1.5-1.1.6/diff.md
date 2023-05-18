# Comparing `tmp/mattlib-1.1.5.tar.gz` & `tmp/mattlib-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mattlib-1.1.5.tar", last modified: Wed May 17 13:13:54 2023, max compression
+gzip compressed data, was "mattlib-1.1.6.tar", last modified: Thu May 18 14:02:35 2023, max compression
```

## Comparing `mattlib-1.1.5.tar` & `mattlib-1.1.6.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-17 13:13:54.784493 mattlib-1.1.5/
--rwxrwxrwx   0 livia     (1000) livia     (1000)    35149 2023-03-10 11:27:09.000000 mattlib-1.1.5/COPYING
--rwxrwxrwx   0 livia     (1000) livia     (1000)      629 2023-05-17 13:13:54.786020 mattlib-1.1.5/PKG-INFO
--rwxrwxrwx   0 livia     (1000) livia     (1000)      147 2023-03-10 11:27:09.000000 mattlib-1.1.5/README.md
--rwxrwxrwx   0 livia     (1000) livia     (1000)      104 2023-03-10 11:27:09.000000 mattlib-1.1.5/pyproject.toml
--rwxrwxrwx   0 livia     (1000) livia     (1000)      807 2023-05-17 13:13:54.796097 mattlib-1.1.5/setup.cfg
-drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-17 13:13:50.094392 mattlib-1.1.5/src/
-drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-17 13:13:50.653260 mattlib-1.1.5/src/mattlib/
--rwxrwxrwx   0 livia     (1000) livia     (1000)      733 2023-03-10 11:27:09.000000 mattlib-1.1.5/src/mattlib/API_factory.py
--rwxrwxrwx   0 livia     (1000) livia     (1000)     3173 2023-05-12 00:03:57.000000 mattlib-1.1.5/src/mattlib/BaseAPI.py
--rwxrwxrwx   0 livia     (1000) livia     (1000)      193 2023-03-10 11:27:09.000000 mattlib-1.1.5/src/mattlib/__init__.py
-drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-17 13:13:51.256315 mattlib-1.1.5/src/mattlib/adobe/
--rwxrwxrwx   0 livia     (1000) livia     (1000)     3332 2023-03-10 11:27:09.000000 mattlib-1.1.5/src/mattlib/adobe/AdobeAPI.py
--rwxrwxrwx   0 livia     (1000) livia     (1000)       30 2023-03-10 11:27:09.000000 mattlib-1.1.5/src/mattlib/adobe/__init__.py
-drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-17 13:13:51.528623 mattlib-1.1.5/src/mattlib/clockify/
--rwxrwxrwx   0 livia     (1000) livia     (1000)      751 2023-03-10 11:27:10.000000 mattlib-1.1.5/src/mattlib/clockify/ClockifyAPI.py
--rwxrwxrwx   0 livia     (1000) livia     (1000)       26 2023-03-10 11:27:10.000000 mattlib-1.1.5/src/mattlib/clockify/__init__.py
-drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-17 13:13:51.787286 mattlib-1.1.5/src/mattlib/fourmatters/
--rwxrwxrwx   0 livia     (1000) livia     (1000)     8016 2023-03-10 11:27:10.000000 mattlib-1.1.5/src/mattlib/fourmatters/virtual_machine.py
--rwxrwxrwx   0 livia     (1000) livia     (1000)     2964 2023-03-10 11:27:10.000000 mattlib-1.1.5/src/mattlib/fourmatters/virtual_network.py
-drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-17 13:13:52.089791 mattlib-1.1.5/src/mattlib/gcp/
--rwxrwxrwx   0 livia     (1000) livia     (1000)      484 2023-03-10 11:27:10.000000 mattlib-1.1.5/src/mattlib/gcp/PubSub.py
--rwxrwxrwx   0 livia     (1000) livia     (1000)       21 2023-03-10 11:27:10.000000 mattlib-1.1.5/src/mattlib/gcp/__init__.py
-drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-17 13:13:53.092592 mattlib-1.1.5/src/mattlib/google/
--rwxrwxrwx   0 livia     (1000) livia     (1000)     1116 2023-03-10 11:27:10.000000 mattlib-1.1.5/src/mattlib/google/BaseGoogleAPI.py
--rwxrwxrwx   0 livia     (1000) livia     (1000)     1061 2023-03-10 11:27:10.000000 mattlib-1.1.5/src/mattlib/google/GCPAPI.py
--rwxrwxrwx   0 livia     (1000) livia     (1000)     1175 2023-03-10 11:27:10.000000 mattlib-1.1.5/src/mattlib/google/GoogleWorkspaceAPI.py
--rwxrwxrwx   0 livia     (1000) livia     (1000)      484 2023-03-10 11:27:11.000000 mattlib-1.1.5/src/mattlib/google/PubSub.py
--rwxrwxrwx   0 livia     (1000) livia     (1000)     1483 2023-03-10 11:27:11.000000 mattlib-1.1.5/src/mattlib/google/SQL.py
--rwxrwxrwx   0 livia     (1000) livia     (1000)      750 2023-03-10 11:27:11.000000 mattlib-1.1.5/src/mattlib/google/Storage.py
--rwxrwxrwx   0 livia     (1000) livia     (1000)      139 2023-03-10 11:27:11.000000 mattlib-1.1.5/src/mattlib/google/__init__.py
-drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-17 13:13:53.671475 mattlib-1.1.5/src/mattlib/microsoft/
--rwxrwxrwx   0 livia     (1000) livia     (1000)    18681 2023-03-16 17:34:31.000000 mattlib-1.1.5/src/mattlib/microsoft/AzureAPI.py
--rwxrwxrwx   0 livia     (1000) livia     (1000)     2022 2023-05-11 14:13:25.000000 mattlib-1.1.5/src/mattlib/microsoft/BaseMicrosoftAPI.py
--rwxrwxrwx   0 livia     (1000) livia     (1000)     5700 2023-05-11 22:56:46.000000 mattlib-1.1.5/src/mattlib/microsoft/GraphAPI.py
--rwxrwxrwx   0 livia     (1000) livia     (1000)       61 2023-03-10 11:27:11.000000 mattlib-1.1.5/src/mattlib/microsoft/__init__.py
-drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-17 13:13:54.068458 mattlib-1.1.5/src/mattlib/network/
--rwxrwxrwx   0 livia     (1000) livia     (1000)     1373 2023-03-10 11:27:11.000000 mattlib-1.1.5/src/mattlib/network/HttpListener.py
--rwxrwxrwx   0 livia     (1000) livia     (1000)       39 2023-03-10 11:27:11.000000 mattlib-1.1.5/src/mattlib/network/__init__.py
-drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-17 13:13:54.273085 mattlib-1.1.5/src/mattlib/salesforce/
--rwxrwxrwx   0 livia     (1000) livia     (1000)     6518 2023-05-17 13:10:58.000000 mattlib-1.1.5/src/mattlib/salesforce/SalesForceAPI.py
--rwxrwxrwx   0 livia     (1000) livia     (1000)       41 2023-03-10 11:27:11.000000 mattlib-1.1.5/src/mattlib/salesforce/__init__.py
-drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-17 13:13:54.557973 mattlib-1.1.5/src/mattlib/system/
--rwxrwxrwx   0 livia     (1000) livia     (1000)     1370 2023-03-10 11:27:11.000000 mattlib-1.1.5/src/mattlib/system/Logger.py
--rwxrwxrwx   0 livia     (1000) livia     (1000)       27 2023-03-10 11:27:11.000000 mattlib-1.1.5/src/mattlib/system/__init__.py
-drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-17 13:13:51.038097 mattlib-1.1.5/src/mattlib.egg-info/
--rwxrwxrwx   0 livia     (1000) livia     (1000)      629 2023-05-17 13:13:49.000000 mattlib-1.1.5/src/mattlib.egg-info/PKG-INFO
--rwxrwxrwx   0 livia     (1000) livia     (1000)     1173 2023-05-17 13:13:50.000000 mattlib-1.1.5/src/mattlib.egg-info/SOURCES.txt
--rwxrwxrwx   0 livia     (1000) livia     (1000)        1 2023-05-17 13:13:49.000000 mattlib-1.1.5/src/mattlib.egg-info/dependency_links.txt
--rwxrwxrwx   0 livia     (1000) livia     (1000)       91 2023-05-17 13:13:49.000000 mattlib-1.1.5/src/mattlib.egg-info/requires.txt
--rwxrwxrwx   0 livia     (1000) livia     (1000)        8 2023-05-17 13:13:49.000000 mattlib-1.1.5/src/mattlib.egg-info/top_level.txt
-drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-17 13:13:54.710999 mattlib-1.1.5/test/
--rwxrwxrwx   0 livia     (1000) livia     (1000)      628 2023-03-10 11:27:11.000000 mattlib-1.1.5/test/test_salesforce.py
--rwxrwxrwx   0 livia     (1000) livia     (1000)      766 2023-03-10 11:27:11.000000 mattlib-1.1.5/test/test_vm_size.py
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-18 14:02:35.540539 mattlib-1.1.6/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)    35149 2023-03-10 11:27:09.000000 mattlib-1.1.6/COPYING
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      629 2023-05-18 14:02:35.543526 mattlib-1.1.6/PKG-INFO
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      147 2023-03-10 11:27:09.000000 mattlib-1.1.6/README.md
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      104 2023-03-10 11:27:09.000000 mattlib-1.1.6/pyproject.toml
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      807 2023-05-18 14:02:35.560026 mattlib-1.1.6/setup.cfg
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-18 14:02:31.120468 mattlib-1.1.6/src/
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-18 14:02:31.691199 mattlib-1.1.6/src/mattlib/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      733 2023-03-10 11:27:09.000000 mattlib-1.1.6/src/mattlib/API_factory.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     3173 2023-05-12 00:03:57.000000 mattlib-1.1.6/src/mattlib/BaseAPI.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      193 2023-03-10 11:27:09.000000 mattlib-1.1.6/src/mattlib/__init__.py
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-18 14:02:32.254351 mattlib-1.1.6/src/mattlib/adobe/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     3332 2023-03-10 11:27:09.000000 mattlib-1.1.6/src/mattlib/adobe/AdobeAPI.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)       30 2023-03-10 11:27:09.000000 mattlib-1.1.6/src/mattlib/adobe/__init__.py
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-18 14:02:32.442967 mattlib-1.1.6/src/mattlib/clockify/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      751 2023-03-10 11:27:10.000000 mattlib-1.1.6/src/mattlib/clockify/ClockifyAPI.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)       26 2023-03-10 11:27:10.000000 mattlib-1.1.6/src/mattlib/clockify/__init__.py
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-18 14:02:32.614159 mattlib-1.1.6/src/mattlib/fourmatters/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     8016 2023-03-10 11:27:10.000000 mattlib-1.1.6/src/mattlib/fourmatters/virtual_machine.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     2964 2023-03-10 11:27:10.000000 mattlib-1.1.6/src/mattlib/fourmatters/virtual_network.py
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-18 14:02:33.207304 mattlib-1.1.6/src/mattlib/gcp/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      484 2023-03-10 11:27:10.000000 mattlib-1.1.6/src/mattlib/gcp/PubSub.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)       21 2023-03-10 11:27:10.000000 mattlib-1.1.6/src/mattlib/gcp/__init__.py
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-18 14:02:34.247432 mattlib-1.1.6/src/mattlib/google/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     1116 2023-03-10 11:27:10.000000 mattlib-1.1.6/src/mattlib/google/BaseGoogleAPI.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     1061 2023-03-10 11:27:10.000000 mattlib-1.1.6/src/mattlib/google/GCPAPI.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     1175 2023-03-10 11:27:10.000000 mattlib-1.1.6/src/mattlib/google/GoogleWorkspaceAPI.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      484 2023-03-10 11:27:11.000000 mattlib-1.1.6/src/mattlib/google/PubSub.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     1483 2023-03-10 11:27:11.000000 mattlib-1.1.6/src/mattlib/google/SQL.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      750 2023-03-10 11:27:11.000000 mattlib-1.1.6/src/mattlib/google/Storage.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      139 2023-03-10 11:27:11.000000 mattlib-1.1.6/src/mattlib/google/__init__.py
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-18 14:02:34.658738 mattlib-1.1.6/src/mattlib/microsoft/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)    18681 2023-03-16 17:34:31.000000 mattlib-1.1.6/src/mattlib/microsoft/AzureAPI.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     2022 2023-05-11 14:13:25.000000 mattlib-1.1.6/src/mattlib/microsoft/BaseMicrosoftAPI.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     5700 2023-05-11 22:56:46.000000 mattlib-1.1.6/src/mattlib/microsoft/GraphAPI.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)       61 2023-03-10 11:27:11.000000 mattlib-1.1.6/src/mattlib/microsoft/__init__.py
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-18 14:02:34.827043 mattlib-1.1.6/src/mattlib/network/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     1373 2023-03-10 11:27:11.000000 mattlib-1.1.6/src/mattlib/network/HttpListener.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)       39 2023-03-10 11:27:11.000000 mattlib-1.1.6/src/mattlib/network/__init__.py
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-18 14:02:35.123048 mattlib-1.1.6/src/mattlib/salesforce/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     6520 2023-05-18 14:00:42.000000 mattlib-1.1.6/src/mattlib/salesforce/SalesForceAPI.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)       41 2023-03-10 11:27:11.000000 mattlib-1.1.6/src/mattlib/salesforce/__init__.py
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-18 14:02:35.293335 mattlib-1.1.6/src/mattlib/system/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     1370 2023-03-10 11:27:11.000000 mattlib-1.1.6/src/mattlib/system/Logger.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)       27 2023-03-10 11:27:11.000000 mattlib-1.1.6/src/mattlib/system/__init__.py
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-18 14:02:32.049211 mattlib-1.1.6/src/mattlib.egg-info/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      629 2023-05-18 14:02:30.000000 mattlib-1.1.6/src/mattlib.egg-info/PKG-INFO
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     1173 2023-05-18 14:02:31.000000 mattlib-1.1.6/src/mattlib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 livia     (1000) livia     (1000)        1 2023-05-18 14:02:30.000000 mattlib-1.1.6/src/mattlib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 livia     (1000) livia     (1000)       91 2023-05-18 14:02:30.000000 mattlib-1.1.6/src/mattlib.egg-info/requires.txt
+-rwxrwxrwx   0 livia     (1000) livia     (1000)        8 2023-05-18 14:02:30.000000 mattlib-1.1.6/src/mattlib.egg-info/top_level.txt
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-18 14:02:35.405094 mattlib-1.1.6/test/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      628 2023-03-10 11:27:11.000000 mattlib-1.1.6/test/test_salesforce.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      766 2023-03-10 11:27:11.000000 mattlib-1.1.6/test/test_vm_size.py
```

### Comparing `mattlib-1.1.5/COPYING` & `mattlib-1.1.6/COPYING`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.5/PKG-INFO` & `mattlib-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mattlib
-Version: 1.1.5
+Version: 1.1.6
 Summary: API data extraction and formatting utilities.
 Home-page: https://source.cloud.google.com/mtz-repos-global/mattlib
 Author: 4matt
 Author-email: mattzero@4matt.com.br
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `mattlib-1.1.5/setup.cfg` & `mattlib-1.1.6/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mattlib
-version = 1.1.5
+version = 1.1.6
 author = 4matt
 author_email = mattzero@4matt.com.br
 description = API data extraction and formatting utilities.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://source.cloud.google.com/mtz-repos-global/mattlib
 classifiers =
```

### Comparing `mattlib-1.1.5/src/mattlib/API_factory.py` & `mattlib-1.1.6/src/mattlib/API_factory.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.5/src/mattlib/BaseAPI.py` & `mattlib-1.1.6/src/mattlib/BaseAPI.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.5/src/mattlib/adobe/AdobeAPI.py` & `mattlib-1.1.6/src/mattlib/adobe/AdobeAPI.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.5/src/mattlib/clockify/ClockifyAPI.py` & `mattlib-1.1.6/src/mattlib/clockify/ClockifyAPI.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.5/src/mattlib/fourmatters/virtual_machine.py` & `mattlib-1.1.6/src/mattlib/fourmatters/virtual_machine.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.5/src/mattlib/fourmatters/virtual_network.py` & `mattlib-1.1.6/src/mattlib/fourmatters/virtual_network.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.5/src/mattlib/google/BaseGoogleAPI.py` & `mattlib-1.1.6/src/mattlib/google/BaseGoogleAPI.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.5/src/mattlib/google/GCPAPI.py` & `mattlib-1.1.6/src/mattlib/google/GCPAPI.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.5/src/mattlib/google/GoogleWorkspaceAPI.py` & `mattlib-1.1.6/src/mattlib/google/GoogleWorkspaceAPI.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.5/src/mattlib/google/SQL.py` & `mattlib-1.1.6/src/mattlib/google/SQL.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.5/src/mattlib/google/Storage.py` & `mattlib-1.1.6/src/mattlib/google/Storage.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.5/src/mattlib/microsoft/AzureAPI.py` & `mattlib-1.1.6/src/mattlib/microsoft/AzureAPI.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.5/src/mattlib/microsoft/BaseMicrosoftAPI.py` & `mattlib-1.1.6/src/mattlib/microsoft/BaseMicrosoftAPI.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.5/src/mattlib/microsoft/GraphAPI.py` & `mattlib-1.1.6/src/mattlib/microsoft/GraphAPI.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.5/src/mattlib/network/HttpListener.py` & `mattlib-1.1.6/src/mattlib/network/HttpListener.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.5/src/mattlib/salesforce/SalesForceAPI.py` & `mattlib-1.1.6/src/mattlib/salesforce/SalesForceAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         self.consumer_key = consumer_key.rstrip()
         self.consumer_secret = consumer_secret.rstrip()
         self.username = username.rstrip()
         self.password = password.rstrip()
         self.url = f'https://{self.domain}.my.salesforce.com'
         if self.type == 'username-password':
             self.headers = self.__get_auth_user()
-        if type == 'web server':
+        elif type == 'web server':
             self.headers = self.__get_auth_web_server(authorization)
         else:
             raise "Type of connection not exist"
         # headers must be: 
         # { 'Authorization': <token>, 'X-PrettyPrint': 1 }
 
     def __get_auth_user(self):
```

### Comparing `mattlib-1.1.5/src/mattlib/system/Logger.py` & `mattlib-1.1.6/src/mattlib/system/Logger.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.5/src/mattlib.egg-info/PKG-INFO` & `mattlib-1.1.6/src/mattlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mattlib
-Version: 1.1.5
+Version: 1.1.6
 Summary: API data extraction and formatting utilities.
 Home-page: https://source.cloud.google.com/mtz-repos-global/mattlib
 Author: 4matt
 Author-email: mattzero@4matt.com.br
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `mattlib-1.1.5/src/mattlib.egg-info/SOURCES.txt` & `mattlib-1.1.6/src/mattlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.5/test/test_salesforce.py` & `mattlib-1.1.6/test/test_salesforce.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.5/test/test_vm_size.py` & `mattlib-1.1.6/test/test_vm_size.py`

 * *Files identical despite different names*

