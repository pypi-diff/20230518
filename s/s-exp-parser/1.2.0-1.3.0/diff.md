# Comparing `tmp/s-exp-parser-1.2.0.tar.gz` & `tmp/s-exp-parser-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/s-exp-parser-1.2.0.tar", last modified: Tue Aug  4 02:10:42 2020, max compression
+gzip compressed data, was "s-exp-parser-1.3.0.tar", last modified: Thu May 18 17:44:41 2023, max compression
```

## Comparing `s-exp-parser-1.2.0.tar` & `s-exp-parser-1.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2020-08-04 02:10:42.000000 s-exp-parser-1.2.0/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      724 2020-08-04 02:10:42.000000 s-exp-parser-1.2.0/PKG-INFO
--rw-r--r--   0 kavi      (1000) kavi      (1000)      123 2020-06-04 07:33:22.000000 s-exp-parser-1.2.0/README.md
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2020-08-04 02:10:42.000000 s-exp-parser-1.2.0/s_exp_parser.egg-info/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      724 2020-08-04 02:10:41.000000 s-exp-parser-1.2.0/s_exp_parser.egg-info/PKG-INFO
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      446 2020-08-04 02:10:41.000000 s-exp-parser-1.2.0/s_exp_parser.egg-info/SOURCES.txt
--rw-rw-r--   0 kavi      (1000) kavi      (1000)        1 2020-08-04 02:10:41.000000 s-exp-parser-1.2.0/s_exp_parser.egg-info/dependency_links.txt
--rw-rw-r--   0 kavi      (1000) kavi      (1000)       14 2020-08-04 02:10:41.000000 s-exp-parser-1.2.0/s_exp_parser.egg-info/requires.txt
--rw-rw-r--   0 kavi      (1000) kavi      (1000)       26 2020-08-04 02:10:41.000000 s-exp-parser-1.2.0/s_exp_parser.egg-info/top_level.txt
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2020-08-04 02:10:42.000000 s-exp-parser-1.2.0/s_expression_parser/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      159 2020-08-04 02:09:32.000000 s-exp-parser-1.2.0/s_expression_parser/__init__.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      379 2020-08-04 02:09:32.000000 s-exp-parser-1.2.0/s_expression_parser/configs.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     2050 2020-08-04 02:09:56.000000 s-exp-parser-1.2.0/s_expression_parser/lexer.py
--rw-r--r--   0 kavi      (1000) kavi      (1000)     2546 2020-06-05 08:25:15.000000 s-exp-parser-1.2.0/s_expression_parser/parser.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     1682 2020-08-04 02:09:32.000000 s-exp-parser-1.2.0/s_expression_parser/renderer.py
--rw-r--r--   0 kavi      (1000) kavi      (1000)       79 2020-08-04 02:10:42.000000 s-exp-parser-1.2.0/setup.cfg
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      797 2020-08-04 02:10:30.000000 s-exp-parser-1.2.0/setup.py
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2020-08-04 02:10:42.000000 s-exp-parser-1.2.0/tests/
--rw-r--r--   0 kavi      (1000) kavi      (1000)        0 2020-06-04 07:28:03.000000 s-exp-parser-1.2.0/tests/__init__.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     1836 2020-08-04 02:09:32.000000 s-exp-parser-1.2.0/tests/lexer_tests.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     2321 2020-08-04 02:09:32.000000 s-exp-parser-1.2.0/tests/parser_tests.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     2586 2020-08-04 02:09:32.000000 s-exp-parser-1.2.0/tests/renderer_tests.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-05-18 17:44:41.057483 s-exp-parser-1.3.0/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      724 2023-05-18 17:44:41.057483 s-exp-parser-1.3.0/PKG-INFO
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      123 2023-03-16 02:52:18.000000 s-exp-parser-1.3.0/README.md
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-05-18 17:44:41.057483 s-exp-parser-1.3.0/s_exp_parser.egg-info/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      724 2023-05-18 17:44:40.000000 s-exp-parser-1.3.0/s_exp_parser.egg-info/PKG-INFO
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      446 2023-05-18 17:44:40.000000 s-exp-parser-1.3.0/s_exp_parser.egg-info/SOURCES.txt
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)        1 2023-05-18 17:44:40.000000 s-exp-parser-1.3.0/s_exp_parser.egg-info/dependency_links.txt
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)       14 2023-05-18 17:44:40.000000 s-exp-parser-1.3.0/s_exp_parser.egg-info/requires.txt
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)       26 2023-05-18 17:44:40.000000 s-exp-parser-1.3.0/s_exp_parser.egg-info/top_level.txt
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-05-18 17:44:41.057483 s-exp-parser-1.3.0/s_expression_parser/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      159 2023-03-16 02:52:18.000000 s-exp-parser-1.3.0/s_expression_parser/__init__.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      379 2023-03-16 02:52:18.000000 s-exp-parser-1.3.0/s_expression_parser/configs.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2050 2023-03-16 02:52:18.000000 s-exp-parser-1.3.0/s_expression_parser/lexer.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2546 2023-03-16 02:52:18.000000 s-exp-parser-1.3.0/s_expression_parser/parser.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     1754 2023-05-18 17:40:57.000000 s-exp-parser-1.3.0/s_expression_parser/renderer.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)       79 2023-05-18 17:44:41.061483 s-exp-parser-1.3.0/setup.cfg
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      797 2023-05-18 17:44:28.000000 s-exp-parser-1.3.0/setup.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-05-18 17:44:41.057483 s-exp-parser-1.3.0/tests/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)        0 2023-03-16 02:52:18.000000 s-exp-parser-1.3.0/tests/__init__.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     1836 2023-03-16 02:52:18.000000 s-exp-parser-1.3.0/tests/lexer_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2321 2023-03-16 02:52:18.000000 s-exp-parser-1.3.0/tests/parser_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     3288 2023-05-18 17:44:14.000000 s-exp-parser-1.3.0/tests/renderer_tests.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `s-exp-parser-1.2.0/PKG-INFO` & `s-exp-parser-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s-exp-parser
-Version: 1.2.0
+Version: 1.3.0
 Summary: S expression parser for python.
 Home-page: https://github.com/kavigupta/s-exp-parser
 Author: Kavi Gupta
 Author-email: s_exp_parser@kavigupta.org
 License: UNKNOWN
 Description: 
         # S expression parser
```

### Comparing `s-exp-parser-1.2.0/s_exp_parser.egg-info/PKG-INFO` & `s-exp-parser-1.3.0/s_exp_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s-exp-parser
-Version: 1.2.0
+Version: 1.3.0
 Summary: S expression parser for python.
 Home-page: https://github.com/kavigupta/s-exp-parser
 Author: Kavi Gupta
 Author-email: s_exp_parser@kavigupta.org
 License: UNKNOWN
 Description: 
         # S expression parser
```

### Comparing `s-exp-parser-1.2.0/s_expression_parser/lexer.py` & `s-exp-parser-1.3.0/s_expression_parser/lexer.py`

 * *Files identical despite different names*

### Comparing `s-exp-parser-1.2.0/s_expression_parser/parser.py` & `s-exp-parser-1.3.0/s_expression_parser/parser.py`

 * *Files identical despite different names*

### Comparing `s-exp-parser-1.2.0/s_expression_parser/renderer.py` & `s-exp-parser-1.3.0/s_expression_parser/renderer.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 from .parser import Pair, nil
 
 
 @attr.s
 class Renderer:
     indent = attr.ib(default=2)
     columns = attr.ib(default=120)
+    nil_as_word = attr.ib(default=False)
 
     def render_multiple(self, parsed):
         return "".join(self.render(x) for x in parsed)
 
     def render(self, parsed):
         return self._render(self._to_list(parsed))
 
     def _render(self, parsed, indent=0):
         if isinstance(parsed, str):
             return self._indent(parsed, indent)
 
         if not parsed:
-            return self._indent("()", indent)
+            return self._indent("nil" if self.nil_as_word else "()", indent)
 
         single_line = self._indent(self._render_one_line(parsed), indent)
         if len(single_line) <= self.columns:
             return single_line
 
         assert isinstance(parsed, list)
         parsed = parsed[:]
```

### Comparing `s-exp-parser-1.2.0/setup.py` & `s-exp-parser-1.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="s-exp-parser",
-    version="1.2.0",
+    version="1.3.0",
     author="Kavi Gupta",
     author_email="s_exp_parser@kavigupta.org",
     description="S expression parser for python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kavigupta/s-exp-parser",
     packages=setuptools.find_packages(),
```

### Comparing `s-exp-parser-1.2.0/tests/lexer_tests.py` & `s-exp-parser-1.3.0/tests/lexer_tests.py`

 * *Files identical despite different names*

### Comparing `s-exp-parser-1.2.0/tests/parser_tests.py` & `s-exp-parser-1.3.0/tests/parser_tests.py`

 * *Files identical despite different names*

### Comparing `s-exp-parser-1.2.0/tests/renderer_tests.py` & `s-exp-parser-1.3.0/tests/renderer_tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,7 +101,37 @@
                     1
                     (* x (factorial (- x 1)))
                   )
                 )
                 """
             ),
         )
+
+    def test_nil_as_word(self):
+        self.assertEqual(
+            Renderer(nil_as_word=True).render(nil),
+            process(
+                """
+                nil
+                """
+            ),
+        )
+
+        self.assertEqual(
+            Renderer(nil_as_word=True, columns=10).render_multiple(
+                parse("(1 2 3 4 5 6 (7) (8) ())", ParserConfig({"'", "quote"}, True))
+            ),
+            process(
+                """
+                (1
+                  2
+                  3
+                  4
+                  5
+                  6
+                  (7)
+                  (8)
+                  nil
+                )
+                """
+            ),
+        )
```

