# Comparing `tmp/fudgeo-0.5.1-py3-none-any.whl.zip` & `tmp/fudgeo-0.5.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,22 @@
-Zip file size: 28084 bytes, number of entries: 17
--rw-r--r--  2.0 unx      117 b- defN 23-May-17 18:29 fudgeo/__init__.py
--rw-r--r--  2.0 unx     2538 b- defN 23-May-11 16:25 fudgeo/constant.py
+Zip file size: 31166 bytes, number of entries: 20
+-rw-r--r--  2.0 unx      117 b- defN 23-May-18 20:04 fudgeo/__init__.py
+-rw-r--r--  2.0 unx     2852 b- defN 23-May-18 20:04 fudgeo/constant.py
 -rw-r--r--  2.0 unx     1157 b- defN 23-Jan-04 21:53 fudgeo/enumeration.py
 -rw-r--r--  2.0 unx    20081 b- defN 23-May-12 12:57 fudgeo/geopkg.py
 -rw-r--r--  2.0 unx     2673 b- defN 23-May-06 22:48 fudgeo/geopkg.sql
 -rw-r--r--  2.0 unx     7768 b- defN 23-May-06 22:48 fudgeo/sql.py
 -rw-r--r--  2.0 unx      974 b- defN 23-May-06 22:48 fudgeo/geometry/__init__.py
--rw-r--r--  2.0 unx     1983 b- defN 23-May-17 18:29 fudgeo/geometry/base.py
--rw-r--r--  2.0 unx    18746 b- defN 23-May-17 18:29 fudgeo/geometry/linestring.py
--rw-r--r--  2.0 unx    19883 b- defN 23-May-17 18:29 fudgeo/geometry/point.py
--rw-r--r--  2.0 unx    26514 b- defN 23-May-17 18:29 fudgeo/geometry/polygon.py
--rw-r--r--  2.0 unx    16219 b- defN 23-May-17 18:29 fudgeo/geometry/util.py
--rw-r--r--  2.0 unx     1088 b- defN 23-May-17 18:30 fudgeo-0.5.1.dist-info/LICENSE
--rw-r--r--  2.0 unx    12716 b- defN 23-May-17 18:30 fudgeo-0.5.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-17 18:30 fudgeo-0.5.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-May-17 18:30 fudgeo-0.5.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1323 b- defN 23-May-17 18:30 fudgeo-0.5.1.dist-info/RECORD
-17 files, 133879 bytes uncompressed, 25952 bytes compressed:  80.6%
+-rw-r--r--  2.0 unx     2042 b- defN 23-May-18 20:04 fudgeo/geometry/base.py
+-rw-r--r--  2.0 unx     8392 b- defN 23-May-18 20:04 fudgeo/geometry/linestring.py
+-rw-r--r--  2.0 unx     6742 b- defN 23-May-18 20:04 fudgeo/geometry/linestring.pyi
+-rw-r--r--  2.0 unx    14895 b- defN 23-May-18 20:04 fudgeo/geometry/point.py
+-rw-r--r--  2.0 unx     6425 b- defN 23-May-18 20:04 fudgeo/geometry/point.pyi
+-rw-r--r--  2.0 unx    10787 b- defN 23-May-18 20:04 fudgeo/geometry/polygon.py
+-rw-r--r--  2.0 unx     9350 b- defN 23-May-18 20:04 fudgeo/geometry/polygon.pyi
+-rw-r--r--  2.0 unx    17249 b- defN 23-May-18 20:04 fudgeo/geometry/util.py
+-rw-r--r--  2.0 unx     1088 b- defN 23-May-18 20:05 fudgeo-0.5.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx    13095 b- defN 23-May-18 20:05 fudgeo-0.5.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-18 20:05 fudgeo-0.5.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-May-18 20:05 fudgeo-0.5.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1575 b- defN 23-May-18 20:05 fudgeo-0.5.2.dist-info/RECORD
+20 files, 127361 bytes uncompressed, 28642 bytes compressed:  77.5%
```

## zipnote {}

```diff
@@ -21,32 +21,41 @@
 
 Filename: fudgeo/geometry/base.py
 Comment: 
 
 Filename: fudgeo/geometry/linestring.py
 Comment: 
 
+Filename: fudgeo/geometry/linestring.pyi
+Comment: 
+
 Filename: fudgeo/geometry/point.py
 Comment: 
 
+Filename: fudgeo/geometry/point.pyi
+Comment: 
+
 Filename: fudgeo/geometry/polygon.py
 Comment: 
 
+Filename: fudgeo/geometry/polygon.pyi
+Comment: 
+
 Filename: fudgeo/geometry/util.py
 Comment: 
 
-Filename: fudgeo-0.5.1.dist-info/LICENSE
+Filename: fudgeo-0.5.2.dist-info/LICENSE
 Comment: 
 
-Filename: fudgeo-0.5.1.dist-info/METADATA
+Filename: fudgeo-0.5.2.dist-info/METADATA
 Comment: 
 
-Filename: fudgeo-0.5.1.dist-info/WHEEL
+Filename: fudgeo-0.5.2.dist-info/WHEEL
 Comment: 
 
-Filename: fudgeo-0.5.1.dist-info/top_level.txt
+Filename: fudgeo-0.5.2.dist-info/top_level.txt
 Comment: 
 
-Filename: fudgeo-0.5.1.dist-info/RECORD
+Filename: fudgeo-0.5.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fudgeo/__init__.py

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 """
 Package Initialization
 """
 
 
-__version__ = '0.5.1'
+__version__ = '0.5.2'
 
 
 if __name__ == '__main__':
     pass
```

## fudgeo/constant.py

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 Constants
 """
 
 
 from struct import pack
-from typing import Dict, List, Tuple, Union
+from typing import ClassVar, Dict, List, Tuple, Union
 
 
 DOUBLE = Tuple[float, float]
 TRIPLE = Tuple[float, float, float]
 QUADRUPLE = Tuple[float, float, float, float]
 COORDINATES = Union[List[DOUBLE], List[TRIPLE], List[QUADRUPLE]]
 
@@ -68,15 +68,29 @@
     (False, False): WKB_POINT_PRE,
     (True, False): WKB_POINT_Z_PRE,
     (False, True): WKB_POINT_M_PRE,
     (True, True): WKB_POINT_ZM_PRE,
 }
 
 
+class EnvelopeCode:
+    """
+    Envelope Code
+    """
+    empty: ClassVar[int] = 0
+    xy: ClassVar[int] = 1
+    xyz: ClassVar[int] = 2
+    xym: ClassVar[int] = 3
+    xyzm: ClassVar[int] = 4
+# End EnvelopeCode class
+
+
 HEADER_OFFSET: int = 8
-ENVELOPE_LENGTH: Dict[int, int] = {0: 0, 1: 32, 2: 48, 3: 48, 4: 64}
+ENVELOPE_LENGTH: Dict[int, int] = {
+    EnvelopeCode.empty: 0, EnvelopeCode.xy: 32, EnvelopeCode.xyz: 48,
+    EnvelopeCode.xym: 48, EnvelopeCode.xyzm: 64}
 ENVELOPE_COUNT: Dict[int, int] = {k: v // 8 for k, v in ENVELOPE_LENGTH.items()}
 ENVELOPE_OFFSET = {k: v + HEADER_OFFSET for k, v in ENVELOPE_LENGTH.items()}
 
 
 if __name__ == '__main__':
     pass
```

## fudgeo/geometry/base.py

```diff
@@ -10,24 +10,25 @@
 from fudgeo.geometry.util import EMPTY_ENVELOPE, Envelope, make_header
 
 
 class AbstractGeometry:
     """
     Abstract Geometry
     """
-    __slots__ = 'srs_id', '_env', '_args'
+    __slots__ = 'srs_id', '_env', '_args', '_is_empty'
 
     def __init__(self, srs_id: int) -> None:
         """
         Initialize the AbstractGeometry class
         """
         super().__init__()
         self.srs_id: int = srs_id
         self._env: Envelope = EMPTY_ENVELOPE
         self._args: Optional[Tuple[memoryview, int]] = None
+        self._is_empty: Optional[bool] = None
     # End init built-in
 
     @abstractmethod
     def _to_wkb(self, ary: bytearray) -> bytearray:  # pragma: nocover
         """
         To WKB
         """
```

## fudgeo/geometry/linestring.py

```diff
@@ -1,55 +1,58 @@
 # -*- coding: utf-8 -*-
 """
 Line String
 """
 
 
 from struct import pack
-from typing import List, TYPE_CHECKING
+from typing import Any, ClassVar, List, TYPE_CHECKING
 
 from fudgeo.constant import (
-    COUNT_CODE, DOUBLE, FOUR_D, QUADRUPLE, THREE_D, TRIPLE, TWO_D,
+    COUNT_CODE, EMPTY, EnvelopeCode, FOUR_D, THREE_D, TWO_D,
     WKB_LINESTRING_M_PRE, WKB_LINESTRING_PRE, WKB_LINESTRING_ZM_PRE,
     WKB_LINESTRING_Z_PRE, WKB_MULTI_LINESTRING_M_PRE, WKB_MULTI_LINESTRING_PRE,
     WKB_MULTI_LINESTRING_ZM_PRE, WKB_MULTI_LINESTRING_Z_PRE)
 from fudgeo.geometry.base import AbstractGeometry
 from fudgeo.geometry.point import Point, PointM, PointZ, PointZM
 from fudgeo.geometry.util import (
-    EMPTY_ENVELOPE, Envelope, as_array, envelope_from_coordinates,
-    envelope_from_coordinates_m, envelope_from_coordinates_z,
-    envelope_from_coordinates_zm, envelope_from_geometries,
-    envelope_from_geometries_m, envelope_from_geometries_z,
-    envelope_from_geometries_zm, lazy_unpack, pack_coordinates, unpack_line,
-    unpack_lines)
+    EMPTY_ENVELOPE, ENV_COORD, ENV_GEOM, Envelope, as_array, lazy_unpack,
+    pack_coordinates, unpack_line, unpack_lines)
 
 
 if TYPE_CHECKING:
     from numpy import ndarray
 
 
-class LineString(AbstractGeometry):
+class BaseLineString(AbstractGeometry):
     """
-    LineString
+    Base Line String
     """
     __slots__ = '_coordinates',
 
-    def __init__(self, coordinates: List[DOUBLE], srs_id: int) -> None:
+    _class: ClassVar[Any] = object
+    _dimension: ClassVar[int] = 0
+    _env_code: ClassVar[int] = EnvelopeCode.empty
+    _has_m: ClassVar[bool] = False
+    _has_z: ClassVar[bool] = False
+    _wkb_prefix: ClassVar[bytes] = EMPTY
+
+    def __init__(self, coordinates: List, srs_id: int) -> None:
         """
-        Initialize the LineString class
+        Initialize the BaseLineString class
         """
         super().__init__(srs_id=srs_id)
         self._coordinates: 'ndarray' = as_array(coordinates)
     # End init built-in
 
-    def __eq__(self, other: 'LineString') -> bool:
+    def __eq__(self, other: Any) -> bool:
         """
         Equals
         """
-        if not isinstance(other, LineString):  # pragma: nocover
+        if not isinstance(other, self.__class__):  # pragma: nocover
             return NotImplemented
         if self.srs_id != other.srs_id:
             return False
         return self.points == other.points
     # End eq built-in
 
     @property
@@ -65,346 +68,156 @@
     # End coordinates property
 
     @property
     def is_empty(self) -> bool:
         """
         Is Empty
         """
-        return not len(self.coordinates)
+        return self._is_empty or not len(self.coordinates)
     # End is_empty property
 
     @property
-    def points(self) -> List[Point]:
+    def points(self) -> List:
         """
         Points
         """
         srs_id = self.srs_id
-        return [Point(x=x, y=y, srs_id=srs_id) for x, y in self.coordinates]
+        cls = self._class
+        return [cls.from_tuple(coords, srs_id=srs_id)
+                for coords in self.coordinates]
     # End points property
 
     @property
     def envelope(self) -> Envelope:
         """
         Envelope
         """
         if self._env is not EMPTY_ENVELOPE:
             return self._env
-        env = envelope_from_coordinates(self.coordinates)
+        env = ENV_COORD[self._env_code](self.coordinates)
         self._env = env
         return env
     # End envelope property
 
     def _to_wkb(self, ary: bytearray) -> bytearray:
         """
         To WKB
         """
-        return pack_coordinates(ary, WKB_LINESTRING_PRE, self.coordinates)
+        return pack_coordinates(ary, self._wkb_prefix, self.coordinates,
+                                has_z=self._has_z, has_m=self._has_m)
     # End _to_wkb method
 
     @classmethod
-    def from_gpkg(cls, value: bytes) -> 'LineString':
+    def from_gpkg(cls, value: bytes) -> Any:
         """
         From Geopackage
         """
-        return lazy_unpack(cls=cls, value=value, dimension=TWO_D)
+        return lazy_unpack(cls=cls, value=value, dimension=cls._dimension)
     # End from_gpkg method
-# End LineString class
+# End BaseLineString class
 
 
-class LineStringZ(AbstractGeometry):
+class LineString(BaseLineString):
     """
-    LineStringZ
+    Line String
     """
     __slots__ = '_coordinates',
 
-    def __init__(self, coordinates: List[TRIPLE], srs_id: int) -> None:
-        """
-        Initialize the LineStringZ class
-        """
-        super().__init__(srs_id=srs_id)
-        self._coordinates: 'ndarray' = as_array(coordinates)
-    # End init built-in
-
-    def __eq__(self, other: 'LineStringZ') -> bool:
-        """
-        Equals
-        """
-        if not isinstance(other, LineStringZ):  # pragma: nocover
-            return NotImplemented
-        if self.srs_id != other.srs_id:
-            return False
-        return self.points == other.points
-    # End eq built-in
-
-    @property
-    def coordinates(self) -> 'ndarray':
-        """
-        Coordinates
-        """
-        if self._args:
-            self._coordinates = unpack_line(*self._args)
-            self._args = None
-        # noinspection PyTypeChecker
-        return self._coordinates
-    # End coordinates property
-
-    @property
-    def is_empty(self) -> bool:
-        """
-        Is Empty
-        """
-        return not len(self.coordinates)
-    # End is_empty property
-
-    @property
-    def points(self) -> List[PointZ]:
-        """
-        Points
-        """
-        srs_id = self.srs_id
-        return [PointZ(x=x, y=y, z=z, srs_id=srs_id)
-                for x, y, z in self.coordinates]
-    # End points property
+    _class: ClassVar[Any] = Point
+    _dimension: ClassVar[int] = TWO_D
+    _env_code: ClassVar[int] = EnvelopeCode.xy
+    _wkb_prefix: ClassVar[bytes] = WKB_LINESTRING_PRE
+# End LineString class
 
-    @property
-    def envelope(self) -> Envelope:
-        """
-        Envelope
-        """
-        if self._env is not EMPTY_ENVELOPE:
-            return self._env
-        env = envelope_from_coordinates_z(self.coordinates)
-        self._env = env
-        return env
-    # End envelope property
 
-    def _to_wkb(self, ary: bytearray) -> bytearray:
-        """
-        To WKB
-        """
-        return pack_coordinates(
-            ary, WKB_LINESTRING_Z_PRE, self.coordinates, has_z=True)
-    # End _to_wkb method
+class LineStringZ(BaseLineString):
+    """
+    Line String Z
+    """
+    __slots__ = '_coordinates',
 
-    @classmethod
-    def from_gpkg(cls, value: bytes) -> 'LineStringZ':
-        """
-        From Geopackage
-        """
-        return lazy_unpack(cls=cls, value=value, dimension=THREE_D)
-    # End from_gpkg method
+    _class: ClassVar[Any] = PointZ
+    _dimension: ClassVar[int] = THREE_D
+    _env_code: ClassVar[int] = EnvelopeCode.xyz
+    _has_z: ClassVar[bool] = True
+    _wkb_prefix: ClassVar[bytes] = WKB_LINESTRING_Z_PRE
 # End LineStringZ class
 
 
-class LineStringM(AbstractGeometry):
+class LineStringM(BaseLineString):
     """
-    LineStringM
+    Line String M
     """
     __slots__ = '_coordinates',
 
-    def __init__(self, coordinates: List[TRIPLE], srs_id: int) -> None:
-        """
-        Initialize the LineStringM class
-        """
-        super().__init__(srs_id=srs_id)
-        self._coordinates: 'ndarray' = as_array(coordinates)
-    # End init built-in
-
-    def __eq__(self, other: 'LineStringM') -> bool:
-        """
-        Equals
-        """
-        if not isinstance(other, LineStringM):  # pragma: nocover
-            return NotImplemented
-        if self.srs_id != other.srs_id:
-            return False
-        return self.points == other.points
-    # End eq built-in
-
-    @property
-    def coordinates(self) -> 'ndarray':
-        """
-        Coordinates
-        """
-        if self._args:
-            self._coordinates = unpack_line(*self._args)
-            self._args = None
-        # noinspection PyTypeChecker
-        return self._coordinates
-    # End coordinates property
-
-    @property
-    def is_empty(self) -> bool:
-        """
-        Is Empty
-        """
-        return not len(self.coordinates)
-    # End is_empty property
-
-    @property
-    def points(self) -> List[PointM]:
-        """
-        Points
-        """
-        srs_id = self.srs_id
-        return [PointM(x=x, y=y, m=m, srs_id=srs_id)
-                for x, y, m in self.coordinates]
-    # End points property
-
-    @property
-    def envelope(self) -> Envelope:
-        """
-        Envelope
-        """
-        if self._env is not EMPTY_ENVELOPE:
-            return self._env
-        env = envelope_from_coordinates_m(self.coordinates)
-        self._env = env
-        return env
-    # End envelope property
-
-    def _to_wkb(self, ary: bytearray) -> bytearray:
-        """
-        To WKB
-        """
-        return pack_coordinates(
-            ary, WKB_LINESTRING_M_PRE, self.coordinates, has_m=True)
-    # End _to_wkb method
-
-    @classmethod
-    def from_gpkg(cls, value: bytes) -> 'LineStringM':
-        """
-        From Geopackage
-        """
-        return lazy_unpack(cls=cls, value=value, dimension=THREE_D)
-    # End from_gpkg method
+    _class: ClassVar[Any] = PointM
+    _dimension: ClassVar[int] = THREE_D
+    _env_code: ClassVar[int] = EnvelopeCode.xym
+    _has_m: ClassVar[bool] = True
+    _wkb_prefix: ClassVar[bytes] = WKB_LINESTRING_M_PRE
 # End LineStringM class
 
 
-class LineStringZM(AbstractGeometry):
+class LineStringZM(BaseLineString):
     """
-    LineStringZM
+    Line String ZM
     """
     __slots__ = '_coordinates',
 
-    def __init__(self, coordinates: List[QUADRUPLE], srs_id: int) -> None:
-        """
-        Initialize the LineStringZM class
-        """
-        super().__init__(srs_id=srs_id)
-        self._coordinates: 'ndarray' = as_array(coordinates)
-    # End init built-in
-
-    def __eq__(self, other: 'LineStringZM') -> bool:
-        """
-        Equals
-        """
-        if not isinstance(other, LineStringZM):  # pragma: nocover
-            return NotImplemented
-        if self.srs_id != other.srs_id:
-            return False
-        return self.points == other.points
-    # End eq built-in
-
-    @property
-    def coordinates(self) -> 'ndarray':
-        """
-        Coordinates
-        """
-        if self._args:
-            self._coordinates = unpack_line(*self._args)
-            self._args = None
-        # noinspection PyTypeChecker
-        return self._coordinates
-    # End coordinates property
-
-    @property
-    def is_empty(self) -> bool:
-        """
-        Is Empty
-        """
-        return not len(self.coordinates)
-    # End is_empty property
-
-    @property
-    def points(self) -> List[PointZM]:
-        """
-        Points
-        """
-        srs_id = self.srs_id
-        return [PointZM(x=x, y=y, z=z, m=m, srs_id=srs_id)
-                for x, y, z, m in self.coordinates]
-    # End points property
-
-    @property
-    def envelope(self) -> Envelope:
-        """
-        Envelope
-        """
-        if self._env is not EMPTY_ENVELOPE:
-            return self._env
-        env = envelope_from_coordinates_zm(self.coordinates)
-        self._env = env
-        return env
-    # End envelope property
-
-    def _to_wkb(self, ary: bytearray) -> bytearray:
-        """
-        To WKB
-        """
-        return pack_coordinates(
-            ary, WKB_LINESTRING_ZM_PRE, self.coordinates,
-            has_z=True, has_m=True)
-    # End _to_wkb method
-
-    @classmethod
-    def from_gpkg(cls, value: bytes) -> 'LineStringZM':
-        """
-        From Geopackage
-        """
-        return lazy_unpack(cls=cls, value=value, dimension=FOUR_D)
-    # End from_gpkg method
+    _class: ClassVar[Any] = PointZM
+    _dimension: ClassVar[int] = FOUR_D
+    _env_code: ClassVar[int] = EnvelopeCode.xyzm
+    _has_m: ClassVar[bool] = True
+    _has_z: ClassVar[bool] = True
+    _wkb_prefix: ClassVar[bytes] = WKB_LINESTRING_ZM_PRE
 # End LineStringZM class
 
 
-class MultiLineString(AbstractGeometry):
+class BaseMultiLineString(AbstractGeometry):
     """
-    Multi LineString
+    Base Multi Line String
     """
     __slots__ = '_lines',
 
-    def __init__(self, coordinates: List[List[DOUBLE]], srs_id: int) -> None:
+    _class: ClassVar[Any] = object
+    _dimension: ClassVar[int] = 0
+    _env_code: ClassVar[int] = EnvelopeCode.empty
+    _wkb_prefix: ClassVar[bytes] = EMPTY
+
+    def __init__(self, coordinates: List[List], srs_id: int) -> None:
         """
         Initialize the MultiLineString class
         """
         super().__init__(srs_id=srs_id)
         self._lines: List[LineString] = self._make_lines(coordinates)
     # End init built-in
 
-    def __eq__(self, other: 'MultiLineString') -> bool:
+    def __eq__(self, other: Any) -> bool:
         """
         Equals
         """
-        if not isinstance(other, MultiLineString):  # pragma: nocover
+        if not isinstance(other, self.__class__):  # pragma: nocover
             return NotImplemented
         if self.srs_id != other.srs_id:
             return False
         return self.lines == other.lines
     # End eq built-in
 
-    def _make_lines(self, coordinates: List[List[DOUBLE]]) -> List[LineString]:
+    def _make_lines(self, coordinates: List[List]) -> List:
         """
         Make Lines
         """
         srs_id = self.srs_id
-        return [LineString(coords, srs_id=srs_id) for coords in coordinates]
+        cls = self._class
+        # noinspection PyArgumentList
+        return [cls(coords, srs_id=srs_id) for coords in coordinates]
     # End init built-in
 
     @property
-    def lines(self) -> List[LineString]:
+    def lines(self) -> List:
         """
         Lines
         """
         if self._args:
             # noinspection PyTypeChecker
             self._lines = self._make_lines(unpack_lines(*self._args))
             self._args = None
@@ -412,296 +225,95 @@
     # End lines property
 
     @property
     def is_empty(self) -> bool:
         """
         Is Empty
         """
-        return not (bool(self._args) or bool(self.lines))
+        return self._is_empty or not (bool(self._args) or bool(self.lines))
     # End is_empty property
 
     def _to_wkb(self, ary: bytearray) -> bytearray:
         """
         To WKB
         """
         geoms = self.lines
-        ary.extend(WKB_MULTI_LINESTRING_PRE + pack(COUNT_CODE, len(geoms)))
+        ary.extend(self._wkb_prefix + pack(COUNT_CODE, len(geoms)))
         return self._join_geometries(ary, geoms)
     # End _to_wkb method
 
     @property
     def envelope(self) -> Envelope:
         """
         Envelope
         """
         if self._env is not EMPTY_ENVELOPE:
             return self._env
-        env = envelope_from_geometries(self.lines)
+        env = ENV_GEOM[self._env_code](self.lines)
         self._env = env
         return env
     # End envelope property
 
     @classmethod
-    def from_gpkg(cls, value: bytes) -> 'MultiLineString':
+    def from_gpkg(cls, value: bytes) -> Any:
         """
         From Geopackage
         """
-        return lazy_unpack(cls=cls, value=value, dimension=TWO_D)
+        return lazy_unpack(cls=cls, value=value, dimension=cls._dimension)
     # End from_gpkg method
-# End MultiLineString class
+# End BaseMultiLineString class
 
 
-class MultiLineStringZ(AbstractGeometry):
+class MultiLineString(BaseMultiLineString):
     """
-    Multi LineString Z
+    Multi Line String
     """
     __slots__ = '_lines',
 
-    def __init__(self, coordinates: List[List[TRIPLE]], srs_id: int) -> None:
-        """
-        Initialize the MultiLineStringZ class
-        """
-        super().__init__(srs_id=srs_id)
-        self._lines: List[LineStringZ] = self._make_lines(coordinates)
-    # End init built-in
-
-    def __eq__(self, other: 'MultiLineStringZ') -> bool:
-        """
-        Equals
-        """
-        if not isinstance(other, MultiLineStringZ):  # pragma: nocover
-            return NotImplemented
-        if self.srs_id != other.srs_id:
-            return False
-        return self.lines == other.lines
-    # End eq built-in
-
-    def _make_lines(self, coordinates: List[List[TRIPLE]]) -> List[LineStringZ]:
-        """
-        Make Lines
-        """
-        srs_id = self.srs_id
-        return [LineStringZ(coords, srs_id=srs_id) for coords in coordinates]
-    # End init built-in
-
-    @property
-    def lines(self) -> List[LineStringZ]:
-        """
-        Lines
-        """
-        if self._args:
-            # noinspection PyTypeChecker
-            self._lines = self._make_lines(unpack_lines(*self._args))
-            self._args = None
-        return self._lines
-    # End lines property
+    _class: ClassVar[Any] = LineString
+    _dimension: ClassVar[int] = TWO_D
+    _env_code: ClassVar[int] = EnvelopeCode.xy
+    _wkb_prefix: ClassVar[bytes] = WKB_MULTI_LINESTRING_PRE
+# End MultiLineString class
 
-    @property
-    def is_empty(self) -> bool:
-        """
-        Is Empty
-        """
-        return not (bool(self._args) or bool(self.lines))
-    # End is_empty property
 
-    @property
-    def envelope(self) -> Envelope:
-        """
-        Envelope
-        """
-        if self._env is not EMPTY_ENVELOPE:
-            return self._env
-        env = envelope_from_geometries_z(self.lines)
-        self._env = env
-        return env
-    # End envelope property
-
-    def _to_wkb(self, ary: bytearray) -> bytearray:
-        """
-        To WKB
-        """
-        geoms = self.lines
-        ary.extend(WKB_MULTI_LINESTRING_Z_PRE + pack(COUNT_CODE, len(geoms)))
-        return self._join_geometries(ary, geoms)
-    # End _to_wkb method
+class MultiLineStringZ(BaseMultiLineString):
+    """
+    Multi Line String Z
+    """
+    __slots__ = '_lines',
 
-    @classmethod
-    def from_gpkg(cls, value: bytes) -> 'MultiLineStringZ':
-        """
-        From Geopackage
-        """
-        return lazy_unpack(cls=cls, value=value, dimension=THREE_D)
-    # End from_gpkg method
+    _class: ClassVar[Any] = LineStringZ
+    _dimension: ClassVar[int] = THREE_D
+    _env_code: ClassVar[int] = EnvelopeCode.xyz
+    _wkb_prefix: ClassVar[bytes] = WKB_MULTI_LINESTRING_Z_PRE
 # End MultiLineStringZ class
 
 
-class MultiLineStringM(AbstractGeometry):
+class MultiLineStringM(BaseMultiLineString):
     """
-    Multi LineString M
+    Multi Line String M
     """
     __slots__ = '_lines',
 
-    def __init__(self, coordinates: List[List[TRIPLE]], srs_id: int) -> None:
-        """
-        Initialize the MultiLineStringM class
-        """
-        super().__init__(srs_id=srs_id)
-        self._lines: List[LineStringM] = self._make_lines(coordinates)
-    # End init built-in
-
-    def __eq__(self, other: 'MultiLineStringM') -> bool:
-        """
-        Equals
-        """
-        if not isinstance(other, MultiLineStringM):  # pragma: nocover
-            return NotImplemented
-        if self.srs_id != other.srs_id:
-            return False
-        return self.lines == other.lines
-    # End eq built-in
-
-    def _make_lines(self, coordinates: List[List[TRIPLE]]) -> List[LineStringM]:
-        """
-        Make Lines
-        """
-        srs_id = self.srs_id
-        return [LineStringM(coords, srs_id=srs_id) for coords in coordinates]
-    # End init built-in
-
-    @property
-    def lines(self) -> List[LineStringM]:
-        """
-        Lines
-        """
-        if self._args:
-            # noinspection PyTypeChecker
-            self._lines = self._make_lines(unpack_lines(*self._args))
-            self._args = None
-        return self._lines
-    # End lines property
-
-    @property
-    def is_empty(self) -> bool:
-        """
-        Is Empty
-        """
-        return not (bool(self._args) or bool(self.lines))
-    # End is_empty property
-
-    @property
-    def envelope(self) -> Envelope:
-        """
-        Envelope
-        """
-        if self._env is not EMPTY_ENVELOPE:
-            return self._env
-        env = envelope_from_geometries_m(self.lines)
-        self._env = env
-        return env
-    # End envelope property
-
-    def _to_wkb(self, ary: bytearray) -> bytearray:
-        """
-        To WKB
-        """
-        geoms = self.lines
-        ary.extend(WKB_MULTI_LINESTRING_M_PRE + pack(COUNT_CODE, len(geoms)))
-        return self._join_geometries(ary, geoms)
-    # End _to_wkb method
-
-    @classmethod
-    def from_gpkg(cls, value: bytes) -> 'MultiLineStringM':
-        """
-        From Geopackage
-        """
-        return lazy_unpack(cls=cls, value=value, dimension=THREE_D)
-    # End from_gpkg method
+    _class: ClassVar[Any] = LineStringM
+    _dimension: ClassVar[int] = THREE_D
+    _env_code: ClassVar[int] = EnvelopeCode.xym
+    _wkb_prefix: ClassVar[bytes] = WKB_MULTI_LINESTRING_M_PRE
 # End MultiLineStringM class
 
 
-class MultiLineStringZM(AbstractGeometry):
+class MultiLineStringZM(BaseMultiLineString):
     """
-    Multi LineString ZM
+    Multi Line String ZM
     """
     __slots__ = '_lines',
 
-    def __init__(self, coordinates: List[List[QUADRUPLE]], srs_id: int) -> None:
-        """
-        Initialize the MultiLineStringZM class
-        """
-        super().__init__(srs_id=srs_id)
-        self._lines: List[LineStringZM] = self._make_lines(coordinates)
-    # End init built-in
-
-    def __eq__(self, other: 'MultiLineStringZM') -> bool:
-        """
-        Equals
-        """
-        if not isinstance(other, MultiLineStringZM):  # pragma: nocover
-            return NotImplemented
-        if self.srs_id != other.srs_id:
-            return False
-        return self.lines == other.lines
-    # End eq built-in
-
-    def _make_lines(self, coordinates: List[List[QUADRUPLE]]) \
-            -> List[LineStringZM]:
-        """
-        Make Lines
-        """
-        srs_id = self.srs_id
-        return [LineStringZM(coords, srs_id=srs_id) for coords in coordinates]
-    # End init built-in
-
-    @property
-    def lines(self) -> List[LineStringZM]:
-        """
-        Lines
-        """
-        if self._args:
-            # noinspection PyTypeChecker
-            self._lines = self._make_lines(unpack_lines(*self._args))
-            self._args = None
-        return self._lines
-    # End lines property
-
-    @property
-    def is_empty(self) -> bool:
-        """
-        Is Empty
-        """
-        return not (bool(self._args) or bool(self.lines))
-    # End is_empty property
-
-    @property
-    def envelope(self) -> Envelope:
-        """
-        Envelope
-        """
-        if self._env is not EMPTY_ENVELOPE:
-            return self._env
-        env = envelope_from_geometries_zm(self.lines)
-        self._env = env
-        return env
-    # End envelope property
-
-    def _to_wkb(self, ary: bytearray) -> bytearray:
-        """
-        To WKB
-        """
-        geoms = self.lines
-        ary.extend(WKB_MULTI_LINESTRING_ZM_PRE + pack(COUNT_CODE, len(geoms)))
-        return self._join_geometries(ary, geoms)
-    # End _to_wkb method
-
-    @classmethod
-    def from_gpkg(cls, value: bytes) -> 'MultiLineStringZM':
-        """
-        From Geopackage
-        """
-        return lazy_unpack(cls=cls, value=value, dimension=FOUR_D)
-    # End from_gpkg method
+    _class: ClassVar[Any] = LineStringZM
+    _dimension: ClassVar[int] = FOUR_D
+    _env_code: ClassVar[int] = EnvelopeCode.xyzm
+    _wkb_prefix: ClassVar[bytes] = WKB_MULTI_LINESTRING_ZM_PRE
 # End MultiLineStringZM class
 
 
 if __name__ == '__main__':  # pragma: no cover
     pass
```

## fudgeo/geometry/point.py

```diff
@@ -2,29 +2,26 @@
 """
 Points
 """
 
 
 from math import isnan, nan
 from struct import pack, unpack
-from typing import List, Optional, TYPE_CHECKING
+from typing import Any, ClassVar, List, Optional, TYPE_CHECKING
 
 from fudgeo.constant import (
-    DOUBLE, FOUR_D, FOUR_D_PACK_CODE, FOUR_D_UNPACK_CODE, HEADER_OFFSET,
-    QUADRUPLE, THREE_D, THREE_D_PACK_CODE, THREE_D_UNPACK_CODE, TRIPLE, TWO_D,
-    TWO_D_PACK_CODE, TWO_D_UNPACK_CODE, WKB_MULTI_POINT_M_PRE,
+    DOUBLE, EMPTY, EnvelopeCode, FOUR_D, FOUR_D_PACK_CODE, FOUR_D_UNPACK_CODE,
+    HEADER_OFFSET, QUADRUPLE, THREE_D, THREE_D_PACK_CODE, THREE_D_UNPACK_CODE,
+    TRIPLE, TWO_D, TWO_D_PACK_CODE, TWO_D_UNPACK_CODE, WKB_MULTI_POINT_M_PRE,
     WKB_MULTI_POINT_PRE, WKB_MULTI_POINT_ZM_PRE, WKB_MULTI_POINT_Z_PRE,
     WKB_POINT_M_PRE, WKB_POINT_PRE, WKB_POINT_ZM_PRE, WKB_POINT_Z_PRE)
 from fudgeo.geometry.base import AbstractGeometry
 from fudgeo.geometry.util import (
-    EMPTY_ENVELOPE, Envelope, as_array, envelope_from_coordinates,
-    envelope_from_coordinates_m, envelope_from_coordinates_z,
-    envelope_from_coordinates_zm, lazy_unpack, make_header, pack_coordinates,
-    unpack_header, unpack_points)
-
+    EMPTY_ENVELOPE, ENV_COORD, Envelope, as_array, lazy_unpack, make_header,
+    pack_coordinates, unpack_header, unpack_points)
 
 if TYPE_CHECKING:
     from numpy import ndarray
 
 
 class Point(AbstractGeometry):
     """
@@ -422,33 +419,40 @@
         Empty Point
         """
         return cls(x=nan, y=nan, z=nan, m=nan, srs_id=srs_id)
     # End empty method
 # End PointZM class
 
 
-class MultiPoint(AbstractGeometry):
+class BaseMultiPoint(AbstractGeometry):
     """
-    Multi Point
+    Base Multi Point
     """
     __slots__ = '_coordinates',
 
-    def __init__(self, coordinates: List[DOUBLE], srs_id: int) -> None:
+    _class: ClassVar[Any] = object
+    _dimension: ClassVar[int] = 0
+    _env_code: ClassVar[int] = EnvelopeCode.empty
+    _has_m: ClassVar[bool] = False
+    _has_z: ClassVar[bool] = False
+    _wkb_prefix: ClassVar[bytes] = EMPTY
+
+    def __init__(self, coordinates: List, srs_id: int) -> None:
         """
-        Initialize the MultiPoint class
+        Initialize the BaseMultiPoint class
         """
         super().__init__(srs_id=srs_id)
         self._coordinates: 'ndarray' = as_array(coordinates)
     # End init built-in
 
-    def __eq__(self, other: 'MultiPoint') -> bool:
+    def __eq__(self, other: Any) -> bool:
         """
         Equals
         """
-        if not isinstance(other, MultiPoint):  # pragma: nocover
+        if not isinstance(other, self.__class__):  # pragma: nocover
             return NotImplemented
         if self.srs_id != other.srs_id:
             return False
         return self.points == other.points
     # End eq built-in
 
     @property
@@ -464,309 +468,111 @@
     # End coordinates property
 
     @property
     def is_empty(self) -> bool:
         """
         Is Empty
         """
-        return not len(self.coordinates)
+        return self._is_empty or not len(self.coordinates)
     # End is_empty property
 
     @property
-    def points(self) -> List[Point]:
+    def points(self) -> List:
         """
         Points
         """
         srs_id = self.srs_id
-        return [Point(x=x, y=y, srs_id=srs_id) for x, y in self.coordinates]
+        cls = self._class
+        return [cls.from_tuple(coords, srs_id=srs_id)
+                for coords in self.coordinates]
     # End points property
 
     @property
     def envelope(self) -> Envelope:
         """
         Envelope
         """
         if self._env is not EMPTY_ENVELOPE:
             return self._env
-        env = envelope_from_coordinates(self.coordinates)
+        env = ENV_COORD[self._env_code](self.coordinates)
         self._env = env
         return env
     # End envelope property
 
     def _to_wkb(self, ary: bytearray) -> bytearray:
         """
         To WKB
         """
         return pack_coordinates(
-            ary, WKB_MULTI_POINT_PRE, self.coordinates, use_point_prefix=True)
+            ary, self._wkb_prefix, self.coordinates,
+            has_z=self._has_z, has_m=self._has_m,
+            use_point_prefix=True)
     # End _to_wkb method
 
     @classmethod
-    def from_gpkg(cls, value: bytes) -> 'MultiPoint':
+    def from_gpkg(cls, value: bytes) -> Any:
         """
         From Geopackage
         """
-        return lazy_unpack(cls=cls, value=value, dimension=TWO_D)
+        return lazy_unpack(cls=cls, value=value, dimension=cls._dimension)
     # End from_gpkg method
-# End MultiPoint class
+# End BaseMultiPoint class
 
 
-class MultiPointZ(AbstractGeometry):
+class MultiPoint(BaseMultiPoint):
     """
-    Multi Point Z
+    Multi Point
     """
     __slots__ = '_coordinates',
 
-    def __init__(self, coordinates: List[TRIPLE], srs_id: int) -> None:
-        """
-        Initialize the MultiPointZ class
-        """
-        super().__init__(srs_id=srs_id)
-        self._coordinates: 'ndarray' = as_array(coordinates)
-    # End init built-in
-
-    def __eq__(self, other: 'MultiPointZ') -> bool:
-        """
-        Equals
-        """
-        if not isinstance(other, MultiPointZ):  # pragma: nocover
-            return NotImplemented
-        if self.srs_id != other.srs_id:
-            return False
-        return self.points == other.points
-    # End eq built-in
-
-    @property
-    def coordinates(self) -> 'ndarray':
-        """
-        Coordinates
-        """
-        if self._args:
-            self._coordinates = unpack_points(*self._args)
-            self._args = None
-        # noinspection PyTypeChecker
-        return self._coordinates
-    # End coordinates property
-
-    @property
-    def is_empty(self) -> bool:
-        """
-        Is Empty
-        """
-        return not len(self.coordinates)
-    # End is_empty property
-
-    @property
-    def points(self) -> List[PointZ]:
-        """
-        Points
-        """
-        srs_id = self.srs_id
-        return [PointZ(x=x, y=y, z=z, srs_id=srs_id)
-                for x, y, z in self.coordinates]
-    # End points property
+    _class: ClassVar[Any] = Point
+    _dimension: ClassVar[int] = TWO_D
+    _env_code: ClassVar[int] = EnvelopeCode.xy
+    _wkb_prefix: ClassVar[bytes] = WKB_MULTI_POINT_PRE
+# End MultiPoint class
 
-    @property
-    def envelope(self) -> Envelope:
-        """
-        Envelope
-        """
-        if self._env is not EMPTY_ENVELOPE:
-            return self._env
-        env = envelope_from_coordinates_z(self.coordinates)
-        self._env = env
-        return env
-    # End envelope property
 
-    def _to_wkb(self, ary: bytearray) -> bytearray:
-        """
-        To WKB
-        """
-        return pack_coordinates(
-            ary, WKB_MULTI_POINT_Z_PRE, self.coordinates,
-            has_z=True, use_point_prefix=True)
-    # End _to_wkb method
+class MultiPointZ(BaseMultiPoint):
+    """
+    Multi Point Z
+    """
+    __slots__ = '_coordinates',
 
-    @classmethod
-    def from_gpkg(cls, value: bytes) -> 'MultiPointZ':
-        """
-        From Geopackage
-        """
-        return lazy_unpack(cls=cls, value=value, dimension=THREE_D)
-    # End from_gpkg method
+    _class: ClassVar[Any] = PointZ
+    _dimension: ClassVar[int] = THREE_D
+    _env_code: ClassVar[int] = EnvelopeCode.xyz
+    _has_z: ClassVar[bool] = True
+    _wkb_prefix: ClassVar[bytes] = WKB_MULTI_POINT_Z_PRE
 # End MultiPointZ class
 
 
-class MultiPointM(AbstractGeometry):
+class MultiPointM(BaseMultiPoint):
     """
     Multi Point M
     """
     __slots__ = '_coordinates',
 
-    def __init__(self, coordinates: List[TRIPLE], srs_id: int) -> None:
-        """
-        Initialize the MultiPointM class
-        """
-        super().__init__(srs_id=srs_id)
-        self._coordinates: 'ndarray' = as_array(coordinates)
-    # End init built-in
-
-    def __eq__(self, other: 'MultiPointM') -> bool:
-        """
-        Equals
-        """
-        if not isinstance(other, MultiPointM):  # pragma: nocover
-            return NotImplemented
-        if self.srs_id != other.srs_id:
-            return False
-        return self.points == other.points
-    # End eq built-in
-
-    @property
-    def coordinates(self) -> 'ndarray':
-        """
-        Coordinates
-        """
-        if self._args:
-            self._coordinates = unpack_points(*self._args)
-            self._args = None
-        # noinspection PyTypeChecker
-        return self._coordinates
-    # End coordinates property
-
-    @property
-    def is_empty(self) -> bool:
-        """
-        Is Empty
-        """
-        return not len(self.coordinates)
-    # End is_empty property
-
-    @property
-    def points(self) -> List[PointM]:
-        """
-        Points
-        """
-        srs_id = self.srs_id
-        return [PointM(x=x, y=y, m=m, srs_id=srs_id)
-                for x, y, m in self.coordinates]
-    # End points property
-
-    @property
-    def envelope(self) -> Envelope:
-        """
-        Envelope
-        """
-        if self._env is not EMPTY_ENVELOPE:
-            return self._env
-        env = envelope_from_coordinates_m(self.coordinates)
-        self._env = env
-        return env
-    # End envelope property
-
-    def _to_wkb(self, ary: bytearray) -> bytearray:
-        """
-        To WKB
-        """
-        return pack_coordinates(
-            ary, WKB_MULTI_POINT_M_PRE, self.coordinates,
-            has_m=True, use_point_prefix=True)
-    # End _to_wkb method
-
-    @classmethod
-    def from_gpkg(cls, value: bytes) -> 'MultiPointM':
-        """
-        From Geopackage
-        """
-        return lazy_unpack(cls=cls, value=value, dimension=THREE_D)
-    # End from_gpkg method
+    _class: ClassVar[Any] = PointM
+    _dimension: ClassVar[int] = THREE_D
+    _env_code: ClassVar[int] = EnvelopeCode.xym
+    _has_m: ClassVar[bool] = True
+    _wkb_prefix: ClassVar[bytes] = WKB_MULTI_POINT_M_PRE
 # End MultiPointM class
 
 
-class MultiPointZM(AbstractGeometry):
+class MultiPointZM(BaseMultiPoint):
     """
     Multi Point ZM
     """
     __slots__ = '_coordinates',
 
-    def __init__(self, coordinates: List[QUADRUPLE], srs_id: int) -> None:
-        """
-        Initialize the MultiPointZM class
-        """
-        super().__init__(srs_id=srs_id)
-        self._coordinates: 'ndarray' = as_array(coordinates)
-    # End init built-in
-
-    def __eq__(self, other: 'MultiPointZM') -> bool:
-        """
-        Equals
-        """
-        if not isinstance(other, MultiPointZM):  # pragma: nocover
-            return NotImplemented
-        if self.srs_id != other.srs_id:
-            return False
-        return self.points == other.points
-    # End eq built-in
-
-    @property
-    def coordinates(self) -> 'ndarray':
-        """
-        Coordinates
-        """
-        if self._args:
-            self._coordinates = unpack_points(*self._args)
-            self._args = None
-        # noinspection PyTypeChecker
-        return self._coordinates
-    # End coordinates property
-
-    @property
-    def is_empty(self) -> bool:
-        """
-        Is Empty
-        """
-        return not len(self.coordinates)
-    # End is_empty property
-
-    @property
-    def points(self) -> List[PointZM]:
-        """
-        Points
-        """
-        srs_id = self.srs_id
-        return [PointZM(x=x, y=y, z=z, m=m, srs_id=srs_id)
-                for x, y, z, m in self.coordinates]
-    # End points property
-
-    @property
-    def envelope(self) -> Envelope:
-        """
-        Envelope
-        """
-        if self._env is not EMPTY_ENVELOPE:
-            return self._env
-        env = envelope_from_coordinates_zm(self.coordinates)
-        self._env = env
-        return env
-    # End envelope property
-
-    def _to_wkb(self, ary: bytearray) -> bytearray:
-        """
-        To WKB
-        """
-        return pack_coordinates(
-            ary, WKB_MULTI_POINT_ZM_PRE, self.coordinates,
-            has_z=True, has_m=True, use_point_prefix=True)
-    # End _to_wkb method
-
-    @classmethod
-    def from_gpkg(cls, value: bytes) -> 'MultiPointZM':
-        """
-        From Geopackage
-        """
-        return lazy_unpack(cls=cls, value=value, dimension=FOUR_D)
-    # End from_gpkg method
+    _class: ClassVar[Any] = PointZM
+    _dimension: ClassVar[int] = FOUR_D
+    _env_code: ClassVar[int] = EnvelopeCode.xyzm
+    _has_m: ClassVar[bool] = True
+    _has_z: ClassVar[bool] = True
+    _wkb_prefix: ClassVar[bytes] = WKB_MULTI_POINT_ZM_PRE
 # End MultiPointZM class
 
 
 if __name__ == '__main__':  # pragma: no cover
     pass
```

## fudgeo/geometry/polygon.py

```diff
@@ -1,55 +1,54 @@
 # -*- coding: utf-8 -*-
 """
 Polygons
 """
 
 
 from struct import pack
-from typing import List, TYPE_CHECKING
+from typing import Any, ClassVar, List, TYPE_CHECKING
 
 from fudgeo.constant import (
-    COUNT_CODE, DOUBLE, EMPTY, FOUR_D, QUADRUPLE, THREE_D, TRIPLE, TWO_D,
+    COUNT_CODE, EMPTY, EnvelopeCode, FOUR_D, THREE_D, TWO_D,
     WKB_MULTI_POLYGON_M_PRE, WKB_MULTI_POLYGON_PRE, WKB_MULTI_POLYGON_ZM_PRE,
     WKB_MULTI_POLYGON_Z_PRE, WKB_POLYGON_M_PRE, WKB_POLYGON_PRE,
     WKB_POLYGON_ZM_PRE, WKB_POLYGON_Z_PRE)
 from fudgeo.geometry.base import AbstractGeometry
 from fudgeo.geometry.point import Point, PointM, PointZ, PointZM
 from fudgeo.geometry.util import (
-    EMPTY_ENVELOPE, Envelope, as_array, envelope_from_coordinates,
-    envelope_from_coordinates_m, envelope_from_coordinates_z,
-    envelope_from_coordinates_zm, envelope_from_geometries,
-    envelope_from_geometries_m, envelope_from_geometries_z,
-    envelope_from_geometries_zm, lazy_unpack, pack_coordinates, unpack_lines,
-    unpack_polygons)
+    EMPTY_ENVELOPE, ENV_COORD, ENV_GEOM, Envelope, as_array, lazy_unpack,
+    pack_coordinates, unpack_lines, unpack_polygons)
 
 
 if TYPE_CHECKING:
     from numpy import ndarray
 
 
-class LinearRing(AbstractGeometry):
+class BaseLinearRing(AbstractGeometry):
     """
-    Linear Ring
+    Base Linear Ring
     """
     __slots__ = 'coordinates',
 
-    def __init__(self, coordinates: List[DOUBLE], srs_id: int) -> None:
+    _class: ClassVar[Any] = object
+    _env_code: ClassVar[int] = EnvelopeCode.empty
+
+    def __init__(self, coordinates: List, srs_id: int) -> None:
         """
-        Initialize the LinearRing class
+        Initialize the BaseLinearRing class
         """
         super().__init__(srs_id=srs_id)
         self.coordinates: 'ndarray' = as_array(coordinates)
     # End init built-in
 
-    def __eq__(self, other: 'LinearRing') -> bool:
+    def __eq__(self, other: Any) -> bool:
         """
         Equals
         """
-        if not isinstance(other, LinearRing):  # pragma: nocover
+        if not isinstance(other, self.__class__):  # pragma: nocover
             return NotImplemented
         if self.srs_id != other.srs_id:
             return False
         return self.points == other.points
     # End eq built-in
 
     @property
@@ -57,301 +56,138 @@
         """
         Is Empty
         """
         return not len(self.coordinates)
     # End is_empty property
 
     @property
-    def points(self) -> List[Point]:
+    def points(self) -> List:
         """
         Points
         """
         srs_id = self.srs_id
-        return [Point(x=x, y=y, srs_id=srs_id) for x, y in self.coordinates]
+        cls = self._class
+        return [cls.from_tuple(coords, srs_id=srs_id)
+                for coords in self.coordinates]
     # End points property
 
     @property
     def envelope(self) -> Envelope:
         """
         Envelope
         """
         if self._env is not EMPTY_ENVELOPE:
             return self._env
-        env = envelope_from_coordinates(self.coordinates)
+        env = ENV_COORD[self._env_code](self.coordinates)
         self._env = env
         return env
     # End envelope property
 
     def _to_wkb(self, ary: bytearray) -> bytearray:
         """
         To WKB
         """
         return pack_coordinates(ary, EMPTY, self.coordinates)
     # End _to_wkb method
 
     @classmethod
-    def from_gpkg(cls, value: bytes) -> 'LinearRing':  # pragma: nocover
+    def from_gpkg(cls, value: bytes) -> Any:  # pragma: nocover
         """
         From Geopackage, no-op for Linear Ring
         """
         pass
     # End from_gpkg method
-# End LinearRing class
+# End BaseLinearRing class
 
 
-class LinearRingZ(AbstractGeometry):
+class LinearRing(BaseLinearRing):
     """
-    Linear Ring Z
+    Linear Ring
     """
     __slots__ = 'coordinates',
 
-    def __init__(self, coordinates: List[TRIPLE], srs_id: int) -> None:
-        """
-        Initialize the LinearRingZ class
-        """
-        super().__init__(srs_id=srs_id)
-        self.coordinates: 'ndarray' = as_array(coordinates)
-    # End init built-in
-
-    def __eq__(self, other: 'LinearRingZ') -> bool:
-        """
-        Equals
-        """
-        if not isinstance(other, LinearRingZ):  # pragma: nocover
-            return NotImplemented
-        if self.srs_id != other.srs_id:
-            return False
-        return self.points == other.points
-    # End eq built-in
-
-    @property
-    def is_empty(self) -> bool:
-        """
-        Is Empty
-        """
-        return not len(self.coordinates)
-    # End is_empty property
-
-    @property
-    def points(self) -> List[PointZ]:
-        """
-        Points
-        """
-        srs_id = self.srs_id
-        return [PointZ(x=x, y=y, z=z, srs_id=srs_id)
-                for x, y, z in self.coordinates]
-    # End points property
+    _class: ClassVar[Any] = Point
+    _env_code: ClassVar[int] = EnvelopeCode.xy
+# End LinearRing class
 
-    def _to_wkb(self, ary: bytearray) -> bytearray:
-        """
-        To WKB
-        """
-        return pack_coordinates(ary, EMPTY, self.coordinates, has_z=True)
-    # End _to_wkb method
 
-    @property
-    def envelope(self) -> Envelope:
-        """
-        Envelope
-        """
-        if self._env is not EMPTY_ENVELOPE:
-            return self._env
-        env = envelope_from_coordinates_z(self.coordinates)
-        self._env = env
-        return env
-    # End envelope property
+class LinearRingZ(BaseLinearRing):
+    """
+    Linear Ring Z
+    """
+    __slots__ = 'coordinates',
 
-    @classmethod
-    def from_gpkg(cls, value: bytes) -> 'LinearRingZ':  # pragma: nocover
-        """
-        From Geopackage, no-op for Linear Ring
-        """
-        pass
-    # End from_gpkg method
+    _class: ClassVar[Any] = PointZ
+    _env_code: ClassVar[int] = EnvelopeCode.xyz
 # End LinearRingZ class
 
 
-class LinearRingM(AbstractGeometry):
+class LinearRingM(BaseLinearRing):
     """
     Linear Ring M
     """
     __slots__ = 'coordinates',
 
-    def __init__(self, coordinates: List[TRIPLE], srs_id: int) -> None:
-        """
-        Initialize the LinearRingM class
-        """
-        super().__init__(srs_id=srs_id)
-        self.coordinates: 'ndarray' = as_array(coordinates)
-    # End init built-in
-
-    def __eq__(self, other: 'LinearRingM') -> bool:
-        """
-        Equals
-        """
-        if not isinstance(other, LinearRingM):  # pragma: nocover
-            return NotImplemented
-        if self.srs_id != other.srs_id:
-            return False
-        return self.points == other.points
-    # End eq built-in
-
-    @property
-    def is_empty(self) -> bool:
-        """
-        Is Empty
-        """
-        return not len(self.coordinates)
-    # End is_empty property
-
-    @property
-    def points(self) -> List[PointM]:
-        """
-        Points
-        """
-        srs_id = self.srs_id
-        return [PointM(x=x, y=y, m=m, srs_id=srs_id)
-                for x, y, m in self.coordinates]
-    # End points property
-
-    @property
-    def envelope(self) -> Envelope:
-        """
-        Envelope
-        """
-        if self._env is not EMPTY_ENVELOPE:
-            return self._env
-        env = envelope_from_coordinates_m(self.coordinates)
-        self._env = env
-        return env
-    # End envelope property
-
-    def _to_wkb(self, ary: bytearray) -> bytearray:
-        """
-        To WKB
-        """
-        return pack_coordinates(ary, EMPTY, self.coordinates, has_m=True)
-    # End _to_wkb method
-
-    @classmethod
-    def from_gpkg(cls, value: bytes) -> 'LinearRingM':  # pragma: nocover
-        """
-        From Geopackage, no-op for Linear Ring
-        """
-        pass
-    # End from_gpkg method
+    _class: ClassVar[Any] = PointM
+    _env_code: ClassVar[int] = EnvelopeCode.xym
 # End LinearRingM class
 
 
-class LinearRingZM(AbstractGeometry):
+class LinearRingZM(BaseLinearRing):
     """
     Linear Ring ZM
     """
     __slots__ = 'coordinates',
 
-    def __init__(self, coordinates: List[QUADRUPLE], srs_id: int) -> None:
-        """
-        Initialize the LinearRingZM class
-        """
-        super().__init__(srs_id=srs_id)
-        self.coordinates: 'ndarray' = as_array(coordinates)
-    # End init built-in
-
-    def __eq__(self, other: 'LinearRingZM') -> bool:
-        """
-        Equals
-        """
-        if not isinstance(other, LinearRingZM):  # pragma: nocover
-            return NotImplemented
-        return self.points == other.points
-    # End eq built-in
-
-    @property
-    def is_empty(self) -> bool:
-        """
-        Is Empty
-        """
-        return not len(self.coordinates)
-    # End is_empty property
-
-    @property
-    def points(self) -> List[PointZM]:
-        """
-        Points
-        """
-        srs_id = self.srs_id
-        return [PointZM(x=x, y=y, z=z, m=m, srs_id=srs_id)
-                for x, y, z, m in self.coordinates]
-    # End points property
-
-    @property
-    def envelope(self) -> Envelope:
-        """
-        Envelope
-        """
-        if self._env is not EMPTY_ENVELOPE:
-            return self._env
-        env = envelope_from_coordinates_zm(self.coordinates)
-        self._env = env
-        return env
-    # End envelope property
-
-    def _to_wkb(self, ary: bytearray) -> bytearray:
-        """
-        To WKB
-        """
-        return pack_coordinates(
-            ary, EMPTY, self.coordinates, has_z=True, has_m=True)
-    # End _to_wkb method
-
-    @classmethod
-    def from_gpkg(cls, value: bytes) -> 'LinearRingZM':  # pragma: nocover
-        """
-        From Geopackage, no-op for Linear Ring
-        """
-        pass
-    # End from_gpkg method
+    _class: ClassVar[Any] = PointZM
+    _env_code: ClassVar[int] = EnvelopeCode.xyzm
 # End LinearRingZM class
 
 
-class Polygon(AbstractGeometry):
+class BasePolygon(AbstractGeometry):
     """
-    Polygon
+    Base Polygon
     """
     __slots__ = '_rings',
 
-    def __init__(self, coordinates: List[List[DOUBLE]], srs_id: int) -> None:
+    _class: ClassVar[Any] = object
+    _dimension: ClassVar[int] = 0
+    _env_code: ClassVar[int] = EnvelopeCode.empty
+    _wkb_prefix: ClassVar[bytes] = EMPTY
+
+    def __init__(self, coordinates: List[List], srs_id: int) -> None:
         """
-        Initialize the Polygon class
+        Initialize the BasePolygon class
         """
         super().__init__(srs_id=srs_id)
-        self._rings: List[LinearRing] = self._make_rings(coordinates)
+        self._rings: List = self._make_rings(coordinates)
     # End init built-in
 
-    def __eq__(self, other: 'Polygon') -> bool:
+    def __eq__(self, other: Any) -> bool:
         """
         Equals
         """
-        if not isinstance(other, Polygon):  # pragma: nocover
+        if not isinstance(other, self.__class__):  # pragma: nocover
             return NotImplemented
         if self.srs_id != other.srs_id:
             return False
         return self.rings == other.rings
     # End eq built-in
 
-    def _make_rings(self, coordinates: List[List[DOUBLE]]) -> List[LinearRing]:
+    def _make_rings(self, coordinates: List[List]) -> List:
         """
         Make Rings
         """
         srs_id = self.srs_id
-        return [LinearRing(coords, srs_id=srs_id) for coords in coordinates]
+        cls = self._class
+        return [cls(coords, srs_id=srs_id) for coords in coordinates]
     # End _make_rings method
 
     @property
-    def rings(self) -> List[LinearRing]:
+    def rings(self) -> List:
         """
         Rings
         """
         if self._args:
             # noinspection PyTypeChecker
             self._rings = self._make_rings(
                 unpack_lines(*self._args, is_ring=True))
@@ -360,341 +196,142 @@
     # End rings property
 
     @property
     def is_empty(self) -> bool:
         """
         Is Empty
         """
-        return not (bool(self._args) or bool(self.rings))
+        return self._is_empty or not (bool(self._args) or bool(self.rings))
     # End is_empty property
 
     @property
     def envelope(self) -> Envelope:
         """
         Envelope
         """
         if self._env is not EMPTY_ENVELOPE:
             return self._env
-        env = envelope_from_geometries(self.rings)
+        env = ENV_GEOM[self._env_code](self.rings)
         self._env = env
         return env
     # End envelope property
 
     def _to_wkb(self, ary: bytearray) -> bytearray:
         """
         To WKB
         """
         geoms = self.rings
-        ary.extend(WKB_POLYGON_PRE + pack(COUNT_CODE, len(geoms)))
+        ary.extend(self._wkb_prefix + pack(COUNT_CODE, len(geoms)))
         return self._join_geometries(ary, geoms)
     # End _to_wkb method
 
     @classmethod
-    def from_gpkg(cls, value: bytes) -> 'Polygon':
+    def from_gpkg(cls, value: bytes) -> Any:
         """
         From Geopackage
         """
-        return lazy_unpack(cls=cls, value=value, dimension=TWO_D)
+        return lazy_unpack(cls=cls, value=value, dimension=cls._dimension)
     # End from_gpkg method
-# End Polygon class
+# End BasePolygon class
 
 
-class PolygonZ(AbstractGeometry):
+class Polygon(BasePolygon):
     """
-    Polygon Z
+    Polygon
     """
     __slots__ = '_rings',
 
-    def __init__(self, coordinates: List[List[TRIPLE]], srs_id: int) -> None:
-        """
-        Initialize the PolygonZ class
-        """
-        super().__init__(srs_id=srs_id)
-        self._rings: List[LinearRingZ] = self._make_rings(coordinates)
-    # End init built-in
-
-    def __eq__(self, other: 'PolygonZ') -> bool:
-        """
-        Equals
-        """
-        if not isinstance(other, PolygonZ):  # pragma: nocover
-            return NotImplemented
-        if self.srs_id != other.srs_id:
-            return False
-        return self.rings == other.rings
-    # End eq built-in
-
-    def _make_rings(self, coordinates: List[List[TRIPLE]]) -> List[LinearRingZ]:
-        """
-        Make Rings
-        """
-        srs_id = self.srs_id
-        return [LinearRingZ(coords, srs_id=srs_id) for coords in coordinates]
-    # End _make_rings method
-
-    @property
-    def rings(self) -> List[LinearRingZ]:
-        """
-        Rings
-        """
-        if self._args:
-            # noinspection PyTypeChecker
-            self._rings = self._make_rings(
-                unpack_lines(*self._args, is_ring=True))
-            self._args = None
-        return self._rings
-    # End rings property
+    _class: ClassVar[Any] = LinearRing
+    _dimension: ClassVar[int] = TWO_D
+    _env_code: ClassVar[int] = EnvelopeCode.xy
+    _wkb_prefix: ClassVar[bytes] = WKB_POLYGON_PRE
+# End Polygon class
 
-    @property
-    def is_empty(self) -> bool:
-        """
-        Is Empty
-        """
-        return not (bool(self._args) or bool(self.rings))
-    # End is_empty property
 
-    @property
-    def envelope(self) -> Envelope:
-        """
-        Envelope
-        """
-        if self._env is not EMPTY_ENVELOPE:
-            return self._env
-        env = envelope_from_geometries_z(self.rings)
-        self._env = env
-        return env
-    # End envelope property
-
-    def _to_wkb(self, ary: bytearray) -> bytearray:
-        """
-        To WKB
-        """
-        geoms = self.rings
-        ary.extend(WKB_POLYGON_Z_PRE + pack(COUNT_CODE, len(geoms)))
-        return self._join_geometries(ary, geoms)
-    # End _to_wkb method
+class PolygonZ(BasePolygon):
+    """
+    Polygon Z
+    """
+    __slots__ = '_rings',
 
-    @classmethod
-    def from_gpkg(cls, value: bytes) -> 'PolygonZ':
-        """
-        From Geopackage
-        """
-        return lazy_unpack(cls=cls, value=value, dimension=THREE_D)
-    # End from_gpkg method
+    _class: ClassVar[Any] = LinearRingZ
+    _dimension: ClassVar[int] = THREE_D
+    _env_code: ClassVar[int] = EnvelopeCode.xyz
+    _wkb_prefix: ClassVar[bytes] = WKB_POLYGON_Z_PRE
 # End PolygonZ class
 
 
-class PolygonM(AbstractGeometry):
+class PolygonM(BasePolygon):
     """
     Polygon M
     """
     __slots__ = '_rings',
 
-    def __init__(self, coordinates: List[List[TRIPLE]], srs_id: int) -> None:
-        """
-        Initialize the PolygonM class
-        """
-        super().__init__(srs_id=srs_id)
-        self._rings: List[LinearRingM] = self._make_rings(coordinates)
-    # End init built-in
-
-    def __eq__(self, other: 'PolygonM') -> bool:
-        """
-        Equals
-        """
-        if not isinstance(other, PolygonM):  # pragma: nocover
-            return NotImplemented
-        if self.srs_id != other.srs_id:
-            return False
-        return self.rings == other.rings
-    # End eq built-in
-
-    def _make_rings(self, coordinates: List[List[TRIPLE]]) -> List[LinearRingM]:
-        """
-        Make Rings
-        """
-        srs_id = self.srs_id
-        return [LinearRingM(coords, srs_id=srs_id) for coords in coordinates]
-    # End _make_rings method
-
-    @property
-    def rings(self) -> List[LinearRingM]:
-        """
-        Rings
-        """
-        if self._args:
-            # noinspection PyTypeChecker
-            self._rings = self._make_rings(
-                unpack_lines(*self._args, is_ring=True))
-            self._args = None
-        return self._rings
-    # End rings property
-
-    @property
-    def is_empty(self) -> bool:
-        """
-        Is Empty
-        """
-        return not (bool(self._args) or bool(self.rings))
-    # End is_empty property
-
-    @property
-    def envelope(self) -> Envelope:
-        """
-        Envelope
-        """
-        if self._env is not EMPTY_ENVELOPE:
-            return self._env
-        env = envelope_from_geometries_m(self.rings)
-        self._env = env
-        return env
-    # End envelope property
-
-    def _to_wkb(self, ary: bytearray) -> bytearray:
-        """
-        To WKB
-        """
-        geoms = self.rings
-        ary.extend(WKB_POLYGON_M_PRE + pack(COUNT_CODE, len(geoms)))
-        return self._join_geometries(ary, geoms)
-    # End _to_wkb method
-
-    @classmethod
-    def from_gpkg(cls, value: bytes) -> 'PolygonM':
-        """
-        From Geopackage
-        """
-        return lazy_unpack(cls=cls, value=value, dimension=THREE_D)
-    # End from_gpkg method
+    _class: ClassVar[Any] = LinearRingM
+    _dimension: ClassVar[int] = THREE_D
+    _env_code: ClassVar[int] = EnvelopeCode.xym
+    _wkb_prefix: ClassVar[bytes] = WKB_POLYGON_M_PRE
 # End PolygonM class
 
 
-class PolygonZM(AbstractGeometry):
+class PolygonZM(BasePolygon):
     """
     Polygon ZM
     """
     __slots__ = '_rings',
 
-    def __init__(self, coordinates: List[List[QUADRUPLE]], srs_id: int) -> None:
-        """
-        Initialize the PolygonZM class
-        """
-        super().__init__(srs_id=srs_id)
-        self._rings: List[LinearRingZM] = self._make_rings(coordinates)
-    # End init built-in
-
-    def __eq__(self, other: 'PolygonZM') -> bool:
-        """
-        Equals
-        """
-        if not isinstance(other, PolygonZM):  # pragma: nocover
-            return NotImplemented
-        if self.srs_id != other.srs_id:
-            return False
-        return self.rings == other.rings
-    # End eq built-in
-
-    def _make_rings(self, coordinates: List[List[QUADRUPLE]]) \
-            -> List[LinearRingZM]:
-        """
-        Make Rings
-        """
-        srs_id = self.srs_id
-        return [LinearRingZM(coords, srs_id=srs_id) for coords in coordinates]
-    # End _make_rings method
-
-    @property
-    def rings(self) -> List[LinearRingZM]:
-        """
-        Rings
-        """
-        if self._args:
-            # noinspection PyTypeChecker
-            self._rings = self._make_rings(
-                unpack_lines(*self._args, is_ring=True))
-            self._args = None
-        return self._rings
-    # End rings property
-
-    @property
-    def is_empty(self) -> bool:
-        """
-        Is Empty
-        """
-        return not (bool(self._args) or bool(self.rings))
-    # End is_empty property
-
-    @property
-    def envelope(self) -> Envelope:
-        """
-        Envelope
-        """
-        if self._env is not EMPTY_ENVELOPE:
-            return self._env
-        env = envelope_from_geometries_zm(self.rings)
-        self._env = env
-        return env
-    # End envelope property
-
-    def _to_wkb(self, ary: bytearray) -> bytearray:
-        """
-        To WKB
-        """
-        geoms = self.rings
-        ary.extend(WKB_POLYGON_ZM_PRE + pack(COUNT_CODE, len(geoms)))
-        return self._join_geometries(ary, geoms)
-    # End _to_wkb method
-
-    @classmethod
-    def from_gpkg(cls, value: bytes) -> 'PolygonZM':
-        """
-        From Geopackage
-        """
-        return lazy_unpack(cls=cls, value=value, dimension=FOUR_D)
-    # End from_gpkg method
+    _class: ClassVar[Any] = LinearRingZM
+    _dimension: ClassVar[int] = FOUR_D
+    _env_code: ClassVar[int] = EnvelopeCode.xyzm
+    _wkb_prefix: ClassVar[bytes] = WKB_POLYGON_ZM_PRE
 # End PolygonZM class
 
 
-class MultiPolygon(AbstractGeometry):
+class BaseMultiPolygon(AbstractGeometry):
     """
-    Multi Polygon
+    Base Multi Polygon
     """
     __slots__ = '_polygons',
 
-    def __init__(self, coordinates: List[List[List[DOUBLE]]],
+    _class: ClassVar[Any] = object
+    _dimension: ClassVar[int] = 0
+    _env_code: ClassVar[int] = EnvelopeCode.empty
+    _wkb_prefix: ClassVar[bytes] = EMPTY
+
+    def __init__(self, coordinates: List[List[List]],
                  srs_id: int) -> None:
         """
-        Initialize the MultiPolygon class
+        Initialize the BaseMultiPolygon class
         """
         super().__init__(srs_id=srs_id)
-        self._polygons: List[Polygon] = self._make_polygons(coordinates)
+        self._polygons: List = self._make_polygons(coordinates)
     # End init built-in
 
-    def __eq__(self, other: 'MultiPolygon') -> bool:
+    def __eq__(self, other: Any) -> bool:
         """
         Equals
         """
-        if not isinstance(other, MultiPolygon):  # pragma: nocover
+        if not isinstance(other, self.__class__):  # pragma: nocover
             return NotImplemented
         if self.srs_id != other.srs_id:
             return False
         return self.polygons == other.polygons
     # End eq built-in
 
-    def _make_polygons(self, coordinates: List[List[List[DOUBLE]]]) \
-            -> List[Polygon]:
+    def _make_polygons(self, coordinates: List[List[List]]) -> List:
         """
         Make Polygons
         """
         srs_id = self.srs_id
-        return [Polygon(coords, srs_id=srs_id) for coords in coordinates]
+        cls = self._class
+        return [cls(coords, srs_id=srs_id) for coords in coordinates]
     # End _make_polygons method
 
     @property
-    def polygons(self) -> List[Polygon]:
+    def polygons(self) -> List:
         """
         Polygons
         """
         if self._args:
             # noinspection PyTypeChecker
             self._polygons = self._make_polygons(unpack_polygons(*self._args))
             self._args = None
@@ -702,301 +339,95 @@
     # End polygons property
 
     @property
     def is_empty(self) -> bool:
         """
         Is Empty
         """
-        return not (bool(self._args) or bool(self.polygons))
+        return self._is_empty or not (bool(self._args) or bool(self.polygons))
     # End is_empty property
 
     @property
     def envelope(self) -> Envelope:
         """
         Envelope
         """
         if self._env is not EMPTY_ENVELOPE:
             return self._env
-        env = envelope_from_geometries(self.polygons)
+        env = ENV_GEOM[self._env_code](self.polygons)
         self._env = env
         return env
     # End envelope property
 
     def _to_wkb(self, ary: bytearray) -> bytearray:
         """
         To WKB
         """
         geoms = self.polygons
-        ary.extend(WKB_MULTI_POLYGON_PRE + pack(COUNT_CODE, len(geoms)))
+        ary.extend(self._wkb_prefix + pack(COUNT_CODE, len(geoms)))
         return self._join_geometries(ary, geoms)
     # End _to_wkb method
 
     @classmethod
-    def from_gpkg(cls, value: bytes) -> 'MultiPolygon':
+    def from_gpkg(cls, value: bytes) -> Any:
         """
         From Geopackage
         """
-        return lazy_unpack(cls=cls, value=value, dimension=TWO_D)
+        return lazy_unpack(cls=cls, value=value, dimension=cls._dimension)
     # End from_gpkg method
-# End MultiPolygon class
+# End BaseMultiPolygon class
 
 
-class MultiPolygonZ(AbstractGeometry):
+class MultiPolygon(BaseMultiPolygon):
     """
-    Multi Polygon Z
+    Multi Polygon
     """
     __slots__ = '_polygons',
 
-    def __init__(self, coordinates: List[List[List[TRIPLE]]],
-                 srs_id: int) -> None:
-        """
-        Initialize the MultiPolygonZ class
-        """
-        super().__init__(srs_id=srs_id)
-        self._polygons: List[PolygonZ] = self._make_polygons(coordinates)
-    # End init built-in
-
-    def __eq__(self, other: 'MultiPolygonZ') -> bool:
-        """
-        Equals
-        """
-        if not isinstance(other, MultiPolygonZ):  # pragma: nocover
-            return NotImplemented
-        if self.srs_id != other.srs_id:
-            return False
-        return self.polygons == other.polygons
-    # End eq built-in
-
-    def _make_polygons(self, coordinates: List[List[List[TRIPLE]]]) \
-            -> List[PolygonZ]:
-        """
-        Make Polygons
-        """
-        srs_id = self.srs_id
-        return [PolygonZ(coords, srs_id=srs_id) for coords in coordinates]
-    # End _make_polygons method
-
-    @property
-    def polygons(self) -> List[PolygonZ]:
-        """
-        Polygons
-        """
-        if self._args:
-            # noinspection PyTypeChecker
-            self._polygons = self._make_polygons(unpack_polygons(*self._args))
-            self._args = None
-        return self._polygons
-    # End polygons property
-
-    @property
-    def is_empty(self) -> bool:
-        """
-        Is Empty
-        """
-        return not (bool(self._args) or bool(self.polygons))
-    # End is_empty property
+    _class: ClassVar[Any] = Polygon
+    _dimension: ClassVar[int] = TWO_D
+    _env_code: ClassVar[int] = EnvelopeCode.xy
+    _wkb_prefix: ClassVar[bytes] = WKB_MULTI_POLYGON_PRE
+# End MultiPolygon class
 
-    @property
-    def envelope(self) -> Envelope:
-        """
-        Envelope
-        """
-        if self._env is not EMPTY_ENVELOPE:
-            return self._env
-        env = envelope_from_geometries_z(self.polygons)
-        self._env = env
-        return env
-    # End envelope property
 
-    def _to_wkb(self, ary: bytearray) -> bytearray:
-        """
-        To WKB
-        """
-        geoms = self.polygons
-        ary.extend(WKB_MULTI_POLYGON_Z_PRE + pack(COUNT_CODE, len(geoms)))
-        return self._join_geometries(ary, geoms)
-    # End _to_wkb method
+class MultiPolygonZ(BaseMultiPolygon):
+    """
+    Multi Polygon Z
+    """
+    __slots__ = '_polygons',
 
-    @classmethod
-    def from_gpkg(cls, value: bytes) -> 'MultiPolygonZ':
-        """
-        From Geopackage
-        """
-        return lazy_unpack(cls=cls, value=value, dimension=THREE_D)
-    # End from_gpkg method
+    _class: ClassVar[Any] = PolygonZ
+    _dimension: ClassVar[int] = THREE_D
+    _env_code: ClassVar[int] = EnvelopeCode.xyz
+    _wkb_prefix: ClassVar[bytes] = WKB_MULTI_POLYGON_Z_PRE
 # End MultiPolygonZ class
 
 
-class MultiPolygonM(AbstractGeometry):
+class MultiPolygonM(BaseMultiPolygon):
     """
     Multi Polygon M
     """
     __slots__ = '_polygons',
 
-    def __init__(self, coordinates: List[List[List[TRIPLE]]],
-                 srs_id: int) -> None:
-        """
-        Initialize the MultiPolygonM class
-        """
-        super().__init__(srs_id=srs_id)
-        self._polygons: List[PolygonM] = self._make_polygons(coordinates)
-    # End init built-in
-
-    def __eq__(self, other: 'MultiPolygonM') -> bool:
-        """
-        Equals
-        """
-        if not isinstance(other, MultiPolygonM):  # pragma: nocover
-            return NotImplemented
-        if self.srs_id != other.srs_id:
-            return False
-        return self.polygons == other.polygons
-    # End eq built-in
-
-    def _make_polygons(self, coordinates: List[List[List[TRIPLE]]]) \
-            -> List[PolygonM]:
-        """
-        Make Polygons
-        """
-        srs_id = self.srs_id
-        return [PolygonM(coords, srs_id=srs_id) for coords in coordinates]
-    # End _make_polygons method
-
-    @property
-    def polygons(self) -> List[PolygonM]:
-        """
-        Polygons
-        """
-        if self._args:
-            # noinspection PyTypeChecker
-            self._polygons = self._make_polygons(unpack_polygons(*self._args))
-            self._args = None
-        return self._polygons
-    # End polygons property
-
-    @property
-    def is_empty(self) -> bool:
-        """
-        Is Empty
-        """
-        return not (bool(self._args) or bool(self.polygons))
-    # End is_empty property
-
-    @property
-    def envelope(self) -> Envelope:
-        """
-        Envelope
-        """
-        if self._env is not EMPTY_ENVELOPE:
-            return self._env
-        env = envelope_from_geometries_m(self.polygons)
-        self._env = env
-        return env
-    # End envelope property
-
-    def _to_wkb(self, ary: bytearray) -> bytearray:
-        """
-        To WKB
-        """
-        geoms = self.polygons
-        ary.extend(WKB_MULTI_POLYGON_M_PRE + pack(COUNT_CODE, len(geoms)))
-        return self._join_geometries(ary, geoms)
-    # End _to_wkb method
-
-    @classmethod
-    def from_gpkg(cls, value: bytes) -> 'MultiPolygonM':
-        """
-        From Geopackage
-        """
-        return lazy_unpack(cls=cls, value=value, dimension=THREE_D)
-    # End from_gpkg method
+    _class: ClassVar[Any] = PolygonM
+    _dimension: ClassVar[int] = THREE_D
+    _env_code: ClassVar[int] = EnvelopeCode.xym
+    _wkb_prefix: ClassVar[bytes] = WKB_MULTI_POLYGON_M_PRE
 # End MultiPolygonM class
 
 
-class MultiPolygonZM(AbstractGeometry):
+class MultiPolygonZM(BaseMultiPolygon):
     """
-    Multi Polygon M
+    Multi Polygon ZM
     """
     __slots__ = '_polygons',
 
-    def __init__(self, coordinates: List[List[List[QUADRUPLE]]],
-                 srs_id: int) -> None:
-        """
-        Initialize the MultiPolygonZM class
-        """
-        super().__init__(srs_id=srs_id)
-        self._polygons: List[PolygonZM] = self._make_polygons(coordinates)
-    # End init built-in
-
-    def __eq__(self, other: 'MultiPolygonZM') -> bool:
-        """
-        Equals
-        """
-        if not isinstance(other, MultiPolygonZM):  # pragma: nocover
-            return NotImplemented
-        if self.srs_id != other.srs_id:
-            return False
-        return self.polygons == other.polygons
-    # End eq built-in
-
-    def _make_polygons(self, coordinates: List[List[List[QUADRUPLE]]]) \
-            -> List[PolygonZM]:
-        """
-        Make Polygons
-        """
-        srs_id = self.srs_id
-        return [PolygonZM(coords, srs_id=srs_id) for coords in coordinates]
-    # End _make_rings method
-
-    @property
-    def polygons(self) -> List[PolygonZM]:
-        """
-        Polygons
-        """
-        if self._args:
-            # noinspection PyTypeChecker
-            self._polygons = self._make_polygons(unpack_polygons(*self._args))
-            self._args = None
-        return self._polygons
-    # End polygons property
-
-    @property
-    def is_empty(self) -> bool:
-        """
-        Is Empty
-        """
-        return not (bool(self._args) or bool(self.polygons))
-    # End is_empty property
-
-    @property
-    def envelope(self) -> Envelope:
-        """
-        Envelope
-        """
-        if self._env is not EMPTY_ENVELOPE:
-            return self._env
-        env = envelope_from_geometries_zm(self.polygons)
-        self._env = env
-        return env
-    # End envelope property
-
-    def _to_wkb(self, ary: bytearray) -> bytearray:
-        """
-        To WKB
-        """
-        geoms = self.polygons
-        ary.extend(WKB_MULTI_POLYGON_ZM_PRE + pack(COUNT_CODE, len(geoms)))
-        return self._join_geometries(ary, geoms)
-    # End _to_wkb method
-
-    @classmethod
-    def from_gpkg(cls, value: bytes) -> 'MultiPolygonZM':
-        """
-        From Geopackage
-        """
-        return lazy_unpack(cls=cls, value=value, dimension=FOUR_D)
-    # End from_gpkg method
+    _class: ClassVar[Any] = PolygonZM
+    _dimension: ClassVar[int] = FOUR_D
+    _env_code: ClassVar[int] = EnvelopeCode.xyzm
+    _wkb_prefix: ClassVar[bytes] = WKB_MULTI_POLYGON_ZM_PRE
 # End MultiPolygonZM class
 
 
 if __name__ == '__main__':  # pragma: no cover
     pass
```

## fudgeo/geometry/util.py

```diff
@@ -4,21 +4,22 @@
 """
 
 
 from functools import lru_cache
 from math import nan
 # noinspection PyPep8Naming
 from struct import error as StructError, pack, unpack
-from typing import Any, List, TYPE_CHECKING, Tuple, Union
+from typing import Any, Callable, Dict, List, TYPE_CHECKING, Tuple, Union
 
 from numpy import array, frombuffer, ndarray
 from bottleneck import nanmax, nanmin
 
 from fudgeo.constant import (
-    COUNT_CODE, EMPTY, ENVELOPE_COUNT, ENVELOPE_OFFSET, GP_MAGIC, HEADER_CODE,
+    COUNT_CODE, EMPTY, ENVELOPE_COUNT, ENVELOPE_OFFSET, EnvelopeCode, GP_MAGIC,
+    HEADER_CODE,
     HEADER_OFFSET, POINT_PREFIX)
 
 
 if TYPE_CHECKING:  # pragma: no cover
     # noinspection PyUnresolvedReferences
     from fudgeo.geometry.linestring import (
         LineString, LineStringZ, LineStringM, LineStringZM)
@@ -91,40 +92,41 @@
         if code != other.code:
             return False
         if not code:
             return True
         same_x = self.min_x == other.min_x and self.max_x == other.max_x
         same_y = self.min_y == other.min_y and self.max_y == other.max_y
         same_xy = same_x and same_y
-        if not same_xy or code == 1:
+        if not same_xy or code == EnvelopeCode.xy:
             return same_xy
         same_z = self.min_z == other.min_z and self.max_z == other.max_z
-        if code == 2:
+        if code == EnvelopeCode.xyz:
             return same_z
         same_m = self.min_m == other.min_m and self.max_m == other.max_m
-        if code == 3:
+        if code == EnvelopeCode.xym:
             return same_m
         return same_m and same_z
     # End eq built-in
 
     def to_wkb(self) -> Tuple[int, bytes]:
         """
         To WKB
         """
         code = self.code
-        if code not in {1, 2, 3, 4}:
-            return 0, EMPTY
+        if code not in {EnvelopeCode.xy, EnvelopeCode.xyz,
+                        EnvelopeCode.xym, EnvelopeCode.xyzm}:
+            return EnvelopeCode.empty, EMPTY
         values = self.min_x, self.max_x, self.min_y, self.max_y
-        if code == 1:
+        if code == EnvelopeCode.xy:
             pass
-        elif code == 2:
+        elif code == EnvelopeCode.xyz:
             values = *values, self.min_z, self.max_z
-        elif code == 3:
+        elif code == EnvelopeCode.xym:
             values = *values, self.min_m, self.max_m
-        elif code == 4:
+        elif code == EnvelopeCode.xyzm:
             values = *values, self.min_z, self.max_z, self.min_m, self.max_m
         return code, pack(f'<{ENVELOPE_COUNT[code]}d', *values)
     # End to_wkb method
 
     @property
     def code(self) -> int:
         """
@@ -203,16 +205,18 @@
 
 
 def lazy_unpack(cls: Any, value: Union[bytes, bytearray],
                 dimension: int) -> Any:
     """
     Unpack just the header and envelope, adding data to class for later use.
     """
-    srs_id, env_code, offset, is_empty = unpack_header(bytes(value[:HEADER_OFFSET]))
+    (srs_id, env_code, offset,
+     is_empty) = unpack_header(bytes(value[:HEADER_OFFSET]))
     obj = cls([], srs_id=srs_id)
+    obj._is_empty = is_empty
     if is_empty:
         return obj
     view = memoryview(value)
     obj._env = unpack_envelope(code=env_code, view=view[:offset])
     obj._args = view[offset:], dimension
     return obj
 # End lazy_unpack function
@@ -251,15 +255,15 @@
                      use_point_prefix: bool = False) -> bytearray:
     """
     Pack Coordinates
     """
     count = len(coordinates)
     ary.extend(prefix + pack(COUNT_CODE, count))
     data = coordinates.tobytes()
-    if not use_point_prefix:
+    if not use_point_prefix or not count:
         ary.extend(data)
         return ary
     length = len(data)
     view = memoryview(data)
     step = length // count
     prefix = POINT_PREFIX.get((has_z, has_m))
     for i in range(0, length, step):
@@ -358,21 +362,21 @@
     if code not in ENVELOPE_COUNT:  # pragma: no cover
         return EMPTY_ENVELOPE
     try:
         values = unpack(f'<{ENVELOPE_COUNT[code]}d', view[HEADER_OFFSET:])
     except StructError:  # pragma: no cover
         return EMPTY_ENVELOPE
     min_x = max_x = min_y = max_y = min_z = max_z = min_m = max_m = nan
-    if code == 1:
+    if code == EnvelopeCode.xy:
         min_x, max_x, min_y, max_y = values
-    elif code == 2:
+    elif code == EnvelopeCode.xyz:
         min_x, max_x, min_y, max_y, min_z, max_z = values
-    elif code == 3:
+    elif code == EnvelopeCode.xym:
         min_x, max_x, min_y, max_y, min_m, max_m = values
-    elif code == 4:
+    elif code == EnvelopeCode.xyzm:
         min_x, max_x, min_y, max_y, min_z, max_z, min_m, max_m = values
     return Envelope(
         code=code, min_x=min_x, max_x=max_x, min_y=min_y, max_y=max_y,
         min_z=min_z, max_z=max_z, min_m=min_m, max_m=max_m)
 # End unpack_envelope function
 
 
@@ -492,54 +496,73 @@
 
 def _envelope_xy(xs: ndarray, ys: ndarray) -> Envelope:
     """
     Envelope XY
     """
     min_x, max_x = nanmin(xs), nanmax(xs)
     min_y, max_y = nanmin(ys), nanmax(ys)
-    return Envelope(code=1, min_x=min_x, max_x=max_x, min_y=min_y, max_y=max_y)
+    return Envelope(code=EnvelopeCode.xy,
+                    min_x=min_x, max_x=max_x, min_y=min_y, max_y=max_y)
 # End _envelope_xy function
 
 
 def _envelope_xyz(xs: ndarray, ys: ndarray, zs: ndarray) -> Envelope:
     """
     Envelope XYZ
     """
     min_x, max_x = nanmin(xs), nanmax(xs)
     min_y, max_y = nanmin(ys), nanmax(ys)
     min_z, max_z = nanmin(zs), nanmax(zs)
-    return Envelope(code=2, min_x=min_x, max_x=max_x,
-                    min_y=min_y, max_y=max_y,
+    return Envelope(code=EnvelopeCode.xyz,
+                    min_x=min_x, max_x=max_x, min_y=min_y, max_y=max_y,
                     min_z=min_z, max_z=max_z)
 # End _envelope_xyz function
 
 
 def _envelope_xym(xs: ndarray, ys: ndarray, ms: ndarray) -> Envelope:
     """
     Envelope XYM
     """
     min_x, max_x = nanmin(xs), nanmax(xs)
     min_y, max_y = nanmin(ys), nanmax(ys)
     min_m, max_m = nanmin(ms), nanmax(ms)
-    return Envelope(code=3, min_x=min_x, max_x=max_x,
-                    min_y=min_y, max_y=max_y,
+    return Envelope(code=EnvelopeCode.xym,
+                    min_x=min_x, max_x=max_x, min_y=min_y, max_y=max_y,
                     min_m=min_m, max_m=max_m)
 # End _envelope_xym function
 
 
 def _envelope_xyzm(xs: ndarray, ys: ndarray,
                    zs: ndarray, ms: ndarray) -> Envelope:
     """
     Envelope XYZM
     """
     min_x, max_x = nanmin(xs), nanmax(xs)
     min_y, max_y = nanmin(ys), nanmax(ys)
     min_z, max_z = nanmin(zs), nanmax(zs)
     min_m, max_m = nanmin(ms), nanmax(ms)
-    return Envelope(
-        code=4, min_x=min_x, max_x=max_x, min_y=min_y, max_y=max_y,
-        min_z=min_z, max_z=max_z, min_m=min_m, max_m=max_m)
+    return Envelope(code=EnvelopeCode.xyzm,
+                    min_x=min_x, max_x=max_x, min_y=min_y, max_y=max_y,
+                    min_z=min_z, max_z=max_z, min_m=min_m, max_m=max_m)
 # End _envelope_xyzm function
 
 
+ENV_GEOM: Dict[int, Callable] = {
+    EnvelopeCode.empty: lambda _: EMPTY_ENVELOPE,
+    EnvelopeCode.xy: envelope_from_geometries,
+    EnvelopeCode.xyz: envelope_from_geometries_z,
+    EnvelopeCode.xym: envelope_from_geometries_m,
+    EnvelopeCode.xyzm: envelope_from_geometries_zm,
+}
+
+
+ENV_COORD: Dict[int, Callable] = {
+    EnvelopeCode.empty: lambda _: EMPTY_ENVELOPE,
+    EnvelopeCode.xy: envelope_from_coordinates,
+    EnvelopeCode.xyz: envelope_from_coordinates_z,
+    EnvelopeCode.xym: envelope_from_coordinates_m,
+    EnvelopeCode.xyzm: envelope_from_coordinates_zm,
+}
+
+
 if __name__ == '__main__':  # pragma: no cover
     pass
```

## Comparing `fudgeo-0.5.1.dist-info/LICENSE` & `fudgeo-0.5.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fudgeo-0.5.1.dist-info/METADATA` & `fudgeo-0.5.2.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fudgeo
-Version: 0.5.1
+Version: 0.5.2
 Summary: GeoPackage support from Python.  fudgeo is a simple package for creating OGC GeoPackages, Feature Classes, Tables, and geometries (read and write).
 Author-email: "Integrated Informatics Inc." <contact@integrated-informatics.com>
 License: MIT License
         
         Copyright (c) 2021-2023 Integrated Informatics Inc
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -68,18 +68,20 @@
 
 ## Usage
 
 `fudgeo` can be used to: 
 * Create a new empty `GeoPackage`
 * Open an existing `GeoPackage`
 * Create new `FeatureClass` or `Table` with optional overwrite
+* Create `SpatialReferenceSystem` for a `FeatureClass`
 * Insert record (attributes) into a `Table`
 * Insert feature (geometry and attributes) into a `FeatureClass`
-* Insert rows into a `Table` (in the normal `SQLite` way)
-* Drop `FeatureClass` or Table`
+* Work with data in `Table` or `FeatureClass` in a normal `SQLite` manner (e.g. `SELECT`, `INSERT`, `UPDATE`, `DELETE`)
+* Drop `FeatureClass` or `Table`
+* Retrieve fields from a `FeatureClass` or `Table`
 
 
 ### Create an Empty GeoPackage / Open GeoPackage
 
 ```python
 from fudgeo.geopkg import GeoPackage
 
@@ -256,14 +258,19 @@
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
 
 ## Release History
 
+### v0.5.2
+* store empty state on the instance during geometry read
+* introduce base classes for common capability and parametrize via class attributes
+* add stub files to provide type hinting specialization 
+
 ### v0.5.1
 * small performance improvements by reducing `bytes` concatenation and building up `bytearray`
 
 ### v0.5.0
 * performance improvements for geometry reading (especially for geometries with large numbers of points / parts)
 * performance improvements for geometry writing
 * incorporated `numpy` and `bottleneck` as dependencies
```

