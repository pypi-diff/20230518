# Comparing `tmp/yarrow_diagrams-0.0.1.tar.gz` & `tmp/yarrow_diagrams-0.0.2.tar.gz`

## Comparing `yarrow_diagrams-0.0.1.tar` & `yarrow_diagrams-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.1/yarrow/__init__.py
--rw-r--r--   0        0        0     8151 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.1/yarrow/bipartite_multigraph.py
--rw-r--r--   0        0        0    11906 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.1/yarrow/diagram.py
--rw-r--r--   0        0        0    12499 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.1/yarrow/finite_function.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.1/yarrow/array/__init__.py
--rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.1/yarrow/array/numpy.py
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.1/yarrow/decompose/frobenius.py
--rw-r--r--   0        0        0     6135 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.1/yarrow/functor/functor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.1/yarrow/segmented/__init__.py
--rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.1/yarrow/segmented/finite_function.py
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.1/yarrow/segmented/operations.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.1/LICENSE
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.1/README.md
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2/yarrow/__init__.py
+-rw-r--r--   0        0        0     8173 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2/yarrow/bipartite_multigraph.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2/yarrow/cupy.py
+-rw-r--r--   0        0        0    11961 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2/yarrow/diagram.py
+-rw-r--r--   0        0        0    12537 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2/yarrow/finite_function.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2/yarrow/array/__init__.py
+-rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2/yarrow/array/cupy.py
+-rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2/yarrow/array/numpy.py
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2/yarrow/decompose/frobenius.py
+-rw-r--r--   0        0        0     6135 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2/yarrow/functor/functor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2/yarrow/segmented/__init__.py
+-rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2/yarrow/segmented/finite_function.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2/yarrow/segmented/operations.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2/README.md
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2/PKG-INFO
```

### Comparing `yarrow_diagrams-0.0.1/yarrow/bipartite_multigraph.py` & `yarrow_diagrams-0.0.2/yarrow/bipartite_multigraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-""" The internal wiring of string diagrams is represented as bipartite multigraphs,
-whose edge labels are *port numbers*, and whose node labels are either generating objects
-or generating operations.
+"""A representation of the "internal wiring" of string diagrams.
+Bipartite multigraphs have edge labels corresponding to the "ports" of
+operations, and node labels either generating objects or generating operations
+of a signature Σ.
 
 As with other classes, these graphs are implemented with an abstract base class
 :py:class:`AbstractBipartiteMultigraph`,
 whose concrete instantiations choose a backend.
 For example, :py:class:`BipartiteMultigraph` are backed by numpy arrays.
 """
 from dataclasses import dataclass
@@ -156,15 +157,15 @@
         Returns:
             The coproduct ``self + g``.
         """
         # check signatures match
         assert f.wn.target == g.wn.target
         assert f.xn.target == g.xn.target
 
-        return BipartiteMultigraph(
+        return type(f)(
             # Tensor product of data
             wi=f.wi @ g.wi,
             wo=f.wo @ g.wo,
             xi=f.xi @ g.xi,
             xo=f.xo @ g.xo,
             # Coproduct of attributes
             wn=f.wn + g.wn,
```

### Comparing `yarrow_diagrams-0.0.1/yarrow/diagram.py` & `yarrow_diagrams-0.0.2/yarrow/diagram.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""".. _Diagram:
+"""Diagrams are the main datastructure of yarrow, and represent string diagrams.
 
 The :py:class:`AbstractDiagram` is the main datastructure of yarrow.
 It represents a string diagram as a *cospan of bipartite multigraphs*.
 For example, the diagram below left is represented internally below right:
 
 .. image:: /string-diagram-side-by-side.svg
    :scale: 150%
@@ -165,15 +165,15 @@
             AbstractDiagram: The symmetry diagram `σ : A ● B → B ● A`.
         """
         assert xn.source == 0
         wn = wn_A + wn_B
         s = cls._Fun.identity(wn.source)
         t = cls._Fun.twist(wn_A.source, wn_B.source)
         G = cls._Graph.discrete(wn, xn)
-        return Diagram(s, t, G)
+        return cls(s, t, G)
 
     @classmethod
     def spider(cls,
                s: AbstractFiniteFunction,
                t: AbstractFiniteFunction,
                w: AbstractFiniteFunction,
                x: AbstractFiniteFunction):
@@ -188,23 +188,23 @@
         Returns:
             AbstractDiagram: A frobenius spider with `S` inputs and `T` outputs.
         """
         assert x.source == 0
         assert w.source == s.target
         assert w.source == t.target
         G = cls._Graph.discrete(w, x)
-        return Diagram(s, t, G)
+        return cls(s, t, G)
 
     def dagger(self):
         """Swap the *source* and *target* maps of the diagram.
 
         Returns:
             AbstractDiagram: The dagger functor applied to this diagram.
         """
-        return Diagram(self.t, self.s, self.G)
+        return type(self)(self.t, self.s, self.G)
 
     @classmethod
     def singleton(cls, a: AbstractFiniteFunction, b: AbstractFiniteFunction, xn: AbstractFiniteFunction):
         """ Construct a diagram consisting of a single operation (Definition 4.9, :cite:p:`dpafsd`).
 
         Args:
             x: A single operation represented as an AbstractFiniteFunction of type `1 → Σ₁`
@@ -261,16 +261,15 @@
 
         Args:
             g(AbstractDiagram): An arbitrary diagram
 
         Returns:
             AbstractDiagram: The tensor product of this diagram with `g`.
         """
-
-        return Diagram(
+        return type(f)(
             s = f.s @ g.s,
             t = f.t @ g.t,
             G = f.G @ g.G)
 
     def __matmul__(f, g):
         """ Shorthand for :py:meth:`yarrow.Diagram.tensor`.
         f @ g == f.tensor(g)
@@ -295,15 +294,15 @@
         Raises:
             AssertionError: If `g.type[0] != f.type[1]`
         """
 
         assert f.type[1] == g.type[0]
         h = f @ g
         q = f.t.inject0(g.G.W).coequalizer(g.s.inject1(f.G.W))
-        return Diagram(
+        return type(f)(
             s = f.s.inject0(g.G.W) >> q,
             t = g.t.inject1(f.G.W) >> q,
             G = h.G.coequalize_wires(q))
 
     def __rshift__(f, g):
         return f.compose(g)
 
@@ -335,15 +334,15 @@
 
         i0 = Fun.inj0(Ki, Ko)
         i1 = Fun.inj1(Ki, Ko)
 
         return cls(
             s = i0,
             t = i1,
-            G = Diagram._Graph(
+            G = cls._Graph(
                 xn = xn,
                 # Tensor product of terminal maps
                 # e.g. 1 1 1 | 2 2 | 3 3 3 3 ...
                 xi = Fun(xn.source, Array.repeat(r, s_type.sources.table)),
                 xo = Fun(xn.source, Array.repeat(r, t_type.sources.table)),
                 # Coproduct of ι₀ maps
                 # e.g. 0 1 2 | 0 1 | 0 1 2 3 ...
```

### Comparing `yarrow_diagrams-0.0.1/yarrow/finite_function.py` & `yarrow_diagrams-0.0.2/yarrow/finite_function.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-"""All yarrow datastructures are ultimately built from finite functions.
+"""An implementation of finite functions as arrays.
+All yarrow datastructures are ultimately built from finite functions.
 For an overview, see :cite:t:`dpafsd`, Section 2.2.2.
 
 Finite functions can be thought of as a thin wrapper around integer arrays whose
 elements are within a specified range.
 Here's an example of contructing a finite function:
 
 >>> print(FiniteFunction(3, [0, 1, 2, 0]))
@@ -98,15 +99,15 @@
         Args:
             n(int): The object of which to return the identity map
 
         Returns:
             AbstractFiniteFunction: Identity map at n
         """
         assert n >= 0
-        return FiniteFunction(n, cls._Array.arange(0, n, dtype=DTYPE))
+        return cls(n, cls._Array.arange(0, n, dtype=DTYPE))
 
     # Compute (f ; g), i.e., the function x → g(f(x))
     def compose(f: 'AbstractFiniteFunction', g: 'AbstractFiniteFunction'):
         """Compose this finite function with another
 
         Args:
             g: A FiniteFunction for which self.target == g.source
```

### Comparing `yarrow_diagrams-0.0.1/yarrow/decompose/frobenius.py` & `yarrow_diagrams-0.0.2/yarrow/decompose/frobenius.py`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.1/yarrow/functor/functor.py` & `yarrow_diagrams-0.0.2/yarrow/functor/functor.py`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.1/yarrow/segmented/finite_function.py` & `yarrow_diagrams-0.0.2/yarrow/segmented/finite_function.py`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.1/yarrow/segmented/operations.py` & `yarrow_diagrams-0.0.2/yarrow/segmented/operations.py`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.1/LICENSE` & `yarrow_diagrams-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.1/pyproject.toml` & `yarrow_diagrams-0.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "yarrow-diagrams"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Paul Wilson", email="paul@statusfailed.com" }
 ]
 description = "yarrow diagrams"
 readme = "README.md"
 requires-python = ">= 3.7"
 classifiers = [
@@ -15,14 +15,15 @@
   "numpy~=1.23.3",
   "scipy~=1.9.0",
 ]
 
 [project.urls]
 "Homepage" = "https://yarrow.id"
 "Github" = "https://github.com/yarrow-id/diagrams/"
+"Documentation" = "https://yarrow-diagrams.readthedocs.io/"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build]
 packages = ["yarrow"]
```

