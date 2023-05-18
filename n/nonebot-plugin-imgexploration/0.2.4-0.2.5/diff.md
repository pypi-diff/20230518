# Comparing `tmp/nonebot_plugin_imgexploration-0.2.4.tar.gz` & `tmp/nonebot-plugin-imgexploration-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_imgexploration-0.2.4.tar", last modified: Mon Feb 13 13:33:37 2023, max compression
+gzip compressed data, was "nonebot-plugin-imgexploration-0.2.5.tar", last modified: Thu May 18 14:37:06 2023, max compression
```

## Comparing `nonebot_plugin_imgexploration-0.2.4.tar` & `nonebot-plugin-imgexploration-0.2.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-02-13 13:33:37.029155 nonebot_plugin_imgexploration-0.2.4/
--rw-rw-rw-   0        0        0     1088 2022-12-26 13:04:44.000000 nonebot_plugin_imgexploration-0.2.4/LICENSE.txt
--rw-rw-rw-   0        0        0      166 2022-12-26 13:05:40.000000 nonebot_plugin_imgexploration-0.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2656 2023-02-13 13:33:37.028052 nonebot_plugin_imgexploration-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     1950 2023-02-13 13:33:13.000000 nonebot_plugin_imgexploration-0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-02-13 13:33:36.995538 nonebot_plugin_imgexploration-0.2.4/nonebot_plugin_imgexploration/
--rw-rw-rw-   0        0        0     4082 2023-02-13 13:28:02.000000 nonebot_plugin_imgexploration-0.2.4/nonebot_plugin_imgexploration/__init__.py
--rw-rw-rw-   0        0        0    19661 2023-02-13 13:13:35.000000 nonebot_plugin_imgexploration-0.2.4/nonebot_plugin_imgexploration/imgexploration.py
-drwxrwxrwx   0        0        0        0 2023-02-13 13:33:37.027055 nonebot_plugin_imgexploration-0.2.4/nonebot_plugin_imgexploration.egg-info/
--rw-rw-rw-   0        0        0     2656 2023-02-13 13:33:36.000000 nonebot_plugin_imgexploration-0.2.4/nonebot_plugin_imgexploration.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      411 2023-02-13 13:33:36.000000 nonebot_plugin_imgexploration-0.2.4/nonebot_plugin_imgexploration.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-13 13:33:36.000000 nonebot_plugin_imgexploration-0.2.4/nonebot_plugin_imgexploration.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      178 2023-02-13 13:33:36.000000 nonebot_plugin_imgexploration-0.2.4/nonebot_plugin_imgexploration.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2023-02-13 13:33:36.000000 nonebot_plugin_imgexploration-0.2.4/nonebot_plugin_imgexploration.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      491 2023-02-13 13:33:30.000000 nonebot_plugin_imgexploration-0.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-13 13:33:37.029155 nonebot_plugin_imgexploration-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1911 2023-02-13 13:33:27.000000 nonebot_plugin_imgexploration-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 14:37:06.777393 nonebot-plugin-imgexploration-0.2.5/
+-rw-rw-rw-   0        0        0     1088 2023-05-18 14:00:48.000000 nonebot-plugin-imgexploration-0.2.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      166 2023-05-18 14:00:48.000000 nonebot-plugin-imgexploration-0.2.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     2777 2023-05-18 14:37:06.777393 nonebot-plugin-imgexploration-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2024 2023-05-18 14:00:48.000000 nonebot-plugin-imgexploration-0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 14:37:06.767983 nonebot-plugin-imgexploration-0.2.5/nonebot_plugin_imgexploration/
+-rw-rw-rw-   0        0        0     4082 2023-05-18 14:00:48.000000 nonebot-plugin-imgexploration-0.2.5/nonebot_plugin_imgexploration/__init__.py
+-rw-rw-rw-   0        0        0    22358 2023-05-18 14:07:03.000000 nonebot-plugin-imgexploration-0.2.5/nonebot_plugin_imgexploration/imgexploration.py
+drwxrwxrwx   0        0        0        0 2023-05-18 14:37:06.775392 nonebot-plugin-imgexploration-0.2.5/nonebot_plugin_imgexploration.egg-info/
+-rw-rw-rw-   0        0        0     2777 2023-05-18 14:37:06.000000 nonebot-plugin-imgexploration-0.2.5/nonebot_plugin_imgexploration.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      421 2023-05-18 14:37:06.000000 nonebot-plugin-imgexploration-0.2.5/nonebot_plugin_imgexploration.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 14:37:06.000000 nonebot-plugin-imgexploration-0.2.5/nonebot_plugin_imgexploration.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       99 2023-05-18 14:37:06.000000 nonebot-plugin-imgexploration-0.2.5/nonebot_plugin_imgexploration.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2023-05-18 14:37:06.000000 nonebot-plugin-imgexploration-0.2.5/nonebot_plugin_imgexploration.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      491 2023-05-18 14:36:30.000000 nonebot-plugin-imgexploration-0.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0      146 2023-05-18 14:37:06.778395 nonebot-plugin-imgexploration-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     8571 2023-05-18 14:20:37.000000 nonebot-plugin-imgexploration-0.2.5/setup.py
```

### Comparing `nonebot_plugin_imgexploration-0.2.4/LICENSE.txt` & `nonebot-plugin-imgexploration-0.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_imgexploration-0.2.4/PKG-INFO` & `nonebot-plugin-imgexploration-0.2.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
-Name: nonebot_plugin_imgexploration
-Version: 0.2.4
-Summary: Google、Yandx和基于PicImageSearch的saucenao、ascii2d搜图
+Name: nonebot-plugin-imgexploration
+Version: 0.2.5
+Summary: Nonebot2 插件，Google、Yandx和基于PicImageSearch的saucenao、ascii2d搜图
 Home-page: https://github.com/cpuopt/nonebot_plugin_imgexploration
 Author: cpufan
-Author-email: 554950835@qq.com
-Keywords: ssh linux
+Author-email: cpufan2001@gmail.com
+Keywords: nonebot nonebot-plugin imagesearch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 <div align="center">
 <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
 
@@ -23,15 +23,15 @@
 
 _✨ [Nonebot2](https://github.com/nonebot/nonebot2) 插件，Google、Yandx和基于PicImageSearch的saucenao、ascii2d搜图  ✨_
 
 
 
 </div> 
 
-需要能稳定访问Google等网站的代理  
+**需要能稳定访问Google等网站的代理**  
 ## 一.**安装**
 ### 1.使用nb-cli安装
 依次执行
 ```
 nb plugin install nonebot_plugin_guild_patch
 ```
 ```
@@ -64,19 +64,22 @@
 nonebot.load_plugin('nonebot_plugin_guild_patch')
 ```
 </details>
 
 ## 二.**配置**  
 ### 1.env中的配置
 ```
-proxy_port=xxxx  #代理端口号(不使用本地代理可缺省)
+#代理端口号(不使用本地代理可缺省，例如：使用软路由透明代理、程序运行在境外)
+proxy_port=xxxx  
 
-saucenao_apikey=xxxxx  #saucenao apikey 在https://saucenao.com/user.php?page=search-api注册获取
+#saucenao apikey 在https://saucenao.com/user.php?page=search-api注册获取
+saucenao_apikey=xxxxx 
 
-SESSION_EXPIRE_TIMEOUT=180 #等待用户回复的超时时间(可选) https://v2.nonebot.dev/docs/api/config#Config-session_expire_timeout
+#等待用户回复的超时时间(可选) https://v2.nonebot.dev/docs/api/config#Config-session_expire_timeout
+SESSION_EXPIRE_TIMEOUT=180 
 ```  
 ## 三.**使用**  
 ### 
 ```
 /搜图
 /搜图 <图片>
 ```
```

#### html2text {}

```diff
@@ -1,33 +1,36 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_imgexploration Version: 0.2.4
-Summary: GoogleãYandxååºäºPicImageSearchçsaucenaoãascii2dæå¾ Home-
+Metadata-Version: 2.1 Name: nonebot-plugin-imgexploration Version: 0.2.5
+Summary: Nonebot2
+æä»¶ï¼GoogleãYandxååºäºPicImageSearchçsaucenaoãascii2dæå¾ Home-
 page: https://github.com/cpuopt/nonebot_plugin_imgexploration Author: cpufan
-Author-email: 554950835@qq.com Keywords: ssh linux Classifier: Development
-Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
-Topic :: Software Development :: Build Tools Classifier: License :: OSI
-Approved :: MIT License Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python Description-Content-Type: text/markdown License-File:
-LICENSE.txt
+Author-email: cpufan2001@gmail.com Keywords: nonebot nonebot-plugin imagesearch
+Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
+Developers Classifier: Topic :: Software Development :: Build Tools Classifier:
+License :: OSI Approved :: MIT License Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python Description-Content-Type: text/markdown License-
+File: LICENSE.txt
  [nonebot] # nonebot_plugin_imgexploration _â¨ [Nonebot2](https://github.com/
                                nonebot/nonebot2)
 æä»¶ï¼GoogleãYandxååºäºPicImageSearchçsaucenaoãascii2dæå¾ â¨_
-éè¦è½ç¨³å®è®¿é®Googleç­ç½ç«çä»£ç ## ä¸.**å®è£** ### 1.ä½¿ç¨nb-
-cliå®è£ ä¾æ¬¡æ§è¡ ``` nb plugin install nonebot_plugin_guild_patch ``` ```
-nb plugin install nonebot-plugin-imgexploration ``` æå¶ä»ä»»æå è½½æ¹å¼
-### 2.éè¦å­ä½ ``` HarmonyOS_Sans_SC_Regular.ttf HarmonyOS_Sans_SC_Bold.ttf
+**éè¦è½ç¨³å®è®¿é®Googleç­ç½ç«çä»£ç** ## ä¸.**å®è£** ###
+1.ä½¿ç¨nb-cliå®è£ ä¾æ¬¡æ§è¡ ``` nb plugin install
+nonebot_plugin_guild_patch ``` ``` nb plugin install nonebot-plugin-
+imgexploration ``` æå¶ä»ä»»æå è½½æ¹å¼ ### 2.éè¦å­ä½ ```
+HarmonyOS_Sans_SC_Regular.ttf HarmonyOS_Sans_SC_Bold.ttf
 HarmonyOS_Sans_SC_Light.ttf ``` https://developer.harmonyos.com/cn/docs/design/
 des-guides/font-0000001157868583 å®è£å°ç³»ç»å­ä½å³å¯ ### 3.ä¾èµ (nb-
 cliæpipå®è£æ ééç½®ä¾èµ)  å±å¼/æ¶èµ· ``` pip install -
 r requirements.txt ``` go-cqhttp é¢éæ¯æééè¡¥ä¸`nonebot-plugin-guild-
 patch` ``` pip install nonebot-plugin-guild-patch ```
 å¨å è½½æ¬æä»¶åæ·»å  ``` nonebot.load_plugin
 ('nonebot_plugin_guild_patch') ```  ## äº.**éç½®** ### 1.envä¸­çéç½® ```
-proxy_port=xxxx #ä»£çç«¯å£å·(ä¸ä½¿ç¨æ¬å°ä»£çå¯ç¼ºç)
-saucenao_apikey=xxxxx #saucenao apikey å¨https://saucenao.com/
-user.php?page=search-apiæ³¨åè·å SESSION_EXPIRE_TIMEOUT=180
-#ç­å¾ç¨æ·åå¤çè¶æ¶æ¶é´(å¯é) https://v2.nonebot.dev/docs/api/
-config#Config-session_expire_timeout ``` ## ä¸.**ä½¿ç¨** ### ``` /æå¾ /
-æå¾ <å¾ç> ``` ### **ä½¿ç¨ç¤ºä¾**
+#ä»£çç«¯å£å·
+(ä¸ä½¿ç¨æ¬å°ä»£çå¯ç¼ºçï¼ä¾å¦ï¼ä½¿ç¨è½¯è·¯ç±éæä»£çãç¨åºè¿è¡å¨å¢å¤)
+proxy_port=xxxx #saucenao apikey å¨https://saucenao.com/user.php?page=search-
+apiæ³¨åè·å saucenao_apikey=xxxxx #ç­å¾ç¨æ·åå¤çè¶æ¶æ¶é´
+(å¯é) https://v2.nonebot.dev/docs/api/config#Config-session_expire_timeout
+SESSION_EXPIRE_TIMEOUT=180 ``` ## ä¸.**ä½¿ç¨** ### ``` /æå¾ /æå¾
+<å¾ç> ``` ### **ä½¿ç¨ç¤ºä¾**
                [https://p.inari.site/usr/369/63b6cfe0cd8a8.jpg]
 ### æå¾ç»æ
                [https://p.inari.site/usr/369/63b6cd6f24abc.jpg]
```

### Comparing `nonebot_plugin_imgexploration-0.2.4/README.md` & `nonebot-plugin-imgexploration-0.2.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 _✨ [Nonebot2](https://github.com/nonebot/nonebot2) 插件，Google、Yandx和基于PicImageSearch的saucenao、ascii2d搜图  ✨_
 
 
 
 </div> 
 
-需要能稳定访问Google等网站的代理  
+**需要能稳定访问Google等网站的代理**  
 ## 一.**安装**
 ### 1.使用nb-cli安装
 依次执行
 ```
 nb plugin install nonebot_plugin_guild_patch
 ```
 ```
@@ -46,19 +46,22 @@
 nonebot.load_plugin('nonebot_plugin_guild_patch')
 ```
 </details>
 
 ## 二.**配置**  
 ### 1.env中的配置
 ```
-proxy_port=xxxx  #代理端口号(不使用本地代理可缺省)
+#代理端口号(不使用本地代理可缺省，例如：使用软路由透明代理、程序运行在境外)
+proxy_port=xxxx  
 
-saucenao_apikey=xxxxx  #saucenao apikey 在https://saucenao.com/user.php?page=search-api注册获取
+#saucenao apikey 在https://saucenao.com/user.php?page=search-api注册获取
+saucenao_apikey=xxxxx 
 
-SESSION_EXPIRE_TIMEOUT=180 #等待用户回复的超时时间(可选) https://v2.nonebot.dev/docs/api/config#Config-session_expire_timeout
+#等待用户回复的超时时间(可选) https://v2.nonebot.dev/docs/api/config#Config-session_expire_timeout
+SESSION_EXPIRE_TIMEOUT=180 
 ```  
 ## 三.**使用**  
 ### 
 ```
 /搜图
 /搜图 <图片>
 ```  
@@ -68,8 +71,8 @@
     <img decoding="async" align="middle" src="https://p.inari.site/usr/369/63b6cfe0cd8a8.jpg" width="80%">
 </div>
 
 ### 搜图结果
 
 <div align=center>
     <img decoding="async" align="middle" src="https://p.inari.site/usr/369/63b6cd6f24abc.jpg" height="1280px">
-</div>
+</div>
```

#### html2text {}

```diff
@@ -1,23 +1,25 @@
  [nonebot] # nonebot_plugin_imgexploration _â¨ [Nonebot2](https://github.com/
                                nonebot/nonebot2)
 æä»¶ï¼GoogleãYandxååºäºPicImageSearchçsaucenaoãascii2dæå¾ â¨_
-éè¦è½ç¨³å®è®¿é®Googleç­ç½ç«çä»£ç ## ä¸.**å®è£** ### 1.ä½¿ç¨nb-
-cliå®è£ ä¾æ¬¡æ§è¡ ``` nb plugin install nonebot_plugin_guild_patch ``` ```
-nb plugin install nonebot-plugin-imgexploration ``` æå¶ä»ä»»æå è½½æ¹å¼
-### 2.éè¦å­ä½ ``` HarmonyOS_Sans_SC_Regular.ttf HarmonyOS_Sans_SC_Bold.ttf
+**éè¦è½ç¨³å®è®¿é®Googleç­ç½ç«çä»£ç** ## ä¸.**å®è£** ###
+1.ä½¿ç¨nb-cliå®è£ ä¾æ¬¡æ§è¡ ``` nb plugin install
+nonebot_plugin_guild_patch ``` ``` nb plugin install nonebot-plugin-
+imgexploration ``` æå¶ä»ä»»æå è½½æ¹å¼ ### 2.éè¦å­ä½ ```
+HarmonyOS_Sans_SC_Regular.ttf HarmonyOS_Sans_SC_Bold.ttf
 HarmonyOS_Sans_SC_Light.ttf ``` https://developer.harmonyos.com/cn/docs/design/
 des-guides/font-0000001157868583 å®è£å°ç³»ç»å­ä½å³å¯ ### 3.ä¾èµ (nb-
 cliæpipå®è£æ ééç½®ä¾èµ)  å±å¼/æ¶èµ· ``` pip install -
 r requirements.txt ``` go-cqhttp é¢éæ¯æééè¡¥ä¸`nonebot-plugin-guild-
 patch` ``` pip install nonebot-plugin-guild-patch ```
 å¨å è½½æ¬æä»¶åæ·»å  ``` nonebot.load_plugin
 ('nonebot_plugin_guild_patch') ```  ## äº.**éç½®** ### 1.envä¸­çéç½® ```
-proxy_port=xxxx #ä»£çç«¯å£å·(ä¸ä½¿ç¨æ¬å°ä»£çå¯ç¼ºç)
-saucenao_apikey=xxxxx #saucenao apikey å¨https://saucenao.com/
-user.php?page=search-apiæ³¨åè·å SESSION_EXPIRE_TIMEOUT=180
-#ç­å¾ç¨æ·åå¤çè¶æ¶æ¶é´(å¯é) https://v2.nonebot.dev/docs/api/
-config#Config-session_expire_timeout ``` ## ä¸.**ä½¿ç¨** ### ``` /æå¾ /
-æå¾ <å¾ç> ``` ### **ä½¿ç¨ç¤ºä¾**
+#ä»£çç«¯å£å·
+(ä¸ä½¿ç¨æ¬å°ä»£çå¯ç¼ºçï¼ä¾å¦ï¼ä½¿ç¨è½¯è·¯ç±éæä»£çãç¨åºè¿è¡å¨å¢å¤)
+proxy_port=xxxx #saucenao apikey å¨https://saucenao.com/user.php?page=search-
+apiæ³¨åè·å saucenao_apikey=xxxxx #ç­å¾ç¨æ·åå¤çè¶æ¶æ¶é´
+(å¯é) https://v2.nonebot.dev/docs/api/config#Config-session_expire_timeout
+SESSION_EXPIRE_TIMEOUT=180 ``` ## ä¸.**ä½¿ç¨** ### ``` /æå¾ /æå¾
+<å¾ç> ``` ### **ä½¿ç¨ç¤ºä¾**
                [https://p.inari.site/usr/369/63b6cfe0cd8a8.jpg]
 ### æå¾ç»æ
                [https://p.inari.site/usr/369/63b6cd6f24abc.jpg]
```

### Comparing `nonebot_plugin_imgexploration-0.2.4/nonebot_plugin_imgexploration/__init__.py` & `nonebot-plugin-imgexploration-0.2.5/nonebot_plugin_imgexploration/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_imgexploration-0.2.4/nonebot_plugin_imgexploration/imgexploration.py` & `nonebot-plugin-imgexploration-0.2.5/nonebot_plugin_imgexploration/imgexploration.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import asyncio
-import base64
 import re
 from PIL import Image, ImageDraw, ImageFont, ImageFilter
 from PicImageSearch import Ascii2D, Network, SauceNAO
 from lxml import etree
 import httpx, json
 from io import BytesIO
 from loguru import logger
@@ -221,79 +220,105 @@
         except IndexError as e:
             logger.error(e)
             return []
         finally:
             logger.success(f"saucenao result:{len(resList)}")
             return resList
 
-    async def __google_build_result(self, result_num=3) -> dict:
+    async def __google_build_result(self, result_num=5) -> dict:
         google_header = {
-            "referer": "https://lens.google.com/",
-            "sec-ch-ua": '"Chromium";v="106", "Google Chrome";v="106", "Not;A=Brand";v="99"',
-            "sec-ch-ua-mobile": "?0",
-            "sec-ch-ua-platform": '"Windows"',
-            "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/106.0.0.0 Safari/537.36",
-            "accept-language": "zh-CN,zh;q=0.9",
+            "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
+            "Accept-Encoding": "gzip, deflate, br",
+            "Accept-Language": "zh-CN,zh;q=0.9",
+            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36",
+            "Cookie": "HSID=AN1NB4ajlQr5qei6f; SSID=ALaw3m9KIVaJjFK9y; APISID=vIbKriTWaSAod2_u/Ay7WaK0LBSW17bpOG; SAPISID=lunaAAzV5yGLTyHi/Axv3LgL-wrjG4nfsu; __Secure-1PAPISID=lunaAAzV5yGLTyHi/Axv3LgL-wrjG4nfsu; __Secure-3PAPISID=lunaAAzV5yGLTyHi/Axv3LgL-wrjG4nfsu; __Secure-ENID=12.SE=RnUkgdkHmJcPpt55puSILcbqdy_gzbHm7glrHHTBTN9YZkji1c494qZ2FaLt0KQVJ-Cfw7hhoTKYGAAzoc45BlLy_5P2qIIKgKRn_dxtXqXFuDsA50JKx22WwSQfzU0eFB4m4bppPvZ-vbTDXpnjXkCeGd_lfNPxlxCZaiIho2EGSSw-BcoMGP74E4m_G7ua4-l1WHyS6Y3wvTOA-bcDeJ6kwZOqX2-8f5vnA_kNEhIuOKpCw8VkRqga5yspgoYhBtbGzOuYToovf2rMDFs; SID=WggP8LizO7-VBAyCCeGRBcHrg45CcdNJRi3TThWlbExDGQwxsmNkXG9V-Kw0YnWvTLIRtw.; __Secure-1PSID=WggP8LizO7-VBAyCCeGRBcHrg45CcdNJRi3TThWlbExDGQwxb1PICWUK5PKQv1wyZi9gwA.; __Secure-3PSID=WggP8LizO7-VBAyCCeGRBcHrg45CcdNJRi3TThWlbExDGQwxxh89XT_3pJD36RKjz_iujw.; SEARCH_SAMESITE=CgQIopgB; OSID=WggP8Bs6BfB-E67o2EYB9qSl9l2nvnkwrbuP48OchHo7ef4VegwgPP56cu6wMrFPCVwZog.; __Secure-OSID=WggP8Bs6BfB-E67o2EYB9qSl9l2nvnkwrbuP48OchHo7ef4VXRVVAjRSHJlfXqR1OJ369g.; OTZ=7027999_24_24__24_; AEC=AUEFqZcfy6MGqG23vJKNkIagdtWH7erOX_7NH2i_yLiHkJ1cByzFFdelyjk; NID=511=WBV32XnmKFPJ7wx2TvFd5eeT6Y0LBXYmjHIPjWxObQZv0pVJS6067Lf-gyhphBlCT_X2x9jSE-IDwbm2YbHBsXp9b5S6M6rwW3_TR_JVXGqNRCZViN_bSxZcieEYi_RzKJdiXA_PRo7taBbA7VSKUwjU24zvtg7d_b-Tls-ukEkKXwsEQkeBK7PDWSqH9JlyHsXF6WFGGJhkTgcy7iYM3rmB3WJjufftrFz0Umf3i1rHMsoUAbwpoliw-N-BnSD2v6PLMNTfuXBXqzXjVenWq7muycI1C--4b6O6MvBlAUAlFzjGAYbP; __Secure-1PSIDTS=sidts-CjIBLFra0lu7QUEJ6z4bktjLrzH_to8utCsrKAyVGD1G0-zW2ht-_PZxDdVIiiCAOw2J0RAA; __Secure-3PSIDTS=sidts-CjIBLFra0lu7QUEJ6z4bktjLrzH_to8utCsrKAyVGD1G0-zW2ht-_PZxDdVIiiCAOw2J0RAA; SIDCC=AP8dLtz6qzRUTAC6bSh-YVncfW0vzWyIglUq8aVnFb2M09z1WzfHZ4XfeWC6DCgCnyq8QZgjz64; __Secure-1PSIDCC=AP8dLtz0A5aNpbgGTlTGv7d1jpHbFIrjopths1OggUiXTQ3-34KF71LRud3PqIEuIQCp9yvaX0o; __Secure-3PSIDCC=AP8dLtwOb41aEvrWGAp6KnXtwz-QywAgLUDPVBtlRrR_205MjEwGDuD4ge3yn6zfoEYWMP5wIiA4; 1P_JAR=2023-05-16-12",
         }
         resList = []
         google_lens_text = ""
         google_search_text = ""
         logger.info("google searching...")
         try:
             params = {
-                "hl": "zh-CN",
-                "re": "df",
-                "ep": "gsbubu",
                 "url": self.__imgopsUrl,
             }
             google_lens_text = (await self.client.get(f"https://lens.google.com/uploadbyurl", params=params, headers=google_header, follow_redirects=True, timeout=10)).text
-            f = google_lens_text.rindex(r"https://www.google.com/search?tbs\u003dsbi:")
-            l = google_lens_text.index("]", f)
-            url = "https://www.google.com/search?tbs=sbi:" + google_lens_text[f + 43 : l - 1]
-            google_search_text = (await self.client.get(url, headers=google_header, follow_redirects=True, timeout=10)).text
-
-            google_search_html = etree.HTML(google_search_text)
-            resultDiv = google_search_html.xpath('//*[@id="rso"]/div/div/div//*[contains(text(), "包含匹配图片的页面")]/parent::div/parent::div//div[@lang]')
-
-            # 获取预览图base64
-            nonce = google_search_html.xpath("//script[@nonce]/@nonce")
-            if len(nonce) > 0:
-                nonce = nonce[0]
-            else:
-                return []
-            imgbase64s = google_search_html.xpath(f'//script[@nonce="' + nonce + '"][contains(text(),"(function(){var s=\'data:image")]/text()')
-            base64DIC = {}
-            for imgbase in imgbase64s:
-                result = re.search("data:image/.*;base64,(?P<data>.*)';var ii=(?P<attr>.*);_.*", imgbase, re.DOTALL)
-                data = result.groupdict().get("data").replace("\\x3d", "=")
-                attr = result.groupdict().get("attr")
-                attrs = json.loads(attr.replace("'", '"'))
-                for id in attrs:
-                    base64DIC[id] = data
 
-            for singleDiv in resultDiv:
+            req_tex = re.findall(r"var AF_dataServiceRequests = (.+?); var AF_initDataChunkQueue", google_lens_text)
+            if req_tex:
+                ds1 = re.findall(r"'ds:1' : (.*)}", req_tex[0])
+                if ds1:
+                    ds = ds1[0]
+                    # print(ds)
+                    ds = (
+                        ds.replace("id:", '"id":')
+                        .replace("request:", '"request":')
+                        .replace("'", '"')
+                        .replace("[4,true],null,null,[],null", 'null,null,null,[],"000000"')
+                        .replace("true", "1")
+                        .replace("false", "0")
+                        .replace("Asia/Kuching", "Asia/Hong_Kong")
+                        .replace("[5,6,7,2]", "[5,6,2]")
+                        .replace("[],[null,5],null,[5]", "[null,null],[null,5],null,[5],[]")
+                    )
+                    dic = json.loads(ds)
+                    dic["request"][1][-1].remove(1)
+                    dic["request"][-3].append(dic["request"][1])
+
+            qest = [
+                [
+                    [
+                        dic["id"],
+                        json.dumps(dic["request"]),
+                        None,
+                        "generic",
+                    ],
+                ],
+            ]
+            postDate = {"f.req": json.dumps(qest)}
+            post_headers = {
+                "Accept": "*/*",
+                "Accept-Encoding": "gzip, deflate, br",
+                "Accept-Language": "zh-CN,zh;q=0.9",
+                "Content-Type": "application/x-www-form-urlencoded;charset=UTF-8",
+                "Sec-Ch-Ua": '"Google Chrome";v="113", "Chromium";v="113", "Not-A.Brand";v="24"',
+                "Referer": "https://lens.google.com/",
+                "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36",
+            }
+            te = await self.client.post(url="https://lens.google.com/_/LensWebStandaloneUi/data/batchexecute?hl=zh-CN", data=postDate, headers=post_headers)
+
+            res_j = json.loads(te.text.replace(r")]}'", "", 1))
+            search_result = json.loads(res_j[0][2])[1][0][1][8][20][0][0]
+
+            for singleDiv in search_result[:result_num]:
                 try:
-                    thumbnail_base64 = base64DIC[singleDiv.xpath("div//img/@id")[0]] if singleDiv.xpath("div//img/@id")[0] in base64DIC.keys() else ""
                     sin_di = {
-                        "title": singleDiv.xpath("div[1]//h3/text()")[0],
-                        "thumbnail_bytes": base64.b64decode(thumbnail_base64),
-                        "url": singleDiv.xpath("div[1]/div[1]/div/a/@href")[0],
+                        "title": singleDiv[4],
+                        "thumbnail_url": singleDiv[0][0],
+                        "url": singleDiv[2][2][2],
                         "source": "Google",
+                        "domain": singleDiv[1][2],
                     }
-                except (IndexError):
+                except IndexError:
                     continue
                 resList.append(sin_di)
 
+            thumbnail_urls = [single["thumbnail_url"] for single in resList]
+            print(thumbnail_urls)
+            thumbnail_bytes = await self.ImageBatchDownload(thumbnail_urls, self.client)
+            i = 0
+            for single in resList:
+                single["thumbnail_bytes"] = thumbnail_bytes[i]
+                i += 1
             return resList
+
         except Exception as e:
             logger.error(e)
             with open("Googlelens_error_page.html", "w+", encoding="utf-8") as file:
                 file.write(google_lens_text)
-            with open("GoogleSearch_error_page.html", "w+", encoding="utf-8") as file:
-                file.write(google_search_text)
+
         finally:
             logger.success(f"google result:{len(resList)}")
             return resList
 
     def __ascii2d_get_external_url(self, rawhtml):
         rawhtml = str(rawhtml)
         external_url_li = etree.HTML(rawhtml).xpath('//div[@class="external"]/a[1]/@href')
```

### Comparing `nonebot_plugin_imgexploration-0.2.4/nonebot_plugin_imgexploration.egg-info/PKG-INFO` & `nonebot-plugin-imgexploration-0.2.5/nonebot_plugin_imgexploration.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-imgexploration
-Version: 0.2.4
-Summary: Google、Yandx和基于PicImageSearch的saucenao、ascii2d搜图
+Version: 0.2.5
+Summary: Nonebot2 插件，Google、Yandx和基于PicImageSearch的saucenao、ascii2d搜图
 Home-page: https://github.com/cpuopt/nonebot_plugin_imgexploration
 Author: cpufan
-Author-email: 554950835@qq.com
-Keywords: ssh linux
+Author-email: cpufan2001@gmail.com
+Keywords: nonebot nonebot-plugin imagesearch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 <div align="center">
 <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
 
@@ -23,15 +23,15 @@
 
 _✨ [Nonebot2](https://github.com/nonebot/nonebot2) 插件，Google、Yandx和基于PicImageSearch的saucenao、ascii2d搜图  ✨_
 
 
 
 </div> 
 
-需要能稳定访问Google等网站的代理  
+**需要能稳定访问Google等网站的代理**  
 ## 一.**安装**
 ### 1.使用nb-cli安装
 依次执行
 ```
 nb plugin install nonebot_plugin_guild_patch
 ```
 ```
@@ -64,19 +64,22 @@
 nonebot.load_plugin('nonebot_plugin_guild_patch')
 ```
 </details>
 
 ## 二.**配置**  
 ### 1.env中的配置
 ```
-proxy_port=xxxx  #代理端口号(不使用本地代理可缺省)
+#代理端口号(不使用本地代理可缺省，例如：使用软路由透明代理、程序运行在境外)
+proxy_port=xxxx  
 
-saucenao_apikey=xxxxx  #saucenao apikey 在https://saucenao.com/user.php?page=search-api注册获取
+#saucenao apikey 在https://saucenao.com/user.php?page=search-api注册获取
+saucenao_apikey=xxxxx 
 
-SESSION_EXPIRE_TIMEOUT=180 #等待用户回复的超时时间(可选) https://v2.nonebot.dev/docs/api/config#Config-session_expire_timeout
+#等待用户回复的超时时间(可选) https://v2.nonebot.dev/docs/api/config#Config-session_expire_timeout
+SESSION_EXPIRE_TIMEOUT=180 
 ```  
 ## 三.**使用**  
 ### 
 ```
 /搜图
 /搜图 <图片>
 ```
```

#### html2text {}

```diff
@@ -1,33 +1,36 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-imgexploration Version: 0.2.4
-Summary: GoogleãYandxååºäºPicImageSearchçsaucenaoãascii2dæå¾ Home-
+Metadata-Version: 2.1 Name: nonebot-plugin-imgexploration Version: 0.2.5
+Summary: Nonebot2
+æä»¶ï¼GoogleãYandxååºäºPicImageSearchçsaucenaoãascii2dæå¾ Home-
 page: https://github.com/cpuopt/nonebot_plugin_imgexploration Author: cpufan
-Author-email: 554950835@qq.com Keywords: ssh linux Classifier: Development
-Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
-Topic :: Software Development :: Build Tools Classifier: License :: OSI
-Approved :: MIT License Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python Description-Content-Type: text/markdown License-File:
-LICENSE.txt
+Author-email: cpufan2001@gmail.com Keywords: nonebot nonebot-plugin imagesearch
+Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
+Developers Classifier: Topic :: Software Development :: Build Tools Classifier:
+License :: OSI Approved :: MIT License Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python Description-Content-Type: text/markdown License-
+File: LICENSE.txt
  [nonebot] # nonebot_plugin_imgexploration _â¨ [Nonebot2](https://github.com/
                                nonebot/nonebot2)
 æä»¶ï¼GoogleãYandxååºäºPicImageSearchçsaucenaoãascii2dæå¾ â¨_
-éè¦è½ç¨³å®è®¿é®Googleç­ç½ç«çä»£ç ## ä¸.**å®è£** ### 1.ä½¿ç¨nb-
-cliå®è£ ä¾æ¬¡æ§è¡ ``` nb plugin install nonebot_plugin_guild_patch ``` ```
-nb plugin install nonebot-plugin-imgexploration ``` æå¶ä»ä»»æå è½½æ¹å¼
-### 2.éè¦å­ä½ ``` HarmonyOS_Sans_SC_Regular.ttf HarmonyOS_Sans_SC_Bold.ttf
+**éè¦è½ç¨³å®è®¿é®Googleç­ç½ç«çä»£ç** ## ä¸.**å®è£** ###
+1.ä½¿ç¨nb-cliå®è£ ä¾æ¬¡æ§è¡ ``` nb plugin install
+nonebot_plugin_guild_patch ``` ``` nb plugin install nonebot-plugin-
+imgexploration ``` æå¶ä»ä»»æå è½½æ¹å¼ ### 2.éè¦å­ä½ ```
+HarmonyOS_Sans_SC_Regular.ttf HarmonyOS_Sans_SC_Bold.ttf
 HarmonyOS_Sans_SC_Light.ttf ``` https://developer.harmonyos.com/cn/docs/design/
 des-guides/font-0000001157868583 å®è£å°ç³»ç»å­ä½å³å¯ ### 3.ä¾èµ (nb-
 cliæpipå®è£æ ééç½®ä¾èµ)  å±å¼/æ¶èµ· ``` pip install -
 r requirements.txt ``` go-cqhttp é¢éæ¯æééè¡¥ä¸`nonebot-plugin-guild-
 patch` ``` pip install nonebot-plugin-guild-patch ```
 å¨å è½½æ¬æä»¶åæ·»å  ``` nonebot.load_plugin
 ('nonebot_plugin_guild_patch') ```  ## äº.**éç½®** ### 1.envä¸­çéç½® ```
-proxy_port=xxxx #ä»£çç«¯å£å·(ä¸ä½¿ç¨æ¬å°ä»£çå¯ç¼ºç)
-saucenao_apikey=xxxxx #saucenao apikey å¨https://saucenao.com/
-user.php?page=search-apiæ³¨åè·å SESSION_EXPIRE_TIMEOUT=180
-#ç­å¾ç¨æ·åå¤çè¶æ¶æ¶é´(å¯é) https://v2.nonebot.dev/docs/api/
-config#Config-session_expire_timeout ``` ## ä¸.**ä½¿ç¨** ### ``` /æå¾ /
-æå¾ <å¾ç> ``` ### **ä½¿ç¨ç¤ºä¾**
+#ä»£çç«¯å£å·
+(ä¸ä½¿ç¨æ¬å°ä»£çå¯ç¼ºçï¼ä¾å¦ï¼ä½¿ç¨è½¯è·¯ç±éæä»£çãç¨åºè¿è¡å¨å¢å¤)
+proxy_port=xxxx #saucenao apikey å¨https://saucenao.com/user.php?page=search-
+apiæ³¨åè·å saucenao_apikey=xxxxx #ç­å¾ç¨æ·åå¤çè¶æ¶æ¶é´
+(å¯é) https://v2.nonebot.dev/docs/api/config#Config-session_expire_timeout
+SESSION_EXPIRE_TIMEOUT=180 ``` ## ä¸.**ä½¿ç¨** ### ``` /æå¾ /æå¾
+<å¾ç> ``` ### **ä½¿ç¨ç¤ºä¾**
                [https://p.inari.site/usr/369/63b6cfe0cd8a8.jpg]
 ### æå¾ç»æ
                [https://p.inari.site/usr/369/63b6cd6f24abc.jpg]
```

