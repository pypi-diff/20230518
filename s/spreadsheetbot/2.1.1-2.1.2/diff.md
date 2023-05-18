# Comparing `tmp/spreadsheetbot-2.1.1.tar.gz` & `tmp/spreadsheetbot-2.1.2.tar.gz`

## Comparing `spreadsheetbot-2.1.1.tar` & `spreadsheetbot-2.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/Makefile
--rw-r--r--   0        0        0     7029 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/src/spreadsheetbot/__init__.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/src/spreadsheetbot/basic/__init__.py
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/src/spreadsheetbot/basic/drive.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/src/spreadsheetbot/basic/errors.py
--rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/src/spreadsheetbot/basic/handlers.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/src/spreadsheetbot/basic/log.py
--rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/__init__.py
--rw-r--r--   0        0        0     9538 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/abstract.py
--rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/groups.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/i18n.py
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/keyboard.py
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/log.py
--rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/notifications.py
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/registration.py
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/report.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/settings.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/switch.py
--rw-r--r--   0        0        0    20944 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/users.py
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/.gitignore
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/LICENSE.txt
--rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/README.md
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/Makefile
+-rw-r--r--   0        0        0     7029 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/src/spreadsheetbot/__init__.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/src/spreadsheetbot/basic/__init__.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/src/spreadsheetbot/basic/drive.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/src/spreadsheetbot/basic/errors.py
+-rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/src/spreadsheetbot/basic/handlers.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/src/spreadsheetbot/basic/log.py
+-rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/__init__.py
+-rw-r--r--   0        0        0     9538 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/abstract.py
+-rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/groups.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/i18n.py
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/keyboard.py
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/log.py
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/notifications.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/registration.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/report.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/settings.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/switch.py
+-rw-r--r--   0        0        0    20944 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/users.py
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/.gitignore
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/LICENSE.txt
+-rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/README.md
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/PKG-INFO
```

### Comparing `spreadsheetbot-2.1.1/src/spreadsheetbot/__init__.py` & `spreadsheetbot-2.1.2/src/spreadsheetbot/__init__.py`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.1/src/spreadsheetbot/basic/drive.py` & `spreadsheetbot-2.1.2/src/spreadsheetbot/basic/drive.py`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.1/src/spreadsheetbot/basic/handlers.py` & `spreadsheetbot-2.1.2/src/spreadsheetbot/basic/handlers.py`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.1/src/spreadsheetbot/basic/log.py` & `spreadsheetbot-2.1.2/src/spreadsheetbot/basic/log.py`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/__init__.py` & `spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 import asyncio
 from telegram.ext import Application
 from telegram.constants import ParseMode
 
 from spreadsheetbot.basic.log import Log
 
 def PerformAndScheldueNotifications(app: Application):
-    app.create_task(
-        _perform_notifications(app),
-        {
-            'action': 'Perform first notifications'
-        }
-    )
+    # app.create_task(
+    #     _perform_notifications(app),
+    #     {
+    #         'action': 'Perform first notifications'
+    #     }
+    # )
     ScheldueNotifications(app)
 
 def ScheldueNotifications(app: Application) -> None:
     app.create_task(
         _scheldue_and_perform_notification(app),
         {
             'action': 'Perform scheldued notifications'
```

### Comparing `spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/abstract.py` & `spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/abstract.py`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/groups.py` & `spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/groups.py`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/i18n.py` & `spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/i18n.py`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/keyboard.py` & `spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/keyboard.py`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/log.py` & `spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/log.py`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/notifications.py` & `spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/notifications.py`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/registration.py` & `spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/registration.py`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/report.py` & `spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/report.py`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/settings.py` & `spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/settings.py`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/switch.py` & `spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/switch.py`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.1/src/spreadsheetbot/sheets/users.py` & `spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/users.py`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.1/.gitignore` & `spreadsheetbot-2.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.1/LICENSE.txt` & `spreadsheetbot-2.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.1/README.md` & `spreadsheetbot-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.1/pyproject.toml` & `spreadsheetbot-2.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "spreadsheetbot"
-version = "2.1.1"
+version = "2.1.2"
 authors = [
   { name="Egor Dubrovin", email="dubrovin.en@ya.ru" },
 ]
 description = "Google Spreadsheet-based Telegram Bot Package"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `spreadsheetbot-2.1.1/PKG-INFO` & `spreadsheetbot-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spreadsheetbot
-Version: 2.1.1
+Version: 2.1.2
 Summary: Google Spreadsheet-based Telegram Bot Package
 Project-URL: Homepage, https://github.com/twobrowin-study/spreadsheetbot-lib
 Project-URL: Bug Tracker, https://github.com/twobrowin-study/spreadsheetbot-lib/issues
 Author-email: Egor Dubrovin <dubrovin.en@ya.ru>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

