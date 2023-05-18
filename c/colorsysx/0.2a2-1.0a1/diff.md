# Comparing `tmp/colorsysx-0.2a2.tar.gz` & `tmp/colorsysx-1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colorsysx-0.2a2.tar", last modified: Mon May 15 12:34:58 2023, max compression
+gzip compressed data, was "colorsysx-1.0a1.tar", last modified: Thu May 18 12:42:45 2023, max compression
```

## Comparing `colorsysx-0.2a2.tar` & `colorsysx-1.0a1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0      506 2023-05-13 17:41:09.960408 colorsysx-0.2a2/.github/workflows/python-package.yml
--rw-r--r--   0        0        0       53 2023-05-11 22:49:25.520127 colorsysx-0.2a2/.gitignore
--rw-r--r--   0        0        0    32422 2023-05-15 12:34:48.810921 colorsysx-0.2a2/LICENSE
--rw-r--r--   0        0        0     3191 2023-05-15 12:23:34.051206 colorsysx-0.2a2/README.md
--rw-r--r--   0        0        0     1448 2023-05-15 12:25:11.137654 colorsysx-0.2a2/colorsysx/__init__.py
--rw-r--r--   0        0        0     5553 2023-05-15 12:23:34.055206 colorsysx-0.2a2/colorsysx/_glhs.py
--rw-r--r--   0        0        0     4471 2023-05-15 12:23:34.055206 colorsysx-0.2a2/colorsysx/_hcy.py
--rw-r--r--   0        0        0      379 2023-05-11 02:07:41.913560 colorsysx-0.2a2/colorsysx/_helpers.py
--rw-r--r--   0        0        0      741 2023-05-13 16:25:55.939388 colorsysx-0.2a2/colorsysx/_swizzle.py
--rw-r--r--   0        0        0     2760 2023-05-13 16:30:36.870102 colorsysx-0.2a2/colorsysx/_yuv.py
--rw-r--r--   0        0        0     1807 2023-05-13 00:51:20.967395 colorsysx-0.2a2/colorsysx/weights.py
--rw-r--r--   0        0        0      688 2023-05-15 12:34:48.810921 colorsysx-0.2a2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-13 01:06:47.992623 colorsysx-0.2a2/tests/__init__.py
--rw-r--r--   0        0        0      319 2023-05-13 01:01:00.825464 colorsysx-0.2a2/tests/context.py
--rw-r--r--   0        0        0     5702 2023-05-15 12:23:34.055206 colorsysx-0.2a2/tests/test_glhs.py
--rw-r--r--   0        0        0     2677 2023-05-15 12:23:34.055206 colorsysx-0.2a2/tests/test_hcy.py
--rw-r--r--   0        0        0      592 2023-05-13 16:25:28.626827 colorsysx-0.2a2/tests/test_swizzle.py
--rw-r--r--   0        0        0      799 2023-05-13 01:05:35.215977 colorsysx-0.2a2/tests/test_weights.py
--rw-r--r--   0        0        0     1673 2023-05-13 01:06:48.008623 colorsysx-0.2a2/tests/test_yuv.py
--rw-r--r--   0        0        0      865 2023-05-13 19:25:52.937780 colorsysx-0.2a2/tox.ini
--rw-r--r--   0        0        0     3718 1970-01-01 00:00:00.000000 colorsysx-0.2a2/PKG-INFO
+-rw-r--r--   0        0        0      506 2023-05-13 17:41:09.960408 colorsysx-1.0a1/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0       53 2023-05-11 22:49:25.520127 colorsysx-1.0a1/.gitignore
+-rw-r--r--   0        0        0     1082 2023-05-15 12:35:15.890023 colorsysx-1.0a1/LICENSE
+-rw-r--r--   0        0        0     3186 2023-05-17 15:23:29.534628 colorsysx-1.0a1/README.md
+-rw-r--r--   0        0        0     1448 2023-05-18 12:41:04.379228 colorsysx-1.0a1/colorsysx/__init__.py
+-rw-r--r--   0        0        0     5566 2023-05-18 12:01:21.430173 colorsysx-1.0a1/colorsysx/_glhs.py
+-rw-r--r--   0        0        0     4482 2023-05-18 12:00:28.891978 colorsysx-1.0a1/colorsysx/_hcy.py
+-rw-r--r--   0        0        0      379 2023-05-11 02:07:41.913560 colorsysx-1.0a1/colorsysx/_helpers.py
+-rw-r--r--   0        0        0      741 2023-05-13 16:25:55.939388 colorsysx-1.0a1/colorsysx/_swizzle.py
+-rw-r--r--   0        0        0     2771 2023-05-18 11:59:52.814338 colorsysx-1.0a1/colorsysx/_yuv.py
+-rw-r--r--   0        0        0     2569 2023-05-18 12:10:16.947498 colorsysx-1.0a1/colorsysx/weights.py
+-rw-r--r--   0        0        0      819 2023-05-17 13:04:58.016321 colorsysx-1.0a1/pyproject.toml
+-rw-r--r--   0        0        0     1261 2023-05-17 13:04:58.016321 colorsysx-1.0a1/requirements.txt
+-rw-r--r--   0        0        0        0 2023-05-13 01:06:47.992623 colorsysx-1.0a1/tests/__init__.py
+-rw-r--r--   0        0        0      319 2023-05-13 01:01:00.825464 colorsysx-1.0a1/tests/context.py
+-rw-r--r--   0        0        0     5822 2023-05-18 12:07:06.124196 colorsysx-1.0a1/tests/test_glhs.py
+-rw-r--r--   0        0        0     2710 2023-05-18 12:06:33.075493 colorsysx-1.0a1/tests/test_hcy.py
+-rw-r--r--   0        0        0      592 2023-05-13 16:25:28.626827 colorsysx-1.0a1/tests/test_swizzle.py
+-rw-r--r--   0        0        0      860 2023-05-18 12:09:20.418639 colorsysx-1.0a1/tests/test_weights.py
+-rw-r--r--   0        0        0     1706 2023-05-18 12:07:20.784493 colorsysx-1.0a1/tests/test_yuv.py
+-rw-r--r--   0        0        0     1030 2023-05-18 12:41:04.371228 colorsysx-1.0a1/tox.ini
+-rw-r--r--   0        0        0     3975 1970-01-01 00:00:00.000000 colorsysx-1.0a1/PKG-INFO
```

### Comparing `colorsysx-0.2a2/README.md` & `colorsysx-1.0a1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ![PyPI](https://img.shields.io/pypi/v/colorsysx)
 ![GitHub](https://img.shields.io/github/license/achadwick/python-colorsysx)
 ![GitHub issues](https://img.shields.io/github/issues/achadwick/python-colorsysx)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/achadwick/python-colorsysx/python-package.yml?branch=main)
 
 # colorsysX
 
-🎨👁️ _Extra, human-relevant, colour spaces derived from RGB_
+🌈👁️ _Extra, human-relevant, colour spaces derived from RGB_
 
 This package extends the standard Python library's `colorsys` module
 with a few additional, useful, colour spaces. The models of colour
 provided here are simple, but relevant to human vision and the perceived
 lightness of different colour hues.
 
 ## Colour models
@@ -73,15 +73,15 @@
 
 ```sh
 # Run all standard tests in parallel on all available Pythons
 tox -p
 
 # Run the system version of Python interactively in a venv with
 # colorsysx available.
-tox -e py python
+tox -e repl
 ```
 
 The build system is [flit][8], and the project is PEP 621 and PEP 517
 compliant.
 
 [1]: https://en.wikipedia.org/wiki/YUV#Related_color_models
 [2]: https://chilliant.com/rgb2hsv.html
```

### Comparing `colorsysx-0.2a2/colorsysx/__init__.py` & `colorsysx-1.0a1/colorsysx/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 See the corresponding module help texts for further details about each
 model. All of the colour spaces added by this package can be
 parameterized to tune them for different tasks. See the
 colorsysx.weights module for details.
 
 """
 
-__version__ = "0.2a2"
+__version__ = "1.0a1"
 
 # Imports::
 
 # Import just the functions,
 # people wanting weights can import .weights submodule.
 from ._yuv import rgb_to_yuv, yuv_to_rgb  # noqa: F401
 from ._hcy import rgb_to_hcy, hcy_to_rgb  # noqa: F401
```

### Comparing `colorsysx-0.2a2/colorsysx/_glhs.py` & `colorsysx-1.0a1/colorsysx/_glhs.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from . import weights
 from ._helpers import clamp
 from . import _swizzle
 
 
 # Default values::
 
-DEFAULT_WEIGHTS_MIN2MAX = weights.W_MIN2MAX_HLS
+DEFAULT_WEIGHTS_MIN2MAX = weights.SortedComponentWeights.HLS
 
 
 # Conversion functions::
 
 def rgb_to_glhs(r, g, b, w_min2max=None, w_rgb=None):
     """Convert a colour from RGB to a model covered by GLHS.
```

### Comparing `colorsysx-0.2a2/colorsysx/_hcy.py` & `colorsysx-1.0a1/colorsysx/_hcy.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from . import weights
 from ._helpers import clamp
 from . import _swizzle
 
 
 # Default values::
 
-DEFAULT_WEIGHTS = weights.W_RGB_REC709
+DEFAULT_WEIGHTS = weights.ComponentWeights.REC709
 
 
 # Conversion functions::
 
 def rgb_to_hcy(r, g, b, w_rgb=None):
     """Converts from RGB to HCY.
```

### Comparing `colorsysx-0.2a2/colorsysx/_swizzle.py` & `colorsysx-1.0a1/colorsysx/_swizzle.py`

 * *Files identical despite different names*

### Comparing `colorsysx-0.2a2/colorsysx/_yuv.py` & `colorsysx-1.0a1/colorsysx/_yuv.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from . import weights
 from ._helpers import matmul
 from ._helpers import clamp
 
 
 # Default values::
 
-DEFAULT_WEIGHTS = weights.W_RGB_REC709
+DEFAULT_WEIGHTS = weights.ComponentWeights.REC709
 
 
 # Conversion functions::
 
 def rgb_to_yuv(r, g, b, w_rgb=None):
     """Convert RGB to YUV (YPbBr).
```

### Comparing `colorsysx-0.2a2/tests/test_glhs.py` & `colorsysx-1.0a1/tests/test_glhs.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 import itertools
 
 
 # Module vars::
 
 EPSILON = float_info.epsilon
 WEIGHTS_MIN2MAX = (
-    colorsysx.weights.W_MIN2MAX_HSI,
-    colorsysx.weights.W_MIN2MAX_HSV,
-    colorsysx.weights.W_MIN2MAX_HLS,
+    colorsysx.weights.SortedComponentWeights.HSI,
+    colorsysx.weights.SortedComponentWeights.HSV,
+    colorsysx.weights.SortedComponentWeights.HLS,
 )
 WEIGHTS_RGB = (
-    colorsysx.weights.W_RGB_REC601,
-    colorsysx.weights.W_RGB_REC709,
-    colorsysx.weights.W_RGB_REC2020,
+    colorsysx.weights.ComponentWeights.REC601,
+    colorsysx.weights.ComponentWeights.REC709,
+    colorsysx.weights.ComponentWeights.REC2020,
 )
 
 
 # Test funcs::
 
 def test_grey_is_grey_min2max():
     """Neutral grey is always neutral grey."""
@@ -141,36 +141,36 @@
     fudge = 1
     for rn, gn, bn in itertools.product(range(n+1), repeat=3):
         r, g, b = (rn/n, gn/n, bn/n)
 
         # "HLS" double hexcone model
         (gl1, gh1, gs1) = colorsysx.rgb_to_glhs(
             r, g, b,
-            w_min2max=colorsysx.weights.W_MIN2MAX_HLS,
+            w_min2max=colorsysx.weights.SortedComponentWeights.HLS,
         )
         (h1, l1, s1) = colorsys.rgb_to_hls(r, g, b)
         assert abs(gl1 - l1) <= EPSILON*fudge
         assert abs(gs1 - s1) <= EPSILON*fudge
         assert abs(gh1 - h1) <= EPSILON*fudge
 
         # "HSV" hexcone model
         (gl2, gh2, gs2) = colorsysx.rgb_to_glhs(
             r, g, b,
-            w_min2max=colorsysx.weights.W_MIN2MAX_HSV,
+            w_min2max=colorsysx.weights.SortedComponentWeights.HSV,
         )
         (h2, s2, v2) = colorsys.rgb_to_hsv(r, g, b)
         assert abs(gl2 - v2) <= EPSILON*fudge
         assert abs(gs2 - s2) <= EPSILON*fudge
         assert abs(gh2 - h2) <= EPSILON*fudge
 
         # "HCY" luma-based model
         (gl3, gh3, gs3) = colorsysx.rgb_to_glhs(
             r, g, b,
-            w_rgb=colorsysx.weights.W_RGB_REC709,
+            w_rgb=colorsysx.weights.ComponentWeights.REC709,
         )
         (h3, c3, y3) = colorsysx.rgb_to_hcy(
             r, g, b,
-            w_rgb=colorsysx.weights.W_RGB_REC709,
+            w_rgb=colorsysx.weights.ComponentWeights.REC709,
         )
         assert abs(gl3 - y3) <= EPSILON*fudge
         assert abs(gs3 - c3) <= EPSILON*fudge
         assert abs(gh3 - h3) <= EPSILON*fudge
```

### Comparing `colorsysx-0.2a2/tests/test_hcy.py` & `colorsysx-1.0a1/tests/test_hcy.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 import itertools
 
 
 # Module vars::
 
 EPSILON = float_info.epsilon
 WEIGHTS = (
-    colorsysx.weights.W_RGB_REC601,
-    colorsysx.weights.W_RGB_REC709,
-    colorsysx.weights.W_RGB_REC2020,
+    colorsysx.weights.ComponentWeights.REC601,
+    colorsysx.weights.ComponentWeights.REC709,
+    colorsysx.weights.ComponentWeights.REC2020,
 )
 
 
 # Test funcs::
 
 def test_grey_is_grey():
     """Neutral grey is always neutral grey."""
```

### Comparing `colorsysx-0.2a2/tests/test_swizzle.py` & `colorsysx-1.0a1/tests/test_swizzle.py`

 * *Files identical despite different names*

### Comparing `colorsysx-0.2a2/tests/test_yuv.py` & `colorsysx-1.0a1/tests/test_yuv.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 import itertools
 
 
 # Module vars::
 
 EPSILON = float_info.epsilon
 WEIGHTS = (
-    colorsysx.weights.W_RGB_REC601,
-    colorsysx.weights.W_RGB_REC709,
-    colorsysx.weights.W_RGB_REC2020,
+    colorsysx.weights.ComponentWeights.REC601,
+    colorsysx.weights.ComponentWeights.REC709,
+    colorsysx.weights.ComponentWeights.REC2020,
 )
 
 
 # Test funcs::
 
 def test_grey_is_grey():
     """Neutral grey is always neutral grey."""
```

### Comparing `colorsysx-0.2a2/PKG-INFO` & `colorsysx-1.0a1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 Metadata-Version: 2.1
 Name: colorsysx
-Version: 0.2a2
+Version: 1.0a1
 Summary: Extra, human-relevant, colour spaces derived from RGB.
+Author-email: Andrew Chadwick <a.t.chadwick@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Multimedia :: Graphics :: Presentation
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Dist: pytest >=7,<8 ; extra == "dev"
+Requires-Dist: flake8 >=6,<7 ; extra == "dev"
+Requires-Dist: pip-tools ; extra == "dev"
+Requires-Dist: pip-sync-faster ; extra == "dev"
+Requires-Dist: ptpython ; extra == "dev"
+Provides-Extra: dev
 
 ![PyPI](https://img.shields.io/pypi/v/colorsysx)
 ![GitHub](https://img.shields.io/github/license/achadwick/python-colorsysx)
 ![GitHub issues](https://img.shields.io/github/issues/achadwick/python-colorsysx)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/achadwick/python-colorsysx/python-package.yml?branch=main)
 
 # colorsysX
 
-🎨👁️ _Extra, human-relevant, colour spaces derived from RGB_
+🌈👁️ _Extra, human-relevant, colour spaces derived from RGB_
 
 This package extends the standard Python library's `colorsys` module
 with a few additional, useful, colour spaces. The models of colour
 provided here are simple, but relevant to human vision and the perceived
 lightness of different colour hues.
 
 ## Colour models
@@ -86,15 +93,15 @@
 
 ```sh
 # Run all standard tests in parallel on all available Pythons
 tox -p
 
 # Run the system version of Python interactively in a venv with
 # colorsysx available.
-tox -e py python
+tox -e repl
 ```
 
 The build system is [flit][8], and the project is PEP 621 and PEP 517
 compliant.
 
 [1]: https://en.wikipedia.org/wiki/YUV#Related_color_models
 [2]: https://chilliant.com/rgb2hsv.html
```

