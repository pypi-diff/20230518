# Comparing `tmp/channels_yroom-0.0.5.tar.gz` & `tmp/channels_yroom-0.0.6.tar.gz`

## Comparing `channels_yroom-0.0.5.tar` & `channels_yroom-0.0.6.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/.dockerignore
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/.readthedocs.yaml
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/CHANGELOG.md
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/Dockerfile
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/docker-compose.yml
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/mkdocs.yml
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/.github/workflows/release.yml
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/.github/workflows/test.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/channels_yroom/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/channels_yroom/__init__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/channels_yroom/admin.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/channels_yroom/apps.py
--rw-r--r--   0        0        0     8646 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/channels_yroom/channel.py
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/channels_yroom/conf.py
--rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/channels_yroom/consumer.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/channels_yroom/models.py
--rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/channels_yroom/proxy.py
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/channels_yroom/storage.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/channels_yroom/utils.py
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/channels_yroom/worker.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/channels_yroom/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/channels_yroom/management/commands/__init__.py
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/channels_yroom/management/commands/yroom.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/channels_yroom/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/channels_yroom/migrations/__init__.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/docs/api.md
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/docs/explanation.md
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/docs/index.md
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/docs/requirements.in
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/docs/requirements.txt
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/docs/settings.md
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/docs/tutorial.md
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/docs/howto/tiptap.md
--rwxr-xr-x   0        0        0      674 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/manage.py
--rw-r--r--   0        0        0   174304 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/package-lock.json
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/package.json
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/requirements.txt
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/vite.config.js
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/frontend/main.js
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/frontend/prosemirror.js
--rw-r--r--   0        0        0     6466 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/frontend/schema.js
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/frontend/style.css
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/frontend/tiptap.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/textcollab/__init__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/textcollab/admin.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/textcollab/apps.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/textcollab/consumers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/textcollab/models.py
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/textcollab/routing.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/textcollab/tests.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/textcollab/urls.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/textcollab/views.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/textcollab/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/textcollab/migrations/__init__.py
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/textcollab/templates/textcollab/index.html
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/textcollab/templates/textcollab/room.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/textcollab_project/__init__.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/textcollab_project/asgi.py
--rw-r--r--   0        0        0     5400 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/textcollab_project/settings.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/textcollab_project/urls.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/example/textcollab_project/wsgi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/tests/conftest.py
--rw-r--r--   0        0        0    11246 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/tests/test_consumer.py
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/tests/test_worker.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/LICENSE
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/README.md
--rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 channels_yroom-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/.dockerignore
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/.readthedocs.yaml
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/CHANGELOG.md
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/Dockerfile
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/docker-compose.yml
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/mkdocs.yml
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/.github/workflows/release.yml
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/.github/workflows/test.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/channels_yroom/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/channels_yroom/__init__.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/channels_yroom/admin.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/channels_yroom/apps.py
+-rw-r--r--   0        0        0     8913 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/channels_yroom/channel.py
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/channels_yroom/conf.py
+-rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/channels_yroom/consumer.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/channels_yroom/models.py
+-rw-r--r--   0        0        0     4825 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/channels_yroom/proxy.py
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/channels_yroom/storage.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/channels_yroom/utils.py
+-rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/channels_yroom/worker.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/channels_yroom/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/channels_yroom/management/commands/__init__.py
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/channels_yroom/management/commands/yroom.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/channels_yroom/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/channels_yroom/migrations/__init__.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/docs/api.md
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/docs/explanation.md
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/docs/index.md
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/docs/requirements.in
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/docs/requirements.txt
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/docs/settings.md
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/docs/tutorial.md
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/docs/howto/tiptap.md
+-rwxr-xr-x   0        0        0      674 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/example/manage.py
+-rw-r--r--   0        0        0   174304 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/example/package-lock.json
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/example/package.json
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/example/requirements.txt
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/example/vite.config.js
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/example/frontend/main.js
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/example/frontend/prosemirror.js
+-rw-r--r--   0        0        0     6466 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/example/frontend/schema.js
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/example/frontend/style.css
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/example/frontend/tiptap.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/example/textcollab/__init__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/example/textcollab/admin.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/example/textcollab/apps.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/example/textcollab/consumers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/example/textcollab/models.py
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/example/textcollab/routing.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/example/textcollab/tests.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/example/textcollab/urls.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/example/textcollab/views.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/example/textcollab/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/example/textcollab/migrations/__init__.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/example/textcollab/templates/textcollab/index.html
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/example/textcollab/templates/textcollab/room.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/example/textcollab_project/__init__.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/example/textcollab_project/asgi.py
+-rw-r--r--   0        0        0     5400 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/example/textcollab_project/settings.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/example/textcollab_project/urls.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/example/textcollab_project/wsgi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/tests/conftest.py
+-rw-r--r--   0        0        0    11246 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/tests/test_consumer.py
+-rw-r--r--   0        0        0     6119 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/tests/test_worker.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/LICENSE
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/README.md
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 channels_yroom-0.0.6/PKG-INFO
```

### Comparing `channels_yroom-0.0.5/Dockerfile` & `channels_yroom-0.0.6/Dockerfile`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.5/docker-compose.yml` & `channels_yroom-0.0.6/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.5/mkdocs.yml` & `channels_yroom-0.0.6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.5/.github/workflows/release.yml` & `channels_yroom-0.0.6/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.5/.github/workflows/test.yml` & `channels_yroom-0.0.6/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.5/channels_yroom/channel.py` & `channels_yroom-0.0.6/channels_yroom/channel.py`

 * *Files 5% similar despite different names*

```diff
@@ -94,30 +94,36 @@
         if not hasattr(self.room_manager, method):
             logger.warning("yroom consumer bad rpc method %s %s", room_name, method)
             return
         manager_method = getattr(self.room_manager, method)
         if not callable(manager_method):
             logger.warning("yroom consumer bad rpc method %s %s", room_name, method)
             return
-
+        logger.debug("yroom consumer rpc %s %s", room_name, method)
         async with self.try_room(room_name) as room_available:
             if not room_available:
                 # No room and no snapshot, send back empty result
                 await self.channel_layer.send(
-                    message["channel"],
+                    message["channel_name"],
                     {
                         "type": "rpc_response",
                         "result": None,
                     },
                 )
                 return
             result = manager_method(room_name, *message["params"])
-
+        logger.debug(
+            "yroom consumer rpc response %s %s to %s: %s",
+            room_name,
+            method,
+            message["channel_name"],
+            result,
+        )
         await self.channel_layer.send(
-            message["channel"],
+            message["channel_name"],
             {
                 "type": "rpc_response",
                 "result": result,
             },
         )
 
     async def respond(
```

### Comparing `channels_yroom-0.0.5/channels_yroom/conf.py` & `channels_yroom-0.0.6/channels_yroom/conf.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.5/channels_yroom/consumer.py` & `channels_yroom-0.0.6/channels_yroom/consumer.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.5/channels_yroom/models.py` & `channels_yroom-0.0.6/channels_yroom/models.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.5/channels_yroom/proxy.py` & `channels_yroom-0.0.6/channels_yroom/proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         channel_name: str = await self.channel_layer.new_channel()
         room_settings = get_room_settings(self.room_name)
         await self.channel_layer.send(
             room_settings["CHANNEL_NAME"],
             YroomChannelRPCMessage(
                 type=YroomChannelMessageType.rpc.value,
                 room=self.room_name,
-                channel=channel_name,
+                channel_name=channel_name,
                 method=method,
                 params=params,
             ),
         )
         response: YroomChannelRPCResponse = await self.channel_layer.receive(
             channel_name
         )
```

### Comparing `channels_yroom-0.0.5/channels_yroom/storage.py` & `channels_yroom-0.0.6/channels_yroom/storage.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.5/channels_yroom/management/commands/yroom.py` & `channels_yroom-0.0.6/channels_yroom/management/commands/yroom.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.5/channels_yroom/migrations/0001_initial.py` & `channels_yroom-0.0.6/channels_yroom/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.5/docs/explanation.md` & `channels_yroom-0.0.6/docs/explanation.md`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.5/docs/index.md` & `channels_yroom-0.0.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.5/docs/settings.md` & `channels_yroom-0.0.6/docs/settings.md`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.5/docs/tutorial.md` & `channels_yroom-0.0.6/docs/tutorial.md`

 * *Files 4% similar despite different names*

```diff
@@ -49,19 +49,14 @@
 # ...
 application = ProtocolTypeRouter(
     {
         "http": get_asgi_application(),
         "websocket": AllowedHostsOriginValidator(
             AuthMiddlewareStack(URLRouter(textcollab.routing.websocket_urlpatterns))
         ),
-        "channel": ChannelNameRouter(
-            {
-                "yroom": YRoomChannelConsumer.as_asgi(),
-            }
-        ),
     }
 )
 ```
 
 ### Use a channel layer for inter-process communication
 
 **Warning: The In-Memory Channel Layer will not work with `channels-yroom`!**
```

### Comparing `channels_yroom-0.0.5/docs/howto/tiptap.md` & `channels_yroom-0.0.6/docs/howto/tiptap.md`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         return get_tiptap_room_name(room_name)
 
 ```
 
 Your `settings.py` should contain the following:
 
 ```python
-YROOM_ROOM_SETTINGS = {
+YROOM_SETTINGS = {
     "tiptap-editor": {
         # HocuspocusProvider adds and expects a name prefix
         "PROTOCOL_NAME_PREFIX": True,
         # Since the server doesn't know the name on connect,
         # it has to wait for communication from client
         "SERVER_START_SYNC": False,
         # HocuspocusProvider can only read one message per WS frame
```

### Comparing `channels_yroom-0.0.5/example/manage.py` & `channels_yroom-0.0.6/example/manage.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.5/example/package-lock.json` & `channels_yroom-0.0.6/example/package-lock.json`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.5/example/package.json` & `channels_yroom-0.0.6/example/package.json`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.5/example/frontend/main.js` & `channels_yroom-0.0.6/example/frontend/main.js`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.5/example/frontend/prosemirror.js` & `channels_yroom-0.0.6/example/frontend/prosemirror.js`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.5/example/frontend/schema.js` & `channels_yroom-0.0.6/example/frontend/schema.js`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.5/example/frontend/tiptap.js` & `channels_yroom-0.0.6/example/frontend/tiptap.js`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.5/example/textcollab/consumers.py` & `channels_yroom-0.0.6/example/textcollab/consumers.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.5/example/textcollab/urls.py` & `channels_yroom-0.0.6/example/textcollab/urls.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.5/example/textcollab/views.py` & `channels_yroom-0.0.6/example/textcollab/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,14 @@
 async def save_room(request, room_name, editor="prosemirror"):
     # Get the XML fragment from the server ydoc
     if editor == "prosemirror":
         room_group_name = get_prosemirror_room_name(room_name)
         YDOC_XML_FRAGMENT_KEY = "prosemirror"
     elif editor == "tiptap":
         room_group_name = get_tiptap_room_name(room_name)
-        YDOC_XML_FRAGMENT_KEY = "default"
+        YDOC_XML_FRAGMENT_KEY = "content"
     doc = YroomDocument(room_group_name)
     try:
         result: Optional[str] = await doc.export_xml_fragment(YDOC_XML_FRAGMENT_KEY)
     except DataUnavailable:
         return HttpResponse(status=404)
     return HttpResponse(result)
```

### Comparing `channels_yroom-0.0.5/example/textcollab/migrations/0001_initial.py` & `channels_yroom-0.0.6/example/textcollab/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.5/example/textcollab/templates/textcollab/index.html` & `channels_yroom-0.0.6/example/textcollab/templates/textcollab/index.html`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.5/example/textcollab_project/asgi.py` & `channels_yroom-0.0.6/example/textcollab_project/asgi.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,25 +13,18 @@
 
 os.environ.setdefault("DJANGO_SETTINGS_MODULE", "textcollab_project.settings")
 django_asgi_app = get_asgi_application()
 
 
 import textcollab.routing
 from channels.auth import AuthMiddlewareStack
-from channels.routing import ChannelNameRouter, ProtocolTypeRouter, URLRouter
+from channels.routing import ProtocolTypeRouter, URLRouter
 from channels.security.websocket import AllowedHostsOriginValidator
 
-from channels_yroom.channel import YRoomChannelConsumer
-
 application = ProtocolTypeRouter(
     {
         "http": django_asgi_app,
         "websocket": AllowedHostsOriginValidator(
             AuthMiddlewareStack(URLRouter(textcollab.routing.websocket_urlpatterns))
         ),
-        "channel": ChannelNameRouter(
-            {
-                "yroom": YRoomChannelConsumer.as_asgi(),
-            }
-        ),
     }
 )
```

### Comparing `channels_yroom-0.0.5/example/textcollab_project/settings.py` & `channels_yroom-0.0.6/example/textcollab_project/settings.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.5/example/textcollab_project/urls.py` & `channels_yroom-0.0.6/example/textcollab_project/urls.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.5/tests/conftest.py` & `channels_yroom-0.0.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.5/tests/test_consumer.py` & `channels_yroom-0.0.6/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.5/LICENSE` & `channels_yroom-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.5/README.md` & `channels_yroom-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.5/pyproject.toml` & `channels_yroom-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.5/PKG-INFO` & `channels_yroom-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: channels-yroom
-Version: 0.0.5
+Version: 0.0.6
 Summary: Yjs sync protocol server for Django channels
 Project-URL: Documentation, https://github.com/stefanw/channels-yroom#readme
 Project-URL: Issues, https://github.com/stefanw/channels-yroom/issues
 Project-URL: Source, https://github.com/stefanw/channels-yroom
 Author-email: Stefan Wehrmeyer <mail@stefanwehrmeyer.com>
 License-Expression: MIT
 License-File: LICENSE
```

