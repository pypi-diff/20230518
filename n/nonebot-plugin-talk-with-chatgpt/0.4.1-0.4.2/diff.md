# Comparing `tmp/nonebot_plugin_talk_with_chatgpt-0.4.1.tar.gz` & `tmp/nonebot_plugin_talk_with_chatgpt-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_talk_with_chatgpt-0.4.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_talk_with_chatgpt-0.4.2.tar", max compression
```

## Comparing `nonebot_plugin_talk_with_chatgpt-0.4.1.tar` & `nonebot_plugin_talk_with_chatgpt-0.4.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     8454 2023-04-22 14:28:18.532815 nonebot_plugin_talk_with_chatgpt-0.4.1/nonebot_plugin_talk_with_chatgpt/__init__.py
--rw-r--r--   0        0        0    13518 2023-04-22 14:27:21.436142 nonebot_plugin_talk_with_chatgpt-0.4.1/nonebot_plugin_talk_with_chatgpt/config.py
--rw-r--r--   0        0        0     5277 2023-04-21 09:07:58.978243 nonebot_plugin_talk_with_chatgpt-0.4.1/nonebot_plugin_talk_with_chatgpt/data_handle.py
--rw-r--r--   0        0        0      974 2023-04-22 14:28:28.184174 nonebot_plugin_talk_with_chatgpt-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     4834 2023-04-22 14:30:17.504552 nonebot_plugin_talk_with_chatgpt-0.4.1/README.md
--rw-r--r--   0        0        0     5767 1970-01-01 00:00:00.000000 nonebot_plugin_talk_with_chatgpt-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     8454 2023-04-22 14:28:18.532815 nonebot_plugin_talk_with_chatgpt-0.4.2/nonebot_plugin_talk_with_chatgpt/__init__.py
+-rw-r--r--   0        0        0    13518 2023-04-22 14:27:21.436142 nonebot_plugin_talk_with_chatgpt-0.4.2/nonebot_plugin_talk_with_chatgpt/config.py
+-rw-r--r--   0        0        0     5281 2023-05-18 02:26:25.865457 nonebot_plugin_talk_with_chatgpt-0.4.2/nonebot_plugin_talk_with_chatgpt/data_handle.py
+-rw-r--r--   0        0        0      974 2023-05-18 02:26:39.929502 nonebot_plugin_talk_with_chatgpt-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     4902 2023-05-18 02:26:59.624892 nonebot_plugin_talk_with_chatgpt-0.4.2/README.md
+-rw-r--r--   0        0        0     5831 1970-01-01 00:00:00.000000 nonebot_plugin_talk_with_chatgpt-0.4.2/PKG-INFO
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.4.1/nonebot_plugin_talk_with_chatgpt/__init__.py` & `nonebot_plugin_talk_with_chatgpt-0.4.2/nonebot_plugin_talk_with_chatgpt/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_chatgpt-0.4.1/nonebot_plugin_talk_with_chatgpt/config.py` & `nonebot_plugin_talk_with_chatgpt-0.4.2/nonebot_plugin_talk_with_chatgpt/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_chatgpt-0.4.1/nonebot_plugin_talk_with_chatgpt/data_handle.py` & `nonebot_plugin_talk_with_chatgpt-0.4.2/nonebot_plugin_talk_with_chatgpt/data_handle.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         # 尝试重命名（需api支持）
         if new_talk:
             await handle_req(id, "", "rename")
         result: str = json_data["message"]["content"]["parts"][0]
 
     except Exception as e:
         # 会话丢失
-        if "Conversation not found" in err_msg:
+        if resp_code == 404 and "found" in err_msg:
             # 清空会话id
             var.session_data[id][0] = ""
             var.session_data[id][1] = ""
             return await handle_req(id, req_text, operation)
         # 冲突，等待2秒再尝试
         if "Only one message at a time" in err_msg:
             await sleep(2)
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.4.1/pyproject.toml` & `nonebot_plugin_talk_with_chatgpt-0.4.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_talk_with_chatgpt"
-version = "0.4.1"
+version = "0.4.2"
 description = "Nonebot2 基于accessToken登录的ChatGPT聊天插件"
 authors = ["nikissXI <1299577815@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_talk_with_chatgpt"}]
 homepage = "https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_chatgpt"
 repository = "https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_chatgpt"
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.4.1/README.md` & `nonebot_plugin_talk_with_chatgpt-0.4.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 # 只允许超级管理员修改预设
 talk_with_chatgpt_prompt_admin_only = true
 ```
 
 #### 如果要修改触发命令就填
 ```bash
 # 触发对话的命令前缀，默认群聊直接艾特也可以触发
-talk_with_chatgpt_start_cmd = /talk
+talk_with_chatgpt_talk_cmd = /talk
 # 群聊艾特是否响应
 talk_with_chatgpt_talk_at = true
 # 私聊沉浸式对话触发命令
 talk_with_chatgpt_talk_p_cmd = /hi
 # 重置对话的命令，就是清空聊天记录
 talk_with_chatgpt_reset_cmd = /reset
 # 设置预设的命令前缀
@@ -98,14 +98,18 @@
 |:-----:|:----:|
 | /talk | 开始对话，默认群里@机器人也可以 |
 | /hi | 沉浸式对话（仅限私聊） |
 | /clear | 重置对话（不会重置预设） |
 | /prompt | 设置预设（人格），设置后会重置对话 |
 
 ## 更新日志
+### 2023/5/18 \[v0.4.2]
+
+* 修复会话丢失不重置的问题
+
 ### 2023/4/22 \[v0.4.1]
 
 * 增加群聊at触发开关
 
 ### 2023/4/21 \[v0.4.0]
 
 * 更换了默认API，暂时能用，建议还是自己搭建API
```

#### html2text {}

```diff
@@ -28,15 +28,15 @@
 é»è®¤æ ä»£çï¼è§apiæåµçæ¯å¦éè¦æ¢¯å­ãè¿ä¸ªåç½®çåä»£ææµè¿æ¯ä¸éè¦æ¢¯å­çã
 talk_with_chatgpt_http_proxy = null # å¤çæ¶æ¯æ¶æ¯å¦æç¤º
 talk_with_chatgpt_reply_notice = true # ç¾¤èæ¯å¦å±äº«ä¼è¯
 talk_with_chatgpt_group_share = false # åªåè®¸è¶çº§ç®¡çåä¿®æ¹é¢è®¾
 talk_with_chatgpt_prompt_admin_only = true ``` ####
 å¦æè¦ä¿®æ¹è§¦åå½ä»¤å°±å¡« ```bash #
 è§¦åå¯¹è¯çå½ä»¤åç¼ï¼é»è®¤ç¾¤èç´æ¥è¾ç¹ä¹å¯ä»¥è§¦å
-talk_with_chatgpt_start_cmd = /talk # ç¾¤èè¾ç¹æ¯å¦ååº
+talk_with_chatgpt_talk_cmd = /talk # ç¾¤èè¾ç¹æ¯å¦ååº
 talk_with_chatgpt_talk_at = true # ç§èæ²æµ¸å¼å¯¹è¯è§¦åå½ä»¤
 talk_with_chatgpt_talk_p_cmd = /hi #
 éç½®å¯¹è¯çå½ä»¤ï¼å°±æ¯æ¸ç©ºèå¤©è®°å½ talk_with_chatgpt_reset_cmd =
 /reset # è®¾ç½®é¢è®¾çå½ä»¤åç¼ talk_with_chatgpt_prompt_cmd = /prompt ```
 #### å¤§æ¦çç¨ä¸ä¸çéå¡«é¡¹ ```bash #
 è¯·æ±è¶æ¶æ¶é´ï¼åç­çæçæ¶é´ä¹è¦ç®å¨è¿éé¢çï¼æä»¥ä¸è½å¤ªç­ï¼é»è®¤60ç§
 talk_with_chatgpt_timeout = 60 # chatgptæ¨¡åï¼é»è®¤ text-davinci-002-
@@ -50,12 +50,13 @@
 æä»¶æ°æ®æä»¶åï¼é»è®¤./data/talk_with_chatgpt.json
 talk_with_chatgpt_data = talk_with_chatgpt.json ``` ##
 æä»¶å½ä»¤ï¼åå¯ä¿®æ¹ï¼ï¼ | æä»¤ | è¯´æ | |:-----:|:----:| | /talk
 | å¼å§å¯¹è¯ï¼é»è®¤ç¾¤é@æºå¨äººä¹å¯ä»¥ | | /hi |
 æ²æµ¸å¼å¯¹è¯ï¼ä»éç§èï¼ | | /clear |
 éç½®å¯¹è¯ï¼ä¸ä¼éç½®é¢è®¾ï¼ | | /prompt |
 è®¾ç½®é¢è®¾ï¼äººæ ¼ï¼ï¼è®¾ç½®åä¼éç½®å¯¹è¯ | ## æ´æ°æ¥å¿ ### 2023/
-4/22 \[v0.4.1] * å¢å ç¾¤èatè§¦åå¼å³ ### 2023/4/21 \[v0.4.0] *
+5/18 \[v0.4.2] * ä¿®å¤ä¼è¯ä¸¢å¤±ä¸éç½®çé®é¢ ### 2023/4/22 \[v0.4.1] *
+å¢å ç¾¤èatè§¦åå¼å³ ### 2023/4/21 \[v0.4.0] *
 æ´æ¢äºé»è®¤APIï¼ææ¶è½ç¨ï¼å»ºè®®è¿æ¯èªå·±æ­å»ºAPI *
 æ°å¢å¤é¢è®¾åè½ï¼åç½®ä¸ä¸ªé¢è®¾ï¼ç«å¨ãé­é­ãå¼åèæ¨¡å¼
 * å¢å ç§èæ²æµ¸å¼å¯¹è¯ * ä¼åå¤§éç»è ### 2023/4/11 \[v0.2.3] *
 åå¸ç¬¬ä¸çè¾ç®éçæä»¶ï¼å¹¶ä¿®å¤äºäºå°é®é¢ï¼ç»èå¾éè¦
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.4.1/PKG-INFO` & `nonebot_plugin_talk_with_chatgpt-0.4.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-talk-with-chatgpt
-Version: 0.4.1
+Version: 0.4.2
 Summary: Nonebot2 基于accessToken登录的ChatGPT聊天插件
 Home-page: https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_chatgpt
 License: MIT
 Author: nikissXI
 Author-email: 1299577815@qq.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -86,15 +86,15 @@
 # 只允许超级管理员修改预设
 talk_with_chatgpt_prompt_admin_only = true
 ```
 
 #### 如果要修改触发命令就填
 ```bash
 # 触发对话的命令前缀，默认群聊直接艾特也可以触发
-talk_with_chatgpt_start_cmd = /talk
+talk_with_chatgpt_talk_cmd = /talk
 # 群聊艾特是否响应
 talk_with_chatgpt_talk_at = true
 # 私聊沉浸式对话触发命令
 talk_with_chatgpt_talk_p_cmd = /hi
 # 重置对话的命令，就是清空聊天记录
 talk_with_chatgpt_reset_cmd = /reset
 # 设置预设的命令前缀
@@ -121,14 +121,18 @@
 |:-----:|:----:|
 | /talk | 开始对话，默认群里@机器人也可以 |
 | /hi | 沉浸式对话（仅限私聊） |
 | /clear | 重置对话（不会重置预设） |
 | /prompt | 设置预设（人格），设置后会重置对话 |
 
 ## 更新日志
+### 2023/5/18 \[v0.4.2]
+
+* 修复会话丢失不重置的问题
+
 ### 2023/4/22 \[v0.4.1]
 
 * 增加群聊at触发开关
 
 ### 2023/4/21 \[v0.4.0]
 
 * 更换了默认API，暂时能用，建议还是自己搭建API
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-talk-with-chatgpt Version: 0.4.1
+Metadata-Version: 2.1 Name: nonebot-plugin-talk-with-chatgpt Version: 0.4.2
 Summary: Nonebot2 åºäºaccessTokenç»å½çChatGPTèå¤©æä»¶ Home-page:
 https://github.com/nikissXI/nonebot_plugins/tree/main/
 nonebot_plugin_talk_with_chatgpt License: MIT Author: nikissXI Author-email:
 1299577815@qq.com Requires-Python: >=3.8 Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
@@ -43,15 +43,15 @@
 é»è®¤æ ä»£çï¼è§apiæåµçæ¯å¦éè¦æ¢¯å­ãè¿ä¸ªåç½®çåä»£ææµè¿æ¯ä¸éè¦æ¢¯å­çã
 talk_with_chatgpt_http_proxy = null # å¤çæ¶æ¯æ¶æ¯å¦æç¤º
 talk_with_chatgpt_reply_notice = true # ç¾¤èæ¯å¦å±äº«ä¼è¯
 talk_with_chatgpt_group_share = false # åªåè®¸è¶çº§ç®¡çåä¿®æ¹é¢è®¾
 talk_with_chatgpt_prompt_admin_only = true ``` ####
 å¦æè¦ä¿®æ¹è§¦åå½ä»¤å°±å¡« ```bash #
 è§¦åå¯¹è¯çå½ä»¤åç¼ï¼é»è®¤ç¾¤èç´æ¥è¾ç¹ä¹å¯ä»¥è§¦å
-talk_with_chatgpt_start_cmd = /talk # ç¾¤èè¾ç¹æ¯å¦ååº
+talk_with_chatgpt_talk_cmd = /talk # ç¾¤èè¾ç¹æ¯å¦ååº
 talk_with_chatgpt_talk_at = true # ç§èæ²æµ¸å¼å¯¹è¯è§¦åå½ä»¤
 talk_with_chatgpt_talk_p_cmd = /hi #
 éç½®å¯¹è¯çå½ä»¤ï¼å°±æ¯æ¸ç©ºèå¤©è®°å½ talk_with_chatgpt_reset_cmd =
 /reset # è®¾ç½®é¢è®¾çå½ä»¤åç¼ talk_with_chatgpt_prompt_cmd = /prompt ```
 #### å¤§æ¦çç¨ä¸ä¸çéå¡«é¡¹ ```bash #
 è¯·æ±è¶æ¶æ¶é´ï¼åç­çæçæ¶é´ä¹è¦ç®å¨è¿éé¢çï¼æä»¥ä¸è½å¤ªç­ï¼é»è®¤60ç§
 talk_with_chatgpt_timeout = 60 # chatgptæ¨¡åï¼é»è®¤ text-davinci-002-
@@ -65,12 +65,13 @@
 æä»¶æ°æ®æä»¶åï¼é»è®¤./data/talk_with_chatgpt.json
 talk_with_chatgpt_data = talk_with_chatgpt.json ``` ##
 æä»¶å½ä»¤ï¼åå¯ä¿®æ¹ï¼ï¼ | æä»¤ | è¯´æ | |:-----:|:----:| | /talk
 | å¼å§å¯¹è¯ï¼é»è®¤ç¾¤é@æºå¨äººä¹å¯ä»¥ | | /hi |
 æ²æµ¸å¼å¯¹è¯ï¼ä»éç§èï¼ | | /clear |
 éç½®å¯¹è¯ï¼ä¸ä¼éç½®é¢è®¾ï¼ | | /prompt |
 è®¾ç½®é¢è®¾ï¼äººæ ¼ï¼ï¼è®¾ç½®åä¼éç½®å¯¹è¯ | ## æ´æ°æ¥å¿ ### 2023/
-4/22 \[v0.4.1] * å¢å ç¾¤èatè§¦åå¼å³ ### 2023/4/21 \[v0.4.0] *
+5/18 \[v0.4.2] * ä¿®å¤ä¼è¯ä¸¢å¤±ä¸éç½®çé®é¢ ### 2023/4/22 \[v0.4.1] *
+å¢å ç¾¤èatè§¦åå¼å³ ### 2023/4/21 \[v0.4.0] *
 æ´æ¢äºé»è®¤APIï¼ææ¶è½ç¨ï¼å»ºè®®è¿æ¯èªå·±æ­å»ºAPI *
 æ°å¢å¤é¢è®¾åè½ï¼åç½®ä¸ä¸ªé¢è®¾ï¼ç«å¨ãé­é­ãå¼åèæ¨¡å¼
 * å¢å ç§èæ²æµ¸å¼å¯¹è¯ * ä¼åå¤§éç»è ### 2023/4/11 \[v0.2.3] *
 åå¸ç¬¬ä¸çè¾ç®éçæä»¶ï¼å¹¶ä¿®å¤äºäºå°é®é¢ï¼ç»èå¾éè¦
```

