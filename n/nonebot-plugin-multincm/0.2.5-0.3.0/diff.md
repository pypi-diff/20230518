# Comparing `tmp/nonebot_plugin_multincm-0.2.5.tar.gz` & `tmp/nonebot_plugin_multincm-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_multincm-0.2.5.tar", last modified: Wed May 17 19:27:49 2023, max compression
+gzip compressed data, was "nonebot_plugin_multincm-0.3.0.tar", last modified: Thu May 18 20:07:18 2023, max compression
```

## Comparing `nonebot_plugin_multincm-0.2.5.tar` & `nonebot_plugin_multincm-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1069 2023-05-17 19:27:36.549958 nonebot_plugin_multincm-0.2.5/LICENSE
--rw-r--r--   0        0        0     6066 2023-05-17 19:27:36.549958 nonebot_plugin_multincm-0.2.5/README.md
--rw-r--r--   0        0        0     1248 2023-05-17 19:27:36.549958 nonebot_plugin_multincm-0.2.5/nonebot_plugin_multincm/__init__.py
--rw-r--r--   0        0        0     8572 2023-05-17 19:27:36.549958 nonebot_plugin_multincm-0.2.5/nonebot_plugin_multincm/__main__.py
--rw-r--r--   0        0        0      512 2023-05-17 19:27:36.553958 nonebot_plugin_multincm-0.2.5/nonebot_plugin_multincm/config.py
--rw-r--r--   0        0        0      134 2023-05-17 19:27:36.553958 nonebot_plugin_multincm-0.2.5/nonebot_plugin_multincm/const.py
--rw-r--r--   0        0        0     4457 2023-05-17 19:27:36.553958 nonebot_plugin_multincm-0.2.5/nonebot_plugin_multincm/data_source.py
--rw-r--r--   0        0        0    10221 2023-05-17 19:27:36.553958 nonebot_plugin_multincm-0.2.5/nonebot_plugin_multincm/draw.py
--rw-r--r--   0        0        0     2957 2023-05-17 19:27:36.553958 nonebot_plugin_multincm-0.2.5/nonebot_plugin_multincm/lrc_parser.py
--rw-r--r--   0        0        0     2143 2023-05-17 19:27:36.553958 nonebot_plugin_multincm-0.2.5/nonebot_plugin_multincm/msg_cache.py
--rw-r--r--   0        0        0   212591 2023-05-17 19:27:36.553958 nonebot_plugin_multincm-0.2.5/nonebot_plugin_multincm/res/bg.jpg
--rw-r--r--   0        0        0     1688 2023-05-17 19:27:36.553958 nonebot_plugin_multincm-0.2.5/nonebot_plugin_multincm/types.py
--rw-r--r--   0        0        0      851 2023-05-17 19:27:36.553958 nonebot_plugin_multincm-0.2.5/nonebot_plugin_multincm/utils.py
--rw-r--r--   0        0        0      867 2023-05-17 19:27:49.437802 nonebot_plugin_multincm-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     7016 1970-01-01 00:00:00.000000 nonebot_plugin_multincm-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-18 20:07:05.007333 nonebot_plugin_multincm-0.3.0/LICENSE
+-rw-r--r--   0        0        0     7087 2023-05-18 20:07:05.007333 nonebot_plugin_multincm-0.3.0/README.md
+-rw-r--r--   0        0        0     1646 2023-05-18 20:07:05.007333 nonebot_plugin_multincm-0.3.0/nonebot_plugin_multincm/__init__.py
+-rw-r--r--   0        0        0    11595 2023-05-18 20:07:05.007333 nonebot_plugin_multincm-0.3.0/nonebot_plugin_multincm/__main__.py
+-rw-r--r--   0        0        0      512 2023-05-18 20:07:05.007333 nonebot_plugin_multincm-0.3.0/nonebot_plugin_multincm/config.py
+-rw-r--r--   0        0        0      134 2023-05-18 20:07:05.007333 nonebot_plugin_multincm-0.3.0/nonebot_plugin_multincm/const.py
+-rw-r--r--   0        0        0     5500 2023-05-18 20:07:05.007333 nonebot_plugin_multincm-0.3.0/nonebot_plugin_multincm/data_source.py
+-rw-r--r--   0        0        0    11617 2023-05-18 20:07:05.007333 nonebot_plugin_multincm-0.3.0/nonebot_plugin_multincm/draw.py
+-rw-r--r--   0        0        0     2957 2023-05-18 20:07:05.007333 nonebot_plugin_multincm-0.3.0/nonebot_plugin_multincm/lrc_parser.py
+-rw-r--r--   0        0        0     2228 2023-05-18 20:07:05.007333 nonebot_plugin_multincm-0.3.0/nonebot_plugin_multincm/msg_cache.py
+-rw-r--r--   0        0        0   212591 2023-05-18 20:07:05.007333 nonebot_plugin_multincm-0.3.0/nonebot_plugin_multincm/res/bg.jpg
+-rw-r--r--   0        0        0     2997 2023-05-18 20:07:05.007333 nonebot_plugin_multincm-0.3.0/nonebot_plugin_multincm/types.py
+-rw-r--r--   0        0        0      851 2023-05-18 20:07:05.007333 nonebot_plugin_multincm-0.3.0/nonebot_plugin_multincm/utils.py
+-rw-r--r--   0        0        0      867 2023-05-18 20:07:18.899345 nonebot_plugin_multincm-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     8037 1970-01-01 00:00:00.000000 nonebot_plugin_multincm-0.3.0/PKG-INFO
```

### Comparing `nonebot_plugin_multincm-0.2.5/LICENSE` & `nonebot_plugin_multincm-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.2.5/README.md` & `nonebot_plugin_multincm-0.3.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 <p>
   <img src="https://raw.githubusercontent.com/A-kirami/nonebot-plugin-template/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText">
 </p>
 
 # NoneBot-Plugin-MultiNCM
 
-_✨ NoneBot 插件简单描述 ✨_
+_✨ 网易云多选点歌 ✨_
 
 <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 <a href="https://pdm.fming.dev">
   <img src="https://img.shields.io/badge/pdm-managed-blueviolet" alt="pdm-managed">
 </a>
 <a href="https://wakatime.com/badge/user/b61b0f9a-f40b-4c82-bc51-0a75c67bfccf/project/f4778875-45a4-4688-8e1b-b8c844440abb">
   <img src="https://wakatime.com/badge/user/b61b0f9a-f40b-4c82-bc51-0a75c67bfccf/project/f4778875-45a4-4688-8e1b-b8c844440abb.svg" alt="wakatime">
@@ -36,18 +36,37 @@
 
 </div>
 
 ## 📖 介绍
 
 一个网易云多选点歌插件，可以翻页，可以登录网易云账号点 vip 歌曲听（插件发送的是自定义音乐卡片），没了
 
-### 歌曲列表效果图
+### 效果图
+
+<details>
+<summary>歌曲列表效果图（点击展开）</summary>
 
 ![pic](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/multincm/QQ图片20230515025601.jpg)
 
+</details>
+
+<details>
+<summary>电台列表效果图（点击展开）</summary>
+
+![pic](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/multincm/QQ图片20230519034438.jpg)
+
+</details>
+
+<details>
+<summary>歌词效果图（点击展开）</summary>
+
+![pic](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/multincm/QQ图片20230519034757.png)
+
+</details>
+
 ## 💿 安装
 
 以下提到的方法 任选**其一** 即可
 
 <details open>
 <summary>[推荐] 使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
@@ -128,39 +147,51 @@
 | `NCM_MAX_ARTIST_LEN` |  否  | `400`  | 歌曲列表中歌手列的最大文本宽度（像素）  |
 
 ## 🎉 使用
 
 ### 指令
 
 - 点歌 [歌曲名 / 音乐 ID]
-  - 介绍：顾名思义。当输入音乐 ID 时会直接发送对应音乐
+  - 介绍：搜索歌曲。当输入音乐 ID 时会直接发送对应音乐
   - 别名：`网易云`、`wyy`
-- 解析 <回复 音乐卡片 / 链接>
-  - 介绍：获取该音乐的播放链接并使用自定义卡片发送
+- 电台 [歌曲名 / 节目 ID]
+  - 介绍：搜索电台节目。当输入电台 ID 时会直接发送对应节目
+  - 别名：`声音`、`网易电台`、`wtdt`、`wydj`
+- 解析 [回复 音乐卡片 / 链接]
+  - 介绍：获取该 音乐 / 电台节目 的播放链接并使用自定义卡片发送
   - 别名：`resolve`、`parse`、`get`
-- 歌词 <回复 音乐卡片 / 链接>
+- 歌词 [回复 音乐卡片 / 链接]
   - 介绍：获取该音乐的歌词，以图片形式发送
   - 别名：`lrc`、`lyric`、`lyrics`
-- 链接 <回复 音乐卡片>
-  - 介绍：获取 Bot 发送的音乐卡片的网易云歌曲链接
-  - 别名：`link`
+- 链接 [回复 音乐卡片]
+  - 介绍：获取 Bot 发送的音乐卡片的网易云链接
+  - 别名：`link`、`url`
 
 ### Tip
 
 - 点击 Bot 发送的音乐卡片会跳转到音乐直链，可以直接下载
+- 使用需要回复音乐卡片的指令时，如果没有回复，会自动使用你触发发送的最近一个音乐卡片的信息
 
 ## 📞 联系
 
 QQ：3076823485  
 Telegram：[@lgc2333](https://t.me/lgc2333)  
 吹水群：[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp)  
 邮箱：<lgc2333@126.com>
 
 ## 💡 鸣谢
 
+### [mos9527/pyncm](https://github.com/mos9527/pyncm)
+
+项目使用的网易云 API 调用库
+
+### [Binaryify/NeteaseCloudMusicApi](https://github.com/Binaryify/NeteaseCloudMusicApi)
+
+项目电台相关 API 来源
+
 ### [MeetWq/pil-utils](https://github.com/MeetWq/pil-utils)
 
 超好用的 Pillow 辅助库
 
 ## 💰 赞助
 
 感谢大家的赞助！你们的赞助将是我继续创作的动力！
@@ -171,14 +202,18 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.3.0
+
+- 支持电台节目的解析与点播
+
 ### 0.2.5
 
 - `解析`、`歌词`、`链接` 指令可以直接根据 Bot 发送的上个音乐卡片作出回应了
 - 歌词解析会合并多行空行和去掉首尾空行了
 - 现在插件会定时清理自身内存中的缓存了
 
 ### 0.2.4
```

#### html2text {}

```diff
@@ -1,25 +1,30 @@
                               [NoneBotPluginLogo]
                               [NoneBotPluginText]
- # NoneBot-Plugin-MultiNCM _â¨ NoneBot æä»¶ç®åæè¿° â¨_ [python] [pdm-
+   # NoneBot-Plugin-MultiNCM _â¨ ç½æäºå¤éç¹æ­ â¨_ [python] [pdm-
                              managed] [wakatime]
                        [license] [pypi] [pypi_download]
 ## ð ä»ç»
 ä¸ä¸ªç½æäºå¤éç¹æ­æä»¶ï¼å¯ä»¥ç¿»é¡µï¼å¯ä»¥ç»å½ç½æäºè´¦å·ç¹
 vip æ­æ²å¬ï¼æä»¶åéçæ¯èªå®ä¹é³ä¹å¡çï¼ï¼æ²¡äº ###
-æ­æ²åè¡¨ææå¾ ![pic](https://raw.githubusercontent.com/lgc-NB2Dev/
-readme/main/multincm/QQå¾ç20230515025601.jpg) ## ð¿ å®è£
-ä»¥ä¸æå°çæ¹æ³ ä»»é**å¶ä¸** å³å¯  [æ¨è] ä½¿ç¨ nb-cli å®è£
-å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
-è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```bash nb plugin install nonebot-plugin-
-multincm ```   ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
-æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
-pip ```bash pip install nonebot-plugin-multincm ```   pdm ```bash pdm add
-nonebot-plugin-multincm ```   poetry ```bash poetry add nonebot-plugin-multincm
-```   conda ```bash conda install nonebot-plugin-multincm ```  æå¼ nonebot2
+ææå¾  æ­æ²åè¡¨ææå¾ï¼ç¹å»å±å¼ï¼ ![pic](https://
+raw.githubusercontent.com/lgc-NB2Dev/readme/main/multincm/
+QQå¾ç20230515025601.jpg)   çµå°åè¡¨ææå¾ï¼ç¹å»å±å¼ï¼ ![pic]
+(https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/multincm/
+QQå¾ç20230519034438.jpg)   æ­è¯ææå¾ï¼ç¹å»å±å¼ï¼ ![pic](https://
+raw.githubusercontent.com/lgc-NB2Dev/readme/main/multincm/
+QQå¾ç20230519034757.png)  ## ð¿ å®è£ ä»¥ä¸æå°çæ¹æ³
+ä»»é**å¶ä¸** å³å¯  [æ¨è] ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
+é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```bash nb
+plugin install nonebot-plugin-multincm ```   ä½¿ç¨åç®¡çå¨å®è£ å¨
+nonebot2 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡,
+æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤  pip ```bash pip
+install nonebot-plugin-multincm ```   pdm ```bash pdm add nonebot-plugin-
+multincm ```   poetry ```bash poetry add nonebot-plugin-multincm ```   conda
+```bash conda install nonebot-plugin-multincm ```  æå¼ nonebot2
 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åç
 `plugins` é¡¹éè¿½å åå¥ ```toml [tool.nonebot] plugins = [ # ...
 "nonebot_plugin_multincm" ] ```  ## âï¸ éç½® å¦æä½ å®è£äº [nonebot-
 plugin-ncm](https://github.com/kitUIN/nonebot-plugin-
 ncm)ï¼æ¬æä»¶ä¼ä¸å¶å±ç¨åä¸ä¸ª
 Sessionï¼å°±å¯ä»¥ä¸ç¨å¡«ä¸é¢çè´¦å·å¯ç äº
 ä¸é¢éç½®ä¸­ï¼ææºå·ç»å½ å é®ç®±ç»å½ãææå¯ç  å MD5
@@ -35,32 +40,39 @@
 `NCM_LIST_LIMIT` | å¦ | `20` | æ­æ²åè¡¨æ¯é¡µçæå¤§æ°é | |
 `NCM_LIST_FONT` | å¦ | æ  | æ¸²ææ­æ²åè¡¨ä½¿ç¨çå­ä½ | |
 `NCM_MAX_NAME_LEN` | å¦ | `600` |
 æ­æ²åè¡¨ä¸­æ­ååçæå¤§ææ¬å®½åº¦ï¼åç´ ï¼ | |
 `NCM_MAX_ARTIST_LEN` | å¦ | `400` |
 æ­æ²åè¡¨ä¸­æ­æåçæå¤§ææ¬å®½åº¦ï¼åç´ ï¼ | ## ð ä½¿ç¨ ###
 æä»¤ - ç¹æ­ [æ­æ²å / é³ä¹ ID] -
-ä»ç»ï¼é¡¾åæä¹ãå½è¾å¥é³ä¹ ID æ¶ä¼ç´æ¥åéå¯¹åºé³ä¹ -
-å«åï¼`ç½æäº`ã`wyy` - è§£æ <åå¤ é³ä¹å¡ç / é¾æ¥> -
-ä»ç»ï¼è·åè¯¥é³ä¹çæ­æ¾é¾æ¥å¹¶ä½¿ç¨èªå®ä¹å¡çåé -
-å«åï¼`resolve`ã`parse`ã`get` - æ­è¯ <åå¤ é³ä¹å¡ç / é¾æ¥> -
+ä»ç»ï¼æç´¢æ­æ²ãå½è¾å¥é³ä¹ ID æ¶ä¼ç´æ¥åéå¯¹åºé³ä¹ -
+å«åï¼`ç½æäº`ã`wyy` - çµå° [æ­æ²å / èç® ID] -
+ä»ç»ï¼æç´¢çµå°èç®ãå½è¾å¥çµå° ID æ¶ä¼ç´æ¥åéå¯¹åºèç®
+- å«åï¼`å£°é³`ã`ç½æçµå°`ã`wtdt`ã`wydj` - è§£æ [åå¤
+é³ä¹å¡ç / é¾æ¥] - ä»ç»ï¼è·åè¯¥ é³ä¹ / çµå°èç®
+çæ­æ¾é¾æ¥å¹¶ä½¿ç¨èªå®ä¹å¡çåé -
+å«åï¼`resolve`ã`parse`ã`get` - æ­è¯ [åå¤ é³ä¹å¡ç / é¾æ¥] -
 ä»ç»ï¼è·åè¯¥é³ä¹çæ­è¯ï¼ä»¥å¾çå½¢å¼åé -
-å«åï¼`lrc`ã`lyric`ã`lyrics` - é¾æ¥ <åå¤ é³ä¹å¡ç> -
-ä»ç»ï¼è·å Bot åéçé³ä¹å¡ççç½æäºæ­æ²é¾æ¥ -
-å«åï¼`link` ### Tip - ç¹å» Bot
-åéçé³ä¹å¡çä¼è·³è½¬å°é³ä¹ç´é¾ï¼å¯ä»¥ç´æ¥ä¸è½½ ## ð
-èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼
-[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
-126.com> ## ð¡ é¸£è°¢ ### [MeetWq/pil-utils](https://github.com/MeetWq/pil-
-utils) è¶å¥½ç¨ç Pillow è¾å©åº ## ð° èµå©
+å«åï¼`lrc`ã`lyric`ã`lyrics` - é¾æ¥ [åå¤ é³ä¹å¡ç] -
+ä»ç»ï¼è·å Bot åéçé³ä¹å¡ççç½æäºé¾æ¥ -
+å«åï¼`link`ã`url` ### Tip - ç¹å» Bot
+åéçé³ä¹å¡çä¼è·³è½¬å°é³ä¹ç´é¾ï¼å¯ä»¥ç´æ¥ä¸è½½ -
+ä½¿ç¨éè¦åå¤é³ä¹å¡ççæä»¤æ¶ï¼å¦ææ²¡æåå¤ï¼ä¼èªå¨ä½¿ç¨ä½ è§¦ååéçæè¿ä¸ä¸ªé³ä¹å¡ççä¿¡æ¯
+## ð èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333)
+å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
+126.com> ## ð¡ é¸£è°¢ ### [mos9527/pyncm](https://github.com/mos9527/pyncm)
+é¡¹ç®ä½¿ç¨çç½æäº API è°ç¨åº ### [Binaryify/NeteaseCloudMusicApi]
+(https://github.com/Binaryify/NeteaseCloudMusicApi) é¡¹ç®çµå°ç¸å³ API
+æ¥æº ### [MeetWq/pil-utils](https://github.com/MeetWq/pil-utils) è¶å¥½ç¨ç
+Pillow è¾å©åº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.2.5 -
-`è§£æ`ã`æ­è¯`ã`é¾æ¥` æä»¤å¯ä»¥ç´æ¥æ ¹æ® Bot
-åéçä¸ä¸ªé³ä¹å¡çä½åºååºäº -
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.3.0 -
+æ¯æçµå°èç®çè§£æä¸ç¹æ­ ### 0.2.5 - `è§£æ`ã`æ­è¯`ã`é¾æ¥`
+æä»¤å¯ä»¥ç´æ¥æ ¹æ® Bot åéçä¸ä¸ªé³ä¹å¡çä½åºååºäº -
 æ­è¯è§£æä¼åå¹¶å¤è¡ç©ºè¡åå»æé¦å°¾ç©ºè¡äº -
 ç°å¨æä»¶ä¼å®æ¶æ¸çèªèº«åå­ä¸­çç¼å­äº ### 0.2.4 -
 ä¿®å¤ä¸ä¸ªæ­è¯è§£æ bug ### 0.2.3 - å¾®è°æ­æ²åè¡¨æç -
 å¾®è°æä»¶å¸®å©ææ¬ ### 0.2.2 - ä¿®å¤ææ­ `KeyError` ### 0.2.1 -
 å é¤æ­è¯å°¾é¨çç©ºè¡ä¸å¤ä½åå²çº¿ ### 0.2.0 - æ°å¢äºä¸ä¸ªæä»¤
 `è§£æ`ã`æ­è¯`ã`é¾æ¥` - ç¹æ­æä»¤æ¯æç´æ¥è¾å¥é³ä¹ ID
```

### Comparing `nonebot_plugin_multincm-0.2.5/nonebot_plugin_multincm/__init__.py` & `nonebot_plugin_multincm-0.3.0/nonebot_plugin_multincm/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 from nonebot.plugin import PluginMetadata, require
 
 require("nonebot_plugin_apscheduler")
 
 from . import __main__ as __main__  # noqa: E402
 from .config import ConfigModel  # noqa: E402
 
-__version__ = "0.2.5"
+__version__ = "0.3.0"
 __plugin_meta__ = PluginMetadata(
     "MultiNCM",
     "网易云多选点歌",
     (
-        "指令列表\n"
+        "指令列表：\n"
         "▶ 点歌 [歌曲名 / 音乐 ID]\n"
-        "    ▷ 介绍：顾名思义。当输入音乐 ID 时会直接发送对应音乐\n"
+        "    ▷ 介绍：搜索歌曲。当输入音乐 ID 时会直接发送对应音乐\n"
         "    ▷ 别名：`网易云`、`wyy`\n"
-        "▶ 解析 <回复 音乐卡片 / 链接>\n"
+        "▶ 电台 [歌曲名 / 节目 ID]\n"
+        "    ▷ 介绍：搜索电台节目。当输入电台 ID 时会直接发送对应节目\n"
+        "    ▷ 别名：`声音`、`网易电台`、`wtdt`、`wydj`\n"
+        "▶ 解析 [回复 音乐卡片 / 链接]\n"
         "    ▷ 介绍：获取该音乐的播放链接并使用自定义卡片发送\n"
         "    ▷ 别名：`resolve`、`parse`、`get`\n"
-        "▶ 歌词 <回复 音乐卡片 / 链接>\n"
+        "▶ 歌词 [回复 音乐卡片 / 链接]\n"
         "    ▷ 介绍：获取该音乐的歌词，以图片形式发送\n"
         "    ▷ 别名：`lrc`、`lyric`、`lyrics`\n"
-        "▶ 链接 <回复 音乐卡片>\n"
+        "▶ 链接 [回复 音乐卡片]\n"
         "    ▷ 介绍：获取 Bot 发送的音乐卡片的网易云歌曲链接\n"
-        "    ▷ 别名：`link`\n"
+        "    ▷ 别名：`link`、`url`\n"
         " \n"
-        "Tip: 点击 Bot 发送的音乐卡片会跳转到音乐直链，可以直接下载"
+        "Tip：\n"
+        "▶ 点击 Bot 发送的音乐卡片会跳转到音乐直链，可以直接下载\n"
+        "▶ 使用需要回复音乐卡片的指令时，如果没有回复，会自动使用你触发发送的最近一个音乐卡片的信息"
     ),
     ConfigModel,
     {"License": "MIT", "Author": "student_2333"},
 )
```

### Comparing `nonebot_plugin_multincm-0.2.5/nonebot_plugin_multincm/__main__.py` & `nonebot_plugin_multincm-0.3.0/nonebot_plugin_multincm/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,23 @@
-import asyncio
 import re
 from contextlib import suppress
 from math import ceil
-from typing import Any, Awaitable, Callable, Dict, Optional, Union, cast
+from typing import (
+    Any,
+    Awaitable,
+    Callable,
+    Dict,
+    List,
+    Literal,
+    Optional,
+    Tuple,
+    Union,
+    cast,
+    overload,
+)
 
 from nonebot import logger, on_command
 from nonebot.adapters.onebot.v11 import (
     Bot,
     Event,
     GroupMessageEvent,
     Message,
@@ -15,195 +26,293 @@
 )
 from nonebot.internal.matcher import Matcher, current_event
 from nonebot.params import ArgPlainText, CommandArg
 from nonebot.rule import Rule
 from nonebot.typing import T_RuleChecker, T_State
 
 from .config import config
-from .data_source import get_track_audio, get_track_info, get_track_lrc, search_song
+from .data_source import (
+    get_track_audio,
+    get_track_info,
+    get_track_lrc,
+    get_voice_info,
+    search_song,
+    search_voice,
+)
 from .draw import draw_search_res, format_lrc, str_to_pic
-from .msg_cache import SongCache, chat_last_song_cache, song_msg_id_cache
-from .types import Song, SongSearchResult
+from .msg_cache import (
+    CALLING_MAP,
+    SongCache,
+    SongType,
+    chat_last_song_cache,
+    song_msg_id_cache,
+)
+from .types import (
+    SearchResult,
+    Song,
+    SongInfo,
+    SongSearchResult,
+    VoiceBaseInfo,
+    VoiceResource,
+)
 from .utils import format_alias, format_artists
 
-SONG_ID_REGEX = re.compile(r"music\.163\.com(.*)(song|url)/?\?id=(?P<id>[0-9]+)(|&)")
+LINK_TYPE_MAP: Dict[SongType, Tuple[str, ...]] = {
+    "song": ("song", "url"),
+    "voice": ("dj", "program"),
+}
+
+link_types: List[str] = []
+[link_types.extend(x) for x in LINK_TYPE_MAP.values()]
+link_type_reg = "|".join(link_types)
+
+SONG_ID_REGEX = re.compile(
+    rf"music\.163\.com(.*?)(?P<type>{link_type_reg})/?\?id=(?P<id>[0-9]+)(|&)",
+)
 
 
 def get_chat_cache_key(event: MessageEvent) -> str:
     g = event.group_id if isinstance(event, GroupMessageEvent) else 0
     return f"{g}.{event.user_id}"
 
 
-def extract_id_from_text(text: str) -> Optional[int]:
-    res = re.search(SONG_ID_REGEX, text)
-    return int(res["id"]) if res else None
-
-
 async def cache_music_msg_rule(event: MessageEvent, state: T_State) -> bool:
     if reply := event.reply:
         song_cache = song_msg_id_cache.get(reply.message_id)
         if song_cache:
             state["song_cache"] = song_cache
             return True
 
     return False
 
 
+def get_type_from_url_type(type_name: str) -> SongType:
+    type_name = type_name.lower()
+    for k, v in LINK_TYPE_MAP.items():
+        if type_name in v:
+            return cast(Any, k)
+    raise ValueError(f"invalid type {type_name}")
+
+
 async def reply_music_rule(event: MessageEvent, state: T_State) -> bool:
     if reply := event.reply:
-        song_id = extract_id_from_text(str(reply.message))
-        if song_id:
-            state["song_cache"] = SongCache(id=song_id, type="song")
-            return True
+        res = re.search(SONG_ID_REGEX, str(reply.message))
+        if res:
+            type_name = None
+            with suppress(ValueError):
+                type_name = get_type_from_url_type(res["type"])
+
+            if type_name:
+                state["song_cache"] = SongCache(id=int(res["id"]), type=type_name)
+                return True
 
     return False
 
 
 async def chat_last_music_rule(event: MessageEvent, state: T_State) -> bool:
     if song_cache := chat_last_song_cache.get(get_chat_cache_key(event)):
         state["song_cache"] = song_cache
         return True
 
     return False
 
 
 def any_rule(*rules: Union[T_RuleChecker, Rule]) -> Callable[..., Awaitable[bool]]:
     async def rule(bot: Bot, event: Event, state: T_State):
-        return any(
-            await asyncio.gather(*(Rule(x)(bot, event, state) for x in rules)),
-        )
+        # 要按顺序执行，所以不能用 asyncio.gather
+        for x in rules:  # noqa: SIM110
+            if await Rule(x)(bot, event, state):
+                return True
+        return False
 
     return rule
 
 
 music_msg_matcher_rule = any_rule(
     cache_music_msg_rule,
     reply_music_rule,
     chat_last_music_rule,
 )
 
 
-async def send_music(matcher: Matcher, song: Song):
+async def send_music(matcher: Matcher, song: SongInfo):
+    is_song = isinstance(song, Song)
+    calling = CALLING_MAP["song" if is_song else "voice"]
+    song_id = song.id if is_song else song.mainTrackId
+    bitrate = 999999
+    # 管你妈那么多闲事干嘛，直接上最高就得了
+    # bitrate = (
+    #     song.privilege.pl if is_song and song.privilege.plLevel else None
+    # ) or 999999
+
     try:
-        audio_info = await get_track_audio(
-            [song.id],
-            999999 if song.privilege.plLevel == "none" else song.privilege.pl,
-        )
+        audio_info = await get_track_audio([song_id], bitrate)
     except:
-        logger.exception("获取歌曲播放链接失败")
-        await matcher.finish("获取歌曲播放链接失败，请检查后台输出")
+        logger.exception(f"获取{calling}播放链接失败")
+        await matcher.finish(f"获取{calling}播放链接失败，请检查后台输出")
 
     if not audio_info:
-        await matcher.finish("抱歉，没有获取到歌曲播放链接")
+        await matcher.finish(f"抱歉，没有获取到{calling}播放链接")
 
     info = audio_info[0]
     ret: Dict[str, Any] = await matcher.send(
         MessageSegment(
             "music",
             {
                 "type": "custom",
                 "subtype": "163",
                 "url": info.url,
                 "voice": info.url,
-                "title": format_alias(song.name, song.alia),
-                "content": format_artists(song.ar),
-                "image": song.al.picUrl,
+                "title": format_alias(song.name, song.alia) if is_song else song.name,
+                "content": format_artists(song.ar) if is_song else song.radio.name,
+                "image": song.al.picUrl if is_song else song.coverUrl,
             },
         ),
     )
 
-    song_cache = SongCache(id=song.id, type="song")
+    song_cache = SongCache(id=song.id, type="song" if is_song else "voice")
     event = cast(MessageEvent, current_event.get())
 
     chat_last_song_cache[get_chat_cache_key(event)] = song_cache
     if msg_id := ret.get("message_id"):
         song_msg_id_cache[msg_id] = song_cache
 
     await matcher.finish()
 
 
 async def get_cache_by_index(
-    cache: Dict[int, SongSearchResult],
+    cache: Dict[int, SearchResult],
     arg: int,
-) -> Optional[Song]:
+) -> Optional[SongInfo]:
     ori_index = arg - 1
     page_index = ceil(ori_index / config.ncm_list_limit)
     page_index = 1 if page_index == 0 else page_index
     index = ori_index % config.ncm_list_limit
 
-    if (not (res := cache.get(page_index))) or (not (0 <= index < len(res.songs))):
+    res = cache.get(page_index)
+    if not (res):
         return None
 
-    return res.songs[index]
+    results = res.songs if isinstance(res, SongSearchResult) else res.resources
+    if not (0 <= index < len(results)):
+        return None
+
+    got = results[index]
+    if isinstance(got, VoiceResource):
+        return got.baseInfo
+    return got
 
 
 async def get_page(
     matcher: Matcher,
     state: T_State,
     page: int = 1,
 ) -> MessageSegment:
     param: str = state["param"]
-    cache: Dict[int, SongSearchResult] = state["cache"]
+    cache: Dict[int, SearchResult] = state["cache"]
+    song_type: SongType = state["type"]
+    calling = CALLING_MAP[song_type]
 
     if not (res := cache.get(page)):
         try:
-            res = await search_song(param, page=page)
+            func = search_song if song_type == "song" else search_voice
+            res = await func(param, page=page)
         except:
             logger.exception("搜索歌曲失败")
             await matcher.finish("搜索歌曲失败，请检查后台输出")
 
-        if not res.songCount:
+        if not (res.songCount if isinstance(res, SongSearchResult) else res.totalCount):
             await matcher.finish("没搜到任何歌曲捏")
 
+    is_song = isinstance(res, SongSearchResult)
+    total_count = res.songCount if is_song else res.totalCount
+
     state["page"] = page
     cache[page] = res
-    state["page_max"] = ceil(res.songCount / config.ncm_list_limit)
+    state["page_max"] = ceil(total_count / config.ncm_list_limit)
 
-    if page == 1 and len(res.songs) == 1:
+    results = res.songs if is_song else res.resources
+    if page == 1 and len(results) == 1:
         await get_cache_by_index(cache, 1)
 
     try:
         pic = draw_search_res(res, page)
     except:
-        logger.exception("绘制歌曲列表失败")
-        await matcher.finish("绘制歌曲列表失败，请检查后台输出")
+        logger.exception(f"绘制{calling}列表失败")
+        await matcher.finish(f"绘制{calling}列表失败，请检查后台输出")
 
     return MessageSegment.image(pic)
 
 
-cmd_pick_song = on_command("点歌", aliases={"网易云", "wyy"})
+@overload
+async def get_song_info(song_id: int, song_type: Literal["song"]) -> Optional[Song]:
+    ...
+
+
+@overload
+async def get_song_info(
+    song_id: int,
+    song_type: Literal["voice"],
+) -> Optional[VoiceBaseInfo]:
+    ...
+
+
+async def get_song_info(song_id, song_type):
+    if song_type == "voice":
+        return await get_voice_info(song_id)
+
+    song = await get_track_info([song_id])
+    return song[0] if song else None
+
+
+cmd_pick_song = on_command(
+    "点歌",
+    aliases={"网易云", "wyy"},
+    state={"type": "song"},
+)
+cmd_pick_voice = on_command(
+    "电台",
+    aliases={"声音", "网易电台", "wydt", "wydj"},
+    state={"type": "voice"},
+)
 
 
 @cmd_pick_song.handle()
+@cmd_pick_voice.handle()
 async def _(matcher: Matcher, arg_msg: Message = CommandArg()):
     if arg_msg.extract_plain_text().strip():
         matcher.set_arg("arg", arg_msg)
 
 
 @cmd_pick_song.got("arg", "请发送搜索内容")
+@cmd_pick_voice.got("arg", "请发送搜索内容")
 async def _(matcher: Matcher, state: T_State, arg: str = ArgPlainText("arg")):
+    song_type: SongType = state["type"]
+    calling = CALLING_MAP[song_type]
+
     param = arg.strip()
     if not param:
-        await matcher.finish("消息无文本，放弃点歌")
+        await matcher.finish("消息无文本，放弃点播")
 
     if param.isdigit():
-        song = []
+        song = None
         with suppress(Exception):
-            song = await get_track_info([int(param)])
+            song = await get_song_info(int(param), song_type)
         if song:
-            await matcher.send("检测到输入了音乐 ID，将直接获取并发送对应歌曲")
-            await send_music(matcher, song[0])
+            await matcher.send(f"检测到输入了{calling} ID，将直接获取并发送对应{calling}")
+            await send_music(matcher, song)
 
     state["param"] = param
     state["page"] = 1
     state["cache"] = {}
     await matcher.pause(await get_page(matcher, state))
 
 
 @cmd_pick_song.handle()
+@cmd_pick_voice.handle()
 async def _(matcher: Matcher, state: T_State, event: MessageEvent):
     arg = event.get_message().extract_plain_text().strip().lower()
     page: int = state["page"]
     page_max: int = state["page_max"]
 
     if arg in ["退出", "tc", "取消", "qx", "exit", "e", "cancel", "c", "0"]:
         await matcher.finish("已退出选择")
@@ -215,15 +324,15 @@
 
     if arg in ["下一页", "xyy", "next", "n"]:
         if page >= page_max:
             await matcher.reject("已经是最后一页了")
         await matcher.reject(await get_page(matcher, state, page + 1))
 
     if arg.isdigit():
-        cache = state["cache"]
+        cache: Dict[int, SearchResult] = state["cache"]
         song = await get_cache_by_index(cache, int(arg))
         if not song:
             await matcher.reject("序号输入有误，请重新输入")
         await send_music(matcher, song)
 
     await matcher.reject("非正确指令，请重新输入")
 
@@ -234,54 +343,67 @@
     rule=music_msg_matcher_rule,
 )
 
 
 @cmd_get_song.handle()
 async def _(matcher: Matcher, state: T_State):
     song_cache: SongCache = state["song_cache"]
-    song_id = song_cache.id
+    calling = CALLING_MAP[song_cache.type]
 
     try:
-        song = await get_track_info([song_id])
+        if song_cache.type == "voice":
+            song = await get_voice_info(song_cache.id)
+        else:
+            song = await get_track_info([song_cache.id])
+            song = song[0] if song else None
     except:
-        logger.exception("获取歌曲信息失败")
-        await matcher.finish("获取歌曲信息失败，请检查后台输出")
+        logger.exception(f"获取{calling}信息失败")
+        await matcher.finish(f"获取{calling}信息失败，请检查后台输出")
 
     if not song:
-        await matcher.finish("未获取到对应歌曲信息")
+        await matcher.finish(f"未获取到对应{calling}信息")
 
-    await send_music(matcher, song[0])
+    await send_music(matcher, song)
 
 
 cmd_get_lrc = on_command(
     "歌词",
     aliases={"lrc", "lyric", "lyrics"},
     rule=music_msg_matcher_rule,
 )
 
 
 @cmd_get_lrc.handle()
 async def _(matcher: Matcher, state: T_State):
     song_cache: SongCache = state["song_cache"]
-    song_id = song_cache.id
 
+    if song_cache.type == "voice":
+        await matcher.finish("电台节目无法获取歌词")
+
+    song_id = song_cache.id
     try:
         lrc_data = await get_track_lrc(song_id)
     except:
         logger.exception("获取歌曲歌词失败")
         await matcher.finish("获取歌曲歌词失败，请检查后台输出")
 
     lrc = format_lrc(lrc_data)
     if not lrc:
         await matcher.finish("该歌曲没有歌词")
 
     await matcher.finish(MessageSegment.image(str_to_pic(lrc)))
 
 
-cmd_get_cache_link = on_command("链接", aliases={"link"}, rule=music_msg_matcher_rule)
+cmd_get_cache_link = on_command(
+    "链接",
+    aliases={"link", "url"},
+    rule=music_msg_matcher_rule,
+)
 
 
 @cmd_get_cache_link.handle()
 async def _(matcher: Matcher, state: T_State):
     song_cache: SongCache = state["song_cache"]
     song_id = song_cache.id
-    await matcher.finish(f"https://music.163.com/song?id={song_id}")
+
+    link_type = "dj" if song_cache.type == "voice" else song_cache.type
+    await matcher.finish(f"https://music.163.com/{link_type}?id={song_id}")
```

### Comparing `nonebot_plugin_multincm-0.2.5/nonebot_plugin_multincm/config.py` & `nonebot_plugin_multincm-0.3.0/nonebot_plugin_multincm/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.2.5/nonebot_plugin_multincm/data_source.py` & `nonebot_plugin_multincm-0.3.0/nonebot_plugin_multincm/data_source.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,52 +5,82 @@
 from nonebot import get_available_plugin_names, logger, require
 from pyncm import (
     DumpSessionAsString,
     GetCurrentSession,
     LoadSessionFromString,
     SetCurrentSession,
 )
+from pyncm.apis import WeapiCryptoRequest
 from pyncm.apis.cloudsearch import GetSearchResult
 from pyncm.apis.login import (
     GetCurrentLoginStatus,
     LoginViaAnonymousAccount,
     LoginViaCellphone,
     LoginViaEmail,
 )
 from pyncm.apis.track import GetTrackAudio, GetTrackDetail, GetTrackLyrics
 
 from .config import config
 from .const import DATA_PATH
-from .types import LyricData, Privilege, Song, SongSearchResult, TrackAudio
+from .types import (
+    LyricData,
+    Privilege,
+    Song,
+    SongSearchResult,
+    TrackAudio,
+    VoiceBaseInfo,
+    VoiceSearchResult,
+)
 from .utils import awaitable
 
 SESSION_FILE = DATA_PATH / "session.cache"
 
 
+def get_offset_by_page_num(page: int, limit: int = config.ncm_list_limit) -> int:
+    return limit * (page - 1)
+
+
 async def ncm_request(api: Callable, *args, **kwargs) -> Dict[str, Any]:
     ret = await awaitable(api)(*args, **kwargs)
     if ret.get("code", 200) != 200:
         raise RuntimeError(f"请求 {api.__name__} 失败\n{ret}")
     logger.debug(f"{api.__name__} - {ret}")
     return ret
 
 
 async def search_song(keyword: str, page: int = 1, **kwargs) -> SongSearchResult:
-    limit = config.ncm_list_limit
-    offset = limit * (page - 1)
+    offset = get_offset_by_page_num(page)
     res = await ncm_request(
         GetSearchResult,
         keyword=keyword,
-        limit=limit,
+        limit=config.ncm_list_limit,
         offset=offset,
         **kwargs,
     )
     return SongSearchResult(**res["result"])
 
 
+async def search_voice(keyword: str, page: int = 1) -> VoiceSearchResult:
+    @WeapiCryptoRequest  # type: ignore
+    def SearchVoice():  # noqa: N802
+        return (
+            "/api/search/voice/get",
+            {
+                "keyword": keyword,
+                "scene": "normal",
+                "limit": config.ncm_list_limit,
+                "offset": offset or 0,
+            },
+        )
+
+    offset = get_offset_by_page_num(page)
+    res = await ncm_request(SearchVoice)
+    return VoiceSearchResult(**res["data"])
+
+
 async def get_track_audio(
     song_ids: List[int],
     bit_rate: int = 320000,
     **kwargs,
 ) -> List[TrackAudio]:
     res = await ncm_request(GetTrackAudio, song_ids, bitrate=bit_rate, **kwargs)
     return [TrackAudio(**x) for x in cast(List[dict], res["data"])]
@@ -73,14 +103,23 @@
 
 
 async def get_track_lrc(song_id: int) -> LyricData:
     res = await ncm_request(GetTrackLyrics, song_id)
     return LyricData(**res)
 
 
+async def get_voice_info(program_id: int) -> VoiceBaseInfo:
+    @WeapiCryptoRequest  # type: ignore
+    def GetProgramDetail():  # noqa: N802
+        return ("/api/dj/program/detail", {"id": program_id})
+
+    res = await ncm_request(GetProgramDetail)
+    return VoiceBaseInfo(**res["program"])
+
+
 async def login(retry=True):
     if SESSION_FILE.exists():
         logger.info(f"使用缓存登录态 ({str(SESSION_FILE)})")
         SetCurrentSession(
             LoadSessionFromString(
                 (await anyio.Path(SESSION_FILE).read_text(encoding="u8")),
             ),
```

### Comparing `nonebot_plugin_multincm-0.2.5/nonebot_plugin_multincm/draw.py` & `nonebot_plugin_multincm-0.3.0/nonebot_plugin_multincm/draw.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 from dataclasses import dataclass
 from io import BytesIO
 from math import ceil
 from pathlib import Path
-from typing import List, Optional, Sequence, Union, cast
+from typing import List, Optional, Sequence, Tuple, Union, cast
 
 from pil_utils import BuildImage, Text2Image
 from pil_utils.types import ColorType, HAlignType
 
+from nonebot_plugin_multincm.msg_cache import CALLING_MAP
+
 from . import lrc_parser
 from .config import config
-from .types import Lyric, LyricData, SongSearchResult, User
+from .types import (
+    Lyric,
+    LyricData,
+    SearchResult,
+    SongSearchResult,
+    User,
+    VoiceSearchResult,
+)
 from .utils import format_alias, format_artists, format_time
 
 BACKGROUND = BuildImage.open(Path(__file__).parent / "res" / "bg.jpg")
 
 
 @dataclass()
 class TableHead:
@@ -184,21 +193,19 @@
                 fill=border_color,
                 width=border_width,
             )
 
     return pic
 
 
-def draw_search_res(res: SongSearchResult, page_num: int = 1) -> BytesIO:
-    pic_padding = 50
-    table_padding = 20
-    table_border_radius = 15
-
-    index_offset = (page_num - 1) * config.ncm_list_limit
-    table = draw_table(
+def get_song_search_res_table(
+    res: SongSearchResult,
+    index_offset: int = 0,
+) -> Tuple[List[TableHead], List[List[str]]]:
+    return (
         [
             TableHead("序号", align="right"),
             TableHead("歌名", max_width=config.ncm_max_name_len),
             TableHead("歌手", max_width=config.ncm_max_artist_len),
             TableHead("时长", align="center"),
             TableHead("热度", align="center"),
         ],
@@ -208,34 +215,77 @@
                 format_alias(x.name, x.alia),
                 format_artists(x.ar),
                 format_time(x.dt),
                 f"{int(x.pop)}",
             ]
             for i, x in enumerate(res.songs)
         ],
+    )
+
+
+def get_voice_search_res_table(
+    res: VoiceSearchResult,
+    index_offset: int = 0,
+) -> Tuple[List[TableHead], List[List[str]]]:
+    return (
+        [
+            TableHead("序号", align="right"),
+            TableHead("节目", max_width=config.ncm_max_name_len),
+            TableHead("电台", max_width=config.ncm_max_name_len),
+            TableHead("台主", max_width=config.ncm_max_artist_len),
+            TableHead("时长", align="center"),
+        ],
+        [
+            [
+                f"[b]{i + index_offset + 1}[/b]",
+                x.baseInfo.name,
+                x.baseInfo.radio.name,
+                x.baseInfo.dj.nickname,
+                format_time(x.baseInfo.duration),
+            ]
+            for i, x in enumerate(res.resources)
+        ],
+    )
+
+
+def draw_search_res(res: SearchResult, page_num: int = 1) -> BytesIO:
+    pic_padding = 50
+    table_padding = 20
+    table_border_radius = 15
+
+    is_song = isinstance(res, SongSearchResult)
+    index_offset = (page_num - 1) * config.ncm_list_limit
+    table = draw_table(
+        *(
+            get_song_search_res_table(res, index_offset)
+            if is_song
+            else get_voice_search_res_table(res, index_offset)
+        ),
         border_radius=table_border_radius,
     )
 
-    max_page = ceil(res.songCount / config.ncm_list_limit)
+    calling = CALLING_MAP["song" if is_song else "voice"]
+    max_count = res.songCount if is_song else res.totalCount
+    max_page = ceil(max_count / config.ncm_list_limit)
     title_txt = Text2Image.from_text(
-        "歌曲列表",
+        f"{calling}列表",
         80,
         weight="bold",
         fill=(255, 255, 255),
         fontname=config.ncm_list_font or "",
     )
     tip_txt = Text2Image.from_bbcode_text(
-        "Tip：[b]发送序号[/b] 选择歌曲\n其他操作：[b]上一页[/b](P) | [b]下一页[/b](N) | [b]退出[/b](E)",
+        f"Tip：[b]发送序号[/b] 选择{calling}\n其他操作：[b]上一页[/b](P) | [b]下一页[/b](N) | [b]退出[/b](E)",
         30,
         align="center",
         fill=(255, 255, 255),
         fontname=config.ncm_list_font or "",
     )
     footer_txt = Text2Image.from_bbcode_text(
-        f"第 [b]{page_num}[/b] / [b]{max_page}[/b] 页 | 共 [b]{res.songCount}[/b] 首",
+        f"第 [b]{page_num}[/b] / [b]{max_page}[/b] 页 | 共 [b]{max_count}[/b] 首",
         30,
         align="center",
         fill=(255, 255, 255),
         fontname=config.ncm_list_font or "",
     )
 
     width = table.width + pic_padding * 2 + table_padding * 2
```

### Comparing `nonebot_plugin_multincm-0.2.5/nonebot_plugin_multincm/lrc_parser.py` & `nonebot_plugin_multincm-0.3.0/nonebot_plugin_multincm/lrc_parser.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.2.5/nonebot_plugin_multincm/msg_cache.py` & `nonebot_plugin_multincm-0.3.0/nonebot_plugin_multincm/msg_cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,21 +3,26 @@
 from typing import Dict, Generic, Iterable, Literal, Optional, Tuple, TypeVar, overload
 
 from nonebot_plugin_apscheduler import scheduler
 
 KT = TypeVar("KT")
 VT = TypeVar("VT")
 
-SongType = Literal["song"]
+SongType = Literal["song", "voice"]
+
+CALLING_MAP: Dict[SongType, str] = {
+    "song": "歌曲",
+    "voice": "节目",
+}
 
 
 @dataclass
 class SongCache:
     id: int  # noqa: A003
-    type: SongType = "song"  # noqa: A003
+    type: SongType  # noqa: A003
 
 
 # “优雅”
 class CacheManager(Generic[KT, VT], Dict[KT, Tuple[float, VT]]):
     def __init__(self, *args, **kwargs):
         self._job = scheduler.add_job(self.clear_expired, "interval", hours=1)
         super().__init__(*args, **kwargs)
```

### Comparing `nonebot_plugin_multincm-0.2.5/nonebot_plugin_multincm/res/bg.jpg` & `nonebot_plugin_multincm-0.3.0/nonebot_plugin_multincm/res/bg.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.2.5/nonebot_plugin_multincm/types.py` & `nonebot_plugin_multincm-0.3.0/nonebot_plugin_multincm/types.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,15 @@
-from typing import List, Literal, Optional
+from typing import List, Literal, Optional, Union
 
 from pydantic import BaseModel
 
-BrLevel = Literal["hires", "lossless", "exhigh", "higher", "standard", "none"]
+BrLevel = Literal["hires", "lossless", "exhigh", "higher", "standard"]
+
+SearchResult = Union["SongSearchResult", "VoiceSearchResult"]
+SongInfo = Union["Song", "VoiceBaseInfo"]
 
 
 class Artist(BaseModel):
     id: int  # noqa: A003
     name: str
     tns: List[str]
     alias: List[str]
@@ -18,15 +21,15 @@
     picUrl: str  # noqa: N815
     tns: List[str]
 
 
 class Privilege(BaseModel):
     id: int  # noqa: A003
     pl: int
-    plLevel: BrLevel  # noqa: N815
+    plLevel: Optional[BrLevel]  # noqa: N815
 
 
 class Song(BaseModel):
     name: str
     id: int  # noqa: A003
     ar: List[Artist]
     alia: List[str]
@@ -58,16 +61,16 @@
 
 class TrackAudio(BaseModel):
     id: int  # noqa: A003
     url: str
     br: int
     size: int
     md5: str
-    level: str
-    encodeType: str  # noqa: N815
+    level: Optional[str]
+    encodeType: Optional[str]  # noqa: N815
     time: int
 
 
 class User(BaseModel):
     id: int  # noqa: A003
     userid: int
     nickname: str
@@ -80,7 +83,56 @@
 
 class LyricData(BaseModel):
     transUser: Optional[User]  # noqa: N815
     lyricUser: Optional[User]  # noqa: N815
     lrc: Optional[Lyric]
     tlyric: Optional[Lyric]
     romalrc: Optional[Lyric]
+
+
+class DJ(BaseModel):
+    userId: int  # noqa: N815
+    nickname: str
+    avatarUrl: str  # noqa: N815
+    gender: int
+    signature: str
+    backgroundUrl: str  # noqa: N815
+
+
+class Radio(BaseModel):
+    id: int  # noqa: A003
+    name: str
+    picUrl: str  # noqa: N815
+    desc: str
+    subCount: int  # noqa: N815
+    programCount: int  # noqa: N815
+    categoryId: int  # noqa: N815
+    secondCategoryId: Optional[int]  # noqa: N815
+    category: str
+    secondCategory: Optional[str]  # noqa: N815
+    lastProgramId: int  # noqa: N815
+
+
+class VoiceBaseInfo(BaseModel):
+    id: int  # noqa: A003
+    mainTrackId: int  # noqa: N815
+    name: str
+    coverUrl: str  # noqa: N815
+    description: str
+    dj: DJ
+    radio: Radio
+    duration: int
+    listenerCount: int  # noqa: N815
+    shareCount: int  # noqa: N815
+    likedCount: int  # noqa: N815
+    commentCount: int  # noqa: N815
+    commentThreadId: str  # noqa: N815
+
+
+class VoiceResource(BaseModel):
+    baseInfo: VoiceBaseInfo  # noqa: N815
+
+
+class VoiceSearchResult(BaseModel):
+    resources: List[VoiceResource]
+    totalCount: int  # noqa: N815
+    searchQcReminder: Optional[SearchQcReminder]  # noqa: N815
```

### Comparing `nonebot_plugin_multincm-0.2.5/nonebot_plugin_multincm/utils.py` & `nonebot_plugin_multincm-0.3.0/nonebot_plugin_multincm/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.2.5/pyproject.toml` & `nonebot_plugin_multincm-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-multincm"
-version = "0.2.5"
+version = "0.3.0"
 description = "NCM Song Searcher"
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0-rc.1",
     "nonebot-adapter-onebot>=2.2.0",
```

### Comparing `nonebot_plugin_multincm-0.2.5/PKG-INFO` & `nonebot_plugin_multincm-0.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-multincm
-Version: 0.2.5
+Version: 0.3.0
 Summary: NCM Song Searcher
 Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-multincm
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lgc-NB2Dev/nonebot-plugin-multincm
 Requires-Python: <4.0,>=3.8
 Requires-Dist: nonebot2>=2.0.0-rc.1
@@ -34,15 +34,15 @@
 
 <p>
   <img src="https://raw.githubusercontent.com/A-kirami/nonebot-plugin-template/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText">
 </p>
 
 # NoneBot-Plugin-MultiNCM
 
-_✨ NoneBot 插件简单描述 ✨_
+_✨ 网易云多选点歌 ✨_
 
 <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 <a href="https://pdm.fming.dev">
   <img src="https://img.shields.io/badge/pdm-managed-blueviolet" alt="pdm-managed">
 </a>
 <a href="https://wakatime.com/badge/user/b61b0f9a-f40b-4c82-bc51-0a75c67bfccf/project/f4778875-45a4-4688-8e1b-b8c844440abb">
   <img src="https://wakatime.com/badge/user/b61b0f9a-f40b-4c82-bc51-0a75c67bfccf/project/f4778875-45a4-4688-8e1b-b8c844440abb.svg" alt="wakatime">
@@ -62,18 +62,37 @@
 
 </div>
 
 ## 📖 介绍
 
 一个网易云多选点歌插件，可以翻页，可以登录网易云账号点 vip 歌曲听（插件发送的是自定义音乐卡片），没了
 
-### 歌曲列表效果图
+### 效果图
+
+<details>
+<summary>歌曲列表效果图（点击展开）</summary>
 
 ![pic](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/multincm/QQ图片20230515025601.jpg)
 
+</details>
+
+<details>
+<summary>电台列表效果图（点击展开）</summary>
+
+![pic](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/multincm/QQ图片20230519034438.jpg)
+
+</details>
+
+<details>
+<summary>歌词效果图（点击展开）</summary>
+
+![pic](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/multincm/QQ图片20230519034757.png)
+
+</details>
+
 ## 💿 安装
 
 以下提到的方法 任选**其一** 即可
 
 <details open>
 <summary>[推荐] 使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
@@ -154,39 +173,51 @@
 | `NCM_MAX_ARTIST_LEN` |  否  | `400`  | 歌曲列表中歌手列的最大文本宽度（像素）  |
 
 ## 🎉 使用
 
 ### 指令
 
 - 点歌 [歌曲名 / 音乐 ID]
-  - 介绍：顾名思义。当输入音乐 ID 时会直接发送对应音乐
+  - 介绍：搜索歌曲。当输入音乐 ID 时会直接发送对应音乐
   - 别名：`网易云`、`wyy`
-- 解析 <回复 音乐卡片 / 链接>
-  - 介绍：获取该音乐的播放链接并使用自定义卡片发送
+- 电台 [歌曲名 / 节目 ID]
+  - 介绍：搜索电台节目。当输入电台 ID 时会直接发送对应节目
+  - 别名：`声音`、`网易电台`、`wtdt`、`wydj`
+- 解析 [回复 音乐卡片 / 链接]
+  - 介绍：获取该 音乐 / 电台节目 的播放链接并使用自定义卡片发送
   - 别名：`resolve`、`parse`、`get`
-- 歌词 <回复 音乐卡片 / 链接>
+- 歌词 [回复 音乐卡片 / 链接]
   - 介绍：获取该音乐的歌词，以图片形式发送
   - 别名：`lrc`、`lyric`、`lyrics`
-- 链接 <回复 音乐卡片>
-  - 介绍：获取 Bot 发送的音乐卡片的网易云歌曲链接
-  - 别名：`link`
+- 链接 [回复 音乐卡片]
+  - 介绍：获取 Bot 发送的音乐卡片的网易云链接
+  - 别名：`link`、`url`
 
 ### Tip
 
 - 点击 Bot 发送的音乐卡片会跳转到音乐直链，可以直接下载
+- 使用需要回复音乐卡片的指令时，如果没有回复，会自动使用你触发发送的最近一个音乐卡片的信息
 
 ## 📞 联系
 
 QQ：3076823485  
 Telegram：[@lgc2333](https://t.me/lgc2333)  
 吹水群：[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp)  
 邮箱：<lgc2333@126.com>
 
 ## 💡 鸣谢
 
+### [mos9527/pyncm](https://github.com/mos9527/pyncm)
+
+项目使用的网易云 API 调用库
+
+### [Binaryify/NeteaseCloudMusicApi](https://github.com/Binaryify/NeteaseCloudMusicApi)
+
+项目电台相关 API 来源
+
 ### [MeetWq/pil-utils](https://github.com/MeetWq/pil-utils)
 
 超好用的 Pillow 辅助库
 
 ## 💰 赞助
 
 感谢大家的赞助！你们的赞助将是我继续创作的动力！
@@ -197,14 +228,18 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.3.0
+
+- 支持电台节目的解析与点播
+
 ### 0.2.5
 
 - `解析`、`歌词`、`链接` 指令可以直接根据 Bot 发送的上个音乐卡片作出回应了
 - 歌词解析会合并多行空行和去掉首尾空行了
 - 现在插件会定时清理自身内存中的缓存了
 
 ### 0.2.4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-multincm Version: 0.2.5 Summary: NCM
+Metadata-Version: 2.1 Name: nonebot-plugin-multincm Version: 0.3.0 Summary: NCM
 Song Searcher Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-multincm
 Author-Email: student_2333
 126.com> License: MIT Project-URL: Homepage, https://github.com/lgc-NB2Dev/
 nonebot-plugin-multincm Requires-Python: <4.0,>=3.8 Requires-Dist:
 nonebot2>=2.0.0-rc.1 Requires-Dist: nonebot-adapter-onebot>=2.2.0 Requires-
 Dist: pydantic>=1.10.4 Requires-Dist: pil-utils>=0.1.7 Requires-Dist:
 pyncm>=1.6.8.9.1 Requires-Dist: typing-extensions>=4.5.0 Requires-Dist:
@@ -10,30 +10,35 @@
 pip>=23.0.1; extra == "dev" Requires-Dist: setuptools>=67.6.1; extra == "dev"
 Requires-Dist: nb-cli>=1.0.5; extra == "dev" Requires-Dist: black>=23.3.0;
 extra == "dev" Requires-Dist: ruff>=0.0.260; extra == "dev" Requires-Dist:
 isort>=5.12.0; extra == "dev" Provides-Extra: dev Description-Content-Type:
 text/markdown
                               [NoneBotPluginLogo]
                               [NoneBotPluginText]
- # NoneBot-Plugin-MultiNCM _â¨ NoneBot æä»¶ç®åæè¿° â¨_ [python] [pdm-
+   # NoneBot-Plugin-MultiNCM _â¨ ç½æäºå¤éç¹æ­ â¨_ [python] [pdm-
                              managed] [wakatime]
                        [license] [pypi] [pypi_download]
 ## ð ä»ç»
 ä¸ä¸ªç½æäºå¤éç¹æ­æä»¶ï¼å¯ä»¥ç¿»é¡µï¼å¯ä»¥ç»å½ç½æäºè´¦å·ç¹
 vip æ­æ²å¬ï¼æä»¶åéçæ¯èªå®ä¹é³ä¹å¡çï¼ï¼æ²¡äº ###
-æ­æ²åè¡¨ææå¾ ![pic](https://raw.githubusercontent.com/lgc-NB2Dev/
-readme/main/multincm/QQå¾ç20230515025601.jpg) ## ð¿ å®è£
-ä»¥ä¸æå°çæ¹æ³ ä»»é**å¶ä¸** å³å¯  [æ¨è] ä½¿ç¨ nb-cli å®è£
-å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
-è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```bash nb plugin install nonebot-plugin-
-multincm ```   ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
-æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
-pip ```bash pip install nonebot-plugin-multincm ```   pdm ```bash pdm add
-nonebot-plugin-multincm ```   poetry ```bash poetry add nonebot-plugin-multincm
-```   conda ```bash conda install nonebot-plugin-multincm ```  æå¼ nonebot2
+ææå¾  æ­æ²åè¡¨ææå¾ï¼ç¹å»å±å¼ï¼ ![pic](https://
+raw.githubusercontent.com/lgc-NB2Dev/readme/main/multincm/
+QQå¾ç20230515025601.jpg)   çµå°åè¡¨ææå¾ï¼ç¹å»å±å¼ï¼ ![pic]
+(https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/multincm/
+QQå¾ç20230519034438.jpg)   æ­è¯ææå¾ï¼ç¹å»å±å¼ï¼ ![pic](https://
+raw.githubusercontent.com/lgc-NB2Dev/readme/main/multincm/
+QQå¾ç20230519034757.png)  ## ð¿ å®è£ ä»¥ä¸æå°çæ¹æ³
+ä»»é**å¶ä¸** å³å¯  [æ¨è] ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
+é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```bash nb
+plugin install nonebot-plugin-multincm ```   ä½¿ç¨åç®¡çå¨å®è£ å¨
+nonebot2 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡,
+æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤  pip ```bash pip
+install nonebot-plugin-multincm ```   pdm ```bash pdm add nonebot-plugin-
+multincm ```   poetry ```bash poetry add nonebot-plugin-multincm ```   conda
+```bash conda install nonebot-plugin-multincm ```  æå¼ nonebot2
 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åç
 `plugins` é¡¹éè¿½å åå¥ ```toml [tool.nonebot] plugins = [ # ...
 "nonebot_plugin_multincm" ] ```  ## âï¸ éç½® å¦æä½ å®è£äº [nonebot-
 plugin-ncm](https://github.com/kitUIN/nonebot-plugin-
 ncm)ï¼æ¬æä»¶ä¼ä¸å¶å±ç¨åä¸ä¸ª
 Sessionï¼å°±å¯ä»¥ä¸ç¨å¡«ä¸é¢çè´¦å·å¯ç äº
 ä¸é¢éç½®ä¸­ï¼ææºå·ç»å½ å é®ç®±ç»å½ãææå¯ç  å MD5
@@ -49,32 +54,39 @@
 `NCM_LIST_LIMIT` | å¦ | `20` | æ­æ²åè¡¨æ¯é¡µçæå¤§æ°é | |
 `NCM_LIST_FONT` | å¦ | æ  | æ¸²ææ­æ²åè¡¨ä½¿ç¨çå­ä½ | |
 `NCM_MAX_NAME_LEN` | å¦ | `600` |
 æ­æ²åè¡¨ä¸­æ­ååçæå¤§ææ¬å®½åº¦ï¼åç´ ï¼ | |
 `NCM_MAX_ARTIST_LEN` | å¦ | `400` |
 æ­æ²åè¡¨ä¸­æ­æåçæå¤§ææ¬å®½åº¦ï¼åç´ ï¼ | ## ð ä½¿ç¨ ###
 æä»¤ - ç¹æ­ [æ­æ²å / é³ä¹ ID] -
-ä»ç»ï¼é¡¾åæä¹ãå½è¾å¥é³ä¹ ID æ¶ä¼ç´æ¥åéå¯¹åºé³ä¹ -
-å«åï¼`ç½æäº`ã`wyy` - è§£æ <åå¤ é³ä¹å¡ç / é¾æ¥> -
-ä»ç»ï¼è·åè¯¥é³ä¹çæ­æ¾é¾æ¥å¹¶ä½¿ç¨èªå®ä¹å¡çåé -
-å«åï¼`resolve`ã`parse`ã`get` - æ­è¯ <åå¤ é³ä¹å¡ç / é¾æ¥> -
+ä»ç»ï¼æç´¢æ­æ²ãå½è¾å¥é³ä¹ ID æ¶ä¼ç´æ¥åéå¯¹åºé³ä¹ -
+å«åï¼`ç½æäº`ã`wyy` - çµå° [æ­æ²å / èç® ID] -
+ä»ç»ï¼æç´¢çµå°èç®ãå½è¾å¥çµå° ID æ¶ä¼ç´æ¥åéå¯¹åºèç®
+- å«åï¼`å£°é³`ã`ç½æçµå°`ã`wtdt`ã`wydj` - è§£æ [åå¤
+é³ä¹å¡ç / é¾æ¥] - ä»ç»ï¼è·åè¯¥ é³ä¹ / çµå°èç®
+çæ­æ¾é¾æ¥å¹¶ä½¿ç¨èªå®ä¹å¡çåé -
+å«åï¼`resolve`ã`parse`ã`get` - æ­è¯ [åå¤ é³ä¹å¡ç / é¾æ¥] -
 ä»ç»ï¼è·åè¯¥é³ä¹çæ­è¯ï¼ä»¥å¾çå½¢å¼åé -
-å«åï¼`lrc`ã`lyric`ã`lyrics` - é¾æ¥ <åå¤ é³ä¹å¡ç> -
-ä»ç»ï¼è·å Bot åéçé³ä¹å¡ççç½æäºæ­æ²é¾æ¥ -
-å«åï¼`link` ### Tip - ç¹å» Bot
-åéçé³ä¹å¡çä¼è·³è½¬å°é³ä¹ç´é¾ï¼å¯ä»¥ç´æ¥ä¸è½½ ## ð
-èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼
-[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
-126.com> ## ð¡ é¸£è°¢ ### [MeetWq/pil-utils](https://github.com/MeetWq/pil-
-utils) è¶å¥½ç¨ç Pillow è¾å©åº ## ð° èµå©
+å«åï¼`lrc`ã`lyric`ã`lyrics` - é¾æ¥ [åå¤ é³ä¹å¡ç] -
+ä»ç»ï¼è·å Bot åéçé³ä¹å¡ççç½æäºé¾æ¥ -
+å«åï¼`link`ã`url` ### Tip - ç¹å» Bot
+åéçé³ä¹å¡çä¼è·³è½¬å°é³ä¹ç´é¾ï¼å¯ä»¥ç´æ¥ä¸è½½ -
+ä½¿ç¨éè¦åå¤é³ä¹å¡ççæä»¤æ¶ï¼å¦ææ²¡æåå¤ï¼ä¼èªå¨ä½¿ç¨ä½ è§¦ååéçæè¿ä¸ä¸ªé³ä¹å¡ççä¿¡æ¯
+## ð èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333)
+å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
+126.com> ## ð¡ é¸£è°¢ ### [mos9527/pyncm](https://github.com/mos9527/pyncm)
+é¡¹ç®ä½¿ç¨çç½æäº API è°ç¨åº ### [Binaryify/NeteaseCloudMusicApi]
+(https://github.com/Binaryify/NeteaseCloudMusicApi) é¡¹ç®çµå°ç¸å³ API
+æ¥æº ### [MeetWq/pil-utils](https://github.com/MeetWq/pil-utils) è¶å¥½ç¨ç
+Pillow è¾å©åº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.2.5 -
-`è§£æ`ã`æ­è¯`ã`é¾æ¥` æä»¤å¯ä»¥ç´æ¥æ ¹æ® Bot
-åéçä¸ä¸ªé³ä¹å¡çä½åºååºäº -
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.3.0 -
+æ¯æçµå°èç®çè§£æä¸ç¹æ­ ### 0.2.5 - `è§£æ`ã`æ­è¯`ã`é¾æ¥`
+æä»¤å¯ä»¥ç´æ¥æ ¹æ® Bot åéçä¸ä¸ªé³ä¹å¡çä½åºååºäº -
 æ­è¯è§£æä¼åå¹¶å¤è¡ç©ºè¡åå»æé¦å°¾ç©ºè¡äº -
 ç°å¨æä»¶ä¼å®æ¶æ¸çèªèº«åå­ä¸­çç¼å­äº ### 0.2.4 -
 ä¿®å¤ä¸ä¸ªæ­è¯è§£æ bug ### 0.2.3 - å¾®è°æ­æ²åè¡¨æç -
 å¾®è°æä»¶å¸®å©ææ¬ ### 0.2.2 - ä¿®å¤ææ­ `KeyError` ### 0.2.1 -
 å é¤æ­è¯å°¾é¨çç©ºè¡ä¸å¤ä½åå²çº¿ ### 0.2.0 - æ°å¢äºä¸ä¸ªæä»¤
 `è§£æ`ã`æ­è¯`ã`é¾æ¥` - ç¹æ­æä»¤æ¯æç´æ¥è¾å¥é³ä¹ ID
```

