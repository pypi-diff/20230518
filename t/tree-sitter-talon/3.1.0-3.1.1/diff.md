# Comparing `tmp/tree_sitter_talon-3.1.0.tar.gz` & `tmp/tree_sitter_talon-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tree_sitter_talon-3.1.0.tar", last modified: Thu Sep  1 17:23:17 2022, max compression
+gzip compressed data, was "tree_sitter_talon-3.1.1.tar", last modified: Mon Sep  5 12:37:07 2022, max compression
```

## Comparing `tree_sitter_talon-3.1.0.tar` & `tree_sitter_talon-3.1.1.tar`

### file list

```diff
@@ -1,49 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 17:23:17.659254 tree_sitter_talon-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-09-01 17:22:43.000000 tree_sitter_talon-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      987 2022-09-01 17:22:43.000000 tree_sitter_talon-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      925 2022-09-01 17:23:17.659254 tree_sitter_talon-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      297 2022-09-01 17:22:43.000000 tree_sitter_talon-3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1259 2022-09-01 17:22:43.000000 tree_sitter_talon-3.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-01 17:23:17.659254 tree_sitter_talon-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2856 2022-09-01 17:22:43.000000 tree_sitter_talon-3.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 17:23:17.655254 tree_sitter_talon-3.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1834 2022-09-01 17:22:43.000000 tree_sitter_talon-3.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      581 2022-09-01 17:22:43.000000 tree_sitter_talon-3.1.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (121)      293 2022-09-01 17:22:43.000000 tree_sitter_talon-3.1.0/tests/test_golden.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 17:23:17.655254 tree_sitter_talon-3.1.0/tree_sitter_talon/
--rw-r--r--   0 runner    (1001) docker     (121)     3215 2022-09-01 17:22:43.000000 tree_sitter_talon-3.1.0/tree_sitter_talon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      977 2022-09-01 17:22:43.000000 tree_sitter_talon-3.1.0/tree_sitter_talon/binding.c
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-09-01 17:22:43.000000 tree_sitter_talon-3.1.0/tree_sitter_talon/binding.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4436 2022-09-01 17:22:43.000000 tree_sitter_talon-3.1.0/tree_sitter_talon/core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 17:23:17.651254 tree_sitter_talon-3.1.0/tree_sitter_talon/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 17:23:17.655254 tree_sitter_talon-3.1.0/tree_sitter_talon/data/tree-sitter-talon/
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-09-01 17:22:43.000000 tree_sitter_talon-3.1.0/tree_sitter_talon/data/tree-sitter-talon/binding.gyp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 17:23:17.655254 tree_sitter_talon-3.1.0/tree_sitter_talon/data/tree-sitter-talon/bindings/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 17:23:17.655254 tree_sitter_talon-3.1.0/tree_sitter_talon/data/tree-sitter-talon/bindings/node/
--rw-r--r--   0 runner    (1001) docker     (121)      865 2022-09-01 17:22:43.000000 tree_sitter_talon-3.1.0/tree_sitter_talon/data/tree-sitter-talon/bindings/node/binding.cc
--rw-r--r--   0 runner    (1001) docker     (121)      461 2022-09-01 17:22:43.000000 tree_sitter_talon-3.1.0/tree_sitter_talon/data/tree-sitter-talon/bindings/node/index.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 17:23:17.655254 tree_sitter_talon-3.1.0/tree_sitter_talon/data/tree-sitter-talon/bindings/rust/
--rw-r--r--   0 runner    (1001) docker     (121)     1305 2022-09-01 17:22:43.000000 tree_sitter_talon-3.1.0/tree_sitter_talon/data/tree-sitter-talon/bindings/rust/build.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1943 2022-09-01 17:22:43.000000 tree_sitter_talon-3.1.0/tree_sitter_talon/data/tree-sitter-talon/bindings/rust/lib.rs
--rw-r--r--   0 runner    (1001) docker     (121)     7998 2022-09-01 17:22:43.000000 tree_sitter_talon-3.1.0/tree_sitter_talon/data/tree-sitter-talon/grammar.js
--rw-r--r--   0 runner    (1001) docker     (121)     1265 2022-09-01 17:22:43.000000 tree_sitter_talon-3.1.0/tree_sitter_talon/data/tree-sitter-talon/package.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 17:23:17.655254 tree_sitter_talon-3.1.0/tree_sitter_talon/data/tree-sitter-talon/src/
--rw-r--r--   0 runner    (1001) docker     (121)    37584 2022-09-01 17:22:43.000000 tree_sitter_talon-3.1.0/tree_sitter_talon/data/tree-sitter-talon/src/grammar.json
--rw-r--r--   0 runner    (1001) docker     (121)    16451 2022-09-01 17:22:43.000000 tree_sitter_talon-3.1.0/tree_sitter_talon/data/tree-sitter-talon/src/node-types.json
--rw-r--r--   0 runner    (1001) docker     (121)   185876 2022-09-01 17:22:43.000000 tree_sitter_talon-3.1.0/tree_sitter_talon/data/tree-sitter-talon/src/parser.c
--rw-r--r--   0 runner    (1001) docker     (121)    11232 2022-09-01 17:22:43.000000 tree_sitter_talon-3.1.0/tree_sitter_talon/data/tree-sitter-talon/src/scanner.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 17:23:17.655254 tree_sitter_talon-3.1.0/tree_sitter_talon/data/tree-sitter-talon/src/tree_sitter/
--rw-r--r--   0 runner    (1001) docker     (121)     5378 2022-09-01 17:22:43.000000 tree_sitter_talon-3.1.0/tree_sitter_talon/data/tree-sitter-talon/src/tree_sitter/parser.h
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-09-01 17:22:43.000000 tree_sitter_talon-3.1.0/tree_sitter_talon/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (121)     8199 2022-09-01 17:22:43.000000 tree_sitter_talon-3.1.0/tree_sitter_talon/dynamic.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 17:23:17.659254 tree_sitter_talon-3.1.0/tree_sitter_talon/extra/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-01 17:22:43.000000 tree_sitter_talon-3.1.0/tree_sitter_talon/extra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11757 2022-09-01 17:22:43.000000 tree_sitter_talon-3.1.0/tree_sitter_talon/extra/__pickle_compat.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-01 17:22:43.000000 tree_sitter_talon-3.1.0/tree_sitter_talon/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     3527 2022-09-01 17:22:43.000000 tree_sitter_talon-3.1.0/tree_sitter_talon/re.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 17:23:17.655254 tree_sitter_talon-3.1.0/tree_sitter_talon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      925 2022-09-01 17:23:17.000000 tree_sitter_talon-3.1.0/tree_sitter_talon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1327 2022-09-01 17:23:17.000000 tree_sitter_talon-3.1.0/tree_sitter_talon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-01 17:23:17.000000 tree_sitter_talon-3.1.0/tree_sitter_talon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-09-01 17:23:17.000000 tree_sitter_talon-3.1.0/tree_sitter_talon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-09-01 17:23:17.000000 tree_sitter_talon-3.1.0/tree_sitter_talon.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:37:07.818216 tree_sitter_talon-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-09-05 12:36:27.000000 tree_sitter_talon-3.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      987 2022-09-05 12:36:27.000000 tree_sitter_talon-3.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      925 2022-09-05 12:37:07.818216 tree_sitter_talon-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      297 2022-09-05 12:36:27.000000 tree_sitter_talon-3.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1259 2022-09-05 12:36:27.000000 tree_sitter_talon-3.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-05 12:37:07.818216 tree_sitter_talon-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2856 2022-09-05 12:36:27.000000 tree_sitter_talon-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:37:07.810216 tree_sitter_talon-3.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     1834 2022-09-05 12:36:27.000000 tree_sitter_talon-3.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      581 2022-09-05 12:36:27.000000 tree_sitter_talon-3.1.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)      293 2022-09-05 12:36:27.000000 tree_sitter_talon-3.1.1/tests/test_golden.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:37:07.814216 tree_sitter_talon-3.1.1/tree_sitter_talon/
+-rw-r--r--   0 runner    (1001) docker     (121)     3062 2022-09-05 12:36:27.000000 tree_sitter_talon-3.1.1/tree_sitter_talon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      977 2022-09-05 12:36:27.000000 tree_sitter_talon-3.1.1/tree_sitter_talon/binding.c
+-rw-r--r--   0 runner    (1001) docker     (121)       40 2022-09-05 12:36:27.000000 tree_sitter_talon-3.1.1/tree_sitter_talon/binding.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     4548 2022-09-05 12:36:27.000000 tree_sitter_talon-3.1.1/tree_sitter_talon/core.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:37:07.806216 tree_sitter_talon-3.1.1/tree_sitter_talon/data/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:37:07.814216 tree_sitter_talon-3.1.1/tree_sitter_talon/data/tree-sitter-talon/
+-rw-r--r--   0 runner    (1001) docker     (121)      335 2022-09-05 12:36:29.000000 tree_sitter_talon-3.1.1/tree_sitter_talon/data/tree-sitter-talon/binding.gyp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:37:07.806216 tree_sitter_talon-3.1.1/tree_sitter_talon/data/tree-sitter-talon/bindings/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:37:07.814216 tree_sitter_talon-3.1.1/tree_sitter_talon/data/tree-sitter-talon/bindings/node/
+-rw-r--r--   0 runner    (1001) docker     (121)      865 2022-09-05 12:36:29.000000 tree_sitter_talon-3.1.1/tree_sitter_talon/data/tree-sitter-talon/bindings/node/binding.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      461 2022-09-05 12:36:29.000000 tree_sitter_talon-3.1.1/tree_sitter_talon/data/tree-sitter-talon/bindings/node/index.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:37:07.814216 tree_sitter_talon-3.1.1/tree_sitter_talon/data/tree-sitter-talon/bindings/rust/
+-rw-r--r--   0 runner    (1001) docker     (121)     1305 2022-09-05 12:36:29.000000 tree_sitter_talon-3.1.1/tree_sitter_talon/data/tree-sitter-talon/bindings/rust/build.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1943 2022-09-05 12:36:29.000000 tree_sitter_talon-3.1.1/tree_sitter_talon/data/tree-sitter-talon/bindings/rust/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     7998 2022-09-05 12:36:29.000000 tree_sitter_talon-3.1.1/tree_sitter_talon/data/tree-sitter-talon/grammar.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1265 2022-09-05 12:36:29.000000 tree_sitter_talon-3.1.1/tree_sitter_talon/data/tree-sitter-talon/package.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:37:07.818216 tree_sitter_talon-3.1.1/tree_sitter_talon/data/tree-sitter-talon/src/
+-rw-r--r--   0 runner    (1001) docker     (121)    37584 2022-09-05 12:36:29.000000 tree_sitter_talon-3.1.1/tree_sitter_talon/data/tree-sitter-talon/src/grammar.json
+-rw-r--r--   0 runner    (1001) docker     (121)    16451 2022-09-05 12:36:29.000000 tree_sitter_talon-3.1.1/tree_sitter_talon/data/tree-sitter-talon/src/node-types.json
+-rw-r--r--   0 runner    (1001) docker     (121)   185876 2022-09-05 12:36:29.000000 tree_sitter_talon-3.1.1/tree_sitter_talon/data/tree-sitter-talon/src/parser.c
+-rw-r--r--   0 runner    (1001) docker     (121)    11232 2022-09-05 12:36:29.000000 tree_sitter_talon-3.1.1/tree_sitter_talon/data/tree-sitter-talon/src/scanner.cc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:37:07.818216 tree_sitter_talon-3.1.1/tree_sitter_talon/data/tree-sitter-talon/src/tree_sitter/
+-rw-r--r--   0 runner    (1001) docker     (121)     5378 2022-09-05 12:36:29.000000 tree_sitter_talon-3.1.1/tree_sitter_talon/data/tree-sitter-talon/src/tree_sitter/parser.h
+-rw-r--r--   0 runner    (1001) docker     (121)       89 2022-09-05 12:36:27.000000 tree_sitter_talon-3.1.1/tree_sitter_talon/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18658 2022-09-05 12:36:27.000000 tree_sitter_talon-3.1.1/tree_sitter_talon/dynamic.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    20023 2022-09-05 12:36:27.000000 tree_sitter_talon-3.1.1/tree_sitter_talon/extra.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 12:36:27.000000 tree_sitter_talon-3.1.1/tree_sitter_talon/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:37:07.814216 tree_sitter_talon-3.1.1/tree_sitter_talon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      925 2022-09-05 12:37:07.000000 tree_sitter_talon-3.1.1/tree_sitter_talon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1251 2022-09-05 12:37:07.000000 tree_sitter_talon-3.1.1/tree_sitter_talon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-05 12:37:07.000000 tree_sitter_talon-3.1.1/tree_sitter_talon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      248 2022-09-05 12:37:07.000000 tree_sitter_talon-3.1.1/tree_sitter_talon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-09-05 12:37:07.000000 tree_sitter_talon-3.1.1/tree_sitter_talon.egg-info/top_level.txt
```

### Comparing `tree_sitter_talon-3.1.0/LICENSE` & `tree_sitter_talon-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tree_sitter_talon-3.1.0/MANIFEST.in` & `tree_sitter_talon-3.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `tree_sitter_talon-3.1.0/PKG-INFO` & `tree_sitter_talon-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree_sitter_talon
-Version: 3.1.0
+Version: 3.1.1
 Summary: Parser for Talon files in Python
 Home-page: https://github.com/wenkokke/py-tree-sitter-talon
 Author: Wen Kokke
 License: MIT
 Project-URL: Documentation, https://wenkokke.github.io/py-tree-sitter-talon/
 Project-URL: Source, https://github.com/tree-sitter/py-tree-sitter
 Keywords: talon,parser
```

### Comparing `tree_sitter_talon-3.1.0/pyproject.toml` & `tree_sitter_talon-3.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 [tool.pytest.ini_options]
 enable_assertion_pass_hook = true
 filterwarnings = ["ignore::DeprecationWarning:.*:"]
 addopts = "--ignore=test/data"
 
 [tool.bumpver]
-current_version = "3.1.0"
+current_version = "3.1.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `tree_sitter_talon-3.1.0/setup.py` & `tree_sitter_talon-3.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 with open(os.path.join(os.path.dirname(__file__), "README.md")) as f:
     LONG_DESCRIPTION = f.read()
 
 setuptools.setup(
     name="tree_sitter_talon",
-    version="3.1.0",
+    version="3.1.1",
     description="Parser for Talon files in Python",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     author="Wen Kokke",
     url="https://github.com/wenkokke/py-tree-sitter-talon",
     project_urls={
         "Documentation": "https://wenkokke.github.io/py-tree-sitter-talon/",
```

### Comparing `tree_sitter_talon-3.1.0/tests/__init__.py` & `tree_sitter_talon-3.1.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tree_sitter_talon-3.1.0/tests/test_api.py` & `tree_sitter_talon-3.1.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `tree_sitter_talon-3.1.0/tree_sitter_talon/binding.c` & `tree_sitter_talon-3.1.1/tree_sitter_talon/binding.c`

 * *Files identical despite different names*

### Comparing `tree_sitter_talon-3.1.0/tree_sitter_talon/core.py` & `tree_sitter_talon-3.1.1/tree_sitter_talon/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 class TalonLanguage(tree_sitter.Language):
     def __init__(self):
         self.language_id = _tree_sitter_talon_id()
 
 
 class TreeSitterTalon(tree_sitter_type_provider.TreeSitterTypeProvider):
 
-    __version__: str = "3.1.0"
+    __version__: str = "3.1.1"
 
     _library_path: typing.Optional[str] = None
 
     _language: typing.Optional[tree_sitter.Language] = None
 
     _parser: typing.Optional[tree_sitter.Parser] = None
 
@@ -97,15 +97,18 @@
     ) -> typing.Union[
         typing.Sequence[tree_sitter_type_provider.Node],
         tree_sitter_type_provider.Node,
         None,
     ]:
         tree = self._parse(contents, encoding=encoding)
         return self.from_tree_sitter(
-            tree.root_node, filename=filename, raise_parse_error=raise_parse_error
+            tree.root_node,
+            encoding=encoding,
+            filename=filename,
+            raise_parse_error=raise_parse_error,
         )
 
     def parse_file(
         self,
         path: typing.Union[str, pathlib.Path],
         *,
         encoding: str = "utf-8",
@@ -113,15 +116,18 @@
     ) -> typing.Union[
         typing.Sequence[tree_sitter_type_provider.Node],
         tree_sitter_type_provider.Node,
         None,
     ]:
         tree = self._parse_file(path, encoding=encoding)
         return self.from_tree_sitter(
-            tree.root_node, filename=str(path), raise_parse_error=raise_parse_error
+            tree.root_node,
+            encoding=encoding,
+            filename=str(path),
+            raise_parse_error=raise_parse_error,
         )
 
     def _parse(
         self,
         contents: typing.Union[str, bytes],
         *,
         encoding: str = "utf-8",
```

### Comparing `tree_sitter_talon-3.1.0/tree_sitter_talon/data/tree-sitter-talon/bindings/node/binding.cc` & `tree_sitter_talon-3.1.1/tree_sitter_talon/data/tree-sitter-talon/bindings/node/binding.cc`

 * *Files identical despite different names*

### Comparing `tree_sitter_talon-3.1.0/tree_sitter_talon/data/tree-sitter-talon/bindings/rust/build.rs` & `tree_sitter_talon-3.1.1/tree_sitter_talon/data/tree-sitter-talon/bindings/rust/build.rs`

 * *Files identical despite different names*

### Comparing `tree_sitter_talon-3.1.0/tree_sitter_talon/data/tree-sitter-talon/bindings/rust/lib.rs` & `tree_sitter_talon-3.1.1/tree_sitter_talon/data/tree-sitter-talon/bindings/rust/lib.rs`

 * *Files identical despite different names*

### Comparing `tree_sitter_talon-3.1.0/tree_sitter_talon/data/tree-sitter-talon/grammar.js` & `tree_sitter_talon-3.1.1/tree_sitter_talon/data/tree-sitter-talon/grammar.js`

 * *Files identical despite different names*

### Comparing `tree_sitter_talon-3.1.0/tree_sitter_talon/data/tree-sitter-talon/package.json` & `tree_sitter_talon-3.1.1/tree_sitter_talon/data/tree-sitter-talon/package.json`

 * *Files identical despite different names*

### Comparing `tree_sitter_talon-3.1.0/tree_sitter_talon/data/tree-sitter-talon/src/grammar.json` & `tree_sitter_talon-3.1.1/tree_sitter_talon/data/tree-sitter-talon/src/grammar.json`

 * *Files identical despite different names*

### Comparing `tree_sitter_talon-3.1.0/tree_sitter_talon/data/tree-sitter-talon/src/node-types.json` & `tree_sitter_talon-3.1.1/tree_sitter_talon/data/tree-sitter-talon/src/node-types.json`

 * *Files identical despite different names*

### Comparing `tree_sitter_talon-3.1.0/tree_sitter_talon/data/tree-sitter-talon/src/parser.c` & `tree_sitter_talon-3.1.1/tree_sitter_talon/data/tree-sitter-talon/src/parser.c`

 * *Files identical despite different names*

### Comparing `tree_sitter_talon-3.1.0/tree_sitter_talon/data/tree-sitter-talon/src/scanner.cc` & `tree_sitter_talon-3.1.1/tree_sitter_talon/data/tree-sitter-talon/src/scanner.cc`

 * *Files identical despite different names*

### Comparing `tree_sitter_talon-3.1.0/tree_sitter_talon/data/tree-sitter-talon/src/tree_sitter/parser.h` & `tree_sitter_talon-3.1.1/tree_sitter_talon/data/tree-sitter-talon/src/tree_sitter/parser.h`

 * *Files identical despite different names*

### Comparing `tree_sitter_talon-3.1.0/tree_sitter_talon.egg-info/PKG-INFO` & `tree_sitter_talon-3.1.1/tree_sitter_talon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-sitter-talon
-Version: 3.1.0
+Version: 3.1.1
 Summary: Parser for Talon files in Python
 Home-page: https://github.com/wenkokke/py-tree-sitter-talon
 Author: Wen Kokke
 License: MIT
 Project-URL: Documentation, https://wenkokke.github.io/py-tree-sitter-talon/
 Project-URL: Source, https://github.com/tree-sitter/py-tree-sitter
 Keywords: talon,parser
```

### Comparing `tree_sitter_talon-3.1.0/tree_sitter_talon.egg-info/SOURCES.txt` & `tree_sitter_talon-3.1.1/tree_sitter_talon.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 tests/test_golden.py
 tree_sitter_talon/__init__.py
 tree_sitter_talon/binding.c
 tree_sitter_talon/binding.pyi
 tree_sitter_talon/core.py
 tree_sitter_talon/dynamic.py
 tree_sitter_talon/dynamic.pyi
+tree_sitter_talon/extra.py
 tree_sitter_talon/py.typed
-tree_sitter_talon/re.py
 tree_sitter_talon.egg-info/PKG-INFO
 tree_sitter_talon.egg-info/SOURCES.txt
 tree_sitter_talon.egg-info/dependency_links.txt
 tree_sitter_talon.egg-info/requires.txt
 tree_sitter_talon.egg-info/top_level.txt
 tree_sitter_talon/data/tree-sitter-talon/binding.gyp
 tree_sitter_talon/data/tree-sitter-talon/grammar.js
@@ -26,10 +26,8 @@
 tree_sitter_talon/data/tree-sitter-talon/bindings/node/index.js
 tree_sitter_talon/data/tree-sitter-talon/bindings/rust/build.rs
 tree_sitter_talon/data/tree-sitter-talon/bindings/rust/lib.rs
 tree_sitter_talon/data/tree-sitter-talon/src/grammar.json
 tree_sitter_talon/data/tree-sitter-talon/src/node-types.json
 tree_sitter_talon/data/tree-sitter-talon/src/parser.c
 tree_sitter_talon/data/tree-sitter-talon/src/scanner.cc
-tree_sitter_talon/data/tree-sitter-talon/src/tree_sitter/parser.h
-tree_sitter_talon/extra/__init__.py
-tree_sitter_talon/extra/__pickle_compat.py
+tree_sitter_talon/data/tree-sitter-talon/src/tree_sitter/parser.h
```

