# Comparing `tmp/config_joker-0.4.0.tar.gz` & `tmp/config_joker-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "config_joker-0.4.0.tar", max compression
+gzip compressed data, was "config_joker-0.5.0.tar", max compression
```

## Comparing `config_joker-0.4.0.tar` & `config_joker-0.5.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1083 2023-05-18 00:27:20.456274 config_joker-0.4.0/LICENSE
--rw-r--r--   0        0        0      796 2023-05-18 00:27:20.456274 config_joker-0.4.0/README.md
--rw-r--r--   0        0        0      122 2023-05-18 00:27:20.456274 config_joker-0.4.0/config_joker/__init__.py
--rw-r--r--   0        0        0     1293 2023-05-18 00:27:20.456274 config_joker-0.4.0/config_joker/config.py
--rw-r--r--   0        0        0        0 2023-05-18 00:27:20.456274 config_joker-0.4.0/config_joker/sources/__init__.py
--rw-r--r--   0        0        0      422 2023-05-18 00:27:20.456274 config_joker-0.4.0/config_joker/sources/environment.py
--rw-r--r--   0        0        0      360 2023-05-18 00:27:20.456274 config_joker-0.4.0/config_joker/sources/source.py
--rw-r--r--   0        0        0      881 2023-05-18 00:27:20.456274 config_joker-0.4.0/config_joker/sources/yamlfile.py
--rw-r--r--   0        0        0        0 2023-05-18 00:27:20.456274 config_joker-0.4.0/config_joker/utils/__init__.py
--rw-r--r--   0        0        0      997 2023-05-18 00:27:20.456274 config_joker-0.4.0/config_joker/utils/parser.py
--rw-r--r--   0        0        0      740 2023-05-18 00:27:20.456274 config_joker-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1375 1970-01-01 00:00:00.000000 config_joker-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-05-18 02:32:12.162606 config_joker-0.5.0/LICENSE
+-rw-r--r--   0        0        0      796 2023-05-18 02:32:12.162606 config_joker-0.5.0/README.md
+-rw-r--r--   0        0        0      167 2023-05-18 02:32:12.162606 config_joker-0.5.0/config_joker/__init__.py
+-rw-r--r--   0        0        0     1293 2023-05-18 02:32:12.162606 config_joker-0.5.0/config_joker/config.py
+-rw-r--r--   0        0        0        0 2023-05-18 02:32:12.162606 config_joker-0.5.0/config_joker/sources/__init__.py
+-rw-r--r--   0        0        0      422 2023-05-18 02:32:12.162606 config_joker-0.5.0/config_joker/sources/environment.py
+-rw-r--r--   0        0        0      339 2023-05-18 02:32:12.162606 config_joker-0.5.0/config_joker/sources/jsonfile.py
+-rw-r--r--   0        0        0     1150 2023-05-18 02:32:12.162606 config_joker-0.5.0/config_joker/sources/source.py
+-rw-r--r--   0        0        0      354 2023-05-18 02:32:12.162606 config_joker-0.5.0/config_joker/sources/yamlfile.py
+-rw-r--r--   0        0        0        0 2023-05-18 02:32:12.162606 config_joker-0.5.0/config_joker/utils/__init__.py
+-rw-r--r--   0        0        0      997 2023-05-18 02:32:12.166607 config_joker-0.5.0/config_joker/utils/parser.py
+-rw-r--r--   0        0        0      740 2023-05-18 02:32:12.166607 config_joker-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1375 1970-01-01 00:00:00.000000 config_joker-0.5.0/PKG-INFO
```

### Comparing `config_joker-0.4.0/LICENSE` & `config_joker-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `config_joker-0.4.0/README.md` & `config_joker-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `config_joker-0.4.0/config_joker/config.py` & `config_joker-0.5.0/config_joker/config.py`

 * *Files identical despite different names*

### Comparing `config_joker-0.4.0/config_joker/sources/yamlfile.py` & `config_joker-0.5.0/config_joker/sources/source.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,42 @@
-from yaml import safe_load
+from typing import Any
+from abc import ABC, abstractmethod
 
-from config_joker.sources.source import Source, SourceResponse
+from dataclasses import dataclass
 from config_joker.utils.parser import dict_extractor
 
 
-class YamlFileSource(Source):
+@dataclass
+class SourceResponse:
+    exists: bool
+    value: Any
+
+
+class Source(ABC):
+    @abstractmethod
+    def get_value(self, key: str) -> SourceResponse:
+        'Get the value in the source using the key'
+
+
+class SourceAsDict(Source):
     def __init__(self, file_path: str, config_path: str = None) -> None:
-        self._file_path = file_path
-        self._file_contents = safe_load(self._file_path)
+        self._file_contents = self._load_from_file(file_path)
         if config_path:
             self._data = dict_extractor(path=config_path, data=self._file_contents)
         else:
             self._data = self._file_contents
 
+    def _load_from_file(self, path: str) -> dict:
+        raise NotImplementedError()
+
     def get_value(self, key: str) -> SourceResponse:
         try:
             response = dict_extractor(path=key, data=self._data)
             return SourceResponse(
                 exists=True,
                 value=response
             )
         except KeyError:
             return SourceResponse(
                 exists=False,
                 value=None
-            )
+            )
```

### Comparing `config_joker-0.4.0/config_joker/utils/parser.py` & `config_joker-0.5.0/config_joker/utils/parser.py`

 * *Files identical despite different names*

### Comparing `config_joker-0.4.0/pyproject.toml` & `config_joker-0.5.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "config-joker"
-version = "0.4.0"
+version = "0.5.0"
 description = "A package to ease usage of different configuration conditions in your projects."
 authors = ["Joao Pedro Mendes Goulart"]
 readme = "README.md"
 packages = [
     {include = "config_joker"},
     {include = "./config_joker/config.py"},
     {include = "./config_joker/sources/environment.py"},
```

### Comparing `config_joker-0.4.0/PKG-INFO` & `config_joker-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: config-joker
-Version: 0.4.0
+Version: 0.5.0
 Summary: A package to ease usage of different configuration conditions in your projects.
 Author: Joao Pedro Mendes Goulart
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

