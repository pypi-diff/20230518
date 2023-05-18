# Comparing `tmp/soundstorm-pytorch-0.0.5.tar.gz` & `tmp/soundstorm-pytorch-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soundstorm-pytorch-0.0.5.tar", last modified: Thu May 18 17:16:54 2023, max compression
+gzip compressed data, was "soundstorm-pytorch-0.0.6.tar", last modified: Thu May 18 19:17:47 2023, max compression
```

## Comparing `soundstorm-pytorch-0.0.5.tar` & `soundstorm-pytorch-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:16:54.503322 soundstorm-pytorch-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-18 17:16:37.000000 soundstorm-pytorch-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-18 17:16:54.503322 soundstorm-pytorch-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-18 17:16:37.000000 soundstorm-pytorch-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 17:16:54.503322 soundstorm-pytorch-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-18 17:16:37.000000 soundstorm-pytorch-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:16:54.503322 soundstorm-pytorch-0.0.5/soundstorm_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-18 17:16:37.000000 soundstorm-pytorch-0.0.5/soundstorm_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-05-18 17:16:37.000000 soundstorm-pytorch-0.0.5/soundstorm_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    13371 2023-05-18 17:16:37.000000 soundstorm-pytorch-0.0.5/soundstorm_pytorch/soundstorm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:16:54.503322 soundstorm-pytorch-0.0.5/soundstorm_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-18 17:16:54.000000 soundstorm-pytorch-0.0.5/soundstorm_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-18 17:16:54.000000 soundstorm-pytorch-0.0.5/soundstorm_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 17:16:54.000000 soundstorm-pytorch-0.0.5/soundstorm_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-18 17:16:54.000000 soundstorm-pytorch-0.0.5/soundstorm_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-18 17:16:54.000000 soundstorm-pytorch-0.0.5/soundstorm_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:17:47.145687 soundstorm-pytorch-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-18 19:17:34.000000 soundstorm-pytorch-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-18 19:17:47.145687 soundstorm-pytorch-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-05-18 19:17:34.000000 soundstorm-pytorch-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 19:17:47.145687 soundstorm-pytorch-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-18 19:17:34.000000 soundstorm-pytorch-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:17:47.145687 soundstorm-pytorch-0.0.6/soundstorm_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-18 19:17:34.000000 soundstorm-pytorch-0.0.6/soundstorm_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-05-18 19:17:34.000000 soundstorm-pytorch-0.0.6/soundstorm_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14551 2023-05-18 19:17:34.000000 soundstorm-pytorch-0.0.6/soundstorm_pytorch/soundstorm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:17:47.145687 soundstorm-pytorch-0.0.6/soundstorm_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-18 19:17:47.000000 soundstorm-pytorch-0.0.6/soundstorm_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-18 19:17:47.000000 soundstorm-pytorch-0.0.6/soundstorm_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 19:17:47.000000 soundstorm-pytorch-0.0.6/soundstorm_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-18 19:17:47.000000 soundstorm-pytorch-0.0.6/soundstorm_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-18 19:17:47.000000 soundstorm-pytorch-0.0.6/soundstorm_pytorch.egg-info/top_level.txt
```

### Comparing `soundstorm-pytorch-0.0.5/LICENSE` & `soundstorm-pytorch-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `soundstorm-pytorch-0.0.5/PKG-INFO` & `soundstorm-pytorch-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soundstorm-pytorch
-Version: 0.0.5
+Version: 0.0.6
 Summary: SoundStorm - Efficient Parallel Audio Generation from Google Deepmind, in Pytorch
 Home-page: https://github.com/lucidrains/soundstorm-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `soundstorm-pytorch-0.0.5/README.md` & `soundstorm-pytorch-0.0.6/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
 ## Appreciation
 
 - <a href="https://stability.ai/">Stability</a> and <a href="https://huggingface.co/">🤗 Huggingface</a> for their generous sponsorships to work on and open source cutting edge artificial intelligence research
 
 - <a href="https://huggingface.co/docs/accelerate/index">🤗 Accelerate</a> for providing a simple and powerful solution for training
 
+- <a href="https://einops.rocks/">Einops</a> for the indispensable abstraction that makes building neural networks fun, easy, and uplifting
+
 ## Install
 
 ```bash
 $ pip install soundstorm-pytorch
 ```
 
 ## Usage
@@ -51,17 +53,54 @@
 loss.backward()
 
 # generate by de-masking iteratively
 
 generated = model.generate(1024, batch_size = 2) # (2, 1024)
 ```
 
+To directly train on raw audio, you need to pass in your pretrained `SoundStream` into `SoundStorm`. You can train your own `SoundStream` at <a href="https://github.com/lucidrains/audiolm-pytorch#soundstream--encodec">audiolm-pytorch</a>.
+
+```python
+import torch
+from soundstorm_pytorch import SoundStorm, ConformerWrapper, Conformer, SoundStream
+
+conformer = ConformerWrapper(
+    codebook_size = 1024,
+    num_quantizers = 4,
+    conformer = dict(
+        dim = 512,
+        depth = 2
+    ),
+)
+
+soundstream = SoundStream(
+    codebook_size = 1024,
+    rq_num_quantizers = 4,
+    attn_window_size = 128,
+    attn_depth = 2
+)
+
+model = SoundStorm(
+    conformer,
+    soundstream = soundstream   # pass in the soundstream
+)
+
+audio = torch.randn(2, 10080)   # now you have a raw audio that you directly pass into the model
+
+loss, _ = model(audio)
+loss.backward()
+
+generated_audio = model.generate(1024, batch_size = 2)  # generated audio is also a raw wave now
+```
+
 ## Todo
 
-- [ ] integrate soundstream
+- [x] integrate soundstream
+
+- [ ] when generating, make sure it can return audio file, and length can be defined in seconds (takes into sampling freq etc)
 - [ ] turn it into a command line tool
 - [ ] add cross attention and adaptive layernorm conditioning (just copy paste in the entire conformer repository, if conditioning adds too much cruft to the other repo)
 
 ## Citations
 
 ```bibtex
 @misc{borsos2023soundstorm,
@@ -107,7 +146,17 @@
 @inproceedings{Nijkamp2021SCRIPTSP,
     title   = {SCRIPT: Self-Critic PreTraining of Transformers},
     author  = {Erik Nijkamp and Bo Pang and Ying Nian Wu and Caiming Xiong},
     booktitle = {North American Chapter of the Association for Computational Linguistics},
     year    = {2021}
 }
 ```
+
+```bibtex
+@inproceedings{rogozhnikov2022einops,
+    title   = {Einops: Clear and Reliable Tensor Manipulations with Einstein-like Notation},
+    author  = {Alex Rogozhnikov},
+    booktitle = {International Conference on Learning Representations},
+    year    = {2022},
+    url     = {https://openreview.net/forum?id=oapKSVM2bcj}
+}
+```
```

#### html2text {}

```diff
@@ -1,25 +1,39 @@
 [./soundstorm.png] ## Soundstorm - Pytorch (wip) Implementation of SoundStorm,
 Efficient Parallel Audio Generation from Google Deepmind, in Pytorch. They
 basically applied MaskGiT to the residual vector quantized latents from
 Soundstream. The transformer architecture they chose to use is one that fits
 well with the audio domain, named Conformer Project_Page ## Appreciation -
 Stability and ð¤_Huggingface for their generous sponsorships to work on and
 open source cutting edge artificial intelligence research - ð¤_Accelerate for
-providing a simple and powerful solution for training ## Install ```bash $ pip
-install soundstorm-pytorch ``` ## Usage ```python import torch from
-soundstorm_pytorch import SoundStorm, ConformerWrapper conformer =
-ConformerWrapper( codebook_size = 1024, num_quantizers = 4, conformer = dict
-( dim = 512, depth = 2 ), ) model = SoundStorm( conformer, steps = 18, # 18
-steps, as in original maskgit paper schedule = 'cosine' # currently the best
-schedule is cosine ) # get your codes from the soundstream codes =
-torch.randint(0, 1024, (2, 1024)) # learn to de-mask loss, _ = model(codes)
-loss.backward() # generate by de-masking iteratively generated = model.generate
-(1024, batch_size = 2) # (2, 1024) ``` ## Todo - [ ] integrate soundstream -
-[ ] turn it into a command line tool - [ ] add cross attention and adaptive
+providing a simple and powerful solution for training - Einops for the
+indispensable abstraction that makes building neural networks fun, easy, and
+uplifting ## Install ```bash $ pip install soundstorm-pytorch ``` ## Usage
+```python import torch from soundstorm_pytorch import SoundStorm,
+ConformerWrapper conformer = ConformerWrapper( codebook_size = 1024,
+num_quantizers = 4, conformer = dict( dim = 512, depth = 2 ), ) model =
+SoundStorm( conformer, steps = 18, # 18 steps, as in original maskgit paper
+schedule = 'cosine' # currently the best schedule is cosine ) # get your codes
+from the soundstream codes = torch.randint(0, 1024, (2, 1024)) # learn to de-
+mask loss, _ = model(codes) loss.backward() # generate by de-masking
+iteratively generated = model.generate(1024, batch_size = 2) # (2, 1024) ``` To
+directly train on raw audio, you need to pass in your pretrained `SoundStream`
+into `SoundStorm`. You can train your own `SoundStream` at audiolm-pytorch.
+```python import torch from soundstorm_pytorch import SoundStorm,
+ConformerWrapper, Conformer, SoundStream conformer = ConformerWrapper
+( codebook_size = 1024, num_quantizers = 4, conformer = dict( dim = 512, depth
+= 2 ), ) soundstream = SoundStream( codebook_size = 1024, rq_num_quantizers =
+4, attn_window_size = 128, attn_depth = 2 ) model = SoundStorm( conformer,
+soundstream = soundstream # pass in the soundstream ) audio = torch.randn(2,
+10080) # now you have a raw audio that you directly pass into the model loss, _
+= model(audio) loss.backward() generated_audio = model.generate(1024,
+batch_size = 2) # generated audio is also a raw wave now ``` ## Todo - [x]
+integrate soundstream - [ ] when generating, make sure it can return audio
+file, and length can be defined in seconds (takes into sampling freq etc) - [ ]
+turn it into a command line tool - [ ] add cross attention and adaptive
 layernorm conditioning (just copy paste in the entire conformer repository, if
 conditioning adds too much cruft to the other repo) ## Citations ```bibtex
 @misc{borsos2023soundstorm, title = {SoundStorm: Efficient Parallel Audio
 Generation}, author = {ZalÃ¡n Borsos and Matt Sharifi and Damien Vincent and
 Eugene Kharitonov and Neil Zeghidour and Marco Tagliasacchi}, year = {2023},
 eprint = {2305.09636}, archivePrefix = {arXiv}, primaryClass = {cs.SD} } ```
 ```bibtex @inproceedings{dao2022flashattention, title = {Flash{A}ttention: Fast
@@ -33,8 +47,12 @@
 {11305-11315} } ``` ```bibtex @article{Lezama2022ImprovedMI, title = {Improved
 Masked Image Generation with Token-Critic}, author = {Jos{\'e} Lezama and
 Huiwen Chang and Lu Jiang and Irfan Essa}, journal = {ArXiv}, year = {2022},
 volume = {abs/2209.04439} } ``` ```bibtex @inproceedings{Nijkamp2021SCRIPTSP,
 title = {SCRIPT: Self-Critic PreTraining of Transformers}, author = {Erik
 Nijkamp and Bo Pang and Ying Nian Wu and Caiming Xiong}, booktitle = {North
 American Chapter of the Association for Computational Linguistics}, year =
-{2021} } ```
+{2021} } ``` ```bibtex @inproceedings{rogozhnikov2022einops, title = {Einops:
+Clear and Reliable Tensor Manipulations with Einstein-like Notation}, author =
+{Alex Rogozhnikov}, booktitle = {International Conference on Learning
+Representations}, year = {2022}, url = {https://openreview.net/
+forum?id=oapKSVM2bcj} } ```
```

### Comparing `soundstorm-pytorch-0.0.5/setup.py` & `soundstorm-pytorch-0.0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'soundstorm-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.5',
+  version = '0.0.6',
   license='MIT',
   description = 'SoundStorm - Efficient Parallel Audio Generation from Google Deepmind, in Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/soundstorm-pytorch',
   keywords = [
@@ -15,15 +15,15 @@
     'deep learning',
     'transformers',
     'attention mechanism',
     'audio generation'
   ],
   install_requires=[
     'accelerate',
-    'audiolm-pytorch>=1.0.0',
+    'audiolm-pytorch>=1.0.1',
     'beartype',
     'conformer>=0.3.2',
     'einops>=0.6.1',
     'torch>=1.6',
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
```

### Comparing `soundstorm-pytorch-0.0.5/soundstorm_pytorch/attend.py` & `soundstorm-pytorch-0.0.6/soundstorm_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `soundstorm-pytorch-0.0.5/soundstorm_pytorch/soundstorm.py` & `soundstorm-pytorch-0.0.6/soundstorm_pytorch/soundstorm.py`

 * *Files 5% similar despite different names*

```diff
@@ -118,14 +118,17 @@
         self.num_tokens_per_head = default(num_tokens_per_head, num_quantizers)
 
         self.heads = nn.Sequential(
             nn.Linear(dim, dim * self.num_tokens_per_head),
             Rearrange('b n (h d) -> b (n h) d', h = self.num_tokens_per_head)
         )
 
+        # each quantizer codebook would require its own logits weight and bias matrices
+        # the amazing einops makes this easy with 'EinMix'
+
         self.to_logits = nn.Sequential(
             nn.LayerNorm(dim),
             Rearrange('b (n q) d -> b n q d', q = self.num_quantizers),
             EinMix(
                 'b n q d -> b n q l',
                 weight_shape = 'q d l',
                 bias_shape = 'q l',
@@ -212,21 +215,29 @@
         random_token_prob = 0.1,         # which percentage of tokens to be replaced with random token, done in original MLM paper
         schedule = 'linear',
         can_mask_prev_unmasked = False,  # when unmasking, whether it can remask previously unmasked        
         self_token_critic = False,       # https://aclanthology.org/2021.naacl-main.409/
         critic_loss_weight = 1.
     ):
         super().__init__()
+        self.soundstream = soundstream
+
+        if exists(self.soundstream):
+            assert soundstream.rq_groups == 1, 'grouped residual vector quantized soundstream not supported, yet'
+            assert net.codebook_size == soundstream.codebook_size
+            assert net.num_quantizers == soundstream.num_quantizers
+
         assert not (self_token_critic and exists(token_critic))
 
         self.net = net
 
         dim = net.dim
         self.dim = dim
         self.num_tokens = net.codebook_size
+        self.num_quantizers = net.num_quantizers
 
         self.mask_id = net.codebook_size
 
         # afaict, maskgit paper did not do this
         # but may help for self conditioning, as used successfully in original BERT
 
         self.no_replace_prob = no_replace_prob
@@ -341,27 +352,46 @@
 
             mask_indices = scores.topk(mask_num_tokens, dim = -1).indices
             mask = torch.zeros_like(scores, dtype = torch.bool).scatter(1, mask_indices, True)
             seq = seq.masked_fill(mask, self.mask_id)
 
         self.train(was_training)
 
+        out = seq
+
+        if exists(self.soundstream):
+            seq = rearrange(seq, 'b (n q) -> b n q', q = self.num_quantizers)
+
+            with torch.no_grad():
+                self.soundstream.eval()
+                out = self.soundstream.decode_from_codebook_indices(seq)
+                out = rearrange(out, 'b 1 ... -> b ...')
+
         if sample_one:
-            seq = rearrange(seq, '1 n -> n')
+            out = rearrange(out, '1 ... -> ...')
 
-        return seq
+        return out
 
     def forward(
         self,
         x,
         only_train_generator = False,
         only_train_critic = False,
         generator_sample_temperature = None,
         **kwargs
     ):
+        is_raw_audio = x.dtype == torch.float
+
+        if is_raw_audio:
+            assert exists(self.soundstream)
+            with torch.no_grad():
+                self.soundstream.eval()
+                _, x, _ = self.soundstream(x, return_encoded = True)
+                x = rearrange(x, 'b n q -> b (n q)')
+
         b, n, device = *x.shape, x.device
 
         orig_seq = x.clone()
 
         rand_times = torch.empty(b, device = device).uniform_(0, 1)
         batched_randperm = torch.rand((b, n), device = device).argsort(dim = -1).float()
```

### Comparing `soundstorm-pytorch-0.0.5/soundstorm_pytorch.egg-info/PKG-INFO` & `soundstorm-pytorch-0.0.6/soundstorm_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soundstorm-pytorch
-Version: 0.0.5
+Version: 0.0.6
 Summary: SoundStorm - Efficient Parallel Audio Generation from Google Deepmind, in Pytorch
 Home-page: https://github.com/lucidrains/soundstorm-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

