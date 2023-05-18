# Comparing `tmp/bipl-0.1.1.tar.gz` & `tmp/bipl-0.1.2.tar.gz`

## Comparing `bipl-0.1.1.tar` & `bipl-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 bipl-0.1.1/src/bipl/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bipl-0.1.1/src/bipl/py.typed
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 bipl-0.1.1/src/bipl/io/__init__.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 bipl-0.1.1/src/bipl/io/_dzi.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 bipl-0.1.1/src/bipl/io/_libs.py
--rw-r--r--   0        0        0     6226 2020-02-02 00:00:00.000000 bipl-0.1.1/src/bipl/io/_openslide.py
--rw-r--r--   0        0        0     5516 2020-02-02 00:00:00.000000 bipl-0.1.1/src/bipl/io/_slide.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 bipl-0.1.1/src/bipl/io/_slide_bases.py
--rw-r--r--   0        0        0    10840 2020-02-02 00:00:00.000000 bipl-0.1.1/src/bipl/io/_tiff.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 bipl-0.1.1/src/bipl/ops/__init__.py
--rw-r--r--   0        0        0    14278 2020-02-02 00:00:00.000000 bipl-0.1.1/src/bipl/ops/_mosaic.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 bipl-0.1.1/src/bipl/ops/_util.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 bipl-0.1.1/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 bipl-0.1.1/LICENSE
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 bipl-0.1.1/README.md
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 bipl-0.1.1/hatch_build.py
--rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 bipl-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4841 2020-02-02 00:00:00.000000 bipl-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 bipl-0.1.2/src/bipl/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bipl-0.1.2/src/bipl/py.typed
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 bipl-0.1.2/src/bipl/io/__init__.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 bipl-0.1.2/src/bipl/io/_dzi.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 bipl-0.1.2/src/bipl/io/_libs.py
+-rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 bipl-0.1.2/src/bipl/io/_openslide.py
+-rw-r--r--   0        0        0     5483 2020-02-02 00:00:00.000000 bipl-0.1.2/src/bipl/io/_slide.py
+-rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 bipl-0.1.2/src/bipl/io/_slide_bases.py
+-rw-r--r--   0        0        0    10893 2020-02-02 00:00:00.000000 bipl-0.1.2/src/bipl/io/_tiff.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 bipl-0.1.2/src/bipl/ops/__init__.py
+-rw-r--r--   0        0        0    14324 2020-02-02 00:00:00.000000 bipl-0.1.2/src/bipl/ops/_mosaic.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 bipl-0.1.2/src/bipl/ops/_util.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 bipl-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 bipl-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 bipl-0.1.2/README.md
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 bipl-0.1.2/hatch_build.py
+-rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 bipl-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 bipl-0.1.2/PKG-INFO
```

### Comparing `bipl-0.1.1/src/bipl/io/__init__.py` & `bipl-0.1.2/src/bipl/io/__init__.py`

 * *Files identical despite different names*

### Comparing `bipl-0.1.1/src/bipl/io/_dzi.py` & `bipl-0.1.2/src/bipl/io/_dzi.py`

 * *Files identical despite different names*

### Comparing `bipl-0.1.1/src/bipl/io/_libs.py` & `bipl-0.1.2/src/bipl/io/_libs.py`

 * *Files identical despite different names*

### Comparing `bipl-0.1.1/src/bipl/io/_openslide.py` & `bipl-0.1.2/src/bipl/io/_openslide.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,16 @@
 
 
 @dataclass(frozen=True)
 class _Item(Item):
     name: bytes
     osd: Openslide
 
-    def get_key(self) -> str:
+    @property
+    def key(self) -> str:
         return self.name.decode()
 
     def __array__(self) -> np.ndarray:
         bgra = np.empty((*self.shape[:2], 4), 'u1')
         OSD.openslide_read_associated_image(self.osd.ptr, self.name,
                                             c_void_p(bgra.ctypes.data))
         rgb = _mbgra_to_rgb(bgra, self.osd.bg_color)
```

### Comparing `bipl-0.1.1/src/bipl/io/_slide.py` & `bipl-0.1.2/src/bipl/io/_slide.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,23 +81,23 @@
 
         lods: dict[int, Lod] = {1: item_0}
         self.extras: dict[str, Item] = {}
         for item in items:
             if isinstance(item, Lod):
                 pool = round(item_0.shape[0] / item.shape[0])
                 lods[pool] = item
-            elif key := item.get_key():
+            elif key := item.key:
                 self.extras[key] = item
 
         self.pools = *sorted(lods.keys()),
         self.lods = *(lods[pool] for pool in self.pools),
         self.shape = self.lods[0].shape
         self.spacing = self.lods[0].spacing
 
-        self.extras |= {key: driver.get(key) for key in driver.keys()}
+        self.extras |= driver.named_items()
         self.driver = driver_cls.__name__
 
     def __reduce__(self) -> tuple:
         return Slide.open, (self.path, )
 
     def __repr__(self) -> str:
         line = f"'{self.path}', shape={self.shape}, pools={self.pools}"
```

### Comparing `bipl-0.1.1/src/bipl/io/_slide_bases.py` & `bipl-0.1.2/src/bipl/io/_slide_bases.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,27 +25,29 @@
     ) for s, axis_len in zip(slices, shape)),
 
 
 @dataclass(frozen=True)
 class Item:
     shape: tuple[int, ...]
 
-    def get_key(self) -> str | None:
+    @property
+    def key(self) -> str | None:
         raise NotImplementedError
 
     def __array__(self) -> np.ndarray:
         raise NotImplementedError
 
 
 @dataclass(frozen=True)
 class Lod(Item):
     spacing: float | None
 
     @final
-    def get_key(self) -> None:
+    @property
+    def key(self) -> None:
         return None
 
     def crop(self, slices: tuple[slice, ...]) -> np.ndarray:
         """Reads crop of LOD. Overridable"""
         raise NotImplementedError
 
     @final
@@ -101,14 +103,18 @@
         """Count of indexed items"""
         return 0
 
     def __getitem__(self, index: int) -> Item:
         """Gives indexed item"""
         raise NotImplementedError
 
+    def named_items(self) -> dict[str, Item]:
+        keys = self.keys()
+        return {k: self.get(k) for k in keys}
+
     def keys(self) -> list[str]:
         """List of names for named items"""
         return []
 
     def get(self, key: str) -> Item:
         """Gives named item"""
         raise NotImplementedError
```

### Comparing `bipl-0.1.1/src/bipl/io/_tiff.py` & `bipl-0.1.2/src/bipl/io/_tiff.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,30 +67,31 @@
     SGILOG24 = 34677
     JPEG2000 = 34712
     LZMA = 34925
     ZSTD = 50000
     WEBP = 50001
 
 
-class _Tag:  # noqa: PIE795
+class _Tag:  # noqa: PIE795,RUF100
     JPEG_TABLES = 347
     TILE_BYTE_COUNTS = 325
     BACKGROUND_COLOR = 434
 
 
 class _Tags:
     def __init__(self, ptr):
         self._ptr = ptr
         self.compression, = self._get(c_uint16, 259)
         self.colorspace, = self._get(c_uint16, 262)
         self.spp, = self._get(c_uint16, 277)
         self.is_planar, = self._get(c_uint16, 284)
         self.image_size = self._get(c_uint32, 257, 256)
         self.tile_size = self._get(c_uint32, 323, 322)
-        self.description = self._get(c_char_p, 270).pop() or b''
+        dscr = self._get(c_char_p, 270)
+        self.description: bytes = dscr and dscr.pop() or b''
         self.resolution = self._get(c_float, 283, 282)
 
     def _get(self, tp: type[ctypes._SimpleCData[_T]], *tags: int) -> list[_T]:
         values = []
         for tag in tags:
             cv = tp()
             if TIFF.TIFFGetField(self._ptr, c_uint32(tag), byref(cv)):
@@ -132,15 +133,16 @@
     bg_color: np.ndarray
     compression: _Compression
     jpt: bytes = field(repr=False)
 
 
 @dataclass(frozen=True)
 class _Item(_ItemBase):
-    def get_key(self) -> str | None:
+    @property
+    def key(self) -> str | None:
         if self.tiff.is_svs and self.index == 1:
             return 'thumbnail'
         for key in ('label', 'macro'):
             if any(key in s for s in self.head):
                 return key
         return None
```

### Comparing `bipl-0.1.1/src/bipl/ops/_mosaic.py` & `bipl-0.1.2/src/bipl/ops/_mosaic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from __future__ import annotations
 
 __all__ = ['Mosaic', 'Tile', 'get_fusion']
 
 import dataclasses
 from collections import defaultdict
 from collections.abc import Callable, Iterable, Iterator
+from contextlib import AbstractContextManager
 from dataclasses import dataclass, field
 from functools import partial
 from itertools import chain
-from typing import ContextManager, NamedTuple, Protocol, TypeVar, cast
+from typing import NamedTuple, Protocol, TypeVar, cast
 
 import cv2
 import numpy as np
 from glow import chunked, map_n
 
 from ._util import get_trapz
 
@@ -203,15 +204,15 @@
         assert v_scale >= 1
         for tile in self:
             tw, th = tile.data.shape[:2]
             v = view[tile.vec[0] // v_scale:,
                      tile.vec[1] // v_scale:][:tw // v_scale, :th // v_scale]
             yield tile.idx, tile.vec, tile.data, v
 
-    def with_cm(self: _Self, cm: ContextManager) -> _Self:
+    def with_cm(self: _Self, cm: AbstractContextManager) -> _Self:
         return cast(_Self, _CmView(self.m, self.shape, self.cells, self, cm))
 
 
 @dataclass
 class _View(_BaseView):
     def map_batched(self,
                     fn: Callable[[list[np.ndarray]], Iterable[np.ndarray]],
@@ -270,15 +271,15 @@
     def __iter__(self) -> Iterator[Tile]:
         return iter(self.source)
 
 
 @dataclass
 class _CmView(_BaseView):
     source: Iterable[Tile]
-    _cm: ContextManager
+    _cm: AbstractContextManager
 
     def __iter__(self) -> Iterator[Tile]:
         with self._cm:
             yield from self.source
 
 
 @dataclass
```

### Comparing `bipl-0.1.1/src/bipl/ops/_util.py` & `bipl-0.1.2/src/bipl/ops/_util.py`

 * *Files identical despite different names*

### Comparing `bipl-0.1.1/LICENSE` & `bipl-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bipl-0.1.1/README.md` & `bipl-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `bipl-0.1.1/hatch_build.py` & `bipl-0.1.2/hatch_build.py`

 * *Files identical despite different names*

### Comparing `bipl-0.1.1/pyproject.toml` & `bipl-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [tool.hatch.build.targets.wheel]
 artifacts = ["*.dll"]  # only wheel keeps DLLs
 
 [tool.hatch.build.hooks.custom]  # enable "custom" hook
 
 [project]
 name = "bipl"
-version = "0.1.1"
+version = "0.1.2"
 description = "Big Image Python Library"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 keywords = ["TIFF", "SVS", "OpenSlide", "tiles"]
 authors = [
     {name = "Paul Maevskikh", email = "arquolo@gmail.com"},
@@ -49,17 +49,16 @@
     "flake8-pie",
     "flake8-pyi",
     "flake8-pyproject",
     "flake8-simplify",
     "isort",
     "mypy~=0.990",
     "pytest~=6.0",
-    "ruff",
-    "yapf[pyproject]~=0.29,!=0.30,!=0.31,!=0.32",
-    "toml; python_version>='3.11'",  # See: https://github.com/google/yapf/pull/1040. Drop for yapf~=0.33
+    "ruff~=0.0.264",
+    "yapf~=0.33.0",
 ]
 dev = [
     "bipl[dev-core]",
     "flake8-alphabetize",
     # "flake8-class-attributes-order",
     # "flake8-newspaper-style",
     "typing-extensions~=4.4",
```

### Comparing `bipl-0.1.1/PKG-INFO` & `bipl-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bipl
-Version: 0.1.1
+Version: 0.1.2
 Summary: Big Image Python Library
 Project-URL: homepage, https://github.com/arquolo/bipl
 Project-URL: repository, https://github.com
 Author-email: Paul Maevskikh <arquolo@gmail.com>
 Maintainer-email: Paul Maevskikh <arquolo@gmail.com>
 License: MIT License
         
@@ -52,17 +52,16 @@
 Requires-Dist: flake8-pyi; extra == 'dev-core'
 Requires-Dist: flake8-pyproject; extra == 'dev-core'
 Requires-Dist: flake8-simplify; extra == 'dev-core'
 Requires-Dist: flake8~=6.0.0; extra == 'dev-core'
 Requires-Dist: isort; extra == 'dev-core'
 Requires-Dist: mypy~=0.990; extra == 'dev-core'
 Requires-Dist: pytest~=6.0; extra == 'dev-core'
-Requires-Dist: ruff; extra == 'dev-core'
-Requires-Dist: toml; python_version >= '3.11' and extra == 'dev-core'
-Requires-Dist: yapf[pyproject]!=0.30,!=0.31,!=0.32,~=0.29; extra == 'dev-core'
+Requires-Dist: ruff~=0.0.264; extra == 'dev-core'
+Requires-Dist: yapf~=0.33.0; extra == 'dev-core'
 Provides-Extra: dev-wemake
 Requires-Dist: bipl[dev-core]; extra == 'dev-wemake'
 Requires-Dist: wemake-python-styleguide~=0.15.0; extra == 'dev-wemake'
 Description-Content-Type: text/markdown
 
 # BIPL is a Big Image Python Library
```

