# Comparing `tmp/les_louisdelatech-0.3.0.tar.gz` & `tmp/les_louisdelatech-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "les_louisdelatech-0.3.0.tar", max compression
+gzip compressed data, was "les_louisdelatech-0.3.1.tar", max compression
```

## Comparing `les_louisdelatech-0.3.0.tar` & `les_louisdelatech-0.3.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    22294 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/LICENSE
--rw-r--r--   0        0        0    23504 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/LICENSE.fr
--rw-r--r--   0        0        0     2307 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/__init__.py
--rw-r--r--   0        0        0     3330 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/bot.py
--rw-r--r--   0        0        0      824 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/extensions/cats.py
--rw-r--r--   0        0        0      492 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/extensions/config.py
--rw-r--r--   0        0        0     2902 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/extensions/management.py
--rw-r--r--   0        0        0     4632 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/extensions/otp.py
--rw-r--r--   0        0        0      683 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/extensions/task.py
--rw-r--r--   0        0        0    15315 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/extensions/user.py
--rw-r--r--   0        0        0     1366 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/main.py
--rw-r--r--   0        0        0       45 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/models/__init__.py
--rw-r--r--   0        0        0      481 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/models/otp.py
--rw-r--r--   0        0        0     1094 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/templates/discord/base.j2
--rw-r--r--   0        0        0        0 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/templates/discord/ca.j2
--rw-r--r--   0        0        0        0 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/templates/discord/logistique.j2
--rw-r--r--   0        0        0        0 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/templates/discord/marketing.j2
--rw-r--r--   0        0        0      459 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/templates/discord/reset_password.j2
--rw-r--r--   0        0        0        0 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/templates/discord/scene.j2
--rw-r--r--   0        0        0        0 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/templates/discord/technique.j2
--rw-r--r--   0        0        0        0 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/templates/discord/tournoi.j2
--rw-r--r--   0        0        0     2705 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/templates/google/gmail_signature.j2
--rw-r--r--   0        0        0       48 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/utils/LouisDeLaTechError.py
--rw-r--r--   0        0        0     2958 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/utils/User.py
--rw-r--r--   0        0        0      753 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/utils/discord.py
--rw-r--r--   0        0        0     6169 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/utils/gsuite.py
--rw-r--r--   0        0        0      380 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/utils/password.py
--rw-r--r--   0        0        0     1474 2023-05-08 22:04:47.821780 les_louisdelatech-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3861 1970-01-01 00:00:00.000000 les_louisdelatech-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    22294 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/LICENSE
+-rw-r--r--   0        0        0    23504 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/LICENSE.fr
+-rw-r--r--   0        0        0     2307 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/les_louisdelatech/__init__.py
+-rw-r--r--   0        0        0     3330 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/les_louisdelatech/bot.py
+-rw-r--r--   0        0        0      824 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/les_louisdelatech/extensions/cats.py
+-rw-r--r--   0        0        0      492 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/les_louisdelatech/extensions/config.py
+-rw-r--r--   0        0        0     2913 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/les_louisdelatech/extensions/management.py
+-rw-r--r--   0        0        0     4632 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/les_louisdelatech/extensions/otp.py
+-rw-r--r--   0        0        0      683 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/les_louisdelatech/extensions/task.py
+-rw-r--r--   0        0        0    15315 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/les_louisdelatech/extensions/user.py
+-rw-r--r--   0        0        0     1366 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/les_louisdelatech/main.py
+-rw-r--r--   0        0        0       45 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/les_louisdelatech/models/__init__.py
+-rw-r--r--   0        0        0      481 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/les_louisdelatech/models/otp.py
+-rw-r--r--   0        0        0     1094 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/les_louisdelatech/templates/discord/base.j2
+-rw-r--r--   0        0        0        0 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/les_louisdelatech/templates/discord/ca.j2
+-rw-r--r--   0        0        0        0 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/les_louisdelatech/templates/discord/logistique.j2
+-rw-r--r--   0        0        0        0 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/les_louisdelatech/templates/discord/marketing.j2
+-rw-r--r--   0        0        0      459 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/les_louisdelatech/templates/discord/reset_password.j2
+-rw-r--r--   0        0        0        0 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/les_louisdelatech/templates/discord/scene.j2
+-rw-r--r--   0        0        0        0 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/les_louisdelatech/templates/discord/technique.j2
+-rw-r--r--   0        0        0        0 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/les_louisdelatech/templates/discord/tournoi.j2
+-rw-r--r--   0        0        0     2705 2023-05-18 18:55:38.708489 les_louisdelatech-0.3.1/les_louisdelatech/templates/google/gmail_signature.j2
+-rw-r--r--   0        0        0       48 2023-05-18 18:55:38.708489 les_louisdelatech-0.3.1/les_louisdelatech/utils/LouisDeLaTechError.py
+-rw-r--r--   0        0        0     2958 2023-05-18 18:55:38.708489 les_louisdelatech-0.3.1/les_louisdelatech/utils/User.py
+-rw-r--r--   0        0        0      753 2023-05-18 18:55:38.708489 les_louisdelatech-0.3.1/les_louisdelatech/utils/discord.py
+-rw-r--r--   0        0        0     6169 2023-05-18 18:55:38.708489 les_louisdelatech-0.3.1/les_louisdelatech/utils/gsuite.py
+-rw-r--r--   0        0        0      380 2023-05-18 18:55:38.708489 les_louisdelatech-0.3.1/les_louisdelatech/utils/password.py
+-rw-r--r--   0        0        0     1474 2023-05-18 18:56:14.196703 les_louisdelatech-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3861 1970-01-01 00:00:00.000000 les_louisdelatech-0.3.1/PKG-INFO
```

### Comparing `les_louisdelatech-0.3.0/LICENSE` & `les_louisdelatech-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `les_louisdelatech-0.3.0/LICENSE.fr` & `les_louisdelatech-0.3.1/LICENSE.fr`

 * *Files identical despite different names*

### Comparing `les_louisdelatech-0.3.0/README.md` & `les_louisdelatech-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `les_louisdelatech-0.3.0/les_louisdelatech/bot.py` & `les_louisdelatech-0.3.1/les_louisdelatech/bot.py`

 * *Files identical despite different names*

### Comparing `les_louisdelatech-0.3.0/les_louisdelatech/extensions/cats.py` & `les_louisdelatech-0.3.1/les_louisdelatech/extensions/cats.py`

 * *Files identical despite different names*

### Comparing `les_louisdelatech-0.3.0/les_louisdelatech/extensions/management.py` & `les_louisdelatech-0.3.1/les_louisdelatech/extensions/management.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,15 +55,15 @@
                     new_channel_name = channel_name_check
                 channel_number = channel_number + 1
 
             # Create the channel and move member
             new_channel = await member.guild.create_voice_channel(
                 new_channel_name,
                 category=after.channel.category,
-                bitrate=self.bot.config["voice_channel_creation"]["bitrate"],
+                bitrate=self.bot.config["discord"]["voice_channel_creation"]["bitrate"],
             )
             await member.move_to(new_channel)
 
         # Delete voice channel block
         if (
             before.channel
             and before.channel.name.startswith(
```

### Comparing `les_louisdelatech-0.3.0/les_louisdelatech/extensions/otp.py` & `les_louisdelatech-0.3.1/les_louisdelatech/extensions/otp.py`

 * *Files identical despite different names*

### Comparing `les_louisdelatech-0.3.0/les_louisdelatech/extensions/task.py` & `les_louisdelatech-0.3.1/les_louisdelatech/extensions/task.py`

 * *Files identical despite different names*

### Comparing `les_louisdelatech-0.3.0/les_louisdelatech/extensions/user.py` & `les_louisdelatech-0.3.1/les_louisdelatech/extensions/user.py`

 * *Files identical despite different names*

### Comparing `les_louisdelatech-0.3.0/les_louisdelatech/main.py` & `les_louisdelatech-0.3.1/les_louisdelatech/main.py`

 * *Files identical despite different names*

### Comparing `les_louisdelatech-0.3.0/les_louisdelatech/templates/discord/base.j2` & `les_louisdelatech-0.3.1/les_louisdelatech/templates/discord/base.j2`

 * *Files identical despite different names*

### Comparing `les_louisdelatech-0.3.0/les_louisdelatech/templates/google/gmail_signature.j2` & `les_louisdelatech-0.3.1/les_louisdelatech/templates/google/gmail_signature.j2`

 * *Files identical despite different names*

### Comparing `les_louisdelatech-0.3.0/les_louisdelatech/utils/User.py` & `les_louisdelatech-0.3.1/les_louisdelatech/utils/User.py`

 * *Files identical despite different names*

### Comparing `les_louisdelatech-0.3.0/les_louisdelatech/utils/discord.py` & `les_louisdelatech-0.3.1/les_louisdelatech/utils/discord.py`

 * *Files identical despite different names*

### Comparing `les_louisdelatech-0.3.0/les_louisdelatech/utils/gsuite.py` & `les_louisdelatech-0.3.1/les_louisdelatech/utils/gsuite.py`

 * *Files identical despite different names*

### Comparing `les_louisdelatech-0.3.0/pyproject.toml` & `les_louisdelatech-0.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "les-louisdelatech"
-version = "0.3.0"
+version = "0.3.1"
 description = "LouisDeLaTech is a discord bot manager for Lyon e-Sport"
 authors = [
     "Ludovic Ortega <ludovic.ortega@lyon-esport.fr>",
     "Etienne 'PoPs' G. <etienne.guilluy@lyon-esport.fr>",
     "Pierre 'DrumSlayer' Sarret <pierre.sarret@lyon-esport.fr>",
 
 ]
@@ -39,12 +39,12 @@
 aiosqlite = "^0.17.0"
 cryptography = ">=37.0.4,<41.0.0"
 sentry-sdk = "^1.6.0"
 httpx = ">=0.23,<0.25"
 tomli = "^2.0.1"
 
 [tool.poetry.dev-dependencies]
-pre-commit = "^3.3.1"
+pre-commit = "^3.3.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `les_louisdelatech-0.3.0/PKG-INFO` & `les_louisdelatech-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: les-louisdelatech
-Version: 0.3.0
+Version: 0.3.1
 Summary: LouisDeLaTech is a discord bot manager for Lyon e-Sport
 Home-page: https://github.com/lyon-esport/LouisDeLaTech
 License: CeCILL
 Keywords: google,discord
 Author: Ludovic Ortega
 Author-email: ludovic.ortega@lyon-esport.fr
 Requires-Python: >=3.8,<4.0
```

