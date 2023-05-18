# Comparing `tmp/dftrans-2.0.2.5.tar.gz` & `tmp/dftrans-2.0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dftrans-2.0.2.5.tar", last modified: Wed May 10 13:56:13 2023, max compression
+gzip compressed data, was "dftrans-2.0.2.6.tar", last modified: Thu May 18 02:31:29 2023, max compression
```

## Comparing `dftrans-2.0.2.5.tar` & `dftrans-2.0.2.6.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 13:56:13.637893 dftrans-2.0.2.5/
-drwxrwxrwx   0        0        0        0 2023-05-10 13:56:13.634893 dftrans-2.0.2.5/DFTrans.egg-info/
--rw-rw-rw-   0        0        0      307 2023-05-10 13:56:13.000000 dftrans-2.0.2.5/DFTrans.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      577 2023-05-10 13:56:13.000000 dftrans-2.0.2.5/DFTrans.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 13:56:13.000000 dftrans-2.0.2.5/DFTrans.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-05-10 13:56:13.000000 dftrans-2.0.2.5/DFTrans.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      284 2023-05-10 13:56:13.000000 dftrans-2.0.2.5/DFTrans.egg-info/requires.txt
--rw-rw-rw-   0        0        0       80 2023-05-10 13:56:13.000000 dftrans-2.0.2.5/DFTrans.egg-info/top_level.txt
--rw-rw-rw-   0        0        0   315088 2023-05-10 13:54:55.000000 dftrans-2.0.2.5/DFTrans_main.py
--rw-rw-rw-   0        0        0      307 2023-05-10 13:56:13.636892 dftrans-2.0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0      175 2023-04-18 13:45:30.000000 dftrans-2.0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 13:56:13.608887 dftrans-2.0.2.5/config/
-drwxrwxrwx   0        0        0        0 2023-05-10 13:56:13.628891 dftrans-2.0.2.5/config/DFTrans/
--rw-rw-rw-   0        0        0   162264 2023-04-18 13:07:06.000000 dftrans-2.0.2.5/config/DFTrans/DFTrans_config.json
-drwxrwxrwx   0        0        0        0 2023-05-10 13:56:13.631891 dftrans-2.0.2.5/config/img/
--rw-rw-rw-   0        0        0    42148 2023-03-08 01:46:58.000000 dftrans-2.0.2.5/config/img/table_arrow9_transparent_256.png
--rw-rw-rw-   0        0        0    16958 2023-03-08 01:46:58.000000 dftrans-2.0.2.5/config/img/table_arrow9_transparent_64.ico
--rw-rw-rw-   0        0        0   208159 2023-05-10 13:53:28.000000 dftrans-2.0.2.5/df_excel_define.py
--rw-rw-rw-   0        0        0     3418 2023-04-06 04:23:37.000000 dftrans-2.0.2.5/df_excel_define_user.py
--rw-rw-rw-   0        0        0    17037 2023-04-18 14:54:25.000000 dftrans-2.0.2.5/df_excel_plot.py
--rw-rw-rw-   0        0        0     7706 2023-04-18 13:30:39.000000 dftrans-2.0.2.5/df_stock_define.py
--rw-rw-rw-   0        0        0       42 2023-05-10 13:56:13.637893 dftrans-2.0.2.5/setup.cfg
--rw-rw-rw-   0        0        0     6380 2023-05-10 13:55:20.000000 dftrans-2.0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 02:31:29.241868 dftrans-2.0.2.6/
+drwxrwxrwx   0        0        0        0 2023-05-18 02:31:29.238868 dftrans-2.0.2.6/DFTrans.egg-info/
+-rw-rw-rw-   0        0        0      330 2023-05-18 02:31:29.000000 dftrans-2.0.2.6/DFTrans.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      585 2023-05-18 02:31:29.000000 dftrans-2.0.2.6/DFTrans.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 02:31:29.000000 dftrans-2.0.2.6/DFTrans.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-05-18 02:31:29.000000 dftrans-2.0.2.6/DFTrans.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      284 2023-05-18 02:31:29.000000 dftrans-2.0.2.6/DFTrans.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       80 2023-05-18 02:31:29.000000 dftrans-2.0.2.6/DFTrans.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0   315088 2023-05-10 13:54:55.000000 dftrans-2.0.2.6/DFTrans_main.py
+-rw-rw-rw-   0        0        0     1539 2023-05-18 01:57:46.000000 dftrans-2.0.2.6/LICENSE
+-rw-rw-rw-   0        0        0      330 2023-05-18 02:31:29.240868 dftrans-2.0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1431 2023-05-18 01:35:35.000000 dftrans-2.0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 02:31:29.208861 dftrans-2.0.2.6/config/
+drwxrwxrwx   0        0        0        0 2023-05-18 02:31:29.230867 dftrans-2.0.2.6/config/DFTrans/
+-rw-rw-rw-   0        0        0   162264 2023-04-18 13:07:06.000000 dftrans-2.0.2.6/config/DFTrans/DFTrans_config.json
+drwxrwxrwx   0        0        0        0 2023-05-18 02:31:29.234867 dftrans-2.0.2.6/config/img/
+-rw-rw-rw-   0        0        0    42148 2023-03-08 01:46:58.000000 dftrans-2.0.2.6/config/img/table_arrow9_transparent_256.png
+-rw-rw-rw-   0        0        0    16958 2023-03-08 01:46:58.000000 dftrans-2.0.2.6/config/img/table_arrow9_transparent_64.ico
+-rw-rw-rw-   0        0        0   208159 2023-05-10 13:53:28.000000 dftrans-2.0.2.6/df_excel_define.py
+-rw-rw-rw-   0        0        0     3418 2023-04-06 04:23:37.000000 dftrans-2.0.2.6/df_excel_define_user.py
+-rw-rw-rw-   0        0        0    17037 2023-04-18 14:54:25.000000 dftrans-2.0.2.6/df_excel_plot.py
+-rw-rw-rw-   0        0        0     7706 2023-04-18 13:30:39.000000 dftrans-2.0.2.6/df_stock_define.py
+-rw-rw-rw-   0        0        0       42 2023-05-18 02:31:29.241868 dftrans-2.0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     6380 2023-05-18 02:30:46.000000 dftrans-2.0.2.6/setup.py
```

### Comparing `dftrans-2.0.2.5/DFTrans.egg-info/SOURCES.txt` & `dftrans-2.0.2.6/DFTrans.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 DFTrans_main.py
+LICENSE
 README.md
 df_excel_define.py
 df_excel_define_user.py
 df_excel_plot.py
 df_stock_define.py
 setup.py
 DFTrans.egg-info/PKG-INFO
```

### Comparing `dftrans-2.0.2.5/DFTrans_main.py` & `dftrans-2.0.2.6/DFTrans_main.py`

 * *Files identical despite different names*

### Comparing `dftrans-2.0.2.5/config/DFTrans/DFTrans_config.json` & `dftrans-2.0.2.6/config/DFTrans/DFTrans_config.json`

 * *Files identical despite different names*

### Comparing `dftrans-2.0.2.5/config/img/table_arrow9_transparent_256.png` & `dftrans-2.0.2.6/config/img/table_arrow9_transparent_256.png`

 * *Files identical despite different names*

### Comparing `dftrans-2.0.2.5/config/img/table_arrow9_transparent_64.ico` & `dftrans-2.0.2.6/config/img/table_arrow9_transparent_64.ico`

 * *Files identical despite different names*

### Comparing `dftrans-2.0.2.5/df_excel_define.py` & `dftrans-2.0.2.6/df_excel_define.py`

 * *Files identical despite different names*

### Comparing `dftrans-2.0.2.5/df_excel_define_user.py` & `dftrans-2.0.2.6/df_excel_define_user.py`

 * *Files identical despite different names*

### Comparing `dftrans-2.0.2.5/df_excel_plot.py` & `dftrans-2.0.2.6/df_excel_plot.py`

 * *Files identical despite different names*

### Comparing `dftrans-2.0.2.5/df_stock_define.py` & `dftrans-2.0.2.6/df_stock_define.py`

 * *Files identical despite different names*

### Comparing `dftrans-2.0.2.5/setup.py` & `dftrans-2.0.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,15 +156,15 @@
 000009b0: 6e66 6967 6469 722c 205b 6f72 6769 6e63  nfigdir, [orginc
 000009c0: 6f6e 6669 6766 696c 655d 292c 0d0a 2020  onfigfile]),..  
 000009d0: 2020 2020 2020 5d0d 0a20 2020 2072 6574        ]..    ret
 000009e0: 7572 6e20 6461 7461 5f66 696c 6573 0d0a  urn data_files..
 000009f0: 0d0a 0d0a 7365 7475 7028 0d0a 2020 2020  ....setup(..    
 00000a00: 6e61 6d65 3d27 6466 7472 616e 7327 2c0d  name='dftrans',.
 00000a10: 0a20 2020 2076 6572 7369 6f6e 3d27 322e  .    version='2.
-00000a20: 302e 322e 3527 2c0d 0a20 2020 2064 6573  0.2.5',..    des
+00000a20: 302e 322e 3627 2c0d 0a20 2020 2064 6573  0.2.6',..    des
 00000a30: 6372 6970 7469 6f6e 3d27 e794 a8e4 ba8e  cription='......
 00000a40: e689 b9e9 878f e5a4 84e7 9086 6578 6365  ............exce
 00000a50: 6ce3 8081 7371 6ce6 95b0 e68d aee5 ba93  l...sql.........
 00000a60: e8a1 a8e3 8081 6a73 6f6e 6ce3 8081 6373  ......jsonl...cs
 00000a70: 76e7 ad89 e695 b0e6 8dae e6ba 90e7 9a84  v...............
 00000a80: e696 87e4 bbb6 efbc 8ce5 b9b6 e8be 93e5  ................
 00000a90: 87ba e588 b0e6 95b0 e68d aee5 ba93 e8a1  ................
@@ -178,15 +178,15 @@
 00000b10: 2829 2c20 2020 2020 2020 2023 20e8 a1a8  (),        # ...
 00000b20: e7a4 bae4 bda0 e8a6 81e5 b081 e8a3 85e7  ................
 00000b30: 9a84 e58c 85ef bc8c 6669 6e64 5f70 6163  ........find_pac
 00000b40: 6b61 6765 73e7 94a8 e4ba 8ee7 b3bb e7bb  kages...........
 00000b50: 9fe8 87aa e58a a8e4 bb8e e5bd 93e5 898d  ................
 00000b60: e79b aee5 bd95 e5bc 80e5 a78b e689 bee5  ................
 00000b70: 8c85 0d0a 2020 2020 6c69 6365 6e73 653d  ....    license=
-00000b80: 224d 4954 222c 0d0a 2020 2020 7572 6c3d  "MIT",..    url=
+00000b80: 2242 5344 222c 0d0a 2020 2020 7572 6c3d  "BSD",..    url=
 00000b90: 2768 7474 7073 3a2f 2f67 6974 6565 2e63  'https://gitee.c
 00000ba0: 6f6d 2f46 7261 6e6b 5f35 3833 3938 3337  om/Frank_5839837
 00000bb0: 3136 2f64 6674 7261 6e73 272c 0d0a 2020  16/dftrans',..  
 00000bc0: 2020 7079 5f6d 6f64 756c 6573 3d5b 2744    py_modules=['D
 00000bd0: 4654 7261 6e73 5f6d 6169 6e27 2c20 2764  FTrans_main', 'd
 00000be0: 665f 6578 6365 6c5f 6465 6669 6e65 272c  f_excel_define',
 00000bf0: 2027 6466 5f65 7863 656c 5f64 6566 696e   'df_excel_defin
```

