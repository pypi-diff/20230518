# Comparing `tmp/nonebot_plugin_bottle-1.0.0.4.tar.gz` & `tmp/nonebot_plugin_bottle-1.0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bottle-1.0.0.4.tar", max compression
+gzip compressed data, was "nonebot_plugin_bottle-1.0.0.5.tar", max compression
```

## Comparing `nonebot_plugin_bottle-1.0.0.4.tar` & `nonebot_plugin_bottle-1.0.0.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     7592 2023-05-01 04:27:26.560496 nonebot_plugin_bottle-1.0.0.4/README.md
--rw-r--r--   0        0        0    17112 2023-05-01 04:27:26.560496 nonebot_plugin_bottle-1.0.0.4/nonebot_plugin_bottle/__init__.py
--rw-r--r--   0        0        0      636 2023-05-01 04:27:26.560496 nonebot_plugin_bottle-1.0.0.4/nonebot_plugin_bottle/config.py
--rw-r--r--   0        0        0    17798 2023-05-01 04:27:26.560496 nonebot_plugin_bottle-1.0.0.4/nonebot_plugin_bottle/data_source.py
--rw-r--r--   0        0        0     2647 2023-05-01 04:27:26.560496 nonebot_plugin_bottle-1.0.0.4/nonebot_plugin_bottle/migrations/449e066410fd_init_db.py
--rw-r--r--   0        0        0     1426 2023-05-01 04:27:26.560496 nonebot_plugin_bottle-1.0.0.4/nonebot_plugin_bottle/model.py
--rw-r--r--   0        0        0      625 2023-05-01 04:27:26.560496 nonebot_plugin_bottle-1.0.0.4/pyproject.toml
--rw-r--r--   0        0        0     8356 1970-01-01 00:00:00.000000 nonebot_plugin_bottle-1.0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     7592 2023-05-18 02:06:42.540047 nonebot_plugin_bottle-1.0.0.5/README.md
+-rw-r--r--   0        0        0    17116 2023-05-18 02:06:42.540047 nonebot_plugin_bottle-1.0.0.5/nonebot_plugin_bottle/__init__.py
+-rw-r--r--   0        0        0      636 2023-05-18 02:06:42.540047 nonebot_plugin_bottle-1.0.0.5/nonebot_plugin_bottle/config.py
+-rw-r--r--   0        0        0    17798 2023-05-18 02:06:42.540047 nonebot_plugin_bottle-1.0.0.5/nonebot_plugin_bottle/data_source.py
+-rw-r--r--   0        0        0     2647 2023-05-18 02:06:42.540047 nonebot_plugin_bottle-1.0.0.5/nonebot_plugin_bottle/migrations/449e066410fd_init_db.py
+-rw-r--r--   0        0        0     1426 2023-05-18 02:06:42.540047 nonebot_plugin_bottle-1.0.0.5/nonebot_plugin_bottle/model.py
+-rw-r--r--   0        0        0      625 2023-05-18 02:06:42.540047 nonebot_plugin_bottle-1.0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     8356 1970-01-01 00:00:00.000000 nonebot_plugin_bottle-1.0.0.5/PKG-INFO
```

### Comparing `nonebot_plugin_bottle-1.0.0.4/README.md` & `nonebot_plugin_bottle-1.0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bottle-1.0.0.4/nonebot_plugin_bottle/__init__.py` & `nonebot_plugin_bottle-1.0.0.5/nonebot_plugin_bottle/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
     await verify(matcher=matcher, event=event)
 
     bottle = await bottle_manager.select(session=session)
     if not bottle:
         await get.finish("好像一个瓶子也没有呢..要不要扔一个？")
     try:
         user_info = await bot.get_group_member_info(
-            group_id=event.group_id, user_id=event.user_id
+            group_id=bottle.group_id, user_id=bottle.user_id
         )
         user_name = user_info.get("card") or user_info.get("nickname")
     except ActionFailed:
         user_name = bottle.user_name
     try:
         group_info = await bot.get_group_info(group_id=bottle.group_id)
         group_name = group_info["group_name"]
@@ -306,15 +306,15 @@
     session: AsyncSession = Depends(get_session),
 ):
     index = args.extract_plain_text().strip()
     bottle = await get_bottle(index=index, matcher=matcher, session=session)
 
     try:
         user_info = await bot.get_group_member_info(
-            group_id=event.group_id, user_id=event.user_id
+            group_id=bottle.group_id, user_id=bottle.user_id
         )
         user_name = user_info.get("card") or user_info.get("nickname")
     except ActionFailed:
         user_name = bottle.user_name
     try:
         group_info = await bot.get_group_info(group_id=bottle.group_id)
         group_name = group_info["group_name"]
```

### Comparing `nonebot_plugin_bottle-1.0.0.4/nonebot_plugin_bottle/config.py` & `nonebot_plugin_bottle-1.0.0.5/nonebot_plugin_bottle/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bottle-1.0.0.4/nonebot_plugin_bottle/data_source.py` & `nonebot_plugin_bottle-1.0.0.5/nonebot_plugin_bottle/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bottle-1.0.0.4/nonebot_plugin_bottle/migrations/449e066410fd_init_db.py` & `nonebot_plugin_bottle-1.0.0.5/nonebot_plugin_bottle/migrations/449e066410fd_init_db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bottle-1.0.0.4/nonebot_plugin_bottle/model.py` & `nonebot_plugin_bottle-1.0.0.5/nonebot_plugin_bottle/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bottle-1.0.0.4/pyproject.toml` & `nonebot_plugin_bottle-1.0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_bottle"
-version = "1.0.0.4"
+version = "1.0.0.5"
 description = "Bottle post plugin in Nonebot"
 authors = ["Todysheep <todysheep@163.com>"]
 license = "GNU GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Todysheep/nonebot_plugin_bottle"
 repository = "https://github.com/Todysheep/nonebot_plugin_bottle"
```

### Comparing `nonebot_plugin_bottle-1.0.0.4/PKG-INFO` & `nonebot_plugin_bottle-1.0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bottle
-Version: 1.0.0.4
+Version: 1.0.0.5
 Summary: Bottle post plugin in Nonebot
 Home-page: https://github.com/Todysheep/nonebot_plugin_bottle
 License: GNU GPLv3
 Author: Todysheep
 Author-email: todysheep@163.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

