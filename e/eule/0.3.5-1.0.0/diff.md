# Comparing `tmp/eule-0.3.5.tar.gz` & `tmp/eule-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eule-0.3.5.tar", max compression
+gzip compressed data, was "eule-1.0.0.tar", max compression
```

## Comparing `eule-0.3.5.tar` & `eule-1.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2023-02-27 21:15:10.623533 eule-0.3.5/LICENSE
--rw-r--r--   0        0        0     1873 2023-04-23 22:40:19.368385 eule-0.3.5/README.md
--rw-r--r--   0        0        0      222 2023-04-30 12:36:21.742153 eule-0.3.5/eule/__init__.py
--rw-r--r--   0        0        0     5697 2023-04-18 19:12:36.364911 eule-0.3.5/eule/eule.py
--rw-r--r--   0        0        0     2856 2023-04-18 19:12:36.364911 eule-0.3.5/eule/utils.py
--rw-r--r--   0        0        0     1358 2023-04-30 12:37:25.166400 eule-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     2942 1970-01-01 00:00:00.000000 eule-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-02-27 21:15:10.623533 eule-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2143 2023-05-18 18:13:32.035040 eule-1.0.0/README.md
+-rw-r--r--   0        0        0      225 2023-05-18 17:59:12.995691 eule-1.0.0/eule/__init__.py
+-rw-r--r--   0        0        0     6021 2023-05-18 17:41:10.495471 eule-1.0.0/eule/eule.py
+-rw-r--r--   0        0        0     3015 2023-05-18 17:42:29.587779 eule-1.0.0/eule/utils.py
+-rw-r--r--   0        0        0     1358 2023-05-18 18:15:42.783550 eule-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3212 1970-01-01 00:00:00.000000 eule-1.0.0/PKG-INFO
```

### Comparing `eule-0.3.5/LICENSE` & `eule-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eule-0.3.5/README.md` & `eule-1.0.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -31,29 +31,37 @@
 Minimal example
 ================
 
 We run command `python example.py` on the folder with file `example.py` and following content:
 
 ``` {.python}
 #!/usr/bin/env python
-import eule
+from eule import euler
 
-set = {
+sets = {
     'a': [1, 2, 3],
     'b': [2, 3, 4],
     'c': [3, 4, 5],
     'd': [3, 5, 6]
 }
 
-diagram = eule.euler(set)
+euler_diagram = euler(sets)
+euler_keys = euler_keys(sets)
+euler_boundaries = euler_boundaries(sets)
 
-# Euler dictionary:
+# Euler dictionary: 
+# {'a,b': [2], 'b,c': [4], 'a,b,c,d': [3], 'c,d': [5], 'd': [6], 'a': [1]}
+print(euler_diagram)
+
+# Euler keys list:
+# ['a,b', 'b,c', 'a,b,c,d', 'c,d', 'd', 'a']
+print(euler_keys)
+
+# Euler boundaries dictionary: 
 # {
-#     ('a', 'b'): [2], 
-#     ('b', 'c'): [4], 
-#     ('a', 'b', 'c', 'd'): [3], 
-#     ('d',): [6], 
-#     ('c', 'd'): [5], 
-#     ('a',): [1]
+#   'a': ['b', 'c', 'd'], 
+#   'b': ['a', 'c', 'd'], 
+#   'c': ['a', 'b', 'd'], 
+#   'd': ['a', 'b', 'c']
 # }
-print(diagram)
+print(euler_boundaries)
 ```
```

### Comparing `eule-0.3.5/eule/eule.py` & `eule-1.0.0/eule/eule.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,15 @@
 """Main module."""
 
 from copy import deepcopy
 from warnings import warn
 
 from .utils import update_tuple, clear, reduc, uniq, union, difference, intersection, tuplify
 
-def eulerGenerator(sets):
-    """This generator function returns each tuple (key, elems) of the Euler diagram in a generator-wise fashion systematic:
-    
-    1. Begin with the available `sets` and their exclusive elements;
-    2. Compute complementary elements to current key-set;
-    3. In case complementary set-keys AND current set content are not empty, continue; Otherwise, go to next key-set;
-    4. Find the euler diagram on complementary sets;
-    5. Compute exclusive combination elements;
-    6. In case there are exclusive elements to combination: yield exclusive combination elements; Remove exclusive combination elements from current key-set. 
-
-    :param dict sets: array/dict of arrays
-    :returns: (key, euler_set) tuple of given sets
-    :rtype: tuple
-    """
-    sets_ = deepcopy(sets)
-
+def validate_euler_generator_input(sets_):
     # There are no sets
     if not isinstance(sets_, (list, dict)):
         msg_1 = 'Ill-conditioned input.'
         msg_2 = 'It must be either a dict or array of arrays object!'
         raise TypeError(msg_1 + msg_2)
 
     is_unique_set_arr = [
@@ -32,84 +17,107 @@
     ]
 
     def and_map(a, b):
         return (a and b)
 
     if not reduc(and_map, is_unique_set_arr, True):
         warn('Each array MUST NOT have duplicates')
-        sets = {key: uniq(values) for key, values in sets.items()}
+        sets_ = {key: uniq(values) for key, values in sets_.items()}
+
+    return sets_
+
+
+def euler_generator(sets):
+    """This generator function returns each tuple (key, elems) of the Euler diagram in a generator-wise fashion systematic:
+    
+    1. Begin with the available `sets` and their exclusive elements;
+    2. Compute complementary elements to current key-set;
+    3. In case complementary set-keys AND current set content are not empty, continue; Otherwise, go to next key-set;
+    4. Find the euler diagram on complementary sets;
+    5. Compute exclusive combination elements;
+    6. In case there are exclusive elements to combination: yield exclusive combination elements; Remove exclusive combination elements from current key-set. 
+
+    :param dict sets: array/dict of arrays
+    :returns: (key, euler_set) tuple of given sets
+    :rtype: tuple
+    """
+    sets_ = deepcopy(sets)
+    sets_ = validate_euler_generator_input(sets_)
 
     # Only a set
     if len(sets_.keys()) == 1:
         comb_key = list(sets_.keys())[0]
         comb_elements = list(sets_.values())[0]
         yield ((comb_key), comb_elements)
 
     else:
         # Sets with non-empty elements
         set_keys = clear(sets_)
 
         # Traverse the combination lattice
         for set_key in set_keys:
             compl_sets_keys = difference(set_keys, [set_key])
-
+            
             # There are still sets to analyze
             if len(compl_sets_keys) != 0 and len(sets[set_key]) != 0:
                 # Complementary sets
                 csets = {cset_key: sets_[cset_key] for cset_key in compl_sets_keys}
 
                 # Instrospective recursion: Exclusive combination elements
-                for euler_tuple, celements in eulerGenerator(csets):
+                for euler_tuple, celements in euler_generator(csets):
 
                     # Remove current set_key elements
                     comb_elems = difference(celements, sets_[set_key])
-
+                    
                     # Non-empty combination exclusivity case
                     if len(comb_elems) != 0:
                         # Sort keys to assure deterministic behavior
                         sorted_comb_key = tuplify(sorted(tuplify(euler_tuple)))
                         
-                        # 1. Exclusive group elements except current analysis set
+                        # 1. Exclusive elements respective complementary keys
                         yield (sorted_comb_key, comb_elems)
-
+                        
                         # Remove comb_elems elements from its original sets
-                        for euler_set_key in euler_tuple:
+                        for euler_set_key in sorted_comb_key:
                             sets_[euler_set_key] = difference(sets_[euler_set_key], comb_elems)
                     else:
                         pass
 
                     # Retrieve intersection elements
                     comb_elems = intersection(celements, sets[set_key]) 
                     
                     # Non-empty intersection set
                     if len(comb_elems) != 0:
-                        # 2. Intersection of analysis element and exclusive group:
                         # Sort keys to assure deterministic behavior
+                        print('------')
+                        print(euler_tuple)
+                        print(set_key)
+                        print(update_tuple(euler_tuple, set_key))
                         comb_key = tuplify(sorted(update_tuple(euler_tuple, set_key)))
                         
+                        # 2. Intersection of analysis element and exclusive group:
                         yield (comb_key, comb_elems)
 
                         # Remove intersection elements from current key-set and complementary sets
-                        for euler_set_key in euler_tuple:
+                        for euler_set_key in comb_key:
                             sets_[euler_set_key] = difference(sets_[euler_set_key], comb_elems)
 
                         sets_[set_key] = difference(sets_[set_key], comb_elems)
 
                     else:
                         pass
 
                     set_keys = clear(sets_)
 
-                # 3. Remaining exclusive elements
                 if len(sets_[set_key]) != 0:
                     # Load combination key
-                    comb_key = tuplify([set_key])
+                    comb_key = (set_key, )
                     comb_elems = sets_[set_key]       
 
-                    # Yield tuple
+                    # 3. Remaining exclusive elements
                     yield (comb_key, comb_elems)
 
                     # Remove remaining set elements
                     sets_[set_key] = []
                 
                 else:
                     pass
@@ -120,35 +128,35 @@
 def euler(sets):
     """Euler diagram dictionary of set-dictionary of non-repetitive elements
     
     :param dict sets: array/dict of arrays
     :returns: euler sets
     :rtype: dict
     """
-    return dict(eulerGenerator(sets))
+    return dict(euler_generator(sets))
 
-def eulerKeys(sets):
+def euler_keys(sets):
     """Euler diagram keys
     
     :param dict sets: array/dict of arrays
     :returns: euler sets keys
     :rtype: list
     """
     return list(euler(sets).keys())
 
-def eulerBoundaries(sets):
+def euler_boundaries(sets):
     """Euler diagram set boundaries 
     
     :param dict sets: array/dict of arrays
     :returns: euler boundary dict
     :rtype: list
     """
 
     setsKeys = list(sets.keys())
-    eulerSetsKeys = eulerKeys(sets)
+    eulerSetsKeys = euler_keys(sets)
 
     boundaries = dict(map(lambda key: (key, []), setsKeys))
 
     for setKey in setsKeys:
         for eulerSetKeys in eulerSetsKeys:
             if setKey in eulerSetKeys:
                 boundaries[setKey] = union(boundaries[setKey], difference(eulerSetKeys, [setKey]))
```

### Comparing `eule-0.3.5/eule/utils.py` & `eule-1.0.0/eule/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,25 +7,23 @@
 
     :param function func: Reduce callback
     :param dict elems: list of elements
     :param dict elem0: first elements 
     """
     return reduce(func, elems + [elem0])
 
-
 def uniq(lst):
     """This map returns list with unique elements
 
     :param list lst: array of elements entries 
     :returns: list with unique elements 
     :rtype: list
     """
     return list(unique(lst))
 
-
 def dsort(str_, delimiter):
     """This map returns a sorted string delimited by token
 
     :param str str_:  string with delimiter between elements 
     :returns: string with sorted elements delimited by given delimiter 
     :rtype: str
     """
@@ -37,15 +35,18 @@
     :param candidate: tuplification candidate
     :returns: string with sorted elements delimited by given delimiter 
     :rtype: str
     """
     return candidate if isinstance(candidate, tuple) \
         else ( \
             tuple(candidate) if isinstance(candidate, list) \
-            else (candidate)
+            else ( \
+                (candidate,) if isinstance(candidate, str) \
+                else (candidate,) 
+            )
         )
 
 
 def clear(sets):
     """This map returns a set with non-empty values
 
     :param dict set:  
@@ -62,15 +63,18 @@
 
     :param tuple of elements:
     :param value: element to update
     :returns: an ordered and updated tuple
     :rtype: tuple
     """
     
-    return tuple(list(tuple_)+[value])
+    tuple_lst=list(tuplify(tuple_))
+    tuple_lst.append(value)
+    
+    return tuple(tuple_lst)
 
 def list_to_set(arr):
     """This map converts a list into a set
 
     :param list of elements:  
     :returns: a set-converted list
     :rtype: set
@@ -105,7 +109,8 @@
     :param listA:
     :param listB:
     :returns: intersection list with non-repeated elements
     :rtype: list
     """
     
     return list(list_to_set(listA).intersection(list_to_set(listB)))
+
```

### Comparing `eule-0.3.5/pyproject.toml` & `eule-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eule"
-version = "0.3.5"
+version = "1.0.0"
 description = "Euler diagrams in python"
 authors = ["Bruno Peixoto <brunolnetto@gmail.com>"]
 license = "MIT license"
 readme = "README.md"
 packages = [{include = "eule"}]
 homepage = "https://pypi.org/project/eule/"
 repository = "https://github.com/trouchet/eule"
```

### Comparing `eule-0.3.5/PKG-INFO` & `eule-1.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eule
-Version: 0.3.5
+Version: 1.0.0
 Summary: Euler diagrams in python
 Home-page: https://pypi.org/project/eule/
 License: MIT
 Keywords: euler-diagram,sets
 Author: Bruno Peixoto
 Author-email: brunolnetto@gmail.com
 Requires-Python: >=3.8.1,<4.0
@@ -59,30 +59,38 @@
 Minimal example
 ================
 
 We run command `python example.py` on the folder with file `example.py` and following content:
 
 ``` {.python}
 #!/usr/bin/env python
-import eule
+from eule import euler
 
-set = {
+sets = {
     'a': [1, 2, 3],
     'b': [2, 3, 4],
     'c': [3, 4, 5],
     'd': [3, 5, 6]
 }
 
-diagram = eule.euler(set)
+euler_diagram = euler(sets)
+euler_keys = euler_keys(sets)
+euler_boundaries = euler_boundaries(sets)
+
+# Euler dictionary: 
+# {'a,b': [2], 'b,c': [4], 'a,b,c,d': [3], 'c,d': [5], 'd': [6], 'a': [1]}
+print(euler_diagram)
+
+# Euler keys list:
+# ['a,b', 'b,c', 'a,b,c,d', 'c,d', 'd', 'a']
+print(euler_keys)
 
-# Euler dictionary:
+# Euler boundaries dictionary: 
 # {
-#     ('a', 'b'): [2], 
-#     ('b', 'c'): [4], 
-#     ('a', 'b', 'c', 'd'): [3], 
-#     ('d',): [6], 
-#     ('c', 'd'): [5], 
-#     ('a',): [1]
+#   'a': ['b', 'c', 'd'], 
+#   'b': ['a', 'c', 'd'], 
+#   'c': ['a', 'b', 'd'], 
+#   'd': ['a', 'b', 'c']
 # }
-print(diagram)
+print(euler_boundaries)
 ```
```

