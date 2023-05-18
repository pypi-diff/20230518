# Comparing `tmp/srtlst-0.1.3.tar.gz` & `tmp/srtlst-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srtlst-0.1.3.tar", max compression
+gzip compressed data, was "srtlst-0.2.0.tar", max compression
```

## Comparing `srtlst-0.1.3.tar` & `srtlst-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0     1071 2023-05-07 18:30:37.563519 srtlst-0.1.3/LICENSE
--rw-r--r--   0        0        0     1073 2023-05-16 13:35:55.200320 srtlst-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2628 2023-05-07 18:30:37.564820 srtlst-0.1.3/readme.md
--rw-r--r--   0        0        0      141 2023-05-16 13:33:41.633609 srtlst-0.1.3/src/srtlst/__init__.py
--rw-r--r--   0        0        0      118 2023-05-07 18:30:37.565554 srtlst-0.1.3/src/srtlst/protocols.py
--rw-r--r--   0        0        0        0 2023-05-07 18:30:37.565639 srtlst-0.1.3/src/srtlst/py.typed
--rw-r--r--   0        0        0     7665 2023-05-16 13:34:08.254186 srtlst-0.1.3/src/srtlst/sorted_list.py
--rw-r--r--   0        0        0     1338 2023-05-16 13:34:08.254697 srtlst-0.1.3/src/srtlst/sorted_list_by_key.py
--rw-r--r--   0        0        0     3549 1970-01-01 00:00:00.000000 srtlst-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-07 18:30:37.563519 srtlst-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1125 2023-05-18 19:35:37.002432 srtlst-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2820 2023-05-18 19:32:19.413705 srtlst-0.2.0/readme.md
+-rw-r--r--   0        0        0      141 2023-05-18 19:32:19.396685 srtlst-0.2.0/src/srtlst/__init__.py
+-rw-r--r--   0        0        0     2650 2023-05-18 19:32:19.414002 srtlst-0.2.0/src/srtlst/bisect.py
+-rw-r--r--   0        0        0      519 2023-05-18 19:32:19.414313 srtlst-0.2.0/src/srtlst/collections_abc.py
+-rw-r--r--   0        0        0      118 2023-05-07 18:30:37.565554 srtlst-0.2.0/src/srtlst/protocols.py
+-rw-r--r--   0        0        0        0 2023-05-07 18:30:37.565639 srtlst-0.2.0/src/srtlst/py.typed
+-rw-r--r--   0        0        0     8516 2023-05-18 19:32:19.414817 srtlst-0.2.0/src/srtlst/sorted_list.py
+-rw-r--r--   0        0        0     1699 2023-05-18 19:32:19.415439 srtlst-0.2.0/src/srtlst/sorted_list_by_key.py
+-rw-r--r--   0        0        0     3840 1970-01-01 00:00:00.000000 srtlst-0.2.0/PKG-INFO
```

### Comparing `srtlst-0.1.3/LICENSE` & `srtlst-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `srtlst-0.1.3/pyproject.toml` & `srtlst-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "srtlst"
-version = "0.1.3"
+version = "0.2.0"
 description = "a simple, generically type-annotated, sorted list"
 authors = ["exoriente"]
 license = "MIT"
 readme = "readme.md"
 repository = "https://github.com/exoriente/srtlst"
 keywords = ["sorted", "list", "simple", "container", "sorting", "bisect", "typed", "mypy"]
 classifiers = [
@@ -15,15 +15,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Software Development :: Libraries",
     "Typing :: Typed"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.8"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.262"
 black = "^23.3.0"
 mypy = "^1.2.0"
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
@@ -34,8 +34,12 @@
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [mypy]
 strict = true
 
 [tool.coverage.report]
-exclude_lines = ["class .*\\bProtocol\\):"]
+exclude_lines = [
+    "class .*\\bProtocol\\):",
+    "^\\s*\\.\\.\\.\\s*$",
+    "^\\s*from\\s"
+]
```

### Comparing `srtlst-0.1.3/readme.md` & `srtlst-0.2.0/readme.md`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,23 @@
 >>> s = SortedList([5, 3, 1])
 >>> s.add(3)
 >>> s.add(2)
 >>> print(s)
 [1, 2, 3, 3, 5]
 ```
 
+If you need your data to be sorted in descending order use the optional `reverse` parameter:
+
+```python
+>>> s = SortedList([1, 2, 3], reverse=True)
+>>> s.add(4)
+>>> print(s)
+[4, 3, 2, 1]
+```
+
 If your data is not inherently sortable, or you want to sort it in a non-default way, you can use `SortedListByKey`
 and supply a function to sort it (just like with `sorted()`):
 
 ```python
 >>> from srtlst import SortedListByKey
 >>> my_function = lambda x: x * (-1) ** x
 >>> s = SortedListByKey([1, 2, 3, 4], key=my_function)
```

### Comparing `srtlst-0.1.3/src/srtlst/sorted_list.py` & `srtlst-0.2.0/src/srtlst/sorted_list.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,67 +1,76 @@
 from __future__ import annotations
-from bisect import insort_right, insort_left, bisect_right, bisect_left
-from collections.abc import Iterable
-from typing import TypeVar, Generic, Any, Iterator, SupportsIndex
 
+from srtlst.collections_abc import Iterable, Sequence
+
+from typing import TypeVar, Any, Iterator, SupportsIndex, overload, cast
+
+from srtlst.bisect import bisect_right, bisect_left
 from srtlst.protocols import _SupportsLT
 
 _S = TypeVar("_S", bound=_SupportsLT)
 _T = TypeVar("_T")
 
 
-class SortedList(Generic[_S]):
+class SortedList(Sequence[_S]):
     """
     a list that stays sorted under all operations
     """
 
-    def __init__(self, seq: Iterable[_S] = (), /):
+    def __init__(self, seq: Iterable[_S] = (), /, *, reverse: bool = False):
         """
         create a new sorted list from an optional iterable of values
         """
         self._key = lambda x: x
-        self._list = list(sorted(seq, key=self._key))
+        self._reverse = reverse
+        self._list = list(sorted(seq, key=self._key, reverse=self._reverse))
 
     def add_right(self, value: _S) -> None:
         """
         add a value to the list and sort it into the right place
         (to the right of existing duplicate values,
         or of items with the same sort key value)
         """
-        insort_right(self._list, value, key=self._key)
+        position = bisect_right(
+            self._list, self._key(value), key=self._key, reverse=self._reverse
+        )
+        self._list.insert(position, value)
 
     def add_left(self, value: _S) -> None:
         """
         add a value to the list and sort it into the right place
         (to the left of existing duplicate values,
         or of items with the same sort key value)
         """
-        insort_left(self._list, value, key=self._key)
+        position = bisect_left(
+            self._list, self._key(value), key=self._key, reverse=self._reverse
+        )
+        self._list.insert(position, value)
 
     add = add_right
 
     def remove_right(self, value: _S) -> None:
         """
         remove a value from the list (if multiple exists, remove the right-most value)
         """
-        position = bisect_right(self._list, value, key=self._key)
+        position = bisect_right(self._list, value, key=self._key, reverse=self._reverse)
         value_key = self._key(value)
         for i in reversed(range(position)):
             if self._key(self._list[i]) != value_key:
                 break
             if self._list[i] == value:
                 del self._list[i]
                 return
         raise ValueError(f"{value} not in list")
 
     def remove_left(self, value: _S) -> None:
         """
         remove a value from the list (if multiple exists, remove the left-most value)
         """
-        position = bisect_left(self._list, value, key=self._key)
+        position = bisect_left(self._list, value, key=self._key, reverse=self._reverse)
         value_key = self._key(value)
         for i in range(position, len(self._list)):
             if self._key(self._list[i]) != value_key:
                 break
             if self._list[i] == value:
                 del self._list[i]
                 return
@@ -173,14 +182,22 @@
 
     def __len__(self) -> int:
         """
         return the number of values in the list
         """
         return len(self._list)
 
+    @overload
+    def __getitem__(self, index: int, /) -> _S:
+        ...
+
+    @overload
+    def __getitem__(self, index: slice, /) -> SortedList[_S]:
+        ...
+
     def __getitem__(self, index: SupportsIndex | slice) -> SortedList[_S] | _S:
         """
         return the value at position index,
         or, if index is a slice, return a SortedList
         """
         found = self._list[index]
         if isinstance(found, Iterable):
@@ -202,20 +219,28 @@
 
     def __mul__(self, other: SupportsIndex) -> list[_S]:
         """
         return self * other as a list
         """
         return self._list * other
 
-    def __contains__(self, item: _S) -> bool:
+    def __contains__(self, item: object) -> bool:
         """
         return true if item in self, false otherwise
+
+        (will fall back on list.__contains__ if item is not comparable to
+        contents of SortedList)
         """
-        position = bisect_left(self._list, item, key=self._key)
-        return position != len(self._list)
+        try:
+            position = bisect_left(
+                self._list, cast(_S, item), key=self._key, reverse=self._reverse
+            )
+            return position != len(self._list)
+        except TypeError:
+            return item in self._list
 
     def __iadd__(self, other: Iterable[_S]) -> SortedList[_S]:  # type:ignore[misc]
         """
         implement self += other
         """
         self._list += other
         self._list.sort(key=self._key)
@@ -239,26 +264,28 @@
         return the position of the first occurrence of x in the list,
         if start and end are given only self[start:end] will be searched,
         or self[start:] or self[:end] if only one is given
         """
         lo = 0 if start is None else start
         hi = len(self._list) if end is None else end
 
-        position = bisect_left(self._list, x, lo, hi, key=self._key)
+        position = bisect_left(
+            self._list, x, key=self._key, reverse=self._reverse, lo=lo, hi=hi
+        )
 
         if position < hi and self._list[position] == x:
             return position
         else:
             raise ValueError(f"{x} is not in sorted list")
 
     def count(self, x: _S) -> int:
         """
         return the number of occurrences of x in the list
         """
-        position = bisect_left(self._list, x, key=self._key)
+        position = bisect_left(self._list, x, key=self._key, reverse=self._reverse)
         count = 0
         for item in self._list[position:]:
             if item == x:
                 count += 1
             else:
                 break
         return count
```

### Comparing `srtlst-0.1.3/PKG-INFO` & `srtlst-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: srtlst
-Version: 0.1.3
+Version: 0.2.0
 Summary: a simple, generically type-annotated, sorted list
 Home-page: https://github.com/exoriente/srtlst
 License: MIT
 Keywords: sorted,list,simple,container,sorting,bisect,typed,mypy
 Author: exoriente
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
@@ -54,14 +56,23 @@
 >>> s = SortedList([5, 3, 1])
 >>> s.add(3)
 >>> s.add(2)
 >>> print(s)
 [1, 2, 3, 3, 5]
 ```
 
+If you need your data to be sorted in descending order use the optional `reverse` parameter:
+
+```python
+>>> s = SortedList([1, 2, 3], reverse=True)
+>>> s.add(4)
+>>> print(s)
+[4, 3, 2, 1]
+```
+
 If your data is not inherently sortable, or you want to sort it in a non-default way, you can use `SortedListByKey`
 and supply a function to sort it (just like with `sorted()`):
 
 ```python
 >>> from srtlst import SortedListByKey
 >>> my_function = lambda x: x * (-1) ** x
 >>> s = SortedListByKey([1, 2, 3, 4], key=my_function)
```

