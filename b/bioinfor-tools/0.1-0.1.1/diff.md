# Comparing `tmp/bioinfor_tools-0.1-py3-none-any.whl.zip` & `tmp/bioinfor_tools-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 6283 bytes, number of entries: 8
--rw-r--r--  2.0 unx      488 b- defN 23-Apr-28 06:28 bioinfor_tools/__init__.py
+Zip file size: 6305 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      490 b- defN 23-May-18 06:02 bioinfor_tools/__init__.py
 -rw-r--r--  2.0 unx      514 b- defN 23-Apr-28 05:56 bioinfor_tools/_bio_basic.py
--rw-r--r--  2.0 unx    10841 b- defN 23-Apr-28 06:43 bioinfor_tools/_cmd_runner.py
+-rw-r--r--  2.0 unx    10894 b- defN 23-May-18 06:01 bioinfor_tools/_cmd_runner.py
 -rw-r--r--  2.0 unx     1292 b- defN 23-Apr-28 05:37 bioinfor_tools/_utils.py
--rw-r--r--  2.0 unx      189 b- defN 23-Apr-28 06:47 bioinfor_tools-0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-28 06:47 bioinfor_tools-0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Apr-28 06:47 bioinfor_tools-0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      651 b- defN 23-Apr-28 06:47 bioinfor_tools-0.1.dist-info/RECORD
-8 files, 14082 bytes uncompressed, 5143 bytes compressed:  63.5%
+-rw-r--r--  2.0 unx      191 b- defN 23-May-18 06:02 bioinfor_tools-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-18 06:02 bioinfor_tools-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-May-18 06:02 bioinfor_tools-0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      659 b- defN 23-May-18 06:02 bioinfor_tools-0.1.1.dist-info/RECORD
+8 files, 14147 bytes uncompressed, 5149 bytes compressed:  63.6%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: bioinfor_tools/_cmd_runner.py
 Comment: 
 
 Filename: bioinfor_tools/_utils.py
 Comment: 
 
-Filename: bioinfor_tools-0.1.dist-info/METADATA
+Filename: bioinfor_tools-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: bioinfor_tools-0.1.dist-info/WHEEL
+Filename: bioinfor_tools-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: bioinfor_tools-0.1.dist-info/top_level.txt
+Filename: bioinfor_tools-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: bioinfor_tools-0.1.dist-info/RECORD
+Filename: bioinfor_tools-0.1.1.dist-info/RECORD
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
+__version__ = 'v0.1.1 beta'
 
 from ._bio_basic import BioBasic
 from ._cmd_runner import CmdRunner as __CmdRunner
 from ._utils import *
 
 cmd_wrapper = __CmdRunner.cmd_wrapper
 cmd = __CmdRunner.cmd
```

## bioinfor_tools/_cmd_runner.py

```diff
@@ -1,8 +1,8 @@
-from concurrent.futures import ThreadPoolExecutor, wait, FIRST_EXCEPTION
+from concurrent.futures import ThreadPoolExecutor, wait, FIRST_EXCEPTION, as_completed
 import bioinfor_tools._utils as _utils
 from ._bio_basic import BioBasic
 from threading import Event
 from pathlib import Path
 import subprocess
 import functools
 import datetime
@@ -171,40 +171,43 @@
 
             cmd_list = cmd_qsub_list
 
         with ThreadPoolExecutor(max_workers=n_jobs) as executor_cmd:
             event = Event()
             run_shell = functools.partial(cls._run_shell, use_qsub=use_qsub, event=event)
 
-            # task_list = []
-            # for cmd in cmd_list:
-            #     task = executor_cmd.submit(run_shell, cmd)
-            #     task_list.append(task)
-            futures = [executor_cmd.submit(run_shell, cmd) for cmd in cmd_list]
-
-            if len(futures) >1:
-
-                done, not_done = wait(futures, return_when=FIRST_EXCEPTION)
-                if len(done) == 1 or len(done) != len(futures):
-                    future = list(done)[0]
-                    logging.info(future.exception())
-                    error_info = f'One task failed with: {future.exception()}, shutting down'
-                    for future in futures:
-                        future.cancel()
-
-                    event.set()
-                    raise Exception(error_info)
+            task_list = []
+            for cmd in cmd_list:
+                task = executor_cmd.submit(run_shell, cmd)
+                task_list.append(task)
+
+            for future in as_completed(task_list):
+                future.result()
+
+
+            #futures = [executor_cmd.submit(run_shell, cmd) for cmd in cmd_list]
+
+            # if len(futures) >=1:
+            #
+            #     done, not_done = wait(futures, return_when=FIRST_EXCEPTION)
+            #     if len(done) == 1 or len(done) != len(futures):
+            #         future = list(done)[0]
+            #         logging.info(future.exception())
+            #         error_info = f'One task failed with: {future.exception()}, shutting down'
+            #         for future in futures:
+            #             future.cancel()
+            #
+            #         event.set()
+            #         raise Exception(error_info)
 
             # while True:
             #     logging.info(cls.ERROR_LIST)
             #     if len(cls.ERROR_LIST) >= 1:
             #         executor_cmd.shutdown(wait=False)
 
-            # for future in as_completed(task_list):
-            #     future.result()
 
             # try:
             #     wait(task_list)
             # except ValueError:
             #     print("An error occurs in one of the threads, terminating all threads")
             #     executor_cmd.shutdown(wait=False)  # 立即关闭线程
```

