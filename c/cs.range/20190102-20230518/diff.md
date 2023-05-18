# Comparing `tmp/cs.range-20190102.tar.gz` & `tmp/cs.range-20230518.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cs.range-20190102.tar", last modified: Wed Jan  2 06:23:03 2019, max compression
+gzip compressed data, was "cs.range-20230518.tar", last modified: Thu May 18 10:18:07 2023, max compression
```

## Comparing `cs.range-20190102.tar` & `cs.range-20230518.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 cameron    (501) cameron    (508)        0 2019-01-02 06:23:03.000000 cs.range-20190102/
-drwxrwxr-x   0 cameron    (501) cameron    (508)        0 2019-01-02 06:23:02.000000 cs.range-20190102/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (508)        0 2019-01-02 06:23:02.000000 cs.range-20190102/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (508)        0 2019-01-02 06:23:02.000000 cs.range-20190102/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (508)       21 2019-01-02 06:22:54.000000 cs.range-20190102/lib/python/cs/__init__.py
--rw-r--r--   0 cameron    (501) cameron    (508)    16040 2019-01-02 06:22:54.000000 cs.range-20190102/lib/python/cs/range.py
-drwxrwxr-x   0 cameron    (501) cameron    (508)        0 2019-01-02 06:23:03.000000 cs.range-20190102/lib/python/cs.range.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (508)        1 2019-01-02 06:23:02.000000 cs.range-20190102/lib/python/cs.range.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (508)     2036 2019-01-02 06:23:02.000000 cs.range-20190102/lib/python/cs.range.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (508)       19 2019-01-02 06:23:02.000000 cs.range-20190102/lib/python/cs.range.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (508)      283 2019-01-02 06:23:02.000000 cs.range-20190102/lib/python/cs.range.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (508)        3 2019-01-02 06:23:02.000000 cs.range-20190102/lib/python/cs.range.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (508)       19 2019-01-02 06:23:02.000000 cs.range-20190102/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (508)     2036 2019-01-02 06:23:03.000000 cs.range-20190102/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (508)       38 2019-01-02 06:23:03.000000 cs.range-20190102/setup.cfg
--rw-rw-r--   0 cameron    (501) cameron    (508)     1906 2019-01-02 06:23:02.000000 cs.range-20190102/setup.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-05-18 10:18:07.383448 cs.range-20230518/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-05-18 10:17:48.000000 cs.range-20230518/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)     2659 2023-05-18 10:18:07.383564 cs.range-20230518/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)     6133 2023-05-18 10:17:50.000000 cs.range-20230518/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-05-18 10:18:07.379233 cs.range-20230518/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-05-18 10:18:07.379571 cs.range-20230518/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-05-18 10:18:07.381422 cs.range-20230518/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    16581 2023-05-18 10:17:34.000000 cs.range-20230518/lib/python/cs/range.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-05-18 10:18:07.383181 cs.range-20230518/lib/python/cs.range.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)     2659 2023-05-18 10:18:07.000000 cs.range-20230518/lib/python/cs.range.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      292 2023-05-18 10:18:07.000000 cs.range-20230518/lib/python/cs.range.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-05-18 10:18:07.000000 cs.range-20230518/lib/python/cs.range.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)       39 2023-05-18 10:18:07.000000 cs.range-20230518/lib/python/cs.range.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-05-18 10:18:07.000000 cs.range-20230518/lib/python/cs.range.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)     2853 2023-05-18 10:17:54.000000 cs.range-20230518/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)      937 2023-05-18 10:18:07.384097 cs.range-20230518/setup.cfg
+-rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-05-18 10:17:50.000000 cs.range-20230518/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cs.range-20190102/lib/python/cs/range.py` & `cs.range-20230518/lib/python/cs/range.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,28 @@
-#!/usr/bin/python
+#!/usr/bin/env python3
 #
+
 '''
 A Range is an object resembling a set but optimised for contiguous
 ranges of int members.
 '''
 
 from __future__ import print_function
 import sys
 from bisect import bisect_left
 from collections import namedtuple
 from cs.logutils import ifdebug
 from cs.seq import first
 
+__version__ = '20230518'
+
 DISTINFO = {
     'description':
-        "a Range class implementing compact integer ranges with a set-like API,"
-        " and associated functions",
+    "a Range class implementing compact integer ranges with a set-like API,"
+    " and associated functions",
     'keywords': ["python2", "python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
     ],
     'install_requires': ['cs.logutils', 'cs.seq'],
@@ -61,47 +64,56 @@
       yield Span(*span)
     return
 
   # otherwise compute by examination
   prev = None
   for i in items:
     if prev is None:
-      prev = [i, i+1]
+      prev = [i, i + 1]
     elif i == prev[1]:
       prev[1] += 1
     else:
       yield Span(*prev)
-      prev = [i, i+1]
+      prev = [i, i + 1]
   if prev is not None:
     yield Span(*prev)
 
 class Span(namedtuple('Span', 'start end')):
   ''' A namedtuple with `.start` and `.end` attributes.
   '''
 
   def __str__(self):
     return "%d:%d" % (self.start, self.end)
+
   __repr__ = __str__
+
   def __eq__(self, other):
     return self[0] == other[0] and self[1] == other[1]
+
   def __lt__(self, other):
     return self[0] < other[0] or (self[0] == other[0] and self[1] < other[1])
+
   def __len__(self):
     return self.end - self.start
+
   @property
   def size(self):
     ''' The `.size` of a `Span` is its length: `end - start`.
     '''
     return len(self)
 
+  def as_list(self):
+    ''' This `Span` as a 2 element `list`. '''
+    return [self.start, self.end]
+
 class Range(object):
-  ''' A collection of ints that collates adjacent ints.
+  ''' A collection of `int`s that collates adjacent ints.
 
       The interface is as for a `set` with additional methods:
-      * `spans()`: return an iterable of `Spans`, with `.start`
+      * `spans()`: return an iterable of `Span`s, with `.start`
         included in each `Span` and `.end` just beyond
 
       Additionally, the update/remove/etc methods have a secondary
       calling signature: `(start,end)`, which is the same as passing
       in `Range(start,end)` but much more efficient.
   '''
 
@@ -122,15 +134,17 @@
         # "start" must be an iterable of ints
         for substart, subend in spans(start):
           self.add_span(substart, subend)
       else:
         self.add_span(start, end)
 
   def __str__(self):
-    return "[%s]" % (",".join( [ "[%d:%d)" % (S.start, S.end) for S in self._spans ] ))
+    return "[%s]" % (
+        ",".join(["[%d:%d)" % (S.start, S.end) for S in self._spans])
+    )
     ##spans = [ "%d"%(start,) if start == end-1
     ##          else "%d,%d"%(start,end-1) if start == end-2
     ##          else "%d..%d"%(start,end-1) for start, end in self._spans ]
     ##return "[%s]" % (",".join(spans))
 
   def __eq__(self, other):
     if isinstance(other, Range):
@@ -155,57 +169,77 @@
 
   @property
   def span0(self):
     ''' Return the first `Span`; raises `IndexError` if there are no spans.
     '''
     return first(self.spans())
 
+  def as_list(self):
+    ''' This `Range` as a `list` of 2-element per-`Span` `list`s.
+
+            >>> R = Range(4, 8)
+            >>> R.as_list()
+            [[4, 8]]
+            >>> R.add(11, 14)
+            >>> R.as_list()
+            [[4, 8], [11, 14]]
+            >>> R.remove(12)
+            >>> R.as_list()
+            [[4, 8], [11, 12], [13, 14]]
+
+    '''
+    return [span.as_list() for span in self._spans]
+
   def _check(self):
     self._check_spans()
 
   def _check_spans(self):
     ''' Sanity check the ._spans attribute.
         Raises TypeError or ValueError on failure.
     '''
     _spans = self._spans
     if type(_spans) is not list:
       raise TypeError("._spans should be a list")
     ospan = None
     for span in _spans:
       if not isinstance(span, Span):
-        raise TypeError("._spans elements should be lists, found "+repr(span))
-      if len(span) != 2:
-        raise ValueError("._spans elements should have length 2, found "+repr(span))
+        raise TypeError(
+            "._spans elements should be lists, found " + repr(span)
+        )
       start, end = span
       if not isinstance(start, int) or not isinstance(end, int):
-        raise TypeError("._spans elements should be a pair of ints, found "+repr(span))
+        raise TypeError(
+            "._spans elements should be a pair of ints, found " + repr(span)
+        )
       if start >= end:
-        raise ValueError("._spans elements should have low < high, found "+repr(span))
+        raise ValueError(
+            "._spans elements should have low < high, found " + repr(span)
+        )
       if ospan is not None:
         if ospan[1] >= start:
           raise ValueError(
               "._spans elements should be strictly greater than their"
-              " predecessors, found %s then %s"
-              % (ospan, span))
+              " predecessors, found %s then %s" % (ospan, span)
+          )
       ospan = span
 
   def __iter__(self):
     ''' Yield all the elements.
     '''
     for _span in self._spans:
-      for x in range( *_span ):
+      for x in range(*_span):
         yield x
 
   def __bool__(self):
     return len(self._spans) > 0
 
   __nonzero__ = __bool__
 
   def __len__(self):
-    return sum( [ end-start for start, end in self._spans ] )
+    return sum([end - start for start, end in self._spans])
 
   @property
   def start(self):
     ''' Return the start offset of the `Range`,
         the minimum `Span` .start or `0` if the `Range` is empty.
     '''
     spans = self._spans
@@ -238,20 +272,20 @@
     '''
     if isinstance(x, Range):
       return self.issuperset(x)
     if isinstance(x, Span):
       start = x.start
       end = x.end
     elif isinstance(x, int):
-      start, end = x, x+1
+      start, end = x, x + 1
     else:
       start, end = list(x)
     _spans = self._spans
     ndx = bisect_left(_spans, Span(start, start))
-    if ndx > 0 and _spans[ndx-1].end > start:
+    if ndx > 0 and _spans[ndx - 1].end > start:
       ndx -= 1
     elif ndx >= len(_spans):
       return False
     span = _spans[ndx]
     if start < span.start:
       return False
     if end > span.end:
@@ -263,15 +297,15 @@
         such that all spans with indices < `i`
         strictly preceed `start` amd all spans with indices > `j`
         strictly follow `end`.
     '''
     _spans = self._spans
     i = bisect_left(_spans, Span(start, start))
     # check preceeding span
-    assert i == 0 or _spans[i-1].end <= start
+    assert i == 0 or _spans[i - 1].end <= start
     # check current span
     assert i == len(_spans) or _spans[i].start >= start
     raise RuntimeError("INCOMPLETE")
 
   def slices(self, start=None, end=None):
     ''' Return an iterable of (inside, Span) covering the gaps and spans in this Range.
         If `start` is omitted, start at the minimum of 0 and the
@@ -346,15 +380,15 @@
     '''
     if start >= end:
       return
     _spans = self._spans
     # locate start index: all affected spans start from here
     S0 = Span(start, start)
     i = bisect_left(_spans, S0)
-    if i > 0 and _spans[i-1].end >= start:
+    if i > 0 and _spans[i - 1].end >= start:
       i -= 1
     drop_from = i
     new_start = start
     new_end = end
     while i < len(_spans) and _spans[i].start <= end:
       span = _spans[i]
       # check that the spans overlap
@@ -362,15 +396,15 @@
       new_start = min(new_start, span.start)
       new_end = max(new_end, span.end)
       i += 1
     drop_to = i
     new_span = Span(new_start, new_end)
     if self._debug:
       self._check()
-    _spans[drop_from:drop_to] = [ new_span ]
+    _spans[drop_from:drop_to] = [new_span]
     if self._debug:
       self._check()
 
   def discard_span(self, start, end, remove_mode=False):
     ''' Remove [start,end] from Range if present.
     '''
     if start >= end:
@@ -410,51 +444,52 @@
           pass
       i += 1
 
     if remove_mode and start < end:
       raise KeyError("span %s not entirely in Range" % (ospan,))
 
     drop_to = i
-    if (drop_from is not None and drop_from < drop_to) or len(insert_spans) > 0:
+    if (drop_from is not None
+        and drop_from < drop_to) or len(insert_spans) > 0:
       _spans[drop_from:drop_to] = insert_spans
     if self._debug:
       self._check()
 
   def add(self, start, end=None):
     ''' Like `set.add` but with an extended signature.
     '''
     if end is not None:
       self.add_span(start, end)
     elif isinstance(start, Range):
       for span in start.spans():
         self.add_span(*span)
     else:
-      self.add_span(start, start+1)
+      self.add_span(start, start + 1)
 
   def discard(self, start, end=None):
     ''' Like `set.discard` but with an extended signature.
     '''
     if end is not None:
       self.discard_span(start, end)
     elif isinstance(start, Range):
       for span in start.spans():
         self.discard_span(*span)
     else:
-      self.discard_span(start, start+1)
+      self.discard_span(start, start + 1)
 
   def remove(self, start, end=None):
     ''' Like `set.remove` but with an extended signature.
     '''
     if end is not None:
       self.discard_span(start, end, remove_mode=True)
     elif isinstance(start, Range):
       for span in start.spans():
         self.discard_span(*span, remove_mode=True)
     else:
-      self.discard_span(start, start+1, remove_mode=True)
+      self.discard_span(start, start + 1, remove_mode=True)
 
   def update(self, iterable):
     ''' Update the `Range` to include the values from `iterable`.
     '''
     start = None
     for i in iterable:
       if start is None:
```

### Comparing `cs.range-20190102/setup.py` & `cs.range-20230518/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,92 @@
-#!/usr/bin/env python
-from setuptools import setup
-setup(
-  name = 'cs.range',
-  description = 'a Range class implementing compact integer ranges with a set-like API, and associated functions',
-  author = 'Cameron Simpson',
-  author_email = 'cs@cskk.id.au',
-  version = '20190102',
-  url = 'https://bitbucket.org/cameron_simpson/css/commits/all',
-  classifiers = ['Programming Language :: Python', 'Programming Language :: Python :: 2', 'Programming Language :: Python :: 3', 'Development Status :: 4 - Beta', 'Intended Audience :: Developers', 'Operating System :: OS Independent', 'Topic :: Software Development :: Libraries :: Python Modules', 'License :: OSI Approved :: GNU General Public License v3 (GPLv3)'],
-  install_requires = ['cs.logutils', 'cs.seq'],
-  keywords = ['python2', 'python3'],
-  long_description = 'A Range is an object resembling a set but optimised for contiguous\nranges of int members.\n\n## Function `overlap(span1, span2)`\n\nReturn a list `[start,end]` denoting the overlap of two spans.\n\nExample:\n\n    >>> overlap([1,9], [5,13])\n    [5, 9]\n\n## Class `Range`\n\nA collection of ints that collates adjacent ints.\n\nThe interface is as for a `set` with additional methods:\n* `spans()`: return an iterable of `Spans`, with `.start`\n  included in each `Span` and `.end` just beyond\n\nAdditionally, the update/remove/etc methods have a secondary\ncalling signature: `(start,end)`, which is the same as passing\nin `Range(start,end)` but much more efficient.\n\n## Class `Span`\n\nMRO: `Span`, `builtins.tuple`  \nA namedtuple with `.start` and `.end` attributes.\n\n## Function `spans(items)`\n\nReturn an iterable of `Spans` for all contiguous sequences in\n`items`.\n\nExample:\n\n    >>> list(spans([1,2,3,7,8,11,5]))\n    [1:4, 7:9, 11:12, 5:6]',
-  long_description_content_type = 'text/markdown',
-  package_dir = {'': 'lib/python'},
-  py_modules = ['cs.range'],
-)
+Metadata-Version: 2.1
+Name: cs.range
+Version: 20230518
+Summary: a Range class implementing compact integer ranges with a set-like API, and associated functions
+Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
+Author: Cameron Simpson
+Author-email: Cameron Simpson <cs@cskk.id.au>
+License: GNU General Public License v3 or later (GPLv3+)
+Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
+Keywords: python2,python3
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Description-Content-Type: text/markdown
+
+A Range is an object resembling a set but optimised for contiguous
+ranges of int members.
+
+*Latest release 20230518*:
+Span,Range: new as_list() methods.
+
+## Function `overlap(span1, span2)`
+
+Return a list `[start,end]` denoting the overlap of two spans.
+
+Example:
+
+    >>> overlap([1,9], [5,13])
+    [5, 9]
+
+## Class `Range`
+
+A collection of `int`s that collates adjacent ints.
+
+The interface is as for a `set` with additional methods:
+* `spans()`: return an iterable of `Span`s, with `.start`
+  included in each `Span` and `.end` just beyond
+
+Additionally, the update/remove/etc methods have a secondary
+calling signature: `(start,end)`, which is the same as passing
+in `Range(start,end)` but much more efficient.
+
+*Method `Range.__init__(self, start=None, end=None, debug=None)`*:
+Initialise the Range.
+
+Called with `start` and `end`, these specify the initial
+`Span` of the `Range`.
+If called with just one argument that argument instead be an iterable
+of integer values comprising the values in the `Range`.
+
+## Class `Span(Span, builtins.tuple)`
+
+A namedtuple with `.start` and `.end` attributes.
+
+## Function `spans(items)`
+
+Return an iterable of `Spans` for all contiguous sequences in
+`items`.
+
+Example:
+
+    >>> list(spans([1,2,3,7,8,11,5]))
+    [1:4, 7:9, 11:12, 5:6]
+
+# Release Log
+
+
+
+*Release 20230518*:
+Span,Range: new as_list() methods.
+
+*Release 20190102*:
+Span: provide __len__.
+
+*Release 20171231*:
+* Add Range.span0, returning the first Span.
+* Implement __bool__ and__nonzero__.
+* Accept a Span in __contains__.
+* Some small bugfixes.
+
+*Release 20160828*:
+* Add Range.start like existing Range.end.
+* Use "install_requires" instead of "requires" in DISTINFO.
+* Small bugfix.
+
+*Release 20150116*:
+First PyPI release.
```

