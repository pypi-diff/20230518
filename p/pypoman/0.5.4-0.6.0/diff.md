# Comparing `tmp/pypoman-0.5.4.tar.gz` & `tmp/pypoman-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pypoman-0.5.4.tar", last modified: Mon Nov  5 17:23:03 2018, max compression
+gzip compressed data, was "pypoman-0.6.0.tar", last modified: Thu May 18 15:11:34 2023, max compression
```

## Comparing `pypoman-0.5.4.tar` & `pypoman-0.6.0.tar`

### file list

```diff
@@ -1,21 +1,28 @@
-drwxrwxr-x   0 tastalian  (1000) tastalian  (1000)        0 2018-11-05 17:23:03.000000 pypoman-0.5.4/
-drwxrwxr-x   0 tastalian  (1000) tastalian  (1000)        0 2018-11-05 17:23:03.000000 pypoman-0.5.4/pypoman.egg-info/
--rw-rw-r--   0 tastalian  (1000) tastalian  (1000)     4567 2018-11-05 17:23:03.000000 pypoman-0.5.4/pypoman.egg-info/PKG-INFO
--rw-rw-r--   0 tastalian  (1000) tastalian  (1000)        8 2018-11-05 17:23:03.000000 pypoman-0.5.4/pypoman.egg-info/top_level.txt
--rw-rw-r--   0 tastalian  (1000) tastalian  (1000)      345 2018-11-05 17:23:03.000000 pypoman-0.5.4/pypoman.egg-info/SOURCES.txt
--rw-rw-r--   0 tastalian  (1000) tastalian  (1000)       16 2018-11-05 17:23:03.000000 pypoman-0.5.4/pypoman.egg-info/requires.txt
--rw-rw-r--   0 tastalian  (1000) tastalian  (1000)        1 2018-11-05 17:23:03.000000 pypoman-0.5.4/pypoman.egg-info/dependency_links.txt
--rw-rw-r--   0 tastalian  (1000) tastalian  (1000)       38 2018-11-05 17:23:03.000000 pypoman-0.5.4/setup.cfg
--rw-rw-r--   0 tastalian  (1000) tastalian  (1000)     4920 2018-11-05 17:22:31.000000 pypoman-0.5.4/setup.py
--rw-rw-r--   0 tastalian  (1000) tastalian  (1000)     4567 2018-11-05 17:23:03.000000 pypoman-0.5.4/PKG-INFO
--rw-rw-r--   0 tastalian  (1000) tastalian  (1000)     3484 2018-11-05 17:18:33.000000 pypoman-0.5.4/README.md
-drwxrwxr-x   0 tastalian  (1000) tastalian  (1000)        0 2018-11-05 17:23:03.000000 pypoman-0.5.4/pypoman/
--rw-rw-r--   0 tastalian  (1000) tastalian  (1000)     7586 2018-11-05 14:38:02.000000 pypoman-0.5.4/pypoman/projection.py
--rw-rw-r--   0 tastalian  (1000) tastalian  (1000)     1833 2018-04-17 16:03:41.000000 pypoman-0.5.4/pypoman/misc.py
--rw-rw-r--   0 tastalian  (1000) tastalian  (1000)     3096 2018-04-17 16:23:57.000000 pypoman-0.5.4/pypoman/lp.py
--rw-rw-r--   0 tastalian  (1000) tastalian  (1000)     5063 2018-04-17 16:23:30.000000 pypoman-0.5.4/pypoman/intersection.py
--rw-rw-r--   0 tastalian  (1000) tastalian  (1000)     2128 2018-04-17 16:22:30.000000 pypoman-0.5.4/pypoman/polyhedron.py
--rw-rw-r--   0 tastalian  (1000) tastalian  (1000)     5201 2018-06-04 14:57:44.000000 pypoman-0.5.4/pypoman/polygon.py
--rw-rw-r--   0 tastalian  (1000) tastalian  (1000)     6987 2018-11-05 14:37:47.000000 pypoman-0.5.4/pypoman/bretl.py
--rw-rw-r--   0 tastalian  (1000) tastalian  (1000)     3949 2018-05-02 11:01:55.000000 pypoman-0.5.4/pypoman/duality.py
--rw-rw-r--   0 tastalian  (1000) tastalian  (1000)     1624 2018-06-04 14:59:34.000000 pypoman-0.5.4/pypoman/__init__.py
+-rw-r--r--   0        0        0     2742 2023-05-18 14:46:36.317124 pypoman-0.6.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0       80 2023-05-18 13:23:11.734357 pypoman-0.6.0/.gitignore
+-rw-r--r--   0        0        0      681 2023-05-18 14:47:12.769698 pypoman-0.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0    35141 2021-02-06 12:59:19.279343 pypoman-0.6.0/LICENSE
+-rw-r--r--   0        0        0     4241 2022-05-30 20:21:12.028658 pypoman-0.6.0/README.md
+-rw-r--r--   0        0        0        6 2021-02-06 12:59:19.279343 pypoman-0.6.0/doc/.gitignore
+-rw-r--r--   0        0        0     1531 2023-02-02 13:58:26.059716 pypoman-0.6.0/doc/Makefile
+-rw-r--r--   0        0        0     8782 2021-02-06 13:15:20.729613 pypoman-0.6.0/doc/src/conf.py
+-rw-r--r--   0        0        0      956 2021-10-13 09:23:53.563423 pypoman-0.6.0/doc/src/index.rst
+-rw-r--r--   0        0        0     1505 2021-10-13 09:35:52.660876 pypoman-0.6.0/examples/point_to_polytope_projection.py
+-rw-r--r--   0        0        0     1678 2021-10-13 09:35:29.380588 pypoman-0.6.0/examples/polytope_projection.py
+-rw-r--r--   0        0        0     2231 2021-10-13 09:33:53.575393 pypoman-0.6.0/examples/vertex_enumeration.py
+-rw-r--r--   0        0        0     1776 2023-05-18 14:35:26.271202 pypoman-0.6.0/pypoman/__init__.py
+-rw-r--r--   0        0        0     9426 2023-05-18 14:50:21.580701 pypoman-0.6.0/pypoman/bretl.py
+-rw-r--r--   0        0        0     4848 2023-05-18 14:40:00.339074 pypoman-0.6.0/pypoman/duality.py
+-rw-r--r--   0        0        0     5362 2023-05-18 14:35:05.898930 pypoman-0.6.0/pypoman/intersection.py
+-rw-r--r--   0        0        0     3386 2023-05-18 14:03:11.969183 pypoman-0.6.0/pypoman/lp.py
+-rw-r--r--   0        0        0     1876 2023-05-18 14:04:25.612560 pypoman-0.6.0/pypoman/misc.py
+-rw-r--r--   0        0        0     5655 2023-05-18 14:34:22.334358 pypoman-0.6.0/pypoman/polygon.py
+-rw-r--r--   0        0        0     2234 2023-05-18 13:47:44.860925 pypoman-0.6.0/pypoman/polyhedron.py
+-rw-r--r--   0        0        0     8769 2023-05-18 13:33:01.896412 pypoman-0.6.0/pypoman/projection.py
+-rw-r--r--   0        0        0     1846 2023-05-18 14:25:52.109030 pypoman-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       59 2023-05-18 13:15:14.165396 pypoman-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0     1403 2023-05-18 13:22:28.054613 pypoman-0.6.0/tests/test_halfspace_enumeration.py
+-rw-r--r--   0        0        0     2407 2023-05-18 13:21:27.266974 pypoman-0.6.0/tests/test_vertex_enumeration.py
+-rw-r--r--   0        0        0     1250 2023-05-18 14:48:25.290846 pypoman-0.6.0/tox.ini
+-rw-r--r--   0        0        0      634 1970-01-01 00:00:00.000000 pypoman-0.6.0/setup.py
+-rw-r--r--   0        0        0     5680 1970-01-01 00:00:00.000000 pypoman-0.6.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pypoman-0.5.4/setup.py` & `pypoman-0.6.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,143 +1,118 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-#
-# Copyright (C) 2018 Stephane Caron <stephane.caron@lirmm.fr>
-#
-# This file is part of pypoman.
-#
-# pypoman is free software: you can redistribute it and/or modify it under the
-# terms of the GNU Lesser General Public License as published by the Free
-# Software Foundation, either version 3 of the License, or (at your option) any
-# later version.
-#
-# pypoman is distributed in the hope that it will be useful, but WITHOUT ANY
-# WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
-# A PARTICULAR PURPOSE.  See the GNU Lesser General Public License for more
-# details.
-#
-# You should have received a copy of the GNU Lesser General Public License
-# along with pypoman. If not, see <http://www.gnu.org/licenses/>.
-
-import os
-
-from setuptools import setup
-
-classifiers = """\
-Development Status :: 5 - Production/Stable
-License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Intended Audience :: Developers
-Intended Audience :: Science/Research
-Topic :: Scientific/Engineering :: Mathematics
-Programming Language :: Python
-Programming Language :: Python :: 2
-Programming Language :: Python :: 3
-Operating System :: OS Independent"""
-
-links = [
-    'https://en.wikipedia.org/wiki/Convex_polyhedron',
-    'https://scaron.info/doc/pypoman/index.html#module-pypoman.projection',
-    'https://scaron.info/doc/pypoman/index.html#module-pypoman.duality',
-    'https://scaron.info/doc/pypoman/index.html#chebyshev-center',
-    'https://scaron.info/doc/pypoman/']
-
-long_description = """\
-This library implements common operations over `convex polyhedra <%s>`_ such
-as `polytope projection <%s>`_, `double description <%s>`_ (conversion between
-halfspace and vertex representations), computing the `Chebyshev center <%s>`_,
-etc.
-
-See the complete `API documentation <%s>`_ for details.
-
-Examples
---------
-
-Vertex enumeration
-~~~~~~~~~~~~~~~~~~
-
-We can compute the list of vertices of a polytope described in halfspace
-representation by ``A * x <= b``:
-
-.. code:: python
-
-    import numpy
-    import pypoman
-
-    A = numpy.array([
-        [-1,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0],
-        [0, -1,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0],
-        [0,  0, -1,  0,  0,  0,  0,  0,  0,  0,  0,  0],
-        [0,  0,  0, -1,  0,  0,  0,  0,  0,  0,  0,  0],
-        [0,  0,  0,  0, -1,  0,  0,  0,  0,  0,  0,  0],
-        [0,  0,  0,  0,  0, -1,  0,  0,  0,  0,  0,  0],
-        [0,  0,  0,  0,  0,  0, -1,  0,  0,  0,  0,  0],
-        [0,  0,  0,  0,  0,  0,  0, -1,  0,  0,  0,  0],
-        [0,  0,  0,  0,  0,  0,  0,  0, -1,  0,  0,  0],
-        [0,  0,  0,  0,  0,  0,  0,  0,  0, -1,  0,  0],
-        [0,  0,  0,  0,  0,  0,  0,  0,  0,  0, -1,  0],
-        [0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0, -1],
-        [1,  1,  1,  0,  0,  0,  0,  0,  0,  0,  0,  0],
-        [0,  0,  0,  1,  1,  1,  0,  0,  0,  0,  0,  0],
-        [0,  0,  0,  0,  0,  0,  1,  1,  1,  0,  0,  0],
-        [0,  0,  0,  0,  0,  0,  0,  0,  0,  1,  1,  1],
-        [1,  0,  0,  1,  0,  0,  1,  0,  0,  1,  0,  0],
-        [0,  1,  0,  0,  1,  0,  0,  1,  0,  0,  1,  0],
-        [0,  0,  1,  0,  0,  1,  0,  0,  1,  0,  0,  1]])
-    b = numpy.array([0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 2, 1, 2, 2, 1, 2, 3])
-    vertices = pypoman.compute_polytope_vertices(A, b)
-
-Polytope projection
-~~~~~~~~~~~~~~~~~~~
-
-Let us project an n-dimensional polytope over ``x = [x_1 ... x_n]`` onto its
-first two coordinates ``proj(x) = [x_1 x_2]``:
-
-.. code:: python
-
-    import pypoman
-    from numpy import array, eye, ones, vstack, zeros
-
-    n = 10  # dimension of the original polytope
-    p = 2   # dimension of the projected polytope
-
-    # Original polytope:
-    # - inequality constraints: \\forall i, |x_i| <= 1
-    # - equality constraint: sum_i x_i = 0
-    A = vstack([+eye(n), -eye(n)])
-    b = ones(2 * n)
-    C = ones(n).reshape((1, n))
-    d = array([0])
-    ineq = (A, b)  # A * x <= b
-    eq = (C, d)    # C * x == d
-
-    # Projection is proj(x) = [x_0 x_1]
-    E = zeros((p, n))
-    E[0, 0] = 1.
-    E[1, 1] = 1.
-    f = zeros(p)
-    proj = (E, f)  # proj(x) = E * x + f
-
-    vertices = pypoman.project_polytope(proj, ineq, eq, method='bretl')
-
-    if __name__ == "__main__":   # plot projected polytope
-        import pylab
-        pylab.ion()
-        pylab.figure()
-        pypoman.plot_polygon(vertices)
-""" % tuple(links)
-
-os.environ['CVXOPT_BUILD_GLPK'] = '1'
-
-setup(
-    name='pypoman',
-    version='0.5.4',
-    description="Polyhedron and polytope manipulation in Python",
-    long_description=long_description,
-    url="https://github.com/stephane-caron/pypoman",
-    author="Stéphane Caron",
-    author_email="stephane.caron@lirmm.fr",
-    license="LGPL",
-    keywords="convex, polyhedron, polyhedra, polytope, projection, duality",
-    classifiers=classifiers.split('\n'),
-    packages=['pypoman'],
-    install_requires=['cvxopt', 'pycddlib']
+# Polyhedron manipulation in Python
+
+[![PyPI package](https://img.shields.io/pypi/v/pypoman)](https://pypi.org/project/pypoman/)
+[![Documentation](https://img.shields.io/badge/documentation-online-brightgreen?logo=read-the-docs&style=flat)](https://scaron.info/doc/pypoman/)
+![Status](https://img.shields.io/pypi/status/pypoman)
+
+This library allows common operations over [convex polyhedra](https://en.wikipedia.org/wiki/Convex_polyhedron) such as [polytope projection](https://scaron.info/doc/pypoman/index.html#module-pypoman.projection) and [vertex enumeration](https://scaron.info/doc/pypoman/index.html#module-pypoman.duality).
+
+See the [API documentation](https://scaron.info/doc/pypoman/) for details.
+
+## Installation
+
+Install system packages (here for Debian-based distributions) for Python and GLPK by:
+
+```console
+$ sudo apt-get install cython libglpk-dev python python-dev python-pip python-scipy
+```
+
+Then, install the library by:
+
+```console
+$ pip install pypoman
+```
+
+## Examples
+
+### Vertex enumeration
+
+We can compute the list of vertices of a polytope described in halfspace representation by $A x \leq b$:
+
+```python
+import numpy as np
+from pypoman import compute_polytope_vertices
+
+A = np.array([
+    [-1,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0],
+    [0, -1,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0],
+    [0,  0, -1,  0,  0,  0,  0,  0,  0,  0,  0,  0],
+    [0,  0,  0, -1,  0,  0,  0,  0,  0,  0,  0,  0],
+    [0,  0,  0,  0, -1,  0,  0,  0,  0,  0,  0,  0],
+    [0,  0,  0,  0,  0, -1,  0,  0,  0,  0,  0,  0],
+    [0,  0,  0,  0,  0,  0, -1,  0,  0,  0,  0,  0],
+    [0,  0,  0,  0,  0,  0,  0, -1,  0,  0,  0,  0],
+    [0,  0,  0,  0,  0,  0,  0,  0, -1,  0,  0,  0],
+    [0,  0,  0,  0,  0,  0,  0,  0,  0, -1,  0,  0],
+    [0,  0,  0,  0,  0,  0,  0,  0,  0,  0, -1,  0],
+    [0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0, -1],
+    [1,  1,  1,  0,  0,  0,  0,  0,  0,  0,  0,  0],
+    [0,  0,  0,  1,  1,  1,  0,  0,  0,  0,  0,  0],
+    [0,  0,  0,  0,  0,  0,  1,  1,  1,  0,  0,  0],
+    [0,  0,  0,  0,  0,  0,  0,  0,  0,  1,  1,  1],
+    [1,  0,  0,  1,  0,  0,  1,  0,  0,  1,  0,  0],
+    [0,  1,  0,  0,  1,  0,  0,  1,  0,  0,  1,  0],
+    [0,  0,  1,  0,  0,  1,  0,  0,  1,  0,  0,  1]])
+b = np.array([0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 2, 1, 2, 2, 1, 2, 3])
+
+vertices = compute_polytope_vertices(A, b)
+```
+
+### Halfspace enumeration
+
+The other way round, assume we know the vertices of a polytope, and want to get its halfspace representation $A x \leq b$.
+
+```python
+import numpy as np
+from pypoman import compute_polytope_halfspaces
+
+vertices = map(
+    np.array,
+    [[1, 0, 0], [0, 1, 0], [1, 1, 0], [0, 0, 1], [0, 1, 1]],
 )
+
+A, b = compute_polytope_halfspaces(vertices)
+```
+
+### Polytope projection
+
+Let us project an $n$-dimensional polytope $A x \leq b$ over $x = [x_1\ \ldots\ x_n]$ onto its first two coordinates $proj(x) = [x_1 x_2]$:
+
+```python
+from numpy import array, eye, ones, vstack, zeros
+from pypoman import plot_polygon, project_polytope
+
+n = 10  # dimension of the original polytope
+p = 2   # dimension of the projected polytope
+
+# Original polytope:
+# - inequality constraints: \forall i, |x_i| <= 1
+# - equality constraint: sum_i x_i = 0
+A = vstack([+eye(n), -eye(n)])
+b = ones(2 * n)
+C = ones(n).reshape((1, n))
+d = array([0])
+ineq = (A, b)  # A * x <= b
+eq = (C, d)    # C * x == d
+
+# Projection is proj(x) = [x_0 x_1]
+E = zeros((p, n))
+E[0, 0] = 1.
+E[1, 1] = 1.
+f = zeros(p)
+proj = (E, f)  # proj(x) = E * x + f
+
+vertices = project_polytope(proj, ineq, eq, method='bretl')
+
+if __name__ == "__main__":   # plot projected polytope
+    import pylab
+    pylab.ion()
+    pylab.figure()
+    plot_polygon(vertices)
+```
+
+## See also
+
+- A short introduction to [Polyhedra and polytopes](https://scaron.info/teaching/polyhedra-and-polytopes.html)
+- Komei Fukuda's [Frequently Asked Questions in Polyhedral Computation](https://www.inf.ethz.ch/personal/fukudak/polyfaq/polyfaq.html)
+- The [Polyhedron](http://doc.sagemath.org/html/en/reference/discrete_geometry/sage/geometry/polyhedron/constructor.html) class in [Sage](http://www.sagemath.org/)
+- [StabiliPy](https://github.com/haudren/stabilipy): a Python package implementing a more general recursive method for polytope projection
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pypoman-0.5.4/pypoman/projection.py` & `pypoman-0.6.0/pypoman/projection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,57 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2018 Stephane Caron <stephane.caron@lirmm.fr>
+# Copyright (C) 2018-2020 Stephane Caron <stephane.caron@normalesup.org>
 #
 # This file is part of pypoman <https://github.com/stephane-caron/pypoman>.
 #
 # pypoman is free software: you can redistribute it and/or modify it under the
-# terms of the GNU Lesser General Public License as published by the Free
-# Software Foundation, either version 3 of the License, or (at your option) any
-# later version.
+# terms of the GNU General Public License as published by the Free Software
+# Foundation, either version 3 of the License, or (at your option) any later
+# version.
 #
 # pypoman is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
-# A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more
-# details.
+# A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 #
-# You should have received a copy of the GNU Lesser General Public License
-# along with pypoman. If not, see <http://www.gnu.org/licenses/>.
+# You should have received a copy of the GNU General Public License along with
+# pypoman. If not, see <http://www.gnu.org/licenses/>.
+
+"""Polytope projection functions."""
+
+from typing import List, Optional, Tuple
 
 import cdd
 import cvxopt
-
-from numpy import array, dot, hstack, zeros
+import numpy as np
 
 from .bretl import compute_polygon as bretl_compute_polygon
 
 
-def project_polyhedron(proj, ineq, eq=None, canonicalize=True):
-    """
-    Apply the affine projection :math:`y = E x + f` to the polyhedron defined
-    by:
+def project_polyhedron(
+    proj: Tuple[np.ndarray, np.ndarray],
+    ineq: Tuple[np.ndarray, np.ndarray],
+    eq: Optional[Tuple[np.ndarray, np.ndarray]] = None,
+    canonicalize: bool = True,
+) -> Tuple[List[np.ndarray], List[np.ndarray]]:
+    r"""Apply the affine projection :math:`y = E x + f` to a polyhedron.
+
+    The polyhedron is defined by:
 
     .. math::
 
-        A x & \\leq b \\\\
-        C x & = d
+        \begin{split}\begin{array}{ll}
+            A x & \leq b \\
+            C x & = d
+        \end{array}\end{split}
 
     Parameters
     ----------
-    proj : pair of arrays
+    proj :
         Pair (`E`, `f`) describing the affine projection.
     ineq : pair of arrays
         Pair (`A`, `b`) describing the inequality constraint.
     eq : pair of arrays, optional
         Pair (`C`, `d`) describing the equality constraint.
     canonicalize : bool, optional
         Apply equality constraints from `eq` to reduce the dimension of the
@@ -69,54 +78,55 @@
     --------
     This webpage: https://scaron.info/teaching/projecting-polytopes.html
     """
     # the input [b, -A] to cdd.Matrix represents (b - A * x >= 0)
     # see ftp://ftp.ifor.math.ethz.ch/pub/fukuda/cdd/cddlibman/node3.html
     (A, b) = ineq
     b = b.reshape((b.shape[0], 1))
-    linsys = cdd.Matrix(hstack([b, -A]), number_type='float')
+    linsys = cdd.Matrix(np.hstack([b, -A]), number_type="float")
     linsys.rep_type = cdd.RepType.INEQUALITY
 
     # the input [d, -C] to cdd.Matrix.extend represents (d - C * x == 0)
     # see ftp://ftp.ifor.math.ethz.ch/pub/fukuda/cdd/cddlibman/node3.html
     if eq is not None:
         (C, d) = eq
         d = d.reshape((d.shape[0], 1))
-        linsys.extend(hstack([d, -C]), linear=True)
+        linsys.extend(np.hstack([d, -C]), linear=True)
         if canonicalize:
             linsys.canonicalize()
 
     # Convert from H- to V-representation
     P = cdd.Polyhedron(linsys)
     generators = P.get_generators()
     if generators.lin_set:
         print("Generators have linear set: {}".format(generators.lin_set))
-    V = array(generators)
+    V = np.array(generators)
 
     # Project output wrenches to 2D set
     (E, f) = proj
     vertices, rays = [], []
     free_coordinates = []
     for i in range(V.shape[0]):
         if generators.lin_set and i in generators.lin_set:
-            free_coordinates.append(list(V[i, 1:]).index(1.))
+            free_coordinates.append(list(V[i, 1:]).index(1.0))
         elif V[i, 0] == 1:  # vertex
-            vertices.append(dot(E, V[i, 1:]) + f)
+            vertices.append(np.dot(E, V[i, 1:]) + f)
         else:  # ray
-            rays.append(dot(E, V[i, 1:]))
+            rays.append(np.dot(E, V[i, 1:]))
     return vertices, rays
 
 
-def project_polytope(proj, ineq, eq=None, method='cdd', **kwargs):
-    """
-    Apply the affine projection :math:`y = E x + f` to the polytope defined by:
+def project_polytope(proj, ineq, eq=None, method="cdd", **kwargs):
+    r"""Apply the affine projection :math:`y = E x + f` to a polytope.
+
+    The polytope is defined by:
 
     .. math::
 
-        A x & \\leq b \\\\
+        A x & \leq b \\
         C x & = d
 
     Parameters
     ----------
     proj : pair of arrays
         Pair (`E`, `f`) describing the affine projection.
     ineq : pair of arrays
@@ -139,32 +149,34 @@
 
     Notes
     -----
     The number of columns of all matrices `A`, `C` and `E` corresponds to the
     dimension of the input space, while the number of lines of `E` corresponds
     to the dimension of the output space.
     """
-    if method == 'bretl':
+    if method == "bretl":
         assert eq is not None, "Bretl method requires = constraints for now"
         return project_polytope_bretl(proj, ineq, eq, **kwargs)
     vertices, rays = project_polyhedron(proj, ineq, eq)
     assert not rays, "Projection is not a polytope"
     return vertices
 
 
-def project_polytope_bretl(proj, ineq, eq, max_radius=1e5, max_iter=1000,
-                           init_angle=None):
-    """
-    Project a polytope into a 2D polygon using the incremental projection
-    algorithm from [Bretl08]_. The 2D affine projection :math:`y = E x + f` is
-    applied to the polyhedron defined by:
+def project_polytope_bretl(
+    proj, ineq, eq, max_radius=1e5, max_iter=1000, init_angle=None
+):
+    r"""Project a polytope into a 2D polygon using the IP algorithm.
+
+    The incremental projection algorithm is detailed in [Bretl08]_. The 2D
+    affine projection :math:`y = E x + f` is applied to the polyhedron defined
+    by:
 
     .. math::
 
-        A x & \\leq b \\\\
+        A x & \leq b \\
         C x & = d
 
     Parameters
     ----------
     proj : pair of arrays
         Pair (`E`, `f`) describing the affine projection.
     ineq : pair of arrays
@@ -185,41 +197,75 @@
         List of vertices of the projected polygon.
     """
     (E, f), (A, b), (C, d) = proj, ineq, eq
     assert E.shape[0] == f.shape[0] == 2
 
     # Inequality constraints: A_ext * [ x  u  v ] <= b_ext iff
     # (1) A * x <= b and (2) |u|, |v| <= max_radius
-    A_ext = zeros((A.shape[0] + 4, A.shape[1] + 2))
+    A_ext = np.zeros((A.shape[0] + 4, A.shape[1] + 2))
     A_ext[:-4, :-2] = A
     A_ext[-4, -2] = 1
     A_ext[-3, -2] = -1
     A_ext[-2, -1] = 1
     A_ext[-1, -1] = -1
     A_ext = cvxopt.matrix(A_ext)
 
-    b_ext = zeros(b.shape[0] + 4)
+    b_ext = np.zeros(b.shape[0] + 4)
     b_ext[:-4] = b
-    b_ext[-4:] = array([max_radius] * 4)
+    b_ext[-4:] = np.array([max_radius] * 4)
     b_ext = cvxopt.matrix(b_ext)
 
     # Equality constraints: C_ext * [ x  u  v ] == d_ext iff
     # (1) C * x == d and (2) [ u  v ] == E * x + f
-    C_ext = zeros((C.shape[0] + 2, C.shape[1] + 2))
+    C_ext = np.zeros((C.shape[0] + 2, C.shape[1] + 2))
     C_ext[:-2, :-2] = C
     C_ext[-2:, :-2] = E[:2]
-    C_ext[-2:, -2:] = array([[-1, 0], [0, -1]])
+    C_ext[-2:, -2:] = np.array([[-1, 0], [0, -1]])
     C_ext = cvxopt.matrix(C_ext)
 
-    d_ext = zeros(d.shape[0] + 2)
+    d_ext = np.zeros(d.shape[0] + 2)
     d_ext[:-2] = d
     d_ext[-2:] = -f[:2]
     d_ext = cvxopt.matrix(d_ext)
 
-    lp_obj = cvxopt.matrix(zeros(A.shape[1] + 2))
+    lp_obj = cvxopt.matrix(np.zeros(A.shape[1] + 2))
     lp = lp_obj, A_ext, b_ext, C_ext, d_ext
-    polygon = bretl_compute_polygon(lp, max_iter=max_iter,
-                                    init_angle=init_angle)
+    polygon = bretl_compute_polygon(
+        lp, max_iter=max_iter, init_angle=init_angle
+    )
     polygon.sort_vertices()
     vertices_list = polygon.export_vertices()
-    vertices = [array([v.x, v.y]) for v in vertices_list]
+    vertices = [np.array([v.x, v.y]) for v in vertices_list]
     return vertices
+
+
+def project_point_to_polytope(point, ineq, solver="quadprog", **kwargs):
+    """
+    Projet a point onto a polytope in H-representation.
+
+    Parameters
+    ----------
+    point : array
+        Point to project.
+    ineq : pair of arrays
+        Pair (`A`, `b`) describing the inequality constraint.
+    solver : string
+        Name of the quadratic programming solver to use.
+
+    Returns
+    -------
+    projection : array
+        Projected point.
+
+    Note
+    ----
+    This function requires `qpsolvers <https://pypi.org/project/qpsolvers/>`_.
+    """
+    try:
+        from qpsolvers import solve_ls
+    except ImportError as e:
+        raise ImportError(
+            "This function requires qpsolvers: pip install qpsolvers"
+        ) from e
+
+    P = np.eye(len(point))
+    return solve_ls(P, point, G=ineq[0], h=ineq[1], solver=solver, **kwargs)
```

### Comparing `pypoman-0.5.4/pypoman/misc.py` & `pypoman-0.6.0/pypoman/misc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,78 +1,78 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2018 Stephane Caron <stephane.caron@lirmm.fr>
+# Copyright (C) 2018-2020 Stephane Caron <stephane.caron@normalesup.org>
 #
 # This file is part of pypoman <https://github.com/stephane-caron/pypoman>.
 #
 # pypoman is free software: you can redistribute it and/or modify it under the
-# terms of the GNU Lesser General Public License as published by the Free
-# Software Foundation, either version 3 of the License, or (at your option) any
-# later version.
+# terms of the GNU General Public License as published by the Free Software
+# Foundation, either version 3 of the License, or (at your option) any later
+# version.
 #
 # pypoman is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
-# A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more
-# details.
+# A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 #
-# You should have received a copy of the GNU Lesser General Public License
-# along with pypoman. If not, see <http://www.gnu.org/licenses/>.
+# You should have received a copy of the GNU General Public License along with
+# pypoman. If not, see <http://www.gnu.org/licenses/>.
+
+"""Other utility functions."""
 
 from datetime import datetime
-from numpy import dot, sqrt
 
+import numpy as np
 
-def norm(v):
-    """
-    Euclidean norm.
+
+def norm(v: np.ndarray) -> float:
+    """Euclidean norm.
 
     Parameters
     ----------
-    v : array
-        Any vector.
+    v :
+        Vector.
 
     Returns
     -------
-    n : scalar
-        Euclidean norm of `v`.
+    :
+        Euclidean norm of the input vector.
 
     Notes
     -----
     This straightforward function is 2x faster than :func:`numpy.linalg.norm`
     on my machine.
     """
-    return sqrt(dot(v, v))
+    return np.sqrt(np.dot(v, v))
 
 
-def normalize(v):
-    """
-    Normalize a vector.
+def normalize(v: np.ndarray) -> np.ndarray:
+    """Normalize a vector.
 
     Parameters
     ----------
-    v : array
+    v :
         Any vector.
 
     Returns
     -------
-    nv : array
+    :
         Unit vector directing `v`.
 
     Notes
     -----
     This method doesn't catch ``ZeroDivisionError`` exceptions on purpose.
     """
     return v / norm(v)
 
 
-def warn(msg):
+def warn(msg: str) -> None:
     """
     Log a warning message (in yellow) to stdout.
 
     Parameters
     ----------
-    msg : str
+    msg :
         Warning message.
     """
     date = datetime.now().strftime("%Y-%m-%d %H:%M:%S,%f")[:-3]
     print("%c[0;%d;48m%s pypoman [WARN] %s%c[m" % (0x1B, 33, date, msg, 0x1B))
```

### Comparing `pypoman-0.5.4/pypoman/lp.py` & `pypoman-0.6.0/pypoman/lp.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,67 +1,78 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2018 Stephane Caron <stephane.caron@lirmm.fr>
+# Copyright (C) 2018-2020 Stephane Caron <stephane.caron@normalesup.org>
 #
 # This file is part of pypoman <https://github.com/stephane-caron/pypoman>.
 #
 # pypoman is free software: you can redistribute it and/or modify it under the
-# terms of the GNU Lesser General Public License as published by the Free
-# Software Foundation, either version 3 of the License, or (at your option) any
-# later version.
+# terms of the GNU General Public License as published by the Free Software
+# Foundation, either version 3 of the License, or (at your option) any later
+# version.
 #
 # pypoman is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
-# A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more
-# details.
+# A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 #
-# You should have received a copy of the GNU Lesser General Public License
-# along with pypoman. If not, see <http://www.gnu.org/licenses/>.
+# You should have received a copy of the GNU General Public License along with
+# pypoman. If not, see <http://www.gnu.org/licenses/>.
+
+"""Functions for linear programming."""
+
+from typing import Optional, Union
 
 import cvxopt
 import cvxopt.solvers
-
+import numpy as np
 from cvxopt.solvers import lp
-from numpy import array
 
 from .misc import warn
 
+cvxopt.solvers.options["show_progress"] = False  # disable cvxopt output
 
-cvxopt.solvers.options['show_progress'] = False  # disable cvxopt output
-
+GLPK_IF_AVAILABLE: Optional[str] = None
 try:
     import cvxopt.glpk
-    GLPK_IF_AVAILABLE = 'glpk'
+
+    GLPK_IF_AVAILABLE = "glpk"
     # GLPK is the fastest LP solver I could find so far:
     # <https://scaron.info/blog/linear-programming-in-python-with-cvxopt.html>
     # ... however, it's verbose by default, so tell it to STFU:
-    cvxopt.solvers.options['glpk'] = {'msg_lev': 'GLP_MSG_OFF'}  # cvxopt 1.1.8
-    cvxopt.solvers.options['msg_lev'] = 'GLP_MSG_OFF'  # cvxopt 1.1.7
-    cvxopt.solvers.options['LPX_K_MSGLEV'] = 0  # previous versions
+    cvxopt.solvers.options["glpk"] = {"msg_lev": "GLP_MSG_OFF"}  # cvxopt 1.1.8
+    cvxopt.solvers.options["msg_lev"] = "GLP_MSG_OFF"  # cvxopt 1.1.7
+    cvxopt.solvers.options["LPX_K_MSGLEV"] = 0  # previous versions
 except ImportError:
     # issue a warning as GLPK is the best LP solver in practice
     warn("GLPK solver not found")
-    GLPK_IF_AVAILABLE = None
 
 
-def cvxmat(M):
+def cvxmat(M: Union[np.ndarray, cvxopt.matrix]) -> cvxopt.matrix:
+    """Convert a NumPy array to a CVXOPT matrix."""
     if isinstance(M, cvxopt.matrix):
         return M
     return cvxopt.matrix(M)
 
 
-def solve_lp(c, G, h, A=None, b=None, solver=GLPK_IF_AVAILABLE):
-    """
-    Solve a linear program defined by:
+def solve_lp(
+    c: np.ndarray,
+    G: np.ndarray,
+    h: np.ndarray,
+    A: Optional[np.ndarray] = None,
+    b: Optional[np.ndarray] = None,
+    solver: Optional[str] = GLPK_IF_AVAILABLE,
+) -> np.ndarray:
+    r"""Solve a linear program (LP).
+
+    The linear program is defined by:
 
     .. math::
 
-        \\mathrm{minimize} \\ & c^T x \\\\
-        \\mathrm{subject\\ to} \\ & G x \\leq h \\\\
+        \mathrm{minimize} \ & c^T x \\
+        \mathrm{subject\ to} \ & G x \leq h \\
             & A x = b
 
     using the `CVXOPT
     <http://cvxopt.org/userguide/coneprog.html#linear-programming>`_ interface
     to LP solvers.
 
     Parameters
@@ -77,22 +88,22 @@
     b : array, shape=(meq,), optional
         Linear equality constraint vector.
     solver : string, optional
         Solver to use, default is GLPK if available
 
     Returns
     -------
-    x : array, shape=(n,)
-        Optimal solution to the LP, if found, otherwise ``None``.
+    :
+        Optimal solution to the LP.
 
     Raises
     ------
     ValueError
         If the LP is not feasible.
     """
     args = [cvxmat(c), cvxmat(G), cvxmat(h)]
     if A is not None:
         args.extend([cvxmat(A), cvxmat(b)])
     sol = lp(*args, solver=solver)
-    if 'optimal' not in sol['status']:
-        raise ValueError("LP optimum not found: %s" % sol['status'])
-    return array(sol['x']).reshape((array(c).shape[0],))
+    if "optimal" not in sol["status"]:
+        raise ValueError("LP optimum not found: %s" % sol["status"])
+    return np.array(sol["x"]).reshape((np.array(c).shape[0],))
```

### Comparing `pypoman-0.5.4/pypoman/intersection.py` & `pypoman-0.6.0/pypoman/intersection.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,66 +1,72 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2018 Stephane Caron <stephane.caron@lirmm.fr>
+# Copyright (C) 2018-2020 Stephane Caron <stephane.caron@normalesup.org>
 #
 # This file is part of pypoman <https://github.com/stephane-caron/pypoman>.
 #
 # pypoman is free software: you can redistribute it and/or modify it under the
-# terms of the GNU Lesser General Public License as published by the Free
-# Software Foundation, either version 3 of the License, or (at your option) any
-# later version.
+# terms of the GNU General Public License as published by the Free Software
+# Foundation, either version 3 of the License, or (at your option) any later
+# version.
 #
 # pypoman is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
-# A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more
-# details.
+# A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 #
-# You should have received a copy of the GNU Lesser General Public License
-# along with pypoman. If not, see <http://www.gnu.org/licenses/>.
+# You should have received a copy of the GNU General Public License along with
+# pypoman. If not, see <http://www.gnu.org/licenses/>.
 
-from numpy import array
+"""Intersections between lines and polyhedra."""
+
+from typing import List, Tuple
+
+import numpy as np
 from scipy.spatial import ConvexHull
 
 from .misc import norm
 
-
 PREC_TOL = 1e-10  # numerical tolerance
 
 
-def intersect_line_polygon(line, vertices, apply_hull):
-    """
-    Intersect a line segment with a polygon.
+def intersect_line_polygon(
+    line: Tuple[np.ndarray, np.ndarray],
+    vertices: List[np.ndarray],
+    apply_hull: bool,
+) -> List[np.ndarray]:
+    """Intersect a line segment with a polygon.
 
     Parameters
     ----------
-    line : couple of arrays
+    line :
         End points of the line segment (2D or 3D).
-    vertices : list of arrays
+    vertices :
         Vertices of the polygon.
-    apply_hull : bool
+    apply_hull :
         Set to `True` to apply a convex hull algorithm to `vertices`.
         Otherwise, the function assumes that vertices are already sorted in
         clockwise or counterclockwise order.
 
     Returns
     -------
-    inter_points : list of array
+    :
         List of intersection points between the line segment and the polygon.
 
     Notes
     -----
     This code is adapted from
     <https://stackoverflow.com/questions/20677795/how-do-i-compute-the-intersection-point-of-two-lines-in-python/20679579#20679579>.
     On the same setting with `apply_hull=False`, it %timeits to 6 us.
     """
+
     def line_coordinates(p1, p2):
-        A = (p1[1] - p2[1])
-        B = (p2[0] - p1[0])
-        C = (p1[0] * p2[1] - p2[0] * p1[1])
+        A = p1[1] - p2[1]
+        B = p2[0] - p1[0]
+        C = p1[0] * p2[1] - p2[0] * p1[1]
         return A, B, -C
 
     def intersection(L1, L2):
         D = L1[0] * L2[1] - L1[1] * L2[0]
         Dx = L1[2] * L2[1] - L1[1] * L2[2]
         Dy = L1[0] * L2[2] - L1[2] * L2[0]
         if abs(D) < 1e-5:
@@ -81,71 +87,88 @@
     y_min, y_max = min(p1[1], p2[1]), max(p1[1], p2[1])
     inter_points = []
     for i, v1 in enumerate(vertices):
         v2 = vertices[(i + 1) % n]
         L2 = line_coordinates(v1, v2)
         p = intersection(L1, L2)
         if p is not None:
-            if not (x_min <= p[0] <= x_max and y_min <= p[1] <= y_max):
+            if not (
+                x_min - PREC_TOL <= p[0] <= x_max + PREC_TOL
+                and y_min - PREC_TOL <= p[1] <= y_max + PREC_TOL
+            ):
                 continue
             vx_min, vx_max = min(v1[0], v2[0]), max(v1[0], v2[0])
             vy_min, vy_max = min(v1[1], v2[1]), max(v1[1], v2[1])
-            if not (vx_min - PREC_TOL <= p[0] <= vx_max + PREC_TOL and
-                    vy_min - PREC_TOL <= p[1] <= vy_max + PREC_TOL):
+            if not (
+                vx_min - PREC_TOL <= p[0] <= vx_max + PREC_TOL
+                and vy_min - PREC_TOL <= p[1] <= vy_max + PREC_TOL
+            ):
                 continue
-            inter_points.append(array(p))
+            inter_points.append(np.array(p))
     return inter_points
 
 
-def intersect_line_cylinder(line, vertices):
-    """
-    Intersect the line segment [p1, p2] with a vertical cylinder of polygonal
-    cross-section. If the intersection has two points, returns the one closest
-    to p1.
+def intersect_line_cylinder(
+    line: Tuple[np.ndarray, np.ndarray], vertices: List[np.ndarray]
+) -> List[np.ndarray]:
+    """Intersect the line segment [p1, p2] with a vertical cylinder.
+
+    The vertical cylinder has a polygonal cross-section. If the intersection
+    has two points, this function returns the one closest to p1.
 
     Parameters
     ----------
-    line : couple of (3,) arrays
+    line :
         End points of the 3D line segment.
-    vertices : list of (3,) arrays
+    vertices :
         Vertices of the polygon.
 
     Returns
     -------
-    inter_points : list of (3,) arrays
+    inter_points :
         List of intersection points between the line segment and the cylinder.
     """
     inter_points = []
     inter_2d = intersect_line_polygon(line, vertices, apply_hull=True)
     for p in inter_2d:
-        p1, p2 = array(line[0]), array(line[1])
+        p1, p2 = np.array(line[0]), np.array(line[1])
         alpha = norm(p - p1[:2]) / norm(p2[:2] - p1[:2])
         z = p1[2] + alpha * (p2[2] - p1[2])
-        inter_points.append(array([p[0], p[1], z]))
+        inter_points.append(np.array([p[0], p[1], z]))
     return inter_points
 
 
-def intersect_polygons(polygon1, polygon2):
+def intersect_polygons(
+    polygon1: List[np.ndarray],
+    polygon2: List[np.ndarray],
+) -> List[np.ndarray]:
     """
     Intersect two polygons.
 
     Parameters
     ----------
-    polygon1 : list of arrays
+    polygon1 :
         Vertices of the first polygon in counterclockwise order.
-    polygon1 : list of arrays
+    polygon1 :
         Vertices of the second polygon in counterclockwise order.
 
     Returns
     -------
-    intersection : list of arrays
+    :
         Vertices of the intersection in counterclockwise order.
     """
-    from pyclipper import Pyclipper, PT_CLIP, PT_SUBJECT, CT_INTERSECTION
-    from pyclipper import scale_to_clipper, scale_from_clipper
+    from pyclipper import (
+        CT_INTERSECTION,
+        PT_CLIP,
+        PT_SUBJECT,
+        Pyclipper,
+        scale_from_clipper,
+        scale_to_clipper,
+    )
+
     # could be accelerated by removing the scale_to/from_clipper()
     subj, clip = (polygon1,), polygon2
     pc = Pyclipper()
     pc.AddPath(scale_to_clipper(clip), PT_CLIP)
     pc.AddPaths(scale_to_clipper(subj), PT_SUBJECT)
     solution = pc.Execute(CT_INTERSECTION)
     if not solution:
```

### Comparing `pypoman-0.5.4/pypoman/polyhedron.py` & `pypoman-0.6.0/pypoman/polyhedron.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2018 Stephane Caron <stephane.caron@lirmm.fr>
+# Copyright (C) 2018-2020 Stephane Caron <stephane.caron@normalesup.org>
 #
 # This file is part of pypoman <https://github.com/stephane-caron/pypoman>.
 #
 # pypoman is free software: you can redistribute it and/or modify it under the
-# terms of the GNU Lesser General Public License as published by the Free
-# Software Foundation, either version 3 of the License, or (at your option) any
-# later version.
+# terms of the GNU General Public License as published by the Free Software
+# Foundation, either version 3 of the License, or (at your option) any later
+# version.
 #
 # pypoman is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
-# A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more
-# details.
+# A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 #
-# You should have received a copy of the GNU Lesser General Public License
-# along with pypoman. If not, see <http://www.gnu.org/licenses/>.
+# You should have received a copy of the GNU General Public License along with
+# pypoman. If not, see <http://www.gnu.org/licenses/>.
+
+"""General polyhedron-related functions."""
 
 from __future__ import division
 
-from numpy import array, hstack, zeros
+import numpy as np
 
 from .lp import solve_lp
 from .misc import norm, warn
 
-
 try:
     import cdd
 except ImportError:
     warn("Could not import cdd, some functions will not be available")
     cdd = None
 
 
@@ -37,17 +37,17 @@
     import cvxopt
 except ImportError:
     warn("Could not import CVXOPT, some functions will not be available")
     cvxopt = None
 
 
 def compute_chebyshev_center(A, b):
-    """
-    Compute the Chebyshev center of a polyhedron, that is, the point furthest
-    away from all inequalities.
+    """Compute the Chebyshev center of a polyhedron.
+
+    The Chebyshev center is the point furthest away from all inequalities.
 
     Parameters
     ----------
     A : array, shape=(m, k)
         Matrix of halfspace representation.
     b : array, shape=(m,)
         Vector of halfspace representation.
@@ -57,15 +57,22 @@
     z : array, shape=(k,)
         Point further away from all inequalities.
 
     Notes
     -----
     The Chebyshev center is discussed in [Boyd04]_, Section 4.3.1, p. 148.
     """
-    cost = zeros(A.shape[1] + 1)
-    cost[-1] = -1.
-    a_cheby = array([norm(A[i, :]) for i in range(A.shape[0])])
-    A_cheby = hstack([A, a_cheby.reshape((A.shape[0], 1))])
+    cost = np.zeros(A.shape[1] + 1)
+    cost[-1] = -1.0
+    a_cheby = np.array([norm(A[i, :]) for i in range(A.shape[0])])
+    A_cheby = np.hstack([A, a_cheby.reshape((A.shape[0], 1))])
     z = solve_lp(cost, A_cheby, b)
     if z[-1] < -1e-1:  # last coordinate is distance to boundaries
         raise Exception("Polytope is empty (margin violation %.2f)" % z[-1])
     return z[:-1]
+
+
+__all__ = [
+    "cdd",
+    "compute_chebyshev_center",
+    "cvxopt",
+]
```

### Comparing `pypoman-0.5.4/pypoman/polygon.py` & `pypoman-0.6.0/pypoman/polygon.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,54 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2018 Stephane Caron <stephane.caron@lirmm.fr>
+# Copyright (C) 2018-2020 Stephane Caron <stephane.caron@normalesup.org>
 #
 # This file is part of pypoman <https://github.com/stephane-caron/pypoman>.
 #
 # pypoman is free software: you can redistribute it and/or modify it under the
-# terms of the GNU Lesser General Public License as published by the Free
-# Software Foundation, either version 3 of the License, or (at your option) any
-# later version.
+# terms of the GNU General Public License as published by the Free Software
+# Foundation, either version 3 of the License, or (at your option) any later
+# version.
 #
 # pypoman is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
-# A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more
-# details.
+# A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 #
-# You should have received a copy of the GNU Lesser General Public License
-# along with pypoman. If not, see <http://www.gnu.org/licenses/>.
+# You should have received a copy of the GNU General Public License along with
+# pypoman. If not, see <http://www.gnu.org/licenses/>.
 
+"""Functions on polygons, that is, 2D polyhedra."""
+
+import numpy as np
 from matplotlib.patches import Polygon
 from numpy import array, dot, hstack
 from pylab import axis, gca
 from scipy.spatial import ConvexHull
 
 from .polyhedron import compute_chebyshev_center
 
 
-def __compute_polygon_hull(B, c):
-    """
-    Compute the vertex representation of a polygon defined by:
+def __compute_polygon_hull(B: np.ndarray, c: np.ndarray):
+    r"""Compute the vertex representation of a polygon.
+
+    The polygon is defined by:
 
     .. math::
 
-        B x \\leq c
+        B x \leq c
 
-    where `x` is a 2D vector.
+    where :math:`x` is a 2D vector.
 
     Parameters
     ----------
-    B : array, shape=(2, K)
-        Linear inequality matrix.
-    c : array, shape=(K,)
-        Linear inequality vector with positive coordinates.
+    B :
+        Linear inequality matrix of size :math:`2 \times K`.
+    c :
+        Linear inequality vector of with positive coordinates.
 
     Returns
     -------
     vertices : list of arrays
         List of 2D vertices in counterclowise order.
 
     Notes
@@ -54,60 +57,68 @@
     order to build the polar form. If you don't have this guarantee, call
     ``compute_polar_polygon()`` instead.
 
     Checking that :math:`c > 0` is not optional. The rest of the algorithm can
     be executed when some coordinates :math:`c_i < 0`, but the result would be
     wrong.
     """
-    assert B.shape[1] == 2, \
-        "Input (B, c) is not a polygon: B.shape = %s" % str(B.shape)
-    assert all(c > 0), \
-        "Polygon should contain the origin, but min(c) = %.2f" % min(c)
-
-    B_polar = hstack([
-        (B[:, column] * 1. / c).reshape((B.shape[0], 1))
-        for column in range(2)])
+    assert (
+        B.shape[1] == 2
+    ), "Input (B, c) is not a polygon: B.shape = %s" % str(B.shape)
+    assert all(
+        c > 0
+    ), "Polygon should contain the origin, but min(c) = %.2f" % min(c)
+
+    B_polar = hstack(
+        [
+            (B[:, column] * 1.0 / c).reshape((B.shape[0], 1))
+            for column in range(2)
+        ]
+    )
 
     def axis_intersection(i, j):
         ai, bi = c[i], B[i]
         aj, bj = c[j], B[j]
-        x = (ai * bj[1] - aj * bi[1]) * 1. / (bi[0] * bj[1] - bj[0] * bi[1])
-        y = (bi[0] * aj - bj[0] * ai) * 1. / (bi[0] * bj[1] - bj[0] * bi[1])
+        x = (ai * bj[1] - aj * bi[1]) * 1.0 / (bi[0] * bj[1] - bj[0] * bi[1])
+        y = (bi[0] * aj - bj[0] * ai) * 1.0 / (bi[0] * bj[1] - bj[0] * bi[1])
         return array([x, y])
 
     # QHULL OPTIONS:
     #
     # - ``Pp`` -- do not report precision problems
     # - ``Q0`` -- no merging with C-0 and Qx
     #
     # ``Q0`` avoids [this bug](https://github.com/scipy/scipy/issues/6484).
     # It slightly diminishes computation times (0.9 -> 0.8 ms on my machine)
     # but raises QhullError at the first sight of precision errors.
     #
-    hull = ConvexHull([row for row in B_polar], qhull_options='Pp Q0')
+    hull = ConvexHull([row for row in B_polar], qhull_options="Pp Q0")
     #
     # contrary to hull.simplices (which was not in practice), hull.vertices is
     # guaranteed to be in counterclockwise order for 2-D (see scipy doc)
     #
-    simplices = [(hull.vertices[i], hull.vertices[i + 1])
-                 for i in range(len(hull.vertices) - 1)]
+    simplices = [
+        (hull.vertices[i], hull.vertices[i + 1])
+        for i in range(len(hull.vertices) - 1)
+    ]
     simplices.append((hull.vertices[-1], hull.vertices[0]))
     vertices = [axis_intersection(i, j) for (i, j) in simplices]
     return vertices
 
 
 def compute_polygon_hull(B, c):
-    """
-    Compute the vertex representation of a polygon defined by:
+    r"""Compute the vertex representation of a polygon.
+
+    The polygon is defined by:
 
     .. math::
 
-        B x \\leq c
+        B x \leq c
 
-    where `x` is a 2D vector.
+    where :math:`x` is a 2D vector.
 
     Parameters
     ----------
     B : array, shape=(2, K)
         Linear inequality matrix.
     c : array, shape=(K,)
         Linear inequality vector.
@@ -125,16 +136,23 @@
         raise Exception("Polygon is empty (min. dist. to edge %.2f)" % min(c))
     vertices = __compute_polygon_hull(B, c)
     if x is not None:
         vertices = [v + x for v in vertices]
     return vertices
 
 
-def plot_polygon(points, alpha=.4, color='g', linestyle='solid', fill=True,
-                 linewidth=None):
+def plot_polygon(
+    points,
+    alpha=0.4,
+    color="g",
+    linestyle="solid",
+    fill=True,
+    linewidth=None,
+    resize=False,
+):
     """
     Plot a polygon in matplotlib.
 
     Parameters
     ----------
     points : list of arrays
         List of poitns.
@@ -144,22 +162,36 @@
         Color in matplotlib format.
     linestyle : scalar, optional
         Line style in matplotlib format.
     fill : bool, optional
         When ``True``, fills the area inside the polygon.
     linewidth : scalar, optional
         Line width in matplotlib format.
+    resize : bool, optional
+        When ``True``, resets axis limits to center on the polygon.
     """
     if type(points) is list:
         points = array(points)
     ax = gca()
     hull = ConvexHull(points)
     points = points[hull.vertices, :]
-    xmin1, xmax1, ymin1, ymax1 = axis()
-    xmin2, ymin2 = 1.5 * points.min(axis=0)
-    xmax2, ymax2 = 1.5 * points.max(axis=0)
-    axis((min(xmin1, xmin2), max(xmax1, xmax2),
-          min(ymin1, ymin2), max(ymax1, ymax2)))
+    if resize:
+        xmin1, xmax1, ymin1, ymax1 = axis()
+        xmin2, ymin2 = 1.5 * points.min(axis=0)
+        xmax2, ymax2 = 1.5 * points.max(axis=0)
+        axis(
+            (
+                min(xmin1, xmin2),
+                max(xmax1, xmax2),
+                min(ymin1, ymin2),
+                max(ymax1, ymax2),
+            )
+        )
     patch = Polygon(
-        points, alpha=alpha, color=color, linestyle=linestyle, fill=fill,
-        linewidth=linewidth)
+        points,
+        alpha=alpha,
+        color=color,
+        linestyle=linestyle,
+        fill=fill,
+        linewidth=linewidth,
+    )
     ax.add_patch(patch)
```

### Comparing `pypoman-0.5.4/pypoman/bretl.py` & `pypoman-0.6.0/pypoman/bretl.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,102 +1,181 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2016 Quang-Cuong Pham <cuong.pham@normalesup.org>
-# Copyright (C) 2017-2018 Stephane Caron <stephane.caron@lirmm.fr>
+# Copyright (C) 2017-2020 Stephane Caron <stephane.caron@normalesup.org>
 #
 # This file is part of pypoman <https://github.com/stephane-caron/pypoman>.
 #
 # pypoman is free software: you can redistribute it and/or modify it under the
-# terms of the GNU Lesser General Public License as published by the Free
-# Software Foundation, either version 3 of the License, or (at your option) any
-# later version.
+# terms of the GNU General Public License as published by the Free Software
+# Foundation, either version 3 of the License, or (at your option) any later
+# version.
 #
 # pypoman is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
-# A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more
-# details.
+# A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 #
-# You should have received a copy of the GNU Lesser General Public License
-# along with pypoman. If not, see <http://www.gnu.org/licenses/>.
+# You should have received a copy of the GNU General Public License along with
+# pypoman. If not, see <http://www.gnu.org/licenses/>.
 
-from numpy import array, cos, cross, pi, sin
+"""Iterative projection algorithm by [Bretl08]_."""
+
+from typing import Any, List, Optional, Tuple, Union
+
+import numpy as np
 from numpy.random import random
 from scipy.linalg import norm
 
-from .lp import solve_lp, GLPK_IF_AVAILABLE
+from .lp import GLPK_IF_AVAILABLE, solve_lp
 
 
 class Vertex:
+    """Vertex of the projected polygon, with a pointer to its successor."""
 
-    def __init__(self, p):
+    expanded: bool
+    next: Optional[Any]
+    x: float
+    y: float
+
+    def __init__(self, p: Union[List[float], np.ndarray]):
+        """
+        Initialize vertex from point coordinates.
+
+        Parameters
+        ----------
+        p : array
+            2D coordinates.
+        """
         self.x = p[0]
         self.y = p[1]
         self.next = None
         self.expanded = False
 
-    def length(self):
-        return norm([self.x-self.next.x, self.y-self.next.y])
+    def expand(
+        self,
+        lp: Tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray],
+    ):
+        """
+        Expand the edge from the vertex to its successor.
 
-    def expand(self, lp):
+        Parameters
+        ----------
+        lp :
+            Tuple `(q, G, h, A, b)` defining the linear program. See
+            :func:`pypoman.lp.solve_lp` for details.
+        """
         v1 = self
         v2 = self.next
-        v = array([v2.y - v1.y, v1.x - v2.x])  # orthogonal direction to edge
-        v = 1 / norm(v) * v
+        if v2 is None:
+            raise ValueError("cannot expand vertex as it has no successor")
+        v = np.array(
+            [v2.y - v1.y, v1.x - v2.x]
+        )  # orthogonal direction to edge
+        v /= norm(v)
         try:
             z = optimize_direction(v, lp)
         except ValueError:
             self.expanded = True
-            return False, None
-        xopt, yopt = z
-        if abs(cross([xopt-v1.x, yopt-v1.y], [v1.x-v2.x, v1.y-v2.y])) < 1e-2:
+            return None
+        xopt: float = z[0]
+        yopt: float = z[1]
+        if (
+            abs(
+                np.cross(
+                    [xopt - v1.x, yopt - v1.y], [v1.x - v2.x, v1.y - v2.y]
+                )
+            )
+            < 1e-4
+        ):
             self.expanded = True
-            return False, None
-        else:
-            vnew = Vertex([xopt, yopt])
-            vnew.next = self.next
-            self.next = vnew
-            self.expanded = False
-            return True, vnew
+            return None
+        vnew = Vertex([xopt, yopt])
+        vnew.next = self.next
+        self.next = vnew
+        self.expanded = False
+        return vnew
 
 
 class Polygon:
+    """Polygon, that is, 2D polyhedron."""
+
+    vertices: List[Vertex]
 
-    def from_vertices(self, v1, v2, v3):
+    def __init__(self, v1: Vertex, v2: Vertex, v3: Vertex):
+        """
+        Initialize polygon from inscribed triangle.
+
+        Parameters
+        ----------
+        v1 : array
+            First vertex of the initial triangle.
+        v2 : array
+            Second vertex of the initial triangle.
+        v3 : array
+            Third vertex of the initial triangle.
+        """
         v1.next = v2
         v2.next = v3
         v3.next = v1
         self.vertices = [v1, v2, v3]
 
-    def all_expanded(self):
+    def all_expanded(self) -> bool:
+        """
+        Check for unexpanded vertices.
+
+        Returns
+        -------
+        :
+            True if and only if all vertices have been expanded.
+        """
         for v in self.vertices:
             if not v.expanded:
                 return False
         return True
 
-    def iter_expand(self, qpconstraints, max_iter):
-        """
-        Returns true if there's a edge that can be expanded, and expands that
-        edge, otherwise returns False.
+    def iter_expand(
+        self,
+        lp: Tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray],
+        max_iter: int,
+    ) -> None:
+        """Extend polygon until the termination condition is reached.
+
+        Termination condition: there is no other vertex to expand, or the
+        maximum number of iterations has been reached.
+
+        Parameters
+        ----------
+        lp :
+            Tuple `(q, G, h, A, b)` defining the linear program. See
+            :func:`pypoman.lp.solve_lp` for details.
+        max_iter :
+            Maximum number of iterations.
         """
         nb_iter = 0
         v = self.vertices[0]
         while not self.all_expanded() and nb_iter < max_iter:
             if v.expanded:
+                if v.next is None:
+                    raise ValueError(
+                        "Invalid expanded vertex with no successor"
+                    )
                 v = v.next
                 continue
-            res, vnew = v.expand(qpconstraints)
-            if not res:
+            vnew = v.expand(lp)
+            if vnew is None:
                 continue
             self.vertices.append(vnew)
             nb_iter += 1
 
     def sort_vertices(self):
-        """
-        Export vertices starting from the left-most and going clockwise.
+        """Export vertices starting from the leftmost one and going clockwise.
+
+        Note
+        ----
         Assumes all vertices are on the positive halfplane.
         """
         minsd = 1e10
         ibottom = 0
         for i in range(len(self.vertices)):
             v = self.vertices[i]
             if (v.y + v.next.y) < minsd:
@@ -111,118 +190,133 @@
             newvertices.append(vcur)
             vcur = vcur.next
         newvertices.reverse()
         vfirst = newvertices.pop(-1)
         newvertices.insert(0, vfirst)
         self.vertices = newvertices
 
-    def export_vertices(self, threshold=1e-2):
-        export_list = [self.vertices[0]]
-        for i in range(1, len(self.vertices)-1):
+    def export_vertices(self, min_dist: float = 1e-2) -> List[Vertex]:
+        """Get list of vertices.
+
+        Parameters
+        ----------
+        min_dist :
+            Minimum distance between two consecutive vertices.
+
+        Returns
+        -------
+        :
+            List of vertices.
+        """
+        vertices: List[Vertex] = [self.vertices[0]]
+        for i in range(1, len(self.vertices) - 1):
             vcur = self.vertices[i]
-            vlast = export_list[-1]
-            if norm([vcur.x-vlast.x, vcur.y-vlast.y]) > threshold:
-                export_list.append(vcur)
-        export_list.append(self.vertices[-1])  # always add last vertex
-        return export_list
+            vlast = vertices[-1]
+            if norm([vcur.x - vlast.x, vcur.y - vlast.y]) > min_dist:
+                vertices.append(vcur)
+        vertices.append(self.vertices[-1])  # always add last vertex
+        return vertices
 
 
-def optimize_direction(vdir, lp, solver=GLPK_IF_AVAILABLE):
-    """
-    Optimize in one direction.
+def optimize_direction(
+    vdir: np.ndarray,
+    lp: Tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray],
+    solver: Optional[str] = GLPK_IF_AVAILABLE,
+) -> np.ndarray:
+    """Optimize in one direction.
 
     Parameters
     ----------
     vdir : (3,) array
         Direction in which the optimization is performed.
     lp : array tuple
         Tuple `(q, G, h, A, b)` defining the LP. See
         :func:`pypoman.lp..solve_lp` for details.
     solver : string, optional
         Backend LP solver to call.
 
     Returns
     -------
-    succ : bool
-        Success boolean.
-    z : (3,) array, or 0
-        Maximum vertex of the polygon in the direction `vdir`, or 0 in case of
-        solver failure.
+    :
+        Vector ``z`` representing the maximum vertex of the polygon in the
+        direction `vdir`.
     """
     lp_q, lp_Gextended, lp_hextended, lp_A, lp_b = lp
     lp_q[-2] = -vdir[0]
     lp_q[-1] = -vdir[1]
-    x = solve_lp(
-        lp_q, lp_Gextended, lp_hextended, lp_A, lp_b, solver=solver)
+    x = solve_lp(lp_q, lp_Gextended, lp_hextended, lp_A, lp_b, solver=solver)
     return x[-2:]
 
 
-def optimize_angle(theta, lp, solver=GLPK_IF_AVAILABLE):
-    """
-    Optimize in one direction.
+def optimize_angle(
+    theta: float,
+    lp: Tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray],
+    solver: Optional[str] = GLPK_IF_AVAILABLE,
+) -> np.ndarray:
+    """Optimize in one direction.
 
     Parameters
     ----------
-    theta : scalar
+    theta :
         Angle of the direction in which the optimization is performed.
     lp : array tuple
         Tuple `(q, G, h, A, b)` defining the LP. See
         :func:`pypoman.lp..solve_lp` for details.
     solver : string, optional
         Backend LP solver to call.
 
     Returns
     -------
-    succ : bool
-        Success boolean.
-    z : (3,) array, or 0
-        Maximum vertex of the polygon in the direction `vdir`, or 0 in case of
-        solver failure.
+    :
+        Vector ``z`` representing the maximum vertex of the polygon in the
+        direction `vdir`.
     """
-    d = array([cos(theta), sin(theta)])
+    d = np.array([np.cos(theta), np.sin(theta)])
     z = optimize_direction(d, lp, solver=solver)
     return z
 
 
-def compute_polygon(lp, max_iter=1000, solver=GLPK_IF_AVAILABLE,
-                    init_angle=None):
-    """
-    Expand a polygon iteratively.
+def compute_polygon(
+    lp: Tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray],
+    max_iter: int = 1000,
+    solver: Optional[str] = GLPK_IF_AVAILABLE,
+    init_angle: Optional[float] = None,
+) -> Polygon:
+    """Expand a polygon iteratively.
 
     Parameters
     ----------
-    lp : array tuple
+    lp :
         Tuple `(q, G, h, A, b)` defining the linear program. See
         :func:`pypoman.lp.solve_lp` for details.
-    max_iter : integer, optional
+    max_iter :
         Maximum number of calls to the LP solver.
-    solver : string, optional
+    solver :
         Name of backend LP solver.
-    init_angle : scalar, optional
+    init_angle :
         Angle in [rad] giving the direction of the initial ray cast.
 
     Returns
     -------
-    poly : Polygon
+    :
         Output polygon.
     """
-    theta = init_angle if init_angle is not None else pi * random()
+    theta = init_angle if init_angle is not None else np.pi * random()
     init_vertices = [optimize_angle(theta, lp, solver)]
-    step = 2. * pi / 3.
+    step = 2.0 * np.pi / 3.0
     while len(init_vertices) < 3 and max_iter >= 0:
         theta += step
-        if theta >= 2. * pi:
+        if theta >= 2.0 * np.pi:
             step *= 0.25 + 0.5 * random()
-            theta += step - 2. * pi
+            theta += step - 2.0 * np.pi
         z = optimize_angle(theta, lp, solver)
         if all([norm(z - z0) > 1e-5 for z0 in init_vertices]):
             init_vertices.append(z)
         max_iter -= 1
     if len(init_vertices) < 3:
         raise Exception("problem is not linearly feasible")
     v0 = Vertex(init_vertices[0])
     v1 = Vertex(init_vertices[1])
     v2 = Vertex(init_vertices[2])
-    polygon = Polygon()
-    polygon.from_vertices(v0, v1, v2)
+    polygon = Polygon(v0, v1, v2)
     polygon.iter_expand(lp, max_iter)
     return polygon
```

### Comparing `pypoman-0.5.4/pypoman/duality.py` & `pypoman-0.6.0/pypoman/duality.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,132 +1,165 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2018 Stephane Caron <stephane.caron@lirmm.fr>
+# Copyright (C) 2018-2020 Stephane Caron <stephane.caron@normalesup.org>
 #
 # This file is part of pypoman <https://github.com/stephane-caron/pypoman>.
 #
 # pypoman is free software: you can redistribute it and/or modify it under the
-# terms of the GNU Lesser General Public License as published by the Free
-# Software Foundation, either version 3 of the License, or (at your option) any
-# later version.
+# terms of the GNU General Public License as published by the Free Software
+# Foundation, either version 3 of the License, or (at your option) any later
+# version.
 #
 # pypoman is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
-# A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more
-# details.
+# A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 #
-# You should have received a copy of the GNU Lesser General Public License
-# along with pypoman. If not, see <http://www.gnu.org/licenses/>.
+# You should have received a copy of the GNU General Public License along with
+# pypoman. If not, see <http://www.gnu.org/licenses/>.
 
-import cdd
+"""Functions to switch between halfspace and vertex representations."""
+
+from typing import List, Tuple, Union
 
-from numpy import array, hstack, ones, vstack, zeros
+import cdd
+import numpy as np
+from scipy.spatial import ConvexHull
 
 from .misc import norm
 
 
-def compute_cone_face_matrix(S):
-    """
-    Compute the face matrix of a polyhedral convex cone from its span matrix.
+def compute_cone_face_matrix(S: np.ndarray) -> np.ndarray:
+    r"""Compute the face matrix of a polyhedral cone from its span matrix.
 
     Parameters
     ----------
-    S : array, shape=(n, m)
-        Span matrix defining the cone as :math:`x = S \\lambda` with
-        :math:`\\lambda \\geq 0`.
+    S :
+        Span matrix defining the cone as :math:`x = S \lambda` with
+        :math:`\lambda \geq 0`.
 
     Returns
     -------
-    F : array, shape=(k, n)
+    :
         Face matrix defining the cone equivalently by :math:`F x \\leq 0`.
     """
-    V = vstack([
-        hstack([zeros((S.shape[1], 1)), S.T]),
-        hstack([1, zeros(S.shape[0])])])
+    V = np.vstack(
+        [
+            np.hstack([np.zeros((S.shape[1], 1)), S.T]),
+            np.hstack([1, np.zeros(S.shape[0])]),
+        ]
+    )
     # V-representation: first column is 0 for rays
-    mat = cdd.Matrix(V, number_type='float')
+    mat = cdd.Matrix(V, number_type="float")
     mat.rep_type = cdd.RepType.GENERATOR
     P = cdd.Polyhedron(mat)
     ineq = P.get_inequalities()
-    H = array(ineq)
+    H = np.array(ineq)
     if H.shape == (0,):  # H == []
         return H
     A = []
     for i in range(H.shape[0]):
         # H matrix is [b, -A] for A * x <= b
         if norm(H[i, 1:]) < 1e-10:
             continue
         elif abs(H[i, 0]) > 1e-10:  # b should be zero for a cone
             raise Exception("Polyhedron is not a cone")
         elif i not in ineq.lin_set:
             A.append(-H[i, 1:])
-    return array(A)
+    return np.array(A)
 
 
-def compute_polytope_halfspaces(vertices):
-    """
-    Compute the halfspace representation (H-rep) of a polytope defined as
-    convex hull of a set of vertices:
+def compute_polytope_halfspaces(
+    vertices: List[np.ndarray],
+) -> Union[np.ndarray, Tuple[np.ndarray, np.ndarray]]:
+    r"""Compute the halfspace representation (H-rep) of a polytope.
+
+    The polytope is defined as convex hull of a set of vertices:
 
     .. math::
 
-        A x \\leq b
-        \\quad \\Leftrightarrow \\quad
-        x \\in \\mathrm{conv}(\\mathrm{vertices})
+        A x \leq b
+        \quad \Leftrightarrow \quad
+        x \in \mathrm{conv}(\mathrm{vertices})
 
     Parameters
     ----------
-    vertices : list of arrays
+    vertices :
         List of polytope vertices.
 
     Returns
     -------
-    A : array, shape=(m, k)
-        Matrix of halfspace representation.
-    b : array, shape=(m,)
-        Vector of halfspace representation.
-    """
-    V = vstack(vertices)
-    t = ones((V.shape[0], 1))  # first column is 1 for vertices
-    tV = hstack([t, V])
-    mat = cdd.Matrix(tV, number_type='float')
+    :
+        Tuple ``(A, b)`` of the halfspace representation, or empty array if it
+        is empty.
+    """
+    V = np.vstack(vertices)
+    t = np.ones((V.shape[0], 1))  # first column is 1 for vertices
+    tV = np.hstack([t, V])
+    mat = cdd.Matrix(tV, number_type="float")
     mat.rep_type = cdd.RepType.GENERATOR
     P = cdd.Polyhedron(mat)
-    bA = array(P.get_inequalities())
+    bA = np.array(P.get_inequalities())
     if bA.shape == (0,):  # bA == []
         return bA
     # the polyhedron is given by b + A x >= 0 where bA = [b|A]
-    b, A = array(bA[:, 0]), -array(bA[:, 1:])
+    b, A = np.array(bA[:, 0]), -np.array(bA[:, 1:])
     return (A, b)
 
 
-def compute_polytope_vertices(A, b):
-    """
-    Compute the vertices of a polytope given in halfspace representation by
-    :math:`A x \\leq b`.
+def compute_polytope_vertices(
+    A: np.ndarray, b: np.ndarray
+) -> List[np.ndarray]:
+    r"""Compute the vertices of a polytope.
+
+    The polytope is given in halfspace representation by :math:`A x \leq b`.
 
     Parameters
     ----------
-    A : array, shape=(m, k)
+    A :
         Matrix of halfspace representation.
-    b : array, shape=(m,)
+    b :
         Vector of halfspace representation.
 
     Returns
     -------
-    vertices : list of arrays
+    :
         List of polytope vertices.
+
+    Notes
+    -----
+    This method won't work well if your halfspace representation includes
+    equality constraints :math:`A x = b` written as :math:`(A x \\leq b \\wedge
+    -A x \\leq -b)`. If this is your use case, consider using directly the
+    linear set ``lin_set`` of `equality-constraint generatorsin pycddlib
+    <https://pycddlib.readthedocs.io/en/latest/matrix.html>`_.
     """
     b = b.reshape((b.shape[0], 1))
-    mat = cdd.Matrix(hstack([b, -A]), number_type='float')
+    mat = cdd.Matrix(np.hstack([b, -A]), number_type="float")
     mat.rep_type = cdd.RepType.INEQUALITY
     P = cdd.Polyhedron(mat)
     g = P.get_generators()
-    V = array(g)
+    V = np.array(g)
     vertices = []
     for i in range(V.shape[0]):
         if V[i, 0] != 1:  # 1 = vertex, 0 = ray
             raise Exception("Polyhedron is not a polytope")
         elif i not in g.lin_set:
             vertices.append(V[i, 1:])
     return vertices
+
+
+def convex_hull(points: List[np.ndarray]) -> List[np.ndarray]:
+    """Compute the convex hull of a set of points.
+
+    Parameters
+    ----------
+    points :
+        Set of points.
+
+    Returns
+    -------
+    :
+        List of polytope vertices.
+    """
+    hull = ConvexHull(points)
+    return [points[i] for i in hull.vertices]
```

### Comparing `pypoman-0.5.4/pypoman/__init__.py` & `pypoman-0.6.0/pypoman/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,59 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2018 Stephane Caron <stephane.caron@lirmm.fr>
+# Copyright (C) 2018-2020 Stephane Caron <stephane.caron@normalesup.org>
 #
 # This file is part of pypoman <https://github.com/stephane-caron/pypoman>.
 #
 # pypoman is free software: you can redistribute it and/or modify it under the
-# terms of the GNU Lesser General Public License as published by the Free
-# Software Foundation, either version 3 of the License, or (at your option) any
-# later version.
+# terms of the GNU General Public License as published by the Free Software
+# Foundation, either version 3 of the License, or (at your option) any later
+# version.
 #
 # pypoman is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
-# A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more
-# details.
+# A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 #
-# You should have received a copy of the GNU Lesser General Public License
-# along with pypoman. If not, see <http://www.gnu.org/licenses/>.
+# You should have received a copy of the GNU General Public License along with
+# pypoman. If not, see <http://www.gnu.org/licenses/>.
 
-from .duality import compute_cone_face_matrix
-from .duality import compute_polytope_halfspaces
-from .duality import compute_polytope_vertices
-from .intersection import intersect_line_cylinder
-from .intersection import intersect_line_polygon
-from .intersection import intersect_polygons
+"""Python module for polyhedral geometry."""
+
+from .duality import (
+    compute_cone_face_matrix,
+    compute_polytope_halfspaces,
+    compute_polytope_vertices,
+    convex_hull,
+)
+from .intersection import (
+    intersect_line_cylinder,
+    intersect_line_polygon,
+    intersect_polygons,
+)
 from .lp import solve_lp
-from .polygon import compute_polygon_hull
-from .polygon import plot_polygon
-from .projection import project_polytope
-from .projection import project_polytope_bretl
+from .polygon import compute_polygon_hull, plot_polygon
+from .polyhedron import compute_chebyshev_center
+from .projection import (
+    project_point_to_polytope,
+    project_polytope,
+    project_polytope_bretl,
+)
+
+__version__ = "0.6.0"
 
 __all__ = [
-    'compute_cone_face_matrix',
-    'compute_polygon_hull',
-    'compute_polytope_halfspaces',
-    'compute_polytope_vertices',
-    'intersect_line_cylinder',
-    'intersect_line_polygon',
-    'intersect_polygons',
-    'plot_polygon',
-    'project_polytope',
-    'project_polytope_bretl',
-    'solve_lp',
+    "compute_chebyshev_center",
+    "compute_cone_face_matrix",
+    "compute_polygon_hull",
+    "compute_polytope_halfspaces",
+    "compute_polytope_vertices",
+    "convex_hull",
+    "intersect_line_cylinder",
+    "intersect_line_polygon",
+    "intersect_polygons",
+    "plot_polygon",
+    "project_polytope",
+    "project_polytope_bretl",
+    "project_point_to_polytope",
+    "solve_lp",
 ]
```

