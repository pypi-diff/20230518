# Comparing `tmp/nexus-utilities-0.4.0.tar.gz` & `tmp/nexus-utilities-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexus-utilities-0.4.0.tar", last modified: Sat May 13 20:27:43 2023, max compression
+gzip compressed data, was "nexus-utilities-0.4.1.tar", last modified: Thu May 18 17:23:41 2023, max compression
```

## Comparing `nexus-utilities-0.4.0.tar` & `nexus-utilities-0.4.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 20:27:43.278534 nexus-utilities-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-13 20:27:27.000000 nexus-utilities-0.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-13 20:27:43.278534 nexus-utilities-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13493 2023-05-13 20:27:27.000000 nexus-utilities-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 20:27:43.278534 nexus-utilities-0.4.0/nexus_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-13 20:27:43.000000 nexus-utilities-0.4.0/nexus_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-13 20:27:43.000000 nexus-utilities-0.4.0/nexus_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 20:27:43.000000 nexus-utilities-0.4.0/nexus_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-13 20:27:43.000000 nexus-utilities-0.4.0/nexus_utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-13 20:27:43.000000 nexus-utilities-0.4.0/nexus_utilities.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 20:27:43.278534 nexus-utilities-0.4.0/nexus_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-13 20:27:27.000000 nexus-utilities-0.4.0/nexus_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-13 20:27:27.000000 nexus-utilities-0.4.0/nexus_utils/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-05-13 20:27:27.000000 nexus-utilities-0.4.0/nexus_utils/database_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-05-13 20:27:27.000000 nexus-utilities-0.4.0/nexus_utils/datetime_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-13 20:27:27.000000 nexus-utilities-0.4.0/nexus_utils/flatfile_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-13 20:27:27.000000 nexus-utilities-0.4.0/nexus_utils/package_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-13 20:27:27.000000 nexus-utilities-0.4.0/nexus_utils/password_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-13 20:27:27.000000 nexus-utilities-0.4.0/nexus_utils/string_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 20:27:43.278534 nexus-utilities-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-13 20:27:27.000000 nexus-utilities-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:23:41.006468 nexus-utilities-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-18 17:23:30.000000 nexus-utilities-0.4.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-18 17:23:41.006468 nexus-utilities-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13576 2023-05-18 17:23:30.000000 nexus-utilities-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:23:41.002468 nexus-utilities-0.4.1/nexus_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-18 17:23:40.000000 nexus-utilities-0.4.1/nexus_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-18 17:23:40.000000 nexus-utilities-0.4.1/nexus_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 17:23:40.000000 nexus-utilities-0.4.1/nexus_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-18 17:23:40.000000 nexus-utilities-0.4.1/nexus_utilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-18 17:23:40.000000 nexus-utilities-0.4.1/nexus_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:23:41.006468 nexus-utilities-0.4.1/nexus_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-18 17:23:30.000000 nexus-utilities-0.4.1/nexus_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-18 17:23:30.000000 nexus-utilities-0.4.1/nexus_utils/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-05-18 17:23:30.000000 nexus-utilities-0.4.1/nexus_utils/database_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-05-18 17:23:30.000000 nexus-utilities-0.4.1/nexus_utils/datetime_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-18 17:23:30.000000 nexus-utilities-0.4.1/nexus_utils/flatfile_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-18 17:23:30.000000 nexus-utilities-0.4.1/nexus_utils/package_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-18 17:23:30.000000 nexus-utilities-0.4.1/nexus_utils/password_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-18 17:23:30.000000 nexus-utilities-0.4.1/nexus_utils/string_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 17:23:41.006468 nexus-utilities-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-18 17:23:30.000000 nexus-utilities-0.4.1/setup.py
```

### Comparing `nexus-utilities-0.4.0/LICENSE.txt` & `nexus-utilities-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.4.0/PKG-INFO` & `nexus-utilities-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus-utilities
-Version: 0.4.0
+Version: 0.4.1
 Summary: Common python utilities
 Home-page: https://github.com/james-larsen/nexus-utilities
 Author: James Larsen
 Author-email: james.larsen42@gmail.com
 License: UNKNOWN
 Description: This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.
 Platform: UNKNOWN
```

### Comparing `nexus-utilities-0.4.0/README.md` & `nexus-utilities-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 - [config\_utils.py](#config_utilspy)
   - [**read\_config\_file(config\_filepath)**](#read_config_fileconfig_filepath)
 - [database\_utils.py](#database_utilspy)
   - [**build\_engine(connect\_type, server\_address, server\_port, server\_name, user\_name, password, schema=None)**](#build_engineconnect_type-server_address-server_port-server_name-user_name-password-schemanone)
   - [**clean\_sql\_statement(sql\_statement)**](#clean_sql_statementsql_statement)
 - [datetime\_utils.py](#datetime_utilspy)
   - [**get\_current\_timestamp()**](#get_current_timestamp)
-  - [**getDuration(then, now=datetime.datetime.now())**](#getdurationthen-nowdatetimedatetimenow)
+  - [**get\_duration(then, now=datetime.datetime.now())**](#get_durationthen-nowdatetimedatetimenow)
+  - [**determine\_date\_format(date\_list)**](#determine_date_formatdate_list)
 - [package\_utils.py](#package_utilspy)
   - [**add\_package\_to\_path()**](#add_package_to_path)
   - [**import\_relative(package\_root\_name, module\_path, import\_name, alias=None)**](#import_relativepackage_root_name-module_path-import_name-aliasnone)
 - [password\_utils.py](#password_utilspy)
   - [**get\_password(password\_method, password\_key, account\_name=None, access\_key=None, secret\_key=None, endpoint\_url=None, region\_name=None, password\_path=None, encoding='utf-8')**](#get_passwordpassword_method-password_key-account_namenone-access_keynone-secret_keynone-endpoint_urlnone-region_namenone-password_pathnone-encodingutf-8)
 - [string\_utils.py](#string_utilspy)
   - [**cleanse\_string(string, remove\_symbols=True, title\_to\_snake\_case=False, hyphen\_to\_underscore=True, period\_to\_underscore=True, to\_upper=False, to\_lower=True)**](#cleanse_stringstring-remove_symbolstrue-title_to_snake_casefalse-hyphen_to_underscoretrue-period_to_underscoretrue-to_upperfalse-to_lowertrue)
@@ -93,15 +94,15 @@
 Returns:
  * ***current_timestamp (datetime Class):*** Datetime Class object - Used for difference calculations
  * ***filename_timestamp (str):*** Timestamp string formated 'YYYY-MM-DD_HHMMSS' - Used for filenames
  * ***log_timestamp (str):*** Timestamp string formated 'YYYY-MM-DD HH:MM:SS' - Used for logs
 
 Calculates the current time in UTC timezone and returns 3 variations to be used for different purposes.
 
-### **getDuration(then, now=datetime.datetime.now())**
+### **get_duration(then, now=datetime.datetime.now())**
 
 Arguments:
  * ***then (datetime Class):*** Datetime Class object representing the lower limit of a time comparison
  * ***now (datetime Class):*** Datetime Class object representing the upper limit of a time comparison
 
 Returns:
  * ***days_between (int):*** Days between two timestamps
```

### Comparing `nexus-utilities-0.4.0/nexus_utilities.egg-info/PKG-INFO` & `nexus-utilities-0.4.1/nexus_utilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus-utilities
-Version: 0.4.0
+Version: 0.4.1
 Summary: Common python utilities
 Home-page: https://github.com/james-larsen/nexus-utilities
 Author: James Larsen
 Author-email: james.larsen42@gmail.com
 License: UNKNOWN
 Description: This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.
 Platform: UNKNOWN
```

### Comparing `nexus-utilities-0.4.0/nexus_utils/config_utils.py` & `nexus-utilities-0.4.1/nexus_utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.4.0/nexus_utils/database_utils.py` & `nexus-utilities-0.4.1/nexus_utils/database_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.4.0/nexus_utils/datetime_utils.py` & `nexus-utilities-0.4.1/nexus_utils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.4.0/nexus_utils/package_utils.py` & `nexus-utilities-0.4.1/nexus_utils/package_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 """Utilities for working with Python packages"""
 import sys
 import os
 import inspect
 
 def add_package_to_path(verbose=False):
     """Programmatically determine the most likely root of the current running program, add its parent to the path, and return the root folder name"""
+    # Get the path of the calling script
+    calling_script = inspect.stack()[1].filename
+    calling_script_path = os.path.abspath(calling_script)
+    calling_script_dir = os.path.dirname(calling_script_path)
+
+    # Set the working directory to the calling script's directory
+    os.chdir(calling_script_dir)
+    
     # Define the list of common package root files and folders with lowercase
     package_root_items = ["src", "tests", "templates", "docs", "dist", "build", "readme.md", "license.txt", ".gitignore", "pyproject.toml", "requirements.txt", "poetry.lock", "setup.py", "manifest.in", ".editorconfig"]
 
     # Initialize a dictionary to store the count of package root items found in each directory
     item_counts = {}
 
     # Traverse upward from the current directory, counting the instances of package root items found in each directory
```

### Comparing `nexus-utilities-0.4.0/nexus_utils/password_utils.py` & `nexus-utilities-0.4.1/nexus_utils/password_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.4.0/nexus_utils/string_utils.py` & `nexus-utilities-0.4.1/nexus_utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.4.0/setup.py` & `nexus-utilities-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nexus-utilities',
-    version='0.4.0',
+    version='0.4.1',
     author='James Larsen',
     author_email='james.larsen42@gmail.com',
     description='Common python utilities',
     long_description='This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.',
     long_description_content_type='text/markdown',
     url='https://github.com/james-larsen/nexus-utilities',
     packages=['nexus_utils'],
```

