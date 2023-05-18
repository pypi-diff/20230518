# Comparing `tmp/moat-util-0.31.0.tar.gz` & `tmp/moat-util-0.35.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moat-util-0.31.0.tar", last modified: Thu Mar 23 17:00:33 2023, max compression
+gzip compressed data, was "moat-util-0.35.0.tar", last modified: Thu May 18 12:49:29 2023, max compression
```

## Comparing `moat-util-0.31.0.tar` & `moat-util-0.35.0.tar`

### file list

```diff
@@ -1,46 +1,50 @@
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-03-23 17:00:33.520761 moat-util-0.31.0/
--rw-r--r--   0 smurf      (501) smurf      (501)      436 2023-01-03 18:03:27.000000 moat-util-0.31.0/.gitignore
--rw-r--r--   0 smurf      (501) smurf      (501)      167 2023-01-03 18:03:27.000000 moat-util-0.31.0/LICENSE.txt
--rw-r--r--   0 smurf      (501) smurf      (501)      240 2023-01-03 18:03:27.000000 moat-util-0.31.0/Makefile
--rw-r--r--   0 smurf      (501) smurf      (501)     2544 2023-03-23 17:00:33.520761 moat-util-0.31.0/PKG-INFO
--rw-r--r--   0 smurf      (501) smurf      (501)     1521 2023-01-03 18:03:27.000000 moat-util-0.31.0/README.rst
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-03-23 17:00:33.516761 moat-util-0.31.0/moat/
--rw-r--r--   0 smurf      (501) smurf      (501)       65 2023-01-03 18:03:27.000000 moat-util-0.31.0/moat/__init__.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-03-23 17:00:33.516761 moat-util-0.31.0/moat/util/
--rw-r--r--   0 smurf      (501) smurf      (501)        0 2023-01-03 18:03:27.000000 moat-util-0.31.0/moat/util/.no_load
--rw-r--r--   0 smurf      (501) smurf      (501)     1982 2023-03-23 16:11:19.000000 moat-util-0.31.0/moat/util/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)     3782 2023-03-22 11:53:53.000000 moat-util-0.31.0/moat/util/_main.py
--rw-r--r--   0 smurf      (501) smurf      (501)     8126 2023-03-23 16:59:54.000000 moat-util-0.31.0/moat/util/alert.py
--rw-r--r--   0 smurf      (501) smurf      (501)      526 2023-02-24 18:19:03.000000 moat-util-0.31.0/moat/util/ctx.py
--rw-r--r--   0 smurf      (501) smurf      (501)     5836 2023-02-24 18:19:03.000000 moat-util-0.31.0/moat/util/dict.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2008 2023-02-24 18:19:03.000000 moat-util-0.31.0/moat/util/event.py
--rw-r--r--   0 smurf      (501) smurf      (501)     5713 2023-03-22 10:22:38.000000 moat-util-0.31.0/moat/util/impl.py
--rw-r--r--   0 smurf      (501) smurf      (501)    22480 2023-03-09 13:25:55.000000 moat-util-0.31.0/moat/util/main.py
--rw-r--r--   0 smurf      (501) smurf      (501)     3247 2023-02-24 18:19:03.000000 moat-util-0.31.0/moat/util/merge.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1920 2023-02-24 18:19:03.000000 moat-util-0.31.0/moat/util/module.py
--rw-r--r--   0 smurf      (501) smurf      (501)     3890 2023-02-24 18:19:03.000000 moat-util-0.31.0/moat/util/msg.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2127 2023-03-22 11:55:34.000000 moat-util-0.31.0/moat/util/msgpack.py
--rw-r--r--   0 smurf      (501) smurf      (501)    14884 2023-02-24 18:19:03.000000 moat-util-0.31.0/moat/util/path.py
--rw-r--r--   0 smurf      (501) smurf      (501)     9446 2023-03-23 08:43:37.000000 moat-util-0.31.0/moat/util/queue.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2126 2023-02-24 18:19:03.000000 moat-util-0.31.0/moat/util/server.py
--rw-r--r--   0 smurf      (501) smurf      (501)      584 2023-02-24 18:19:03.000000 moat-util-0.31.0/moat/util/spawn.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1750 2023-02-24 18:19:03.000000 moat-util-0.31.0/moat/util/systemd.py
--rw-r--r--   0 smurf      (501) smurf      (501)    16701 2023-03-10 18:03:30.000000 moat-util-0.31.0/moat/util/times.py
--rw-r--r--   0 smurf      (501) smurf      (501)     5436 2023-02-24 18:19:03.000000 moat-util-0.31.0/moat/util/yaml.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-03-23 17:00:33.520761 moat-util-0.31.0/moat_util.egg-info/
--rw-r--r--   0 smurf      (501) smurf      (501)     2544 2023-03-23 17:00:33.000000 moat-util-0.31.0/moat_util.egg-info/PKG-INFO
--rw-r--r--   0 smurf      (501) smurf      (501)      777 2023-03-23 17:00:33.000000 moat-util-0.31.0/moat_util.egg-info/SOURCES.txt
--rw-r--r--   0 smurf      (501) smurf      (501)        1 2023-03-23 17:00:33.000000 moat-util-0.31.0/moat_util.egg-info/dependency_links.txt
--rw-r--r--   0 smurf      (501) smurf      (501)      240 2023-03-23 17:00:33.000000 moat-util-0.31.0/moat_util.egg-info/requires.txt
--rw-r--r--   0 smurf      (501) smurf      (501)        5 2023-03-23 17:00:33.000000 moat-util-0.31.0/moat_util.egg-info/top_level.txt
--rw-r--r--   0 smurf      (501) smurf      (501)     2266 2023-03-23 16:33:37.000000 moat-util-0.31.0/pyproject.toml
--rw-r--r--   0 smurf      (501) smurf      (501)       38 2023-03-23 17:00:33.520761 moat-util-0.31.0/setup.cfg
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-03-23 17:00:33.520761 moat-util-0.31.0/tests/
--rw-r--r--   0 smurf      (501) smurf      (501)        0 2023-01-03 18:03:27.000000 moat-util-0.31.0/tests/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)      141 2023-03-22 10:04:54.000000 moat-util-0.31.0/tests/conftest.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1224 2023-03-23 16:54:24.000000 moat-util-0.31.0/tests/test_alerts.py
--rw-r--r--   0 smurf      (501) smurf      (501)      173 2023-01-03 18:03:27.000000 moat-util-0.31.0/tests/test_basic.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1034 2023-03-22 11:54:36.000000 moat-util-0.31.0/tests/test_broadcast.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1052 2023-01-03 18:03:27.000000 moat-util-0.31.0/tests/test_dict.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2929 2023-01-03 18:03:27.000000 moat-util-0.31.0/tests/test_path.py
--rw-r--r--   0 smurf      (501) smurf      (501)     4903 2023-03-10 18:03:30.000000 moat-util-0.31.0/tests/test_times.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 12:49:29.216625 moat-util-0.35.0/
+-rw-r--r--   0 smurf      (501) smurf      (501)      436 2023-05-18 12:49:20.000000 moat-util-0.35.0/.gitignore
+-rw-r--r--   0 smurf      (501) smurf      (501)      167 2022-09-12 09:54:59.000000 moat-util-0.35.0/LICENSE.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)      270 2023-05-18 12:46:39.000000 moat-util-0.35.0/Makefile
+-rw-r--r--   0 smurf      (501) smurf      (501)     2544 2023-05-18 12:49:29.216625 moat-util-0.35.0/PKG-INFO
+-rw-r--r--   0 smurf      (501) smurf      (501)     1521 2022-09-12 09:54:59.000000 moat-util-0.35.0/README.rst
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 12:49:29.212625 moat-util-0.35.0/moat/
+-rw-r--r--   0 smurf      (501) smurf      (501)      105 2023-05-18 12:46:39.000000 moat-util-0.35.0/moat/__init__.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 12:49:29.216625 moat-util-0.35.0/moat/util/
+-rw-r--r--   0 smurf      (501) smurf      (501)        0 2022-09-09 13:36:22.000000 moat-util-0.35.0/moat/util/.no_load
+-rw-r--r--   0 smurf      (501) smurf      (501)     2041 2023-05-18 12:46:39.000000 moat-util-0.35.0/moat/util/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     3782 2023-05-18 12:46:39.000000 moat-util-0.35.0/moat/util/_main.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     8118 2023-05-18 12:46:39.000000 moat-util-0.35.0/moat/util/alert.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     4931 2023-05-18 12:46:39.000000 moat-util-0.35.0/moat/util/broadcast.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     4824 2023-05-18 12:46:39.000000 moat-util-0.35.0/moat/util/compat.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      526 2023-02-17 16:33:58.000000 moat-util-0.35.0/moat/util/ctx.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     5840 2023-05-18 12:46:39.000000 moat-util-0.35.0/moat/util/dict.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2008 2023-02-17 16:33:58.000000 moat-util-0.35.0/moat/util/event.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     6324 2023-05-18 12:46:39.000000 moat-util-0.35.0/moat/util/impl.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    22787 2023-05-18 12:46:39.000000 moat-util-0.35.0/moat/util/main.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     3251 2023-05-18 12:46:39.000000 moat-util-0.35.0/moat/util/merge.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1920 2023-02-17 16:33:58.000000 moat-util-0.35.0/moat/util/module.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     3890 2023-02-17 16:33:58.000000 moat-util-0.35.0/moat/util/msg.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2962 2023-05-18 12:46:39.000000 moat-util-0.35.0/moat/util/msgpack.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    14884 2023-02-17 16:33:58.000000 moat-util-0.35.0/moat/util/path.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2318 2023-05-18 12:46:39.000000 moat-util-0.35.0/moat/util/proxy.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     5578 2023-05-18 12:46:39.000000 moat-util-0.35.0/moat/util/queue.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2126 2023-02-17 16:33:58.000000 moat-util-0.35.0/moat/util/server.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      584 2023-02-17 16:33:58.000000 moat-util-0.35.0/moat/util/spawn.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1750 2023-02-17 16:33:58.000000 moat-util-0.35.0/moat/util/systemd.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    16701 2023-05-18 12:46:39.000000 moat-util-0.35.0/moat/util/times.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     5436 2023-02-17 16:33:58.000000 moat-util-0.35.0/moat/util/yaml.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 12:49:29.216625 moat-util-0.35.0/moat_util.egg-info/
+-rw-r--r--   0 smurf      (501) smurf      (501)     2544 2023-05-18 12:49:29.000000 moat-util-0.35.0/moat_util.egg-info/PKG-INFO
+-rw-r--r--   0 smurf      (501) smurf      (501)      861 2023-05-18 12:49:29.000000 moat-util-0.35.0/moat_util.egg-info/SOURCES.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)        1 2023-05-18 12:49:29.000000 moat-util-0.35.0/moat_util.egg-info/dependency_links.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)      240 2023-05-18 12:49:29.000000 moat-util-0.35.0/moat_util.egg-info/requires.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)        5 2023-05-18 12:49:29.000000 moat-util-0.35.0/moat_util.egg-info/top_level.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)     2266 2023-05-18 12:49:20.000000 moat-util-0.35.0/pyproject.toml
+-rw-r--r--   0 smurf      (501) smurf      (501)       38 2023-05-18 12:49:29.216625 moat-util-0.35.0/setup.cfg
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 12:49:29.216625 moat-util-0.35.0/tests/
+-rw-r--r--   0 smurf      (501) smurf      (501)        0 2022-09-19 15:23:20.000000 moat-util-0.35.0/tests/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      141 2023-05-18 12:46:39.000000 moat-util-0.35.0/tests/conftest.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1224 2023-05-18 12:46:39.000000 moat-util-0.35.0/tests/test_alerts.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      173 2022-09-16 05:43:11.000000 moat-util-0.35.0/tests/test_basic.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1044 2023-05-18 12:46:39.000000 moat-util-0.35.0/tests/test_broadcast.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1052 2022-10-13 12:19:12.000000 moat-util-0.35.0/tests/test_dict.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      795 2023-05-18 12:46:39.000000 moat-util-0.35.0/tests/test_msgpack.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2929 2022-09-16 05:43:11.000000 moat-util-0.35.0/tests/test_path.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     4903 2023-05-18 12:46:39.000000 moat-util-0.35.0/tests/test_times.py
```

### Comparing `moat-util-0.31.0/PKG-INFO` & `moat-util-0.35.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moat-util
-Version: 0.31.0
+Version: 0.35.0
 Summary: Utility code for the rest of MoaT
 Author-email: Matthias Urlichs <matthias@urlichs.de>
 License: The code in this repository is part of the MoaT project.
         
         The licensing information in the moat-main repository at
         https://github.com/M-o-a-T/moat-main is applicable.
```

### Comparing `moat-util-0.31.0/README.rst` & `moat-util-0.35.0/README.rst`

 * *Files identical despite different names*

### Comparing `moat-util-0.31.0/moat/util/__init__.py` & `moat-util-0.35.0/moat/util/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 
 # pylint: disable=cyclic-import,wrong-import-position
 
 import logging as _logging
 
 _log = _logging.getLogger(__name__)
 
+from .alert import *  # noqa: F401,F403,E402  # isort:skip
 from .impl import *  # noqa: F401,F403,E402  # isort:skip
 from .dict import *  # noqa: F401,F403,E402  # isort:skip
 from .merge import *  # noqa: F401,F403,E402  # isort:skip
-from .alert import *  # noqa: F401,F403,E402  # isort:skip
+from .proxy import *  # noqa: F401,F403,E402  # isort:skip
 
 try:
     from .event import *  # noqa: F401,F403
 except ImportError as exc:
     _log.warning("Missing: %s", exc)
 
 try:
```

### Comparing `moat-util-0.31.0/moat/util/_main.py` & `moat-util-0.35.0/moat/util/_main.py`

 * *Files identical despite different names*

### Comparing `moat-util-0.31.0/moat/util/alert.py` & `moat-util-0.35.0/moat/util/alert.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,27 +6,23 @@
 Waiting will succeed when the alarm is resolved/closed.
 Iterating will receive new state and end when the alert is resolved.
 
 The dispatcher is a context manager that can be iterated to receive new
 alerts.
 """
 
-import logging
 from contextlib import asynccontextmanager
 
-import anyio
-
+from .broadcast import Broadcaster, BroadcastReader
+from .compat import Event, TaskGroup
 from .ctx import CtxObj
-from .queue import Broadcaster, BroadcastReader
-
-logger = logging.getLogger(__name__)
 
 __all__ = [
-    "BaseAlert",
     "Alert",
+    "BaseAlert",
     "RepeatAlert",
     "AlertHandler",
     "AlertMixin",
     "AlertCollector",
 ]
 
 
@@ -43,19 +39,19 @@
 
     The iterator terminates when the condition has passed.
 
     Intended use: subclass this, distribute using an AlarmHandler mix-in.
     """
 
     state: list = None
-    evt: anyio.Event = None
+    evt: Event = None
 
     def __init__(self, *data):
         super().__init__(*data)
-        self.evt = anyio.Event()
+        self.evt = Event()
         self.q = Broadcaster()
         self.q.__enter__()
         self.set(data)
 
     def __aiter__(self):
         return self.q.__aiter__()
 
@@ -227,15 +223,16 @@
         """
         self._alerts.raise_(cls, *msg)
 
 
 class AlertCollector(CtxObj):
     """
     This context manager stores a variety of alerts, or in fact any other
-    object that can be ``await``ed.
+    object that can be ``await``ed. It is basically the read-side
+    counterpart of an `AlertHandler`.
 
     Awaiting it will delay until all alerts that have been fed to it are
     resolved.
 
     If the object itself needs to be awaited, or a function other than
     ``wait``, set @access to an appropriate Lambda:
 
@@ -245,16 +242,16 @@
     _tg = None
     _working = None
 
     def __init__(self, access=lambda x: x.wait()):
         self.objs = set()
         self.access = access
 
-        self.non_empty = anyio.Event()
-        self.evt = anyio.Event()
+        self.non_empty = Event()
+        self.evt = Event()
         self.evt.set()
 
     # if non_empty is not None:
     #    .evt is set
     #    the system is idle.
     # otherwise
     #    .evt is not set
@@ -287,15 +284,15 @@
                     self.objs.add(w)
                     raise
                 finally:
                     self._working = None
             else:
                 self.evt.set()
                 if self.non_empty is None:
-                    self.non_empty = anyio.Event()
+                    self.non_empty = Event()
                 await self.non_empty.wait()
                 self.non_empty = None
 
     async def wait_busy(self):
         """
         wait until an alert has been raised.
         """
@@ -310,18 +307,18 @@
         May be spuriously positive if the internal task is slow, or not
         running.
         """
         return self.non_empty is None
 
     @asynccontextmanager
     async def _ctx(self):
-        async with anyio.create_task_group() as self._tg:
+        async with TaskGroup() as self._tg:
             self._tg.start_soon(self._runner)
             yield self
             self._tg.cancel_scope.cancel()
 
     def add(self, thing):
         """Wait for this event."""
         if self.non_empty is not None:
-            self.evt = anyio.Event()
+            self.evt = Event()
             self.non_empty.set()
         self.objs.add(thing)
```

### Comparing `moat-util-0.31.0/moat/util/ctx.py` & `moat-util-0.35.0/moat/util/ctx.py`

 * *Files identical despite different names*

### Comparing `moat-util-0.31.0/moat/util/dict.py` & `moat-util-0.35.0/moat/util/dict.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 This module contains various helper functions and classes.
 """
 from copy import deepcopy
 from typing import Mapping, Tuple, Union
 
-from . import NotGiven
+from .impl import NotGiven
 
 __all__ = ["combine_dict", "drop_dict", "attrdict", "to_attrdict"]
 
 
 def combine_dict(*d, cls=dict, deep=False) -> dict:
     """
     Returns a dict with all keys+values of all dict arguments.
```

### Comparing `moat-util-0.31.0/moat/util/event.py` & `moat-util-0.35.0/moat/util/event.py`

 * *Files identical despite different names*

### Comparing `moat-util-0.31.0/moat/util/impl.py` & `moat-util-0.35.0/moat/util/impl.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,70 @@
 """
 This module contains various helper functions and classes.
 """
 import logging
 import sys
 from collections import deque
+from contextlib import nullcontext
 from getpass import getpass
 from math import log10
 
 __all__ = [
     "NoneType",
     "singleton",
     "TimeOnlyFormatter",
     "NotGiven",
     "count",
     "acount",
     "Cache",
     "NoLock",
+    "OptCtx",
     "digits",
     "num2byte",
     "byte2num",
     "split_arg",
     "id36",
     "import_",
     "load_from_cfg",
 ]
 
 NoneType = type(None)
 
+NoLock = nullcontext()
+
+
+class OptCtx:
+    """
+    Optional context. Unlike `contextlib.nullcontext` this doesn't return a
+    fixed value; instead it delegates to the wrapped context manager – if
+    there is one.
+    """
+
+    def __init__(self, obj=None):
+        self.obj = obj
+
+    def __enter__(self):
+        if self.obj is not None:
+            return self.obj.__enter__()
+        return None
+
+    def __exit__(self, *tb):
+        if self.obj is not None:
+            return self.obj.__exit__(*tb)
+        return None
+
+    async def __aenter__(self):
+        if self.obj is not None:
+            return await self.obj.__aenter__()
+        return None
+
+    async def __aexit__(self, *tb):
+        if self.obj is not None:
+            return await self.obj.__aexit__(*tb)
+
 
 def import_(name, off=0):
     """
     Import a module and access an object in it.
 
     `import_("a.b.c.d.e", 2)` imports "a.b.c" and returns the e attribute
     of object d from it.
@@ -43,25 +77,27 @@
             res = getattr(res, nn)
     except Exception as exc:
         sys.modules.pop(mn, None)
         raise exc
     return res
 
 
-def load_from_cfg(cfg, *a, _attr="server", **k):
+def load_from_cfg(cfg, *a, _attr="server", _raise=False, **k):
     """
     A simple frontend to load a module, access a class/object from it,
     and call that with the config (and whchever other arguments you want to
     use).
 
     The module+object name is the "server" attribute (or @_attr).
     """
     try:
         name = cfg[_attr]
     except KeyError:
+        if _raise:
+            raise
         return None
     if isinstance(name, (list, tuple)):
         name, off = name
     else:
         off = 1
     m = import_(name, off=off)
     return m(cfg, *a, **k)
@@ -149,31 +185,14 @@
     def clear(self):
         """Clear the cache"""
         while self._head > self._tail:
             self._q.popleft()
             self._tail += 1
 
 
-@singleton
-class NoLock:
-    """A dummy singleton that can replace a lock.
-
-    Usage::
-
-        with NoLock if _locked else self._lock:
-            pass
-    """
-
-    async def __aenter__(self):
-        return self
-
-    async def __aexit__(self, *tb):
-        return
-
-
 def digits(n, digits=6):  # pylint: disable=redefined-outer-name
     """
     Returns ``n`` rounded to ``digits`` significant digits. Default: 6.
     Ensures that the number doesn't carry nonsense precision or
     floating-point artefacts.
 
     >>> digits(123456789, 4)
```

### Comparing `moat-util-0.31.0/moat/util/main.py` & `moat-util-0.35.0/moat/util/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,17 +229,18 @@
     path = name.split(".")
     path.extend(attr[:-1])
     dp = ".".join(path)
     dpe = ".".join(path[:-1])
     try:
         mod = importlib.import_module(dp)
     except (ModuleNotFoundError, FileNotFoundError) as exc:
-        logger.debug("Err %s: %r", dp, exc)
         if err:
             raise
+        if err is not None:
+            logger.debug("Err %s: %r", dp, exc)
         if (
             exc.name != dp
             and exc.name != dpe
             and not exc.name.startswith(f"{dp}._")  # pylint: disable=no-member ## duh?
         ):
             raise
         return None
@@ -256,21 +257,19 @@
         return mod
 
 
 def load_cfg(name):
     """
     Load a module's configuration
     """
-    cf = {}
-    try:
-        try:
-            cf = load_ext(name, "_config", "CFG", err=True)
-        except ModuleNotFoundError:
-            cf = load_ext(name, "config", "CFG", err=True)
-    except ModuleNotFoundError:
+    cf = load_ext(name, "_config", "CFG", err=None)
+    if cf is None:
+        cf = load_ext(name, "config", "CFG", err=None)
+    if cf is None:
+        cf = {}
         ext = sys.modules[name]
         try:
             p = ext.__path__
         except AttributeError:
             p = (str(Path(ext.__file__).parent),)
         for d in p:
             fn = Path(d) / "_config.yaml"
@@ -281,19 +280,21 @@
 
 def _namespaces(name):
     import pkgutil  # pylint: disable=import-outside-toplevel
 
     try:
         ext = importlib.import_module(name)
     except ModuleNotFoundError:
+        logger.debug("No NS: %s", name)
         return ()
     try:
         p = ext.__path__
     except AttributeError:
         p = (str(Path(ext.__file__).parent),)
+    logger.debug("NS: %s %s", name, p)
     return pkgutil.iter_modules(p, ext.__name__ + ".")
 
 
 _ext_cache = defaultdict(dict)
 
 
 def _cache_ext(ext_name, pkg_only):
@@ -301,15 +302,17 @@
 
     Yields (name,path) tuples.
 
     TODO: This is not zip safe.
     """
     for finder, name, ispkg in _namespaces(ext_name):
         if pkg_only and not ispkg:
+            logger.debug("ExtNoC %s", name)
             continue
+        logger.debug("ExtC %s", name)
         x = name.rsplit(".", 1)[-1]
         f = Path(finder.path) / x
         _ext_cache[ext_name][x] = f
 
 
 def list_ext(name, func=None, pkg_only=True):
     """List external modules
@@ -731,15 +734,19 @@
         else:
             try:
                 v = path_eval(v)
             except Exception:  # pylint: disable=broad-except
                 pass
         obj.cfg._update(P(k), v)  # pylint: disable=protected-access
 
-    if not wrap:
+    if wrap:
+        pass
+    elif logging.root.handlers:
+        logging.debug("Logging already set up")
+    else:
         # Configure logging. This is a somewhat arcane art.
         lcfg = obj.cfg.setdefault("logging", dict())
         lcfg.setdefault("version", 1)
         lcfg.setdefault("root", dict())["level"] = (
             "DEBUG"
             if verbose > 2
             else "INFO"
@@ -752,14 +759,16 @@
             k, v = k.split("=")
             lcfg["loggers"].setdefault(k, {})["level"] = v
         dictConfig(lcfg)
         logging.captureWarnings(verbose > 0)
         logger.disabled = False
         if debug_loader:
             logger.level = logging.DEBUG
+            for p in sys.path:
+                logger.debug("Path: %s", p)
 
     obj.logger = logging.getLogger(name)
 
     try:
         # pylint: disable=no-value-for-parameter,unexpected-keyword-arg
         # NOTE this return an awaitable
         if ctx is not None:
```

### Comparing `moat-util-0.31.0/moat/util/merge.py` & `moat-util-0.35.0/moat/util/merge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __all__ = ["merge"]
 
 
-from . import NotGiven
+from .impl import NotGiven
 
 
 def _merge_dict(d, other, drop=False, replace=True):
     for key, value in other.items():
         if value is NotGiven:
             d.pop(key, None)
         elif key in d:
```

### Comparing `moat-util-0.31.0/moat/util/module.py` & `moat-util-0.35.0/moat/util/module.py`

 * *Files identical despite different names*

### Comparing `moat-util-0.31.0/moat/util/msg.py` & `moat-util-0.35.0/moat/util/msg.py`

 * *Files identical despite different names*

### Comparing `moat-util-0.31.0/moat/util/msgpack.py` & `moat-util-0.35.0/moat/util/msgpack.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,57 +10,85 @@
 
 from functools import partial
 
 import msgpack
 
 from .dict import attrdict
 from .path import Path
+from .proxy import Proxy, _CProxy, obj2name
 
-__all__ = ["packer", "unpacker", "stream_unpacker", "Proxy", "NoProxyError"]
-
-
-class Proxy:
-    """
-    A proxy object, i.e. a placeholder for things that cannot pass through MsgPack.
-    """
-
-    def __init__(self, name):
-        self.name = name
-
-    def __repr__(self):
-        return f"{self.__class__.__name__}({self.name !r})"
-
-
-class NoProxyError(ValueError):
-    "Error for nonexistent proxy values"
-    pass  # pylint:disable=unnecessary-pass
+__all__ = ["packer", "unpacker", "stream_unpacker"]
 
 
 def _encode(data):
     if isinstance(data, int) and data >= 1 << 64:
+        # bignum
         return msgpack.ExtType(2, data.to_bytes((data.bit_length() + 7) // 8, "big"))
-    elif isinstance(data, Path):
+    if isinstance(data, Path):
+        # Path
         return msgpack.ExtType(3, b"".join(packer(x) for x in data))
-    elif isinstance(data, Proxy):
+    if isinstance(data, Proxy):
+        # Proxy object
         return msgpack.ExtType(4, data.name.encode("utf-8"))
+    if isinstance(data, Proxy):
+        # proxy class
+        return msgpack.ExtType(5, packer(data.name) + b"".join(packer(x) for x in data.data))
+    try:
+        name = obj2name(data)
+    except KeyError:
+        pass
+    else:
+        return msgpack.ExtType(4, name.encode("utf-8"))
+
+    try:
+        name = obj2name(type(data))
+    except KeyError:
+        pass
+    else:
+        p = data.__getstate__()
+        if not isinstance(p, (list, tuple)):
+            p = (p,)
+        return msgpack.ExtType(5, packer(name) + b"".join(packer(x) for x in p))
+
+    # XXX we crash instead of sending an unnamed proxy
+    # TODO sending a proxied object a second time will build a new one
     return data
 
 
 def _decode(code, data):
     if code == 2:
         return int.from_bytes(data, "big")
     elif code == 3:
         s = stream_unpacker()
         s.feed(data)
         return Path(*s)
     elif code == 4:
         try:
-            return Proxy(data.decode("utf-8"))
+            n = data.decode("utf-8")
         except UnicodeDecodeError:
-            return Proxy(str(data))
+            n = str(data)
+        try:
+            return _CProxy[n]
+        except KeyError:
+            return Proxy(n)
+    elif code == 5:
+        s = stream_unpacker()
+        s.feed(data)
+        s = iter(s)
+        pk = next(s)
+        try:
+            pk = _CProxy[pk]
+        except KeyError:
+            pk = partial(Proxy, pk)
+        pk = object.__new__(pk)
+        try:
+            pk.__setstate__(*s)
+        except AttributeError:
+            pk.__dict__.update(next(s))
+        return pk
     return msgpack.ExtType(code, data)
 
 
 # single message packer
 packer = partial(msgpack.packb, strict_types=False, use_bin_type=True, default=_encode)
 
 # single message unpacker
```

### Comparing `moat-util-0.31.0/moat/util/path.py` & `moat-util-0.35.0/moat/util/path.py`

 * *Files identical despite different names*

### Comparing `moat-util-0.31.0/moat/util/server.py` & `moat-util-0.35.0/moat/util/server.py`

 * *Files identical despite different names*

### Comparing `moat-util-0.31.0/moat/util/spawn.py` & `moat-util-0.35.0/moat/util/spawn.py`

 * *Files identical despite different names*

### Comparing `moat-util-0.31.0/moat/util/systemd.py` & `moat-util-0.35.0/moat/util/systemd.py`

 * *Files identical despite different names*

### Comparing `moat-util-0.31.0/moat/util/times.py` & `moat-util-0.35.0/moat/util/times.py`

 * *Files identical despite different names*

### Comparing `moat-util-0.31.0/moat/util/yaml.py` & `moat-util-0.35.0/moat/util/yaml.py`

 * *Files identical despite different names*

### Comparing `moat-util-0.31.0/moat_util.egg-info/PKG-INFO` & `moat-util-0.35.0/moat_util.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moat-util
-Version: 0.31.0
+Version: 0.35.0
 Summary: Utility code for the rest of MoaT
 Author-email: Matthias Urlichs <matthias@urlichs.de>
 License: The code in this repository is part of the MoaT project.
         
         The licensing information in the moat-main repository at
         https://github.com/M-o-a-T/moat-main is applicable.
```

### Comparing `moat-util-0.31.0/moat_util.egg-info/SOURCES.txt` & `moat-util-0.35.0/moat_util.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -4,24 +4,27 @@
 README.rst
 pyproject.toml
 moat/__init__.py
 moat/util/.no_load
 moat/util/__init__.py
 moat/util/_main.py
 moat/util/alert.py
+moat/util/broadcast.py
+moat/util/compat.py
 moat/util/ctx.py
 moat/util/dict.py
 moat/util/event.py
 moat/util/impl.py
 moat/util/main.py
 moat/util/merge.py
 moat/util/module.py
 moat/util/msg.py
 moat/util/msgpack.py
 moat/util/path.py
+moat/util/proxy.py
 moat/util/queue.py
 moat/util/server.py
 moat/util/spawn.py
 moat/util/systemd.py
 moat/util/times.py
 moat/util/yaml.py
 moat_util.egg-info/PKG-INFO
@@ -31,9 +34,10 @@
 moat_util.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
 tests/test_alerts.py
 tests/test_basic.py
 tests/test_broadcast.py
 tests/test_dict.py
+tests/test_msgpack.py
 tests/test_path.py
 tests/test_times.py
```

### Comparing `moat-util-0.31.0/pyproject.toml` & `moat-util-0.35.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `moat-util-0.31.0/tests/test_alerts.py` & `moat-util-0.35.0/tests/test_alerts.py`

 * *Files identical despite different names*

### Comparing `moat-util-0.31.0/tests/test_broadcast.py` & `moat-util-0.35.0/tests/test_broadcast.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 # pylint: disable=missing-function-docstring
 
 import anyio
 import pytest
 
-from moat.util import Broadcaster, LostData
+from moat.util.broadcast import Broadcaster, LostData
 
 
 @pytest.mark.anyio
 async def test_basic():
     seen = [0, 0, 0]
 
     async def a(b, n):
```

### Comparing `moat-util-0.31.0/tests/test_dict.py` & `moat-util-0.35.0/tests/test_dict.py`

 * *Files identical despite different names*

### Comparing `moat-util-0.31.0/tests/test_path.py` & `moat-util-0.35.0/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `moat-util-0.31.0/tests/test_times.py` & `moat-util-0.35.0/tests/test_times.py`

 * *Files identical despite different names*

