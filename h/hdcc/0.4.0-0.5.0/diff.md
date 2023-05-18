# Comparing `tmp/hdcc-0.4.0.tar.gz` & `tmp/hdcc-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdcc-0.4.0.tar", max compression
+gzip compressed data, was "hdcc-0.5.0.tar", max compression
```

## Comparing `hdcc-0.4.0.tar` & `hdcc-0.5.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       90 2023-05-18 07:58:44.444416 hdcc-0.4.0/README.md
--rw-r--r--   0        0        0    19737 2023-05-18 10:41:09.677964 hdcc-0.4.0/hdcc/HDProg.py
--rw-r--r--   0        0        0    16280 2023-05-18 09:07:27.261645 hdcc-0.4.0/hdcc/HDTypes.py
--rw-r--r--   0        0        0        0 2023-05-18 07:58:44.444416 hdcc-0.4.0/hdcc/__init__.py
--rw-r--r--   0        0        0      330 2023-05-18 10:41:18.518125 hdcc-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 hdcc-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0       90 2023-05-18 07:58:44.444416 hdcc-0.5.0/README.md
+-rw-r--r--   0        0        0    19739 2023-05-18 10:47:53.905314 hdcc-0.5.0/hdcc/HDProg.py
+-rw-r--r--   0        0        0    16280 2023-05-18 09:07:27.261645 hdcc-0.5.0/hdcc/HDTypes.py
+-rw-r--r--   0        0        0        0 2023-05-18 07:58:44.444416 hdcc-0.5.0/hdcc/__init__.py
+-rw-r--r--   0        0        0      330 2023-05-18 10:48:03.642158 hdcc-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 hdcc-0.5.0/PKG-INFO
```

### Comparing `hdcc-0.4.0/hdcc/HDProg.py` & `hdcc-0.5.0/hdcc/HDProg.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,15 +288,15 @@
     def run(self, state: HDProgState, args: dict):
         while state.pc < len(self.statements):
             self.step(state, args)
         return state, *(state.val_table[out][3] for out in self.outputs)
         
 
     def step(self, state: HDProgState, args: dict):
-        print("PC: " + str(state.pc) + " " + str(self.statements[state.pc]))
+        # print("PC: " + str(state.pc) + " " + str(self.statements[state.pc]))
         if state.pc == 0:
             # plug in arguments/inputs
             for k in self.inputs.keys():
                 if not k in args:
                     raise Exception("Missing input: " + k)
                 if not issubclass(type(args[k]), self.inputs[k][0]):
                     raise Exception("Invalid input type for " + k + ": expected " + str(self.inputs[k][0]) + " but got " + str(type(args[k])))
```

### Comparing `hdcc-0.4.0/hdcc/HDTypes.py` & `hdcc-0.5.0/hdcc/HDTypes.py`

 * *Files identical despite different names*

### Comparing `hdcc-0.4.0/PKG-INFO` & `hdcc-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdcc
-Version: 0.4.0
+Version: 0.5.0
 Summary: 
 Author: Yifan Yang
 Author-email: yyang29@stanford.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

