# Comparing `tmp/model_hub-0.22.1rc1-py3-none-any.whl.zip` & `tmp/model_hub-0.22.2rc0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,20 @@
-Zip file size: 23212 bytes, number of entries: 17
--rw-r--r--  2.0 unx        0 b- defN 23-May-17 18:35 model_hub/__init__.py
--rw-r--r--  2.0 unx       27 b- defN 23-May-17 18:35 model_hub/__version__.py
--rw-r--r--  2.0 unx     3110 b- defN 23-May-17 18:35 model_hub/utils.py
--rw-r--r--  2.0 unx      555 b- defN 23-May-17 18:35 model_hub/huggingface/__init__.py
--rw-r--r--  2.0 unx    13124 b- defN 23-May-17 18:35 model_hub/huggingface/_config_parser.py
--rw-r--r--  2.0 unx    12168 b- defN 23-May-17 18:35 model_hub/huggingface/_trial.py
--rw-r--r--  2.0 unx     1529 b- defN 23-May-17 18:35 model_hub/huggingface/_utils.py
--rw-r--r--  2.0 unx      385 b- defN 23-May-17 18:35 model_hub/mmdetection/__init__.py
--rw-r--r--  2.0 unx     4389 b- defN 23-May-17 18:35 model_hub/mmdetection/_callbacks.py
--rw-r--r--  2.0 unx     7547 b- defN 23-May-17 18:35 model_hub/mmdetection/_data.py
--rw-r--r--  2.0 unx     6137 b- defN 23-May-17 18:35 model_hub/mmdetection/_data_backends.py
--rw-r--r--  2.0 unx    11576 b- defN 23-May-17 18:35 model_hub/mmdetection/_trial.py
--rw-r--r--  2.0 unx     4345 b- defN 23-May-17 18:35 model_hub/mmdetection/utils.py
--rw-r--r--  2.0 unx      444 b- defN 23-May-17 18:35 model_hub-0.22.1rc1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-17 18:35 model_hub-0.22.1rc1.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-May-17 18:35 model_hub-0.22.1rc1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1453 b- defN 23-May-17 18:35 model_hub-0.22.1rc1.dist-info/RECORD
-17 files, 66891 bytes uncompressed, 20804 bytes compressed:  68.9%
+Zip file size: 23337 bytes, number of entries: 18
+-rw-r--r--  2.0 unx        0 b- defN 23-May-17 23:33 model_hub/__init__.py
+-rw-r--r--  2.0 unx       27 b- defN 23-May-17 23:33 model_hub/__version__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-17 23:33 model_hub/py.typed
+-rw-r--r--  2.0 unx     3110 b- defN 23-May-17 23:33 model_hub/utils.py
+-rw-r--r--  2.0 unx      555 b- defN 23-May-17 23:33 model_hub/huggingface/__init__.py
+-rw-r--r--  2.0 unx    13124 b- defN 23-May-17 23:33 model_hub/huggingface/_config_parser.py
+-rw-r--r--  2.0 unx    12168 b- defN 23-May-17 23:33 model_hub/huggingface/_trial.py
+-rw-r--r--  2.0 unx     1529 b- defN 23-May-17 23:33 model_hub/huggingface/_utils.py
+-rw-r--r--  2.0 unx      385 b- defN 23-May-17 23:33 model_hub/mmdetection/__init__.py
+-rw-r--r--  2.0 unx     4389 b- defN 23-May-17 23:33 model_hub/mmdetection/_callbacks.py
+-rw-r--r--  2.0 unx     7547 b- defN 23-May-17 23:33 model_hub/mmdetection/_data.py
+-rw-r--r--  2.0 unx     6137 b- defN 23-May-17 23:33 model_hub/mmdetection/_data_backends.py
+-rw-r--r--  2.0 unx    11576 b- defN 23-May-17 23:33 model_hub/mmdetection/_trial.py
+-rw-r--r--  2.0 unx     4345 b- defN 23-May-17 23:33 model_hub/mmdetection/utils.py
+-rw-r--r--  2.0 unx      444 b- defN 23-May-17 23:33 model_hub-0.22.2rc0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-17 23:33 model_hub-0.22.2rc0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-May-17 23:33 model_hub-0.22.2rc0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1525 b- defN 23-May-17 23:33 model_hub-0.22.2rc0.dist-info/RECORD
+18 files, 66963 bytes uncompressed, 20817 bytes compressed:  68.9%
```

## zipnote {}

```diff
@@ -1,13 +1,16 @@
 Filename: model_hub/__init__.py
 Comment: 
 
 Filename: model_hub/__version__.py
 Comment: 
 
+Filename: model_hub/py.typed
+Comment: 
+
 Filename: model_hub/utils.py
 Comment: 
 
 Filename: model_hub/huggingface/__init__.py
 Comment: 
 
 Filename: model_hub/huggingface/_config_parser.py
@@ -33,20 +36,20 @@
 
 Filename: model_hub/mmdetection/_trial.py
 Comment: 
 
 Filename: model_hub/mmdetection/utils.py
 Comment: 
 
-Filename: model_hub-0.22.1rc1.dist-info/METADATA
+Filename: model_hub-0.22.2rc0.dist-info/METADATA
 Comment: 
 
-Filename: model_hub-0.22.1rc1.dist-info/WHEEL
+Filename: model_hub-0.22.2rc0.dist-info/WHEEL
 Comment: 
 
-Filename: model_hub-0.22.1rc1.dist-info/top_level.txt
+Filename: model_hub-0.22.2rc0.dist-info/top_level.txt
 Comment: 
 
-Filename: model_hub-0.22.1rc1.dist-info/RECORD
+Filename: model_hub-0.22.2rc0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## model_hub/__version__.py

```diff
@@ -1 +1 @@
-__version__ = "0.22.1-rc1"
+__version__ = "0.22.2-rc0"
```

## Comparing `model_hub-0.22.1rc1.dist-info/RECORD` & `model_hub-0.22.2rc0.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 model_hub/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-model_hub/__version__.py,sha256=Zkgakjh89ajlZaixVMNWURCfCDI4LZMfyTG_73y2L98,27
+model_hub/__version__.py,sha256=k8Z531YiIghK2-4DuYKqHDRf6inkAi_EVqwLdNFvtc4,27
+model_hub/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 model_hub/utils.py,sha256=vecXGhVDjflfNjQMioKYUCVNN5wKS0oTvngXS4IvveU,3110
 model_hub/huggingface/__init__.py,sha256=xyqXOGi_SILBPWRBJacSZg_oDsHxrr1mb3hwaVhOXkE,555
 model_hub/huggingface/_config_parser.py,sha256=15TWjt0RbNem1fPUGLqUMvwRMEJbd0MRFt0rydXH2Bg,13124
 model_hub/huggingface/_trial.py,sha256=2a8Q5xaHDY7gQK6n6SKloW-RtXB-Mnu_oTgS_9EAMqo,12168
 model_hub/huggingface/_utils.py,sha256=QkQKRi4cfLaFdCcQqaYf6096W6RItfACeS12v6IlpM0,1529
 model_hub/mmdetection/__init__.py,sha256=Eyu-gXEgIy_VDWx7ie1dQgsQjkdTEyJv7gDKuJrPKIQ,385
 model_hub/mmdetection/_callbacks.py,sha256=sajGtqPldUVgYjZ_RCrJ17ysUtfztll6BUt16jgamus,4389
 model_hub/mmdetection/_data.py,sha256=xhopmmIQO0mTmlkZSpshIwDFpQ9f4CoPa2oKCZ40q8M,7547
 model_hub/mmdetection/_data_backends.py,sha256=QNnMjRjTg64J0bbgpuoZu7hm9zCQ5sCXY4keCdaAF_k,6137
 model_hub/mmdetection/_trial.py,sha256=oH89J0tF45r8MHlhSLIFmrohVZxK7sBCwo_sGpqUirg,11576
 model_hub/mmdetection/utils.py,sha256=cQucxk9gO8QACuiiYU6XB_-qmZYDzmwiBUX054F99q4,4345
-model_hub-0.22.1rc1.dist-info/METADATA,sha256=QmpWm8a2RM002tPFomszMRyHYAnZi_eLttSUtddgu68,444
-model_hub-0.22.1rc1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-model_hub-0.22.1rc1.dist-info/top_level.txt,sha256=qMud2IqWbRcQyKjzoPTdmR8Yd40scxRam5UwNdsK_WE,10
-model_hub-0.22.1rc1.dist-info/RECORD,,
+model_hub-0.22.2rc0.dist-info/METADATA,sha256=WX4b5CGHGEYZTYlV3G95P5Q9Lyhi5a0eyKRQGYI5Nw8,444
+model_hub-0.22.2rc0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+model_hub-0.22.2rc0.dist-info/top_level.txt,sha256=qMud2IqWbRcQyKjzoPTdmR8Yd40scxRam5UwNdsK_WE,10
+model_hub-0.22.2rc0.dist-info/RECORD,,
```

