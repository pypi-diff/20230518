# Comparing `tmp/amazon-braket-build-tools-0.2.0.post0.tar.gz` & `tmp/amazon-braket-build-tools-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon-braket-build-tools-0.2.0.post0.tar", last modified: Thu Mar 16 16:04:29 2023, max compression
+gzip compressed data, was "amazon-braket-build-tools-0.2.1.tar", last modified: Thu May 18 16:04:56 2023, max compression
```

## Comparing `amazon-braket-build-tools-0.2.0.post0.tar` & `amazon-braket-build-tools-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:04:29.723428 amazon-braket-build-tools-0.2.0.post0/
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-03-16 16:04:20.000000 amazon-braket-build-tools-0.2.0.post0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-16 16:04:20.000000 amazon-braket-build-tools-0.2.0.post0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-03-16 16:04:29.723428 amazon-braket-build-tools-0.2.0.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-03-16 16:04:20.000000 amazon-braket-build-tools-0.2.0.post0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-16 16:04:20.000000 amazon-braket-build-tools-0.2.0.post0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-03-16 16:04:29.723428 amazon-braket-build-tools-0.2.0.post0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-03-16 16:04:20.000000 amazon-braket-build-tools-0.2.0.post0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:04:29.723428 amazon-braket-build-tools-0.2.0.post0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:04:29.723428 amazon-braket-build-tools-0.2.0.post0/src/amazon_braket_build_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-03-16 16:04:29.000000 amazon-braket-build-tools-0.2.0.post0/src/amazon_braket_build_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-03-16 16:04:29.000000 amazon-braket-build-tools-0.2.0.post0/src/amazon_braket_build_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 16:04:29.000000 amazon-braket-build-tools-0.2.0.post0/src/amazon_braket_build_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-16 16:04:29.000000 amazon-braket-build-tools-0.2.0.post0/src/amazon_braket_build_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-16 16:04:29.000000 amazon-braket-build-tools-0.2.0.post0/src/amazon_braket_build_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-16 16:04:29.000000 amazon-braket-build-tools-0.2.0.post0/src/amazon_braket_build_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:04:29.723428 amazon-braket-build-tools-0.2.0.post0/src/braket/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:04:29.723428 amazon-braket-build-tools-0.2.0.post0/src/braket/_build_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-03-16 16:04:20.000000 amazon-braket-build-tools-0.2.0.post0/src/braket/_build_tools/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:04:29.723428 amazon-braket-build-tools-0.2.0.post0/src/braket/flake8_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)    18354 2023-03-16 16:04:20.000000 amazon-braket-build-tools-0.2.0.post0/src/braket/flake8_plugins/braket_checkstyle_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:04:56.415351 amazon-braket-build-tools-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-05-18 16:04:42.000000 amazon-braket-build-tools-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-18 16:04:42.000000 amazon-braket-build-tools-0.2.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-18 16:04:56.415351 amazon-braket-build-tools-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-18 16:04:42.000000 amazon-braket-build-tools-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-18 16:04:42.000000 amazon-braket-build-tools-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-18 16:04:56.415351 amazon-braket-build-tools-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-18 16:04:42.000000 amazon-braket-build-tools-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:04:56.415351 amazon-braket-build-tools-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:04:56.415351 amazon-braket-build-tools-0.2.1/src/amazon_braket_build_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-18 16:04:56.000000 amazon-braket-build-tools-0.2.1/src/amazon_braket_build_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-18 16:04:56.000000 amazon-braket-build-tools-0.2.1/src/amazon_braket_build_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 16:04:56.000000 amazon-braket-build-tools-0.2.1/src/amazon_braket_build_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-18 16:04:56.000000 amazon-braket-build-tools-0.2.1/src/amazon_braket_build_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-18 16:04:56.000000 amazon-braket-build-tools-0.2.1/src/amazon_braket_build_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-18 16:04:56.000000 amazon-braket-build-tools-0.2.1/src/amazon_braket_build_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:04:56.415351 amazon-braket-build-tools-0.2.1/src/braket/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:04:56.415351 amazon-braket-build-tools-0.2.1/src/braket/_build_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-18 16:04:42.000000 amazon-braket-build-tools-0.2.1/src/braket/_build_tools/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:04:56.415351 amazon-braket-build-tools-0.2.1/src/braket/flake8_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)    18537 2023-05-18 16:04:42.000000 amazon-braket-build-tools-0.2.1/src/braket/flake8_plugins/braket_checkstyle_plugin.py
```

### Comparing `amazon-braket-build-tools-0.2.0.post0/LICENSE` & `amazon-braket-build-tools-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `amazon-braket-build-tools-0.2.0.post0/PKG-INFO` & `amazon-braket-build-tools-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-braket-build-tools
-Version: 0.2.0.post0
+Version: 0.2.1
 Summary: A set of build tools for Amazon Braket
 Home-page: https://github.com/aws/amazon-braket-build-tools
 Author: Amazon Web Services
 License: Apache License 2.0
 Keywords: Amazon AWS Quantum
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `amazon-braket-build-tools-0.2.0.post0/README.md` & `amazon-braket-build-tools-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `amazon-braket-build-tools-0.2.0.post0/setup.cfg` & `amazon-braket-build-tools-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `amazon-braket-build-tools-0.2.0.post0/setup.py` & `amazon-braket-build-tools-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-build-tools-0.2.0.post0/src/amazon_braket_build_tools.egg-info/PKG-INFO` & `amazon-braket-build-tools-0.2.1/src/amazon_braket_build_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-braket-build-tools
-Version: 0.2.0.post0
+Version: 0.2.1
 Summary: A set of build tools for Amazon Braket
 Home-page: https://github.com/aws/amazon-braket-build-tools
 Author: Amazon Web Services
 License: Apache License 2.0
 Keywords: Amazon AWS Quantum
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `amazon-braket-build-tools-0.2.0.post0/src/braket/_build_tools/_version.py` & `amazon-braket-build-tools-0.2.1/src/braket/_build_tools/_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # language governing permissions and limitations under the License.
 
 """Version information.
 
 Version number (major.minor.patch[-label])
 """
 
-__version__ = "0.2.0.post0"
+__version__ = "0.2.1"
```

### Comparing `amazon-braket-build-tools-0.2.0.post0/src/braket/flake8_plugins/braket_checkstyle_plugin.py` & `amazon-braket-build-tools-0.2.1/src/braket/flake8_plugins/braket_checkstyle_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 class _Visitor(ast.NodeVisitor):
     ARGS_REGEX = re.compile(r"^(\s*)Args\s*:\s*$")
     RETURN_REGEX = re.compile(r"^(\s*)(Returns|Yields)\s*:\s*$")
     MISC_REGEX = re.compile(
         r"^(\s*)(Throws|Raises|See Also|Note|Example|Examples|Warnings)\s*:\s*$"
     )
-    ARG_INFO_REGEX = re.compile(r"^(\s*)(\*{0,2}\w*)\s*(\([^:]*\))?\s*:\s*(.*)")
+    ARG_INFO_REGEX = re.compile(r"^(\s*)(`?\*{0,2}\w*`?)\s*(\([^:]*\))?\s*:\s*(.*)")
     RETURN_INFO_REGEX = re.compile(r"^(\s*)([^:]*)\s*(:)?\s*(.*)")
     INDENT_REGEX = re.compile(r"^(\s*)\S+.*")
     RESERVED_ARGS = {"self", "cls"}
 
     MESSAGES = {
         "BCS001": "Argument '%s' is missing a type hint.",
         "BCS002": "Function '%s' is missing a type hint for the return value.",
@@ -183,15 +183,18 @@
             context.current_section = DocSection.RETURN_REST
         elif context.current_section == DocSection.RETURN_REST:
             self._check_indent(context.return_indent, doc_line, context)
 
     def _check_argument_info(
         self, regex_matches: re.Match, context: DocContext, node: ast.FunctionDef
     ) -> None:
-        arg_indent, arg_name, arg_type, arg_description = regex_matches.groups()
+        arg_indent = regex_matches.group(1)
+        arg_name = regex_matches.group(2).strip("`") if regex_matches.group(2) else None
+        arg_type = regex_matches.group(3) if regex_matches.group(3) else None
+        arg_description = regex_matches.group(4)
         arg_index = _get_argument_with_name(arg_name, node)
         self._check_argument_indent(arg_indent, arg_name, arg_index, context, node)
         if arg_index is None:
             return
         self._check_argument_docs(arg_name, arg_type, arg_description, arg_index, context, node)
         context.current_arg = arg_index + 1
```

