# Comparing `tmp/colorsysx-1.0.tar.gz` & `tmp/colorsysx-1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colorsysx-1.0.tar", last modified: Thu May 18 19:13:44 2023, max compression
+gzip compressed data, was "colorsysx-1.0a1.tar", last modified: Thu May 18 12:42:45 2023, max compression
```

## Comparing `colorsysx-1.0.tar` & `colorsysx-1.0a1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      506 2023-05-18 19:10:02.291178 colorsysx-1.0/.github/workflows/python-package.yml
--rw-r--r--   0        0        0       53 2023-05-18 19:10:02.291178 colorsysx-1.0/.gitignore
--rw-r--r--   0        0        0     1082 2023-05-18 19:10:02.295178 colorsysx-1.0/LICENSE
--rw-r--r--   0        0        0     3186 2023-05-18 19:10:02.295178 colorsysx-1.0/README.md
--rw-r--r--   0        0        0     1446 2023-05-18 19:11:52.819679 colorsysx-1.0/colorsysx/__init__.py
--rw-r--r--   0        0        0     5566 2023-05-18 19:10:02.295178 colorsysx-1.0/colorsysx/_glhs.py
--rw-r--r--   0        0        0     4482 2023-05-18 19:10:02.295178 colorsysx-1.0/colorsysx/_hcy.py
--rw-r--r--   0        0        0      379 2023-05-18 19:10:02.295178 colorsysx-1.0/colorsysx/_helpers.py
--rw-r--r--   0        0        0      741 2023-05-18 19:10:02.303178 colorsysx-1.0/colorsysx/_swizzle.py
--rw-r--r--   0        0        0     2771 2023-05-18 19:10:02.303178 colorsysx-1.0/colorsysx/_yuv.py
--rw-r--r--   0        0        0     2569 2023-05-18 19:10:02.307178 colorsysx-1.0/colorsysx/weights.py
--rw-r--r--   0        0        0      819 2023-05-18 19:10:02.307178 colorsysx-1.0/pyproject.toml
--rw-r--r--   0        0        0     1261 2023-05-18 19:10:02.307178 colorsysx-1.0/requirements.txt
--rw-r--r--   0        0        0        0 2023-05-18 19:10:02.307178 colorsysx-1.0/tests/__init__.py
--rw-r--r--   0        0        0      319 2023-05-18 19:10:02.307178 colorsysx-1.0/tests/context.py
--rw-r--r--   0        0        0     5822 2023-05-18 19:10:02.307178 colorsysx-1.0/tests/test_glhs.py
--rw-r--r--   0        0        0     2710 2023-05-18 19:10:02.307178 colorsysx-1.0/tests/test_hcy.py
--rw-r--r--   0        0        0      592 2023-05-18 19:10:02.307178 colorsysx-1.0/tests/test_swizzle.py
--rw-r--r--   0        0        0      860 2023-05-18 19:10:02.307178 colorsysx-1.0/tests/test_weights.py
--rw-r--r--   0        0        0     1706 2023-05-18 19:10:02.307178 colorsysx-1.0/tests/test_yuv.py
--rw-r--r--   0        0        0     1030 2023-05-18 19:10:02.311179 colorsysx-1.0/tox.ini
--rw-r--r--   0        0        0     3973 1970-01-01 00:00:00.000000 colorsysx-1.0/PKG-INFO
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

### Comparing `colorsysx-1.0/LICENSE` & `colorsysx-1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `colorsysx-1.0/README.md` & `colorsysx-1.0a1/README.md`

 * *Files identical despite different names*

### Comparing `colorsysx-1.0/colorsysx/__init__.py` & `colorsysx-1.0a1/colorsysx/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 See the corresponding module help texts for further details about each
 model. All of the colour spaces added by this package can be
 parameterized to tune them for different tasks. See the
 colorsysx.weights module for details.
 
 """
 
-__version__ = "1.0"
+__version__ = "1.0a1"
 
 # Imports::
 
 # Import just the functions,
 # people wanting weights can import .weights submodule.
 from ._yuv import rgb_to_yuv, yuv_to_rgb  # noqa: F401
 from ._hcy import rgb_to_hcy, hcy_to_rgb  # noqa: F401
```

### Comparing `colorsysx-1.0/colorsysx/_glhs.py` & `colorsysx-1.0a1/colorsysx/_glhs.py`

 * *Files identical despite different names*

### Comparing `colorsysx-1.0/colorsysx/_hcy.py` & `colorsysx-1.0a1/colorsysx/_hcy.py`

 * *Files identical despite different names*

### Comparing `colorsysx-1.0/colorsysx/_swizzle.py` & `colorsysx-1.0a1/colorsysx/_swizzle.py`

 * *Files identical despite different names*

### Comparing `colorsysx-1.0/colorsysx/_yuv.py` & `colorsysx-1.0a1/colorsysx/_yuv.py`

 * *Files identical despite different names*

### Comparing `colorsysx-1.0/colorsysx/weights.py` & `colorsysx-1.0a1/colorsysx/weights.py`

 * *Files identical despite different names*

### Comparing `colorsysx-1.0/pyproject.toml` & `colorsysx-1.0a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `colorsysx-1.0/requirements.txt` & `colorsysx-1.0a1/requirements.txt`

 * *Files identical despite different names*

### Comparing `colorsysx-1.0/tests/test_glhs.py` & `colorsysx-1.0a1/tests/test_glhs.py`

 * *Files identical despite different names*

### Comparing `colorsysx-1.0/tests/test_hcy.py` & `colorsysx-1.0a1/tests/test_hcy.py`

 * *Files identical despite different names*

### Comparing `colorsysx-1.0/tests/test_swizzle.py` & `colorsysx-1.0a1/tests/test_swizzle.py`

 * *Files identical despite different names*

### Comparing `colorsysx-1.0/tests/test_weights.py` & `colorsysx-1.0a1/tests/test_weights.py`

 * *Files identical despite different names*

### Comparing `colorsysx-1.0/tests/test_yuv.py` & `colorsysx-1.0a1/tests/test_yuv.py`

 * *Files identical despite different names*

### Comparing `colorsysx-1.0/tox.ini` & `colorsysx-1.0a1/tox.ini`

 * *Files identical despite different names*

### Comparing `colorsysx-1.0/PKG-INFO` & `colorsysx-1.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colorsysx
-Version: 1.0
+Version: 1.0a1
 Summary: Extra, human-relevant, colour spaces derived from RGB.
 Author-email: Andrew Chadwick <a.t.chadwick@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Multimedia :: Graphics :: Presentation
```

