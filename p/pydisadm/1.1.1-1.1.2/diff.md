# Comparing `tmp/pydisadm-1.1.1.tar.gz` & `tmp/pydisadm-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydisadm-1.1.1.tar", max compression
+gzip compressed data, was "pydisadm-1.1.2.tar", max compression
```

## Comparing `pydisadm-1.1.1.tar` & `pydisadm-1.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     2853 2023-05-17 11:55:30.268500 pydisadm-1.1.1/README.md
--rw-r--r--   0        0        0      111 2023-05-17 11:55:30.268500 pydisadm-1.1.1/pydisadm/__init__.py
--rw-r--r--   0        0        0     1060 2023-05-17 11:55:30.268500 pydisadm-1.1.1/pydisadm/__main__.py
--rw-r--r--   0        0        0     1541 2023-05-17 11:55:30.268500 pydisadm-1.1.1/pydisadm/bot/adm_bot.py
--rw-r--r--   0        0        0     6691 2023-05-17 11:55:30.268500 pydisadm-1.1.1/pydisadm/bot/adm_cog.py
--rw-r--r--   0        0        0     2649 2023-05-17 11:55:30.268500 pydisadm-1.1.1/pydisadm/bot/update_adm_modal.py
--rw-r--r--   0        0        0      702 2023-05-17 11:55:30.268500 pydisadm-1.1.1/pydisadm/bot/utils.py
--rw-r--r--   0        0        0      816 2023-05-17 11:55:30.268500 pydisadm-1.1.1/pydisadm/configuration.py
--rw-r--r--   0        0        0     7883 2023-05-17 11:55:30.268500 pydisadm-1.1.1/pydisadm/controller/adm_controller.py
--rw-r--r--   0        0        0   368313 2023-05-17 11:55:30.268500 pydisadm-1.1.1/pydisadm/data/mapConstellations.csv
--rw-r--r--   0        0        0    34613 2023-05-17 11:55:30.272500 pydisadm-1.1.1/pydisadm/data/mapRegions.csv
--rw-r--r--   0        0        0  3277768 2023-05-17 11:55:30.288500 pydisadm-1.1.1/pydisadm/data/mapSolarSystems.csv
--rw-r--r--   0        0        0      607 2023-05-17 11:55:30.288500 pydisadm-1.1.1/pydisadm/loader/datasets.py
--rw-r--r--   0        0        0     1085 2023-05-17 11:55:30.288500 pydisadm-1.1.1/pydisadm/loader/static_data.py
--rw-r--r--   0        0        0     1108 2023-05-17 11:55:30.288500 pydisadm-1.1.1/pydisadm/runnable/runnable_refresh.py
--rw-r--r--   0        0        0     3442 2023-05-17 11:55:30.288500 pydisadm-1.1.1/pydisadm/services/database.py
--rw-r--r--   0        0        0     1543 2023-05-17 11:55:30.288500 pydisadm-1.1.1/pydisadm/services/esi.py
--rw-r--r--   0        0        0      484 2023-05-17 11:55:30.288500 pydisadm-1.1.1/pydisadm/utils/adm_utils.py
--rw-r--r--   0        0        0      472 2023-05-17 11:55:30.288500 pydisadm-1.1.1/pydisadm/utils/datetime_utils.py
--rw-r--r--   0        0        0      623 2023-05-17 11:55:30.288500 pydisadm-1.1.1/pydisadm/utils/plot_utils.py
--rw-r--r--   0        0        0      193 2023-05-17 11:55:30.288500 pydisadm-1.1.1/pydisadm/utils/thread_utils.py
--rw-r--r--   0        0        0      953 2023-05-17 11:55:59.292027 pydisadm-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     3709 1970-01-01 00:00:00.000000 pydisadm-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2847 2023-05-18 16:11:10.523574 pydisadm-1.1.2/README.md
+-rw-r--r--   0        0        0      111 2023-05-18 16:11:10.527574 pydisadm-1.1.2/pydisadm/__init__.py
+-rw-r--r--   0        0        0     1060 2023-05-18 16:11:10.527574 pydisadm-1.1.2/pydisadm/__main__.py
+-rw-r--r--   0        0        0     1541 2023-05-18 16:11:10.527574 pydisadm-1.1.2/pydisadm/bot/adm_bot.py
+-rw-r--r--   0        0        0     6691 2023-05-18 16:11:10.527574 pydisadm-1.1.2/pydisadm/bot/adm_cog.py
+-rw-r--r--   0        0        0     2649 2023-05-18 16:11:10.527574 pydisadm-1.1.2/pydisadm/bot/update_adm_modal.py
+-rw-r--r--   0        0        0      702 2023-05-18 16:11:10.527574 pydisadm-1.1.2/pydisadm/bot/utils.py
+-rw-r--r--   0        0        0      816 2023-05-18 16:11:10.527574 pydisadm-1.1.2/pydisadm/configuration.py
+-rw-r--r--   0        0        0     7883 2023-05-18 16:11:10.527574 pydisadm-1.1.2/pydisadm/controller/adm_controller.py
+-rw-r--r--   0        0        0   368313 2023-05-18 16:11:10.527574 pydisadm-1.1.2/pydisadm/data/mapConstellations.csv
+-rw-r--r--   0        0        0    34613 2023-05-18 16:11:10.527574 pydisadm-1.1.2/pydisadm/data/mapRegions.csv
+-rw-r--r--   0        0        0  3277768 2023-05-18 16:11:10.543574 pydisadm-1.1.2/pydisadm/data/mapSolarSystems.csv
+-rw-r--r--   0        0        0      607 2023-05-18 16:11:10.543574 pydisadm-1.1.2/pydisadm/loader/datasets.py
+-rw-r--r--   0        0        0     1085 2023-05-18 16:11:10.543574 pydisadm-1.1.2/pydisadm/loader/static_data.py
+-rw-r--r--   0        0        0     1108 2023-05-18 16:11:10.543574 pydisadm-1.1.2/pydisadm/runnable/runnable_refresh.py
+-rw-r--r--   0        0        0     3442 2023-05-18 16:11:10.547574 pydisadm-1.1.2/pydisadm/services/database.py
+-rw-r--r--   0        0        0     1543 2023-05-18 16:11:10.547574 pydisadm-1.1.2/pydisadm/services/esi.py
+-rw-r--r--   0        0        0      484 2023-05-18 16:11:10.547574 pydisadm-1.1.2/pydisadm/utils/adm_utils.py
+-rw-r--r--   0        0        0      472 2023-05-18 16:11:10.547574 pydisadm-1.1.2/pydisadm/utils/datetime_utils.py
+-rw-r--r--   0        0        0      623 2023-05-18 16:11:10.547574 pydisadm-1.1.2/pydisadm/utils/plot_utils.py
+-rw-r--r--   0        0        0      193 2023-05-18 16:11:10.547574 pydisadm-1.1.2/pydisadm/utils/thread_utils.py
+-rw-r--r--   0        0        0      953 2023-05-18 16:11:49.811854 pydisadm-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3703 1970-01-01 00:00:00.000000 pydisadm-1.1.2/PKG-INFO
```

### Comparing `pydisadm-1.1.1/README.md` & `pydisadm-1.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 ## 📃 Commands
 
 - `/adm summary` - send a summary of ADM's
 - `/adm csv` - send a csv of ADM's
 - `/adm history <name>` - send a graph showing system, constellation, or region ADM over time
 - `/adm refresh` - manually refresh the data
-- `/adm update <system> <adm>` - manually update ADM for system
+- `/adm update <system>` - manually update ADM for system
 - `/adm recommend` - recommend a system to raise ADM in
 
 ## 🔧 Configuration
 Configuration is done using environment variables or `dotenv`. See `.env.example` for example configuration.
 
 - `DISCORD_TOKEN` - the token bot should use when communicating with discord.
 - `DISCORD_CHANNEL` - the channel name bot should listen too, if this is empty the bot will listen to all channels.
```

### Comparing `pydisadm-1.1.1/pydisadm/__main__.py` & `pydisadm-1.1.2/pydisadm/__main__.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.1.1/pydisadm/bot/adm_bot.py` & `pydisadm-1.1.2/pydisadm/bot/adm_bot.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.1.1/pydisadm/bot/adm_cog.py` & `pydisadm-1.1.2/pydisadm/bot/adm_cog.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.1.1/pydisadm/bot/update_adm_modal.py` & `pydisadm-1.1.2/pydisadm/bot/update_adm_modal.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.1.1/pydisadm/bot/utils.py` & `pydisadm-1.1.2/pydisadm/bot/utils.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.1.1/pydisadm/configuration.py` & `pydisadm-1.1.2/pydisadm/configuration.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.1.1/pydisadm/controller/adm_controller.py` & `pydisadm-1.1.2/pydisadm/controller/adm_controller.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.1.1/pydisadm/data/mapConstellations.csv` & `pydisadm-1.1.2/pydisadm/data/mapConstellations.csv`

 * *Files identical despite different names*

### Comparing `pydisadm-1.1.1/pydisadm/data/mapRegions.csv` & `pydisadm-1.1.2/pydisadm/data/mapRegions.csv`

 * *Files identical despite different names*

### Comparing `pydisadm-1.1.1/pydisadm/data/mapSolarSystems.csv` & `pydisadm-1.1.2/pydisadm/data/mapSolarSystems.csv`

 * *Files identical despite different names*

### Comparing `pydisadm-1.1.1/pydisadm/loader/datasets.py` & `pydisadm-1.1.2/pydisadm/loader/datasets.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.1.1/pydisadm/loader/static_data.py` & `pydisadm-1.1.2/pydisadm/loader/static_data.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.1.1/pydisadm/runnable/runnable_refresh.py` & `pydisadm-1.1.2/pydisadm/runnable/runnable_refresh.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.1.1/pydisadm/services/database.py` & `pydisadm-1.1.2/pydisadm/services/database.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.1.1/pydisadm/services/esi.py` & `pydisadm-1.1.2/pydisadm/services/esi.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.1.1/pydisadm/utils/plot_utils.py` & `pydisadm-1.1.2/pydisadm/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.1.1/pyproject.toml` & `pydisadm-1.1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydisadm"
-version = "1.1.1"
+version = "1.1.2"
 description = "A Discord bot providing ADM summaries."
 repository = "https://github.com/agelito/adm-bot"
 authors = ["Axel Wettervik"]
 license = "MIT"
 readme = "README.md"
 include = ["data/*.csv"]
```

### Comparing `pydisadm-1.1.1/PKG-INFO` & `pydisadm-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydisadm
-Version: 1.1.1
+Version: 1.1.2
 Summary: A Discord bot providing ADM summaries.
 Home-page: https://github.com/agelito/adm-bot
 License: MIT
 Author: Axel Wettervik
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -65,15 +65,15 @@
 
 ## 📃 Commands
 
 - `/adm summary` - send a summary of ADM's
 - `/adm csv` - send a csv of ADM's
 - `/adm history <name>` - send a graph showing system, constellation, or region ADM over time
 - `/adm refresh` - manually refresh the data
-- `/adm update <system> <adm>` - manually update ADM for system
+- `/adm update <system>` - manually update ADM for system
 - `/adm recommend` - recommend a system to raise ADM in
 
 ## 🔧 Configuration
 Configuration is done using environment variables or `dotenv`. See `.env.example` for example configuration.
 
 - `DISCORD_TOKEN` - the token bot should use when communicating with discord.
 - `DISCORD_CHANNEL` - the channel name bot should listen too, if this is empty the bot will listen to all channels.
```

