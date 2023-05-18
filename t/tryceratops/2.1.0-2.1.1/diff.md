# Comparing `tmp/tryceratops-2.1.0.tar.gz` & `tmp/tryceratops-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tryceratops-2.1.0.tar", max compression
+gzip compressed data, was "tryceratops-2.1.1.tar", max compression
```

## Comparing `tryceratops-2.1.0.tar` & `tryceratops-2.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1084 2023-05-13 18:43:29.642857 tryceratops-2.1.0/LICENSE
--rw-r--r--   0        0        0     6179 2023-05-13 18:43:59.494800 tryceratops-2.1.0/README.md
--rw-r--r--   0        0        0     2146 2023-05-13 18:43:59.538800 tryceratops-2.1.0/pyproject.toml
--rw-r--r--   0        0        0       69 2023-05-13 18:43:59.494800 tryceratops-2.1.0/src/tryceratops/__init__.py
--rw-r--r--   0        0        0     2220 2023-05-13 18:43:29.646857 tryceratops-2.1.0/src/tryceratops/__main__.py
--rw-r--r--   0        0        0     1090 2023-05-13 18:43:29.646857 tryceratops-2.1.0/src/tryceratops/analyzers/__init__.py
--rw-r--r--   0        0        0     1746 2023-05-13 18:43:29.646857 tryceratops-2.1.0/src/tryceratops/analyzers/base.py
--rw-r--r--   0        0        0     5616 2023-05-13 18:43:29.646857 tryceratops-2.1.0/src/tryceratops/analyzers/call.py
--rw-r--r--   0        0        0     2154 2023-05-13 18:43:29.646857 tryceratops-2.1.0/src/tryceratops/analyzers/conditional.py
--rw-r--r--   0        0        0     6385 2023-05-13 18:43:29.646857 tryceratops-2.1.0/src/tryceratops/analyzers/exception_block.py
--rw-r--r--   0        0        0      342 2023-05-13 18:43:29.646857 tryceratops-2.1.0/src/tryceratops/analyzers/exceptions.py
--rw-r--r--   0        0        0     1192 2023-05-13 18:43:29.646857 tryceratops-2.1.0/src/tryceratops/analyzers/try_block.py
--rw-r--r--   0        0        0       50 2023-05-13 18:43:29.646857 tryceratops-2.1.0/src/tryceratops/files/__init__.py
--rw-r--r--   0        0        0     3610 2023-05-13 18:43:29.646857 tryceratops-2.1.0/src/tryceratops/files/discovery.py
--rw-r--r--   0        0        0     1454 2023-05-13 18:43:29.646857 tryceratops-2.1.0/src/tryceratops/files/parser.py
--rw-r--r--   0        0        0     3126 2023-05-13 18:43:29.646857 tryceratops-2.1.0/src/tryceratops/filters.py
--rw-r--r--   0        0        0      601 2023-05-13 18:43:29.646857 tryceratops-2.1.0/src/tryceratops/fixers/__init__.py
--rw-r--r--   0        0        0     2653 2023-05-13 18:43:29.646857 tryceratops-2.1.0/src/tryceratops/fixers/base.py
--rw-r--r--   0        0        0     2747 2023-05-13 18:43:29.646857 tryceratops-2.1.0/src/tryceratops/fixers/exception_block.py
--rw-r--r--   0        0        0      353 2023-05-13 18:43:29.646857 tryceratops-2.1.0/src/tryceratops/fixers/exceptions.py
--rw-r--r--   0        0        0     2121 2023-05-13 18:43:29.646857 tryceratops-2.1.0/src/tryceratops/flake_plugin.py
--rw-r--r--   0        0        0     2715 2023-05-13 18:43:29.646857 tryceratops-2.1.0/src/tryceratops/interfaces.py
--rw-r--r--   0        0        0      165 2023-05-13 18:43:29.646857 tryceratops-2.1.0/src/tryceratops/processors.py
--rw-r--r--   0        0        0     3030 2023-05-13 18:43:29.646857 tryceratops-2.1.0/src/tryceratops/runners.py
--rw-r--r--   0        0        0     1065 2023-05-13 18:43:29.646857 tryceratops-2.1.0/src/tryceratops/settings.py
--rw-r--r--   0        0        0      629 2023-05-13 18:43:29.646857 tryceratops-2.1.0/src/tryceratops/types.py
--rw-r--r--   0        0        0      108 2023-05-13 18:43:29.646857 tryceratops-2.1.0/src/tryceratops/violations/__init__.py
--rw-r--r--   0        0        0     1389 2023-05-13 18:43:29.646857 tryceratops-2.1.0/src/tryceratops/violations/codes.py
--rw-r--r--   0        0        0     1773 2023-05-13 18:43:29.646857 tryceratops-2.1.0/src/tryceratops/violations/violations.py
--rw-r--r--   0        0        0     7358 1970-01-01 00:00:00.000000 tryceratops-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-05-18 08:27:50.690437 tryceratops-2.1.1/LICENSE
+-rw-r--r--   0        0        0     6179 2023-05-18 08:28:24.286208 tryceratops-2.1.1/README.md
+-rw-r--r--   0        0        0     2146 2023-05-18 08:28:24.330208 tryceratops-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-05-18 08:28:24.282209 tryceratops-2.1.1/src/tryceratops/__init__.py
+-rw-r--r--   0        0        0     2220 2023-05-18 08:27:50.694437 tryceratops-2.1.1/src/tryceratops/__main__.py
+-rw-r--r--   0        0        0     1090 2023-05-18 08:27:50.694437 tryceratops-2.1.1/src/tryceratops/analyzers/__init__.py
+-rw-r--r--   0        0        0     1746 2023-05-18 08:27:50.694437 tryceratops-2.1.1/src/tryceratops/analyzers/base.py
+-rw-r--r--   0        0        0     5616 2023-05-18 08:27:50.694437 tryceratops-2.1.1/src/tryceratops/analyzers/call.py
+-rw-r--r--   0        0        0     2154 2023-05-18 08:27:50.694437 tryceratops-2.1.1/src/tryceratops/analyzers/conditional.py
+-rw-r--r--   0        0        0     6385 2023-05-18 08:27:50.694437 tryceratops-2.1.1/src/tryceratops/analyzers/exception_block.py
+-rw-r--r--   0        0        0      342 2023-05-18 08:27:50.694437 tryceratops-2.1.1/src/tryceratops/analyzers/exceptions.py
+-rw-r--r--   0        0        0     1192 2023-05-18 08:27:50.694437 tryceratops-2.1.1/src/tryceratops/analyzers/try_block.py
+-rw-r--r--   0        0        0       50 2023-05-18 08:27:50.694437 tryceratops-2.1.1/src/tryceratops/files/__init__.py
+-rw-r--r--   0        0        0     3610 2023-05-18 08:27:50.694437 tryceratops-2.1.1/src/tryceratops/files/discovery.py
+-rw-r--r--   0        0        0     1454 2023-05-18 08:27:50.694437 tryceratops-2.1.1/src/tryceratops/files/parser.py
+-rw-r--r--   0        0        0     3126 2023-05-18 08:27:50.694437 tryceratops-2.1.1/src/tryceratops/filters.py
+-rw-r--r--   0        0        0      601 2023-05-18 08:27:50.694437 tryceratops-2.1.1/src/tryceratops/fixers/__init__.py
+-rw-r--r--   0        0        0     2653 2023-05-18 08:27:50.694437 tryceratops-2.1.1/src/tryceratops/fixers/base.py
+-rw-r--r--   0        0        0     2747 2023-05-18 08:27:50.694437 tryceratops-2.1.1/src/tryceratops/fixers/exception_block.py
+-rw-r--r--   0        0        0      353 2023-05-18 08:27:50.694437 tryceratops-2.1.1/src/tryceratops/fixers/exceptions.py
+-rw-r--r--   0        0        0     2121 2023-05-18 08:27:50.694437 tryceratops-2.1.1/src/tryceratops/flake_plugin.py
+-rw-r--r--   0        0        0     2715 2023-05-18 08:27:50.694437 tryceratops-2.1.1/src/tryceratops/interfaces.py
+-rw-r--r--   0        0        0      165 2023-05-18 08:27:50.698437 tryceratops-2.1.1/src/tryceratops/processors.py
+-rw-r--r--   0        0        0     3030 2023-05-18 08:27:50.698437 tryceratops-2.1.1/src/tryceratops/runners.py
+-rw-r--r--   0        0        0     1065 2023-05-18 08:27:50.698437 tryceratops-2.1.1/src/tryceratops/settings.py
+-rw-r--r--   0        0        0      629 2023-05-18 08:27:50.698437 tryceratops-2.1.1/src/tryceratops/types.py
+-rw-r--r--   0        0        0      108 2023-05-18 08:27:50.698437 tryceratops-2.1.1/src/tryceratops/violations/__init__.py
+-rw-r--r--   0        0        0     1389 2023-05-18 08:27:50.698437 tryceratops-2.1.1/src/tryceratops/violations/codes.py
+-rw-r--r--   0        0        0     1773 2023-05-18 08:27:50.698437 tryceratops-2.1.1/src/tryceratops/violations/violations.py
+-rw-r--r--   0        0        0     7358 1970-01-01 00:00:00.000000 tryceratops-2.1.1/PKG-INFO
```

### Comparing `tryceratops-2.1.0/LICENSE` & `tryceratops-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tryceratops-2.1.0/README.md` & `tryceratops-2.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
 
 ## Pre-commit
 
 If you wish to use pre-commit, add this:
 
 ```yaml
   - repo: https://github.com/guilatrova/tryceratops
-    rev: v2.1.0
+    rev: v2.1.1
     hooks:
       - id: tryceratops
 ```
 
 ## Show your style
 
 [![try/except style: tryceratops](https://img.shields.io/badge/try%2Fexcept%20style-tryceratops%20%F0%9F%A6%96%E2%9C%A8-black)](https://github.com/guilatrova/tryceratops)
```

### Comparing `tryceratops-2.1.0/pyproject.toml` & `tryceratops-2.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tryceratops"
-version = "2.1.0"
+version = "2.1.1"
 description = "Prevent Exception Handling AntiPatterns"
 authors = ["Guilherme Latrova <hello@guilatrova.dev>"]
 license = "MIT"
 keywords = ["lint", "try", "except"]
 readme = "README.md"
 homepage = "https://github.com/guilatrova/tryceratops"
 repository = "https://github.com/guilatrova/tryceratops"
```

### Comparing `tryceratops-2.1.0/src/tryceratops/__main__.py` & `tryceratops-2.1.1/src/tryceratops/__main__.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.1.0/src/tryceratops/analyzers/__init__.py` & `tryceratops-2.1.1/src/tryceratops/analyzers/__init__.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.1.0/src/tryceratops/analyzers/base.py` & `tryceratops-2.1.1/src/tryceratops/analyzers/base.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.1.0/src/tryceratops/analyzers/call.py` & `tryceratops-2.1.1/src/tryceratops/analyzers/call.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.1.0/src/tryceratops/analyzers/conditional.py` & `tryceratops-2.1.1/src/tryceratops/analyzers/conditional.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.1.0/src/tryceratops/analyzers/exception_block.py` & `tryceratops-2.1.1/src/tryceratops/analyzers/exception_block.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.1.0/src/tryceratops/analyzers/try_block.py` & `tryceratops-2.1.1/src/tryceratops/analyzers/try_block.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.1.0/src/tryceratops/files/discovery.py` & `tryceratops-2.1.1/src/tryceratops/files/discovery.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.1.0/src/tryceratops/files/parser.py` & `tryceratops-2.1.1/src/tryceratops/files/parser.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.1.0/src/tryceratops/filters.py` & `tryceratops-2.1.1/src/tryceratops/filters.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.1.0/src/tryceratops/fixers/__init__.py` & `tryceratops-2.1.1/src/tryceratops/fixers/__init__.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.1.0/src/tryceratops/fixers/base.py` & `tryceratops-2.1.1/src/tryceratops/fixers/base.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.1.0/src/tryceratops/fixers/exception_block.py` & `tryceratops-2.1.1/src/tryceratops/fixers/exception_block.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.1.0/src/tryceratops/flake_plugin.py` & `tryceratops-2.1.1/src/tryceratops/flake_plugin.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.1.0/src/tryceratops/interfaces.py` & `tryceratops-2.1.1/src/tryceratops/interfaces.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.1.0/src/tryceratops/runners.py` & `tryceratops-2.1.1/src/tryceratops/runners.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.1.0/src/tryceratops/settings.py` & `tryceratops-2.1.1/src/tryceratops/settings.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.1.0/src/tryceratops/types.py` & `tryceratops-2.1.1/src/tryceratops/types.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.1.0/src/tryceratops/violations/codes.py` & `tryceratops-2.1.1/src/tryceratops/violations/codes.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,13 +34,13 @@
     "TRY002",
     "TRY003",
     "TRY100",
     "TRY101",
     "TRY200",
     "TRY201",
     "TRY202",
+    "TRY203",
     "TRY300",
     "TRY301",
-    "TRY302",
     "TRY400",
     "TRY401",
 }
```

### Comparing `tryceratops-2.1.0/src/tryceratops/violations/violations.py` & `tryceratops-2.1.1/src/tryceratops/violations/violations.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.1.0/PKG-INFO` & `tryceratops-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tryceratops
-Version: 2.1.0
+Version: 2.1.1
 Summary: Prevent Exception Handling AntiPatterns
 Home-page: https://github.com/guilatrova/tryceratops
 License: MIT
 Keywords: lint,try,except
 Author: Guilherme Latrova
 Author-email: hello@guilatrova.dev
 Requires-Python: >=3.8,<4.0
@@ -169,15 +169,15 @@
 
 ## Pre-commit
 
 If you wish to use pre-commit, add this:
 
 ```yaml
   - repo: https://github.com/guilatrova/tryceratops
-    rev: v2.1.0
+    rev: v2.1.1
     hooks:
       - id: tryceratops
 ```
 
 ## Show your style
 
 [![try/except style: tryceratops](https://img.shields.io/badge/try%2Fexcept%20style-tryceratops%20%F0%9F%A6%96%E2%9C%A8-black)](https://github.com/guilatrova/tryceratops)
```

