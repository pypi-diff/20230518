# Comparing `tmp/qosd-20230516.tar.gz` & `tmp/qosd-20230518.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qosd-20230516.tar", last modified: Thu May 18 14:59:42 2023, max compression
+gzip compressed data, was "qosd-20230518.tar", last modified: Thu May 18 15:05:16 2023, max compression
```

## Comparing `qosd-20230516.tar` & `qosd-20230518.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-05-18 14:59:42.597178 qosd-20230516/
--rw-rw-r--   0 l         (1000) l         (1000)     1986 2023-05-18 14:59:42.597178 qosd-20230516/PKG-INFO
--rw-rw-r--   0 l         (1000) l         (1000)     1673 2023-05-18 14:45:10.000000 qosd-20230516/README.md
--rw-rw-r--   0 l         (1000) l         (1000)      613 2023-05-18 08:50:17.000000 qosd-20230516/pyproject.toml
--rw-rw-r--   0 l         (1000) l         (1000)       38 2023-05-18 14:59:42.597178 qosd-20230516/setup.cfg
-drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-05-18 14:59:42.597178 qosd-20230516/src/
--rw-rw-r--   0 l         (1000) l         (1000)        0 2023-05-18 08:26:03.000000 qosd-20230516/src/__init__.py
-drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-05-18 14:59:42.597178 qosd-20230516/src/qosd.egg-info/
--rw-rw-r--   0 l         (1000) l         (1000)     1986 2023-05-18 14:59:42.000000 qosd-20230516/src/qosd.egg-info/PKG-INFO
--rw-rw-r--   0 l         (1000) l         (1000)      246 2023-05-18 14:59:42.000000 qosd-20230516/src/qosd.egg-info/SOURCES.txt
--rw-rw-r--   0 l         (1000) l         (1000)        1 2023-05-18 14:59:42.000000 qosd-20230516/src/qosd.egg-info/dependency_links.txt
--rw-rw-r--   0 l         (1000) l         (1000)       35 2023-05-18 14:59:42.000000 qosd-20230516/src/qosd.egg-info/entry_points.txt
--rw-rw-r--   0 l         (1000) l         (1000)       54 2023-05-18 14:59:42.000000 qosd-20230516/src/qosd.egg-info/requires.txt
--rw-rw-r--   0 l         (1000) l         (1000)       14 2023-05-18 14:59:42.000000 qosd-20230516/src/qosd.egg-info/top_level.txt
--rwxrwxr-x   0 l         (1000) l         (1000)     7832 2023-05-18 08:39:41.000000 qosd-20230516/src/qosd.py
+drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-05-18 15:05:16.455188 qosd-20230518/
+-rw-rw-r--   0 l         (1000) l         (1000)     1978 2023-05-18 15:05:16.455188 qosd-20230518/PKG-INFO
+-rw-rw-r--   0 l         (1000) l         (1000)     1673 2023-05-18 14:45:10.000000 qosd-20230518/README.md
+-rw-rw-r--   0 l         (1000) l         (1000)      605 2023-05-18 15:02:10.000000 qosd-20230518/pyproject.toml
+-rw-rw-r--   0 l         (1000) l         (1000)       38 2023-05-18 15:05:16.455188 qosd-20230518/setup.cfg
+drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-05-18 15:05:16.455188 qosd-20230518/src/
+-rw-rw-r--   0 l         (1000) l         (1000)        0 2023-05-18 08:26:03.000000 qosd-20230518/src/__init__.py
+drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-05-18 15:05:16.455188 qosd-20230518/src/qosd.egg-info/
+-rw-rw-r--   0 l         (1000) l         (1000)     1978 2023-05-18 15:05:16.000000 qosd-20230518/src/qosd.egg-info/PKG-INFO
+-rw-rw-r--   0 l         (1000) l         (1000)      246 2023-05-18 15:05:16.000000 qosd-20230518/src/qosd.egg-info/SOURCES.txt
+-rw-rw-r--   0 l         (1000) l         (1000)        1 2023-05-18 15:05:16.000000 qosd-20230518/src/qosd.egg-info/dependency_links.txt
+-rw-rw-r--   0 l         (1000) l         (1000)       35 2023-05-18 15:05:16.000000 qosd-20230518/src/qosd.egg-info/entry_points.txt
+-rw-rw-r--   0 l         (1000) l         (1000)       54 2023-05-18 15:05:16.000000 qosd-20230518/src/qosd.egg-info/requires.txt
+-rw-rw-r--   0 l         (1000) l         (1000)       14 2023-05-18 15:05:16.000000 qosd-20230518/src/qosd.egg-info/top_level.txt
+-rwxrwxr-x   0 l         (1000) l         (1000)     7832 2023-05-18 15:02:21.000000 qosd-20230518/src/qosd.py
```

### Comparing `qosd-20230516/PKG-INFO` & `qosd-20230518/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: qosd
-Version: 20230516
+Version: 20230518
 Summary: QOSD for python
-Author-email: Laurent Ghigonis <laurent.ghigonis@p1sec.com>
+Author-email: Laurent Ghigonis <ooookiwi@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/looran/qosd
 Keywords: osd,on-screen-display,tail
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 
 ## qosd - display text over your Xorg screen
```

### Comparing `qosd-20230516/README.md` & `qosd-20230518/README.md`

 * *Files identical despite different names*

### Comparing `qosd-20230516/pyproject.toml` & `qosd-20230518/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qosd"
-authors = [ {name = "Laurent Ghigonis", email = "laurent.ghigonis@p1sec.com"}, ]
+authors = [ {name = "Laurent Ghigonis", email = "ooookiwi@gmail.com"}, ]
 description = "QOSD for python"
 readme = "README.md"
 requires-python = ">=3.0"
 keywords = ["osd", "on-screen-display", "tail"]
 license = {text = "BSD-3-Clause"}
 dependencies = [
     "pyside6",
```

### Comparing `qosd-20230516/src/qosd.egg-info/PKG-INFO` & `qosd-20230518/src/qosd.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: qosd
-Version: 20230516
+Version: 20230518
 Summary: QOSD for python
-Author-email: Laurent Ghigonis <laurent.ghigonis@p1sec.com>
+Author-email: Laurent Ghigonis <ooookiwi@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/looran/qosd
 Keywords: osd,on-screen-display,tail
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 
 ## qosd - display text over your Xorg screen
```

### Comparing `qosd-20230516/src/qosd.py` & `qosd-20230518/src/qosd.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-VERSION = "20230516"
+VERSION = "20230518"
 DESCRIPTION = "display text over your Xorg screen"
 EXAMPLES = """examples:
 $ qosd hello
 $ tail -f /var/log/{messages,auth.log} | qosd -
 """
 
 from pathlib import Path
```

