# Comparing `tmp/eule-1.0.0.tar.gz` & `tmp/eule-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eule-1.0.0.tar", max compression
+gzip compressed data, was "eule-1.0.1.tar", max compression
```

## Comparing `eule-1.0.0.tar` & `eule-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2023-02-27 21:15:10.623533 eule-1.0.0/LICENSE
--rw-r--r--   0        0        0     2143 2023-05-18 18:13:32.035040 eule-1.0.0/README.md
--rw-r--r--   0        0        0      225 2023-05-18 17:59:12.995691 eule-1.0.0/eule/__init__.py
--rw-r--r--   0        0        0     6021 2023-05-18 17:41:10.495471 eule-1.0.0/eule/eule.py
--rw-r--r--   0        0        0     3015 2023-05-18 17:42:29.587779 eule-1.0.0/eule/utils.py
--rw-r--r--   0        0        0     1358 2023-05-18 18:15:42.783550 eule-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3212 1970-01-01 00:00:00.000000 eule-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-02-27 21:15:10.623533 eule-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2143 2023-05-18 18:13:32.035040 eule-1.0.1/README.md
+-rw-r--r--   0        0        0      225 2023-05-18 17:59:12.995691 eule-1.0.1/eule/__init__.py
+-rw-r--r--   0        0        0     5833 2023-05-18 18:53:33.608403 eule-1.0.1/eule/eule.py
+-rw-r--r--   0        0        0     3015 2023-05-18 17:42:29.587779 eule-1.0.1/eule/utils.py
+-rw-r--r--   0        0        0     1358 2023-05-18 19:13:25.369049 eule-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3212 1970-01-01 00:00:00.000000 eule-1.0.1/PKG-INFO
```

### Comparing `eule-1.0.0/LICENSE` & `eule-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eule-1.0.0/README.md` & `eule-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `eule-1.0.0/eule/eule.py` & `eule-1.0.1/eule/eule.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,18 +84,14 @@
 
                     # Retrieve intersection elements
                     comb_elems = intersection(celements, sets[set_key]) 
                     
                     # Non-empty intersection set
                     if len(comb_elems) != 0:
                         # Sort keys to assure deterministic behavior
-                        print('------')
-                        print(euler_tuple)
-                        print(set_key)
-                        print(update_tuple(euler_tuple, set_key))
                         comb_key = tuplify(sorted(update_tuple(euler_tuple, set_key)))
                         
                         # 2. Intersection of analysis element and exclusive group:
                         yield (comb_key, comb_elems)
 
                         # Remove intersection elements from current key-set and complementary sets
                         for euler_set_key in comb_key:
```

### Comparing `eule-1.0.0/eule/utils.py` & `eule-1.0.1/eule/utils.py`

 * *Files identical despite different names*

### Comparing `eule-1.0.0/pyproject.toml` & `eule-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eule"
-version = "1.0.0"
+version = "1.0.1"
 description = "Euler diagrams in python"
 authors = ["Bruno Peixoto <brunolnetto@gmail.com>"]
 license = "MIT license"
 readme = "README.md"
 packages = [{include = "eule"}]
 homepage = "https://pypi.org/project/eule/"
 repository = "https://github.com/trouchet/eule"
```

### Comparing `eule-1.0.0/PKG-INFO` & `eule-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eule
-Version: 1.0.0
+Version: 1.0.1
 Summary: Euler diagrams in python
 Home-page: https://pypi.org/project/eule/
 License: MIT
 Keywords: euler-diagram,sets
 Author: Bruno Peixoto
 Author-email: brunolnetto@gmail.com
 Requires-Python: >=3.8.1,<4.0
```

