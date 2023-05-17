# Comparing `tmp/loanpy-3.0.0.tar.gz` & `tmp/loanpy-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loanpy-3.0.0.tar", last modified: Thu May  4 19:32:41 2023, max compression
+gzip compressed data, was "loanpy-3.0.1.tar", last modified: Wed May 17 22:08:27 2023, max compression
```

## Comparing `loanpy-3.0.0.tar` & `loanpy-3.0.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2023-05-04 19:32:41.701367 loanpy-3.0.0/
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     1066 2023-04-16 19:03:02.000000 loanpy-3.0.0/LICENSE
--rw-rw-r--   0 viktor    (1000) viktor    (1000)       20 2023-04-26 13:54:21.000000 loanpy-3.0.0/MANIFEST.in
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     4890 2023-05-04 19:32:41.701367 loanpy-3.0.0/PKG-INFO
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     3222 2023-05-04 19:19:00.000000 loanpy-3.0.0/README.rst
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2023-05-04 19:32:41.701367 loanpy-3.0.0/loanpy/
--rw-rw-r--   0 viktor    (1000) viktor    (1000)        0 2023-04-24 21:01:57.000000 loanpy-3.0.0/loanpy/__init__.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     8247 2023-04-27 23:30:23.000000 loanpy-3.0.0/loanpy/eval_sca.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)   435389 2023-04-25 21:27:41.000000 loanpy-3.0.0/loanpy/ipa_all.csv
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     6845 2023-05-04 18:49:25.000000 loanpy-3.0.0/loanpy/loanfinder.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)    37335 2023-05-03 17:44:27.000000 loanpy-3.0.0/loanpy/scapplier.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     9260 2023-04-27 23:29:00.000000 loanpy-3.0.0/loanpy/scminer.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)    23190 2023-04-27 23:28:10.000000 loanpy-3.0.0/loanpy/utils.py
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2023-05-04 19:32:41.701367 loanpy-3.0.0/loanpy.egg-info/
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     4890 2023-05-04 19:32:41.000000 loanpy-3.0.0/loanpy.egg-info/PKG-INFO
--rw-rw-r--   0 viktor    (1000) viktor    (1000)      643 2023-05-04 19:32:41.000000 loanpy-3.0.0/loanpy.egg-info/SOURCES.txt
--rw-rw-r--   0 viktor    (1000) viktor    (1000)        1 2023-05-04 19:32:41.000000 loanpy-3.0.0/loanpy.egg-info/dependency_links.txt
--rw-rw-r--   0 viktor    (1000) viktor    (1000)       64 2023-05-04 19:32:41.000000 loanpy-3.0.0/loanpy.egg-info/requires.txt
--rw-rw-r--   0 viktor    (1000) viktor    (1000)        7 2023-05-04 19:32:41.000000 loanpy-3.0.0/loanpy.egg-info/top_level.txt
--rw-rw-r--   0 viktor    (1000) viktor    (1000)      210 2023-05-04 19:32:41.701367 loanpy-3.0.0/setup.cfg
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     1956 2023-05-04 19:32:24.000000 loanpy-3.0.0/setup.py
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2023-05-04 19:32:41.701367 loanpy-3.0.0/tests/
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     5427 2023-04-25 17:53:13.000000 loanpy-3.0.0/tests/test_eval_sca_integration.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     3576 2023-04-25 23:59:23.000000 loanpy-3.0.0/tests/test_eval_sca_unit.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)      660 2023-04-23 22:13:44.000000 loanpy-3.0.0/tests/test_loanfinder_integration.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     1680 2023-04-23 22:13:26.000000 loanpy-3.0.0/tests/test_loanfinder_unit.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)    12621 2023-04-25 23:59:22.000000 loanpy-3.0.0/tests/test_scapplier_integration.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)    27616 2023-04-25 23:59:22.000000 loanpy-3.0.0/tests/test_scapplier_unit.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     1727 2023-04-16 19:03:02.000000 loanpy-3.0.0/tests/test_scminer_integration.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     6820 2023-04-25 23:59:23.000000 loanpy-3.0.0/tests/test_scminer_unit.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     3482 2023-04-25 21:48:43.000000 loanpy-3.0.0/tests/test_utils_integration.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)    11626 2023-04-25 22:18:49.000000 loanpy-3.0.0/tests/test_utils_unit.py
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2023-05-17 22:08:27.587864 loanpy-3.0.1/
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     1066 2023-04-16 19:03:02.000000 loanpy-3.0.1/LICENSE
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)       20 2023-04-26 13:54:21.000000 loanpy-3.0.1/MANIFEST.in
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     4890 2023-05-17 22:08:27.587864 loanpy-3.0.1/PKG-INFO
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     3222 2023-05-04 19:19:00.000000 loanpy-3.0.1/README.rst
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2023-05-17 22:08:27.587864 loanpy-3.0.1/loanpy/
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)        0 2023-04-24 21:01:57.000000 loanpy-3.0.1/loanpy/__init__.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     8355 2023-05-17 21:41:29.000000 loanpy-3.0.1/loanpy/eval_sca.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)   435389 2023-04-25 21:27:41.000000 loanpy-3.0.1/loanpy/ipa_all.csv
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     6845 2023-05-17 21:37:27.000000 loanpy-3.0.1/loanpy/loanfinder.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)    37335 2023-05-03 17:44:27.000000 loanpy-3.0.1/loanpy/scapplier.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     9260 2023-04-27 23:29:00.000000 loanpy-3.0.1/loanpy/scminer.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)    23190 2023-04-27 23:28:10.000000 loanpy-3.0.1/loanpy/utils.py
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2023-05-17 22:08:27.587864 loanpy-3.0.1/loanpy.egg-info/
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     4890 2023-05-17 22:08:27.000000 loanpy-3.0.1/loanpy.egg-info/PKG-INFO
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)      643 2023-05-17 22:08:27.000000 loanpy-3.0.1/loanpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)        1 2023-05-17 22:08:27.000000 loanpy-3.0.1/loanpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)       64 2023-05-17 22:08:27.000000 loanpy-3.0.1/loanpy.egg-info/requires.txt
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)        7 2023-05-17 22:08:27.000000 loanpy-3.0.1/loanpy.egg-info/top_level.txt
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)      210 2023-05-17 22:08:27.587864 loanpy-3.0.1/setup.cfg
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     1956 2023-05-17 22:07:15.000000 loanpy-3.0.1/setup.py
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2023-05-17 22:08:27.587864 loanpy-3.0.1/tests/
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     5427 2023-04-25 17:53:13.000000 loanpy-3.0.1/tests/test_eval_sca_integration.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     5117 2023-05-17 21:53:28.000000 loanpy-3.0.1/tests/test_eval_sca_unit.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)      660 2023-04-23 22:13:44.000000 loanpy-3.0.1/tests/test_loanfinder_integration.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     1680 2023-04-23 22:13:26.000000 loanpy-3.0.1/tests/test_loanfinder_unit.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)    12621 2023-04-25 23:59:22.000000 loanpy-3.0.1/tests/test_scapplier_integration.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)    27616 2023-04-25 23:59:22.000000 loanpy-3.0.1/tests/test_scapplier_unit.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     1727 2023-04-16 19:03:02.000000 loanpy-3.0.1/tests/test_scminer_integration.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     6820 2023-04-25 23:59:23.000000 loanpy-3.0.1/tests/test_scminer_unit.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     3482 2023-04-25 21:48:43.000000 loanpy-3.0.1/tests/test_utils_integration.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)    11626 2023-04-25 22:18:49.000000 loanpy-3.0.1/tests/test_utils_unit.py
```

### Comparing `loanpy-3.0.0/LICENSE` & `loanpy-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `loanpy-3.0.0/PKG-INFO` & `loanpy-3.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loanpy
-Version: 3.0.0
+Version: 3.0.1
 Summary: a linguistic toolkit for detecting old loanwords by predicting,evaluating and applying changes in horizontal and vertical lexical transfers
 Home-page: https://github.com/martino-vic/loanpy
 Download-URL: https://github.com/LoanpyDataHub/loanpy/archive/3.0.0.tar.gz
 Author: Viktor Martinović
 Author-email: viktor_martinovic@eva.mpg.de
 License: MIT
 Project-URL: documentation, https://loanpy.readthedocs.io/en/latest/home.html
```

### Comparing `loanpy-3.0.0/README.rst` & `loanpy-3.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `loanpy-3.0.0/loanpy/eval_sca.py` & `loanpy-3.0.1/loanpy/eval_sca.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,16 +179,19 @@
         src = srcrow[h["ALIGNMENT"]]   # define left-outs as test input
         tgt = "".join(re.sub("[-. ]", "", tgtrow[h["ALIGNMENT"]]))
         src_pros = srcrow[h["PROSODY"]] if pros else ""
         adrc = Adrc()   # initiate adapt-reconstruct class
         adrc.set_sc(get_correspondences(intable, heur))  # extract info from traing data
         adrc.set_prosodic_inventory(get_prosodic_inventory(intable))  # extract prosodic_inventory
         if adapt:
-            ad = adrc.adapt(src, howmany, src_pros)
-            out.append(tgt in ad)
+            try:
+                ad = adrc.adapt(src, howmany, src_pros)
+                out.append(tgt in ad)
+            except KeyError:  # bugfix issue #50
+                out.append(False)
         else:
             rc = adrc.reconstruct(src, howmany)
             out.append(bool(re.match(rc, tgt)))
         intable.insert(i, tgtrow)
         intable.insert(i, srcrow)
 
     return round(len([i for i in out if i]) / len(out), 2)
```

### Comparing `loanpy-3.0.0/loanpy/ipa_all.csv` & `loanpy-3.0.1/loanpy/ipa_all.csv`

 * *Files identical despite different names*

### Comparing `loanpy-3.0.0/loanpy/loanfinder.py` & `loanpy-3.0.1/loanpy/loanfinder.py`

 * *Files identical despite different names*

### Comparing `loanpy-3.0.0/loanpy/scapplier.py` & `loanpy-3.0.1/loanpy/scapplier.py`

 * *Files identical despite different names*

### Comparing `loanpy-3.0.0/loanpy/scminer.py` & `loanpy-3.0.1/loanpy/scminer.py`

 * *Files identical despite different names*

### Comparing `loanpy-3.0.0/loanpy/utils.py` & `loanpy-3.0.1/loanpy/utils.py`

 * *Files identical despite different names*

### Comparing `loanpy-3.0.0/loanpy.egg-info/PKG-INFO` & `loanpy-3.0.1/loanpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loanpy
-Version: 3.0.0
+Version: 3.0.1
 Summary: a linguistic toolkit for detecting old loanwords by predicting,evaluating and applying changes in horizontal and vertical lexical transfers
 Home-page: https://github.com/martino-vic/loanpy
 Download-URL: https://github.com/LoanpyDataHub/loanpy/archive/3.0.0.tar.gz
 Author: Viktor Martinović
 Author-email: viktor_martinovic@eva.mpg.de
 License: MIT
 Project-URL: documentation, https://loanpy.readthedocs.io/en/latest/home.html
```

### Comparing `loanpy-3.0.0/loanpy.egg-info/SOURCES.txt` & `loanpy-3.0.1/loanpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `loanpy-3.0.0/setup.py` & `loanpy-3.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 setup(
   name='loanpy',
   description='a linguistic toolkit for detecting old loanwords by predicting,\
 evaluating and applying changes in horizontal and vertical lexical transfers',
   long_description=open("README.rst").read(),
   author='Viktor Martinović',
   author_email='viktor_martinovic@eva.mpg.de',
-  version='3.0.0',
+  version='3.0.1',
   packages=find_packages(),
   data_files=[("loanpy", ["loanpy/ipa_all.csv"])],
   include_package_data=True,
   extras_require={
   "test": ["pytest>=7.1.2", "coverage>=7.2.2"],
   "dev": ["wheel", "twine", "sphinx"]
   },
```

### Comparing `loanpy-3.0.0/tests/test_eval_sca_integration.py` & `loanpy-3.0.1/tests/test_eval_sca_integration.py`

 * *Files identical despite different names*

### Comparing `loanpy-3.0.0/tests/test_eval_sca_unit.py` & `loanpy-3.0.1/tests/test_eval_sca_unit.py`

 * *Files 22% similar despite different names*

```diff
@@ -62,14 +62,52 @@
     assert adrc_monkey.adapt_called_with == [['#aː t͡ʃ# -#', 2, "VC"],
                                             ['#aː ɟ uː#', 2, "VCV"]
                                             ]
     get_correspondences_mock.assert_called_with(intable, heuristic)
     get_prosodic_inventory_mock.assert_called_with(intable)
     assert not adrc_monkey.init_called_with
 
+#same as before but make adapt raise a keyerror
+adrc_monkey2 = AdrcMonkey()
+def raise_keyerror(*args):
+    print("here")
+    adrc_monkey2.adapt_called_with.append([*args])
+    raise KeyError("Raising a KeyError from this mock function")
+adrc_monkey2.adapt = raise_keyerror
+@patch("loanpy.eval_sca.Adrc", side_effect=[adrc_monkey2, adrc_monkey2])
+@patch("loanpy.eval_sca.get_correspondences")
+@patch("loanpy.eval_sca.get_prosodic_inventory")
+def test_eval_one_adapt_keyerror(get_prosodic_inventory_mock, get_correspondences_mock, adrc_mock):
+    # define patched functions' return value
+    get_prosodic_inventory_mock.return_value = 321
+    get_correspondences_mock.return_value = 123
+    # define input variables
+    intable = [  ['ID', 'COGID', 'DOCULECT', 'ALIGNMENT', 'PROSODY'],
+  ['0', '1', 'H', '#aː t͡ʃ# -#', 'VC'],
+  ['1', '1', 'EAH', 'a.ɣ.a t͡ʃ i', 'VCVCV'],
+  ['2', '2', 'H', '#aː ɟ uː#', 'VCV'],
+  ['3', '2', 'EAH', 'a l.d a.ɣ', 'VCCVC']
+]
+    heuristic = "some_heuristic"
+    adapt = True
+    howmany = 2
+    pros = True
+
+    # assert results
+    result = eval_one(intable, heuristic, adapt, howmany, pros)
+    assert result == 0.0
+
+    # assert calls
+    assert adrc_monkey2.adapt_called_with == [['#aː t͡ʃ# -#', 2, "VC"],
+                                            ['#aː ɟ uː#', 2, "VCV"]
+                                            ]
+    get_correspondences_mock.assert_called_with(intable, heuristic)
+    get_prosodic_inventory_mock.assert_called_with(intable)
+    assert not adrc_monkey2.init_called_with
+
 adrc_monkey2 = AdrcMonkey()
 @patch("loanpy.eval_sca.Adrc", side_effect=[adrc_monkey2, adrc_monkey2])
 @patch("loanpy.eval_sca.get_correspondences")
 @patch("loanpy.eval_sca.get_prosodic_inventory")
 @patch("loanpy.eval_sca.re.match")
 def test_eval_one_reconstruct(match_mock, get_prosodic_inventory_mock, get_correspondences_mock, adrc_mock):
     match_mock.return_value = 111
```

### Comparing `loanpy-3.0.0/tests/test_loanfinder_integration.py` & `loanpy-3.0.1/tests/test_loanfinder_integration.py`

 * *Files identical despite different names*

### Comparing `loanpy-3.0.0/tests/test_loanfinder_unit.py` & `loanpy-3.0.1/tests/test_loanfinder_unit.py`

 * *Files identical despite different names*

### Comparing `loanpy-3.0.0/tests/test_scapplier_integration.py` & `loanpy-3.0.1/tests/test_scapplier_integration.py`

 * *Files identical despite different names*

### Comparing `loanpy-3.0.0/tests/test_scapplier_unit.py` & `loanpy-3.0.1/tests/test_scapplier_unit.py`

 * *Files identical despite different names*

### Comparing `loanpy-3.0.0/tests/test_scminer_integration.py` & `loanpy-3.0.1/tests/test_scminer_integration.py`

 * *Files identical despite different names*

### Comparing `loanpy-3.0.0/tests/test_scminer_unit.py` & `loanpy-3.0.1/tests/test_scminer_unit.py`

 * *Files identical despite different names*

### Comparing `loanpy-3.0.0/tests/test_utils_integration.py` & `loanpy-3.0.1/tests/test_utils_integration.py`

 * *Files identical despite different names*

### Comparing `loanpy-3.0.0/tests/test_utils_unit.py` & `loanpy-3.0.1/tests/test_utils_unit.py`

 * *Files identical despite different names*

