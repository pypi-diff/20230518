# Comparing `tmp/pycelium_specifications-0.0.2.1.tar.gz` & `tmp/pycelium_specifications-0.0.2.2.tar.gz`

## Comparing `pycelium_specifications-0.0.2.1.tar` & `pycelium_specifications-0.0.2.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.2.1/specifications/__init__.py
--rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.2.1/specifications/common.py
--rw-r--r--   0        0        0    15120 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.2.1/specifications/merkletree.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.2.1/.gitignore
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.2.1/license
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3159 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.2.1/readme.md
--rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.2.2/specifications/__init__.py
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.2.2/specifications/common.py
+-rw-r--r--   0        0        0    14995 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.2.2/specifications/merkletree.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.2.2/.gitignore
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.2.2/license
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.2.2/readme.md
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.2.2/PKG-INFO
```

### Comparing `pycelium_specifications-0.0.2.1/specifications/common.py` & `pycelium_specifications-0.0.2.2/specifications/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,14 +54,30 @@
     return [*_notes]
 
 def clear_notes() -> None:
     """Clears the list of notes."""
     _notes.clear()
 
 
+def post_test_report() -> None:
+    """Report the test results."""
+    print('')
+
+    for err in get_errors():
+        print(f'error: {err}')
+
+    for nt in get_notes():
+        print(f'note: {nt}')
+
+    if len(get_errors()) > 0:
+        print(f'Specification test failed with {len(get_errors())} error(s) and {len(get_notes())} note(s).')
+    else:
+        print(f'Sepcification test passed with {len(get_notes())} note(s).')
+
+
 class TestCase:
     label: str
     def __init__(self, label: str) -> None:
         self.label = label
 
     def __enter__(self) -> None:
         pass
```

### Comparing `pycelium_specifications-0.0.2.1/specifications/merkletree.py` & `pycelium_specifications-0.0.2.2/specifications/merkletree.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from __future__ import annotations
 from .common import (
     ImplementationError,
     TestCase,
     RaisesError,
     tressa,
     eton,
-    get_notes,
     clear_notes,
     error,
-    get_errors,
-    clear_errors
+    clear_errors,
+    post_test_report
 )
 from random import randint
 from typing import Any, Protocol, runtime_checkable
 import hashlib
 import traceback
 
 
@@ -114,21 +113,15 @@
             check_implementation(key, value)
         except BaseException as e:
             if e.__traceback__:
                 error(False, f'{e}: {traceback.format_exc()}')
             else:
                 error(False, f'{e}')
 
-    print('')
-
-    for err in get_errors():
-        print(f'error: {err}')
-
-    for nt in get_notes():
-        print(f'note: {nt}')
+    post_test_report()
 
 
 def check_implementation(implementation, protocol) -> None:
     """Checks the implementation of the protocol."""
     if protocol is MerkleTreeProtocol:
         check_implementation_of_MerkleTreeProtocol(implementation)
```

### Comparing `pycelium_specifications-0.0.2.1/license` & `pycelium_specifications-0.0.2.2/license`

 * *Files identical despite different names*

### Comparing `pycelium_specifications-0.0.2.1/pyproject.toml` & `pycelium_specifications-0.0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pycelium-specifications"
-version = "0.0.2.1"
+version = "0.0.2.2"
 authors = [
   { name="k98kurz", email="k98kurz@gmail.com" },
 ]
 description = "Library of common interfaces for the Pycelium project."
 readme = "readme.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pycelium_specifications-0.0.2.1/readme.md` & `pycelium_specifications-0.0.2.2/readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,18 @@
 There are two types of specification requirements: must-haves and should-haves.
 Any failure to meet a must-have requirement will be reported as an
 `ImplementationError`. Any detectable failure to meet a should-have requirement
 will be reported as an `ImplementationNote`. Not all should-have requirements
 can be automatically detected, e.g. lack of documentation or test coverage for
 additional features.
 
-The following subpackages are currently included:
+## Current Specifications
+
+The following specifications are currently included:
+
 - merkletree: a specification showing what a Merkle tree should do
 
 # ISC License
 
 Copyleft (c) 2023 k98kurz
 
 Permission to use, copy, modify, and/or distribute this software
```

### Comparing `pycelium_specifications-0.0.2.1/PKG-INFO` & `pycelium_specifications-0.0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycelium-specifications
-Version: 0.0.2.1
+Version: 0.0.2.2
 Summary: Library of common interfaces for the Pycelium project.
 Project-URL: Homepage, https://github.com/k98kurz/pycelium-specifications
 Project-URL: Bug Tracker, https://github.com/k98kurz/pycelium-specifications/issues
 Author-email: k98kurz <k98kurz@gmail.com>
 License-File: license
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
@@ -59,15 +59,18 @@
 There are two types of specification requirements: must-haves and should-haves.
 Any failure to meet a must-have requirement will be reported as an
 `ImplementationError`. Any detectable failure to meet a should-have requirement
 will be reported as an `ImplementationNote`. Not all should-have requirements
 can be automatically detected, e.g. lack of documentation or test coverage for
 additional features.
 
-The following subpackages are currently included:
+## Current Specifications
+
+The following specifications are currently included:
+
 - merkletree: a specification showing what a Merkle tree should do
 
 # ISC License
 
 Copyleft (c) 2023 k98kurz
 
 Permission to use, copy, modify, and/or distribute this software
```

