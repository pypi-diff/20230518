# Comparing `tmp/nonebot_plugin_bottle-1.0.0.7.tar.gz` & `tmp/nonebot_plugin_bottle-1.0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bottle-1.0.0.7.tar", max compression
+gzip compressed data, was "nonebot_plugin_bottle-1.0.0.8.tar", max compression
```

## Comparing `nonebot_plugin_bottle-1.0.0.7.tar` & `nonebot_plugin_bottle-1.0.0.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     7592 2023-05-18 11:23:18.055650 nonebot_plugin_bottle-1.0.0.7/README.md
--rw-r--r--   0        0        0    19581 2023-05-18 11:23:18.055650 nonebot_plugin_bottle-1.0.0.7/nonebot_plugin_bottle/__init__.py
--rw-r--r--   0        0        0      636 2023-05-18 11:23:18.055650 nonebot_plugin_bottle-1.0.0.7/nonebot_plugin_bottle/config.py
--rw-r--r--   0        0        0    18367 2023-05-18 11:23:18.055650 nonebot_plugin_bottle-1.0.0.7/nonebot_plugin_bottle/data_source.py
--rw-r--r--   0        0        0     2647 2023-05-18 11:23:18.055650 nonebot_plugin_bottle-1.0.0.7/nonebot_plugin_bottle/migrations/449e066410fd_init_db.py
--rw-r--r--   0        0        0     1426 2023-05-18 11:23:18.055650 nonebot_plugin_bottle-1.0.0.7/nonebot_plugin_bottle/model.py
--rw-r--r--   0        0        0      625 2023-05-18 11:23:18.055650 nonebot_plugin_bottle-1.0.0.7/pyproject.toml
--rw-r--r--   0        0        0     8356 1970-01-01 00:00:00.000000 nonebot_plugin_bottle-1.0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     7617 2023-05-18 11:35:19.599344 nonebot_plugin_bottle-1.0.0.8/README.md
+-rw-r--r--   0        0        0    19581 2023-05-18 11:35:19.599344 nonebot_plugin_bottle-1.0.0.8/nonebot_plugin_bottle/__init__.py
+-rw-r--r--   0        0        0      636 2023-05-18 11:35:19.599344 nonebot_plugin_bottle-1.0.0.8/nonebot_plugin_bottle/config.py
+-rw-r--r--   0        0        0    18355 2023-05-18 11:35:19.599344 nonebot_plugin_bottle-1.0.0.8/nonebot_plugin_bottle/data_source.py
+-rw-r--r--   0        0        0     2647 2023-05-18 11:35:19.599344 nonebot_plugin_bottle-1.0.0.8/nonebot_plugin_bottle/migrations/449e066410fd_init_db.py
+-rw-r--r--   0        0        0     1426 2023-05-18 11:35:19.599344 nonebot_plugin_bottle-1.0.0.8/nonebot_plugin_bottle/model.py
+-rw-r--r--   0        0        0      625 2023-05-18 11:35:19.599344 nonebot_plugin_bottle-1.0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     8380 1970-01-01 00:00:00.000000 nonebot_plugin_bottle-1.0.0.8/PKG-INFO
```

### Comparing `nonebot_plugin_bottle-1.0.0.7/README.md` & `nonebot_plugin_bottle-1.0.0.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     - `扔漂流瓶` [文本/图片]
     - `寄漂流瓶` [文本/图片] （同`扔漂流瓶`，防止指令冲突用）
     - `捡漂流瓶` 
     - `评论漂流瓶` [漂流瓶编号] [文本]
     - `举报漂流瓶` [漂流瓶编号]
     - `查看漂流瓶` [漂流瓶编号]
     - `删除漂流瓶` [漂流瓶编号]
+    - `我的漂流瓶`
     - SUPERUSER指令：
         - `清空漂流瓶`
         - `恢复漂流瓶 [漂流瓶编号]`
         - `删除漂流瓶评论` [漂流瓶编号] [QQ号]
         - `漂流瓶白名单` [QQ / 群聊] [QQ号 / 群号]
         - `漂流瓶黑名单` [QQ / 群聊 / 举报] [QQ号 / 群号]
         - `漂流瓶详情` [漂流瓶编号]
```

### Comparing `nonebot_plugin_bottle-1.0.0.7/nonebot_plugin_bottle/__init__.py` & `nonebot_plugin_bottle-1.0.0.8/nonebot_plugin_bottle/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bottle-1.0.0.7/nonebot_plugin_bottle/config.py` & `nonebot_plugin_bottle-1.0.0.8/nonebot_plugin_bottle/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bottle-1.0.0.7/nonebot_plugin_bottle/data_source.py` & `nonebot_plugin_bottle-1.0.0.8/nonebot_plugin_bottle/data_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -317,17 +317,17 @@
             statement=select(Comment).where(
                 Comment.bottle_id == bottle.id, Comment.user_id == user_id
             )
         )
         for comment in comments:
             await session.delete(comment)
     
-    async def list_bottles(self, bottle: Bottle, user_id: int, session: AsyncSession) -> Sequence[Bottle]:
+    async def list_bottles(self, user_id: int, session: AsyncSession) -> Sequence[Bottle]:
         """获取用户扔出的所有漂流瓶
-
+    
         Args:
             user_id (int): 用户ID
             session (AsyncSession): 数据库会话
 
         Returns:
             Sequence[Bottle]: 用户扔出的所有漂流瓶
         """
```

### Comparing `nonebot_plugin_bottle-1.0.0.7/nonebot_plugin_bottle/migrations/449e066410fd_init_db.py` & `nonebot_plugin_bottle-1.0.0.8/nonebot_plugin_bottle/migrations/449e066410fd_init_db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bottle-1.0.0.7/nonebot_plugin_bottle/model.py` & `nonebot_plugin_bottle-1.0.0.8/nonebot_plugin_bottle/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bottle-1.0.0.7/pyproject.toml` & `nonebot_plugin_bottle-1.0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_bottle"
-version = "1.0.0.7"
+version = "1.0.0.8"
 description = "Bottle post plugin in Nonebot"
 authors = ["Todysheep <todysheep@163.com>"]
 license = "GNU GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Todysheep/nonebot_plugin_bottle"
 repository = "https://github.com/Todysheep/nonebot_plugin_bottle"
```

### Comparing `nonebot_plugin_bottle-1.0.0.7/PKG-INFO` & `nonebot_plugin_bottle-1.0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bottle
-Version: 1.0.0.7
+Version: 1.0.0.8
 Summary: Bottle post plugin in Nonebot
 Home-page: https://github.com/Todysheep/nonebot_plugin_bottle
 License: GNU GPLv3
 Author: Todysheep
 Author-email: todysheep@163.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
@@ -31,14 +31,15 @@
     - `扔漂流瓶` [文本/图片]
     - `寄漂流瓶` [文本/图片] （同`扔漂流瓶`，防止指令冲突用）
     - `捡漂流瓶` 
     - `评论漂流瓶` [漂流瓶编号] [文本]
     - `举报漂流瓶` [漂流瓶编号]
     - `查看漂流瓶` [漂流瓶编号]
     - `删除漂流瓶` [漂流瓶编号]
+    - `我的漂流瓶`
     - SUPERUSER指令：
         - `清空漂流瓶`
         - `恢复漂流瓶 [漂流瓶编号]`
         - `删除漂流瓶评论` [漂流瓶编号] [QQ号]
         - `漂流瓶白名单` [QQ / 群聊] [QQ号 / 群号]
         - `漂流瓶黑名单` [QQ / 群聊 / 举报] [QQ号 / 群号]
         - `漂流瓶详情` [漂流瓶编号]
```

