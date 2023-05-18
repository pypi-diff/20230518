# Comparing `tmp/pdtr-0.1.1.tar.gz` & `tmp/pdtr-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdtr-0.1.1.tar", last modified: Wed May 17 16:05:19 2023, max compression
+gzip compressed data, was "pdtr-0.1.2.tar", last modified: Thu May 18 16:22:12 2023, max compression
```

## Comparing `pdtr-0.1.1.tar` & `pdtr-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-05-17 16:05:19.927967 pdtr-0.1.1/
--rw-r--r--   0 lubberit   (501) staff       (20)     1065 2023-05-12 08:26:44.000000 pdtr-0.1.1/LICENSE
--rw-r--r--   0 lubberit   (501) staff       (20)     8477 2023-05-17 16:05:19.927685 pdtr-0.1.1/PKG-INFO
--rw-r--r--   0 lubberit   (501) staff       (20)     7751 2023-05-17 14:15:07.000000 pdtr-0.1.1/README.md
-drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-05-17 16:05:19.925673 pdtr-0.1.1/pdtr/
--rw-r--r--   0 lubberit   (501) staff       (20)      265 2023-05-17 16:05:07.000000 pdtr-0.1.1/pdtr/__init__.py
--rw-r--r--   0 lubberit   (501) staff       (20)    21376 2023-05-17 15:26:47.000000 pdtr-0.1.1/pdtr/excel_writer.py
--rw-r--r--   0 lubberit   (501) staff       (20)    25148 2023-05-17 15:58:18.000000 pdtr-0.1.1/pdtr/transforme.py
-drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-05-17 16:05:19.927294 pdtr-0.1.1/pdtr.egg-info/
--rw-r--r--   0 lubberit   (501) staff       (20)     8477 2023-05-17 16:05:19.000000 pdtr-0.1.1/pdtr.egg-info/PKG-INFO
--rw-r--r--   0 lubberit   (501) staff       (20)      222 2023-05-17 16:05:19.000000 pdtr-0.1.1/pdtr.egg-info/SOURCES.txt
--rw-r--r--   0 lubberit   (501) staff       (20)        1 2023-05-17 16:05:19.000000 pdtr-0.1.1/pdtr.egg-info/dependency_links.txt
--rw-r--r--   0 lubberit   (501) staff       (20)      199 2023-05-17 16:05:19.000000 pdtr-0.1.1/pdtr.egg-info/requires.txt
--rw-r--r--   0 lubberit   (501) staff       (20)        5 2023-05-17 16:05:19.000000 pdtr-0.1.1/pdtr.egg-info/top_level.txt
--rw-r--r--   0 lubberit   (501) staff       (20)       38 2023-05-17 16:05:19.928071 pdtr-0.1.1/setup.cfg
--rw-r--r--   0 lubberit   (501) staff       (20)     1632 2023-05-17 16:04:40.000000 pdtr-0.1.1/setup.py
+drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-05-18 16:22:12.868715 pdtr-0.1.2/
+-rw-r--r--   0 lubberit   (501) staff       (20)     1065 2023-05-12 08:26:44.000000 pdtr-0.1.2/LICENSE
+-rw-r--r--   0 lubberit   (501) staff       (20)    10914 2023-05-18 16:22:12.868394 pdtr-0.1.2/PKG-INFO
+-rw-r--r--   0 lubberit   (501) staff       (20)    10188 2023-05-18 16:21:18.000000 pdtr-0.1.2/README.md
+drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-05-18 16:22:12.866539 pdtr-0.1.2/pdtr/
+-rw-r--r--   0 lubberit   (501) staff       (20)      265 2023-05-18 16:21:51.000000 pdtr-0.1.2/pdtr/__init__.py
+-rw-r--r--   0 lubberit   (501) staff       (20)    21376 2023-05-17 15:26:47.000000 pdtr-0.1.2/pdtr/excel_writer.py
+-rw-r--r--   0 lubberit   (501) staff       (20)    30113 2023-05-18 16:05:17.000000 pdtr-0.1.2/pdtr/transforme.py
+drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-05-18 16:22:12.868034 pdtr-0.1.2/pdtr.egg-info/
+-rw-r--r--   0 lubberit   (501) staff       (20)    10914 2023-05-18 16:22:12.000000 pdtr-0.1.2/pdtr.egg-info/PKG-INFO
+-rw-r--r--   0 lubberit   (501) staff       (20)      222 2023-05-18 16:22:12.000000 pdtr-0.1.2/pdtr.egg-info/SOURCES.txt
+-rw-r--r--   0 lubberit   (501) staff       (20)        1 2023-05-18 16:22:12.000000 pdtr-0.1.2/pdtr.egg-info/dependency_links.txt
+-rw-r--r--   0 lubberit   (501) staff       (20)      204 2023-05-18 16:22:12.000000 pdtr-0.1.2/pdtr.egg-info/requires.txt
+-rw-r--r--   0 lubberit   (501) staff       (20)        5 2023-05-18 16:22:12.000000 pdtr-0.1.2/pdtr.egg-info/top_level.txt
+-rw-r--r--   0 lubberit   (501) staff       (20)       38 2023-05-18 16:22:12.868799 pdtr-0.1.2/setup.cfg
+-rw-r--r--   0 lubberit   (501) staff       (20)     1632 2023-05-17 16:04:40.000000 pdtr-0.1.2/setup.py
```

### Comparing `pdtr-0.1.1/LICENSE` & `pdtr-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pdtr-0.1.1/PKG-INFO` & `pdtr-0.1.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,51 @@
-Metadata-Version: 2.1
-Name: pdtr
-Version: 0.1.1
-Summary: 自动决策树规则挖掘工具包
-Home-page: https://github.com/itlubber/pdtr
-Author: itlubber
-Author-email: itlubber@qq.com
-License: MIT
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # 自动决策树规则挖掘工具包
 
+在笔者金融风控的日常工作中，很多时候需要根据数据集内的诸多特征（有很多其他称呼，比如因子、变量、自变量、解释变量等）来挖掘一些有用的规则和组合策略，在保证通过率的基础上尽可能多的拒绝坏客户。面对成千上万的特征，如何从数据集中找到有效的规则和组合策略，一直以来都是金融风控搬砖工的日常工作。 `pdtr` 旨在帮助读者快速从高维数据中提取出有效的规则和组合策略。
+
+> 仓库地址：https://github.com/itlubber/pdtr
+> 
+> 博文地址：https://itlubber.art/archives/auto-strategy-mining
+> 
+> 微信公共号推文：https://mp.weixin.qq.com/s/8s785MfmVznNgQyy38YnWw
+> 
+> pipy包：https://pypi.org/project/pdtr/
+
 ## 背景简介
 
 金融场景风险大致可以概括为三种：系统性风险、欺诈风险（无还款意愿）、信用风险（无还款能力），而作为一名风控搬砖工，日常工作中有大量的数据挖掘工作，如何从高维数据集中挖掘出行之有效的规则、策略及模型来防范欺诈风险和信用风险每个搬砖工的基操。本仓库由笔者基于网上开源的一系列相关知识，结合实际工作中遇到的实际需求，整理得到。旨在为诸位仁兄提供一个便捷、高效、赏心悦目的决策树组合策略挖掘报告，及一系列能够实际运用到风险控制上的策略。
 
+## 项目结构
+
+```bash
+pdtr
+.
+|   README.md                           # 说明文档
+|   setup.py                            # 打包发布文件
+|   LICENSE                             # 开源协议
+|   requirements.txt                    # 项目依赖包
++---examples                            # 演示样例
+|   |   combine_rules_cache             # 缓存文件
+|   |   combine_rules_cache.svg         # 缓存文件
+|   |   pdtr_samplts.ipynb              # 演示样例程序
+|   \---model_report                    # 模型报告输出文件夹
+|       |   决策树组合策略挖掘.xlsx        # 策略挖掘报告
+|       +---auto_mining_rules           # 组合策略可视化存储文件夹
+|       |       combiner_rules_0.png    # 决策树可视化图片
+|       |       ......
+|       \---bin_plots                   # 简单策略可视化存储文件夹
+|               bin_vars_A.png          # 变量分箱可视化图片
+|               ......
+\---pdtr                                # PDTR 源码包
+        template.xlsx                   # excel 模版文件
+        excel_writer.py                 # excel写入公共方法
+        matplot_chinese.ttf             # matplotlib 中文字体
+        transforme.py                   # 策略挖掘方法
+```
+
 ## 环境准备
 
 ### 创建虚拟环境（可选）
 
 + 通过`conda`创建虚拟环境
 
 ```bash
@@ -144,14 +161,24 @@
 
 ### `PDTR` 安装
 
 ```bash
 pip install pdtr
 ```
 
+### 版本介绍
+
++ `0.1.0`
+
+仅包含决策树策略挖掘相关工具
+
++ `0.1.1`
+
+除版本 `0.1.0` 中的决策树挖掘相关工具以外，新增了基于 `toad` 和 `optbinning` 的单变量策略挖掘相关方法
+
 
 ### 运行样例
 
 + 导入相关依赖
 
 ```python
 import os
@@ -209,15 +236,15 @@
 
 ```python
 pdtr_instance.save()
 ```
 
 + 挖掘报告
 
-`examples/决策树组合策略挖掘.xlsx`
+[`examples/决策树组合策略挖掘.xlsx`](https://github.com/itlubber/pdtr/blob/main/examples/model_report/%E5%86%B3%E7%AD%96%E6%A0%91%E7%BB%84%E5%90%88%E7%AD%96%E7%95%A5%E6%8C%96%E6%8E%98.xlsx)
 
 
 ## 参考
 
 > https://github.com/itlubber/LogisticRegressionPipeline
 > 
 > https://github.com/itlubber/itlubber-excel-writer
```

### Comparing `pdtr-0.1.1/pdtr/excel_writer.py` & `pdtr-0.1.2/pdtr/excel_writer.py`

 * *Files identical despite different names*

### Comparing `pdtr-0.1.1/pdtr.egg-info/PKG-INFO` & `pdtr-0.1.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdtr
-Version: 0.1.1
+Version: 0.1.2
 Summary: 自动决策树规则挖掘工具包
 Home-page: https://github.com/itlubber/pdtr
 Author: itlubber
 Author-email: itlubber@qq.com
 License: MIT
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
@@ -17,18 +17,56 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 自动决策树规则挖掘工具包
 
+在笔者金融风控的日常工作中，很多时候需要根据数据集内的诸多特征（有很多其他称呼，比如因子、变量、自变量、解释变量等）来挖掘一些有用的规则和组合策略，在保证通过率的基础上尽可能多的拒绝坏客户。面对成千上万的特征，如何从数据集中找到有效的规则和组合策略，一直以来都是金融风控搬砖工的日常工作。 `pdtr` 旨在帮助读者快速从高维数据中提取出有效的规则和组合策略。
+
+> 仓库地址：https://github.com/itlubber/pdtr
+> 
+> 博文地址：https://itlubber.art/archives/auto-strategy-mining
+> 
+> 微信公共号推文：https://mp.weixin.qq.com/s/8s785MfmVznNgQyy38YnWw
+> 
+> pipy包：https://pypi.org/project/pdtr/
+
 ## 背景简介
 
 金融场景风险大致可以概括为三种：系统性风险、欺诈风险（无还款意愿）、信用风险（无还款能力），而作为一名风控搬砖工，日常工作中有大量的数据挖掘工作，如何从高维数据集中挖掘出行之有效的规则、策略及模型来防范欺诈风险和信用风险每个搬砖工的基操。本仓库由笔者基于网上开源的一系列相关知识，结合实际工作中遇到的实际需求，整理得到。旨在为诸位仁兄提供一个便捷、高效、赏心悦目的决策树组合策略挖掘报告，及一系列能够实际运用到风险控制上的策略。
 
+## 项目结构
+
+```bash
+pdtr
+.
+|   README.md                           # 说明文档
+|   setup.py                            # 打包发布文件
+|   LICENSE                             # 开源协议
+|   requirements.txt                    # 项目依赖包
++---examples                            # 演示样例
+|   |   combine_rules_cache             # 缓存文件
+|   |   combine_rules_cache.svg         # 缓存文件
+|   |   pdtr_samplts.ipynb              # 演示样例程序
+|   \---model_report                    # 模型报告输出文件夹
+|       |   决策树组合策略挖掘.xlsx        # 策略挖掘报告
+|       +---auto_mining_rules           # 组合策略可视化存储文件夹
+|       |       combiner_rules_0.png    # 决策树可视化图片
+|       |       ......
+|       \---bin_plots                   # 简单策略可视化存储文件夹
+|               bin_vars_A.png          # 变量分箱可视化图片
+|               ......
+\---pdtr                                # PDTR 源码包
+        template.xlsx                   # excel 模版文件
+        excel_writer.py                 # excel写入公共方法
+        matplot_chinese.ttf             # matplotlib 中文字体
+        transforme.py                   # 策略挖掘方法
+```
+
 ## 环境准备
 
 ### 创建虚拟环境（可选）
 
 + 通过`conda`创建虚拟环境
 
 ```bash
@@ -144,14 +182,24 @@
 
 ### `PDTR` 安装
 
 ```bash
 pip install pdtr
 ```
 
+### 版本介绍
+
++ `0.1.0`
+
+仅包含决策树策略挖掘相关工具
+
++ `0.1.1`
+
+除版本 `0.1.0` 中的决策树挖掘相关工具以外，新增了基于 `toad` 和 `optbinning` 的单变量策略挖掘相关方法
+
 
 ### 运行样例
 
 + 导入相关依赖
 
 ```python
 import os
@@ -209,15 +257,15 @@
 
 ```python
 pdtr_instance.save()
 ```
 
 + 挖掘报告
 
-`examples/决策树组合策略挖掘.xlsx`
+[`examples/决策树组合策略挖掘.xlsx`](https://github.com/itlubber/pdtr/blob/main/examples/model_report/%E5%86%B3%E7%AD%96%E6%A0%91%E7%BB%84%E5%90%88%E7%AD%96%E7%95%A5%E6%8C%96%E6%8E%98.xlsx)
 
 
 ## 参考
 
 > https://github.com/itlubber/LogisticRegressionPipeline
 > 
 > https://github.com/itlubber/itlubber-excel-writer
```

### Comparing `pdtr-0.1.1/setup.py` & `pdtr-0.1.2/setup.py`

 * *Files identical despite different names*

