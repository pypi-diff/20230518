# Comparing `tmp/py21cmemu-1.0.5.dev0.tar.gz` & `tmp/py21cmemu-1.0.6.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py21cmemu-1.0.5.dev0.tar", max compression
+gzip compressed data, was "py21cmemu-1.0.6.dev0.tar", max compression
```

## Comparing `py21cmemu-1.0.5.dev0.tar` & `py21cmemu-1.0.6.dev0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1073 2023-03-03 11:01:58.918549 py21cmemu-1.0.5.dev0/LICENSE
--rw-r--r--   0        0        0     2441 2023-05-17 16:21:22.516197 py21cmemu-1.0.5.dev0/README.rst
--rw-r--r--   0        0        0     2370 2023-05-18 10:38:20.000046 py21cmemu-1.0.5.dev0/pyproject.toml
--rw-r--r--   0        0        0      213 2023-05-16 14:39:00.912610 py21cmemu-1.0.5.dev0/src/py21cmemu/__init__.py
--rw-r--r--   0        0        0     2776 2023-05-09 14:54:55.861960 py21cmemu-1.0.5.dev0/src/py21cmemu/config.py
--rw-r--r--   0        0        0     3510 2023-05-04 09:57:53.996907 py21cmemu-1.0.5.dev0/src/py21cmemu/emulator.py
--rw-r--r--   0        0        0    14978 2023-05-04 09:52:14.387649 py21cmemu-1.0.5.dev0/src/py21cmemu/emulator_constants.npz
--rw-r--r--   0        0        0     1199 2023-05-03 14:37:25.023190 py21cmemu-1.0.5.dev0/src/py21cmemu/get_emulator.py
--rw-r--r--   0        0        0     5483 2023-05-05 12:51:51.765886 py21cmemu-1.0.5.dev0/src/py21cmemu/inputs.py
--rw-r--r--   0        0        0     7254 2023-05-05 09:35:21.501068 py21cmemu-1.0.5.dev0/src/py21cmemu/outputs.py
--rw-r--r--   0        0        0     2795 2023-05-04 13:04:49.223046 py21cmemu-1.0.5.dev0/src/py21cmemu/properties.py
--rw-r--r--   0        0        0     3761 1970-01-01 00:00:00.000000 py21cmemu-1.0.5.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-18 12:15:48.906323 py21cmemu-1.0.6.dev0/LICENSE
+-rw-r--r--   0        0        0     2441 2023-05-18 12:15:48.906323 py21cmemu-1.0.6.dev0/README.rst
+-rw-r--r--   0        0        0     2372 2023-05-18 12:16:07.594564 py21cmemu-1.0.6.dev0/pyproject.toml
+-rw-r--r--   0        0        0      410 2023-05-18 12:16:07.594564 py21cmemu-1.0.6.dev0/src/py21cmemu/__init__.py
+-rw-r--r--   0        0        0     2776 2023-05-18 12:15:48.926323 py21cmemu-1.0.6.dev0/src/py21cmemu/config.py
+-rw-r--r--   0        0        0     3542 2023-05-18 12:16:07.594564 py21cmemu-1.0.6.dev0/src/py21cmemu/emulator.py
+-rw-r--r--   0        0        0    14978 2023-05-18 12:15:48.930323 py21cmemu-1.0.6.dev0/src/py21cmemu/emulator_constants.npz
+-rw-r--r--   0        0        0     1199 2023-05-18 12:15:48.930323 py21cmemu-1.0.6.dev0/src/py21cmemu/get_emulator.py
+-rw-r--r--   0        0        0     5483 2023-05-18 12:15:48.930323 py21cmemu-1.0.6.dev0/src/py21cmemu/inputs.py
+-rw-r--r--   0        0        0     7303 2023-05-18 12:16:07.594564 py21cmemu-1.0.6.dev0/src/py21cmemu/outputs.py
+-rw-r--r--   0        0        0     2795 2023-05-18 12:15:48.930323 py21cmemu-1.0.6.dev0/src/py21cmemu/properties.py
+-rw-r--r--   0        0        0     3912 1970-01-01 00:00:00.000000 py21cmemu-1.0.6.dev0/PKG-INFO
```

### Comparing `py21cmemu-1.0.5.dev0/LICENSE` & `py21cmemu-1.0.6.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `py21cmemu-1.0.5.dev0/README.rst` & `py21cmemu-1.0.6.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `py21cmemu-1.0.5.dev0/pyproject.toml` & `py21cmemu-1.0.6.dev0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py21cmEMU"
-version = "1.0.5dev"
+version = "1.0.6.dev0"
 description = "Emulator of 21cmFAST summaries."
 authors = ["Daniela Breitman <daniela.breitman@sns.it>"]
 license = "MIT"
 readme = ["README.rst"]
 homepage = "https://github.com/21cmFAST/21cmEMU"
 repository = "https://github.com/21cmFAST/21cmEMU"
 documentation = "https://21cmEMU.readthedocs.io"
```

### Comparing `py21cmemu-1.0.5.dev0/src/py21cmemu/config.py` & `py21cmemu-1.0.6.dev0/src/py21cmemu/config.py`

 * *Files identical despite different names*

### Comparing `py21cmemu-1.0.5.dev0/src/py21cmemu/emulator.py` & `py21cmemu-1.0.6.dev0/src/py21cmemu/emulator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""The actual emulator code."""
+"""Module that interacts with the Emulator Tensorflow model."""
 from __future__ import annotations
 
 import logging
 from typing import Any
 
 import numpy as np
 import tensorflow as tf
```

### Comparing `py21cmemu-1.0.5.dev0/src/py21cmemu/emulator_constants.npz` & `py21cmemu-1.0.6.dev0/src/py21cmemu/emulator_constants.npz`

 * *Files identical despite different names*

### Comparing `py21cmemu-1.0.5.dev0/src/py21cmemu/get_emulator.py` & `py21cmemu-1.0.6.dev0/src/py21cmemu/get_emulator.py`

 * *Files identical despite different names*

### Comparing `py21cmemu-1.0.5.dev0/src/py21cmemu/inputs.py` & `py21cmemu-1.0.6.dev0/src/py21cmemu/inputs.py`

 * *Files identical despite different names*

### Comparing `py21cmemu-1.0.5.dev0/src/py21cmemu/outputs.py` & `py21cmemu-1.0.6.dev0/src/py21cmemu/outputs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Output class."""
+"""Module whose functionality is to organise the emulator output."""
 from __future__ import annotations
 
 import dataclasses as dc
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Generator
```

### Comparing `py21cmemu-1.0.5.dev0/src/py21cmemu/properties.py` & `py21cmemu-1.0.6.dev0/src/py21cmemu/properties.py`

 * *Files identical despite different names*

### Comparing `py21cmemu-1.0.5.dev0/PKG-INFO` & `py21cmemu-1.0.6.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py21cmemu
-Version: 1.0.5.dev0
+Version: 1.0.6.dev0
 Summary: Emulator of 21cmFAST summaries.
 Home-page: https://github.com/21cmFAST/21cmEMU
 License: MIT
 Keywords: Epoch of Reionization,Cosmology
 Author: Daniela Breitman
 Author-email: daniela.breitman@sns.it
 Requires-Python: >=3.8,<3.12
@@ -14,15 +14,18 @@
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: GitPython (>=3.1.31,<4.0.0)
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: click (>=8.0.1)
 Requires-Dist: numpy (>=1.22.0,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: tensorflow (>=2.6.0,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
```

