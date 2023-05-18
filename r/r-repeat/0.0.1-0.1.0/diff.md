# Comparing `tmp/r_repeat-0.0.1-py3-none-any.whl.zip` & `tmp/r_repeat-0.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3001 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat       49 b- defN 23-May-18 07:51 r_repeat/__init__.py
--rw-rw-rw-  2.0 fat     3541 b- defN 23-May-18 07:32 r_repeat/main.py
--rw-rw-rw-  2.0 fat     1855 b- defN 23-May-18 07:51 r_repeat-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-18 07:51 r_repeat-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-May-18 07:51 r_repeat-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      449 b- defN 23-May-18 07:51 r_repeat-0.0.1.dist-info/RECORD
-6 files, 5995 bytes uncompressed, 2187 bytes compressed:  63.5%
+Zip file size: 3540 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat       74 b- defN 23-May-18 11:30 r_repeat/__init__.py
+-rw-rw-rw-  2.0 fat     5220 b- defN 23-May-18 12:17 r_repeat/main.py
+-rw-rw-rw-  2.0 fat     1836 b- defN 23-May-18 12:21 r_repeat-0.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-18 12:21 r_repeat-0.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-18 12:21 r_repeat-0.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      449 b- defN 23-May-18 12:21 r_repeat-0.1.0.dist-info/RECORD
+6 files, 7680 bytes uncompressed, 2726 bytes compressed:  64.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: r_repeat/__init__.py
 Comment: 
 
 Filename: r_repeat/main.py
 Comment: 
 
-Filename: r_repeat-0.0.1.dist-info/METADATA
+Filename: r_repeat-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: r_repeat-0.0.1.dist-info/WHEEL
+Filename: r_repeat-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: r_repeat-0.0.1.dist-info/top_level.txt
+Filename: r_repeat-0.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: r_repeat-0.0.1.dist-info/RECORD
+Filename: r_repeat-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## r_repeat/__init__.py

```diff
@@ -1 +1 @@
-from r_repeat.main import Repeater, ProgressBar
+from r_repeat.main import repeat, collect, seed, Repeatable, ProgressBar
```

## r_repeat/main.py

```diff
@@ -1,120 +1,168 @@
-from math import floor
+from __future__ import annotations
 from random import random
 from functools import wraps
+from typing import Callable, Optional, TypeVar, Generic
+
+T = TypeVar('T')
 
 
 class ProgressBar:
-    started = 0
-    percent = 0
-    length = 0
-    filled = 0
-    partial = 0
-    symbols = [' ', '▏', '▎', '▍', '▌', '▋', '▊', '▉', '█']
-
-    def __init__(self, length):
-        self.length = length
-
-    def draw(self):
-        print('\r[' + self.filled * self.symbols[8] + self.symbols[self.partial] + (self.length - 1 - self.filled) * ' ' + '] ' + f'{self.percent:.2f}%', end='')
-
-    def progress(self, percent):
-        self.percent = 100 * percent
-        filled = floor(self.length * percent)
-        decimal = self.length * percent - filled
-        if 0 <= decimal < 0.125:
-            partial = 0
-        elif 0.125 <= decimal < 0.25:
-            partial = 1
-        elif 0.25 <= decimal < 0.375:
-            partial = 2
-        elif 0.375 <= decimal < 0.5:
-            partial = 3
-        elif 0.5 <= decimal < 0.625:
-            partial = 4
-        elif 0.625 <= decimal < 0.75:
-            partial = 5
-        elif 0.75 <= decimal < 0.875:
-            partial = 6
-        elif 0.875 <= decimal < 1:
-            partial = 7
-        else:
-            partial = 8
-        if not self.started:
-            self.started = 1
+    detail: int
+    showPercent: bool
+    symbols: list
+    started: bool = False
+    percent: float = 0
+    filled: int = 0
+    partial: int = 0
+
+    def __init__(self, detail: int = 30, showPercent: bool = True, symbols: Optional[list] = None) -> None:
+        """Create a simple progress bar"""
+        self.detail = detail
+        self.showPercent = showPercent
+        self.symbols = symbols or [' ', '▏', '▎', '▍', '▌', '▋', '▊', '▉', '█']
+
+    def draw(self) -> None:
+        """Draw the current state of the progress bar"""
+        self.clearline()
+        print('[' +  # start of bar
+              self.filled * self.symbols[-1] +  # filled boxes
+              self.symbols[self.partial] +  # partially filled box
+              (self.detail - 1 - self.filled) * self.symbols[0] +  # empty boxes
+              ']',  # end of bar
+              end='')  # do not go to next line
+        if self.showPercent:
+            print(f' {self.percent:.1f}%', end='')
+
+    def progress(self, fraction: float) -> None:
+        """Update the state of the progress bar"""
+        self.percent = 100 * fraction
+        filled = int(self.detail * fraction)
+        decimal = self.detail * fraction - filled
+        partial = len(self.symbols) - 1
+        frac = 1/len(self.symbols)
+        for i in range(len(self.symbols)):
+            if i * frac <= decimal < (i + 1) * frac:
+                partial = i
+                break
+        if not self.started:  # first time drawing
+            self.filled = filled
+            self.partial = partial
+            self.started = True
             self.draw()
         elif filled > self.filled:
             self.filled = filled
             self.partial = 0
             self.draw()
         elif partial > self.partial:
             self.partial = partial
             self.draw()
 
-    def clear(self):
+    @staticmethod
+    def clearline() -> None:
+        """Clear the terminal line"""
         print('\r\033[K', end='')
 
 
-class Repeater:
-    pb: ProgressBar
-
-    def __init__(self, progressbar_length=30):
-        self.pb = ProgressBar(progressbar_length)
+class Repeatable(Callable, Generic[T]):
+    f: Callable[..., T]
+    n: int
+    repeat_enumerate: bool
+    i: int
+    args: tuple
+    kwargs: dict
+
+    def __init__(self, f: Callable[..., T], n: int, /, *args, repeat_enumerate: bool = False, **kwargs) -> None:
+        self.f = f
+        self.n = int(n)
+        self.repeat_enumerate = repeat_enumerate
+        self.i = 0
+        self.args = args
+        self.kwargs = kwargs
+
+    def __call__(self, /, *args, repeat_enumerate: bool = False, **kwargs) -> Repeatable[..., T]:
+        self.i = 0
+        self.args = args
+        self.kwargs = kwargs
+        return self
+
+    def __len__(self) -> int:
+        return self.n
+
+    def __iter__(self) -> Repeatable[..., T]:
+        self.i = 0
+        return self
+
+    def __next__(self) -> T:
+        if self.i < len(self):
+            self.i += 1
+            if not self.repeat_enumerate:
+                return self.f(*self.args, **self.kwargs)
+            else:
+                return self.f(*self.args, **self.kwargs, enumeration=self.i)
+        else:
+            raise StopIteration
 
-    def collect(self, f, /, *args, col=lambda a, b: a + b, **kwargs):
-        self.pb.progress(0)
-        gen = f(*args, **kwargs)
-        res = next(gen)
-        for i, v in enumerate(gen):
-            res = col(res, v)
-            self.pb.progress(i / len(gen))
-        self.pb.progress(1)
-        self.pb.clear()
-        return res
 
-    @staticmethod
-    def repeat(func=None, /, n=1):
-        def g(f):
-            class H:
-                def __init__(self, *args, **kwargs):
-                    self.i = 0
-                    self.args = args
-                    self.kwargs = kwargs
-
-                def __call__(self, *args, **kwargs):
-                    self.__init__(*args, **kwargs)
-                    return self
-
-                def __len__(self):
-                    return int(n)
-
-                def __iter__(self):
-                    self.i = 0
-                    return self
-
-                def __next__(self):
-                    if self.i < len(self):
-                        self.i += 1
-                        return f(*self.args, **self.kwargs)
-                    else:
-                        raise StopIteration
-            return H
-        if func is None:
-            return g
+def repeat(
+          func: Callable[..., T] = None,
+          /,
+          n: int = 10**3,
+          repeat_enumerate: bool = False
+          ) -> Repeatable[..., T] | Callable[[Callable[..., T]], Repeatable[..., T]]:
+    def g(f):
+        return Repeatable(f, n, repeat_enumerate=repeat_enumerate)
+    if func is None:
+        return g
+    else:
+        return g(func)
+
+
+def collect(
+           f: Repeatable[..., T],
+           /,
+           collector: Optional[Callable[[T, T], T]] = None,
+           collector_enumerate: bool = False,
+           progressbar_detail: int = 30
+           ) -> T:
+    collector = collector or ((lambda a, b: a + b) if not collector_enumerate else (lambda a, b, i: a + b))
+    pb = ProgressBar(progressbar_detail)
+    pb.progress(0)
+    res = next(f)
+    for i, v in enumerate(f):
+        if not collector_enumerate:
+            res = collector(res, v)
         else:
-            return g(func)
+            res = collector(res, v, i)
+        pb.progress(i / len(f))
+    pb.progress(1)
+    pb.clearline()
+    return res
 
-    @staticmethod
-    def seed(func=None, /, transform=lambda x: x, kwarg=None):
-        def g(f):
+
+def seed(
+        func: Callable[..., T] = None,
+        /,
+        transform: Callable = lambda x: x,
+        kwarg: str | list[str] = None
+        ) -> Callable[..., T]:
+    def g(f):
+        if kwarg is None:
             @wraps(f)
             def h(*args, **kwargs):
-                if kwarg is None:
-                    return f(*args, transform(random()), **kwargs)
-                else:
-                    kwargs[kwarg] = transform(random())
-                    return f(*args, **kwargs)
-            return h
-        if func is None:
-            return g
+                return f(*args, transform(random()), **kwargs)
+        elif isinstance(kwarg, str):
+            @wraps(f)
+            def h(*args, **kwargs):
+                kwargs[kwarg] = transform(random())
+                return f(*args, **kwargs)
         else:
-            return g(func)
+            @wraps(f)
+            def h(*args, **kwargs):
+                for i in kwarg:
+                    kwargs[i] = transform(random())
+                return f(*args, **kwargs)
+        return h
+    if func is None:
+        return g
+    else:
+        return g(func)
```

## Comparing `r_repeat-0.0.1.dist-info/METADATA` & `r_repeat-0.1.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: r-repeat
-Version: 0.0.1
+Version: 0.1.0
 Summary: Create a palette preview image by using a simple config file
 Home-page: https://github.com/Aonodensetsu/r_repeat
 Author: Remigiusz Dończyk
 Author-email: donczyk.remigiusz@gmail.com
 License: GPL-3.0
 Keywords: repeat,probability,random
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,18 +16,15 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 ## Simple library for gathering results from probabilistic functions
 
 ![size](https://img.shields.io/github/repo-size/aonodensetsu/r_repeat?label=size) ![files](https://img.shields.io/github/directory-file-count/aonodensetsu/r_repeat) ![lines](https://img.shields.io/tokei/lines/github/aonodensetsu/r_repeat)   
-![py dep](https://img.shields.io/pypi/pyversions/r-repeat) [![version](https://img.shields.io/pypi/v/r-repeat)](https://pypi.org/project/r-repeat/0.0.1/)  
+![py dep](https://img.shields.io/pypi/pyversions/r-repeat) [![version](https://img.shields.io/pypi/v/r-repeat)](https://pypi.org/project/r-repeat/0.1.0/)  
 ![license](https://img.shields.io/pypi/l/r-repeat) [![downloads](https://img.shields.io/badge/releases-here-green?logo=pypi)](https://pypi.org/project/r-repeat/#history)  
 [![downloads](https://img.shields.io/badge/wiki-here-pink)](https://github.com/Aonodensetsu/r_repeat/blob/main/WIKI.md) [![downloads](https://img.shields.io/badge/changelog-here-pink)](https://github.com/Aonodensetsu/r_repeat/blob/main/CHANGELOG.md)  
 
 # Usage:
 1. `pip install r_repeat`
 2. Open up [the wiki](https://github.com/Aonodensetsu/r_repeat/blob/main/WIKI.md) to see how everything works or check the examples
 3. Enjoy
-
-# Example:
-WIP
```

