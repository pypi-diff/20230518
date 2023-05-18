# Comparing `tmp/cads_sdk-0.0.18-py3-none-any.whl.zip` & `tmp/cads_sdk-0.0.19-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 55906 bytes, number of entries: 18
--rw-rw-r--  2.0 unx     1265 b- defN 23-May-18 07:36 cads_sdk/__init__.py
+Zip file size: 55896 bytes, number of entries: 18
+-rw-rw-r--  2.0 unx     1265 b- defN 23-May-18 08:24 cads_sdk/__init__.py
 -rw-rw-r--  2.0 unx     1264 b- defN 23-Apr-01 02:59 cads_sdk/nosql/__init__.py
 -rw-rw-r--  2.0 unx    11231 b- defN 23-Apr-17 08:04 cads_sdk/nosql/codec.py
--rw-rw-r--  2.0 unx    87328 b- defN 23-May-18 07:33 cads_sdk/nosql/converter.py
+-rw-rw-r--  2.0 unx    87289 b- defN 23-May-18 08:23 cads_sdk/nosql/converter.py
 -rw-rw-r--  2.0 unx    18968 b- defN 23-May-17 09:34 cads_sdk/nosql/display.py
 -rw-rw-r--  2.0 unx     1187 b- defN 23-Apr-10 10:46 cads_sdk/nosql/etl.py
 -rw-rw-r--  2.0 unx      881 b- defN 23-May-14 04:02 cads_sdk/nosql/utils.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-09 14:03 cads_sdk/petastorm/__init__.py
 -rw-rw-r--  2.0 unx    19967 b- defN 23-Apr-10 04:34 cads_sdk/petastorm/dataset_metadata.py
 -rw-rw-r--  2.0 unx    10508 b- defN 23-Apr-10 07:19 cads_sdk/petastorm/fs_utils.py
 -rw-rw-r--  2.0 unx     5427 b- defN 23-Apr-10 04:42 cads_sdk/petastorm/utils.py
 -rw-rw-r--  2.0 unx    22554 b- defN 23-Apr-18 15:18 cads_sdk/pytorch/__init__.py
 -rw-rw-r--  2.0 unx    10653 b- defN 23-Apr-17 08:05 cads_sdk/pytorch/codec.py
 -rw-rw-r--  2.0 unx    78369 b- defN 23-Apr-20 08:23 cads_sdk/pytorch/converter.py
--rw-rw-r--  2.0 unx     7126 b- defN 23-May-18 07:37 cads_sdk-0.0.18.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-18 07:37 cads_sdk-0.0.18.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-May-18 07:37 cads_sdk-0.0.18.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1479 b- defN 23-May-18 07:37 cads_sdk-0.0.18.dist-info/RECORD
-18 files, 278308 bytes uncompressed, 53500 bytes compressed:  80.8%
+-rw-rw-r--  2.0 unx     7126 b- defN 23-May-18 08:24 cads_sdk-0.0.19.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-18 08:24 cads_sdk-0.0.19.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-May-18 08:24 cads_sdk-0.0.19.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1479 b- defN 23-May-18 08:24 cads_sdk-0.0.19.dist-info/RECORD
+18 files, 278269 bytes uncompressed, 53490 bytes compressed:  80.8%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: cads_sdk/pytorch/codec.py
 Comment: 
 
 Filename: cads_sdk/pytorch/converter.py
 Comment: 
 
-Filename: cads_sdk-0.0.18.dist-info/METADATA
+Filename: cads_sdk-0.0.19.dist-info/METADATA
 Comment: 
 
-Filename: cads_sdk-0.0.18.dist-info/WHEEL
+Filename: cads_sdk-0.0.19.dist-info/WHEEL
 Comment: 
 
-Filename: cads_sdk-0.0.18.dist-info/top_level.txt
+Filename: cads_sdk-0.0.19.dist-info/top_level.txt
 Comment: 
 
-Filename: cads_sdk-0.0.18.dist-info/RECORD
+Filename: cads_sdk-0.0.19.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cads_sdk/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.0.18'
+__version__ = '0.0.19'
 
 __doc__ = """
 cads-sdk: Functions to help Data Scientist work more effectively with unstructured data and datalake
 =====================================================================
 **cads-sdk**
 Function to convert 
 -------------
```

## cads_sdk/nosql/converter.py

```diff
@@ -2043,15 +2043,14 @@
                             database = self.database,
                             numPartition = self.numPartition,
                             compression = self.compression)
             if self.shorten:
                 Schema.__dict__['_fields']['rel_path'] = UnischemaField('rel_path', np.str_, (), ScalarCodec(StringType()), False)
                 Schema.__dict__['rel_path'] = UnischemaField('rel_path', np.str_, (), ScalarCodec(StringType()), False)
             with materialize_dataset(spark, self.output_path, Schema, ROWGROUP_SIZE_MB):
-                print("DEBUG", Schema)
                 print("Write metadata")
         else:
             logging.warn("No files were found, check your input_path")
             
         logging.info("Convert complete")
```

## Comparing `cads_sdk-0.0.18.dist-info/METADATA` & `cads_sdk-0.0.19.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cads-sdk
-Version: 0.0.18
+Version: 0.0.19
 Summary: Function to help Data Scientist work more effectively with DWH
 Home-page: http://git.bigdata.local/data-engineers/sdk/utilities
 Author: duyvnc
 Author-email: duyvnc@fpt.com.vn
 License: duyvnc
 Platform: UNKNOWN
 Requires-Python: >=3.5
```

## Comparing `cads_sdk-0.0.18.dist-info/RECORD` & `cads_sdk-0.0.19.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-cads_sdk/__init__.py,sha256=HI7WMAX9xElE9f47tdMfq4kvoaM6I2v9pDb7LDEASdU,1265
+cads_sdk/__init__.py,sha256=8zDonxJcdicUMyZucsdjzthM40Z7PNpDHc8psCquSOs,1265
 cads_sdk/nosql/__init__.py,sha256=Yu2Zt5cpSXSLqIRAvIxaXOtoyj3yBisGTbnFlH4UD2A,1264
 cads_sdk/nosql/codec.py,sha256=Z0RdndLtSHAnqHOpDGE-Wb_jD9eIWvKiuX4Yj1KudX4,11231
-cads_sdk/nosql/converter.py,sha256=dW0Hghhiqax1dVxJrH3piDwL-_oaaMnbc8qSEqstHAQ,87328
+cads_sdk/nosql/converter.py,sha256=xk5VgzW6z1EzWoDAQZRf1CbjYqVnOOPISth3sV1gb3w,87289
 cads_sdk/nosql/display.py,sha256=lOaFffzd6p5eDIFFoKcw37XgyxhhFVpPkeV_Ipm-DaA,18968
 cads_sdk/nosql/etl.py,sha256=PWhXNWZyIFFEEvTIoUNuKK5cDqTy8A4FPn07BGMr0Vk,1187
 cads_sdk/nosql/utils.py,sha256=avlOSkBze2SWZnF38kdw15i_lHy57EaZ5AhWgK8J1XI,881
 cads_sdk/petastorm/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cads_sdk/petastorm/dataset_metadata.py,sha256=3sXVulFmpZEJC7mM0cwEXBVmB-0TD-U746ltLcsqIno,19967
 cads_sdk/petastorm/fs_utils.py,sha256=qFAzfi_VM4Rr2mBW8JsgxPUojLFFQGZI93MpI4sL_Xo,10508
 cads_sdk/petastorm/utils.py,sha256=CyeRPL_ih9wC1BdElvf1VknF1lBdNvJxgldSiU1OkFs,5427
 cads_sdk/pytorch/__init__.py,sha256=qyLEDZ_2BXLQBqievSj4wg2h4EQf9AdbIi_1SKFyIsM,22554
 cads_sdk/pytorch/codec.py,sha256=5XZulM21El-lsL3jZMexnJAHc2cIeRZj721PMuPhsJU,10653
 cads_sdk/pytorch/converter.py,sha256=lT2c3ix8Q35TEOUdFzlQVIzf7GfRklomwrdfRaXcY7k,78369
-cads_sdk-0.0.18.dist-info/METADATA,sha256=Mr2CqP5dGl3XIadXBsz7cQUF_zs4qNmad3XiYOmzqUs,7126
-cads_sdk-0.0.18.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-cads_sdk-0.0.18.dist-info/top_level.txt,sha256=OaTWVG-YiGPwrATCivDFDqvFPPP_T6y0TYXz8dkujOU,9
-cads_sdk-0.0.18.dist-info/RECORD,,
+cads_sdk-0.0.19.dist-info/METADATA,sha256=Xm_KReNYS2p-tid4KTF4Am_7XivYENFQF2jd8QTMs8k,7126
+cads_sdk-0.0.19.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+cads_sdk-0.0.19.dist-info/top_level.txt,sha256=OaTWVG-YiGPwrATCivDFDqvFPPP_T6y0TYXz8dkujOU,9
+cads_sdk-0.0.19.dist-info/RECORD,,
```

