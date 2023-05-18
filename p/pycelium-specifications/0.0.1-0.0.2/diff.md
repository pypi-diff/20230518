# Comparing `tmp/pycelium_specifications-0.0.1.tar.gz` & `tmp/pycelium_specifications-0.0.2.tar.gz`

## Comparing `pycelium_specifications-0.0.1.tar` & `pycelium_specifications-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.1/specifications/__init__.py
--rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.1/specifications/common.py
--rw-r--r--   0        0        0    15103 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.1/specifications/merkletree.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.1/.gitignore
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.1/license
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.1/readme.md
--rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.2/specifications/__init__.py
+-rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.2/specifications/common.py
+-rw-r--r--   0        0        0    15120 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.2/specifications/merkletree.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.2/license
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.2/readme.md
+-rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 pycelium_specifications-0.0.2/PKG-INFO
```

### Comparing `pycelium_specifications-0.0.1/specifications/common.py` & `pycelium_specifications-0.0.2/specifications/common.py`

 * *Files 15% similar despite different names*

```diff
@@ -66,17 +66,22 @@
     def __enter__(self) -> None:
         pass
 
     def __exit__(self, __exc_type, __exc_value, __traceback) -> bool | None:
         if __exc_value is not None:
             if __exc_type is ImplementationNote:
                 note(__exc_value)
+                print('N', end='', sep='', flush=True)
                 return True
-            else:
-                error(False, f'{self.label}: {__exc_value}')
+
+            print('F', end='', sep='', flush=True)
+            error(False, f'{self.label}: {__exc_value}')
+            return True
+
+        print('.', end='', sep='', flush=True)
 
 
 class RaisesError:
     label: str
     exception: None | BaseException
 
     def __init__(self, label: str) -> None:
```

### Comparing `pycelium_specifications-0.0.1/specifications/merkletree.py` & `pycelium_specifications-0.0.2/specifications/merkletree.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,14 +114,16 @@
             check_implementation(key, value)
         except BaseException as e:
             if e.__traceback__:
                 error(False, f'{e}: {traceback.format_exc()}')
             else:
                 error(False, f'{e}')
 
+    print('')
+
     for err in get_errors():
         print(f'error: {err}')
 
     for nt in get_notes():
         print(f'note: {nt}')
```

### Comparing `pycelium_specifications-0.0.1/license` & `pycelium_specifications-0.0.2/license`

 * *Files identical despite different names*

### Comparing `pycelium_specifications-0.0.1/pyproject.toml` & `pycelium_specifications-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pycelium-specifications"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="k98kurz", email="k98kurz@gmail.com" },
 ]
 description = "Library of common interfaces for the Pycelium project."
 readme = "readme.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pycelium_specifications-0.0.1/readme.md` & `pycelium_specifications-0.0.2/readme.md`

 * *Files identical despite different names*

### Comparing `pycelium_specifications-0.0.1/PKG-INFO` & `pycelium_specifications-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycelium-specifications
-Version: 0.0.1
+Version: 0.0.2
 Summary: Library of common interfaces for the Pycelium project.
 Project-URL: Homepage, https://github.com/k98kurz/pycelium-specifications
 Project-URL: Bug Tracker, https://github.com/k98kurz/pycelium-specifications/issues
 Author-email: k98kurz <k98kurz@gmail.com>
 License-File: license
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
```

