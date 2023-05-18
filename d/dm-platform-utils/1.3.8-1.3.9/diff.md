# Comparing `tmp/dm_platform_utils-1.3.8-py3-none-any.whl.zip` & `tmp/dm_platform_utils-1.3.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 18089 bytes, number of entries: 12
+Zip file size: 18103 bytes, number of entries: 12
 -rw-r--r--  2.0 unx     4032 b- defN 23-Apr-03 08:07 dm_platform_utils/DataLoader.py
 -rw-r--r--  2.0 unx    19333 b- defN 23-Mar-29 03:31 dm_platform_utils/DataWriter.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-20 09:08 dm_platform_utils/__init__.py
--rw-r--r--  2.0 unx     3480 b- defN 23-Apr-03 11:19 dm_platform_utils/utils.py
+-rw-r--r--  2.0 unx     3508 b- defN 23-Apr-03 11:39 dm_platform_utils/utils.py
 -rw-r--r--  2.0 unx      121 b- defN 23-Mar-20 09:08 dm_platform_utils/conf/process_dtypes.yml
 -rw-r--r--  2.0 unx    11504 b- defN 23-Mar-20 09:08 dm_platform_utils/conf/raw_sql.yml
 -rw-r--r--  2.0 unx     8845 b- defN 23-Apr-03 10:40 dm_platform_utils/conf/sql.yml
--rw-r--r--  2.0 unx     1070 b- defN 23-Apr-03 11:20 dm_platform_utils-1.3.8.dist-info/LICENSE.md
--rw-r--r--  2.0 unx    10532 b- defN 23-Apr-03 11:20 dm_platform_utils-1.3.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-03 11:20 dm_platform_utils-1.3.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 23-Apr-03 11:20 dm_platform_utils-1.3.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1059 b- defN 23-Apr-03 11:20 dm_platform_utils-1.3.8.dist-info/RECORD
-12 files, 60086 bytes uncompressed, 16287 bytes compressed:  72.9%
+-rw-r--r--  2.0 unx     1070 b- defN 23-Apr-03 11:39 dm_platform_utils-1.3.9.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx    10532 b- defN 23-Apr-03 11:39 dm_platform_utils-1.3.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-03 11:39 dm_platform_utils-1.3.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 23-Apr-03 11:39 dm_platform_utils-1.3.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1059 b- defN 23-Apr-03 11:39 dm_platform_utils-1.3.9.dist-info/RECORD
+12 files, 60114 bytes uncompressed, 16301 bytes compressed:  72.9%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: dm_platform_utils/conf/raw_sql.yml
 Comment: 
 
 Filename: dm_platform_utils/conf/sql.yml
 Comment: 
 
-Filename: dm_platform_utils-1.3.8.dist-info/LICENSE.md
+Filename: dm_platform_utils-1.3.9.dist-info/LICENSE.md
 Comment: 
 
-Filename: dm_platform_utils-1.3.8.dist-info/METADATA
+Filename: dm_platform_utils-1.3.9.dist-info/METADATA
 Comment: 
 
-Filename: dm_platform_utils-1.3.8.dist-info/WHEEL
+Filename: dm_platform_utils-1.3.9.dist-info/WHEEL
 Comment: 
 
-Filename: dm_platform_utils-1.3.8.dist-info/top_level.txt
+Filename: dm_platform_utils-1.3.9.dist-info/top_level.txt
 Comment: 
 
-Filename: dm_platform_utils-1.3.8.dist-info/RECORD
+Filename: dm_platform_utils-1.3.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dm_platform_utils/utils.py

```diff
@@ -63,16 +63,16 @@
             else:
                 df.loc[df.index, k] = pd.to_datetime(df[k], format='%Y%m')
         else:
             df.loc[df.index, k] = df[k].astype(eval(v))
     return df
 
 def insert_hbase(df: pd.DataFrame, host: str, port: int, tbl_name:str,
-                 env: str, row_key_cols: list, tbl_struct: dict = None,
-                 family: str = 'INFO'):
+                 env: str, encrypt_cols: list, tbl_struct: dict = None,
+                 family: str = 'INFO', rowkey_col: str = 'uuid'):
     """dataframe写入hbase通用函数
 
     Args:
         df (pd.DataFrame): 输入数据
         host (str): hbase ip
         port (int): hbase 端口
         tbl_name (str): 表名, e.g. "xxx:xxxxx"
@@ -84,22 +84,22 @@
     from easy_db.db import encrypt_df
     from bmai_dm_hbase.hbase_client import HBaseClient
     
     hbase = HBaseClient(host=host, port=port, env=env)
     data = deepcopy(df)
     data = encrypt_df(
         data,
-        row_key_cols
+        encrypt_cols
     )
     raw_cols = data.columns.tolist()
     new_cols = []
     for col in raw_cols:
         if family in col:
             new_cols.append(col)
-        elif col != row_key_cols:
+        elif col != rowkey_col:
             new_cols.append(family + ':' + col)
         else:
             new_cols.append(col)
     data.columns = new_cols
     hbase.build_pool()
     try:
         hbase.scan_tables(tbl_name)
@@ -109,10 +109,10 @@
                 family: dict()
             }
         hbase.create_tbl(tbl_name, tbl_struct)
     hbase.build_pool()
     hbase.insert_df(
         table_name=tbl_name,
         df=data,
-        rowkeys_col='uuid'
+        rowkeys_col=rowkey_col
     )
     print('Inserting hbase successfully.')
```

## Comparing `dm_platform_utils-1.3.8.dist-info/LICENSE.md` & `dm_platform_utils-1.3.9.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `dm_platform_utils-1.3.8.dist-info/METADATA` & `dm_platform_utils-1.3.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dm-platform-utils
-Version: 1.3.8
+Version: 1.3.9
 Summary: Data mining platform develop utils
 Home-page: http://gitlab.admin.bluemoon.com.cn/DM_group/dm-platform-utils.git
 Author: Shenxian Shi
 Author-email: shishenxian@bluemoon.com.cn
 License: MIT License        
         Copyright 2022 Bluemoon Algorithm        
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:        
@@ -309,14 +309,14 @@
 
 2023-03-21 # v1.2.0
 1. 新增get_raw_data & insert_hbase
 
 2023-3-25 # v1.2.2
 1. insert_hbase新增查表逻辑，首次查表自动建表
    
-2023-3-29 # v1.3.0 ~ # v1.3.8
+2023-3-29 # v1.3.0 ~ # v1.3.9
 1. 修改取数表
 2. 新增事件反馈列表接口请求 & 事件反馈进度编辑接口请求
 3. 修改header配置方式，在每个接口调用函数中进行更新
 4. utils新增hbase通用插数
```

## Comparing `dm_platform_utils-1.3.8.dist-info/RECORD` & `dm_platform_utils-1.3.9.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 dm_platform_utils/DataLoader.py,sha256=JNsoSOexGf4uxDw5-_MGbe3P9IusT-E1_QxNidNGtVY,4032
 dm_platform_utils/DataWriter.py,sha256=wrKlIjvU3Uw4ryHoA2T3zeiopg3ygdOHHTGo2FKD3f4,19333
 dm_platform_utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-dm_platform_utils/utils.py,sha256=TNnbTBaKdwO5PqnhBXZ0_PknljBMokTSe2V-bm-2rKc,3480
+dm_platform_utils/utils.py,sha256=tRQj_fXH5S443fbNJv5cZ9b595p8k0WuYJxV0dLp2Zk,3508
 dm_platform_utils/conf/process_dtypes.yml,sha256=vuK5-ILZdU9aWb1mm3shfFcYqSpbqZ69WXOIpN4zjc0,121
 dm_platform_utils/conf/raw_sql.yml,sha256=_RtsHzvTEPsAcqDQWaPcoFg9NNLEjkQLMfrmeTPHs8w,11504
 dm_platform_utils/conf/sql.yml,sha256=PaX71_UlnrOV-HTrVwfHbj5mwrxWywSBZJvV_r8txD0,8845
-dm_platform_utils-1.3.8.dist-info/LICENSE.md,sha256=nj4YRBXV2kr3Hbf_kHWvVZKidLs1TqpOg6L5mOUBWww,1070
-dm_platform_utils-1.3.8.dist-info/METADATA,sha256=TojWvA3n2rV4jROs0TWaGjYYyDN0XEBwwSzsKSPtulE,10532
-dm_platform_utils-1.3.8.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-dm_platform_utils-1.3.8.dist-info/top_level.txt,sha256=x4dT2gnq16hZPgHsM7FZe8j8TeWhMjFmSERC_kb4TNc,18
-dm_platform_utils-1.3.8.dist-info/RECORD,,
+dm_platform_utils-1.3.9.dist-info/LICENSE.md,sha256=nj4YRBXV2kr3Hbf_kHWvVZKidLs1TqpOg6L5mOUBWww,1070
+dm_platform_utils-1.3.9.dist-info/METADATA,sha256=zizPERQQgYZN7zL0_VqO47vzk5tMsrHWTjFDAJ0fX_k,10532
+dm_platform_utils-1.3.9.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+dm_platform_utils-1.3.9.dist-info/top_level.txt,sha256=x4dT2gnq16hZPgHsM7FZe8j8TeWhMjFmSERC_kb4TNc,18
+dm_platform_utils-1.3.9.dist-info/RECORD,,
```

