# Comparing `tmp/sshkey-tools-0.9.0.tar.gz` & `tmp/sshkey-tools-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sshkey-tools-0.9.0.tar", last modified: Wed Jul 20 15:13:35 2022, max compression
+gzip compressed data, was "sshkey-tools-0.9.1.tar", last modified: Thu May 18 21:35:24 2023, max compression
```

## Comparing `sshkey-tools-0.9.0.tar` & `sshkey-tools-0.9.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:13:35.074524 sshkey-tools-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-07-20 15:13:23.000000 sshkey-tools-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    15952 2022-07-20 15:13:35.074524 sshkey-tools-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    15293 2022-07-20 15:13:23.000000 sshkey-tools-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-07-20 15:13:23.000000 sshkey-tools-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-20 15:13:35.074524 sshkey-tools-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1888 2022-07-20 15:13:23.000000 sshkey-tools-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:13:35.070523 sshkey-tools-0.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:13:35.074524 sshkey-tools-0.9.0/src/sshkey_tools/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-07-20 15:13:23.000000 sshkey-tools-0.9.0/src/sshkey_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      631 2022-07-20 15:13:23.000000 sshkey-tools-0.9.0/src/sshkey_tools/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20238 2022-07-20 15:13:23.000000 sshkey-tools-0.9.0/src/sshkey_tools/cert.py
--rw-r--r--   0 runner    (1001) docker     (121)     2229 2022-07-20 15:13:23.000000 sshkey-tools-0.9.0/src/sshkey_tools/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    48541 2022-07-20 15:13:23.000000 sshkey-tools-0.9.0/src/sshkey_tools/fields.py
--rw-r--r--   0 runner    (1001) docker     (121)    29287 2022-07-20 15:13:23.000000 sshkey-tools-0.9.0/src/sshkey_tools/keys.py
--rw-r--r--   0 runner    (1001) docker     (121)     7776 2022-07-20 15:13:23.000000 sshkey-tools-0.9.0/src/sshkey_tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:13:35.074524 sshkey-tools-0.9.0/src/sshkey_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15952 2022-07-20 15:13:35.000000 sshkey-tools-0.9.0/src/sshkey_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      513 2022-07-20 15:13:35.000000 sshkey-tools-0.9.0/src/sshkey_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-20 15:13:35.000000 sshkey-tools-0.9.0/src/sshkey_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-07-20 15:13:35.000000 sshkey-tools-0.9.0/src/sshkey_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-07-20 15:13:35.000000 sshkey-tools-0.9.0/src/sshkey_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-07-20 15:13:35.000000 sshkey-tools-0.9.0/src/sshkey_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-20 15:13:35.000000 sshkey-tools-0.9.0/src/sshkey_tools.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:35:24.510807 sshkey-tools-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 21:35:12.000000 sshkey-tools-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15926 2023-05-18 21:35:24.510807 sshkey-tools-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15293 2023-05-18 21:35:12.000000 sshkey-tools-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-18 21:35:12.000000 sshkey-tools-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 21:35:24.510807 sshkey-tools-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-18 21:35:12.000000 sshkey-tools-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:35:24.506806 sshkey-tools-0.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:35:24.510807 sshkey-tools-0.9.1/src/sshkey_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-18 21:35:12.000000 sshkey-tools-0.9.1/src/sshkey_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-18 21:35:12.000000 sshkey-tools-0.9.1/src/sshkey_tools/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20238 2023-05-18 21:35:12.000000 sshkey-tools-0.9.1/src/sshkey_tools/cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-18 21:35:12.000000 sshkey-tools-0.9.1/src/sshkey_tools/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48541 2023-05-18 21:35:12.000000 sshkey-tools-0.9.1/src/sshkey_tools/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29285 2023-05-18 21:35:12.000000 sshkey-tools-0.9.1/src/sshkey_tools/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-05-18 21:35:12.000000 sshkey-tools-0.9.1/src/sshkey_tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:35:24.510807 sshkey-tools-0.9.1/src/sshkey_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15926 2023-05-18 21:35:24.000000 sshkey-tools-0.9.1/src/sshkey_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-18 21:35:24.000000 sshkey-tools-0.9.1/src/sshkey_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 21:35:24.000000 sshkey-tools-0.9.1/src/sshkey_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-18 21:35:24.000000 sshkey-tools-0.9.1/src/sshkey_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-18 21:35:24.000000 sshkey-tools-0.9.1/src/sshkey_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-18 21:35:24.000000 sshkey-tools-0.9.1/src/sshkey_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 21:35:24.000000 sshkey-tools-0.9.1/src/sshkey_tools.egg-info/zip-safe
```

### Comparing `sshkey-tools-0.9.0/LICENSE` & `sshkey-tools-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sshkey-tools-0.9.0/PKG-INFO` & `sshkey-tools-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: sshkey-tools
-Version: 0.9.0
-Summary:      A Python module for generating, parsing and handling OpenSSH keys and certificates 
+Version: 0.9.1
+Summary: A Python module for generating, parsing and handling OpenSSH keys and certificates
 Home-page: https://github.com/scheiblingco/sshkey-tools
 Author: Lars Scheibling
 Author-email: lars@scheibling.se
 License: GnuPG 3.0
 Keywords: python openssh ssh keys sshkey ssh-keygen ssh-certificate certificate parser decoder
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -341,9 +340,7 @@
 - Added verification of certificate signature
 - Added option to choose RSA hashing algorithm for signing
 - Removed test files
 - Added documentation deployment CD for GH pages
 
 ### 0.8
 - Initial public release
-
-
```

### Comparing `sshkey-tools-0.9.0/README.md` & `sshkey-tools-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `sshkey-tools-0.9.0/setup.py` & `sshkey-tools-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `sshkey-tools-0.9.0/src/sshkey_tools/__version__.py` & `sshkey-tools-0.9.1/src/sshkey_tools/__version__.py`

 * *Files identical despite different names*

### Comparing `sshkey-tools-0.9.0/src/sshkey_tools/cert.py` & `sshkey-tools-0.9.1/src/sshkey_tools/cert.py`

 * *Files identical despite different names*

### Comparing `sshkey-tools-0.9.0/src/sshkey_tools/exceptions.py` & `sshkey-tools-0.9.1/src/sshkey_tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `sshkey-tools-0.9.0/src/sshkey_tools/fields.py` & `sshkey-tools-0.9.1/src/sshkey_tools/fields.py`

 * *Files identical despite different names*

### Comparing `sshkey-tools-0.9.0/src/sshkey_tools/keys.py` & `sshkey-tools-0.9.1/src/sshkey_tools/keys.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 
 class PublicKey:
     """
     Class for handling SSH public keys
     """
 
     def __init__(
-        self, key: PrivkeyClasses = None, comment: Union[str, bytes] = None, **kwargs
+        self, key: PrivkeyClasses = None, comment: Union[str, bytes] = "", **kwargs
     ) -> None:
         self.key = key
         self.comment = comment
         self.public_numbers = kwargs.get("public_numbers", None)
         self.key_type = kwargs.get("key_type", None)
         self.serialized = kwargs.get("serialized", None)
```

### Comparing `sshkey-tools-0.9.0/src/sshkey_tools/utils.py` & `sshkey-tools-0.9.1/src/sshkey_tools/utils.py`

 * *Files identical despite different names*

### Comparing `sshkey-tools-0.9.0/src/sshkey_tools.egg-info/PKG-INFO` & `sshkey-tools-0.9.1/src/sshkey_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: sshkey-tools
-Version: 0.9.0
-Summary:      A Python module for generating, parsing and handling OpenSSH keys and certificates 
+Version: 0.9.1
+Summary: A Python module for generating, parsing and handling OpenSSH keys and certificates
 Home-page: https://github.com/scheiblingco/sshkey-tools
 Author: Lars Scheibling
 Author-email: lars@scheibling.se
 License: GnuPG 3.0
 Keywords: python openssh ssh keys sshkey ssh-keygen ssh-certificate certificate parser decoder
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -341,9 +340,7 @@
 - Added verification of certificate signature
 - Added option to choose RSA hashing algorithm for signing
 - Removed test files
 - Added documentation deployment CD for GH pages
 
 ### 0.8
 - Initial public release
-
-
```

### Comparing `sshkey-tools-0.9.0/src/sshkey_tools.egg-info/SOURCES.txt` & `sshkey-tools-0.9.1/src/sshkey_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

