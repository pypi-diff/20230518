# Comparing `tmp/comgen-0.0.11-py3-none-any.whl.zip` & `tmp/comgen-0.0.12-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 58106 bytes, number of entries: 14
+Zip file size: 58104 bytes, number of entries: 14
 -rw-r--r--  2.0 unx      158 b- defN 23-Feb-01 19:52 comgen/__init__.py
 -rw-r--r--  2.0 unx     5212 b- defN 23-Feb-22 22:42 comgen/species.py
 -rw-r--r--  2.0 unx     1355 b- defN 23-Feb-01 20:44 comgen/util.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Feb-01 16:24 comgen/constraintsystems/__init__.py
 -rw-r--r--  2.0 unx     1673 b- defN 23-Feb-01 20:46 comgen/constraintsystems/base.py
--rw-r--r--  2.0 unx    21851 b- defN 23-Feb-24 16:03 comgen/constraintsystems/ionic.py
+-rw-r--r--  2.0 unx    21853 b- defN 23-Feb-24 16:13 comgen/constraintsystems/ionic.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Feb-01 16:24 comgen/data/__init__.py
 -rw-r--r--  2.0 unx      522 b- defN 22-Sep-05 09:26 comgen/data/common_poly_ions.txt
 -rw-r--r--  2.0 unx     2121 b- defN 23-Feb-01 20:45 comgen/data/data.py
 -rw-r--r--  2.0 unx   241638 b- defN 22-Jun-24 15:04 comgen/data/periodic_table.json
--rw-r--r--  2.0 unx      169 b- defN 23-Feb-24 16:07 comgen-0.0.11.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-24 16:07 comgen-0.0.11.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Feb-24 16:07 comgen-0.0.11.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1116 b- defN 23-Feb-24 16:07 comgen-0.0.11.dist-info/RECORD
-14 files, 275914 bytes uncompressed, 56254 bytes compressed:  79.6%
+-rw-r--r--  2.0 unx      169 b- defN 23-Feb-24 16:24 comgen-0.0.12.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Feb-24 16:24 comgen-0.0.12.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Feb-24 16:24 comgen-0.0.12.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1116 b- defN 23-Feb-24 16:24 comgen-0.0.12.dist-info/RECORD
+14 files, 275916 bytes uncompressed, 56252 bytes compressed:  79.6%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: comgen/data/data.py
 Comment: 
 
 Filename: comgen/data/periodic_table.json
 Comment: 
 
-Filename: comgen-0.0.11.dist-info/METADATA
+Filename: comgen-0.0.12.dist-info/METADATA
 Comment: 
 
-Filename: comgen-0.0.11.dist-info/WHEEL
+Filename: comgen-0.0.12.dist-info/WHEEL
 Comment: 
 
-Filename: comgen-0.0.11.dist-info/top_level.txt
+Filename: comgen-0.0.12.dist-info/top_level.txt
 Comment: 
 
-Filename: comgen-0.0.11.dist-info/RECORD
+Filename: comgen-0.0.12.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## comgen/constraintsystems/ionic.py

```diff
@@ -255,15 +255,15 @@
 		cons = []
 		for multiplier in range(1, ub+1):
 			and_cons = []
 			for el_label, q in Element_Quantities.items():
 				and_cons.append(q * int(multiplier) == Element_Integer_Quantities[el_label])
 			cons.append(And(*and_cons))
 
-		return Or(*cons)
+		return [Or(*cons)]
 
 	@staticmethod
 	def sum_of_quantities_constraints(
 		Element_Quantities: dict, 
 	    bounds: tuple) -> list:
 		"""
 		This should only be used when Element_Quantities variables are Integer types.
```

## Comparing `comgen-0.0.11.dist-info/RECORD` & `comgen-0.0.12.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 comgen/__init__.py,sha256=5yrjNO_BrorhE6_KwKPXQkCFm9Xu0rVNEPjBx2nClPM,158
 comgen/species.py,sha256=F5SYUxwoM8GKCTqyfgh4f9zU2iiZOnl8BEP8VtWqd4g,5212
 comgen/util.py,sha256=SEx3HCG3bpxuU4a52ZlsRf5LJKJmExTKwladm-7buDk,1355
 comgen/constraintsystems/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 comgen/constraintsystems/base.py,sha256=FFd-R3SwIVBSTgTvva7YcLCPCzrqjUxCyuW-QMPYeuY,1673
-comgen/constraintsystems/ionic.py,sha256=Yu4udyd_YIDmsZYwNQnok_1kH1k7S9pNqfMR5xv_xZY,21851
+comgen/constraintsystems/ionic.py,sha256=WMzQD7CsC91dtBOpb-4cAm-MbnSX7qZbnLzzMniJVzs,21853
 comgen/data/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 comgen/data/common_poly_ions.txt,sha256=9-7baAy05X_x3nxoyZeRUwf1HBBdJJzJin6VHfcnAGE,522
 comgen/data/data.py,sha256=37-PY_XMgWmgXzWbCuSjYcR5Ubx48TnCOrU3bCHzGyQ,2121
 comgen/data/periodic_table.json,sha256=t6IcFRYoPDdfDjS1O8ufG5MKx-ARq_KPntTrqvDpjnU,241638
-comgen-0.0.11.dist-info/METADATA,sha256=wL6PocvPpVVmR5HseEl_pjb9W_797hMWJyV4AQhoMEQ,169
-comgen-0.0.11.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-comgen-0.0.11.dist-info/top_level.txt,sha256=mJIuYGYcA0BymZYLiwhgfqFrN2P9ypMSbjnfjiWr1Kk,7
-comgen-0.0.11.dist-info/RECORD,,
+comgen-0.0.12.dist-info/METADATA,sha256=3OeSRBXqHqV-ZRiF-Lsz8H_lqy_Q9x2Xp7cvZE1ZHlg,169
+comgen-0.0.12.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+comgen-0.0.12.dist-info/top_level.txt,sha256=mJIuYGYcA0BymZYLiwhgfqFrN2P9ypMSbjnfjiWr1Kk,7
+comgen-0.0.12.dist-info/RECORD,,
```

