# Comparing `tmp/hdcc-0.3.0.tar.gz` & `tmp/hdcc-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdcc-0.3.0.tar", max compression
+gzip compressed data, was "hdcc-0.4.0.tar", max compression
```

## Comparing `hdcc-0.3.0.tar` & `hdcc-0.4.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       90 2023-05-18 07:58:44.444416 hdcc-0.3.0/README.md
--rw-r--r--   0        0        0    19719 2023-05-18 10:30:56.973416 hdcc-0.3.0/hdcc/HDProg.py
--rw-r--r--   0        0        0    16280 2023-05-18 09:07:27.261645 hdcc-0.3.0/hdcc/HDTypes.py
--rw-r--r--   0        0        0        0 2023-05-18 07:58:44.444416 hdcc-0.3.0/hdcc/__init__.py
--rw-r--r--   0        0        0      330 2023-05-18 10:31:07.046935 hdcc-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 hdcc-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       90 2023-05-18 07:58:44.444416 hdcc-0.4.0/README.md
+-rw-r--r--   0        0        0    19737 2023-05-18 10:41:09.677964 hdcc-0.4.0/hdcc/HDProg.py
+-rw-r--r--   0        0        0    16280 2023-05-18 09:07:27.261645 hdcc-0.4.0/hdcc/HDTypes.py
+-rw-r--r--   0        0        0        0 2023-05-18 07:58:44.444416 hdcc-0.4.0/hdcc/__init__.py
+-rw-r--r--   0        0        0      330 2023-05-18 10:41:18.518125 hdcc-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 hdcc-0.4.0/PKG-INFO
```

### Comparing `hdcc-0.3.0/hdcc/HDProg.py` & `hdcc-0.4.0/hdcc/HDProg.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,16 @@
         self.statements.append((StatementType.DECL_VAR, type, identifier, dim))
         self.add_symbol(HDSymbolType.VAR, identifier, (type, dim, None))
 
     def decl_const(self, type: type, identifier, value):
         self.statements.append((StatementType.DECL_CONST, type, identifier, value))
         if isinstance(value, Types.HyperVector):
             self.add_symbol(HDSymbolType.CONST, identifier, (type, value.dim, value))
-        self.add_symbol(HDSymbolType.CONST, identifier, (type, None, value))
+        else:
+            self.add_symbol(HDSymbolType.CONST, identifier, (type, None, value))
 
     def assign(self, lhs: str, rhs: Union[Expression, str, int, float, Types.HyperVector]):
         rhs_type = type(rhs)
         if rhs_type == Expression:
             rhs_type = rhs.outType
         elif rhs_type == str:
             if rhs not in self.symbols:
```

### Comparing `hdcc-0.3.0/hdcc/HDTypes.py` & `hdcc-0.4.0/hdcc/HDTypes.py`

 * *Files identical despite different names*

### Comparing `hdcc-0.3.0/PKG-INFO` & `hdcc-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdcc
-Version: 0.3.0
+Version: 0.4.0
 Summary: 
 Author: Yifan Yang
 Author-email: yyang29@stanford.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

