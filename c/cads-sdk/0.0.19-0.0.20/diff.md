# Comparing `tmp/cads_sdk-0.0.19-py3-none-any.whl.zip` & `tmp/cads_sdk-0.0.20-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 55896 bytes, number of entries: 18
--rw-rw-r--  2.0 unx     1265 b- defN 23-May-18 08:24 cads_sdk/__init__.py
+Zip file size: 55942 bytes, number of entries: 18
+-rw-rw-r--  2.0 unx     1265 b- defN 23-May-18 09:04 cads_sdk/__init__.py
 -rw-rw-r--  2.0 unx     1264 b- defN 23-Apr-01 02:59 cads_sdk/nosql/__init__.py
 -rw-rw-r--  2.0 unx    11231 b- defN 23-Apr-17 08:04 cads_sdk/nosql/codec.py
--rw-rw-r--  2.0 unx    87289 b- defN 23-May-18 08:23 cads_sdk/nosql/converter.py
+-rw-rw-r--  2.0 unx    86938 b- defN 23-May-18 09:04 cads_sdk/nosql/converter.py
 -rw-rw-r--  2.0 unx    18968 b- defN 23-May-17 09:34 cads_sdk/nosql/display.py
 -rw-rw-r--  2.0 unx     1187 b- defN 23-Apr-10 10:46 cads_sdk/nosql/etl.py
--rw-rw-r--  2.0 unx      881 b- defN 23-May-14 04:02 cads_sdk/nosql/utils.py
+-rw-rw-r--  2.0 unx     1199 b- defN 23-May-18 08:43 cads_sdk/nosql/utils.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-09 14:03 cads_sdk/petastorm/__init__.py
 -rw-rw-r--  2.0 unx    19967 b- defN 23-Apr-10 04:34 cads_sdk/petastorm/dataset_metadata.py
 -rw-rw-r--  2.0 unx    10508 b- defN 23-Apr-10 07:19 cads_sdk/petastorm/fs_utils.py
 -rw-rw-r--  2.0 unx     5427 b- defN 23-Apr-10 04:42 cads_sdk/petastorm/utils.py
 -rw-rw-r--  2.0 unx    22554 b- defN 23-Apr-18 15:18 cads_sdk/pytorch/__init__.py
 -rw-rw-r--  2.0 unx    10653 b- defN 23-Apr-17 08:05 cads_sdk/pytorch/codec.py
 -rw-rw-r--  2.0 unx    78369 b- defN 23-Apr-20 08:23 cads_sdk/pytorch/converter.py
--rw-rw-r--  2.0 unx     7126 b- defN 23-May-18 08:24 cads_sdk-0.0.19.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-18 08:24 cads_sdk-0.0.19.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-May-18 08:24 cads_sdk-0.0.19.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1479 b- defN 23-May-18 08:24 cads_sdk-0.0.19.dist-info/RECORD
-18 files, 278269 bytes uncompressed, 53490 bytes compressed:  80.8%
+-rw-rw-r--  2.0 unx     7126 b- defN 23-May-18 09:04 cads_sdk-0.0.20.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-18 09:04 cads_sdk-0.0.20.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-May-18 09:04 cads_sdk-0.0.20.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1480 b- defN 23-May-18 09:04 cads_sdk-0.0.20.dist-info/RECORD
+18 files, 278237 bytes uncompressed, 53536 bytes compressed:  80.8%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: cads_sdk/pytorch/codec.py
 Comment: 
 
 Filename: cads_sdk/pytorch/converter.py
 Comment: 
 
-Filename: cads_sdk-0.0.19.dist-info/METADATA
+Filename: cads_sdk-0.0.20.dist-info/METADATA
 Comment: 
 
-Filename: cads_sdk-0.0.19.dist-info/WHEEL
+Filename: cads_sdk-0.0.20.dist-info/WHEEL
 Comment: 
 
-Filename: cads_sdk-0.0.19.dist-info/top_level.txt
+Filename: cads_sdk-0.0.20.dist-info/top_level.txt
 Comment: 
 
-Filename: cads_sdk-0.0.19.dist-info/RECORD
+Filename: cads_sdk-0.0.20.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cads_sdk/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.0.19'
+__version__ = '0.0.20'
 
 __doc__ = """
 cads-sdk: Functions to help Data Scientist work more effectively with unstructured data and datalake
 =====================================================================
 **cads-sdk**
 Function to convert 
 -------------
```

## cads_sdk/nosql/converter.py

```diff
@@ -27,15 +27,15 @@
 from petastorm.etl.dataset_metadata import materialize_dataset
 
 import warnings
 warnings.simplefilter(action='ignore', category=FutureWarning)
 
 from cads_sdk.nosql.codec import *
 from cads_sdk.nosql.etl import read_mp3,read_pcm,padding
-from cads_sdk.nosql.utils import get_size_of_dir,get_size_of_list,check_delta
+from cads_sdk.nosql.utils import get_size_of_dir,get_size_of_list,check_delta,replace_special_characters
 
 class ConvertFromFolder:
     def __init__(
         self,
         input_path,
         input_type,
         output_path,
@@ -203,17 +203,17 @@
                 .mode('overwrite') \
                 .option("path", output_path) \
                 .saveAsTable(database + '.' + table_name)
         
         if file_format == 'delta':
             if self.shorten:
                 logging.info("OPTIMIZE")
-                #ss.sql(f"""
-                #OPTIMIZE delta.`{output_path}` ZORDER BY(rel_path)
-                #""")
+                ss.sql(f"""
+                OPTIMIZE delta.`{output_path}` ZORDER BY(rel_path)
+                """)
             logging.info("VACUUM")
             ss.sql(f"""
             VACUUM delta.`{output_path}` RETAIN 0 HOURS
             """)
 
 
 class ConvertFromFolderImage(ConvertFromFolder):
@@ -450,31 +450,23 @@
         if not self.resize_mode:
             logging.warning(f"Not resize image, If get size error try to turn resize_mode='padding' or resize_mode='resize'")
         if self.shorten:
             return spark.createDataFrame(spark_df.rdd.mapPartitions(self.row_generator), Schema.as_spark_schema()).withColumn("rel_path", expr(f"""replace(path, '{self.commonpath}', '') """))
         else:
             return spark.createDataFrame(spark_df.rdd.mapPartitions(self.row_generator), Schema.as_spark_schema())
     
-    def replace_special_characters(self, txt: str):
-        if self.debug:
-            print(txt)
-        for i in range(56527, 56576):
-            txt = txt.replace(chr(i).encode('unicode_escape').decode('utf-8'), chr(i))
-        for i in range(7840, 7930):
-            txt = txt.replace(chr(i).encode('unicode_escape').decode('utf-8'), chr(i))
-        return txt
     
     def row_generator(self, partitionData):
         """Returns a dict of row input to rdd spark dataframe"""
         for row in partitionData:
             path = row.path
             if self.debug:
                 print(f"Convert Image {path}") #, file=self.log_file)
-                print(self.replace_special_characters(path))
-            path = self.replace_special_characters(path)
+                print(replace_special_characters(path))
+            path = replace_special_characters(path)
             try:
                 img = Image.open(path)
             except Exception as e:
                 print(e)
                 print(path)
                 img = None
             if type(img).__name__ != "NoneType":
```

## cads_sdk/nosql/utils.py

```diff
@@ -14,21 +14,28 @@
         for entry in it:
             if entry.is_file():
                 total += entry.stat().st_size
             elif entry.is_dir():
                 total += get_size_of_dir(entry.path)
     return total
 
+def replace_special_characters(txt: str):
+    for i in range(56527, 56576):
+        txt = txt.replace(chr(i).encode('unicode_escape').decode('utf-8'), chr(i))
+    for i in range(7840, 7930):
+        txt = txt.replace(chr(i).encode('unicode_escape').decode('utf-8'), chr(i))
+    return txt
+
 def get_all_file_of_dir(path):
     total = []
     with os.scandir(path) as it:
         for entry in it:
             if entry.is_file():
                 total.append(entry.path)
             elif entry.is_dir():
                 total.extend(get_all_file_of_dir(entry.path))
     return total
 
 
 def get_size_of_list(input_files):
-    total = sum([os.stat(path).st_size for path in input_files])
+    total = sum([os.stat(replace_special_characters(path)).st_size for path in input_files])
     return total
```

## Comparing `cads_sdk-0.0.19.dist-info/METADATA` & `cads_sdk-0.0.20.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cads-sdk
-Version: 0.0.19
+Version: 0.0.20
 Summary: Function to help Data Scientist work more effectively with DWH
 Home-page: http://git.bigdata.local/data-engineers/sdk/utilities
 Author: duyvnc
 Author-email: duyvnc@fpt.com.vn
 License: duyvnc
 Platform: UNKNOWN
 Requires-Python: >=3.5
```

## Comparing `cads_sdk-0.0.19.dist-info/RECORD` & `cads_sdk-0.0.20.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-cads_sdk/__init__.py,sha256=8zDonxJcdicUMyZucsdjzthM40Z7PNpDHc8psCquSOs,1265
+cads_sdk/__init__.py,sha256=X8nqmAOslfWH-4rurdH9Edv9qZR6RqnuesFcrMU4lyk,1265
 cads_sdk/nosql/__init__.py,sha256=Yu2Zt5cpSXSLqIRAvIxaXOtoyj3yBisGTbnFlH4UD2A,1264
 cads_sdk/nosql/codec.py,sha256=Z0RdndLtSHAnqHOpDGE-Wb_jD9eIWvKiuX4Yj1KudX4,11231
-cads_sdk/nosql/converter.py,sha256=xk5VgzW6z1EzWoDAQZRf1CbjYqVnOOPISth3sV1gb3w,87289
+cads_sdk/nosql/converter.py,sha256=TUVOQIEqE60zpoxZbyc9fcgaFOVkYy37ZmwtBVG8LoI,86938
 cads_sdk/nosql/display.py,sha256=lOaFffzd6p5eDIFFoKcw37XgyxhhFVpPkeV_Ipm-DaA,18968
 cads_sdk/nosql/etl.py,sha256=PWhXNWZyIFFEEvTIoUNuKK5cDqTy8A4FPn07BGMr0Vk,1187
-cads_sdk/nosql/utils.py,sha256=avlOSkBze2SWZnF38kdw15i_lHy57EaZ5AhWgK8J1XI,881
+cads_sdk/nosql/utils.py,sha256=Qbumcpi4m7eSwVOZGoF6NDN6_AqW1NtQ0ECwNziXSms,1199
 cads_sdk/petastorm/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cads_sdk/petastorm/dataset_metadata.py,sha256=3sXVulFmpZEJC7mM0cwEXBVmB-0TD-U746ltLcsqIno,19967
 cads_sdk/petastorm/fs_utils.py,sha256=qFAzfi_VM4Rr2mBW8JsgxPUojLFFQGZI93MpI4sL_Xo,10508
 cads_sdk/petastorm/utils.py,sha256=CyeRPL_ih9wC1BdElvf1VknF1lBdNvJxgldSiU1OkFs,5427
 cads_sdk/pytorch/__init__.py,sha256=qyLEDZ_2BXLQBqievSj4wg2h4EQf9AdbIi_1SKFyIsM,22554
 cads_sdk/pytorch/codec.py,sha256=5XZulM21El-lsL3jZMexnJAHc2cIeRZj721PMuPhsJU,10653
 cads_sdk/pytorch/converter.py,sha256=lT2c3ix8Q35TEOUdFzlQVIzf7GfRklomwrdfRaXcY7k,78369
-cads_sdk-0.0.19.dist-info/METADATA,sha256=Xm_KReNYS2p-tid4KTF4Am_7XivYENFQF2jd8QTMs8k,7126
-cads_sdk-0.0.19.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-cads_sdk-0.0.19.dist-info/top_level.txt,sha256=OaTWVG-YiGPwrATCivDFDqvFPPP_T6y0TYXz8dkujOU,9
-cads_sdk-0.0.19.dist-info/RECORD,,
+cads_sdk-0.0.20.dist-info/METADATA,sha256=AnMblL5nhlxK5hxCXxdYHdI2v7HddKIsRYjai59-BuY,7126
+cads_sdk-0.0.20.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+cads_sdk-0.0.20.dist-info/top_level.txt,sha256=OaTWVG-YiGPwrATCivDFDqvFPPP_T6y0TYXz8dkujOU,9
+cads_sdk-0.0.20.dist-info/RECORD,,
```

