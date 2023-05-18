# Comparing `tmp/quickstart_rhy-0.7.1.tar.gz` & `tmp/quickstart_rhy-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstart_rhy-0.7.1.tar", max compression
+gzip compressed data, was "quickstart_rhy-0.7.2.tar", max compression
```

## Comparing `quickstart_rhy-0.7.1.tar` & `quickstart_rhy-0.7.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1067 2019-09-20 01:32:29.136250 quickstart_rhy-0.7.1/LICENSE
--rw-r--r--   0        0        0     5952 2023-02-05 05:20:04.108908 quickstart_rhy-0.7.1/QuickStart_Rhy/API/AliCloud.py
--rw-r--r--   0        0        0     3525 2023-03-27 00:35:40.568103 quickstart_rhy-0.7.1/QuickStart_Rhy/API/BaiduCloud.py
--rw-r--r--   0        0        0     3419 2023-04-15 03:33:34.034264 quickstart_rhy-0.7.1/QuickStart_Rhy/API/ChatGPT.py
--rw-r--r--   0        0        0      462 2023-02-24 04:34:17.917996 quickstart_rhy-0.7.1/QuickStart_Rhy/API/DeepL.py
--rw-r--r--   0        0        0      778 2023-04-28 07:11:41.378497 quickstart_rhy-0.7.1/QuickStart_Rhy/API/DeepLX.py
--rw-r--r--   0        0        0     1191 2023-04-30 06:41:55.816233 quickstart_rhy-0.7.1/QuickStart_Rhy/API/Lolicon.py
--rw-r--r--   0        0        0     6264 2023-01-22 11:43:21.457920 quickstart_rhy-0.7.1/QuickStart_Rhy/API/QiniuOSS.py
--rw-r--r--   0        0        0     9434 2023-01-22 17:11:40.937202 quickstart_rhy-0.7.1/QuickStart_Rhy/API/SimpleAPI.py
--rw-r--r--   0        0        0     7276 2023-02-22 02:46:13.021767 quickstart_rhy-0.7.1/QuickStart_Rhy/API/TencentCloud.py
--rw-r--r--   0        0        0     1701 2023-03-04 05:55:10.455205 quickstart_rhy-0.7.1/QuickStart_Rhy/API/__init__.py
--rw-r--r--   0        0        0    16615 2023-02-22 02:45:56.238555 quickstart_rhy-0.7.1/QuickStart_Rhy/API/alapi.py
--rw-r--r--   0        0        0     2420 2023-01-16 11:59:57.162445 quickstart_rhy-0.7.1/QuickStart_Rhy/ImageTools/ColorTools.py
--rw-r--r--   0        0        0    13292 2023-04-18 12:58:33.288943 quickstart_rhy-0.7.1/QuickStart_Rhy/ImageTools/ImagePreview.py
--rw-r--r--   0        0        0     3805 2023-04-18 12:54:35.211459 quickstart_rhy-0.7.1/QuickStart_Rhy/ImageTools/ImageTools.py
--rw-r--r--   0        0        0     4035 2023-01-16 12:04:31.734545 quickstart_rhy-0.7.1/QuickStart_Rhy/ImageTools/VideoTools.py
--rw-r--r--   0        0        0       75 2021-01-14 15:40:19.416041 quickstart_rhy-0.7.1/QuickStart_Rhy/ImageTools/__init__.py
--rw-r--r--   0        0        0     1768 2022-11-18 20:23:12.379800 quickstart_rhy-0.7.1/QuickStart_Rhy/NetTools/HttpServer.py
--rw-r--r--   0        0        0     5133 2023-01-22 12:27:25.009662 quickstart_rhy-0.7.1/QuickStart_Rhy/NetTools/M3u8DL.py
--rw-r--r--   0        0        0     9151 2023-04-24 09:10:36.431917 quickstart_rhy-0.7.1/QuickStart_Rhy/NetTools/MultiSingleDL.py
--rw-r--r--   0        0        0    14748 2023-04-04 03:26:04.977775 quickstart_rhy-0.7.1/QuickStart_Rhy/NetTools/NormalDL.py
--rw-r--r--   0        0        0     3818 2022-11-18 20:23:25.282202 quickstart_rhy-0.7.1/QuickStart_Rhy/NetTools/WiFi.py
--rw-r--r--   0        0        0     3227 2022-11-18 20:23:28.660759 quickstart_rhy-0.7.1/QuickStart_Rhy/NetTools/WiFiDarwin.py
--rw-r--r--   0        0        0     6001 2023-02-16 12:56:59.801774 quickstart_rhy-0.7.1/QuickStart_Rhy/NetTools/__init__.py
--rw-r--r--   0        0        0     1075 2023-05-04 07:12:24.212283 quickstart_rhy-0.7.1/QuickStart_Rhy/NumbaTools/__init__.py
--rw-r--r--   0        0        0     8935 2023-01-16 13:31:49.562044 quickstart_rhy-0.7.1/QuickStart_Rhy/SystemTools/Compress.py
--rw-r--r--   0        0        0     5145 2023-01-16 13:34:40.162030 quickstart_rhy-0.7.1/QuickStart_Rhy/SystemTools/Diff.py
--rw-r--r--   0        0        0     1377 2022-11-18 19:05:09.495382 quickstart_rhy-0.7.1/QuickStart_Rhy/SystemTools/DiskMac.py
--rw-r--r--   0        0        0     1130 2022-11-18 20:23:45.475865 quickstart_rhy-0.7.1/QuickStart_Rhy/SystemTools/FileHash.py
--rw-r--r--   0        0        0      795 2023-01-29 05:36:58.386300 quickstart_rhy-0.7.1/QuickStart_Rhy/SystemTools/__init__.py
--rw-r--r--   0        0        0     3255 2023-01-17 09:56:11.282076 quickstart_rhy-0.7.1/QuickStart_Rhy/ThreadTools/__init__.py
--rw-r--r--   0        0        0     1603 2023-04-22 06:36:51.515102 quickstart_rhy-0.7.1/QuickStart_Rhy/TuiTools/Bar.py
--rw-r--r--   0        0        0     1268 2022-11-18 20:24:15.189225 quickstart_rhy-0.7.1/QuickStart_Rhy/TuiTools/Line.py
--rw-r--r--   0        0        0     1753 2023-01-16 10:23:26.070865 quickstart_rhy-0.7.1/QuickStart_Rhy/TuiTools/Table.py
--rw-r--r--   0        0        0       18 2022-05-03 07:21:41.109725 quickstart_rhy-0.7.1/QuickStart_Rhy/TuiTools/__init__.py
--rw-r--r--   0        0        0     3782 2023-01-22 07:37:58.889811 quickstart_rhy-0.7.1/QuickStart_Rhy/Wrapper/__init__.py
--rw-r--r--   0        0        0      772 2022-11-18 20:24:38.518900 quickstart_rhy-0.7.1/QuickStart_Rhy/__cache__.py
--rw-r--r--   0        0        0     8625 2023-05-04 11:46:15.495588 quickstart_rhy-0.7.1/QuickStart_Rhy/__config__.py
--rw-r--r--   0        0        0    14948 2023-05-04 11:44:40.865270 quickstart_rhy-0.7.1/QuickStart_Rhy/__init__.py
--rw-r--r--   0        0        0    38783 2023-05-04 11:22:21.159295 quickstart_rhy-0.7.1/QuickStart_Rhy/apiTools.py
--rw-r--r--   0        0        0     6720 2023-05-04 11:42:01.250240 quickstart_rhy-0.7.1/QuickStart_Rhy/funcList.py
--rw-r--r--   0        0        0     5844 2023-04-18 12:49:20.558808 quickstart_rhy-0.7.1/QuickStart_Rhy/imageDeal.py
--rw-r--r--   0        0        0    35036 2023-05-04 11:39:59.498252 quickstart_rhy-0.7.1/QuickStart_Rhy/lang.json
--rw-r--r--   0        0        0     1728 2023-05-04 11:40:39.962676 quickstart_rhy-0.7.1/QuickStart_Rhy/main.py
--rw-r--r--   0        0        0    11808 2023-05-04 08:04:12.459408 quickstart_rhy-0.7.1/QuickStart_Rhy/netTools.py
--rw-r--r--   0        0        0     1957 2023-01-22 12:33:43.387980 quickstart_rhy-0.7.1/QuickStart_Rhy/qsLesson.py
--rw-r--r--   0        0        0     6096 2023-03-16 03:09:08.732591 quickstart_rhy-0.7.1/QuickStart_Rhy/system.py
--rw-r--r--   0        0        0      701 2023-01-16 10:30:39.811901 quickstart_rhy-0.7.1/README.md
--rw-r--r--   0        0        0      548 2023-05-04 11:48:24.493927 quickstart_rhy-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     1846 1970-01-01 00:00:00.000000 quickstart_rhy-0.7.1/setup.py
--rw-r--r--   0        0        0     1488 1970-01-01 00:00:00.000000 quickstart_rhy-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2019-09-20 01:32:29.136250 quickstart_rhy-0.7.2/LICENSE
+-rw-r--r--   0        0        0     5952 2023-02-05 05:20:04.108908 quickstart_rhy-0.7.2/QuickStart_Rhy/API/AliCloud.py
+-rw-r--r--   0        0        0     3525 2023-03-27 00:35:40.568103 quickstart_rhy-0.7.2/QuickStart_Rhy/API/BaiduCloud.py
+-rw-r--r--   0        0        0     4041 2023-05-18 09:09:18.744642 quickstart_rhy-0.7.2/QuickStart_Rhy/API/ChatGPT.py
+-rw-r--r--   0        0        0      462 2023-02-24 04:34:17.917996 quickstart_rhy-0.7.2/QuickStart_Rhy/API/DeepL.py
+-rw-r--r--   0        0        0     1221 2023-05-18 04:35:41.557810 quickstart_rhy-0.7.2/QuickStart_Rhy/API/DeepLX.py
+-rw-r--r--   0        0        0     1191 2023-04-30 06:41:55.816233 quickstart_rhy-0.7.2/QuickStart_Rhy/API/Lolicon.py
+-rw-r--r--   0        0        0     6264 2023-01-22 11:43:21.457920 quickstart_rhy-0.7.2/QuickStart_Rhy/API/QiniuOSS.py
+-rw-r--r--   0        0        0     9434 2023-01-22 17:11:40.937202 quickstart_rhy-0.7.2/QuickStart_Rhy/API/SimpleAPI.py
+-rw-r--r--   0        0        0     7276 2023-02-22 02:46:13.021767 quickstart_rhy-0.7.2/QuickStart_Rhy/API/TencentCloud.py
+-rw-r--r--   0        0        0     1701 2023-03-04 05:55:10.455205 quickstart_rhy-0.7.2/QuickStart_Rhy/API/__init__.py
+-rw-r--r--   0        0        0    16615 2023-02-22 02:45:56.238555 quickstart_rhy-0.7.2/QuickStart_Rhy/API/alapi.py
+-rw-r--r--   0        0        0     2420 2023-01-16 11:59:57.162445 quickstart_rhy-0.7.2/QuickStart_Rhy/ImageTools/ColorTools.py
+-rw-r--r--   0        0        0    13292 2023-04-18 12:58:33.288943 quickstart_rhy-0.7.2/QuickStart_Rhy/ImageTools/ImagePreview.py
+-rw-r--r--   0        0        0     3805 2023-04-18 12:54:35.211459 quickstart_rhy-0.7.2/QuickStart_Rhy/ImageTools/ImageTools.py
+-rw-r--r--   0        0        0     4035 2023-01-16 12:04:31.734545 quickstart_rhy-0.7.2/QuickStart_Rhy/ImageTools/VideoTools.py
+-rw-r--r--   0        0        0       75 2021-01-14 15:40:19.416041 quickstart_rhy-0.7.2/QuickStart_Rhy/ImageTools/__init__.py
+-rw-r--r--   0        0        0     1768 2022-11-18 20:23:12.379800 quickstart_rhy-0.7.2/QuickStart_Rhy/NetTools/HttpServer.py
+-rw-r--r--   0        0        0     5133 2023-01-22 12:27:25.009662 quickstart_rhy-0.7.2/QuickStart_Rhy/NetTools/M3u8DL.py
+-rw-r--r--   0        0        0     9151 2023-04-24 09:10:36.431917 quickstart_rhy-0.7.2/QuickStart_Rhy/NetTools/MultiSingleDL.py
+-rw-r--r--   0        0        0    14748 2023-04-04 03:26:04.977775 quickstart_rhy-0.7.2/QuickStart_Rhy/NetTools/NormalDL.py
+-rw-r--r--   0        0        0     3818 2022-11-18 20:23:25.282202 quickstart_rhy-0.7.2/QuickStart_Rhy/NetTools/WiFi.py
+-rw-r--r--   0        0        0     3227 2022-11-18 20:23:28.660759 quickstart_rhy-0.7.2/QuickStart_Rhy/NetTools/WiFiDarwin.py
+-rw-r--r--   0        0        0     6001 2023-02-16 12:56:59.801774 quickstart_rhy-0.7.2/QuickStart_Rhy/NetTools/__init__.py
+-rw-r--r--   0        0        0     1075 2023-05-04 07:12:24.212283 quickstart_rhy-0.7.2/QuickStart_Rhy/NumbaTools/__init__.py
+-rw-r--r--   0        0        0     8935 2023-01-16 13:31:49.562044 quickstart_rhy-0.7.2/QuickStart_Rhy/SystemTools/Compress.py
+-rw-r--r--   0        0        0     5145 2023-01-16 13:34:40.162030 quickstart_rhy-0.7.2/QuickStart_Rhy/SystemTools/Diff.py
+-rw-r--r--   0        0        0     1377 2022-11-18 19:05:09.495382 quickstart_rhy-0.7.2/QuickStart_Rhy/SystemTools/DiskMac.py
+-rw-r--r--   0        0        0     1130 2022-11-18 20:23:45.475865 quickstart_rhy-0.7.2/QuickStart_Rhy/SystemTools/FileHash.py
+-rw-r--r--   0        0        0      795 2023-01-29 05:36:58.386300 quickstart_rhy-0.7.2/QuickStart_Rhy/SystemTools/__init__.py
+-rw-r--r--   0        0        0     3255 2023-01-17 09:56:11.282076 quickstart_rhy-0.7.2/QuickStart_Rhy/ThreadTools/__init__.py
+-rw-r--r--   0        0        0     1603 2023-04-22 06:36:51.515102 quickstart_rhy-0.7.2/QuickStart_Rhy/TuiTools/Bar.py
+-rw-r--r--   0        0        0     1268 2022-11-18 20:24:15.189225 quickstart_rhy-0.7.2/QuickStart_Rhy/TuiTools/Line.py
+-rw-r--r--   0        0        0     1753 2023-01-16 10:23:26.070865 quickstart_rhy-0.7.2/QuickStart_Rhy/TuiTools/Table.py
+-rw-r--r--   0        0        0       18 2022-05-03 07:21:41.109725 quickstart_rhy-0.7.2/QuickStart_Rhy/TuiTools/__init__.py
+-rw-r--r--   0        0        0     3782 2023-01-22 07:37:58.889811 quickstart_rhy-0.7.2/QuickStart_Rhy/Wrapper/__init__.py
+-rw-r--r--   0        0        0      772 2022-11-18 20:24:38.518900 quickstart_rhy-0.7.2/QuickStart_Rhy/__cache__.py
+-rw-r--r--   0        0        0     8625 2023-05-04 11:46:15.495588 quickstart_rhy-0.7.2/QuickStart_Rhy/__config__.py
+-rw-r--r--   0        0        0    14948 2023-05-04 11:44:40.865270 quickstart_rhy-0.7.2/QuickStart_Rhy/__init__.py
+-rw-r--r--   0        0        0    38978 2023-05-15 09:52:32.288702 quickstart_rhy-0.7.2/QuickStart_Rhy/apiTools.py
+-rw-r--r--   0        0        0     6720 2023-05-04 11:42:01.250240 quickstart_rhy-0.7.2/QuickStart_Rhy/funcList.py
+-rw-r--r--   0        0        0     5844 2023-04-18 12:49:20.558808 quickstart_rhy-0.7.2/QuickStart_Rhy/imageDeal.py
+-rw-r--r--   0        0        0    35036 2023-05-18 15:01:45.230103 quickstart_rhy-0.7.2/QuickStart_Rhy/lang.json
+-rw-r--r--   0        0        0     1729 2023-05-18 14:59:51.881230 quickstart_rhy-0.7.2/QuickStart_Rhy/main.py
+-rw-r--r--   0        0        0    11808 2023-05-04 08:04:12.459408 quickstart_rhy-0.7.2/QuickStart_Rhy/netTools.py
+-rw-r--r--   0        0        0     1957 2023-01-22 12:33:43.387980 quickstart_rhy-0.7.2/QuickStart_Rhy/qsLesson.py
+-rw-r--r--   0        0        0     6096 2023-03-16 03:09:08.732591 quickstart_rhy-0.7.2/QuickStart_Rhy/system.py
+-rw-r--r--   0        0        0      701 2023-01-16 10:30:39.811901 quickstart_rhy-0.7.2/README.md
+-rw-r--r--   0        0        0      548 2023-05-18 15:02:23.884592 quickstart_rhy-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     1846 1970-01-01 00:00:00.000000 quickstart_rhy-0.7.2/setup.py
+-rw-r--r--   0        0        0     1488 1970-01-01 00:00:00.000000 quickstart_rhy-0.7.2/PKG-INFO
```

### Comparing `quickstart_rhy-0.7.1/LICENSE` & `quickstart_rhy-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/API/AliCloud.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/API/AliCloud.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/API/BaiduCloud.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/API/BaiduCloud.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/API/ChatGPT.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/API/ChatGPT.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from .. import requirePackage, user_lang
+from .. import requirePackage, user_lang, qs_default_console, qs_error_string
 from . import pre_check
+import time
 
 lang_table = {
     'zh': 'Chinese',
     'en': 'English',
     'fra': 'French',
     'ru': 'Russian',
     'spa': 'Spanish',
@@ -17,17 +18,22 @@
     import json
 
 
 _chatbot = None
 
 
 class AlapiChatbot:
-    def __init__(self, system_prompt=f"You are ChatGPT, a large language model trained by OpenAI. Respond conversationally with Markdown format and using {lang_table[user_lang]} Language."):
+    def __init__(
+            self, 
+            system_prompt=f"You are ChatGPT, a large language model trained by OpenAI. Respond conversationally with Markdown format and using {lang_table[user_lang]} Language.",
+            no_record: bool = False
+        ):
         from .alapi import alapi_token, v2_url
 
+        self.no_record = no_record
         self.api_key = alapi_token
         self.url = v2_url
         self.messages = [
             {
                 "role": "system",
                 "content": system_prompt,
             }
@@ -36,32 +42,38 @@
     def ask(self, prompt):
         self.messages.append(
             {
                 "role": "user",
                 "content": prompt,
             }
         )
-        res = (
+        while res := (
             requests.post(
                 self.url + "chatgpt/pro",
                 json={
                     "token": self.api_key,
                     "message": self.messages,
                 },
             )
             .json()
-            .get("data")
-            .get("content")
-        )
-        self.messages.append(
-            {
-                "role": "assistant",
-                "content": res,
-            }
-        )
+        ):
+            if res['code'] == 422 or not res.get('data'):
+                qs_default_console.print(qs_error_string, res)
+                time.sleep(3)
+                continue
+            else:
+                break
+        res = res.get("data").get("content")
+        if not self.no_record:
+            self.messages.append(
+                {
+                    "role": "assistant",
+                    "content": res,
+                }
+            )
         return res
 
     def ask_stream(self, prompt):  # not support now
         self.messages.append(
             {
                 "role": "user",
                 "content": prompt,
@@ -81,25 +93,26 @@
             if not line:
                 continue
             res = json.loads(line)
             if res['success']:
                 total_res = res['text']
                 yield total_res
 
-        self.messages.append(
-            {
-                "role": "assistant",
-                "content": total_res,
-            }
-        )
+        if not self.no_record:
+            self.messages.append(
+                {
+                    "role": "assistant",
+                    "content": total_res,
+                }
+            )
 
 
-def create_bot():
+def create_bot(no_record: bool = False):
     if ALAPI:
-        return AlapiChatbot()
+        return AlapiChatbot(no_record=no_record)
     else:
         return (
             requirePackage("revChatGPT.V3", "Chatbot", "revChatGPT")(
                 API_KEY,
                 system_prompt=f"You are ChatGPT, a large language model trained by OpenAI. Respond conversationally with Markdown format and using {lang_table[user_lang]} Language.",
             )
             if API_KEY
@@ -112,21 +125,23 @@
             )
         )
 
 
 def chatGPT(
     prompt: str,
     wait_all: bool = False,
+    no_record: bool = False,
 ):
     """
     使用OpenAI的GPT-3 API进行聊天
 
     :param prompt: 聊天内容
     :param wait_all: 是否等待所有内容
+    :param no_record: 是否不记录聊天内容
     """
     global _chatbot
     if _chatbot is None:
-        _chatbot = create_bot()
+        _chatbot = create_bot(no_record=no_record)
     if wait_all:
         return _chatbot.ask(prompt)
     else:
         return _chatbot.ask_stream(prompt)
```

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/API/DeepLX.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/API/DeepLX.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from . import pre_check, user_lang
 import requests
+import random
 
 url = pre_check("DeepLX")
 
 if isinstance(url, list):
-    _load_balancer_ = -1
+    _load_balancer_ = random.randint(0, len(url) - 1)
 
 def get_url():
     """获取当前使用的API地址"""
     if isinstance(url, list):
         global _load_balancer_
         _load_balancer_ = (_load_balancer_ + 1) % len(url)
         return url[_load_balancer_]
@@ -21,15 +22,24 @@
     _url = get_url()
     res = requests.post(f"{_url}/translate", json={
         'text': text,
         'source_lang': 'auto',
         'target_lang': target_lang,
     })
     if res.text.strip():
-        return res.json().get('data')
+        # return res.json().get('data')
+        # get json data
+        try:
+            return res.json().get('data')
+        except Exception as e:
+            from .. import qs_default_console, qs_error_string
+            qs_default_console.print(qs_error_string, f"DeepLX: {_url}")
+            return None
     else:
+        from .. import qs_default_console, qs_error_string
+        qs_default_console.print(qs_error_string, f"DeepLX: {_url}")
         return None
 
 
 if __name__ == "__main__":
     print(translate("Hello world!"))
```

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/API/Lolicon.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/API/Lolicon.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/API/QiniuOSS.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/API/QiniuOSS.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/API/SimpleAPI.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/API/SimpleAPI.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/API/TencentCloud.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/API/TencentCloud.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/API/__init__.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/API/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/API/alapi.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/API/alapi.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/ImageTools/ColorTools.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/ImageTools/ColorTools.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/ImageTools/ImagePreview.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/ImageTools/ImagePreview.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/ImageTools/ImageTools.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/ImageTools/ImageTools.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/ImageTools/VideoTools.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/ImageTools/VideoTools.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/NetTools/HttpServer.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/NetTools/HttpServer.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/NetTools/M3u8DL.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/NetTools/M3u8DL.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/NetTools/MultiSingleDL.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/NetTools/MultiSingleDL.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/NetTools/NormalDL.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/NetTools/NormalDL.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/NetTools/WiFi.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/NetTools/WiFi.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/NetTools/WiFiDarwin.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/NetTools/WiFiDarwin.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/NetTools/__init__.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/NetTools/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/NumbaTools/__init__.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/NumbaTools/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/SystemTools/Compress.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/SystemTools/Compress.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/SystemTools/Diff.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/SystemTools/Diff.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/SystemTools/DiskMac.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/SystemTools/DiskMac.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/SystemTools/FileHash.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/SystemTools/FileHash.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/SystemTools/__init__.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/SystemTools/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/ThreadTools/__init__.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/ThreadTools/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/TuiTools/Bar.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/TuiTools/Bar.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/TuiTools/Line.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/TuiTools/Line.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/TuiTools/Table.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/TuiTools/Table.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/Wrapper/__init__.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/Wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/__cache__.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/__cache__.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/__config__.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/__config__.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/__init__.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/apiTools.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/apiTools.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,20 +155,23 @@
                 else "抱歉，但是“pyperclip”不支持你的系统\n，所以你需要手动输入内容:"
             )
     if content:
         retry = 3
         lang = requirePackage("langid", "classify")(content)[0]
         while retry:
             try:
-                ret = _translate(
+                if not (ret := _translate(
                     content,
                     target_lang="en"
                     if target_lang == user_lang == lang
                     else target_lang,
-                )
+                )):
+                    retry -= 1
+                    qs_default_console.print(qs_warning_string, "结果为空" if user_lang != "zh" else "Result is empty")
+                    continue
                 break
             except SSLError:
                 retry -= 1
                 qs_default_console.log(
                     qs_warning_string,
                     f"SSL Error, Retrying... \[{3 - retry} / 3]"
                     if user_lang != "zh"
```

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/funcList.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/funcList.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/imageDeal.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/imageDeal.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/lang.json` & `quickstart_rhy-0.7.2/QuickStart_Rhy/lang.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9803921568627451%*

 * *Differences: {"'decompress'": "OrderedDict([('zh', '解压缩{}文件'), ('en', 'unzip {} file'), ('fra', 'décompresser "*

 * *                 "le fichier {}'), ('spa', 'descomprimir archivo {}'), ('ara', 'فك ضغط ملف {}'), "*

 * *                 "('ru', 'распаковать {} файл')])",*

 * * 'delete': "['uncompress']"}*

```diff
@@ -91,14 +91,22 @@
         "ara": "\u062a\u0623\u0643\u064a\u062f \u0627\u0644\u062a\u062b\u0628\u064a\u062a",
         "en": "confirm installation",
         "fra": "confirmer l'installation",
         "ru": "\u043f\u043e\u0434\u0442\u0432\u0435\u0440\u0434\u0438\u0442\u044c \u0443\u0441\u0442\u0430\u043d\u043e\u0432\u043a\u0443",
         "spa": "confirmar instalaci\u00f3n",
         "zh": "\u786e\u8ba4\u5b89\u88c5"
     },
+    "decompress": {
+        "ara": "\u0641\u0643 \u0636\u063a\u0637 \u0645\u0644\u0641 {}",
+        "en": "unzip {} file",
+        "fra": "d\u00e9compresser le fichier {}",
+        "ru": "\u0440\u0430\u0441\u043f\u0430\u043a\u043e\u0432\u0430\u0442\u044c {} \u0444\u0430\u0439\u043b",
+        "spa": "descomprimir archivo {}",
+        "zh": "\u89e3\u538b\u7f29{}\u6587\u4ef6"
+    },
     "download_from_bucket": {
         "ara": "\u062a\u062d\u0645\u064a\u0644 \u0627\u0644\u0645\u0644\u0641 \u0645\u0646 \u062f\u0644\u0648",
         "en": "Download File from Bucket",
         "fra": "T\u00e9l\u00e9charger le fichier du seau",
         "ru": "\u0417\u0430\u0433\u0440\u0443\u0437\u0438\u0442\u044c \u0444\u0430\u0439\u043b \u0438\u0437 \u0432\u0435\u0434\u0440\u0430",
         "spa": "Descargar archivo del cubo",
         "zh": "\u4ece\u6876\u4e0b\u8f7d\u6587\u4ef6"
@@ -747,22 +755,14 @@
         "ara": "\u062f\u0631\u0633 \u062a\u0639\u0644\u064a\u0645\u064a",
         "en": "Tutorial",
         "fra": "Tutoriel",
         "ru": "\u041e\u0431\u0443\u0447\u0435\u043d\u0438\u0435",
         "spa": "Tutorial",
         "zh": "\u5f15\u5bfc"
     },
-    "uncompress": {
-        "ara": "\u0641\u0643 \u0636\u063a\u0637 \u0645\u0644\u0641 {}",
-        "en": "unzip {} file",
-        "fra": "d\u00e9compresser le fichier {}",
-        "ru": "\u0440\u0430\u0441\u043f\u0430\u043a\u043e\u0432\u0430\u0442\u044c {} \u0444\u0430\u0439\u043b",
-        "spa": "descomprimir archivo {}",
-        "zh": "\u89e3\u538b\u7f29{}\u6587\u4ef6"
-    },
     "updated": {
         "ara": "\u062a\u0645 \u0627\u0644\u062a\u062d\u062f\u064a\u062b",
         "en": "Updated",
         "fra": "Mis \u00e0 jour",
         "ru": "\u041e\u0431\u043d\u043e\u0432\u043b\u0435\u043d\u043e",
         "spa": "Actualizado",
         "zh": "\u66f4\u65b0\u5b8c\u6210"
```

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/main.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 def qs_help(rep:str=""):
     """输出菜单 | Output menu"""
     if not rep or rep not in ['basic', 'system', 'net', 'api', 'image']:
         menu_show([
             ['basic', 'u, a, f, cal, time, pcat..'],
-            ['system', 'top, \[mk/un][zip/tar/7z]..'],
+            ['system', 'top, \[mk/un]\[zip/tar/7z]..'],
             ['net', 'http, dl, netinfo, wifi...'],
             ['api', 'trans, smms, rmbg, loli...'],
             ['image', 'stbg, v2gif, v2mp3, v2mp4.']
         ])
         qs_default_console.print(f"\n[bold]{lang_detector['tutorial']}[/]\n", justify="center")
         qs_default_console.print("[bold magenta]qs lesson[/]", justify="center")
     else:
```

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/netTools.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/netTools.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/qsLesson.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/qsLesson.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.1/QuickStart_Rhy/system.py` & `quickstart_rhy-0.7.2/QuickStart_Rhy/system.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.1/README.md` & `quickstart_rhy-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.1/pyproject.toml` & `quickstart_rhy-0.7.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "QuickStart-Rhy"
-version = "0.7.1"
+version = "0.7.2"
 description = "A Command Line Toolbox"
 authors = ["Rhythmicc <rhythmlian.cn@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "QuickStart_Rhy"}, {include = "QuickStart_Rhy/lang.json"}]
 
 [tool.poetry.dependencies]
```

### Comparing `quickstart_rhy-0.7.1/setup.py` & `quickstart_rhy-0.7.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
  'urllib3>=1.26.15,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['qs = QuickStart_Rhy.main:main']}
 
 setup_kwargs = {
     'name': 'quickstart-rhy',
-    'version': '0.7.1',
+    'version': '0.7.2',
     'description': 'A Command Line Toolbox',
     'long_description': '# QuickStart_Rhy\n\n```shell\npip3 install quickstart-rhy                                         # stable version\npip3 install git+https://github.com/Rhythmicc/quickstart-rhy.git -U # beta version but more features\n```\n\n| Key  | Value                                              |\n| :--: | -------------------------------------------------- |\n| ENV  | **^Python 3.7**                                    |\n| FONT | **Cascadia Code / Meslo**                          |\n| DOCS | <https://rhythmlian.cn/2020/02/14/QuickStart-Rhy/> |\n\n## Tab Complete\n\n1. fig\n\n   ```shell\n   npx @fig/publish-spec -p complete/fig/qs-<your language>.ts --name qs\n   ```\n\n2. zsh\n\n   ```shell\n   mv _qs /path/in/$FPATH/\n   ```\n',
     'author': 'Rhythmicc',
     'author_email': 'rhythmlian.cn@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `quickstart_rhy-0.7.1/PKG-INFO` & `quickstart_rhy-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-rhy
-Version: 0.7.1
+Version: 0.7.2
 Summary: A Command Line Toolbox
 License: MIT
 Author: Rhythmicc
 Author-email: rhythmlian.cn@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

