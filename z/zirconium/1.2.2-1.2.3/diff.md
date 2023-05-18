# Comparing `tmp/zirconium-1.2.2.tar.gz` & `tmp/zirconium-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zirconium-1.2.2.tar", last modified: Tue May 16 13:31:40 2023, max compression
+gzip compressed data, was "zirconium-1.2.3.tar", last modified: Thu May 18 18:40:24 2023, max compression
```

## Comparing `zirconium-1.2.2.tar` & `zirconium-1.2.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 13:31:40.832571 zirconium-1.2.2/
--rw-rw-rw-   0        0        0     1058 2023-04-28 14:59:36.000000 zirconium-1.2.2/LICENSE
--rw-rw-rw-   0        0        0    11871 2023-05-16 13:31:40.832571 zirconium-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0    11326 2023-05-15 21:53:38.000000 zirconium-1.2.2/README.md
--rw-rw-rw-   0        0        0       88 2023-04-28 14:59:36.000000 zirconium-1.2.2/pyproject.toml
--rw-rw-rw-   0        0        0      684 2023-05-16 13:31:40.833573 zirconium-1.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-16 13:31:40.807569 zirconium-1.2.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-16 13:31:40.822574 zirconium-1.2.2/src/zirconium/
--rw-rw-rw-   0        0        0      331 2023-05-16 13:31:28.000000 zirconium-1.2.2/src/zirconium/__init__.py
--rw-rw-rw-   0        0        0    23443 2023-05-16 13:31:17.000000 zirconium-1.2.2/src/zirconium/config.py
--rw-rw-rw-   0        0        0     5155 2023-04-28 14:59:36.000000 zirconium-1.2.2/src/zirconium/parsers.py
--rw-rw-rw-   0        0        0     1148 2023-04-28 14:59:36.000000 zirconium-1.2.2/src/zirconium/sproviders.py
--rw-rw-rw-   0        0        0     9581 2023-05-15 21:37:14.000000 zirconium-1.2.2/src/zirconium/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-16 13:31:40.827571 zirconium-1.2.2/src/zirconium.egg-info/
--rw-rw-rw-   0        0        0    11871 2023-05-16 13:31:40.000000 zirconium-1.2.2/src/zirconium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-05-16 13:31:40.000000 zirconium-1.2.2/src/zirconium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 13:31:40.000000 zirconium-1.2.2/src/zirconium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-16 13:31:40.000000 zirconium-1.2.2/src/zirconium.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-16 13:31:40.830571 zirconium-1.2.2/tests/
--rw-rw-rw-   0        0        0    23017 2023-05-16 13:30:42.000000 zirconium-1.2.2/tests/test_config.py
--rw-rw-rw-   0        0        0    12057 2023-04-28 14:59:36.000000 zirconium-1.2.2/tests/test_handlers.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:40:24.691616 zirconium-1.2.3/
+-rw-rw-rw-   0        0        0     1058 2023-04-28 14:59:36.000000 zirconium-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0    11871 2023-05-18 18:40:24.692616 zirconium-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0    11326 2023-05-15 21:53:38.000000 zirconium-1.2.3/README.md
+-rw-rw-rw-   0        0        0       88 2023-04-28 14:59:36.000000 zirconium-1.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0      684 2023-05-18 18:40:24.693615 zirconium-1.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-18 18:40:24.664685 zirconium-1.2.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-18 18:40:24.678692 zirconium-1.2.3/src/zirconium/
+-rw-rw-rw-   0        0        0      331 2023-05-18 18:40:06.000000 zirconium-1.2.3/src/zirconium/__init__.py
+-rw-rw-rw-   0        0        0    23443 2023-05-16 13:31:17.000000 zirconium-1.2.3/src/zirconium/config.py
+-rw-rw-rw-   0        0        0     5155 2023-04-28 14:59:36.000000 zirconium-1.2.3/src/zirconium/parsers.py
+-rw-rw-rw-   0        0        0     1148 2023-04-28 14:59:36.000000 zirconium-1.2.3/src/zirconium/sproviders.py
+-rw-rw-rw-   0        0        0     9608 2023-05-18 18:39:59.000000 zirconium-1.2.3/src/zirconium/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:40:24.685616 zirconium-1.2.3/src/zirconium.egg-info/
+-rw-rw-rw-   0        0        0    11871 2023-05-18 18:40:24.000000 zirconium-1.2.3/src/zirconium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-05-18 18:40:24.000000 zirconium-1.2.3/src/zirconium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 18:40:24.000000 zirconium-1.2.3/src/zirconium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-18 18:40:24.000000 zirconium-1.2.3/src/zirconium.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 18:40:24.690616 zirconium-1.2.3/tests/
+-rw-rw-rw-   0        0        0    23017 2023-05-16 13:30:42.000000 zirconium-1.2.3/tests/test_config.py
+-rw-rw-rw-   0        0        0    12057 2023-04-28 14:59:36.000000 zirconium-1.2.3/tests/test_handlers.py
```

### Comparing `zirconium-1.2.2/LICENSE` & `zirconium-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zirconium-1.2.2/PKG-INFO` & `zirconium-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zirconium
-Version: 1.2.2
+Version: 1.2.3
 Summary: Excellent configuration management for Python
 Home-page: https://github.com/turnbullerin/zirconium
 Author: Erin Turnbull
 Author-email: erin.a.turnbull@gmail.com
 Project-URL: Bug Tracker, https://github.com/turnbullerin/zirconium/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `zirconium-1.2.2/README.md` & `zirconium-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `zirconium-1.2.2/setup.cfg` & `zirconium-1.2.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 207a 6972 636f 6e69 756d 0d0a 7665   = zirconium..ve
-00000020: 7273 696f 6e20 3d20 312e 322e 320d 0a61  rsion = 1.2.2..a
+00000020: 7273 696f 6e20 3d20 312e 322e 330d 0a61  rsion = 1.2.3..a
 00000030: 7574 686f 7220 3d20 4572 696e 2054 7572  uthor = Erin Tur
 00000040: 6e62 756c 6c0d 0a61 7574 686f 725f 656d  nbull..author_em
 00000050: 6169 6c20 3d20 6572 696e 2e61 2e74 7572  ail = erin.a.tur
 00000060: 6e62 756c 6c40 676d 6169 6c2e 636f 6d0d  nbull@gmail.com.
 00000070: 0a64 6573 6372 6970 7469 6f6e 203d 2045  .description = E
 00000080: 7863 656c 6c65 6e74 2063 6f6e 6669 6775  xcellent configu
 00000090: 7261 7469 6f6e 206d 616e 6167 656d 656e  ration managemen
```

### Comparing `zirconium-1.2.2/src/zirconium/config.py` & `zirconium-1.2.3/src/zirconium/config.py`

 * *Files identical despite different names*

### Comparing `zirconium-1.2.2/src/zirconium/parsers.py` & `zirconium-1.2.3/src/zirconium/parsers.py`

 * *Files identical despite different names*

### Comparing `zirconium-1.2.2/src/zirconium/sproviders.py` & `zirconium-1.2.3/src/zirconium/sproviders.py`

 * *Files identical despite different names*

### Comparing `zirconium-1.2.2/src/zirconium/utils.py` & `zirconium-1.2.3/src/zirconium/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
             for entry in val:
                 print(f"{prefix * (level+1)}- {_obfuscate_entry(entry)}")
         else:
             print(f"{prefix * level}{key}: {_obfuscate_entry(val)}")
 
 
 def _obfuscate_entry(entry):
-    if "://" in entry:
+    if isinstance(entry, str) and "://" in entry:
         try:
             uri = urlparse(entry)
             if uri.password:
                 qs = f"?{uri.query}" if uri.query else ""
                 fs = f"#{uri.fragment}" if uri.fragment else ""
                 return f"{uri.scheme}://{uri.username}:{'*' * len(uri.password)}@{uri.hostname}{uri.path}{qs}{fs}"
         except ValueError:
```

### Comparing `zirconium-1.2.2/src/zirconium.egg-info/PKG-INFO` & `zirconium-1.2.3/src/zirconium.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zirconium
-Version: 1.2.2
+Version: 1.2.3
 Summary: Excellent configuration management for Python
 Home-page: https://github.com/turnbullerin/zirconium
 Author: Erin Turnbull
 Author-email: erin.a.turnbull@gmail.com
 Project-URL: Bug Tracker, https://github.com/turnbullerin/zirconium/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `zirconium-1.2.2/tests/test_config.py` & `zirconium-1.2.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `zirconium-1.2.2/tests/test_handlers.py` & `zirconium-1.2.3/tests/test_handlers.py`

 * *Files identical despite different names*

