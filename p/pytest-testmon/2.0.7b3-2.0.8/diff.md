# Comparing `tmp/pytest-testmon-2.0.7b3.tar.gz` & `tmp/pytest-testmon-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-testmon-2.0.7b3.tar", last modified: Fri May 12 12:45:43 2023, max compression
+gzip compressed data, was "pytest-testmon-2.0.8.tar", last modified: Thu May 18 06:49:44 2023, max compression
```

## Comparing `pytest-testmon-2.0.7b3.tar` & `pytest-testmon-2.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 tibor      (502) staff       (20)        0 2023-05-12 12:45:43.294234 pytest-testmon-2.0.7b3/
--rw-r--r--   0 tibor      (502) staff       (20)    34633 2023-01-17 15:34:55.000000 pytest-testmon-2.0.7b3/LICENSE
--rw-r--r--   0 tibor      (502) staff       (20)       74 2023-05-02 14:55:45.000000 pytest-testmon-2.0.7b3/MANIFEST.in
--rw-r--r--   0 tibor      (502) staff       (20)     2431 2023-05-12 12:45:43.294311 pytest-testmon-2.0.7b3/PKG-INFO
--rw-r--r--   0 tibor      (502) staff       (20)     1208 2023-05-02 14:55:45.000000 pytest-testmon-2.0.7b3/README.md
--rw-r--r--   0 tibor      (502) staff       (20)     1619 2023-05-12 12:40:21.000000 pytest-testmon-2.0.7b3/pyproject.toml
-drwxr-xr-x   0 tibor      (502) staff       (20)        0 2023-05-12 12:45:43.292067 pytest-testmon-2.0.7b3/pytest_testmon.egg-info/
--rw-r--r--   0 tibor      (502) staff       (20)     2431 2023-05-12 12:45:43.000000 pytest-testmon-2.0.7b3/pytest_testmon.egg-info/PKG-INFO
--rw-r--r--   0 tibor      (502) staff       (20)      463 2023-05-12 12:45:43.000000 pytest-testmon-2.0.7b3/pytest_testmon.egg-info/SOURCES.txt
--rw-r--r--   0 tibor      (502) staff       (20)        1 2023-05-12 12:45:43.000000 pytest-testmon-2.0.7b3/pytest_testmon.egg-info/dependency_links.txt
--rw-r--r--   0 tibor      (502) staff       (20)       51 2023-05-12 12:45:43.000000 pytest-testmon-2.0.7b3/pytest_testmon.egg-info/entry_points.txt
--rw-r--r--   0 tibor      (502) staff       (20)       28 2023-05-12 12:45:43.000000 pytest-testmon-2.0.7b3/pytest_testmon.egg-info/requires.txt
--rw-r--r--   0 tibor      (502) staff       (20)        8 2023-05-12 12:45:43.000000 pytest-testmon-2.0.7b3/pytest_testmon.egg-info/top_level.txt
--rw-r--r--   0 tibor      (502) staff       (20)     1219 2023-05-12 12:45:43.294598 pytest-testmon-2.0.7b3/setup.cfg
--rw-r--r--   0 tibor      (502) staff       (20)       69 2023-05-12 12:40:21.000000 pytest-testmon-2.0.7b3/setup.py
-drwxr-xr-x   0 tibor      (502) staff       (20)        0 2023-05-12 12:45:43.294012 pytest-testmon-2.0.7b3/testmon/
--rw-r--r--   0 tibor      (502) staff       (20)       46 2023-05-12 12:40:22.000000 pytest-testmon-2.0.7b3/testmon/__init__.py
--rw-r--r--   0 tibor      (502) staff       (20)     2125 2023-05-12 12:40:22.000000 pytest-testmon-2.0.7b3/testmon/common.py
--rw-r--r--   0 tibor      (502) staff       (20)     3786 2023-05-12 12:40:22.000000 pytest-testmon-2.0.7b3/testmon/configure.py
--rw-r--r--   0 tibor      (502) staff       (20)    22743 2023-05-12 12:40:22.000000 pytest-testmon-2.0.7b3/testmon/db.py
--rw-r--r--   0 tibor      (502) staff       (20)     8052 2023-05-12 12:40:22.000000 pytest-testmon-2.0.7b3/testmon/process_code.py
--rw-r--r--   0 tibor      (502) staff       (20)    16979 2023-05-12 12:40:21.000000 pytest-testmon-2.0.7b3/testmon/pytest_testmon.py
--rw-r--r--   0 tibor      (502) staff       (20)    19133 2023-05-12 12:40:22.000000 pytest-testmon-2.0.7b3/testmon/testmon_core.py
--rw-r--r--   0 tibor      (502) staff       (20)     1232 2023-01-18 05:16:27.000000 pytest-testmon-2.0.7b3/testmon/tox_testmon.py
+drwxr-xr-x   0 tibor      (502) staff       (20)        0 2023-05-18 06:49:44.223853 pytest-testmon-2.0.8/
+-rw-r--r--   0 tibor      (502) staff       (20)    34633 2023-01-17 15:34:55.000000 pytest-testmon-2.0.8/LICENSE
+-rw-r--r--   0 tibor      (502) staff       (20)       74 2023-05-02 14:55:45.000000 pytest-testmon-2.0.8/MANIFEST.in
+-rw-r--r--   0 tibor      (502) staff       (20)     2429 2023-05-18 06:49:44.223936 pytest-testmon-2.0.8/PKG-INFO
+-rw-r--r--   0 tibor      (502) staff       (20)     1208 2023-05-02 14:55:45.000000 pytest-testmon-2.0.8/README.md
+-rw-r--r--   0 tibor      (502) staff       (20)     1619 2023-05-18 06:49:21.000000 pytest-testmon-2.0.8/pyproject.toml
+drwxr-xr-x   0 tibor      (502) staff       (20)        0 2023-05-18 06:49:44.221526 pytest-testmon-2.0.8/pytest_testmon.egg-info/
+-rw-r--r--   0 tibor      (502) staff       (20)     2429 2023-05-18 06:49:44.000000 pytest-testmon-2.0.8/pytest_testmon.egg-info/PKG-INFO
+-rw-r--r--   0 tibor      (502) staff       (20)      463 2023-05-18 06:49:44.000000 pytest-testmon-2.0.8/pytest_testmon.egg-info/SOURCES.txt
+-rw-r--r--   0 tibor      (502) staff       (20)        1 2023-05-18 06:49:44.000000 pytest-testmon-2.0.8/pytest_testmon.egg-info/dependency_links.txt
+-rw-r--r--   0 tibor      (502) staff       (20)       51 2023-05-18 06:49:44.000000 pytest-testmon-2.0.8/pytest_testmon.egg-info/entry_points.txt
+-rw-r--r--   0 tibor      (502) staff       (20)       28 2023-05-18 06:49:44.000000 pytest-testmon-2.0.8/pytest_testmon.egg-info/requires.txt
+-rw-r--r--   0 tibor      (502) staff       (20)        8 2023-05-18 06:49:44.000000 pytest-testmon-2.0.8/pytest_testmon.egg-info/top_level.txt
+-rw-r--r--   0 tibor      (502) staff       (20)     1219 2023-05-18 06:49:44.224236 pytest-testmon-2.0.8/setup.cfg
+-rw-r--r--   0 tibor      (502) staff       (20)       69 2023-05-18 06:49:21.000000 pytest-testmon-2.0.8/setup.py
+drwxr-xr-x   0 tibor      (502) staff       (20)        0 2023-05-18 06:49:44.223487 pytest-testmon-2.0.8/testmon/
+-rw-r--r--   0 tibor      (502) staff       (20)       44 2023-05-18 06:49:22.000000 pytest-testmon-2.0.8/testmon/__init__.py
+-rw-r--r--   0 tibor      (502) staff       (20)     2149 2023-05-18 06:49:22.000000 pytest-testmon-2.0.8/testmon/common.py
+-rw-r--r--   0 tibor      (502) staff       (20)     3786 2023-05-18 06:49:22.000000 pytest-testmon-2.0.8/testmon/configure.py
+-rw-r--r--   0 tibor      (502) staff       (20)    22743 2023-05-18 06:49:22.000000 pytest-testmon-2.0.8/testmon/db.py
+-rw-r--r--   0 tibor      (502) staff       (20)     8052 2023-05-18 06:49:22.000000 pytest-testmon-2.0.8/testmon/process_code.py
+-rw-r--r--   0 tibor      (502) staff       (20)    16979 2023-05-18 06:49:21.000000 pytest-testmon-2.0.8/testmon/pytest_testmon.py
+-rw-r--r--   0 tibor      (502) staff       (20)    19133 2023-05-18 06:49:21.000000 pytest-testmon-2.0.8/testmon/testmon_core.py
+-rw-r--r--   0 tibor      (502) staff       (20)     1232 2023-01-18 05:16:27.000000 pytest-testmon-2.0.8/testmon/tox_testmon.py
```

### Comparing `pytest-testmon-2.0.7b3/LICENSE` & `pytest-testmon-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-testmon-2.0.7b3/PKG-INFO` & `pytest-testmon-2.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-testmon
-Version: 2.0.7b3
+Version: 2.0.8
 Summary: selects tests affected by changed files and methods
 Home-page: https://testmon.org
 Author: Tibor Arpas, Tomas Matlovic
 Author-email: Tibor Arpas <tibor@testmon.org>
 License: AGPL
 Project-URL: Source, https://github.com/tarpas/pytest-testmon
 Keywords: testing,pytest,plugin
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytest-testmon Version: 2.0.7b3 Summary: selects
+Metadata-Version: 2.1 Name: pytest-testmon Version: 2.0.8 Summary: selects
 tests affected by changed files and methods Home-page: https://testmon.org
 Author: Tibor Arpas, Tomas Matlovic Author-email: Tibor Arpas
 testmon.org> License: AGPL Project-URL: Source, https://github.com/tarpas/
 pytest-testmon Keywords: testing,pytest,plugin Platform: linux Platform: osx
 Platform: win32 Classifier: Development Status :: 4 - Beta Classifier: Intended
 Audience :: Developers Classifier: Operating System :: POSIX Classifier:
 Operating System :: Microsoft :: Windows Classifier: Operating System :: MacOS
```

### Comparing `pytest-testmon-2.0.7b3/README.md` & `pytest-testmon-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pytest-testmon-2.0.7b3/pyproject.toml` & `pytest-testmon-2.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest-testmon-2.0.7b3/pytest_testmon.egg-info/PKG-INFO` & `pytest-testmon-2.0.8/pytest_testmon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-testmon
-Version: 2.0.7b3
+Version: 2.0.8
 Summary: selects tests affected by changed files and methods
 Home-page: https://testmon.org
 Author: Tibor Arpas, Tomas Matlovic
 Author-email: Tibor Arpas <tibor@testmon.org>
 License: AGPL
 Project-URL: Source, https://github.com/tarpas/pytest-testmon
 Keywords: testing,pytest,plugin
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytest-testmon Version: 2.0.7b3 Summary: selects
+Metadata-Version: 2.1 Name: pytest-testmon Version: 2.0.8 Summary: selects
 tests affected by changed files and methods Home-page: https://testmon.org
 Author: Tibor Arpas, Tomas Matlovic Author-email: Tibor Arpas
 testmon.org> License: AGPL Project-URL: Source, https://github.com/tarpas/
 pytest-testmon Keywords: testing,pytest,plugin Platform: linux Platform: osx
 Platform: win32 Classifier: Development Status :: 4 - Beta Classifier: Intended
 Audience :: Developers Classifier: Operating System :: POSIX Classifier:
 Operating System :: Microsoft :: Windows Classifier: Operating System :: MacOS
```

### Comparing `pytest-testmon-2.0.7b3/setup.cfg` & `pytest-testmon-2.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytest-testmon-2.0.7b3/testmon/common.py` & `pytest-testmon-2.0.8/testmon/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import re
 
 try:
     import importlib.metadata
 
     def get_system_packages_raw():
         return (
-            f"{pkg.name} {pkg.version}" for pkg in importlib.metadata.distributions()
+            f"{pkg.metadata['Name']} {pkg.version}"
+            for pkg in importlib.metadata.distributions()
         )
 
 except ImportError:
     import pkg_resources
 
     def get_system_packages_raw():
         return (
```

### Comparing `pytest-testmon-2.0.7b3/testmon/configure.py` & `pytest-testmon-2.0.8/testmon/configure.py`

 * *Files identical despite different names*

### Comparing `pytest-testmon-2.0.7b3/testmon/db.py` & `pytest-testmon-2.0.8/testmon/db.py`

 * *Files identical despite different names*

### Comparing `pytest-testmon-2.0.7b3/testmon/process_code.py` & `pytest-testmon-2.0.8/testmon/process_code.py`

 * *Files identical despite different names*

### Comparing `pytest-testmon-2.0.7b3/testmon/pytest_testmon.py` & `pytest-testmon-2.0.8/testmon/pytest_testmon.py`

 * *Files identical despite different names*

### Comparing `pytest-testmon-2.0.7b3/testmon/testmon_core.py` & `pytest-testmon-2.0.8/testmon/testmon_core.py`

 * *Files identical despite different names*

### Comparing `pytest-testmon-2.0.7b3/testmon/tox_testmon.py` & `pytest-testmon-2.0.8/testmon/tox_testmon.py`

 * *Files identical despite different names*

