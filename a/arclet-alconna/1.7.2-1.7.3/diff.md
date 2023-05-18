# Comparing `tmp/arclet-alconna-1.7.2.tar.gz` & `tmp/arclet-alconna-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet-alconna-1.7.2.tar", last modified: Fri May 12 11:27:45 2023, max compression
+gzip compressed data, was "arclet-alconna-1.7.3.tar", last modified: Thu May 18 15:42:13 2023, max compression
```

## Comparing `arclet-alconna-1.7.2.tar` & `arclet-alconna-1.7.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 arclet-alconna-1.7.2/LICENSE
--rw-r--r--   0        0        0     2810 2023-05-11 05:55:21.918053 arclet-alconna-1.7.2/pyproject.toml
--rw-r--r--   0        0        0     6702 2023-05-11 05:55:23.383958 arclet-alconna-1.7.2/README-EN.md
--rw-r--r--   0        0        0     1084 2023-05-12 11:13:09.377302 arclet-alconna-1.7.2/src/arclet/alconna/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 05:53:44.746150 arclet-alconna-1.7.2/src/arclet/alconna/_internal/__init__.py
--rw-r--r--   0        0        0    17787 2023-05-12 08:33:12.924712 arclet-alconna-1.7.2/src/arclet/alconna/_internal/_analyser.py
--rw-r--r--   0        0        0     8476 2023-05-11 05:53:44.748144 arclet-alconna-1.7.2/src/arclet/alconna/_internal/_argv.py
--rw-r--r--   0        0        0    23045 2023-05-11 05:53:44.748144 arclet-alconna-1.7.2/src/arclet/alconna/_internal/_handlers.py
--rw-r--r--   0        0        0     7811 2023-05-11 05:53:44.749146 arclet-alconna-1.7.2/src/arclet/alconna/_internal/_header.py
--rw-r--r--   0        0        0      837 2023-05-11 05:53:44.749146 arclet-alconna-1.7.2/src/arclet/alconna/_internal/_util.py
--rw-r--r--   0        0        0     1543 2023-05-11 05:54:34.441719 arclet-alconna-1.7.2/src/arclet/alconna/action.py
--rw-r--r--   0        0        0    14429 2023-05-11 05:55:00.317381 arclet-alconna-1.7.2/src/arclet/alconna/args.py
--rw-r--r--   0        0        0     1499 2023-05-11 05:53:44.752371 arclet-alconna-1.7.2/src/arclet/alconna/argv.py
--rw-r--r--   0        0        0    15660 2023-05-11 05:55:01.638197 arclet-alconna-1.7.2/src/arclet/alconna/arparma.py
--rw-r--r--   0        0        0    13248 2023-05-11 05:55:02.886909 arclet-alconna-1.7.2/src/arclet/alconna/base.py
--rw-r--r--   0        0        0     1889 2023-05-11 05:55:04.954858 arclet-alconna-1.7.2/src/arclet/alconna/builtin.py
--rw-r--r--   0        0        0     4867 2023-05-11 05:53:44.757144 arclet-alconna-1.7.2/src/arclet/alconna/completion.py
--rw-r--r--   0        0        0     4465 2023-05-11 05:55:07.597153 arclet-alconna-1.7.2/src/arclet/alconna/config.py
--rw-r--r--   0        0        0    14029 2023-05-12 11:11:57.973132 arclet-alconna-1.7.2/src/arclet/alconna/core.py
--rw-r--r--   0        0        0     2617 2023-05-11 05:55:14.716787 arclet-alconna-1.7.2/src/arclet/alconna/duplication.py
--rw-r--r--   0        0        0     1009 2023-05-11 05:55:16.833416 arclet-alconna-1.7.2/src/arclet/alconna/exceptions.py
--rw-r--r--   0        0        0    11287 2023-05-11 05:55:17.442184 arclet-alconna-1.7.2/src/arclet/alconna/formatter.py
--rw-r--r--   0        0        0       99 2023-05-11 05:53:44.763145 arclet-alconna-1.7.2/src/arclet/alconna/i18n/.config.json
--rw-r--r--   0        0        0     3565 2023-05-11 05:53:44.764143 arclet-alconna-1.7.2/src/arclet/alconna/i18n/en-US.json
--rw-r--r--   0        0        0     3602 2023-05-11 05:53:44.764143 arclet-alconna-1.7.2/src/arclet/alconna/i18n/zh-CN.json
--rw-r--r--   0        0        0    16956 2023-05-11 05:55:18.044404 arclet-alconna-1.7.2/src/arclet/alconna/manager.py
--rw-r--r--   0        0        0     1484 2023-05-11 05:55:18.667097 arclet-alconna-1.7.2/src/arclet/alconna/model.py
--rw-r--r--   0        0        0     1943 2023-05-11 05:55:19.651541 arclet-alconna-1.7.2/src/arclet/alconna/model.pyi
--rw-r--r--   0        0        0     3940 2023-05-11 05:55:20.308191 arclet-alconna-1.7.2/src/arclet/alconna/output.py
--rw-r--r--   0        0        0        0 2023-05-11 05:53:44.769149 arclet-alconna-1.7.2/src/arclet/alconna/py.typed
--rw-r--r--   0        0        0     5815 2023-05-11 05:55:25.933152 arclet-alconna-1.7.2/src/arclet/alconna/stub.py
--rw-r--r--   0        0        0     3586 2023-05-11 05:55:26.563876 arclet-alconna-1.7.2/src/arclet/alconna/typing.py
--rw-r--r--   0        0        0     3246 2023-05-11 05:53:44.772143 arclet-alconna-1.7.2/tests/analyser_test.py
--rw-r--r--   0        0        0     7583 2023-05-11 05:53:44.773143 arclet-alconna-1.7.2/tests/args_test.py
--rw-r--r--   0        0        0     2167 2023-05-11 05:55:03.459296 arclet-alconna-1.7.2/tests/base_test.py
--rw-r--r--   0        0        0     3113 2023-05-11 05:53:44.774144 arclet-alconna-1.7.2/tests/components_test.py
--rw-r--r--   0        0        0     1199 2023-05-11 05:53:44.774144 arclet-alconna-1.7.2/tests/config_test.py
--rw-r--r--   0        0        0    23493 2023-05-12 08:33:12.926710 arclet-alconna-1.7.2/tests/core_test.py
--rw-r--r--   0        0        0      505 2023-05-11 05:53:44.775105 arclet-alconna-1.7.2/tests/util_test.py
--rw-r--r--   0        0        0     7363 1970-01-01 00:00:00.000000 arclet-alconna-1.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 arclet-alconna-1.7.3/LICENSE
+-rw-r--r--   0        0        0     2810 2023-05-11 05:55:21.918053 arclet-alconna-1.7.3/pyproject.toml
+-rw-r--r--   0        0        0     6702 2023-05-11 05:55:23.383958 arclet-alconna-1.7.3/README-EN.md
+-rw-r--r--   0        0        0     1084 2023-05-18 15:41:15.142189 arclet-alconna-1.7.3/src/arclet/alconna/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 05:53:44.746150 arclet-alconna-1.7.3/src/arclet/alconna/_internal/__init__.py
+-rw-r--r--   0        0        0    17993 2023-05-18 15:37:17.306466 arclet-alconna-1.7.3/src/arclet/alconna/_internal/_analyser.py
+-rw-r--r--   0        0        0     8476 2023-05-11 05:53:44.748144 arclet-alconna-1.7.3/src/arclet/alconna/_internal/_argv.py
+-rw-r--r--   0        0        0    23045 2023-05-11 05:53:44.748144 arclet-alconna-1.7.3/src/arclet/alconna/_internal/_handlers.py
+-rw-r--r--   0        0        0     7811 2023-05-11 05:53:44.749146 arclet-alconna-1.7.3/src/arclet/alconna/_internal/_header.py
+-rw-r--r--   0        0        0      837 2023-05-11 05:53:44.749146 arclet-alconna-1.7.3/src/arclet/alconna/_internal/_util.py
+-rw-r--r--   0        0        0     1543 2023-05-11 05:54:34.441719 arclet-alconna-1.7.3/src/arclet/alconna/action.py
+-rw-r--r--   0        0        0    14429 2023-05-11 05:55:00.317381 arclet-alconna-1.7.3/src/arclet/alconna/args.py
+-rw-r--r--   0        0        0     1499 2023-05-11 05:53:44.752371 arclet-alconna-1.7.3/src/arclet/alconna/argv.py
+-rw-r--r--   0        0        0    15660 2023-05-11 05:55:01.638197 arclet-alconna-1.7.3/src/arclet/alconna/arparma.py
+-rw-r--r--   0        0        0    13248 2023-05-11 05:55:02.886909 arclet-alconna-1.7.3/src/arclet/alconna/base.py
+-rw-r--r--   0        0        0     1889 2023-05-11 05:55:04.954858 arclet-alconna-1.7.3/src/arclet/alconna/builtin.py
+-rw-r--r--   0        0        0     4867 2023-05-11 05:53:44.757144 arclet-alconna-1.7.3/src/arclet/alconna/completion.py
+-rw-r--r--   0        0        0     4465 2023-05-11 05:55:07.597153 arclet-alconna-1.7.3/src/arclet/alconna/config.py
+-rw-r--r--   0        0        0    14029 2023-05-12 11:11:57.973132 arclet-alconna-1.7.3/src/arclet/alconna/core.py
+-rw-r--r--   0        0        0     2617 2023-05-11 05:55:14.716787 arclet-alconna-1.7.3/src/arclet/alconna/duplication.py
+-rw-r--r--   0        0        0     1009 2023-05-11 05:55:16.833416 arclet-alconna-1.7.3/src/arclet/alconna/exceptions.py
+-rw-r--r--   0        0        0    11287 2023-05-11 05:55:17.442184 arclet-alconna-1.7.3/src/arclet/alconna/formatter.py
+-rw-r--r--   0        0        0       99 2023-05-11 05:53:44.763145 arclet-alconna-1.7.3/src/arclet/alconna/i18n/.config.json
+-rw-r--r--   0        0        0     3565 2023-05-11 05:53:44.764143 arclet-alconna-1.7.3/src/arclet/alconna/i18n/en-US.json
+-rw-r--r--   0        0        0     3602 2023-05-11 05:53:44.764143 arclet-alconna-1.7.3/src/arclet/alconna/i18n/zh-CN.json
+-rw-r--r--   0        0        0    16956 2023-05-11 05:55:18.044404 arclet-alconna-1.7.3/src/arclet/alconna/manager.py
+-rw-r--r--   0        0        0     1484 2023-05-11 05:55:18.667097 arclet-alconna-1.7.3/src/arclet/alconna/model.py
+-rw-r--r--   0        0        0     1943 2023-05-11 05:55:19.651541 arclet-alconna-1.7.3/src/arclet/alconna/model.pyi
+-rw-r--r--   0        0        0     3940 2023-05-11 05:55:20.308191 arclet-alconna-1.7.3/src/arclet/alconna/output.py
+-rw-r--r--   0        0        0        0 2023-05-11 05:53:44.769149 arclet-alconna-1.7.3/src/arclet/alconna/py.typed
+-rw-r--r--   0        0        0     5815 2023-05-11 05:55:25.933152 arclet-alconna-1.7.3/src/arclet/alconna/stub.py
+-rw-r--r--   0        0        0     3586 2023-05-11 05:55:26.563876 arclet-alconna-1.7.3/src/arclet/alconna/typing.py
+-rw-r--r--   0        0        0     3246 2023-05-11 05:53:44.772143 arclet-alconna-1.7.3/tests/analyser_test.py
+-rw-r--r--   0        0        0     7583 2023-05-11 05:53:44.773143 arclet-alconna-1.7.3/tests/args_test.py
+-rw-r--r--   0        0        0     2167 2023-05-11 05:55:03.459296 arclet-alconna-1.7.3/tests/base_test.py
+-rw-r--r--   0        0        0     3113 2023-05-11 05:53:44.774144 arclet-alconna-1.7.3/tests/components_test.py
+-rw-r--r--   0        0        0     1199 2023-05-11 05:53:44.774144 arclet-alconna-1.7.3/tests/config_test.py
+-rw-r--r--   0        0        0    23555 2023-05-18 15:40:31.384319 arclet-alconna-1.7.3/tests/core_test.py
+-rw-r--r--   0        0        0      505 2023-05-11 05:53:44.775105 arclet-alconna-1.7.3/tests/util_test.py
+-rw-r--r--   0        0        0     7363 1970-01-01 00:00:00.000000 arclet-alconna-1.7.3/PKG-INFO
```

### Comparing `arclet-alconna-1.7.2/LICENSE` & `arclet-alconna-1.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.2/pyproject.toml` & `arclet-alconna-1.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
 ]
-version = "1.7.2"
+version = "1.7.3"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 documentation = "https://arcletproject.github.io/docs/alconna/tutorial"
 repository = "https://github.com/ArcletProject/Alconna"
```

### Comparing `arclet-alconna-1.7.2/README-EN.md` & `arclet-alconna-1.7.3/README-EN.md`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.2/src/arclet/alconna/__init__.py` & `arclet-alconna-1.7.3/src/arclet/alconna/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,12 +17,12 @@
 from .builtin import set_default
 from .model import OptionResult, SubcommandResult, HeadResult
 from .output import output_manager
 from .formatter import TextFormatter
 from .duplication import Duplication
 from .stub import ArgsStub, OptionStub, SubcommandStub
 
-__version__ = "1.7.2"
+__version__ = "1.7.3"
 
 # backward compatibility
 Arpamar = Arparma
 DataCollectionContainer = Argv
```

### Comparing `arclet-alconna-1.7.2/src/arclet/alconna/_internal/_analyser.py` & `arclet-alconna-1.7.3/src/arclet/alconna/_internal/_analyser.py`

 * *Files 1% similar despite different names*

```diff
@@ -346,16 +346,21 @@
         ):
             return res
         try:
             self.header_result = analyse_header(self.command_header, argv)
         except ParamsUnmatched as e:
             argv.raw_data = argv.bak_data.copy()
             argv.current_index = 0
+            _next = argv.next(move=False)[0]
+            if _next.__class__ is not str:
+                if self.command.meta.raise_exception:
+                    raise e
+                return self.export(argv, True, e)
             try:
-                _res = command_manager.find_shortcut(self.command, argv.next(move=False)[0])
+                _res = command_manager.find_shortcut(self.command, _next)
             except ValueError as exc:
                 if self.command.meta.raise_exception:
                     raise e from exc
                 return self.export(argv, True, e)
             else:
                 argv.next()
                 data = argv.release()
```

### Comparing `arclet-alconna-1.7.2/src/arclet/alconna/_internal/_argv.py` & `arclet-alconna-1.7.3/src/arclet/alconna/_internal/_argv.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.2/src/arclet/alconna/_internal/_handlers.py` & `arclet-alconna-1.7.3/src/arclet/alconna/_internal/_handlers.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.2/src/arclet/alconna/_internal/_header.py` & `arclet-alconna-1.7.3/src/arclet/alconna/_internal/_header.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.2/src/arclet/alconna/_internal/_util.py` & `arclet-alconna-1.7.3/src/arclet/alconna/_internal/_util.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.2/src/arclet/alconna/action.py` & `arclet-alconna-1.7.3/src/arclet/alconna/action.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.2/src/arclet/alconna/args.py` & `arclet-alconna-1.7.3/src/arclet/alconna/args.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.2/src/arclet/alconna/argv.py` & `arclet-alconna-1.7.3/src/arclet/alconna/argv.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.2/src/arclet/alconna/arparma.py` & `arclet-alconna-1.7.3/src/arclet/alconna/arparma.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.2/src/arclet/alconna/base.py` & `arclet-alconna-1.7.3/src/arclet/alconna/base.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.2/src/arclet/alconna/builtin.py` & `arclet-alconna-1.7.3/src/arclet/alconna/builtin.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.2/src/arclet/alconna/completion.py` & `arclet-alconna-1.7.3/src/arclet/alconna/completion.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.2/src/arclet/alconna/config.py` & `arclet-alconna-1.7.3/src/arclet/alconna/config.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.2/src/arclet/alconna/core.py` & `arclet-alconna-1.7.3/src/arclet/alconna/core.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.2/src/arclet/alconna/duplication.py` & `arclet-alconna-1.7.3/src/arclet/alconna/duplication.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.2/src/arclet/alconna/exceptions.py` & `arclet-alconna-1.7.3/src/arclet/alconna/exceptions.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.2/src/arclet/alconna/formatter.py` & `arclet-alconna-1.7.3/src/arclet/alconna/formatter.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.2/src/arclet/alconna/i18n/en-US.json` & `arclet-alconna-1.7.3/src/arclet/alconna/i18n/en-US.json`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.2/src/arclet/alconna/i18n/zh-CN.json` & `arclet-alconna-1.7.3/src/arclet/alconna/i18n/zh-CN.json`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.2/src/arclet/alconna/manager.py` & `arclet-alconna-1.7.3/src/arclet/alconna/manager.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.2/src/arclet/alconna/model.py` & `arclet-alconna-1.7.3/src/arclet/alconna/model.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.2/src/arclet/alconna/model.pyi` & `arclet-alconna-1.7.3/src/arclet/alconna/model.pyi`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.2/src/arclet/alconna/output.py` & `arclet-alconna-1.7.3/src/arclet/alconna/output.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.2/src/arclet/alconna/stub.py` & `arclet-alconna-1.7.3/src/arclet/alconna/stub.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.2/src/arclet/alconna/typing.py` & `arclet-alconna-1.7.3/src/arclet/alconna/typing.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.2/tests/analyser_test.py` & `arclet-alconna-1.7.3/tests/analyser_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.2/tests/args_test.py` & `arclet-alconna-1.7.3/tests/args_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.2/tests/base_test.py` & `arclet-alconna-1.7.3/tests/base_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.2/tests/components_test.py` & `arclet-alconna-1.7.3/tests/components_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.2/tests/config_test.py` & `arclet-alconna-1.7.3/tests/config_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.2/tests/core_test.py` & `arclet-alconna-1.7.3/tests/core_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -405,14 +405,16 @@
     alc16_1.shortcut("echo", {"command": "exec print({%0})"})
     alc16_1.shortcut("echo1", {"command": "exec print(\\'{*\n}\\')"})
     res5 = alc16_1.parse("echo 123")
     assert res5.content == "print(123)"
     assert not alc16_1.parse("echo 123 456").matched
     res6 = alc16_1.parse(["echo1", "123", "456 789"])
     assert res6.content == "print('123\n456\n789')"
+    res7 = alc16_1.parse([123])
+    assert not res7.matched
 
 
 def test_help():
     from arclet.alconna.exceptions import SpecialOptionTriggered
 
     alc17 = Alconna("core17") + Option("foo", Args["bar", str])
     res = alc17.parse("core17 --help")
```

### Comparing `arclet-alconna-1.7.2/PKG-INFO` & `arclet-alconna-1.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arclet-alconna
-Version: 1.7.2
+Version: 1.7.3
 Summary: A High-performance, Generality, Humane Command Line Arguments Parser Library.
 License: MIT
 Keywords: command,argparse,fast,alconna,cli,command-line,parsing,optparse
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

