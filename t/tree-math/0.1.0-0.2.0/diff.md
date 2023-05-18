# Comparing `tmp/tree-math-0.1.0.tar.gz` & `tmp/tree-math-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tree-math-0.1.0.tar", last modified: Tue Dec 28 23:14:23 2021, max compression
+gzip compressed data, was "tree-math-0.2.0.tar", last modified: Thu May 18 17:47:46 2023, max compression
```

## Comparing `tree-math-0.1.0.tar` & `tree-math-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2021-12-28 23:14:23.000000 tree-math-0.1.0/
--rw-r--r--   0 shoyer   (365133) eng       (5000)      271 2021-12-28 23:14:23.000000 tree-math-0.1.0/PKG-INFO
--rw-r--r--   0 shoyer   (365133) eng       (5000)     2513 2021-12-28 23:13:05.000000 tree-math-0.1.0/README.md
--rw-r--r--   0 shoyer   (365133) eng       (5000)       38 2021-12-28 23:14:23.000000 tree-math-0.1.0/setup.cfg
--rw-r--r--   0 shoyer   (365133) eng       (5000)     1197 2021-12-28 23:13:05.000000 tree-math-0.1.0/setup.py
-drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2021-12-28 23:14:23.000000 tree-math-0.1.0/tree_math/
--rw-r--r--   0 shoyer   (365133) eng       (5000)      831 2021-12-28 23:13:05.000000 tree-math-0.1.0/tree_math/__init__.py
-drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2021-12-28 23:14:23.000000 tree-math-0.1.0/tree_math/_src/
--rw-r--r--   0 shoyer   (365133) eng       (5000)        0 2021-12-28 20:41:50.000000 tree-math-0.1.0/tree_math/_src/__init__.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     2720 2021-12-28 20:41:50.000000 tree-math-0.1.0/tree_math/_src/arg_util.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     2686 2021-12-28 20:41:50.000000 tree-math-0.1.0/tree_math/_src/func_wrappers.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     2846 2021-12-28 20:41:50.000000 tree-math-0.1.0/tree_math/_src/func_wrappers_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     1350 2021-12-28 20:41:50.000000 tree-math-0.1.0/tree_math/_src/numpy.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     2956 2021-12-28 20:41:50.000000 tree-math-0.1.0/tree_math/_src/numpy_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     1939 2021-12-28 20:41:50.000000 tree-math-0.1.0/tree_math/_src/test_util.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     7063 2021-12-28 20:41:50.000000 tree-math-0.1.0/tree_math/_src/vector.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     5635 2021-12-28 20:41:50.000000 tree-math-0.1.0/tree_math/_src/vector_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     2681 2021-12-28 23:13:05.000000 tree-math-0.1.0/tree_math/integration_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)      836 2021-12-28 20:41:50.000000 tree-math-0.1.0/tree_math/numpy.py
-drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2021-12-28 23:14:23.000000 tree-math-0.1.0/tree_math.egg-info/
--rw-r--r--   0 shoyer   (365133) eng       (5000)      271 2021-12-28 23:14:23.000000 tree-math-0.1.0/tree_math.egg-info/PKG-INFO
--rw-r--r--   0 shoyer   (365133) eng       (5000)      512 2021-12-28 23:14:23.000000 tree-math-0.1.0/tree_math.egg-info/SOURCES.txt
--rw-r--r--   0 shoyer   (365133) eng       (5000)        1 2021-12-28 23:14:23.000000 tree-math-0.1.0/tree_math.egg-info/dependency_links.txt
--rw-r--r--   0 shoyer   (365133) eng       (5000)       53 2021-12-28 23:14:23.000000 tree-math-0.1.0/tree_math.egg-info/requires.txt
--rw-r--r--   0 shoyer   (365133) eng       (5000)       10 2021-12-28 23:14:23.000000 tree-math-0.1.0/tree_math.egg-info/top_level.txt
+drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2023-05-18 17:47:46.271663 tree-math-0.2.0/
+-rw-r--r--   0 shoyer   (365133) eng       (5000)    11358 2021-12-28 20:41:50.000000 tree-math-0.2.0/LICENSE
+-rw-r--r--   0 shoyer   (365133) eng       (5000)      314 2023-05-18 17:47:46.270984 tree-math-0.2.0/PKG-INFO
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     5943 2023-05-12 02:20:53.000000 tree-math-0.2.0/README.md
+-rw-r--r--   0 shoyer   (365133) eng       (5000)       38 2023-05-18 17:47:46.271714 tree-math-0.2.0/setup.cfg
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     1243 2023-05-18 17:46:01.000000 tree-math-0.2.0/setup.py
+drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2023-05-18 17:47:46.267791 tree-math-0.2.0/tree_math/
+-rw-r--r--   0 shoyer   (365133) eng       (5000)      886 2023-05-12 02:20:53.000000 tree-math-0.2.0/tree_math/__init__.py
+drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2023-05-18 17:47:46.270744 tree-math-0.2.0/tree_math/_src/
+-rw-r--r--   0 shoyer   (365133) eng       (5000)        0 2021-12-28 20:41:50.000000 tree-math-0.2.0/tree_math/_src/__init__.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     2720 2021-12-28 20:41:50.000000 tree-math-0.2.0/tree_math/_src/arg_util.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     2686 2021-12-28 20:41:50.000000 tree-math-0.2.0/tree_math/_src/func_wrappers.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     2846 2021-12-28 20:41:50.000000 tree-math-0.2.0/tree_math/_src/func_wrappers_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     1350 2021-12-28 20:41:50.000000 tree-math-0.2.0/tree_math/_src/numpy.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     2961 2022-03-04 04:00:56.000000 tree-math-0.2.0/tree_math/_src/numpy_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     2408 2023-05-12 02:20:53.000000 tree-math-0.2.0/tree_math/_src/structs.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     3639 2023-05-12 02:20:53.000000 tree-math-0.2.0/tree_math/_src/structs_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     1939 2021-12-28 20:41:50.000000 tree-math-0.2.0/tree_math/_src/test_util.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     7209 2023-05-12 02:20:53.000000 tree-math-0.2.0/tree_math/_src/vector.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     6211 2023-05-12 02:20:53.000000 tree-math-0.2.0/tree_math/_src/vector_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     2681 2021-12-28 23:13:05.000000 tree-math-0.2.0/tree_math/integration_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)      836 2021-12-28 20:41:50.000000 tree-math-0.2.0/tree_math/numpy.py
+drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2023-05-18 17:47:46.268569 tree-math-0.2.0/tree_math.egg-info/
+-rw-r--r--   0 shoyer   (365133) eng       (5000)      314 2023-05-18 17:47:45.000000 tree-math-0.2.0/tree_math.egg-info/PKG-INFO
+-rw-r--r--   0 shoyer   (365133) eng       (5000)      577 2023-05-18 17:47:46.000000 tree-math-0.2.0/tree_math.egg-info/SOURCES.txt
+-rw-r--r--   0 shoyer   (365133) eng       (5000)        1 2023-05-18 17:47:46.000000 tree-math-0.2.0/tree_math.egg-info/dependency_links.txt
+-rw-r--r--   0 shoyer   (365133) eng       (5000)       47 2023-05-18 17:47:46.000000 tree-math-0.2.0/tree_math.egg-info/requires.txt
+-rw-r--r--   0 shoyer   (365133) eng       (5000)       10 2023-05-18 17:47:46.000000 tree-math-0.2.0/tree_math.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tree-math-0.1.0/setup.py` & `tree-math-0.2.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 # ==============================================================================
 """Setup for tree-math."""
 import setuptools
 
 
 base_requires = [
     'jax',
-    'numpy',
 ]
 tests_requires = [
     'absl-py',
     'jaxlib',
     'numpy>=1.17',
     'pytest',
 ]
 
 setuptools.setup(
     name='tree-math',
-    version='0.1.0 ',
+    description='Mathematical operations for JAX pytrees',
+    version='0.2.0 ',
     license='Apache 2.0',
     author='Google LLC',
     author_email='noreply@google.com',
     install_requires=base_requires,
     extras_require={
         'tests': tests_requires,
     },
```

### Comparing `tree-math-0.1.0/tree_math/__init__.py` & `tree-math-0.2.0/tree_math/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,11 +16,12 @@
 # pylint: disable=g-multiple-import
 # pylint: disable=unused-import
 
 from tree_math._src.func_wrappers import (
     wrap,
     unwrap,
 )
-from tree_math._src.vector import Vector
+from tree_math._src.structs import struct
+from tree_math._src.vector import Vector, VectorMixin
 import tree_math.numpy
 
-__version__ = '0.1.0'
+__version__ = '0.2.0'
```

### Comparing `tree-math-0.1.0/tree_math/_src/arg_util.py` & `tree-math-0.2.0/tree_math/_src/arg_util.py`

 * *Files identical despite different names*

### Comparing `tree-math-0.1.0/tree_math/_src/func_wrappers.py` & `tree-math-0.2.0/tree_math/_src/func_wrappers.py`

 * *Files identical despite different names*

### Comparing `tree-math-0.1.0/tree_math/_src/func_wrappers_test.py` & `tree-math-0.2.0/tree_math/_src/func_wrappers_test.py`

 * *Files identical despite different names*

### Comparing `tree-math-0.1.0/tree_math/_src/numpy.py` & `tree-math-0.2.0/tree_math/_src/numpy.py`

 * *Files identical despite different names*

### Comparing `tree-math-0.1.0/tree_math/_src/numpy_test.py` & `tree-math-0.2.0/tree_math/_src/numpy_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     self.assertTreeEqual(actual, expected, check_dtypes=True)
 
   def test_where_all_scalars(self):
     expected = 1
     actual = tnp.where(True, 1, 2)
     self.assertTreeEqual(actual, expected, check_dtypes=False)
     with self.assertRaisesRegex(
-        TypeError, "non-tree_math.Vector argument is not a scalar",
+        TypeError, "non-tree_math.VectorMixin argument is not a scalar",
     ):
       tnp.where(True, jnp.array([1, 2]), 3)
 
   def test_zeros_like(self):
     x = jnp.array([1, 2])
     expected = tm.Vector({"a": jnp.zeros_like(x)})
     actual = tnp.zeros_like(tm.Vector({"a": x}))
```

### Comparing `tree-math-0.1.0/tree_math/_src/test_util.py` & `tree-math-0.2.0/tree_math/_src/test_util.py`

 * *Files identical despite different names*

### Comparing `tree-math-0.1.0/tree_math/_src/vector.py` & `tree-math-0.2.0/tree_math/_src/vector.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,26 +49,28 @@
     return f(*args3)
   args2 = tuple(x for i, x in enumerate(args) if i not in static_argnums)
   return g, args2
 
 
 def broadcasting_map(func, *args):
   """Like tree_map, but scalar arguments are broadcast to all leaves."""
-  static_argnums = [i for i, x in enumerate(args) if not isinstance(x, Vector)]
+  static_argnums = [
+      i for i, x in enumerate(args) if not isinstance(x, VectorMixin)
+  ]
   func2, vector_args = _argnums_partial(func, args, static_argnums)
   for arg in args:
-    if not isinstance(arg, Vector):
+    if not isinstance(arg, VectorMixin):
       shape = jnp.shape(arg)
       if shape:
         raise TypeError(
-            f"non-tree_math.Vector argument is not a scalar: {arg!r}"
+            f"non-tree_math.VectorMixin argument is not a scalar: {arg!r}"
         )
   if not vector_args:
     return func2()  # result is a scalar
-  _flatten_together(*[arg.tree for arg in vector_args])  # check shapes
+  _flatten_together(*[arg for arg in vector_args])  # check shapes
   return tree_util.tree_map(func2, *vector_args)
 
 
 def _binary_method(func, name):
   """Implement a forward binary method, e.g., __add__."""
   def wrapper(self, other):
     return broadcasting_map(func, self, other)
@@ -108,51 +110,32 @@
     left: left argument.
     right: right argument.
     precision: precision.
 
   Returns:
     Resulting dot product (scalar).
   """
-  if not isinstance(left, Vector) or not isinstance(right, Vector):
-    raise TypeError("matmul arguments must both be tree_math.Vector objects")
+  if not isinstance(left, VectorMixin) or not isinstance(right, VectorMixin):
+    raise TypeError(
+        "matmul arguments must both be tree_math.VectorMixin objects")
 
   def _vector_dot(a, b):
     return jnp.dot(jnp.ravel(a), jnp.ravel(b), precision=precision)
 
-  (left_values, right_values), _ = _flatten_together(left.tree, right.tree)
+  (left_values, right_values), _ = _flatten_together(left, right)
   parts = map(_vector_dot, left_values, right_values)
   return functools.reduce(operator.add, parts)
 
 
-@tree_util.register_pytree_node_class
-class Vector:
-  """A wrapper for treating an arbitrary pytree as a 1D vector."""
-
-  def __init__(self, tree):
-    self._tree = tree
-
-  @property
-  def tree(self):
-    return self._tree
-
-  # TODO(shoyer): consider casting to a common dtype?
-
-  def __repr__(self):
-    return f"tree_math.Vector({self._tree!r})"
-
-  def tree_flatten(self):
-    return (self.tree,), None
-
-  @classmethod
-  def tree_unflatten(cls, _, args):
-    return cls(*args)
+class VectorMixin:
+  """A mixin class that adds a 1D vector-like behaviour to any custom pytree class."""
 
   @property
   def size(self):
-    values = tree_util.tree_leaves(self.tree)
+    values = tree_util.tree_leaves(self)
     return sum(jnp.size(value) for value in values)
 
   def __len__(self):
     return self.size
 
   @property
   def shape(self):
@@ -160,15 +143,15 @@
 
   @property
   def ndim(self):
     return 1
 
   @property
   def dtype(self):
-    values = tree_util.tree_leaves(self.tree)
+    values = tree_util.tree_leaves(self)
     return jnp.result_type(*values)
 
   # comparison
   __lt__ = _binary_method(operator.lt, "lt")
   __le__ = _binary_method(operator.le, "le")
   __eq__ = _binary_method(operator.eq, "eq")
   __ne__ = _binary_method(operator.ne, "ne")
@@ -221,7 +204,31 @@
   def min(self):
     parts = map(jnp.min, tree_util.tree_leaves(self))
     return jnp.asarray(list(parts)).min()
 
   def max(self):
     parts = map(jnp.max, tree_util.tree_leaves(self))
     return jnp.asarray(list(parts)).max()
+
+
+@tree_util.register_pytree_node_class
+class Vector(VectorMixin):
+  """A wrapper for treating an arbitrary pytree as a 1D vector."""
+
+  def __init__(self, tree):
+    self._tree = tree
+
+  @property
+  def tree(self):
+    return self._tree
+
+  # TODO(shoyer): consider casting to a common dtype?
+
+  def __repr__(self):
+    return f"tree_math.Vector({self._tree!r})"
+
+  def tree_flatten(self):
+    return (self._tree,), None
+
+  @classmethod
+  def tree_unflatten(cls, _, args):
+    return cls(*args)
```

### Comparing `tree-math-0.1.0/tree_math/_src/vector_test.py` & `tree-math-0.2.0/tree_math/_src/vector_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 
 import operator
 
 from absl.testing import absltest
 from absl.testing import parameterized
 from jax import tree_util
 import jax.numpy as jnp
+import numpy as np
 import tree_math as tm
 from tree_math._src import test_util
-import numpy as np
 
 # pylint: disable=g-complex-comprehension
 
 
 class VectorTest(test_util.TestCase):
 
   def test_vector(self):
@@ -54,15 +54,15 @@
 
   def test_arithmetic_with_scalar(self):
     vector = tm.Vector({"a": 0, "b": jnp.array([1, 2])})
     expected = tm.Vector({"a": 1, "b": jnp.array([2, 3])})
     self.assertTreeEqual(vector + 1, expected, check_dtypes=True)
     self.assertTreeEqual(1 + vector, expected, check_dtypes=True)
     with self.assertRaisesRegex(
-        TypeError, "non-tree_math.Vector argument is not a scalar",
+        TypeError, "non-tree_math.VectorMixin argument is not a scalar",
     ):
       vector + jnp.ones((3,))  # pylint: disable=expression-not-assigned
 
   @parameterized.named_parameters(*(
       {"testcase_name": op.__name__, "op": op}
       for op in [
           operator.add,
@@ -119,15 +119,16 @@
     actual = vector1 @ vector2
     self.assertAllClose(actual, expected)
 
     actual = vector1.dot(vector2)
     self.assertAllClose(actual, expected)
 
     with self.assertRaisesRegex(
-        TypeError, "matmul arguments must both be tree_math.Vector objects",
+        TypeError,
+        "matmul arguments must both be tree_math.VectorMixin objects",
     ):
       vector1 @ jnp.ones((7,))  # pylint: disable=expression-not-assigned
 
   # TODO(shoyer): test comparisons and bitwise ops
 
   def test_conj(self):
     vector = tm.Vector({"a": jnp.array([1, 1j])})
@@ -144,10 +145,33 @@
 
   def test_sum_mean_min_max(self):
     vector = tm.Vector({"a": 1, "b": jnp.array([2, 3, 4])})
     self.assertTreeEqual(vector.sum(), 10, check_dtypes=False)
     self.assertTreeEqual(vector.min(), 1, check_dtypes=False)
     self.assertTreeEqual(vector.max(), 4, check_dtypes=False)
 
+  def test_custom_class(self):
+
+    @tree_util.register_pytree_node_class
+    class CustomVector(tm.VectorMixin):
+
+      def __init__(self, a: int, b: float):
+        self.a = a
+        self.b = b
+
+      def tree_flatten(self):
+        return (self.a, self.b), None
+
+      @classmethod
+      def tree_unflatten(cls, _, args):
+        return cls(*args)
+
+    v1 = CustomVector(1, 2.0)
+    v2 = v1 + 3
+    self.assertTreeEqual(v2, CustomVector(4, 5.0), check_dtypes=True)
+
+    v3 = v2 + v1
+    self.assertTreeEqual(v3, CustomVector(5, 7.0), check_dtypes=True)
+
 
 if __name__ == "__main__":
   absltest.main()
```

### Comparing `tree-math-0.1.0/tree_math/integration_test.py` & `tree-math-0.2.0/tree_math/integration_test.py`

 * *Files identical despite different names*

### Comparing `tree-math-0.1.0/tree_math/numpy.py` & `tree-math-0.2.0/tree_math/numpy.py`

 * *Files identical despite different names*

### Comparing `tree-math-0.1.0/tree_math.egg-info/SOURCES.txt` & `tree-math-0.2.0/tree_math.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 tree_math/__init__.py
 tree_math/integration_test.py
 tree_math/numpy.py
 tree_math.egg-info/PKG-INFO
 tree_math.egg-info/SOURCES.txt
@@ -10,10 +11,12 @@
 tree_math.egg-info/top_level.txt
 tree_math/_src/__init__.py
 tree_math/_src/arg_util.py
 tree_math/_src/func_wrappers.py
 tree_math/_src/func_wrappers_test.py
 tree_math/_src/numpy.py
 tree_math/_src/numpy_test.py
+tree_math/_src/structs.py
+tree_math/_src/structs_test.py
 tree_math/_src/test_util.py
 tree_math/_src/vector.py
 tree_math/_src/vector_test.py
```

