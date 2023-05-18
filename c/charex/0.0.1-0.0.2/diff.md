# Comparing `tmp/charex-0.0.1.tar.gz` & `tmp/charex-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charex-0.0.1.tar", last modified: Thu May 18 14:41:05 2023, max compression
+gzip compressed data, was "charex-0.0.2.tar", last modified: Thu May 18 15:18:28 2023, max compression
```

## Comparing `charex-0.0.1.tar` & `charex-0.0.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-05-18 14:41:05.635619 charex-0.0.1/
--rw-r--r--   0 pji        (501) staff       (20)     1069 2023-04-20 18:29:08.000000 charex-0.0.1/LICENSE
--rw-r--r--   0 pji        (501) staff       (20)       38 2023-05-17 17:45:10.000000 charex-0.0.1/MANIFEST.in
--rw-r--r--   0 pji        (501) staff       (20)     3113 2023-05-18 14:41:05.635785 charex-0.0.1/PKG-INFO
--rw-r--r--   0 pji        (501) staff       (20)     2536 2023-05-17 17:47:37.000000 charex-0.0.1/README.rst
-drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-05-18 14:41:05.609323 charex-0.0.1/charex/
--rw-r--r--   0 pji        (501) staff       (20)      371 2023-05-18 14:38:22.000000 charex-0.0.1/charex/__init__.py
--rw-r--r--   0 pji        (501) staff       (20)      402 2023-05-18 14:38:22.000000 charex-0.0.1/charex/__main__.py
--rw-r--r--   0 pji        (501) staff       (20)    10185 2023-05-18 14:38:22.000000 charex-0.0.1/charex/charex.py
--rw-r--r--   0 pji        (501) staff       (20)    15803 2023-05-18 14:38:22.000000 charex-0.0.1/charex/charsets.py
-drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-05-18 14:41:05.630504 charex-0.0.1/charex/data/
--rw-r--r--   0 pji        (501) staff       (20)    76759 2023-04-24 18:02:02.000000 charex-0.0.1/charex/data/PropertyValueAliases.txt
--rw-r--r--   0 pji        (501) staff       (20)  1897793 2023-04-28 15:11:52.000000 charex-0.0.1/charex/data/UnicodeData.txt
--rw-r--r--   0 pji        (501) staff       (20)        0 2023-04-21 22:16:00.000000 charex-0.0.1/charex/data/__init__.py
-drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-05-18 14:41:05.631279 charex-0.0.1/charex/data/__pycache__/
--rw-r--r--   0 pji        (501) staff       (20)      154 2023-04-25 11:55:58.000000 charex-0.0.1/charex/data/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 pji        (501) staff       (20)   145897 2023-05-11 13:10:11.000000 charex-0.0.1/charex/data/entities.json
--rw-r--r--   0 pji        (501) staff       (20)      126 2023-05-08 18:24:17.000000 charex-0.0.1/charex/data/help_xt.txt
--rw-r--r--   0 pji        (501) staff       (20)      574 2023-05-04 17:01:12.000000 charex-0.0.1/charex/data/quote.html
--rw-r--r--   0 pji        (501) staff       (20)      573 2023-05-05 11:29:50.000000 charex-0.0.1/charex/data/result.html
--rw-r--r--   0 pji        (501) staff       (20)    99273 2023-05-17 16:34:15.000000 charex-0.0.1/charex/data/rev_casefold.json
--rw-r--r--   0 pji        (501) staff       (20)   685484 2023-05-17 16:25:24.000000 charex-0.0.1/charex/data/rev_nfc.json
--rw-r--r--   0 pji        (501) staff       (20)   676626 2023-05-17 16:28:18.000000 charex-0.0.1/charex/data/rev_nfd.json
--rw-r--r--   0 pji        (501) staff       (20)   802292 2023-05-17 16:29:56.000000 charex-0.0.1/charex/data/rev_nfkc.json
--rw-r--r--   0 pji        (501) staff       (20)   793983 2023-05-17 16:28:34.000000 charex-0.0.1/charex/data/rev_nfkd.json
--rw-r--r--   0 pji        (501) staff       (20)      391 2023-05-11 13:19:35.000000 charex-0.0.1/charex/data/sources.json
--rw-r--r--   0 pji        (501) staff       (20)     5028 2023-05-18 14:38:22.000000 charex-0.0.1/charex/denormal.py
--rw-r--r--   0 pji        (501) staff       (20)    15455 2023-05-18 14:38:22.000000 charex-0.0.1/charex/escape.py
--rw-r--r--   0 pji        (501) staff       (20)     2883 2023-05-18 14:38:22.000000 charex-0.0.1/charex/http.py
--rw-r--r--   0 pji        (501) staff       (20)     5064 2023-05-18 14:38:22.000000 charex-0.0.1/charex/normal.py
--rw-r--r--   0 pji        (501) staff       (20)    22728 2023-05-18 14:38:22.000000 charex-0.0.1/charex/shell.py
-drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-05-18 14:41:05.603132 charex-0.0.1/charex/static/
-drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-05-18 14:41:05.631808 charex-0.0.1/charex/static/styles/
--rw-r--r--   0 pji        (501) staff       (20)      455 2023-05-05 11:30:23.000000 charex-0.0.1/charex/static/styles/styles.css
--rw-r--r--   0 pji        (501) staff       (20)     4561 2023-05-18 14:38:22.000000 charex-0.0.1/charex/util.py
-drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-05-18 14:41:05.611492 charex-0.0.1/charex.egg-info/
--rw-r--r--   0 pji        (501) staff       (20)     3113 2023-05-18 14:41:05.000000 charex-0.0.1/charex.egg-info/PKG-INFO
--rw-r--r--   0 pji        (501) staff       (20)     1003 2023-05-18 14:41:05.000000 charex-0.0.1/charex.egg-info/SOURCES.txt
--rw-r--r--   0 pji        (501) staff       (20)        1 2023-05-18 14:41:05.000000 charex-0.0.1/charex.egg-info/dependency_links.txt
--rw-r--r--   0 pji        (501) staff       (20)       48 2023-05-18 14:41:05.000000 charex-0.0.1/charex.egg-info/entry_points.txt
--rw-r--r--   0 pji        (501) staff       (20)        6 2023-05-18 14:41:05.000000 charex-0.0.1/charex.egg-info/requires.txt
--rw-r--r--   0 pji        (501) staff       (20)        7 2023-05-18 14:41:05.000000 charex-0.0.1/charex.egg-info/top_level.txt
--rw-r--r--   0 pji        (501) staff       (20)      895 2023-05-18 12:33:55.000000 charex-0.0.1/pyproject.toml
--rw-r--r--   0 pji        (501) staff       (20)      204 2023-05-18 14:41:05.636420 charex-0.0.1/setup.cfg
-drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-05-18 14:41:05.635123 charex-0.0.1/tests/
--rw-r--r--   0 pji        (501) staff       (20)     5956 2023-05-18 14:38:23.000000 charex-0.0.1/tests/test_charex.py
--rw-r--r--   0 pji        (501) staff       (20)     2489 2023-05-18 14:38:22.000000 charex-0.0.1/tests/test_charset.py
--rw-r--r--   0 pji        (501) staff       (20)     2783 2023-05-18 14:38:22.000000 charex-0.0.1/tests/test_denormal.py
--rw-r--r--   0 pji        (501) staff       (20)     8775 2023-05-18 14:38:23.000000 charex-0.0.1/tests/test_escape.py
--rw-r--r--   0 pji        (501) staff       (20)     8204 2023-05-18 14:38:23.000000 charex-0.0.1/tests/test_main.py
--rw-r--r--   0 pji        (501) staff       (20)     3274 2023-05-18 14:38:23.000000 charex-0.0.1/tests/test_normal.py
--rw-r--r--   0 pji        (501) staff       (20)     6079 2023-05-18 14:38:23.000000 charex-0.0.1/tests/test_shell.py
--rw-r--r--   0 pji        (501) staff       (20)     2377 2023-05-18 14:38:22.000000 charex-0.0.1/tests/test_utility.py
+drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-05-18 15:18:28.977571 charex-0.0.2/
+-rw-r--r--   0 pji        (501) staff       (20)     1069 2023-04-20 18:29:08.000000 charex-0.0.2/LICENSE
+-rw-r--r--   0 pji        (501) staff       (20)       38 2023-05-17 17:45:10.000000 charex-0.0.2/MANIFEST.in
+-rw-r--r--   0 pji        (501) staff       (20)     3113 2023-05-18 15:18:28.977714 charex-0.0.2/PKG-INFO
+-rw-r--r--   0 pji        (501) staff       (20)     2536 2023-05-17 17:47:37.000000 charex-0.0.2/README.rst
+drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-05-18 15:18:28.948537 charex-0.0.2/charex/
+-rw-r--r--   0 pji        (501) staff       (20)      371 2023-05-18 15:17:51.000000 charex-0.0.2/charex/__init__.py
+-rw-r--r--   0 pji        (501) staff       (20)      402 2023-05-18 15:17:51.000000 charex-0.0.2/charex/__main__.py
+-rw-r--r--   0 pji        (501) staff       (20)    10185 2023-05-18 15:17:51.000000 charex-0.0.2/charex/charex.py
+-rw-r--r--   0 pji        (501) staff       (20)    15803 2023-05-18 15:17:51.000000 charex-0.0.2/charex/charsets.py
+drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-05-18 15:18:28.973271 charex-0.0.2/charex/data/
+-rw-r--r--   0 pji        (501) staff       (20)    76759 2023-04-24 18:02:02.000000 charex-0.0.2/charex/data/PropertyValueAliases.txt
+-rw-r--r--   0 pji        (501) staff       (20)  1897793 2023-04-28 15:11:52.000000 charex-0.0.2/charex/data/UnicodeData.txt
+-rw-r--r--   0 pji        (501) staff       (20)        0 2023-04-21 22:16:00.000000 charex-0.0.2/charex/data/__init__.py
+drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-05-18 15:18:28.974026 charex-0.0.2/charex/data/__pycache__/
+-rw-r--r--   0 pji        (501) staff       (20)      154 2023-04-25 11:55:58.000000 charex-0.0.2/charex/data/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 pji        (501) staff       (20)   145897 2023-05-11 13:10:11.000000 charex-0.0.2/charex/data/entities.json
+-rw-r--r--   0 pji        (501) staff       (20)      126 2023-05-08 18:24:17.000000 charex-0.0.2/charex/data/help_xt.txt
+-rw-r--r--   0 pji        (501) staff       (20)      574 2023-05-04 17:01:12.000000 charex-0.0.2/charex/data/quote.html
+-rw-r--r--   0 pji        (501) staff       (20)      573 2023-05-05 11:29:50.000000 charex-0.0.2/charex/data/result.html
+-rw-r--r--   0 pji        (501) staff       (20)    99273 2023-05-17 16:34:15.000000 charex-0.0.2/charex/data/rev_casefold.json
+-rw-r--r--   0 pji        (501) staff       (20)   685484 2023-05-17 16:25:24.000000 charex-0.0.2/charex/data/rev_nfc.json
+-rw-r--r--   0 pji        (501) staff       (20)   676626 2023-05-17 16:28:18.000000 charex-0.0.2/charex/data/rev_nfd.json
+-rw-r--r--   0 pji        (501) staff       (20)   802292 2023-05-17 16:29:56.000000 charex-0.0.2/charex/data/rev_nfkc.json
+-rw-r--r--   0 pji        (501) staff       (20)   793983 2023-05-17 16:28:34.000000 charex-0.0.2/charex/data/rev_nfkd.json
+-rw-r--r--   0 pji        (501) staff       (20)      391 2023-05-11 13:19:35.000000 charex-0.0.2/charex/data/sources.json
+-rw-r--r--   0 pji        (501) staff       (20)     5028 2023-05-18 15:17:51.000000 charex-0.0.2/charex/denormal.py
+-rw-r--r--   0 pji        (501) staff       (20)    15455 2023-05-18 15:17:51.000000 charex-0.0.2/charex/escape.py
+-rw-r--r--   0 pji        (501) staff       (20)     2883 2023-05-18 15:17:51.000000 charex-0.0.2/charex/http.py
+-rw-r--r--   0 pji        (501) staff       (20)     5064 2023-05-18 15:17:51.000000 charex-0.0.2/charex/normal.py
+-rw-r--r--   0 pji        (501) staff       (20)    23246 2023-05-18 15:17:51.000000 charex-0.0.2/charex/shell.py
+drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-05-18 15:18:28.944031 charex-0.0.2/charex/static/
+drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-05-18 15:18:28.974650 charex-0.0.2/charex/static/styles/
+-rw-r--r--   0 pji        (501) staff       (20)      455 2023-05-05 11:30:23.000000 charex-0.0.2/charex/static/styles/styles.css
+-rw-r--r--   0 pji        (501) staff       (20)     4561 2023-05-18 15:17:51.000000 charex-0.0.2/charex/util.py
+drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-05-18 15:18:28.950382 charex-0.0.2/charex.egg-info/
+-rw-r--r--   0 pji        (501) staff       (20)     3113 2023-05-18 15:18:28.000000 charex-0.0.2/charex.egg-info/PKG-INFO
+-rw-r--r--   0 pji        (501) staff       (20)     1003 2023-05-18 15:18:28.000000 charex-0.0.2/charex.egg-info/SOURCES.txt
+-rw-r--r--   0 pji        (501) staff       (20)        1 2023-05-18 15:18:28.000000 charex-0.0.2/charex.egg-info/dependency_links.txt
+-rw-r--r--   0 pji        (501) staff       (20)       48 2023-05-18 15:18:28.000000 charex-0.0.2/charex.egg-info/entry_points.txt
+-rw-r--r--   0 pji        (501) staff       (20)        6 2023-05-18 15:18:28.000000 charex-0.0.2/charex.egg-info/requires.txt
+-rw-r--r--   0 pji        (501) staff       (20)        7 2023-05-18 15:18:28.000000 charex-0.0.2/charex.egg-info/top_level.txt
+-rw-r--r--   0 pji        (501) staff       (20)      895 2023-05-18 15:15:01.000000 charex-0.0.2/pyproject.toml
+-rw-r--r--   0 pji        (501) staff       (20)      204 2023-05-18 15:18:28.978400 charex-0.0.2/setup.cfg
+drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-05-18 15:18:28.977321 charex-0.0.2/tests/
+-rw-r--r--   0 pji        (501) staff       (20)     5956 2023-05-18 15:17:51.000000 charex-0.0.2/tests/test_charex.py
+-rw-r--r--   0 pji        (501) staff       (20)     2489 2023-05-18 15:17:51.000000 charex-0.0.2/tests/test_charset.py
+-rw-r--r--   0 pji        (501) staff       (20)     2783 2023-05-18 15:17:51.000000 charex-0.0.2/tests/test_denormal.py
+-rw-r--r--   0 pji        (501) staff       (20)     8775 2023-05-18 15:17:51.000000 charex-0.0.2/tests/test_escape.py
+-rw-r--r--   0 pji        (501) staff       (20)     8204 2023-05-18 15:17:51.000000 charex-0.0.2/tests/test_main.py
+-rw-r--r--   0 pji        (501) staff       (20)     3274 2023-05-18 15:17:51.000000 charex-0.0.2/tests/test_normal.py
+-rw-r--r--   0 pji        (501) staff       (20)     6079 2023-05-18 15:17:51.000000 charex-0.0.2/tests/test_shell.py
+-rw-r--r--   0 pji        (501) staff       (20)     2377 2023-05-18 15:17:51.000000 charex-0.0.2/tests/test_utility.py
```

### Comparing `charex-0.0.1/LICENSE` & `charex-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `charex-0.0.1/PKG-INFO` & `charex-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: charex
-Version: 0.0.1
+Version: 0.0.2
 Summary: A unicode and character set explorer.
 Author-email: "Paul J. Iutzi" <pji@mac.com>
 Project-URL: Homepage, https://charex.readthedocs.io/en/latest/index.html#
 Project-URL: Documentation, https://charex.readthedocs.io/en/latest/index.html#
 Project-URL: Source, https://github.com/pji/charex
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `charex-0.0.1/README.rst` & `charex-0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `charex-0.0.1/charex/charex.py` & `charex-0.0.2/charex/charex.py`

 * *Files identical despite different names*

### Comparing `charex-0.0.1/charex/charsets.py` & `charex-0.0.2/charex/charsets.py`

 * *Files identical despite different names*

### Comparing `charex-0.0.1/charex/data/PropertyValueAliases.txt` & `charex-0.0.2/charex/data/PropertyValueAliases.txt`

 * *Files identical despite different names*

### Comparing `charex-0.0.1/charex/data/UnicodeData.txt` & `charex-0.0.2/charex/data/UnicodeData.txt`

 * *Files identical despite different names*

### Comparing `charex-0.0.1/charex/data/entities.json` & `charex-0.0.2/charex/data/entities.json`

 * *Files identical despite different names*

### Comparing `charex-0.0.1/charex/data/quote.html` & `charex-0.0.2/charex/data/quote.html`

 * *Files identical despite different names*

### Comparing `charex-0.0.1/charex/data/result.html` & `charex-0.0.2/charex/data/result.html`

 * *Files identical despite different names*

### Comparing `charex-0.0.1/charex/data/rev_casefold.json` & `charex-0.0.2/charex/data/rev_casefold.json`

 * *Files identical despite different names*

### Comparing `charex-0.0.1/charex/data/rev_nfc.json` & `charex-0.0.2/charex/data/rev_nfc.json`

 * *Files identical despite different names*

### Comparing `charex-0.0.1/charex/data/rev_nfd.json` & `charex-0.0.2/charex/data/rev_nfd.json`

 * *Files identical despite different names*

### Comparing `charex-0.0.1/charex/data/rev_nfkc.json` & `charex-0.0.2/charex/data/rev_nfkc.json`

 * *Files identical despite different names*

### Comparing `charex-0.0.1/charex/data/rev_nfkd.json` & `charex-0.0.2/charex/data/rev_nfkd.json`

 * *Files identical despite different names*

### Comparing `charex-0.0.1/charex/denormal.py` & `charex-0.0.2/charex/denormal.py`

 * *Files identical despite different names*

### Comparing `charex-0.0.1/charex/escape.py` & `charex-0.0.2/charex/escape.py`

 * *Files identical despite different names*

### Comparing `charex-0.0.1/charex/http.py` & `charex-0.0.2/charex/http.py`

 * *Files identical despite different names*

### Comparing `charex-0.0.1/charex/normal.py` & `charex-0.0.2/charex/normal.py`

 * *Files identical despite different names*

### Comparing `charex-0.0.1/charex/shell.py` & `charex-0.0.2/charex/shell.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,15 +205,21 @@
                     char = ch.Character(item)
                     values.append('  ' + char.summarize())
         if not values:
             return ''
         return ('\n' + ' ' * 22).join(v for v in values)
 
     # Gather the details for display.
-    char = ch.Character(args.codepoint)
+    cp = args.codepoint
+    if cp.startswith('U+'):
+        cp = '0x' + cp[2:]
+    if cp.startswith('0x'):
+        n = int(cp, 16)
+        cp = chr(n)
+    char = ch.Character(cp)
     details = (
         ('Display', char.value),
         ('Name', char.name),
         ('Code Point', char.code_point),
         ('Category', char.category),
         ('UTF-8', char.encode('utf8')),
         ('UTF-16', char.encode('utf_16_be')),
@@ -279,14 +285,21 @@
 
     :param args: The arguments used when the script was invoked.
     :return: None.
     :rtype: NoneType
     """
     result = nl.normalize(args.form, args.base)
     print(result)
+    if args.expand:
+        for item in result:
+            char = ch.Character(item)
+            indent = '  '
+            if 'mark' in char.category.casefold():
+                indent += ' '
+            print(f'  {char.summarize()}')
     print()
 
 
 def mode_sh(args: Namespace | None) -> None:
     """Run in an interactive shell.
 
     :param args: The arguments used when the script was invoked.
@@ -650,14 +663,19 @@
     )
     sp.add_argument(
         'base',
         help='The base normalized string.',
         action='store',
         type=str
     )
+    sp.add_argument(
+        '-e', '--expand',
+        help='Show each character in the normalized string.',
+        action='store_true'
+    )
     sp.set_defaults(func=mode_nl)
 
 
 def parse_sh(spa: _SubParsersAction) -> None:
     """Add the shell mode subparser.
 
     :param spa: The subparser action used to add a new subparser to
```

### Comparing `charex-0.0.1/charex/util.py` & `charex-0.0.2/charex/util.py`

 * *Files identical despite different names*

### Comparing `charex-0.0.1/charex.egg-info/PKG-INFO` & `charex-0.0.2/charex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: charex
-Version: 0.0.1
+Version: 0.0.2
 Summary: A unicode and character set explorer.
 Author-email: "Paul J. Iutzi" <pji@mac.com>
 Project-URL: Homepage, https://charex.readthedocs.io/en/latest/index.html#
 Project-URL: Documentation, https://charex.readthedocs.io/en/latest/index.html#
 Project-URL: Source, https://github.com/pji/charex
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `charex-0.0.1/charex.egg-info/SOURCES.txt` & `charex-0.0.2/charex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `charex-0.0.1/pyproject.toml` & `charex-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 [tool.pytest.ini_options]
 addopts = [
     "--import-mode=importlib",
 ]
 
 [project]
 name = "charex"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     {name="Paul J. Iutzi", email="pji@mac.com"},
 ]
 description = "A unicode and character set explorer."
 readme = "README.rst"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `charex-0.0.1/tests/test_charex.py` & `charex-0.0.2/tests/test_charex.py`

 * *Files identical despite different names*

### Comparing `charex-0.0.1/tests/test_charset.py` & `charex-0.0.2/tests/test_charset.py`

 * *Files identical despite different names*

### Comparing `charex-0.0.1/tests/test_denormal.py` & `charex-0.0.2/tests/test_denormal.py`

 * *Files identical despite different names*

### Comparing `charex-0.0.1/tests/test_escape.py` & `charex-0.0.2/tests/test_escape.py`

 * *Files identical despite different names*

### Comparing `charex-0.0.1/tests/test_main.py` & `charex-0.0.2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `charex-0.0.1/tests/test_normal.py` & `charex-0.0.2/tests/test_normal.py`

 * *Files identical despite different names*

### Comparing `charex-0.0.1/tests/test_shell.py` & `charex-0.0.2/tests/test_shell.py`

 * *Files identical despite different names*

### Comparing `charex-0.0.1/tests/test_utility.py` & `charex-0.0.2/tests/test_utility.py`

 * *Files identical despite different names*

