# Comparing `tmp/hart-protocol-2023.4.0.tar.gz` & `tmp/hart_protocol-2023.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hart-protocol-2023.4.0.tar", last modified: Fri Apr 14 16:44:54 2023, max compression
+gzip compressed data, was "hart_protocol-2023.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `hart-protocol-2023.4.0.tar` & `hart_protocol-2023.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      429 2023-04-14 16:44:50.237508 hart-protocol-2023.4.0/.github/workflows/python-mypy.yml
--rw-r--r--   0        0        0      793 2023-04-14 16:44:50.237508 hart-protocol-2023.4.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      447 2023-04-14 16:44:50.237508 hart-protocol-2023.4.0/.gitignore
--rw-r--r--   0        0        0      649 2023-04-14 16:44:50.237508 hart-protocol-2023.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1155 2023-04-14 16:44:50.237508 hart-protocol-2023.4.0/CHANGELOG.md
--rw-r--r--   0        0        0     1100 2023-04-14 16:44:50.237508 hart-protocol-2023.4.0/LICENSE
--rw-r--r--   0        0        0     8501 2023-04-14 16:44:50.237508 hart-protocol-2023.4.0/README.md
--rw-r--r--   0        0        0        9 2023-04-14 16:44:50.237508 hart-protocol-2023.4.0/hart_protocol/VERSION
--rw-r--r--   0        0        0      212 2023-04-14 16:44:50.237508 hart-protocol-2023.4.0/hart_protocol/__init__.py
--rw-r--r--   0        0        0      493 2023-04-14 16:44:50.237508 hart-protocol-2023.4.0/hart_protocol/__version__.py
--rw-r--r--   0        0        0     7840 2023-04-14 16:44:50.237508 hart-protocol-2023.4.0/hart_protocol/_parsing.py
--rw-r--r--   0        0        0     4087 2023-04-14 16:44:50.237508 hart-protocol-2023.4.0/hart_protocol/_unpacker.py
--rw-r--r--   0        0        0     1348 2023-04-14 16:44:50.237508 hart-protocol-2023.4.0/hart_protocol/common.py
--rw-r--r--   0        0        0        0 2023-04-14 16:44:50.237508 hart-protocol-2023.4.0/hart_protocol/py.typed
--rw-r--r--   0        0        0     1576 2023-04-14 16:44:50.237508 hart-protocol-2023.4.0/hart_protocol/tools.py
--rw-r--r--   0        0        0     2205 2023-04-14 16:44:50.237508 hart-protocol-2023.4.0/hart_protocol/universal.py
--rw-r--r--   0        0        0     1220 2023-04-14 16:44:50.237508 hart-protocol-2023.4.0/pyproject.toml
--rw-r--r--   0        0        0     9558 1970-01-01 00:00:00.000000 hart-protocol-2023.4.0/PKG-INFO
+-rw-r--r--   0        0        0      429 2023-05-18 21:03:57.831139 hart_protocol-2023.5.0/.github/workflows/python-mypy.yml
+-rw-r--r--   0        0        0      793 2023-05-18 21:03:57.831139 hart_protocol-2023.5.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      447 2023-05-18 21:03:57.831139 hart_protocol-2023.5.0/.gitignore
+-rw-r--r--   0        0        0      649 2023-05-18 21:03:57.831139 hart_protocol-2023.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1305 2023-05-18 21:03:57.831139 hart_protocol-2023.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1100 2023-05-18 21:03:57.831139 hart_protocol-2023.5.0/LICENSE
+-rw-r--r--   0        0        0     8501 2023-05-18 21:03:57.831139 hart_protocol-2023.5.0/README.md
+-rw-r--r--   0        0        0        9 2023-05-18 21:03:57.835138 hart_protocol-2023.5.0/hart_protocol/VERSION
+-rw-r--r--   0        0        0      212 2023-05-18 21:03:57.835138 hart_protocol-2023.5.0/hart_protocol/__init__.py
+-rw-r--r--   0        0        0      493 2023-05-18 21:03:57.835138 hart_protocol-2023.5.0/hart_protocol/__version__.py
+-rw-r--r--   0        0        0     7840 2023-05-18 21:03:57.835138 hart_protocol-2023.5.0/hart_protocol/_parsing.py
+-rw-r--r--   0        0        0     4087 2023-05-18 21:03:57.835138 hart_protocol-2023.5.0/hart_protocol/_unpacker.py
+-rw-r--r--   0        0        0     1348 2023-05-18 21:03:57.835138 hart_protocol-2023.5.0/hart_protocol/common.py
+-rw-r--r--   0        0        0        0 2023-05-18 21:03:57.835138 hart_protocol-2023.5.0/hart_protocol/py.typed
+-rw-r--r--   0        0        0     1576 2023-05-18 21:03:57.835138 hart_protocol-2023.5.0/hart_protocol/tools.py
+-rw-r--r--   0        0        0     2205 2023-05-18 21:03:57.835138 hart_protocol-2023.5.0/hart_protocol/universal.py
+-rw-r--r--   0        0        0     1220 2023-05-18 21:03:57.835138 hart_protocol-2023.5.0/pyproject.toml
+-rw-r--r--   0        0        0     9558 1970-01-01 00:00:00.000000 hart_protocol-2023.5.0/PKG-INFO
```

### Comparing `hart-protocol-2023.4.0/.github/workflows/python-publish.yml` & `hart_protocol-2023.5.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `hart-protocol-2023.4.0/.pre-commit-config.yaml` & `hart_protocol-2023.5.0/.pre-commit-config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,15 @@
       - id: black
         name: black
         entry: black
         require_serial: true
         types: [python]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.2.0
+    rev: v1.3.0
     hooks:
       - id: mypy
         exclude: ^docs/conf.py
 
   - repo: https://gitlab.com/yaq/yaq-traits
     rev: v2022.3.0
     hooks:
```

### Comparing `hart-protocol-2023.4.0/CHANGELOG.md` & `hart_protocol-2023.5.0/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/).
 
 ## [Unreleased]
 
+## [2023.5.0]
+
+### Fixed
+- missing final byte from message 16
+
 ## [2023.4.0]
 
 ### Fixed
 - missing final byte from messages 12, 13, 14, 17, 18
 
 ## [2023.3.0]
 
@@ -27,13 +32,14 @@
 - unpacker was broken in an async context
 
 ## [2022.8.0]
 
 ### Added
 - initial release
 
-[Unreleased]: https://github.com/yaq-project/hart-protocol/compare/v2023.4.0...main
+[Unreleased]: https://github.com/yaq-project/hart-protocol/compare/v2023.5.0...main
+[2023.5.0]: https://github.com/yaq-project/hart-protocol/compare/v2023.4.0...v2023.5.0
 [2023.4.0]: https://github.com/yaq-project/hart-protocol/compare/v2023.3.0...v2023.4.0
 [2023.3.0]: https://github.com/yaq-project/hart-protocol/compare/v2022.8.2...v2023.3.0
 [2022.8.2]: https://github.com/yaq-project/hart-protocol/compare/v2022.8.1...v2022.8.2
 [2022.8.1]: https://github.com/yaq-project/hart-protocol/compare/v2022.8.0...v2022.8.1
 [2022.8.0]: https://gitlab.com/yaq/yaqd-picotech/tags/v2022.8.0
```

### Comparing `hart-protocol-2023.4.0/LICENSE` & `hart_protocol-2023.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hart-protocol-2023.4.0/README.md` & `hart_protocol-2023.5.0/README.md`

 * *Files identical despite different names*

### Comparing `hart-protocol-2023.4.0/hart_protocol/_parsing.py` & `hart_protocol-2023.5.0/hart_protocol/_parsing.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         out["upper_range_value"] = upper_range_value
         out["lower_range_value"] = lower_range_value
         out["damping_value"] = damping_value
         out["write_protect"] = write_protect
         out["private_label"] = private_label
     elif command in [16]:
         out["command_name"] = "read_final_assembly_number"
-        out["final_assembly_no"] = int.from_bytes(data[0:2], "big")
+        out["final_assembly_no"] = int.from_bytes(data[0:3], "big")
     elif command in [17]:
         out["command_name"] = "write_message"
         out["message"] = data[0:24]
     elif command in [18]:
         out["command_name"] = "write_tag_descriptor_date"
         out["device_tag_name"] = data[0:6]
         out["device_descriptor"] = data[6:18]
```

### Comparing `hart-protocol-2023.4.0/hart_protocol/_unpacker.py` & `hart_protocol-2023.5.0/hart_protocol/_unpacker.py`

 * *Files identical despite different names*

### Comparing `hart-protocol-2023.4.0/hart_protocol/common.py` & `hart_protocol-2023.5.0/hart_protocol/common.py`

 * *Files identical despite different names*

### Comparing `hart-protocol-2023.4.0/hart_protocol/tools.py` & `hart_protocol-2023.5.0/hart_protocol/tools.py`

 * *Files identical despite different names*

### Comparing `hart-protocol-2023.4.0/hart_protocol/universal.py` & `hart_protocol-2023.5.0/hart_protocol/universal.py`

 * *Files identical despite different names*

### Comparing `hart-protocol-2023.4.0/pyproject.toml` & `hart_protocol-2023.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hart-protocol-2023.4.0/PKG-INFO` & `hart_protocol-2023.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hart-protocol
-Version: 2023.4.0
+Version: 2023.5.0
 Summary: A sans-io python implementation of the Highway Addressable Remote Transducer Protocol.
 Home-page: https://github.com/yaq-project/hart-protocol
 Author: Blaise Thompson
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

