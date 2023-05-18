# Comparing `tmp/doc_printer-0.8.4.tar.gz` & `tmp/doc_printer-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doc_printer-0.8.4.tar", last modified: Mon Aug  1 18:07:54 2022, max compression
+gzip compressed data, was "doc_printer-0.9.0.tar", last modified: Tue Aug  2 20:14:36 2022, max compression
```

## Comparing `doc_printer-0.8.4.tar` & `doc_printer-0.9.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 wen        (502) staff       (20)        0 2022-08-01 18:07:54.812052 doc_printer-0.8.4/
--rw-r--r--   0 wen        (502) staff       (20)     1066 2022-07-21 20:02:47.000000 doc_printer-0.8.4/LICENSE
--rw-r--r--   0 wen        (502) staff       (20)       63 2022-07-21 20:55:00.000000 doc_printer-0.8.4/MANIFEST.in
--rw-r--r--   0 wen        (502) staff       (20)      845 2022-08-01 18:07:54.811732 doc_printer-0.8.4/PKG-INFO
--rw-r--r--   0 wen        (502) staff       (20)      325 2022-07-21 21:01:42.000000 doc_printer-0.8.4/README.md
-drwxr-xr-x   0 wen        (502) staff       (20)        0 2022-08-01 18:07:54.802687 doc_printer-0.8.4/doc_printer/
--rw-r--r--   0 wen        (502) staff       (20)     1312 2022-08-01 18:00:41.000000 doc_printer-0.8.4/doc_printer/__init__.py
--rw-r--r--   0 wen        (502) staff       (20)      598 2022-08-01 16:39:30.000000 doc_printer-0.8.4/doc_printer/abc.py
--rw-r--r--   0 wen        (502) staff       (20)    16404 2022-08-01 18:00:01.000000 doc_printer-0.8.4/doc_printer/doc.py
--rw-r--r--   0 wen        (502) staff       (20)        0 2022-07-21 20:02:47.000000 doc_printer-0.8.4/doc_printer/py.typed
--rw-r--r--   0 wen        (502) staff       (20)     4751 2022-08-01 18:00:31.000000 doc_printer-0.8.4/doc_printer/simple.py
--rw-r--r--   0 wen        (502) staff       (20)     1531 2022-08-01 17:59:06.000000 doc_printer-0.8.4/doc_printer/smart.py
--rw-r--r--   0 wen        (502) staff       (20)     4382 2022-08-01 17:56:32.000000 doc_printer-0.8.4/doc_printer/table.py
-drwxr-xr-x   0 wen        (502) staff       (20)        0 2022-08-01 18:07:54.810077 doc_printer-0.8.4/doc_printer.egg-info/
--rw-r--r--   0 wen        (502) staff       (20)      845 2022-08-01 18:07:54.000000 doc_printer-0.8.4/doc_printer.egg-info/PKG-INFO
--rw-r--r--   0 wen        (502) staff       (20)      402 2022-08-01 18:07:54.000000 doc_printer-0.8.4/doc_printer.egg-info/SOURCES.txt
--rw-r--r--   0 wen        (502) staff       (20)        1 2022-08-01 18:07:54.000000 doc_printer-0.8.4/doc_printer.egg-info/dependency_links.txt
--rw-r--r--   0 wen        (502) staff       (20)       92 2022-08-01 18:07:54.000000 doc_printer-0.8.4/doc_printer.egg-info/requires.txt
--rw-r--r--   0 wen        (502) staff       (20)       12 2022-08-01 18:07:54.000000 doc_printer-0.8.4/doc_printer.egg-info/top_level.txt
--rw-r--r--   0 wen        (502) staff       (20)     1258 2022-08-01 18:01:02.000000 doc_printer-0.8.4/pyproject.toml
--rw-r--r--   0 wen        (502) staff       (20)       38 2022-08-01 18:07:54.812190 doc_printer-0.8.4/setup.cfg
-drwxr-xr-x   0 wen        (502) staff       (20)        0 2022-08-01 18:07:54.810994 doc_printer-0.8.4/test/
--rw-r--r--   0 wen        (502) staff       (20)     2020 2022-08-01 15:58:50.000000 doc_printer-0.8.4/test/test_doc.py
--rw-r--r--   0 wen        (502) staff       (20)     1479 2022-08-01 15:58:50.000000 doc_printer-0.8.4/test/test_simple.py
+drwxr-xr-x   0 wen        (502) staff       (20)        0 2022-08-02 20:14:36.343910 doc_printer-0.9.0/
+-rw-r--r--   0 wen        (502) staff       (20)     1066 2022-07-21 20:02:47.000000 doc_printer-0.9.0/LICENSE
+-rw-r--r--   0 wen        (502) staff       (20)       63 2022-07-21 20:55:00.000000 doc_printer-0.9.0/MANIFEST.in
+-rw-r--r--   0 wen        (502) staff       (20)      869 2022-08-02 20:14:36.339982 doc_printer-0.9.0/PKG-INFO
+-rw-r--r--   0 wen        (502) staff       (20)      325 2022-07-21 21:01:42.000000 doc_printer-0.9.0/README.md
+drwxr-xr-x   0 wen        (502) staff       (20)        0 2022-08-02 20:14:36.318309 doc_printer-0.9.0/doc_printer/
+-rw-r--r--   0 wen        (502) staff       (20)     1390 2022-08-02 20:12:35.000000 doc_printer-0.9.0/doc_printer/__init__.py
+-rw-r--r--   0 wen        (502) staff       (20)      598 2022-08-01 16:39:30.000000 doc_printer-0.9.0/doc_printer/abc.py
+-rw-r--r--   0 wen        (502) staff       (20)    17177 2022-08-02 20:12:38.000000 doc_printer-0.9.0/doc_printer/doc.py
+-rw-r--r--   0 wen        (502) staff       (20)        0 2022-07-21 20:02:47.000000 doc_printer-0.9.0/doc_printer/py.typed
+-rw-r--r--   0 wen        (502) staff       (20)     4751 2022-08-01 18:00:31.000000 doc_printer-0.9.0/doc_printer/simple.py
+-rw-r--r--   0 wen        (502) staff       (20)     1531 2022-08-01 17:59:06.000000 doc_printer-0.9.0/doc_printer/smart.py
+-rw-r--r--   0 wen        (502) staff       (20)     4382 2022-08-01 17:56:32.000000 doc_printer-0.9.0/doc_printer/table.py
+drwxr-xr-x   0 wen        (502) staff       (20)        0 2022-08-02 20:14:36.324671 doc_printer-0.9.0/doc_printer.egg-info/
+-rw-r--r--   0 wen        (502) staff       (20)      869 2022-08-02 20:14:36.000000 doc_printer-0.9.0/doc_printer.egg-info/PKG-INFO
+-rw-r--r--   0 wen        (502) staff       (20)      402 2022-08-02 20:14:36.000000 doc_printer-0.9.0/doc_printer.egg-info/SOURCES.txt
+-rw-r--r--   0 wen        (502) staff       (20)        1 2022-08-02 20:14:36.000000 doc_printer-0.9.0/doc_printer.egg-info/dependency_links.txt
+-rw-r--r--   0 wen        (502) staff       (20)      115 2022-08-02 20:14:36.000000 doc_printer-0.9.0/doc_printer.egg-info/requires.txt
+-rw-r--r--   0 wen        (502) staff       (20)       12 2022-08-02 20:14:36.000000 doc_printer-0.9.0/doc_printer.egg-info/top_level.txt
+-rw-r--r--   0 wen        (502) staff       (20)     1287 2022-08-02 20:13:26.000000 doc_printer-0.9.0/pyproject.toml
+-rw-r--r--   0 wen        (502) staff       (20)       38 2022-08-02 20:14:36.344433 doc_printer-0.9.0/setup.cfg
+drwxr-xr-x   0 wen        (502) staff       (20)        0 2022-08-02 20:14:36.327917 doc_printer-0.9.0/test/
+-rw-r--r--   0 wen        (502) staff       (20)     2020 2022-08-01 15:58:50.000000 doc_printer-0.9.0/test/test_doc.py
+-rw-r--r--   0 wen        (502) staff       (20)     1479 2022-08-01 15:58:50.000000 doc_printer-0.9.0/test/test_simple.py
```

### Comparing `doc_printer-0.8.4/LICENSE` & `doc_printer-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `doc_printer-0.8.4/PKG-INFO` & `doc_printer-0.9.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: doc_printer
-Version: 0.8.4
+Version: 0.9.0
 Summary: A Wadler-Leijen Pretty Printer in Python
 Author: Wen Kokke
 Project-URL: documentation, https://wenkokke.github.io/py-doc-printer/
 Project-URL: repository, https://github.com/wenkokke/py-doc-printer
 Keywords: doc-printer
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Compilers
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: sphinx
+Provides-Extra: publish
 License-File: LICENSE
 
 # Document Printer
 
 ![GitHub Workflow Status](https://img.shields.io/github/workflow/status/wenkokke/py-doc-printer/CI) ![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/wenkokke/py-doc-printer)
 
 A Wadler-Leijen Pretty Printer in Python.
```

### Comparing `doc_printer-0.8.4/doc_printer/__init__.py` & `doc_printer-0.9.0/doc_printer/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,16 +19,18 @@
 from .doc import Token as Token
 from .doc import TokenStream as TokenStream
 from .doc import alt as alt
 from .doc import angles as angles
 from .doc import braces as braces
 from .doc import brackets as brackets
 from .doc import cat as cat
+from .doc import create_table as create_table
 from .doc import create_tables as create_tables
 from .doc import double_quote as double_quote
+from .doc import group as group
 from .doc import nest as nest
 from .doc import parens as parens
 from .doc import row as row
 from .doc import single_quote as single_quote
 from .doc import table as table
 from .simple import SimpleDocRenderer as SimpleDocRenderer
 from .simple import SimpleLayout as SimpleLayout
```

### Comparing `doc_printer-0.8.4/doc_printer/abc.py` & `doc_printer-0.9.0/doc_printer/abc.py`

 * *Files identical despite different names*

### Comparing `doc_printer-0.8.4/doc_printer/doc.py` & `doc_printer-0.9.0/doc_printer/doc.py`

 * *Files 3% similar despite different names*

```diff
@@ -443,14 +443,27 @@
     doc = cat(doclike)
     if auto_quote:
         doc = Map(escape_double, doc)
     return cat('"', doc, '"')
 
 
 ################################################################################
+# Group: Removing Lines
+################################################################################
+
+
+def group(doc: Doc) -> Doc:
+    def inline(token: Token) -> TokenStream:
+        if not token is Line:
+            yield token
+
+    return Map(function=inline, doc=doc)
+
+
+################################################################################
 # Alignment: Rows and Tables
 ################################################################################
 
 
 @dataclasses.dataclass
 class RowInfo:
     table_type: typing.Optional[str]
@@ -552,28 +565,38 @@
         return False
 
     def __iter__(self) -> collections.abc.Iterator[typing.Union[Doc, Row, None]]:
         yield self.doc
         yield self.row
 
 
-def create_table(*doclike: DocLike) -> Doc:
+def create_table(*doclike: DocLike) -> typing.Optional[Table]:
     buffer: list[Row] = []
-    for doc in splat(doclike):
-        if isinstance(doc, Row):
-            buffer.append(doc)
+    previous_doc_was_row: bool = False
+    row_candidates = map(RowCandidate, splat(doclike))
+    for row_candidate in row_candidates:
+        if row_candidate.row:
+            buffer.append(row_candidate.row)
+            previous_doc_was_row = True
+        elif row_candidate.doc is Line and previous_doc_was_row:
+            previous_doc_was_row = False
         else:
-            return Fail
+            return None
+    # NOTE: only return tables with >=2 rows
     if len(buffer) < 2:
-        return Fail
+        return None
     else:
         return Table(tuple(iter(buffer)))
 
 
 def create_tables(
     docs: collections.abc.Iterator[Doc], *, separator: Text = Line
 ) -> collections.abc.Iterator[Doc]:
     row_candidates = map(RowCandidate, docs)
     table_candidates = itertools.groupby(row_candidates, key=lambda rc: rc.table_type)
     for _, group in table_candidates:
         subdocs, subrows = zip(*group)
-        yield alt(separator.join(subdocs), create_table(subrows))
+        table = create_table(subrows)
+        if table:
+            yield alt(separator.join(subdocs), table)
+        else:
+            yield from subdocs
```

### Comparing `doc_printer-0.8.4/doc_printer/simple.py` & `doc_printer-0.9.0/doc_printer/simple.py`

 * *Files identical despite different names*

### Comparing `doc_printer-0.8.4/doc_printer/smart.py` & `doc_printer-0.9.0/doc_printer/smart.py`

 * *Files identical despite different names*

### Comparing `doc_printer-0.8.4/doc_printer/table.py` & `doc_printer-0.9.0/doc_printer/table.py`

 * *Files identical despite different names*

### Comparing `doc_printer-0.8.4/doc_printer.egg-info/PKG-INFO` & `doc_printer-0.9.0/doc_printer.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: doc-printer
-Version: 0.8.4
+Version: 0.9.0
 Summary: A Wadler-Leijen Pretty Printer in Python
 Author: Wen Kokke
 Project-URL: documentation, https://wenkokke.github.io/py-doc-printer/
 Project-URL: repository, https://github.com/wenkokke/py-doc-printer
 Keywords: doc-printer
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Compilers
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: sphinx
+Provides-Extra: publish
 License-File: LICENSE
 
 # Document Printer
 
 ![GitHub Workflow Status](https://img.shields.io/github/workflow/status/wenkokke/py-doc-printer/CI) ![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/wenkokke/py-doc-printer)
 
 A Wadler-Leijen Pretty Printer in Python.
```

### Comparing `doc_printer-0.8.4/pyproject.toml` & `doc_printer-0.9.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "doc_printer"
-version = "0.8.4"
+version = "0.9.0"
 description = "A Wadler-Leijen Pretty Printer in Python"
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ["doc-printer"]
 authors = [{ name = "Wen Kokke" }]
 classifiers = [
   "License :: OSI Approved :: MIT License",
@@ -21,14 +21,15 @@
     "pytest"
 ]
 sphinx = [
     "sphinx",
     "sphinx-toolbox >=3.1.2",
     "sphinx_bootstrap_theme",
 ]
+publish = ["build", "twine"]
 
 [project.urls]
 documentation = "https://wenkokke.github.io/py-doc-printer/"
 repository = "https://github.com/wenkokke/py-doc-printer"
 
 [tool.setuptools.package-data]
 doc_printer = ["py.typed"]
@@ -37,15 +38,15 @@
 testpaths = "test"
 
 [tool.pytest.ini_options]
 enable_assertion_pass_hook = true
 filterwarnings = ["ignore::DeprecationWarning:.*:"]
 
 [tool.bumpver]
-current_version = "0.8.4"
+current_version = "0.9.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `doc_printer-0.8.4/test/test_doc.py` & `doc_printer-0.9.0/test/test_doc.py`

 * *Files identical despite different names*

### Comparing `doc_printer-0.8.4/test/test_simple.py` & `doc_printer-0.9.0/test/test_simple.py`

 * *Files identical despite different names*

