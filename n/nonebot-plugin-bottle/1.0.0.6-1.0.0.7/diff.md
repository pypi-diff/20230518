# Comparing `tmp/nonebot_plugin_bottle-1.0.0.6.tar.gz` & `tmp/nonebot_plugin_bottle-1.0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bottle-1.0.0.6.tar", max compression
+gzip compressed data, was "nonebot_plugin_bottle-1.0.0.7.tar", max compression
```

## Comparing `nonebot_plugin_bottle-1.0.0.6.tar` & `nonebot_plugin_bottle-1.0.0.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     7592 2023-05-18 04:10:26.263686 nonebot_plugin_bottle-1.0.0.6/README.md
--rw-r--r--   0        0        0    17187 2023-05-18 04:10:26.267686 nonebot_plugin_bottle-1.0.0.6/nonebot_plugin_bottle/__init__.py
--rw-r--r--   0        0        0      636 2023-05-18 04:10:26.267686 nonebot_plugin_bottle-1.0.0.6/nonebot_plugin_bottle/config.py
--rw-r--r--   0        0        0    17798 2023-05-18 04:10:26.267686 nonebot_plugin_bottle-1.0.0.6/nonebot_plugin_bottle/data_source.py
--rw-r--r--   0        0        0     2647 2023-05-18 04:10:26.267686 nonebot_plugin_bottle-1.0.0.6/nonebot_plugin_bottle/migrations/449e066410fd_init_db.py
--rw-r--r--   0        0        0     1426 2023-05-18 04:10:26.267686 nonebot_plugin_bottle-1.0.0.6/nonebot_plugin_bottle/model.py
--rw-r--r--   0        0        0      625 2023-05-18 04:10:26.267686 nonebot_plugin_bottle-1.0.0.6/pyproject.toml
--rw-r--r--   0        0        0     8356 1970-01-01 00:00:00.000000 nonebot_plugin_bottle-1.0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     7592 2023-05-18 11:23:18.055650 nonebot_plugin_bottle-1.0.0.7/README.md
+-rw-r--r--   0        0        0    19581 2023-05-18 11:23:18.055650 nonebot_plugin_bottle-1.0.0.7/nonebot_plugin_bottle/__init__.py
+-rw-r--r--   0        0        0      636 2023-05-18 11:23:18.055650 nonebot_plugin_bottle-1.0.0.7/nonebot_plugin_bottle/config.py
+-rw-r--r--   0        0        0    18367 2023-05-18 11:23:18.055650 nonebot_plugin_bottle-1.0.0.7/nonebot_plugin_bottle/data_source.py
+-rw-r--r--   0        0        0     2647 2023-05-18 11:23:18.055650 nonebot_plugin_bottle-1.0.0.7/nonebot_plugin_bottle/migrations/449e066410fd_init_db.py
+-rw-r--r--   0        0        0     1426 2023-05-18 11:23:18.055650 nonebot_plugin_bottle-1.0.0.7/nonebot_plugin_bottle/model.py
+-rw-r--r--   0        0        0      625 2023-05-18 11:23:18.055650 nonebot_plugin_bottle-1.0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     8356 1970-01-01 00:00:00.000000 nonebot_plugin_bottle-1.0.0.7/PKG-INFO
```

### Comparing `nonebot_plugin_bottle-1.0.0.6/README.md` & `nonebot_plugin_bottle-1.0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bottle-1.0.0.6/nonebot_plugin_bottle/__init__.py` & `nonebot_plugin_bottle-1.0.0.7/nonebot_plugin_bottle/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     扔漂流瓶 [文本/图片]
     寄漂流瓶 [文本/图片] （同扔漂流瓶，防止指令冲突用）
     捡漂流瓶
     评论漂流瓶 [漂流瓶编号] [文本]
     举报漂流瓶 [漂流瓶编号]
     查看漂流瓶 [漂流瓶编号]
     删除漂流瓶 [漂流瓶编号]
+    我的漂流瓶
 SUPERUSER指令：
     清空漂流瓶
     恢复漂流瓶 [漂流瓶编号]
     删除漂流瓶评论 [漂流瓶编号] [QQ号]
     漂流瓶白名单 [QQ / 群聊 / 举报] [QQ号 / 群号]
     漂流瓶黑名单 [QQ / 群聊] [QQ号 / 群号]
     漂流瓶详情 [漂流瓶编号]
@@ -63,14 +64,15 @@
     "扔漂流瓶", aliases=set(["寄漂流瓶", "丢漂流瓶"]), permission=GROUP, priority=100, block=True
 )
 get = on_command("捡漂流瓶", priority=100, block=True)
 report = on_command("举报漂流瓶", priority=100, block=True)
 comment = on_command("评论漂流瓶", priority=100, block=True)
 check_bottle = on_command("查看漂流瓶", priority=100, block=True)
 remove = on_command("删除漂流瓶", priority=100, block=True)
+listb = on_command("我的漂流瓶", priority=100, block=True)
 
 resume = on_command("恢复漂流瓶", permission=SUPERUSER, priority=100, block=True)
 clear = on_command("清空漂流瓶", permission=SUPERUSER, priority=100, block=True)
 comrem = on_command("删除漂流瓶评论", permission=SUPERUSER, priority=100, block=True)
 listqq = on_command("漂流瓶详情", permission=SUPERUSER, priority=100, block=True)
 ban = on_command(
     "漂流瓶黑名单",
@@ -102,14 +104,78 @@
 
 
 async def verify(matcher: Matcher, event: GroupMessageEvent) -> None:
     if not ba.verify(event.user_id, event.group_id):
         await matcher.finish(ba.bannedMessage)
 
 
+@listb.handle()
+async def _(
+    bot: Bot,
+    event: GroupMessageEvent,
+    session: AsyncSession = Depends(get_session),
+):
+    bottles = await bottle_manager.list_bottles(user_id=event.user_id, session=session)
+    if not bottles:
+        await listb.finish("你还没有扔过漂流瓶哦～")
+
+    bottles_info = []
+    for bottle in bottles:
+        message_parts = deserialize_message(bottle.content)
+        content_preview = ""
+        for part in message_parts:
+            if part.type == "text":
+                # 文字截取
+                text = part.data["text"]
+                content_preview += text[:20] + "..." if len(text) > 20 else text
+            elif part.type == "image":
+                # 图片处理
+                content_preview += "[图片]"
+        bottles_info.append(f"#{bottle.id}：{content_preview}")
+
+    messages = []
+    total_bottles_info = f"您总共扔了{len(bottles_info)}个漂流瓶～\n"
+    if len(bottles_info) > 10:
+        i = 1
+        while len(bottles_info) > 10:
+            messages.append(
+                total_bottles_info + "\n".join(bottles_info[:10]) + f"\n【第{i}页】"
+            )
+            bottles_info = bottles_info[10:]
+            i = i + 1
+        messages.append(
+            total_bottles_info + "\n".join(bottles_info[:10]) + f"\n【第{i}页-完】"
+        )
+
+        # 发送合并转发消息
+        if isinstance(event, GroupMessageEvent):
+            await bot.send_group_forward_msg(
+                group_id=event.group_id,
+                messages=[
+                    MessageSegment.node_custom(
+                        user_id=event.self_id, nickname="bottle", content=msg
+                    )
+                    for msg in messages
+                ],
+            )
+        else:
+            await bot.send_private_forward_msg(
+                user_id=event.user_id,
+                messages=[
+                    MessageSegment.node_custom(
+                        user_id=event.self_id, nickname="bottle", content=msg
+                    )
+                    for msg in messages
+                ],
+            )
+    else:
+        await listb.finish(total_bottles_info + "\n".join(bottles_info[:10]))
+    ba.add("cooldown", event.user_id)
+
+
 @throw.handle()
 async def _(
     bot: Bot,
     matcher: Matcher,
     event: GroupMessageEvent,
     args: Message = CommandArg(),
     session: AsyncSession = Depends(get_session),
```

### Comparing `nonebot_plugin_bottle-1.0.0.6/nonebot_plugin_bottle/config.py` & `nonebot_plugin_bottle-1.0.0.7/nonebot_plugin_bottle/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bottle-1.0.0.6/nonebot_plugin_bottle/data_source.py` & `nonebot_plugin_bottle-1.0.0.7/nonebot_plugin_bottle/data_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -316,15 +316,32 @@
         comments = await session.scalars(
             statement=select(Comment).where(
                 Comment.bottle_id == bottle.id, Comment.user_id == user_id
             )
         )
         for comment in comments:
             await session.delete(comment)
+    
+    async def list_bottles(self, bottle: Bottle, user_id: int, session: AsyncSession) -> Sequence[Bottle]:
+        """获取用户扔出的所有漂流瓶
 
+        Args:
+            user_id (int): 用户ID
+            session (AsyncSession): 数据库会话
+
+        Returns:
+            Sequence[Bottle]: 用户扔出的所有漂流瓶
+        """
+        return(
+            await session.scalars(
+                select(Bottle)
+                .where(Bottle.user_id == user_id)
+                .order_by(Bottle.id)
+            )
+        ).all()
 
 bottle_manager = BottleManager()
 
 
 class Audit(object):
     bannedMessage = ""
```

### Comparing `nonebot_plugin_bottle-1.0.0.6/nonebot_plugin_bottle/migrations/449e066410fd_init_db.py` & `nonebot_plugin_bottle-1.0.0.7/nonebot_plugin_bottle/migrations/449e066410fd_init_db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bottle-1.0.0.6/nonebot_plugin_bottle/model.py` & `nonebot_plugin_bottle-1.0.0.7/nonebot_plugin_bottle/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bottle-1.0.0.6/pyproject.toml` & `nonebot_plugin_bottle-1.0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_bottle"
-version = "1.0.0.6"
+version = "1.0.0.7"
 description = "Bottle post plugin in Nonebot"
 authors = ["Todysheep <todysheep@163.com>"]
 license = "GNU GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Todysheep/nonebot_plugin_bottle"
 repository = "https://github.com/Todysheep/nonebot_plugin_bottle"
```

### Comparing `nonebot_plugin_bottle-1.0.0.6/PKG-INFO` & `nonebot_plugin_bottle-1.0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bottle
-Version: 1.0.0.6
+Version: 1.0.0.7
 Summary: Bottle post plugin in Nonebot
 Home-page: https://github.com/Todysheep/nonebot_plugin_bottle
 License: GNU GPLv3
 Author: Todysheep
 Author-email: todysheep@163.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

