# Comparing `tmp/nonebot_plugin_pluginupdatecheck-0.1.0.tar.gz` & `tmp/nonebot_plugin_pluginupdatecheck-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_pluginupdatecheck-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_pluginupdatecheck-0.1.1.tar", max compression
```

## Comparing `nonebot_plugin_pluginupdatecheck-0.1.0.tar` & `nonebot_plugin_pluginupdatecheck-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11640 2023-05-18 14:02:31.800200 nonebot_plugin_pluginupdatecheck-0.1.0/nonebot_plugin_pluginupdatecheck/__init__.py
--rw-r--r--   0        0        0      114 2023-05-15 16:49:10.271000 nonebot_plugin_pluginupdatecheck-0.1.0/nonebot_plugin_pluginupdatecheck/config.py
--rw-r--r--   0        0        0      722 2023-05-16 11:39:45.831000 nonebot_plugin_pluginupdatecheck-0.1.0/nonebot_plugin_pluginupdatecheck/tool.py
--rw-r--r--   0        0        0      535 2023-05-16 14:35:20.146675 nonebot_plugin_pluginupdatecheck-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2260 2023-05-16 15:02:29.979491 nonebot_plugin_pluginupdatecheck-0.1.0/README.md
--rw-r--r--   0        0        0     3053 1970-01-01 00:00:00.000000 nonebot_plugin_pluginupdatecheck-0.1.0/setup.py
--rw-r--r--   0        0        0     2820 1970-01-01 00:00:00.000000 nonebot_plugin_pluginupdatecheck-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11628 2023-05-18 14:13:07.594478 nonebot_plugin_pluginupdatecheck-0.1.1/nonebot_plugin_pluginupdatecheck/__init__.py
+-rw-r--r--   0        0        0      114 2023-05-15 16:49:10.271000 nonebot_plugin_pluginupdatecheck-0.1.1/nonebot_plugin_pluginupdatecheck/config.py
+-rw-r--r--   0        0        0      722 2023-05-16 11:39:45.831000 nonebot_plugin_pluginupdatecheck-0.1.1/nonebot_plugin_pluginupdatecheck/tool.py
+-rw-r--r--   0        0        0      554 2023-05-18 16:24:33.890903 nonebot_plugin_pluginupdatecheck-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2260 2023-05-16 15:02:29.979491 nonebot_plugin_pluginupdatecheck-0.1.1/README.md
+-rw-r--r--   0        0        0     3077 1970-01-01 00:00:00.000000 nonebot_plugin_pluginupdatecheck-0.1.1/setup.py
+-rw-r--r--   0        0        0     2859 1970-01-01 00:00:00.000000 nonebot_plugin_pluginupdatecheck-0.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_pluginupdatecheck-0.1.0/nonebot_plugin_pluginupdatecheck/__init__.py` & `nonebot_plugin_pluginupdatecheck-0.1.1/nonebot_plugin_pluginupdatecheck/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import asyncio
-import json
 
 import numpy as np
 import toml
 from nonebot import get_driver, on_command
 from nonebot.matcher import Matcher
 from nonebot.adapters.onebot.v11 import Bot, MessageEvent, Message
 from nonebot.params import CommandArg, ArgPlainText
```

### Comparing `nonebot_plugin_pluginupdatecheck-0.1.0/nonebot_plugin_pluginupdatecheck/tool.py` & `nonebot_plugin_pluginupdatecheck-0.1.1/nonebot_plugin_pluginupdatecheck/tool.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pluginupdatecheck-0.1.0/pyproject.toml` & `nonebot_plugin_pluginupdatecheck-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [tool.poetry]
 name = "nonebot-plugin-pluginupdatecheck"
-version = "0.1.0"
+version = "0.1.1"
 description = "A plugin of chatbot based on nonebot2 framework,it can check the updateable plugins already installed.Also can install new plugins."
 authors = ["xi-yue-233 <1004514855@qq.com>"]
 readme = "README.md"
 packages = [{include = "nonebot_plugin_pluginupdatecheck"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 nonebot2 = "^2.0.0rc2"
 toml = "^0.10.2"
+numpy = "^1.24.3"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_pluginupdatecheck-0.1.0/README.md` & `nonebot_plugin_pluginupdatecheck-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pluginupdatecheck-0.1.0/setup.py` & `nonebot_plugin_pluginupdatecheck-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['nonebot_plugin_pluginupdatecheck']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['nonebot2>=2.0.0rc2,<3.0.0', 'toml>=0.10.2,<0.11.0']
+['nonebot2>=2.0.0rc2,<3.0.0', 'numpy>=1.24.3,<2.0.0', 'toml>=0.10.2,<0.11.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-pluginupdatecheck',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'A plugin of chatbot based on nonebot2 framework,it can check the updateable plugins already installed.Also can install new plugins.',
     'long_description': '<p align="center">\n  <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>\n</p>\n\n<div align="center">\n\n# nonebot_plugin_pluginupdatecheck\n\nnonebot2便携插件安装器\n\n</div>\n\n## 💬 前言\n\n一个nonebot2的插件便捷安装和升级插件（基于nb-cli和pip)\n\n## 📖 介绍\n\n为了方便我在手机上直接控制bot安装和更新插件而开发的一款插件\n\n## 💿 安装\n\n<details>\n<summary>nb-cli安装</summary>\n在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装\n  \n    nb plugin install nonebot-plugin-pluginupdatecheck\n\n</details>\n\n<details>\n<summary>pip安装</summary>\n  \n    pip install nonebot-plugin-pluginupdatecheck\n\n</details>\n\n## 🎉 使用\n\n检测插件更新：输入检测插件更新、检查插件更新\n\n![image](https://github.com/xi-yue-233/nonebot-plugin-pluginupdatecheck/assets/58218656/f6defd18-6279-45f4-a009-83cfda529e2d)\n![20230516225101](https://github.com/xi-yue-233/nonebot-plugin-pluginupdatecheck/assets/58218656/8d26d5d0-ef2b-458b-803e-0aa0afc5fa41)\n\n更新指定插件：输入更新插件“你指定的插件”空格后加的数字编号代表python源（默认清华源）\n\n![20230516225504](https://github.com/xi-yue-233/nonebot-plugin-pluginupdatecheck/assets/58218656/74707dc0-2bd8-46b9-b143-2a23e885ad39)\n\n\n安装指定插件：输入安装插件“你指定的插件”空格后加的数字编号代表python源（默认清华源）\n\n![20230516225647](https://github.com/xi-yue-233/nonebot-plugin-pluginupdatecheck/assets/58218656/aa60add9-93e2-4da6-8eff-fcd3085441cd)\n\n查看源：查看可以用的python源，前面的数字编号可以在插件安装的时候使用\n\n![20230516225748](https://github.com/xi-yue-233/nonebot-plugin-pluginupdatecheck/assets/58218656/e6e7f048-f75e-4a2f-9c9c-eb2ec8cec271)\n\n添加env环境变量：输入添加env后接要加的变量\n\n![20230516225930](https://github.com/xi-yue-233/nonebot-plugin-pluginupdatecheck/assets/58218656/c424be62-b99b-486b-83a3-4b458be6c086)\n![20230516230020](https://github.com/xi-yue-233/nonebot-plugin-pluginupdatecheck/assets/58218656/ce09af1d-72e3-448a-8c42-65f902d48f08)\n',
     'author': 'xi-yue-233',
     'author_email': '1004514855@qq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['nonebot_plugin_pluginupdatecheck'] package_data = \ {'': ['*']}
-install_requires = \ ['nonebot2>=2.0.0rc2,<3.0.0', 'toml>=0.10.2,<0.11.0']
-setup_kwargs = { 'name': 'nonebot-plugin-pluginupdatecheck', 'version':
-'0.1.0', 'description': 'A plugin of chatbot based on nonebot2 framework,it can
-check the updateable plugins already installed.Also can install new plugins.',
-'long_description': '
+install_requires = \ ['nonebot2>=2.0.0rc2,<3.0.0', 'numpy>=1.24.3,<2.0.0',
+'toml>=0.10.2,<0.11.0'] setup_kwargs = { 'name': 'nonebot-plugin-
+pluginupdatecheck', 'version': '0.1.1', 'description': 'A plugin of chatbot
+based on nonebot2 framework,it can check the updateable plugins already
+installed.Also can install new plugins.', 'long_description': '
                                 \n [nonebot]\n
 \n\n
   \n\n# nonebot_plugin_pluginupdatecheck\n\nnonebot2ä¾¿æºæä»¶å®è£å¨\n\n
 \n\n## ð¬
 åè¨\n\nä¸ä¸ªnonebot2çæä»¶ä¾¿æ·å®è£ååçº§æä»¶ï¼åºäºnb-
 cliåpip)\n\n## ð
 ä»ç»\n\nä¸ºäºæ¹ä¾¿æå¨ææºä¸ç´æ¥æ§å¶botå®è£åæ´æ°æä»¶èå¼åçä¸æ¬¾æä»¶\n\n##
```

### Comparing `nonebot_plugin_pluginupdatecheck-0.1.0/PKG-INFO` & `nonebot_plugin_pluginupdatecheck-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-pluginupdatecheck
-Version: 0.1.0
+Version: 0.1.1
 Summary: A plugin of chatbot based on nonebot2 framework,it can check the updateable plugins already installed.Also can install new plugins.
 Author: xi-yue-233
 Author-email: 1004514855@qq.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: nonebot2 (>=2.0.0rc2,<3.0.0)
+Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
 </p>
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-pluginupdatecheck Version: 0.1.0
+Metadata-Version: 2.1 Name: nonebot-plugin-pluginupdatecheck Version: 0.1.1
 Summary: A plugin of chatbot based on nonebot2 framework,it can check the
 updateable plugins already installed.Also can install new plugins. Author: xi-
 yue-233 Author-email: 1004514855@qq.com Requires-Python: >=3.9,<4.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: nonebot2
-(>=2.0.0rc2,<3.0.0) Requires-Dist: toml (>=0.10.2,<0.11.0) Description-Content-
-Type: text/markdown
+(>=2.0.0rc2,<3.0.0) Requires-Dist: numpy (>=1.24.3,<2.0.0) Requires-Dist: toml
+(>=0.10.2,<0.11.0) Description-Content-Type: text/markdown
                                    [nonebot]
        # nonebot_plugin_pluginupdatecheck nonebot2ä¾¿æºæä»¶å®è£å¨
 ## ð¬ åè¨ ä¸ä¸ªnonebot2çæä»¶ä¾¿æ·å®è£ååçº§æä»¶ï¼åºäºnb-
 cliåpip) ## ð ä»ç»
 ä¸ºäºæ¹ä¾¿æå¨ææºä¸ç´æ¥æ§å¶botå®è£åæ´æ°æä»¶èå¼åçä¸æ¬¾æä»¶
 ## ð¿ å®è£  nb-cliå®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-
```

