# Comparing `tmp/starrlib-0.1.0.tar.gz` & `tmp/starrlib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrlib-0.1.0.tar", max compression
+gzip compressed data, was "starrlib-0.1.1.tar", max compression
```

## Comparing `starrlib-0.1.0.tar` & `starrlib-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1064 2023-05-17 22:52:20.329540 starrlib-0.1.0/LICENSE
--rw-r--r--   0        0        0       55 2023-05-17 22:53:09.863440 starrlib-0.1.0/README.md
--rw-r--r--   0        0        0      667 2023-05-17 23:25:57.691371 starrlib-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      131 2023-05-17 23:34:48.177862 starrlib-0.1.0/starrlib/__init__.py
--rw-r--r--   0        0        0     2369 2023-05-17 23:34:35.154294 starrlib-0.1.0/starrlib/typed_bytes.py
--rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 starrlib-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-17 22:52:20.329540 starrlib-0.1.1/LICENSE
+-rw-r--r--   0        0        0       55 2023-05-17 22:53:09.863440 starrlib-0.1.1/README.md
+-rw-r--r--   0        0        0      667 2023-05-18 00:16:22.895789 starrlib-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      131 2023-05-17 23:34:48.177862 starrlib-0.1.1/starrlib/__init__.py
+-rw-r--r--   0        0        0     2387 2023-05-18 00:13:48.913289 starrlib-0.1.1/starrlib/typed_bytes.py
+-rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 starrlib-0.1.1/PKG-INFO
```

### Comparing `starrlib-0.1.0/LICENSE` & `starrlib-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `starrlib-0.1.0/pyproject.toml` & `starrlib-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "starrlib"
-version = "0.1.0"
+version = "0.1.1"
 description = "common starr utils"
 authors = ["StarrFox <starrfox6312@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/StarrFox/starrlib"
 
 [tool.poetry.dependencies]
```

### Comparing `starrlib-0.1.0/starrlib/typed_bytes.py` & `starrlib-0.1.1/starrlib/typed_bytes.py`

 * *Files 9% similar despite different names*

```diff
@@ -70,23 +70,23 @@
         return struct.unpack(type_format, data)[0]
 
     def write_typed(self, type_name: str, data) -> int:
         type_format = self.format_dict[type_name]
         packed = struct.pack(type_format, data)
         return self.buffer.write(packed)
 
-    def read_string(self, encoding: str = "utf-8") -> str:
-        string_len = self.read_typed("unsigned short")
+    def read_string(self, size_type: str, encoding: str = "utf-8") -> str:
+        string_len = self.read_typed(size_type)
         string_data = self.buffer.read(string_len)
         return string_data.decode(encoding=encoding)
 
-    def write_string(self, string: str, encoding: str = "utf-8"):
+    def write_string(self, size_type: str, string: str, encoding: str = "utf-8"):
         string_len = len(string)
         string_data = string.encode(encoding=encoding)
-        self.write_typed("unsigned short", string_len)
+        self.write_typed(size_type, string_len)
         self.buffer.write(string_data)
 
     def seek_forward_typed(self, type_name: str):
         at = self.buffer.tell()
         size = struct.calcsize(self.format_dict[type_name])
         self.buffer.seek(at + size)
```

### Comparing `starrlib-0.1.0/PKG-INFO` & `starrlib-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrlib
-Version: 0.1.0
+Version: 0.1.1
 Summary: common starr utils
 Home-page: https://github.com/StarrFox/starrlib
 License: MIT
 Author: StarrFox
 Author-email: starrfox6312@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

