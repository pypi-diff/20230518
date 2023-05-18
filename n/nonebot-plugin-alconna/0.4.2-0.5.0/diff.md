# Comparing `tmp/nonebot-plugin-alconna-0.4.2.tar.gz` & `tmp/nonebot-plugin-alconna-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-alconna-0.4.2.tar", last modified: Sat May 13 01:54:28 2023, max compression
+gzip compressed data, was "nonebot-plugin-alconna-0.5.0.tar", last modified: Thu May 18 16:53:07 2023, max compression
```

## Comparing `nonebot-plugin-alconna-0.4.2.tar` & `nonebot-plugin-alconna-0.5.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 nonebot-plugin-alconna-0.4.2/LICENSE
--rw-r--r--   0        0        0     1135 2023-05-13 01:53:49.312142 nonebot-plugin-alconna-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     8579 2023-05-11 05:49:49.600962 nonebot-plugin-alconna-0.4.2/README.md
--rw-r--r--   0        0        0     1208 2023-05-10 08:50:46.247626 nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/__init__.py
--rw-r--r--   0        0        0      383 2023-05-11 04:41:26.166268 nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/adapters/__init__.py
--rw-r--r--   0        0        0      523 2023-05-10 10:09:15.599546 nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/adapters/bilibili.py
--rw-r--r--   0        0        0     1007 2023-05-10 10:09:15.573188 nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/adapters/console.py
--rw-r--r--   0        0        0     1661 2023-05-10 10:09:15.609172 nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/adapters/ding.py
--rw-r--r--   0        0        0     2141 2023-05-10 10:09:15.564123 nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/adapters/feishu.py
--rw-r--r--   0        0        0      519 2023-05-10 10:09:15.541809 nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/adapters/github.py
--rw-r--r--   0        0        0     1163 2023-05-10 10:09:15.636179 nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/adapters/kook.py
--rw-r--r--   0        0        0      761 2023-05-10 10:09:15.651191 nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/adapters/minecraft.py
--rw-r--r--   0        0        0     3155 2023-05-10 10:09:15.519983 nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/adapters/mirai.py
--rw-r--r--   0        0        0     1088 2023-05-10 10:09:15.628175 nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/adapters/ntchat.py
--rw-r--r--   0        0        0     3177 2023-05-10 10:09:15.618177 nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/adapters/onebot11.py
--rw-r--r--   0        0        0     2517 2023-05-10 10:09:15.661217 nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/adapters/onebot12.py
--rw-r--r--   0        0        0     3227 2023-05-10 10:09:15.529594 nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/adapters/qqguild.py
--rw-r--r--   0        0        0     3126 2023-05-10 10:09:15.670151 nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/adapters/telegram.py
--rw-r--r--   0        0        0      581 2023-05-10 10:09:15.553296 nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/argv.py
--rw-r--r--   0        0        0      405 2023-05-10 09:00:57.054628 nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/config.py
--rw-r--r--   0        0        0      180 2023-05-10 08:33:24.079951 nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/consts.py
--rw-r--r--   0        0        0      109 2023-05-11 15:42:43.320472 nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/i18n/.config.json
--rw-r--r--   0        0        0      301 2023-05-11 15:42:18.920450 nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/i18n/en-US.json
--rw-r--r--   0        0        0      262 2023-05-11 15:42:18.885191 nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/i18n/zh-CN.json
--rw-r--r--   0        0        0     3812 2023-05-10 09:00:57.030628 nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/matcher.py
--rw-r--r--   0        0        0     1499 2023-05-10 08:54:25.558632 nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/matcher.pyi
--rw-r--r--   0        0        0     1448 2023-05-11 15:34:24.694684 nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/model.py
--rw-r--r--   0        0        0     2187 2023-04-02 14:03:55.798752 nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/params.py
--rw-r--r--   0        0        0     9210 2023-05-13 01:50:44.284586 nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/rule.py
--rw-r--r--   0        0        0     1967 2023-05-11 04:48:52.932671 nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/typings.py
--rw-r--r--   0        0        0     8658 1970-01-01 00:00:00.000000 nonebot-plugin-alconna-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 nonebot-plugin-alconna-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1135 2023-05-18 16:06:27.923196 nonebot-plugin-alconna-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     8401 2023-05-18 16:06:27.910527 nonebot-plugin-alconna-0.5.0/README.md
+-rw-r--r--   0        0        0     1241 2023-05-18 15:49:31.978140 nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/__init__.py
+-rw-r--r--   0        0        0      383 2023-05-11 04:41:26.166268 nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/adapters/__init__.py
+-rw-r--r--   0        0        0      523 2023-05-10 10:09:15.599546 nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/adapters/bilibili.py
+-rw-r--r--   0        0        0     1007 2023-05-10 10:09:15.573188 nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/adapters/console.py
+-rw-r--r--   0        0        0     1661 2023-05-10 10:09:15.609172 nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/adapters/ding.py
+-rw-r--r--   0        0        0     2141 2023-05-10 10:09:15.564123 nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/adapters/feishu.py
+-rw-r--r--   0        0        0      519 2023-05-10 10:09:15.541809 nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/adapters/github.py
+-rw-r--r--   0        0        0     1163 2023-05-10 10:09:15.636179 nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/adapters/kook.py
+-rw-r--r--   0        0        0      761 2023-05-10 10:09:15.651191 nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/adapters/minecraft.py
+-rw-r--r--   0        0        0     3155 2023-05-10 10:09:15.519983 nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/adapters/mirai.py
+-rw-r--r--   0        0        0     1088 2023-05-10 10:09:15.628175 nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/adapters/ntchat.py
+-rw-r--r--   0        0        0     3177 2023-05-10 10:09:15.618177 nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/adapters/onebot11.py
+-rw-r--r--   0        0        0     2517 2023-05-10 10:09:15.661217 nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/adapters/onebot12.py
+-rw-r--r--   0        0        0     3227 2023-05-10 10:09:15.529594 nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/adapters/qqguild.py
+-rw-r--r--   0        0        0     3126 2023-05-10 10:09:15.670151 nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/adapters/telegram.py
+-rw-r--r--   0        0        0      581 2023-05-10 10:09:15.553296 nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/argv.py
+-rw-r--r--   0        0        0      405 2023-05-10 09:00:57.054628 nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/config.py
+-rw-r--r--   0        0        0      180 2023-05-10 08:33:24.079951 nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/consts.py
+-rw-r--r--   0        0        0      109 2023-05-11 15:42:43.320472 nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/i18n/.config.json
+-rw-r--r--   0        0        0      301 2023-05-11 15:42:18.920450 nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/i18n/en-US.json
+-rw-r--r--   0        0        0      262 2023-05-11 15:42:18.885191 nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/i18n/zh-CN.json
+-rw-r--r--   0        0        0     2405 2023-05-18 15:49:32.019141 nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/matcher.py
+-rw-r--r--   0        0        0     1231 2023-05-18 15:49:32.003141 nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/matcher.pyi
+-rw-r--r--   0        0        0     1448 2023-05-11 15:34:24.694684 nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/model.py
+-rw-r--r--   0        0        0     3819 2023-05-18 16:17:32.686671 nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/params.py
+-rw-r--r--   0        0        0     8955 2023-05-18 16:51:04.066805 nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/rule.py
+-rw-r--r--   0        0        0     1967 2023-05-11 04:48:52.932671 nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/typings.py
+-rw-r--r--   0        0        0     8484 1970-01-01 00:00:00.000000 nonebot-plugin-alconna-0.5.0/PKG-INFO
```

### Comparing `nonebot-plugin-alconna-0.4.2/LICENSE` & `nonebot-plugin-alconna-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.4.2/pyproject.toml` & `nonebot-plugin-alconna-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "nonebot-plugin-alconna"
-version = "0.4.2"
+version = "0.5.0"
 description = "Alconna Adapter for Nonebot"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0rc4",
-    "arclet-alconna<2.0.0, >=1.7.0",
+    "arclet-alconna<2.0.0, >=1.7.3",
     "arclet-alconna-tools<0.7.0, >=0.6.0",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 keywords = [
     "command",
     "argparse",
```

### Comparing `nonebot-plugin-alconna-0.4.2/README.md` & `nonebot-plugin-alconna-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -150,15 +150,15 @@
 ```python
 ...
 from nonebot import require
 require("nonebot_plugin_alconna")
 ...
 
 from arclet.alconna import Alconna, Subcommand, Option, Args
-from nonebot_plugin_alconna import assign, on_alconna, AlconnaResult, CommandResult
+from nonebot_plugin_alconna import assign, on_alconna, AlconnaResult, CommandResult, Check
 
 pip = Alconna(
     "pip",
     Subcommand(
         "install", 
         Args["pak", str],
         Option("--upgrade"),
@@ -166,27 +166,25 @@
     ),
     Subcommand(
         "list",
         Option("--out-dated")
     )
 )
 
-pip_update = on_alconna(pip, [assign("install.pak", "pip")])
-pip_match_install = on_alconna(pip, [assign("install")])
-pip_match_list = on_alconna(pip, [assign("list")])
+pip_cmd = on_alconna(pip)
 
-@pip_update.handle()
+@pip_cmd.handle([Check(assign("install.pak", "pip"))])
 async def update(arp: CommandResult = AlconnaResult()):
     ...
 
-@pip_match_list.handle()
+@pip_cmd.handle([Check(assign("list"))])
 async def list_(arp: CommandResult = AlconnaResult()):
     ...
 
-@pip_match_install.handle()
+@pip_cmd.handle([Check(assign("install"))])
 async def install(arp: CommandResult = AlconnaResult()):
     ...
 ```
 
 
 ### Duplication
 
@@ -232,26 +230,24 @@
 - ALCONNA_AUTO_COMPLETION: 是否全局启用补全会话功能
 
 ## 参数解释
 
 ```python
 def on_alconna(
     command: Alconna | str,
-    checker: list[Callable[[Arparma], bool]] | None = None,
     skip_for_unmatch: bool = True,
     auto_send_output: bool = False,
     output_converter: Callable[[OutputType, str], Message | Awaitable[Message]] | None = None,
     aliases: set[str | tuple[str, ...]] | None = None,
     comp_config: CompConfig | None = None,
     **kwargs,
 ) -> type[Matcher]:
 ```
 
 - `command`: Alconna 命令
-- `checker`: 命令解析结果的检查器
 - `skip_for_unmatch`: 是否在命令不匹配时跳过该响应
 - `auto_send_output`: 是否自动发送输出信息并跳过响应
 - `output_converter`: 输出信息字符串转换为 Message 方法
 - `aliases`: 命令别名, 作用类似于 `on_command`
 - `comp_config`: 补全会话配置, 不传入则不启用补全会话
 
 ## 提供了 MessageSegment标注 的协议:
```

### Comparing `nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/adapters/bilibili.py` & `nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/adapters/bilibili.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/adapters/console.py` & `nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/adapters/console.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/adapters/ding.py` & `nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/adapters/ding.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/adapters/feishu.py` & `nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/adapters/feishu.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/adapters/github.py` & `nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/adapters/github.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/adapters/kook.py` & `nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/adapters/kook.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/adapters/minecraft.py` & `nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/adapters/minecraft.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/adapters/mirai.py` & `nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/adapters/mirai.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/adapters/ntchat.py` & `nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/adapters/ntchat.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/adapters/onebot11.py` & `nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/adapters/onebot11.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/adapters/onebot12.py` & `nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/adapters/onebot12.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/adapters/qqguild.py` & `nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/adapters/qqguild.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/adapters/telegram.py` & `nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/adapters/telegram.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/argv.py` & `nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/argv.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/matcher.pyi` & `nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/matcher.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 from __future__ import annotations
 
 from datetime import datetime, timedelta
-from typing import Any, Awaitable, Callable
+from typing import Awaitable, Callable
 
 from arclet.alconna import Alconna, Arparma
 from nonebot.adapters import Message
 from nonebot.dependencies import Dependent
 from nonebot.matcher import Matcher
 from nonebot.permission import Permission
 from nonebot.rule import Rule
 from nonebot.typing import T_Handler, T_PermissionChecker, T_RuleChecker, T_State
 from nonebot_plugin_alconna.typings import OutputType
 from nonebot_plugin_alconna.model import CompConfig
 
-def match_path(path: str): ...
-def match_value(path: str, value: Any, or_not: bool = False): ...
-def assign(
-    path: str, value: Any = ..., or_not: bool = False
-) -> Callable[[Arparma], bool]: ...
+
 def on_alconna(
     command: Alconna | str,
-    checker: list[Callable[[Arparma], bool]] | None = None,
     rule: Rule | T_RuleChecker | None = None,
     skip_for_unmatch: bool = True,
     auto_send_output: bool = False,
     output_converter: Callable[[OutputType, str], Message | Awaitable[Message]] | None = None,
     aliases: set[str | tuple[str, ...]] | None = None,
     comp_config: CompConfig | None = None,
     permission: Permission | T_PermissionChecker | None = ...,
```

### Comparing `nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/model.py` & `nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/model.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/rule.py` & `nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import asyncio
-from typing import Awaitable, Callable, ClassVar, List, Optional, Union, Dict
+from typing import Awaitable, Callable, ClassVar, Optional, Union, Dict
 
 from arclet.alconna import (
     Alconna,
     Arparma,
     Args,
     CompSession,
     AllParam,
@@ -11,14 +11,15 @@
     output_manager,
     namespace
 )
 import traceback
 from arclet.alconna.exceptions import SpecialOptionTriggered
 from nonebot import get_driver
 from nonebot.adapters import Bot, Event, Message
+from nonebot.internal.matcher import matchers
 from nonebot.internal.rule import Rule as Rule
 from nonebot.plugin.on import on_message
 from nonebot.params import EventMessage
 from nonebot.typing import T_State
 from nonebot.utils import is_coroutine_callable, run_sync
 from tarina import lang
 
@@ -29,38 +30,35 @@
 
 
 class AlconnaRule:
     """检查消息字符串是否能够通过此 Alconna 命令。
 
     参数:
         command: Alconna 命令
-        checker: 命令解析结果的检查器
         skip_for_unmatch: 是否在命令不匹配时跳过该响应
         auto_send_output: 是否自动发送输出信息并跳过响应
         output_converter: 输出信息字符串转换为 Message 方法
         comp_config: 自动补全配置
     """
 
     default_converter: ClassVar[
         Callable[[OutputType, str], Union[Message, Awaitable[Message]]]
     ] = lambda _, x: Message(x)
 
     __slots__ = (
         "command",
         "skip",
-        "checkers",
         "auto_send",
         "output_converter",
         "comp_config",
     )
 
     def __init__(
         self,
         command: Alconna,
-        checker: Optional[List[Callable[[Arparma], bool]]] = None,
         skip_for_unmatch: bool = True,
         auto_send_output: bool = False,
         output_converter: Optional[
             Callable[[OutputType, str], Union[Message, Awaitable[Message]]]
         ] = None,
         comp_config: Optional[CompConfig] = None,
     ):
@@ -76,15 +74,14 @@
                 command_manager.register(command)
             if config.alconna_auto_completion and not self.comp_config:
                 self.comp_config = {}
         except ValueError:
             self.auto_send = auto_send_output
         self.command = command
         self.skip = skip_for_unmatch
-        self.checkers = checker
         self.output_converter = output_converter or self.__class__.default_converter
         if not is_coroutine_callable(self.output_converter):
             self.output_converter = run_sync(self.output_converter)
 
     def __repr__(self) -> str:
         return f"Alconna(command={self.command!r})"
 
@@ -103,36 +100,39 @@
         with namespace("#completion") as ns:
             ns.prefixes = []
             ns.compact = True
             ns.hide = True
             _tab = Alconna(self.comp_config.get("tab", "/tab"), Args["offset", int, 1])
             _enter = Alconna(self.comp_config.get("enter", "/enter"), Args["content", AllParam, []])
             _exit = Alconna(self.comp_config.get("exit", "/exit"))
-        _waiter = on_message(priority=self.comp_config.get('priority', -100), block=True)
+
+        _waiter = on_message(priority=self.comp_config.get('priority', -1), block=True)
         _futures: Dict[str, asyncio.Future] = {}
         res = Arparma(self.command.path, msg, False, error_info=SpecialOptionTriggered("completion"))
 
         @_waiter.handle()
         async def _waiter_handle(_event: Event, content: Message = EventMessage()):
             if _exit.parse(content).matched:
                 _futures["_"].set_result(False)
                 await _waiter.finish()
             if (mat := _tab.parse(content)).matched:
                 interface.tab(mat.offset)
                 await _waiter.send(await self._convert("\n".join(interface.lines()), _event, res))
-                await _waiter.reject()
+                await _waiter.skip()
             if (mat := _enter.parse(content)).matched:
                 _futures["_"].set_result(mat.content)
                 await _waiter.finish()
             await _waiter.send(await self._convert(interface.current(), _event, res))
-            await _waiter.reject()
+            await _waiter.skip()
 
         def clear():
             interface.clear()
             _waiter.destroy()
+            _waiter.handlers.clear()
+            matchers.pop(-1)
             command_manager.delete(_tab)
             command_manager.delete(_enter)
             command_manager.delete(_exit)
 
         with interface:
             res = self.command.parse(msg)
         while interface.available:
@@ -186,17 +186,14 @@
                 arp = Arparma(self.command.path, msg, False, error_info=repr(e))
             may_help_text: Optional[str] = cap.get("output", None)
         if not arp.matched and not may_help_text and self.skip:
             return False
         if self.auto_send and may_help_text:
             await bot.send(event, await self._convert(may_help_text, event, arp))
             return False
-        for checker in self.checkers:
-            if not checker(arp):
-                return False
         state[ALCONNA_RESULT] = CommandResult(arp, may_help_text)
         return True
 
     async def _convert(self, text: str, event: Event, arp: Arparma) -> Message:
         _t = (
             str(arp.error_info)
             if isinstance(arp.error_info, SpecialOptionTriggered)
@@ -206,26 +203,24 @@
             return await self.output_converter(_t, text)  # type: ignore
         except NotImplementedError:
             return event.get_message().__class__(text)
 
 
 def alconna(
     command: Alconna,
-    checker: Optional[List[Callable[[Arparma], bool]]] = None,
     skip_for_unmatch: bool = True,
     auto_send_output: bool = False,
     output_converter: Optional[
         Callable[[OutputType, str], Union[Message, Awaitable[Message]]]
     ] = None,
     comp_config: Optional[CompConfig] = None,
 ) -> Rule:
     return Rule(
         AlconnaRule(
             command,
-            checker,
             skip_for_unmatch,
             auto_send_output,
             output_converter,
             comp_config,
         )
     )
```

### Comparing `nonebot-plugin-alconna-0.4.2/src/nonebot_plugin_alconna/typings.py` & `nonebot-plugin-alconna-0.5.0/src/nonebot_plugin_alconna/typings.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.4.2/PKG-INFO` & `nonebot-plugin-alconna-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-alconna
-Version: 0.4.2
+Version: 0.5.0
 Summary: Alconna Adapter for Nonebot
 License: MIT
 Keywords: command,argparse,cli,alconna,nonebot
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Project-URL: repository, https://github.com/ArcletProject/nonebot-plugin-alconna
 Description-Content-Type: text/markdown
@@ -161,15 +161,15 @@
 ```python
 ...
 from nonebot import require
 require("nonebot_plugin_alconna")
 ...
 
 from arclet.alconna import Alconna, Subcommand, Option, Args
-from nonebot_plugin_alconna import assign, on_alconna, AlconnaResult, CommandResult
+from nonebot_plugin_alconna import assign, on_alconna, AlconnaResult, CommandResult, Check
 
 pip = Alconna(
     "pip",
     Subcommand(
         "install", 
         Args["pak", str],
         Option("--upgrade"),
@@ -177,27 +177,25 @@
     ),
     Subcommand(
         "list",
         Option("--out-dated")
     )
 )
 
-pip_update = on_alconna(pip, [assign("install.pak", "pip")])
-pip_match_install = on_alconna(pip, [assign("install")])
-pip_match_list = on_alconna(pip, [assign("list")])
+pip_cmd = on_alconna(pip)
 
-@pip_update.handle()
+@pip_cmd.handle([Check(assign("install.pak", "pip"))])
 async def update(arp: CommandResult = AlconnaResult()):
     ...
 
-@pip_match_list.handle()
+@pip_cmd.handle([Check(assign("list"))])
 async def list_(arp: CommandResult = AlconnaResult()):
     ...
 
-@pip_match_install.handle()
+@pip_cmd.handle([Check(assign("install"))])
 async def install(arp: CommandResult = AlconnaResult()):
     ...
 ```
 
 
 ### Duplication
 
@@ -243,26 +241,24 @@
 - ALCONNA_AUTO_COMPLETION: 是否全局启用补全会话功能
 
 ## 参数解释
 
 ```python
 def on_alconna(
     command: Alconna | str,
-    checker: list[Callable[[Arparma], bool]] | None = None,
     skip_for_unmatch: bool = True,
     auto_send_output: bool = False,
     output_converter: Callable[[OutputType, str], Message | Awaitable[Message]] | None = None,
     aliases: set[str | tuple[str, ...]] | None = None,
     comp_config: CompConfig | None = None,
     **kwargs,
 ) -> type[Matcher]:
 ```
 
 - `command`: Alconna 命令
-- `checker`: 命令解析结果的检查器
 - `skip_for_unmatch`: 是否在命令不匹配时跳过该响应
 - `auto_send_output`: 是否自动发送输出信息并跳过响应
 - `output_converter`: 输出信息字符串转换为 Message 方法
 - `aliases`: 命令别名, 作用类似于 `on_command`
 - `comp_config`: 补全会话配置, 不传入则不启用补全会话
 
 ## 提供了 MessageSegment标注 的协议:
```

