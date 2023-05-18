# Comparing `tmp/tab-aaron-alphabet-0.0.0.tar.gz` & `tmp/tab-aaron-alphabet-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tab-aaron-alphabet-0.0.0.tar", last modified: Sat Apr  8 08:02:14 2023, max compression
+gzip compressed data, was "tab-aaron-alphabet-0.0.1.tar", last modified: Thu May 18 12:36:17 2023, max compression
```

## Comparing `tab-aaron-alphabet-0.0.0.tar` & `tab-aaron-alphabet-0.0.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 lk        (1002) lk        (1002)        0 2023-04-08 08:02:14.881969 tab-aaron-alphabet-0.0.0/
--rwxrwxrwx   0 lk        (1002) lk        (1002)     1066 2023-03-01 20:28:52.000000 tab-aaron-alphabet-0.0.0/LICENSE
--rw-rw-r--   0 lk        (1002) lk        (1002)     1470 2023-04-08 08:02:14.881969 tab-aaron-alphabet-0.0.0/PKG-INFO
--rwxrwxrwx   0 lk        (1002) lk        (1002)      499 2023-04-08 07:54:17.000000 tab-aaron-alphabet-0.0.0/pyproject.toml
--rwxrwxrwx   0 lk        (1002) lk        (1002)       38 2023-04-08 08:02:14.881969 tab-aaron-alphabet-0.0.0/setup.cfg
-drwxrwxr-x   0 lk        (1002) lk        (1002)        0 2023-04-08 08:02:14.881969 tab-aaron-alphabet-0.0.0/src/
-drwxrwxr-x   0 lk        (1002) lk        (1002)        0 2023-04-08 08:02:14.881969 tab-aaron-alphabet-0.0.0/src/tab_aaron_alphabet/
--rwxrwxrwx   0 lk        (1002) lk        (1002)      956 2023-04-08 08:01:25.000000 tab-aaron-alphabet-0.0.0/src/tab_aaron_alphabet/__init__.py
--rwxrwxrwx   0 lk        (1002) lk        (1002)       75 2023-04-08 07:54:57.000000 tab-aaron-alphabet-0.0.0/src/tab_aaron_alphabet/__main__.py
-drwxrwxr-x   0 lk        (1002) lk        (1002)        0 2023-04-08 08:02:14.881969 tab-aaron-alphabet-0.0.0/src/tab_aaron_alphabet.egg-info/
--rw-rw-r--   0 lk        (1002) lk        (1002)     1470 2023-04-08 08:02:14.000000 tab-aaron-alphabet-0.0.0/src/tab_aaron_alphabet.egg-info/PKG-INFO
--rw-rw-r--   0 lk        (1002) lk        (1002)      286 2023-04-08 08:02:14.000000 tab-aaron-alphabet-0.0.0/src/tab_aaron_alphabet.egg-info/SOURCES.txt
--rw-rw-r--   0 lk        (1002) lk        (1002)        1 2023-04-08 08:02:14.000000 tab-aaron-alphabet-0.0.0/src/tab_aaron_alphabet.egg-info/dependency_links.txt
--rw-rw-r--   0 lk        (1002) lk        (1002)       19 2023-04-08 08:02:14.000000 tab-aaron-alphabet-0.0.0/src/tab_aaron_alphabet.egg-info/top_level.txt
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-18 12:36:17.035159 tab-aaron-alphabet-0.0.1/
+-rwxrwxrwx   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 tab-aaron-alphabet-0.0.1/LICENSE
+-rw-rw-r--   0 base      (1001) base      (1001)     1470 2023-05-18 12:36:17.035159 tab-aaron-alphabet-0.0.1/PKG-INFO
+-rwxrwxrwx   0 base      (1001) base      (1001)      530 2023-05-18 12:34:01.000000 tab-aaron-alphabet-0.0.1/pyproject.toml
+-rwxrwxrwx   0 base      (1001) base      (1001)       38 2023-05-18 12:36:17.035159 tab-aaron-alphabet-0.0.1/setup.cfg
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-18 12:36:17.035159 tab-aaron-alphabet-0.0.1/src/
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-18 12:36:17.035159 tab-aaron-alphabet-0.0.1/src/tab_aaron_alphabet/
+-rwxrwxrwx   0 base      (1001) base      (1001)      560 2023-05-18 12:20:33.000000 tab-aaron-alphabet-0.0.1/src/tab_aaron_alphabet/__init__.py
+-rwxrwxrwx   0 base      (1001) base      (1001)       75 2023-04-08 07:54:57.000000 tab-aaron-alphabet-0.0.1/src/tab_aaron_alphabet/__main__.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-18 12:36:17.035159 tab-aaron-alphabet-0.0.1/src/tab_aaron_alphabet.egg-info/
+-rw-rw-r--   0 base      (1001) base      (1001)     1470 2023-05-18 12:36:17.000000 tab-aaron-alphabet-0.0.1/src/tab_aaron_alphabet.egg-info/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)      331 2023-05-18 12:36:17.000000 tab-aaron-alphabet-0.0.1/src/tab_aaron_alphabet.egg-info/SOURCES.txt
+-rw-rw-r--   0 base      (1001) base      (1001)        1 2023-05-18 12:36:17.000000 tab-aaron-alphabet-0.0.1/src/tab_aaron_alphabet.egg-info/dependency_links.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       25 2023-05-18 12:36:17.000000 tab-aaron-alphabet-0.0.1/src/tab_aaron_alphabet.egg-info/requires.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       19 2023-05-18 12:36:17.000000 tab-aaron-alphabet-0.0.1/src/tab_aaron_alphabet.egg-info/top_level.txt
```

### Comparing `tab-aaron-alphabet-0.0.0/LICENSE` & `tab-aaron-alphabet-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tab-aaron-alphabet-0.0.0/PKG-INFO` & `tab-aaron-alphabet-0.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tab-aaron-alphabet
-Version: 0.0.0
+Version: 0.0.1
 Summary: Convert tab to 4 spaces. 
 Author-email: Aaron Alphabet <aaron.alphabet@gmx.ch>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `tab-aaron-alphabet-0.0.0/src/tab_aaron_alphabet.egg-info/PKG-INFO` & `tab-aaron-alphabet-0.0.1/src/tab_aaron_alphabet.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tab-aaron-alphabet
-Version: 0.0.0
+Version: 0.0.1
 Summary: Convert tab to 4 spaces. 
 Author-email: Aaron Alphabet <aaron.alphabet@gmx.ch>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

