# Comparing `tmp/config_joker-0.3.0.tar.gz` & `tmp/config_joker-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "config_joker-0.3.0.tar", max compression
+gzip compressed data, was "config_joker-0.4.0.tar", max compression
```

## Comparing `config_joker-0.3.0.tar` & `config_joker-0.4.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1083 2023-04-04 01:35:47.633704 config_joker-0.3.0/LICENSE
--rw-r--r--   0        0        0      796 2023-05-05 14:26:07.467811 config_joker-0.3.0/README.md
--rw-r--r--   0        0        0      122 2023-05-05 14:25:37.792222 config_joker-0.3.0/config_joker/__init__.py
--rw-r--r--   0        0        0     1293 2023-04-05 01:44:05.797405 config_joker-0.3.0/config_joker/config.py
--rw-r--r--   0        0        0        0 2023-04-04 02:48:43.263208 config_joker-0.3.0/config_joker/sources/__init__.py
--rw-r--r--   0        0        0      422 2023-04-04 03:07:58.416142 config_joker-0.3.0/config_joker/sources/environment.py
--rw-r--r--   0        0        0      360 2023-04-11 01:44:37.188523 config_joker-0.3.0/config_joker/sources/source.py
--rw-r--r--   0        0        0      680 2023-04-11 03:34:20.915789 config_joker-0.3.0/config_joker/sources/yamlfile.py
--rw-r--r--   0        0        0        0 2023-04-11 02:22:08.615358 config_joker-0.3.0/config_joker/utils/__init__.py
--rw-r--r--   0        0        0      997 2023-04-11 03:33:33.152316 config_joker-0.3.0/config_joker/utils/parser.py
--rw-r--r--   0        0        0      724 2023-05-05 15:00:55.393195 config_joker-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1340 1970-01-01 00:00:00.000000 config_joker-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-05-18 00:27:20.456274 config_joker-0.4.0/LICENSE
+-rw-r--r--   0        0        0      796 2023-05-18 00:27:20.456274 config_joker-0.4.0/README.md
+-rw-r--r--   0        0        0      122 2023-05-18 00:27:20.456274 config_joker-0.4.0/config_joker/__init__.py
+-rw-r--r--   0        0        0     1293 2023-05-18 00:27:20.456274 config_joker-0.4.0/config_joker/config.py
+-rw-r--r--   0        0        0        0 2023-05-18 00:27:20.456274 config_joker-0.4.0/config_joker/sources/__init__.py
+-rw-r--r--   0        0        0      422 2023-05-18 00:27:20.456274 config_joker-0.4.0/config_joker/sources/environment.py
+-rw-r--r--   0        0        0      360 2023-05-18 00:27:20.456274 config_joker-0.4.0/config_joker/sources/source.py
+-rw-r--r--   0        0        0      881 2023-05-18 00:27:20.456274 config_joker-0.4.0/config_joker/sources/yamlfile.py
+-rw-r--r--   0        0        0        0 2023-05-18 00:27:20.456274 config_joker-0.4.0/config_joker/utils/__init__.py
+-rw-r--r--   0        0        0      997 2023-05-18 00:27:20.456274 config_joker-0.4.0/config_joker/utils/parser.py
+-rw-r--r--   0        0        0      740 2023-05-18 00:27:20.456274 config_joker-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1375 1970-01-01 00:00:00.000000 config_joker-0.4.0/PKG-INFO
```

### Comparing `config_joker-0.3.0/LICENSE` & `config_joker-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `config_joker-0.3.0/README.md` & `config_joker-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `config_joker-0.3.0/config_joker/config.py` & `config_joker-0.4.0/config_joker/config.py`

 * *Files identical despite different names*

### Comparing `config_joker-0.3.0/config_joker/sources/yamlfile.py` & `config_joker-0.4.0/config_joker/sources/yamlfile.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from yaml import safe_load
 
 from config_joker.sources.source import Source, SourceResponse
 from config_joker.utils.parser import dict_extractor
 
 
 class YamlFileSource(Source):
-    def __init__(self, file_path: str) -> None:
+    def __init__(self, file_path: str, config_path: str = None) -> None:
         self._file_path = file_path
-        self._data = safe_load(self._file_path)
+        self._file_contents = safe_load(self._file_path)
+        if config_path:
+            self._data = dict_extractor(path=config_path, data=self._file_contents)
+        else:
+            self._data = self._file_contents
 
     def get_value(self, key: str) -> SourceResponse:
         try:
             response = dict_extractor(path=key, data=self._data)
             return SourceResponse(
                 exists=True,
                 value=response
```

### Comparing `config_joker-0.3.0/config_joker/utils/parser.py` & `config_joker-0.4.0/config_joker/utils/parser.py`

 * *Files identical despite different names*

### Comparing `config_joker-0.3.0/pyproject.toml` & `config_joker-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "config-joker"
-version = "0.3.0"
+version = "0.4.0"
 description = "A package to ease usage of different configuration conditions in your projects."
 authors = ["Joao Pedro Mendes Goulart"]
 readme = "README.md"
 packages = [
     {include = "config_joker"},
     {include = "./config_joker/config.py"},
     {include = "./config_joker/sources/environment.py"},
     {include = "./config_joker/sources/yamlfile.py"}
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 regex = "^2023.3.23"
+PyYAML = "^6.0"
 
 
 
 [tool.commitizen]
 name = "cz_conventional_commits"
 tag_format = "$version"
 version_type = "semver"
```

### Comparing `config_joker-0.3.0/PKG-INFO` & `config_joker-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: config-joker
-Version: 0.3.0
+Version: 0.4.0
 Summary: A package to ease usage of different configuration conditions in your projects.
 Author: Joao Pedro Mendes Goulart
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: regex (>=2023.3.23,<2024.0.0)
 Description-Content-Type: text/markdown
 
 # config-joker
 A package to ease usage of different configuration conditions in your projects.
 
 ## How to use in
```

