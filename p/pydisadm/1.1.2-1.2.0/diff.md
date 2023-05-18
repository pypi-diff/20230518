# Comparing `tmp/pydisadm-1.1.2.tar.gz` & `tmp/pydisadm-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydisadm-1.1.2.tar", max compression
+gzip compressed data, was "pydisadm-1.2.0.tar", max compression
```

## Comparing `pydisadm-1.1.2.tar` & `pydisadm-1.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     2847 2023-05-18 16:11:10.523574 pydisadm-1.1.2/README.md
--rw-r--r--   0        0        0      111 2023-05-18 16:11:10.527574 pydisadm-1.1.2/pydisadm/__init__.py
--rw-r--r--   0        0        0     1060 2023-05-18 16:11:10.527574 pydisadm-1.1.2/pydisadm/__main__.py
--rw-r--r--   0        0        0     1541 2023-05-18 16:11:10.527574 pydisadm-1.1.2/pydisadm/bot/adm_bot.py
--rw-r--r--   0        0        0     6691 2023-05-18 16:11:10.527574 pydisadm-1.1.2/pydisadm/bot/adm_cog.py
--rw-r--r--   0        0        0     2649 2023-05-18 16:11:10.527574 pydisadm-1.1.2/pydisadm/bot/update_adm_modal.py
--rw-r--r--   0        0        0      702 2023-05-18 16:11:10.527574 pydisadm-1.1.2/pydisadm/bot/utils.py
--rw-r--r--   0        0        0      816 2023-05-18 16:11:10.527574 pydisadm-1.1.2/pydisadm/configuration.py
--rw-r--r--   0        0        0     7883 2023-05-18 16:11:10.527574 pydisadm-1.1.2/pydisadm/controller/adm_controller.py
--rw-r--r--   0        0        0   368313 2023-05-18 16:11:10.527574 pydisadm-1.1.2/pydisadm/data/mapConstellations.csv
--rw-r--r--   0        0        0    34613 2023-05-18 16:11:10.527574 pydisadm-1.1.2/pydisadm/data/mapRegions.csv
--rw-r--r--   0        0        0  3277768 2023-05-18 16:11:10.543574 pydisadm-1.1.2/pydisadm/data/mapSolarSystems.csv
--rw-r--r--   0        0        0      607 2023-05-18 16:11:10.543574 pydisadm-1.1.2/pydisadm/loader/datasets.py
--rw-r--r--   0        0        0     1085 2023-05-18 16:11:10.543574 pydisadm-1.1.2/pydisadm/loader/static_data.py
--rw-r--r--   0        0        0     1108 2023-05-18 16:11:10.543574 pydisadm-1.1.2/pydisadm/runnable/runnable_refresh.py
--rw-r--r--   0        0        0     3442 2023-05-18 16:11:10.547574 pydisadm-1.1.2/pydisadm/services/database.py
--rw-r--r--   0        0        0     1543 2023-05-18 16:11:10.547574 pydisadm-1.1.2/pydisadm/services/esi.py
--rw-r--r--   0        0        0      484 2023-05-18 16:11:10.547574 pydisadm-1.1.2/pydisadm/utils/adm_utils.py
--rw-r--r--   0        0        0      472 2023-05-18 16:11:10.547574 pydisadm-1.1.2/pydisadm/utils/datetime_utils.py
--rw-r--r--   0        0        0      623 2023-05-18 16:11:10.547574 pydisadm-1.1.2/pydisadm/utils/plot_utils.py
--rw-r--r--   0        0        0      193 2023-05-18 16:11:10.547574 pydisadm-1.1.2/pydisadm/utils/thread_utils.py
--rw-r--r--   0        0        0      953 2023-05-18 16:11:49.811854 pydisadm-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     3703 1970-01-01 00:00:00.000000 pydisadm-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2936 2023-05-18 16:16:15.595143 pydisadm-1.2.0/README.md
+-rw-r--r--   0        0        0      111 2023-05-18 16:16:15.599143 pydisadm-1.2.0/pydisadm/__init__.py
+-rw-r--r--   0        0        0     1130 2023-05-18 16:16:15.599143 pydisadm-1.2.0/pydisadm/__main__.py
+-rw-r--r--   0        0        0     1541 2023-05-18 16:16:15.599143 pydisadm-1.2.0/pydisadm/bot/adm_bot.py
+-rw-r--r--   0        0        0     6691 2023-05-18 16:16:15.599143 pydisadm-1.2.0/pydisadm/bot/adm_cog.py
+-rw-r--r--   0        0        0     2649 2023-05-18 16:16:15.599143 pydisadm-1.2.0/pydisadm/bot/update_adm_modal.py
+-rw-r--r--   0        0        0      702 2023-05-18 16:16:15.599143 pydisadm-1.2.0/pydisadm/bot/utils.py
+-rw-r--r--   0        0        0     1413 2023-05-18 16:16:15.599143 pydisadm-1.2.0/pydisadm/configuration.py
+-rw-r--r--   0        0        0     8044 2023-05-18 16:16:15.599143 pydisadm-1.2.0/pydisadm/controller/adm_controller.py
+-rw-r--r--   0        0        0   368313 2023-05-18 16:16:15.599143 pydisadm-1.2.0/pydisadm/data/mapConstellations.csv
+-rw-r--r--   0        0        0    34613 2023-05-18 16:16:15.599143 pydisadm-1.2.0/pydisadm/data/mapRegions.csv
+-rw-r--r--   0        0        0  3277768 2023-05-18 16:16:15.619143 pydisadm-1.2.0/pydisadm/data/mapSolarSystems.csv
+-rw-r--r--   0        0        0      607 2023-05-18 16:16:15.619143 pydisadm-1.2.0/pydisadm/loader/datasets.py
+-rw-r--r--   0        0        0     1085 2023-05-18 16:16:15.619143 pydisadm-1.2.0/pydisadm/loader/static_data.py
+-rw-r--r--   0        0        0     1294 2023-05-18 16:16:15.619143 pydisadm-1.2.0/pydisadm/runnable/runnable_refresh.py
+-rw-r--r--   0        0        0     3814 2023-05-18 16:16:15.619143 pydisadm-1.2.0/pydisadm/services/database.py
+-rw-r--r--   0        0        0     1543 2023-05-18 16:16:15.619143 pydisadm-1.2.0/pydisadm/services/esi.py
+-rw-r--r--   0        0        0      484 2023-05-18 16:16:15.619143 pydisadm-1.2.0/pydisadm/utils/adm_utils.py
+-rw-r--r--   0        0        0      472 2023-05-18 16:16:15.619143 pydisadm-1.2.0/pydisadm/utils/datetime_utils.py
+-rw-r--r--   0        0        0      623 2023-05-18 16:16:15.619143 pydisadm-1.2.0/pydisadm/utils/plot_utils.py
+-rw-r--r--   0        0        0      193 2023-05-18 16:16:15.619143 pydisadm-1.2.0/pydisadm/utils/thread_utils.py
+-rw-r--r--   0        0        0      953 2023-05-18 16:16:54.255335 pydisadm-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3792 1970-01-01 00:00:00.000000 pydisadm-1.2.0/PKG-INFO
```

### Comparing `pydisadm-1.1.2/README.md` & `pydisadm-1.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 ## 🔧 Configuration
 Configuration is done using environment variables or `dotenv`. See `.env.example` for example configuration.
 
 - `DISCORD_TOKEN` - the token bot should use when communicating with discord.
 - `DISCORD_CHANNEL` - the channel name bot should listen too, if this is empty the bot will listen to all channels.
 - `DISCORD_APP_ID` - the bot application ID
 - `ALLIANCE_ID` - the alliance ID for collecting ADM values, only systems owned by this alliance will be collected.
+- `DB_KEEP_ADM_DAYS` - how many days adm history should be kept in database (default 7).
 
 ## 🔍 Caveats
 * The ADM data from ESI is only updated once a day, so refreshing more often than that is not necessary.
 * The database will continue to fill up with historic entries, manually inspect size and purge older entries if it's too big.
 
 ## 🚧 Development
```

### Comparing `pydisadm-1.1.2/pydisadm/__main__.py` & `pydisadm-1.2.0/pydisadm/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,17 @@
     configuration = Configuration()
 
     database = Database()
 
     update_static_data(database)
 
     controller = AdmController(configuration, database)
+    
     controller.update_adm_data()
+    controller.purge_adm_records(configuration.db_keep_adm_days)
 
     bot = AdmBot(configuration, controller)
     bot.setup_cogs()
     bot.run()
 
     interrupt_event.set()
```

### Comparing `pydisadm-1.1.2/pydisadm/bot/adm_bot.py` & `pydisadm-1.2.0/pydisadm/bot/adm_bot.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.1.2/pydisadm/bot/adm_cog.py` & `pydisadm-1.2.0/pydisadm/bot/adm_cog.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.1.2/pydisadm/bot/update_adm_modal.py` & `pydisadm-1.2.0/pydisadm/bot/update_adm_modal.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.1.2/pydisadm/bot/utils.py` & `pydisadm-1.2.0/pydisadm/bot/utils.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.1.2/pydisadm/configuration.py` & `pydisadm-1.2.0/pydisadm/configuration.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,17 +6,35 @@
     def __init__(self):
         self.discord_token = os.getenv('DISCORD_TOKEN')
         self.discord_channel = os.getenv('DISCORD_CHANNEL')
         self.discord_app_id = os.getenv('DISCORD_APP_ID')
 
         alliance_id = os.getenv('ALLIANCE_ID')
 
+        db_keep_adm_days = os.getenv('DB_KEEP_ADM_DAYS', '7')
+        if db_keep_adm_days is not None:
+            try:
+                db_keep_adm_days = int(db_keep_adm_days)
+            except ValueError as error:
+                raise ValueError(
+                    '[configuration] invalid `DB_KEEP_ADM_DAYS` value',
+                    db_keep_adm_days) from error
+
+        self.db_keep_adm_days = db_keep_adm_days
+
         if alliance_id is not None:
             try:
                 alliance_id = int(alliance_id)
             except ValueError as error:
-                raise ValueError('[configuration] invalid `ALLIANCE_ID` value', alliance_id) from error
+                raise ValueError(
+                    '[configuration] invalid `ALLIANCE_ID` value',
+                    alliance_id) from error
 
         self.alliance_id = alliance_id
 
     def __str__(self):
-        return f'{self.__class__.__name__}(discord_token={self.discord_token}, discord_channel={self.discord_channel}, discord_app_id={self.discord_app_id}, alliance_id={self.alliance_id})'
+        return (f'{self.__class__.__name__}' +
+            f'(discord_token={self.discord_token}, ' +
+            f'discord_channel={self.discord_channel}, ' +
+            f'discord_app_id={self.discord_app_id}, ' +
+            f'alliance_id={self.alliance_id} ' +
+            f'db_keep_adm_days={self.db_keep_adm_days})')
```

### Comparing `pydisadm-1.1.2/pydisadm/controller/adm_controller.py` & `pydisadm-1.2.0/pydisadm/controller/adm_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,14 +201,19 @@
     def update_adm_data(self):
         """Update ADM data"""
         alliance_id = self.configuration.alliance_id
         system_adms = self.get_system_adms(alliance_id)
 
         self.database.insert_systems(system_adms)
 
+    def purge_adm_records(self, days_old: int):
+        """Purge adm records more than days_old days old"""
+
+        self.database.delete_system_rows(days_old)
+
     def write_file(self, file_name, content) -> bool:
         """Write content to file"""
         with open(file_name, 'w', encoding='UTF-8') as file:
             file.write(content)
 
         return os.path.isfile(file_name)
```

### Comparing `pydisadm-1.1.2/pydisadm/data/mapConstellations.csv` & `pydisadm-1.2.0/pydisadm/data/mapConstellations.csv`

 * *Files identical despite different names*

### Comparing `pydisadm-1.1.2/pydisadm/data/mapRegions.csv` & `pydisadm-1.2.0/pydisadm/data/mapRegions.csv`

 * *Files identical despite different names*

### Comparing `pydisadm-1.1.2/pydisadm/data/mapSolarSystems.csv` & `pydisadm-1.2.0/pydisadm/data/mapSolarSystems.csv`

 * *Files identical despite different names*

### Comparing `pydisadm-1.1.2/pydisadm/loader/datasets.py` & `pydisadm-1.2.0/pydisadm/loader/datasets.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.1.2/pydisadm/loader/static_data.py` & `pydisadm-1.2.0/pydisadm/loader/static_data.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.1.2/pydisadm/runnable/runnable_refresh.py` & `pydisadm-1.2.0/pydisadm/runnable/runnable_refresh.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,24 +12,28 @@
 def scheduler_loop(interrupt_event):
     """Scheduler main loop"""
     configuration = Configuration()
     database = Database()
 
     controller = AdmController(configuration, database)
 
-    schedule.every().day.at('11:30', tz='UTC').do(refresh_job, controller)
+    schedule.every().day.at('11:30', tz='UTC').do(refresh_job, controller, configuration)
 
     while True:
         schedule.run_pending()
         if interrupt_event.wait(timeout=1000):
             break
 
-def refresh_job(controller: AdmController):
+def refresh_job(controller: AdmController, configuration: Configuration):
     """Refresh adm data"""
     logger.info('updating adm data...')
     controller.update_adm_data()
     logger.info('adm data update finished')
 
+    logger.info('purge old adm data...')
+    controller.purge_adm_records(configuration.db_keep_adm_days)
+    logger.info('purge finished')
+
 def run_auto_refresh(interrupt_event):
     """Run automatic adm data refresh in separate thread"""
     logger.info('starting adm data update thread')
     run_threaded(lambda: scheduler_loop(interrupt_event))
```

### Comparing `pydisadm-1.1.2/pydisadm/services/database.py` & `pydisadm-1.2.0/pydisadm/services/database.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,7 +76,19 @@
     def select_system_history(self, system, limit) -> pd.DataFrame:
         """Select history of a single system"""
         return pd.read_sql_query("""
             SELECT system_id, adm, tier, created_at FROM systems
             INNER JOIN map ON map.solarSystemID = systems.system_id
             WHERE map.solarSystemName=? ORDER BY created_at DESC LIMIT ?
         """, self.conn, params=[system, limit])
+
+    def delete_system_rows(self, days_old):
+        """Delete system rows older than days_old"""
+        cur = self.conn.cursor()
+        cur.execute(f"""
+            DELETE FROM systems 
+            WHERE id IN (
+                SELECT id FROM systems WHERE created_at < (select datetime('now', '-{days_old} day'))
+            )
+        """)
+
+        self.conn.commit()
```

### Comparing `pydisadm-1.1.2/pydisadm/services/esi.py` & `pydisadm-1.2.0/pydisadm/services/esi.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.1.2/pydisadm/utils/plot_utils.py` & `pydisadm-1.2.0/pydisadm/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.1.2/pyproject.toml` & `pydisadm-1.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydisadm"
-version = "1.1.2"
+version = "1.2.0"
 description = "A Discord bot providing ADM summaries."
 repository = "https://github.com/agelito/adm-bot"
 authors = ["Axel Wettervik"]
 license = "MIT"
 readme = "README.md"
 include = ["data/*.csv"]
```

### Comparing `pydisadm-1.1.2/PKG-INFO` & `pydisadm-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydisadm
-Version: 1.1.2
+Version: 1.2.0
 Summary: A Discord bot providing ADM summaries.
 Home-page: https://github.com/agelito/adm-bot
 License: MIT
 Author: Axel Wettervik
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -75,14 +75,15 @@
 ## 🔧 Configuration
 Configuration is done using environment variables or `dotenv`. See `.env.example` for example configuration.
 
 - `DISCORD_TOKEN` - the token bot should use when communicating with discord.
 - `DISCORD_CHANNEL` - the channel name bot should listen too, if this is empty the bot will listen to all channels.
 - `DISCORD_APP_ID` - the bot application ID
 - `ALLIANCE_ID` - the alliance ID for collecting ADM values, only systems owned by this alliance will be collected.
+- `DB_KEEP_ADM_DAYS` - how many days adm history should be kept in database (default 7).
 
 ## 🔍 Caveats
 * The ADM data from ESI is only updated once a day, so refreshing more often than that is not necessary.
 * The database will continue to fill up with historic entries, manually inspect size and purge older entries if it's too big.
 
 ## 🚧 Development
```

