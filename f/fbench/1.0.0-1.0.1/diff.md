# Comparing `tmp/fbench-1.0.0.tar.gz` & `tmp/fbench-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fbench-1.0.0.tar", max compression
+gzip compressed data, was "fbench-1.0.1.tar", max compression
```

## Comparing `fbench-1.0.0.tar` & `fbench-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1523 2023-05-18 18:39:30.529763 fbench-1.0.0/LICENSE
-drwxr-xr-x   0        0        0        0 2023-05-18 18:39:30.529763 fbench-1.0.0/LICENSES/
--rw-r--r--   0        0        0     1543 2023-05-18 18:39:30.529763 fbench-1.0.0/LICENSES/NUMPY_LICENSE
--rw-r--r--   0        0        0     2433 2023-05-18 18:39:30.529763 fbench-1.0.0/README.md
--rw-r--r--   0        0        0     1193 2023-05-18 18:41:09.335842 fbench-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      206 2023-05-18 18:39:30.589763 fbench-1.0.0/src/fbench/__init__.py
--rw-r--r--   0        0        0    10558 2023-05-18 18:39:30.589763 fbench-1.0.0/src/fbench/function.py
--rw-r--r--   0        0        0      677 2023-05-18 18:39:30.589763 fbench-1.0.0/src/fbench/structure.py
--rw-r--r--   0        0        0     1009 2023-05-18 18:39:30.589763 fbench-1.0.0/src/fbench/validation.py
--rw-r--r--   0        0        0    25296 2023-05-18 18:39:30.589763 fbench-1.0.0/src/fbench/viz.py
--rw-r--r--   0        0        0     3251 1970-01-01 00:00:00.000000 fbench-1.0.0/setup.py
--rw-r--r--   0        0        0     3311 1970-01-01 00:00:00.000000 fbench-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1523 2023-05-18 19:10:39.499642 fbench-1.0.1/LICENSE
+drwxr-xr-x   0        0        0        0 2023-05-18 19:10:39.499642 fbench-1.0.1/LICENSES/
+-rw-r--r--   0        0        0     1543 2023-05-18 19:10:39.499642 fbench-1.0.1/LICENSES/NUMPY_LICENSE
+-rw-r--r--   0        0        0     2433 2023-05-18 19:10:39.499642 fbench-1.0.1/README.md
+-rw-r--r--   0        0        0     1193 2023-05-18 19:12:20.944723 fbench-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      206 2023-05-18 19:10:39.551642 fbench-1.0.1/src/fbench/__init__.py
+-rw-r--r--   0        0        0    10606 2023-05-18 19:10:39.551642 fbench-1.0.1/src/fbench/function.py
+-rw-r--r--   0        0        0      677 2023-05-18 19:10:39.551642 fbench-1.0.1/src/fbench/structure.py
+-rw-r--r--   0        0        0     1009 2023-05-18 19:10:39.551642 fbench-1.0.1/src/fbench/validation.py
+-rw-r--r--   0        0        0    25296 2023-05-18 19:10:39.551642 fbench-1.0.1/src/fbench/viz.py
+-rw-r--r--   0        0        0     3251 1970-01-01 00:00:00.000000 fbench-1.0.1/setup.py
+-rw-r--r--   0        0        0     3311 1970-01-01 00:00:00.000000 fbench-1.0.1/PKG-INFO
```

### Comparing `fbench-1.0.0/LICENSE` & `fbench-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fbench-1.0.0/LICENSES/NUMPY_LICENSE` & `fbench-1.0.1/LICENSES/NUMPY_LICENSE`

 * *Files identical despite different names*

### Comparing `fbench-1.0.0/README.md` & `fbench-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `fbench-1.0.0/pyproject.toml` & `fbench-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fbench"
-version = "1.0.0"
+version = "1.0.1"
 description = "A collection of benchmark functions."
 authors = ["fBench Developers"]
 license = "BSD 3-Clause"
 readme = "README.md"
 repository = "https://github.com/estripling/fbench"
 documentation = "https://fbench.readthedocs.io/en/stable/"
 include = ["LICENSES/"]
```

### Comparing `fbench-1.0.0/src/fbench/function.py` & `fbench-1.0.1/src/fbench/function.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     )
 
 
 def beale(x, /):
     """Beale function.
 
     A function :math:`f\\colon \\mathbb{R}^{2} \\rightarrow \\mathbb{R}`
-    that takes an :math:`2`-vector as input and returns a scalar value.
+    that takes a :math:`2`-vector as input and returns a scalar value.
 
     .. math::
 
        f(\\mathbf{x}) =
        \\left( 1.5 - x_{1} + x_{1} x_{2} \\right)^{2}
        + \\left( 2.25 - x_{1} + x_{1} x_{2}^{2} \\right)^{2}
        + \\left( 2.625 - x_{1} + x_{1} x_{2}^{3}\\right)^{2}
@@ -138,17 +138,20 @@
         Optima with specified dimension for fBench function if defined.
 
     Notes
     -----
     - Function is curried.
     - Optima are defined for the following functions:
         - ackley
+        - beale
         - peaks
         - rastrigin
         - rosenbrock
+        - schwefel
+        - sinc
         - sphere
 
     Examples
     --------
     >>> import fbench
     >>> optima = fbench.get_optima(5, fbench.sphere)
     >>> optima
@@ -184,15 +187,15 @@
     return optima.get(func, None)
 
 
 def peaks(x, /):
     """Peaks function.
 
     A function :math:`f\\colon \\mathbb{R}^{2} \\rightarrow \\mathbb{R}`
-    that takes an :math:`2`-vector as input and returns a scalar value.
+    that takes a :math:`2`-vector as input and returns a scalar value.
 
     .. math::
 
        f(\\mathbf{x}) =
        3 (1 - x_{1})^{2}
          \\exp\\left( - x_{1}^{2} - (x_{2} + 1)^{2} \\right)
        - 10 \\left( \\frac{x_{1}}{5} - x_{1}^{3} - x_{2}^{5} \\right)
```

### Comparing `fbench-1.0.0/src/fbench/structure.py` & `fbench-1.0.1/src/fbench/structure.py`

 * *Files identical despite different names*

### Comparing `fbench-1.0.0/src/fbench/validation.py` & `fbench-1.0.1/src/fbench/validation.py`

 * *Files identical despite different names*

### Comparing `fbench-1.0.0/src/fbench/viz.py` & `fbench-1.0.1/src/fbench/viz.py`

 * *Files identical despite different names*

### Comparing `fbench-1.0.0/setup.py` & `fbench-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['bumbag>=5.0.0,<6.0.0', 'matplotlib>=3.7.1,<4.0.0', 'numpy>=1.24.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'fbench',
-    'version': '1.0.0',
+    'version': '1.0.1',
     'description': 'A collection of benchmark functions.',
     'long_description': '<h1 align="center">fBench</h1>\n\n<p align="center">\n<a href="https://pypi.org/project/fbench"><img alt="pypi" src="https://img.shields.io/pypi/v/fbench"></a>\n<a href="https://readthedocs.org/projects/fbench/?badge=latest"><img alt="docs" src="https://readthedocs.org/projects/fbench/badge/?version=latest"></a>\n<a href="https://github.com/estripling/fbench/actions/workflows/ci.yml"><img alt="ci status" src="https://github.com/estripling/fbench/actions/workflows/ci.yml/badge.svg?branch=main"></a>\n<a href="https://codecov.io/gh/estripling/fbench"><img alt="coverage" src="https://codecov.io/github/estripling/fbench/coverage.svg?branch=main"></a>\n<a href="https://github.com/estripling/fbench/blob/main/LICENSE"><img alt="license" src="https://img.shields.io/pypi/l/fbench"></a>\n</p>\n\n## About\n\nA collection of benchmark functions:\n\n- [Documentation](https://fbench.readthedocs.io/en/stable/index.html)\n- [Overview of fBench functions](https://fbench.readthedocs.io/en/stable/fBench-functions.html)\n- [Example usage](https://fbench.readthedocs.io/en/stable/example.html)\n- [API Reference](https://fbench.readthedocs.io/en/stable/autoapi/fbench/index.html)\n\n## Installation\n\n`fbench` is available on [PyPI](https://pypi.org/project/fbench/) for Python 3.8+:\n\n```console\npip install fbench\n```\n\n## Examples\n\nThe [`ackley`](https://fbench.readthedocs.io/en/stable/autoapi/fbench/index.html#fbench.ackley) function:\n\n```python\n>>> import fbench\n>>> round(fbench.ackley([1, 1]), 4)\n3.6254\n```\n\nVisualize function with [`FunctionPlotter`](https://fbench.readthedocs.io/en/stable/autoapi/fbench/viz/index.html#fbench.viz.FunctionPlotter):\n\n```python\n>>> import matplotlib.pyplot as plt\n>>> plotter = fbench.viz.FunctionPlotter(func=fbench.ackley, bounds=[(-5, 5)] * 2)\n>>> plotter.plot()\n>>> plt.show()\n```\n<p align="left">\n<img src="https://raw.githubusercontent.com/estripling/fbench/main/images/readme-ackley.png" width="800" alt="Ackley function.">\n</p>\n\n## Contributing to fBench\n\nYour contribution is greatly appreciated!\nSee the following links to help you get started:\n\n- [Contributing Guide](https://fbench.readthedocs.io/en/latest/contributing.html)\n- [Developer Guide](https://fbench.readthedocs.io/en/latest/developers.html)\n- [Contributor Code of Conduct](https://fbench.readthedocs.io/en/latest/conduct.html)\n\n## License\n\n`fbench` was created by fBench Developers.\nIt is licensed under the terms of the BSD 3-Clause license.\n',
     'author': 'fBench Developers',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/estripling/fbench',
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['fbench'] package_data = \ {'': ['*']} install_requires =
 \ ['bumbag>=5.0.0,<6.0.0', 'matplotlib>=3.7.1,<4.0.0', 'numpy>=1.24.2,<2.0.0']
-setup_kwargs = { 'name': 'fbench', 'version': '1.0.0', 'description': 'A
+setup_kwargs = { 'name': 'fbench', 'version': '1.0.1', 'description': 'A
 collection of benchmark functions.', 'long_description': '
                              ****** fBench ******
 \n\n
             \n[pypi]\n[docs]\n[ci_status]\n[coverage]\n[license]\n
 \n\n## About\n\nA collection of benchmark functions:\n\n- [Documentation]
 (https://fbench.readthedocs.io/en/stable/index.html)\n- [Overview of fBench
 functions](https://fbench.readthedocs.io/en/stable/fBench-functions.html)\n-
```

### Comparing `fbench-1.0.0/PKG-INFO` & `fbench-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fbench
-Version: 1.0.0
+Version: 1.0.1
 Summary: A collection of benchmark functions.
 Home-page: https://github.com/estripling/fbench
 License: BSD 3-Clause
 Keywords: fbench
 Author: fBench Developers
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fbench Version: 1.0.0 Summary: A collection of
+Metadata-Version: 2.1 Name: fbench Version: 1.0.1 Summary: A collection of
 benchmark functions. Home-page: https://github.com/estripling/fbench License:
 BSD 3-Clause Keywords: fbench Author: fBench Developers Requires-Python:
 >=3.8,<4.0 Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3 Requires-Dist:
```

