# Comparing `tmp/tree_sitter_type_provider-2.1.7.tar.gz` & `tmp/tree_sitter_type_provider-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tree_sitter_type_provider-2.1.7.tar", last modified: Tue Sep  6 17:24:23 2022, max compression
+gzip compressed data, was "tree_sitter_type_provider-2.1.8.tar", last modified: Wed Sep  7 12:22:48 2022, max compression
```

## Comparing `tree_sitter_type_provider-2.1.7.tar` & `tree_sitter_type_provider-2.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 17:24:23.173268 tree_sitter_type_provider-2.1.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-09-06 17:24:00.000000 tree_sitter_type_provider-2.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-09-06 17:24:00.000000 tree_sitter_type_provider-2.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2758 2022-09-06 17:24:23.173268 tree_sitter_type_provider-2.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2282 2022-09-06 17:24:00.000000 tree_sitter_type_provider-2.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1458 2022-09-06 17:24:00.000000 tree_sitter_type_provider-2.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-06 17:24:23.173268 tree_sitter_type_provider-2.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 17:24:23.169268 tree_sitter_type_provider-2.1.7/tree_sitter_type_provider/
--rw-r--r--   0 runner    (1001) docker     (121)    10696 2022-09-06 17:24:00.000000 tree_sitter_type_provider-2.1.7/tree_sitter_type_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8153 2022-09-06 17:24:00.000000 tree_sitter_type_provider-2.1.7/tree_sitter_type_provider/node_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     2112 2022-09-06 17:24:00.000000 tree_sitter_type_provider-2.1.7/tree_sitter_type_provider/parse_error.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-06 17:24:00.000000 tree_sitter_type_provider-2.1.7/tree_sitter_type_provider/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 17:24:23.173268 tree_sitter_type_provider-2.1.7/tree_sitter_type_provider.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2758 2022-09-06 17:24:23.000000 tree_sitter_type_provider-2.1.7/tree_sitter_type_provider.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-09-06 17:24:23.000000 tree_sitter_type_provider-2.1.7/tree_sitter_type_provider.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-06 17:24:23.000000 tree_sitter_type_provider-2.1.7/tree_sitter_type_provider.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-09-06 17:24:23.000000 tree_sitter_type_provider-2.1.7/tree_sitter_type_provider.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-09-06 17:24:23.000000 tree_sitter_type_provider-2.1.7/tree_sitter_type_provider.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 12:22:48.817985 tree_sitter_type_provider-2.1.8/
+-rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-09-07 12:21:58.000000 tree_sitter_type_provider-2.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       77 2022-09-07 12:21:58.000000 tree_sitter_type_provider-2.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2758 2022-09-07 12:22:48.817985 tree_sitter_type_provider-2.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2282 2022-09-07 12:21:58.000000 tree_sitter_type_provider-2.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1467 2022-09-07 12:21:58.000000 tree_sitter_type_provider-2.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-07 12:22:48.817985 tree_sitter_type_provider-2.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 12:22:48.817985 tree_sitter_type_provider-2.1.8/tree_sitter_type_provider/
+-rw-r--r--   0 runner    (1001) docker     (121)    10696 2022-09-07 12:21:58.000000 tree_sitter_type_provider-2.1.8/tree_sitter_type_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8153 2022-09-07 12:21:58.000000 tree_sitter_type_provider-2.1.8/tree_sitter_type_provider/node_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2112 2022-09-07 12:21:58.000000 tree_sitter_type_provider-2.1.8/tree_sitter_type_provider/parse_error.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-07 12:21:58.000000 tree_sitter_type_provider-2.1.8/tree_sitter_type_provider/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 12:22:48.817985 tree_sitter_type_provider-2.1.8/tree_sitter_type_provider.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2758 2022-09-07 12:22:48.000000 tree_sitter_type_provider-2.1.8/tree_sitter_type_provider.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      442 2022-09-07 12:22:48.000000 tree_sitter_type_provider-2.1.8/tree_sitter_type_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-07 12:22:48.000000 tree_sitter_type_provider-2.1.8/tree_sitter_type_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      149 2022-09-07 12:22:48.000000 tree_sitter_type_provider-2.1.8/tree_sitter_type_provider.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2022-09-07 12:22:48.000000 tree_sitter_type_provider-2.1.8/tree_sitter_type_provider.egg-info/top_level.txt
```

### Comparing `tree_sitter_type_provider-2.1.7/LICENSE` & `tree_sitter_type_provider-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tree_sitter_type_provider-2.1.7/PKG-INFO` & `tree_sitter_type_provider-2.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree_sitter_type_provider
-Version: 2.1.7
+Version: 2.1.8
 Summary: Type providers for tree-sitter in Python
 Author: Wen Kokke
 Project-URL: repository, https://github.com/wenkokke/py-tree-sitter-type-provider
 Keywords: type-provider
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Compilers
 Requires-Python: >=3.9
```

### Comparing `tree_sitter_type_provider-2.1.7/README.md` & `tree_sitter_type_provider-2.1.8/README.md`

 * *Files identical despite different names*

### Comparing `tree_sitter_type_provider-2.1.7/pyproject.toml` & `tree_sitter_type_provider-2.1.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tree_sitter_type_provider"
-version = "2.1.7"
+version = "2.1.8"
 description = "Type providers for tree-sitter in Python"
 requires-python = ">=3.9"
 keywords = ["type-provider"]
 authors = [{ name = "Wen Kokke" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Topic :: Software Development :: Compilers",
 ]
-dependencies = ["tree-sitter ==0.20.0", "dataclasses-json >=0.5.7, <0.6"]
+dependencies = ["tree-sitter >=0.20.0, <0.20.2", "dataclasses-json >=0.5.7, <0.6"]
 
 [project.optional-dependencies]
 dev = ["build >=0.8.0, <0.9", "twine >=4.0.1, <5"]
 test = ["pytest >=7.1.2, <8", "pytest-golden >=0.2.2, <0.3"]
 
 [project.readme]
 file = "README.md"
@@ -33,15 +33,15 @@
 testpaths = "tests"
 
 [tool.pytest.ini_options]
 enable_assertion_pass_hook = true
 filterwarnings = ["ignore::DeprecationWarning:.*:"]
 
 [tool.bumpver]
-current_version = "2.1.7"
+current_version = "2.1.8"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `tree_sitter_type_provider-2.1.7/tree_sitter_type_provider/__init__.py` & `tree_sitter_type_provider-2.1.8/tree_sitter_type_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `tree_sitter_type_provider-2.1.7/tree_sitter_type_provider/node_types.py` & `tree_sitter_type_provider-2.1.8/tree_sitter_type_provider/node_types.py`

 * *Files identical despite different names*

### Comparing `tree_sitter_type_provider-2.1.7/tree_sitter_type_provider/parse_error.py` & `tree_sitter_type_provider-2.1.8/tree_sitter_type_provider/parse_error.py`

 * *Files identical despite different names*

### Comparing `tree_sitter_type_provider-2.1.7/tree_sitter_type_provider.egg-info/PKG-INFO` & `tree_sitter_type_provider-2.1.8/tree_sitter_type_provider.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-sitter-type-provider
-Version: 2.1.7
+Version: 2.1.8
 Summary: Type providers for tree-sitter in Python
 Author: Wen Kokke
 Project-URL: repository, https://github.com/wenkokke/py-tree-sitter-type-provider
 Keywords: type-provider
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Compilers
 Requires-Python: >=3.9
```

