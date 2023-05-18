# Comparing `tmp/pycelium_specifications-0.0.2.tar.gz` & `tmp/pycelium_specifications-0.0.2.1.tar.gz`

## Comparing `pycelium_specifications-0.0.2.tar` & `pycelium_specifications-0.0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.2/specifications/__init__.py
--rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.2/specifications/common.py
--rw-r--r--   0        0        0    15120 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.2/specifications/merkletree.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.2/.gitignore
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.2/license
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.2/readme.md
--rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.2.1/specifications/__init__.py
+-rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.2.1/specifications/common.py
+-rw-r--r--   0        0        0    15120 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.2.1/specifications/merkletree.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.2.1/.gitignore
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.2.1/license
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3159 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.2.1/readme.md
+-rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.2.1/PKG-INFO
```

### Comparing `pycelium_specifications-0.0.2/specifications/common.py` & `pycelium_specifications-0.0.2.1/specifications/common.py`

 * *Files identical despite different names*

### Comparing `pycelium_specifications-0.0.2/specifications/merkletree.py` & `pycelium_specifications-0.0.2.1/specifications/merkletree.py`

 * *Files identical despite different names*

### Comparing `pycelium_specifications-0.0.2/license` & `pycelium_specifications-0.0.2.1/license`

 * *Files identical despite different names*

### Comparing `pycelium_specifications-0.0.2/pyproject.toml` & `pycelium_specifications-0.0.2.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pycelium-specifications"
-version = "0.0.2"
+version = "0.0.2.1"
 authors = [
   { name="k98kurz", email="k98kurz@gmail.com" },
 ]
 description = "Library of common interfaces for the Pycelium project."
 readme = "readme.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pycelium_specifications-0.0.2/readme.md` & `pycelium_specifications-0.0.2.1/readme.md`

 * *Files 18% similar despite different names*

```diff
@@ -21,23 +21,23 @@
 protocol(s) and the `check_module` function. The `check_module` function is
 called by passing in a dict mapping implementation classes to protocols. For
 example:
 
 ```python
 from sepcifications.something import SomethingProtocol, check_module
 from someimplementation import SomethingClass
+import someimplementation
 
-check_module({
-    SomethingClass: SomethingProtocol
-})
+check_module(someimplementation, {SomethingClass: SomethingProtocol})
 ```
 
-The `check_module` function calls `check_implementation` for each (key, value)
-pair in the dict parameter, and this then runs a test suite on the
-implementation class. Any failures to meet the specification will be reported.
+The `check_module` function runs high-level tests on the module, then it
+calls `check_implementation` for each (key, value) pair in the dict parameter,
+and this then runs a test suite on the implementation class. Any failures to
+meet the specification will be reported.
 
 Note that some types of implementation failures will prevent the full test suite
 from running, e.g. failure to instantiate.
 
 There are two types of specification requirements: must-haves and should-haves.
 Any failure to meet a must-have requirement will be reported as an
 `ImplementationError`. Any detectable failure to meet a should-have requirement
```

### Comparing `pycelium_specifications-0.0.2/PKG-INFO` & `pycelium_specifications-0.0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycelium-specifications
-Version: 0.0.2
+Version: 0.0.2.1
 Summary: Library of common interfaces for the Pycelium project.
 Project-URL: Homepage, https://github.com/k98kurz/pycelium-specifications
 Project-URL: Bug Tracker, https://github.com/k98kurz/pycelium-specifications/issues
 Author-email: k98kurz <k98kurz@gmail.com>
 License-File: license
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
@@ -39,23 +39,23 @@
 protocol(s) and the `check_module` function. The `check_module` function is
 called by passing in a dict mapping implementation classes to protocols. For
 example:
 
 ```python
 from sepcifications.something import SomethingProtocol, check_module
 from someimplementation import SomethingClass
+import someimplementation
 
-check_module({
-    SomethingClass: SomethingProtocol
-})
+check_module(someimplementation, {SomethingClass: SomethingProtocol})
 ```
 
-The `check_module` function calls `check_implementation` for each (key, value)
-pair in the dict parameter, and this then runs a test suite on the
-implementation class. Any failures to meet the specification will be reported.
+The `check_module` function runs high-level tests on the module, then it
+calls `check_implementation` for each (key, value) pair in the dict parameter,
+and this then runs a test suite on the implementation class. Any failures to
+meet the specification will be reported.
 
 Note that some types of implementation failures will prevent the full test suite
 from running, e.g. failure to instantiate.
 
 There are two types of specification requirements: must-haves and should-haves.
 Any failure to meet a must-have requirement will be reported as an
 `ImplementationError`. Any detectable failure to meet a should-have requirement
```

