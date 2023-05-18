# Comparing `tmp/gpt_code_ui-0.42.5.tar.gz` & `tmp/gpt_code_ui-0.42.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_code_ui-0.42.5.tar", last modified: Thu May 18 10:47:32 2023, max compression
+gzip compressed data, was "gpt_code_ui-0.42.6.tar", last modified: Thu May 18 11:19:43 2023, max compression
```

## Comparing `gpt_code_ui-0.42.5.tar` & `gpt_code_ui-0.42.6.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 rick      (1000) rick      (1000)        0 2023-05-18 10:47:32.557512 gpt_code_ui-0.42.5/
--rw-r--r--   0 rick      (1000) rick      (1000)      186 2023-05-18 10:47:32.557512 gpt_code_ui-0.42.5/PKG-INFO
--rw-r--r--   0 rick      (1000) rick      (1000)      902 2023-05-18 10:30:13.000000 gpt_code_ui-0.42.5/README.md
-drwxr-xr-x   0 rick      (1000) rick      (1000)        0 2023-05-18 10:47:32.549512 gpt_code_ui-0.42.5/gpt_code_ui/
--rw-r--r--   0 rick      (1000) rick      (1000)        0 2023-05-12 07:34:59.000000 gpt_code_ui-0.42.5/gpt_code_ui/__init__.py
-drwxr-xr-x   0 rick      (1000) rick      (1000)        0 2023-05-18 10:47:32.549512 gpt_code_ui-0.42.5/gpt_code_ui/kernel_program/
--rw-r--r--   0 rick      (1000) rick      (1000)        0 2023-05-18 10:32:42.000000 gpt_code_ui-0.42.5/gpt_code_ui/kernel_program/__init__.py
--rw-r--r--   0 rick      (1000) rick      (1000)      396 2023-05-10 19:08:20.000000 gpt_code_ui-0.42.5/gpt_code_ui/kernel_program/config.py
--rw-r--r--   0 rick      (1000) rick      (1000)     6801 2023-05-18 10:35:50.000000 gpt_code_ui-0.42.5/gpt_code_ui/kernel_program/kernel_manager.py
--rw-r--r--   0 rick      (1000) rick      (1000)      100 2023-05-10 18:53:26.000000 gpt_code_ui-0.42.5/gpt_code_ui/kernel_program/launch_kernel.py
--rw-r--r--   0 rick      (1000) rick      (1000)     3588 2023-05-18 10:23:42.000000 gpt_code_ui-0.42.5/gpt_code_ui/kernel_program/main.py
--rw-r--r--   0 rick      (1000) rick      (1000)      943 2023-05-18 10:23:41.000000 gpt_code_ui-0.42.5/gpt_code_ui/kernel_program/utils.py
--rw-r--r--   0 rick      (1000) rick      (1000)     3092 2023-05-18 10:47:05.000000 gpt_code_ui-0.42.5/gpt_code_ui/main.py
-drwxr-xr-x   0 rick      (1000) rick      (1000)        0 2023-05-18 10:47:32.549512 gpt_code_ui-0.42.5/gpt_code_ui/webapp/
--rw-r--r--   0 rick      (1000) rick      (1000)        0 2023-05-18 10:32:38.000000 gpt_code_ui-0.42.5/gpt_code_ui/webapp/__init__.py
--rw-r--r--   0 rick      (1000) rick      (1000)     5496 2023-05-18 10:36:08.000000 gpt_code_ui-0.42.5/gpt_code_ui/webapp/main.py
-drwxr-xr-x   0 rick      (1000) rick      (1000)        0 2023-05-18 10:47:32.553512 gpt_code_ui-0.42.5/gpt_code_ui/webapp/static/
-drwxr-xr-x   0 rick      (1000) rick      (1000)        0 2023-05-18 10:47:32.557512 gpt_code_ui-0.42.5/gpt_code_ui/webapp/static/assets/
--rw-r--r--   0 rick      (1000) rick      (1000)      312 2023-05-18 10:47:32.000000 gpt_code_ui-0.42.5/gpt_code_ui/webapp/static/assets/assistant.svg
--rw-r--r--   0 rick      (1000) rick      (1000)  1122211 2023-05-17 14:56:08.000000 gpt_code_ui-0.42.5/gpt_code_ui/webapp/static/assets/index-06bbd008.js
--rw-r--r--   0 rick      (1000) rick      (1000)  1122082 2023-05-18 10:45:08.000000 gpt_code_ui-0.42.5/gpt_code_ui/webapp/static/assets/index-33a24bb9.js
--rw-r--r--   0 rick      (1000) rick      (1000)  1122082 2023-05-18 10:37:40.000000 gpt_code_ui-0.42.5/gpt_code_ui/webapp/static/assets/index-400857ec.js
--rw-r--r--   0 rick      (1000) rick      (1000)  1122082 2023-05-18 10:47:32.000000 gpt_code_ui-0.42.5/gpt_code_ui/webapp/static/assets/index-6b7f1bce.js
--rw-r--r--   0 rick      (1000) rick      (1000)  1122186 2023-05-17 15:07:40.000000 gpt_code_ui-0.42.5/gpt_code_ui/webapp/static/assets/index-9a493ce2.js
--rw-r--r--   0 rick      (1000) rick      (1000)  1122212 2023-05-17 15:36:25.000000 gpt_code_ui-0.42.5/gpt_code_ui/webapp/static/assets/index-b21b058a.js
--rw-r--r--   0 rick      (1000) rick      (1000)  1122185 2023-05-17 15:06:48.000000 gpt_code_ui-0.42.5/gpt_code_ui/webapp/static/assets/index-b3ab57c8.js
--rw-r--r--   0 rick      (1000) rick      (1000)  1122082 2023-05-18 10:25:13.000000 gpt_code_ui-0.42.5/gpt_code_ui/webapp/static/assets/index-d49e0219.js
--rw-r--r--   0 rick      (1000) rick      (1000)  1122222 2023-05-17 14:32:15.000000 gpt_code_ui-0.42.5/gpt_code_ui/webapp/static/assets/index-df4fc120.js
--rw-r--r--   0 rick      (1000) rick      (1000)  1122310 2023-05-18 09:47:59.000000 gpt_code_ui-0.42.5/gpt_code_ui/webapp/static/assets/index-e0f0db3d.js
--rw-r--r--   0 rick      (1000) rick      (1000)  1122082 2023-05-18 10:33:01.000000 gpt_code_ui-0.42.5/gpt_code_ui/webapp/static/assets/index-f33d4af3.js
--rw-r--r--   0 rick      (1000) rick      (1000)  1122082 2023-05-18 10:41:38.000000 gpt_code_ui-0.42.5/gpt_code_ui/webapp/static/assets/index-f357f93a.js
--rw-r--r--   0 rick      (1000) rick      (1000)  1122079 2023-05-18 10:19:08.000000 gpt_code_ui-0.42.5/gpt_code_ui/webapp/static/assets/index-f72f262a.js
--rw-r--r--   0 rick      (1000) rick      (1000)     2790 2023-05-18 10:47:32.000000 gpt_code_ui-0.42.5/gpt_code_ui/webapp/static/assets/index-f84b874e.css
--rw-r--r--   0 rick      (1000) rick      (1000)      312 2023-05-17 14:38:37.000000 gpt_code_ui-0.42.5/gpt_code_ui/webapp/static/assistant.svg
--rw-r--r--   0 rick      (1000) rick      (1000)      463 2023-05-18 10:47:32.000000 gpt_code_ui-0.42.5/gpt_code_ui/webapp/static/index.html
-drwxr-xr-x   0 rick      (1000) rick      (1000)        0 2023-05-18 10:47:32.549512 gpt_code_ui-0.42.5/gpt_code_ui.egg-info/
--rw-r--r--   0 rick      (1000) rick      (1000)      186 2023-05-18 10:47:32.000000 gpt_code_ui-0.42.5/gpt_code_ui.egg-info/PKG-INFO
--rw-r--r--   0 rick      (1000) rick      (1000)     1407 2023-05-18 10:47:32.000000 gpt_code_ui-0.42.5/gpt_code_ui.egg-info/SOURCES.txt
--rw-r--r--   0 rick      (1000) rick      (1000)        1 2023-05-18 10:47:32.000000 gpt_code_ui-0.42.5/gpt_code_ui.egg-info/dependency_links.txt
--rw-r--r--   0 rick      (1000) rick      (1000)       51 2023-05-18 10:47:32.000000 gpt_code_ui-0.42.5/gpt_code_ui.egg-info/entry_points.txt
--rw-r--r--   0 rick      (1000) rick      (1000)       94 2023-05-18 10:47:32.000000 gpt_code_ui-0.42.5/gpt_code_ui.egg-info/requires.txt
--rw-r--r--   0 rick      (1000) rick      (1000)       12 2023-05-18 10:47:32.000000 gpt_code_ui-0.42.5/gpt_code_ui.egg-info/top_level.txt
--rw-r--r--   0 rick      (1000) rick      (1000)       38 2023-05-18 10:47:32.557512 gpt_code_ui-0.42.5/setup.cfg
--rw-r--r--   0 rick      (1000) rick      (1000)      506 2023-05-18 10:47:10.000000 gpt_code_ui-0.42.5/setup.py
+drwxr-xr-x   0 rick      (1000) rick      (1000)        0 2023-05-18 11:19:43.067888 gpt_code_ui-0.42.6/
+-rw-r--r--   0 rick      (1000) rick      (1000)      186 2023-05-18 11:19:43.067888 gpt_code_ui-0.42.6/PKG-INFO
+-rw-r--r--   0 rick      (1000) rick      (1000)      902 2023-05-18 10:30:13.000000 gpt_code_ui-0.42.6/README.md
+drwxr-xr-x   0 rick      (1000) rick      (1000)        0 2023-05-18 11:19:43.059888 gpt_code_ui-0.42.6/gpt_code_ui/
+-rw-r--r--   0 rick      (1000) rick      (1000)        0 2023-05-12 07:34:59.000000 gpt_code_ui-0.42.6/gpt_code_ui/__init__.py
+drwxr-xr-x   0 rick      (1000) rick      (1000)        0 2023-05-18 11:19:43.059888 gpt_code_ui-0.42.6/gpt_code_ui/kernel_program/
+-rw-r--r--   0 rick      (1000) rick      (1000)        0 2023-05-18 10:32:42.000000 gpt_code_ui-0.42.6/gpt_code_ui/kernel_program/__init__.py
+-rw-r--r--   0 rick      (1000) rick      (1000)      396 2023-05-18 11:02:01.000000 gpt_code_ui-0.42.6/gpt_code_ui/kernel_program/config.py
+-rw-r--r--   0 rick      (1000) rick      (1000)     6801 2023-05-18 11:04:12.000000 gpt_code_ui-0.42.6/gpt_code_ui/kernel_program/kernel_manager.py
+-rw-r--r--   0 rick      (1000) rick      (1000)      100 2023-05-10 18:53:26.000000 gpt_code_ui-0.42.6/gpt_code_ui/kernel_program/launch_kernel.py
+-rw-r--r--   0 rick      (1000) rick      (1000)     4011 2023-05-18 11:18:34.000000 gpt_code_ui-0.42.6/gpt_code_ui/kernel_program/main.py
+-rw-r--r--   0 rick      (1000) rick      (1000)      943 2023-05-18 10:23:41.000000 gpt_code_ui-0.42.6/gpt_code_ui/kernel_program/utils.py
+-rw-r--r--   0 rick      (1000) rick      (1000)     3092 2023-05-18 10:47:05.000000 gpt_code_ui-0.42.6/gpt_code_ui/main.py
+drwxr-xr-x   0 rick      (1000) rick      (1000)        0 2023-05-18 11:19:43.059888 gpt_code_ui-0.42.6/gpt_code_ui/webapp/
+-rw-r--r--   0 rick      (1000) rick      (1000)        0 2023-05-18 10:32:38.000000 gpt_code_ui-0.42.6/gpt_code_ui/webapp/__init__.py
+-rw-r--r--   0 rick      (1000) rick      (1000)     5496 2023-05-18 10:36:08.000000 gpt_code_ui-0.42.6/gpt_code_ui/webapp/main.py
+drwxr-xr-x   0 rick      (1000) rick      (1000)        0 2023-05-18 11:19:43.059888 gpt_code_ui-0.42.6/gpt_code_ui/webapp/static/
+drwxr-xr-x   0 rick      (1000) rick      (1000)        0 2023-05-18 11:19:43.067888 gpt_code_ui-0.42.6/gpt_code_ui/webapp/static/assets/
+-rw-r--r--   0 rick      (1000) rick      (1000)      312 2023-05-18 11:19:42.000000 gpt_code_ui-0.42.6/gpt_code_ui/webapp/static/assets/assistant.svg
+-rw-r--r--   0 rick      (1000) rick      (1000)  1122211 2023-05-17 14:56:08.000000 gpt_code_ui-0.42.6/gpt_code_ui/webapp/static/assets/index-06bbd008.js
+-rw-r--r--   0 rick      (1000) rick      (1000)  1122082 2023-05-18 10:45:08.000000 gpt_code_ui-0.42.6/gpt_code_ui/webapp/static/assets/index-33a24bb9.js
+-rw-r--r--   0 rick      (1000) rick      (1000)  1122082 2023-05-18 10:37:40.000000 gpt_code_ui-0.42.6/gpt_code_ui/webapp/static/assets/index-400857ec.js
+-rw-r--r--   0 rick      (1000) rick      (1000)  1122082 2023-05-18 10:47:32.000000 gpt_code_ui-0.42.6/gpt_code_ui/webapp/static/assets/index-6b7f1bce.js
+-rw-r--r--   0 rick      (1000) rick      (1000)  1122082 2023-05-18 11:19:42.000000 gpt_code_ui-0.42.6/gpt_code_ui/webapp/static/assets/index-73967258.js
+-rw-r--r--   0 rick      (1000) rick      (1000)  1122186 2023-05-17 15:07:40.000000 gpt_code_ui-0.42.6/gpt_code_ui/webapp/static/assets/index-9a493ce2.js
+-rw-r--r--   0 rick      (1000) rick      (1000)  1122212 2023-05-17 15:36:25.000000 gpt_code_ui-0.42.6/gpt_code_ui/webapp/static/assets/index-b21b058a.js
+-rw-r--r--   0 rick      (1000) rick      (1000)  1122185 2023-05-17 15:06:48.000000 gpt_code_ui-0.42.6/gpt_code_ui/webapp/static/assets/index-b3ab57c8.js
+-rw-r--r--   0 rick      (1000) rick      (1000)  1122082 2023-05-18 10:25:13.000000 gpt_code_ui-0.42.6/gpt_code_ui/webapp/static/assets/index-d49e0219.js
+-rw-r--r--   0 rick      (1000) rick      (1000)  1122222 2023-05-17 14:32:15.000000 gpt_code_ui-0.42.6/gpt_code_ui/webapp/static/assets/index-df4fc120.js
+-rw-r--r--   0 rick      (1000) rick      (1000)  1122310 2023-05-18 09:47:59.000000 gpt_code_ui-0.42.6/gpt_code_ui/webapp/static/assets/index-e0f0db3d.js
+-rw-r--r--   0 rick      (1000) rick      (1000)  1122082 2023-05-18 10:33:01.000000 gpt_code_ui-0.42.6/gpt_code_ui/webapp/static/assets/index-f33d4af3.js
+-rw-r--r--   0 rick      (1000) rick      (1000)  1122082 2023-05-18 10:41:38.000000 gpt_code_ui-0.42.6/gpt_code_ui/webapp/static/assets/index-f357f93a.js
+-rw-r--r--   0 rick      (1000) rick      (1000)  1122079 2023-05-18 10:19:08.000000 gpt_code_ui-0.42.6/gpt_code_ui/webapp/static/assets/index-f72f262a.js
+-rw-r--r--   0 rick      (1000) rick      (1000)     2790 2023-05-18 11:19:42.000000 gpt_code_ui-0.42.6/gpt_code_ui/webapp/static/assets/index-f84b874e.css
+-rw-r--r--   0 rick      (1000) rick      (1000)      312 2023-05-17 14:38:37.000000 gpt_code_ui-0.42.6/gpt_code_ui/webapp/static/assistant.svg
+-rw-r--r--   0 rick      (1000) rick      (1000)      463 2023-05-18 11:19:42.000000 gpt_code_ui-0.42.6/gpt_code_ui/webapp/static/index.html
+drwxr-xr-x   0 rick      (1000) rick      (1000)        0 2023-05-18 11:19:43.059888 gpt_code_ui-0.42.6/gpt_code_ui.egg-info/
+-rw-r--r--   0 rick      (1000) rick      (1000)      186 2023-05-18 11:19:43.000000 gpt_code_ui-0.42.6/gpt_code_ui.egg-info/PKG-INFO
+-rw-r--r--   0 rick      (1000) rick      (1000)     1458 2023-05-18 11:19:43.000000 gpt_code_ui-0.42.6/gpt_code_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 rick      (1000) rick      (1000)        1 2023-05-18 11:19:43.000000 gpt_code_ui-0.42.6/gpt_code_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 rick      (1000) rick      (1000)       51 2023-05-18 11:19:43.000000 gpt_code_ui-0.42.6/gpt_code_ui.egg-info/entry_points.txt
+-rw-r--r--   0 rick      (1000) rick      (1000)       94 2023-05-18 11:19:43.000000 gpt_code_ui-0.42.6/gpt_code_ui.egg-info/requires.txt
+-rw-r--r--   0 rick      (1000) rick      (1000)       12 2023-05-18 11:19:43.000000 gpt_code_ui-0.42.6/gpt_code_ui.egg-info/top_level.txt
+-rw-r--r--   0 rick      (1000) rick      (1000)       38 2023-05-18 11:19:43.067888 gpt_code_ui-0.42.6/setup.cfg
+-rw-r--r--   0 rick      (1000) rick      (1000)      506 2023-05-18 11:19:16.000000 gpt_code_ui-0.42.6/setup.py
```

### Comparing `gpt_code_ui-0.42.5/README.md` & `gpt_code_ui-0.42.6/README.md`

 * *Files identical despite different names*

### Comparing `gpt_code_ui-0.42.5/gpt_code_ui/kernel_program/kernel_manager.py` & `gpt_code_ui-0.42.6/gpt_code_ui/kernel_program/kernel_manager.py`

 * *Files identical despite different names*

### Comparing `gpt_code_ui-0.42.5/gpt_code_ui/kernel_program/main.py` & `gpt_code_ui-0.42.6/gpt_code_ui/kernel_program/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import subprocess
 import sys
 import pathlib
 import json
 import logging
+import time
 
 import asyncio
 import json
 import threading
 
 from queue import Queue
 
@@ -25,14 +26,15 @@
 logger = config.get_logger()
 
 # Note, only one kernel_manager_process can be active
 kernel_manager_process = None
 
 # Use efficient Python queues to store messages
 result_queue = Queue()
+send_queue = Queue()
 
 messaging = None
 
 # We know this Flask app is for local use. So we can disable the verbose Werkzeug logger
 log = logging.getLogger('werkzeug')
 log.setLevel(logging.ERROR)
 
@@ -78,36 +80,48 @@
             logger.debug("%s of type %s" % (message["value"], message["type"]))
 
             result_queue.put(message["value"])
 
     messaging.on_message_recv.add(on_recv)
     logger.info("Starting snakemq loop")
 
-    # Wrap the snakemq_link.Link loop in an asyncio task
-    loop = asyncio.get_event_loop()
-    link_loop_task = loop.run_in_executor(None, link.loop)
+    def send_queued_messages():
+        while True:
+            if send_queue.qsize() > 0:
+                message = send_queue.get()
+                utils.send_json(messaging, 
+                    {"type": "execute", "value": message["command"]}, 
+                    config.IDENT_KERNEL_MANAGER
+                )
+            time.sleep(0.1)
+
+    async def async_send_queued_messages():
+        loop = asyncio.get_event_loop()
+        await loop.run_in_executor(None, send_queued_messages)
+
+    async def async_link_loop():
+        loop = asyncio.get_event_loop()
+        await loop.run_in_executor(None, link.loop)
 
-    # Wait for the snakemq_link.Link loop to complete (if ever)
-    await link_loop_task
+    # Wrap the snakemq_link.Link loop in an asyncio task
+    await asyncio.gather(async_send_queued_messages(), async_link_loop())
 
 
 @app.route("/api", methods=["POST", "GET"])
 def handle_request():
-    
+   
     if request.method == "GET":
         # Handle GET requests by sending everything that's in the receive_queue
         results = [result_queue.get() for _ in range(result_queue.qsize())]
         return jsonify({"results": results})
     elif request.method == "POST":
         data = request.json
 
-        utils.send_json(messaging, 
-            {"type": "execute", "value": data["command"]}, 
-            config.IDENT_KERNEL_MANAGER
-        )
+        send_queue.put(data)
+
         return jsonify({"result": "success"})
     
 @app.route("/restart", methods=["POST"])
 def handle_restart():
 
     cleanup_kernel_program()
     start_kernel_manager()
```

### Comparing `gpt_code_ui-0.42.5/gpt_code_ui/kernel_program/utils.py` & `gpt_code_ui-0.42.6/gpt_code_ui/kernel_program/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_code_ui-0.42.5/gpt_code_ui/main.py` & `gpt_code_ui-0.42.6/gpt_code_ui/main.py`

 * *Files identical despite different names*

### Comparing `gpt_code_ui-0.42.5/gpt_code_ui/webapp/main.py` & `gpt_code_ui-0.42.6/gpt_code_ui/webapp/main.py`

 * *Files identical despite different names*

### Comparing `gpt_code_ui-0.42.5/gpt_code_ui/webapp/static/assets/index-06bbd008.js` & `gpt_code_ui-0.42.6/gpt_code_ui/webapp/static/assets/index-06bbd008.js`

 * *Files identical despite different names*

### Comparing `gpt_code_ui-0.42.5/gpt_code_ui/webapp/static/assets/index-33a24bb9.js` & `gpt_code_ui-0.42.6/gpt_code_ui/webapp/static/assets/index-33a24bb9.js`

 * *Files identical despite different names*

### Comparing `gpt_code_ui-0.42.5/gpt_code_ui/webapp/static/assets/index-400857ec.js` & `gpt_code_ui-0.42.6/gpt_code_ui/webapp/static/assets/index-400857ec.js`

 * *Files identical despite different names*

### Comparing `gpt_code_ui-0.42.5/gpt_code_ui/webapp/static/assets/index-6b7f1bce.js` & `gpt_code_ui-0.42.6/gpt_code_ui/webapp/static/assets/index-6b7f1bce.js`

 * *Files identical despite different names*

### Comparing `gpt_code_ui-0.42.5/gpt_code_ui/webapp/static/assets/index-9a493ce2.js` & `gpt_code_ui-0.42.6/gpt_code_ui/webapp/static/assets/index-9a493ce2.js`

 * *Files identical despite different names*

### Comparing `gpt_code_ui-0.42.5/gpt_code_ui/webapp/static/assets/index-b21b058a.js` & `gpt_code_ui-0.42.6/gpt_code_ui/webapp/static/assets/index-b21b058a.js`

 * *Files identical despite different names*

### Comparing `gpt_code_ui-0.42.5/gpt_code_ui/webapp/static/assets/index-b3ab57c8.js` & `gpt_code_ui-0.42.6/gpt_code_ui/webapp/static/assets/index-b3ab57c8.js`

 * *Files identical despite different names*

### Comparing `gpt_code_ui-0.42.5/gpt_code_ui/webapp/static/assets/index-d49e0219.js` & `gpt_code_ui-0.42.6/gpt_code_ui/webapp/static/assets/index-d49e0219.js`

 * *Files identical despite different names*

### Comparing `gpt_code_ui-0.42.5/gpt_code_ui/webapp/static/assets/index-df4fc120.js` & `gpt_code_ui-0.42.6/gpt_code_ui/webapp/static/assets/index-df4fc120.js`

 * *Files identical despite different names*

### Comparing `gpt_code_ui-0.42.5/gpt_code_ui/webapp/static/assets/index-e0f0db3d.js` & `gpt_code_ui-0.42.6/gpt_code_ui/webapp/static/assets/index-e0f0db3d.js`

 * *Files identical despite different names*

### Comparing `gpt_code_ui-0.42.5/gpt_code_ui/webapp/static/assets/index-f33d4af3.js` & `gpt_code_ui-0.42.6/gpt_code_ui/webapp/static/assets/index-f33d4af3.js`

 * *Files identical despite different names*

### Comparing `gpt_code_ui-0.42.5/gpt_code_ui/webapp/static/assets/index-f357f93a.js` & `gpt_code_ui-0.42.6/gpt_code_ui/webapp/static/assets/index-f357f93a.js`

 * *Files identical despite different names*

### Comparing `gpt_code_ui-0.42.5/gpt_code_ui/webapp/static/assets/index-f72f262a.js` & `gpt_code_ui-0.42.6/gpt_code_ui/webapp/static/assets/index-f72f262a.js`

 * *Files identical despite different names*

### Comparing `gpt_code_ui-0.42.5/gpt_code_ui/webapp/static/assets/index-f84b874e.css` & `gpt_code_ui-0.42.6/gpt_code_ui/webapp/static/assets/index-f84b874e.css`

 * *Files identical despite different names*

### Comparing `gpt_code_ui-0.42.5/gpt_code_ui.egg-info/SOURCES.txt` & `gpt_code_ui-0.42.6/gpt_code_ui.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 gpt_code_ui/webapp/static/assistant.svg
 gpt_code_ui/webapp/static/index.html
 gpt_code_ui/webapp/static/assets/assistant.svg
 gpt_code_ui/webapp/static/assets/index-06bbd008.js
 gpt_code_ui/webapp/static/assets/index-33a24bb9.js
 gpt_code_ui/webapp/static/assets/index-400857ec.js
 gpt_code_ui/webapp/static/assets/index-6b7f1bce.js
+gpt_code_ui/webapp/static/assets/index-73967258.js
 gpt_code_ui/webapp/static/assets/index-9a493ce2.js
 gpt_code_ui/webapp/static/assets/index-b21b058a.js
 gpt_code_ui/webapp/static/assets/index-b3ab57c8.js
 gpt_code_ui/webapp/static/assets/index-d49e0219.js
 gpt_code_ui/webapp/static/assets/index-df4fc120.js
 gpt_code_ui/webapp/static/assets/index-e0f0db3d.js
 gpt_code_ui/webapp/static/assets/index-f33d4af3.js
```

