# Comparing `tmp/shlib-1.5.tar.gz` & `tmp/shlib-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shlib-1.5.tar", last modified: Fri Nov 18 04:58:50 2022, max compression
+gzip compressed data, was "shlib-1.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `shlib-1.5.tar` & `shlib-1.6.tar`

### file list

```diff
@@ -1,17 +1,6 @@
-drwx------   0 ken       (1000) ken       (1001)        0 2022-11-18 04:58:50.250331 shlib-1.5/
--rw-rw-r--   0 ken       (1000) ken       (1001)    35142 2019-11-13 05:28:21.000000 shlib-1.5/LICENSE
--rw-------   0 ken       (1000) ken       (1001)    22734 2022-11-18 04:58:50.250331 shlib-1.5/PKG-INFO
--rw-rw-r--   0 ken       (1000) ken       (1001)    22040 2022-11-04 18:40:53.000000 shlib-1.5/README.rst
--rw-------   0 ken       (1000) ken       (1001)       38 2022-11-18 04:58:50.250331 shlib-1.5/setup.cfg
--rw-rw-r--   0 ken       (1000) ken       (1001)     1164 2022-11-04 18:40:53.000000 shlib-1.5/setup.py
-drwx------   0 ken       (1000) ken       (1001)        0 2022-11-18 04:58:50.248331 shlib-1.5/shlib/
--rw-rw-r--   0 ken       (1000) ken       (1001)      605 2022-11-04 18:40:53.000000 shlib-1.5/shlib/__init__.py
--rw-rw-r--   0 ken       (1000) ken       (1001)     4886 2022-01-01 18:08:06.000000 shlib-1.5/shlib/extended_pathlib.py
--rw-rw-r--   0 ken       (1000) ken       (1001)    31790 2022-11-04 18:40:53.000000 shlib-1.5/shlib/shlib.py
-drwx------   0 ken       (1000) ken       (1001)        0 2022-11-18 04:58:50.250331 shlib-1.5/shlib.egg-info/
--rw-------   0 ken       (1000) ken       (1001)    22734 2022-11-18 04:58:50.000000 shlib-1.5/shlib.egg-info/PKG-INFO
--rw-------   0 ken       (1000) ken       (1001)      254 2022-11-18 04:58:50.000000 shlib-1.5/shlib.egg-info/SOURCES.txt
--rw-------   0 ken       (1000) ken       (1001)        1 2022-11-18 04:58:50.000000 shlib-1.5/shlib.egg-info/dependency_links.txt
--rw-------   0 ken       (1000) ken       (1001)       19 2022-11-18 04:58:50.000000 shlib-1.5/shlib.egg-info/requires.txt
--rw-------   0 ken       (1000) ken       (1001)        6 2022-11-18 04:58:50.000000 shlib-1.5/shlib.egg-info/top_level.txt
--rw-------   0 ken       (1000) ken       (1001)        1 2022-11-18 04:58:49.000000 shlib-1.5/shlib.egg-info/zip-safe
+-rw-r--r--   0        0        0    22040 2023-05-18 18:11:31.569690 shlib-1.6/README.rst
+-rw-r--r--   0        0        0      936 2023-05-18 18:11:31.563690 shlib-1.6/pyproject.toml
+-rw-r--r--   0        0        0      605 2023-05-18 18:11:31.566690 shlib-1.6/shlib/__init__.py
+-rw-r--r--   0        0        0     4886 2023-01-02 02:02:56.745798 shlib-1.6/shlib/extended_pathlib.py
+-rw-r--r--   0        0        0    31790 2023-05-18 18:11:31.565689 shlib-1.6/shlib/shlib.py
+-rw-r--r--   0        0        0    22857 1970-01-01 00:00:00.000000 shlib-1.6/PKG-INFO
```

### Comparing `shlib-1.5/PKG-INFO` & `shlib-1.6/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: shlib
-Version: 1.5
-Summary: shell library
-Home-page: https://nurdletech.com/linux-utilities/shlib
-Download-URL: https://github.com/kenkundert/shlib/tarball/master
-Author: Ken Kundert
-Author-email: shlib@nurdletech.com
-License: GPLv3+
-Keywords: shlib,shell,utilities
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Natural Language :: English
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Utilities
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 ShLib — Shell Library
 =====================
 
 .. image:: https://pepy.tech/badge/shlib/month
     :target: https://pepy.tech/project/shlib
 
 ..  image:: https://github.com/KenKundert/shlib/actions/workflows/build.yaml/badge.svg
@@ -34,16 +14,16 @@
 .. image:: https://img.shields.io/pypi/v/shlib.svg
     :target: https://pypi.python.org/pypi/shlib
 
 .. image:: https://img.shields.io/pypi/pyversions/shlib.svg
     :target: https://pypi.python.org/pypi/shlib/
 
 :Author: Ken Kundert
-:Version: 1.5
-:Released: 2022-11-04
+:Version: 1.6
+:Released: 2023-05-18
 
 A light-weight package with few dependencies that allows users to do 
 shell-script like things relatively easily in Python. Is a natural complement to 
 the pathlib library. Pathlib does pretty much what you would like to do with 
 a single path; shlib does similar things with many paths at once. For example, 
 with pathlib you can remove (unlink) a single file, but with shlib you can 
 remove many files at once. Furthermore, most of the features of pathlib are
```

### Comparing `shlib-1.5/README.rst` & `shlib-1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: shlib
+Version: 1.6
+Summary: shell library
+Keywords: shlib,shell,shell utilities
+Author: Ken Kundert
+Author-email: shlib@nurdletech.com
+Requires-Python: >=3.6
+Description-Content-Type: text/x-rst
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Utilities
+Requires-Dist: braceexpand
+Requires-Dist: inform>=1.28
+Project-URL: documentation, https://github.com/kenkundert/shlib
+Project-URL: homepage, https://github.com/kenkundert/shlib
+Project-URL: repository, https://github.com/kenkundert/shlib
+
 ShLib — Shell Library
 =====================
 
 .. image:: https://pepy.tech/badge/shlib/month
     :target: https://pepy.tech/project/shlib
 
 ..  image:: https://github.com/KenKundert/shlib/actions/workflows/build.yaml/badge.svg
@@ -14,16 +36,16 @@
 .. image:: https://img.shields.io/pypi/v/shlib.svg
     :target: https://pypi.python.org/pypi/shlib
 
 .. image:: https://img.shields.io/pypi/pyversions/shlib.svg
     :target: https://pypi.python.org/pypi/shlib/
 
 :Author: Ken Kundert
-:Version: 1.5
-:Released: 2022-11-04
+:Version: 1.6
+:Released: 2023-05-18
 
 A light-weight package with few dependencies that allows users to do 
 shell-script like things relatively easily in Python. Is a natural complement to 
 the pathlib library. Pathlib does pretty much what you would like to do with 
 a single path; shlib does similar things with many paths at once. For example, 
 with pathlib you can remove (unlink) a single file, but with shlib you can 
 remove many files at once. Furthermore, most of the features of pathlib are 
@@ -709,7 +731,8 @@
 
     >> from inform import fatal, os_error
     >>
     >> try:
     ..    cp(from, to)
     .. except OSError as e:
     ..    fatal(os_error(e))
+
```

### Comparing `shlib-1.5/shlib/__init__.py` & `shlib-1.6/shlib/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-__version__ = '1.5'
-__released__ = '2022-11-04'
+__version__ = '1.6'
+__released__ = '2023-05-18'
 
 from .extended_pathlib import Path
 from .shlib import (
     # path utilities
     is_str, is_iterable, is_collection, to_path, to_paths,
 
     # preferences
```

### Comparing `shlib-1.5/shlib/extended_pathlib.py` & `shlib-1.6/shlib/extended_pathlib.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pathlib -- extends system pathlib
 
 # License {{{1
-# Copyright (C) 2016-2022 Kenneth S. Kundert
+# Copyright (C) 2016-2023 Kenneth S. Kundert
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `shlib-1.5/shlib/shlib.py` & `shlib-1.6/shlib/shlib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # shlib -- Scripting utilities
 #
 # A light-weight package with few dependencies that allows users to do
 # shell-script-like things relatively easily in Python.
 
 # License {{{1
-# Copyright (C) 2016-2022 Kenneth S. Kundert
+# Copyright (C) 2016-2023 Kenneth S. Kundert
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 
-__version__ = "1.5"
-__released__ = "2022-11-04"
+__version__ = "1.6"
+__released__ = "2023-05-18"
 
 # Imports {{{1
 try:
     from .extended_pathlib import Path
 except ImportError:
     from pathlib import Path
 import errno
@@ -107,20 +107,20 @@
         from shlex import quote
     except ImportError:
         try:
             from pipes import quote
             import re
         except ImportError:
 
-            def quote(arg):
-                if not arg:
+            def quote(s):  # type: (str) -> str
+                if not s:
                     return "''"
-                if re.search(r"[^\w@%+=:,./-]", arg, re.ASCII) is None:
-                    return arg
-                return "'" + arg.replace("'", "'\"'\"'") + "'"
+                if re.search(r"[^\w@%+=:,./-]", s, re.ASCII) is None:
+                    return s
+                return "'" + s.replace("'", "'\"'\"'") + "'"
 
     return quote(str(arg))
 
 
 # _use_log {{{2
 def _use_log(log):
     if log is None:
@@ -253,25 +253,25 @@
         path.mkdir(parents=True, exist_ok=True)
 
 
 # mount/umount {{{2
 class mount:
     def __init__(self, path):
         self.path = to_path(path)
-        self.mounted_externally = is_mounted(self.path)
+        self.previously_mounted = is_mounted(self.path)
         modes = 'sOEW0' if PREFERENCES["use_inform"] else 'soeW0'
 
-        if not self.mounted_externally:
+        if not self.previously_mounted:
             Run(["mount", self.path], modes=modes)
 
     def __enter__(self):
         pass
 
     def __exit__(self, exc_type, exc_value, exc_traceback):
-        if not self.mounted_externally:
+        if not self.previously_mounted:
             umount(self.path)
 
 
 def umount(path):
     modes = 'sOEW0' if PREFERENCES["use_inform"] else 'soeW0'
     Run(["umount", path], modes=modes)
 
@@ -450,22 +450,22 @@
     for f in ls(*args, **kwargs):
         yield f
 
 
 # Path list functions (leaves, cartesian_product, brace_expand, etc.) {{{1
 def _leaves(path, hidden, report):
     try:
-        for each in path.iterdir():
-            if each.is_dir():
+        if path.is_file():
+            if hidden or not path.name.startswith("."):
+                yield path
+        elif path.is_dir():
+            for each in path.iterdir():
                 if hidden or not each.name.startswith("."):
                     for p in _leaves(each, hidden, report):
                         yield p
-            elif each.is_file():
-                if hidden or not each.name.startswith("."):
-                    yield each
     except OSError as e:
         if report:
             report(e)
 
 
 # leaves()  {{{2
 def leaves(path, hidden=False, report=None):
```

