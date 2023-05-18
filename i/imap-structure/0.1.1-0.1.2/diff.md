# Comparing `tmp/imap_structure-0.1.1.tar.gz` & `tmp/imap_structure-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imap_structure-0.1.1.tar", max compression
+gzip compressed data, was "imap_structure-0.1.2.tar", max compression
```

## Comparing `imap_structure-0.1.1.tar` & `imap_structure-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       44 2023-05-18 02:15:45.592944 imap_structure-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-05-18 02:11:07.503068 imap_structure-0.1.1/imap_structure/__init__.py
--rw-r--r--   0        0        0    10088 2023-05-18 02:13:15.533013 imap_structure-0.1.1/imap_structure/body_structure.py
--rw-r--r--   0        0        0     4816 2023-05-18 02:50:48.401972 imap_structure-0.1.1/imap_structure/metadata.py
--rw-r--r--   0        0        0     1467 2023-05-18 02:13:15.573013 imap_structure-0.1.1/imap_structure/parser.py
--rw-r--r--   0        0        0      540 2023-05-18 02:51:21.481960 imap_structure-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      707 1970-01-01 00:00:00.000000 imap_structure-0.1.1/setup.py
--rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 imap_structure-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       44 2023-05-18 03:04:19.021602 imap_structure-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-18 03:04:19.021602 imap_structure-0.1.2/imap_structure/__init__.py
+-rw-r--r--   0        0        0    10793 2023-05-18 04:10:01.609785 imap_structure-0.1.2/imap_structure/body_structure.py
+-rw-r--r--   0        0        0     4816 2023-05-18 03:04:19.021602 imap_structure-0.1.2/imap_structure/metadata.py
+-rw-r--r--   0        0        0     1467 2023-05-18 03:04:19.021602 imap_structure-0.1.2/imap_structure/parser.py
+-rw-r--r--   0        0        0      540 2023-05-18 04:10:40.839765 imap_structure-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      707 1970-01-01 00:00:00.000000 imap_structure-0.1.2/setup.py
+-rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 imap_structure-0.1.2/PKG-INFO
```

### Comparing `imap_structure-0.1.1/imap_structure/body_structure.py` & `imap_structure-0.1.2/imap_structure/body_structure.py`

 * *Files 8% similar despite different names*

```diff
@@ -99,19 +99,35 @@
     def body_part(self) -> BodyPart:
         return extract_body_part(self.parse_results)
 
     @cached_property
     def text_sections(self) -> list[tuple[str, str]]:
         return extract_text_sections(self.body_part)
 
+    def attachments(self):
+        for part in self.body_part.children:
+            if not isinstance(part, BodyPartNonMultipart):
+                continue
+            if part.body_disposition is None:
+                continue
+            if "attachment" not in part.body_disposition:
+                continue
+            disposition = part.body_disposition.as_list()
+            if len(disposition) > 1 and isinstance(disposition[1], list):
+                filename_idx = disposition[1].index("filename")
+                if len(disposition[1]) > filename_idx + 1:
+                    filename = disposition[1][filename_idx + 1]
+                    yield filename
+
     @cached_property
     def has_attachment(self) -> bool:
         return any(
-            part.mime_type[0].lower() == "application"
-            and part.mime_type[1].lower() == "octet-stream"
+            isinstance(part, BodyPartNonMultipart)
+            and part.body_disposition is not None
+            and "attachment" in part.body_disposition
             for part in self.body_part.children
         )
 
 
 def parse_body_structure(body_structure: str) -> BodyStructure:
     """
     Parse BODYSTRUCTURE into AST.
```

### Comparing `imap_structure-0.1.1/imap_structure/metadata.py` & `imap_structure-0.1.2/imap_structure/metadata.py`

 * *Files identical despite different names*

### Comparing `imap_structure-0.1.1/imap_structure/parser.py` & `imap_structure-0.1.2/imap_structure/parser.py`

 * *Files identical despite different names*

### Comparing `imap_structure-0.1.1/pyproject.toml` & `imap_structure-0.1.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "imap-structure"
-version = "0.1.1"
+version = "0.1.2"
 description = "IMAP BODYSTRUCTURE parser"
 authors = ["Kiruya Momochi <65301509+kiruyamomochi@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "imap_structure" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `imap_structure-0.1.1/setup.py` & `imap_structure-0.1.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pyparsing>=3.0.9,<4.0.0']
 
 setup_kwargs = {
     'name': 'imap-structure',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'IMAP BODYSTRUCTURE parser',
     'long_description': '# imap-structure\n\nIMAP BODYSTRUCTURE parser\n',
     'author': 'Kiruya Momochi',
     'author_email': '65301509+kiruyamomochi@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

