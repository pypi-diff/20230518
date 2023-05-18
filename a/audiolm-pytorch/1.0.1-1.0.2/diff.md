# Comparing `tmp/audiolm-pytorch-1.0.1.tar.gz` & `tmp/audiolm-pytorch-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiolm-pytorch-1.0.1.tar", last modified: Thu May 18 19:08:00 2023, max compression
+gzip compressed data, was "audiolm-pytorch-1.0.2.tar", last modified: Thu May 18 19:09:10 2023, max compression
```

## Comparing `audiolm-pytorch-1.0.1.tar` & `audiolm-pytorch-1.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:08:00.879644 audiolm-pytorch-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-18 19:07:49.000000 audiolm-pytorch-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-18 19:08:00.879644 audiolm-pytorch-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18129 2023-05-18 19:07:49.000000 audiolm-pytorch-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:08:00.879644 audiolm-pytorch-1.0.1/audiolm_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-18 19:07:49.000000 audiolm-pytorch-1.0.1/audiolm_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    65627 2023-05-18 19:07:49.000000 audiolm-pytorch-1.0.1/audiolm_pytorch/audiolm_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-05-18 19:07:49.000000 audiolm-pytorch-1.0.1/audiolm_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-05-18 19:07:49.000000 audiolm-pytorch-1.0.1/audiolm_pytorch/encodec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-18 19:07:49.000000 audiolm-pytorch-1.0.1/audiolm_pytorch/hubert_kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-18 19:07:49.000000 audiolm-pytorch-1.0.1/audiolm_pytorch/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    30003 2023-05-18 19:07:49.000000 audiolm-pytorch-1.0.1/audiolm_pytorch/soundstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-18 19:07:49.000000 audiolm-pytorch-1.0.1/audiolm_pytorch/t5.py
--rw-r--r--   0 runner    (1001) docker     (123)    42310 2023-05-18 19:07:49.000000 audiolm-pytorch-1.0.1/audiolm_pytorch/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-18 19:07:49.000000 audiolm-pytorch-1.0.1/audiolm_pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-18 19:07:49.000000 audiolm-pytorch-1.0.1/audiolm_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-18 19:07:49.000000 audiolm-pytorch-1.0.1/audiolm_pytorch/vq_wav2vec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:08:00.879644 audiolm-pytorch-1.0.1/audiolm_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-18 19:08:00.000000 audiolm-pytorch-1.0.1/audiolm_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-18 19:08:00.000000 audiolm-pytorch-1.0.1/audiolm_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 19:08:00.000000 audiolm-pytorch-1.0.1/audiolm_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-18 19:08:00.000000 audiolm-pytorch-1.0.1/audiolm_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-18 19:08:00.000000 audiolm-pytorch-1.0.1/audiolm_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 19:08:00.879644 audiolm-pytorch-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-18 19:07:49.000000 audiolm-pytorch-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:09:10.734339 audiolm-pytorch-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-18 19:08:58.000000 audiolm-pytorch-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-18 19:09:10.734339 audiolm-pytorch-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18129 2023-05-18 19:08:58.000000 audiolm-pytorch-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:09:10.730339 audiolm-pytorch-1.0.2/audiolm_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-18 19:08:58.000000 audiolm-pytorch-1.0.2/audiolm_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65627 2023-05-18 19:08:58.000000 audiolm-pytorch-1.0.2/audiolm_pytorch/audiolm_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-05-18 19:08:58.000000 audiolm-pytorch-1.0.2/audiolm_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-05-18 19:08:58.000000 audiolm-pytorch-1.0.2/audiolm_pytorch/encodec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-18 19:08:58.000000 audiolm-pytorch-1.0.2/audiolm_pytorch/hubert_kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-18 19:08:58.000000 audiolm-pytorch-1.0.2/audiolm_pytorch/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30000 2023-05-18 19:08:58.000000 audiolm-pytorch-1.0.2/audiolm_pytorch/soundstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-18 19:08:58.000000 audiolm-pytorch-1.0.2/audiolm_pytorch/t5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42310 2023-05-18 19:08:58.000000 audiolm-pytorch-1.0.2/audiolm_pytorch/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-18 19:08:58.000000 audiolm-pytorch-1.0.2/audiolm_pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-18 19:08:58.000000 audiolm-pytorch-1.0.2/audiolm_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-18 19:08:58.000000 audiolm-pytorch-1.0.2/audiolm_pytorch/vq_wav2vec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:09:10.734339 audiolm-pytorch-1.0.2/audiolm_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-18 19:09:10.000000 audiolm-pytorch-1.0.2/audiolm_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-18 19:09:10.000000 audiolm-pytorch-1.0.2/audiolm_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 19:09:10.000000 audiolm-pytorch-1.0.2/audiolm_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-18 19:09:10.000000 audiolm-pytorch-1.0.2/audiolm_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-18 19:09:10.000000 audiolm-pytorch-1.0.2/audiolm_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 19:09:10.734339 audiolm-pytorch-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-18 19:08:58.000000 audiolm-pytorch-1.0.2/setup.py
```

### Comparing `audiolm-pytorch-1.0.1/LICENSE` & `audiolm-pytorch-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.1/PKG-INFO` & `audiolm-pytorch-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiolm-pytorch
-Version: 1.0.1
+Version: 1.0.2
 Summary: AudioLM - Language Modeling Approach to Audio Generation from Google Research - Pytorch
 Home-page: https://github.com/lucidrains/audiolm-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `audiolm-pytorch-1.0.1/README.md` & `audiolm-pytorch-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.1/audiolm_pytorch/__init__.py` & `audiolm-pytorch-1.0.2/audiolm_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.1/audiolm_pytorch/audiolm_pytorch.py` & `audiolm-pytorch-1.0.2/audiolm_pytorch/audiolm_pytorch.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.1/audiolm_pytorch/data.py` & `audiolm-pytorch-1.0.2/audiolm_pytorch/data.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.1/audiolm_pytorch/encodec.py` & `audiolm-pytorch-1.0.2/audiolm_pytorch/encodec.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.1/audiolm_pytorch/hubert_kmeans.py` & `audiolm-pytorch-1.0.2/audiolm_pytorch/hubert_kmeans.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.1/audiolm_pytorch/optimizer.py` & `audiolm-pytorch-1.0.2/audiolm_pytorch/optimizer.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.1/audiolm_pytorch/soundstream.py` & `audiolm-pytorch-1.0.2/audiolm_pytorch/soundstream.py`

 * *Files 0% similar despite different names*

```diff
@@ -500,15 +500,15 @@
         self.encoder_attn = LocalTransformer(**attn_kwargs) if use_local_attn else None
 
         self.encoder_film = FiLM(codebook_dim, dim_cond = 2)
 
         self.num_quantizers = rq_num_quantizers
 
         self.codebook_dim = codebook_dim
-        self.codebook_size = rq_codebook_size
+        self.codebook_size = codebook_size
 
         self.rq_groups = rq_groups
 
         self.rq = GroupedResidualVQ(
             dim = codebook_dim,
             num_quantizers = rq_num_quantizers,
             codebook_size = codebook_size,
```

### Comparing `audiolm-pytorch-1.0.1/audiolm_pytorch/t5.py` & `audiolm-pytorch-1.0.2/audiolm_pytorch/t5.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.1/audiolm_pytorch/trainer.py` & `audiolm-pytorch-1.0.2/audiolm_pytorch/trainer.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.1/audiolm_pytorch/vq_wav2vec.py` & `audiolm-pytorch-1.0.2/audiolm_pytorch/vq_wav2vec.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.1/audiolm_pytorch.egg-info/PKG-INFO` & `audiolm-pytorch-1.0.2/audiolm_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiolm-pytorch
-Version: 1.0.1
+Version: 1.0.2
 Summary: AudioLM - Language Modeling Approach to Audio Generation from Google Research - Pytorch
 Home-page: https://github.com/lucidrains/audiolm-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `audiolm-pytorch-1.0.1/audiolm_pytorch.egg-info/SOURCES.txt` & `audiolm-pytorch-1.0.2/audiolm_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.1/setup.py` & `audiolm-pytorch-1.0.2/setup.py`

 * *Files identical despite different names*

