# Comparing `tmp/retrack-0.4.1.tar.gz` & `tmp/retrack-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retrack-0.4.1.tar", max compression
+gzip compressed data, was "retrack-0.5.0.tar", max compression
```

## Comparing `retrack-0.4.1.tar` & `retrack-0.5.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1072 2023-05-02 17:30:19.838518 retrack-0.4.1/LICENSE
--rw-r--r--   0        0        0     4914 2023-05-02 17:30:19.838518 retrack-0.4.1/README.md
--rw-r--r--   0        0        0     1518 2023-05-02 17:30:19.838518 retrack-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      366 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/engine/__init__.py
--rw-r--r--   0        0        0     6675 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/engine/parser.py
--rw-r--r--   0        0        0     2907 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/engine/request_manager.py
--rw-r--r--   0        0        0     6463 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/engine/runner.py
--rw-r--r--   0        0        0     1322 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/nodes/__init__.py
--rw-r--r--   0        0        0     1800 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/nodes/base.py
--rw-r--r--   0        0        0     2574 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/nodes/check.py
--rw-r--r--   0        0        0     2234 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/nodes/constants.py
--rw-r--r--   0        0        0      873 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/nodes/contains.py
--rw-r--r--   0        0        0      910 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/nodes/endswith.py
--rw-r--r--   0        0        0      941 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/nodes/endswithany.py
--rw-r--r--   0        0        0     1009 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/nodes/inputs.py
--rw-r--r--   0        0        0     1606 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/nodes/logic.py
--rw-r--r--   0        0        0     1056 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/nodes/match.py
--rw-r--r--   0        0        0     2116 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/nodes/math.py
--rw-r--r--   0        0        0     1085 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/nodes/outputs.py
--rw-r--r--   0        0        0      581 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/nodes/start.py
--rw-r--r--   0        0        0      926 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/nodes/startswith.py
--rw-r--r--   0        0        0      957 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/nodes/startswithany.py
--rw-r--r--   0        0        0        0 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/utils/__init__.py
--rw-r--r--   0        0        0      197 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/utils/constants.py
--rw-r--r--   0        0        0     1324 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/utils/registry.py
--rw-r--r--   0        0        0      154 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/utils/transformers.py
--rw-r--r--   0        0        0      594 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/validators/__init__.py
--rw-r--r--   0        0        0      267 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/validators/base.py
--rw-r--r--   0        0        0      407 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/validators/check_is_dag.py
--rw-r--r--   0        0        0     1296 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/validators/node_exists.py
--rw-r--r--   0        0        0     5846 2023-05-02 17:30:29.127900 retrack-0.4.1/setup.py
--rw-r--r--   0        0        0     5630 2023-05-02 17:30:29.128374 retrack-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-18 17:13:18.083398 retrack-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4914 2023-05-18 17:13:18.083398 retrack-0.5.0/README.md
+-rw-r--r--   0        0        0     1580 2023-05-18 17:13:18.083398 retrack-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      366 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/engine/__init__.py
+-rw-r--r--   0        0        0     6675 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/engine/parser.py
+-rw-r--r--   0        0        0     2907 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/engine/request_manager.py
+-rw-r--r--   0        0        0     6463 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/engine/runner.py
+-rw-r--r--   0        0        0     1462 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/nodes/__init__.py
+-rw-r--r--   0        0        0     1800 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/nodes/base.py
+-rw-r--r--   0        0        0     2574 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/nodes/check.py
+-rw-r--r--   0        0        0     2234 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/nodes/constants.py
+-rw-r--r--   0        0        0      873 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/nodes/contains.py
+-rw-r--r--   0        0        0      951 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/nodes/datetime.py
+-rw-r--r--   0        0        0      910 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/nodes/endswith.py
+-rw-r--r--   0        0        0      941 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/nodes/endswithany.py
+-rw-r--r--   0        0        0     1009 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/nodes/inputs.py
+-rw-r--r--   0        0        0     1606 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/nodes/logic.py
+-rw-r--r--   0        0        0     1056 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/nodes/match.py
+-rw-r--r--   0        0        0     2623 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/nodes/math.py
+-rw-r--r--   0        0        0     1085 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/nodes/outputs.py
+-rw-r--r--   0        0        0      581 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/nodes/start.py
+-rw-r--r--   0        0        0      926 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/nodes/startswith.py
+-rw-r--r--   0        0        0      957 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/nodes/startswithany.py
+-rw-r--r--   0        0        0        0 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/utils/__init__.py
+-rw-r--r--   0        0        0      197 2023-05-18 17:13:18.083398 retrack-0.5.0/retrack/utils/constants.py
+-rw-r--r--   0        0        0     1324 2023-05-18 17:13:18.087399 retrack-0.5.0/retrack/utils/registry.py
+-rw-r--r--   0        0        0      154 2023-05-18 17:13:18.087399 retrack-0.5.0/retrack/utils/transformers.py
+-rw-r--r--   0        0        0      594 2023-05-18 17:13:18.087399 retrack-0.5.0/retrack/validators/__init__.py
+-rw-r--r--   0        0        0      267 2023-05-18 17:13:18.087399 retrack-0.5.0/retrack/validators/base.py
+-rw-r--r--   0        0        0      407 2023-05-18 17:13:18.087399 retrack-0.5.0/retrack/validators/check_is_dag.py
+-rw-r--r--   0        0        0     1296 2023-05-18 17:13:18.087399 retrack-0.5.0/retrack/validators/node_exists.py
+-rw-r--r--   0        0        0     5681 1970-01-01 00:00:00.000000 retrack-0.5.0/PKG-INFO
```

### Comparing `retrack-0.4.1/LICENSE` & `retrack-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `retrack-0.4.1/README.md` & `retrack-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `retrack-0.4.1/pyproject.toml` & `retrack-0.5.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "retrack"
-version = "0.4.1"
+version = "0.5.0"
 description = "A business rules engine"
 authors = ["Gabriel Guarisa <gabrielguarisa@gmail.com>", "Nathalia Trotte <nathaliatrotte@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/gabrielguarisa/retrack"
 homepage = "https://github.com/gabrielguarisa/retrack"
 keywords = ["rules", "models", "business", "node", "graph"]
@@ -17,17 +17,20 @@
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.4"
 pytest-cov = "^3.0.0"
 black = "^22.6.0"
 isort = {extras = ["colors"], version = "^5.12.0"}
 
+[tool.poetry.group.dev.dependencies]
+pytest-mock = "^3.10.0"
+
 [tool.black]
 # https://github.com/psf/black
-target-version = ["py37"]
+target-version = ["py39"]
 line-length = 88
 color = true
 
 exclude = '''
 /(
     \.git
     | \.hg
```

### Comparing `retrack-0.4.1/retrack/engine/parser.py` & `retrack-0.5.0/retrack/engine/parser.py`

 * *Files identical despite different names*

### Comparing `retrack-0.4.1/retrack/engine/request_manager.py` & `retrack-0.5.0/retrack/engine/request_manager.py`

 * *Files identical despite different names*

### Comparing `retrack-0.4.1/retrack/engine/runner.py` & `retrack-0.5.0/retrack/engine/runner.py`

 * *Files identical despite different names*

### Comparing `retrack-0.4.1/retrack/nodes/__init__.py` & `retrack-0.5.0/retrack/nodes/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from retrack.nodes.base import BaseNode
 from retrack.nodes.check import Check
 from retrack.nodes.constants import Bool, Constant, List
 from retrack.nodes.contains import Contains
+from retrack.nodes.datetime import CurrentYear
 from retrack.nodes.endswith import EndsWith
 from retrack.nodes.endswithany import EndsWithAny
 from retrack.nodes.inputs import Input
 from retrack.nodes.logic import And, Not, Or
 from retrack.nodes.match import If
-from retrack.nodes.math import Math
+from retrack.nodes.math import AbsoluteValue, Math
 from retrack.nodes.outputs import Output
 from retrack.nodes.start import Start
 from retrack.nodes.startswith import StartsWith
 from retrack.nodes.startswithany import StartsWithAny
 from retrack.utils.registry import Registry
 
 _registry = Registry()
@@ -33,14 +34,16 @@
 register("Output", Output)
 register("Check", Check)
 register("If", If)
 register("And", And)
 register("Or", Or)
 register("Not", Not)
 register("Math", Math)
+register("AbsoluteValue", AbsoluteValue)
 register("StartsWith", StartsWith)
 register("EndsWith", EndsWith)
 register("StartsWithAny", StartsWithAny)
 register("EndsWithAny", EndsWithAny)
 register("Contains", Contains)
+register("CurrentYear", CurrentYear)
 
 __all__ = ["registry", "register", "BaseNode"]
```

### Comparing `retrack-0.4.1/retrack/nodes/base.py` & `retrack-0.5.0/retrack/nodes/base.py`

 * *Files identical despite different names*

### Comparing `retrack-0.4.1/retrack/nodes/check.py` & `retrack-0.5.0/retrack/nodes/check.py`

 * *Files identical despite different names*

### Comparing `retrack-0.4.1/retrack/nodes/constants.py` & `retrack-0.5.0/retrack/nodes/constants.py`

 * *Files identical despite different names*

### Comparing `retrack-0.4.1/retrack/nodes/contains.py` & `retrack-0.5.0/retrack/nodes/contains.py`

 * *Files identical despite different names*

### Comparing `retrack-0.4.1/retrack/nodes/endswith.py` & `retrack-0.5.0/retrack/nodes/endswith.py`

 * *Files identical despite different names*

### Comparing `retrack-0.4.1/retrack/nodes/endswithany.py` & `retrack-0.5.0/retrack/nodes/endswithany.py`

 * *Files identical despite different names*

### Comparing `retrack-0.4.1/retrack/nodes/inputs.py` & `retrack-0.5.0/retrack/nodes/inputs.py`

 * *Files identical despite different names*

### Comparing `retrack-0.4.1/retrack/nodes/logic.py` & `retrack-0.5.0/retrack/nodes/logic.py`

 * *Files identical despite different names*

### Comparing `retrack-0.4.1/retrack/nodes/match.py` & `retrack-0.5.0/retrack/nodes/match.py`

 * *Files identical despite different names*

### Comparing `retrack-0.4.1/retrack/nodes/math.py` & `retrack-0.5.0/retrack/nodes/math.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,7 +70,27 @@
         elif self.data.operator == MathOperator.DIVISION:
             return {
                 "output_value": input_value_0.astype(float)
                 / input_value_1.astype(float)
             }
         else:
             raise ValueError("Unknown operator")
+
+
+###############################################################
+# Absolute Value Node
+###############################################################
+
+
+class AbsoluteValueInputsModel(pydantic.BaseModel):
+    input_value: InputConnectionModel
+
+
+class AbsoluteValue(BaseNode):
+    inputs: AbsoluteValueInputsModel
+    outputs: MathOutputsModel
+
+    def run(
+        self,
+        input_value: pd.Series,
+    ) -> typing.Dict[str, pd.Series]:
+        return {"output_value": input_value.astype(float).abs()}
```

### Comparing `retrack-0.4.1/retrack/nodes/outputs.py` & `retrack-0.5.0/retrack/nodes/outputs.py`

 * *Files identical despite different names*

### Comparing `retrack-0.4.1/retrack/nodes/start.py` & `retrack-0.5.0/retrack/nodes/start.py`

 * *Files identical despite different names*

### Comparing `retrack-0.4.1/retrack/nodes/startswith.py` & `retrack-0.5.0/retrack/nodes/startswith.py`

 * *Files identical despite different names*

### Comparing `retrack-0.4.1/retrack/nodes/startswithany.py` & `retrack-0.5.0/retrack/nodes/startswithany.py`

 * *Files identical despite different names*

### Comparing `retrack-0.4.1/retrack/utils/registry.py` & `retrack-0.5.0/retrack/utils/registry.py`

 * *Files identical despite different names*

### Comparing `retrack-0.4.1/retrack/validators/__init__.py` & `retrack-0.5.0/retrack/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `retrack-0.4.1/retrack/validators/node_exists.py` & `retrack-0.5.0/retrack/validators/node_exists.py`

 * *Files identical despite different names*

### Comparing `retrack-0.4.1/setup.py` & `retrack-0.5.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,366 +1,356 @@
-00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
-00000010: 662d 3820 2d2a 2d0a 6672 6f6d 2073 6574  f-8 -*-.from set
-00000020: 7570 746f 6f6c 7320 696d 706f 7274 2073  uptools import s
-00000030: 6574 7570 0a0a 7061 636b 6167 6573 203d  etup..packages =
-00000040: 205c 0a5b 2772 6574 7261 636b 272c 0a20   \.['retrack',. 
-00000050: 2772 6574 7261 636b 2e65 6e67 696e 6527  'retrack.engine'
-00000060: 2c0a 2027 7265 7472 6163 6b2e 6e6f 6465  ,. 'retrack.node
-00000070: 7327 2c0a 2027 7265 7472 6163 6b2e 7574  s',. 'retrack.ut
-00000080: 696c 7327 2c0a 2027 7265 7472 6163 6b2e  ils',. 'retrack.
-00000090: 7661 6c69 6461 746f 7273 275d 0a0a 7061  validators']..pa
-000000a0: 636b 6167 655f 6461 7461 203d 205c 0a7b  ckage_data = \.{
-000000b0: 2727 3a20 5b27 2a27 5d7d 0a0a 696e 7374  '': ['*']}..inst
-000000c0: 616c 6c5f 7265 7175 6972 6573 203d 205c  all_requires = \
-000000d0: 0a5b 276e 6574 776f 726b 783e 3d33 2e30  .['networkx>=3.0
-000000e0: 2c3c 342e 3027 2c20 2770 616e 6461 733e  ,<4.0', 'pandas>
-000000f0: 3d31 2e35 2e32 2c3c 322e 302e 3027 2c20  =1.5.2,<2.0.0', 
-00000100: 2770 7964 616e 7469 633e 3d31 2e31 302e  'pydantic>=1.10.
-00000110: 342c 3c32 2e30 2e30 275d 0a0a 7365 7475  4,<2.0.0']..setu
-00000120: 705f 6b77 6172 6773 203d 207b 0a20 2020  p_kwargs = {.   
-00000130: 2027 6e61 6d65 273a 2027 7265 7472 6163   'name': 'retrac
-00000140: 6b27 2c0a 2020 2020 2776 6572 7369 6f6e  k',.    'version
-00000150: 273a 2027 302e 342e 3127 2c0a 2020 2020  ': '0.4.1',.    
-00000160: 2764 6573 6372 6970 7469 6f6e 273a 2027  'description': '
-00000170: 4120 6275 7369 6e65 7373 2072 756c 6573  A business rules
-00000180: 2065 6e67 696e 6527 2c0a 2020 2020 276c   engine',.    'l
-00000190: 6f6e 675f 6465 7363 7269 7074 696f 6e27  ong_description'
-000001a0: 3a20 273c 7020 616c 6967 6e3d 2263 656e  : '<p align="cen
-000001b0: 7465 7222 3e5c 6e20 203c 6120 6872 6566  ter">\n  <a href
-000001c0: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
-000001d0: 2e63 6f6d 2f67 6162 7269 656c 6775 6172  .com/gabrielguar
-000001e0: 6973 612f 7265 7472 6163 6b22 3e3c 696d  isa/retrack"><im
-000001f0: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
-00000200: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00000210: 7465 6e74 2e63 6f6d 2f67 6162 7269 656c  tent.com/gabriel
-00000220: 6775 6172 6973 612f 7265 7472 6163 6b2f  guarisa/retrack/
-00000230: 6d61 696e 2f6c 6f67 6f2e 706e 6722 2061  main/logo.png" a
-00000240: 6c74 3d22 7265 7472 6163 6b22 3e3c 2f61  lt="retrack"></a
-00000250: 3e5c 6e3c 2f70 3e5c 6e3c 7020 616c 6967  >\n</p>\n<p alig
-00000260: 6e3d 2263 656e 7465 7222 3e5c 6e20 2020  n="center">\n   
-00000270: 203c 656d 3e41 2062 7573 696e 6573 7320   <em>A business 
-00000280: 7275 6c65 7320 656e 6769 6e65 3c2f 656d  rules engine</em
-00000290: 3e5c 6e3c 2f70 3e5c 6e5c 6e3c 6469 7620  >\n</p>\n\n<div 
-000002a0: 616c 6967 6e3d 2263 656e 7465 7222 3e5c  align="center">\
-000002b0: 6e5c 6e5b 215b 5061 636b 6167 6520 7665  n\n[![Package ve
-000002c0: 7273 696f 6e5d 2868 7474 7073 3a2f 2f69  rsion](https://i
-000002d0: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-000002e0: 7069 2f76 2f72 6574 7261 636b 3f63 6f6c  pi/v/retrack?col
-000002f0: 6f72 3d25 3233 3334 4430 3538 266c 6162  or=%2334D058&lab
-00000300: 656c 3d70 7970 6925 3230 7061 636b 6167  el=pypi%20packag
-00000310: 6529 5d28 6874 7470 733a 2f2f 7079 7069  e)](https://pypi
-00000320: 2e6f 7267 2f70 726f 6a65 6374 2f72 6574  .org/project/ret
-00000330: 7261 636b 2f29 5c6e 5b21 5b43 6f64 6520  rack/)\n[![Code 
-00000340: 7374 796c 653a 2062 6c61 636b 5d28 6874  style: black](ht
-00000350: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000360: 732e 696f 2f62 6164 6765 2f63 6f64 6525  s.io/badge/code%
-00000370: 3230 7374 796c 652d 626c 6163 6b2d 3030  20style-black-00
-00000380: 3030 3030 2e73 7667 295d 2868 7474 7073  0000.svg)](https
-00000390: 3a2f 2f67 6974 6875 622e 636f 6d2f 7073  ://github.com/ps
-000003a0: 662f 626c 6163 6b29 5c6e 5b21 5b53 656d  f/black)\n[![Sem
-000003b0: 616e 7469 6320 5665 7273 696f 6e73 5d28  antic Versions](
-000003c0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-000003d0: 6c64 732e 696f 2f62 6164 6765 2f25 3230  lds.io/badge/%20
-000003e0: 2532 3025 4630 2539 4625 3933 2541 3625  %20%F0%9F%93%A6%
-000003f0: 4630 2539 4625 3941 2538 302d 7365 6d61  F0%9F%9A%80-sema
-00000400: 6e74 6963 2d2d 7665 7273 696f 6e73 2d65  ntic--versions-e
-00000410: 3130 3037 392e 7376 6729 5d28 6874 7470  10079.svg)](http
-00000420: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f67  s://github.com/g
-00000430: 6162 7269 656c 6775 6172 6973 612f 7265  abrielguarisa/re
-00000440: 7472 6163 6b2f 7265 6c65 6173 6573 295c  track/releases)\
-00000450: 6e5b 215b 4c69 6365 6e73 655d 2868 7474  n[![License](htt
-00000460: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000470: 2e69 6f2f 6769 7468 7562 2f6c 6963 656e  .io/github/licen
-00000480: 7365 2f67 6162 7269 656c 6775 6172 6973  se/gabrielguaris
-00000490: 612f 7265 7472 6163 6b29 5d28 6874 7470  a/retrack)](http
-000004a0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f67  s://github.com/g
-000004b0: 6162 7269 656c 6775 6172 6973 612f 7265  abrielguarisa/re
-000004c0: 7472 6163 6b2f 626c 6f62 2f6d 6169 6e2f  track/blob/main/
-000004d0: 4c49 4345 4e53 4529 5c6e 5c6e 3c2f 6469  LICENSE)\n\n</di
-000004e0: 763e 5c6e 5c6e 5c6e 2323 2049 6e73 7461  v>\n\n\n## Insta
-000004f0: 6c6c 6174 696f 6e5c 6e5c 6e60 6060 6261  llation\n\n```ba
-00000500: 7368 5c6e 7069 7020 696e 7374 616c 6c20  sh\npip install 
-00000510: 7265 7472 6163 6b5c 6e60 6060 5c6e 5c6e  retrack\n```\n\n
-00000520: 2323 2055 7361 6765 5c6e 5c6e 6060 6070  ## Usage\n\n```p
-00000530: 7974 686f 6e5c 6e69 6d70 6f72 7420 7265  ython\nimport re
-00000540: 7472 6163 6b5c 6e5c 6e23 2050 6172 7365  track\n\n# Parse
-00000550: 2074 6865 2072 756c 652f 6d6f 6465 6c5c   the rule/model\
-00000560: 6e70 6172 7365 7220 3d20 7265 7472 6163  nparser = retrac
-00000570: 6b2e 5061 7273 6572 2872 756c 6529 5c6e  k.Parser(rule)\n
-00000580: 5c6e 2320 4372 6561 7465 2061 2072 756e  \n# Create a run
-00000590: 6e65 725c 6e72 756e 6e65 7220 3d20 7265  ner\nrunner = re
-000005a0: 7472 6163 6b2e 5275 6e6e 6572 2870 6172  track.Runner(par
-000005b0: 7365 7229 5c6e 5c6e 2320 5275 6e20 7468  ser)\n\n# Run th
-000005c0: 6520 7275 6c65 2f6d 6f64 656c 2070 6173  e rule/model pas
-000005d0: 7369 6e67 2074 6865 2064 6174 615c 6e72  sing the data\nr
-000005e0: 756e 6e65 722e 6578 6563 7574 6528 6461  unner.execute(da
-000005f0: 7461 295c 6e60 6060 5c6e 5c6e 5468 6520  ta)\n```\n\nThe 
-00000600: 6050 6172 7365 7260 2063 6c61 7373 2070  `Parser` class p
-00000610: 6172 7365 7320 7468 6520 7275 6c65 2f6d  arses the rule/m
-00000620: 6f64 656c 2061 6e64 2063 7265 6174 6573  odel and creates
-00000630: 2061 2067 7261 7068 206f 6620 6e6f 6465   a graph of node
-00000640: 732e 2054 6865 2060 5275 6e6e 6572 6020  s. The `Runner` 
-00000650: 636c 6173 7320 7275 6e73 2074 6865 2072  class runs the r
-00000660: 756c 652f 6d6f 6465 6c20 7573 696e 6720  ule/model using 
-00000670: 7468 6520 6461 7461 2070 6173 7365 6420  the data passed 
-00000680: 746f 2074 6865 2072 756e 6e65 722e 2054  to the runner. T
-00000690: 6865 2060 6461 7461 6020 6973 2061 2064  he `data` is a d
-000006a0: 6963 7469 6f6e 6172 7920 6f72 2061 206c  ictionary or a l
-000006b0: 6973 7420 6f66 2064 6963 7469 6f6e 6172  ist of dictionar
-000006c0: 6965 7320 636f 6e74 6169 6e69 6e67 2074  ies containing t
-000006d0: 6865 2064 6174 6120 7468 6174 2077 696c  he data that wil
-000006e0: 6c20 6265 2075 7365 6420 746f 2065 7661  l be used to eva
-000006f0: 6c75 6174 6520 7468 6520 636f 6e64 6974  luate the condit
-00000700: 696f 6e73 2061 6e64 2065 7865 6375 7465  ions and execute
-00000710: 2074 6865 2061 6374 696f 6e73 2e20 546f   the actions. To
-00000720: 2073 6565 2077 6963 6820 6461 7461 2069   see wich data i
-00000730: 7320 7265 7175 6972 6564 2066 6f72 2074  s required for t
-00000740: 6865 2067 6976 656e 2072 756c 652f 6d6f  he given rule/mo
-00000750: 6465 6c2c 2063 6865 636b 2074 6865 2060  del, check the `
-00000760: 7275 6e6e 6572 2e72 6571 7565 7374 5f6d  runner.request_m
-00000770: 6f64 656c 6020 7072 6f70 6572 7479 2074  odel` property t
-00000780: 6861 7420 6973 2061 2070 7964 616e 7469  hat is a pydanti
-00000790: 6320 6d6f 6465 6c20 7573 6564 2074 6f20  c model used to 
-000007a0: 7661 6c69 6461 7465 2074 6865 2064 6174  validate the dat
-000007b0: 612e 5c6e 5c6e 2323 2320 4372 6561 7469  a.\n\n### Creati
-000007c0: 6e67 2061 2072 756c 652f 6d6f 6465 6c5c  ng a rule/model\
-000007d0: 6e5c 6e41 2072 756c 6520 6973 2061 2073  n\nA rule is a s
-000007e0: 6574 206f 6620 636f 6e64 6974 696f 6e73  et of conditions
-000007f0: 2061 6e64 2061 6374 696f 6e73 2074 6861   and actions tha
-00000800: 7420 6172 6520 6578 6563 7574 6564 2077  t are executed w
-00000810: 6865 6e20 7468 6520 636f 6e64 6974 696f  hen the conditio
-00000820: 6e73 2061 7265 206d 6574 2e20 5468 6520  ns are met. The 
-00000830: 636f 6e64 6974 696f 6e73 2061 7265 2065  conditions are e
-00000840: 7661 6c75 6174 6564 2075 7369 6e67 2074  valuated using t
-00000850: 6865 2064 6174 6120 7061 7373 6564 2074  he data passed t
-00000860: 6f20 7468 6520 7275 6e6e 6572 2e20 5468  o the runner. Th
-00000870: 6520 6163 7469 6f6e 7320 6172 6520 6578  e actions are ex
-00000880: 6563 7574 6564 2077 6865 6e20 7468 6520  ecuted when the 
-00000890: 636f 6e64 6974 696f 6e73 2061 7265 206d  conditions are m
-000008a0: 6574 2e5c 6e5c 6e45 6163 6820 7275 6c65  et.\n\nEach rule
-000008b0: 2069 7320 636f 6d70 6f73 6564 206f 6620   is composed of 
-000008c0: 6d61 6e79 206e 6f64 6573 2e20 546f 2073  many nodes. To s
-000008d0: 6565 2065 6163 6820 6e6f 6465 2074 7970  ee each node typ
-000008e0: 652c 2063 6865 636b 2074 6865 205b 6e6f  e, check the [no
-000008f0: 6465 735d 2868 7474 7073 3a2f 2f67 6974  des](https://git
-00000900: 6875 622e 636f 6d2f 6761 6272 6965 6c67  hub.com/gabrielg
-00000910: 7561 7269 7361 2f72 6574 7261 636b 2f74  uarisa/retrack/t
-00000920: 7265 652f 6d61 696e 2f72 6574 7261 636b  ree/main/retrack
-00000930: 2f6e 6f64 6573 2920 666f 6c64 6572 2e5c  /nodes) folder.\
-00000940: 6e5c 6e54 6f20 6372 6561 7465 2061 2072  n\nTo create a r
-00000950: 756c 652c 2079 6f75 206e 6565 6420 746f  ule, you need to
-00000960: 2063 7265 6174 6520 6120 4a53 4f4e 2066   create a JSON f
-00000970: 696c 6520 7769 7468 2074 6865 2066 6f6c  ile with the fol
-00000980: 6c6f 7769 6e67 2073 7472 7563 7475 7265  lowing structure
-00000990: 3a5c 6e5c 6e60 6060 6a73 6f6e 5c6e 7b5c  :\n\n```json\n{\
-000009a0: 6e20 2022 6e6f 6465 7322 3a20 7b5c 6e5c  n  "nodes": {\n\
-000009b0: 745c 7422 6e6f 6465 2069 6422 3a20 7b5c  t\t"node id": {\
-000009c0: 6e5c 745c 745c 7422 6964 223a 2022 6e6f  n\t\t\t"id": "no
-000009d0: 6465 2069 6422 2c5c 6e5c 745c 745c 7422  de id",\n\t\t\t"
-000009e0: 6461 7461 223a 207b 7d2c 5c6e 5c74 5c74  data": {},\n\t\t
-000009f0: 5c74 2269 6e70 7574 7322 3a20 7b7d 2c5c  \t"inputs": {},\
-00000a00: 6e5c 745c 745c 7422 6f75 7470 7574 7322  n\t\t\t"outputs"
-00000a10: 3a20 7b7d 2c5c 6e5c 745c 745c 7422 6e61  : {},\n\t\t\t"na
-00000a20: 6d65 223a 2022 6e6f 6465 206e 616d 6522  me": "node name"
-00000a30: 2c5c 6e5c 745c 747d 2c5c 6e20 2020 202f  ,\n\t\t},\n    /
-00000a40: 2f20 2e2e 2e20 6d6f 7265 206e 6f64 6573  / ... more nodes
-00000a50: 5c6e 2020 7d5c 6e7d 5c6e 6060 605c 6e5c  \n  }\n}\n```\n\
-00000a60: 6e54 6865 2060 6e6f 6465 7360 206b 6579  nThe `nodes` key
-00000a70: 2069 7320 6120 6469 6374 696f 6e61 7279   is a dictionary
-00000a80: 206f 6620 6e6f 6465 732e 2045 6163 6820   of nodes. Each 
-00000a90: 6e6f 6465 2068 6173 2074 6865 2066 6f6c  node has the fol
-00000aa0: 6c6f 7769 6e67 2070 726f 7065 7274 6965  lowing propertie
-00000ab0: 733a 5c6e 5c6e 2d20 6069 6460 3a20 5468  s:\n\n- `id`: Th
-00000ac0: 6520 6e6f 6465 2069 642e 2054 6869 7320  e node id. This 
-00000ad0: 6973 2075 7365 6420 746f 2072 6566 6572  is used to refer
-00000ae0: 656e 6365 2074 6865 206e 6f64 6520 696e  ence the node in
-00000af0: 2074 6865 2060 696e 7075 7473 6020 616e   the `inputs` an
-00000b00: 6420 606f 7574 7075 7473 6020 7072 6f70  d `outputs` prop
-00000b10: 6572 7469 6573 2e5c 6e2d 2060 6461 7461  erties.\n- `data
-00000b20: 603a 2054 6865 206e 6f64 6520 6461 7461  `: The node data
-00000b30: 2e20 5468 6973 2069 7320 7573 6564 2061  . This is used a
-00000b40: 7320 6120 6d65 7461 6461 7461 2066 6f72  s a metadata for
-00000b50: 2074 6865 206e 6f64 652e 5c6e 2d20 6069   the node.\n- `i
-00000b60: 6e70 7574 7360 3a20 5468 6520 6e6f 6465  nputs`: The node
-00000b70: 2069 6e70 7574 732e 2054 6869 7320 6973   inputs. This is
-00000b80: 2075 7365 6420 746f 2072 6566 6572 656e   used to referen
-00000b90: 6365 2074 6865 206e 6f64 6520 696e 7075  ce the node inpu
-00000ba0: 7473 2e5c 6e2d 2060 6f75 7470 7574 7360  ts.\n- `outputs`
-00000bb0: 3a20 5468 6520 6e6f 6465 206f 7574 7075  : The node outpu
-00000bc0: 7473 2e20 5468 6973 2069 7320 7573 6564  ts. This is used
-00000bd0: 2074 6f20 7265 6665 7265 6e63 6520 7468   to reference th
-00000be0: 6520 6e6f 6465 206f 7574 7075 7473 2e5c  e node outputs.\
-00000bf0: 6e2d 2060 6e61 6d65 603a 2054 6865 206e  n- `name`: The n
-00000c00: 6f64 6520 6e61 6d65 2e20 5468 6973 2069  ode name. This i
-00000c10: 7320 7573 6564 2074 6f20 6465 6669 6e65  s used to define
-00000c20: 2074 6865 206e 6f64 6520 7479 7065 2e5c   the node type.\
-00000c30: 6e5c 6e54 6865 2060 696e 7075 7473 6020  n\nThe `inputs` 
-00000c40: 616e 6420 606f 7574 7075 7473 6020 7072  and `outputs` pr
-00000c50: 6f70 6572 7469 6573 2061 7265 2064 6963  operties are dic
-00000c60: 7469 6f6e 6172 6965 7320 6f66 206e 6f64  tionaries of nod
-00000c70: 6520 636f 6e6e 6563 7469 6f6e 732e 2045  e connections. E
-00000c80: 6163 6820 636f 6e6e 6563 7469 6f6e 2068  ach connection h
-00000c90: 6173 2074 6865 2066 6f6c 6c6f 7769 6e67  as the following
-00000ca0: 2070 726f 7065 7274 6965 733a 5c6e 5c6e   properties:\n\n
-00000cb0: 2d20 606e 6f64 6560 3a20 5468 6520 6e6f  - `node`: The no
-00000cc0: 6465 2069 6420 7468 6174 2069 7320 636f  de id that is co
-00000cd0: 6e6e 6563 7465 6420 746f 2074 6865 2063  nnected to the c
-00000ce0: 7572 7265 6e74 206e 6f64 652e 5c6e 2d20  urrent node.\n- 
-00000cf0: 6069 6e70 7574 603a 2054 6865 2069 6e70  `input`: The inp
-00000d00: 7574 206e 616d 6520 6f66 2074 6865 2063  ut name of the c
-00000d10: 6f6e 6e65 6374 696f 6e20 7468 6174 2069  onnection that i
-00000d20: 7320 636f 6e6e 6563 7465 6420 746f 2074  s connected to t
-00000d30: 6865 2063 7572 7265 6e74 206e 6f64 652e  he current node.
-00000d40: 2054 6869 7320 6973 206f 6e6c 7920 7573   This is only us
-00000d50: 6564 2069 6e20 7468 6520 6069 6e70 7574  ed in the `input
-00000d60: 7360 2070 726f 7065 7274 792e 5c6e 2d20  s` property.\n- 
-00000d70: 606f 7574 7075 7460 3a20 5468 6520 6f75  `output`: The ou
-00000d80: 7470 7574 206e 616d 6520 6f66 2074 6865  tput name of the
-00000d90: 2063 6f6e 6e65 6374 696f 6e20 7468 6174   connection that
-00000da0: 2069 7320 636f 6e6e 6563 7465 6420 746f   is connected to
-00000db0: 2074 6865 2063 7572 7265 6e74 206e 6f64   the current nod
-00000dc0: 652e 2054 6869 7320 6973 206f 6e6c 7920  e. This is only 
-00000dd0: 7573 6564 2069 6e20 7468 6520 606f 7574  used in the `out
-00000de0: 7075 7473 6020 7072 6f70 6572 7479 2e5c  puts` property.\
-00000df0: 6e5c 6e54 6f20 7365 6520 736f 6d65 2065  n\nTo see some e
-00000e00: 7861 6d70 6c65 732c 2063 6865 636b 2074  xamples, check t
-00000e10: 6865 205b 6578 616d 706c 6573 5d28 6874  he [examples](ht
-00000e20: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000e30: 2f67 6162 7269 656c 6775 6172 6973 612f  /gabrielguarisa/
-00000e40: 7265 7472 6163 6b2f 7472 6565 2f6d 6169  retrack/tree/mai
-00000e50: 6e2f 6578 616d 706c 6573 2920 666f 6c64  n/examples) fold
-00000e60: 6572 2e5c 6e5c 6e23 2323 2043 7265 6174  er.\n\n### Creat
-00000e70: 696e 6720 6120 6375 7374 6f6d 206e 6f64  ing a custom nod
-00000e80: 655c 6e5c 6e54 6f20 6372 6561 7465 2061  e\n\nTo create a
-00000e90: 2063 7573 746f 6d20 6e6f 6465 2c20 796f   custom node, yo
-00000ea0: 7520 6e65 6564 2074 6f20 6372 6561 7465  u need to create
-00000eb0: 2061 2063 6c61 7373 2074 6861 7420 696e   a class that in
-00000ec0: 6865 7269 7473 2066 726f 6d20 7468 6520  herits from the 
-00000ed0: 6042 6173 654e 6f64 6560 2063 6c61 7373  `BaseNode` class
-00000ee0: 2e20 4561 6368 206e 6f64 6520 6973 2061  . Each node is a
-00000ef0: 2070 7964 616e 7469 6320 6d6f 6465 6c2c   pydantic model,
-00000f00: 2073 6f20 796f 7520 6361 6e20 7573 6520   so you can use 
-00000f10: 7079 6461 6e74 6963 2066 6561 7475 7265  pydantic feature
-00000f20: 7320 746f 2063 7265 6174 6520 796f 7572  s to create your
-00000f30: 2063 7573 746f 6d20 6e6f 6465 2e20 546f   custom node. To
-00000f40: 2073 6565 2074 6865 2061 7661 696c 6162   see the availab
-00000f50: 6c65 2066 6561 7475 7265 732c 2063 6865  le features, che
-00000f60: 636b 2074 6865 205b 7079 6461 6e74 6963  ck the [pydantic
-00000f70: 2064 6f63 756d 656e 7461 7469 6f6e 5d28   documentation](
-00000f80: 6874 7470 733a 2f2f 7079 6461 6e74 6963  https://pydantic
-00000f90: 2d64 6f63 732e 6865 6c70 6d61 6e75 616c  -docs.helpmanual
-00000fa0: 2e69 6f2f 292e 5c6e 5c6e 546f 2063 7265  .io/).\n\nTo cre
-00000fb0: 6174 6520 6120 6375 7374 6f6d 206e 6f64  ate a custom nod
-00000fc0: 6520 796f 7520 6e65 6564 2074 6f20 6465  e you need to de
-00000fd0: 6669 6e65 2074 6865 2069 6e70 7574 7320  fine the inputs 
-00000fe0: 616e 6420 6f75 7470 7574 7320 6f66 2074  and outputs of t
-00000ff0: 6865 206e 6f64 652e 2054 6f20 646f 2074  he node. To do t
-00001000: 6869 732c 2079 6f75 206e 6565 6420 746f  his, you need to
-00001010: 2064 6566 696e 6520 7468 6520 6069 6e70   define the `inp
-00001020: 7574 7360 2061 6e64 2060 6f75 7470 7574  uts` and `output
-00001030: 7360 2063 6c61 7373 2061 7474 7269 6275  s` class attribu
-00001040: 7465 732e 204c 6574 5c27 7320 7365 6520  tes. Let\'s see 
-00001050: 616e 2065 7861 6d70 6c65 206f 6620 6120  an example of a 
-00001060: 6375 7374 6f6d 206e 6f64 6520 7468 6174  custom node that
-00001070: 2068 6173 2074 776f 2069 6e70 7574 732c   has two inputs,
-00001080: 2073 756d 2074 6865 6d20 616e 6420 7265   sum them and re
-00001090: 7475 726e 2074 6865 2072 6573 756c 743a  turn the result:
-000010a0: 5c6e 5c6e 6060 6070 7974 686f 6e5c 6e69  \n\n```python\ni
-000010b0: 6d70 6f72 7420 7265 7472 6163 6b5c 6e69  mport retrack\ni
-000010c0: 6d70 6f72 7420 7079 6461 6e74 6963 5c6e  mport pydantic\n
-000010d0: 696d 706f 7274 2070 616e 6461 7320 6173  import pandas as
-000010e0: 2070 645c 6e69 6d70 6f72 7420 7479 7069   pd\nimport typi
-000010f0: 6e67 5c6e 5c6e 5c6e 636c 6173 7320 5375  ng\n\n\nclass Su
-00001100: 6d49 6e70 7574 734d 6f64 656c 2870 7964  mInputsModel(pyd
-00001110: 616e 7469 632e 4261 7365 4d6f 6465 6c29  antic.BaseModel)
-00001120: 3a5c 6e20 2020 2069 6e70 7574 5f76 616c  :\n    input_val
-00001130: 7565 5f30 3a20 7265 7472 6163 6b2e 496e  ue_0: retrack.In
-00001140: 7075 7443 6f6e 6e65 6374 696f 6e4d 6f64  putConnectionMod
-00001150: 656c 5c6e 2020 2020 696e 7075 745f 7661  el\n    input_va
-00001160: 6c75 655f 313a 2072 6574 7261 636b 2e49  lue_1: retrack.I
-00001170: 6e70 7574 436f 6e6e 6563 7469 6f6e 4d6f  nputConnectionMo
-00001180: 6465 6c5c 6e5c 6e5c 6e63 6c61 7373 2053  del\n\n\nclass S
-00001190: 756d 4f75 7470 7574 734d 6f64 656c 2870  umOutputsModel(p
-000011a0: 7964 616e 7469 632e 4261 7365 4d6f 6465  ydantic.BaseMode
-000011b0: 6c29 3a5c 6e20 2020 206f 7574 7075 745f  l):\n    output_
-000011c0: 7661 6c75 653a 2072 6574 7261 636b 2e4f  value: retrack.O
-000011d0: 7574 7075 7443 6f6e 6e65 6374 696f 6e4d  utputConnectionM
-000011e0: 6f64 656c 5c6e 5c6e 5c6e 636c 6173 7320  odel\n\n\nclass 
-000011f0: 5375 6d4e 6f64 6528 7265 7472 6163 6b2e  SumNode(retrack.
-00001200: 4261 7365 4e6f 6465 293a 5c6e 2020 2020  BaseNode):\n    
-00001210: 696e 7075 7473 3a20 5375 6d49 6e70 7574  inputs: SumInput
-00001220: 734d 6f64 656c 5c6e 2020 2020 6f75 7470  sModel\n    outp
-00001230: 7574 733a 2053 756d 4f75 7470 7574 734d  uts: SumOutputsM
-00001240: 6f64 656c 5c6e 5c6e 2020 2020 6465 6620  odel\n\n    def 
-00001250: 7275 6e28 7365 6c66 2c20 696e 7075 745f  run(self, input_
-00001260: 7661 6c75 655f 303a 2070 642e 5365 7269  value_0: pd.Seri
-00001270: 6573 2c5c 6e20 2020 2020 2020 2069 6e70  es,\n        inp
-00001280: 7574 5f76 616c 7565 5f31 3a20 7064 2e53  ut_value_1: pd.S
-00001290: 6572 6965 732c 5c6e 2020 2020 2920 2d3e  eries,\n    ) ->
-000012a0: 2074 7970 696e 672e 4469 6374 5b73 7472   typing.Dict[str
-000012b0: 2c20 7064 2e53 6572 6965 735d 3a5c 6e20  , pd.Series]:\n 
-000012c0: 2020 2020 2020 206f 7574 7075 745f 7661         output_va
-000012d0: 6c75 6520 3d20 696e 7075 745f 7661 6c75  lue = input_valu
-000012e0: 655f 302e 6173 7479 7065 2866 6c6f 6174  e_0.astype(float
-000012f0: 2920 2b20 696e 7075 745f 7661 6c75 655f  ) + input_value_
-00001300: 312e 6173 7479 7065 2866 6c6f 6174 295c  1.astype(float)\
-00001310: 6e20 2020 2020 2020 2072 6574 7572 6e20  n        return 
-00001320: 7b5c 6e20 2020 2020 2020 2020 2020 2022  {\n            "
-00001330: 6f75 7470 7574 5f76 616c 7565 223a 206f  output_value": o
-00001340: 7574 7075 745f 7661 6c75 652c 5c6e 2020  utput_value,\n  
-00001350: 2020 2020 2020 7d5c 6e60 6060 5c6e 5c6e        }\n```\n\n
-00001360: 4166 7465 7220 6372 6561 7469 6e67 2074  After creating t
-00001370: 6865 2063 7573 746f 6d20 6e6f 6465 2c20  he custom node, 
-00001380: 796f 7520 6e65 6564 2074 6f20 7265 6769  you need to regi
-00001390: 7374 6572 2069 7420 696e 2074 6865 206e  ster it in the n
-000013a0: 6f64 6573 2072 6567 6973 7472 7920 616e  odes registry an
-000013b0: 6420 7061 7373 2074 6865 2072 6567 6973  d pass the regis
-000013c0: 7472 7920 746f 2074 6865 2070 6172 7365  try to the parse
-000013d0: 722e 204c 6574 5c27 7320 7365 6520 616e  r. Let\'s see an
-000013e0: 2065 7861 6d70 6c65 3a5c 6e5c 6e60 6060   example:\n\n```
-000013f0: 7079 7468 6f6e 5c6e 696d 706f 7274 2072  python\nimport r
-00001400: 6574 7261 636b 5c6e 5c6e 2320 5265 6769  etrack\n\n# Regi
-00001410: 7374 6572 2074 6865 2063 7573 746f 6d20  ster the custom 
-00001420: 6e6f 6465 5c6e 7265 7472 6163 6b2e 636f  node\nretrack.co
-00001430: 6d70 6f6e 656e 745f 7265 6769 7374 7279  mponent_registry
-00001440: 2e72 6567 6973 7465 725f 6e6f 6465 2822  .register_node("
-00001450: 7375 6d22 2c20 5375 6d4e 6f64 6529 5c6e  sum", SumNode)\n
-00001460: 5c6e 2320 5061 7273 6520 7468 6520 7275  \n# Parse the ru
-00001470: 6c65 2f6d 6f64 656c 5c6e 7061 7273 6572  le/model\nparser
-00001480: 203d 2050 6172 7365 7228 7275 6c65 2c20   = Parser(rule, 
-00001490: 636f 6d70 6f6e 656e 745f 7265 6769 7374  component_regist
-000014a0: 7279 3d72 6574 7261 636b 2e63 6f6d 706f  ry=retrack.compo
-000014b0: 6e65 6e74 5f72 6567 6973 7472 7929 5c6e  nent_registry)\n
-000014c0: 6060 605c 6e5c 6e23 2320 436f 6e74 7269  ```\n\n## Contri
-000014d0: 6275 7469 6e67 5c6e 5c6e 436f 6e74 7269  buting\n\nContri
-000014e0: 6275 7469 6f6e 7320 6172 6520 7765 6c63  butions are welc
-000014f0: 6f6d 6521 2050 6c65 6173 6520 7265 6164  ome! Please read
-00001500: 2074 6865 205b 636f 6e74 7269 6275 7469   the [contributi
-00001510: 6e67 2067 7569 6465 6c69 6e65 735d 2868  ng guidelines](h
-00001520: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001530: 6d2f 6761 6272 6965 6c67 7561 7269 7361  m/gabrielguarisa
-00001540: 2f72 6574 7261 636b 2f74 7265 652f 6d61  /retrack/tree/ma
-00001550: 696e 2f43 4f4e 5452 4942 5554 494e 472e  in/CONTRIBUTING.
-00001560: 6d64 2920 6669 7273 742e 272c 0a20 2020  md) first.',.   
-00001570: 2027 6175 7468 6f72 273a 2027 4761 6272   'author': 'Gabr
-00001580: 6965 6c20 4775 6172 6973 6127 2c0a 2020  iel Guarisa',.  
-00001590: 2020 2761 7574 686f 725f 656d 6169 6c27    'author_email'
-000015a0: 3a20 2767 6162 7269 656c 6775 6172 6973  : 'gabrielguaris
-000015b0: 6140 676d 6169 6c2e 636f 6d27 2c0a 2020  a@gmail.com',.  
-000015c0: 2020 276d 6169 6e74 6169 6e65 7227 3a20    'maintainer': 
-000015d0: 4e6f 6e65 2c0a 2020 2020 276d 6169 6e74  None,.    'maint
-000015e0: 6169 6e65 725f 656d 6169 6c27 3a20 4e6f  ainer_email': No
-000015f0: 6e65 2c0a 2020 2020 2775 726c 273a 2027  ne,.    'url': '
-00001600: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001610: 6f6d 2f67 6162 7269 656c 6775 6172 6973  om/gabrielguaris
-00001620: 612f 7265 7472 6163 6b27 2c0a 2020 2020  a/retrack',.    
-00001630: 2770 6163 6b61 6765 7327 3a20 7061 636b  'packages': pack
-00001640: 6167 6573 2c0a 2020 2020 2770 6163 6b61  ages,.    'packa
-00001650: 6765 5f64 6174 6127 3a20 7061 636b 6167  ge_data': packag
-00001660: 655f 6461 7461 2c0a 2020 2020 2769 6e73  e_data,.    'ins
-00001670: 7461 6c6c 5f72 6571 7569 7265 7327 3a20  tall_requires': 
-00001680: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
-00001690: 2c0a 2020 2020 2770 7974 686f 6e5f 7265  ,.    'python_re
-000016a0: 7175 6972 6573 273a 2027 3e3d 332e 382e  quires': '>=3.8.
-000016b0: 3136 2c3c 342e 302e 3027 2c0a 7d0a 0a0a  16,<4.0.0',.}...
-000016c0: 7365 7475 7028 2a2a 7365 7475 705f 6b77  setup(**setup_kw
-000016d0: 6172 6773 290a                           args).
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 7265 7472  : 2.1.Name: retr
+00000020: 6163 6b0a 5665 7273 696f 6e3a 2030 2e35  ack.Version: 0.5
+00000030: 2e30 0a53 756d 6d61 7279 3a20 4120 6275  .0.Summary: A bu
+00000040: 7369 6e65 7373 2072 756c 6573 2065 6e67  siness rules eng
+00000050: 696e 650a 486f 6d65 2d70 6167 653a 2068  ine.Home-page: h
+00000060: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000070: 6d2f 6761 6272 6965 6c67 7561 7269 7361  m/gabrielguarisa
+00000080: 2f72 6574 7261 636b 0a4c 6963 656e 7365  /retrack.License
+00000090: 3a20 4d49 540a 4b65 7977 6f72 6473 3a20  : MIT.Keywords: 
+000000a0: 7275 6c65 732c 6d6f 6465 6c73 2c62 7573  rules,models,bus
+000000b0: 696e 6573 732c 6e6f 6465 2c67 7261 7068  iness,node,graph
+000000c0: 0a41 7574 686f 723a 2047 6162 7269 656c  .Author: Gabriel
+000000d0: 2047 7561 7269 7361 0a41 7574 686f 722d   Guarisa.Author-
+000000e0: 656d 6169 6c3a 2067 6162 7269 656c 6775  email: gabrielgu
+000000f0: 6172 6973 6140 676d 6169 6c2e 636f 6d0a  arisa@gmail.com.
+00000100: 5265 7175 6972 6573 2d50 7974 686f 6e3a  Requires-Python:
+00000110: 203e 3d33 2e38 2e31 362c 3c34 2e30 2e30   >=3.8.16,<4.0.0
+00000120: 0a43 6c61 7373 6966 6965 723a 204c 6963  .Classifier: Lic
+00000130: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
+00000140: 6f76 6564 203a 3a20 4d49 5420 4c69 6365  oved :: MIT Lice
+00000150: 6e73 650a 436c 6173 7369 6669 6572 3a20  nse.Classifier: 
+00000160: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000170: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000180: 3a20 330a 436c 6173 7369 6669 6572 3a20  : 3.Classifier: 
+00000190: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000001a0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+000001b0: 3a20 332e 390a 436c 6173 7369 6669 6572  : 3.9.Classifier
+000001c0: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+000001d0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+000001e0: 203a 3a20 332e 3130 0a43 6c61 7373 6966   :: 3.10.Classif
+000001f0: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+00000200: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000210: 686f 6e20 3a3a 2033 2e31 310a 5265 7175  hon :: 3.11.Requ
+00000220: 6972 6573 2d44 6973 743a 206e 6574 776f  ires-Dist: netwo
+00000230: 726b 7820 283e 3d33 2e30 2c3c 342e 3029  rkx (>=3.0,<4.0)
+00000240: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000250: 7061 6e64 6173 2028 3e3d 312e 352e 322c  pandas (>=1.5.2,
+00000260: 3c32 2e30 2e30 290a 5265 7175 6972 6573  <2.0.0).Requires
+00000270: 2d44 6973 743a 2070 7964 616e 7469 6320  -Dist: pydantic 
+00000280: 283e 3d31 2e31 302e 342c 3c32 2e30 2e30  (>=1.10.4,<2.0.0
+00000290: 290a 5072 6f6a 6563 742d 5552 4c3a 2052  ).Project-URL: R
+000002a0: 6570 6f73 6974 6f72 792c 2068 7474 7073  epository, https
+000002b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6761  ://github.com/ga
+000002c0: 6272 6965 6c67 7561 7269 7361 2f72 6574  brielguarisa/ret
+000002d0: 7261 636b 0a44 6573 6372 6970 7469 6f6e  rack.Description
+000002e0: 2d43 6f6e 7465 6e74 2d54 7970 653a 2074  -Content-Type: t
+000002f0: 6578 742f 6d61 726b 646f 776e 0a0a 3c70  ext/markdown..<p
+00000300: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
+00000310: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
+00000320: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f67  s://github.com/g
+00000330: 6162 7269 656c 6775 6172 6973 612f 7265  abrielguarisa/re
+00000340: 7472 6163 6b22 3e3c 696d 6720 7372 633d  track"><img src=
+00000350: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
+00000360: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+00000370: 6f6d 2f67 6162 7269 656c 6775 6172 6973  om/gabrielguaris
+00000380: 612f 7265 7472 6163 6b2f 6d61 696e 2f6c  a/retrack/main/l
+00000390: 6f67 6f2e 706e 6722 2061 6c74 3d22 7265  ogo.png" alt="re
+000003a0: 7472 6163 6b22 3e3c 2f61 3e0a 3c2f 703e  track"></a>.</p>
+000003b0: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+000003c0: 7222 3e0a 2020 2020 3c65 6d3e 4120 6275  r">.    <em>A bu
+000003d0: 7369 6e65 7373 2072 756c 6573 2065 6e67  siness rules eng
+000003e0: 696e 653c 2f65 6d3e 0a3c 2f70 3e0a 0a3c  ine</em>.</p>..<
+000003f0: 6469 7620 616c 6967 6e3d 2263 656e 7465  div align="cente
+00000400: 7222 3e0a 0a5b 215b 5061 636b 6167 6520  r">..[![Package 
+00000410: 7665 7273 696f 6e5d 2868 7474 7073 3a2f  version](https:/
+00000420: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000430: 7079 7069 2f76 2f72 6574 7261 636b 3f63  pypi/v/retrack?c
+00000440: 6f6c 6f72 3d25 3233 3334 4430 3538 266c  olor=%2334D058&l
+00000450: 6162 656c 3d70 7970 6925 3230 7061 636b  abel=pypi%20pack
+00000460: 6167 6529 5d28 6874 7470 733a 2f2f 7079  age)](https://py
+00000470: 7069 2e6f 7267 2f70 726f 6a65 6374 2f72  pi.org/project/r
+00000480: 6574 7261 636b 2f29 0a5b 215b 436f 6465  etrack/).[![Code
+00000490: 2073 7479 6c65 3a20 626c 6163 6b5d 2868   style: black](h
+000004a0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+000004b0: 6473 2e69 6f2f 6261 6467 652f 636f 6465  ds.io/badge/code
+000004c0: 2532 3073 7479 6c65 2d62 6c61 636b 2d30  %20style-black-0
+000004d0: 3030 3030 302e 7376 6729 5d28 6874 7470  00000.svg)](http
+000004e0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
+000004f0: 7366 2f62 6c61 636b 290a 5b21 5b53 656d  sf/black).[![Sem
+00000500: 616e 7469 6320 5665 7273 696f 6e73 5d28  antic Versions](
+00000510: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000520: 6c64 732e 696f 2f62 6164 6765 2f25 3230  lds.io/badge/%20
+00000530: 2532 3025 4630 2539 4625 3933 2541 3625  %20%F0%9F%93%A6%
+00000540: 4630 2539 4625 3941 2538 302d 7365 6d61  F0%9F%9A%80-sema
+00000550: 6e74 6963 2d2d 7665 7273 696f 6e73 2d65  ntic--versions-e
+00000560: 3130 3037 392e 7376 6729 5d28 6874 7470  10079.svg)](http
+00000570: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f67  s://github.com/g
+00000580: 6162 7269 656c 6775 6172 6973 612f 7265  abrielguarisa/re
+00000590: 7472 6163 6b2f 7265 6c65 6173 6573 290a  track/releases).
+000005a0: 5b21 5b4c 6963 656e 7365 5d28 6874 7470  [![License](http
+000005b0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+000005c0: 696f 2f67 6974 6875 622f 6c69 6365 6e73  io/github/licens
+000005d0: 652f 6761 6272 6965 6c67 7561 7269 7361  e/gabrielguarisa
+000005e0: 2f72 6574 7261 636b 295d 2868 7474 7073  /retrack)](https
+000005f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6761  ://github.com/ga
+00000600: 6272 6965 6c67 7561 7269 7361 2f72 6574  brielguarisa/ret
+00000610: 7261 636b 2f62 6c6f 622f 6d61 696e 2f4c  rack/blob/main/L
+00000620: 4943 454e 5345 290a 0a3c 2f64 6976 3e0a  ICENSE)..</div>.
+00000630: 0a0a 2323 2049 6e73 7461 6c6c 6174 696f  ..## Installatio
+00000640: 6e0a 0a60 6060 6261 7368 0a70 6970 2069  n..```bash.pip i
+00000650: 6e73 7461 6c6c 2072 6574 7261 636b 0a60  nstall retrack.`
+00000660: 6060 0a0a 2323 2055 7361 6765 0a0a 6060  ``..## Usage..``
+00000670: 6070 7974 686f 6e0a 696d 706f 7274 2072  `python.import r
+00000680: 6574 7261 636b 0a0a 2320 5061 7273 6520  etrack..# Parse 
+00000690: 7468 6520 7275 6c65 2f6d 6f64 656c 0a70  the rule/model.p
+000006a0: 6172 7365 7220 3d20 7265 7472 6163 6b2e  arser = retrack.
+000006b0: 5061 7273 6572 2872 756c 6529 0a0a 2320  Parser(rule)..# 
+000006c0: 4372 6561 7465 2061 2072 756e 6e65 720a  Create a runner.
+000006d0: 7275 6e6e 6572 203d 2072 6574 7261 636b  runner = retrack
+000006e0: 2e52 756e 6e65 7228 7061 7273 6572 290a  .Runner(parser).
+000006f0: 0a23 2052 756e 2074 6865 2072 756c 652f  .# Run the rule/
+00000700: 6d6f 6465 6c20 7061 7373 696e 6720 7468  model passing th
+00000710: 6520 6461 7461 0a72 756e 6e65 722e 6578  e data.runner.ex
+00000720: 6563 7574 6528 6461 7461 290a 6060 600a  ecute(data).```.
+00000730: 0a54 6865 2060 5061 7273 6572 6020 636c  .The `Parser` cl
+00000740: 6173 7320 7061 7273 6573 2074 6865 2072  ass parses the r
+00000750: 756c 652f 6d6f 6465 6c20 616e 6420 6372  ule/model and cr
+00000760: 6561 7465 7320 6120 6772 6170 6820 6f66  eates a graph of
+00000770: 206e 6f64 6573 2e20 5468 6520 6052 756e   nodes. The `Run
+00000780: 6e65 7260 2063 6c61 7373 2072 756e 7320  ner` class runs 
+00000790: 7468 6520 7275 6c65 2f6d 6f64 656c 2075  the rule/model u
+000007a0: 7369 6e67 2074 6865 2064 6174 6120 7061  sing the data pa
+000007b0: 7373 6564 2074 6f20 7468 6520 7275 6e6e  ssed to the runn
+000007c0: 6572 2e20 5468 6520 6064 6174 6160 2069  er. The `data` i
+000007d0: 7320 6120 6469 6374 696f 6e61 7279 206f  s a dictionary o
+000007e0: 7220 6120 6c69 7374 206f 6620 6469 6374  r a list of dict
+000007f0: 696f 6e61 7269 6573 2063 6f6e 7461 696e  ionaries contain
+00000800: 696e 6720 7468 6520 6461 7461 2074 6861  ing the data tha
+00000810: 7420 7769 6c6c 2062 6520 7573 6564 2074  t will be used t
+00000820: 6f20 6576 616c 7561 7465 2074 6865 2063  o evaluate the c
+00000830: 6f6e 6469 7469 6f6e 7320 616e 6420 6578  onditions and ex
+00000840: 6563 7574 6520 7468 6520 6163 7469 6f6e  ecute the action
+00000850: 732e 2054 6f20 7365 6520 7769 6368 2064  s. To see wich d
+00000860: 6174 6120 6973 2072 6571 7569 7265 6420  ata is required 
+00000870: 666f 7220 7468 6520 6769 7665 6e20 7275  for the given ru
+00000880: 6c65 2f6d 6f64 656c 2c20 6368 6563 6b20  le/model, check 
+00000890: 7468 6520 6072 756e 6e65 722e 7265 7175  the `runner.requ
+000008a0: 6573 745f 6d6f 6465 6c60 2070 726f 7065  est_model` prope
+000008b0: 7274 7920 7468 6174 2069 7320 6120 7079  rty that is a py
+000008c0: 6461 6e74 6963 206d 6f64 656c 2075 7365  dantic model use
+000008d0: 6420 746f 2076 616c 6964 6174 6520 7468  d to validate th
+000008e0: 6520 6461 7461 2e0a 0a23 2323 2043 7265  e data...### Cre
+000008f0: 6174 696e 6720 6120 7275 6c65 2f6d 6f64  ating a rule/mod
+00000900: 656c 0a0a 4120 7275 6c65 2069 7320 6120  el..A rule is a 
+00000910: 7365 7420 6f66 2063 6f6e 6469 7469 6f6e  set of condition
+00000920: 7320 616e 6420 6163 7469 6f6e 7320 7468  s and actions th
+00000930: 6174 2061 7265 2065 7865 6375 7465 6420  at are executed 
+00000940: 7768 656e 2074 6865 2063 6f6e 6469 7469  when the conditi
+00000950: 6f6e 7320 6172 6520 6d65 742e 2054 6865  ons are met. The
+00000960: 2063 6f6e 6469 7469 6f6e 7320 6172 6520   conditions are 
+00000970: 6576 616c 7561 7465 6420 7573 696e 6720  evaluated using 
+00000980: 7468 6520 6461 7461 2070 6173 7365 6420  the data passed 
+00000990: 746f 2074 6865 2072 756e 6e65 722e 2054  to the runner. T
+000009a0: 6865 2061 6374 696f 6e73 2061 7265 2065  he actions are e
+000009b0: 7865 6375 7465 6420 7768 656e 2074 6865  xecuted when the
+000009c0: 2063 6f6e 6469 7469 6f6e 7320 6172 6520   conditions are 
+000009d0: 6d65 742e 0a0a 4561 6368 2072 756c 6520  met...Each rule 
+000009e0: 6973 2063 6f6d 706f 7365 6420 6f66 206d  is composed of m
+000009f0: 616e 7920 6e6f 6465 732e 2054 6f20 7365  any nodes. To se
+00000a00: 6520 6561 6368 206e 6f64 6520 7479 7065  e each node type
+00000a10: 2c20 6368 6563 6b20 7468 6520 5b6e 6f64  , check the [nod
+00000a20: 6573 5d28 6874 7470 733a 2f2f 6769 7468  es](https://gith
+00000a30: 7562 2e63 6f6d 2f67 6162 7269 656c 6775  ub.com/gabrielgu
+00000a40: 6172 6973 612f 7265 7472 6163 6b2f 7472  arisa/retrack/tr
+00000a50: 6565 2f6d 6169 6e2f 7265 7472 6163 6b2f  ee/main/retrack/
+00000a60: 6e6f 6465 7329 2066 6f6c 6465 722e 0a0a  nodes) folder...
+00000a70: 546f 2063 7265 6174 6520 6120 7275 6c65  To create a rule
+00000a80: 2c20 796f 7520 6e65 6564 2074 6f20 6372  , you need to cr
+00000a90: 6561 7465 2061 204a 534f 4e20 6669 6c65  eate a JSON file
+00000aa0: 2077 6974 6820 7468 6520 666f 6c6c 6f77   with the follow
+00000ab0: 696e 6720 7374 7275 6374 7572 653a 0a0a  ing structure:..
+00000ac0: 6060 606a 736f 6e0a 7b0a 2020 226e 6f64  ```json.{.  "nod
+00000ad0: 6573 223a 207b 0a09 0922 6e6f 6465 2069  es": {..."node i
+00000ae0: 6422 3a20 7b0a 0909 0922 6964 223a 2022  d": {...."id": "
+00000af0: 6e6f 6465 2069 6422 2c0a 0909 0922 6461  node id",...."da
+00000b00: 7461 223a 207b 7d2c 0a09 0909 2269 6e70  ta": {},...."inp
+00000b10: 7574 7322 3a20 7b7d 2c0a 0909 0922 6f75  uts": {},...."ou
+00000b20: 7470 7574 7322 3a20 7b7d 2c0a 0909 0922  tputs": {},...."
+00000b30: 6e61 6d65 223a 2022 6e6f 6465 206e 616d  name": "node nam
+00000b40: 6522 2c0a 0909 7d2c 0a20 2020 202f 2f20  e",...},.    // 
+00000b50: 2e2e 2e20 6d6f 7265 206e 6f64 6573 0a20  ... more nodes. 
+00000b60: 207d 0a7d 0a60 6060 0a0a 5468 6520 606e   }.}.```..The `n
+00000b70: 6f64 6573 6020 6b65 7920 6973 2061 2064  odes` key is a d
+00000b80: 6963 7469 6f6e 6172 7920 6f66 206e 6f64  ictionary of nod
+00000b90: 6573 2e20 4561 6368 206e 6f64 6520 6861  es. Each node ha
+00000ba0: 7320 7468 6520 666f 6c6c 6f77 696e 6720  s the following 
+00000bb0: 7072 6f70 6572 7469 6573 3a0a 0a2d 2060  properties:..- `
+00000bc0: 6964 603a 2054 6865 206e 6f64 6520 6964  id`: The node id
+00000bd0: 2e20 5468 6973 2069 7320 7573 6564 2074  . This is used t
+00000be0: 6f20 7265 6665 7265 6e63 6520 7468 6520  o reference the 
+00000bf0: 6e6f 6465 2069 6e20 7468 6520 6069 6e70  node in the `inp
+00000c00: 7574 7360 2061 6e64 2060 6f75 7470 7574  uts` and `output
+00000c10: 7360 2070 726f 7065 7274 6965 732e 0a2d  s` properties..-
+00000c20: 2060 6461 7461 603a 2054 6865 206e 6f64   `data`: The nod
+00000c30: 6520 6461 7461 2e20 5468 6973 2069 7320  e data. This is 
+00000c40: 7573 6564 2061 7320 6120 6d65 7461 6461  used as a metada
+00000c50: 7461 2066 6f72 2074 6865 206e 6f64 652e  ta for the node.
+00000c60: 0a2d 2060 696e 7075 7473 603a 2054 6865  .- `inputs`: The
+00000c70: 206e 6f64 6520 696e 7075 7473 2e20 5468   node inputs. Th
+00000c80: 6973 2069 7320 7573 6564 2074 6f20 7265  is is used to re
+00000c90: 6665 7265 6e63 6520 7468 6520 6e6f 6465  ference the node
+00000ca0: 2069 6e70 7574 732e 0a2d 2060 6f75 7470   inputs..- `outp
+00000cb0: 7574 7360 3a20 5468 6520 6e6f 6465 206f  uts`: The node o
+00000cc0: 7574 7075 7473 2e20 5468 6973 2069 7320  utputs. This is 
+00000cd0: 7573 6564 2074 6f20 7265 6665 7265 6e63  used to referenc
+00000ce0: 6520 7468 6520 6e6f 6465 206f 7574 7075  e the node outpu
+00000cf0: 7473 2e0a 2d20 606e 616d 6560 3a20 5468  ts..- `name`: Th
+00000d00: 6520 6e6f 6465 206e 616d 652e 2054 6869  e node name. Thi
+00000d10: 7320 6973 2075 7365 6420 746f 2064 6566  s is used to def
+00000d20: 696e 6520 7468 6520 6e6f 6465 2074 7970  ine the node typ
+00000d30: 652e 0a0a 5468 6520 6069 6e70 7574 7360  e...The `inputs`
+00000d40: 2061 6e64 2060 6f75 7470 7574 7360 2070   and `outputs` p
+00000d50: 726f 7065 7274 6965 7320 6172 6520 6469  roperties are di
+00000d60: 6374 696f 6e61 7269 6573 206f 6620 6e6f  ctionaries of no
+00000d70: 6465 2063 6f6e 6e65 6374 696f 6e73 2e20  de connections. 
+00000d80: 4561 6368 2063 6f6e 6e65 6374 696f 6e20  Each connection 
+00000d90: 6861 7320 7468 6520 666f 6c6c 6f77 696e  has the followin
+00000da0: 6720 7072 6f70 6572 7469 6573 3a0a 0a2d  g properties:..-
+00000db0: 2060 6e6f 6465 603a 2054 6865 206e 6f64   `node`: The nod
+00000dc0: 6520 6964 2074 6861 7420 6973 2063 6f6e  e id that is con
+00000dd0: 6e65 6374 6564 2074 6f20 7468 6520 6375  nected to the cu
+00000de0: 7272 656e 7420 6e6f 6465 2e0a 2d20 6069  rrent node..- `i
+00000df0: 6e70 7574 603a 2054 6865 2069 6e70 7574  nput`: The input
+00000e00: 206e 616d 6520 6f66 2074 6865 2063 6f6e   name of the con
+00000e10: 6e65 6374 696f 6e20 7468 6174 2069 7320  nection that is 
+00000e20: 636f 6e6e 6563 7465 6420 746f 2074 6865  connected to the
+00000e30: 2063 7572 7265 6e74 206e 6f64 652e 2054   current node. T
+00000e40: 6869 7320 6973 206f 6e6c 7920 7573 6564  his is only used
+00000e50: 2069 6e20 7468 6520 6069 6e70 7574 7360   in the `inputs`
+00000e60: 2070 726f 7065 7274 792e 0a2d 2060 6f75   property..- `ou
+00000e70: 7470 7574 603a 2054 6865 206f 7574 7075  tput`: The outpu
+00000e80: 7420 6e61 6d65 206f 6620 7468 6520 636f  t name of the co
+00000e90: 6e6e 6563 7469 6f6e 2074 6861 7420 6973  nnection that is
+00000ea0: 2063 6f6e 6e65 6374 6564 2074 6f20 7468   connected to th
+00000eb0: 6520 6375 7272 656e 7420 6e6f 6465 2e20  e current node. 
+00000ec0: 5468 6973 2069 7320 6f6e 6c79 2075 7365  This is only use
+00000ed0: 6420 696e 2074 6865 2060 6f75 7470 7574  d in the `output
+00000ee0: 7360 2070 726f 7065 7274 792e 0a0a 546f  s` property...To
+00000ef0: 2073 6565 2073 6f6d 6520 6578 616d 706c   see some exampl
+00000f00: 6573 2c20 6368 6563 6b20 7468 6520 5b65  es, check the [e
+00000f10: 7861 6d70 6c65 735d 2868 7474 7073 3a2f  xamples](https:/
+00000f20: 2f67 6974 6875 622e 636f 6d2f 6761 6272  /github.com/gabr
+00000f30: 6965 6c67 7561 7269 7361 2f72 6574 7261  ielguarisa/retra
+00000f40: 636b 2f74 7265 652f 6d61 696e 2f65 7861  ck/tree/main/exa
+00000f50: 6d70 6c65 7329 2066 6f6c 6465 722e 0a0a  mples) folder...
+00000f60: 2323 2320 4372 6561 7469 6e67 2061 2063  ### Creating a c
+00000f70: 7573 746f 6d20 6e6f 6465 0a0a 546f 2063  ustom node..To c
+00000f80: 7265 6174 6520 6120 6375 7374 6f6d 206e  reate a custom n
+00000f90: 6f64 652c 2079 6f75 206e 6565 6420 746f  ode, you need to
+00000fa0: 2063 7265 6174 6520 6120 636c 6173 7320   create a class 
+00000fb0: 7468 6174 2069 6e68 6572 6974 7320 6672  that inherits fr
+00000fc0: 6f6d 2074 6865 2060 4261 7365 4e6f 6465  om the `BaseNode
+00000fd0: 6020 636c 6173 732e 2045 6163 6820 6e6f  ` class. Each no
+00000fe0: 6465 2069 7320 6120 7079 6461 6e74 6963  de is a pydantic
+00000ff0: 206d 6f64 656c 2c20 736f 2079 6f75 2063   model, so you c
+00001000: 616e 2075 7365 2070 7964 616e 7469 6320  an use pydantic 
+00001010: 6665 6174 7572 6573 2074 6f20 6372 6561  features to crea
+00001020: 7465 2079 6f75 7220 6375 7374 6f6d 206e  te your custom n
+00001030: 6f64 652e 2054 6f20 7365 6520 7468 6520  ode. To see the 
+00001040: 6176 6169 6c61 626c 6520 6665 6174 7572  available featur
+00001050: 6573 2c20 6368 6563 6b20 7468 6520 5b70  es, check the [p
+00001060: 7964 616e 7469 6320 646f 6375 6d65 6e74  ydantic document
+00001070: 6174 696f 6e5d 2868 7474 7073 3a2f 2f70  ation](https://p
+00001080: 7964 616e 7469 632d 646f 6373 2e68 656c  ydantic-docs.hel
+00001090: 706d 616e 7561 6c2e 696f 2f29 2e0a 0a54  pmanual.io/)...T
+000010a0: 6f20 6372 6561 7465 2061 2063 7573 746f  o create a custo
+000010b0: 6d20 6e6f 6465 2079 6f75 206e 6565 6420  m node you need 
+000010c0: 746f 2064 6566 696e 6520 7468 6520 696e  to define the in
+000010d0: 7075 7473 2061 6e64 206f 7574 7075 7473  puts and outputs
+000010e0: 206f 6620 7468 6520 6e6f 6465 2e20 546f   of the node. To
+000010f0: 2064 6f20 7468 6973 2c20 796f 7520 6e65   do this, you ne
+00001100: 6564 2074 6f20 6465 6669 6e65 2074 6865  ed to define the
+00001110: 2060 696e 7075 7473 6020 616e 6420 606f   `inputs` and `o
+00001120: 7574 7075 7473 6020 636c 6173 7320 6174  utputs` class at
+00001130: 7472 6962 7574 6573 2e20 4c65 7427 7320  tributes. Let's 
+00001140: 7365 6520 616e 2065 7861 6d70 6c65 206f  see an example o
+00001150: 6620 6120 6375 7374 6f6d 206e 6f64 6520  f a custom node 
+00001160: 7468 6174 2068 6173 2074 776f 2069 6e70  that has two inp
+00001170: 7574 732c 2073 756d 2074 6865 6d20 616e  uts, sum them an
+00001180: 6420 7265 7475 726e 2074 6865 2072 6573  d return the res
+00001190: 756c 743a 0a0a 6060 6070 7974 686f 6e0a  ult:..```python.
+000011a0: 696d 706f 7274 2072 6574 7261 636b 0a69  import retrack.i
+000011b0: 6d70 6f72 7420 7079 6461 6e74 6963 0a69  mport pydantic.i
+000011c0: 6d70 6f72 7420 7061 6e64 6173 2061 7320  mport pandas as 
+000011d0: 7064 0a69 6d70 6f72 7420 7479 7069 6e67  pd.import typing
+000011e0: 0a0a 0a63 6c61 7373 2053 756d 496e 7075  ...class SumInpu
+000011f0: 7473 4d6f 6465 6c28 7079 6461 6e74 6963  tsModel(pydantic
+00001200: 2e42 6173 654d 6f64 656c 293a 0a20 2020  .BaseModel):.   
+00001210: 2069 6e70 7574 5f76 616c 7565 5f30 3a20   input_value_0: 
+00001220: 7265 7472 6163 6b2e 496e 7075 7443 6f6e  retrack.InputCon
+00001230: 6e65 6374 696f 6e4d 6f64 656c 0a20 2020  nectionModel.   
+00001240: 2069 6e70 7574 5f76 616c 7565 5f31 3a20   input_value_1: 
+00001250: 7265 7472 6163 6b2e 496e 7075 7443 6f6e  retrack.InputCon
+00001260: 6e65 6374 696f 6e4d 6f64 656c 0a0a 0a63  nectionModel...c
+00001270: 6c61 7373 2053 756d 4f75 7470 7574 734d  lass SumOutputsM
+00001280: 6f64 656c 2870 7964 616e 7469 632e 4261  odel(pydantic.Ba
+00001290: 7365 4d6f 6465 6c29 3a0a 2020 2020 6f75  seModel):.    ou
+000012a0: 7470 7574 5f76 616c 7565 3a20 7265 7472  tput_value: retr
+000012b0: 6163 6b2e 4f75 7470 7574 436f 6e6e 6563  ack.OutputConnec
+000012c0: 7469 6f6e 4d6f 6465 6c0a 0a0a 636c 6173  tionModel...clas
+000012d0: 7320 5375 6d4e 6f64 6528 7265 7472 6163  s SumNode(retrac
+000012e0: 6b2e 4261 7365 4e6f 6465 293a 0a20 2020  k.BaseNode):.   
+000012f0: 2069 6e70 7574 733a 2053 756d 496e 7075   inputs: SumInpu
+00001300: 7473 4d6f 6465 6c0a 2020 2020 6f75 7470  tsModel.    outp
+00001310: 7574 733a 2053 756d 4f75 7470 7574 734d  uts: SumOutputsM
+00001320: 6f64 656c 0a0a 2020 2020 6465 6620 7275  odel..    def ru
+00001330: 6e28 7365 6c66 2c20 696e 7075 745f 7661  n(self, input_va
+00001340: 6c75 655f 303a 2070 642e 5365 7269 6573  lue_0: pd.Series
+00001350: 2c0a 2020 2020 2020 2020 696e 7075 745f  ,.        input_
+00001360: 7661 6c75 655f 313a 2070 642e 5365 7269  value_1: pd.Seri
+00001370: 6573 2c0a 2020 2020 2920 2d3e 2074 7970  es,.    ) -> typ
+00001380: 696e 672e 4469 6374 5b73 7472 2c20 7064  ing.Dict[str, pd
+00001390: 2e53 6572 6965 735d 3a0a 2020 2020 2020  .Series]:.      
+000013a0: 2020 6f75 7470 7574 5f76 616c 7565 203d    output_value =
+000013b0: 2069 6e70 7574 5f76 616c 7565 5f30 2e61   input_value_0.a
+000013c0: 7374 7970 6528 666c 6f61 7429 202b 2069  stype(float) + i
+000013d0: 6e70 7574 5f76 616c 7565 5f31 2e61 7374  nput_value_1.ast
+000013e0: 7970 6528 666c 6f61 7429 0a20 2020 2020  ype(float).     
+000013f0: 2020 2072 6574 7572 6e20 7b0a 2020 2020     return {.    
+00001400: 2020 2020 2020 2020 226f 7574 7075 745f          "output_
+00001410: 7661 6c75 6522 3a20 6f75 7470 7574 5f76  value": output_v
+00001420: 616c 7565 2c0a 2020 2020 2020 2020 7d0a  alue,.        }.
+00001430: 6060 600a 0a41 6674 6572 2063 7265 6174  ```..After creat
+00001440: 696e 6720 7468 6520 6375 7374 6f6d 206e  ing the custom n
+00001450: 6f64 652c 2079 6f75 206e 6565 6420 746f  ode, you need to
+00001460: 2072 6567 6973 7465 7220 6974 2069 6e20   register it in 
+00001470: 7468 6520 6e6f 6465 7320 7265 6769 7374  the nodes regist
+00001480: 7279 2061 6e64 2070 6173 7320 7468 6520  ry and pass the 
+00001490: 7265 6769 7374 7279 2074 6f20 7468 6520  registry to the 
+000014a0: 7061 7273 6572 2e20 4c65 7427 7320 7365  parser. Let's se
+000014b0: 6520 616e 2065 7861 6d70 6c65 3a0a 0a60  e an example:..`
+000014c0: 6060 7079 7468 6f6e 0a69 6d70 6f72 7420  ``python.import 
+000014d0: 7265 7472 6163 6b0a 0a23 2052 6567 6973  retrack..# Regis
+000014e0: 7465 7220 7468 6520 6375 7374 6f6d 206e  ter the custom n
+000014f0: 6f64 650a 7265 7472 6163 6b2e 636f 6d70  ode.retrack.comp
+00001500: 6f6e 656e 745f 7265 6769 7374 7279 2e72  onent_registry.r
+00001510: 6567 6973 7465 725f 6e6f 6465 2822 7375  egister_node("su
+00001520: 6d22 2c20 5375 6d4e 6f64 6529 0a0a 2320  m", SumNode)..# 
+00001530: 5061 7273 6520 7468 6520 7275 6c65 2f6d  Parse the rule/m
+00001540: 6f64 656c 0a70 6172 7365 7220 3d20 5061  odel.parser = Pa
+00001550: 7273 6572 2872 756c 652c 2063 6f6d 706f  rser(rule, compo
+00001560: 6e65 6e74 5f72 6567 6973 7472 793d 7265  nent_registry=re
+00001570: 7472 6163 6b2e 636f 6d70 6f6e 656e 745f  track.component_
+00001580: 7265 6769 7374 7279 290a 6060 600a 0a23  registry).```..#
+00001590: 2320 436f 6e74 7269 6275 7469 6e67 0a0a  # Contributing..
+000015a0: 436f 6e74 7269 6275 7469 6f6e 7320 6172  Contributions ar
+000015b0: 6520 7765 6c63 6f6d 6521 2050 6c65 6173  e welcome! Pleas
+000015c0: 6520 7265 6164 2074 6865 205b 636f 6e74  e read the [cont
+000015d0: 7269 6275 7469 6e67 2067 7569 6465 6c69  ributing guideli
+000015e0: 6e65 735d 2868 7474 7073 3a2f 2f67 6974  nes](https://git
+000015f0: 6875 622e 636f 6d2f 6761 6272 6965 6c67  hub.com/gabrielg
+00001600: 7561 7269 7361 2f72 6574 7261 636b 2f74  uarisa/retrack/t
+00001610: 7265 652f 6d61 696e 2f43 4f4e 5452 4942  ree/main/CONTRIB
+00001620: 5554 494e 472e 6d64 2920 6669 7273 742e  UTING.md) first.
+00001630: 0a                                       .
```

