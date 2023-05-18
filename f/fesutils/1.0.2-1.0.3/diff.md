# Comparing `tmp/fesutils-1.0.2-py3-none-any.whl.zip` & `tmp/fesutils-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,25 +1,25 @@
-Zip file size: 27244 bytes, number of entries: 23
--rw-r--r--  2.0 unx     1083 b- defN 22-Nov-29 16:30 fesutils/__init__.py
+Zip file size: 27256 bytes, number of entries: 23
+-rw-r--r--  2.0 unx     1083 b- defN 23-May-18 05:16 fesutils/__init__.py
 -rw-r--r--  2.0 unx     1153 b- defN 20-Mar-11 04:59 fesutils/_cmdutils.py
 -rw-r--r--  2.0 unx     3473 b- defN 21-Jun-04 10:02 fesutils/_containerutils.py
 -rw-r--r--  2.0 unx      647 b- defN 20-Mar-02 11:21 fesutils/_err_msg.py
 -rw-r--r--  2.0 unx     6838 b- defN 20-Mar-02 10:26 fesutils/_oidutils.py
 -rw-r--r--  2.0 unx     1066 b- defN 20-Mar-02 11:15 fesutils/_poolutils.py
--rw-r--r--  2.0 unx     2800 b- defN 20-Oct-16 07:28 fesutils/_strutils.py
+-rw-r--r--  2.0 unx     2864 b- defN 23-May-18 05:26 fesutils/_strutils.py
 -rw-r--r--  2.0 unx     4607 b- defN 20-Sep-03 07:37 fesutils/_timeparse.py
 -rw-r--r--  2.0 unx     3082 b- defN 21-Feb-25 09:16 fesutils/_wraputils.py
 -rw-r--r--  2.0 unx     1637 b- defN 20-Mar-02 11:23 fesutils/err.py
 -rw-r--r--  2.0 unx      761 b- defN 20-Sep-03 08:27 fesutils/parseutils.py
 -rw-r--r--  2.0 unx     3698 b- defN 20-Sep-03 07:18 fesutils/schedutils.py
 -rw-r--r--  2.0 unx      271 b- defN 20-Mar-06 04:09 fesutils/cacheutils/__init__.py
 -rw-r--r--  2.0 unx    10870 b- defN 20-Sep-03 08:27 fesutils/cacheutils/_cachelru.py
 -rw-r--r--  2.0 unx     3936 b- defN 22-Nov-29 16:29 fesutils/cacheutils/_cacheutils.py
 -rw-r--r--  2.0 unx      300 b- defN 20-Sep-03 08:15 fesutils/schemautils/__init__.py
 -rw-r--r--  2.0 unx     2648 b- defN 20-Mar-14 12:07 fesutils/schemautils/_fields.py
 -rw-r--r--  2.0 unx    16923 b- defN 20-Sep-03 08:13 fesutils/schemautils/_schemautils.py
--rw-r--r--  2.0 unx     1066 b- defN 22-Nov-29 16:33 fesutils-1.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1105 b- defN 22-Nov-29 16:33 fesutils-1.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Nov-29 16:33 fesutils-1.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 22-Nov-29 16:33 fesutils-1.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1865 b- defN 22-Nov-29 16:33 fesutils-1.0.2.dist-info/RECORD
-23 files, 69930 bytes uncompressed, 24244 bytes compressed:  65.3%
+-rw-r--r--  2.0 unx     1066 b- defN 23-May-18 05:28 fesutils-1.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1105 b- defN 23-May-18 05:28 fesutils-1.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-18 05:28 fesutils-1.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-May-18 05:28 fesutils-1.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1865 b- defN 23-May-18 05:28 fesutils-1.0.3.dist-info/RECORD
+23 files, 69994 bytes uncompressed, 24256 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -48,23 +48,23 @@
 
 Filename: fesutils/schemautils/_fields.py
 Comment: 
 
 Filename: fesutils/schemautils/_schemautils.py
 Comment: 
 
-Filename: fesutils-1.0.2.dist-info/LICENSE
+Filename: fesutils-1.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: fesutils-1.0.2.dist-info/METADATA
+Filename: fesutils-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: fesutils-1.0.2.dist-info/WHEEL
+Filename: fesutils-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: fesutils-1.0.2.dist-info/top_level.txt
+Filename: fesutils-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: fesutils-1.0.2.dist-info/RECORD
+Filename: fesutils-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fesutils/__init__.py

```diff
@@ -36,8 +36,8 @@
     "gmt2time", "ymd2time", "time2gmt", "time2ymd", "iso2time", "time2iso", "stamp2time", "time2stamp",
 
     "expand_nested_list", "is_iterable", "chunked", "chunked_iter",
 
     "__version__",
 )
 
-__version__ = "1.0.2"
+__version__ = "1.0.3"
```

## fesutils/_strutils.py

```diff
@@ -7,14 +7,15 @@
 @time: 2020/3/2 下午6:36
 """
 import hashlib
 import re
 import secrets
 import string
 import uuid
+from decimal import Decimal
 from typing import Union
 
 __all__ = ("gen_ident", "gen_unique_ident", "camel2under", "under2camel", "number", "str2md5")
 
 _camel2under_re = re.compile('((?<=[a-z0-9])[A-Z]|(?!^)[A-Z](?=[a-z]))')
 
 
@@ -59,24 +60,24 @@
 
     >>> under2camel('complex_tokenizer')
     'ComplexTokenizer'
     """
     return ''.join(w.capitalize() or '_' for w in under_string.split('_'))
 
 
-def number(str_value: str, default: Union[int, float] = 0) -> Union[int, float]:
+def number(str_value: str, default: Union[int, float, Decimal] = 0) -> Union[int, float, Decimal]:
     """
     把字符串值转换为int或者float
     Args:
         str_value: 需要转换的字符串值
         default: 转换失败的默认值,默认值只能为Number类型,默认为0
     Returns:
 
     """
-    default = default if isinstance(default, (int, float)) else 0
+    default = default if isinstance(default, (int, float, Decimal)) else 0
     if isinstance(str_value, str):
         number_value: Union[int, float] = default  # 先赋予默认值
         # 处理有符号的整数和小数
         if str_value.startswith(("-", "+")):
             if str_value[1:].isdecimal():
                 number_value = int(str_value)
             elif str_value[1:].replace(".", "").isdecimal():
@@ -85,15 +86,15 @@
         elif str_value.isdecimal():
             number_value = int(str_value)
         # 处理无符号的小数
         elif str_value.replace(".", "").isdecimal():
             number_value = float(str_value)
 
         return number_value
-    elif isinstance(str_value, (int, float)):
+    elif isinstance(str_value, (int, float, Decimal)):
         return str_value
     else:
         return default
 
 
 def str2md5(content: str):
     """
```

## Comparing `fesutils-1.0.2.dist-info/LICENSE` & `fesutils-1.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fesutils-1.0.2.dist-info/METADATA` & `fesutils-1.0.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fesutils
-Version: 1.0.2
+Version: 1.0.3
 Summary: 常用工具方法库
 Home-page: https://github.com/tinybees/fesutils
 Author: TinyBees
 Author-email: a598824322@qq.com
 License: MIT
 Keywords: utils
 Platform: UNKNOWN
```

## Comparing `fesutils-1.0.2.dist-info/RECORD` & `fesutils-1.0.3.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-fesutils/__init__.py,sha256=t1gnY6T-j_ZGw7IJq2UN8AuFW3zKum01wIB0A2NeaJ8,1083
+fesutils/__init__.py,sha256=Q5Zl23yh-npIEHGT_0yaGdJO5mnnIpp001KKSHo-WWY,1083
 fesutils/_cmdutils.py,sha256=WIuY2XXG474quzJoX0eUoB279uy0pfMbC6dp2h8Eyk8,1153
 fesutils/_containerutils.py,sha256=Q8Synj-55kfB-_1XuSfd-joSzngLAARJnWo4USUP1YU,3473
 fesutils/_err_msg.py,sha256=WuyzF_xU6s3sMCaCEbK1efjueb6QpQz2VOvt-7ek4PE,647
 fesutils/_oidutils.py,sha256=uvkWNx2wuYv5WYag1kAH1CqyTdbHzIW5pXT9GGgK30Q,6838
 fesutils/_poolutils.py,sha256=K8J4TkrxTj2LK9kIWwUmwJnOOS0BMGPNuVVoP6m0SOA,1066
-fesutils/_strutils.py,sha256=THE1rPSD7HIq913fSkYNgN1TvMd6nn2266X-RveV3qg,2800
+fesutils/_strutils.py,sha256=Zgo7SDJIL9DaRWd--puj2xhKpbd10t4H9T1kNRmo1I4,2864
 fesutils/_timeparse.py,sha256=cBm5619Zm_d2CgJ6b-A7sGkIo90reCaZo_6IZ3YEf_4,4607
 fesutils/_wraputils.py,sha256=5G3eN2968cc_uo7Ye0de8oMZGbJtJjHIuNW1d9HmPOY,3082
 fesutils/err.py,sha256=4v0m4Svdf5bLs5ueVGCLd2p6VJrBFI1FXaLiGqSL17A,1637
 fesutils/parseutils.py,sha256=DdboBvFFnt8mOLWTwRUhZAalTvMAx6iEG2Qr6nuu_NQ,761
 fesutils/schedutils.py,sha256=9CNw1SSCXgeUXXXoYQKoHeCjSjZ8GVg3At7m6Cpqksg,3698
 fesutils/cacheutils/__init__.py,sha256=8TNKtCUdXKB7VXtChpd2j-n1Sc94LYgcutFzu7BYbk0,271
 fesutils/cacheutils/_cachelru.py,sha256=spbZJnByYZ2fsRcgEzeSzCZ_1oJSsjj6F66Ia5gF_Qg,10870
 fesutils/cacheutils/_cacheutils.py,sha256=ztSCSvnUCriekokLChRiCSAkKqg33Sk5YGK7R8dvqow,3936
 fesutils/schemautils/__init__.py,sha256=DtaVDbaPapLfdhVSnfZcT6LfGQ56fMCwBY9TeXEfbyw,300
 fesutils/schemautils/_fields.py,sha256=xpB6fj-PKPyBI1brS9KLJ0WdNDI23KZBkxlQHI9sNHc,2648
 fesutils/schemautils/_schemautils.py,sha256=FskseDYUoJrA8J4EPLm8N__f0CcjWqnHmKar1GRgL6I,16923
-fesutils-1.0.2.dist-info/LICENSE,sha256=TWwJMCl9W3NMEJQVyefTtObKkavZbw16Rcoq-Ez7WvU,1066
-fesutils-1.0.2.dist-info/METADATA,sha256=YYKMYegztxJJCFV4lEQC-Gs3SjFEMz6QgsTtRHqMuME,1105
-fesutils-1.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-fesutils-1.0.2.dist-info/top_level.txt,sha256=Hsm84--n30fV9LT8Q77U2m07qVg3iDKd4LzCgoGILcY,9
-fesutils-1.0.2.dist-info/RECORD,,
+fesutils-1.0.3.dist-info/LICENSE,sha256=TWwJMCl9W3NMEJQVyefTtObKkavZbw16Rcoq-Ez7WvU,1066
+fesutils-1.0.3.dist-info/METADATA,sha256=klGlMlP2Qi44_Xwyn8tQyllHMps85OLWrco6GdDDVfU,1105
+fesutils-1.0.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+fesutils-1.0.3.dist-info/top_level.txt,sha256=Hsm84--n30fV9LT8Q77U2m07qVg3iDKd4LzCgoGILcY,9
+fesutils-1.0.3.dist-info/RECORD,,
```

