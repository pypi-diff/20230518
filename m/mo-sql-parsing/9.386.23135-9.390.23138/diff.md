# Comparing `tmp/mo_sql_parsing-9.386.23135-py2.py3-none-any.whl.zip` & `tmp/mo_sql_parsing-9.390.23138-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 38297 bytes, number of entries: 13
+Zip file size: 38303 bytes, number of entries: 13
 -rw-rw-rw-  2.0 fat     2597 b- defN 22-Dec-18 22:41 mo_sql_parsing/__init__.py
--rw-rw-rw-  2.0 fat    22407 b- defN 23-May-15 22:26 mo_sql_parsing/formatting.py
+-rw-rw-rw-  2.0 fat    22427 b- defN 23-May-18 01:33 mo_sql_parsing/formatting.py
 -rw-rw-rw-  2.0 fat    10666 b- defN 23-May-03 23:07 mo_sql_parsing/keywords.py
 -rw-rw-rw-  2.0 fat    33444 b- defN 23-May-15 22:26 mo_sql_parsing/sql_parser.py
 -rw-rw-rw-  2.0 fat     7321 b- defN 23-Mar-26 12:53 mo_sql_parsing/types.py
 -rw-rw-rw-  2.0 fat    22999 b- defN 23-May-15 22:26 mo_sql_parsing/utils.py
 -rw-rw-rw-  2.0 fat     2987 b- defN 23-Mar-26 12:53 mo_sql_parsing/windows.py
--rw-rw-rw-  2.0 fat    15922 b- defN 23-May-15 22:26 mo_sql_parsing-9.386.23135.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     9345 b- defN 23-May-15 22:26 mo_sql_parsing-9.386.23135.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-May-15 22:26 mo_sql_parsing-9.386.23135.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-May-15 22:26 mo_sql_parsing-9.386.23135.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-May-15 22:26 mo_sql_parsing-9.386.23135.dist-info/zip-safe
-?rw-rw-r--  2.0 fat     1134 b- defN 23-May-15 22:26 mo_sql_parsing-9.386.23135.dist-info/RECORD
-13 files, 128949 bytes uncompressed, 36391 bytes compressed:  71.8%
+-rw-rw-rw-  2.0 fat    15922 b- defN 23-May-18 01:33 mo_sql_parsing-9.390.23138.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     9345 b- defN 23-May-18 01:33 mo_sql_parsing-9.390.23138.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-May-18 01:33 mo_sql_parsing-9.390.23138.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 23-May-18 01:33 mo_sql_parsing-9.390.23138.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-May-18 01:33 mo_sql_parsing-9.390.23138.dist-info/zip-safe
+?rw-rw-r--  2.0 fat     1134 b- defN 23-May-18 01:33 mo_sql_parsing-9.390.23138.dist-info/RECORD
+13 files, 128969 bytes uncompressed, 36397 bytes compressed:  71.8%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: mo_sql_parsing/utils.py
 Comment: 
 
 Filename: mo_sql_parsing/windows.py
 Comment: 
 
-Filename: mo_sql_parsing-9.386.23135.dist-info/LICENSE
+Filename: mo_sql_parsing-9.390.23138.dist-info/LICENSE
 Comment: 
 
-Filename: mo_sql_parsing-9.386.23135.dist-info/METADATA
+Filename: mo_sql_parsing-9.390.23138.dist-info/METADATA
 Comment: 
 
-Filename: mo_sql_parsing-9.386.23135.dist-info/WHEEL
+Filename: mo_sql_parsing-9.390.23138.dist-info/WHEEL
 Comment: 
 
-Filename: mo_sql_parsing-9.386.23135.dist-info/top_level.txt
+Filename: mo_sql_parsing-9.390.23138.dist-info/top_level.txt
 Comment: 
 
-Filename: mo_sql_parsing-9.386.23135.dist-info/zip-safe
+Filename: mo_sql_parsing-9.390.23138.dist-info/zip-safe
 Comment: 
 
-Filename: mo_sql_parsing-9.386.23135.dist-info/RECORD
+Filename: mo_sql_parsing-9.390.23138.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mo_sql_parsing/formatting.py

```diff
@@ -306,15 +306,15 @@
             else:
                 return f"({method(value, op_prec)})"
 
         # treat as regular function call
         if isinstance(value, dict) and len(value) == 0:
             return key.upper() + "()"  # NOT SURE IF AN EMPTY dict SHOULD BE DELT WITH HERE, OR IN self.format()
         else:
-            params = ", ".join(self.dispatch(p) for p in listwrap(value))
+            params = ", ".join(self.dispatch(p, precedence["from"]) for p in listwrap(value))
             return f"{key.upper()}({params})"
 
     def _binary_not(self, value, prec):
         return "~{0}".format(self.dispatch(value))
 
     def _not(self, value, prec):
         op_prec = precedence["not"]
```

## Comparing `mo_sql_parsing-9.386.23135.dist-info/LICENSE` & `mo_sql_parsing-9.390.23138.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mo_sql_parsing-9.386.23135.dist-info/METADATA` & `mo_sql_parsing-9.390.23138.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-sql-parsing
-Version: 9.386.23135
+Version: 9.390.23138
 Summary: More SQL Parsing! Parse SQL into JSON parse tree
 Home-page: https://github.com/klahnakoski/mo-sql-parsing
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Software Development :: Libraries
```

## Comparing `mo_sql_parsing-9.386.23135.dist-info/RECORD` & `mo_sql_parsing-9.390.23138.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 mo_sql_parsing/__init__.py,sha256=qu67hMKaz6Rn_c0idUNZ9e_BvFuxXsDZRuwQmmGYqpI,2597
-mo_sql_parsing/formatting.py,sha256=nWP7KfL5rSPdpuyEugHW9LT0-iqwJY91ueGcDd5dQaA,22407
+mo_sql_parsing/formatting.py,sha256=suxoyUZ-8Tq6r4p5zX3yXycumkBIKUIDGfchYIgRdAA,22427
 mo_sql_parsing/keywords.py,sha256=4huuey_x1Q2ervkRWMqj4woMsmmSlDDCFhKCViN5jDs,10666
 mo_sql_parsing/sql_parser.py,sha256=3I88hSICoXxIkLOty_OM7NMgmcdM8AJw32DUV-X5GG4,33444
 mo_sql_parsing/types.py,sha256=4nnewHeuD_q3W7muesXsSS4JW73TM17YgBjlxQkOfpo,7321
 mo_sql_parsing/utils.py,sha256=1vVp9zi1uqq04Y9K0Y4yAfrqMyPhyXr7U06s4NXiqrc,22999
 mo_sql_parsing/windows.py,sha256=DNYTT34qFS8lfaDEg4oXigmYoSA72_LyHLgIQjBSpWI,2987
-mo_sql_parsing-9.386.23135.dist-info/LICENSE,sha256=YCIsKMGn9qksffmOXF9EWeYk5uKF4Lm5RGevX2qzND0,15922
-mo_sql_parsing-9.386.23135.dist-info/METADATA,sha256=QR0p3gIRiV1s5Bti_Sm-rg-Apb-nDuAv28r7BoXNWLU,9345
-mo_sql_parsing-9.386.23135.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-mo_sql_parsing-9.386.23135.dist-info/top_level.txt,sha256=P9tODVsRxMEL1jG7yBYiLD3rRo_rjSKa_r-F6cbnfgA,15
-mo_sql_parsing-9.386.23135.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-mo_sql_parsing-9.386.23135.dist-info/RECORD,,
+mo_sql_parsing-9.390.23138.dist-info/LICENSE,sha256=YCIsKMGn9qksffmOXF9EWeYk5uKF4Lm5RGevX2qzND0,15922
+mo_sql_parsing-9.390.23138.dist-info/METADATA,sha256=NMKgydsPpwqg7RHldJpWgoPLiFWgPan8dJvSMP2q1uc,9345
+mo_sql_parsing-9.390.23138.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+mo_sql_parsing-9.390.23138.dist-info/top_level.txt,sha256=P9tODVsRxMEL1jG7yBYiLD3rRo_rjSKa_r-F6cbnfgA,15
+mo_sql_parsing-9.390.23138.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
+mo_sql_parsing-9.390.23138.dist-info/RECORD,,
```

