# Comparing `tmp/gpt-term-1.0.5.tar.gz` & `tmp/gpt-term-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-term-1.0.5.tar", last modified: Wed May 17 07:48:41 2023, max compression
+gzip compressed data, was "gpt-term-1.1.0.tar", last modified: Thu May 18 13:34:43 2023, max compression
```

## Comparing `gpt-term-1.0.5.tar` & `gpt-term-1.1.0.tar`

### file list

```diff
@@ -1,29 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:48:41.572279 gpt-term-1.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:48:41.560279 gpt-term-1.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:48:41.564279 gpt-term-1.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-17 07:48:26.000000 gpt-term-1.0.5/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-17 07:48:26.000000 gpt-term-1.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-17 07:48:26.000000 gpt-term-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15226 2023-05-17 07:48:41.572279 gpt-term-1.0.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:48:41.564279 gpt-term-1.0.5/README.assets/
--rw-r--r--   0 runner    (1001) docker     (123)   297411 2023-05-17 07:48:26.000000 gpt-term-1.0.5/README.assets/image-20230303233352970.png
--rw-r--r--   0 runner    (1001) docker     (123)  3707698 2023-05-17 07:48:26.000000 gpt-term-1.0.5/README.assets/small.gif
--rw-r--r--   0 runner    (1001) docker     (123)    13525 2023-05-17 07:48:26.000000 gpt-term-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-05-17 07:48:26.000000 gpt-term-1.0.5/README.zh-CN.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      117 2023-05-17 07:48:26.000000 gpt-term-1.0.5/chat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:48:41.572279 gpt-term-1.0.5/gpt_term/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-17 07:48:26.000000 gpt-term-1.0.5/gpt_term/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-17 07:48:26.000000 gpt-term-1.0.5/gpt_term/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-17 07:48:41.000000 gpt-term-1.0.5/gpt_term/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-17 07:48:26.000000 gpt-term-1.0.5/gpt_term/config.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)    48444 2023-05-17 07:48:26.000000 gpt-term-1.0.5/gpt_term/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:48:41.572279 gpt-term-1.0.5/gpt_term.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15226 2023-05-17 07:48:41.000000 gpt-term-1.0.5/gpt_term.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-17 07:48:41.000000 gpt-term-1.0.5/gpt_term.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 07:48:41.000000 gpt-term-1.0.5/gpt_term.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-17 07:48:41.000000 gpt-term-1.0.5/gpt_term.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-17 07:48:41.000000 gpt-term-1.0.5/gpt_term.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 07:48:41.000000 gpt-term-1.0.5/gpt_term.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-17 07:48:26.000000 gpt-term-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-17 07:48:26.000000 gpt-term-1.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 07:48:41.572279 gpt-term-1.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:34:43.660858 gpt-term-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:34:43.652858 gpt-term-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:34:43.652858 gpt-term-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-18 13:34:31.000000 gpt-term-1.1.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-18 13:34:31.000000 gpt-term-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-18 13:34:31.000000 gpt-term-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15585 2023-05-18 13:34:43.656858 gpt-term-1.1.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:34:43.652858 gpt-term-1.1.0/README.assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   297411 2023-05-18 13:34:31.000000 gpt-term-1.1.0/README.assets/image-20230303233352970.png
+-rw-r--r--   0 runner    (1001) docker     (123)  3707698 2023-05-18 13:34:31.000000 gpt-term-1.1.0/README.assets/small.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    13884 2023-05-18 13:34:31.000000 gpt-term-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12877 2023-05-18 13:34:31.000000 gpt-term-1.1.0/README.zh-CN.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      117 2023-05-18 13:34:31.000000 gpt-term-1.1.0/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:34:43.656858 gpt-term-1.1.0/gpt_term/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 13:34:31.000000 gpt-term-1.1.0/gpt_term/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-18 13:34:31.000000 gpt-term-1.1.0/gpt_term/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-18 13:34:43.000000 gpt-term-1.1.0/gpt_term/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-18 13:34:31.000000 gpt-term-1.1.0/gpt_term/config.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:34:43.656858 gpt-term-1.1.0/gpt_term/locale/
+-rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-05-18 13:34:31.000000 gpt-term-1.1.0/gpt_term/locale/gpt_term.de.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-05-18 13:34:31.000000 gpt-term-1.1.0/gpt_term/locale/gpt_term.en.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    12194 2023-05-18 13:34:31.000000 gpt-term-1.1.0/gpt_term/locale/gpt_term.jp.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-05-18 13:34:31.000000 gpt-term-1.1.0/gpt_term/locale/gpt_term.zh_CN.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-18 13:34:31.000000 gpt-term-1.1.0/gpt_term/locale.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47638 2023-05-18 13:34:31.000000 gpt-term-1.1.0/gpt_term/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:34:43.656858 gpt-term-1.1.0/gpt_term.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15585 2023-05-18 13:34:43.000000 gpt-term-1.1.0/gpt_term.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-18 13:34:43.000000 gpt-term-1.1.0/gpt_term.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 13:34:43.000000 gpt-term-1.1.0/gpt_term.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-18 13:34:43.000000 gpt-term-1.1.0/gpt_term.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-18 13:34:43.000000 gpt-term-1.1.0/gpt_term.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-18 13:34:43.000000 gpt-term-1.1.0/gpt_term.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-18 13:34:31.000000 gpt-term-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-18 13:34:31.000000 gpt-term-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 13:34:43.660858 gpt-term-1.1.0/setup.cfg
```

### Comparing `gpt-term-1.0.5/.github/workflows/pypi-publish.yml` & `gpt-term-1.1.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `gpt-term-1.0.5/LICENSE` & `gpt-term-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-term-1.0.5/PKG-INFO` & `gpt-term-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-term
-Version: 1.0.5
+Version: 1.1.0
 Summary: Chat with GPT in Terminal
 Author: xiaoxx970, Ace-Radom
 License: MIT License
         
         Copyright (c) 2023 xiaoxx970
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -53,27 +53,31 @@
 
 ![example](https://github.com/xiaoxx970/chatgpt-in-terminal/raw/main/README.assets/small.gif)
 
 Uses the [gpt-3.5-turbo](https://platform.openai.com/docs/guides/chat/chat-completions-beta) model, which is the same model used by ChatGPT (Free Edition), as default.
 
 ## Changelog
 
+### 2023-05-18
+
+- Added multi-language support: English, Chinese, Japanese, German, follow the system language by default, now you can use `/lang` to switch languages
+
+<details>
+  <summary>More Change log</summary>
+
 ### 2023-05-11
 
 - Find the command the user most likely intended to enter when typing an unrecognized command
 
 ### 2023-05-05
 
 - Add `/rand` command to set temperature parameter
 
 - Add overflow mode switch for `/stream` command, now you can run command `/stream visible` to switch to always visible mode. In this mode, the content that exceeds the screen will be scrolled up, and the new content will be output until it is completed
 
-<details>
-  <summary>More Change log</summary>
-
 ### 2023-04-23
 Released `gpt-term` on [Pypi](https://pypi.org/project/gpt-term/), started version control. No need to clone the project locally anymore, simply use the `pip` command to install gpt-term.
 
 ### 2023-04-15
 
 - Added the ability to create a line break in single-line mode using `Esc` + `Enter`
 
@@ -182,14 +186,15 @@
 | -m, --multi   | Enable multi-line mode          | `gpt-term --multi`                            |
 | -r, --raw     | Enable raw mode                 | `gpt-term --raw`                              |
 | --set-apikey KEY        | Set the OpenAI API key                                   | `gpt-term --set-apikey sk-xxx`   |
 | --set-timeout SEC       | Set the maximum wait time for API requests               | `gpt-term --set-timeout 10`      |
 | --set-gentitle BOOL     | Set whether to auto-generate a title for the chat        | `gpt-term --set-gentitle True`   |
 | --set-saveperfix PERFIX | Set the save prefix for chat history files               | `gpt-term --set-saveperfix chat_history_` |
 | --set-loglevel LEVEL    | Set the log level: DEBUG, INFO, WARNING, ERROR, CRITICAL | `gpt-term --set-loglevel DEBUG`  |
+| --set-lang LANG    | Set the language: en, zh_CN, jp, de | `gpt-term --set-lang en` |
 
 > Multi-line mode and raw mode can be used simultaneously
 
 ### Configuration File
 
 The configuration file is located at `~/.gpt-term/config.ini` and is autogenerated. It can be modified using the program's `--set` option or edited manually.
 
@@ -208,14 +213,17 @@
 
 # Define the default file prefix when the /save command saves the chat history. The default value is "./chat_history_", which means that the chat history will be saved in the file starting with "chat_history_" in the current directory
 # At the same time, the prefix can also be specified as a directory + / to allow the program to save the chat history in a folder (note that the corresponding folder needs to be created in advance), for example: CHAT_SAVE_PERFIX=chat_history/
 CHAT_SAVE_PERFIX=./chat_history_
 
 # Log level, default is INFO, available value: DEBUG, INFO, WARNING, ERROR, CRITICAL
 LOG_LEVEL=INFO
+
+# Set the language of the program, the default is empty, it will follow the system language
+LANGUAGE=
 ```
 
 ### Available Commands
 
 - `/raw`: Display raw text in replies instead of rendered Markdown format
 
   > After switching, use the `/last` command to reprint the last reply
```

### Comparing `gpt-term-1.0.5/README.assets/image-20230303233352970.png` & `gpt-term-1.1.0/README.assets/image-20230303233352970.png`

 * *Files identical despite different names*

### Comparing `gpt-term-1.0.5/README.assets/small.gif` & `gpt-term-1.1.0/README.assets/small.gif`

 * *Files identical despite different names*

### Comparing `gpt-term-1.0.5/README.md` & `gpt-term-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -17,27 +17,31 @@
 
 ![example](https://github.com/xiaoxx970/chatgpt-in-terminal/raw/main/README.assets/small.gif)
 
 Uses the [gpt-3.5-turbo](https://platform.openai.com/docs/guides/chat/chat-completions-beta) model, which is the same model used by ChatGPT (Free Edition), as default.
 
 ## Changelog
 
+### 2023-05-18
+
+- Added multi-language support: English, Chinese, Japanese, German, follow the system language by default, now you can use `/lang` to switch languages
+
+<details>
+  <summary>More Change log</summary>
+
 ### 2023-05-11
 
 - Find the command the user most likely intended to enter when typing an unrecognized command
 
 ### 2023-05-05
 
 - Add `/rand` command to set temperature parameter
 
 - Add overflow mode switch for `/stream` command, now you can run command `/stream visible` to switch to always visible mode. In this mode, the content that exceeds the screen will be scrolled up, and the new content will be output until it is completed
 
-<details>
-  <summary>More Change log</summary>
-
 ### 2023-04-23
 Released `gpt-term` on [Pypi](https://pypi.org/project/gpt-term/), started version control. No need to clone the project locally anymore, simply use the `pip` command to install gpt-term.
 
 ### 2023-04-15
 
 - Added the ability to create a line break in single-line mode using `Esc` + `Enter`
 
@@ -146,14 +150,15 @@
 | -m, --multi   | Enable multi-line mode          | `gpt-term --multi`                            |
 | -r, --raw     | Enable raw mode                 | `gpt-term --raw`                              |
 | --set-apikey KEY        | Set the OpenAI API key                                   | `gpt-term --set-apikey sk-xxx`   |
 | --set-timeout SEC       | Set the maximum wait time for API requests               | `gpt-term --set-timeout 10`      |
 | --set-gentitle BOOL     | Set whether to auto-generate a title for the chat        | `gpt-term --set-gentitle True`   |
 | --set-saveperfix PERFIX | Set the save prefix for chat history files               | `gpt-term --set-saveperfix chat_history_` |
 | --set-loglevel LEVEL    | Set the log level: DEBUG, INFO, WARNING, ERROR, CRITICAL | `gpt-term --set-loglevel DEBUG`  |
+| --set-lang LANG    | Set the language: en, zh_CN, jp, de | `gpt-term --set-lang en` |
 
 > Multi-line mode and raw mode can be used simultaneously
 
 ### Configuration File
 
 The configuration file is located at `~/.gpt-term/config.ini` and is autogenerated. It can be modified using the program's `--set` option or edited manually.
 
@@ -172,14 +177,17 @@
 
 # Define the default file prefix when the /save command saves the chat history. The default value is "./chat_history_", which means that the chat history will be saved in the file starting with "chat_history_" in the current directory
 # At the same time, the prefix can also be specified as a directory + / to allow the program to save the chat history in a folder (note that the corresponding folder needs to be created in advance), for example: CHAT_SAVE_PERFIX=chat_history/
 CHAT_SAVE_PERFIX=./chat_history_
 
 # Log level, default is INFO, available value: DEBUG, INFO, WARNING, ERROR, CRITICAL
 LOG_LEVEL=INFO
+
+# Set the language of the program, the default is empty, it will follow the system language
+LANGUAGE=
 ```
 
 ### Available Commands
 
 - `/raw`: Display raw text in replies instead of rendered Markdown format
 
   > After switching, use the `/last` command to reprint the last reply
```

### Comparing `gpt-term-1.0.5/README.zh-CN.md` & `gpt-term-1.1.0/README.zh-CN.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,27 +19,31 @@
 
 ![example](https://github.com/xiaoxx970/chatgpt-in-terminal/raw/main/README.assets/small.gif)
 
 默认使用 [gpt-3.5-turbo](https://platform.openai.com/docs/guides/chat/chat-completions-beta) 模型，也就是 ChatGPT(免费版) 所使用的模型。
 
 ## 更新记录
 
+### 2023-05-18
+
+- 新增多语言支持：英语、中文、日语、德语，默认跟随系统语言，现在可以使用 `/lang` 来切换语言
+
+<details>
+  <summary>更多 Change log</summary>
+
 ### 2023-05-11
 
 - 在输入未被识别的命令时查找用户最可能想输入的命令
 
 ### 2023-05-05
 
 - 添加`/rand`命令设置temperature参数
 
 - 为 `/stream` 命令添加 overflow 模式切换，现在可以运行命令 `/stream visible` 切换到始终可见模式。在这个模式下，超出屏幕的内容将被向上滚动，新内容会一直输出直到完成
 
-<details>
-  <summary>更多 Change log</summary>
-
 ### 2023-04-23
 
 - 发布 `gpt-term` 到 [Pypi](https://pypi.org/project/gpt-term/)，开始版本管理，现在不需要克隆项目到本地，直接使用 `pip` 命令就可以安装 `gpt-term`
 
 ### 2023-04-15
 
 - 新增在单行模式下换行功能，现在可以使用 `Esc` + `Enter` 在单行模式下换行
@@ -149,14 +153,15 @@
 | -m, --multi   | 启用多行模式                      | `gpt-term --multi`                            |
 | -r, --raw     | 启用原始模式                      | `gpt-term --raw`                              |
 | --set-apikey KEY        | 设置 OpenAI 的 API 密钥                          | `gpt-term --set-apikey sk-xxx` |
 | --set-timeout SEC       | 设置 API 请求的最大等待时间                         | `gpt-term --set-timeout 10` |
 | --set-gentitle BOOL     | 设置是否为聊天自动生成标题                          | `gpt-term --set-gentitle True` |
 | --set-saveperfix PERFIX | 设置聊天历史文件的保存前缀                          | `gpt-term --set-saveperfix chat_history_` |
 | --set-loglevel LEVEL    | 设置日志级别：DEBUG, INFO, WARNING, ERROR, CRITICAL | `gpt-term --set-loglevel DEBUG` |
+| --set-lang LANG    | 设置语言：en, zh_CN, jp, de | `gpt-term --set-lang en` |
 
 > 多行模式与 raw 模式可以同时使用
 
 ### 配置文件
 
 配置文件位于 `~/.gpt-term/config.ini`，由程序自动生成，可以通过程序 `--set` 参数修改，也可手动修改
 
@@ -175,14 +180,17 @@
 
 # 定义 /save 命令保存聊天历史时的默认文件前缀，默认值为"./chat_history_"，表示将聊天历史存到当前目录的以"chat_history_"开头的文件中
 # 同时该前缀还可以指定为目录+/的形式来让程序保存聊天历史到一个文件夹中(注意需要提前创建好对应文件夹)，比如：CHAT_SAVE_PERFIX=chat_history/
 CHAT_SAVE_PERFIX=./chat_history_
 
 # 日志级别，默认为INFO，可选值：DEBUG、INFO、WARNING、ERROR、CRITICAL
 LOG_LEVEL=INFO
+
+# 设置程序的语言，默认为空，将跟随系统语言
+LANGUAGE=
 ```
 
 ### 可用命令
 
 - `/raw`：在回复中显示原始文本，而不是渲染后的 Markdown 格式
 
   > 切换后可使用 `/last` 命令重新打印当前回复
```

### Comparing `gpt-term-1.0.5/gpt_term/config.ini` & `gpt-term-1.1.0/gpt_term/config.ini`

 * *Files 21% similar despite different names*

```diff
@@ -7,8 +7,11 @@
 # Whether to automatically generate titles for conversations, enabled by default (generating titles will consume a small amount of tokens)
 AUTO_GENERATE_TITLE=True
 # Define the default file prefix when the /save command saves the chat history. The default value is "./chat_history_", which means that the chat history will be saved in the file starting with "chat_history_" in the current directory
 # At the same time, the prefix can also be specified as a directory + / to allow the program to save the chat history in a folder (note that the corresponding folder needs to be created in advance), for example: CHAT_SAVE_PERFIX=chat_history/
 CHAT_SAVE_PERFIX=./chat_history_
 
 # Log level, default is INFO, available value: DEBUG, INFO, WARNING, ERROR, CRITICAL
-LOG_LEVEL=INFO
+LOG_LEVEL=INFO
+
+# Set the language of the program, the default is empty, it will follow the system language
+LANGUAGE=
```

### Comparing `gpt-term-1.0.5/gpt_term/main.py` & `gpt-term-1.1.0/gpt_term/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 from rich import print as rprint
 from rich.console import Console, Group
 from rich.live import Live
 from rich.markdown import Markdown
 from rich.panel import Panel
 
 from . import __version__
+from .locale import set_lang, get_lang
+import locale
 
 data_dir = Path.home() / '.gpt-term'
 data_dir.mkdir(parents=True, exist_ok=True)
 config_path = data_dir / 'config.ini'
 if not config_path.exists():
     with config_path.open('w') as f:
         f.write(read_text('gpt_term', 'config.ini'))
@@ -66,35 +68,37 @@
     raw_mode = False
     multi_line_mode = False
     stream_mode = True
 
     @classmethod
     def toggle_raw_mode(cls):
         cls.raw_mode = not cls.raw_mode
-        console.print(
-            f"[dim]Raw mode {'[green]enabled[/]' if cls.raw_mode else '[bright_red]disabled[/]'}, use `[bright_magenta]/last[/]` to display the last answer.")
+        if cls.raw_mode:
+            console.print(_("gpt_term.raw_mode_enabled"))
+        else:
+            console.print(_("gpt_term.raw_mode_disabled"))
 
     @classmethod
     def toggle_stream_mode(cls):
         cls.stream_mode = not cls.stream_mode
         if cls.stream_mode:
             console.print(
-                f"[dim]Stream mode [green]enabled[/], the answer will start outputting as soon as the first response arrives.")
+                _("gpt_term.stream_mode_enabled"))
         else:
             console.print(
-                f"[dim]Stream mode [bright_red]disabled[/], the answer is being displayed after the server finishes responding.")
+                _("gpt_term.stream_mode_disabled"))
 
     @classmethod
     def toggle_multi_line_mode(cls):
         cls.multi_line_mode = not cls.multi_line_mode
         if cls.multi_line_mode:
             console.print(
-                f"[dim]Multi-line mode [green]enabled[/], press [[bright_magenta]Esc[/]] + [[bright_magenta]ENTER[/]] to submit.")
+                _("gpt_term.multi_line_enabled"))
         else:
-            console.print(f"[dim]Multi-line mode [bright_red]disabled[/].")
+            console.print(_("gpt_term.multi_line_disabled"))
 
 
 class ChatGPT:
     def __init__(self, api_key: str, timeout: float):
         self.api_key = api_key
         self.endpoint = "https://api.openai.com/v1/chat/completions"
         self.headers = {
@@ -125,35 +129,35 @@
     def add_total_tokens(self, tokens: int):
         self.threadlock_total_tokens_spent.acquire()
         self.total_tokens_spent += tokens
         self.threadlock_total_tokens_spent.release()
 
     def send_request(self, data):
         try:
-            with console.status(f"[bold cyan]ChatGPT is thinking..."):
+            with console.status(_("gpt_term.ChatGPT_thinking")):
                 response = requests.post(
                     self.endpoint, headers=self.headers, data=json.dumps(data), timeout=self.timeout, stream=ChatMode.stream_mode)
             # 匹配4xx错误，显示服务器返回的具体原因
             if response.status_code // 100 == 4:
                 error_msg = response.json()['error']['message']
-                console.print(f"[red]Error: {error_msg}")
+                console.print(_("gpt_term.Error_message",error_msg=error_msg))
                 log.error(error_msg)
                 return None
 
             response.raise_for_status()
             return response
         except KeyboardInterrupt:
-            console.print("[bold cyan]Aborted.")
+            console.print(_("gpt_term.Aborted"))
             raise
         except requests.exceptions.ReadTimeout as e:
             console.print(
-                f"[red]Error: API read timed out ({self.timeout}s). You can retry or increase the timeout.", highlight=False)
+                _("gpt_term.Error_timeout",timeout=self.timeout), highlight=False)
             return None
         except requests.exceptions.RequestException as e:
-            console.print(f"[red]Error: {str(e)}")
+            console.print(_("gpt_term.Error_message",error_msg=str(e)))
             log.exception(e)
             return None
 
     def send_request_silent(self, data):
         # this is a silent sub function, for sending request without outputs (silently)
         # it SHOULD NOT be triggered or used by not-silent functions
         # it is only used by gen_title_silent now
@@ -191,15 +195,15 @@
                         reply += content
                         if ChatMode.raw_mode:
                             rprint(content, end="", flush=True),
                         else:
                             live.update(Markdown(reply), refresh=True)
             except KeyboardInterrupt:
                 live.stop()
-                console.print("Aborted.", style="bold cyan")
+                console.print(_('gpt_term.Aborted'))
             finally:
                 return {'role': 'assistant', 'content': reply}
 
     def process_response(self, response: requests.Response):
         if ChatMode.stream_mode:
             return self.process_stream_response(response)
         else:
@@ -222,40 +226,40 @@
 
             # recount current tokens
             new_tokens = count_token(self.messages)
             tokens_saved = self.current_tokens - new_tokens
             self.current_tokens = new_tokens
 
             console.print(
-                f"[dim]First question: '{truncated_question}' and it's answer has been deleted, saved tokens: {tokens_saved}")
+                _('gpt_term.delete_first_conversation_yes',truncated_question=truncated_question,tokens_saved=tokens_saved))
         else:
-            console.print("[red]No conversations yet.")
+            console.print(_('gpt_term.delete_first_conversation_no'))
     
     def delete_all_conversation(self):
         del self.messages[1:]
         self.title = None
         # recount current tokens
         self.current_tokens = count_token(self.messages)
         os.system('cls' if os.name == 'nt' else 'clear')
-        console.print("[dim]Current chat cleared.")
+        console.print(_('gpt_term.delete_all'))
 
     def handle(self, message: str):
         try:
             self.messages.append({"role": "user", "content": message})
             data = {
                 "model": self.model,
                 "messages": self.messages,
                 "stream": ChatMode.stream_mode,
                 "temperature": self.temperature
             }
             response = self.send_request(data)
             if response is None:
                 self.messages.pop()
                 if self.current_tokens >= self.tokens_limit:
-                    if confirm("Reached tokens limit, do you want me to forget the earliest message of current chat?"):
+                    if confirm(_('gpt_term.tokens_reached')):
                         self.delete_first_conversation()
                 return
 
             reply_message = self.process_response(response)
             if reply_message is not None:
                 log.info(f"ChatGPT: {reply_message['content']}")
                 self.messages.append(reply_message)
@@ -263,46 +267,46 @@
                 self.add_total_tokens(self.current_tokens)
 
                 if len(self.messages) == 3 and self.auto_gen_title_background_enable:
                     self.gen_title_messages.put(self.messages[1]['content'])
 
                 if self.tokens_limit - self.current_tokens in range(1, 500):
                     console.print(
-                        f"[dim]Approaching the tokens limit: {self.tokens_limit - self.current_tokens} tokens left")
+                        _("gpt_term.tokens_approaching",token_left=self.tokens_limit - self.current_tokens))
                 # approaching tokens limit (less than 500 left), show info
 
         except Exception as e:
             console.print(
-                f"[red]Error: {str(e)}. Check log for more information")
+                _("chat_term.Error_look_log",error_msg=str(e)))
             log.exception(e)
             self.save_chat_history_urgent()
             raise EOFError
 
         return reply_message
 
     def gen_title(self, force: bool = False):
         # Empty the title if there is only system message left
         if len(self.messages) < 2:
             self.title = None
             return
 
         try:
-            with console.status("[bold cyan]Waiting last generationg to finish..."):
+            with console.status(_("gpt_term.title_waiting_gen")):
                 self.gen_title_messages.join()
             if self.title and not force:
                 return self.title
 
             # title not generated, do
 
             content_this_time = self.messages[1]['content']
             self.gen_title_messages.put(content_this_time)
-            with console.status("[bold cyan]Generating title... [/](Ctrl-C to skip)"):
+            with console.status(_("gpt_term.title_gening")):
                 self.gen_title_messages.join()
         except KeyboardInterrupt:
-            console.print("Skip wait.", style="bold cyan")
+            console.print(_("gpt_term.title_skip_gen"))
             raise
 
         return self.title
 
     def gen_title_silent(self, content: str):
         # this is a silent sub function, only for sub thread which auto-generates title when first conversation is made and debug functions
         # it SHOULD NOT be triggered or used by any other functions or commands
@@ -343,64 +347,64 @@
                 if not new_title:
                     log.error("Background Title auto-generation Failed")
                 else:
                     change_CLI_title(self.title)
                 log.debug("Title Generation Daemon Thread: Pause")
 
             except Exception as e:
-                console.print(
-                    f"[red]Background Title auto-generation Error: {str(e)}. Check log for more information")
+                console.print(_("gpt_term.title_auto_gen_fail",error_msg=str(e))
+                    )
                 log.exception(e)
                 self.save_chat_history_urgent()
                 while self.gen_title_messages.unfinished_tasks:
                     self.gen_title_messages.task_done()
                 continue
                 # something went wrong, continue the loop
 
     def save_chat_history(self, filename):
         try:
             with open(f"{filename}", 'w', encoding='utf-8') as f:
                 json.dump(self.messages, f, ensure_ascii=False, indent=4)
             console.print(
-                f"[dim]Chat history saved to: [bright_magenta]{filename}", highlight=False)
+                _("gpt_term.save_history_success",filename=filename), highlight=False)
         except Exception as e:
             console.print(
-                f"[red]Error: {str(e)}. Check log for more information")
+                _("gpt_term.Error_look_log"))
             log.exception(e)
             self.save_chat_history_urgent()
             return
 
     def save_chat_history_urgent(self):
         filename = f'{data_dir}/chat_history_backup_{datetime.now().strftime("%Y-%m-%d_%H,%M,%S")}.json'
         with open(f"{filename}", 'w', encoding='utf-8') as f:
             json.dump(self.messages, f, ensure_ascii=False, indent=4)
         console.print(
-            f"[dim]Chat history urgently saved to: [bright_magenta]{filename}", highlight=False)
+            _("gpt_term.save_history_urgent_success",filename=filename), highlight=False)
 
     def send_get(self, url, params=None):
         try:
             response = requests.get(
                 url, headers=self.headers, timeout=self.timeout, params=params)
         # 匹配4xx错误，显示服务器返回的具体原因
             if response.status_code // 100 == 4:
                 error_msg = response.json()['error']['message']
-                console.print(f"[red]Get {url} Error: {error_msg}")
+                console.print(_("gpt_term.Error_get_url",url=url,error_msg=error_msg))
                 log.error(error_msg)
                 return None
             response.raise_for_status()
             return response
         except KeyboardInterrupt:
-            console.print("[bold cyan]Aborted.")
+            console.print(_("gpt_term.Aborted"))
             raise
         except requests.exceptions.ReadTimeout as e:
             console.print(
-                f"[red]Error: API read timed out ({self.timeout}s). You can retry or increase the timeout.", highlight=False)
+                _("gpt_term.Error_timeot",timeout=self.timeout), highlight=False)
             return None
         except requests.exceptions.RequestException as e:
-            console.print(f"[red]Error: {str(e)}")
+            console.print(_("gpt_term.Error_message",error_msg=str(e)))
             log.exception(e)
             return None
 
     def fetch_credit_total_granted(self):
         url_subscription = "https://api.openai.com/dashboard/billing/subscription"
         response_subscription = self.send_get(url_subscription)
         if not response_subscription:
@@ -458,96 +462,96 @@
                 result = future.result()
                 if result:
                     credit_total_used_cent += result.json()["total_usage"]
             # get all usage info from 2023-01-01 to now
             self.credit_total_used = credit_total_used_cent / 100
 
         except KeyboardInterrupt:
-            console.print("[bold cyan]Aborted.")
+            console.print(_("gpt_term.Aborted"))
             raise
         except Exception as e:
             console.print(
-                f"[red]Error: {str(e)}. Check log for more information")
+                _("gpt_term.Error_message",error_msg=str(e)))
             log.exception(e)
             self.save_chat_history_urgent()
             raise EOFError
         return True
 
     def modify_system_prompt(self, new_content: str):
         if self.messages[0]['role'] == 'system':
             old_content = self.messages[0]['content']
             self.messages[0]['content'] = new_content
             console.print(
-                f"[dim]System prompt has been modified from '{old_content}' to '{new_content}'.")
+                _("gpt_term.system_prompt_moodified",old_content=old_content,new_content=new_content))
             self.current_tokens = count_token(self.messages)
             # recount current tokens
             if len(self.messages) > 1:
                 console.print(
-                    "[dim]Note this is not a new chat, modifications to the system prompt have limited impact on answers.")
+                    _("gpt_term.system_prompt_note"))
         else:
             console.print(
-                f"[dim]No system prompt found in messages.")
+                _("gpt_term.system_prompt_found"))
 
     def set_stream_overflow(self, new_overflow: str):
         # turn on stream if not
         if not ChatMode.stream_mode:
             ChatMode.toggle_stream_mode()
 
         if new_overflow == self.stream_overflow:
-            console.print("[dim]No change.")
+            console.print(_("gpt_term.No_change"))
             return
 
         old_overflow = self.stream_overflow
         if new_overflow == 'ellipsis' or new_overflow == 'visible':
             self.stream_overflow = new_overflow
             console.print(
-                f"[dim]Stream overflow option has been modified from '{old_overflow}' to '{new_overflow}'.")
+                _("gpt_term.stream_overflow_modified",old_overflow=old_overflow,new_overflow=new_overflow))
             if new_overflow == 'visible':
-                console.print("[dim]Note that in this mode the terminal will not properly clean up off-screen content.")
+                console.print(_("gpt_term.stream_overflow_visible"))
         else:
-            console.print(f"[dim]No such Stream overflow option, remain '{old_overflow}' unchanged.")
+            console.print(_("gpt_term.stream_overflow_no_changed",old_overflow=old_overflow))
         
 
     def set_model(self, new_model: str):
         old_model = self.model
         if not new_model:
             console.print(
-                f"[dim]Empty input, the model remains '{old_model}'.")
+                _("gpt_term.model_set"),old_model=old_model)
             return
         self.model = str(new_model)
         if "gpt-4-32k" in self.model:
             self.tokens_limit = 32768
         elif "gpt-4" in self.model:
             self.tokens_limit = 8192
         elif "gpt-3.5-turbo" in self.model:
             self.tokens_limit = 4096
         else:
             self.tokens_limit = float('nan')
         console.print(
-            f"[dim]Model has been set from '{old_model}' to '{new_model}'.")
+            _("gpt_term.model_changed",old_model=old_model,new_model=new_model))
 
     def set_timeout(self, timeout):
         try:
             self.timeout = float(timeout)
         except ValueError:
-            console.print("[red]Input must be a number")
+            console.print(_("gpt_term.Error_input_number"))
             return
-        console.print(f"[dim]API timeout set to [green]{timeout}s[/].")
+        console.print(_("gpt_term.timeput_changed",timeout=timeout))
 
     def set_temperature(self, temperature):
         try:
             new_temperature = float(temperature)
         except ValueError:
-            console.print("[red]Input must be a number between 0 and 2")
+            console.print(_("gpt_term.temperature_must_between"))
             return
         if new_temperature > 2 or new_temperature < 0:
-            console.print("[red]Input must be a number between 0 and 2")
+            console.print(_("gpt_term.temperature_must_between"))
             return
         self.temperature = new_temperature
-        console.print(f"[dim]Randomness set to [green]{temperature}[/].")
+        console.print(_("gpt_term.temperature_set",temperature=temperature))
 
 
 class CommandCompleter(Completer):
     def __init__(self):
         self.nested_completer = NestedCompleter.from_nested_dict({
             '/raw': None,
             '/multi': None,
@@ -568,14 +572,15 @@
             '/rand': None,
             '/temperature': None,
             '/title': None,
             '/timeout': None,
             '/undo': None,
             '/delete': {"first", "all"},
             '/reset': None,
+            '/lang' : {"zh_CN","en","jp","de"},
             '/version': None,
             '/help': None,
             '/exit': None,
         })
 
     def path_filter(self, filename):
         # 路径自动补全，只补全json文件和文件夹
@@ -607,32 +612,32 @@
     return length
 
 
 class NumberValidator(Validator):
     def validate(self, document):
         text = document.text
         if not text.isdigit():
-            raise ValidationError(message="Please input an Integer!",
+            raise ValidationError(message=_("gpt_term.Error_input_int"),
                                   cursor_position=len(text))
 
 class FloatRangeValidator(Validator):
     def __init__(self, min_value=None, max_value=None):
         self.min_value = min_value
         self.max_value = max_value
 
     def validate(self, document):
         try:
             value = float(document.text)
         except ValueError:
-            raise ValidationError(message='Input must be a number')
+            raise ValidationError(message=_('gpt_term.Error_input_number'))
 
         if self.min_value is not None and value < self.min_value:
-            raise ValidationError(message=f'Input must be at least {self.min_value}')
+            raise ValidationError(message=_("gpt_term.Error_input_least",min_value=self.min_value))
         if self.max_value is not None and value > self.max_value:
-            raise ValidationError(message=f'Input must be at most {self.max_value}')
+            raise ValidationError(message=_("gpt_term.Error_input_most",max_value=self.max_value))
         
 temperature_validator = FloatRangeValidator(min_value=0.0, max_value=2.0)
 
 def print_message(message: Dict[str, str]):
     '''打印单条来自 ChatGPT 或用户的消息'''
     role = message["role"]
     content = message["content"]
@@ -646,55 +651,55 @@
             console.print(Markdown(content), new_line_start=True)
 
 
 def copy_code(message: Dict[str, str], select_code_idx: int = None):
     '''Copy the code in ChatGPT's last reply to Clipboard'''
     code_list = re.findall(r'```[\s\S]*?```', message["content"])
     if len(code_list) == 0:
-        console.print("[dim]No code found")
+        console.print(_("gpt_term.code_not_found"))
         return
 
     if len(code_list) == 1 and select_code_idx is None:
         selected_code = code_list[0]
         # if there's only one code, and select_code_idx not given, just copy it
     else:
         if select_code_idx is None:
             console.print(
-                "[dim]There are more than one code in ChatGPT's last reply")
+                _("gpt_term.code_too_many_found"))
             code_num = 0
             for codes in code_list:
                 code_num += 1
-                console.print(f"[yellow]Code {code_num}:")
+                console.print(_("gpt_term.code_num",code_num=code_num))
                 console.print(Markdown(codes))
 
             select_code_idx = prompt(
-                "Please select which code to copy: ", style=style, validator=NumberValidator())
+                _("gpt_term.code_select"), style=style, validator=NumberValidator())
             # get the number of the selected code
         try:
             selected_code = code_list[int(select_code_idx)-1]
         except ValueError:
-            console.print("[red]Code index must be an Integer")
+            console.print(_("gpt_term.code_index_must_int"))
             return
         except IndexError:
             if len(code_list) == 1:
                 console.print(
-                    "[red]Index out of range: There is only one code in ChatGPT's last reply")
+                    _("gpt_term.code_index_out_range_one"))
             else:
                 console.print(
-                    f"[red]Index out of range: You should input an Integer in range 1 ~ {len(code_list)}")
+                    _("gpt_term.code_index_out_range_many",len(code_list)))
                 # show idx range
                 # use len(code_list) instead of code_num as the max of idx
                 # in order to avoid error 'UnboundLocalError: local variable 'code_num' referenced before assignment' when inputing select_code_idx directly
             return
 
     bpos = selected_code.find('\n')    # code begin pos.
     epos = selected_code.rfind('```')  # code end pos.
     pyperclip.copy(''.join(selected_code[bpos+1:epos-1]))
     # erase code begin and end sign
-    console.print("[dim]Code copied to Clipboard")
+    console.print(_("gpt_term.code_copy"))
 
 
 def change_CLI_title(new_title: str):
     if platform.system() == "Windows":
         os.system(f"title {new_title}")
     else:
         print(f"\033]0;{new_title}\007", end='')
@@ -719,76 +724,76 @@
                 v[i][j] = min(v[i-1][j-1], min(v[i][j-1], v[i-1][j])) + 1
 
     return v[s1_len][s2_len]
 
 
 def handle_command(command: str, chat_gpt: ChatGPT, key_bindings: KeyBindings, chat_save_perfix: str):
     '''处理斜杠(/)命令'''
+    global _
     if command == '/raw':
         ChatMode.toggle_raw_mode()
     elif command == '/multi':
         ChatMode.toggle_multi_line_mode()
 
     elif command.startswith('/stream'):
         args = command.split()
         if len(args) > 1:
             chat_gpt.set_stream_overflow(args[1])
         else:
             ChatMode.toggle_stream_mode()
 
     elif command == '/tokens':
         chat_gpt.threadlock_total_tokens_spent.acquire()
-        console.print(Panel(f"[bold bright_magenta]Total Tokens Spent:[/]\t{chat_gpt.total_tokens_spent}\n"
-                            f"[bold green]Current Tokens:[/]\t\t{chat_gpt.current_tokens}/[bold]{chat_gpt.tokens_limit}",
-                            title='token_summary', title_align='left', width=40))
+        console.print(Panel(_("gpt_term.tokens_used",total_tokens_spent=chat_gpt.total_tokens_spent,current_tokens=chat_gpt.current_tokens,tokens_limit=chat_gpt.tokens_limit),
+                            title=_("gpt_term.tokens_title"), title_align='left', width=40))
         chat_gpt.threadlock_total_tokens_spent.release()
 
     elif command == '/usage':
-        with console.status("[cyan]Getting credit usage..."):
+        with console.status(_("gpt_term.usage_getting")):
             if not chat_gpt.get_credit_usage():
                 return
-        console.print(Panel(f"[bold green]Total Granted:[/]\t\t${format(chat_gpt.credit_total_granted, '.2f')}\n"
-                            f"[bold cyan]Used This Month:[/]\t${format(chat_gpt.credit_used_this_month, '.2f')}\n"
-                            f"[bold blue]Used Total:[/]\t\t${format(chat_gpt.credit_total_used, '.2f')}",
-                            title="Credit Summary", title_align='left', subtitle=f"[bright_blue]Plan: {chat_gpt.credit_plan}", width=35))
+        console.print(Panel(f'{_("gpt_term.usage_granted",credit_total_granted=format(chat_gpt.credit_total_granted, ".2f"))}\n'
+                            f'{_("gpt_term.usage_used_month",credit_used_this_month=format(chat_gpt.credit_used_this_month, ".2f"))}\n'
+                            f'{_("gpt_term.usage_total",credit_total_used=format(chat_gpt.credit_total_used, ".2f"))}',
+                            title=_("gpt_term.usage_title"), title_align='left', subtitle=_("gpt_term.usage_plan",credit_plan=chat_gpt.credit_plan), width=35))
 
     elif command.startswith('/model'):
         args = command.split()
         if len(args) > 1:
             new_model = args[1]
         else:
             new_model = prompt(
                 "OpenAI API model: ", default=chat_gpt.model, style=style)
         if new_model != chat_gpt.model:
             chat_gpt.set_model(new_model)
         else:
-            console.print("[dim]No change.")
+            console.print(_("gpt_term.No_change"))
 
     elif command == '/last':
         reply = chat_gpt.messages[-1]
         print_message(reply)
 
     elif command.startswith('/copy'):
         args = command.split()
         reply = chat_gpt.messages[-1]
         if len(args) > 1:
             if args[1] == 'all':
                 pyperclip.copy(reply["content"])
-                console.print("[dim]Last reply copied to Clipboard")
+                console.print(_("gpt_term.code_last_copy"))
             elif args[1] == 'code':
                 if len(args) > 2:
                     copy_code(reply, args[2])
                 else:
                     copy_code(reply)
             else:
                 console.print(
-                    "[dim]Nothing to do. Available copy command: `[bright_magenta]/copy code \[index][/]` or `[bright_magenta]/copy all[/]`")
+                    _("gpt_term.code_copy_fail"))
         else:
             pyperclip.copy(reply["content"])
-            console.print("[dim]Last reply copied to Clipboard")
+            console.print(_("gpt_term.code_last_copy"))
 
     elif command.startswith('/save'):
         args = command.split()
         if len(args) > 1:
             filename = args[1]
         else:
             gen_filename = chat_gpt.gen_title()
@@ -804,150 +809,146 @@
 
     elif command.startswith('/system'):
         args = command.split()
         if len(args) > 1:
             new_content = ' '.join(args[1:])
         else:
             new_content = prompt(
-                "System prompt: ", default=chat_gpt.messages[0]['content'], style=style, key_bindings=key_bindings)
+                _("gpt_term.system_prompt"), default=chat_gpt.messages[0]['content'], style=style, key_bindings=key_bindings)
         if new_content != chat_gpt.messages[0]['content']:
             chat_gpt.modify_system_prompt(new_content)
         else:
-            console.print("[dim]No change.")
+            console.print(_("gpt_term.No_change"))
 
     elif command.startswith('/rand') or command.startswith('/temperature'):
         args = command.split()
         if len(args) > 1:
             new_temperature = args[1]
         else:
             new_temperature = prompt(
-                "New Randomness: ", default=str(chat_gpt.temperature), style=style, validator=temperature_validator)
+                _("gpt_term.new_temperature"), default=str(chat_gpt.temperature), style=style, validator=temperature_validator)
         if new_temperature != str(chat_gpt.temperature):
             chat_gpt.set_temperature(new_temperature)
         else:
-            console.print("[dim]No change.")            
+            console.print(_("gpt_term.No_change"))            
 
     elif command.startswith('/title'):
         args = command.split()
         if len(args) > 1:
             chat_gpt.title = ' '.join(args[1:])
             change_CLI_title(chat_gpt.title)
         else:
             # generate a new title
             new_title = chat_gpt.gen_title(force=True)
             if not new_title:
-                console.print("[red]Failed to generate title.")
+                console.print(_("gpt_term.title_gen_fail"))
                 return
-        console.print(f"[dim]CLI Title changed to '{chat_gpt.title}'")
+        console.print(_('gpt_term.title_changed',title=chat_gpt.title))
 
     elif command.startswith('/timeout'):
         args = command.split()
         if len(args) > 1:
             new_timeout = args[1]
         else:
             new_timeout = prompt(
-                "OpenAI API timeout: ", default=str(chat_gpt.timeout), style=style)
+                _("gpt_term.timeout_prompt"), default=str(chat_gpt.timeout), style=style)
         if new_timeout != str(chat_gpt.timeout):
             chat_gpt.set_timeout(new_timeout)
         else:
-            console.print("[dim]No change.")
+            console.print(_("gpt_term.No_change"))
 
     elif command == '/undo':
         if len(chat_gpt.messages) > 2:
             question = chat_gpt.messages.pop()
             if question['role'] == "assistant":
                 question = chat_gpt.messages.pop()
             truncated_question = question['content'].split('\n')[0]
             if len(question['content']) > len(truncated_question):
                 truncated_question += "..."
             console.print(
-                f"[dim]Last question: '{truncated_question}' and it's answer has been removed.")
+                _("gpt_term.undo_removed",truncated_question=truncated_question))
             chat_gpt.current_tokens = count_token(chat_gpt.messages)
         else:
-            console.print("[dim]Nothing to undo.")
+            console.print(_("gpt_term.undo_nothing"))
 
     elif command.startswith('/reset'):
         chat_gpt.delete_all_conversation()
 
     elif command.startswith('/delete'):
         args = command.split()
         if len(args) > 1:
             if args[1] == 'first':
                 chat_gpt.delete_first_conversation()
             elif args[1] == 'all':
                 chat_gpt.delete_all_conversation()
             else:
                 console.print(
-                    "[dim]Nothing to do. Avaliable delete command: `[bright_magenta]/delete first[/]` or `[bright_magenta]/delete all[/]`")
+                    _("gpt_term.delete_nothing"))
         else:
             chat_gpt.delete_first_conversation()
 
     elif command == '/version':
         threadlock_remote_version.acquire()
-        console.print(Panel(f"[bold blue]Local Version:[/]\tv{str(local_version)}\n"
-                            f"[bold green]Remote Version:[/]\tv{str(remote_version)}",
-                            title='Version', title_align='left', width=28))
+        string=_("gpt_term.version_all",local_version=str(local_version),remote_version=str(remote_version))
+        console.print(Panel(string,
+                            title=_("gpt_term.version_name"), title_align='left', width=28))
         threadlock_remote_version.release()
+    
+    elif command.startswith('/lang'):
+        args = command.split()
+        if len(args) > 1:
+            new_lang = args[1]
+        else:
+            new_lang = prompt(
+                _("gpt_term.new_lang_prompt"), default=get_lang(), style=style)
+        if new_lang != get_lang():
+            if new_lang in supported_langs:
+                _=set_lang(new_lang)
+                console.print(_("gpt_term.lang_switch"))
+            else:
+                console.print(_("gpt_term.lang_unsupport", new_lang=new_lang))
+        else:
+            console.print(_("gpt_term.No_change"))
 
     elif command == '/exit':
         raise EOFError
 
     elif command == '/help':
-        console.print('''[bold]Available commands:[/]
-    /raw                     - Toggle raw mode (showing raw text of ChatGPT's reply)
-    /multi                   - Toggle multi-line mode (allow multi-line input)
-    /stream \[overflow_mode]  - Toggle stream output mode (flow print the answer)
-    /tokens                  - Show the total tokens spent and the tokens for the current conversation
-    /usage                   - Show total credits and current credits used
-    /last                    - Display last ChatGPT's reply
-    /copy (all)              - Copy the full ChatGPT's last reply (raw) to Clipboard
-    /copy code \[index]       - Copy the code in ChatGPT's last reply to Clipboard
-    /save \[filename_or_path] - Save the chat history to a file, suggest title if filename_or_path not provided
-    /model \[model_name]      - Change AI model
-    /system \[new_prompt]     - Modify the system prompt
-    /rand \[randomness]       - Set Model sampling temperature (0~2)
-    /title \[new_title]       - Set title for this chat, if new_title is not provided, a new title will be generated
-    /timeout \[new_timeout]   - Modify the api timeout
-    /undo                    - Undo the last question and remove its answer
-    /delete (first)          - Delete the first conversation in current chat
-    /delete all              - Clear all messages and conversations current chat
-    /version                 - Show gpt-term local and remote version
-    /help                    - Show this help message
-    /exit                    - Exit the application''')
+        console.print(_("gpt_term.help_text"))
         
     else:
         set_command = set(command)
         min_levenshtein_distance = len(command)
         most_similar_command = ""
         for slash_command in command_completer.nested_completer.options.keys():
             this_levenshtein_distance = get_levenshtein_distance(command, slash_command)
             if this_levenshtein_distance < min_levenshtein_distance:
                 set_slash_command = set(slash_command)
                 if len(set_command & set_slash_command) / len(set_command | set_slash_command) >= 0.75:
                     most_similar_command = slash_command
                     min_levenshtein_distance = this_levenshtein_distance
         
-        console.print(f"Unrecognized Slash Command `[bold red]{command}[/]`", end=" ")
+        console.print(_("gpt_term.help_uncommand",command=command), end=" ")
         if most_similar_command:
-            console.print(f"Do you mean `[bright magenta]{most_similar_command}[/]`?")
+            console.print(_("gpt_term.help_mean_command",most_similar_command=most_similar_command))
         else:
             console.print("")
-        console.print("Use `[bright magenta]/help[/]` to see all available slash commands")
+        console.print(_("gpt_term.help_use_help"))
 
 
 def load_chat_history(file_path):
     '''从 file_path 加载聊天记录'''
     try:
         with open(file_path, 'r', encoding='utf-8') as f:
             chat_history = json.load(f)
         return chat_history
     except FileNotFoundError:
-        console.print(f"[bright_red]File not found: {file_path}")
+        console.print(_("gpt_term.load_file_not",file_path=file_path))
     except json.JSONDecodeError:
-        console.print(f"[bright_red]Invalid JSON format in file: {file_path}")
+        console.print(_("gpt_term.load_json_error",file_path=file_path))
     return None
 
 
 def create_key_bindings():
     '''自定义回车事件绑定，实现斜杠命令的提交忽略多行模式，以及单行模式下 `esc+Enter` 换行'''
     key_bindings = KeyBindings()
 
@@ -989,69 +990,95 @@
 
 def write_config(config_ini: ConfigParser):
     with open(f'{data_dir}/config.ini', 'w') as configfile:
         config_ini.write(configfile)
 
 
 def set_config_by_args(args: argparse.Namespace, config_ini: ConfigParser):
+    global _
     config_need_to_set = {}
     if args.set_apikey:     config_need_to_set.update({"OPENAI_API_KEY"      : args.set_apikey})
     if args.set_timeout:    config_need_to_set.update({"OPENAI_API_TIMEOUT"  : args.set_timeout})
     if args.set_saveperfix: config_need_to_set.update({"CHAT_SAVE_PERFIX"    : args.set_saveperfix})
     if args.set_loglevel:   config_need_to_set.update({"LOG_LEVEL"           : args.set_loglevel})
     if args.set_gentitle:   config_need_to_set.update({"AUTO_GENERATE_TITLE" : args.set_gentitle})
+    # 新的语言设置:
+    if args.set_lang:       config_need_to_set.update({"LANGUAGE"            : args.set_lang})
 
     if len(config_need_to_set) == 0:
         return
     # nothing to set
-
     for key, val in config_need_to_set.items():
         config_ini['DEFAULT'][key] = str(val)
-        console.print(f"Config item `[bright_magenta]{key}[/]` is set to [green]{val}[/]")
+        console.print(_("gpt_term.config_key_to_shell_key",key_word=str(key),val=str(val)))
 
     write_config(config_ini)
     exit(0)
 
 
 def main():
-    parser = argparse.ArgumentParser(description='Use ChatGPT in terminal')
-    parser.add_argument('--version', action='version', version=f'%(prog)s v{local_version}')
-    parser.add_argument('--load', metavar='FILE', type=str, help='Load chat history from file')
-    parser.add_argument('--key', type=str, help='Choose the API key to load')
-    parser.add_argument('--model', type=str, help='Choose the AI model to use')
-    parser.add_argument('-m', '--multi', action='store_true', help='Enable multi-line mode')
-    parser.add_argument('-r', '--raw', action='store_true', help='Enable raw mode')
-    # normal function args
-
-    parser.add_argument('--set-apikey', metavar='KEY', type=str, help='Set API key for OpenAI')
-    parser.add_argument('--set-timeout', metavar='SEC', type=int, help='Set maximum waiting time for API requests')
-    parser.add_argument('--set-gentitle', metavar='BOOL', type=str, help='Set whether to automatically generate a title for chat')
-    parser.add_argument('--set-saveperfix', metavar='PERFIX', type=str, help='Set chat history file\'s save perfix')
-    parser.add_argument('--set-loglevel', metavar='LEVEL', type=str, help='Set log level: DEBUG, INFO, WARNING, ERROR, CRITICAL')
-    # setting args
-    args = parser.parse_args()
+    global _, supported_langs
+    supported_langs = ["en","zh_CN","jp","de"]
+    local_lang = locale.getdefaultlocale()[0]
+    if local_lang not in supported_langs:
+        local_lang = "en"
+    _=set_lang(local_lang)
 
     # 读取配置文件
     config_ini = ConfigParser()
     config_ini.read(f'{data_dir}/config.ini', encoding='utf-8')
     config = config_ini['DEFAULT']
 
+    # 读取语言配置
+    config_lang = config.get("language")
+    if config_lang:
+        if config_lang in supported_langs:
+            _=set_lang(config_lang)
+            console.print(_("gpt_term.lang_switch"))
+        else:
+            console.print(_("gpt_term.lang_config_unsupport", config_lang=config_lang))
+
+    parser = argparse.ArgumentParser(description=_("gpt_term.help_description"),add_help=False)
+    parser.add_argument('-h', '--help',action='help', help=_("gpt_term.help_help"))
+    parser.add_argument('-v','--version', action='version', version=f'%(prog)s v{local_version}',help=_("gpt_term.help_v"))
+    parser.add_argument('--load', metavar='FILE', type=str, help=_("gpt_term.help_load"))
+    parser.add_argument('--key', type=str, help=_("gpt_term.help_key"))
+    parser.add_argument('--model', type=str, help=_("gpt_term.help_model"))
+    parser.add_argument('-m', '--multi', action='store_true', help=_("gpt_term.help_m"))
+    parser.add_argument('-r', '--raw', action='store_true', help=_("gpt_term.help_r"))
+    ## 新添加的选项：--lang
+    parser.add_argument('-l','--lang', type=str, choices=['en', 'zh_CN', 'jp', 'de'], help=_("gpt_term.help_lang"))
+    # normal function args
+
+    parser.add_argument('--set-apikey', metavar='KEY', type=str, help=_("gpt_term.help_set_key"))
+    parser.add_argument('--set-timeout', metavar='SEC', type=int, help=_("gpt_term.help_set_timeout"))
+    parser.add_argument('--set-gentitle', metavar='BOOL', type=str, help=_("gpt_term.help_set_gentitle"))
+    ## 新添加的选项：--set-lang
+    parser.add_argument('--set-lang', type=str, choices=['en', 'zh_CN', 'jp', 'de'], help=_("gpt_term.help_set_lang"))
+    parser.add_argument('--set-saveperfix', metavar='PERFIX', type=str, help=_("gpt_term.help_set_saveperfix"))
+    parser.add_argument('--set-loglevel', metavar='LEVEL', type=str, help=_("gpt_term.help_set_loglevel")+'DEBUG, INFO, WARNING, ERROR, CRITICAL')
+    # setting args
+    args = parser.parse_args()
+
     set_config_by_args(args, config_ini)
 
+    if args.lang:
+        _=set_lang(args.lang)
+        console.print(_("gpt_term.lang_switch"))
+
     try:
         log_level = getattr(logging, config.get("LOG_LEVEL", "INFO").upper())
     except AttributeError as e:
         console.print(
-            f"[dim]Invalid log level: {e}, check config.ini file. Set log level to INFO.")
+            _("gpt_term.log_level_error"))
         log_level = logging.INFO
     log.setLevel(log_level)
     # log level set must be before debug logs, because default log level is INFO, and before new log level being set debug logs will not be written to log file
 
     log.info("GPT-Term start")
-
     log.debug(f"Local version: {str(local_version)}")
     # get local version from pkg resource
 
     check_remote_update_thread = threading.Thread(target=get_remote_version, daemon=True)
     check_remote_update_thread.start()
     log.debug("Remote version get thread started")
     # try to get remote version and check update
@@ -1062,16 +1089,16 @@
         log.debug(f"Try loading API key with {args.key} from config.ini")
         api_key = config.get(args.key)
     else:
         api_key = config.get("OPENAI_API_KEY")
 
     if not api_key:
         log.debug("API Key not found, waiting for input")
-        api_key = prompt("OpenAI API Key not found, please input: ")
-        if confirm('Save API Key to config file?'):
+        api_key = prompt(_("gpt_term.input_api_key"))
+        if confirm(_("gpt_term.save_api_key")):
             config["OPENAI_API_KEY"] = api_key
             write_config(config_ini)
 
     api_key_log = api_key[:3] + '*' * (len(api_key) - 7) + api_key[-4:]
     log.debug(f"Loaded API Key: {api_key_log}")
 
     api_timeout = config.getfloat("OPENAI_API_TIMEOUT", 30)
@@ -1086,17 +1113,14 @@
         log.debug("Auto title generation [bright_red]disabled[/]")
 
     gen_title_daemon_thread = threading.Thread(
         target=chat_gpt.auto_gen_title_background, daemon=True)
     gen_title_daemon_thread.start()
     log.debug("Title generation daemon thread started")
 
-    console.print(
-        "[dim]Hi, welcome to chat with GPT. Type `[bright_magenta]/help[/]` to display available commands.")
-
     if args.model:
         chat_gpt.set_model(args.model)
 
     if args.multi:
         ChatMode.toggle_multi_line_mode()
 
     if args.raw:
@@ -1108,28 +1132,31 @@
             change_CLI_title(args.load.rstrip(".json"))
             chat_gpt.messages = chat_history
             for message in chat_gpt.messages:
                 print_message(message)
             chat_gpt.current_tokens = count_token(chat_gpt.messages)
             log.info(f"Chat history successfully loaded from: {args.load}")
             console.print(
-                f"[dim]Chat history successfully loaded from: [bright_magenta]{args.load}", highlight=False)
+                _("gpt_term.load_chat_history",load=args.load), highlight=False)
+
+    console.print(
+        _("gpt_term.welcome"))
 
     session = PromptSession()
 
     # 绑定回车事件，达到自定义多行模式的效果
     key_bindings = create_key_bindings()
 
     while True:
         try:
             message = session.prompt(
                 '> ', completer=command_completer, complete_while_typing=True, key_bindings=key_bindings)
 
             if message.startswith('/'):
-                command = message.strip().lower()
+                command = message.strip()
                 handle_command(command, chat_gpt,
                                key_bindings, chat_save_perfix)
             else:
                 if not message:
                     continue
 
                 log.info(f"> {message}")
@@ -1137,25 +1164,25 @@
 
                 if message.lower() in ['再见', 'bye', 'goodbye', '结束', 'end', '退出', 'exit', 'quit']:
                     break
 
         except KeyboardInterrupt:
             continue
         except EOFError:
-            console.print("Exiting...")
+            console.print(_("gpt_term.exit"))
             break
 
     log.info(f"Total tokens spent: {chat_gpt.total_tokens_spent}")
     console.print(
-        f"[bright_magenta]Total tokens spent: [bold]{chat_gpt.total_tokens_spent}")
+        _("gpt_term.spent_token",total_tokens_spent=chat_gpt.total_tokens_spent))
     
     threadlock_remote_version.acquire()
     if remote_version and remote_version > local_version:
         console.print(Panel(Group(
-            Markdown("Use `pip install --upgrade gpt-term` to upgrade."),
-            Markdown("Visit our [GitHub Site](https://github.com/xiaoxx970/chatgpt-in-terminal) to see what have been changed!")),
-            title=f"New Version Available: [red]v{str(local_version)}[/] -> [green]v{str(remote_version)}[/]",
+            Markdown(_("gpt_term.upgrade_use_command")),
+            Markdown(_("gpt_term.upgrade_see_git"))),
+            title=_("gpt_term.upgrade_title",local_version=str(local_version),remote_version=str(remote_version)),
             width=58, style="blue", title_align="left"))
     threadlock_remote_version.release()
 
 if __name__ == "__main__":
     main()
```

### Comparing `gpt-term-1.0.5/gpt_term.egg-info/PKG-INFO` & `gpt-term-1.1.0/gpt_term.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-term
-Version: 1.0.5
+Version: 1.1.0
 Summary: Chat with GPT in Terminal
 Author: xiaoxx970, Ace-Radom
 License: MIT License
         
         Copyright (c) 2023 xiaoxx970
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -53,27 +53,31 @@
 
 ![example](https://github.com/xiaoxx970/chatgpt-in-terminal/raw/main/README.assets/small.gif)
 
 Uses the [gpt-3.5-turbo](https://platform.openai.com/docs/guides/chat/chat-completions-beta) model, which is the same model used by ChatGPT (Free Edition), as default.
 
 ## Changelog
 
+### 2023-05-18
+
+- Added multi-language support: English, Chinese, Japanese, German, follow the system language by default, now you can use `/lang` to switch languages
+
+<details>
+  <summary>More Change log</summary>
+
 ### 2023-05-11
 
 - Find the command the user most likely intended to enter when typing an unrecognized command
 
 ### 2023-05-05
 
 - Add `/rand` command to set temperature parameter
 
 - Add overflow mode switch for `/stream` command, now you can run command `/stream visible` to switch to always visible mode. In this mode, the content that exceeds the screen will be scrolled up, and the new content will be output until it is completed
 
-<details>
-  <summary>More Change log</summary>
-
 ### 2023-04-23
 Released `gpt-term` on [Pypi](https://pypi.org/project/gpt-term/), started version control. No need to clone the project locally anymore, simply use the `pip` command to install gpt-term.
 
 ### 2023-04-15
 
 - Added the ability to create a line break in single-line mode using `Esc` + `Enter`
 
@@ -182,14 +186,15 @@
 | -m, --multi   | Enable multi-line mode          | `gpt-term --multi`                            |
 | -r, --raw     | Enable raw mode                 | `gpt-term --raw`                              |
 | --set-apikey KEY        | Set the OpenAI API key                                   | `gpt-term --set-apikey sk-xxx`   |
 | --set-timeout SEC       | Set the maximum wait time for API requests               | `gpt-term --set-timeout 10`      |
 | --set-gentitle BOOL     | Set whether to auto-generate a title for the chat        | `gpt-term --set-gentitle True`   |
 | --set-saveperfix PERFIX | Set the save prefix for chat history files               | `gpt-term --set-saveperfix chat_history_` |
 | --set-loglevel LEVEL    | Set the log level: DEBUG, INFO, WARNING, ERROR, CRITICAL | `gpt-term --set-loglevel DEBUG`  |
+| --set-lang LANG    | Set the language: en, zh_CN, jp, de | `gpt-term --set-lang en` |
 
 > Multi-line mode and raw mode can be used simultaneously
 
 ### Configuration File
 
 The configuration file is located at `~/.gpt-term/config.ini` and is autogenerated. It can be modified using the program's `--set` option or edited manually.
 
@@ -208,14 +213,17 @@
 
 # Define the default file prefix when the /save command saves the chat history. The default value is "./chat_history_", which means that the chat history will be saved in the file starting with "chat_history_" in the current directory
 # At the same time, the prefix can also be specified as a directory + / to allow the program to save the chat history in a folder (note that the corresponding folder needs to be created in advance), for example: CHAT_SAVE_PERFIX=chat_history/
 CHAT_SAVE_PERFIX=./chat_history_
 
 # Log level, default is INFO, available value: DEBUG, INFO, WARNING, ERROR, CRITICAL
 LOG_LEVEL=INFO
+
+# Set the language of the program, the default is empty, it will follow the system language
+LANGUAGE=
 ```
 
 ### Available Commands
 
 - `/raw`: Display raw text in replies instead of rendered Markdown format
 
   > After switching, use the `/last` command to reprint the last reply
```

### Comparing `gpt-term-1.0.5/pyproject.toml` & `gpt-term-1.1.0/pyproject.toml`

 * *Files identical despite different names*

