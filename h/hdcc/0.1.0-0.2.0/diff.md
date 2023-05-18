# Comparing `tmp/hdcc-0.1.0.tar.gz` & `tmp/hdcc-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdcc-0.1.0.tar", max compression
+gzip compressed data, was "hdcc-0.2.0.tar", max compression
```

## Comparing `hdcc-0.1.0.tar` & `hdcc-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       90 2023-05-18 07:58:44.444416 hdcc-0.1.0/README.md
--rw-r--r--   0        0        0    18096 2023-05-18 07:58:44.444416 hdcc-0.1.0/hdcc/HDProg.py
--rw-r--r--   0        0        0    16200 2023-05-18 07:58:44.444416 hdcc-0.1.0/hdcc/HDTypes.py
--rw-r--r--   0        0        0        0 2023-05-18 07:58:44.444416 hdcc-0.1.0/hdcc/__init__.py
--rw-r--r--   0        0        0      330 2023-05-18 08:00:44.053127 hdcc-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 hdcc-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       90 2023-05-18 07:58:44.444416 hdcc-0.2.0/README.md
+-rw-r--r--   0        0        0    19700 2023-05-18 09:16:37.072109 hdcc-0.2.0/hdcc/HDProg.py
+-rw-r--r--   0        0        0    16280 2023-05-18 09:07:27.261645 hdcc-0.2.0/hdcc/HDTypes.py
+-rw-r--r--   0        0        0        0 2023-05-18 07:58:44.444416 hdcc-0.2.0/hdcc/__init__.py
+-rw-r--r--   0        0        0      330 2023-05-18 09:18:21.364170 hdcc-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 hdcc-0.2.0/PKG-INFO
```

### Comparing `hdcc-0.1.0/hdcc/HDProg.py` & `hdcc-0.2.0/hdcc/HDProg.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,111 +21,124 @@
 class Operator(Enum):
     BIND = "BIND"
     UNBIND = "UNBIND"
     BUNDlE = "BUNDLE"
     PERMUTATION = "PERMUTATION"
     FRAC_BIND = "FRAC_BIND"
 
-    def support(self, a: type, b: type) -> type:
+    def support(self, types: list[type]) -> type:
         support_entry = supportted_types[self]
-        if issubclass(a, support_entry[0]) and issubclass(b, support_entry[1]):
-            if issubclass(a, Types.HyperVector):
-                return a
-            elif issubclass(b, Types.HyperVector):
-                return b
-            else:
-                return support_entry[2]
+        if self == Operator.BUNDlE:
+            # bundle takes variable number of arguments
+            for i in range(len(types)):
+                if not issubclass(types[i], Types.HyperVector):
+                    raise Exception("Unsupported type " + str(types[i]) + " for operator " + str(self))
+            return types[0]
         else:
-            raise Exception("Unsupported type combination " + str(a) + " and " + str(b) + " for operator " + str(self))
+            if len(types) != len(support_entry) - 1:
+                raise Exception("Unsupported number of arguments " + str(len(types)) + " for operator " + str(self))
+            for i in range(len(types)):
+                if not issubclass(types[i], support_entry[i]):
+                    raise Exception("Unsupported type " + str(types[i]) + " for operator " + str(self))
+            if issubclass(types[0], Types.HyperVector):
+                return types[0]
+            elif issubclass(types[1], Types.HyperVector):
+                return types[1]
+            else:
+                return support_entry[-1]
     pass
 
 
 supportted_types = {
     Operator.BIND: ((str, Types.HyperVector), (str, Types.HyperVector), Types.HyperVector),
     Operator.UNBIND: ((str, Types.HyperVector), (str, Types.HyperVector), Types.HyperVector),
     Operator.BUNDlE: ((str, Types.HyperVector), (str, Types.HyperVector), Types.HyperVector),
     Operator.PERMUTATION: ((str, Types.HyperVector), (int), Types.HyperVector),
     Operator.FRAC_BIND: ((str, Types.HyperVector), (str, int, float), Types.HyperVector)
 }
 
 
 class Expression:
-    a: Expression | str | int | float | Types.HyperVector
-    aType: type
+    # a: Expression | str | int | float | Types.HyperVector
+    # aType: type
     op: Operator
-    b: Expression | str | int | float | Types.HyperVector
-    bType: type
+    # b: Expression | str | int | float | Types.HyperVector
+    # bType: type
     outType: type
+    operands: list[Expression | str | int | float | Types.HyperVector]
+    types: list[type] = []
 
-    def __init__(self, a: Expression | str | int | float | Types.HyperVector, op: Operator, b: Expression | str | int | float | Types.HyperVector, program: HDProg = None):
-        self.a = a
+    def __init__(self, op: Operator, operands: list[Expression | str | int | float | Types.HyperVector], program: HDProg = None):
         self.op = op
-        self.b = b
+        self.operands = operands
         # parse types
-        if isinstance(a, Expression):
-            self.aType = a.outType
-        elif isinstance(a, str):
-            if program is None:
-                raise Exception("Program is required for symbol type inference")
-            self.aType = program.getSymbolType(a)
-        else:
-            self.aType = type(a)
-        if isinstance(b, Expression):
-            self.bType = b.outType
-        elif isinstance(b, str):
-            if program is None:
-                raise Exception("Program is required for symbol type inference")
-            self.bType = program.getSymbolType(b)
-        else:
-            self.bType = type(b)
+        for i in range(len(operands)):
+            if isinstance(operands[i], Expression):
+                self.types.append(operands[i].outType)
+            elif isinstance(operands[i], str):
+                if program is None:
+                    raise Exception("Program is required for symbol type inference")
+                self.types.append(program.getSymbolType(operands[i]))
+            else:
+                self.types.append(type(operands[i]))
         self.typecheck()
         pass
 
     def __str__(self):
-        return "Expression(" + str(self.a) + " " + str(self.op) + " " + str(self.b) + ")"
+        return "Expression(" + str(self.op) + ", " + str(self.operands) + ")"
     
     def typecheck(self):
-        self.outType = self.op.support(self.aType, self.bType)
+        self.outType = self.op.support(self.types)
         pass
 
     def eval(self, state: HDProgState):
-        if isinstance(self.a, Expression):
-            a = self.a.eval(state)
-        elif isinstance(self.a, str):
-            # type check
-            if self.a not in state.val_table:
-                raise Exception("Symbol " + self.a + " not found")
-            if not issubclass(state.val_table[self.a][1], self.aType):
-                raise Exception("Symbol " + self.a + " is not of type " + str(self.aType))
-            a = state.val_table[self.a][3]
-        else:
-            a = self.a
-        if isinstance(self.b, Expression):
-            b = self.b.eval(state)
-        elif isinstance(self.b, str):
-            # type check
-            if self.b not in state.val_table:
-                raise Exception("Symbol " + self.b + " not found")
-            if not issubclass(state.val_table[self.b][1], self.bType):
-                raise Exception("Symbol " + self.b + " is not of type " + str(self.bType))
-            b = state.val_table[self.b][3]
-        else:
-            b = self.b
-        if self.op == Operator.BIND:
-            return a.bind(b)
-        elif self.op == Operator.UNBIND:
-            return a.unbind(b)
-        elif self.op == Operator.BUNDlE:
-            return a.bundle(b)
-        elif self.op == Operator.PERMUTATION:
-            return a.permutation(b)
-        elif self.op == Operator.FRAC_BIND:
-            return a.frac_bind(b)
+        if not self.op == Operator.BUNDlE:
+            if isinstance(self.operands[0], Expression):
+                self.operands[0] = self.operands[0].eval(state)
+            elif isinstance(self.operands[0], str):
+                # type check
+                if self.operands[0] not in state.val_table:
+                    raise Exception("Symbol " + self.operands[0] + " not found")
+                if not issubclass(state.val_table[self.operands[0]][1], self.types[0]):
+                    raise Exception("Symbol " + self.operands[0] + " is not of type " + str(self.types[0]))
+                self.operands[0] = state.val_table[self.operands[0]][3]
+            if isinstance(self.operands[1], Expression):
+                self.operands[1] = self.operands[1].eval(state)
+            elif isinstance(self.operands[1], str):
+                # type check
+                if self.operands[1] not in state.val_table:
+                    raise Exception("Symbol " + self.operands[1] + " not found")
+                if not issubclass(state.val_table[self.operands[1]][1], self.types[1]):
+                    raise Exception("Symbol " + self.operands[1] + " is not of type " + str(self.types[1]))
+                self.operands[1] = state.val_table[self.operands[1]][3]
+            if self.op == Operator.BIND:
+                return self.operands[0].bind(self.operands[1])
+            elif self.op == Operator.UNBIND:
+                return self.operands[0].unbind(self.operands[1])
+            elif self.op == Operator.PERMUTATION:
+                return self.operands[0].permutation(self.operands[1])
+            elif self.op == Operator.FRAC_BIND:
+                return self.operands[0].frac_bind(self.operands[1])
+            else:
+                raise Exception("Unsupported operator " + str(self.op))
         else:
-            raise Exception("Unsupported operator " + str(self.op))
+            vals = []
+            for i in range(len(self.operands)):
+                if isinstance(self.operands[i], Expression):
+                    vals.append(self.operands[i].eval(state))
+                elif isinstance(self.operands[i], str):
+                    # type check
+                    if self.operands[i] not in state.val_table:
+                        raise Exception("Symbol " + self.operands[i] + " not found")
+                    if not issubclass(state.val_table[self.operands[i]][1], self.types[i]):
+                        raise Exception("Symbol " + self.operands[i] + " is not of type " + str(self.types[i]))
+                    vals.append(state.val_table[self.operands[i]][3])
+                else:
+                    vals.append(self.operands[i])
+            return self.outType.bundle(vals)
     pass
 
 
 Operand = Union[Expression, str, int, float, Types.HyperVector]
 
 
 # Definition of HDProg class
@@ -362,27 +375,27 @@
         if identifier not in self.symbols:
             raise Exception("Symbol " + identifier + " not declared")
         t = self.symbols[identifier][0]
         assert isinstance(t, type)
         return t
     
     def bind(self, a: Operand, b: Operand) -> Expression:
-        return Expression(a, Operator.BIND, b, self)
+        return Expression(Operator.BIND, [a, b], self)
     
     def unbind(self, a: Operand, b: Operand) -> Expression:
-        return Expression(a, Operator.UNBIND, b, self)
+        return Expression(Operator.UNBIND, [a, b], self)
 
-    def bundle(self, a: Operand, b: Operand) -> Expression:
-        return Expression(a, Operator.BUNDlE, b, self)
+    def bundle(self, *operands: Operand) -> Expression:
+        return Expression(Operator.BUNDlE, list(operands), self)
 
     def permutation(self, a: Operand, b: Operand) -> Expression:
-        return Expression(a, Operator.PERMUTATION, b, self)
+        return Expression(Operator.PERMUTATION, [a, b], self)
 
     def frac_bind(self, a: Operand, b: Operand) -> Expression:
-        return Expression(a, Operator.FRAC_BIND, b, self)
+        return Expression(Operator.FRAC_BIND, [a, b], self)
         
     def __str__(self):
         string = ""
         string += "Inputs:\n"
         for k, v in self.inputs.items():
             string += f"\t{k}: {v[0]} dim {v[1]}\n"
         string += "Outputs:\n"
```

### Comparing `hdcc-0.1.0/hdcc/HDTypes.py` & `hdcc-0.2.0/hdcc/HDTypes.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,21 +50,23 @@
     def unbind(self, other: HV_FHRR) -> HV_FHRR:
         # unbind two vectors
         # TODO: check if this is correct
         assert self.dim == other.dim
         data = other.data - self.data
         return HV_FHRR(self.dim, data)
     
-    def bundle(self, other: HV_FHRR) -> HV_FHRR:
-        # bundle two vectors
+    @staticmethod
+    def bundle(vectors: list[HV_FHRR]) -> HV_FHRR:
+        # bundle multiple vectors
         # angles of element addition
         # convert the angles to unit complex exponential then add then convert back to angles
-        assert self.dim == other.dim
-        data = np.angle(np.exp(1j * self.data) + np.exp(1j * other.data))
-        return HV_FHRR(self.dim, data)
+        dim = vectors[0].dim
+        assert all([v.dim == dim for v in vectors])
+        data = np.angle(np.sum(np.exp(1j * np.array([v.data for v in vectors])), axis=0))
+        return HV_FHRR(dim, data)
     
     def frac_bind(self, frac: float) -> HV_FHRR:
         # bind vector with real number
         data = frac * self.data
         return HV_FHRR(self.dim, data)
```

### Comparing `hdcc-0.1.0/PKG-INFO` & `hdcc-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdcc
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: Yifan Yang
 Author-email: yyang29@stanford.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

