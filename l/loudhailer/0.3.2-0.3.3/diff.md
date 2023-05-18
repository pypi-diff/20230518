# Comparing `tmp/loudhailer-0.3.2.tar.gz` & `tmp/loudhailer-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loudhailer-0.3.2.tar", max compression
+gzip compressed data, was "loudhailer-0.3.3.tar", max compression
```

## Comparing `loudhailer-0.3.2.tar` & `loudhailer-0.3.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2023-01-16 16:49:04.992839 loudhailer-0.3.2/LICENSE
--rw-r--r--   0        0        0     4578 2023-01-16 16:49:04.992839 loudhailer-0.3.2/README.md
--rw-r--r--   0        0        0       59 2023-01-16 16:49:04.992839 loudhailer-0.3.2/loudhailer/__init__.py
--rw-r--r--   0        0        0      131 2023-01-16 16:49:04.992839 loudhailer-0.3.2/loudhailer/backends/__init__.py
--rw-r--r--   0        0        0      884 2023-01-16 16:49:04.992839 loudhailer-0.3.2/loudhailer/backends/base.py
--rw-r--r--   0        0        0     5270 2023-01-16 16:49:04.992839 loudhailer-0.3.2/loudhailer/backends/rabbitmq.py
--rw-r--r--   0        0        0     2183 2023-01-16 16:49:04.992839 loudhailer-0.3.2/loudhailer/backends/redis.py
--rw-r--r--   0        0        0      498 2023-01-16 16:49:04.992839 loudhailer-0.3.2/loudhailer/backends/utils.py
--rw-r--r--   0        0        0      365 2023-01-16 16:49:04.992839 loudhailer-0.3.2/loudhailer/dataclasses.py
--rw-r--r--   0        0        0        0 2023-01-16 16:49:04.992839 loudhailer-0.3.2/loudhailer/ext/__init__.py
--rw-r--r--   0        0        0     5640 2023-01-16 16:49:04.992839 loudhailer-0.3.2/loudhailer/ext/channels.py
--rw-r--r--   0        0        0     5164 2023-01-16 16:49:04.992839 loudhailer-0.3.2/loudhailer/loudhailer.py
--rw-r--r--   0        0        0      262 2023-01-16 16:49:04.992839 loudhailer-0.3.2/loudhailer/utils.py
--rw-r--r--   0        0        0     1955 2023-01-16 16:50:23.615176 loudhailer-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     5620 1970-01-01 00:00:00.000000 loudhailer-0.3.2/setup.py
--rw-r--r--   0        0        0     5993 1970-01-01 00:00:00.000000 loudhailer-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-18 18:48:05.088512 loudhailer-0.3.3/LICENSE
+-rw-r--r--   0        0        0     4578 2023-05-18 18:48:05.088512 loudhailer-0.3.3/README.md
+-rw-r--r--   0        0        0       59 2023-05-18 18:48:05.092512 loudhailer-0.3.3/loudhailer/__init__.py
+-rw-r--r--   0        0        0      131 2023-05-18 18:48:05.092512 loudhailer-0.3.3/loudhailer/backends/__init__.py
+-rw-r--r--   0        0        0      884 2023-05-18 18:48:05.092512 loudhailer-0.3.3/loudhailer/backends/base.py
+-rw-r--r--   0        0        0     5270 2023-05-18 18:48:05.092512 loudhailer-0.3.3/loudhailer/backends/rabbitmq.py
+-rw-r--r--   0        0        0     2183 2023-05-18 18:48:05.092512 loudhailer-0.3.3/loudhailer/backends/redis.py
+-rw-r--r--   0        0        0      498 2023-05-18 18:48:05.092512 loudhailer-0.3.3/loudhailer/backends/utils.py
+-rw-r--r--   0        0        0      365 2023-05-18 18:48:05.092512 loudhailer-0.3.3/loudhailer/dataclasses.py
+-rw-r--r--   0        0        0        0 2023-05-18 18:48:05.092512 loudhailer-0.3.3/loudhailer/ext/__init__.py
+-rw-r--r--   0        0        0     5640 2023-05-18 18:48:05.092512 loudhailer-0.3.3/loudhailer/ext/channels.py
+-rw-r--r--   0        0        0     5197 2023-05-18 18:48:05.092512 loudhailer-0.3.3/loudhailer/loudhailer.py
+-rw-r--r--   0        0        0      262 2023-05-18 18:48:05.092512 loudhailer-0.3.3/loudhailer/utils.py
+-rw-r--r--   0        0        0     1955 2023-05-18 18:49:28.046139 loudhailer-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     5620 1970-01-01 00:00:00.000000 loudhailer-0.3.3/setup.py
+-rw-r--r--   0        0        0     5993 1970-01-01 00:00:00.000000 loudhailer-0.3.3/PKG-INFO
```

### Comparing `loudhailer-0.3.2/LICENSE` & `loudhailer-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `loudhailer-0.3.2/README.md` & `loudhailer-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `loudhailer-0.3.2/loudhailer/backends/base.py` & `loudhailer-0.3.3/loudhailer/backends/base.py`

 * *Files identical despite different names*

### Comparing `loudhailer-0.3.2/loudhailer/backends/rabbitmq.py` & `loudhailer-0.3.3/loudhailer/backends/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `loudhailer-0.3.2/loudhailer/backends/redis.py` & `loudhailer-0.3.3/loudhailer/backends/redis.py`

 * *Files identical despite different names*

### Comparing `loudhailer-0.3.2/loudhailer/ext/channels.py` & `loudhailer-0.3.3/loudhailer/ext/channels.py`

 * *Files identical despite different names*

### Comparing `loudhailer-0.3.2/loudhailer/loudhailer.py` & `loudhailer-0.3.3/loudhailer/loudhailer.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
         subscriptions = self._subscriptions.get(group, set())
 
         async with self._lock:
             if subscriber in subscriptions:
                 subscriptions.remove(subscriber)
             if subscriber in self._subscribers:
                 del self._subscribers[subscriber]
-            if not subscriptions:
+            if not subscriptions and group in self._subscriptions:
                 await self._backend.unsubscribe(group)
                 del self._subscriptions[group]
 
     async def receive_message(self, subscriber):
         queue = self._subscribers.setdefault(subscriber, asyncio.Queue())
         return await queue.get()
```

### Comparing `loudhailer-0.3.2/pyproject.toml` & `loudhailer-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "loudhailer"
-version = "0.3.2"
+version = "0.3.3"
 description = ""
 authors = ["CloudBlue LLC"]
 license = "Apache-2.0"
 packages = [
     { include = "loudhailer" },
 ]
 readme = "./README.md"
```

### Comparing `loudhailer-0.3.2/setup.py` & `loudhailer-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 extras_require = \
 {':python_version < "3.9"': ['backports.zoneinfo'],
  ':sys_platform == "win32"': ['tzdata'],
  'channels': ['channels>=3.0.0,<4.0.0']}
 
 setup_kwargs = {
     'name': 'loudhailer',
-    'version': '0.3.2',
+    'version': '0.3.3',
     'description': '',
     'long_description': "# Loudhailer\n\n![pyversions](https://img.shields.io/pypi/pyversions/loudhailer.svg) [![PyPi Status](https://img.shields.io/pypi/v/loudhailer.svg)](https://pypi.org/project/loudhailer/) [![Test Loudhailer](https://github.com/cloudblue/loudhailer/actions/workflows/test.yml/badge.svg)](https://github.com/cloudblue/loudhailer/actions/workflows/test.yml) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=loudhailer&metric=alert_status)](https://sonarcloud.io/dashboard?id=loudhailer) [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=loudhailer&metric=coverage)](https://sonarcloud.io/dashboard?id=loudhailer) [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=loudhailer&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=loudhailer)\n\n## Introduction\n\n`Loudhailer` is a python library that allows to send broadcast messages to groups of consumers. It has been designed for being used in asynchronous applications.\n\nThis initial release natively supports RabbitMQ and Redis backends and can be easily extended to support more backends.\n\n`Loudhailer` includes an extension that allows you to use in django-channels based projects.\n\n\n> Please note that the current version of Loudhailer have to be considered a beta release since it is still under heavy development.\n\n\n\n\n## Install\n\n`Loudhailer` requires python 3.8 or later.\n\n\n`Loudhailer` can be installed from [pypi.org](https://pypi.org/project/loudhailer/) using pip:\n\n```\n$ pip install loudhailer\n```\n\nIf you plan to use it with django-channels you must install the optional channels dependency:\n\n```\n$ pip install loudhailer[channels]\n```\n\n\n## Basic usage\n\n### Publishing messages\n\n```python\nfrom loudhailer import Loudhailer\n\n\nasync with Loudhailer('amqp://localhost') as loudhailer:\n    await loudhailer.publish('my_group', {'message': 'data'})\n```\n\n### Subscribe to group and receive messages\n\n```python\n\nfrom loudhailer import Loudhailer\n\n\nwith Loudhailer('amqp://localhost') as loudhailer:\n    with loudhailer.subscribe('my_group') as messages:\n        message = await messages.get()\n        print(f'received message: {message}')\n```\n\n## Django channels extension\n\nThe django-channels extension is an implementation of the Channel Layers specifications.\n\nIn order to properly works it need to add a ASGI lifespan handler to your channels application.\n\n\n> Please note that Channel Layers specification are not yet fully implemented, only group messaging is supported in this\ninitial release.\n\n\n### Django settings\n\nAdd the following Channel Layers configuration to your Django settings module:\n\n```python \nCHANNEL_LAYERS = {\n    'default': {\n        'BACKEND': 'loudhailer.ext.channels.LoudhailerChannelLayer',\n        'CONFIG': {\n            'url': 'amqp://localhost',\n        },\n    },\n}\n```\n\n### Configure the ASGI lifespan handler\n\nAdd the following configuration to your root channels routing module:\n\n```python\nfrom channels.routing import ProtocolTypeRouter, URLRouter\nfrom loudhailer.ext.channels import LoudhailerChannelLifespan\n\napplication = ProtocolTypeRouter(\n    {\n        'lifespan': LoudhailerChannelLifespan.as_asgi(),\n        'websocket': URLRouter(...),\n    },\n)\n```\n\nIn case you already have an handler to process lifespan **startup** and **shutdown** events you can be notified of\nsuch event by the *LoudhailerChannelLifespan* handler in two ways:\n\n#### Using django signals\n\nYou can register your signal handler for **startup** and **shutdown** events in the following way:\n\n```python\nfrom django.dispatch import receiver\nfrom loudhailer.ext.channels import asgi_application_shutdown, asgi_application_startup\n\n\n@receiver(asgi_application_startup)\ndef handle_startup(sender, **kwargs):\n    pass\n\n@receiver(asgi_application_shutdown)\ndef handle_shutdown(sender, **kwargs):\n    pass\n```\n\n#### Using **on_startup** and **on_shutdown** hooks\n\n```python\nfrom channels.routing import ProtocolTypeRouter, URLRouter\nfrom loudhailer.ext.channels import LoudhailerChannelLifespan\n\nasync def on_startup():\n    pass\n\n\nasync def on_shutdown():\n    pass\n\n\napplication = ProtocolTypeRouter(\n    {\n        'lifespan': LoudhailerChannelLifespan.as_asgi(\n            on_startup=on_startup, on_shutdown=on_shutdown,\n        ),\n        'websocket': URLRouter(...),\n    },\n)\n```\n\nPlease note that the **on_startup** and **on_shutdown** hooks can be implemented both as synchronous or asynchronous functions.\n\n\n## License\n\n`Loudhailer` is released under the [Apache License Version 2.0](https://www.apache.org/licenses/LICENSE-2.0).",
     'author': 'CloudBlue LLC',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://connect.cloudblue.com',
```

### Comparing `loudhailer-0.3.2/PKG-INFO` & `loudhailer-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loudhailer
-Version: 0.3.2
+Version: 0.3.3
 Summary: 
 Home-page: https://connect.cloudblue.com
 License: Apache-2.0
 Author: CloudBlue LLC
 Requires-Python: >=3.8,<4
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

