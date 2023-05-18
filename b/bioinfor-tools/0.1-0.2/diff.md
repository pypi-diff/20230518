# Comparing `tmp/bioinfor_tools-0.1-py3-none-any.whl.zip` & `tmp/bioinfor_tools-0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
 Zip file size: 6283 bytes, number of entries: 8
--rw-r--r--  2.0 unx      488 b- defN 23-Apr-28 06:28 bioinfor_tools/__init__.py
+-rw-r--r--  2.0 unx      488 b- defN 23-May-18 05:52 bioinfor_tools/__init__.py
 -rw-r--r--  2.0 unx      514 b- defN 23-Apr-28 05:56 bioinfor_tools/_bio_basic.py
--rw-r--r--  2.0 unx    10841 b- defN 23-Apr-28 06:43 bioinfor_tools/_cmd_runner.py
+-rw-r--r--  2.0 unx    10842 b- defN 23-May-18 05:51 bioinfor_tools/_cmd_runner.py
 -rw-r--r--  2.0 unx     1292 b- defN 23-Apr-28 05:37 bioinfor_tools/_utils.py
--rw-r--r--  2.0 unx      189 b- defN 23-Apr-28 06:47 bioinfor_tools-0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-28 06:47 bioinfor_tools-0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Apr-28 06:47 bioinfor_tools-0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      651 b- defN 23-Apr-28 06:47 bioinfor_tools-0.1.dist-info/RECORD
-8 files, 14082 bytes uncompressed, 5143 bytes compressed:  63.5%
+-rw-r--r--  2.0 unx      189 b- defN 23-May-18 05:52 bioinfor_tools-0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-18 05:52 bioinfor_tools-0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-May-18 05:52 bioinfor_tools-0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      651 b- defN 23-May-18 05:52 bioinfor_tools-0.2.dist-info/RECORD
+8 files, 14083 bytes uncompressed, 5143 bytes compressed:  63.5%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: bioinfor_tools/_cmd_runner.py
 Comment: 
 
 Filename: bioinfor_tools/_utils.py
 Comment: 
 
-Filename: bioinfor_tools-0.1.dist-info/METADATA
+Filename: bioinfor_tools-0.2.dist-info/METADATA
 Comment: 
 
-Filename: bioinfor_tools-0.1.dist-info/WHEEL
+Filename: bioinfor_tools-0.2.dist-info/WHEEL
 Comment: 
 
-Filename: bioinfor_tools-0.1.dist-info/top_level.txt
+Filename: bioinfor_tools-0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: bioinfor_tools-0.1.dist-info/RECORD
+Filename: bioinfor_tools-0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bioinfor_tools/__init__.py

```diff
@@ -5,15 +5,15 @@
 # @Email : jmzhang1911@gmail.com
 
 import logging
 
 FORMAT = '%(asctime)s %(message)s'
 logging.basicConfig(level=logging.INFO, format=FORMAT, datefmt='%Y-%m-%d %H:%M:%S')
 
-__version__ = 'v0.1 beta'
+__version__ = 'v0.2 beta'
 
 from ._bio_basic import BioBasic
 from ._cmd_runner import CmdRunner as __CmdRunner
 from ._utils import *
 
 cmd_wrapper = __CmdRunner.cmd_wrapper
 cmd = __CmdRunner.cmd
```

## bioinfor_tools/_cmd_runner.py

```diff
@@ -177,15 +177,15 @@
 
             # task_list = []
             # for cmd in cmd_list:
             #     task = executor_cmd.submit(run_shell, cmd)
             #     task_list.append(task)
             futures = [executor_cmd.submit(run_shell, cmd) for cmd in cmd_list]
 
-            if len(futures) >1:
+            if len(futures) >=1:
 
                 done, not_done = wait(futures, return_when=FIRST_EXCEPTION)
                 if len(done) == 1 or len(done) != len(futures):
                     future = list(done)[0]
                     logging.info(future.exception())
                     error_info = f'One task failed with: {future.exception()}, shutting down'
                     for future in futures:
```

## Comparing `bioinfor_tools-0.1.dist-info/RECORD` & `bioinfor_tools-0.2.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-bioinfor_tools/__init__.py,sha256=MLMgScZz6uOgZkZKPfRtihqR8bwR2PD_COZ-102p83U,488
+bioinfor_tools/__init__.py,sha256=EKAppojCr82PVWMBjunoHckscbbc_-aRF6DWOjxTYlc,488
 bioinfor_tools/_bio_basic.py,sha256=iPYdcIBECxQO2K_qvZ8_7o1YEJkG1DYtW0klBhpKWZE,514
-bioinfor_tools/_cmd_runner.py,sha256=AzY09jF180iwkpHJW0OU1Mt1Cb72HK1bKH4mzEAfP1M,10841
+bioinfor_tools/_cmd_runner.py,sha256=ODOiMLf2QR48G3-Ww96isnwNn-s3leESSu7YuzmARsU,10842
 bioinfor_tools/_utils.py,sha256=eDNUgF3TlesPYW40aAQKupn4fEG3PJSBIHEI7F-BQ4c,1292
-bioinfor_tools-0.1.dist-info/METADATA,sha256=COu3A70eh0uxlsbv5CnO6UHmTYuZ6AHhDzlo2-7S_q0,189
-bioinfor_tools-0.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-bioinfor_tools-0.1.dist-info/top_level.txt,sha256=HXy-nag4BdtU9ODJCI6-4ccRu_7p94K8iLU0dqvhSuE,15
-bioinfor_tools-0.1.dist-info/RECORD,,
+bioinfor_tools-0.2.dist-info/METADATA,sha256=8svSe2P9sR4ZMXffVZ-1Neh_vNZnDX7PRCLZx3pVieg,189
+bioinfor_tools-0.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+bioinfor_tools-0.2.dist-info/top_level.txt,sha256=HXy-nag4BdtU9ODJCI6-4ccRu_7p94K8iLU0dqvhSuE,15
+bioinfor_tools-0.2.dist-info/RECORD,,
```

