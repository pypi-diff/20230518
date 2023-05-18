# Comparing `tmp/fbench-0.3.0.tar.gz` & `tmp/fbench-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fbench-0.3.0.tar", max compression
+gzip compressed data, was "fbench-1.0.0.tar", max compression
```

## Comparing `fbench-0.3.0.tar` & `fbench-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,12 @@
--rw-r--r--   0        0        0     1523 2023-04-30 22:43:45.211215 fbench-0.3.0/LICENSE
-drwxr-xr-x   0        0        0        0 2023-04-30 22:43:45.211215 fbench-0.3.0/LICENSES/
--rw-r--r--   0        0        0     1543 2023-04-30 22:43:45.211215 fbench-0.3.0/LICENSES/NUMPY_LICENSE
--rw-r--r--   0        0        0     1898 2023-04-30 22:43:45.211215 fbench-0.3.0/README.md
--rw-r--r--   0        0        0     1193 2023-04-30 22:45:22.364355 fbench-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      259 2023-04-30 22:43:45.235216 fbench-0.3.0/src/fbench/__init__.py
--rw-r--r--   0        0        0     1169 2023-04-30 22:43:45.235216 fbench-0.3.0/src/fbench/config.py
--rw-r--r--   0        0        0      199 2023-04-30 22:43:45.235216 fbench-0.3.0/src/fbench/exception.py
--rw-r--r--   0        0        0     3729 2023-04-30 22:43:45.235216 fbench-0.3.0/src/fbench/function.py
--rw-r--r--   0        0        0      573 2023-04-30 22:43:45.235216 fbench-0.3.0/src/fbench/structure.py
--rw-r--r--   0        0        0     1031 2023-04-30 22:43:45.235216 fbench-0.3.0/src/fbench/validation.py
--rw-r--r--   0        0        0     8060 2023-04-30 22:43:45.235216 fbench-0.3.0/src/fbench/visualization.py
--rw-r--r--   0        0        0     2703 1970-01-01 00:00:00.000000 fbench-0.3.0/setup.py
--rw-r--r--   0        0        0     2776 1970-01-01 00:00:00.000000 fbench-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1523 2023-05-18 18:39:30.529763 fbench-1.0.0/LICENSE
+drwxr-xr-x   0        0        0        0 2023-05-18 18:39:30.529763 fbench-1.0.0/LICENSES/
+-rw-r--r--   0        0        0     1543 2023-05-18 18:39:30.529763 fbench-1.0.0/LICENSES/NUMPY_LICENSE
+-rw-r--r--   0        0        0     2433 2023-05-18 18:39:30.529763 fbench-1.0.0/README.md
+-rw-r--r--   0        0        0     1193 2023-05-18 18:41:09.335842 fbench-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      206 2023-05-18 18:39:30.589763 fbench-1.0.0/src/fbench/__init__.py
+-rw-r--r--   0        0        0    10558 2023-05-18 18:39:30.589763 fbench-1.0.0/src/fbench/function.py
+-rw-r--r--   0        0        0      677 2023-05-18 18:39:30.589763 fbench-1.0.0/src/fbench/structure.py
+-rw-r--r--   0        0        0     1009 2023-05-18 18:39:30.589763 fbench-1.0.0/src/fbench/validation.py
+-rw-r--r--   0        0        0    25296 2023-05-18 18:39:30.589763 fbench-1.0.0/src/fbench/viz.py
+-rw-r--r--   0        0        0     3251 1970-01-01 00:00:00.000000 fbench-1.0.0/setup.py
+-rw-r--r--   0        0        0     3311 1970-01-01 00:00:00.000000 fbench-1.0.0/PKG-INFO
```

### Comparing `fbench-0.3.0/LICENSE` & `fbench-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fbench-0.3.0/LICENSES/NUMPY_LICENSE` & `fbench-1.0.0/LICENSES/NUMPY_LICENSE`

 * *Files identical despite different names*

### Comparing `fbench-0.3.0/README.md` & `fbench-1.0.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 ## About
 
 A collection of benchmark functions:
 
 - [Documentation](https://fbench.readthedocs.io/en/stable/index.html)
 - [Overview of fBench functions](https://fbench.readthedocs.io/en/stable/fBench-functions.html)
+- [Example usage](https://fbench.readthedocs.io/en/stable/example.html)
 - [API Reference](https://fbench.readthedocs.io/en/stable/autoapi/fbench/index.html)
 
 ## Installation
 
 `fbench` is available on [PyPI](https://pypi.org/project/fbench/) for Python 3.8+:
 
 ```console
@@ -30,14 +31,26 @@
 
 ```python
 >>> import fbench
 >>> round(fbench.ackley([1, 1]), 4)
 3.6254
 ```
 
+Visualize function with [`FunctionPlotter`](https://fbench.readthedocs.io/en/stable/autoapi/fbench/viz/index.html#fbench.viz.FunctionPlotter):
+
+```python
+>>> import matplotlib.pyplot as plt
+>>> plotter = fbench.viz.FunctionPlotter(func=fbench.ackley, bounds=[(-5, 5)] * 2)
+>>> plotter.plot()
+>>> plt.show()
+```
+<p align="left">
+<img src="https://raw.githubusercontent.com/estripling/fbench/main/images/readme-ackley.png" width="800" alt="Ackley function.">
+</p>
+
 ## Contributing to fBench
 
 Your contribution is greatly appreciated!
 See the following links to help you get started:
 
 - [Contributing Guide](https://fbench.readthedocs.io/en/latest/contributing.html)
 - [Developer Guide](https://fbench.readthedocs.io/en/latest/developers.html)
```

#### html2text {}

```diff
@@ -1,17 +1,24 @@
                              ****** fBench ******
                 [pypi] [docs] [ci_status] [coverage] [license]
 ## About A collection of benchmark functions: - [Documentation](https://
 fbench.readthedocs.io/en/stable/index.html) - [Overview of fBench functions]
-(https://fbench.readthedocs.io/en/stable/fBench-functions.html) - [API
-Reference](https://fbench.readthedocs.io/en/stable/autoapi/fbench/index.html)
-## Installation `fbench` is available on [PyPI](https://pypi.org/project/
-fbench/) for Python 3.8+: ```console pip install fbench ``` ## Examples The
-[`ackley`](https://fbench.readthedocs.io/en/stable/autoapi/fbench/
+(https://fbench.readthedocs.io/en/stable/fBench-functions.html) - [Example
+usage](https://fbench.readthedocs.io/en/stable/example.html) - [API Reference]
+(https://fbench.readthedocs.io/en/stable/autoapi/fbench/index.html) ##
+Installation `fbench` is available on [PyPI](https://pypi.org/project/fbench/
+) for Python 3.8+: ```console pip install fbench ``` ## Examples The [`ackley`]
+(https://fbench.readthedocs.io/en/stable/autoapi/fbench/
 index.html#fbench.ackley) function: ```python >>> import fbench >>> round
-(fbench.ackley([1, 1]), 4) 3.6254 ``` ## Contributing to fBench Your
-contribution is greatly appreciated! See the following links to help you get
-started: - [Contributing Guide](https://fbench.readthedocs.io/en/latest/
-contributing.html) - [Developer Guide](https://fbench.readthedocs.io/en/latest/
-developers.html) - [Contributor Code of Conduct](https://fbench.readthedocs.io/
-en/latest/conduct.html) ## License `fbench` was created by fBench Developers.
-It is licensed under the terms of the BSD 3-Clause license.
+(fbench.ackley([1, 1]), 4) 3.6254 ``` Visualize function with
+[`FunctionPlotter`](https://fbench.readthedocs.io/en/stable/autoapi/fbench/viz/
+index.html#fbench.viz.FunctionPlotter): ```python >>> import matplotlib.pyplot
+as plt >>> plotter = fbench.viz.FunctionPlotter(func=fbench.ackley, bounds=[(-
+5, 5)] * 2) >>> plotter.plot() >>> plt.show() ```
+[Ackley function.]
+## Contributing to fBench Your contribution is greatly appreciated! See the
+following links to help you get started: - [Contributing Guide](https://
+fbench.readthedocs.io/en/latest/contributing.html) - [Developer Guide](https://
+fbench.readthedocs.io/en/latest/developers.html) - [Contributor Code of
+Conduct](https://fbench.readthedocs.io/en/latest/conduct.html) ## License
+`fbench` was created by fBench Developers. It is licensed under the terms of
+the BSD 3-Clause license.
```

### Comparing `fbench-0.3.0/pyproject.toml` & `fbench-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fbench"
-version = "0.3.0"
+version = "1.0.0"
 description = "A collection of benchmark functions."
 authors = ["fBench Developers"]
 license = "BSD 3-Clause"
 readme = "README.md"
 repository = "https://github.com/estripling/fbench"
 documentation = "https://fbench.readthedocs.io/en/stable/"
 include = ["LICENSES/"]
```

### Comparing `fbench-0.3.0/setup.py` & `fbench-1.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 {'': ['*']}
 
 install_requires = \
 ['bumbag>=5.0.0,<6.0.0', 'matplotlib>=3.7.1,<4.0.0', 'numpy>=1.24.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'fbench',
-    'version': '0.3.0',
+    'version': '1.0.0',
     'description': 'A collection of benchmark functions.',
-    'long_description': '<h1 align="center">fBench</h1>\n\n<p align="center">\n<a href="https://pypi.org/project/fbench"><img alt="pypi" src="https://img.shields.io/pypi/v/fbench"></a>\n<a href="https://readthedocs.org/projects/fbench/?badge=latest"><img alt="docs" src="https://readthedocs.org/projects/fbench/badge/?version=latest"></a>\n<a href="https://github.com/estripling/fbench/actions/workflows/ci.yml"><img alt="ci status" src="https://github.com/estripling/fbench/actions/workflows/ci.yml/badge.svg?branch=main"></a>\n<a href="https://codecov.io/gh/estripling/fbench"><img alt="coverage" src="https://codecov.io/github/estripling/fbench/coverage.svg?branch=main"></a>\n<a href="https://github.com/estripling/fbench/blob/main/LICENSE"><img alt="license" src="https://img.shields.io/pypi/l/fbench"></a>\n</p>\n\n## About\n\nA collection of benchmark functions:\n\n- [Documentation](https://fbench.readthedocs.io/en/stable/index.html)\n- [Overview of fBench functions](https://fbench.readthedocs.io/en/stable/fBench-functions.html)\n- [API Reference](https://fbench.readthedocs.io/en/stable/autoapi/fbench/index.html)\n\n## Installation\n\n`fbench` is available on [PyPI](https://pypi.org/project/fbench/) for Python 3.8+:\n\n```console\npip install fbench\n```\n\n## Examples\n\nThe [`ackley`](https://fbench.readthedocs.io/en/stable/autoapi/fbench/index.html#fbench.ackley) function:\n\n```python\n>>> import fbench\n>>> round(fbench.ackley([1, 1]), 4)\n3.6254\n```\n\n## Contributing to fBench\n\nYour contribution is greatly appreciated!\nSee the following links to help you get started:\n\n- [Contributing Guide](https://fbench.readthedocs.io/en/latest/contributing.html)\n- [Developer Guide](https://fbench.readthedocs.io/en/latest/developers.html)\n- [Contributor Code of Conduct](https://fbench.readthedocs.io/en/latest/conduct.html)\n\n## License\n\n`fbench` was created by fBench Developers.\nIt is licensed under the terms of the BSD 3-Clause license.\n',
+    'long_description': '<h1 align="center">fBench</h1>\n\n<p align="center">\n<a href="https://pypi.org/project/fbench"><img alt="pypi" src="https://img.shields.io/pypi/v/fbench"></a>\n<a href="https://readthedocs.org/projects/fbench/?badge=latest"><img alt="docs" src="https://readthedocs.org/projects/fbench/badge/?version=latest"></a>\n<a href="https://github.com/estripling/fbench/actions/workflows/ci.yml"><img alt="ci status" src="https://github.com/estripling/fbench/actions/workflows/ci.yml/badge.svg?branch=main"></a>\n<a href="https://codecov.io/gh/estripling/fbench"><img alt="coverage" src="https://codecov.io/github/estripling/fbench/coverage.svg?branch=main"></a>\n<a href="https://github.com/estripling/fbench/blob/main/LICENSE"><img alt="license" src="https://img.shields.io/pypi/l/fbench"></a>\n</p>\n\n## About\n\nA collection of benchmark functions:\n\n- [Documentation](https://fbench.readthedocs.io/en/stable/index.html)\n- [Overview of fBench functions](https://fbench.readthedocs.io/en/stable/fBench-functions.html)\n- [Example usage](https://fbench.readthedocs.io/en/stable/example.html)\n- [API Reference](https://fbench.readthedocs.io/en/stable/autoapi/fbench/index.html)\n\n## Installation\n\n`fbench` is available on [PyPI](https://pypi.org/project/fbench/) for Python 3.8+:\n\n```console\npip install fbench\n```\n\n## Examples\n\nThe [`ackley`](https://fbench.readthedocs.io/en/stable/autoapi/fbench/index.html#fbench.ackley) function:\n\n```python\n>>> import fbench\n>>> round(fbench.ackley([1, 1]), 4)\n3.6254\n```\n\nVisualize function with [`FunctionPlotter`](https://fbench.readthedocs.io/en/stable/autoapi/fbench/viz/index.html#fbench.viz.FunctionPlotter):\n\n```python\n>>> import matplotlib.pyplot as plt\n>>> plotter = fbench.viz.FunctionPlotter(func=fbench.ackley, bounds=[(-5, 5)] * 2)\n>>> plotter.plot()\n>>> plt.show()\n```\n<p align="left">\n<img src="https://raw.githubusercontent.com/estripling/fbench/main/images/readme-ackley.png" width="800" alt="Ackley function.">\n</p>\n\n## Contributing to fBench\n\nYour contribution is greatly appreciated!\nSee the following links to help you get started:\n\n- [Contributing Guide](https://fbench.readthedocs.io/en/latest/contributing.html)\n- [Developer Guide](https://fbench.readthedocs.io/en/latest/developers.html)\n- [Contributor Code of Conduct](https://fbench.readthedocs.io/en/latest/conduct.html)\n\n## License\n\n`fbench` was created by fBench Developers.\nIt is licensed under the terms of the BSD 3-Clause license.\n',
     'author': 'fBench Developers',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/estripling/fbench',
     'package_dir': package_dir,
     'packages': packages,
```

#### html2text {}

```diff
@@ -1,26 +1,33 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['fbench'] package_data = \ {'': ['*']} install_requires =
 \ ['bumbag>=5.0.0,<6.0.0', 'matplotlib>=3.7.1,<4.0.0', 'numpy>=1.24.2,<2.0.0']
-setup_kwargs = { 'name': 'fbench', 'version': '0.3.0', 'description': 'A
+setup_kwargs = { 'name': 'fbench', 'version': '1.0.0', 'description': 'A
 collection of benchmark functions.', 'long_description': '
                              ****** fBench ******
 \n\n
             \n[pypi]\n[docs]\n[ci_status]\n[coverage]\n[license]\n
 \n\n## About\n\nA collection of benchmark functions:\n\n- [Documentation]
 (https://fbench.readthedocs.io/en/stable/index.html)\n- [Overview of fBench
 functions](https://fbench.readthedocs.io/en/stable/fBench-functions.html)\n-
-[API Reference](https://fbench.readthedocs.io/en/stable/autoapi/fbench/
+[Example usage](https://fbench.readthedocs.io/en/stable/example.html)\n- [API
+Reference](https://fbench.readthedocs.io/en/stable/autoapi/fbench/
 index.html)\n\n## Installation\n\n`fbench` is available on [PyPI](https://
 pypi.org/project/fbench/) for Python 3.8+:\n\n```console\npip install
 fbench\n```\n\n## Examples\n\nThe [`ackley`](https://fbench.readthedocs.io/en/
 stable/autoapi/fbench/index.html#fbench.ackley) function:\n\n```python\n>>>
-import fbench\n>>> round(fbench.ackley([1, 1]), 4)\n3.6254\n```\n\n##
-Contributing to fBench\n\nYour contribution is greatly appreciated!\nSee the
-following links to help you get started:\n\n- [Contributing Guide](https://
+import fbench\n>>> round(fbench.ackley([1, 1]), 4)\n3.6254\n```\n\nVisualize
+function with [`FunctionPlotter`](https://fbench.readthedocs.io/en/stable/
+autoapi/fbench/viz/index.html#fbench.viz.FunctionPlotter):\n\n```python\n>>>
+import matplotlib.pyplot as plt\n>>> plotter = fbench.viz.FunctionPlotter
+(func=fbench.ackley, bounds=[(-5, 5)] * 2)\n>>> plotter.plot()\n>>> plt.show
+()\n```\n
+\n[Ackley function.]\n
+\n\n## Contributing to fBench\n\nYour contribution is greatly appreciated!\nSee
+the following links to help you get started:\n\n- [Contributing Guide](https://
 fbench.readthedocs.io/en/latest/contributing.html)\n- [Developer Guide](https:/
 /fbench.readthedocs.io/en/latest/developers.html)\n- [Contributor Code of
 Conduct](https://fbench.readthedocs.io/en/latest/conduct.html)\n\n##
 License\n\n`fbench` was created by fBench Developers.\nIt is licensed under the
 terms of the BSD 3-Clause license.\n', 'author': 'fBench Developers',
 'author_email': 'None', 'maintainer': 'None', 'maintainer_email': 'None',
 'url': 'https://github.com/estripling/fbench', 'package_dir': package_dir,
```

### Comparing `fbench-0.3.0/PKG-INFO` & `fbench-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fbench
-Version: 0.3.0
+Version: 1.0.0
 Summary: A collection of benchmark functions.
 Home-page: https://github.com/estripling/fbench
 License: BSD 3-Clause
 Keywords: fbench
 Author: fBench Developers
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
@@ -33,14 +33,15 @@
 
 ## About
 
 A collection of benchmark functions:
 
 - [Documentation](https://fbench.readthedocs.io/en/stable/index.html)
 - [Overview of fBench functions](https://fbench.readthedocs.io/en/stable/fBench-functions.html)
+- [Example usage](https://fbench.readthedocs.io/en/stable/example.html)
 - [API Reference](https://fbench.readthedocs.io/en/stable/autoapi/fbench/index.html)
 
 ## Installation
 
 `fbench` is available on [PyPI](https://pypi.org/project/fbench/) for Python 3.8+:
 
 ```console
@@ -53,14 +54,26 @@
 
 ```python
 >>> import fbench
 >>> round(fbench.ackley([1, 1]), 4)
 3.6254
 ```
 
+Visualize function with [`FunctionPlotter`](https://fbench.readthedocs.io/en/stable/autoapi/fbench/viz/index.html#fbench.viz.FunctionPlotter):
+
+```python
+>>> import matplotlib.pyplot as plt
+>>> plotter = fbench.viz.FunctionPlotter(func=fbench.ackley, bounds=[(-5, 5)] * 2)
+>>> plotter.plot()
+>>> plt.show()
+```
+<p align="left">
+<img src="https://raw.githubusercontent.com/estripling/fbench/main/images/readme-ackley.png" width="800" alt="Ackley function.">
+</p>
+
 ## Contributing to fBench
 
 Your contribution is greatly appreciated!
 See the following links to help you get started:
 
 - [Contributing Guide](https://fbench.readthedocs.io/en/latest/contributing.html)
 - [Developer Guide](https://fbench.readthedocs.io/en/latest/developers.html)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fbench Version: 0.3.0 Summary: A collection of
+Metadata-Version: 2.1 Name: fbench Version: 1.0.0 Summary: A collection of
 benchmark functions. Home-page: https://github.com/estripling/fbench License:
 BSD 3-Clause Keywords: fbench Author: fBench Developers Requires-Python:
 >=3.8,<4.0 Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3 Requires-Dist:
@@ -10,20 +10,27 @@
 Dist: numpy (>=1.24.2,<2.0.0) Project-URL: Documentation, https://
 fbench.readthedocs.io/en/stable/ Project-URL: Repository, https://github.com/
 estripling/fbench Description-Content-Type: text/markdown
                              ****** fBench ******
                 [pypi] [docs] [ci_status] [coverage] [license]
 ## About A collection of benchmark functions: - [Documentation](https://
 fbench.readthedocs.io/en/stable/index.html) - [Overview of fBench functions]
-(https://fbench.readthedocs.io/en/stable/fBench-functions.html) - [API
-Reference](https://fbench.readthedocs.io/en/stable/autoapi/fbench/index.html)
-## Installation `fbench` is available on [PyPI](https://pypi.org/project/
-fbench/) for Python 3.8+: ```console pip install fbench ``` ## Examples The
-[`ackley`](https://fbench.readthedocs.io/en/stable/autoapi/fbench/
+(https://fbench.readthedocs.io/en/stable/fBench-functions.html) - [Example
+usage](https://fbench.readthedocs.io/en/stable/example.html) - [API Reference]
+(https://fbench.readthedocs.io/en/stable/autoapi/fbench/index.html) ##
+Installation `fbench` is available on [PyPI](https://pypi.org/project/fbench/
+) for Python 3.8+: ```console pip install fbench ``` ## Examples The [`ackley`]
+(https://fbench.readthedocs.io/en/stable/autoapi/fbench/
 index.html#fbench.ackley) function: ```python >>> import fbench >>> round
-(fbench.ackley([1, 1]), 4) 3.6254 ``` ## Contributing to fBench Your
-contribution is greatly appreciated! See the following links to help you get
-started: - [Contributing Guide](https://fbench.readthedocs.io/en/latest/
-contributing.html) - [Developer Guide](https://fbench.readthedocs.io/en/latest/
-developers.html) - [Contributor Code of Conduct](https://fbench.readthedocs.io/
-en/latest/conduct.html) ## License `fbench` was created by fBench Developers.
-It is licensed under the terms of the BSD 3-Clause license.
+(fbench.ackley([1, 1]), 4) 3.6254 ``` Visualize function with
+[`FunctionPlotter`](https://fbench.readthedocs.io/en/stable/autoapi/fbench/viz/
+index.html#fbench.viz.FunctionPlotter): ```python >>> import matplotlib.pyplot
+as plt >>> plotter = fbench.viz.FunctionPlotter(func=fbench.ackley, bounds=[(-
+5, 5)] * 2) >>> plotter.plot() >>> plt.show() ```
+[Ackley function.]
+## Contributing to fBench Your contribution is greatly appreciated! See the
+following links to help you get started: - [Contributing Guide](https://
+fbench.readthedocs.io/en/latest/contributing.html) - [Developer Guide](https://
+fbench.readthedocs.io/en/latest/developers.html) - [Contributor Code of
+Conduct](https://fbench.readthedocs.io/en/latest/conduct.html) ## License
+`fbench` was created by fBench Developers. It is licensed under the terms of
+the BSD 3-Clause license.
```

