# Comparing `tmp/torch4keras-0.0.7.post2.tar.gz` & `tmp/torch4keras-0.0.7.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/torch4keras-0.0.7.post2.tar", last modified: Wed May 17 03:08:54 2023, max compression
+gzip compressed data, was "torch4keras-0.0.7.post3.tar", last modified: Thu May 18 14:52:57 2023, max compression
```

## Comparing `torch4keras-0.0.7.post2.tar` & `torch4keras-0.0.7.post3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 lb         (501) staff       (20)        0 2023-05-17 03:08:54.000000 torch4keras-0.0.7.post2/
--rw-r--r--   0 lb         (501) staff       (20)     7400 2023-05-17 03:08:54.000000 torch4keras-0.0.7.post2/PKG-INFO
-drwxr-xr-x   0 lb         (501) staff       (20)        0 2023-05-17 03:08:54.000000 torch4keras-0.0.7.post2/torch4keras/
--rw-r--r--   0 lb         (501) staff       (20)        0 2022-10-21 08:10:37.000000 torch4keras-0.0.7.post2/torch4keras/__init__.py
--rw-r--r--   0 lb         (501) staff       (20)    22806 2023-05-17 01:26:05.000000 torch4keras-0.0.7.post2/torch4keras/model.py
--rw-r--r--   0 lb         (501) staff       (20)    41281 2023-04-24 03:19:19.000000 torch4keras-0.0.7.post2/torch4keras/callbacks.py
--rw-r--r--   0 lb         (501) staff       (20)     7956 2023-04-24 01:52:03.000000 torch4keras-0.0.7.post2/torch4keras/snippets.py
--rw-r--r--   0 lb         (501) staff       (20)     6437 2023-05-17 02:57:10.000000 torch4keras-0.0.7.post2/README.md
--rw-r--r--   0 lb         (501) staff       (20)      491 2023-05-17 03:08:52.000000 torch4keras-0.0.7.post2/setup.py
--rw-r--r--   0 lb         (501) staff       (20)       38 2023-05-17 03:08:54.000000 torch4keras-0.0.7.post2/setup.cfg
-drwxr-xr-x   0 lb         (501) staff       (20)        0 2023-05-17 03:08:54.000000 torch4keras-0.0.7.post2/torch4keras.egg-info/
--rw-r--r--   0 lb         (501) staff       (20)     7400 2023-05-17 03:08:54.000000 torch4keras-0.0.7.post2/torch4keras.egg-info/PKG-INFO
--rw-r--r--   0 lb         (501) staff       (20)      252 2023-05-17 03:08:54.000000 torch4keras-0.0.7.post2/torch4keras.egg-info/SOURCES.txt
--rw-r--r--   0 lb         (501) staff       (20)       12 2023-05-17 03:08:54.000000 torch4keras-0.0.7.post2/torch4keras.egg-info/top_level.txt
--rw-r--r--   0 lb         (501) staff       (20)        1 2023-05-17 03:08:54.000000 torch4keras-0.0.7.post2/torch4keras.egg-info/dependency_links.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 14:52:57.063193 torch4keras-0.0.7.post3/
+-rw-rw-rw-   0        0        0    11558 2022-10-19 12:34:20.000000 torch4keras-0.0.7.post3/LICENSE
+-rw-rw-rw-   0        0        0     6839 2023-05-18 14:52:57.060190 torch4keras-0.0.7.post3/PKG-INFO
+-rw-rw-rw-   0        0        0     6579 2023-05-18 14:49:58.000000 torch4keras-0.0.7.post3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-18 14:52:57.063193 torch4keras-0.0.7.post3/setup.cfg
+-rw-rw-rw-   0        0        0      528 2023-05-18 14:50:18.000000 torch4keras-0.0.7.post3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 14:52:57.054190 torch4keras-0.0.7.post3/torch4keras/
+-rw-rw-rw-   0        0        0        0 2022-10-21 12:52:53.000000 torch4keras-0.0.7.post3/torch4keras/__init__.py
+-rw-rw-rw-   0        0        0    43413 2023-05-17 13:36:22.000000 torch4keras-0.0.7.post3/torch4keras/callbacks.py
+-rw-rw-rw-   0        0        0    23549 2023-05-17 13:39:27.000000 torch4keras-0.0.7.post3/torch4keras/model.py
+-rw-rw-rw-   0        0        0     8167 2023-04-24 15:56:30.000000 torch4keras-0.0.7.post3/torch4keras/snippets.py
+drwxrwxrwx   0        0        0        0 2023-05-18 14:52:57.060190 torch4keras-0.0.7.post3/torch4keras.egg-info/
+-rw-rw-rw-   0        0        0     6839 2023-05-18 14:52:56.000000 torch4keras-0.0.7.post3/torch4keras.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-05-18 14:52:56.000000 torch4keras-0.0.7.post3/torch4keras.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 14:52:56.000000 torch4keras-0.0.7.post3/torch4keras.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-18 14:52:56.000000 torch4keras-0.0.7.post3/torch4keras.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `torch4keras-0.0.7.post2/PKG-INFO` & `torch4keras-0.0.7.post3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,98 +1,89 @@
-Metadata-Version: 2.1
-Name: torch4keras
-Version: 0.0.7.post2
-Summary: Use torch like keras
-Home-page: https://github.com/Tongjilibo/torch4keras
-Author: Tongjilibo
-License: Apache License
-Description: # torch4keras
-        **Use torch like keras**
-        
-        [![licence](https://img.shields.io/github/license/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/blob/master/LICENSE) 
-        [![GitHub release](https://img.shields.io/github/release/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/releases) 
-        [![PyPI](https://img.shields.io/pypi/v/torch4keras?label=pypi%20package)](https://pypi.org/project/torch4keras/) 
-        [![PyPI - Downloads](https://img.shields.io/pypi/dm/torch4keras)](https://pypistats.org/packages/torch4keras)
-        [![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/torch4keras?style=social)](https://github.com/Tongjilibo/torch4keras)
-        [![GitHub Issues](https://img.shields.io/github/issues/Tongjilibo/torch4keras.svg)](https://github.com/Tongjilibo/torch4keras/issues)
-        [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Tongjilibo/torch4keras/issues)
-        
-        [Documentation](https://torch4keras.readthedocs.io) |
-        [Examples](https://github.com/Tongjilibo/torch4keras/blob/master/examples) |
-        [Source code](https://github.com/Tongjilibo/torch4keras)
-        
-        ## 1. 下载安装
-        安装稳定版
-        ```shell
-        pip install torch4keras
-        ```
-        安装最新版
-        ```shell
-        pip install git+https://github.com/Tongjilibo/torch4keras.git
-        ```
-        
-        ## 2. 功能
-        - 简述：抽象出来的Trainer，适用于一般神经网络的训练，仅需关注网络结构代码
-        - 特色：进度条展示训练过程，自定义metric，自带Evaluator, Checkpoint, Tensorboard, Logger等Callback，也可自定义Callback
-        - 初衷：前期功能是作为[bert4torch](https://github.com/Tongjilibo/bert4torch)和[rec4torch](https://github.com/Tongjilibo/rec4torch)的Trainer
-        - 训练：
-        
-            ```text
-            2022-10-28 23:16:10 - Start Training
-            2022-10-28 23:16:10 - Epoch: 1/5
-            5000/5000 [==============================] - 13s 3ms/step - loss: 0.1351 - acc: 0.9601
-            Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 798.09it/s] 
-            test_acc: 0.98045. best_test_acc: 0.98045
-        
-            2022-10-28 23:16:27 - Epoch: 2/5
-            5000/5000 [==============================] - 13s 3ms/step - loss: 0.0465 - acc: 0.9862
-            Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 635.78it/s] 
-            test_acc: 0.98280. best_test_acc: 0.98280
-        
-            2022-10-28 23:16:44 - Epoch: 3/5
-            5000/5000 [==============================] - 15s 3ms/step - loss: 0.0284 - acc: 0.9915
-            Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 673.60it/s] 
-            test_acc: 0.98365. best_test_acc: 0.98365
-        
-            2022-10-28 23:17:03 - Epoch: 4/5
-            5000/5000 [==============================] - 15s 3ms/step - loss: 0.0179 - acc: 0.9948
-            Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 692.34it/s] 
-            test_acc: 0.98265. best_test_acc: 0.98365
-        
-            2022-10-28 23:17:21 - Epoch: 5/5
-            5000/5000 [==============================] - 14s 3ms/step - loss: 0.0129 - acc: 0.9958
-            Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 701.77it/s] 
-            test_acc: 0.98585. best_test_acc: 0.98585
-        
-            2022-10-28 23:17:37 - Finish Training
-            ```
-        
-        ## 3. 快速上手
-        - 参考[bert4torch](https://github.com/Tongjilibo/bert4torch)的训练过程
-        - 简单示例: [turorials_mnist](https://github.com/Tongjilibo/torch4keras/blob/master/examples/turorials_mnist.py)
-        
-        ## 4. 版本说明
-        - **v0.0.7.post2**20230517 Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
-        - **v0.0.7**：20230505 独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
-        - **v0.0.6**：20230212 增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现(增加几个成员变量、增加initilize()、删除对forward参数个数的判断、dp和ddp不解析module、修改use_amp参数为mixed_precision)，增加了AccelerateCallback
-        - **v0.0.5**：20221217 增加Summary的Callback, 增加Tqdm的进度条展示，保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
-        - **v0.0.4**：20221127 为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
-        - **v0.0.3.post2**：20221107 修复DDP下打印的bug
-        - **v0.0.3**：20221106 参考Keras修改了callback的逻辑
-        - **v0.0.2**：20221023 增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
-        - **v0.0.1**：20221019 初始版本
-        
-        ## 5. 更新：
-        - **20230517**：Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
-        - **20230505**：独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
-        - **20230212**：增加hf的accelerator测试用例, ddp需要外部控制执行callback, 混合精度支持bf16
-        - **20230116**：增加resume_from_checkpoint和save_to_checkpoint，动态为nn.Module增加Trainer的方法add_trainer
-        - **20221217**：保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
-        - **20221203**：增加Summary的Callback, 增加Tqdm的进度条展示
-        - **20221127**：为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
-        - **20221107**：修复DDP下打印的bug，metrics中加入detach和auc
-        - **20221106**：默认的Tensorboard的global_step+1, 参考Keras修改了callback的逻辑
-        - **20221020**：增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
-        - **20221019**：初版提交
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+# torch4keras
+**Use torch like keras**
+
+[![licence](https://img.shields.io/github/license/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/blob/master/LICENSE) 
+[![GitHub release](https://img.shields.io/github/release/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/releases) 
+[![PyPI](https://img.shields.io/pypi/v/torch4keras?label=pypi%20package)](https://pypi.org/project/torch4keras/) 
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/torch4keras)](https://pypistats.org/packages/torch4keras)
+[![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/torch4keras?style=social)](https://github.com/Tongjilibo/torch4keras)
+[![GitHub Issues](https://img.shields.io/github/issues/Tongjilibo/torch4keras.svg)](https://github.com/Tongjilibo/torch4keras/issues)
+[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Tongjilibo/torch4keras/issues)
+
+[Documentation](https://torch4keras.readthedocs.io) |
+[Examples](https://github.com/Tongjilibo/torch4keras/blob/master/examples) |
+[Source code](https://github.com/Tongjilibo/torch4keras)
+
+## 1. 下载安装
+安装稳定版
+```shell
+pip install torch4keras
+```
+安装最新版
+```shell
+pip install git+https://github.com/Tongjilibo/torch4keras.git
+```
+
+## 2. 功能
+- 简述：抽象出来的Trainer，适用于一般神经网络的训练，仅需关注网络结构代码
+- 特色：进度条展示训练过程，自定义metric，自带Evaluator, Checkpoint, Tensorboard, Logger等Callback，也可自定义Callback
+- 初衷：前期功能是作为[bert4torch](https://github.com/Tongjilibo/bert4torch)和[rec4torch](https://github.com/Tongjilibo/rec4torch)的Trainer
+- 训练：
+
+    ```text
+    2022-10-28 23:16:10 - Start Training
+    2022-10-28 23:16:10 - Epoch: 1/5
+    5000/5000 [==============================] - 13s 3ms/step - loss: 0.1351 - acc: 0.9601
+    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 798.09it/s] 
+    test_acc: 0.98045. best_test_acc: 0.98045
+
+    2022-10-28 23:16:27 - Epoch: 2/5
+    5000/5000 [==============================] - 13s 3ms/step - loss: 0.0465 - acc: 0.9862
+    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 635.78it/s] 
+    test_acc: 0.98280. best_test_acc: 0.98280
+
+    2022-10-28 23:16:44 - Epoch: 3/5
+    5000/5000 [==============================] - 15s 3ms/step - loss: 0.0284 - acc: 0.9915
+    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 673.60it/s] 
+    test_acc: 0.98365. best_test_acc: 0.98365
+
+    2022-10-28 23:17:03 - Epoch: 4/5
+    5000/5000 [==============================] - 15s 3ms/step - loss: 0.0179 - acc: 0.9948
+    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 692.34it/s] 
+    test_acc: 0.98265. best_test_acc: 0.98365
+
+    2022-10-28 23:17:21 - Epoch: 5/5
+    5000/5000 [==============================] - 14s 3ms/step - loss: 0.0129 - acc: 0.9958
+    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 701.77it/s] 
+    test_acc: 0.98585. best_test_acc: 0.98585
+
+    2022-10-28 23:17:37 - Finish Training
+    ```
+
+## 3. 快速上手
+- 参考[bert4torch](https://github.com/Tongjilibo/bert4torch)的训练过程
+- 简单示例: [turorials_mnist](https://github.com/Tongjilibo/torch4keras/blob/master/examples/turorials_mnist.py)
+
+## 4. 版本说明
+- **v0.0.7.post3**: 20230517 修复保存scheduler
+- **v0.0.7.post2**: 20230517 Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
+- **v0.0.7**：20230505 独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
+- **v0.0.6**：20230212 增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现(增加几个成员变量、增加initilize()、删除对forward参数个数的判断、dp和ddp不解析module、修改use_amp参数为mixed_precision)，增加了AccelerateCallback
+- **v0.0.5**：20221217 增加Summary的Callback, 增加Tqdm的进度条展示，保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
+- **v0.0.4**：20221127 为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
+- **v0.0.3.post2**：20221107 修复DDP下打印的bug
+- **v0.0.3**：20221106 参考Keras修改了callback的逻辑
+- **v0.0.2**：20221023 增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
+- **v0.0.1**：20221019 初始版本
+
+## 5. 更新：
+- **20230517**：Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
+- **20230505**：独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
+- **20230212**：增加hf的accelerator测试用例, ddp需要外部控制执行callback, 混合精度支持bf16
+- **20230116**：增加resume_from_checkpoint和save_to_checkpoint，动态为nn.Module增加Trainer的方法add_trainer
+- **20221217**：保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
+- **20221203**：增加Summary的Callback, 增加Tqdm的进度条展示
+- **20221127**：为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
+- **20221107**：修复DDP下打印的bug，metrics中加入detach和auc
+- **20221106**：默认的Tensorboard的global_step+1, 参考Keras修改了callback的逻辑
+- **20221020**：增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
+- **20221019**：初版提交
```

### Comparing `torch4keras-0.0.7.post2/torch4keras/snippets.py` & `torch4keras-0.0.7.post3/torch4keras/snippets.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,211 +1,211 @@
-import numpy as np
-import torch
-import time
-import inspect
-from packaging import version
-from torch.utils.data import Dataset, IterableDataset
-import os
-import random
-
-try:
-    from sklearn.metrics import roc_auc_score
-except ImportError:
-    roc_auc_score = None
-        
-def take_along_dim(input_tensor, indices, dim=None):
-    '''兼容部分低版本pytorch没有torch.take_along_dim
-    '''
-    if version.parse(torch.__version__) > version.parse('1.8.1'):
-        return torch.take_along_dim(input_tensor, indices, dim)
-    else:
-        # 该逻辑仅在少量数据上测试，如有bug，欢迎反馈
-        if dim is None:
-            res = input_tensor.flatten()[indices]
-        else:
-            res = np.take_along_axis(input_tensor.cpu().numpy(), indices.cpu().numpy(), axis=dim)
-            res = torch.from_numpy(res).to(input_tensor.device)
-        # assert res.equal(torch.take_along_dim(input_tensor, indices, dim))
-        return res
-
-
-def torch_div(input, other, rounding_mode=None):
-    ''' torch.div兼容老版本
-    '''
-    if version.parse(torch.__version__) < version.parse('1.7.2'):
-        indices = input // other  # 兼容老版本
-    else:
-        indices = torch.div(input, other, rounding_mode=rounding_mode)  # 行索引
-    return indices
-
-
-def softmax(x, axis=-1):
-    """numpy版softmax
-    """
-    x = x - x.max(axis=axis, keepdims=True)
-    x = np.exp(x)
-    return x / x.sum(axis=axis, keepdims=True)
-
-
-def search_layer(model, layer_name, retrun_first=True):
-    '''根据layer_name搜索并返回参数/参数list
-    '''
-    return_list = []
-    for name, param in model.named_parameters():
-        if param.requires_grad and layer_name in name:
-            return_list.append(param)
-    if len(return_list) == 0:
-        return None
-    if retrun_first:
-        return return_list[0]
-    else:
-        return return_list
-
-
-class ListDataset(Dataset):
-    '''数据是List格式Dataset，支持传入file_path或者外部已读入的data(List格式)
-
-    :param file_path: str, 待读取的文件的路径，若无可以为None
-    :param data: List[Any], list格式的数据，和file_path至少有一个不为None
-    '''
-    def __init__(self, file_path=None, data=None, **kwargs):
-        self.kwargs = kwargs
-        if isinstance(file_path, (str, tuple, list)):
-            self.data = self.load_data(file_path)
-        elif isinstance(data, list):
-            self.data = data
-        else:
-            raise ValueError('The input args shall be str format file_path / list format dataset')
-
-    def __len__(self):
-        return len(self.data)
-
-    def __getitem__(self, index):
-        return self.data[index]
-
-    @staticmethod
-    def load_data(file_path):
-        return file_path
-
-
-class IterDataset(IterableDataset):
-    '''流式读取文件，用于大数据量、多小文件使用时候需要注意steps_per_epoch != None
-
-    :param file_path: str, 待读取的文件的路径，若无可以为None
-    '''
-    def __init__(self, file_path=None, **kwargs):
-        self.kwargs = kwargs
-        if isinstance(file_path, (str, tuple, list)):
-            self.file_path = file_path
-        else:
-            raise ValueError('The input args shall be str format file_path / list format dataset')
-    
-    def __iter__(self):
-        return self.load_data(self.file_path)
-
-    @staticmethod
-    def load_data(file_path, verbose=0):
-        if isinstance(file_path, (tuple, list)):
-            for file in file_path:
-                if verbose != 0:
-                    print("Load data: ", file)
-                with open(file, 'r') as file_obj:
-                    for line in file_obj:
-                        yield line
-        elif isinstance(file_path, str):
-            with open(file_path, 'r') as file_obj:
-                for line in file_obj:
-                    yield line
-
-
-def metric_mapping(metric, func, y_pred, y_true):
-    '''metric的计算
-
-    :param metric: str, 自带metrics的名称
-    :param func: function, 透传的用户自定的计算指标的函数
-    :param y_pred: torch.Tensor, 样本的预测结果
-    :param y_true: torch.Tensor, 样本的真实结果
-    '''
-    # 自定义metrics
-    if inspect.isfunction(func):
-        metric_res = func(y_pred, y_true)
-        if inspect.isfunction(metric):
-            # 如果直接传入回调函数（无key），要求回调函数返回Dict[String: Int/Float]类型
-            assert isinstance(metric_res, dict), 'Custom metrics callbacks should return `Dict[String: Int/Float]` value'
-        elif isinstance(metric, str):
-            # 如果直接传入回调函数（有key），要求回调函数返回Int/Float类型
-            assert isinstance(metric_res, (int, float)), 'Custom metrics callbacks should return `Int/Float value'
-        return metric_res
-    elif metric == 'loss':
-        pass
-    # 自带metrics
-    elif isinstance(metric, str):
-        # 如果forward返回了list, tuple，则选取第一项
-        y_pred_tmp = y_pred[0] if isinstance(y_pred, (list, tuple)) else y_pred
-        y_true_tmp = y_true[0] if isinstance(y_true, (list, tuple)) else y_true
-        y_pred_tmp = y_pred_tmp.detach()  # 训练过程中评估，detach不进入计算图
-
-        # 根据shape做预处理
-        if len(y_pred_tmp.shape) == len(y_true_tmp.shape) + 1:
-            y_pred_tmp = torch.argmax(y_pred_tmp, dim=-1)
-        elif len(y_pred_tmp.shape) == len(y_true_tmp.shape):
-            pass
-        else:
-            raise ValueError(f'y_pred_tmp.shape={y_pred_tmp.shape} while y_true_tmp.shape={y_true_tmp.shape}')
-
-        # 执行内置的metric
-        if metric in {'accuracy', 'acc'}:
-            return torch.sum(y_pred_tmp.eq(y_true_tmp)).item() / y_true_tmp.numel()
-        elif metric in {'auc'}:
-            if roc_auc_score is None:
-                raise ImportError('roc_auc_score requires the `sklearn` library.')
-            return roc_auc_score(y_true.cpu().numpy(), y_pred_tmp.cpu().numpy())            
-        elif metric in {'mae', 'MAE', 'mean_absolute_error'}:
-            return torch.mean(torch.abs(y_pred_tmp - y_true_tmp)).item()
-        elif metric in {'mse', 'MSE', 'mean_squared_error'}:
-            return torch.mean(torch.square(y_pred_tmp - y_true_tmp)).item()
-        elif metric in {'mape', 'MAPE', 'mean_absolute_percentage_error'}:
-            diff = torch.abs((y_true_tmp - y_pred_tmp) / torch.clamp(torch.abs(y_true_tmp), 1e-7, None))
-            return 100. * torch.mean(diff).item()
-        elif metric in {'msle', 'MSLE', 'mean_squared_logarithmic_error'}:
-            first_log = torch.log(torch.clamp(y_pred_tmp, 1e-7, None) + 1.)
-            second_log = torch.log(torch.clamp(y_true_tmp, 1e-7, None) + 1.)
-            return torch.mean(torch.square(first_log - second_log)).item()
-
-    return None
-
-
-def seed_everything(seed=None):
-    '''固定seed
-    
-    :param seed: int, 随机种子
-    '''
-    max_seed_value = np.iinfo(np.uint32).max
-    min_seed_value = np.iinfo(np.uint32).min
-
-    if (seed is None) or not (min_seed_value <= seed <= max_seed_value):
-        seed = random.randint(np.iinfo(np.uint32).min, np.iinfo(np.uint32).max)
-    print(f"Global seed set to {seed}")
-    os.environ["PYTHONHASHSEED"] = str(seed)
-    random.seed(seed)
-    np.random.seed(seed)
-    torch.manual_seed(seed)
-    torch.cuda.manual_seed(seed)
-    torch.cuda.manual_seed_all(seed)
-    torch.backends.cudnn.benchmark = False
-    torch.backends.cudnn.deterministic = True
-    return seed
-
-
-def spend_time(func):
-    '''装饰器，计算函数消耗的时间
-    '''
-    start = time.time()
-    def warpper(*args, **kwargs):
-        res = func(*args, **kwargs)
-        end = time.time()
-        consume = end - start
-        start1 = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(start))
-        end1 = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(end))
-        print(f'{start1} ~ {end1}  spent {consume:.2f}s')
-        return res
-    return warpper
+import numpy as np
+import torch
+import time
+import inspect
+from packaging import version
+from torch.utils.data import Dataset, IterableDataset
+import os
+import random
+
+try:
+    from sklearn.metrics import roc_auc_score
+except ImportError:
+    roc_auc_score = None
+        
+def take_along_dim(input_tensor, indices, dim=None):
+    '''兼容部分低版本pytorch没有torch.take_along_dim
+    '''
+    if version.parse(torch.__version__) > version.parse('1.8.1'):
+        return torch.take_along_dim(input_tensor, indices, dim)
+    else:
+        # 该逻辑仅在少量数据上测试，如有bug，欢迎反馈
+        if dim is None:
+            res = input_tensor.flatten()[indices]
+        else:
+            res = np.take_along_axis(input_tensor.cpu().numpy(), indices.cpu().numpy(), axis=dim)
+            res = torch.from_numpy(res).to(input_tensor.device)
+        # assert res.equal(torch.take_along_dim(input_tensor, indices, dim))
+        return res
+
+
+def torch_div(input, other, rounding_mode=None):
+    ''' torch.div兼容老版本
+    '''
+    if version.parse(torch.__version__) < version.parse('1.7.2'):
+        indices = input // other  # 兼容老版本
+    else:
+        indices = torch.div(input, other, rounding_mode=rounding_mode)  # 行索引
+    return indices
+
+
+def softmax(x, axis=-1):
+    """numpy版softmax
+    """
+    x = x - x.max(axis=axis, keepdims=True)
+    x = np.exp(x)
+    return x / x.sum(axis=axis, keepdims=True)
+
+
+def search_layer(model, layer_name, retrun_first=True):
+    '''根据layer_name搜索并返回参数/参数list
+    '''
+    return_list = []
+    for name, param in model.named_parameters():
+        if param.requires_grad and layer_name in name:
+            return_list.append(param)
+    if len(return_list) == 0:
+        return None
+    if retrun_first:
+        return return_list[0]
+    else:
+        return return_list
+
+
+class ListDataset(Dataset):
+    '''数据是List格式Dataset，支持传入file_path或者外部已读入的data(List格式)
+
+    :param file_path: str, 待读取的文件的路径，若无可以为None
+    :param data: List[Any], list格式的数据，和file_path至少有一个不为None
+    '''
+    def __init__(self, file_path=None, data=None, **kwargs):
+        self.kwargs = kwargs
+        if isinstance(file_path, (str, tuple, list)):
+            self.data = self.load_data(file_path)
+        elif isinstance(data, list):
+            self.data = data
+        else:
+            raise ValueError('The input args shall be str format file_path / list format dataset')
+
+    def __len__(self):
+        return len(self.data)
+
+    def __getitem__(self, index):
+        return self.data[index]
+
+    @staticmethod
+    def load_data(file_path):
+        return file_path
+
+
+class IterDataset(IterableDataset):
+    '''流式读取文件，用于大数据量、多小文件使用时候需要注意steps_per_epoch != None
+
+    :param file_path: str, 待读取的文件的路径，若无可以为None
+    '''
+    def __init__(self, file_path=None, **kwargs):
+        self.kwargs = kwargs
+        if isinstance(file_path, (str, tuple, list)):
+            self.file_path = file_path
+        else:
+            raise ValueError('The input args shall be str format file_path / list format dataset')
+    
+    def __iter__(self):
+        return self.load_data(self.file_path)
+
+    @staticmethod
+    def load_data(file_path, verbose=0):
+        if isinstance(file_path, (tuple, list)):
+            for file in file_path:
+                if verbose != 0:
+                    print("Load data: ", file)
+                with open(file, 'r') as file_obj:
+                    for line in file_obj:
+                        yield line
+        elif isinstance(file_path, str):
+            with open(file_path, 'r') as file_obj:
+                for line in file_obj:
+                    yield line
+
+
+def metric_mapping(metric, func, y_pred, y_true):
+    '''metric的计算
+
+    :param metric: str, 自带metrics的名称
+    :param func: function, 透传的用户自定的计算指标的函数
+    :param y_pred: torch.Tensor, 样本的预测结果
+    :param y_true: torch.Tensor, 样本的真实结果
+    '''
+    # 自定义metrics
+    if inspect.isfunction(func):
+        metric_res = func(y_pred, y_true)
+        if inspect.isfunction(metric):
+            # 如果直接传入回调函数（无key），要求回调函数返回Dict[String: Int/Float]类型
+            assert isinstance(metric_res, dict), 'Custom metrics callbacks should return `Dict[String: Int/Float]` value'
+        elif isinstance(metric, str):
+            # 如果直接传入回调函数（有key），要求回调函数返回Int/Float类型
+            assert isinstance(metric_res, (int, float)), 'Custom metrics callbacks should return `Int/Float value'
+        return metric_res
+    elif metric == 'loss':
+        pass
+    # 自带metrics
+    elif isinstance(metric, str):
+        # 如果forward返回了list, tuple，则选取第一项
+        y_pred_tmp = y_pred[0] if isinstance(y_pred, (list, tuple)) else y_pred
+        y_true_tmp = y_true[0] if isinstance(y_true, (list, tuple)) else y_true
+        y_pred_tmp = y_pred_tmp.detach()  # 训练过程中评估，detach不进入计算图
+
+        # 根据shape做预处理
+        if len(y_pred_tmp.shape) == len(y_true_tmp.shape) + 1:
+            y_pred_tmp = torch.argmax(y_pred_tmp, dim=-1)
+        elif len(y_pred_tmp.shape) == len(y_true_tmp.shape):
+            pass
+        else:
+            raise ValueError(f'y_pred_tmp.shape={y_pred_tmp.shape} while y_true_tmp.shape={y_true_tmp.shape}')
+
+        # 执行内置的metric
+        if metric in {'accuracy', 'acc'}:
+            return torch.sum(y_pred_tmp.eq(y_true_tmp)).item() / y_true_tmp.numel()
+        elif metric in {'auc'}:
+            if roc_auc_score is None:
+                raise ImportError('roc_auc_score requires the `sklearn` library.')
+            return roc_auc_score(y_true.cpu().numpy(), y_pred_tmp.cpu().numpy())            
+        elif metric in {'mae', 'MAE', 'mean_absolute_error'}:
+            return torch.mean(torch.abs(y_pred_tmp - y_true_tmp)).item()
+        elif metric in {'mse', 'MSE', 'mean_squared_error'}:
+            return torch.mean(torch.square(y_pred_tmp - y_true_tmp)).item()
+        elif metric in {'mape', 'MAPE', 'mean_absolute_percentage_error'}:
+            diff = torch.abs((y_true_tmp - y_pred_tmp) / torch.clamp(torch.abs(y_true_tmp), 1e-7, None))
+            return 100. * torch.mean(diff).item()
+        elif metric in {'msle', 'MSLE', 'mean_squared_logarithmic_error'}:
+            first_log = torch.log(torch.clamp(y_pred_tmp, 1e-7, None) + 1.)
+            second_log = torch.log(torch.clamp(y_true_tmp, 1e-7, None) + 1.)
+            return torch.mean(torch.square(first_log - second_log)).item()
+
+    return None
+
+
+def seed_everything(seed=None):
+    '''固定seed
+    
+    :param seed: int, 随机种子
+    '''
+    max_seed_value = np.iinfo(np.uint32).max
+    min_seed_value = np.iinfo(np.uint32).min
+
+    if (seed is None) or not (min_seed_value <= seed <= max_seed_value):
+        seed = random.randint(np.iinfo(np.uint32).min, np.iinfo(np.uint32).max)
+    print(f"Global seed set to {seed}")
+    os.environ["PYTHONHASHSEED"] = str(seed)
+    random.seed(seed)
+    np.random.seed(seed)
+    torch.manual_seed(seed)
+    torch.cuda.manual_seed(seed)
+    torch.cuda.manual_seed_all(seed)
+    torch.backends.cudnn.benchmark = False
+    torch.backends.cudnn.deterministic = True
+    return seed
+
+
+def spend_time(func):
+    '''装饰器，计算函数消耗的时间
+    '''
+    start = time.time()
+    def warpper(*args, **kwargs):
+        res = func(*args, **kwargs)
+        end = time.time()
+        consume = end - start
+        start1 = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(start))
+        end1 = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(end))
+        print(f'{start1} ~ {end1}  spent {consume:.2f}s')
+        return res
+    return warpper
```

### Comparing `torch4keras-0.0.7.post2/README.md` & `torch4keras-0.0.7.post3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,88 +1,99 @@
-# torch4keras
-**Use torch like keras**
-
-[![licence](https://img.shields.io/github/license/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/blob/master/LICENSE) 
-[![GitHub release](https://img.shields.io/github/release/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/releases) 
-[![PyPI](https://img.shields.io/pypi/v/torch4keras?label=pypi%20package)](https://pypi.org/project/torch4keras/) 
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/torch4keras)](https://pypistats.org/packages/torch4keras)
-[![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/torch4keras?style=social)](https://github.com/Tongjilibo/torch4keras)
-[![GitHub Issues](https://img.shields.io/github/issues/Tongjilibo/torch4keras.svg)](https://github.com/Tongjilibo/torch4keras/issues)
-[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Tongjilibo/torch4keras/issues)
-
-[Documentation](https://torch4keras.readthedocs.io) |
-[Examples](https://github.com/Tongjilibo/torch4keras/blob/master/examples) |
-[Source code](https://github.com/Tongjilibo/torch4keras)
-
-## 1. 下载安装
-安装稳定版
-```shell
-pip install torch4keras
-```
-安装最新版
-```shell
-pip install git+https://github.com/Tongjilibo/torch4keras.git
-```
-
-## 2. 功能
-- 简述：抽象出来的Trainer，适用于一般神经网络的训练，仅需关注网络结构代码
-- 特色：进度条展示训练过程，自定义metric，自带Evaluator, Checkpoint, Tensorboard, Logger等Callback，也可自定义Callback
-- 初衷：前期功能是作为[bert4torch](https://github.com/Tongjilibo/bert4torch)和[rec4torch](https://github.com/Tongjilibo/rec4torch)的Trainer
-- 训练：
-
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
-
-    2022-10-28 23:17:37 - Finish Training
-    ```
-
-## 3. 快速上手
-- 参考[bert4torch](https://github.com/Tongjilibo/bert4torch)的训练过程
-- 简单示例: [turorials_mnist](https://github.com/Tongjilibo/torch4keras/blob/master/examples/turorials_mnist.py)
-
-## 4. 版本说明
-- **v0.0.7.post2**20230517 Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
-- **v0.0.7**：20230505 独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
-- **v0.0.6**：20230212 增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现(增加几个成员变量、增加initilize()、删除对forward参数个数的判断、dp和ddp不解析module、修改use_amp参数为mixed_precision)，增加了AccelerateCallback
-- **v0.0.5**：20221217 增加Summary的Callback, 增加Tqdm的进度条展示，保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
-- **v0.0.4**：20221127 为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
-- **v0.0.3.post2**：20221107 修复DDP下打印的bug
-- **v0.0.3**：20221106 参考Keras修改了callback的逻辑
-- **v0.0.2**：20221023 增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
-- **v0.0.1**：20221019 初始版本
-
-## 5. 更新：
-- **20230517**：Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
-- **20230505**：独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
-- **20230212**：增加hf的accelerator测试用例, ddp需要外部控制执行callback, 混合精度支持bf16
-- **20230116**：增加resume_from_checkpoint和save_to_checkpoint，动态为nn.Module增加Trainer的方法add_trainer
-- **20221217**：保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
-- **20221203**：增加Summary的Callback, 增加Tqdm的进度条展示
-- **20221127**：为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
-- **20221107**：修复DDP下打印的bug，metrics中加入detach和auc
-- **20221106**：默认的Tensorboard的global_step+1, 参考Keras修改了callback的逻辑
-- **20221020**：增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
-- **20221019**：初版提交
+Metadata-Version: 2.1
+Name: torch4keras
+Version: 0.0.7.post3
+Summary: Use torch like keras
+Home-page: https://github.com/Tongjilibo/torch4keras
+Author: Tongjilibo
+License: Apache License
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# torch4keras
+**Use torch like keras**
+
+[![licence](https://img.shields.io/github/license/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/blob/master/LICENSE) 
+[![GitHub release](https://img.shields.io/github/release/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/releases) 
+[![PyPI](https://img.shields.io/pypi/v/torch4keras?label=pypi%20package)](https://pypi.org/project/torch4keras/) 
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/torch4keras)](https://pypistats.org/packages/torch4keras)
+[![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/torch4keras?style=social)](https://github.com/Tongjilibo/torch4keras)
+[![GitHub Issues](https://img.shields.io/github/issues/Tongjilibo/torch4keras.svg)](https://github.com/Tongjilibo/torch4keras/issues)
+[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Tongjilibo/torch4keras/issues)
+
+[Documentation](https://torch4keras.readthedocs.io) |
+[Examples](https://github.com/Tongjilibo/torch4keras/blob/master/examples) |
+[Source code](https://github.com/Tongjilibo/torch4keras)
+
+## 1. 下载安装
+安装稳定版
+```shell
+pip install torch4keras
+```
+安装最新版
+```shell
+pip install git+https://github.com/Tongjilibo/torch4keras.git
+```
+
+## 2. 功能
+- 简述：抽象出来的Trainer，适用于一般神经网络的训练，仅需关注网络结构代码
+- 特色：进度条展示训练过程，自定义metric，自带Evaluator, Checkpoint, Tensorboard, Logger等Callback，也可自定义Callback
+- 初衷：前期功能是作为[bert4torch](https://github.com/Tongjilibo/bert4torch)和[rec4torch](https://github.com/Tongjilibo/rec4torch)的Trainer
+- 训练：
+
+    ```text
+    2022-10-28 23:16:10 - Start Training
+    2022-10-28 23:16:10 - Epoch: 1/5
+    5000/5000 [==============================] - 13s 3ms/step - loss: 0.1351 - acc: 0.9601
+    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 798.09it/s] 
+    test_acc: 0.98045. best_test_acc: 0.98045
+
+    2022-10-28 23:16:27 - Epoch: 2/5
+    5000/5000 [==============================] - 13s 3ms/step - loss: 0.0465 - acc: 0.9862
+    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 635.78it/s] 
+    test_acc: 0.98280. best_test_acc: 0.98280
+
+    2022-10-28 23:16:44 - Epoch: 3/5
+    5000/5000 [==============================] - 15s 3ms/step - loss: 0.0284 - acc: 0.9915
+    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 673.60it/s] 
+    test_acc: 0.98365. best_test_acc: 0.98365
+
+    2022-10-28 23:17:03 - Epoch: 4/5
+    5000/5000 [==============================] - 15s 3ms/step - loss: 0.0179 - acc: 0.9948
+    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 692.34it/s] 
+    test_acc: 0.98265. best_test_acc: 0.98365
+
+    2022-10-28 23:17:21 - Epoch: 5/5
+    5000/5000 [==============================] - 14s 3ms/step - loss: 0.0129 - acc: 0.9958
+    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 701.77it/s] 
+    test_acc: 0.98585. best_test_acc: 0.98585
+
+    2022-10-28 23:17:37 - Finish Training
+    ```
+
+## 3. 快速上手
+- 参考[bert4torch](https://github.com/Tongjilibo/bert4torch)的训练过程
+- 简单示例: [turorials_mnist](https://github.com/Tongjilibo/torch4keras/blob/master/examples/turorials_mnist.py)
+
+## 4. 版本说明
+- **v0.0.7.post3**: 20230517 修复保存scheduler
+- **v0.0.7.post2**: 20230517 Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
+- **v0.0.7**：20230505 独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
+- **v0.0.6**：20230212 增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现(增加几个成员变量、增加initilize()、删除对forward参数个数的判断、dp和ddp不解析module、修改use_amp参数为mixed_precision)，增加了AccelerateCallback
+- **v0.0.5**：20221217 增加Summary的Callback, 增加Tqdm的进度条展示，保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
+- **v0.0.4**：20221127 为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
+- **v0.0.3.post2**：20221107 修复DDP下打印的bug
+- **v0.0.3**：20221106 参考Keras修改了callback的逻辑
+- **v0.0.2**：20221023 增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
+- **v0.0.1**：20221019 初始版本
+
+## 5. 更新：
+- **20230517**：Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
+- **20230505**：独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
+- **20230212**：增加hf的accelerator测试用例, ddp需要外部控制执行callback, 混合精度支持bf16
+- **20230116**：增加resume_from_checkpoint和save_to_checkpoint，动态为nn.Module增加Trainer的方法add_trainer
+- **20221217**：保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
+- **20221203**：增加Summary的Callback, 增加Tqdm的进度条展示
+- **20221127**：为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
+- **20221107**：修复DDP下打印的bug，metrics中加入detach和auc
+- **20221106**：默认的Tensorboard的global_step+1, 参考Keras修改了callback的逻辑
+- **20221020**：增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
+- **20221019**：初版提交
```

### Comparing `torch4keras-0.0.7.post2/torch4keras.egg-info/PKG-INFO` & `torch4keras-0.0.7.post3/torch4keras.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,98 +1,99 @@
-Metadata-Version: 2.1
-Name: torch4keras
-Version: 0.0.7.post2
-Summary: Use torch like keras
-Home-page: https://github.com/Tongjilibo/torch4keras
-Author: Tongjilibo
-License: Apache License
-Description: # torch4keras
-        **Use torch like keras**
-        
-        [![licence](https://img.shields.io/github/license/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/blob/master/LICENSE) 
-        [![GitHub release](https://img.shields.io/github/release/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/releases) 
-        [![PyPI](https://img.shields.io/pypi/v/torch4keras?label=pypi%20package)](https://pypi.org/project/torch4keras/) 
-        [![PyPI - Downloads](https://img.shields.io/pypi/dm/torch4keras)](https://pypistats.org/packages/torch4keras)
-        [![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/torch4keras?style=social)](https://github.com/Tongjilibo/torch4keras)
-        [![GitHub Issues](https://img.shields.io/github/issues/Tongjilibo/torch4keras.svg)](https://github.com/Tongjilibo/torch4keras/issues)
-        [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Tongjilibo/torch4keras/issues)
-        
-        [Documentation](https://torch4keras.readthedocs.io) |
-        [Examples](https://github.com/Tongjilibo/torch4keras/blob/master/examples) |
-        [Source code](https://github.com/Tongjilibo/torch4keras)
-        
-        ## 1. 下载安装
-        安装稳定版
-        ```shell
-        pip install torch4keras
-        ```
-        安装最新版
-        ```shell
-        pip install git+https://github.com/Tongjilibo/torch4keras.git
-        ```
-        
-        ## 2. 功能
-        - 简述：抽象出来的Trainer，适用于一般神经网络的训练，仅需关注网络结构代码
-        - 特色：进度条展示训练过程，自定义metric，自带Evaluator, Checkpoint, Tensorboard, Logger等Callback，也可自定义Callback
-        - 初衷：前期功能是作为[bert4torch](https://github.com/Tongjilibo/bert4torch)和[rec4torch](https://github.com/Tongjilibo/rec4torch)的Trainer
-        - 训练：
-        
-            ```text
-            2022-10-28 23:16:10 - Start Training
-            2022-10-28 23:16:10 - Epoch: 1/5
-            5000/5000 [==============================] - 13s 3ms/step - loss: 0.1351 - acc: 0.9601
-            Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 798.09it/s] 
-            test_acc: 0.98045. best_test_acc: 0.98045
-        
-            2022-10-28 23:16:27 - Epoch: 2/5
-            5000/5000 [==============================] - 13s 3ms/step - loss: 0.0465 - acc: 0.9862
-            Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 635.78it/s] 
-            test_acc: 0.98280. best_test_acc: 0.98280
-        
-            2022-10-28 23:16:44 - Epoch: 3/5
-            5000/5000 [==============================] - 15s 3ms/step - loss: 0.0284 - acc: 0.9915
-            Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 673.60it/s] 
-            test_acc: 0.98365. best_test_acc: 0.98365
-        
-            2022-10-28 23:17:03 - Epoch: 4/5
-            5000/5000 [==============================] - 15s 3ms/step - loss: 0.0179 - acc: 0.9948
-            Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 692.34it/s] 
-            test_acc: 0.98265. best_test_acc: 0.98365
-        
-            2022-10-28 23:17:21 - Epoch: 5/5
-            5000/5000 [==============================] - 14s 3ms/step - loss: 0.0129 - acc: 0.9958
-            Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 701.77it/s] 
-            test_acc: 0.98585. best_test_acc: 0.98585
-        
-            2022-10-28 23:17:37 - Finish Training
-            ```
-        
-        ## 3. 快速上手
-        - 参考[bert4torch](https://github.com/Tongjilibo/bert4torch)的训练过程
-        - 简单示例: [turorials_mnist](https://github.com/Tongjilibo/torch4keras/blob/master/examples/turorials_mnist.py)
-        
-        ## 4. 版本说明
-        - **v0.0.7.post2**20230517 Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
-        - **v0.0.7**：20230505 独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
-        - **v0.0.6**：20230212 增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现(增加几个成员变量、增加initilize()、删除对forward参数个数的判断、dp和ddp不解析module、修改use_amp参数为mixed_precision)，增加了AccelerateCallback
-        - **v0.0.5**：20221217 增加Summary的Callback, 增加Tqdm的进度条展示，保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
-        - **v0.0.4**：20221127 为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
-        - **v0.0.3.post2**：20221107 修复DDP下打印的bug
-        - **v0.0.3**：20221106 参考Keras修改了callback的逻辑
-        - **v0.0.2**：20221023 增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
-        - **v0.0.1**：20221019 初始版本
-        
-        ## 5. 更新：
-        - **20230517**：Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
-        - **20230505**：独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
-        - **20230212**：增加hf的accelerator测试用例, ddp需要外部控制执行callback, 混合精度支持bf16
-        - **20230116**：增加resume_from_checkpoint和save_to_checkpoint，动态为nn.Module增加Trainer的方法add_trainer
-        - **20221217**：保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
-        - **20221203**：增加Summary的Callback, 增加Tqdm的进度条展示
-        - **20221127**：为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
-        - **20221107**：修复DDP下打印的bug，metrics中加入detach和auc
-        - **20221106**：默认的Tensorboard的global_step+1, 参考Keras修改了callback的逻辑
-        - **20221020**：增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
-        - **20221019**：初版提交
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: torch4keras
+Version: 0.0.7.post3
+Summary: Use torch like keras
+Home-page: https://github.com/Tongjilibo/torch4keras
+Author: Tongjilibo
+License: Apache License
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# torch4keras
+**Use torch like keras**
+
+[![licence](https://img.shields.io/github/license/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/blob/master/LICENSE) 
+[![GitHub release](https://img.shields.io/github/release/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/releases) 
+[![PyPI](https://img.shields.io/pypi/v/torch4keras?label=pypi%20package)](https://pypi.org/project/torch4keras/) 
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/torch4keras)](https://pypistats.org/packages/torch4keras)
+[![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/torch4keras?style=social)](https://github.com/Tongjilibo/torch4keras)
+[![GitHub Issues](https://img.shields.io/github/issues/Tongjilibo/torch4keras.svg)](https://github.com/Tongjilibo/torch4keras/issues)
+[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Tongjilibo/torch4keras/issues)
+
+[Documentation](https://torch4keras.readthedocs.io) |
+[Examples](https://github.com/Tongjilibo/torch4keras/blob/master/examples) |
+[Source code](https://github.com/Tongjilibo/torch4keras)
+
+## 1. 下载安装
+安装稳定版
+```shell
+pip install torch4keras
+```
+安装最新版
+```shell
+pip install git+https://github.com/Tongjilibo/torch4keras.git
+```
+
+## 2. 功能
+- 简述：抽象出来的Trainer，适用于一般神经网络的训练，仅需关注网络结构代码
+- 特色：进度条展示训练过程，自定义metric，自带Evaluator, Checkpoint, Tensorboard, Logger等Callback，也可自定义Callback
+- 初衷：前期功能是作为[bert4torch](https://github.com/Tongjilibo/bert4torch)和[rec4torch](https://github.com/Tongjilibo/rec4torch)的Trainer
+- 训练：
+
+    ```text
+    2022-10-28 23:16:10 - Start Training
+    2022-10-28 23:16:10 - Epoch: 1/5
+    5000/5000 [==============================] - 13s 3ms/step - loss: 0.1351 - acc: 0.9601
+    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 798.09it/s] 
+    test_acc: 0.98045. best_test_acc: 0.98045
+
+    2022-10-28 23:16:27 - Epoch: 2/5
+    5000/5000 [==============================] - 13s 3ms/step - loss: 0.0465 - acc: 0.9862
+    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 635.78it/s] 
+    test_acc: 0.98280. best_test_acc: 0.98280
+
+    2022-10-28 23:16:44 - Epoch: 3/5
+    5000/5000 [==============================] - 15s 3ms/step - loss: 0.0284 - acc: 0.9915
+    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 673.60it/s] 
+    test_acc: 0.98365. best_test_acc: 0.98365
+
+    2022-10-28 23:17:03 - Epoch: 4/5
+    5000/5000 [==============================] - 15s 3ms/step - loss: 0.0179 - acc: 0.9948
+    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 692.34it/s] 
+    test_acc: 0.98265. best_test_acc: 0.98365
+
+    2022-10-28 23:17:21 - Epoch: 5/5
+    5000/5000 [==============================] - 14s 3ms/step - loss: 0.0129 - acc: 0.9958
+    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 701.77it/s] 
+    test_acc: 0.98585. best_test_acc: 0.98585
+
+    2022-10-28 23:17:37 - Finish Training
+    ```
+
+## 3. 快速上手
+- 参考[bert4torch](https://github.com/Tongjilibo/bert4torch)的训练过程
+- 简单示例: [turorials_mnist](https://github.com/Tongjilibo/torch4keras/blob/master/examples/turorials_mnist.py)
+
+## 4. 版本说明
+- **v0.0.7.post3**: 20230517 修复保存scheduler
+- **v0.0.7.post2**: 20230517 Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
+- **v0.0.7**：20230505 独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
+- **v0.0.6**：20230212 增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现(增加几个成员变量、增加initilize()、删除对forward参数个数的判断、dp和ddp不解析module、修改use_amp参数为mixed_precision)，增加了AccelerateCallback
+- **v0.0.5**：20221217 增加Summary的Callback, 增加Tqdm的进度条展示，保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
+- **v0.0.4**：20221127 为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
+- **v0.0.3.post2**：20221107 修复DDP下打印的bug
+- **v0.0.3**：20221106 参考Keras修改了callback的逻辑
+- **v0.0.2**：20221023 增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
+- **v0.0.1**：20221019 初始版本
+
+## 5. 更新：
+- **20230517**：Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
+- **20230505**：独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
+- **20230212**：增加hf的accelerator测试用例, ddp需要外部控制执行callback, 混合精度支持bf16
+- **20230116**：增加resume_from_checkpoint和save_to_checkpoint，动态为nn.Module增加Trainer的方法add_trainer
+- **20221217**：保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
+- **20221203**：增加Summary的Callback, 增加Tqdm的进度条展示
+- **20221127**：为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
+- **20221107**：修复DDP下打印的bug，metrics中加入detach和auc
+- **20221106**：默认的Tensorboard的global_step+1, 参考Keras修改了callback的逻辑
+- **20221020**：增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
+- **20221019**：初版提交
```

