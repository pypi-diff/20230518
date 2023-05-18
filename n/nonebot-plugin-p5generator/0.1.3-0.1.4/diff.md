# Comparing `tmp/nonebot_plugin_p5generator-0.1.3.tar.gz` & `tmp/nonebot_plugin_p5generator-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_p5generator-0.1.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_p5generator-0.1.4.tar", max compression
```

## Comparing `nonebot_plugin_p5generator-0.1.3.tar` & `nonebot_plugin_p5generator-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      940 2023-05-18 08:27:21.316896 nonebot_plugin_p5generator-0.1.3/nonebot_plugin_p5generator/__init__.py
--rw-r--r--   0        0        0     8396 2023-05-18 08:27:54.965459 nonebot_plugin_p5generator-0.1.3/nonebot_plugin_p5generator/generator.py
--rw-r--r--   0        0        0      487 2023-05-18 08:30:23.390881 nonebot_plugin_p5generator-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1485 2023-05-16 06:42:08.922667 nonebot_plugin_p5generator-0.1.3/README.md
--rw-r--r--   0        0        0     2237 1970-01-01 00:00:00.000000 nonebot_plugin_p5generator-0.1.3/setup.py
--rw-r--r--   0        0        0     2032 1970-01-01 00:00:00.000000 nonebot_plugin_p5generator-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      940 2023-05-18 08:27:21.316896 nonebot_plugin_p5generator-0.1.4/nonebot_plugin_p5generator/__init__.py
+-rw-r--r--   0        0        0     8502 2023-05-18 08:53:02.245339 nonebot_plugin_p5generator-0.1.4/nonebot_plugin_p5generator/generator.py
+-rw-r--r--   0        0        0      487 2023-05-18 08:37:53.011809 nonebot_plugin_p5generator-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1935 2023-05-18 08:36:59.162075 nonebot_plugin_p5generator-0.1.4/README.md
+-rw-r--r--   0        0        0     2687 1970-01-01 00:00:00.000000 nonebot_plugin_p5generator-0.1.4/setup.py
+-rw-r--r--   0        0        0     2471 1970-01-01 00:00:00.000000 nonebot_plugin_p5generator-0.1.4/PKG-INFO
```

### Comparing `nonebot_plugin_p5generator-0.1.3/nonebot_plugin_p5generator/__init__.py` & `nonebot_plugin_p5generator-0.1.4/nonebot_plugin_p5generator/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_p5generator-0.1.3/nonebot_plugin_p5generator/generator.py` & `nonebot_plugin_p5generator-0.1.4/nonebot_plugin_p5generator/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 import random
 
 RESOURCES_PATH = Path() / 'data' / 'p5generator'
 RESOURCES_PATH.mkdir(parents=True, exist_ok=True)
 
 async def generate_image(text):
     # 设置字体列表
-    fonts = ['msyhbd.ttc']
+    fonts = ['msyh.ttc', 'STHUPO.TTF', 'simsun.ttc', 'msyhbd.ttc', 'simhei.ttf']
     # 设置颜色列表
-    colors = ['white', 'red']
+    colors = ['white', 'black', 'gray', 'red']
     # 设置背景颜色列表
-    bg_colors = {'white': ['black', 'red'], 'red': ['black']}
+    bg_colors = {'white': ['black', 'gray'], 'black': ['white', 'gray'], 'gray': ['white', 'black'], 'red': ['white']}
 
     # 打开背景图片
     background_image = Image.open(os.path.join(RESOURCES_PATH, "background.png"))
 
     # 获取背景图片大小
     width, height = background_image.size
 
@@ -78,15 +78,15 @@
             char_width, char_height = font.getsize(char)
 
             # 创建字符图像和绘图对象
             char_image = Image.new('RGBA', (char_width, char_height))
             char_draw = ImageDraw.Draw(char_image)
 
             # 绘制背景色块
-            char_draw.rectangle((0, 0, char_width, char_height), fill=bg_color, outline='white', width=7)
+            char_draw.rectangle((0, 0, char_width, char_height), fill=bg_color)
             # 绘制字符
             char_draw.text((0, 0), char, fill=color, font=font)
 
             # 随机旋转角度
             angle = random.randint(-5, 5)
             char_image = char_image.rotate(angle, resample=Image.BICUBIC, expand=True)
 
@@ -167,15 +167,15 @@
             color = random.choice(colors)
             # 根据颜色选择背景颜色
             bg_color = random.choice(bg_colors[color])
             # 获取字符大小
             char_width, char_height = font.getsize(char)
 
             # 创建字符图像和绘图对象
-            char_image = Image.new('RGBA', (char_width, char_height))
+            char_image = Image.new('RGBA', (char_width+7, char_height+7))
             char_draw = ImageDraw.Draw(char_image)
 
             # 绘制背景色块
             char_draw.rectangle((0, 0, char_width+7, char_height+7), fill=bg_color, outline='white', width=7)
             # 绘制字符
             char_draw.text((0, 0), char, fill=color, font=font)
```

### Comparing `nonebot_plugin_p5generator-0.1.3/README.md` & `nonebot_plugin_p5generator-0.1.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 《女神异闻录5》预告信的生成插件
 
 </div>
 
 ## 💬 前言
 
-可以生成仿《女神异闻录5》中心之怪盗团向罪人宣战的预告信，做的不太好请见谅
+可以生成仿《女神异闻录5》中心之怪盗团向罪人宣战的预告信和UI，做的不太好请见谅
 
 ## 📖 介绍
 
 使用Pillow库制作的一款插件，因为p5中的预告信字都是从报纸上面剪下来的，所以还原了随机的字体。
 代码比较烂，随便看看吧。
 知识和勇气增加了。
 
@@ -46,7 +46,18 @@
 ## 🎉 使用
 
 输入`p5预告信`后接你想要输入的内容即可生成：
 
 ![946CE1499E017FE129710E8B6E2FB725](https://github.com/xi-yue-233/nonebot-plugin-p5generator/assets/58218656/0a19bacc-bde4-4693-93e7-83678bde4835)
 
 ![5C4D9FCBE4F060A12612D6062287E7E6](https://github.com/xi-yue-233/nonebot-plugin-p5generator/assets/58218656/4aade3a7-34a0-4e81-96ea-612146b76808)
+
+输入`p5ui`后接你想要输入的内容即可生成：
+
+![B@C0RM X1D~R KV E`R@OQ9](https://github.com/xi-yue-233/nonebot-plugin-p5generator/assets/58218656/6d727c63-25d6-4937-b3de-17e3a95c57a3)
+
+![8B9B74C29BC2BD25DA436A7B73E9A461](https://github.com/xi-yue-233/nonebot-plugin-p5generator/assets/58218656/d9b9033c-01f1-4a99-9cb0-efcf1dc5e9b0)
+
+
+## 🎉 感谢
+
+感谢Suica0w0 https://github.com/Suica0w0 提供的生成p5rui功能
```

#### html2text {}

```diff
@@ -1,17 +1,24 @@
                                    [nonebot]
   # nonebot-plugin-p5generator ãå¥³ç¥å¼é»å½5ãé¢åä¿¡ççææä»¶
 ## ð¬ åè¨
-å¯ä»¥çæä»¿ãå¥³ç¥å¼é»å½5ãä¸­å¿ä¹æªçå¢åç½ªäººå®£æçé¢åä¿¡ï¼åçä¸å¤ªå¥½è¯·è§è°
+å¯ä»¥çæä»¿ãå¥³ç¥å¼é»å½5ãä¸­å¿ä¹æªçå¢åç½ªäººå®£æçé¢åä¿¡åUIï¼åçä¸å¤ªå¥½è¯·è§è°
 ## ð ä»ç»
 ä½¿ç¨Pillowåºå¶ä½çä¸æ¬¾æä»¶ï¼å ä¸ºp5ä¸­çé¢åä¿¡å­é½æ¯ä»æ¥çº¸ä¸é¢åªä¸æ¥çï¼æä»¥è¿åäºéæºçå­ä½ã
 ä»£ç æ¯è¾çï¼éä¾¿ççå§ã ç¥è¯ååæ°å¢å äºã ## ð¿ å®è£
 nb-cliå®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-p5generator
 pipå®è£ pip install nonebot-plugin-p5generator  ## ð° èµæºæä»¶
 `data`æä»¶å¤¹ä¸­ç`p5generator`ä¼å­å¨ä¸æä»¶æå³çæä»¶
 ä¸è½½ä»åºä¸­p5generatoræä»¶å¤¹åæ¾å¥dataæä»¶å¤¹ä¸­ ## ð ä½¿ç¨
 è¾å¥`p5é¢åä¿¡`åæ¥ä½ æ³è¦è¾å¥çåå®¹å³å¯çæï¼ !
 [946CE1499E017FE129710E8B6E2FB725](https://github.com/xi-yue-233/nonebot-
 plugin-p5generator/assets/58218656/0a19bacc-bde4-4693-93e7-83678bde4835) !
 [5C4D9FCBE4F060A12612D6062287E7E6](https://github.com/xi-yue-233/nonebot-
 plugin-p5generator/assets/58218656/4aade3a7-34a0-4e81-96ea-612146b76808)
+è¾å¥`p5ui`åæ¥ä½ æ³è¦è¾å¥çåå®¹å³å¯çæï¼ ![B@C0RM X1D~R KV
+E`R@OQ9](https://github.com/xi-yue-233/nonebot-plugin-p5generator/assets/
+58218656/6d727c63-25d6-4937-b3de-17e3a95c57a3) !
+[8B9B74C29BC2BD25DA436A7B73E9A461](https://github.com/xi-yue-233/nonebot-
+plugin-p5generator/assets/58218656/d9b9033c-01f1-4a99-9cb0-efcf1dc5e9b0) ##
+ð æè°¢ æè°¢Suica0w0 https://github.com/Suica0w0
+æä¾ççæp5ruiåè½
```

### Comparing `nonebot_plugin_p5generator-0.1.3/setup.py` & `nonebot_plugin_p5generator-0.1.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 install_requires = \
 ['nonebot-adapter-onebot>=2.2.0,<3.0.0',
  'nonebot2>=2.0.0rc2,<3.0.0',
  'pillow>=9.5.0,<10.0.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-p5generator',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'A generator of persona5 chatbot based on nonebot2 framework',
-    'long_description': '<p align="center">\n  <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>\n</p>\n\n<div align="center">\n\n# nonebot-plugin-p5generator\n\n《女神异闻录5》预告信的生成插件\n\n</div>\n\n## 💬 前言\n\n可以生成仿《女神异闻录5》中心之怪盗团向罪人宣战的预告信，做的不太好请见谅\n\n## 📖 介绍\n\n使用Pillow库制作的一款插件，因为p5中的预告信字都是从报纸上面剪下来的，所以还原了随机的字体。\n代码比较烂，随便看看吧。\n知识和勇气增加了。\n\n## 💿 安装\n\n<details>\n<summary>nb-cli安装</summary>\n在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装\n  \n    nb plugin install nonebot-plugin-p5generator\n\n</details>\n\n<details>\n<summary>pip安装</summary>\n  \n    pip install nonebot-plugin-p5generator\n\n</details>\n\n## 🍰 资源文件\n\n`data`文件夹中的`p5generator`会存储与插件有关的文件\n\n下载仓库中p5generator文件夹后放入data文件夹中\n\n## 🎉 使用\n\n输入`p5预告信`后接你想要输入的内容即可生成：\n\n![946CE1499E017FE129710E8B6E2FB725](https://github.com/xi-yue-233/nonebot-plugin-p5generator/assets/58218656/0a19bacc-bde4-4693-93e7-83678bde4835)\n\n![5C4D9FCBE4F060A12612D6062287E7E6](https://github.com/xi-yue-233/nonebot-plugin-p5generator/assets/58218656/4aade3a7-34a0-4e81-96ea-612146b76808)\n',
+    'long_description': '<p align="center">\n  <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>\n</p>\n\n<div align="center">\n\n# nonebot-plugin-p5generator\n\n《女神异闻录5》预告信的生成插件\n\n</div>\n\n## 💬 前言\n\n可以生成仿《女神异闻录5》中心之怪盗团向罪人宣战的预告信和UI，做的不太好请见谅\n\n## 📖 介绍\n\n使用Pillow库制作的一款插件，因为p5中的预告信字都是从报纸上面剪下来的，所以还原了随机的字体。\n代码比较烂，随便看看吧。\n知识和勇气增加了。\n\n## 💿 安装\n\n<details>\n<summary>nb-cli安装</summary>\n在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装\n  \n    nb plugin install nonebot-plugin-p5generator\n\n</details>\n\n<details>\n<summary>pip安装</summary>\n  \n    pip install nonebot-plugin-p5generator\n\n</details>\n\n## 🍰 资源文件\n\n`data`文件夹中的`p5generator`会存储与插件有关的文件\n\n下载仓库中p5generator文件夹后放入data文件夹中\n\n## 🎉 使用\n\n输入`p5预告信`后接你想要输入的内容即可生成：\n\n![946CE1499E017FE129710E8B6E2FB725](https://github.com/xi-yue-233/nonebot-plugin-p5generator/assets/58218656/0a19bacc-bde4-4693-93e7-83678bde4835)\n\n![5C4D9FCBE4F060A12612D6062287E7E6](https://github.com/xi-yue-233/nonebot-plugin-p5generator/assets/58218656/4aade3a7-34a0-4e81-96ea-612146b76808)\n\n输入`p5ui`后接你想要输入的内容即可生成：\n\n![B@C0RM X1D~R KV E`R@OQ9](https://github.com/xi-yue-233/nonebot-plugin-p5generator/assets/58218656/6d727c63-25d6-4937-b3de-17e3a95c57a3)\n\n![8B9B74C29BC2BD25DA436A7B73E9A461](https://github.com/xi-yue-233/nonebot-plugin-p5generator/assets/58218656/d9b9033c-01f1-4a99-9cb0-efcf1dc5e9b0)\n\n\n## 🎉 感谢\n\n感谢Suica0w0 https://github.com/Suica0w0 提供的生成p5rui功能\n',
     'author': 'xi-yue-233',
     'author_email': '1004514855@qq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,29 +1,35 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['nonebot_plugin_p5generator'] package_data = \ {'': ['*']} install_requires =
 \ ['nonebot-adapter-onebot>=2.2.0,<3.0.0', 'nonebot2>=2.0.0rc2,<3.0.0',
 'pillow>=9.5.0,<10.0.0'] setup_kwargs = { 'name': 'nonebot-plugin-p5generator',
-'version': '0.1.3', 'description': 'A generator of persona5 chatbot based on
+'version': '0.1.4', 'description': 'A generator of persona5 chatbot based on
 nonebot2 framework', 'long_description': '
                                 \n [nonebot]\n
 \n\n
                              \n\n# nonebot-plugin-
        p5generator\n\nãå¥³ç¥å¼é»å½5ãé¢åä¿¡ççææä»¶\n\n
 \n\n## ð¬
-åè¨\n\nå¯ä»¥çæä»¿ãå¥³ç¥å¼é»å½5ãä¸­å¿ä¹æªçå¢åç½ªäººå®£æçé¢åä¿¡ï¼åçä¸å¤ªå¥½è¯·è§è°\n\n##
+åè¨\n\nå¯ä»¥çæä»¿ãå¥³ç¥å¼é»å½5ãä¸­å¿ä¹æªçå¢åç½ªäººå®£æçé¢åä¿¡åUIï¼åçä¸å¤ªå¥½è¯·è§è°\n\n##
 ð
 ä»ç»\n\nä½¿ç¨Pillowåºå¶ä½çä¸æ¬¾æä»¶ï¼å ä¸ºp5ä¸­çé¢åä¿¡å­é½æ¯ä»æ¥çº¸ä¸é¢åªä¸æ¥çï¼æä»¥è¿åäºéæºçå­ä½ã\nä»£ç æ¯è¾çï¼éä¾¿ççå§ã\nç¥è¯ååæ°å¢å äºã\n\n##
 ð¿ å®è£\n\n\nnb-cliå®è£\nå¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£\n \n nb
 plugin install nonebot-plugin-p5generator\n\n\n\n\npipå®è£\n \n pip install
 nonebot-plugin-p5generator\n\n\n\n## ð°
 èµæºæä»¶\n\n`data`æä»¶å¤¹ä¸­ç`p5generator`ä¼å­å¨ä¸æä»¶æå³çæä»¶\n\nä¸è½½ä»åºä¸­p5generatoræä»¶å¤¹åæ¾å¥dataæä»¶å¤¹ä¸­\n\n##
 ð
 ä½¿ç¨\n\nè¾å¥`p5é¢åä¿¡`åæ¥ä½ æ³è¦è¾å¥çåå®¹å³å¯çæï¼\n\n!
 [946CE1499E017FE129710E8B6E2FB725](https://github.com/xi-yue-233/nonebot-
 plugin-p5generator/assets/58218656/0a19bacc-bde4-4693-93e7-83678bde4835)\n\n!
 [5C4D9FCBE4F060A12612D6062287E7E6](https://github.com/xi-yue-233/nonebot-
-plugin-p5generator/assets/58218656/4aade3a7-34a0-4e81-96ea-612146b76808)\n',
-'author': 'xi-yue-233', 'author_email': '1004514855@qq.com', 'maintainer':
-'None', 'maintainer_email': 'None', 'url': 'None', 'packages': packages,
-'package_data': package_data, 'install_requires': install_requires,
-'python_requires': '>=3.9,<4.0', } setup(**setup_kwargs)
+plugin-p5generator/assets/58218656/4aade3a7-34a0-4e81-96ea-
+612146b76808)\n\nè¾å¥`p5ui`åæ¥ä½ æ³è¦è¾å¥çåå®¹å³å¯çæï¼\n\n!
+[B@C0RM X1D~R KV E`R@OQ9](https://github.com/xi-yue-233/nonebot-plugin-
+p5generator/assets/58218656/6d727c63-25d6-4937-b3de-17e3a95c57a3)\n\n!
+[8B9B74C29BC2BD25DA436A7B73E9A461](https://github.com/xi-yue-233/nonebot-
+plugin-p5generator/assets/58218656/d9b9033c-01f1-4a99-9cb0-
+efcf1dc5e9b0)\n\n\n## ð æè°¢\n\næè°¢Suica0w0 https://github.com/Suica0w0
+æä¾ççæp5ruiåè½\n', 'author': 'xi-yue-233', 'author_email':
+'1004514855@qq.com', 'maintainer': 'None', 'maintainer_email': 'None', 'url':
+'None', 'packages': packages, 'package_data': package_data, 'install_requires':
+install_requires, 'python_requires': '>=3.9,<4.0', } setup(**setup_kwargs)
```

### Comparing `nonebot_plugin_p5generator-0.1.3/PKG-INFO` & `nonebot_plugin_p5generator-0.1.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-p5generator
-Version: 0.1.3
+Version: 0.1.4
 Summary: A generator of persona5 chatbot based on nonebot2 framework
 Author: xi-yue-233
 Author-email: 1004514855@qq.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -24,15 +24,15 @@
 
 《女神异闻录5》预告信的生成插件
 
 </div>
 
 ## 💬 前言
 
-可以生成仿《女神异闻录5》中心之怪盗团向罪人宣战的预告信，做的不太好请见谅
+可以生成仿《女神异闻录5》中心之怪盗团向罪人宣战的预告信和UI，做的不太好请见谅
 
 ## 📖 介绍
 
 使用Pillow库制作的一款插件，因为p5中的预告信字都是从报纸上面剪下来的，所以还原了随机的字体。
 代码比较烂，随便看看吧。
 知识和勇气增加了。
 
@@ -63,7 +63,18 @@
 
 输入`p5预告信`后接你想要输入的内容即可生成：
 
 ![946CE1499E017FE129710E8B6E2FB725](https://github.com/xi-yue-233/nonebot-plugin-p5generator/assets/58218656/0a19bacc-bde4-4693-93e7-83678bde4835)
 
 ![5C4D9FCBE4F060A12612D6062287E7E6](https://github.com/xi-yue-233/nonebot-plugin-p5generator/assets/58218656/4aade3a7-34a0-4e81-96ea-612146b76808)
 
+输入`p5ui`后接你想要输入的内容即可生成：
+
+![B@C0RM X1D~R KV E`R@OQ9](https://github.com/xi-yue-233/nonebot-plugin-p5generator/assets/58218656/6d727c63-25d6-4937-b3de-17e3a95c57a3)
+
+![8B9B74C29BC2BD25DA436A7B73E9A461](https://github.com/xi-yue-233/nonebot-plugin-p5generator/assets/58218656/d9b9033c-01f1-4a99-9cb0-efcf1dc5e9b0)
+
+
+## 🎉 感谢
+
+感谢Suica0w0 https://github.com/Suica0w0 提供的生成p5rui功能
+
```

#### html2text {}

```diff
@@ -1,25 +1,32 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-p5generator Version: 0.1.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-p5generator Version: 0.1.4 Summary:
 A generator of persona5 chatbot based on nonebot2 framework Author: xi-yue-233
 Author-email: 1004514855@qq.com Requires-Python: >=3.9,<4.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: nonebot-adapter-onebot
 (>=2.2.0,<3.0.0) Requires-Dist: nonebot2 (>=2.0.0rc2,<3.0.0) Requires-Dist:
 pillow (>=9.5.0,<10.0.0) Description-Content-Type: text/markdown
                                    [nonebot]
   # nonebot-plugin-p5generator ãå¥³ç¥å¼é»å½5ãé¢åä¿¡ççææä»¶
 ## ð¬ åè¨
-å¯ä»¥çæä»¿ãå¥³ç¥å¼é»å½5ãä¸­å¿ä¹æªçå¢åç½ªäººå®£æçé¢åä¿¡ï¼åçä¸å¤ªå¥½è¯·è§è°
+å¯ä»¥çæä»¿ãå¥³ç¥å¼é»å½5ãä¸­å¿ä¹æªçå¢åç½ªäººå®£æçé¢åä¿¡åUIï¼åçä¸å¤ªå¥½è¯·è§è°
 ## ð ä»ç»
 ä½¿ç¨Pillowåºå¶ä½çä¸æ¬¾æä»¶ï¼å ä¸ºp5ä¸­çé¢åä¿¡å­é½æ¯ä»æ¥çº¸ä¸é¢åªä¸æ¥çï¼æä»¥è¿åäºéæºçå­ä½ã
 ä»£ç æ¯è¾çï¼éä¾¿ççå§ã ç¥è¯ååæ°å¢å äºã ## ð¿ å®è£
 nb-cliå®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-p5generator
 pipå®è£ pip install nonebot-plugin-p5generator  ## ð° èµæºæä»¶
 `data`æä»¶å¤¹ä¸­ç`p5generator`ä¼å­å¨ä¸æä»¶æå³çæä»¶
 ä¸è½½ä»åºä¸­p5generatoræä»¶å¤¹åæ¾å¥dataæä»¶å¤¹ä¸­ ## ð ä½¿ç¨
 è¾å¥`p5é¢åä¿¡`åæ¥ä½ æ³è¦è¾å¥çåå®¹å³å¯çæï¼ !
 [946CE1499E017FE129710E8B6E2FB725](https://github.com/xi-yue-233/nonebot-
 plugin-p5generator/assets/58218656/0a19bacc-bde4-4693-93e7-83678bde4835) !
 [5C4D9FCBE4F060A12612D6062287E7E6](https://github.com/xi-yue-233/nonebot-
 plugin-p5generator/assets/58218656/4aade3a7-34a0-4e81-96ea-612146b76808)
+è¾å¥`p5ui`åæ¥ä½ æ³è¦è¾å¥çåå®¹å³å¯çæï¼ ![B@C0RM X1D~R KV
+E`R@OQ9](https://github.com/xi-yue-233/nonebot-plugin-p5generator/assets/
+58218656/6d727c63-25d6-4937-b3de-17e3a95c57a3) !
+[8B9B74C29BC2BD25DA436A7B73E9A461](https://github.com/xi-yue-233/nonebot-
+plugin-p5generator/assets/58218656/d9b9033c-01f1-4a99-9cb0-efcf1dc5e9b0) ##
+ð æè°¢ æè°¢Suica0w0 https://github.com/Suica0w0
+æä¾ççæp5ruiåè½
```

