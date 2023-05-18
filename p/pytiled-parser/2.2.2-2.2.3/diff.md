# Comparing `tmp/pytiled_parser-2.2.2.tar.gz` & `tmp/pytiled_parser-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytiled_parser-2.2.2.tar", last modified: Fri Mar 10 23:10:55 2023, max compression
+gzip compressed data, was "pytiled_parser-2.2.3.tar", last modified: Thu May 18 00:07:15 2023, max compression
```

## Comparing `pytiled_parser-2.2.2.tar` & `pytiled_parser-2.2.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 23:10:55.116602 pytiled_parser-2.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-10 23:10:42.000000 pytiled_parser-2.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-03-10 23:10:55.116602 pytiled_parser-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-03-10 23:10:42.000000 pytiled_parser-2.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-03-10 23:10:42.000000 pytiled_parser-2.2.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 23:10:55.112602 pytiled_parser-2.2.2/pytiled_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-03-10 23:10:42.000000 pytiled_parser-2.2.2/pytiled_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-03-10 23:10:42.000000 pytiled_parser-2.2.2/pytiled_parser/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-10 23:10:42.000000 pytiled_parser-2.2.2/pytiled_parser/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-03-10 23:10:42.000000 pytiled_parser-2.2.2/pytiled_parser/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-03-10 23:10:42.000000 pytiled_parser-2.2.2/pytiled_parser/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 23:10:55.112602 pytiled_parser-2.2.2/pytiled_parser/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 23:10:42.000000 pytiled_parser-2.2.2/pytiled_parser/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 23:10:55.112602 pytiled_parser-2.2.2/pytiled_parser/parsers/json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 23:10:42.000000 pytiled_parser-2.2.2/pytiled_parser/parsers/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-03-10 23:10:42.000000 pytiled_parser-2.2.2/pytiled_parser/parsers/json/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-03-10 23:10:42.000000 pytiled_parser-2.2.2/pytiled_parser/parsers/json/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-03-10 23:10:42.000000 pytiled_parser-2.2.2/pytiled_parser/parsers/json/tiled_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     9685 2023-03-10 23:10:42.000000 pytiled_parser-2.2.2/pytiled_parser/parsers/json/tiled_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-03-10 23:10:42.000000 pytiled_parser-2.2.2/pytiled_parser/parsers/json/tileset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-03-10 23:10:42.000000 pytiled_parser-2.2.2/pytiled_parser/parsers/json/wang_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 23:10:55.112602 pytiled_parser-2.2.2/pytiled_parser/parsers/tmx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 23:10:42.000000 pytiled_parser-2.2.2/pytiled_parser/parsers/tmx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-03-10 23:10:42.000000 pytiled_parser-2.2.2/pytiled_parser/parsers/tmx/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-03-10 23:10:42.000000 pytiled_parser-2.2.2/pytiled_parser/parsers/tmx/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     6716 2023-03-10 23:10:42.000000 pytiled_parser-2.2.2/pytiled_parser/parsers/tmx/tiled_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-03-10 23:10:42.000000 pytiled_parser-2.2.2/pytiled_parser/parsers/tmx/tiled_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-03-10 23:10:42.000000 pytiled_parser-2.2.2/pytiled_parser/parsers/tmx/tileset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-03-10 23:10:42.000000 pytiled_parser-2.2.2/pytiled_parser/parsers/tmx/wang_set.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-03-10 23:10:42.000000 pytiled_parser-2.2.2/pytiled_parser/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-03-10 23:10:42.000000 pytiled_parser-2.2.2/pytiled_parser/tiled_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-03-10 23:10:42.000000 pytiled_parser-2.2.2/pytiled_parser/tiled_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-03-10 23:10:42.000000 pytiled_parser-2.2.2/pytiled_parser/tileset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-03-10 23:10:42.000000 pytiled_parser-2.2.2/pytiled_parser/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-03-10 23:10:42.000000 pytiled_parser-2.2.2/pytiled_parser/wang_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-03-10 23:10:42.000000 pytiled_parser-2.2.2/pytiled_parser/world.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 23:10:55.112602 pytiled_parser-2.2.2/pytiled_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-03-10 23:10:55.000000 pytiled_parser-2.2.2/pytiled_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-03-10 23:10:55.000000 pytiled_parser-2.2.2/pytiled_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 23:10:55.000000 pytiled_parser-2.2.2/pytiled_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-10 23:10:55.000000 pytiled_parser-2.2.2/pytiled_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-10 23:10:55.000000 pytiled_parser-2.2.2/pytiled_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 23:10:55.116602 pytiled_parser-2.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 23:10:55.116602 pytiled_parser-2.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-03-10 23:10:42.000000 pytiled_parser-2.2.2/tests/test_invalid_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-03-10 23:10:42.000000 pytiled_parser-2.2.2/tests/test_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-03-10 23:10:42.000000 pytiled_parser-2.2.2/tests/test_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-03-10 23:10:42.000000 pytiled_parser-2.2.2/tests/test_parse_color.py
--rw-r--r--   0 runner    (1001) docker     (123)    31172 2023-03-10 23:10:42.000000 pytiled_parser-2.2.2/tests/test_tiled_object_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    15235 2023-03-10 23:10:42.000000 pytiled_parser-2.2.2/tests/test_tiled_object_tmx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-03-10 23:10:42.000000 pytiled_parser-2.2.2/tests/test_tileset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-03-10 23:10:42.000000 pytiled_parser-2.2.2/tests/test_world.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 00:07:15.062963 pytiled_parser-2.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-18 00:07:03.000000 pytiled_parser-2.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-05-18 00:07:15.062963 pytiled_parser-2.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-18 00:07:03.000000 pytiled_parser-2.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-18 00:07:03.000000 pytiled_parser-2.2.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 00:07:15.054963 pytiled_parser-2.2.3/pytiled_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-18 00:07:03.000000 pytiled_parser-2.2.3/pytiled_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-18 00:07:03.000000 pytiled_parser-2.2.3/pytiled_parser/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-18 00:07:03.000000 pytiled_parser-2.2.3/pytiled_parser/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-05-18 00:07:03.000000 pytiled_parser-2.2.3/pytiled_parser/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-18 00:07:03.000000 pytiled_parser-2.2.3/pytiled_parser/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 00:07:15.054963 pytiled_parser-2.2.3/pytiled_parser/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 00:07:03.000000 pytiled_parser-2.2.3/pytiled_parser/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 00:07:15.058963 pytiled_parser-2.2.3/pytiled_parser/parsers/json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 00:07:03.000000 pytiled_parser-2.2.3/pytiled_parser/parsers/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-05-18 00:07:03.000000 pytiled_parser-2.2.3/pytiled_parser/parsers/json/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-18 00:07:03.000000 pytiled_parser-2.2.3/pytiled_parser/parsers/json/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-05-18 00:07:03.000000 pytiled_parser-2.2.3/pytiled_parser/parsers/json/tiled_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9685 2023-05-18 00:07:03.000000 pytiled_parser-2.2.3/pytiled_parser/parsers/json/tiled_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-05-18 00:07:03.000000 pytiled_parser-2.2.3/pytiled_parser/parsers/json/tileset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-05-18 00:07:03.000000 pytiled_parser-2.2.3/pytiled_parser/parsers/json/wang_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 00:07:15.058963 pytiled_parser-2.2.3/pytiled_parser/parsers/tmx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 00:07:03.000000 pytiled_parser-2.2.3/pytiled_parser/parsers/tmx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-05-18 00:07:03.000000 pytiled_parser-2.2.3/pytiled_parser/parsers/tmx/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-18 00:07:03.000000 pytiled_parser-2.2.3/pytiled_parser/parsers/tmx/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6716 2023-05-18 00:07:03.000000 pytiled_parser-2.2.3/pytiled_parser/parsers/tmx/tiled_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-05-18 00:07:03.000000 pytiled_parser-2.2.3/pytiled_parser/parsers/tmx/tiled_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-05-18 00:07:03.000000 pytiled_parser-2.2.3/pytiled_parser/parsers/tmx/tileset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-18 00:07:03.000000 pytiled_parser-2.2.3/pytiled_parser/parsers/tmx/wang_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-18 00:07:03.000000 pytiled_parser-2.2.3/pytiled_parser/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-18 00:07:03.000000 pytiled_parser-2.2.3/pytiled_parser/tiled_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-05-18 00:07:03.000000 pytiled_parser-2.2.3/pytiled_parser/tiled_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9750 2023-05-18 00:07:03.000000 pytiled_parser-2.2.3/pytiled_parser/tileset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-18 00:07:03.000000 pytiled_parser-2.2.3/pytiled_parser/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-05-18 00:07:03.000000 pytiled_parser-2.2.3/pytiled_parser/wang_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-05-18 00:07:03.000000 pytiled_parser-2.2.3/pytiled_parser/world.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 00:07:15.054963 pytiled_parser-2.2.3/pytiled_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-05-18 00:07:15.000000 pytiled_parser-2.2.3/pytiled_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-18 00:07:15.000000 pytiled_parser-2.2.3/pytiled_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 00:07:15.000000 pytiled_parser-2.2.3/pytiled_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-18 00:07:15.000000 pytiled_parser-2.2.3/pytiled_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-18 00:07:15.000000 pytiled_parser-2.2.3/pytiled_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 00:07:15.062963 pytiled_parser-2.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 00:07:15.062963 pytiled_parser-2.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-18 00:07:03.000000 pytiled_parser-2.2.3/tests/test_invalid_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-05-18 00:07:03.000000 pytiled_parser-2.2.3/tests/test_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-18 00:07:03.000000 pytiled_parser-2.2.3/tests/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-18 00:07:03.000000 pytiled_parser-2.2.3/tests/test_parse_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31172 2023-05-18 00:07:03.000000 pytiled_parser-2.2.3/tests/test_tiled_object_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15235 2023-05-18 00:07:03.000000 pytiled_parser-2.2.3/tests/test_tiled_object_tmx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-18 00:07:03.000000 pytiled_parser-2.2.3/tests/test_tileset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-18 00:07:03.000000 pytiled_parser-2.2.3/tests/test_world.py
```

### Comparing `pytiled_parser-2.2.2/LICENSE` & `pytiled_parser-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytiled_parser-2.2.2/PKG-INFO` & `pytiled_parser-2.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytiled_parser
-Version: 2.2.2
+Version: 2.2.3
 Summary: A library for parsing Tiled Map Editor maps and tilesets
 Author-email: Benjamin Kirkbride <BenjaminKirkbride@gmail.com>, Darren Eberly <Darren.Eberly@gmail.com>
 Maintainer-email: Darren Eberly <Darren.Eberly@gmail.com>
 License: MIT License
         
         Copyright (c) 2019 Beefy_Swain
         
@@ -22,15 +22,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: homepage, https://github.com/pythonarcade/pytile_parser
+Project-URL: homepage, https://github.com/pythonarcade/pytiled_parser
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pytiled_parser-2.2.2/README.md` & `pytiled_parser-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pytiled_parser-2.2.2/pyproject.toml` & `pytiled_parser-2.2.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pytiled_parser"
-version = "2.2.2"
+version = "2.2.3"
 description = "A library for parsing Tiled Map Editor maps and tilesets"
 readme = "README.md"
 authors = [
     {name="Benjamin Kirkbride", email="BenjaminKirkbride@gmail.com"},
     {name="Darren Eberly", email="Darren.Eberly@gmail.com"},
 ]
 maintainers = [
@@ -28,15 +28,15 @@
 ]
 dependencies = [
     "attrs >= 18.2.0",
     "typing-extensions"
 ]
 
 [project.urls]
-homepage = "https://github.com/pythonarcade/pytile_parser"
+homepage = "https://github.com/pythonarcade/pytiled_parser"
 
 [project.optional-dependencies]
 zstd = [
     "zstd"
 ]
 
 dev = [
@@ -82,13 +82,13 @@
 [tool.mypy]
 python_version = 3.11
 warn_unused_configs = true
 warn_redundant_casts = true
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
-module = "tests.*"
+module = "pytiled_parser.tests.*"
 ignore_errors = true
 
 [tool.ruff]
 exclude = ["__init__.py"]
 ignore = ["E501"]
```

### Comparing `pytiled_parser-2.2.2/pytiled_parser/__init__.py` & `pytiled_parser-2.2.3/pytiled_parser/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,12 +10,12 @@
 """
 
 # pylint: disable=too-few-public-methods
 
 from .common_types import Color, OrderedPair, Size
 from .exception import UnknownFormat
 from .layer import Chunk, ImageLayer, Layer, LayerGroup, ObjectLayer, TileLayer
-from .parser import parse_map, parse_world
+from .parser import parse_map, parse_world, parse_tileset
 from .properties import Properties, Property
 from .tiled_map import TiledMap
 from .tileset import Frame, Grid, Tile, Tileset, Transformations
 from .world import World, WorldMap
```

### Comparing `pytiled_parser-2.2.2/pytiled_parser/common_types.py` & `pytiled_parser-2.2.3/pytiled_parser/common_types.py`

 * *Files identical despite different names*

### Comparing `pytiled_parser-2.2.2/pytiled_parser/layer.py` & `pytiled_parser-2.2.3/pytiled_parser/layer.py`

 * *Files identical despite different names*

### Comparing `pytiled_parser-2.2.2/pytiled_parser/parser.py` & `pytiled_parser-2.2.3/pytiled_parser/parser.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,77 @@
-from pathlib import Path
-
-from pytiled_parser import UnknownFormat
-from pytiled_parser.parsers.json.tiled_map import parse as json_map_parse
-from pytiled_parser.parsers.tmx.tiled_map import parse as tmx_map_parse
-from pytiled_parser.tiled_map import TiledMap
-from pytiled_parser.util import check_format
-from pytiled_parser.world import World
-from pytiled_parser.world import parse_world as _parse_world
-
-
-def parse_map(file: Path) -> TiledMap:
-    """Parse the raw Tiled map into a pytiled_parser type
-
-    Args:
-        file: Path to the map file
-
-    Returns:
-        TiledMap: A parsed and typed TiledMap
-    """
-    parser = check_format(file)
-
-    # The type ignores are because mypy for some reason thinks those functions return Any
-    if parser == "tmx":
-        return tmx_map_parse(file)  # type: ignore
-    else:
-        try:
-            return json_map_parse(file)  # type: ignore
-        except ValueError:
-            raise UnknownFormat(
-                "Unknown Map Format, please use either the TMX or JSON format. "
-                "This message could also mean your map file is invalid or corrupted."
-            )
-
-
-def parse_world(file: Path) -> World:
-    """Parse the raw world file into a pytiled_parser type
-
-    Args:
-        file: Path to the world file
-
-    Returns:
-        World: A parsed and typed World
-    """
-    return _parse_world(file)
+import json
+import xml.etree.ElementTree as etree
+from pathlib import Path
+
+from pytiled_parser import UnknownFormat
+from pytiled_parser.parsers.json.tiled_map import parse as json_map_parse
+from pytiled_parser.parsers.json.tileset import parse as json_tileset_parse
+from pytiled_parser.parsers.tmx.tiled_map import parse as tmx_map_parse
+from pytiled_parser.parsers.tmx.tileset import parse as tmx_tileset_parse
+from pytiled_parser.tiled_map import TiledMap
+from pytiled_parser.tileset import Tileset
+from pytiled_parser.util import check_format
+from pytiled_parser.world import World
+from pytiled_parser.world import parse_world as _parse_world
+
+
+def parse_map(file: Path) -> TiledMap:
+    """Parse the raw Tiled map into a pytiled_parser type
+
+    Args:
+        file: Path to the map file
+
+    Returns:
+        TiledMap: A parsed and typed TiledMap
+    """
+    parser = check_format(file)
+
+    # The type ignores are because mypy for some reason thinks those functions return Any
+    if parser == "tmx":
+        return tmx_map_parse(file)  # type: ignore
+    else:
+        try:
+            return json_map_parse(file)  # type: ignore
+        except ValueError:
+            raise UnknownFormat(
+                "Unknown Map Format, please use either the TMX or JSON format. "
+                "This message could also mean your map file is invalid or corrupted."
+            )
+
+
+def parse_tileset(file: Path) -> Tileset:
+    """Parse the raw Tiled Tileset into a pytiled_parser type
+
+    Args:
+        file: Path to the map file
+
+    Returns:
+        Tileset: A parsed and typed Tileset
+    """
+    parser = check_format(file)
+
+    if parser == "tmx":
+        with open(file) as map_file:
+            raw_tileset = etree.parse(map_file).getroot()
+        return tmx_tileset_parse(raw_tileset, 1)
+    else:
+        try:
+            with open(file) as my_file:
+                raw_tileset = json.load(my_file)
+            return json_tileset_parse(raw_tileset, 1)
+        except ValueError:
+            raise UnknownFormat(
+                "Unknowm Tileset Format, please use either the TSX or JSON format. "
+                "This message could also mean your tileset file is invalid or corrupted."
+            )
+
+
+def parse_world(file: Path) -> World:
+    """Parse the raw world file into a pytiled_parser type
+
+    Args:
+        file: Path to the world file
+
+    Returns:
+        World: A parsed and typed World
+    """
+    return _parse_world(file)
```

### Comparing `pytiled_parser-2.2.2/pytiled_parser/parsers/json/layer.py` & `pytiled_parser-2.2.3/pytiled_parser/parsers/json/layer.py`

 * *Files identical despite different names*

### Comparing `pytiled_parser-2.2.2/pytiled_parser/parsers/json/properties.py` & `pytiled_parser-2.2.3/pytiled_parser/parsers/json/properties.py`

 * *Files identical despite different names*

### Comparing `pytiled_parser-2.2.2/pytiled_parser/parsers/json/tiled_map.py` & `pytiled_parser-2.2.3/pytiled_parser/parsers/json/tiled_map.py`

 * *Files identical despite different names*

### Comparing `pytiled_parser-2.2.2/pytiled_parser/parsers/json/tiled_object.py` & `pytiled_parser-2.2.3/pytiled_parser/parsers/json/tiled_object.py`

 * *Files identical despite different names*

### Comparing `pytiled_parser-2.2.2/pytiled_parser/parsers/json/tileset.py` & `pytiled_parser-2.2.3/pytiled_parser/parsers/json/tileset.py`

 * *Files identical despite different names*

### Comparing `pytiled_parser-2.2.2/pytiled_parser/parsers/json/wang_set.py` & `pytiled_parser-2.2.3/pytiled_parser/parsers/json/wang_set.py`

 * *Files identical despite different names*

### Comparing `pytiled_parser-2.2.2/pytiled_parser/parsers/tmx/layer.py` & `pytiled_parser-2.2.3/pytiled_parser/parsers/tmx/layer.py`

 * *Files identical despite different names*

### Comparing `pytiled_parser-2.2.2/pytiled_parser/parsers/tmx/properties.py` & `pytiled_parser-2.2.3/pytiled_parser/parsers/tmx/properties.py`

 * *Files identical despite different names*

### Comparing `pytiled_parser-2.2.2/pytiled_parser/parsers/tmx/tiled_map.py` & `pytiled_parser-2.2.3/pytiled_parser/parsers/tmx/tiled_map.py`

 * *Files identical despite different names*

### Comparing `pytiled_parser-2.2.2/pytiled_parser/parsers/tmx/tiled_object.py` & `pytiled_parser-2.2.3/pytiled_parser/parsers/tmx/tiled_object.py`

 * *Files identical despite different names*

### Comparing `pytiled_parser-2.2.2/pytiled_parser/parsers/tmx/tileset.py` & `pytiled_parser-2.2.3/pytiled_parser/parsers/tmx/tileset.py`

 * *Files identical despite different names*

### Comparing `pytiled_parser-2.2.2/pytiled_parser/parsers/tmx/wang_set.py` & `pytiled_parser-2.2.3/pytiled_parser/parsers/tmx/wang_set.py`

 * *Files identical despite different names*

### Comparing `pytiled_parser-2.2.2/pytiled_parser/tiled_map.py` & `pytiled_parser-2.2.3/pytiled_parser/tiled_map.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-"""The tiled_map module contains the primary TiledMap class which represents a single
-map from Tiled.
-"""
-
-from pathlib import Path
-from typing import Dict, List, Optional
-
-import attr
-
-from pytiled_parser.common_types import Color, OrderedPair, Size
-from pytiled_parser.layer import Layer
-from pytiled_parser.properties import Properties
-from pytiled_parser.tileset import Tileset
-
-TilesetDict = Dict[int, Tileset]
-
-
-@attr.s(auto_attribs=True)
-class TiledMap:
-    """Object for storing a Tiled map with all associated objects.
-
-    This object is the top level object for a map. It contains all layers within a map,
-    as well as all Tiesets used by the map. When creating an implementation, this will
-    be the primary class to work with to pull all data relating to a map.
-
-    `TMX Reference <https://doc.mapeditor.org/en/stable/reference/tmx-map-format/#map>`_
-
-    `JSON Reference <https://doc.mapeditor.org/en/stable/reference/json-map-format/#map>`_
-
-    Attributes:
-        infinite: If the map is infinite or not.
-        layers: List of layer objects by draw order.
-        map_size: The map width in tiles.
-        next_layer_id: Stores the next available ID for new layers.
-        next_object_id: Stores the next available ID for new objects.
-        orientation: Map orientation. Tiled supports "orthogonal", "isometric",
-            "staggered" and "hexagonal"
-        render_order: The order in which tiles on tile layers are rendered. Valid values
-            are right-down, right-up, left-down and left-up. In all cases, the map is
-            drawn row-by-row. (only supported for orthogonal maps at the moment)
-        tiled_version: The Tiled version used to save the file. May be a date (for
-            snapshot builds).
-        tile_size: The size of a tile.
-        tilesets: Dict of Tileset where Key is the firstgid and the value is the Tileset
-        version: The JSON format version.
-        background_color: The background color of the map.
-        properties: The properties of the Map.
-        hex_side_length: Only for hexagonal maps. Determines the width or height
-            (depending on the staggered axis) of the tile's edge, in pixels.
-        stagger_axis: For staggered and hexagonal maps, determines which axis ("x" or
-            "y") is staggered.
-        stagger_index: For staggered and hexagonal maps, determines whether the "even"
-            or "odd" indexes along the staggered axis are shifted.
-        class_: The Tiled class of this Map.
-        parallax_origin: The point on the map to center the parallax scrolling of layers on.
-    """
-
-    infinite: bool
-    layers: List[Layer]
-    map_size: Size
-    next_layer_id: Optional[int]
-    next_object_id: int
-    orientation: str
-    render_order: str
-    tiled_version: str
-    tile_size: Size
-    tilesets: TilesetDict
-    version: str
-
-    parallax_origin: OrderedPair = OrderedPair(0, 0)
-
-    map_file: Optional[Path] = None
-    class_: Optional[str] = None
-    background_color: Optional[Color] = None
-    properties: Optional[Properties] = None
-    hex_side_length: Optional[int] = None
-    stagger_axis: Optional[str] = None
-    stagger_index: Optional[str] = None
+"""The tiled_map module contains the primary TiledMap class which represents a single
+map from Tiled.
+"""
+
+from pathlib import Path
+from typing import Dict, List, Optional
+
+import attr
+
+from pytiled_parser.common_types import Color, OrderedPair, Size
+from pytiled_parser.layer import Layer
+from pytiled_parser.properties import Properties
+from pytiled_parser.tileset import Tileset
+
+TilesetDict = Dict[int, Tileset]
+
+
+@attr.s(auto_attribs=True)
+class TiledMap:
+    """Object for storing a Tiled map with all associated objects.
+
+    This object is the top level object for a map. It contains all layers within a map,
+    as well as all Tiesets used by the map. When creating an implementation, this will
+    be the primary class to work with to pull all data relating to a map.
+
+    `TMX Reference <https://doc.mapeditor.org/en/stable/reference/tmx-map-format/#map>`_
+
+    `JSON Reference <https://doc.mapeditor.org/en/stable/reference/json-map-format/#map>`_
+
+    Attributes:
+        infinite: If the map is infinite or not.
+        layers: List of layer objects by draw order.
+        map_size: The map width in tiles.
+        next_layer_id: Stores the next available ID for new layers.
+        next_object_id: Stores the next available ID for new objects.
+        orientation: Map orientation. Tiled supports "orthogonal", "isometric",
+            "staggered" and "hexagonal"
+        render_order: The order in which tiles on tile layers are rendered. Valid values
+            are right-down, right-up, left-down and left-up. In all cases, the map is
+            drawn row-by-row. (only supported for orthogonal maps at the moment)
+        tiled_version: The Tiled version used to save the file. May be a date (for
+            snapshot builds).
+        tile_size: The size of a tile.
+        tilesets: Dict of Tileset where Key is the firstgid and the value is the Tileset
+        version: The JSON format version.
+        background_color: The background color of the map.
+        properties: The properties of the Map.
+        hex_side_length: Only for hexagonal maps. Determines the width or height
+            (depending on the staggered axis) of the tile's edge, in pixels.
+        stagger_axis: For staggered and hexagonal maps, determines which axis ("x" or
+            "y") is staggered.
+        stagger_index: For staggered and hexagonal maps, determines whether the "even"
+            or "odd" indexes along the staggered axis are shifted.
+        class_: The Tiled class of this Map.
+        parallax_origin: The point on the map to center the parallax scrolling of layers on.
+    """
+
+    map_file: Path
+    infinite: bool
+    layers: List[Layer]
+    map_size: Size
+    next_layer_id: Optional[int]
+    next_object_id: int
+    orientation: str
+    render_order: str
+    tiled_version: str
+    tile_size: Size
+    tilesets: TilesetDict
+    version: str
+
+    parallax_origin: OrderedPair = OrderedPair(0, 0)
+
+    class_: Optional[str] = None
+    background_color: Optional[Color] = None
+    properties: Optional[Properties] = None
+    hex_side_length: Optional[int] = None
+    stagger_axis: Optional[str] = None
+    stagger_index: Optional[str] = None
```

### Comparing `pytiled_parser-2.2.2/pytiled_parser/tiled_object.py` & `pytiled_parser-2.2.3/pytiled_parser/tiled_object.py`

 * *Files identical despite different names*

### Comparing `pytiled_parser-2.2.2/pytiled_parser/tileset.py` & `pytiled_parser-2.2.3/pytiled_parser/tileset.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,16 +117,16 @@
         class_: The Tiled class of this Tile.
     """
 
     id: int
     opacity: int = 1
     x: int = 0
     y: int = 0
-    width: Optional[int] = None
-    height: Optional[int] = None
+    width: int = 0
+    height: int = 0
     class_: Optional[str] = None
     animation: Optional[List[Frame]] = None
     objects: Optional[layer.Layer] = None
     image: Optional[Path] = None
     image_width: Optional[int] = None
     image_height: Optional[int] = None
     properties: Optional[properties_.Properties] = None
```

### Comparing `pytiled_parser-2.2.2/pytiled_parser/util.py` & `pytiled_parser-2.2.3/pytiled_parser/util.py`

 * *Files identical despite different names*

### Comparing `pytiled_parser-2.2.2/pytiled_parser/wang_set.py` & `pytiled_parser-2.2.3/pytiled_parser/wang_set.py`

 * *Files identical despite different names*

### Comparing `pytiled_parser-2.2.2/pytiled_parser/world.py` & `pytiled_parser-2.2.3/pytiled_parser/world.py`

 * *Files identical despite different names*

### Comparing `pytiled_parser-2.2.2/pytiled_parser.egg-info/PKG-INFO` & `pytiled_parser-2.2.3/pytiled_parser.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytiled-parser
-Version: 2.2.2
+Version: 2.2.3
 Summary: A library for parsing Tiled Map Editor maps and tilesets
 Author-email: Benjamin Kirkbride <BenjaminKirkbride@gmail.com>, Darren Eberly <Darren.Eberly@gmail.com>
 Maintainer-email: Darren Eberly <Darren.Eberly@gmail.com>
 License: MIT License
         
         Copyright (c) 2019 Beefy_Swain
         
@@ -22,15 +22,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: homepage, https://github.com/pythonarcade/pytile_parser
+Project-URL: homepage, https://github.com/pythonarcade/pytiled_parser
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pytiled_parser-2.2.2/pytiled_parser.egg-info/SOURCES.txt` & `pytiled_parser-2.2.3/pytiled_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytiled_parser-2.2.2/tests/test_layer.py` & `pytiled_parser-2.2.3/tests/test_layer.py`

 * *Files identical despite different names*

### Comparing `pytiled_parser-2.2.2/tests/test_map.py` & `pytiled_parser-2.2.3/tests/test_map.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,93 +1,97 @@
-"""Tests for maps"""
-import importlib.util
-import os
-from pathlib import Path
-
-import pytest
-
-from pytiled_parser import UnknownFormat, parse_map
-from pytiled_parser.common_types import OrderedPair, Size
-
-TESTS_DIR = Path(os.path.dirname(os.path.abspath(__file__)))
-TEST_DATA = TESTS_DIR / "test_data"
-MAP_TESTS = TEST_DATA / "map_tests"
-
-ALL_MAP_TESTS = [
-    MAP_TESTS / "external_tileset_dif_dir",
-    MAP_TESTS / "no_layers",
-    MAP_TESTS / "no_background_color",
-    MAP_TESTS / "hexagonal",
-    MAP_TESTS / "embedded_tileset",
-    MAP_TESTS / "template",
-    MAP_TESTS / "cross_format_tileset",
-]
-
-JSON_INVALID_TILESET = MAP_TESTS / "json_invalid_tileset"
-
-def fix_object(my_object):
-    my_object.coordinates = OrderedPair(
-        round(my_object.coordinates[0], 3), round(my_object.coordinates[1], 3)
-    )
-    my_object.size = Size(round(my_object.size[0], 4), round(my_object.size[1], 4))
-
-
-def fix_tileset(tileset):
-    tileset.version = None
-    tileset.tiled_version = None
-    if tileset.tiles:
-        for tile in tileset.tiles.values():
-            if tile.objects:
-                for my_object in tile.objects.tiled_objects:
-                    fix_object(my_object)
-
-
-def fix_layer(layer):
-    for tiled_object in layer.tiled_objects:
-        fix_object(tiled_object)
-
-
-def fix_map(map):
-    map.version = None
-    map.tiled_version = None
-    for layer in [layer for layer in map.layers if hasattr(layer, "tiled_objects")]:
-        fix_layer(layer)
-
-    for tileset in map.tilesets.values():
-        fix_tileset(tileset)
-
-
-@pytest.mark.parametrize("parser_type", ["json", "tmx"])
-@pytest.mark.parametrize("map_test", ALL_MAP_TESTS)
-def test_map_integration(parser_type, map_test):
-    # it's a PITA to import like this, don't do it
-    # https://stackoverflow.com/a/67692/1342874
-    spec = importlib.util.spec_from_file_location("expected", map_test / "expected.py")
-    expected = importlib.util.module_from_spec(spec)
-    spec.loader.exec_module(expected)
-
-    if parser_type == "json":
-        raw_maps_path = map_test / "map.json"
-    elif parser_type == "tmx":
-        raw_maps_path = map_test / "map.tmx"
-
-    casted_map = parse_map(raw_maps_path)
-
-    # file detection when running from unit tests is broken
-    expected.EXPECTED.map_file = casted_map.map_file
-
-    # who even knows what/how/when the gods determine what the
-    # version values in maps/tileset files are, so we're just not
-    # gonna check them, because they don't make sense anyways.
-    #
-    # Yes the values could be set to None in the expected objects
-    # directly, but alas, this is just test code that's already stupid fast
-    # and I'm lazy because there's too many of them already existing.
-    fix_map(expected.EXPECTED)
-    fix_map(casted_map)
-    assert casted_map == expected.EXPECTED
-
-def test_json_invalid_tileset():
-    raw_map_path = JSON_INVALID_TILESET / "map.json"
-
-    with pytest.raises(UnknownFormat):
-        parse_map(raw_map_path)
+"""Tests for maps"""
+import importlib.util
+import os
+from pathlib import Path
+
+import pytest
+
+from pytiled_parser import UnknownFormat, parse_map
+from pytiled_parser.common_types import OrderedPair, Size
+
+TESTS_DIR = Path(os.path.dirname(os.path.abspath(__file__)))
+TEST_DATA = TESTS_DIR / "test_data"
+MAP_TESTS = TEST_DATA / "map_tests"
+
+ALL_MAP_TESTS = [
+    MAP_TESTS / "external_tileset_dif_dir",
+    MAP_TESTS / "no_layers",
+    MAP_TESTS / "no_background_color",
+    MAP_TESTS / "hexagonal",
+    MAP_TESTS / "embedded_tileset",
+    MAP_TESTS / "template",
+    MAP_TESTS / "cross_format_tileset",
+]
+
+JSON_INVALID_TILESET = MAP_TESTS / "json_invalid_tileset"
+
+def fix_object(my_object):
+    my_object.coordinates = OrderedPair(
+        round(my_object.coordinates[0], 3), round(my_object.coordinates[1], 3)
+    )
+    my_object.size = Size(round(my_object.size[0], 4), round(my_object.size[1], 4))
+
+
+def fix_tileset(tileset):
+    tileset.version = None
+    tileset.tiled_version = None
+    if tileset.tiles:
+        for tile in tileset.tiles.values():
+            if tile.objects:
+                for my_object in tile.objects.tiled_objects:
+                    fix_object(my_object)
+
+
+def fix_layer(layer):
+    for tiled_object in layer.tiled_objects:
+        fix_object(tiled_object)
+
+
+def fix_map(map):
+    map.map_file = None
+    map.version = None
+    map.tiled_version = None
+    for layer in [layer for layer in map.layers if hasattr(layer, "tiled_objects")]:
+        fix_layer(layer)
+
+    for tileset in map.tilesets.values():
+        fix_tileset(tileset)
+
+
+@pytest.mark.parametrize("parser_type", ["json", "tmx"])
+@pytest.mark.parametrize("map_test", ALL_MAP_TESTS)
+def test_map_integration(parser_type, map_test):
+    # it's a PITA to import like this, don't do it
+    # https://stackoverflow.com/a/67692/1342874
+    spec = importlib.util.spec_from_file_location("expected", map_test / "expected.py")
+    expected = importlib.util.module_from_spec(spec)
+    spec.loader.exec_module(expected)
+
+    if parser_type == "json":
+        raw_maps_path = map_test / "map.json"
+    elif parser_type == "tmx":
+        raw_maps_path = map_test / "map.tmx"
+
+    casted_map = parse_map(raw_maps_path)
+
+    # file detection when running from unit tests is broken
+    expected.EXPECTED.map_file = casted_map.map_file
+
+    # who even knows what/how/when the gods determine what the
+    # version values in maps/tileset files are, so we're just not
+    # gonna check them, because they don't make sense anyways.
+    #
+    # Yes the values could be set to None in the expected objects
+    # directly, but alas, this is just test code that's already stupid fast
+    # and I'm lazy because there's too many of them already existing.
+    #
+    # This also adjusts the map_file parameter since that can't be known
+    # in a way that is valid for the tests.
+    fix_map(expected.EXPECTED)
+    fix_map(casted_map)
+    assert casted_map == expected.EXPECTED
+
+def test_json_invalid_tileset():
+    raw_map_path = JSON_INVALID_TILESET / "map.json"
+
+    with pytest.raises(UnknownFormat):
+        parse_map(raw_map_path)
```

### Comparing `pytiled_parser-2.2.2/tests/test_tiled_object_json.py` & `pytiled_parser-2.2.3/tests/test_tiled_object_json.py`

 * *Files identical despite different names*

### Comparing `pytiled_parser-2.2.2/tests/test_tiled_object_tmx.py` & `pytiled_parser-2.2.3/tests/test_tiled_object_tmx.py`

 * *Files identical despite different names*

### Comparing `pytiled_parser-2.2.2/tests/test_tileset.py` & `pytiled_parser-2.2.3/tests/test_tileset.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import json
 import os
 import xml.etree.ElementTree as etree
 from pathlib import Path
 
 import pytest
 
+from pytiled_parser import parse_tileset
 from pytiled_parser.common_types import OrderedPair, Size
 from pytiled_parser.parsers.json.tileset import parse as parse_json
 from pytiled_parser.parsers.tmx.tileset import parse as parse_tmx
 
 TESTS_DIR = Path(os.path.dirname(os.path.abspath(__file__)))
 TEST_DATA = TESTS_DIR / "test_data"
 TILE_SETS = TEST_DATA / "tilesets"
@@ -55,18 +56,25 @@
         "expected", tileset_dir / "expected.py"
     )
     expected = importlib.util.module_from_spec(spec)
     spec.loader.exec_module(expected)
 
     if parser_type == "json":
         raw_tileset_path = tileset_dir / "tileset.json"
-        with open(raw_tileset_path) as raw_tileset:
-            tileset_ = parse_json(json.loads(raw_tileset.read()), 1)
     elif parser_type == "tmx":
         raw_tileset_path = tileset_dir / "tileset.tsx"
-        with open(raw_tileset_path) as raw_tileset:
-            tileset_ = parse_tmx(etree.parse(raw_tileset).getroot(), 1)
+
+    tileset_ = parse_tileset(raw_tileset_path)
+
+    # if parser_type == "json":
+    #     raw_tileset_path = tileset_dir / "tileset.json"
+    #     with open(raw_tileset_path) as raw_tileset:
+    #         tileset_ = parse_json(json.loads(raw_tileset.read()), 1)
+    # elif parser_type == "tmx":
+    #     raw_tileset_path = tileset_dir / "tileset.tsx"
+    #     with open(raw_tileset_path) as raw_tileset:
+    #         tileset_ = parse_tmx(etree.parse(raw_tileset).getroot(), 1)
 
     fix_tileset(tileset_)
     fix_tileset(expected.EXPECTED)
 
     assert tileset_ == expected.EXPECTED
```

### Comparing `pytiled_parser-2.2.2/tests/test_world.py` & `pytiled_parser-2.2.3/tests/test_world.py`

 * *Files identical despite different names*

