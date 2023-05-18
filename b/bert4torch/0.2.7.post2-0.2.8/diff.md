# Comparing `tmp/bert4torch-0.2.7.post2.tar.gz` & `tmp/bert4torch-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bert4torch-0.2.7.post2.tar", last modified: Sat Mar 11 02:00:45 2023, max compression
+gzip compressed data, was "bert4torch-0.2.8.tar", last modified: Thu May 18 15:21:02 2023, max compression
```

## Comparing `bert4torch-0.2.7.post2.tar` & `bert4torch-0.2.8.tar`

### file list

```diff
@@ -1,27 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-03-11 02:00:44.997464 bert4torch-0.2.7.post2/
--rw-rw-rw-   0        0        0     1089 2022-03-12 16:30:24.000000 bert4torch-0.2.7.post2/LICENSE
--rw-rw-rw-   0        0        0    19822 2023-03-11 02:00:44.996466 bert4torch-0.2.7.post2/PKG-INFO
--rw-rw-rw-   0        0        0    19564 2023-03-11 01:57:59.000000 bert4torch-0.2.7.post2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-11 02:00:44.965467 bert4torch-0.2.7.post2/bert4torch/
--rw-rw-rw-   0        0        0        0 2022-11-28 12:30:45.000000 bert4torch-0.2.7.post2/bert4torch/__init__.py
--rw-rw-rw-   0        0        0     3117 2022-12-17 14:54:44.000000 bert4torch-0.2.7.post2/bert4torch/activations.py
--rw-rw-rw-   0        0        0    81444 2023-03-10 15:08:54.000000 bert4torch-0.2.7.post2/bert4torch/layers.py
--rw-rw-rw-   0        0        0    16601 2023-02-22 15:31:01.000000 bert4torch-0.2.7.post2/bert4torch/losses.py
--rw-rw-rw-   0        0        0   103357 2023-03-09 15:15:28.000000 bert4torch-0.2.7.post2/bert4torch/models.py
--rw-rw-rw-   0        0        0     5832 2023-02-19 14:03:17.000000 bert4torch-0.2.7.post2/bert4torch/optimizers.py
--rw-rw-rw-   0        0        0    43071 2023-02-09 15:38:33.000000 bert4torch-0.2.7.post2/bert4torch/snippets.py
--rw-rw-rw-   0        0        0    34226 2022-12-21 15:41:54.000000 bert4torch-0.2.7.post2/bert4torch/tokenizers.py
-drwxrwxrwx   0        0        0        0 2023-03-11 02:00:44.990503 bert4torch-0.2.7.post2/bert4torch.egg-info/
--rw-rw-rw-   0        0        0    19822 2023-03-11 02:00:44.000000 bert4torch-0.2.7.post2/bert4torch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      516 2023-03-11 02:00:44.000000 bert4torch-0.2.7.post2/bert4torch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-11 02:00:44.000000 bert4torch-0.2.7.post2/bert4torch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-03-11 02:00:44.000000 bert4torch-0.2.7.post2/bert4torch.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-03-11 02:00:44.000000 bert4torch-0.2.7.post2/bert4torch.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-11 02:00:44.997464 bert4torch-0.2.7.post2/setup.cfg
--rw-rw-rw-   0        0        0      557 2023-03-11 01:57:46.000000 bert4torch-0.2.7.post2/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-11 02:00:44.995466 bert4torch-0.2.7.post2/test/
--rw-rw-rw-   0        0        0     2714 2023-01-31 16:18:03.000000 bert4torch-0.2.7.post2/test/test.py
--rw-rw-rw-   0        0        0    12963 2022-12-30 15:17:51.000000 bert4torch-0.2.7.post2/test/test1.py
--rw-rw-rw-   0        0        0      517 2022-11-13 08:57:04.000000 bert4torch-0.2.7.post2/test/test_deberta.py
--rw-rw-rw-   0        0        0      186 2022-11-15 14:52:37.000000 bert4torch-0.2.7.post2/test/test_deberta_relativeposition.py
--rw-rw-rw-   0        0        0    17673 2022-11-02 08:02:55.000000 bert4torch-0.2.7.post2/test/test_sequence_labeling_ner_CNN_Nested_NER.py
+drwxrwxrwx   0        0        0        0 2023-05-18 15:21:02.252458 bert4torch-0.2.8/
+-rw-rw-rw-   0        0        0     1089 2022-03-12 16:30:24.000000 bert4torch-0.2.8/LICENSE
+-rw-rw-rw-   0        0        0    22857 2023-05-18 15:21:02.251446 bert4torch-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0    22605 2023-05-18 15:17:35.000000 bert4torch-0.2.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 15:21:02.230447 bert4torch-0.2.8/bert4torch/
+-rw-rw-rw-   0        0        0        0 2022-11-28 12:30:45.000000 bert4torch-0.2.8/bert4torch/__init__.py
+-rw-rw-rw-   0        0        0     3117 2023-03-28 15:37:01.000000 bert4torch-0.2.8/bert4torch/activations.py
+-rw-rw-rw-   0        0        0    11689 2023-05-15 14:15:22.000000 bert4torch-0.2.8/bert4torch/callbacks.py
+-rw-rw-rw-   0        0        0    37983 2023-05-15 14:39:00.000000 bert4torch-0.2.8/bert4torch/generation.py
+-rw-rw-rw-   0        0        0    89761 2023-05-11 11:37:38.000000 bert4torch-0.2.8/bert4torch/layers.py
+-rw-rw-rw-   0        0        0    16592 2023-05-11 11:37:38.000000 bert4torch-0.2.8/bert4torch/losses.py
+-rw-rw-rw-   0        0        0   121652 2023-05-16 11:38:12.000000 bert4torch-0.2.8/bert4torch/models.py
+-rw-rw-rw-   0        0        0     7619 2023-03-29 15:35:29.000000 bert4torch-0.2.8/bert4torch/optimizers.py
+-rw-rw-rw-   0        0        0    18596 2023-05-10 15:51:29.000000 bert4torch-0.2.8/bert4torch/quantization.py
+-rw-rw-rw-   0        0        0    22590 2023-05-11 11:37:38.000000 bert4torch-0.2.8/bert4torch/snippets.py
+-rw-rw-rw-   0        0        0    35326 2023-04-28 12:14:08.000000 bert4torch-0.2.8/bert4torch/tokenizers.py
+drwxrwxrwx   0        0        0        0 2023-05-18 15:21:02.250446 bert4torch-0.2.8/bert4torch.egg-info/
+-rw-rw-rw-   0        0        0    22857 2023-05-18 15:21:01.000000 bert4torch-0.2.8/bert4torch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2023-05-18 15:21:02.000000 bert4torch-0.2.8/bert4torch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 15:21:01.000000 bert4torch-0.2.8/bert4torch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-05-18 15:21:01.000000 bert4torch-0.2.8/bert4torch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-18 15:21:01.000000 bert4torch-0.2.8/bert4torch.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 15:21:02.252458 bert4torch-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      557 2023-05-18 15:12:22.000000 bert4torch-0.2.8/setup.py
```

### Comparing `bert4torch-0.2.7.post2/LICENSE` & `bert4torch-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bert4torch-0.2.7.post2/PKG-INFO` & `bert4torch-0.2.8/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,122 +1,120 @@
-Metadata-Version: 2.1
-Name: bert4torch
-Version: 0.2.7.post2
-Summary: an elegant bert4torch
-Home-page: https://github.com/Tongjilibo/bert4torch
-Author: Tongjilibo
-License: MIT Licence
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # bert4torch
+
 **一款用pytorch来复现bert4keras的简洁训练框架**
 
-[![licence](https://img.shields.io/github/license/Tongjilibo/bert4torch.svg?maxAge=3600)](https://github.com/Tongjilibo/bert4torch/blob/master/LICENSE) 
-[![GitHub release](https://img.shields.io/github/release/Tongjilibo/bert4torch.svg?maxAge=3600)](https://github.com/Tongjilibo/bert4torch/releases) 
-[![PyPI](https://img.shields.io/pypi/v/bert4torch?label=pypi%20package)](https://pypi.org/project/bert4torch/) 
+[![licence](https://img.shields.io/github/license/Tongjilibo/bert4torch.svg?maxAge=3600)](https://github.com/Tongjilibo/bert4torch/blob/master/LICENSE)
+[![GitHub release](https://img.shields.io/github/release/Tongjilibo/bert4torch.svg?maxAge=3600)](https://github.com/Tongjilibo/bert4torch/releases)
+[![PyPI](https://img.shields.io/pypi/v/bert4torch?label=pypi%20package)](https://pypi.org/project/bert4torch/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/bert4torch)](https://pypistats.org/packages/bert4torch)
 [![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/bert4torch?style=social)](https://github.com/Tongjilibo/bert4torch)
 [![GitHub Issues](https://img.shields.io/github/issues/Tongjilibo/bert4torch.svg)](https://github.com/Tongjilibo/bert4torch/issues)
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Tongjilibo/bert4torch/issues)
 
 [Documentation](https://bert4torch.readthedocs.io) |
 [Torch4keras](https://github.com/Tongjilibo/torch4keras) |
 [Examples](https://github.com/Tongjilibo/bert4torch/blob/master/examples)
 
 ## 1. 下载安装
+
 安装稳定版
+
 ```shell
 pip install bert4torch
 ```
+
 安装最新版
+
 ```shell
-pip install git+https://www.github.com/Tongjilibo/bert4torch.git
+pip install git+https://github.com/Tongjilibo/bert4torch
 ```
+
 - **注意事项**：pip包的发布慢于git上的开发版本，git clone**注意引用路径**，注意权重是否需要转换
 - **测试用例**：`git clone https://github.com/Tongjilibo/bert4torch`，修改example中的预训练模型文件路径和数据路径即可启动脚本
 - **自行训练**：针对自己的数据，修改相应的数据处理代码块
 - **开发环境**：使用`torch==1.10`版本进行开发，如其他版本遇到不适配，欢迎反馈
 
 ## 2. 功能
+
+- **LLM模型**: 加载chatglm-6b和llama-7b进行推理和finetune
 - **核心功能**：加载bert、roberta、albert、xlnet、nezha、bart、RoFormer、RoFormer_V2、ELECTRA、GPT、GPT2、T5、GAU-alpha、ERNIE等预训练权重继续进行finetune、并支持在bert基础上灵活定义自己模型
 - [**丰富示例**](https://github.com/Tongjilibo/bert4torch/blob/master/examples/)：包含[pretrain](https://github.com/Tongjilibo/bert4torch/blob/master/examples/pretrain)、[sentence_classfication](https://github.com/Tongjilibo/bert4torch/blob/master/examples/sentence_classfication)、[sentence_embedding](https://github.com/Tongjilibo/bert4torch/tree/master/examples/sentence_embedding)、[sequence_labeling](https://github.com/Tongjilibo/bert4torch/blob/master/examples/sequence_labeling)、[relation_extraction](https://github.com/Tongjilibo/bert4torch/blob/master/examples/relation_extraction)、[seq2seq](https://github.com/Tongjilibo/bert4torch/blob/master/examples/seq2seq)、[serving](https://github.com/Tongjilibo/bert4torch/blob/master/examples/serving/)等多种解决方案
 - **实验验证**：已在公开数据集实验验证，使用如下[examples数据集](https://github.com/Tongjilibo/bert4torch/blob/master/examples/README.md)
 - **易用trick**：集成了常见的[trick](https://github.com/Tongjilibo/bert4torch/blob/master/examples/training_trick)，即插即用
 - **其他特性**：[加载transformers库模型](https://github.com/Tongjilibo/bert4torch/blob/master/examples/tutorials/tutorials_load_transformers_model.py)一起使用；调用方式简洁高效；有训练进度条动态展示；配合torchinfo打印参数量；默认Logger和Tensorboard简便记录训练过程；自定义fit过程，满足高阶需求
 - **训练过程**：
 
-    ```text
-    2022-10-28 23:16:10 - Start Training
-    2022-10-28 23:16:10 - Epoch: 1/5
-    5000/5000 [==============================] - 13s 3ms/step - loss: 0.1351 - acc: 0.9601
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 798.09it/s] 
-    test_acc: 0.98045. best_test_acc: 0.98045
-
-    2022-10-28 23:16:27 - Epoch: 2/5
-    5000/5000 [==============================] - 13s 3ms/step - loss: 0.0465 - acc: 0.9862
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 635.78it/s] 
-    test_acc: 0.98280. best_test_acc: 0.98280
-
-    2022-10-28 23:16:44 - Epoch: 3/5
-    5000/5000 [==============================] - 15s 3ms/step - loss: 0.0284 - acc: 0.9915
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 673.60it/s] 
-    test_acc: 0.98365. best_test_acc: 0.98365
-
-    2022-10-28 23:17:03 - Epoch: 4/5
-    5000/5000 [==============================] - 15s 3ms/step - loss: 0.0179 - acc: 0.9948
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 692.34it/s] 
-    test_acc: 0.98265. best_test_acc: 0.98365
-
-    2022-10-28 23:17:21 - Epoch: 5/5
-    5000/5000 [==============================] - 14s 3ms/step - loss: 0.0129 - acc: 0.9958
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 701.77it/s] 
-    test_acc: 0.98585. best_test_acc: 0.98585
+  ```text
+  2022-10-28 23:16:10 - Start Training
+  2022-10-28 23:16:10 - Epoch: 1/2
+  5000/5000 [==============================] - 13s 3ms/step - loss: 0.1351 - acc: 0.9601
+  Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 798.09it/s] 
+  test_acc: 0.98045. best_test_acc: 0.98045
+
+  2022-10-28 23:16:27 - Epoch: 2/2
+  5000/5000 [==============================] - 13s 3ms/step - loss: 0.0465 - acc: 0.9862
+  Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 635.78it/s] 
+  test_acc: 0.98280. best_test_acc: 0.98280
 
-    2022-10-28 23:17:37 - Finish Training
-    ```
+  2022-10-28 23:16:44 - Finish Training
+  ```
 
 ## 3. 快速上手
+
 - [Quick-Start](https://bert4torch.readthedocs.io/en/latest//Quick-Start.html)
 - [快速上手教程](https://github.com/Tongjilibo/bert4torch/blob/master/examples/tutorials/Tutorials.md)，[教程示例](https://github.com/Tongjilibo/bert4torch/blob/master/examples/tutorials)，[实战示例](https://github.com/Tongjilibo/bert4torch/blob/master/examples)
 - [bert4torch介绍(知乎)](https://zhuanlan.zhihu.com/p/486329434)，[bert4torch快速上手(知乎)](https://zhuanlan.zhihu.com/p/508890807)，[bert4torch又双叒叕更新啦(知乎)](https://zhuanlan.zhihu.com/p/560885427?)
 
-## 4. 版本说明
-### 4.1 更新历史
+## 4. 版本历史
+
+<details><summary><b>点击查看</b></summary>
+
+**版本说明**
+- **v0.2.8**：20230518 增加chatglm-6b/llama-7b预训练模型, 修改rope为不使用max_position，修复model.half()类型不一致问题，生成式解码新增SeqGeneration和Seq2SeqGeneration, 支持加载多个权重文件, gpt系列默认不加softmax，更新fnlp的bart2.0。增加苏神Tiger的pytorch实现, 集成苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型, 增加了对attention_key_size的入参支持(skykiseki用户); 修复model.half()类型不一致问题，生成式解码新增SeqGeneration和Seq2SeqGeneration, 支持加载多个权重文件, gpt系列默认不加softmax; 增加苏神Tiger的pytorch实现, 集成苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型, 增加了对attention_key_size的入参支持，单向decoder模型和encoder decoder模型解码增加cache, 更新fnlp的bart2.0, 增加chatglm-6b预训练模型推理, 集成BELLE_llama模型, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2，增加moss模型的int4/int8推理; 增加vicuna的集成, 增加batch_generate()功能, 把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
 - **v0.2.7.post2**：20230310 增加lion优化器, 修复albert_unshared加载权重, 修复lm系列(gpt, seq2seq)存在的forward参数不对的问题，修复GlobalPointer使用rope的bug
 - **v0.2.7**：20230213 修复random_sample()的bug，适配v0.0.6的torch4keras：增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现，增加了AccelerateCallback
 - **v0.2.6**：20221231 build_transformer_model需显式指定add_trainer才从BaseModel继承, 增加guwenbert, macbert，text2vec-bert-chinese, wobert预训练模型，允许position_ids从padding开始, transformer.configs支持点操作，可以使用torch4keras的Trainer(net)来初始化, 修复tokenizer的切分subtoken的bug, 允许embedding_size!=hidden_size
 - **v0.2.5**：20221127 对抗训练从compile转为使用Callback来实现，修复1.7.1版本兼容bug, uie模型内置
 - **v0.2.4**：20221120 删除SpTokenizer基类中的rematch, 增加deberta_v2模型
 - **v0.2.3**：20221023 虚拟对抗VAT在多个ouput时支持指定，把Trainer抽象到[torch4keras](https://github.com/Tongjilibo/torch4keras)中，修复DP和DDP出现resume_epoch不存在的bug, tokenizer的never_split去除None, transformer_xl的bug, 增加gradient_checkpoint
 - **v0.2.2**：20220922 修复t5的norm_mode问题，允许hidden_size不整除num_attention_heads，支持多个schedule(如同时ema+warmup)
 - **v0.2.1**：20220905 兼容torch<=1.7.1的torch.div无rounding_mode，增加自定义metrics，支持断点续训，增加默认Logger和Tensorboard日志
-- **v0.2.0**：20220823 兼容torch<1.9.0的缺失take_along_dim，修复bart中位置向量514的问题，修复Sptokenizer对符号不转换，打印Epoch开始的时间戳，增加parallel_apply
+- **v0.2.0**：20220823 兼容torch1.9.0的缺失take_along_dim，修复bart中位置向量514的问题，修复Sptokenizer对符号不转换，打印Epoch开始的时间戳，增加parallel_apply
 - **v0.1.9**：20220808 增加mixup/manifold_mixup/temporal_ensembling策略，修复pgd策略param.grad为空的问题，修改tokenizer支持批量
 - **v0.1.8**：20220717 修复原来CRF训练中loss陡增的问题，修复xlnet的token_type_ids输入显存占用大的问题
 - **v0.1.7**：20220710 增加EarlyStop，CRF中自带转bool类型
 - **v0.1.6**：20220605 增加transformer_xl、xlnet、t5_pegasus模型，prompt、预训练等示例，支持增加embedding输入，EMA策略，修复tokenizer和sinusoid的bug
 - **v0.1.5**：20220504 增加GAU-alpha，混合梯度，梯度裁剪，单机多卡(DP、DDP)
 - **v0.1.4**：20220421 增加了VAT，修复了linux下apply_embedding返回项有问题的情况
 - **v0.1.3**：20220409 初始版本
 
-### 4.2 版本对应关系
-| bert4torch版本 |  torch4keras版本 |
-|  ----  |  ----  |
-|  0.2.7  | 0.0.6 |
-|  0.2.6  | 0.0.5 |
-|  0.2.5  | 0.0.4 |
-|  0.2.4  | 0.0.3.post2 |
-|  0.2.3  | 0.0.2 |
-|  <0.2.3  | —— |
+**版本对应关系**
 
-
-## 5. 更新：
+| bert4torch版本 | torch4keras版本 |
+| ---------------- | ----------------- |
+| 0.2.8          | 0.0.7.post3     |
+| 0.2.7.post2    | 0.0.6           |
+| 0.2.7          | 0.0.6           |
+| 0.2.6          | 0.0.5           |
+| 0.2.5          | 0.0.4           |
+| 0.2.4          | 0.0.3.post2     |
+| 0.2.3          | 0.0.2           |
+| <0.2.3         | ——            |
+
+</details>
+
+
+## 5. 更新历史：
+<details><summary><b>点击查看</b></summary>
+
+- **20230426**：增加vicuna的集成, 增加batch_generate()功能, 把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
+- **20230408**：增加苏神Tiger的pytorch实现, 集成苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型, 增加了对attention_key_size的入参支持，单向decoder模型和encoder decoder模型解码增加cache, 更新fnlp的bart2.0, 增加chatglm-6b预训练模型推理, 集成BELLE_llama模型, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2，增加moss模型的int4/int8推理
+- **20230326**：增加llama-7b预训练模型, 修改rope为不使用max_position, 增加prompt_clue和nezha_gpt_dialog的finetune示例(skykiseki用户)，修复model.half()类型不一致问题，生成式解码新增SeqGeneration和Seq2SeqGeneration, 支持加载多个权重文件, gpt系列默认不加softmax
 - **20230310**：增加lion优化器, 修改dp和ddp示例更易用，增加PromptCLUE模型, 修复albert_unshared加载权重, 增加uer-gpt2-chinese预训练模型，修复lm系列(gpt, seq2seq)存在的forward参数不对的问题，修复GlobalPointer使用rope的bug
-- **20230212**：兼容accelerate包, 增加ChatYuan模型，修复random_sample()的bug
+- **20230212**：兼容accelerate包, 增加ChatYuan v1模型，修复random_sample()的bug
 - **20221230**：增加macbert，text2vec-bert-chinese, wobert模型，增加LEAR的ner示例, 增加PGRC、SPN4RE的关系提取示例，transformer.configs支持点操作，可以使用torch4keras的Trainer(net)来初始化, 修复tokenizer的切分subtoken的bug, 允许embedding_size!=hidden_size
 - **20221127**：增加deberta_v2模型, 对抗训练从compile转为使用Callback来实现，修复1.7.1版本兼容bug, uie模型内置, 增加triton示例, build_transformer_model需显式指定add_trainer才从BaseModel继承, 增加guwenbert预训练模型，允许position_ids从padding开始
 - **20221102**：增加CNN_Nested_NER示例, 删除SpTokenizer基类中的rematch
 - **20221022**：修复DP和DDP出现resume_epoch不存在的bug, tokenizer的never_split去除None, transformer_xl的bug, 增加gradient_checkpoint
 - **20221011**：虚拟对抗VAT在多个ouput时支持指定，增加elasticsearch示例, 把Trainer抽象到[torch4keras](https://github.com/Tongjilibo/torch4keras)中供更多项目使用，把梯度累积移到compile中
 - **20220920**：增加TensorRT示例，支持多个schedule(如同时ema+warmup)，sanic+onnx部署
 - **20220910**：增加默认Logger和Tensorboard日志，ONNX推理，增加ERNIE模型，修复t5的norm_mode问题，允许hidden_size不整除num_attention_heads
@@ -135,76 +133,98 @@
 - **20220425**：增加了VAT、GAU-alpha等示例，增加了梯度累积，自定义fit()示例
 - **20220415**：增加了ner_mrc、ner_span、roformer_v2、roformer-sim等示例
 - **20220405**：增加了GPLinker、TPlinker、SimBERT等示例
 - **20220329**：增加了CoSENT、R-Drop、UDA等示例
 - **20220322**：添加GPT、GPT2、T5模型
 - **20220312**：初版提交
 
+</details>
 
 ## 6. 预训练权重
+
 - 部分权重是要加载修改的[config.json](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)
 
-| 模型分类 |  权重来源 | 权重链接 | 备注(若有) | 
-|  ----  |  ----  | ----  | ----  |
-|  bert  | 谷歌原版bert(即bert-base-chinese) | [tf](https://github.com/google-research/bert)，[torch](https://huggingface.co/bert-base-chinese) | [tf转pytorch命令](https://huggingface.co/docs/transformers/converting_tensorflow_models)，[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bert-base-chinese.py)
-|  bert  | 哈工大chinese-bert-wwm-ext | [tf/torch](https://github.com/ymcui/Chinese-BERT-wwm)，[torch](https://huggingface.co/hfl/chinese-bert-wwm-ext) |
-|  macbert  | 哈工大chinese-macbert-base/large | [tf/torch](https://github.com/ymcui/MacBERT)，[torch](https://huggingface.co/hfl/chinese-macbert-base) |
-| robert | 哈工大chinese-robert-wwm-ext | [tf/torch](https://github.com/ymcui/Chinese-BERT-wwm)，[torch](https://huggingface.co/hfl/chinese-roberta-wwm-ext)
-| deberta_v2| IDEA Erlangshen-DeBERTa-v2 | [torch](https://huggingface.co/IDEA-CCNL/Erlangshen-DeBERTa-v2-320M-Chinese/tree/main) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_deberta_v2.py) |
-| guwenbert | 古文bert | [torch](https://huggingface.co/ethanyt/guwenbert-base)|[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_guwenbert-base.py)|
-| xlnet | 哈工大xlnet | [tf/torch](https://github.com/ymcui/Chinese-XLNet) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)
-| electra | 哈工大electra | [tf](https://github.com/ymcui/Chinese-ELECTRA)，[torch](https://huggingface.co/hfl/chinese-electra-base-discriminator)
-| macbert | 哈工大macbert | [tf](https://github.com/ymcui/MacBERT)，[torch](https://huggingface.co/hfl/chinese-macbert-base)
-| albert | brightmart | [tf](https://github.com/brightmart/albert_zh)，[torch](https://huggingface.co/voidful)，[torch](https://github.com/lonePatient/albert_pytorch)
-| ernie | 百度文心 |[paddle](https://github.com/PaddlePaddle/ERNIE)，[torch](https://huggingface.co/nghuyong) | 
-| roformer | 追一科技 | [tf](https://github.com/ZhuiyiTechnology/roformer)，[torch](https://huggingface.co/junnyu/roformer_chinese_base) |  
-| roformer_v2 | 追一科技 | [tf](https://github.com/ZhuiyiTechnology/roformer-v2)，[torch](https://huggingface.co/junnyu/roformer_v2_chinese_char_base) | 
-| simbert | 追一科技 | [tf](https://github.com/ZhuiyiTechnology/simbert)，[torch_base](https://huggingface.co/peterchou/simbert-chinese-base/tree/main) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_simbert.py) |
-| roformer-sim | 追一科技 | [tf](https://github.com/ZhuiyiTechnology/roformer-sim)，[torch](https://huggingface.co/junnyu/roformer_chinese_sim_char_base) | 
-| gau-alpha | 追一科技 | [tf](https://github.com/ZhuiyiTechnology/GAU-alpha) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_GAU_alpha.py)
-| wobert | 追一科技 | [tf](https://github.com/ZhuiyiTechnology/WoBERT)，[torch_base](https://huggingface.co/junnyu/wobert_chinese_base)，[torch_plus_base](https://huggingface.co/junnyu/wobert_chinese_plus_base)||
-| nezha | 华为 | [tf](https://github.com/huawei-noah/Pretrained-Language-Model/tree/master/NEZHA-TensorFlow)，[torch](https://github.com/lonePatient/NeZha_Chinese_PyTorch) | 
-| gpt | thu-coai/CDial-GPT | [torch](https://github.com/thu-coai/CDial-GPT) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_gpt__CDial-GPT-LCCC.py)
-| gpt2 | 清华26亿 cmp_lm | [torch](https://github.com/TsinghuaAI/CPM-1-Generate) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_gpt2__cmp_lm_2.6b.py)
-| gpt2 | 中文GPT2_ML模型 | [tf](https://github.com/imcaspar/gpt2-ml)，[torch](https://github.com/ghosthamlet/gpt2-ml-torch) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_gpt2__gpt2-ml.py)
-| gpt2 | UER | [torch](https://huggingface.co/uer/gpt2-chinese-cluecorpussmall) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_gpt2__uer-gpt2-chinese.py) |
-| t5 | UER | [torch](https://huggingface.co/uer/t5-base-chinese-cluecorpussmall) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)
-| mt5 | 谷歌 | [torch](https://huggingface.co/google/mt5-base) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)
-| t5_pegasus | 追一科技 | [tf](https://github.com/ZhuiyiTechnology/t5-pegasus) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_t5_pegasus.py)
-| bart | 复旦 | [torch](https://github.com/fastnlp/CPT) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bart_fudanNLP.py)
-| text2vec | text2vec-base-chinese | [torch](https://huggingface.co/shibing624/text2vec-base-chinese) | 
-| chatyuan | clue-ai | [torch](https://github.com/clue-ai/ChatYuan) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)
-| PromptCLUE | clue-ai | [torch](https://github.com/clue-ai/PromptCLUE) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)
+
+| 模型分类| 权重来源| 权重链接 | 备注(若有)|
+| ----- | ----- | ----- | ----- |
+| bert| 谷歌原版bert(即bert-base-chinese) | [tf](https://github.com/google-research/bert)，[torch](https://huggingface.co/bert-base-chinese) | [tf转pytorch命令](https://huggingface.co/docs/transformers/converting_tensorflow_models)，[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bert-base-chinese.py) |
+| bert| 哈工大chinese-bert-wwm-ext| [tf/torch](https://github.com/ymcui/Chinese-BERT-wwm)，[torch](https://huggingface.co/hfl/chinese-bert-wwm-ext)| |
+| macbert | 哈工大chinese-macbert-base/large| [tf/torch](https://github.com/ymcui/MacBERT)，[torch](https://huggingface.co/hfl/chinese-macbert-base) | |
+| roberta | 哈工大chinese-roberta-wwm-ext | [tf/torch](https://github.com/ymcui/Chinese-BERT-wwm)，[torch](https://huggingface.co/hfl/chinese-roberta-wwm-ext) | |
+| roberta-small/tiny| 追一科技 & UER| [tf](https://github.com/ZhuiyiTechnology/pretrained-models)，[torch](https://huggingface.co/uer) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_roberta-small.py) |
+| deberta_v2| IDEA Erlangshen-DeBERTa-v2| [torch](https://huggingface.co/IDEA-CCNL/Erlangshen-DeBERTa-v2-320M-Chinese/tree/main) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_deberta_v2.py)|
+| guwenbert | 古文bert| [torch](https://huggingface.co/ethanyt/guwenbert-base) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_guwenbert-base.py)|
+| xlnet | 哈工大xlnet | [tf/torch](https://github.com/ymcui/Chinese-XLNet) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
+| electra | 哈工大electra | [tf](https://github.com/ymcui/Chinese-ELECTRA)，[torch](https://huggingface.co/hfl/chinese-electra-base-discriminator) | |
+| macbert | 哈工大macbert | [tf](https://github.com/ymcui/MacBERT)，[torch](https://huggingface.co/hfl/chinese-macbert-base) | |
+| albert| brightmart| [tf](https://github.com/brightmart/albert_zh)，[torch](https://huggingface.co/voidful)，[torch](https://github.com/lonePatient/albert_pytorch) | |
+| ernie | 百度文心| [paddle](https://github.com/PaddlePaddle/ERNIE)，[torch](https://huggingface.co/nghuyong)| |
+| roformer| 追一科技| [tf](https://github.com/ZhuiyiTechnology/roformer)，[torch](https://huggingface.co/junnyu/roformer_chinese_base) | |
+| roformer_v2 | 追一科技| [tf](https://github.com/ZhuiyiTechnology/roformer-v2)，[torch](https://huggingface.co/junnyu/roformer_v2_chinese_char_base)| |
+| simbert | 追一科技| [tf](https://github.com/ZhuiyiTechnology/simbert)，[torch_base](https://huggingface.co/peterchou/simbert-chinese-base/tree/main) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_simbert.py) |
+| simbert_v2/roformer-sim | 追一科技| [tf](https://github.com/ZhuiyiTechnology/roformer-sim)，[torch](https://huggingface.co/junnyu/roformer_chinese_sim_char_base)| |
+| gau-alpha | 追一科技| [tf](https://github.com/ZhuiyiTechnology/GAU-alpha)| [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_GAU_alpha.py) |
+| wobert| 追一科技| [tf](https://github.com/ZhuiyiTechnology/WoBERT)，[torch_base](https://huggingface.co/junnyu/wobert_chinese_base)，[torch_plus_base](https://huggingface.co/junnyu/wobert_chinese_plus_base) | |
+| nezha | 华为| [tf](https://github.com/huawei-noah/Pretrained-Language-Model/tree/master/NEZHA-TensorFlow)，[torch](https://github.com/lonePatient/NeZha_Chinese_PyTorch) | |
+| gpt | thu-coai/CDial-GPT| [torch](https://github.com/thu-coai/CDial-GPT) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_gpt__CDial-GPT-LCCC.py) |
+| gpt2| 清华26亿 cmp_lm | [torch](https://github.com/TsinghuaAI/CPM-1-Generate)| [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_gpt2__cmp_lm_2.6b.py) |
+| gpt2| 中文GPT2_ML模型 | [tf](https://github.com/imcaspar/gpt2-ml)，[torch](https://github.com/ghosthamlet/gpt2-ml-torch) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_gpt2__gpt2-ml.py) |
+| gpt2| UER | [torch](https://huggingface.co/uer/gpt2-chinese-cluecorpussmall) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_gpt2__uer-gpt2-chinese.py)|
+| t5| UER | [torch](https://huggingface.co/uer/t5-base-chinese-cluecorpussmall)| [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
+| mt5 | 谷歌| [torch](https://huggingface.co/google/mt5-base)| [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
+| t5_pegasus| 追一科技| [tf](https://github.com/ZhuiyiTechnology/t5-pegasus) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_t5_pegasus.py)|
+| bart| 复旦| [torch](https://github.com/fastnlp/CPT), [v1.0](https://huggingface.co/fnlp/bart-base-chinese/tree/v1.0), [v2.0](https://huggingface.co/fnlp/bart-base-chinese/tree/v2.0)| [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bart_fudanNLP.py) |
+| text2vec| text2vec-base-chinese | [torch](https://huggingface.co/shibing624/text2vec-base-chinese) | |
+| chatyuan v1&v2| clue-ai | [torch](https://github.com/clue-ai/ChatYuan) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
+| PromptCLUE| clue-ai | [torch](https://github.com/clue-ai/PromptCLUE) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
+| llama | facebook| [torch](https://github.com/facebookresearch/llama) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_facebook.py)|
+| vicuna | FastChat| [torch](https://huggingface.co/AlekseyKorshuk/vicuna-7b) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_vicuna.py)|
+| Belle| LianjiaTech| [torch](https://huggingface.co/BelleGroup/BELLE-LLaMA-7B-2M-enc) | [合成说明](https://github.com/LianjiaTech/BELLE/tree/main/models)、[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_belle.py)|
+| chatglm | THUDM | [torch](https://github.com/THUDM/ChatGLM-6B) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_chatglm.py) |
 
 ## 7. 鸣谢
-- 感谢苏神实现的[bert4keras](https://github.com/bojone/bert4keras)，本实现有不少地方参考了bert4keras的源码，在此衷心感谢大佬的无私奉献; 
-- 其次感谢项目[bert4pytorch](https://github.com/MuQiuJun-AI/bert4pytorch)，也是在该项目的指引下给了我用pytorch来复现bert4keras的想法和思路。
 
+- 感谢苏神实现的[bert4keras](https://github.com/bojone/bert4keras)，本实现有不少地方参考了bert4keras的源码，在此衷心感谢大佬的无私奉献;
+- 其次感谢项目[bert4pytorch](https://github.com/MuQiuJun-AI/bert4pytorch)，也是在该项目的指引下给了我用pytorch来复现bert4keras的想法和思路。
 
 ## 8. 引用
+
 ```
 @misc{bert4torch,
   title={bert4torch},
   author={Bo Li},
   year={2022},
   howpublished={\url{https://github.com/Tongjilibo/bert4torch}},
 }
 ```
 
-## 9. 交流
+## 9. 其他
+
 - Wechat Discussions
 
 <table border="0">
   <tbody>
     <tr align="center" >
       <td>
-        ​ <a href="https://github.com/Tongjilibo"><img width="200" height="250" src="./docs/pics/wechat.jpg" alt="pic"></a><br>
-        ​ <a href="https://github.com/Tongjilibo">微信号</a> ​
-​
+         <a href="https://github.com/Tongjilibo"><img width="200" height="250" src="./docs/pics/wechat.jpg" alt="pic"></a><br>
+         <a href="https://github.com/Tongjilibo">微信号</a> 
       </td>
       <td>
          <a href="https://github.com/Tongjilibo"><img width="200" height="250" src="./docs/pics/wechat_group.jpg" alt="pic"></a><br>
-         <a href="https://github.com/Tongjilibo">微信群</a> ​
+         <a href="https://github.com/Tongjilibo">微信群</a> 
       </td>
     </tr>
   </tbody>
 </table>
+
+- Star History Chart
+
+<table border="0">
+  <tbody>
+    <tr align="center" >
+      <td>
+         <a href="https://star-history.com/#Tongjilibo/bert4torch&Date"><img width="400" height="250" src="https://api.star-history.com/svg?repos=Tongjilibo/bert4torch&type=Date" alt="pic"></a><br>
+         <a href="https://star-history.com/#Tongjilibo/bert4torch&Date">Star History Chart</a> 
+      </td>
+    </tr>
+  </tbody>
+</table>
```

### Comparing `bert4torch-0.2.7.post2/README.md` & `bert4torch-0.2.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,112 +1,130 @@
+Metadata-Version: 2.1
+Name: bert4torch
+Version: 0.2.8
+Summary: an elegant bert4torch
+Home-page: https://github.com/Tongjilibo/bert4torch
+Author: Tongjilibo
+License: MIT Licence
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # bert4torch
+
 **一款用pytorch来复现bert4keras的简洁训练框架**
 
-[![licence](https://img.shields.io/github/license/Tongjilibo/bert4torch.svg?maxAge=3600)](https://github.com/Tongjilibo/bert4torch/blob/master/LICENSE) 
-[![GitHub release](https://img.shields.io/github/release/Tongjilibo/bert4torch.svg?maxAge=3600)](https://github.com/Tongjilibo/bert4torch/releases) 
-[![PyPI](https://img.shields.io/pypi/v/bert4torch?label=pypi%20package)](https://pypi.org/project/bert4torch/) 
+[![licence](https://img.shields.io/github/license/Tongjilibo/bert4torch.svg?maxAge=3600)](https://github.com/Tongjilibo/bert4torch/blob/master/LICENSE)
+[![GitHub release](https://img.shields.io/github/release/Tongjilibo/bert4torch.svg?maxAge=3600)](https://github.com/Tongjilibo/bert4torch/releases)
+[![PyPI](https://img.shields.io/pypi/v/bert4torch?label=pypi%20package)](https://pypi.org/project/bert4torch/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/bert4torch)](https://pypistats.org/packages/bert4torch)
 [![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/bert4torch?style=social)](https://github.com/Tongjilibo/bert4torch)
 [![GitHub Issues](https://img.shields.io/github/issues/Tongjilibo/bert4torch.svg)](https://github.com/Tongjilibo/bert4torch/issues)
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Tongjilibo/bert4torch/issues)
 
 [Documentation](https://bert4torch.readthedocs.io) |
 [Torch4keras](https://github.com/Tongjilibo/torch4keras) |
 [Examples](https://github.com/Tongjilibo/bert4torch/blob/master/examples)
 
 ## 1. 下载安装
+
 安装稳定版
+
 ```shell
 pip install bert4torch
 ```
+
 安装最新版
+
 ```shell
-pip install git+https://www.github.com/Tongjilibo/bert4torch.git
+pip install git+https://github.com/Tongjilibo/bert4torch
 ```
+
 - **注意事项**：pip包的发布慢于git上的开发版本，git clone**注意引用路径**，注意权重是否需要转换
 - **测试用例**：`git clone https://github.com/Tongjilibo/bert4torch`，修改example中的预训练模型文件路径和数据路径即可启动脚本
 - **自行训练**：针对自己的数据，修改相应的数据处理代码块
 - **开发环境**：使用`torch==1.10`版本进行开发，如其他版本遇到不适配，欢迎反馈
 
 ## 2. 功能
+
+- **LLM模型**: 加载chatglm-6b和llama-7b进行推理和finetune
 - **核心功能**：加载bert、roberta、albert、xlnet、nezha、bart、RoFormer、RoFormer_V2、ELECTRA、GPT、GPT2、T5、GAU-alpha、ERNIE等预训练权重继续进行finetune、并支持在bert基础上灵活定义自己模型
 - [**丰富示例**](https://github.com/Tongjilibo/bert4torch/blob/master/examples/)：包含[pretrain](https://github.com/Tongjilibo/bert4torch/blob/master/examples/pretrain)、[sentence_classfication](https://github.com/Tongjilibo/bert4torch/blob/master/examples/sentence_classfication)、[sentence_embedding](https://github.com/Tongjilibo/bert4torch/tree/master/examples/sentence_embedding)、[sequence_labeling](https://github.com/Tongjilibo/bert4torch/blob/master/examples/sequence_labeling)、[relation_extraction](https://github.com/Tongjilibo/bert4torch/blob/master/examples/relation_extraction)、[seq2seq](https://github.com/Tongjilibo/bert4torch/blob/master/examples/seq2seq)、[serving](https://github.com/Tongjilibo/bert4torch/blob/master/examples/serving/)等多种解决方案
 - **实验验证**：已在公开数据集实验验证，使用如下[examples数据集](https://github.com/Tongjilibo/bert4torch/blob/master/examples/README.md)
 - **易用trick**：集成了常见的[trick](https://github.com/Tongjilibo/bert4torch/blob/master/examples/training_trick)，即插即用
 - **其他特性**：[加载transformers库模型](https://github.com/Tongjilibo/bert4torch/blob/master/examples/tutorials/tutorials_load_transformers_model.py)一起使用；调用方式简洁高效；有训练进度条动态展示；配合torchinfo打印参数量；默认Logger和Tensorboard简便记录训练过程；自定义fit过程，满足高阶需求
 - **训练过程**：
 
-    ```text
-    2022-10-28 23:16:10 - Start Training
-    2022-10-28 23:16:10 - Epoch: 1/5
-    5000/5000 [==============================] - 13s 3ms/step - loss: 0.1351 - acc: 0.9601
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 798.09it/s] 
-    test_acc: 0.98045. best_test_acc: 0.98045
-
-    2022-10-28 23:16:27 - Epoch: 2/5
-    5000/5000 [==============================] - 13s 3ms/step - loss: 0.0465 - acc: 0.9862
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 635.78it/s] 
-    test_acc: 0.98280. best_test_acc: 0.98280
-
-    2022-10-28 23:16:44 - Epoch: 3/5
-    5000/5000 [==============================] - 15s 3ms/step - loss: 0.0284 - acc: 0.9915
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 673.60it/s] 
-    test_acc: 0.98365. best_test_acc: 0.98365
-
-    2022-10-28 23:17:03 - Epoch: 4/5
-    5000/5000 [==============================] - 15s 3ms/step - loss: 0.0179 - acc: 0.9948
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 692.34it/s] 
-    test_acc: 0.98265. best_test_acc: 0.98365
-
-    2022-10-28 23:17:21 - Epoch: 5/5
-    5000/5000 [==============================] - 14s 3ms/step - loss: 0.0129 - acc: 0.9958
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 701.77it/s] 
-    test_acc: 0.98585. best_test_acc: 0.98585
+  ```text
+  2022-10-28 23:16:10 - Start Training
+  2022-10-28 23:16:10 - Epoch: 1/2
+  5000/5000 [==============================] - 13s 3ms/step - loss: 0.1351 - acc: 0.9601
+  Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 798.09it/s] 
+  test_acc: 0.98045. best_test_acc: 0.98045
+
+  2022-10-28 23:16:27 - Epoch: 2/2
+  5000/5000 [==============================] - 13s 3ms/step - loss: 0.0465 - acc: 0.9862
+  Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 635.78it/s] 
+  test_acc: 0.98280. best_test_acc: 0.98280
 
-    2022-10-28 23:17:37 - Finish Training
-    ```
+  2022-10-28 23:16:44 - Finish Training
+  ```
 
 ## 3. 快速上手
+
 - [Quick-Start](https://bert4torch.readthedocs.io/en/latest//Quick-Start.html)
 - [快速上手教程](https://github.com/Tongjilibo/bert4torch/blob/master/examples/tutorials/Tutorials.md)，[教程示例](https://github.com/Tongjilibo/bert4torch/blob/master/examples/tutorials)，[实战示例](https://github.com/Tongjilibo/bert4torch/blob/master/examples)
 - [bert4torch介绍(知乎)](https://zhuanlan.zhihu.com/p/486329434)，[bert4torch快速上手(知乎)](https://zhuanlan.zhihu.com/p/508890807)，[bert4torch又双叒叕更新啦(知乎)](https://zhuanlan.zhihu.com/p/560885427?)
 
-## 4. 版本说明
-### 4.1 更新历史
+## 4. 版本历史
+
+<details><summary><b>点击查看</b></summary>
+
+**版本说明**
+- **v0.2.8**：20230518 增加chatglm-6b/llama-7b预训练模型, 修改rope为不使用max_position，修复model.half()类型不一致问题，生成式解码新增SeqGeneration和Seq2SeqGeneration, 支持加载多个权重文件, gpt系列默认不加softmax，更新fnlp的bart2.0。增加苏神Tiger的pytorch实现, 集成苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型, 增加了对attention_key_size的入参支持(skykiseki用户); 修复model.half()类型不一致问题，生成式解码新增SeqGeneration和Seq2SeqGeneration, 支持加载多个权重文件, gpt系列默认不加softmax; 增加苏神Tiger的pytorch实现, 集成苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型, 增加了对attention_key_size的入参支持，单向decoder模型和encoder decoder模型解码增加cache, 更新fnlp的bart2.0, 增加chatglm-6b预训练模型推理, 集成BELLE_llama模型, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2，增加moss模型的int4/int8推理; 增加vicuna的集成, 增加batch_generate()功能, 把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
 - **v0.2.7.post2**：20230310 增加lion优化器, 修复albert_unshared加载权重, 修复lm系列(gpt, seq2seq)存在的forward参数不对的问题，修复GlobalPointer使用rope的bug
 - **v0.2.7**：20230213 修复random_sample()的bug，适配v0.0.6的torch4keras：增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现，增加了AccelerateCallback
 - **v0.2.6**：20221231 build_transformer_model需显式指定add_trainer才从BaseModel继承, 增加guwenbert, macbert，text2vec-bert-chinese, wobert预训练模型，允许position_ids从padding开始, transformer.configs支持点操作，可以使用torch4keras的Trainer(net)来初始化, 修复tokenizer的切分subtoken的bug, 允许embedding_size!=hidden_size
 - **v0.2.5**：20221127 对抗训练从compile转为使用Callback来实现，修复1.7.1版本兼容bug, uie模型内置
 - **v0.2.4**：20221120 删除SpTokenizer基类中的rematch, 增加deberta_v2模型
 - **v0.2.3**：20221023 虚拟对抗VAT在多个ouput时支持指定，把Trainer抽象到[torch4keras](https://github.com/Tongjilibo/torch4keras)中，修复DP和DDP出现resume_epoch不存在的bug, tokenizer的never_split去除None, transformer_xl的bug, 增加gradient_checkpoint
 - **v0.2.2**：20220922 修复t5的norm_mode问题，允许hidden_size不整除num_attention_heads，支持多个schedule(如同时ema+warmup)
 - **v0.2.1**：20220905 兼容torch<=1.7.1的torch.div无rounding_mode，增加自定义metrics，支持断点续训，增加默认Logger和Tensorboard日志
-- **v0.2.0**：20220823 兼容torch<1.9.0的缺失take_along_dim，修复bart中位置向量514的问题，修复Sptokenizer对符号不转换，打印Epoch开始的时间戳，增加parallel_apply
+- **v0.2.0**：20220823 兼容torch1.9.0的缺失take_along_dim，修复bart中位置向量514的问题，修复Sptokenizer对符号不转换，打印Epoch开始的时间戳，增加parallel_apply
 - **v0.1.9**：20220808 增加mixup/manifold_mixup/temporal_ensembling策略，修复pgd策略param.grad为空的问题，修改tokenizer支持批量
 - **v0.1.8**：20220717 修复原来CRF训练中loss陡增的问题，修复xlnet的token_type_ids输入显存占用大的问题
 - **v0.1.7**：20220710 增加EarlyStop，CRF中自带转bool类型
 - **v0.1.6**：20220605 增加transformer_xl、xlnet、t5_pegasus模型，prompt、预训练等示例，支持增加embedding输入，EMA策略，修复tokenizer和sinusoid的bug
 - **v0.1.5**：20220504 增加GAU-alpha，混合梯度，梯度裁剪，单机多卡(DP、DDP)
 - **v0.1.4**：20220421 增加了VAT，修复了linux下apply_embedding返回项有问题的情况
 - **v0.1.3**：20220409 初始版本
 
-### 4.2 版本对应关系
-| bert4torch版本 |  torch4keras版本 |
-|  ----  |  ----  |
-|  0.2.7  | 0.0.6 |
-|  0.2.6  | 0.0.5 |
-|  0.2.5  | 0.0.4 |
-|  0.2.4  | 0.0.3.post2 |
-|  0.2.3  | 0.0.2 |
-|  <0.2.3  | —— |
+**版本对应关系**
 
-
-## 5. 更新：
+| bert4torch版本 | torch4keras版本 |
+| ---------------- | ----------------- |
+| 0.2.8          | 0.0.7.post3     |
+| 0.2.7.post2    | 0.0.6           |
+| 0.2.7          | 0.0.6           |
+| 0.2.6          | 0.0.5           |
+| 0.2.5          | 0.0.4           |
+| 0.2.4          | 0.0.3.post2     |
+| 0.2.3          | 0.0.2           |
+| <0.2.3         | ——            |
+
+</details>
+
+
+## 5. 更新历史：
+<details><summary><b>点击查看</b></summary>
+
+- **20230426**：增加vicuna的集成, 增加batch_generate()功能, 把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
+- **20230408**：增加苏神Tiger的pytorch实现, 集成苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型, 增加了对attention_key_size的入参支持，单向decoder模型和encoder decoder模型解码增加cache, 更新fnlp的bart2.0, 增加chatglm-6b预训练模型推理, 集成BELLE_llama模型, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2，增加moss模型的int4/int8推理
+- **20230326**：增加llama-7b预训练模型, 修改rope为不使用max_position, 增加prompt_clue和nezha_gpt_dialog的finetune示例(skykiseki用户)，修复model.half()类型不一致问题，生成式解码新增SeqGeneration和Seq2SeqGeneration, 支持加载多个权重文件, gpt系列默认不加softmax
 - **20230310**：增加lion优化器, 修改dp和ddp示例更易用，增加PromptCLUE模型, 修复albert_unshared加载权重, 增加uer-gpt2-chinese预训练模型，修复lm系列(gpt, seq2seq)存在的forward参数不对的问题，修复GlobalPointer使用rope的bug
-- **20230212**：兼容accelerate包, 增加ChatYuan模型，修复random_sample()的bug
+- **20230212**：兼容accelerate包, 增加ChatYuan v1模型，修复random_sample()的bug
 - **20221230**：增加macbert，text2vec-bert-chinese, wobert模型，增加LEAR的ner示例, 增加PGRC、SPN4RE的关系提取示例，transformer.configs支持点操作，可以使用torch4keras的Trainer(net)来初始化, 修复tokenizer的切分subtoken的bug, 允许embedding_size!=hidden_size
 - **20221127**：增加deberta_v2模型, 对抗训练从compile转为使用Callback来实现，修复1.7.1版本兼容bug, uie模型内置, 增加triton示例, build_transformer_model需显式指定add_trainer才从BaseModel继承, 增加guwenbert预训练模型，允许position_ids从padding开始
 - **20221102**：增加CNN_Nested_NER示例, 删除SpTokenizer基类中的rematch
 - **20221022**：修复DP和DDP出现resume_epoch不存在的bug, tokenizer的never_split去除None, transformer_xl的bug, 增加gradient_checkpoint
 - **20221011**：虚拟对抗VAT在多个ouput时支持指定，增加elasticsearch示例, 把Trainer抽象到[torch4keras](https://github.com/Tongjilibo/torch4keras)中供更多项目使用，把梯度累积移到compile中
 - **20220920**：增加TensorRT示例，支持多个schedule(如同时ema+warmup)，sanic+onnx部署
 - **20220910**：增加默认Logger和Tensorboard日志，ONNX推理，增加ERNIE模型，修复t5的norm_mode问题，允许hidden_size不整除num_attention_heads
@@ -125,76 +143,98 @@
 - **20220425**：增加了VAT、GAU-alpha等示例，增加了梯度累积，自定义fit()示例
 - **20220415**：增加了ner_mrc、ner_span、roformer_v2、roformer-sim等示例
 - **20220405**：增加了GPLinker、TPlinker、SimBERT等示例
 - **20220329**：增加了CoSENT、R-Drop、UDA等示例
 - **20220322**：添加GPT、GPT2、T5模型
 - **20220312**：初版提交
 
+</details>
 
 ## 6. 预训练权重
+
 - 部分权重是要加载修改的[config.json](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)
 
-| 模型分类 |  权重来源 | 权重链接 | 备注(若有) | 
-|  ----  |  ----  | ----  | ----  |
-|  bert  | 谷歌原版bert(即bert-base-chinese) | [tf](https://github.com/google-research/bert)，[torch](https://huggingface.co/bert-base-chinese) | [tf转pytorch命令](https://huggingface.co/docs/transformers/converting_tensorflow_models)，[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bert-base-chinese.py)
-|  bert  | 哈工大chinese-bert-wwm-ext | [tf/torch](https://github.com/ymcui/Chinese-BERT-wwm)，[torch](https://huggingface.co/hfl/chinese-bert-wwm-ext) |
-|  macbert  | 哈工大chinese-macbert-base/large | [tf/torch](https://github.com/ymcui/MacBERT)，[torch](https://huggingface.co/hfl/chinese-macbert-base) |
-| robert | 哈工大chinese-robert-wwm-ext | [tf/torch](https://github.com/ymcui/Chinese-BERT-wwm)，[torch](https://huggingface.co/hfl/chinese-roberta-wwm-ext)
-| deberta_v2| IDEA Erlangshen-DeBERTa-v2 | [torch](https://huggingface.co/IDEA-CCNL/Erlangshen-DeBERTa-v2-320M-Chinese/tree/main) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_deberta_v2.py) |
-| guwenbert | 古文bert | [torch](https://huggingface.co/ethanyt/guwenbert-base)|[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_guwenbert-base.py)|
-| xlnet | 哈工大xlnet | [tf/torch](https://github.com/ymcui/Chinese-XLNet) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)
-| electra | 哈工大electra | [tf](https://github.com/ymcui/Chinese-ELECTRA)，[torch](https://huggingface.co/hfl/chinese-electra-base-discriminator)
-| macbert | 哈工大macbert | [tf](https://github.com/ymcui/MacBERT)，[torch](https://huggingface.co/hfl/chinese-macbert-base)
-| albert | brightmart | [tf](https://github.com/brightmart/albert_zh)，[torch](https://huggingface.co/voidful)，[torch](https://github.com/lonePatient/albert_pytorch)
-| ernie | 百度文心 |[paddle](https://github.com/PaddlePaddle/ERNIE)，[torch](https://huggingface.co/nghuyong) | 
-| roformer | 追一科技 | [tf](https://github.com/ZhuiyiTechnology/roformer)，[torch](https://huggingface.co/junnyu/roformer_chinese_base) |  
-| roformer_v2 | 追一科技 | [tf](https://github.com/ZhuiyiTechnology/roformer-v2)，[torch](https://huggingface.co/junnyu/roformer_v2_chinese_char_base) | 
-| simbert | 追一科技 | [tf](https://github.com/ZhuiyiTechnology/simbert)，[torch_base](https://huggingface.co/peterchou/simbert-chinese-base/tree/main) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_simbert.py) |
-| roformer-sim | 追一科技 | [tf](https://github.com/ZhuiyiTechnology/roformer-sim)，[torch](https://huggingface.co/junnyu/roformer_chinese_sim_char_base) | 
-| gau-alpha | 追一科技 | [tf](https://github.com/ZhuiyiTechnology/GAU-alpha) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_GAU_alpha.py)
-| wobert | 追一科技 | [tf](https://github.com/ZhuiyiTechnology/WoBERT)，[torch_base](https://huggingface.co/junnyu/wobert_chinese_base)，[torch_plus_base](https://huggingface.co/junnyu/wobert_chinese_plus_base)||
-| nezha | 华为 | [tf](https://github.com/huawei-noah/Pretrained-Language-Model/tree/master/NEZHA-TensorFlow)，[torch](https://github.com/lonePatient/NeZha_Chinese_PyTorch) | 
-| gpt | thu-coai/CDial-GPT | [torch](https://github.com/thu-coai/CDial-GPT) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_gpt__CDial-GPT-LCCC.py)
-| gpt2 | 清华26亿 cmp_lm | [torch](https://github.com/TsinghuaAI/CPM-1-Generate) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_gpt2__cmp_lm_2.6b.py)
-| gpt2 | 中文GPT2_ML模型 | [tf](https://github.com/imcaspar/gpt2-ml)，[torch](https://github.com/ghosthamlet/gpt2-ml-torch) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_gpt2__gpt2-ml.py)
-| gpt2 | UER | [torch](https://huggingface.co/uer/gpt2-chinese-cluecorpussmall) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_gpt2__uer-gpt2-chinese.py) |
-| t5 | UER | [torch](https://huggingface.co/uer/t5-base-chinese-cluecorpussmall) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)
-| mt5 | 谷歌 | [torch](https://huggingface.co/google/mt5-base) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)
-| t5_pegasus | 追一科技 | [tf](https://github.com/ZhuiyiTechnology/t5-pegasus) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_t5_pegasus.py)
-| bart | 复旦 | [torch](https://github.com/fastnlp/CPT) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bart_fudanNLP.py)
-| text2vec | text2vec-base-chinese | [torch](https://huggingface.co/shibing624/text2vec-base-chinese) | 
-| chatyuan | clue-ai | [torch](https://github.com/clue-ai/ChatYuan) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)
-| PromptCLUE | clue-ai | [torch](https://github.com/clue-ai/PromptCLUE) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)
+
+| 模型分类| 权重来源| 权重链接 | 备注(若有)|
+| ----- | ----- | ----- | ----- |
+| bert| 谷歌原版bert(即bert-base-chinese) | [tf](https://github.com/google-research/bert)，[torch](https://huggingface.co/bert-base-chinese) | [tf转pytorch命令](https://huggingface.co/docs/transformers/converting_tensorflow_models)，[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bert-base-chinese.py) |
+| bert| 哈工大chinese-bert-wwm-ext| [tf/torch](https://github.com/ymcui/Chinese-BERT-wwm)，[torch](https://huggingface.co/hfl/chinese-bert-wwm-ext)| |
+| macbert | 哈工大chinese-macbert-base/large| [tf/torch](https://github.com/ymcui/MacBERT)，[torch](https://huggingface.co/hfl/chinese-macbert-base) | |
+| roberta | 哈工大chinese-roberta-wwm-ext | [tf/torch](https://github.com/ymcui/Chinese-BERT-wwm)，[torch](https://huggingface.co/hfl/chinese-roberta-wwm-ext) | |
+| roberta-small/tiny| 追一科技 & UER| [tf](https://github.com/ZhuiyiTechnology/pretrained-models)，[torch](https://huggingface.co/uer) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_roberta-small.py) |
+| deberta_v2| IDEA Erlangshen-DeBERTa-v2| [torch](https://huggingface.co/IDEA-CCNL/Erlangshen-DeBERTa-v2-320M-Chinese/tree/main) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_deberta_v2.py)|
+| guwenbert | 古文bert| [torch](https://huggingface.co/ethanyt/guwenbert-base) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_guwenbert-base.py)|
+| xlnet | 哈工大xlnet | [tf/torch](https://github.com/ymcui/Chinese-XLNet) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
+| electra | 哈工大electra | [tf](https://github.com/ymcui/Chinese-ELECTRA)，[torch](https://huggingface.co/hfl/chinese-electra-base-discriminator) | |
+| macbert | 哈工大macbert | [tf](https://github.com/ymcui/MacBERT)，[torch](https://huggingface.co/hfl/chinese-macbert-base) | |
+| albert| brightmart| [tf](https://github.com/brightmart/albert_zh)，[torch](https://huggingface.co/voidful)，[torch](https://github.com/lonePatient/albert_pytorch) | |
+| ernie | 百度文心| [paddle](https://github.com/PaddlePaddle/ERNIE)，[torch](https://huggingface.co/nghuyong)| |
+| roformer| 追一科技| [tf](https://github.com/ZhuiyiTechnology/roformer)，[torch](https://huggingface.co/junnyu/roformer_chinese_base) | |
+| roformer_v2 | 追一科技| [tf](https://github.com/ZhuiyiTechnology/roformer-v2)，[torch](https://huggingface.co/junnyu/roformer_v2_chinese_char_base)| |
+| simbert | 追一科技| [tf](https://github.com/ZhuiyiTechnology/simbert)，[torch_base](https://huggingface.co/peterchou/simbert-chinese-base/tree/main) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_simbert.py) |
+| simbert_v2/roformer-sim | 追一科技| [tf](https://github.com/ZhuiyiTechnology/roformer-sim)，[torch](https://huggingface.co/junnyu/roformer_chinese_sim_char_base)| |
+| gau-alpha | 追一科技| [tf](https://github.com/ZhuiyiTechnology/GAU-alpha)| [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_GAU_alpha.py) |
+| wobert| 追一科技| [tf](https://github.com/ZhuiyiTechnology/WoBERT)，[torch_base](https://huggingface.co/junnyu/wobert_chinese_base)，[torch_plus_base](https://huggingface.co/junnyu/wobert_chinese_plus_base) | |
+| nezha | 华为| [tf](https://github.com/huawei-noah/Pretrained-Language-Model/tree/master/NEZHA-TensorFlow)，[torch](https://github.com/lonePatient/NeZha_Chinese_PyTorch) | |
+| gpt | thu-coai/CDial-GPT| [torch](https://github.com/thu-coai/CDial-GPT) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_gpt__CDial-GPT-LCCC.py) |
+| gpt2| 清华26亿 cmp_lm | [torch](https://github.com/TsinghuaAI/CPM-1-Generate)| [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_gpt2__cmp_lm_2.6b.py) |
+| gpt2| 中文GPT2_ML模型 | [tf](https://github.com/imcaspar/gpt2-ml)，[torch](https://github.com/ghosthamlet/gpt2-ml-torch) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_gpt2__gpt2-ml.py) |
+| gpt2| UER | [torch](https://huggingface.co/uer/gpt2-chinese-cluecorpussmall) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_gpt2__uer-gpt2-chinese.py)|
+| t5| UER | [torch](https://huggingface.co/uer/t5-base-chinese-cluecorpussmall)| [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
+| mt5 | 谷歌| [torch](https://huggingface.co/google/mt5-base)| [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
+| t5_pegasus| 追一科技| [tf](https://github.com/ZhuiyiTechnology/t5-pegasus) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_t5_pegasus.py)|
+| bart| 复旦| [torch](https://github.com/fastnlp/CPT), [v1.0](https://huggingface.co/fnlp/bart-base-chinese/tree/v1.0), [v2.0](https://huggingface.co/fnlp/bart-base-chinese/tree/v2.0)| [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bart_fudanNLP.py) |
+| text2vec| text2vec-base-chinese | [torch](https://huggingface.co/shibing624/text2vec-base-chinese) | |
+| chatyuan v1&v2| clue-ai | [torch](https://github.com/clue-ai/ChatYuan) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
+| PromptCLUE| clue-ai | [torch](https://github.com/clue-ai/PromptCLUE) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
+| llama | facebook| [torch](https://github.com/facebookresearch/llama) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_facebook.py)|
+| vicuna | FastChat| [torch](https://huggingface.co/AlekseyKorshuk/vicuna-7b) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_vicuna.py)|
+| Belle| LianjiaTech| [torch](https://huggingface.co/BelleGroup/BELLE-LLaMA-7B-2M-enc) | [合成说明](https://github.com/LianjiaTech/BELLE/tree/main/models)、[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_belle.py)|
+| chatglm | THUDM | [torch](https://github.com/THUDM/ChatGLM-6B) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_chatglm.py) |
 
 ## 7. 鸣谢
-- 感谢苏神实现的[bert4keras](https://github.com/bojone/bert4keras)，本实现有不少地方参考了bert4keras的源码，在此衷心感谢大佬的无私奉献; 
-- 其次感谢项目[bert4pytorch](https://github.com/MuQiuJun-AI/bert4pytorch)，也是在该项目的指引下给了我用pytorch来复现bert4keras的想法和思路。
 
+- 感谢苏神实现的[bert4keras](https://github.com/bojone/bert4keras)，本实现有不少地方参考了bert4keras的源码，在此衷心感谢大佬的无私奉献;
+- 其次感谢项目[bert4pytorch](https://github.com/MuQiuJun-AI/bert4pytorch)，也是在该项目的指引下给了我用pytorch来复现bert4keras的想法和思路。
 
 ## 8. 引用
+
 ```
 @misc{bert4torch,
   title={bert4torch},
   author={Bo Li},
   year={2022},
   howpublished={\url{https://github.com/Tongjilibo/bert4torch}},
 }
 ```
 
-## 9. 交流
+## 9. 其他
+
 - Wechat Discussions
 
 <table border="0">
   <tbody>
     <tr align="center" >
       <td>
-        ​ <a href="https://github.com/Tongjilibo"><img width="200" height="250" src="./docs/pics/wechat.jpg" alt="pic"></a><br>
-        ​ <a href="https://github.com/Tongjilibo">微信号</a> ​
-​
+         <a href="https://github.com/Tongjilibo"><img width="200" height="250" src="./docs/pics/wechat.jpg" alt="pic"></a><br>
+         <a href="https://github.com/Tongjilibo">微信号</a> 
       </td>
       <td>
          <a href="https://github.com/Tongjilibo"><img width="200" height="250" src="./docs/pics/wechat_group.jpg" alt="pic"></a><br>
-         <a href="https://github.com/Tongjilibo">微信群</a> ​
+         <a href="https://github.com/Tongjilibo">微信群</a> 
+      </td>
+    </tr>
+  </tbody>
+</table>
+
+- Star History Chart
+
+<table border="0">
+  <tbody>
+    <tr align="center" >
+      <td>
+         <a href="https://star-history.com/#Tongjilibo/bert4torch&Date"><img width="400" height="250" src="https://api.star-history.com/svg?repos=Tongjilibo/bert4torch&type=Date" alt="pic"></a><br>
+         <a href="https://star-history.com/#Tongjilibo/bert4torch&Date">Star History Chart</a> 
       </td>
     </tr>
   </tbody>
-</table>
+</table>
```

### Comparing `bert4torch-0.2.7.post2/bert4torch/activations.py` & `bert4torch-0.2.8/bert4torch/activations.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.2.7.post2/bert4torch/layers.py` & `bert4torch-0.2.8/bert4torch/layers.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 import numpy as np
 import math
 from bert4torch.snippets import get_sinusoid_encoding_table, take_along_dim, torch_div
 from bert4torch.activations import get_activation
 from typing import List, Optional, Union
 import random
 import warnings
-
+try:
+    import loralib as lora
+except ImportError:
+    lora = None
 
 class LayerNorm(nn.Module):
     def __init__(self, hidden_size, eps=1e-12, conditional_size=False, weight=True, bias=True, norm_mode='normal', **kwargs):
         """layernorm 层，这里自行实现，目的是为了兼容 conditianal layernorm，使得可以做条件文本生成、条件分类等任务
            条件layernorm来自于苏剑林的想法，详情：https://spaces.ac.cn/archives/7124
         """
         super(LayerNorm, self).__init__()
@@ -31,72 +34,77 @@
             # 条件layernorm, 用于条件文本生成,
             # 这里采用全零初始化, 目的是在初始状态不干扰原来的预训练权重
             self.dense1 = nn.Linear(conditional_size, hidden_size, bias=False)
             self.dense1.weight.data.uniform_(0, 0)
             self.dense2 = nn.Linear(conditional_size, hidden_size, bias=False)
             self.dense2.weight.data.uniform_(0, 0)
 
-    def forward(self, x):
-        inputs = x[0]
+    def forward(self, inputs):
+        x = inputs[0]
 
         if self.norm_mode == 'rmsnorm':
             # t5使用的是RMSnorm
-            variance = inputs.to(torch.float32).pow(2).mean(-1, keepdim=True)
-            o = inputs * torch.rsqrt(variance + self.eps)
+            variance = x.float().pow(2).mean(-1, keepdim=True)
+            o = (x.float() * torch.rsqrt(variance + self.eps)).type_as(x)
         else:
-            u = inputs.mean(-1, keepdim=True)
-            s = (inputs - u).pow(2).mean(-1, keepdim=True)
-            o = (inputs - u) / torch.sqrt(s + self.eps)
+            u = x.mean(-1, keepdim=True)
+            s = (x - u).pow(2).mean(-1, keepdim=True)
+            o = (x - u) / torch.sqrt(s + self.eps)
 
         if not hasattr(self, 'weight'):
             self.weight = 1
         if not hasattr(self, 'bias'):
             self.bias = 0
 
         if self.conditional_size:
-            cond = x[1]
-            for _ in range(len(inputs.shape) - len(cond.shape)):
+            cond = inputs[1]
+            for _ in range(len(x.shape) - len(cond.shape)):
                 cond = cond.unsqueeze(dim=1)
             return (self.weight + self.dense1(cond)) * o + (self.bias + self.dense2(cond))
         else:
             return self.weight * o + self.bias
 
 
 class MultiHeadAttentionLayer(nn.Module):
     def __init__(self, hidden_size, num_attention_heads, attention_probs_dropout_prob, dropout_rate=0.1, attention_scale=True,
-                 return_attention_scores=False, bias=True, **kwargs):
+                 output_attentions=False, bias=True, layer_id=None, **kwargs):
         super(MultiHeadAttentionLayer, self).__init__()
         self.hidden_size = hidden_size
         self.num_attention_heads = num_attention_heads
-        # assert hidden_size % num_attention_heads == 0  # 旧逻辑，t5_pegasus_small中不可以整除
-        # 兼容t5_pegasus_small
-        if kwargs.get('attention_head_size'):
-            self.attention_head_size = kwargs.get('attention_head_size')
-        else:
-            self.attention_head_size = int(hidden_size / num_attention_heads)
-        self.inner_dim = self.num_attention_heads * self.attention_head_size  # 新逻辑
+        self.layer_id = layer_id  # 第几层
+        self.is_decoder = kwargs.get('is_decoder', False)
         self.attention_scale = attention_scale
-        self.return_attention_scores = return_attention_scores
-
+        self.output_attentions = output_attentions
         self.bias = bias
-        self.q = nn.Linear(hidden_size, self.inner_dim, bias=bias)
-        self.k = nn.Linear(hidden_size, self.inner_dim, bias=bias)
-        self.v = nn.Linear(hidden_size, self.inner_dim, bias=bias)
-        self.o = nn.Linear(self.inner_dim, hidden_size, bias=bias)
+
+        # t5_pegasus_small中hidden_size/num_attention_heads != 0
+        # 苏神的roberta small中qk的维度和v不同
+        self.attention_head_size = kwargs.get('attention_head_size', int(hidden_size/num_attention_heads))
+        self.attention_key_size = kwargs.get('attention_key_size', self.attention_head_size)
+        self.qk_inner_dim = self.attention_key_size * self.num_attention_heads
+        self.v_inner_dim = self.attention_head_size * self.num_attention_heads
+
+        self.q = nn.Linear(hidden_size, self.qk_inner_dim, bias=bias, device=kwargs['skip_init'])
+        self.k = nn.Linear(hidden_size, self.qk_inner_dim, bias=bias, device=kwargs['skip_init'])
+        self.v = nn.Linear(hidden_size, self.v_inner_dim, bias=bias, device=kwargs['skip_init'])
+        self.o = nn.Linear(self.v_inner_dim, hidden_size, bias=bias, device=kwargs['skip_init'])
         self.dropout = nn.Dropout(attention_probs_dropout_prob)
 
         self.a_bias, self.p_bias = kwargs.get('a_bias'), kwargs.get('p_bias')
 
         if self.p_bias == 'typical_relative':  # nezha
             self.relative_positions_encoding = RelativePositionsEncoding(qlen=kwargs.get('max_position'),
                                                                          klen=kwargs.get('max_position'),
                                                                          embedding_size=self.attention_head_size,
                                                                          max_relative_position=kwargs.get('max_relative_position'))
-        elif self.p_bias == 'rotary':  # roformer
-            self.relative_positions_encoding = RoPEPositionEncoding(max_position=kwargs.get('max_position'), embedding_size=self.attention_head_size)
+        elif self.p_bias == 'rotary':  # roformer, llama, chatglm
+            # position_encoding_2d 目前仅在chatglm中使用
+            self.position_encoding_2d = kwargs.get('position_encoding_2d', False)
+            embedding_size = self.attention_head_size//2 if self.position_encoding_2d else self.attention_head_size
+            self.relative_positions_encoding = RoPEPositionEncoding(embedding_size=embedding_size, rope_rank=kwargs.get('rope_rank', 'adjacent'))
         elif self.p_bias == 't5_relative':  # t5
             self.relative_positions = RelativePositionsEncodingT5(qlen=kwargs.get('max_position'), 
                                                                   klen=kwargs.get('max_position'), 
                                                                   relative_attention_num_buckets=kwargs.get('relative_attention_num_buckets'), 
                                                                   is_decoder=kwargs.get('is_decoder'))
             self.relative_positions_encoding = nn.Embedding(kwargs.get('relative_attention_num_buckets'), self.num_attention_heads)
 
@@ -117,52 +125,79 @@
                                                                          klen=kwargs.get('max_position'), 
                                                                          position_buckets=kwargs.get('position_buckets'),
                                                                          max_position=kwargs.get('max_position'))
             self.relative_positions_encoding = nn.Embedding(kwargs.get('max_position'), self.hidden_size)
             self.norm_rel_ebd = [x.strip() for x in kwargs.get("norm_rel_ebd", "none").lower().split("|")]
             if "layer_norm" in self.norm_rel_ebd:
                 self.layernorm = nn.LayerNorm(self.hidden_size, kwargs.get('layer_norm_eps', 1e-12), elementwise_affine=True)
-
             self.pos_dropout = nn.Dropout(dropout_rate)
 
-    def transpose_for_scores(self, x):
+    def transpose_for_qk_scores(self, x):
+        new_x_shape = x.size()[:-1] + (self.num_attention_heads, self.attention_key_size)
+        x = x.view(*new_x_shape)
+        return x.permute(0, 2, 1, 3)
+    
+    def transpose_for_v_scores(self, x):
         new_x_shape = x.size()[:-1] + (self.num_attention_heads, self.attention_head_size)
         x = x.view(*new_x_shape)
         return x.permute(0, 2, 1, 3)
-
-    def forward(self, hidden_states, attention_mask=None, encoder_hidden_states=None, encoder_attention_mask=None, query_states=None):
+    
+    def forward(self, hidden_states=None, attention_mask=None, encoder_hidden_states=None, encoder_attention_mask=None, past_key_value=None, **model_kwargs):
         # hidden_states shape: [batch_size, seq_q, hidden_size]
         # attention_mask shape: [batch_size, 1, 1, seq_q] 或者 [batch_size, 1, seq_q, seq_q]
         # encoder_hidden_states shape: [batch_size, seq_k, hidden_size]
         # encoder_attention_mask shape: [batch_size, 1, 1, seq_k]
+        # past_key_value shape: ([batch_size, num_attention_heads, key_len_cache, attention_head_size], ...)
+
+        query_layer = self.transpose_for_qk_scores(self.q(hidden_states))
 
-        if query_states is None:
-            query_states = hidden_states  # 在deberta_v2中使用
-        mixed_query_layer = self.q(query_states)
-        if encoder_hidden_states is not None:
-            mixed_key_layer = self.k(encoder_hidden_states)
-            mixed_value_layer = self.v(encoder_hidden_states)
+        # 参考hf增加了关于past_key_value的逻辑
+        if self.p_bias == 'rotary':
+            # rotary有cache情况下，需要先rope后再和past_key_value concat
+            key_layer = self.transpose_for_qk_scores(self.k(hidden_states))
+            value_layer = self.transpose_for_v_scores(self.v(hidden_states))
+        elif (encoder_hidden_states is not None) and past_key_value is not None:
+            key_layer = past_key_value[0]
+            value_layer = past_key_value[1]
             attention_mask = encoder_attention_mask
+        elif encoder_hidden_states is not None:
+            key_layer = self.transpose_for_qk_scores(self.k(encoder_hidden_states))
+            value_layer = self.transpose_for_v_scores(self.v(encoder_hidden_states))
+            attention_mask = encoder_attention_mask
+        elif past_key_value is not None:
+            key_layer = self.transpose_for_qk_scores(self.k(hidden_states))
+            value_layer = self.transpose_for_v_scores(self.v(hidden_states))
+            key_layer = torch.cat([past_key_value[0], key_layer], dim=2)
+            value_layer = torch.cat([past_key_value[1], value_layer], dim=2)
         else:
-            mixed_key_layer = self.k(hidden_states)
-            mixed_value_layer = self.v(hidden_states)
-        # mixed_query_layer shape: [batch_size, query_len, hidden_size]
-        # mixed_query_layer shape: [batch_size, key_len, hidden_size]
-        # mixed_query_layer shape: [batch_size, value_len, hidden_size]
-
-        query_layer = self.transpose_for_scores(mixed_query_layer)
-        key_layer = self.transpose_for_scores(mixed_key_layer)
-        value_layer = self.transpose_for_scores(mixed_value_layer)
+            key_layer = self.transpose_for_qk_scores(self.k(hidden_states))
+            value_layer = self.transpose_for_v_scores(self.v(hidden_states))
         # query_layer shape: [batch_size, num_attention_heads, query_len, attention_head_size]
         # key_layer shape: [batch_size, num_attention_heads, key_len, attention_head_size]
         # value_layer shape: [batch_size, num_attention_heads, value_len, attention_head_size]
 
         if self.p_bias == 'rotary':
-            query_layer = self.relative_positions_encoding(query_layer)
-            key_layer = self.relative_positions_encoding(key_layer)
+            if self.position_encoding_2d:  # chatglm独有逻辑
+                q1, q2 = query_layer.chunk(2, dim=(query_layer.ndim - 1))
+                k1, k2 = key_layer.chunk(2, dim=(key_layer.ndim - 1))
+                q1 = self.relative_positions_encoding(q1, model_kwargs['position_ids'][:, 0, :])
+                k1 = self.relative_positions_encoding(k1, model_kwargs['position_ids'][:, 0, :])
+                q2 = self.relative_positions_encoding(q2, model_kwargs['position_ids'][:, 1, :])
+                k2 = self.relative_positions_encoding(k2, model_kwargs['position_ids'][:, 1, :])
+                query_layer = torch.concat([q1, q2], dim=(q1.ndim - 1))
+                key_layer = torch.concat([k1, k2], dim=(k1.ndim - 1))
+            else:  # 原rotary逻辑
+                query_layer = self.relative_positions_encoding(query_layer, model_kwargs['position_ids'])
+                key_layer = self.relative_positions_encoding(key_layer, model_kwargs['position_ids'])
+            if past_key_value is not None:  # 过了rope再concat
+                key_layer = torch.cat([past_key_value[0], key_layer], dim=2)
+                value_layer = torch.cat([past_key_value[1], value_layer], dim=2)
+
+        if self.is_decoder:
+            past_key_value = (key_layer, value_layer)
 
         # 交换k的最后两个维度，然后q和k执行点积, 获得attention score
         attention_scores = torch.matmul(query_layer, key_layer.transpose(-1, -2))
 
         # attention_scores shape: [batch_size, num_attention_heads, query_len, key_len]
         if (self.p_bias == 'typical_relative') and hasattr(self, 'relative_positions_encoding'):
             relations_keys = self.relative_positions_encoding(attention_scores.shape[-1], attention_scores.shape[-1])  # [to_seq_len, to_seq_len, d_hid]
@@ -196,14 +231,19 @@
             attention_scores = attention_scores + rel_att
 
         elif self.attention_scale:
             attention_scores = attention_scores / math.sqrt(self.attention_head_size)
         # 执行attention mask，对于mask为0部分的attention mask，
         # 值为-1e10，经过softmax后，attention_probs几乎为0，所以不会attention到mask为0的部分
         if attention_mask is not None:
+            # attention_mask最后两维是[q_len, k_ken]，如果维度不匹配补齐，目前是在ptuning_v2中使用
+            if attention_mask.shape[-1] < attention_scores.shape[-1]:
+                size_ = attention_mask.shape[:3] + torch.Size([attention_scores.shape[-1]-attention_mask.shape[-1]])
+                pre_attention_mask = torch.ones(size_).to(attention_mask)
+                attention_mask = torch.cat([pre_attention_mask, attention_mask], dim=-1)
             # attention_mask = attention_mask * attention_mask.squeeze(-2).unsqueeze(-1)  # deberta_v2中使用，但是不使用也不影响
             # attention_scores = attention_scores.masked_fill(attention_mask == 0, -1e10)  # 下一行的另一种写法
             attention_mask = (1.0 - attention_mask) * -10000.0  # 所以传入的mask的非padding部分为1, padding部分为0
             attention_scores = attention_scores + attention_mask
 
         # 将attention score 归一化到0-1
         attention_probs = F.softmax(attention_scores, dim=-1)
@@ -223,27 +263,23 @@
             context_layer = context_layer + value_position_scores_r_t
 
         # context_layer shape: [batch_size, query_len, num_attention_heads, attention_head_size]
         # transpose、permute等维度变换操作后，tensor在内存中不再是连续存储的，而view操作要求tensor的内存连续存储，
         # 所以在调用view之前，需要contiguous来返回一个contiguous copy；
         context_layer = context_layer.permute(0, 2, 1, 3).contiguous()
 
-        new_context_layer_shape = context_layer.size()[:-2] + (self.inner_dim,)
+        new_context_layer_shape = context_layer.size()[:-2] + (self.v_inner_dim,)
         context_layer = context_layer.view(*new_context_layer_shape)
 
         # 是否返回attention scores
-        if self.return_attention_scores:
-            # 这里返回的attention_scores没有经过softmax, 可在外部进行归一化操作
-            return self.o(context_layer), attention_scores
-        else:
-            return self.o(context_layer)
+        outputs = (self.o(context_layer), attention_scores) if self.output_attentions else (self.o(context_layer),)
+        return outputs + (past_key_value,) if self.is_decoder else outputs
 
     def disentangled_attention_bias(self, query_layer, key_layer, relative_pos, rel_embeddings, scale_factor):
-        '''deberta_v2使用，和原版区别是query_layer是4维
-        '''
+        '''deberta_v2使用，和原版区别是query_layer是4维'''
         btz, n_head, q_len, d_head = query_layer.size()
         k_len = key_layer.size(-2)
         if relative_pos is None:
             relative_pos = self.relative_positions(q_len, k_len)
         if relative_pos.dim() == 2:
             relative_pos = relative_pos.unsqueeze(0).unsqueeze(0)
         elif relative_pos.dim() == 3:
@@ -253,16 +289,16 @@
             raise ValueError(f"Relative position ids must be of dim 2 or 3 or 4. {relative_pos.dim()}")
 
         att_span = self.pos_ebd_size
         relative_pos = relative_pos.long().to(query_layer.device)
 
         rel_embeddings = rel_embeddings[0 : att_span * 2, :].unsqueeze(0)
         if self.share_att_key:
-            pos_query_layer = self.transpose_for_scores(self.q(rel_embeddings)).repeat(btz, 1, 1, 1)
-            pos_key_layer = self.transpose_for_scores(self.k(rel_embeddings)).repeat(btz, 1, 1, 1)
+            pos_query_layer = self.transpose_for_qk_scores(self.q(rel_embeddings)).repeat(btz, 1, 1, 1)
+            pos_key_layer = self.transpose_for_qk_scores(self.k(rel_embeddings)).repeat(btz, 1, 1, 1)
         else:
             # 这里逻辑去掉了
             pass
 
         score = 0
         # content->position
         if "c2p" in self.pos_att_type:
@@ -296,16 +332,16 @@
         # 这样不统一做法的原因不得而知，不过有没有这一层，差别可能不会很大；
 
         # 为了适配是否dropout，用is_dropout，dropout_rate两个参数控制；如果是实现原始的transformer，直接使用默认参数即可；如果是实现bert，则is_dropout为False，此时的dropout_rate参数并不会使用.
         super(PositionWiseFeedForward, self).__init__()
 
         self.is_dropout = is_dropout
         self.intermediate_act_fn = get_activation(hidden_act)
-        self.intermediateDense = nn.Linear(hidden_size, intermediate_size, bias=bias)
-        self.outputDense = nn.Linear(intermediate_size, hidden_size, bias=bias)
+        self.intermediateDense = nn.Linear(hidden_size, intermediate_size, bias=bias, device=kwargs['skip_init'])
+        self.outputDense = nn.Linear(intermediate_size, hidden_size, bias=bias, device=kwargs['skip_init'])
         if self.is_dropout:
             self.dropout = nn.Dropout(dropout_rate)
 
     def forward(self, x):
         # x shape: (batch size, seq len, hidden_size)
         if self.is_dropout:
             x = self.dropout(self.intermediate_act_fn(self.intermediateDense(x)))
@@ -339,15 +375,15 @@
         self.dropout = nn.Dropout(attention_probs_dropout_prob)
         self.i_dense = nn.Linear(hidden_size, self.intermediate_size*2+attention_key_size, bias=bias)
         self.offsetscale = self.OffsetScale(attention_key_size, heads=2, bias=bias)
         self.o_dense = nn.Linear(self.intermediate_size, hidden_size, bias=bias)
         
         self.a_bias, self.p_bias = kwargs.get('a_bias'), kwargs.get('p_bias')
         if self.p_bias == 'rotary':  # RoPE
-            self.relative_positions_encoding = RoPEPositionEncoding(max_position=kwargs.get('max_position'), embedding_size=self.attention_head_size)
+            self.relative_positions_encoding = RoPEPositionEncoding(embedding_size=self.attention_head_size)
 
     def forward(self, hidden_states, attention_mask):
         # 投影变换
         hidden_states = self.hidden_fn(self.i_dense(hidden_states))
         u, v, qk = hidden_states.split([self.intermediate_size, self.intermediate_size, self.attention_head_size], dim=-1)
         q, k = self.offsetscale(qk)  # 仿射变换
 
@@ -391,16 +427,15 @@
             if method == 'squared_relu':
                 return F.relu(a)**2 / l
             elif method == 'softmax_plus':
                 return F.softmax(a * torch.log(l) / torch.log(torch.tensor(512.0)).to(mask), dim=dim)
         return a
 
     class OffsetScale(nn.Module):
-        '''仿射变换
-        '''
+        '''仿射变换'''
         def __init__(self, head_size, heads=1, bias=True):
             super().__init__()
             self.gamma = nn.Parameter(torch.ones(heads, head_size))
             self.bias = bias
             if bias:
                 self.beta = nn.Parameter(torch.zeros(heads, head_size))
             nn.init.normal_(self.gamma, std = 0.02)
@@ -412,46 +447,46 @@
             return out.unbind(dim = -2)
 
 
 class BertEmbeddings(nn.Module):
     """embeddings层
        构造word, position and token_type embeddings.
     """
-    def __init__(self, vocab_size, embedding_size, hidden_size, max_position, segment_vocab_size, shared_segment_embeddings, dropout_rate, conditional_size=False, token_pad_ids=0, **kwargs):
+    def __init__(self, vocab_size, embedding_size, hidden_size, max_position, segment_vocab_size, shared_segment_embeddings, dropout_rate, conditional_size=False, pad_token_id=0, **kwargs):
         super(BertEmbeddings, self).__init__()
         self.shared_segment_embeddings = shared_segment_embeddings
-        self.word_embeddings = nn.Embedding(vocab_size, embedding_size, padding_idx=token_pad_ids)
+        self.word_embeddings = nn.Embedding(vocab_size, embedding_size, padding_idx=pad_token_id, device=kwargs['skip_init'])
 
         # 位置编码
         if kwargs.get('p_bias') == 'sinusoid':
             self.position_embeddings = SinusoidalPositionEncoding(max_position, embedding_size)
         elif kwargs.get('p_bias') in {'rotary', 'typical_relative', 't5_relative', 'other_relative', 'deberta_v2'}:
             # 如果使用相对位置编码，则不声明PositionEmbeddings
             pass
         elif max_position > 0:
-            self.position_embeddings = nn.Embedding(max_position, embedding_size)
+            self.position_embeddings = nn.Embedding(max_position, embedding_size, device=kwargs['skip_init'])
         
         # segement编码
         if (segment_vocab_size > 0) and (not shared_segment_embeddings) and kwargs.get('use_segment_embedding', True):
             # use_segment_embedding用于lm, unilm场景，不使用segment_embeddings但是传入segment_ids用于计算mask
             # 一般无需设置，目前仅在guwenbert中使用
-            self.segment_embeddings = nn.Embedding(segment_vocab_size, embedding_size)
+            self.segment_embeddings = nn.Embedding(segment_vocab_size, embedding_size, device=kwargs['skip_init'])
 
         # emb_scale
         self.emb_scale = kwargs.get('emb_scale', 1)  # transform_xl, xlnet特有
 
         # LayerNorm
-        self.layerNorm = LayerNorm(embedding_size, eps=1e-12, conditional_size=conditional_size, **kwargs)
+        self.layerNorm = LayerNorm(embedding_size, eps=kwargs.get('layer_norm_eps', 1e-12), conditional_size=conditional_size, **kwargs)
         self.dropout = nn.Dropout(dropout_rate)
 
         # 如果embedding_size != hidden_size，则再有一个linear(适用于albert矩阵分解)
         if embedding_size != hidden_size:
-            self.embedding_hidden_mapping_in = nn.Linear(embedding_size, hidden_size)
+            self.embedding_hidden_mapping_in = nn.Linear(embedding_size, hidden_size, device=kwargs['skip_init'])
 
-    def forward(self, token_ids, segment_ids=None, position_ids=None, conditional_emb=None, additional_embs=None, attention_mask=None):
+    def forward(self, token_ids=None, segment_ids=None, position_ids=None, conditional_emb=None, additional_embs=None, attention_mask=None):
         if (not token_ids.requires_grad) and (token_ids.dtype in {torch.long, torch.int}):
             words_embeddings = self.word_embeddings(token_ids)
         else:
             words_embeddings = token_ids  # 自定义word_embedding，目前仅有VAT中使用
 
         if hasattr(self, 'segment_embeddings'):
             segment_ids = torch.zeros_like(token_ids) if segment_ids is None else segment_ids
@@ -465,19 +500,17 @@
             embeddings = words_embeddings
         
         # 额外的embedding，如词性等
         if additional_embs is not None:
             for emb in additional_embs:
                 embeddings += emb
 
-        if hasattr(self, 'position_embeddings'):
-            seq_length = token_ids.size(1)
-            if position_ids is None:
-                position_ids = torch.arange(seq_length, dtype=torch.long, device=token_ids.device)
-                position_ids = position_ids.unsqueeze(0).repeat(token_ids.shape[0], 1)
+        if hasattr(self, 'position_embeddings') and (position_ids is not None):
+            if position_ids.shape[0] == 1:
+                position_ids = position_ids.repeat(token_ids.shape[0], 1)
             position_embeddings = self.position_embeddings(position_ids)
             embeddings += position_embeddings
 
         if self.emb_scale != 1:
             embeddings = embeddings * self.emb_scale  # transform_xl, xlnet特有
 
         if hasattr(self, 'layerNorm'):
@@ -499,83 +532,101 @@
 
        注意:
         1. 以上都不计dropout层，并不代表没有dropout，每一层的dropout使用略有不同，注意区分
         2. 原始的Transformer的encoder中的Feed Forward层一共有两层linear，
         3. config.intermediate_size的大小不仅是第一层linear的输出尺寸，也是第二层linear的输入尺寸
     """
     def __init__(self, hidden_size, num_attention_heads, dropout_rate, attention_probs_dropout_prob, intermediate_size, hidden_act, 
-                 is_dropout=False, conditional_size=False, **kwargs):
+                 is_dropout=False, conditional_size=False, pre_post_norm='post', **kwargs):
         super(BertLayer, self).__init__()
         self.multiHeadAttention = MultiHeadAttentionLayer(hidden_size, num_attention_heads, attention_probs_dropout_prob, dropout_rate, **kwargs)
         self.dropout1 = nn.Dropout(dropout_rate)
-        self.layerNorm1 = LayerNorm(hidden_size, eps=1e-12, conditional_size=conditional_size, **kwargs)
+        layer_norm_eps = kwargs.get('layer_norm_eps', 1e-12)
+        self.layerNorm1 = LayerNorm(hidden_size, eps=layer_norm_eps, conditional_size=conditional_size, **kwargs)
         self.feedForward = PositionWiseFeedForward(hidden_size, intermediate_size, dropout_rate, hidden_act, is_dropout=is_dropout, **kwargs)
         self.dropout2 = nn.Dropout(dropout_rate)
-        self.layerNorm2 = LayerNorm(hidden_size, eps=1e-12, conditional_size=conditional_size, **kwargs)
-        self.is_decoder = kwargs.get('is_decoder')
-        if self.is_decoder:
+        self.layerNorm2 = LayerNorm(hidden_size, eps=layer_norm_eps, conditional_size=conditional_size, **kwargs)
+        self.pre_post_norm = pre_post_norm
+        self.is_decoder = kwargs.get('is_decoder', False)
+        self.add_cross_attention = kwargs.get('add_cross_attention', False)
+        if self.add_cross_attention and self.is_decoder:
             self.crossAttention = MultiHeadAttentionLayer(hidden_size, num_attention_heads, attention_probs_dropout_prob, dropout_rate, **kwargs)
             self.dropout3 = nn.Dropout(dropout_rate)
-            self.layerNorm3 = LayerNorm(hidden_size, eps=1e-12, conditional_size=conditional_size, **kwargs)
+            self.layerNorm3 = LayerNorm(hidden_size, eps=layer_norm_eps, conditional_size=conditional_size, **kwargs)
 
-    def forward(self, hidden_states, attention_mask, conditional_emb=None, encoder_hidden_states=None, encoder_attention_mask=None):
-        self_attn_output = self.multiHeadAttention(hidden_states, attention_mask)  # self.decoder为true时候，这里的attention_mask是三角的
-        hidden_states = hidden_states + self.dropout1(self_attn_output)
-        hidden_states = self.layerNorm1((hidden_states, conditional_emb))
+    def forward(self, hidden_states=None, attention_mask=None, conditional_emb=None, encoder_hidden_states=None, encoder_attention_mask=None, past_key_value=None, cross_past_key_value=None, **model_kwargs):
+        # self attention
+        x = self.layerNorm1((hidden_states, conditional_emb)) if self.pre_post_norm == 'pre' else hidden_states
+        self_attn_output = self.multiHeadAttention(x, attention_mask, past_key_value=past_key_value, **model_kwargs)  # self.decoder为true时候，这里的attention_mask是三角的
+        hidden_states = hidden_states + self.dropout1(self_attn_output[0])
+        if self.pre_post_norm == 'post':
+            hidden_states = self.layerNorm1((hidden_states, conditional_emb))
         
         # cross attention
         if self.is_decoder and encoder_hidden_states is not None:
-            cross_attn_output = self.crossAttention(hidden_states, None, encoder_hidden_states, encoder_attention_mask)
-            hidden_states = hidden_states + self.dropout3(cross_attn_output)
-            hidden_states = self.layerNorm3((hidden_states, conditional_emb))
-            
-        self_attn_output2 = self.feedForward(hidden_states)
-        hidden_states = hidden_states + self.dropout2(self_attn_output2)
-        hidden_states = self.layerNorm2((hidden_states, conditional_emb))
-        return hidden_states
+            cross_attn_output = self.crossAttention(hidden_states, None, encoder_hidden_states, encoder_attention_mask, cross_past_key_value, **model_kwargs)
+            hidden_states = hidden_states + self.dropout3(cross_attn_output[0])
+            model_kwargs['cross_past_key_value'] = cross_attn_output[-1]
+            if self.pre_post_norm == 'post':
+                hidden_states = self.layerNorm3((hidden_states, conditional_emb))
+
+        # feedforward
+        x = self.layerNorm2((hidden_states, conditional_emb)) if self.pre_post_norm == 'pre' else hidden_states
+        feedforward_output = self.feedForward(x)
+        hidden_states = hidden_states + self.dropout2(feedforward_output)
+        if self.pre_post_norm == 'post':
+            hidden_states = self.layerNorm2((hidden_states, conditional_emb))
+        
+        if self.is_decoder:
+            model_kwargs['past_key_value'] = self_attn_output[-1]
+        model_kwargs['hidden_states'] = hidden_states
+        return model_kwargs
 
 
 class T5Layer(BertLayer):
     """T5的Encoder的主体是基于Self-Attention的模块
     顺序：LN --> Att --> Add --> LN --> FFN --> Add
     """
     def __init__(self, *args, version='t5.1.0', **kwargs):
         super().__init__(*args, **kwargs)
 
         # 如果是t5.1.1结构，则FFN层需要变更
         if version.endswith('t5.1.1'):
-            kwargs['dropout_rate'] = args[2]
-            kwargs['hidden_act'] = args[5]
-            self.feedForward = self.T5PositionWiseFeedForward(hidden_size=args[0], intermediate_size=args[4], **kwargs)
+            self.feedForward = self.T5PositionWiseFeedForward(**kwargs)
 
         # decoder中间有crossAttention
-        if self.is_decoder and hasattr(self.crossAttention, 'relative_positions_encoding'):
+        if self.add_cross_attention and self.is_decoder and hasattr(self.crossAttention, 'relative_positions_encoding'):
             del self.crossAttention.relative_positions_encoding
             del self.crossAttention.relative_positions
 
-    def forward(self, hidden_states, attention_mask, conditional_emb=None, encoder_hidden_states=None, encoder_attention_mask=None):
+    def forward(self, hidden_states=None, attention_mask=None, conditional_emb=None, encoder_hidden_states=None, encoder_attention_mask=None, past_key_value=None, cross_past_key_value=None, **model_kwargs):
         # bert的layernorm是在attn/ffc之后，Openai-gpt2是在之前
         x = self.layerNorm1((hidden_states, conditional_emb))
-        self_attn_output = self.multiHeadAttention(x, attention_mask)
-        hidden_states = hidden_states + self.dropout1(self_attn_output)
+        self_attn_output = self.multiHeadAttention(x, attention_mask, past_key_value=past_key_value)
+        hidden_states = hidden_states + self.dropout1(self_attn_output[0])
 
         # cross attention
         if self.is_decoder and encoder_hidden_states is not None:
             x = self.layerNorm3((hidden_states, conditional_emb))
-            cross_attn_output = self.crossAttention(x, None, encoder_hidden_states, encoder_attention_mask)
-            hidden_states = hidden_states + self.dropout3(cross_attn_output)
+            cross_attn_output = self.crossAttention(x, None, encoder_hidden_states, encoder_attention_mask, cross_past_key_value)
+            hidden_states = hidden_states + self.dropout3(cross_attn_output[0])
+            model_kwargs['cross_past_key_value'] = cross_attn_output[-1]
 
+        # feed forward
         x = self.layerNorm2((hidden_states, conditional_emb))
         ffn_output = self.feedForward(x)
         hidden_states = hidden_states + self.dropout2(ffn_output)
-        return hidden_states
+
+        if self.is_decoder:
+            model_kwargs['past_key_value'] = self_attn_output[-1]
+        model_kwargs['hidden_states'] = hidden_states
+        return model_kwargs
 
     class T5PositionWiseFeedForward(PositionWiseFeedForward):
-        '''参考transformer包: https://github.com/huggingface/transformers/blob/main/src/transformers/models/t5/modeling_t5.py
-        '''
+        '''参考transformer包: https://github.com/huggingface/transformers/blob/main/src/transformers/models/t5/modeling_t5.py'''
         def __init__(self, hidden_size, intermediate_size, **kwargs):
             super().__init__(hidden_size, intermediate_size, **kwargs)
             self.intermediateDense = nn.Linear(hidden_size, intermediate_size, bias=False)
             self.intermediateDense1 = nn.Linear(hidden_size, intermediate_size, bias=False)
             self.outputDense = nn.Linear(intermediate_size, hidden_size, bias=False)
 
         def forward(self, x):
@@ -599,37 +650,37 @@
     '''
     def __init__(self, hidden_size, num_attention_heads, dropout_rate, attention_probs_dropout_prob, intermediate_size, hidden_act, **kwargs):
         super().__init__(hidden_size, num_attention_heads, dropout_rate, attention_probs_dropout_prob, intermediate_size, hidden_act, **kwargs)
         self.pre_lnorm = kwargs.get('pre_lnorm')
         # multiattn层无bias
         self.multiHeadAttention = self.RelPartialLearnableMultiHeadAttn(hidden_size, num_attention_heads, attention_probs_dropout_prob, bias=False, **kwargs)
 
-    def forward(self, hidden_states, segment_ids, pos_emb, attention_mask, mems_i, conditional_emb=None):
+    def forward(self, hidden_states=None, segment_ids=None, pos_emb=None, attention_mask=None, mems_i=None, conditional_emb=None, **model_kwargs):
         # 拼接mems和query，mems_i: [btz, m_len, hdsz], w: [btz, q_len, hdsz] = [btz, k_len, hdsz]
         hidden_states_cat = torch.cat([mems_i, hidden_states], 1) if mems_i is not None else hidden_states
         
         # Attn
         if self.pre_lnorm:
             hidden_states_cat = self.layerNorm1((hidden_states_cat, conditional_emb))
         self_attn_output = self.multiHeadAttention(hidden_states, hidden_states_cat, pos_emb, attention_mask, segment_ids)
-        hidden_states = hidden_states + self.dropout1(self_attn_output)
+        hidden_states = hidden_states + self.dropout1(self_attn_output[0])
         if not self.pre_lnorm:  # post_lnorm
             hidden_states = self.layerNorm1((hidden_states, conditional_emb))
 
         # FFN
         x = self.layerNorm2((hidden_states, conditional_emb)) if self.pre_lnorm else hidden_states
         self_attn_output2 = self.feedForward(x)
         hidden_states = hidden_states + self.dropout2(self_attn_output2)
         if not self.pre_lnorm:  # post_lnorm
             hidden_states = self.layerNorm2((hidden_states, conditional_emb))
-        return hidden_states
+        model_kwargs['hidden_states'] = hidden_states
+        return model_kwargs
 
     class RelPartialLearnableMultiHeadAttn(MultiHeadAttentionLayer):
-        '''Transformer_XL式相对位置编码, 这里修改成了MultiHeadAttentionLayer的batch_first代码格式
-        '''
+        '''Transformer_XL式相对位置编码, 这里修改成了MultiHeadAttentionLayer的batch_first代码格式'''
         def __init__(self, *args, r_w_bias=None, r_r_bias=None, r_s_bias=None, **kwargs):
             super().__init__(*args, **kwargs)
             segment_vocab_size = kwargs.get('segment_vocab_size')
             if r_r_bias is None or r_w_bias is None:  # Biases are not shared
                 self.r_r_bias = nn.Parameter(torch.FloatTensor(self.num_attention_heads, self.attention_head_size))  # 全局内容偏置
                 self.r_w_bias = nn.Parameter(torch.FloatTensor(self.num_attention_heads, self.attention_head_size))  # 全局位置偏置
                 if segment_vocab_size > 0:
@@ -643,30 +694,28 @@
                 self.seg_embed = nn.Parameter(torch.FloatTensor(segment_vocab_size, self.num_attention_heads, self.attention_head_size))
 
             self.r = nn.Linear(self.hidden_size, self.hidden_size, bias=self.bias)
             self.rel_shift_opt = kwargs.get('rel_shift_opt')
 
         @staticmethod
         def rel_shift(x, zero_triu=False):
-            '''transformer_xl使用, 向左shift让右上角都是0, 对角线是同一个值, x: [btz, n_head, q_len, k_len]
-            '''
+            '''transformer_xl使用, 向左shift让右上角都是0, 对角线是同一个值, x: [btz, n_head, q_len, k_len]'''
             q_len, k_len = x.size(2), x.size(-1)
             zero_pad = torch.zeros((*x.size()[:2], q_len, 1), device=x.device, dtype=x.dtype)
             x_padded = torch.cat([zero_pad, x], dim=-1)
             x_padded = x_padded.view(*x.size()[:2], k_len + 1, q_len)
             x = x_padded[:,:,1:,:].view_as(x)
             if zero_triu:
                 ones = torch.ones((q_len, k_len), device=x.device)
                 x = x * torch.tril(ones, k_len - q_len)[None,None,:,:]
             return x
 
         @staticmethod
         def rel_shift_bnij(x, klen=-1):
-            ''' xlnet使用
-            '''
+            ''' xlnet使用'''
             x_size = x.shape
             x = x.reshape(x_size[0], x_size[1], x_size[3], x_size[2])
             x = x[:, :, 1:, :]
             x = x.reshape(x_size[0], x_size[1], x_size[2], x_size[3] - 1)
             x = torch.index_select(x, 3, torch.arange(klen, device=x.device, dtype=torch.long))
             # x = x[:, :, :, :klen]
             return x
@@ -675,17 +724,17 @@
             # w: 词向量[btz, q_len, hdsz], cat: w和mem_i拼接后向量[btz, k_len, hdsz], r：相对位置向量[r_len, hdsz]
             qlen, rlen, bsz = w.size(1), r.size(0), w.size(0)
             
             mixed_query_layer = self.q(cat)[:, -qlen:, :]  # 仅取用query部分，不适用mem部分
             mixed_key_layer = self.k(cat)
             mixed_value_layer = self.v(cat)
 
-            w_head_q = self.transpose_for_scores(mixed_query_layer)  # [btz, n_head, q_len, d_head]
-            w_head_k = self.transpose_for_scores(mixed_key_layer)  # [btz, n_head, k_len, d_head]
-            w_head_v = self.transpose_for_scores(mixed_value_layer)  # [btz, n_head, k_len, d_head]
+            w_head_q = self.transpose_for_qk_scores(mixed_query_layer)  # [btz, n_head, q_len, d_head]
+            w_head_k = self.transpose_for_qk_scores(mixed_key_layer)  # [btz, n_head, k_len, d_head]
+            w_head_v = self.transpose_for_v_scores(mixed_value_layer)  # [btz, n_head, k_len, d_head]
 
             r_head_k = self.r(r)  # [hdsz, nhead*headsize] = [r_len, 1, nhead*headsize]
             r_head_k = r_head_k.view(rlen, self.num_attention_heads, self.attention_head_size)  # rlen x n_head x d_head
 
             #### compute attention score
             rw_head_q = w_head_q + self.r_w_bias.unsqueeze(1)  # [btz, n_head, q_len, d_head]
             AC = torch.einsum('bnid,bnjd->bnij', (rw_head_q, w_head_k))  # [btz, n_head, q_len, k_len]
@@ -724,19 +773,16 @@
             attention_probs = self.dropout(attention_probs)
             context_layer = torch.matmul(attention_probs, w_head_v)  # [batch_size, num_attention_heads, query_len, attention_head_size]
             context_layer = context_layer.permute(0, 2, 1, 3).contiguous()
             new_context_layer_shape = context_layer.size()[:-2] + (self.hidden_size,)
             context_layer = context_layer.view(*new_context_layer_shape)
 
             # 是否返回attention scores
-            if self.return_attention_scores:
-                # 这里返回的attention_scores没有经过softmax, 可在外部进行归一化操作
-                return self.o(context_layer), attention_scores
-            else:
-                return self.o(context_layer)
+            outputs = (self.o(context_layer), attention_scores) if self.output_attentions else (self.o(context_layer),)
+            return outputs
 
 
 class AdaptiveEmbedding(nn.Module):
     '''Transformer_XL的自适应embedding, 实现不同区间使用不同的维度
     可以实现如高频词用比如1024或512维，低频词用256或64维, 再用Linear层project到相同的维数
     '''
     def __init__(self, vocab_size, embedding_size, hidden_size, cutoffs, div_val=1, sample_softmax=False, **kwargs):
@@ -790,20 +836,20 @@
             embed = emb_flat.view(embed_shape)
 
         embed.mul_(self.emb_scale)
 
         return embed
 
 
-class Identity(nn.Module):
+class BlockIdentity(nn.Module):
     def __init__(self, *args, **kwargs):
-        super(Identity, self).__init__()
+        super(BlockIdentity, self).__init__()
 
-    def forward(self, *args):
-        return args[0]
+    def forward(self, *args, **kwargs):
+        return kwargs
 
 
 class XlnetPositionsEncoding(nn.Module):
     '''Xlnet, transformer_xl使用的相对位置编码
        和SinusoidalPositionEncoding区别是一个是间隔排列, 一个是前后排列
     '''
     def __init__(self, embedding_size):
@@ -944,30 +990,63 @@
     def forward(self, position_ids):
         return self.position_embeddings(position_ids)
 
 
 class RoPEPositionEncoding(nn.Module):
     """旋转式位置编码: https://kexue.fm/archives/8265
     """
-    def __init__(self, max_position, embedding_size):
+    def __init__(self, embedding_size, rope_rank='adjacent', **kwargs):
         super(RoPEPositionEncoding, self).__init__()
-        position_embeddings = get_sinusoid_encoding_table(max_position, embedding_size)  # [seq_len, hdsz]
-        cos_position = position_embeddings[:, 1::2].repeat_interleave(2, dim=-1)  # [seq_len, hdsz]
-        sin_position = position_embeddings[:, ::2].repeat_interleave(2, dim=-1)  # [seq_len, hdsz]
-        # register_buffer是为了最外层model.to(device)，不用内部指定device
-        self.register_buffer('cos_position', cos_position)
-        self.register_buffer('sin_position', sin_position)
+        self.max_seq_len_cache = -1
+        self.embedding_size = embedding_size
+        # 支持两种方式，一种是奇偶相邻排列，一种是上下排列, 目前只在chatglm中看到updown排列
+        assert rope_rank in {'adjacent', 'updown'}, "rank kwarg only support 'adjacent' and 'updown' "
+        self.rope_rank = rope_rank
+    
+    def initialize(self, max_position):
+        position_embeddings = get_sinusoid_encoding_table(max_position, self.embedding_size)  # [seq_len, hdsz]
+        if self.rope_rank == 'adjacent':
+            cos_position = position_embeddings[:, 1::2].repeat_interleave(2, dim=-1)  # [seq_len, hdsz]
+            sin_position = position_embeddings[:, ::2].repeat_interleave(2, dim=-1)  # [seq_len, hdsz]
+        elif self.rope_rank == 'updown':  # 目前仅chatglm使用
+            cos_position = position_embeddings[:, 1::2].repeat(1,2)  # [seq_len, hdsz]
+            sin_position = position_embeddings[:, ::2].repeat(1,2)  # [seq_len, hdsz]
+        else:
+            raise ValueError('Args `rope_rank` only support `adjacent` and `adjacent` mode')
+        return cos_position, sin_position
     
-    def forward(self, qw, seq_dim=-2):
+    def forward(self, qw, position_ids=None, seq_dim=-2):
         # MultiHeadAttentionLayer中qw是[btz, n_heads, seq_len, head_size]
         # GlobalPointer中*转置*后qw是[btz, n_heads, seq_len, head_size]
         # EfficientGlobalPointer中qw是[btz, seq_len, head_size]
-        seq_len = qw.shape[seq_dim]
-        qw2 = torch.stack([-qw[..., 1::2], qw[..., ::2]], dim=-1).reshape_as(qw)
-        return qw * self.cos_position[:seq_len] + qw2 * self.sin_position[:seq_len]
+        if self.rope_rank == 'adjacent':
+            qw2 = torch.stack([-qw[..., 1::2], qw[..., ::2]], dim=-1).reshape_as(qw)
+        elif self.rope_rank == 'updown':  # 目前仅chatglm使用
+            qw2 = torch.cat([-qw[..., qw.shape[-1]//2:], qw[..., :qw.shape[-1]//2]], dim=-1)  # cat和stack+reshape是结果不同的
+        
+        # 超过缓存长度
+        seq_len = position_ids.max() + 1 if position_ids is not None else qw.shape[seq_dim]
+        if seq_len > self.max_seq_len_cache:
+            cos_position, sin_position = self.initialize(seq_len)
+            self.cos_position, self.sin_position = cos_position.type_as(qw).to(qw.device), sin_position.type_as(qw).to(qw.device)
+            self.max_seq_len_cache = seq_len
+
+        # 传入position_ids来获取cos和sin, 主要是在use_states时候能直接取到对应位置的编码
+        if position_ids is not None:
+            # position_ids: [btz, seq_len]
+            cos = F.embedding(position_ids, self.cos_position)  # [btz, seq_len, hdsz]
+            sin = F.embedding(position_ids, self.sin_position)
+        else:
+            cos = self.cos_position[:seq_len]  # [seq_len, hdsz]
+            sin = self.sin_position[:seq_len]
+
+        if cos.dim() < qw.dim():
+            cos = cos.unsqueeze(seq_dim-1)
+            sin = sin.unsqueeze(seq_dim-1)
+        return qw * cos + qw2 * sin
 
 
 class CRF(nn.Module):
     '''Conditional random field: https://github.com/lonePatient/BERT-NER-Pytorch/blob/master/models/layers/crf.py
     '''
     def __init__(self, num_tags: int, init_transitions: Optional[List[np.ndarray]] = None, freeze=False) -> None:
         if num_tags <= 0:
@@ -1024,16 +1103,15 @@
             return llh.sum()
         if reduction == 'mean':
             return llh.mean()
         return llh.sum() / mask.float().sum()
 
     def decode(self, emissions: torch.Tensor, mask: Optional[torch.ByteTensor] = None,
                nbest: Optional[int] = None, pad_tag: Optional[int] = None) -> List[List[List[int]]]:
-        """Find the most likely tag sequence using Viterbi algorithm.
-        """
+        """Find the most likely tag sequence using Viterbi algorithm."""
         if nbest is None:
             nbest = 1
         if mask is None:
             mask = torch.ones(emissions.shape[:2], dtype=torch.uint8, device=emissions.device)
         if mask.dtype != torch.uint8:
             mask = mask.byte()
         self._validate(emissions, mask=mask)
@@ -1250,24 +1328,24 @@
 
 
 class GlobalPointer(nn.Module):
     """全局指针模块
     将序列的每个(start, end)作为整体来进行判断
     参考：https://kexue.fm/archives/8373
     """
-    def __init__(self, hidden_size, heads, head_size, RoPE=True, max_len=512, use_bias=True, tril_mask=True):
+    def __init__(self, hidden_size, heads, head_size, RoPE=True, use_bias=True, tril_mask=True):
         super().__init__()
         self.heads = heads
         self.head_size = head_size
         self.RoPE = RoPE
         self.tril_mask = tril_mask
 
         self.dense = nn.Linear(hidden_size, heads * head_size * 2, bias=use_bias)
         if self.RoPE:
-            self.position_embedding = RoPEPositionEncoding(max_len, head_size)
+            self.position_embedding = RoPEPositionEncoding(head_size)
 
     def forward(self, inputs, mask=None):
         ''' 
         :param inputs: shape=[..., hdsz]
         :param mask: shape=[btz, seq_len], padding部分为0
         '''
         sequence_output = self.dense(inputs)  # [..., heads*head_size*2]
@@ -1299,25 +1377,25 @@
 
 
 class EfficientGlobalPointer(nn.Module):
     """更加参数高效的GlobalPointer
     参考：https://kexue.fm/archives/8877
     这里实现和GlobalPointer相似，而未采用原版的奇偶位来取qw和kw，个人理解两种方式是无区别的
     """
-    def __init__(self, hidden_size, heads, head_size, RoPE=True, max_len=512, use_bias=True, tril_mask=True):
+    def __init__(self, hidden_size, heads, head_size, RoPE=True, use_bias=True, tril_mask=True):
         super().__init__()
         self.heads = heads
         self.head_size = head_size
         self.RoPE = RoPE
         self.tril_mask = tril_mask
 
         self.p_dense = nn.Linear(hidden_size, head_size * 2, bias=use_bias)
         self.q_dense = nn.Linear(head_size * 2, heads * 2, bias=use_bias)
         if self.RoPE:
-            self.position_embedding = RoPEPositionEncoding(max_len, head_size)
+            self.position_embedding = RoPEPositionEncoding(head_size)
 
     def forward(self, inputs, mask=None):
         ''' 
         :param inputs: shape=[..., hdsz]
         :param mask: shape=[btz, seq_len], padding部分为0
         '''
         sequence_output = self.p_dense(inputs)  # [..., head_size*2]
@@ -1345,16 +1423,15 @@
         if self.tril_mask:
             logits = logits - torch.tril(torch.ones_like(logits), -1) * 1e12
 
         return logits
 
 
 class TplinkerHandshakingKernel(nn.Module):
-    '''Tplinker的HandshakingKernel实现
-    '''
+    '''Tplinker的HandshakingKernel实现'''
     def __init__(self, hidden_size, shaking_type, inner_enc_type=''):
         super().__init__()
         self.shaking_type = shaking_type
         if shaking_type == "cat":
             self.combine_fc = nn.Linear(hidden_size * 2, hidden_size)
         elif shaking_type == "cat_plus":
             self.combine_fc = nn.Linear(hidden_size * 3, hidden_size)
@@ -1522,16 +1599,15 @@
         '''计算loss
         '''
         y_true1 = y_true[self.perm_index]
         return self.lam * criterion(y_pred, y_true) + (1 - self.lam) * criterion(y_pred, y_true1)
 
 
 class ConvLayer(nn.Module):
-    '''deberta_v2中使用
-    '''
+    '''deberta_v2中使用'''
     def __init__(self, hidden_size, dropout_rate=0.1, layer_norm_eps=1e-12, conv_kernel_size=3, conv_groups=1, conv_act="tanh", **kwargs):
         super().__init__()
         kernel_size = conv_kernel_size
         groups = conv_groups
         self.conv_act = conv_act
         self.conv = nn.Conv1d(hidden_size, hidden_size, kernel_size, padding=(kernel_size - 1) // 2, groups=groups)
         self.LayerNorm = nn.LayerNorm(hidden_size, layer_norm_eps)  # 这里使用bert4torch的LayerNorm会有问题
@@ -1557,19 +1633,66 @@
             input_mask = input_mask.to(output.dtype)
             output_states = output * input_mask
 
         return output_states
 
 
 class MultiSampleDropout(nn.Module):
-    """multisample dropout (wut): https://arxiv.org/abs/1905.09788
-    """
+    """multisample dropout (wut): https://arxiv.org/abs/1905.09788"""
     def __init__(self, hidden_size, num_labels, K=5, p=0.5):
         super().__init__()
         self.K = K
         self.dropout = nn.Dropout(p)
         self.classifier = nn.Linear(hidden_size, num_labels)
 
     def forward(self, input):
         logits = torch.stack([self.classifier(self.dropout(input)) for _ in range(self.K)], dim=0)
         logits = torch.mean(logits, dim=0)
-        return logits
+        return logits
+
+
+class BottleneckAdapterLayer(nn.Module):
+    '''BottleneckAdapterLayer'''
+    def __init__(self, adapter_input_size, bottleneck_size, adapter_non_linearity='gelu'):
+        super().__init__()
+        self.adapter_input_size = adapter_input_size
+        self.bottleneck_size = bottleneck_size
+        self.non_linearity = get_activation(adapter_non_linearity)
+
+        # down proj
+        self.down_proj = nn.Linear(self.adapter_input_size, self.bottleneck_size)
+        # up proj
+        self.up_proj = nn.Linear(self.bottleneck_size, self.adapter_input_size)
+
+        self.init_weights()
+
+    def init_weights(self, init_mean=0.0, init_std=0.01):
+        self.down_proj.weight.data.normal_(mean=init_mean, std=init_std)
+        self.down_proj.bias.data.zero_()
+        self.up_proj.weight.data.normal_(mean=init_mean, std=init_std)
+        self.up_proj.bias.data.zero_()
+
+    def forward(self, x):
+        output = self.up_proj(self.non_linearity(self.down_proj(x)))
+        output = x + output
+        return output
+    
+def add_adapter(model, adapter_method='bottleneck', bottlenect_size=64):
+    # 冻结模型参数
+    for param in model.parameters():
+        param.requires_grad = False
+    if adapter_method == 'bottleneck':
+        # 顺序为: Attention --> Adapter --> Add --> LN --> FeedForward --> Adapter --> Add --> LayerNorm
+        for layer_id in range(model.num_hidden_layers):
+            transformer_layer = model.encoderLayer[layer_id].multiHeadAttention.o
+            out_featuers = transformer_layer.out_features
+            adapter1 = BottleneckAdapterLayer(out_featuers, bottleneck_size=bottlenect_size)
+            model.encoderLayer[layer_id].dropout1 = nn.Sequential(transformer_layer, adapter1)
+
+            transformer_layer = model.encoderLayer[layer_id].feedForward
+            out_featuers = transformer_layer.outputDense.out_features
+            adapter2 = BottleneckAdapterLayer(out_featuers, bottleneck_size=bottlenect_size)
+            model.encoderLayer[layer_id].feedForward = nn.Sequential(transformer_layer, adapter2)
+    # 待新增其余类型adapter
+    else:
+        pass
+    return model
```

### Comparing `bert4torch-0.2.7.post2/bert4torch/losses.py` & `bert4torch-0.2.8/bert4torch/losses.py`

 * *Files 0% similar despite different names*

```diff
@@ -300,16 +300,15 @@
             #     print(w, sup_loss.item(), w * unsup_loss.item())
             #     print(y_true_sup)
             return sup_loss + w * unsup_loss, sup_loss, w * unsup_loss
         else:
             return self.loss_sup(y_pred_sup, y_true_sup)
 
     def same_batch_check(self, y_pred_sup, y_pred_unsup, y_true_sup, bti):
-        '''检测数据的前几个batch必须是一致的, 这里写死是10个
-        '''
+        '''检测数据的前几个batch必须是一致的, 这里写死是10个'''
         if bti >= 10:
             return
         if bti >= len(self.hist_input_y):
             self.hist_input_y.append(y_true_sup.to(self.hist_device))
         else:  # 检测
             err_msg = 'TemporalEnsemblingLoss requests the same sort dataloader, you may need to set train_dataloader shuffle=False'
             assert self.hist_input_y[bti].equal(y_true_sup.to(self.hist_device)), err_msg
```

### Comparing `bert4torch-0.2.7.post2/bert4torch/models.py` & `bert4torch-0.2.8/bert4torch/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 ''' 模型
     v0.2.2版本前Trainer是在bert4torch内部实现的，之后单独为Trainer做了一个包torch4keras
     v0.2.5版本开始，对抗训练模块不在complile中使用，而是用callback方式实现
 '''
 import torch
-import torch.nn as nn
+from torch import nn, Tensor
+import torch.nn.functional as F
 import copy
 import json
 import re
-from bert4torch.layers import LayerNorm, BertEmbeddings, BertLayer, Identity, T5Layer, GatedAttentionUnit, XlnetLayer
+from bert4torch.layers import LayerNorm, BertEmbeddings, BertLayer, BlockIdentity, T5Layer, GatedAttentionUnit, XlnetLayer
 from bert4torch.layers import AdaptiveEmbedding, XlnetPositionsEncoding, ConvLayer
-from bert4torch.snippets import insert_arguments, delete_arguments, get_kw, torch_div
-from bert4torch.snippets import take_along_dim, create_position_ids_from_input_ids, DottableDict
+from bert4torch.snippets import insert_arguments, delete_arguments, print_trainable_parameters, torch_div
+from bert4torch.snippets import take_along_dim, create_position_ids_start_at_padding, DottableDict, get_parameter_device
 from bert4torch.activations import get_activation
 import warnings
 from torch4keras.model import *
 from torch.utils.checkpoint import checkpoint as grad_checkpoint
+from tqdm import tqdm
 
 
 class BERT_BASE(nn.Module):
     """模型基类
     """
     def __init__(
             self,
@@ -34,18 +36,18 @@
             attention_head_size=None,  # Attention中V的head_size
             attention_key_size=None,  # Attention中Q,K的head_size
             initializer_range=0.02,  # 权重初始化方差
             sequence_length=None,  # 是否固定序列长度
             keep_tokens=None,  # 要保留的词ID列表
             compound_tokens=None,  # 扩展Embedding
             residual_attention_scores=False,  # Attention矩阵加残差
-            ignore_invalid_weights=False,  # 允许跳过不存在的权重
             keep_hidden_layers=None, # 保留的hidden_layer层的id
             hierarchical_position=None,  # 是否层次分解位置编码
             gradient_checkpoint=False, # 是否使用gradient_checkpoint
+            output_all_encoded_layers=False, # 是否返回所有layer的hidden_states
             **kwargs
     ):
         super(BERT_BASE, self).__init__()
         if keep_tokens is not None:
             vocab_size = len(keep_tokens)
         if compound_tokens is not None:
             vocab_size += len(compound_tokens)
@@ -64,111 +66,91 @@
         self.sequence_length = sequence_length
         self.keep_tokens = keep_tokens
         self.compound_tokens = compound_tokens
         self.attention_bias = None
         self.position_bias = None
         self.attention_scores = None
         self.residual_attention_scores = residual_attention_scores
-        self.ignore_invalid_weights = ignore_invalid_weights
         self.keep_hidden_layers = set(range(num_hidden_layers)) if keep_hidden_layers is None else set(keep_hidden_layers)
         self.hierarchical_position = hierarchical_position
         self.gradient_checkpoint = gradient_checkpoint
-
-    def build(
-        self,
-        attention_caches=None,
-        layer_norm_cond=None,
-        layer_norm_cond_hidden_size=None,
-        layer_norm_cond_hidden_act=None,
-        additional_input_layers=None,
-        **kwargs
-    ):
-        """模型构建函数
-
-        :param attention_caches: 为Attention的K,V的缓存序列字典，格式为{Attention层名: [K缓存, V缓存]}；
-        :param layer_norm_*: 实现Conditional Layer Normalization时使用，用来实现以“固定长度向量”为条件的条件Bert，暂未使用
-        """
-        # additional_input
-        # if additional_input_layers is not None:
-        #     if not isinstance(additional_input_layers, list):
-        #         self.additional_input_layers = [additional_input_layers]
-        #     else:
-        #         self.additional_input_layers = additional_input_layers
-
-        # Other
-        self.attention_caches = attention_caches or {}
-        # self.layer_norm_conds = [
-        #     layer_norm_cond,
-        #     layer_norm_cond_hidden_size,
-        #     layer_norm_cond_hidden_act or 'linear',
-        # ]
-        self.output_all_encoded_layers = kwargs.get('output_all_encoded_layers', False)
-
-    def args_segmentate(self, inputs):
-        '''解析输入，转成list，tuple类型
-        '''
-        # 如果是([],)类型的则取第一个元素
+        self.quantized = False
+        self.output_all_encoded_layers = output_all_encoded_layers
+        self.skip_init = kwargs['skip_init']
+        self.add_trainer = kwargs['add_trainer']
+
+    def get_kw(self, *args, **kwargs):
+        '''把self.属性设置到kwargs中, 方便传参'''
+        for arg in args:
+            kwargs[arg] = getattr(self, arg)
+        return kwargs
+
+    def args_segmentate(self, inputs, **model_kwargs):
+        '''解析输入，转成list，tuple类型'''
+        # 传入[x1,x2]时，*inputs会解析成([x1,x2],)，此时需要取第一个元素
         if (len(inputs)==1) and isinstance(inputs[0], (tuple,list)):
             return inputs[0]
         return inputs
 
-    def forward(self, *inputs):
+    def forward(self, *inputs, **model_kwargs):
         """定义模型的训练流程
         
         :param inputs: List[torch.Tensor], 默认顺序是[token_ids, segment_ids(若有), position_ids(若有), custom_attention_mask(若有), conditional_input(若有)]
         :return: List[torch.Tensor] or torch.Tensor, 模型输出，默认顺序为[last_hidden_state/all_encoded_layers, pooled_output(若有), mlm_scores(若有), nsp_scores(若有)]
         """
         # 允许model([token_ids, segment_ids]), model(token_ids, segment_ids)调用方式
-        inputs = self.args_segmentate(inputs)
+        inputs = self.args_segmentate(inputs, **model_kwargs)
         # Embedding
-        outputs = self.apply_embeddings(inputs)
+        model_kwargs = self.apply_embeddings(*inputs, **model_kwargs)
         # Main
-        outputs = self.apply_main_layers(outputs)
+        model_kwargs = self.apply_main_layers(**model_kwargs)
         # Final
-        outputs = self.apply_final_layers(outputs)
+        outputs = self.apply_final_layers(**model_kwargs)
+        if model_kwargs.get('use_states', False):
+            return outputs, model_kwargs
         return outputs
 
     @torch.no_grad()
-    def predict(self, *inputs):
+    def predict(self, *inputs, **model_kwargs):
         """定义模型的预测流程
         
         :param inputs: List[torch.Tensor], 默认顺序是[token_ids, segment_ids(若有), position_ids(若有), custom_attention_mask(若有), conditional_input(若有)]
         :return: List[torch.Tensor] or torch.Tensor, 模型输出，默认顺序为[last_hidden_state/all_encoded_layers, pooled_output(若有), mlm_scores(若有), nsp_scores(若有)]
         """
         self.eval()
-        return self.forward(*inputs)
+        return self.forward(*inputs, **model_kwargs)
 
     def init_model_weights(self, module):
-        """ 初始化权重
-        """
-        if isinstance(module, (nn.Linear, nn.Embedding)) and (module.weight.requires_grad):
+        """ 初始化权重 """
+        if self.skip_init == 'meta':
+            if isinstance(module, (nn.Linear, nn.Embedding)):
+                module.to_empty(device='cpu')
+        elif isinstance(module, (nn.Linear, nn.Embedding)) and (module.weight.requires_grad):
             # bert参数初始化, tf版本在linear和Embedding层使用的是截断正太分布, pytorch没有实现该函数,
             # 此种初始化对于加载预训练模型后进行finetune没有任何影响，
             # cf https://github.com/pytorch/pytorch/pull/5617
             # 固定的相对位置编码如Sinusoidal无需初始化
             module.weight.data.normal_(mean=0.0, std=self.initializer_range)
         elif isinstance(module, LayerNorm):
             if hasattr(module, 'bias') and module.bias.requires_grad:  # T5等模型使用的是rmsnorm
                 module.bias.data.zero_()
             if hasattr(module, 'weight') and module.weight.requires_grad:
                 module.weight.data.fill_(1.0)
         if isinstance(module, nn.Linear) and (module.bias is not None) and (module.bias.requires_grad):
             module.bias.data.zero_()
 
     def variable_mapping(self):
-        """构建pytorch层与checkpoint的变量名之间的映射表
-        """
+        """构建pytorch层与checkpoint的变量名之间的映射表"""
         return {}
 
     def load_variable(self):
         raise NotImplementedError
 
     def load_embeddings(self, embeddings):
-        """根据keep_tokens和compound_tokens对embedding进行修改
-        """
+        """根据keep_tokens和compound_tokens对embedding进行修改"""
         if self.keep_tokens is not None:
             embeddings = embeddings[self.keep_tokens]
 
         if self.compound_tokens is not None:
             ext_embeddings = []
             for item in self.compound_tokens:
                 try:
@@ -177,150 +159,226 @@
                     ext_embeddings.append(torch.mean(embeddings, 0, keepdim=True))
                     warnings.warn(f'Initialize ext_embeddings from compound_tokens not in embedding index')
             embeddings = torch.cat([embeddings] + ext_embeddings, 0)
 
         return embeddings
 
     def load_pos_embeddings(self, embeddings):
-        """根据hierarchical_position对pos_embedding进行修改
-        """
+        """根据hierarchical_position对pos_embedding进行修改"""
         if self.hierarchical_position is not None:
             alpha = 0.4 if self.hierarchical_position is True else self.hierarchical_position
             embeddings = embeddings - alpha * embeddings[:1]
             embeddings = embeddings / (1 - alpha)
             position_index = torch.arange(self.max_position)[:, None]
             # 为兼容低版本pytorch没有take_along_dim
             embeddings_x = take_along_dim(embeddings,  torch_div(position_index, embeddings.size(0), rounding_mode='trunc'), dim=0)  # 兼容老版本
             # embeddings_x = take_along_dim(embeddings,  torch.div(position_index, embeddings.size(0), rounding_mode='trunc'), dim=0)
             embeddings_y = take_along_dim(embeddings, position_index % embeddings.size(0), dim=0)
             embeddings = alpha * embeddings_x + (1 - alpha) * embeddings_y
 
         return embeddings
 
-    def load_weights_from_pytorch_checkpoint(self, checkpoint, mapping=None):
-        """根据mapping从checkpoint加载权重
-        """
-        file_state_dict = torch.load(checkpoint, map_location='cpu')  # 加载模型文件
+    def load_weights_from_pytorch_checkpoint(self, checkpoint, mapping=None, verbose=1):
+        """根据mapping从checkpoint加载权重"""
+        # 加载模型文件
+        if isinstance(checkpoint, str):
+            file_state_dict = torch.load(checkpoint, map_location='cpu')
+        else:
+            raise ValueError('Args `checkpoint_path` only support `str` format')
+        
         mapping = mapping or self.variable_mapping()
-        parameters_set = set([i[0] for i in self.named_parameters()])  # 可更新的变量
+        model_params = set([i[0] for i in self.named_parameters()])  # 可更新的变量
         
-        # 如果模型文件和模型结构中同时存在，且不在预设的mapping中，则更新mapping
+        # 如果ckpt和model中同时存在，且不在预设的mapping中，则更新mapping
         # 主要是如为了在外部继承BERT后有其他layer，也能自动从checkpoint中加载进来
-        for layer_name in parameters_set:
+        for layer_name in model_params:
             if (layer_name in file_state_dict) and (layer_name not in mapping):
                 mapping.update({layer_name: layer_name})
 
-        state_dict_new ={}
+        state_dict_new = {}
+        missing_keys, needed_keys = [], []  # 都是old_keys的名字
         for new_key, old_key in mapping.items():
+            # mapping和model不一致，忽略，如with_nsp=False时候在mapping中有但是model中没有
             if new_key not in self.state_dict():
                 continue
-            elif old_key in file_state_dict: # mapping中包含，且模型结构中有
+            # model中有，且ckpt中有，正常加载
+            elif old_key in file_state_dict:
                 state_dict_new[new_key] = self.load_variable(file_state_dict, old_key)
-            elif (old_key not in file_state_dict) and (not self.ignore_invalid_weights):
-                # mapping中包含，但模型文件中没有
-                print(f'[WARNING] {old_key} not found in pretrain models')
-            if new_key in parameters_set:
-                parameters_set.remove(new_key)
-
-        # 未能加载预训练权重的Parameter
-        if not self.ignore_invalid_weights:
-            for key in parameters_set:
-                print(f'[WARNING] Parameter {key} not loaded from pretrain models')
+            # model中有，但ckpt中没有，ckpt中缺失部分参数
+            elif old_key not in file_state_dict:
+                missing_keys.append(old_key)
+            # 保留未能加载预训练权重的Parameter
+            if new_key in model_params:
+                model_params.remove(new_key)
+            needed_keys.append(old_key)
         del file_state_dict
 
+        # mismatch keys的处理
+        if verbose != 0:
+            for key in missing_keys:
+                print(f'[WARNING] {key} not found in pretrain models')
+            for key in model_params:
+                print(f'[WARNING] Parameter {key} not loaded from pretrain models')
+
         # 将ckpt的权重load到模型结构中
         self.load_state_dict(state_dict_new, strict=False)
+        del state_dict_new
+        return missing_keys, needed_keys
 
-    def apply_embeddings(self, inputs):
+    def load_weights_from_pytorch_checkpoints(self, checkpoints, mapping=None, verbose=1):
+        """逐个ckpt加载"""
+        if isinstance(checkpoints, str):
+            self.load_weights_from_pytorch_checkpoint(checkpoints, mapping=mapping, verbose=verbose)
+        elif isinstance(checkpoints, (tuple, list)):
+            all_missing_keys = []
+            for checkpoint in tqdm(checkpoints, desc='Loading checkpoint shards'):
+                missing_keys, needed_keys = self.load_weights_from_pytorch_checkpoint(checkpoint, mapping=mapping, verbose=0)
+                all_missing_keys.extend(missing_keys)
+            all_missing_set = set(all_missing_keys).difference(set(needed_keys))
+            if verbose != 0:
+                for key in all_missing_set:
+                    print(f'[WARNING] {key} not found in pretrain models')
+        else:
+            raise ValueError('Args `checkpoint_path` only support `str` or `list(str)` format')
+
+    def apply_embeddings(self, *inputs, **model_kwargs):
         raise NotImplementedError
 
-    def apply_main_layers(self, inputs):
+    def apply_main_layers(self, *inputs, **model_kwargs):
         raise NotImplementedError
 
-    def apply_final_layers(self, inputs):
+    def apply_final_layers(self, *inputs, **model_kwargs):
         raise NotImplementedError
     
-    def apply_on_layer_begin(self, l_i, inputs):
-        '''新增对layer block输入进行操作的函数
-        '''
-        return inputs
+    def apply_on_layer_begin(self, l_i, **model_kwargs):
+        '''新增对layer block输入进行操作的函数'''
+        model_kwargs['past_key_value'] = model_kwargs.get('past_key_values', [None]*self.num_hidden_layers)[l_i]
+        model_kwargs['cross_past_key_value'] = model_kwargs.get('cross_past_key_values', [None]*self.num_hidden_layers)[l_i]
+        return model_kwargs
     
-    def apply_on_layer_end(self, l_i, inputs):
-        '''新增对layer block输出进行操作的函数
-        '''
-        return inputs
+    def apply_on_layer_end(self, l_i, **model_kwargs):
+        '''新增对layer block输出进行操作的函数, 目前仅在MixUp中使用'''
+        if model_kwargs.get('past_key_value', None) is not None:
+            if 'past_key_values' not in model_kwargs:
+                model_kwargs['past_key_values'] = [None]*self.num_hidden_layers
+            model_kwargs['past_key_values'][l_i] = model_kwargs['past_key_value']
+        if model_kwargs.get('cross_past_key_value', None) is not None:
+            if 'cross_past_key_values' not in model_kwargs:
+                model_kwargs['cross_past_key_values'] = [None]*self.num_hidden_layers
+            model_kwargs['cross_past_key_values'][l_i] = model_kwargs['cross_past_key_value']
+        return model_kwargs
 
     def compute_attention_bias(self, inputs=None):
-        """定义每一层的Attention Bias
-        """
+        """定义每一层的Attention Bias"""
         return self.attention_bias
 
     def compute_position_bias(self, inputs=None):
-        """定义每一层的Position Bias（一般相对位置编码用）
-        """
+        """定义每一层的Position Bias（一般相对位置编码用）"""
         return self.position_bias
 
     def set_outputs(self, outputs):
-        """设置output和oututs属性
-        """
+        """设置output和oututs属性"""
         if not isinstance(outputs, list):
             outputs = [outputs]
 
         outputs = outputs[:]
         self.outputs = outputs
         if len(outputs) > 1:
             self.output = outputs
         else:
             self.output = outputs[0]
 
+    def quantize(self, bits: int, use_quantization_cache=True, empty_init=False, target_modules=None, **kwargs):
+        '''量化'''
+        if bits == 0:
+            return
+
+        from .quantization import quantize
+
+        if self.quantized:
+            print("Already quantized.")
+            return self
+
+        self.quantized = True
+        self.quantization_bit = bits
+        self = quantize(self, bits, empty_init=empty_init, use_quantization_cache=use_quantization_cache, target_modules=target_modules, **kwargs)
+        return self
+
+    def add_adapter(self, adapter_method='bottleneck', bottlenect_size=64):
+        '''增加adapter层'''
+        from bert4torch.layers import add_adapter
+        self = add_adapter(self, adapter_method, bottlenect_size)
+        self.print_trainable_parameters()
+        return self
+        
+    def get_peft_model(self, peft_config, adapter_name="default"):
+        '''hf的peft库：https://github.com/huggingface/peft
+        peft的接口LoraModel接口有变，这里使用v0.0.3
+        '''
+        import peft
+        self.peft_config = {adapter_name: peft_config}
+        if isinstance(peft_config, peft.LoraConfig):
+            model = peft.LoraModel(self, self.peft_config, adapter_name)
+        elif isinstance(peft_config, peft.AdaLoraConfig):
+            model = peft.AdaLoraModel(self, self.peft_config, adapter_name)
+        
+        # 返回的model无法使用torch4keras的trainer
+        self =  add_trainer(model) if self.add_trainer else model
+        self.print_trainable_parameters()
+        return self
+
+    def print_trainable_parameters(self):
+        """打印可训练的参数量"""
+        print_trainable_parameters(self)
+    
+    @property
+    def device(self) -> torch.device:
+        """获取model所在的device"""
+        return get_parameter_device(self)
+
 
 class LM_Mask(object):
-    """定义下三角Attention Mask（语言模型用）
-    """
+    """定义下三角Attention Mask（语言模型用）"""
     def compute_attention_bias(self, inputs=None):
-        """通过idxs序列的比较来得到对应的mask
-        """
-        seq_len = inputs[0].shape[1]
+        """通过idxs序列的比较来得到对应的mask"""
+        token_ids = inputs[0]
+        seq_len = token_ids.shape[1]
         attention_bias = torch.tril(torch.ones(seq_len, seq_len, dtype=torch.long, device=inputs[0].device), diagonal=0)
         self.attention_bias = attention_bias.unsqueeze(0).unsqueeze(1)
         return self.attention_bias
 
 
 def extend_with_language_model(InputModel):
-    """添加下三角的Attention Mask（语言模型用）
-    """
+    """添加下三角的Attention Mask（语言模型用）"""
     class LanguageModel(LM_Mask, InputModel):
-        """带下三角Attention Mask的派生模型
-        """
+        """带下三角Attention Mask的派生模型"""
         def __init__(self, *args, **kwargs):
             kwargs['with_mlm'] = kwargs.get('with_mlm') or True
             super(LanguageModel, self).__init__(*args, **kwargs)
 
     return LanguageModel
 
 
 class UniLM_Mask(object):
     """定义UniLM的Attention Mask（Seq2Seq模型用）；
     其中source和target的分区，由segment_ids来表示。
     UniLM: https://arxiv.org/abs/1905.03197
     """
     def compute_attention_bias(self, inputs=None):
-        """通过idxs序列的比较来得到对应的mask
-        """
+        """通过idxs序列的比较来得到对应的mask"""
         segment_ids = inputs[1]
         attention_bias = torch.cumsum(segment_ids, dim=1)
         attention_bias = (attention_bias.unsqueeze(1)) <= (attention_bias.unsqueeze(2))
         self.attention_bias = attention_bias.unsqueeze(1).long()
 
         return self.attention_bias
 
 
 def extend_with_unified_language_model(InputModel):
-    """添加UniLM的Attention Mask（Seq2Seq模型用）
-    """
+    """添加UniLM的Attention Mask（Seq2Seq模型用）"""
     class UnifiedLanguageModel(UniLM_Mask, InputModel):
         """带UniLM的Attention Mask的派生模型
         UniLM: https://arxiv.org/abs/1905.03197
         """
         def __init__(self, *args, **kwargs):
             kwargs['with_mlm'] = kwargs.get('with_mlm') or True
             super(UnifiedLanguageModel, self).__init__(*args, **kwargs)
@@ -337,42 +395,40 @@
             segment_vocab_size=2,  # segment总数目
             with_pool=False,  # 是否包含Pool部分
             with_nsp=False,  # 是否包含NSP部分
             with_mlm=False,  # 是否包含MLM部分
             custom_position_ids=False,  # 是否自行传入位置id, True表示传入，False表示不传入，'start_at_padding'表示从padding_idx+1开始
             custom_attention_mask=False, # 是否自行传入attention_mask
             shared_segment_embeddings=False,  # 若True，则segment跟token共用embedding
-            layer_norm_cond=None,  # conditional layer_norm
-            layer_add_embs=None, # addtional_embeddng, 比如加入词性，音调，word粒度的自定义embedding
+            conditional_size=None,  # conditional layer_norm
+            additional_embs=False, # addtional_embeddng, 是否有额外的embedding, 比如加入词性，音调，word粒度的自定义embedding
             is_dropout=False,
-            token_pad_ids=0,  # 默认0是padding ids, 但是注意google的mt5padding不是0
+            pad_token_id=0,  # 默认0是padding ids, 但是注意google的mt5padding不是0
             **kwargs  # 其余参数
     ):
         super(BERT, self).__init__(**kwargs)
         self.max_position = max_position
         self.segment_vocab_size = segment_vocab_size
         self.with_pool = with_pool
         self.with_nsp = with_nsp
         self.with_mlm = with_mlm
         self.custom_position_ids = custom_position_ids
         self.custom_attention_mask = custom_attention_mask
         self.shared_segment_embeddings = shared_segment_embeddings
         self.is_dropout = is_dropout
-        self.token_pad_ids = token_pad_ids
+        self.pad_token_id = pad_token_id
         if self.with_nsp and not self.with_pool:
             self.with_pool = True
-        self.layer_norm_conds = layer_norm_cond
-        self.layer_add_embs = layer_add_embs
-        self.conditional_size = layer_norm_cond.weight.size(1) if layer_norm_cond is not None else None
-        self.embeddings = BertEmbeddings(self.vocab_size, self.embedding_size, self.hidden_size, self.max_position, self.segment_vocab_size, self.shared_segment_embeddings, 
-                                         self.dropout_rate, self.conditional_size, **get_kw(BertEmbeddings, kwargs))
-        kwargs['max_position'] = self.max_position  # 相对位置编码需要使用    
-        layer = BertLayer(self.hidden_size, self.num_attention_heads, self.dropout_rate, self.attention_probs_dropout_prob, self.intermediate_size, self.hidden_act, 
-                          is_dropout=self.is_dropout, conditional_size=self.conditional_size, **get_kw(BertLayer, kwargs))
-        self.encoderLayer = nn.ModuleList([copy.deepcopy(layer) if layer_id in self.keep_hidden_layers else Identity() for layer_id in range(self.num_hidden_layers)])
+        self.additional_embs = additional_embs
+        self.conditional_size = conditional_size
+        self.embeddings = BertEmbeddings(**self.get_kw('vocab_size', 'embedding_size', 'hidden_size', 'max_position', 'segment_vocab_size', 
+                                                       'shared_segment_embeddings', 'dropout_rate', 'conditional_size', **kwargs))
+        layer = BertLayer(**self.get_kw('hidden_size', 'num_attention_heads', 'dropout_rate', 'attention_probs_dropout_prob', 
+                                        'intermediate_size', 'hidden_act', 'is_dropout', 'conditional_size', 'max_position', **kwargs))
+        self.encoderLayer = nn.ModuleList([copy.deepcopy(layer) if layer_id in self.keep_hidden_layers else BlockIdentity() for layer_id in range(self.num_hidden_layers)])
         
         if self.with_pool:
             # Pooler部分（提取CLS向量）
             self.pooler = nn.Linear(self.hidden_size, self.hidden_size)
             self.pooler_activation = nn.Tanh() if self.with_pool is True else get_activation(self.with_pool)
             if self.with_nsp:
                 # Next Sentence Prediction部分
@@ -389,126 +445,144 @@
             self.mlmDecoder = nn.Linear(self.embedding_size, self.vocab_size, bias=False)
             if kwargs.get('tie_emb_prj_weight') is True:
                 self.mlmDecoder.weight = self.embeddings.word_embeddings.weight
             self.mlmBias = nn.Parameter(torch.zeros(self.vocab_size))
             self.mlmDecoder.bias = self.mlmBias
         # 下述继承于BERT的有声明新的参数，在这里初始化不能统一初始化到
 
-    def apply_embeddings(self, inputs):
+    def apply_embeddings(self, *inputs, **model_kwargs):
         """BERT的embedding是token、position、segment三者embedding之和
 
-        :param inputs: List[torch.Tensor], 默认顺序是[token_ids, segment_ids(若有), position_ids(若有), custom_attention_mask(若有), conditional_input(若有)]
+        :param inputs: List[torch.Tensor], 默认顺序是[token_ids, segment_ids(若有), position_ids(若有), custom_attention_mask(若有), conditional_input(若有), additional_input(若有)]
         :return: List[torch.Tensor], [hidden_states, attention_mask, conditional_emb, ...]
         """
         assert isinstance(inputs, (tuple, list)), f'Inputs only support list,tuple format but passed {type(inputs)}'
 
-        token_ids = inputs[0]
-        index_ = 1
-        if self.segment_vocab_size > 0:
+        # ========================= token_ids =========================
+        if model_kwargs.get('token_ids') is not None:
+            token_ids = model_kwargs['token_ids']
+        else:
+            token_ids = inputs[0]
+            index_ = 1
+        
+        # ========================= segment_ids =========================
+        if model_kwargs.get('segment_ids') is not None:
+            segment_ids = model_kwargs['segment_ids']
+        elif self.segment_vocab_size > 0:
             segment_ids = inputs[index_]
             index_ += 1
         else:
             segment_ids = None
 
-        if self.custom_position_ids is True:  # 自定义position_ids
+        # ========================= position_ids =========================
+        # [btz, seq_len]
+        if model_kwargs.get('position_ids') is not None:
+            position_ids = model_kwargs['position_ids']
+        elif self.custom_position_ids is True:  # 自定义position_ids
             position_ids = inputs[index_]
             index_ += 1
         elif self.custom_position_ids == 'start_at_padding':
-            position_ids = create_position_ids_from_input_ids(token_ids, self.token_pad_ids)
+            # 从padding位置开始
+            position_ids = create_position_ids_start_at_padding(token_ids, self.pad_token_id)
         else:
-            position_ids = None
+            position_ids = torch.arange(token_ids.shape[1], dtype=torch.long, device=token_ids.device).unsqueeze(0)
+        model_kwargs['position_ids'] = position_ids
 
-        # 根据token_ids创建一个3D的attention mask矩阵，尺寸为[batch_size, 1, 1, to_seq_length]，
-        # 目的是为了适配多头注意力机制，从而能广播到[batch_size, num_heads, from_seq_length, to_seq_length]尺寸
-        if self.custom_attention_mask:
-            attention_mask = inputs[index_].long().unsqueeze(1).unsqueeze(2)
+        # ========================= attention_mask =========================
+        # 这里attention_mask表示传入[btz, seq_len], 而后续的attention_mask其实是extended_attention_mask[btz, 1, 1/q_len, seq_len]
+        if model_kwargs.get('attention_mask') is not None:
+            # attention_mask是根据token_ids生成的，因此外部需要重置下，目前是带cache解码时候使用
+            attention_mask = model_kwargs['attention_mask']
+        elif self.custom_attention_mask:
+            attention_mask = inputs[index_].long()
             index_ += 1
         elif (not token_ids.requires_grad) and (token_ids.dtype in {torch.long, torch.int}): # 正常的token_ids
-            attention_mask = (token_ids != self.token_pad_ids).long().unsqueeze(1).unsqueeze(2)  # 默认0为mask_value
-            if self.token_pad_ids < 0:
-                token_ids = token_ids * attention_mask[:,0,0,:]
+            attention_mask = (token_ids != self.pad_token_id).long()  # 默认0为mask_value
+            if self.pad_token_id < 0:
+                token_ids = token_ids * attention_mask
         else:  # 自定义word_embedding，目前仅有VAT中使用
             attention_mask = self.attention_mask_cache
         self.attention_mask_cache = attention_mask  # 缓存上次用的attention_mask
-        
+        model_kwargs['input_attention_mask'] = attention_mask
+        # 根据token_ids创建一个3D的attention mask矩阵，尺寸为[batch_size, 1, 1, to_seq_length]，
+        # 目的是为了适配多头注意力机制，从而能广播到[batch_size, num_heads, from_seq_length, to_seq_length]尺寸
+        attention_mask = attention_mask.unsqueeze(1).unsqueeze(2)
         self.compute_attention_bias([token_ids, segment_ids])  # 根据lm或者unilm需要对mask做调整
         if self.attention_bias is not None:
             attention_mask = attention_mask * self.attention_bias  # 不可访问padding
             # attention_mask = self.attention_bias  # 可以访问padding
-
         # pytorch >= 1.5时候会导致StopIteration错误
         # https://github.com/huggingface/transformers/issues/3936
         # https://github.com/huggingface/transformers/issues/4189
         # https://github.com/huggingface/transformers/issues/3936
         try:
             attention_mask = attention_mask.to(dtype=next(self.parameters()).dtype)  # 兼容fp16
         except StopIteration:
             attention_mask = attention_mask.to(dtype=torch.float32)
         
-        # 对mask矩阵中，数值为0的转换成很大的负数，使得不需要attention的位置经过softmax后,分数趋近于0
-        # attention_mask = (1.0 - attention_mask) * -10000.0
-        # conditional layer_norm
-        if self.layer_norm_conds is None:
-            conditional_emb = None
-        else:
-            conditional_emb = self.layer_norm_conds(inputs[index_])
+        # ========================= conditional layer_norm =========================
+        if model_kwargs.get('conditional_emb') is not None:
+            conditional_emb = model_kwargs['layer_norm_ids']
+        elif self.conditional_size is not None:
+            conditional_emb = inputs[index_]
             index_ += 1
+        else:
+            conditional_emb = None
 
-        # addtional_embeddng, 比如加入词性，音调，word粒度的自定义embedding
-        if isinstance(self.layer_add_embs, nn.Module):  # 单个
-            additional_embs = [self.layer_add_embs(inputs[index_])]
+        # ========================= addtional_embeddng =========================
+        # 比如加入词性，音调，word粒度的自定义embedding
+        if model_kwargs.get('additional_embs') is not None:
+            additional_embs = model_kwargs['additional_embs']
+        elif self.additional_embs is True:
+            additional_embs = inputs[index_]
             index_ += 1
-        elif isinstance(self.layer_add_embs, (tuple, list)):  # 多个
-            additional_embs = []
-            for layer in self.layer_add_embs:
-                assert isinstance(layer, nn.Module), 'Layer_add_embs element should be nn.Module'
-                additional_embs.append(layer(inputs[index_]))
-                index_ += 1
         else:
             additional_embs = None
+        additional_embs = [additional_embs] if isinstance(additional_embs, torch.Tensor) else additional_embs
+        assert (additional_embs is None) or isinstance(additional_embs, (tuple, list))
 
         # 进入embedding层
         hidden_states = self.embeddings(token_ids, segment_ids, position_ids, conditional_emb, additional_embs)
-        return [hidden_states, attention_mask, conditional_emb] + list(inputs[index_:])
+        model_kwargs.update({'hidden_states': hidden_states, 'attention_mask':attention_mask, 'conditional_emb': conditional_emb})
+        
+        # 解析encoder_hidden_state, encoder_attention_mask
+        if len(inputs[index_:]) >=2:
+            model_kwargs['encoder_hidden_states'], model_kwargs['encoder_attention_mask'] = inputs[index_], inputs[index_+1]
+        return model_kwargs
 
-    def apply_main_layers(self, inputs):
+    def apply_main_layers(self, **model_kwargs):
         """BERT的主体是基于Self-Attention的模块；
         顺序:Att --> Add --> LN --> FFN --> Add --> LN
         
         :param inputs: List[torch.Tensor], 默认顺序为[hidden_states, attention_mask, conditional_emb]
         :return: List[torch.Tensor], 默认顺序为[encoded_layers, conditional_emb]
         """
-        hidden_states, attention_mask, conditional_emb = inputs[:3]
-        if len(inputs[3:]) >= 2:
-            encoder_hidden_state, encoder_attention_mask = inputs[3], inputs[4]
-        else:
-            encoder_hidden_state, encoder_attention_mask = None, None
-
-        encoded_layers = [hidden_states] # 添加embedding的输出
-        layer_inputs = [hidden_states, attention_mask, conditional_emb, encoder_hidden_state, encoder_attention_mask]
+        encoded_layers = [model_kwargs['hidden_states']] # 添加embedding的输出
         for l_i, layer_module in enumerate(self.encoderLayer):
-            layer_inputs = self.apply_on_layer_begin(l_i, layer_inputs)
-            hidden_states = grad_checkpoint(layer_module, *layer_inputs) if self.gradient_checkpoint else layer_module(*layer_inputs)
-            layer_inputs[0] = hidden_states
-            layer_inputs = self.apply_on_layer_end(l_i, layer_inputs)
+            model_kwargs = self.apply_on_layer_begin(l_i, **model_kwargs)
+            outputs = grad_checkpoint(layer_module, **model_kwargs) if self.gradient_checkpoint else layer_module(**model_kwargs)
+            model_kwargs.update(outputs)
+            hidden_states = model_kwargs['hidden_states']
+            model_kwargs = self.apply_on_layer_end(l_i, **model_kwargs)
 
             if self.output_all_encoded_layers:
                 encoded_layers.append(hidden_states)
         if not self.output_all_encoded_layers:
             encoded_layers.append(hidden_states)
-        return [encoded_layers, conditional_emb]
+        model_kwargs['encoded_layers'] = encoded_layers
+        return model_kwargs
     
-    def apply_final_layers(self, inputs):
+    def apply_final_layers(self, **model_kwargs):
         """根据剩余参数决定输出
 
         :param inputs: List[torch.Tensor], 默认顺序为[encoded_layers, conditional_emb]
         :return: List[torch.Tensor] or torch.Tensor, 模型输出，默认顺序为[last_hidden_state/all_encoded_layers, pooled_output(若有), mlm_scores(若有), nsp_scores(若有)]
         """
         # 获取最后一层隐藏层的输出
-        encoded_layers, conditional_emb = inputs
+        encoded_layers, conditional_emb = model_kwargs['encoded_layers'], model_kwargs.get('conditional_emb', None)
         sequence_output = encoded_layers[-1]
         # 是否取最后一层输出
         if not self.output_all_encoded_layers:
             encoded_layers = encoded_layers[-1]
 
         # 是否添加pool层
         if self.with_pool:
@@ -531,16 +605,15 @@
         else:
             mlm_scores = None
         
         outputs = [value for value in [encoded_layers, pooled_output, mlm_scores, nsp_scores] if value is not None]
         return outputs if len(outputs) > 1 else outputs[0]
 
     def load_variable(self, state_dict, name, prefix='bert'):
-        """加载单个变量的函数
-        """
+        """加载单个变量的函数, 这里的名称均为映射前的"""
         variable = state_dict[name]
         if name in {
             f'{prefix}.embeddings.word_embeddings.weight',
             'cls.predictions.bias',
             'cls.predictions.decoder.weight',
             'cls.predictions.decoder.bias'
         }:
@@ -599,37 +672,35 @@
 
 
 class ALBERT(BERT):
     def __init__(self, *args, **kwargs):
         super(ALBERT, self).__init__(*args, **kwargs)
         self.encoderLayer = nn.ModuleList([self.encoderLayer[0]])  # 取上述的第一行
 
-    def apply_main_layers(self, inputs):
+    def apply_main_layers(self, **model_kwargs):
         """BERT的主体是基于Self-Attention的模块（和BERT区别是始终使用self.encoderLayer[0]）；
         顺序:Att --> Add --> LN --> FFN --> Add --> LN
         """
-        hidden_states, attention_mask, conditional_emb = inputs[:3]
-        if len(inputs[3:]) >= 2:
-            encoder_hidden_state, encoder_attention_mask = inputs[3], inputs[4]
-        else:
-            encoder_hidden_state, encoder_attention_mask = None, None
 
-        encoded_layers = [hidden_states] # 添加embedding的输出
-        layer_inputs = [hidden_states, attention_mask, conditional_emb, encoder_hidden_state, encoder_attention_mask]
+        encoded_layers = [model_kwargs['hidden_states']] # 添加embedding的输出
         for l_i in range(self.num_hidden_layers):
-            layer_inputs = self.apply_on_layer_begin(l_i, layer_inputs)
-            hidden_states = self.encoderLayer[0](*layer_inputs)
-            layer_inputs[0] = hidden_states
-            layer_inputs = self.apply_on_layer_end(l_i, layer_inputs)
+            model_kwargs = self.apply_on_layer_begin(l_i, **model_kwargs)
+            layer_module = self.encoderLayer[0]
+            outputs = grad_checkpoint(layer_module, **model_kwargs) if self.gradient_checkpoint else layer_module(**model_kwargs)
+            model_kwargs.update(outputs)
+            hidden_states = model_kwargs['hidden_states']
+            model_kwargs = self.apply_on_layer_end(l_i, **model_kwargs)
 
             if self.output_all_encoded_layers:
                 encoded_layers.append(hidden_states)
         if not self.output_all_encoded_layers:
             encoded_layers.append(hidden_states)
-        return [encoded_layers, conditional_emb]
+        model_kwargs['encoded_layers'] =  encoded_layers
+        return model_kwargs
+
 
     def variable_mapping(self, prefix='albert'):
         mapping = {
             'embeddings.word_embeddings.weight': f'{prefix}.embeddings.word_embeddings.weight',
             'embeddings.position_embeddings.weight': f'{prefix}.embeddings.position_embeddings.weight',
             'embeddings.segment_embeddings.weight': f'{prefix}.embeddings.token_type_embeddings.weight',
             'embeddings.layerNorm.weight': f'{prefix}.embeddings.LayerNorm.weight',
@@ -689,37 +760,19 @@
 
 
 class ALBERT_Unshared(ALBERT):
     def __init__(self, *args, **kwargs):
         super(ALBERT_Unshared, self).__init__(*args, **kwargs)
         self.encoderLayer = nn.ModuleList([copy.deepcopy(self.encoderLayer[0]) for _ in range(self.num_hidden_layers)])
 
-    def apply_main_layers(self, inputs):
-        """BERT的主体是基于Self-Attention的模块（和ALBERT区别是所有层权重独立）；
+    def apply_main_layers(self, **model_kwargs):
+        """BERT的主体是基于Self-Attention的模块（和ALBERT区别是所有层权重独立）；这里就是调用BERT类的方法
         顺序:Att --> Add --> LN --> FFN --> Add --> LN
         """
-        hidden_states, attention_mask, conditional_emb = inputs
-        if len(inputs[3:]) >= 2:
-            encoder_hidden_state, encoder_attention_mask = inputs[3], inputs[4]
-        else:
-            encoder_hidden_state, encoder_attention_mask = None, None
-
-        encoded_layers = [hidden_states] # 添加embedding的输出
-        layer_inputs = [hidden_states, attention_mask, conditional_emb, encoder_hidden_state, encoder_attention_mask]
-        for i in range(self.num_hidden_layers):
-            layer_inputs = self.apply_on_layer_begin(i, layer_inputs)
-            hidden_states = self.encoderLayer[i](*layer_inputs)
-            layer_inputs[0] = hidden_states
-            layer_inputs = self.apply_on_layer_end(i, layer_inputs)
-
-            if self.output_all_encoded_layers:
-                encoded_layers.append(hidden_states)
-        if not self.output_all_encoded_layers:
-            encoded_layers.append(hidden_states)
-        return [encoded_layers, conditional_emb]
+        return BERT.apply_main_layers(self, **model_kwargs)
 
     def variable_mapping(self, prefix='albert'):
         mapping = super().variable_mapping()
         prefix_0 = f'{prefix}.encoder.albert_layer_groups.0.albert_layers.0.'
         for i in range(1, self.num_hidden_layers):
             mapping.update({f'encoderLayer.{i}.multiHeadAttention.q.weight': prefix_0 + 'attention.query.weight',
                             f'encoderLayer.{i}.multiHeadAttention.q.bias': prefix_0 + 'attention.query.bias',
@@ -786,19 +839,19 @@
         mapping = super().variable_mapping(prefix)
         mapping_new = {}
         for k, v in mapping.items():
             if (not re.search('bias|layernorm', k.lower())) and (not re.search('bias|layernorm', v.lower())):
                 mapping_new[k] = v
         return mapping_new
 
-    def apply_final_layers(self, inputs):
+    def apply_final_layers(self, **model_kwargs):
         """根据剩余参数决定输出
         """
         # 获取最后一层隐藏层的输出
-        encoded_layers, conditional_emb = inputs
+        encoded_layers = model_kwargs['encoded_layers']
         sequence_output = encoded_layers[-1]
         # 是否取最后一层输出
         if not self.output_all_encoded_layers:
             encoded_layers = encoded_layers[-1]
 
         # 是否添加mlm
         if self.with_mlm:
@@ -812,15 +865,15 @@
 
 class GAU_alpha(RoFormerV2):
     def __init__(self, *args, **kwargs):
         kwargs.update({'p_bias': 'rotary', 'weight': False, 'bias': False, 'norm_mode': 'rmsnorm', 'normalization': 'softmax_plus'})
         super().__init__(*args, **kwargs)
 
         layer = self.GAU_Layer(**kwargs)
-        self.encoderLayer = nn.ModuleList([copy.deepcopy(layer) if layer_id in self.keep_hidden_layers else Identity() for layer_id in range(self.num_hidden_layers)])
+        self.encoderLayer = nn.ModuleList([copy.deepcopy(layer) if layer_id in self.keep_hidden_layers else BlockIdentity() for layer_id in range(self.num_hidden_layers)])
     
     def load_variable(self, state_dict, name, prefix=''):
         variable = state_dict[name]
         return self.load_embeddings(variable) if name in {'embeddings.word_embeddings.weight', 'mlmDecoder.weight'} else variable
 
     def variable_mapping(self, prefix=''):
         '''在convert脚本里已经把key转成bert4torch可用的
@@ -829,19 +882,20 @@
 
     class GAU_Layer(nn.Module):
         def __init__(self, *args, **kwargs):
             super().__init__()
             self.gau = GatedAttentionUnit(**kwargs)
             self.dropout1 = nn.Dropout(kwargs.get('dropout_rate'))
             self.layerNorm1 = LayerNorm(**kwargs)
-        def forward(self, hidden_states, attention_mask, conditional_emb=None, encoder_hidden_states=None, encoder_attention_mask=None):
+        def forward(self, hidden_states=None, attention_mask=None, conditional_emb=None, **model_kwargs):
             gau_hidden_states = self.gau(hidden_states, attention_mask)
             hidden_states = hidden_states + self.dropout1(gau_hidden_states)
             hidden_states = self.layerNorm1((hidden_states, conditional_emb))
-            return hidden_states
+            model_kwargs['hidden_states'] = hidden_states
+            return model_kwargs
 
     
 class ELECTRA(BERT):
     """Google推出的ELECTRA模型；
     链接：https://arxiv.org/abs/2003.10555
     """
     @insert_arguments(with_discriminator=False)
@@ -850,16 +904,16 @@
         super(ELECTRA, self).__init__(max_position, **kwargs)
         if self.with_discriminator:
             self.dense = nn.Linear(self.hidden_size, self.hidden_size)
             self.dense_act = get_activation(self.hidden_act)
             self.dense_prediction = nn.Linear(self.hidden_size, 1)
             self.dense_prediction_act = get_activation('sigmoid') if self.with_discriminator is True else get_activation(self.with_discriminator)
 
-    def apply_final_layers(self, inputs):
-        hidden_states = super().apply_final_layers(inputs)  # 仅有hidden_state一项输出
+    def apply_final_layers(self, **model_kwargs):
+        hidden_states = super().apply_final_layers(**model_kwargs)  # 仅有hidden_state一项输出
         if self.with_discriminator:
             logit = self.dense_act(self.dense(hidden_states))
             return [hidden_states, self.dense_prediction_act(self.dense_prediction(logit))]
         else:
             return hidden_states
 
     def load_variable(self, state_dict, name):
@@ -877,16 +931,15 @@
                         'mlmLayerNorm.weight', 'mlmLayerNorm.bias', 'mlmBias', 'mlmDecoder.weight', 'mlmDecoder.bias']:
             del mapping[del_key]
 
         return mapping
 
 
 class ERNIE(BERT):
-    """百度文心 https://github.com/PaddlePaddle/ERNIE
-    """
+    """百度文心 https://github.com/PaddlePaddle/ERNIE"""
     def __init__(self, *args, **kwargs):
         super(ERNIE, self).__init__(*args, **kwargs)
 
     def variable_mapping(self):
         mapping = super(ERNIE, self).variable_mapping(prefix='ernie')
         mapping.update({'mlmDecoder.weight': 'ernie.embeddings.word_embeddings.weight',
                         'mlmDecoder.bias': 'cls.predictions.bias'})
@@ -915,46 +968,41 @@
     def __init__(self, *args, **kwargs):
         kwargs.update({'p_bias': 'deberta_v2'})  # 控制在Embedding阶段不生成position_embedding
         super(DebertaV2, self).__init__(*args, **kwargs)
         
         # Encoder中transformer_block前的其他网络结构
         self.relative_attention = kwargs.get("relative_attention", True)
         self.conv = ConvLayer(**kwargs) if kwargs.get("conv_kernel_size", 0) > 0 else None
-
+        
         # 把第二层后的相对位置编码的权重绑定到第一层上，变相实现仅由第一层计算
         for i in range(1, self.num_hidden_layers):
             self.encoderLayer[i].multiHeadAttention.relative_positions_encoding.weight = self.encoderLayer[0].multiHeadAttention.relative_positions_encoding.weight
             self.encoderLayer[i].multiHeadAttention.layernorm.weight = self.encoderLayer[0].multiHeadAttention.layernorm.weight
             self.encoderLayer[i].multiHeadAttention.layernorm.bias = self.encoderLayer[0].multiHeadAttention.layernorm.bias
-    
-    def apply_main_layers(self, inputs):
+
+    def apply_main_layers(self, **model_kwargs):
         """DebertaV2：主要区别是第0层后，会通过卷积层
         """
-        hidden_states, attention_mask, conditional_emb = inputs[:3]
-        if len(inputs[3:]) >= 2:
-            encoder_hidden_state, encoder_attention_mask = inputs[3], inputs[4]
-        else:
-            encoder_hidden_state, encoder_attention_mask = None, None
 
-        encoded_layers = [hidden_states] # 添加embedding的输出
-        layer_inputs = [hidden_states, attention_mask, conditional_emb, encoder_hidden_state, encoder_attention_mask]
+        encoded_layers = [model_kwargs['hidden_states']] # 添加embedding的输出
         for l_i, layer_module in enumerate(self.encoderLayer):
-            layer_inputs = self.apply_on_layer_begin(l_i, layer_inputs)
-            hidden_states = grad_checkpoint(layer_module, *layer_inputs) if self.gradient_checkpoint else layer_module(*layer_inputs)
+            model_kwargs = self.apply_on_layer_begin(l_i, **model_kwargs)
+            outputs = grad_checkpoint(layer_module, **model_kwargs) if self.gradient_checkpoint else layer_module(**model_kwargs)
+            model_kwargs.update(outputs)
             # 第0层要经过卷积
             if l_i == 0 and self.conv is not None:
-                hidden_states = self.conv(encoded_layers[0], hidden_states, attention_mask.squeeze(1).squeeze(1))
-            layer_inputs[0] = hidden_states
-            layer_inputs = self.apply_on_layer_end(l_i, layer_inputs)
+                model_kwargs['hidden_states'] = self.conv(encoded_layers[0], model_kwargs['hidden_states'], model_kwargs['attention_mask'].squeeze(1).squeeze(1))
+            model_kwargs = self.apply_on_layer_end(l_i, **model_kwargs)
 
             if self.output_all_encoded_layers:
-                encoded_layers.append(hidden_states)
+                encoded_layers.append(model_kwargs['hidden_states'])
         if not self.output_all_encoded_layers:
-            encoded_layers.append(hidden_states)
-        return [encoded_layers, conditional_emb]
+            encoded_layers.append(model_kwargs['hidden_states'])
+        model_kwargs['encoded_layers'] =  encoded_layers
+        return model_kwargs
 
     def variable_mapping(self):
         mapping = super(DebertaV2, self).variable_mapping(prefix='deberta')
         mapping.update({'mlmDecoder.weight': 'deberta.embeddings.word_embeddings.weight',
                         'mlmDecoder.bias': 'cls.predictions.bias',
                         'encoderLayer.0.multiHeadAttention.relative_positions_encoding.weight': 'deberta.encoder.rel_embeddings.weight',
                         'encoderLayer.0.multiHeadAttention.layernorm.weight': 'deberta.encoder.LayerNorm.weight',
@@ -990,16 +1038,16 @@
             task_type_embeddings = nn.Embedding(kwargs.get('task_type_vocab_size'), self.hidden_size)
             self.embeddings.task_type_embeddings = task_type_embeddings
 
             def hook(module, input, output):
                 return output+task_type_embeddings(torch.zeros(input[0].size(), dtype=torch.int64, device=input[0].device))
             self.embeddings.word_embeddings.register_forward_hook(hook)
 
-    def apply_final_layers(self, inputs):
-        hidden_states = super().apply_final_layers(inputs)  # 仅有hidden_state一项输出
+    def apply_final_layers(self, **model_kwargs):
+        hidden_states = super().apply_final_layers(**model_kwargs)  # 仅有hidden_state一项输出
         sequence_output = hidden_states[0] if isinstance(hidden_states, (tuple, list)) else hidden_states
 
         start_logits = self.linear_start(sequence_output)
         start_logits = torch.squeeze(start_logits, -1)
         start_prob = self.sigmoid(start_logits) if hasattr(self, 'sigmoid') else start_logits
         end_logits = self.linear_end(sequence_output)
         end_logits = torch.squeeze(end_logits, -1)
@@ -1024,26 +1072,21 @@
 class Encoder(BERT):
     def __init__(self, *args, **kwargs):
         kwargs['vocab_size'] = kwargs.get('src_vocab_size', kwargs['vocab_size'])
         super().__init__(*args, **kwargs)
         # encoder需要返回encoder_attention_mask
         self.encoder_attention_mask = None
     
-    def forward(self, *inputs):
+    def forward(self, *inputs, **model_kwargs):
         """因为encoder需要返回encoder_attention_mask，因此这里从新定义一下，多返回一个参数
         """
-        inputs = self.args_segmentate(inputs)
-        # Embedding
-        outputs = self.apply_embeddings(inputs)
-        encoder_attention_mask = [outputs[1]]
-        # Main
-        outputs = self.apply_main_layers(outputs)
-        # Final
-        outputs = self.apply_final_layers(outputs)
-        return ([outputs] if isinstance(outputs, torch.Tensor) else outputs) + encoder_attention_mask
+        # 返回model_kwargs方便解析attention_mask
+        outputs, model_kwargs = super().forward(*inputs, use_states=True, **model_kwargs)
+        # return: [encoder_hidden_states, encoder_attention_mask]
+        return ([outputs] if isinstance(outputs, torch.Tensor) else outputs) + [model_kwargs['attention_mask']]
 
 
 class Decoder(LM_Mask, BERT):
     @delete_arguments('with_pool', 'with_mlm', 'with_nsp')
     def __init__(self, *args, with_lm=True, tie_emb_prj_weight=False, logit_scale=True, **kwargs):
         kwargs['vocab_size'] = kwargs.get('tgt_vocab_size', kwargs['vocab_size'])
         kwargs['is_decoder'] = True  # 标记是decoder
@@ -1060,36 +1103,36 @@
             if tie_emb_prj_weight:
                 self.final_dense.weight = self.embeddings.word_embeddings.weight
             if logit_scale:  # T5默认会有logit_scale, bart默认没有，所以bart要传入false
                 self.x_logit_scale = (self.hidden_size ** -0.5)
             else:
                 self.x_logit_scale = 1.
 
-    def apply_main_layers(self, inputs):
+    def apply_main_layers(self, **model_kwargs):
         """Dencoder主体是基于Self-Attention、Cross-Attention的模块；
         顺序：Att1 --> Add --> LN --> Att2 --> Add -->  LN --> FFN --> Add --> LN
         """
-        hidden_states, attention_mask, conditional_emb, encoder_hidden_state, encoder_attention_mask = inputs[:5]
-        decoded_layers = [hidden_states] # 添加embedding的输出
-        layer_inputs = [hidden_states, attention_mask, conditional_emb, encoder_hidden_state, encoder_attention_mask]
-        for i, layer_module in enumerate(self.decoderLayer):
-            layer_inputs = self.apply_on_layer_begin(i, layer_inputs)
-            hidden_states = grad_checkpoint(layer_module, *layer_inputs) if self.gradient_checkpoint else layer_module(*layer_inputs)
-            layer_inputs[0] = hidden_states
-            layer_inputs = self.apply_on_layer_end(i, layer_inputs)
+        decoded_layers = [model_kwargs['hidden_states']] # 添加embedding的输出
+        for l_i, layer_module in enumerate(self.decoderLayer):
+            model_kwargs = self.apply_on_layer_begin(l_i, **model_kwargs)
+            outputs = grad_checkpoint(layer_module, **model_kwargs) if self.gradient_checkpoint else layer_module(**model_kwargs)
+            model_kwargs.update(outputs)
+            hidden_states = model_kwargs['hidden_states']
+            model_kwargs = self.apply_on_layer_end(l_i, **model_kwargs)
 
             if self.output_all_encoded_layers:
                 decoded_layers.append(hidden_states)
         if not self.output_all_encoded_layers:
             decoded_layers.append(hidden_states)
-        return [decoded_layers, conditional_emb]
+        model_kwargs['decoded_layers'] = decoded_layers
+        return model_kwargs
     
-    def apply_final_layers(self, inputs):
+    def apply_final_layers(self, **model_kwargs):
         outputs = []
-        hidden_states =  super().apply_final_layers(inputs)  # outputs为decoder顶层的hidden_states [btz, seq_len, hdsz]
+        hidden_states = model_kwargs['decoded_layers'][-1]  # outputs为decoder顶层的hidden_states [btz, seq_len, hdsz]
         outputs.append(hidden_states)
         if self.with_lm:
             logits = self.final_dense(hidden_states) * self.x_logit_scale  # outputs为[btz, seq_len, vocab_size]的logits
             activation = get_activation('linear' if self.with_lm is True else self.with_lm)  # 添加激活，一般是线性激活或softmax
             logits = activation(logits)
             outputs.append(logits)
         return outputs
@@ -1099,55 +1142,44 @@
         mapping = {}
         for k, v in raw_mapping.items():
             mapping[k.replace('encoderLayer', 'decoderLayer')] = v
         return mapping
 
 
 class Transformer(BERT_BASE):
-    '''encoder-decoder结构
-    '''
+    '''encoder-decoder结构'''
     @delete_arguments('with_pool', 'with_mlm', 'with_nsp')
     def __init__(self, *args, tie_emb_src_tgt_weight=False, **kwargs):
         super(Transformer, self).__init__(*args, **kwargs)
 
         # encoder
         self.encoder = Encoder(*args, **kwargs)
-        self.encoder.build(**kwargs)
 
         # decoder
-        self.decoder = Decoder(*args, **kwargs)
-        self.decoder.build(**kwargs)
+        self.decoder = Decoder(*args, add_cross_attention=True, **kwargs)
 
         if tie_emb_src_tgt_weight:
             # encoder和decoder的embedding权重共享
             assert self.encoder.vocab_size == self.decoder.vocab_size, "To share word embedding, the vocab size of src/tgt shall be the same."
             self.encoder.embeddings.word_embeddings.weight = self.decoder.embeddings.word_embeddings.weight
 
     def forward(self, *inputs):
         inputs = self.args_segmentate(inputs)
         encoder_input, decoder_input = inputs[:2]
 
         # encoder
-        # encoder_emb = self.encoder.apply_embeddings(encoder_input)
-        # encode_outputs = self.encoder.apply_main_layers(encoder_emb)
-        # encoder_hidden_state = self.encoder.apply_final_layers(encode_outputs)
-        # encoder_attention_mask = encoder_emb[1]
-        encoder_hidden_state, encoder_attention_mask = self.encoder(encoder_input)
+        encoder_hidden_states, encoder_attention_mask = self.encoder(encoder_input)
 
         # decoder
-        # decoder_emb = self.decoder.apply_embeddings(decoder_input)
-        # decoder_outputs = self.decoder.apply_main_layers([*decoder_emb, encoder_hidden_state, encoder_attention_mask])
-        # decoder_outputs = self.decoder.apply_final_layers(decoder_outputs) # [hidden_states, logits]
-        decoder_outputs = self.decoder(decoder_input + [encoder_hidden_state, encoder_attention_mask])
-        return [encoder_hidden_state] + decoder_outputs  # 输出encoder_hidden_state和decoder_hidden_state，以应对一些多任务情况
+        decoder_outputs = self.decoder(decoder_input + [encoder_hidden_states, encoder_attention_mask])
+        return [encoder_hidden_states] + decoder_outputs  # 输出encoder_hidden_state和decoder_hidden_state，以应对一些多任务情况
 
 
 class BART(Transformer):
-    '''encoder-decoder结构
-    '''
+    '''encoder-decoder结构'''
     def __init__(self, *args, tie_emb_src_tgt_weight=True, **kwargs):
         kwargs['logit_scale'] = kwargs.get('logit_scale', False)
         kwargs['tie_emb_prj_weight'] = kwargs.get('tie_emb_prj_weight', True)
         super(BART, self).__init__(*args, tie_emb_src_tgt_weight=tie_emb_src_tgt_weight, **kwargs)
         self.tie_emb_src_tgt_weight = tie_emb_src_tgt_weight
 
     def load_variable(self, state_dict, name, prefix=''):
@@ -1231,26 +1263,26 @@
     def __init__(self, *args, **kwargs):
         kwargs.update({'p_bias': 't5_relative', 'relative_attention_num_buckets': kwargs.get('relative_attention_num_buckets'), 'version': self.version, 
                        'bias': False, 'norm_mode': 'rmsnorm'})  # p_bias来控制embedding阶段无pos_embedding，t5不使用bias，并且使用rmsnorm
         super().__init__(*args, **kwargs)
         del self.embeddings.layerNorm
 
         # t5的layernorm都在前面，因此重新定义了下
-        layer = T5Layer(self.hidden_size, self.num_attention_heads, self.dropout_rate, self.attention_probs_dropout_prob, self.intermediate_size, self.hidden_act, is_dropout=self.is_dropout, 
-                            conditional_size=self.conditional_size, **get_kw(BertLayer, kwargs))
+        layer = T5Layer(**self.get_kw('hidden_size', 'num_attention_heads', 'dropout_rate', 'attention_probs_dropout_prob', 
+                                      'intermediate_size', 'hidden_act', 'is_dropout', 'conditional_size', **kwargs))
         self.encoderLayer = nn.ModuleList([copy.deepcopy(layer) for _ in range(self.num_hidden_layers)])
 
         # 把第二层后的相对位置编码的权重绑定到第一层上，变相实现仅由第一层计算
         for i in range(1, self.num_hidden_layers):
             self.encoderLayer[i].multiHeadAttention.relative_positions_encoding.weight = self.encoderLayer[0].multiHeadAttention.relative_positions_encoding.weight
         self.final_layer_norm = LayerNorm(self.hidden_size, eps=1e-12, conditional_size=self.conditional_size, bias=False, norm_mode='rmsnorm')
         self.dropout = nn.Dropout(self.dropout_rate)
 
-    def apply_final_layers(self, inputs):
-        hidden_states = super().apply_final_layers(inputs)
+    def apply_final_layers(self, **model_kwargs):
+        hidden_states = super().apply_final_layers(**model_kwargs)
         return self.dropout(self.final_layer_norm([hidden_states]))
 
     def load_variable(self, state_dict, name, prefix=''):
         # 加载单个变量的函数
         variable = state_dict[name]
         if name in {'encoder.embed_tokens.weight', 'shared.weight'}:
             return self.load_embeddings(variable)
@@ -1286,27 +1318,29 @@
     def __init__(self, *args, **kwargs):
         kwargs.update({'p_bias': 't5_relative', 'relative_attention_num_buckets': kwargs.get('relative_attention_num_buckets'), 'version': self.version,
                        'bias': False, 'norm_mode': 'rmsnorm'})  # p_bias来控制embedding阶段无pos_embedding，t5不使用bias，并且使用rmsnorm
         super().__init__(*args, **kwargs)
         del self.embeddings.layerNorm
 
         # t5的layernorm都在前面，因此重新定义了下
-        layer = T5Layer(self.hidden_size, self.num_attention_heads, self.dropout_rate, self.attention_probs_dropout_prob, self.intermediate_size, self.hidden_act, is_dropout=self.is_dropout, 
-                            conditional_size=self.conditional_size, is_decoder=True, **get_kw(BertLayer, kwargs))
+        layer = T5Layer(is_decoder=True, **self.get_kw('hidden_size', 'num_attention_heads', 'dropout_rate', 'attention_probs_dropout_prob', 
+                                                       'intermediate_size', 'hidden_act', 'is_dropout', 'conditional_size', **kwargs))
         self.decoderLayer = nn.ModuleList([copy.deepcopy(layer) for _ in range(self.num_hidden_layers)])
         
         # 把第二层后的相对位置编码的权重绑定到第一层上，变相实现仅由第一层计算
         for i in range(1, self.num_hidden_layers):
             self.decoderLayer[i].multiHeadAttention.relative_positions_encoding.weight = self.decoderLayer[0].multiHeadAttention.relative_positions_encoding.weight
         self.final_layer_norm = LayerNorm(self.hidden_size, eps=1e-12, conditional_size=self.conditional_size, bias=False, norm_mode='rmsnorm')
         self.dropout = nn.Dropout(self.dropout_rate)
 
-    def apply_final_layers(self, inputs):
-        inputs[0][1] = self.dropout(self.final_layer_norm([inputs[0][1]]))  # 在转logit前把最后一层的hidden_states加layernorm
-        return super().apply_final_layers(inputs)
+    def apply_final_layers(self, **model_kwargs):
+        # 这里的encoded_layers没有改成decoded_layers是想使用super()
+        last_hidden_states = model_kwargs['decoded_layers'][-1]
+        model_kwargs['decoded_layers'][-1] = self.dropout(self.final_layer_norm([last_hidden_states]))  # 在转logit前把最后一层的hidden_states加layernorm
+        return super().apply_final_layers(**model_kwargs)
 
     def load_variable(self, state_dict, name, prefix=''):
         # 加载单个变量的函数
         variable = state_dict[name]
         if name in {f'decoder.embed_tokens.weight', 'lm_head.weight', 'shared.weight'}:
             return self.load_embeddings(variable)
         else:
@@ -1342,28 +1376,26 @@
             elif self.version.endswith('t5.1.1'):
                 mapping.update({f'{prefix}decoderLayer.{i}.feedForward.intermediateDense.weight': f'decoder.block.{i}.layer.2.DenseReluDense.wi_0.weight',
                                 f'{prefix}decoderLayer.{i}.feedForward.intermediateDense1.weight': f'decoder.block.{i}.layer.2.DenseReluDense.wi_1.weight'})
         return mapping
 
 
 class T5(Transformer):
-    """Google的T5模型（Encoder-Decoder）
-    """
+    """Google的T5模型（Encoder-Decoder）"""
     @delete_arguments('with_pool', 'with_mlm', 'with_nsp')
     def __init__(self, *args,  tie_emb_src_tgt_weight=True, **kwargs):
         super(T5, self).__init__(*args, **kwargs)
         self.tie_emb_src_tgt_weight = tie_emb_src_tgt_weight
 
         # encoder
         self.encoder = T5_Encoder(*args, **kwargs)
-        self.encoder.build(**kwargs)
 
         # decoder
+        kwargs['add_cross_attention'] = True
         self.decoder = T5_Decoder(*args, **kwargs)
-        self.decoder.build(**kwargs)
 
     def load_variable(self, state_dict, name, prefix=''):
         # 加载单个变量的函数
         variable = state_dict[name]
         if name in {'shared.weight', 'encoder.embed_tokens.weight', 'decoder.embed_tokens.weight', 'lm_head.weight'}:
             return self.load_embeddings(variable)
         else:
@@ -1377,29 +1409,29 @@
                             'decoder.embeddings.word_embeddings.weight': 'shared.weight'})
         return mapping
 
 
 class GPT(LM_Mask, BERT):
     """构建GPT模型；
     链接：https://github.com/openai/finetune-transformer-lm
+    Todo: 理论上gpt系列应该从Decoder继承，自动实现is_decoder=True，且使用decoderLayer
     """
-    @insert_arguments(final_activation='softmax')
     @delete_arguments('with_pool', 'with_mlm', 'with_nsp')
-    def __init__(self, max_position, **kwargs):
+    def __init__(self, *args, **kwargs):
         """GPT的embedding是token、position、segment三者embedding之和，跟BERT的主要区别是三者相加之后没有加LayerNormalization层。
            使用LM_Mask实现预训练ckpt中的bias参数，最后的全连接层由于和embedding层权重一致，因此直接从word_embedding取
         """
-        super(GPT, self).__init__(max_position, **kwargs)
+        super(GPT, self).__init__(*args, is_decoder=True, **kwargs)
         del self.embeddings.layerNorm
         self.dense = nn.Linear(self.hidden_size, self.vocab_size, bias=False)
         self.dense.weight = self.embeddings.word_embeddings.weight
-        self.final_activation = get_activation(self.final_activation)
+        self.final_activation = get_activation(kwargs.get('final_activation', 'linear'))
 
-    def apply_final_layers(self, inputs):
-        hidden_state = super().apply_final_layers(inputs)
+    def apply_final_layers(self, **model_kwargs):
+        hidden_state = super().apply_final_layers(**model_kwargs)
         logit = self.dense(hidden_state)
         return self.final_activation(logit)
 
     def load_variable(self, state_dict, name):
         return super(GPT, self).load_variable(state_dict, name, prefix='gpt')
 
     def variable_mapping(self):
@@ -1408,80 +1440,82 @@
         return mapping
 
 
 class GPT2(LM_Mask, BERT):
     """构建GPT模型；
     链接：https://github.com/openai/finetune-transformer-lm
     """
-    @insert_arguments(final_activation='softmax')
     @delete_arguments('with_pool', 'with_mlm', 'with_nsp')
-    def __init__(self, max_position, **kwargs):
+    def __init__(self, *args, **kwargs):
         """GPT2的embedding是token、position两者embedding之和。
            1、跟BERT的主要区别是三者相加之后没有加LayerNormalization层。
            2、bert的layernorm是在attn/ffc之后，OpenAi-gpt2是在之前。
            使用LM_Mask实现预训练ckpt中的bias参数，最后的全连接层由于和embedding层权重一致，因此直接从word_embedding取
         """
-        super(GPT2, self).__init__(max_position, **kwargs)
+        super(GPT2, self).__init__(*args, **kwargs)
         del self.embeddings.layerNorm
-        layer = self.Gpt2Layer(self.hidden_size, self.num_attention_heads, self.dropout_rate, self.attention_probs_dropout_prob, self.intermediate_size, self.hidden_act, is_dropout=self.is_dropout, conditional_size=self.conditional_size)
-        self.encoderLayer = nn.ModuleList([copy.deepcopy(layer) if layer_id in self.keep_hidden_layers else Identity() for layer_id in range(self.num_hidden_layers)])
-        self.LayerNormFinal = LayerNorm(self.hidden_size, eps=1e-12, conditional_size=self.conditional_size)
-        self.dense = nn.Linear(self.hidden_size, self.vocab_size, bias=False)
+        layer = self.Gpt2Layer(is_decoder=True, **self.get_kw('hidden_size', 'num_attention_heads', 'dropout_rate', 'attention_probs_dropout_prob', 
+                                                              'intermediate_size', 'hidden_act', 'is_dropout', 'conditional_size', **kwargs))
+        self.encoderLayer = nn.ModuleList([copy.deepcopy(layer) if layer_id in self.keep_hidden_layers else BlockIdentity() for layer_id in range(self.num_hidden_layers)])
+        self.LayerNormFinal = LayerNorm(self.hidden_size, eps=1e-12, conditional_size=self.conditional_size, bias=kwargs.get('bias', True))
+        self.dense = nn.Linear(self.hidden_size, self.vocab_size, bias=False) 
         self.dense.weight = self.embeddings.word_embeddings.weight
-        self.final_activation = get_activation(self.final_activation)
+        self.final_activation = get_activation(kwargs.get('final_activation', 'linear'))
 
-    def apply_final_layers(self, inputs):
-        hidden_state = super().apply_final_layers(inputs)
+    def apply_final_layers(self, **model_kwargs):
+        hidden_state = super().apply_final_layers(**model_kwargs)
         logit = self.dense(self.LayerNormFinal([hidden_state]))
         return self.final_activation(logit)
 
     def load_variable(self, state_dict, name):
         return super(GPT2, self).load_variable(state_dict, name, prefix='gpt2')
 
     def variable_mapping(self):
         # 映射到GPT权重格式
-        mapping =  super(GPT2, self).variable_mapping(prefix='gpt2')
+        mapping = super(GPT2, self).variable_mapping(prefix='gpt2')
         mapping.update({'LayerNormFinal.weight': 'gpt2.LayerNormFinal.weight',
                         'LayerNormFinal.bias': 'gpt2.LayerNormFinal.bias'})
         return mapping
     
     class Gpt2Layer(BertLayer):
-        '''顺序：LN --> Att --> Add --> LN --> FFN --> Add
-        '''
-        def __init__(self, *args, **kwargs):
-            super().__init__(*args, **kwargs)
-        def forward(self, hidden_states, attention_mask, conditional_emb=None, encoder_hidden_states=None, encoder_attention_mask=None):
+        '''顺序：LN --> Att --> Add --> LN --> FFN --> Add'''
+        def forward(self, hidden_states=None, attention_mask=None, conditional_emb=None, past_key_value=None, **model_kwargs):
             # bert的layernorm是在attn/ffc之后，Openai-gpt2是在之前
             x = self.layerNorm1((hidden_states, conditional_emb))
-            self_attn_output = self.multiHeadAttention(x, attention_mask)
-            hidden_states = hidden_states + self.dropout1(self_attn_output)
+            self_attn_output = self.multiHeadAttention(x, attention_mask, past_key_value=past_key_value)
+            hidden_states = hidden_states + self.dropout1(self_attn_output[0])
+
             x = self.layerNorm2((hidden_states, conditional_emb))
             ffn_output = self.feedForward(x)
             hidden_states = hidden_states + self.dropout2(ffn_output)
-            return hidden_states
+
+            if self.is_decoder:
+                model_kwargs['past_key_value'] = self_attn_output[-1]
+            model_kwargs['hidden_states'] = hidden_states
+            return model_kwargs
 
 
 class GPT2_ML(LM_Mask, BERT):
     """构建GPT2_ML模型；
     链接: https://github.com/imcaspar/gpt2-ml；
     注意：GPT2_ML虽然号称GPT2，但是它的结构其实更接近GPT，它自称GPT2的原因大概是因为它开源的版本参数量达到了GPT2的15亿参数。
-    看完ckpt中的key，和GPT的区别是embedding后也有layernorm，和bert的区别是第一个跳跃链接是在layernorm前，bert是在之后
+    看完ckpt中的key，和GPT的区别是embedding后也有layernorm，和bert的区别是第二个跳跃链接的输入是在layernorm前，bert是在之后
     """
-    @insert_arguments(final_activation='softmax')
     @delete_arguments('with_pool', 'with_mlm', 'with_nsp')
-    def __init__(self, max_position, **kwargs):
-        super().__init__(max_position, **kwargs)
-        layer = self.Gpt2MlLayer(self.hidden_size, self.num_attention_heads, self.dropout_rate, self.attention_probs_dropout_prob, self.intermediate_size, self.hidden_act, is_dropout=self.is_dropout, conditional_size=self.conditional_size)
-        self.encoderLayer = nn.ModuleList([copy.deepcopy(layer) if layer_id in self.keep_hidden_layers else Identity() for layer_id in range(self.num_hidden_layers)])
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        layer = self.Gpt2MlLayer(self.hidden_size, self.num_attention_heads, self.dropout_rate, self.attention_probs_dropout_prob, self.intermediate_size, self.hidden_act, 
+                                 is_dropout=self.is_dropout, conditional_size=self.conditional_size, is_decoder=True)
+        self.encoderLayer = nn.ModuleList([copy.deepcopy(layer) if layer_id in self.keep_hidden_layers else BlockIdentity() for layer_id in range(self.num_hidden_layers)])
         self.dense = nn.Linear(self.hidden_size, self.vocab_size, bias=False)
         self.dense.weight = self.embeddings.word_embeddings.weight
-        self.final_activation = get_activation(self.final_activation)
+        self.final_activation = get_activation(kwargs.get('final_activation', 'linear'))
 
-    def apply_final_layers(self, inputs):
-        hidden_state = super().apply_final_layers(inputs)
+    def apply_final_layers(self, **model_kwargs):
+        hidden_state = super().apply_final_layers(**model_kwargs)
         logit = self.dense(hidden_state)
         return self.final_activation(logit)
 
     def load_variable(self, state_dict, name):
         return super(GPT2_ML, self).load_variable(state_dict, name, prefix='gpt2_ml')
 
     def variable_mapping(self):
@@ -1489,25 +1523,250 @@
         mapping =  super(GPT2_ML, self).variable_mapping(prefix='gpt2_ml')
         return mapping
 
     class Gpt2MlLayer(BertLayer):
         '''未定义在layer.py中是因为该层针对gpt2_ml模型，不可复用；
         顺序：Att --> Add --> LN --> FFN --> Add --> LN
         '''
-        def __init__(self, *args, **kwargs):
-            super().__init__(*args, **kwargs)
-        def forward(self, hidden_states, attention_mask, conditional_emb=None, encoder_hidden_states=None, encoder_attention_mask=None):
-            self_attn_output = self.multiHeadAttention(hidden_states, attention_mask)
-            hidden_states = hidden_states + self.dropout1(self_attn_output)
+        def forward(self, hidden_states=None, attention_mask=None, conditional_emb=None, past_key_value=None, **model_kwargs):
+            self_attn_output = self.multiHeadAttention(hidden_states, attention_mask, past_key_value=past_key_value)
+            hidden_states = hidden_states + self.dropout1(self_attn_output[0])
             x = self.layerNorm1((hidden_states, conditional_emb))
-            # bert的跳跃连接是在layerNorm之后，gpt2_ml是在layerNorm之前
+
             ffn_output = self.feedForward(x)
+            # bert的第二个跳跃连接的输入1是经过了multiHeadAttention+layerNorm1的hidden_states, 即这里的x
+            # gpt2_ml的第二个跳跃连接的输入1是经过了multiHeadAttention的hidden_states, 不加layerNorm1
             hidden_states = hidden_states + self.dropout2(ffn_output)
             hidden_states = self.layerNorm2((hidden_states, conditional_emb))
-            return hidden_states
+            if self.is_decoder:
+                model_kwargs['past_key_value'] = self_attn_output[-1]
+            model_kwargs['hidden_states'] = hidden_states
+            return model_kwargs
+
+
+class LLaMA(LM_Mask, BERT):
+    '''LLaMA
+    链接: https://github.com/facebookresearch/llama
+    改动：模型结构和gpt2类似，去掉bias，简化Norm, feedForward不同
+    '''
+    @delete_arguments('with_pool', 'with_mlm', 'with_nsp')
+    def __init__(self, *args, **kwargs):
+        kwargs.update({'p_bias': 'rotary', 'weight': True, 'bias': False, 'norm_mode': 'rmsnorm', 'is_decoder': True})
+        super().__init__(*args, **kwargs)
+        del self.embeddings.layerNorm
+        layer = self.TransformerBlock(**self.get_kw('hidden_size', 'num_attention_heads', 'dropout_rate', 'attention_probs_dropout_prob', 
+                                                    'intermediate_size', 'hidden_act', 'is_dropout', 'conditional_size', **kwargs))
+        self.encoderLayer = nn.ModuleList([copy.deepcopy(layer) if layer_id in self.keep_hidden_layers else BlockIdentity() for layer_id in range(self.num_hidden_layers)])
+        self.LayerNormFinal = LayerNorm(self.hidden_size, eps=1e-12, conditional_size=self.conditional_size, norm_mode=kwargs['norm_mode'], bias=kwargs['bias'])
+        self.dense = nn.Linear(self.hidden_size, self.vocab_size, bias=False, device=kwargs['skip_init']) 
+        self.final_activation = get_activation(kwargs.get('final_activation', 'linear'))
+        # 修改feedword
+        for layer in self.encoderLayer:
+            layer.feedForward = self.FeedForward(self.hidden_size, self.hidden_size*4, **kwargs)
+
+    def apply_final_layers(self, **model_kwargs):
+        hidden_state = super().apply_final_layers(**model_kwargs)
+        logit = self.dense(self.LayerNormFinal([hidden_state]))
+        return self.final_activation(logit)
+
+    def load_variable(self, state_dict, name):
+        return super(LLaMA, self).load_variable(state_dict, name, prefix='llama')
+
+    def variable_mapping(self, prefix='llama'):
+        # 映射到权重格式
+        mapping = super(LLaMA, self).variable_mapping(prefix=prefix)
+        mapping.update({'LayerNormFinal.weight': f'{prefix}.LayerNormFinal.weight',
+                        'dense.weight': f'{prefix}.dense.weight'})
+        for i in range(self.num_hidden_layers):
+            prefix_i = f'{prefix}.encoder.layer.%d.' % i
+            mapping.update({f'encoderLayer.{i}.feedForward.intermediateDense2.weight': prefix_i + 'intermediate2.dense.weight'})
+        return mapping
+    
+    class TransformerBlock(BertLayer):
+        '''顺序：LN --> Att --> Add --> LN --> FFN --> Add'''
+        def __init__(self, *args, **kwargs):
+            super().__init__(*args, **kwargs)
+            del self.dropout1
+            del self.dropout2
+
+        def forward(self, hidden_states=None, attention_mask=None, conditional_emb=None, past_key_value=None, **model_kwargs):
+            # bert的layernorm是在attn/ffc之后，Openai-gpt2是在之前
+            x = self.layerNorm1((hidden_states, conditional_emb))
+            self_attn_output = self.multiHeadAttention(x, attention_mask, past_key_value=past_key_value, **model_kwargs)
+            hidden_states = hidden_states + self_attn_output[0]
+
+            x = self.layerNorm2((hidden_states, conditional_emb))
+            hidden_states = hidden_states +  self.feedForward(x)
+            if self.is_decoder:
+                model_kwargs['past_key_value'] = self_attn_output[-1]
+            model_kwargs['hidden_states'] = hidden_states
+            return model_kwargs
+        
+    class FeedForward(nn.Module):
+        '''FeedForward和Bert的不一致，Bert只有两个全连接'''
+        def __init__(self, dim: int, hidden_dim: int, multiple_of: int, **kwargs):
+            super().__init__()
+            hidden_dim = int(2 * hidden_dim / 3)
+            hidden_dim = multiple_of * ((hidden_dim + multiple_of - 1) // multiple_of)
+            self.intermediateDense = nn.Linear(dim, hidden_dim, bias=False, device=kwargs['skip_init'])
+            self.outputDense = nn.Linear(hidden_dim, dim, bias=False, device=kwargs['skip_init'])
+            self.intermediateDense2 = nn.Linear(dim, hidden_dim, bias=False, device=kwargs['skip_init'])
+
+        def forward(self, x):
+            return self.outputDense(F.silu(self.intermediateDense(x)) * self.intermediateDense2(x))
+
+
+class GLM(LM_Mask, BERT):
+    '''GLM: https://github.com/THUDM/GLM
+    Unilm设计，可定义为GLM(UniLM_MASK, BERT)但是要求传入segement_ids比较麻烦，这里继承LM_MASK并使用get_masks()重新构造attention_mask
+    模型结构特点：
+    1）rotary使用的updown+position_encoding_2d
+    2）qkv合并成一个权重convert时不是concat在一起的
+    3）attention_mask类似于Unilm，最后一个token仅能访问之前的，之前的tokens可以互相访问
+    4）跳跃连接有权重设计
+    '''
+    @delete_arguments('with_pool', 'with_mlm', 'with_nsp')
+    def __init__(self, *args, **kwargs):
+        kwargs.update({'p_bias': 'rotary', 'weight': True, 'is_decoder': True})
+        super().__init__(*args, **kwargs)
+        self.bos_token_id, self.mask_token_id, self.gmask_token_id = kwargs['bos_token_id'], kwargs['mask_token_id'], kwargs['gmask_token_id']
+        self.position_encoding_2d = kwargs.get('position_encoding_2d', True)
+        del self.embeddings.layerNorm
+        layer = self.GLMBlock(**self.get_kw('hidden_size', 'num_attention_heads', 'dropout_rate', 'attention_probs_dropout_prob', 
+                                            'intermediate_size', 'hidden_act', 'is_dropout', 'conditional_size', 'num_hidden_layers', **kwargs))
+        self.encoderLayer = nn.ModuleList([copy.deepcopy(layer) if layer_id in self.keep_hidden_layers else BlockIdentity() for layer_id in range(self.num_hidden_layers)])
+        self.LayerNormFinal = torch.nn.LayerNorm(self.hidden_size, eps=kwargs.get('layer_norm_eps', 1e-12))
+        self.dense = nn.Linear(self.hidden_size, self.vocab_size, bias=False, device=kwargs['skip_init'])
+        self.final_activation = get_activation(kwargs.get('final_activation', 'linear'))
+
+    def load_variable(self, state_dict, name, prefix='transformer'):
+        """加载单个变量的函数, 这里的名称均为映射前的
+        """
+        variable = state_dict[name]
+        if name in {f'{prefix}.embeddings.word_embeddings.weight', 'lm_head.weight'}:
+            return self.load_embeddings(variable)
+        else:
+            return variable
+        
+    def variable_mapping(self, prefix='transformer'):
+        # 映射到权重格式
+        mapping = {
+            'LayerNormFinal.weight': "transformer.final_layernorm.weight",
+            'LayerNormFinal.bias': "transformer.final_layernorm.bias",
+            'dense.weight': "lm_head.weight",
+            'embeddings.word_embeddings.weight': 'transformer.word_embeddings.weight'}
+
+        for i in range(self.num_hidden_layers):
+            prefix_i = f'{prefix}.layers.%d.' % i
+            mapping.update({
+                f'encoderLayer.{i}.layerNorm1.weight': prefix_i + 'input_layernorm.weight',
+                f'encoderLayer.{i}.layerNorm1.bias': prefix_i + 'input_layernorm.bias',
+                f'encoderLayer.{i}.layerNorm2.weight': prefix_i + 'post_attention_layernorm.weight',
+                f'encoderLayer.{i}.layerNorm2.bias': prefix_i + 'post_attention_layernorm.bias',
+                f'encoderLayer.{i}.multiHeadAttention.q.weight': prefix_i + 'attention.self.query.weight',
+                f'encoderLayer.{i}.multiHeadAttention.q.bias': prefix_i + 'attention.self.query.bias',
+                f'encoderLayer.{i}.multiHeadAttention.k.weight': prefix_i + 'attention.self.key.weight',
+                f'encoderLayer.{i}.multiHeadAttention.k.bias': prefix_i + 'attention.self.key.bias',
+                f'encoderLayer.{i}.multiHeadAttention.v.weight': prefix_i + 'attention.self.value.weight',
+                f'encoderLayer.{i}.multiHeadAttention.v.bias': prefix_i + 'attention.self.value.bias',
+                f'encoderLayer.{i}.multiHeadAttention.o.weight': prefix_i + 'attention.dense.weight',
+                f'encoderLayer.{i}.multiHeadAttention.o.bias': prefix_i + 'attention.dense.bias',
+                f'encoderLayer.{i}.feedForward.intermediateDense.weight': prefix_i + 'mlp.dense_h_to_4h.weight',
+                f'encoderLayer.{i}.feedForward.intermediateDense.bias': prefix_i + 'mlp.dense_h_to_4h.bias',
+                f'encoderLayer.{i}.feedForward.outputDense.weight': prefix_i + 'mlp.dense_4h_to_h.weight',
+                f'encoderLayer.{i}.feedForward.outputDense.bias': prefix_i + 'mlp.dense_4h_to_h.bias',
+                })
+        return mapping
+
+    def get_masks(self, attention_mask, context_lens, prepad_lens):
+        '''调整mask使得在content_lens前是bi_attention'''
+        for i, (prepad_len, context_len) in enumerate(zip(prepad_lens, context_lens)):
+            attention_mask[i, :, :, prepad_len:context_len] = 1
+        return attention_mask
+        
+    def get_position_ids(self, position_ids, seq_len, context_lens, mask_positions, prepad_lens, gmask=False):
+        '''不使用cache时候的postion_ids'''
+        if position_ids.shape[0] == 1:
+            position_ids = position_ids.repeat(len(context_lens), 1)
+        if self.position_encoding_2d:
+            # 初始版本中这里也有not gmask
+            for i, context_length in enumerate(context_lens):
+                position_ids[i, context_length:] = mask_positions[i] - prepad_lens[i]
+            block_position_ids = [torch.cat((torch.zeros(context_len, dtype=torch.long).to(position_ids),
+                                            torch.arange(seq_len-context_len, dtype=torch.long).to(position_ids) + 1)) for context_len in context_lens]
+            block_position_ids = torch.stack(block_position_ids, dim=0)
+            position_ids = torch.stack((position_ids, block_position_ids), dim=1)
+        else:
+            if not gmask:
+                for i, context_length in enumerate(context_lens):
+                    position_ids[context_length:] = mask_positions[i] - prepad_lens[i]
+        return position_ids
+
+    def prepare_inputs(self, *inputs, **model_kwargs):
+        '''对attention_mask(参考unilm方式)和position_ids做处理'''
+        token_ids = model_kwargs['past_token_ids'] if model_kwargs.get('past_token_ids') is not None else inputs[0]
+        mask_token = self.mask_token_id if self.mask_token_id in token_ids else self.gmask_token_id  # 倒数第2位
+        use_gmask = False if self.mask_token_id in token_ids else True
+        position_ids = model_kwargs['position_ids']
+        device = position_ids.device
+        seqs = token_ids.tolist()
+        mask_positions = [seq.index(mask_token) for seq in seqs]
+        context_lens = [seq.index(self.bos_token_id) for seq in seqs]  # bos_token_id是倒数第一位
+        seq_len = token_ids.shape[1]
+
+        # 1）generation阶段use_states=True且step>0的时候(用cache)
+        if model_kwargs.get('use_states', False) and (model_kwargs.get('step') > 0):
+            if self.position_encoding_2d:  # [btz, 2, 1]
+                position_ids = torch.tensor([[mask_position, seq_len - context_len] for mask_position, context_len in
+                                            zip(mask_positions, context_lens)], dtype=torch.long, device=device).unsqueeze(-1)
+            else:  # [btz, 1]
+                position_ids = torch.tensor([mask_position for mask_position in mask_positions], dtype=torch.long, device=device).unsqueeze(-1)
+            model_kwargs['position_ids'] = position_ids
+        # 1）train阶段；2）generation阶段use_states=False；3）use_states=True且step=0的时候
+        else:
+            prepad_lens = [(ts[:l]==3).sum().item() for l, ts in zip(context_lens, token_ids)]
+            model_kwargs['attention_mask'] = self.get_masks(model_kwargs['attention_mask'], context_lens, prepad_lens)
+            model_kwargs['position_ids'] = self.get_position_ids(position_ids, seq_len, context_lens, mask_positions, prepad_lens, gmask=use_gmask)
+        return model_kwargs
+
+    def apply_embeddings(self, *inputs, **model_kwargs):
+        model_kwargs = super().apply_embeddings(*inputs, **model_kwargs)
+        model_kwargs = self.prepare_inputs(*inputs, **model_kwargs)
+        return model_kwargs
+    
+    def apply_final_layers(self, **model_kwargs):
+        hidden_state = super().apply_final_layers(**model_kwargs)
+        logit = self.dense(self.LayerNormFinal(hidden_state))
+        return self.final_activation(logit)
+    
+    class GLMBlock(BertLayer):
+        '''顺序：LN --> Att --> Add --> LN --> FFN --> Add'''
+        def __init__(self, *args, **kwargs):
+            super().__init__(*args, **kwargs)
+            self.num_hidden_layers = kwargs['num_hidden_layers']
+            hidden_size, eps = kwargs['hidden_size'], kwargs.get('layer_norm_eps', 1e-5)
+            self.layerNorm1 = torch.nn.LayerNorm(hidden_size, eps=eps)
+            self.layerNorm2 = torch.nn.LayerNorm(hidden_size, eps=eps)
+            del self.dropout1
+            del self.dropout2
+
+        def forward(self, hidden_states=None, attention_mask=None, past_key_value=None, **model_kwargs):
+            # 和bert区别有两点，一个是有alpha, 还有一个是跳跃链接用的是经过了layernorm后的
+            x = self.layerNorm1(hidden_states)
+            alpha = (2 * self.num_hidden_layers) ** 0.5
+            self_attn_output = self.multiHeadAttention(x, attention_mask, past_key_value=past_key_value, **model_kwargs)
+            hidden_states = x * alpha + self_attn_output[0]
+
+            x = self.layerNorm2(hidden_states)
+            hidden_states = x *alpha +  self.feedForward(x)
+
+            if self.is_decoder:
+                model_kwargs['past_key_value'] = self_attn_output[-1]
+            model_kwargs['hidden_states'] = hidden_states
+            return model_kwargs
 
 
 class Transformer_XL(BERT):
     '''构建transformer-xl模型, 已加载；
     项目: https://github.com/kimiyoung/transformer-xl；
     不同点:  
     1) 简化了原有的AdaptiveEmbedding(可选)和未使用ProjectedAdaptiveLogSoftmax, 直接输出last_hidden_state；
@@ -1523,15 +1782,15 @@
         super().__init__(*args, **kwargs)
         self.mem_len, self.same_length, self.clamp_len = mem_len, same_length, clamp_len
         self.attn_type = kwargs.get('attn_type', 0)
 
         # embedding
         if kwargs.get('adaptive_embedding'):
             cutoffs, div_val, sample_softmax = kwargs.get('cutoffs', []), kwargs.get('div_val', 1), kwargs.get('sample_softmax', False)
-            self.embeddings = AdaptiveEmbedding(self.vocab_size, self.embedding_size, self.hidden_size, cutoffs, div_val, sample_softmax, **get_kw(AdaptiveEmbedding, kwargs))
+            self.embeddings = AdaptiveEmbedding(self.vocab_size, self.embedding_size, self.hidden_size, cutoffs, div_val, sample_softmax)
         else:
             self.embeddings = nn.Embedding(self.vocab_size, self.embedding_size)
         self.pos_embeddings = XlnetPositionsEncoding(self.embedding_size)
         self.dropout = nn.Dropout(self.dropout_rate)
 
         # 每层自己的r_w_bias和r_r_bias，还是公用
         if not kwargs.get('untie_r'):
@@ -1540,40 +1799,37 @@
             if self.segment_vocab_size > 0:
                 self.r_s_bias = nn.Parameter(torch.FloatTensor(self.num_attention_heads, self.attention_head_size))  # 全局segment偏置
         else:
             self.r_w_bias, self.r_r_bias = None, None
             self.r_s_bias = None
 
         # transformer block
-        layer = XlnetLayer(self.hidden_size, self.num_attention_heads, self.dropout_rate, self.attention_probs_dropout_prob, self.intermediate_size, 
-                           self.hidden_act, is_dropout=self.is_dropout, conditional_size=self.conditional_size, r_w_bias=self.r_w_bias, r_r_bias=self.r_r_bias,
-                           r_s_bias=None, **get_kw(BertLayer, kwargs))
-        self.encoderLayer = nn.ModuleList([copy.deepcopy(layer) if layer_id in self.keep_hidden_layers else Identity() for layer_id in range(self.num_hidden_layers)])
+        layer = XlnetLayer(r_s_bias=None, **self.get_kw('hidden_size', 'num_attention_heads', 'dropout_rate', 'attention_probs_dropout_prob', 'intermediate_size', 
+                                                        'hidden_act', 'is_dropout', 'conditional_size', 'r_w_bias', 'r_r_bias', **kwargs))
+        self.encoderLayer = nn.ModuleList([copy.deepcopy(layer) if layer_id in self.keep_hidden_layers else BlockIdentity() for layer_id in range(self.num_hidden_layers)])
 
         # 映射
         if self.with_lm:
             self.dense = nn.Linear(self.hidden_size, self.vocab_size, bias=True)
 
     def init_mems(self, bsz):
-        '''初始化mems, 用于记忆mlen的各层隐含层状态
-        '''
+        '''初始化mems, 用于记忆mlen的各层隐含层状态'''
         if isinstance(self.mem_len, (int, float)) and (self.mem_len > 0):
             mems = []
             param = next(self.parameters())
             for _ in range(self.num_hidden_layers+1):
                 empty = torch.zeros(bsz, self.mem_len, self.hidden_size, dtype=param.dtype, device=param.device)
                 mems.append(empty)
 
             return mems
         else:
             return None
 
     def _update_mems(self, hids, mlen, qlen):
-        '''更新mems
-        '''
+        '''更新mems'''
         # does not deal with None
         if self.mems is None:
             return None
         # mems is not None
         assert len(hids) == len(self.mems), "len(hids) != len(mems)"
         # There are `mlen + qlen` steps that can be cached into mems
         with torch.no_grad():
@@ -1601,17 +1857,16 @@
             mask_shift_len = qlen - mask_len if mask_len > 0 else qlen
             attention_mask = 1-(torch.triu(all_ones, 1+mlen) + torch.tril(all_ones, -mask_shift_len)).byte() # -1
         else:
             attention_mask = torch.tril(word_emb.new_ones(qlen, klen), diagonal=mlen).byte()  # [q_len, k_len], 下三角为1矩阵
         attention_mask = attention_mask[None, None, :, :]
         return attention_mask
 
-    def apply_embeddings(self, inputs):
-        '''接受的inputs输入: [token_ids, segment_ids], 暂不支持条件LayerNorm输入
-        '''
+    def apply_embeddings(self, *inputs, **model_kwargs):
+        '''接受的inputs输入: [token_ids, segment_ids], 暂不支持条件LayerNorm输入'''
         assert isinstance(inputs, (tuple, list)), f'Inputs only support list,tuple format but passed {type(inputs)}'
 
         self.mems = self.init_mems(inputs[0].size(0))  # 生成mems
         # 精简后embeddings中只计算word_emdedding
         word_emb = self.dropout(self.embeddings(inputs[0]))
         index_ = 1
         btz, qlen = inputs[0].shape[:2]  # query长度
@@ -1632,44 +1887,44 @@
             index_ += 1
         else:
             segment_ids = None
 
         if self.attn_type in {'uni', 0}:  # 兼容transformer_xl的设置: 0
             non_tgt_mask = self.create_mask(word_emb, qlen, klen, mlen)
         elif self.attn_type == 'bi':
-            attention_mask = (inputs[0] != self.token_pad_ids).long().unsqueeze(1).unsqueeze(2)
+            attention_mask = (inputs[0] != self.pad_token_id).long().unsqueeze(1).unsqueeze(2)
             non_tgt_mask = torch.eye(qlen).to(attention_mask)[None, None, :, :]
             non_tgt_mask = ((1 - attention_mask - non_tgt_mask) <= 0).long()
+        model_kwargs.update({'hidden_states': word_emb, 'segment_ids': segment_ids, 'pos_emb': pos_emb, 
+                             'attention_mask': non_tgt_mask})
+        return model_kwargs
 
-        return [word_emb, segment_ids, pos_emb, non_tgt_mask, None]
-
-    def apply_main_layers(self, inputs):
-        hidden_states, segment_ids, pos_emb, attention_mask, conditional_emb = inputs[:5]
-        encoded_layers = [hidden_states] # 添加embedding的输出
-
-        layer_inputs = [hidden_states, segment_ids, pos_emb, attention_mask, None, conditional_emb]
-        for i, layer_module in enumerate(self.encoderLayer):
-            mems_i = None if self.mems is None else self.mems[i]
-            layer_inputs[-2] = mems_i
-            layer_inputs = self.apply_on_layer_begin(i, layer_inputs)
-            hidden_states = grad_checkpoint(layer_module, *layer_inputs) if self.gradient_checkpoint else layer_module(*layer_inputs)
-            layer_inputs[0] = hidden_states
-            layer_inputs = self.apply_on_layer_end(i, layer_inputs)
+    def apply_main_layers(self, **model_kwargs):
+        encoded_layers = [model_kwargs['hidden_states']] # 添加embedding的输出
+        for l_i, layer_module in enumerate(self.encoderLayer):
+            mems_i = None if self.mems is None else self.mems[l_i]
+            model_kwargs['mems_i'] = mems_i
+            model_kwargs = self.apply_on_layer_begin(l_i, **model_kwargs)
+            outputs = grad_checkpoint(layer_module, **model_kwargs) if self.gradient_checkpoint else layer_module(**model_kwargs)
+            model_kwargs.update(outputs)
+            hidden_states = model_kwargs['hidden_states']
+            model_kwargs = self.apply_on_layer_end(l_i, **model_kwargs)
             encoded_layers.append(hidden_states)
         
         # 原实现中word_emb, pos_emb和core_out(hidden_states)使用同一个dropout
         hidden_states = self.dropout(hidden_states)
-        qlen = inputs[0].size(1)  # query长度
+        qlen = hidden_states.size(1)  # query长度
         mlen = self.mems[0].size(0) if self.mems is not None else 0
         self._update_mems(encoded_layers, mlen, qlen)
         
         if not self.output_all_encoded_layers:
             # 不返回所有层，即返回顶层
             encoded_layers = encoded_layers[:1] + [hidden_states]
-        return [encoded_layers, conditional_emb]
+        model_kwargs['encoded_layers'] = encoded_layers
+        return model_kwargs
     
     def load_variable(self, state_dict, name, prefix=''):
         # 这里由于预训练模型使用了AdapterEmbedding，因此暂不支持
         if (self.keep_tokens is not None) or (self.compound_tokens is not None):
             raise ValueError('Custom keep_tokens and compound_tokens is not yet supported in Transformer_XL')
         return state_dict[name]
 
@@ -1711,16 +1966,16 @@
             pos_emb = torch.cat([fwd_pos_emb, bwd_pos_emb], dim=0)
         else:
             pos_emb = fwd_pos_emb
 
         pos_emb = self.dropout(pos_emb)  # 用word_emb的dropout
         return pos_emb
 
-    def apply_final_layers(self, inputs):
-        hidden_state = super().apply_final_layers(inputs)
+    def apply_final_layers(self, **model_kwargs):
+        hidden_state = super().apply_final_layers(**model_kwargs)
         if self.with_lm:
             return [hidden_state, self.dense(hidden_state)]
         else:
             return hidden_state
 
     def load_variable(self, state_dict, name, prefix='transformer'):
         # 加载单个变量的函数
@@ -1765,49 +2020,52 @@
         return mapping
 
 
 def build_transformer_model(config_path=None, checkpoint_path=None, model='bert', application='encoder', **kwargs):
     """根据配置文件构建模型，可选加载checkpoint权重
 
     :param config_path: str, 模型的config文件地址
-    :param checkpoint_path: str, 模型文件地址, 默认值None表示不加载预训练模型
+    :param checkpoint_path: str/list[str], 模型文件地址, 默认值None表示不加载预训练模型
     :param model: str, 加载的模型结构, 这里Model也可以基于nn.Module自定义后传入, 默认为'bert'
     :param application: str, 模型应用, 支持encoder, lm和unilm格式, 默认为'encoder'
     :param segment_vocab_size: int, type_token_ids数量, 默认为2, 如不传入segment_ids则需设置为0
     :param with_pool: bool, 是否包含Pool部分, 默认为False
     :param with_nsp: bool, 是否包含NSP部分, 默认为False
     :param with_mlm: bool, 是否包含MLM部分, 默认为False
     :param output_all_encoded_layers: bool, 是否返回所有hidden_state层, 默认为False
-    :param layer_add_embs: nn.Module, 自定义额外的embedding输入, 如nn.Embedding(2, 768)
+    :param additional_embs: bool, 是否有额外的embedding输入
     :param keep_tokens: list[int], 精简词表, 保留的id的序号如：[0, 100, 101, 102, 106, 107, ...]
-    :param token_pad_ids: int, 默认为0, 部分模型padding不是0时在这里指定, 用于attention_mask生成, 如设置成-100
+    :param pad_token_id: int, 默认为0, 部分模型padding不是0时在这里指定, 用于attention_mask生成, 如设置成-100
     :param custom_position_ids: bool, 是否自行传入位置id, True表示传入, False表示不传入, 'start_at_padding'表示从padding_idx+1开始, 默认为False
     :param custom_attention_mask: bool, 是否自行传入attention_mask, 默认为False
     :param shared_segment_embeddings: bool, 若True, 则segment跟token共用embedding, 默认为False
-    :param layer_norm_cond: conditional layer_norm, 默认为None
+    :param conditional_size: conditional layer_norm, 默认为None
     :param add_trainer: bool, 指定从BaseModel继承, 若build_transformer_model后需直接compile()、fit()需设置为True, 默认为None
     :param compound_tokens: 扩展Embedding, 默认为None
     :param residual_attention_scores: bool, Attention矩阵加残差, 默认为False
     :param ignore_invalid_weights: bool, 允许跳过不存在的权重, 默认为False
     :param keep_hidden_layers: 保留的hidden_layer层的id, 默认为None表示全部使用
     :param hierarchical_position: 是否层次分解位置编码, 默认为None表示不使用
     :param gradient_checkpoint: bool, 是否使用gradient_checkpoint, 默认为False
+    :param skip_init: bool, 是否初始化
     :return: A pytorch model instance
     """
-    configs = {}
+    configs = DottableDict()
     if config_path is not None:
         configs.update(json.load(open(config_path)))
     configs.update(kwargs)
     if 'max_position' not in configs:
         configs['max_position'] = configs.get('max_position_embeddings', 512)
     if 'dropout_rate' not in configs:
         configs['dropout_rate'] = configs.get('hidden_dropout_prob')
     if 'segment_vocab_size' not in configs:
         configs['segment_vocab_size'] = configs.get('type_vocab_size', 2)
-    
+    configs['skip_init'] = 'meta' if configs.get('skip_init') is True else 'cpu'
+    configs['add_trainer'] = configs.get('add_trainer', False)
+
     models = {
         'bert': BERT,
         'roberta': BERT,  
         'albert': ALBERT,
         'albert_unshared': ALBERT_Unshared,
         'nezha': NEZHA,
         'roformer': RoFormer,
@@ -1820,14 +2078,16 @@
         'encoder': Encoder,
         'decoder': Decoder,
         'transformer': Transformer,
         'bart': BART,
         'gpt': GPT,
         'gpt2': GPT2,
         'gpt2_ml': GPT2_ML,
+        'llama': LLaMA,
+        'glm': GLM,
         't5': T5,
         't5_encoder': T5_Encoder,
         't5_decoder': T5_Decoder,
         't5.1.0': T5,
         't5.1.0_encoder': T5_Encoder,
         't5.1.0_decoder': T5_Decoder,
         't5.1.1': T5,
@@ -1845,30 +2105,37 @@
         if model.endswith('t5.1.1'):
             configs['version'] = model
     elif isinstance(model, type) and issubclass(model, BERT_BASE): # nn.Module表示使用自定义的模型：
         MODEL = model
     else:
         raise ValueError('"model" args type should be string or nn.Module')
 
+    # 使用 lm/unilm
     application = application.lower()
     if application in ['lm', 'unilm'] and model in ['electra', 't5', ]:
         raise ValueError(f'"{model}" model can not be used as "{application}" application.\n')
-
     if application == 'lm':
         MODEL = extend_with_language_model(MODEL)
     elif application == 'unilm':
         MODEL = extend_with_unified_language_model(MODEL)
 
     # 动态继承BaseModel
-    if configs.get('add_trainer', False):
+    if configs['add_trainer']:
         class MyModel(MODEL, BaseModel): 
             pass
         MODEL = MyModel
 
+    # 生成网络结构
     transformer = MODEL(**configs)
-    transformer.build(**configs)
     transformer.apply(transformer.init_model_weights)  # 初始化权重
 
+    # 预训练模型是否已量化, 加载量化后的权重使用，如果是加载原权重再自行量化这里不需要甚至恶
+    if configs.get('quantization_bit') is not None:
+        bits = configs.pop('quantization_bit')
+        transformer = transformer.half().quantize(bits=bits, **configs)
+
+    # 权重加载
     if checkpoint_path is not None:
-        transformer.load_weights_from_pytorch_checkpoint(checkpoint_path)   
-    transformer.configs = DottableDict(configs)
+        verbose = not configs.get('ignore_invalid_weights', False)
+        transformer.load_weights_from_pytorch_checkpoints(checkpoint_path, verbose=verbose)
+    transformer.configs = transformer.config = configs
     return transformer
```

### Comparing `bert4torch-0.2.7.post2/bert4torch/tokenizers.py` & `bert4torch-0.2.8/bert4torch/tokenizers.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,19 +66,19 @@
         token_end: 句子切分标记，当只有一句话作为输入时，此标记知识作为结束符；当有两句话作为输入时，此标记作为分隔符、最后一句话的结束符
         pad_token: padding填充标记
         token_start: 分类标记，位于整个序列的第一个
         mask_token: mask标记
         pre_tokenize: 外部传入的分词函数，用作对文本进行预分词。如果传入pre_tokenize，则先执行pre_tokenize(text)，然后在它的基础上执行原本的tokenize函数；
         token_translate: 映射字典，主要用在tokenize之后，将某些特殊的token替换为对应的token。
         """
-        self._token_pad = token_pad
-        self._token_unk = token_unk
-        self._token_mask = token_mask
-        self._token_start = token_start
-        self._token_end = token_end
+        self._token_pad = self.pad_token = token_pad
+        self._token_unk = self.unk_token = token_unk
+        self._token_mask = self.mask_token = token_mask
+        self._token_start = self.start_token = token_start
+        self._token_end = self.end_token = token_end
         self.never_split = [i for i in [self._token_unk, self._token_end, self._token_pad, self._token_start, self._token_mask] if isinstance(i, str)]
         if add_special_tokens is not None:
             if isinstance(add_special_tokens, (tuple, list)):
                 self.never_split.extend(add_special_tokens)
             elif isinstance(add_special_tokens, str):
                 self.never_split.append(add_special_tokens)
         self.tokens_trie = self._create_trie(self.never_split)  # trie树主要是为了special_tokens的分词
@@ -194,15 +194,15 @@
         """id序列为对应的token
         """
         raise NotImplementedError
 
     def ids_to_tokens(self, ids):
         """id序列转换为对应的token序列
         """
-        return [self.id_to_token(i) for i in ids]
+        return [self.id_to_token(int(i)) for i in ids]
 
     def decode(self, ids):
         """转为可读文本
         """
         raise NotImplementedError
 
     def _tokenize(self, text):
@@ -235,21 +235,28 @@
         self._token_dict = token_dict
         self._token_dict_inv = {v: k for k, v in token_dict.items()}
 
         self.do_basic_tokenize = do_basic_tokenize
         if do_basic_tokenize:
             self.basic_tokenizer = BasicTokenizer(do_lower_case=do_lower_case, never_split=self.never_split)
         self.wordpiece_tokenizer = WordpieceTokenizer(vocab=self._token_dict, unk_token=self._token_unk, do_tokenize_unk=do_tokenize_unk)
-
+        # 以下写在外面是方便有代码提示
+        self._token_pad_id = self.pad_token_id = None
+        self._token_unk_id = self.unk_token_id = None
+        self._token_mask_id = self.mask_token_id = None
+        self._token_start_id = self.start_token_id = None
+        self._token_end_id = self.end_token_id = None
         for token in ['pad', 'unk', 'mask', 'start', 'end']:
             try:
                 _token_id = token_dict[getattr(self, '_token_%s' % token)]
                 setattr(self, '_token_%s_id' % token, _token_id)
+                setattr(self, '%s_token_id' % token, _token_id)
             except:
-                pass
+                delattr(self, '_token_%s_id' % token)
+                delattr(self, '%s_token_id' % token)
 
     def _tokenize(self, text, pre_tokenize=True):
         """基本分词函数
         """
         # 以下pre_tokenizer逻辑参考bert4keras
         if self._do_lower_case:
             text = lowercase_and_normalize(text, never_split=self.never_split)
@@ -649,28 +656,36 @@
     """基于SentencePiece模型的封装，使用上跟Tokenizer基本一致。
     """
     def __init__(self, sp_model_path, remove_space=True, keep_accents=False, do_lower_case=False, **kwargs):
         super(SpTokenizer, self).__init__(**kwargs)
         import sentencepiece as spm
         self.sp_model = spm.SentencePieceProcessor()
         self.sp_model.Load(sp_model_path)
-        self._token_pad = self.sp_model.id_to_piece(self.sp_model.pad_id())
-        self._token_unk = self.sp_model.id_to_piece(self.sp_model.unk_id())
         self._vocab_size = self.sp_model.get_piece_size()
+        self._token_pad = self.id_to_token(self.sp_model.pad_id())
+        self._token_unk = self.id_to_token(self.sp_model.unk_id())
         self.remove_space = remove_space
         self.keep_accents = keep_accents
         self.do_lower_case = do_lower_case
 
-        for token in ['pad', 'unk', 'mask', 'start', 'end']:
+        # pad和unk肯定存在，改动是为了处理llama中pad_id是-1的情况
+        self._token_pad_id = self.pad_token_id = self.sp_model.pad_id()
+        self._token_unk_id = self.unk_token_id = self.sp_model.unk_id()
+        self._token_mask_id = self.mask_token_id = None
+        self._token_start_id = self.start_token_id = None
+        self._token_end_id = self.end_token_id = None
+        for token in ['mask', 'start', 'end']:
             try:
                 _token = getattr(self, '_token_%s' % token)
                 _token_id = self.sp_model.piece_to_id(_token)
                 setattr(self, '_token_%s_id' % token, _token_id)
+                setattr(self, '%s_token_id' % token, _token_id)
             except:
-                pass
+                delattr(self, '_token_%s_id' % token)
+                delattr(self, '%s_token_id' % token)
 
     def preprocess_text(self, inputs):
         '''从transformers包的tokenization_xlnet移植过来，主要区别是对标点符号的处理
         '''
         if self.remove_space:
             outputs = " ".join(inputs.strip().split())
         else:
@@ -688,15 +703,15 @@
         """token转换为对应的id
         """
         return self.sp_model.piece_to_id(token)
 
     def id_to_token(self, i):
         """id转换为对应的token
         """
-        if i < self._vocab_size:
+        if (0 <= i) and (i < self._vocab_size):
             return self.sp_model.id_to_piece(i)
         else:
             return ''
 
     def decode(self, ids):
         """转为可读文本
         """
```

### Comparing `bert4torch-0.2.7.post2/bert4torch.egg-info/PKG-INFO` & `bert4torch-0.2.8/bert4torch.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,122 +1,130 @@
 Metadata-Version: 2.1
 Name: bert4torch
-Version: 0.2.7.post2
+Version: 0.2.8
 Summary: an elegant bert4torch
 Home-page: https://github.com/Tongjilibo/bert4torch
 Author: Tongjilibo
 License: MIT Licence
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # bert4torch
+
 **一款用pytorch来复现bert4keras的简洁训练框架**
 
-[![licence](https://img.shields.io/github/license/Tongjilibo/bert4torch.svg?maxAge=3600)](https://github.com/Tongjilibo/bert4torch/blob/master/LICENSE) 
-[![GitHub release](https://img.shields.io/github/release/Tongjilibo/bert4torch.svg?maxAge=3600)](https://github.com/Tongjilibo/bert4torch/releases) 
-[![PyPI](https://img.shields.io/pypi/v/bert4torch?label=pypi%20package)](https://pypi.org/project/bert4torch/) 
+[![licence](https://img.shields.io/github/license/Tongjilibo/bert4torch.svg?maxAge=3600)](https://github.com/Tongjilibo/bert4torch/blob/master/LICENSE)
+[![GitHub release](https://img.shields.io/github/release/Tongjilibo/bert4torch.svg?maxAge=3600)](https://github.com/Tongjilibo/bert4torch/releases)
+[![PyPI](https://img.shields.io/pypi/v/bert4torch?label=pypi%20package)](https://pypi.org/project/bert4torch/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/bert4torch)](https://pypistats.org/packages/bert4torch)
 [![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/bert4torch?style=social)](https://github.com/Tongjilibo/bert4torch)
 [![GitHub Issues](https://img.shields.io/github/issues/Tongjilibo/bert4torch.svg)](https://github.com/Tongjilibo/bert4torch/issues)
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Tongjilibo/bert4torch/issues)
 
 [Documentation](https://bert4torch.readthedocs.io) |
 [Torch4keras](https://github.com/Tongjilibo/torch4keras) |
 [Examples](https://github.com/Tongjilibo/bert4torch/blob/master/examples)
 
 ## 1. 下载安装
+
 安装稳定版
+
 ```shell
 pip install bert4torch
 ```
+
 安装最新版
+
 ```shell
-pip install git+https://www.github.com/Tongjilibo/bert4torch.git
+pip install git+https://github.com/Tongjilibo/bert4torch
 ```
+
 - **注意事项**：pip包的发布慢于git上的开发版本，git clone**注意引用路径**，注意权重是否需要转换
 - **测试用例**：`git clone https://github.com/Tongjilibo/bert4torch`，修改example中的预训练模型文件路径和数据路径即可启动脚本
 - **自行训练**：针对自己的数据，修改相应的数据处理代码块
 - **开发环境**：使用`torch==1.10`版本进行开发，如其他版本遇到不适配，欢迎反馈
 
 ## 2. 功能
+
+- **LLM模型**: 加载chatglm-6b和llama-7b进行推理和finetune
 - **核心功能**：加载bert、roberta、albert、xlnet、nezha、bart、RoFormer、RoFormer_V2、ELECTRA、GPT、GPT2、T5、GAU-alpha、ERNIE等预训练权重继续进行finetune、并支持在bert基础上灵活定义自己模型
 - [**丰富示例**](https://github.com/Tongjilibo/bert4torch/blob/master/examples/)：包含[pretrain](https://github.com/Tongjilibo/bert4torch/blob/master/examples/pretrain)、[sentence_classfication](https://github.com/Tongjilibo/bert4torch/blob/master/examples/sentence_classfication)、[sentence_embedding](https://github.com/Tongjilibo/bert4torch/tree/master/examples/sentence_embedding)、[sequence_labeling](https://github.com/Tongjilibo/bert4torch/blob/master/examples/sequence_labeling)、[relation_extraction](https://github.com/Tongjilibo/bert4torch/blob/master/examples/relation_extraction)、[seq2seq](https://github.com/Tongjilibo/bert4torch/blob/master/examples/seq2seq)、[serving](https://github.com/Tongjilibo/bert4torch/blob/master/examples/serving/)等多种解决方案
 - **实验验证**：已在公开数据集实验验证，使用如下[examples数据集](https://github.com/Tongjilibo/bert4torch/blob/master/examples/README.md)
 - **易用trick**：集成了常见的[trick](https://github.com/Tongjilibo/bert4torch/blob/master/examples/training_trick)，即插即用
 - **其他特性**：[加载transformers库模型](https://github.com/Tongjilibo/bert4torch/blob/master/examples/tutorials/tutorials_load_transformers_model.py)一起使用；调用方式简洁高效；有训练进度条动态展示；配合torchinfo打印参数量；默认Logger和Tensorboard简便记录训练过程；自定义fit过程，满足高阶需求
 - **训练过程**：
 
-    ```text
-    2022-10-28 23:16:10 - Start Training
-    2022-10-28 23:16:10 - Epoch: 1/5
-    5000/5000 [==============================] - 13s 3ms/step - loss: 0.1351 - acc: 0.9601
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 798.09it/s] 
-    test_acc: 0.98045. best_test_acc: 0.98045
-
-    2022-10-28 23:16:27 - Epoch: 2/5
-    5000/5000 [==============================] - 13s 3ms/step - loss: 0.0465 - acc: 0.9862
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 635.78it/s] 
-    test_acc: 0.98280. best_test_acc: 0.98280
-
-    2022-10-28 23:16:44 - Epoch: 3/5
-    5000/5000 [==============================] - 15s 3ms/step - loss: 0.0284 - acc: 0.9915
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 673.60it/s] 
-    test_acc: 0.98365. best_test_acc: 0.98365
-
-    2022-10-28 23:17:03 - Epoch: 4/5
-    5000/5000 [==============================] - 15s 3ms/step - loss: 0.0179 - acc: 0.9948
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 692.34it/s] 
-    test_acc: 0.98265. best_test_acc: 0.98365
-
-    2022-10-28 23:17:21 - Epoch: 5/5
-    5000/5000 [==============================] - 14s 3ms/step - loss: 0.0129 - acc: 0.9958
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 701.77it/s] 
-    test_acc: 0.98585. best_test_acc: 0.98585
+  ```text
+  2022-10-28 23:16:10 - Start Training
+  2022-10-28 23:16:10 - Epoch: 1/2
+  5000/5000 [==============================] - 13s 3ms/step - loss: 0.1351 - acc: 0.9601
+  Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 798.09it/s] 
+  test_acc: 0.98045. best_test_acc: 0.98045
+
+  2022-10-28 23:16:27 - Epoch: 2/2
+  5000/5000 [==============================] - 13s 3ms/step - loss: 0.0465 - acc: 0.9862
+  Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 635.78it/s] 
+  test_acc: 0.98280. best_test_acc: 0.98280
 
-    2022-10-28 23:17:37 - Finish Training
-    ```
+  2022-10-28 23:16:44 - Finish Training
+  ```
 
 ## 3. 快速上手
+
 - [Quick-Start](https://bert4torch.readthedocs.io/en/latest//Quick-Start.html)
 - [快速上手教程](https://github.com/Tongjilibo/bert4torch/blob/master/examples/tutorials/Tutorials.md)，[教程示例](https://github.com/Tongjilibo/bert4torch/blob/master/examples/tutorials)，[实战示例](https://github.com/Tongjilibo/bert4torch/blob/master/examples)
 - [bert4torch介绍(知乎)](https://zhuanlan.zhihu.com/p/486329434)，[bert4torch快速上手(知乎)](https://zhuanlan.zhihu.com/p/508890807)，[bert4torch又双叒叕更新啦(知乎)](https://zhuanlan.zhihu.com/p/560885427?)
 
-## 4. 版本说明
-### 4.1 更新历史
+## 4. 版本历史
+
+<details><summary><b>点击查看</b></summary>
+
+**版本说明**
+- **v0.2.8**：20230518 增加chatglm-6b/llama-7b预训练模型, 修改rope为不使用max_position，修复model.half()类型不一致问题，生成式解码新增SeqGeneration和Seq2SeqGeneration, 支持加载多个权重文件, gpt系列默认不加softmax，更新fnlp的bart2.0。增加苏神Tiger的pytorch实现, 集成苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型, 增加了对attention_key_size的入参支持(skykiseki用户); 修复model.half()类型不一致问题，生成式解码新增SeqGeneration和Seq2SeqGeneration, 支持加载多个权重文件, gpt系列默认不加softmax; 增加苏神Tiger的pytorch实现, 集成苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型, 增加了对attention_key_size的入参支持，单向decoder模型和encoder decoder模型解码增加cache, 更新fnlp的bart2.0, 增加chatglm-6b预训练模型推理, 集成BELLE_llama模型, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2，增加moss模型的int4/int8推理; 增加vicuna的集成, 增加batch_generate()功能, 把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
 - **v0.2.7.post2**：20230310 增加lion优化器, 修复albert_unshared加载权重, 修复lm系列(gpt, seq2seq)存在的forward参数不对的问题，修复GlobalPointer使用rope的bug
 - **v0.2.7**：20230213 修复random_sample()的bug，适配v0.0.6的torch4keras：增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现，增加了AccelerateCallback
 - **v0.2.6**：20221231 build_transformer_model需显式指定add_trainer才从BaseModel继承, 增加guwenbert, macbert，text2vec-bert-chinese, wobert预训练模型，允许position_ids从padding开始, transformer.configs支持点操作，可以使用torch4keras的Trainer(net)来初始化, 修复tokenizer的切分subtoken的bug, 允许embedding_size!=hidden_size
 - **v0.2.5**：20221127 对抗训练从compile转为使用Callback来实现，修复1.7.1版本兼容bug, uie模型内置
 - **v0.2.4**：20221120 删除SpTokenizer基类中的rematch, 增加deberta_v2模型
 - **v0.2.3**：20221023 虚拟对抗VAT在多个ouput时支持指定，把Trainer抽象到[torch4keras](https://github.com/Tongjilibo/torch4keras)中，修复DP和DDP出现resume_epoch不存在的bug, tokenizer的never_split去除None, transformer_xl的bug, 增加gradient_checkpoint
 - **v0.2.2**：20220922 修复t5的norm_mode问题，允许hidden_size不整除num_attention_heads，支持多个schedule(如同时ema+warmup)
 - **v0.2.1**：20220905 兼容torch<=1.7.1的torch.div无rounding_mode，增加自定义metrics，支持断点续训，增加默认Logger和Tensorboard日志
-- **v0.2.0**：20220823 兼容torch<1.9.0的缺失take_along_dim，修复bart中位置向量514的问题，修复Sptokenizer对符号不转换，打印Epoch开始的时间戳，增加parallel_apply
+- **v0.2.0**：20220823 兼容torch1.9.0的缺失take_along_dim，修复bart中位置向量514的问题，修复Sptokenizer对符号不转换，打印Epoch开始的时间戳，增加parallel_apply
 - **v0.1.9**：20220808 增加mixup/manifold_mixup/temporal_ensembling策略，修复pgd策略param.grad为空的问题，修改tokenizer支持批量
 - **v0.1.8**：20220717 修复原来CRF训练中loss陡增的问题，修复xlnet的token_type_ids输入显存占用大的问题
 - **v0.1.7**：20220710 增加EarlyStop，CRF中自带转bool类型
 - **v0.1.6**：20220605 增加transformer_xl、xlnet、t5_pegasus模型，prompt、预训练等示例，支持增加embedding输入，EMA策略，修复tokenizer和sinusoid的bug
 - **v0.1.5**：20220504 增加GAU-alpha，混合梯度，梯度裁剪，单机多卡(DP、DDP)
 - **v0.1.4**：20220421 增加了VAT，修复了linux下apply_embedding返回项有问题的情况
 - **v0.1.3**：20220409 初始版本
 
-### 4.2 版本对应关系
-| bert4torch版本 |  torch4keras版本 |
-|  ----  |  ----  |
-|  0.2.7  | 0.0.6 |
-|  0.2.6  | 0.0.5 |
-|  0.2.5  | 0.0.4 |
-|  0.2.4  | 0.0.3.post2 |
-|  0.2.3  | 0.0.2 |
-|  <0.2.3  | —— |
-
+**版本对应关系**
 
-## 5. 更新：
+| bert4torch版本 | torch4keras版本 |
+| ---------------- | ----------------- |
+| 0.2.8          | 0.0.7.post3     |
+| 0.2.7.post2    | 0.0.6           |
+| 0.2.7          | 0.0.6           |
+| 0.2.6          | 0.0.5           |
+| 0.2.5          | 0.0.4           |
+| 0.2.4          | 0.0.3.post2     |
+| 0.2.3          | 0.0.2           |
+| <0.2.3         | ——            |
+
+</details>
+
+
+## 5. 更新历史：
+<details><summary><b>点击查看</b></summary>
+
+- **20230426**：增加vicuna的集成, 增加batch_generate()功能, 把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
+- **20230408**：增加苏神Tiger的pytorch实现, 集成苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型, 增加了对attention_key_size的入参支持，单向decoder模型和encoder decoder模型解码增加cache, 更新fnlp的bart2.0, 增加chatglm-6b预训练模型推理, 集成BELLE_llama模型, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2，增加moss模型的int4/int8推理
+- **20230326**：增加llama-7b预训练模型, 修改rope为不使用max_position, 增加prompt_clue和nezha_gpt_dialog的finetune示例(skykiseki用户)，修复model.half()类型不一致问题，生成式解码新增SeqGeneration和Seq2SeqGeneration, 支持加载多个权重文件, gpt系列默认不加softmax
 - **20230310**：增加lion优化器, 修改dp和ddp示例更易用，增加PromptCLUE模型, 修复albert_unshared加载权重, 增加uer-gpt2-chinese预训练模型，修复lm系列(gpt, seq2seq)存在的forward参数不对的问题，修复GlobalPointer使用rope的bug
-- **20230212**：兼容accelerate包, 增加ChatYuan模型，修复random_sample()的bug
+- **20230212**：兼容accelerate包, 增加ChatYuan v1模型，修复random_sample()的bug
 - **20221230**：增加macbert，text2vec-bert-chinese, wobert模型，增加LEAR的ner示例, 增加PGRC、SPN4RE的关系提取示例，transformer.configs支持点操作，可以使用torch4keras的Trainer(net)来初始化, 修复tokenizer的切分subtoken的bug, 允许embedding_size!=hidden_size
 - **20221127**：增加deberta_v2模型, 对抗训练从compile转为使用Callback来实现，修复1.7.1版本兼容bug, uie模型内置, 增加triton示例, build_transformer_model需显式指定add_trainer才从BaseModel继承, 增加guwenbert预训练模型，允许position_ids从padding开始
 - **20221102**：增加CNN_Nested_NER示例, 删除SpTokenizer基类中的rematch
 - **20221022**：修复DP和DDP出现resume_epoch不存在的bug, tokenizer的never_split去除None, transformer_xl的bug, 增加gradient_checkpoint
 - **20221011**：虚拟对抗VAT在多个ouput时支持指定，增加elasticsearch示例, 把Trainer抽象到[torch4keras](https://github.com/Tongjilibo/torch4keras)中供更多项目使用，把梯度累积移到compile中
 - **20220920**：增加TensorRT示例，支持多个schedule(如同时ema+warmup)，sanic+onnx部署
 - **20220910**：增加默认Logger和Tensorboard日志，ONNX推理，增加ERNIE模型，修复t5的norm_mode问题，允许hidden_size不整除num_attention_heads
@@ -135,76 +143,98 @@
 - **20220425**：增加了VAT、GAU-alpha等示例，增加了梯度累积，自定义fit()示例
 - **20220415**：增加了ner_mrc、ner_span、roformer_v2、roformer-sim等示例
 - **20220405**：增加了GPLinker、TPlinker、SimBERT等示例
 - **20220329**：增加了CoSENT、R-Drop、UDA等示例
 - **20220322**：添加GPT、GPT2、T5模型
 - **20220312**：初版提交
 
+</details>
 
 ## 6. 预训练权重
+
 - 部分权重是要加载修改的[config.json](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)
 
-| 模型分类 |  权重来源 | 权重链接 | 备注(若有) | 
-|  ----  |  ----  | ----  | ----  |
-|  bert  | 谷歌原版bert(即bert-base-chinese) | [tf](https://github.com/google-research/bert)，[torch](https://huggingface.co/bert-base-chinese) | [tf转pytorch命令](https://huggingface.co/docs/transformers/converting_tensorflow_models)，[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bert-base-chinese.py)
-|  bert  | 哈工大chinese-bert-wwm-ext | [tf/torch](https://github.com/ymcui/Chinese-BERT-wwm)，[torch](https://huggingface.co/hfl/chinese-bert-wwm-ext) |
-|  macbert  | 哈工大chinese-macbert-base/large | [tf/torch](https://github.com/ymcui/MacBERT)，[torch](https://huggingface.co/hfl/chinese-macbert-base) |
-| robert | 哈工大chinese-robert-wwm-ext | [tf/torch](https://github.com/ymcui/Chinese-BERT-wwm)，[torch](https://huggingface.co/hfl/chinese-roberta-wwm-ext)
-| deberta_v2| IDEA Erlangshen-DeBERTa-v2 | [torch](https://huggingface.co/IDEA-CCNL/Erlangshen-DeBERTa-v2-320M-Chinese/tree/main) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_deberta_v2.py) |
-| guwenbert | 古文bert | [torch](https://huggingface.co/ethanyt/guwenbert-base)|[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_guwenbert-base.py)|
-| xlnet | 哈工大xlnet | [tf/torch](https://github.com/ymcui/Chinese-XLNet) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)
-| electra | 哈工大electra | [tf](https://github.com/ymcui/Chinese-ELECTRA)，[torch](https://huggingface.co/hfl/chinese-electra-base-discriminator)
-| macbert | 哈工大macbert | [tf](https://github.com/ymcui/MacBERT)，[torch](https://huggingface.co/hfl/chinese-macbert-base)
-| albert | brightmart | [tf](https://github.com/brightmart/albert_zh)，[torch](https://huggingface.co/voidful)，[torch](https://github.com/lonePatient/albert_pytorch)
-| ernie | 百度文心 |[paddle](https://github.com/PaddlePaddle/ERNIE)，[torch](https://huggingface.co/nghuyong) | 
-| roformer | 追一科技 | [tf](https://github.com/ZhuiyiTechnology/roformer)，[torch](https://huggingface.co/junnyu/roformer_chinese_base) |  
-| roformer_v2 | 追一科技 | [tf](https://github.com/ZhuiyiTechnology/roformer-v2)，[torch](https://huggingface.co/junnyu/roformer_v2_chinese_char_base) | 
-| simbert | 追一科技 | [tf](https://github.com/ZhuiyiTechnology/simbert)，[torch_base](https://huggingface.co/peterchou/simbert-chinese-base/tree/main) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_simbert.py) |
-| roformer-sim | 追一科技 | [tf](https://github.com/ZhuiyiTechnology/roformer-sim)，[torch](https://huggingface.co/junnyu/roformer_chinese_sim_char_base) | 
-| gau-alpha | 追一科技 | [tf](https://github.com/ZhuiyiTechnology/GAU-alpha) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_GAU_alpha.py)
-| wobert | 追一科技 | [tf](https://github.com/ZhuiyiTechnology/WoBERT)，[torch_base](https://huggingface.co/junnyu/wobert_chinese_base)，[torch_plus_base](https://huggingface.co/junnyu/wobert_chinese_plus_base)||
-| nezha | 华为 | [tf](https://github.com/huawei-noah/Pretrained-Language-Model/tree/master/NEZHA-TensorFlow)，[torch](https://github.com/lonePatient/NeZha_Chinese_PyTorch) | 
-| gpt | thu-coai/CDial-GPT | [torch](https://github.com/thu-coai/CDial-GPT) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_gpt__CDial-GPT-LCCC.py)
-| gpt2 | 清华26亿 cmp_lm | [torch](https://github.com/TsinghuaAI/CPM-1-Generate) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_gpt2__cmp_lm_2.6b.py)
-| gpt2 | 中文GPT2_ML模型 | [tf](https://github.com/imcaspar/gpt2-ml)，[torch](https://github.com/ghosthamlet/gpt2-ml-torch) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_gpt2__gpt2-ml.py)
-| gpt2 | UER | [torch](https://huggingface.co/uer/gpt2-chinese-cluecorpussmall) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_gpt2__uer-gpt2-chinese.py) |
-| t5 | UER | [torch](https://huggingface.co/uer/t5-base-chinese-cluecorpussmall) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)
-| mt5 | 谷歌 | [torch](https://huggingface.co/google/mt5-base) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)
-| t5_pegasus | 追一科技 | [tf](https://github.com/ZhuiyiTechnology/t5-pegasus) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_t5_pegasus.py)
-| bart | 复旦 | [torch](https://github.com/fastnlp/CPT) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bart_fudanNLP.py)
-| text2vec | text2vec-base-chinese | [torch](https://huggingface.co/shibing624/text2vec-base-chinese) | 
-| chatyuan | clue-ai | [torch](https://github.com/clue-ai/ChatYuan) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)
-| PromptCLUE | clue-ai | [torch](https://github.com/clue-ai/PromptCLUE) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)
+
+| 模型分类| 权重来源| 权重链接 | 备注(若有)|
+| ----- | ----- | ----- | ----- |
+| bert| 谷歌原版bert(即bert-base-chinese) | [tf](https://github.com/google-research/bert)，[torch](https://huggingface.co/bert-base-chinese) | [tf转pytorch命令](https://huggingface.co/docs/transformers/converting_tensorflow_models)，[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bert-base-chinese.py) |
+| bert| 哈工大chinese-bert-wwm-ext| [tf/torch](https://github.com/ymcui/Chinese-BERT-wwm)，[torch](https://huggingface.co/hfl/chinese-bert-wwm-ext)| |
+| macbert | 哈工大chinese-macbert-base/large| [tf/torch](https://github.com/ymcui/MacBERT)，[torch](https://huggingface.co/hfl/chinese-macbert-base) | |
+| roberta | 哈工大chinese-roberta-wwm-ext | [tf/torch](https://github.com/ymcui/Chinese-BERT-wwm)，[torch](https://huggingface.co/hfl/chinese-roberta-wwm-ext) | |
+| roberta-small/tiny| 追一科技 & UER| [tf](https://github.com/ZhuiyiTechnology/pretrained-models)，[torch](https://huggingface.co/uer) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_roberta-small.py) |
+| deberta_v2| IDEA Erlangshen-DeBERTa-v2| [torch](https://huggingface.co/IDEA-CCNL/Erlangshen-DeBERTa-v2-320M-Chinese/tree/main) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_deberta_v2.py)|
+| guwenbert | 古文bert| [torch](https://huggingface.co/ethanyt/guwenbert-base) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_guwenbert-base.py)|
+| xlnet | 哈工大xlnet | [tf/torch](https://github.com/ymcui/Chinese-XLNet) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
+| electra | 哈工大electra | [tf](https://github.com/ymcui/Chinese-ELECTRA)，[torch](https://huggingface.co/hfl/chinese-electra-base-discriminator) | |
+| macbert | 哈工大macbert | [tf](https://github.com/ymcui/MacBERT)，[torch](https://huggingface.co/hfl/chinese-macbert-base) | |
+| albert| brightmart| [tf](https://github.com/brightmart/albert_zh)，[torch](https://huggingface.co/voidful)，[torch](https://github.com/lonePatient/albert_pytorch) | |
+| ernie | 百度文心| [paddle](https://github.com/PaddlePaddle/ERNIE)，[torch](https://huggingface.co/nghuyong)| |
+| roformer| 追一科技| [tf](https://github.com/ZhuiyiTechnology/roformer)，[torch](https://huggingface.co/junnyu/roformer_chinese_base) | |
+| roformer_v2 | 追一科技| [tf](https://github.com/ZhuiyiTechnology/roformer-v2)，[torch](https://huggingface.co/junnyu/roformer_v2_chinese_char_base)| |
+| simbert | 追一科技| [tf](https://github.com/ZhuiyiTechnology/simbert)，[torch_base](https://huggingface.co/peterchou/simbert-chinese-base/tree/main) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_simbert.py) |
+| simbert_v2/roformer-sim | 追一科技| [tf](https://github.com/ZhuiyiTechnology/roformer-sim)，[torch](https://huggingface.co/junnyu/roformer_chinese_sim_char_base)| |
+| gau-alpha | 追一科技| [tf](https://github.com/ZhuiyiTechnology/GAU-alpha)| [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_GAU_alpha.py) |
+| wobert| 追一科技| [tf](https://github.com/ZhuiyiTechnology/WoBERT)，[torch_base](https://huggingface.co/junnyu/wobert_chinese_base)，[torch_plus_base](https://huggingface.co/junnyu/wobert_chinese_plus_base) | |
+| nezha | 华为| [tf](https://github.com/huawei-noah/Pretrained-Language-Model/tree/master/NEZHA-TensorFlow)，[torch](https://github.com/lonePatient/NeZha_Chinese_PyTorch) | |
+| gpt | thu-coai/CDial-GPT| [torch](https://github.com/thu-coai/CDial-GPT) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_gpt__CDial-GPT-LCCC.py) |
+| gpt2| 清华26亿 cmp_lm | [torch](https://github.com/TsinghuaAI/CPM-1-Generate)| [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_gpt2__cmp_lm_2.6b.py) |
+| gpt2| 中文GPT2_ML模型 | [tf](https://github.com/imcaspar/gpt2-ml)，[torch](https://github.com/ghosthamlet/gpt2-ml-torch) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_gpt2__gpt2-ml.py) |
+| gpt2| UER | [torch](https://huggingface.co/uer/gpt2-chinese-cluecorpussmall) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_gpt2__uer-gpt2-chinese.py)|
+| t5| UER | [torch](https://huggingface.co/uer/t5-base-chinese-cluecorpussmall)| [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
+| mt5 | 谷歌| [torch](https://huggingface.co/google/mt5-base)| [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
+| t5_pegasus| 追一科技| [tf](https://github.com/ZhuiyiTechnology/t5-pegasus) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_t5_pegasus.py)|
+| bart| 复旦| [torch](https://github.com/fastnlp/CPT), [v1.0](https://huggingface.co/fnlp/bart-base-chinese/tree/v1.0), [v2.0](https://huggingface.co/fnlp/bart-base-chinese/tree/v2.0)| [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bart_fudanNLP.py) |
+| text2vec| text2vec-base-chinese | [torch](https://huggingface.co/shibing624/text2vec-base-chinese) | |
+| chatyuan v1&v2| clue-ai | [torch](https://github.com/clue-ai/ChatYuan) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
+| PromptCLUE| clue-ai | [torch](https://github.com/clue-ai/PromptCLUE) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
+| llama | facebook| [torch](https://github.com/facebookresearch/llama) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_facebook.py)|
+| vicuna | FastChat| [torch](https://huggingface.co/AlekseyKorshuk/vicuna-7b) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_vicuna.py)|
+| Belle| LianjiaTech| [torch](https://huggingface.co/BelleGroup/BELLE-LLaMA-7B-2M-enc) | [合成说明](https://github.com/LianjiaTech/BELLE/tree/main/models)、[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_belle.py)|
+| chatglm | THUDM | [torch](https://github.com/THUDM/ChatGLM-6B) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_chatglm.py) |
 
 ## 7. 鸣谢
-- 感谢苏神实现的[bert4keras](https://github.com/bojone/bert4keras)，本实现有不少地方参考了bert4keras的源码，在此衷心感谢大佬的无私奉献; 
-- 其次感谢项目[bert4pytorch](https://github.com/MuQiuJun-AI/bert4pytorch)，也是在该项目的指引下给了我用pytorch来复现bert4keras的想法和思路。
 
+- 感谢苏神实现的[bert4keras](https://github.com/bojone/bert4keras)，本实现有不少地方参考了bert4keras的源码，在此衷心感谢大佬的无私奉献;
+- 其次感谢项目[bert4pytorch](https://github.com/MuQiuJun-AI/bert4pytorch)，也是在该项目的指引下给了我用pytorch来复现bert4keras的想法和思路。
 
 ## 8. 引用
+
 ```
 @misc{bert4torch,
   title={bert4torch},
   author={Bo Li},
   year={2022},
   howpublished={\url{https://github.com/Tongjilibo/bert4torch}},
 }
 ```
 
-## 9. 交流
+## 9. 其他
+
 - Wechat Discussions
 
 <table border="0">
   <tbody>
     <tr align="center" >
       <td>
-        ​ <a href="https://github.com/Tongjilibo"><img width="200" height="250" src="./docs/pics/wechat.jpg" alt="pic"></a><br>
-        ​ <a href="https://github.com/Tongjilibo">微信号</a> ​
-​
+         <a href="https://github.com/Tongjilibo"><img width="200" height="250" src="./docs/pics/wechat.jpg" alt="pic"></a><br>
+         <a href="https://github.com/Tongjilibo">微信号</a> 
       </td>
       <td>
          <a href="https://github.com/Tongjilibo"><img width="200" height="250" src="./docs/pics/wechat_group.jpg" alt="pic"></a><br>
-         <a href="https://github.com/Tongjilibo">微信群</a> ​
+         <a href="https://github.com/Tongjilibo">微信群</a> 
+      </td>
+    </tr>
+  </tbody>
+</table>
+
+- Star History Chart
+
+<table border="0">
+  <tbody>
+    <tr align="center" >
+      <td>
+         <a href="https://star-history.com/#Tongjilibo/bert4torch&Date"><img width="400" height="250" src="https://api.star-history.com/svg?repos=Tongjilibo/bert4torch&type=Date" alt="pic"></a><br>
+         <a href="https://star-history.com/#Tongjilibo/bert4torch&Date">Star History Chart</a> 
       </td>
     </tr>
   </tbody>
 </table>
```

### Comparing `bert4torch-0.2.7.post2/setup.py` & `bert4torch-0.2.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='bert4torch',
-    version='v0.2.7.post2',
+    version='v0.2.8',
     description='an elegant bert4torch',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT Licence',
     url='https://github.com/Tongjilibo/bert4torch',
     author='Tongjilibo',
-    install_requires=['torch>1.6', 'torch4keras==0.0.6'],
+    install_requires=['torch>1.6', 'torch4keras==0.0.7.post3'],
     packages=find_packages()
 )
```

