# Comparing `tmp/interval_sdk-1.2.0.tar.gz` & `tmp/interval_sdk-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interval_sdk-1.2.0.tar", max compression
+gzip compressed data, was "interval_sdk-1.3.0.tar", max compression
```

## Comparing `interval_sdk-1.2.0.tar` & `interval_sdk-1.3.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     5078 2023-05-02 17:56:21.969548 interval_sdk-1.2.0/README.md
--rw-r--r--   0        0        0     1890 2023-05-03 17:16:14.766804 interval_sdk-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      331 2023-02-09 22:23:52.943201 interval_sdk-1.2.0/src/interval_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-02-09 22:23:52.943201 interval_sdk-1.2.0/src/interval_sdk/classes/__init__.py
--rw-r--r--   0        0        0      422 2023-02-09 22:23:52.943201 interval_sdk-1.2.0/src/interval_sdk/classes/action.py
--rw-r--r--   0        0        0     7151 2023-05-02 17:56:24.302863 interval_sdk-1.2.0/src/interval_sdk/classes/component.py
--rw-r--r--   0        0        0      931 2023-02-09 22:23:52.943201 interval_sdk-1.2.0/src/interval_sdk/classes/interval_file.py
--rw-r--r--   0        0        0    60224 2023-05-02 17:56:24.302863 interval_sdk-1.2.0/src/interval_sdk/classes/io.py
--rw-r--r--   0        0        0     8178 2023-05-02 17:56:24.302863 interval_sdk-1.2.0/src/interval_sdk/classes/io_client.py
--rw-r--r--   0        0        0      348 2023-02-09 22:23:52.943201 interval_sdk-1.2.0/src/interval_sdk/classes/io_error.py
--rw-r--r--   0        0        0    35098 2023-04-20 18:40:02.493885 interval_sdk-1.2.0/src/interval_sdk/classes/io_promise.py
--rw-r--r--   0        0        0     7891 2023-04-24 17:19:39.837392 interval_sdk-1.2.0/src/interval_sdk/classes/isocket.py
--rw-r--r--   0        0        0     1162 2023-05-02 17:56:24.302863 interval_sdk-1.2.0/src/interval_sdk/classes/layout.py
--rw-r--r--   0        0        0     3458 2023-02-09 22:23:52.943201 interval_sdk-1.2.0/src/interval_sdk/classes/logger.py
--rw-r--r--   0        0        0     2993 2023-02-09 22:23:52.943201 interval_sdk-1.2.0/src/interval_sdk/classes/page.py
--rw-r--r--   0        0        0     6155 2023-04-24 17:19:39.837392 interval_sdk-1.2.0/src/interval_sdk/classes/rpc.py
--rw-r--r--   0        0        0     2968 2023-03-27 15:09:45.572798 interval_sdk-1.2.0/src/interval_sdk/classes/transaction_loading_state.py
--rw-r--r--   0        0        0        0 2023-02-09 22:23:52.943201 interval_sdk-1.2.0/src/interval_sdk/components/__init__.py
--rw-r--r--   0        0        0     1704 2023-02-09 22:23:52.943201 interval_sdk-1.2.0/src/interval_sdk/components/grid.py
--rw-r--r--   0        0        0     6173 2023-04-24 17:47:34.117311 interval_sdk-1.2.0/src/interval_sdk/components/table.py
--rw-r--r--   0        0        0      810 2023-04-20 18:40:02.493885 interval_sdk-1.2.0/src/interval_sdk/handlers.py
--rw-r--r--   0        0        0    15318 2023-05-02 17:56:21.969548 interval_sdk-1.2.0/src/interval_sdk/internal_rpc_schema.py
--rw-r--r--   0        0        0    25838 2023-05-02 17:56:24.302863 interval_sdk-1.2.0/src/interval_sdk/io_schema.py
--rw-r--r--   0        0        0    65727 2023-05-02 17:56:21.969548 interval_sdk-1.2.0/src/interval_sdk/main.py
--rw-r--r--   0        0        0       41 2023-02-09 22:23:52.943201 interval_sdk-1.2.0/src/interval_sdk/superjson/__init__.py
--rw-r--r--   0        0        0     1081 2023-02-09 22:23:52.943201 interval_sdk-1.2.0/src/interval_sdk/superjson/main.py
--rw-r--r--   0        0        0     3810 2023-02-09 22:23:52.943201 interval_sdk-1.2.0/src/interval_sdk/superjson/plainer.py
--rw-r--r--   0        0        0        0 2023-02-09 22:23:52.943201 interval_sdk-1.2.0/src/interval_sdk/superjson/tests/__init__.py
--rw-r--r--   0        0        0      188 2023-02-09 22:23:52.943201 interval_sdk-1.2.0/src/interval_sdk/superjson/tests/node-only-types.js
--rw-r--r--   0        0        0      416 2023-02-09 22:23:52.943201 interval_sdk-1.2.0/src/interval_sdk/superjson/tests/round-trip-superjson.js
--rw-r--r--   0        0        0     3385 2023-02-09 22:23:52.943201 interval_sdk-1.2.0/src/interval_sdk/superjson/tests/test_superjson.py
--rw-r--r--   0        0        0     5935 2023-05-02 17:56:24.302863 interval_sdk-1.2.0/src/interval_sdk/superjson/transformer.py
--rw-r--r--   0        0        0     4550 2023-04-28 17:09:46.534136 interval_sdk-1.2.0/src/interval_sdk/types.py
--rw-r--r--   0        0        0     7342 2023-05-02 17:56:24.302863 interval_sdk-1.2.0/src/interval_sdk/util.py
--rw-r--r--   0        0        0     6318 1970-01-01 00:00:00.000000 interval_sdk-1.2.0/setup.py
--rw-r--r--   0        0        0     6161 1970-01-01 00:00:00.000000 interval_sdk-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     5078 2023-05-02 17:56:21.969548 interval_sdk-1.3.0/README.md
+-rw-r--r--   0        0        0     1890 2023-05-17 19:40:55.424837 interval_sdk-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      331 2023-02-09 22:23:52.943201 interval_sdk-1.3.0/src/interval_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-09 22:23:52.943201 interval_sdk-1.3.0/src/interval_sdk/classes/__init__.py
+-rw-r--r--   0        0        0      422 2023-02-09 22:23:52.943201 interval_sdk-1.3.0/src/interval_sdk/classes/action.py
+-rw-r--r--   0        0        0     7151 2023-05-02 17:56:24.302863 interval_sdk-1.3.0/src/interval_sdk/classes/component.py
+-rw-r--r--   0        0        0      931 2023-02-09 22:23:52.943201 interval_sdk-1.3.0/src/interval_sdk/classes/interval_file.py
+-rw-r--r--   0        0        0    60224 2023-05-02 17:56:24.302863 interval_sdk-1.3.0/src/interval_sdk/classes/io.py
+-rw-r--r--   0        0        0     8178 2023-05-02 17:56:24.302863 interval_sdk-1.3.0/src/interval_sdk/classes/io_client.py
+-rw-r--r--   0        0        0      348 2023-02-09 22:23:52.943201 interval_sdk-1.3.0/src/interval_sdk/classes/io_error.py
+-rw-r--r--   0        0        0    35098 2023-04-20 18:40:02.493885 interval_sdk-1.3.0/src/interval_sdk/classes/io_promise.py
+-rw-r--r--   0        0        0     8059 2023-05-17 19:37:58.452814 interval_sdk-1.3.0/src/interval_sdk/classes/isocket.py
+-rw-r--r--   0        0        0     1162 2023-05-02 17:56:24.302863 interval_sdk-1.3.0/src/interval_sdk/classes/layout.py
+-rw-r--r--   0        0        0     3458 2023-02-09 22:23:52.943201 interval_sdk-1.3.0/src/interval_sdk/classes/logger.py
+-rw-r--r--   0        0        0     2993 2023-02-09 22:23:52.943201 interval_sdk-1.3.0/src/interval_sdk/classes/page.py
+-rw-r--r--   0        0        0     6155 2023-04-24 17:19:39.837392 interval_sdk-1.3.0/src/interval_sdk/classes/rpc.py
+-rw-r--r--   0        0        0     2968 2023-03-27 15:09:45.572798 interval_sdk-1.3.0/src/interval_sdk/classes/transaction_loading_state.py
+-rw-r--r--   0        0        0        0 2023-02-09 22:23:52.943201 interval_sdk-1.3.0/src/interval_sdk/components/__init__.py
+-rw-r--r--   0        0        0     1704 2023-02-09 22:23:52.943201 interval_sdk-1.3.0/src/interval_sdk/components/grid.py
+-rw-r--r--   0        0        0     6173 2023-04-24 17:47:34.117311 interval_sdk-1.3.0/src/interval_sdk/components/table.py
+-rw-r--r--   0        0        0      810 2023-04-20 18:40:02.493885 interval_sdk-1.3.0/src/interval_sdk/handlers.py
+-rw-r--r--   0        0        0    15318 2023-05-02 17:56:21.969548 interval_sdk-1.3.0/src/interval_sdk/internal_rpc_schema.py
+-rw-r--r--   0        0        0    25838 2023-05-02 17:56:24.302863 interval_sdk-1.3.0/src/interval_sdk/io_schema.py
+-rw-r--r--   0        0        0    65934 2023-05-17 19:37:58.452814 interval_sdk-1.3.0/src/interval_sdk/main.py
+-rw-r--r--   0        0        0       41 2023-02-09 22:23:52.943201 interval_sdk-1.3.0/src/interval_sdk/superjson/__init__.py
+-rw-r--r--   0        0        0     1081 2023-02-09 22:23:52.943201 interval_sdk-1.3.0/src/interval_sdk/superjson/main.py
+-rw-r--r--   0        0        0     3810 2023-02-09 22:23:52.943201 interval_sdk-1.3.0/src/interval_sdk/superjson/plainer.py
+-rw-r--r--   0        0        0        0 2023-02-09 22:23:52.943201 interval_sdk-1.3.0/src/interval_sdk/superjson/tests/__init__.py
+-rw-r--r--   0        0        0      188 2023-02-09 22:23:52.943201 interval_sdk-1.3.0/src/interval_sdk/superjson/tests/node-only-types.js
+-rw-r--r--   0        0        0      416 2023-02-09 22:23:52.943201 interval_sdk-1.3.0/src/interval_sdk/superjson/tests/round-trip-superjson.js
+-rw-r--r--   0        0        0     3385 2023-02-09 22:23:52.943201 interval_sdk-1.3.0/src/interval_sdk/superjson/tests/test_superjson.py
+-rw-r--r--   0        0        0     5935 2023-05-02 17:56:24.302863 interval_sdk-1.3.0/src/interval_sdk/superjson/transformer.py
+-rw-r--r--   0        0        0     4550 2023-04-28 17:09:46.534136 interval_sdk-1.3.0/src/interval_sdk/types.py
+-rw-r--r--   0        0        0     7342 2023-05-02 17:56:24.302863 interval_sdk-1.3.0/src/interval_sdk/util.py
+-rw-r--r--   0        0        0     6318 1970-01-01 00:00:00.000000 interval_sdk-1.3.0/setup.py
+-rw-r--r--   0        0        0     6161 1970-01-01 00:00:00.000000 interval_sdk-1.3.0/PKG-INFO
```

### Comparing `interval_sdk-1.2.0/README.md` & `interval_sdk-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.2.0/pyproject.toml` & `interval_sdk-1.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "interval-sdk"
-version = "1.2.0"
+version = "1.3.0"
 description = "The frontendless framework for high growth companies. Interval automatically generates apps by inlining the UI in your backend code. It's a faster and more maintainable way to build internal tools, rapid prototypes, and more."
 authors = [
 	"Jacob Mischka <jacob@interval.com>",
 	"Ryan Coppolo <ryan@interval.com>",
 ]
 maintainers = [
 	"Jacob Mischka <jacob@interval.com>",
```

### Comparing `interval_sdk-1.2.0/src/interval_sdk/classes/component.py` & `interval_sdk-1.3.0/src/interval_sdk/classes/component.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.2.0/src/interval_sdk/classes/interval_file.py` & `interval_sdk-1.3.0/src/interval_sdk/classes/interval_file.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.2.0/src/interval_sdk/classes/io.py` & `interval_sdk-1.3.0/src/interval_sdk/classes/io.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.2.0/src/interval_sdk/classes/io_client.py` & `interval_sdk-1.3.0/src/interval_sdk/classes/io_client.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.2.0/src/interval_sdk/classes/io_promise.py` & `interval_sdk-1.3.0/src/interval_sdk/classes/io_promise.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.2.0/src/interval_sdk/classes/isocket.py` & `interval_sdk-1.3.0/src/interval_sdk/classes/isocket.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     pass
 
 
 class ISocket:
     _logger: Logger
     _ws: websockets.client.WebSocketClientProtocol
     _send_timeout: float
+    _ping_timeout: float
     _connect_timeout: float
     _is_authenticated: bool
 
     id: UUID
     on_message: Optional[Callable[[str], Awaitable[None]]]
     on_open: Optional[Callable[[], Awaitable[None]]]
     on_error: Optional[Callable[[Exception], Awaitable[None]]]
@@ -51,27 +52,29 @@
     _num_producers: int
 
     def __init__(
         self,
         ws: websockets.client.WebSocketClientProtocol,
         id: Optional[UUID] = None,
         send_timeout: float = 5,
+        ping_timeout: float = 5,
         connect_timeout: float = 10,
         on_message: Optional[Callable[[str], Awaitable[None]]] = None,
         on_open: Optional[Callable[[], Awaitable[None]]] = None,
         on_error: Optional[Callable[[Exception], Awaitable[None]]] = None,
         on_close: Optional[Callable[[int, str], Awaitable[None]]] = None,
         log_level: Optional[LogLevel] = None,
         num_producers: int = 1,
     ):
         self._logger = Logger(log_level=log_level, prefix=self.__class__.__name__)
         self._ws = ws
         self.id = id if id is not None else uuid4()
         self._send_timeout = send_timeout
         self._connect_timeout = connect_timeout
+        self._ping_timeout = ping_timeout
         self.is_closed = False
 
         self.on_message = on_message
         self.on_open = on_open
         self.on_error = on_error
         self.on_close = on_close
 
@@ -224,9 +227,12 @@
             raise NotConnectedError
 
         if self._ws is None:
             raise NotConnectedError
 
         # start the ping
         waiter = await self._ws.ping()
+
         # wait for the response
-        return await waiter
+        response = await asyncio.wait_for(waiter, self._ping_timeout)
+
+        return response
```

### Comparing `interval_sdk-1.2.0/src/interval_sdk/classes/layout.py` & `interval_sdk-1.3.0/src/interval_sdk/classes/layout.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.2.0/src/interval_sdk/classes/logger.py` & `interval_sdk-1.3.0/src/interval_sdk/classes/logger.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.2.0/src/interval_sdk/classes/page.py` & `interval_sdk-1.3.0/src/interval_sdk/classes/page.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.2.0/src/interval_sdk/classes/rpc.py` & `interval_sdk-1.3.0/src/interval_sdk/classes/rpc.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.2.0/src/interval_sdk/classes/transaction_loading_state.py` & `interval_sdk-1.3.0/src/interval_sdk/classes/transaction_loading_state.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.2.0/src/interval_sdk/components/grid.py` & `interval_sdk-1.3.0/src/interval_sdk/components/grid.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.2.0/src/interval_sdk/components/table.py` & `interval_sdk-1.3.0/src/interval_sdk/components/table.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.2.0/src/interval_sdk/handlers.py` & `interval_sdk-1.3.0/src/interval_sdk/handlers.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.2.0/src/interval_sdk/internal_rpc_schema.py` & `interval_sdk-1.3.0/src/interval_sdk/internal_rpc_schema.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.2.0/src/interval_sdk/io_schema.py` & `interval_sdk-1.3.0/src/interval_sdk/io_schema.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.2.0/src/interval_sdk/main.py` & `interval_sdk-1.3.0/src/interval_sdk/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     ButtonItemModel,
     IOFunctionReturnModel,
     SerializableRecord,
 )
 from .classes.io import IO
 from .classes.action import Action
 from .classes.page import Page
-from .classes.isocket import ISocket
+from .classes.isocket import ISocket, NotConnectedError
 from .classes.logger import Logger, LogLevel
 from .classes.io_client import IOClient, IOError, IORender, IOResponse
 from .classes.rpc import DuplexRPCClient
 from .classes.layout import (
     BasicLayoutModel,
     Layout,
     PageError,
@@ -461,14 +461,20 @@
         loop.run_forever()
 
     async def listen_async(self):
         await self._create_socket_connection(uuid4())
         self._create_rpc_client()
         await self._initialize_host()
 
+    async def ping(self):
+        if self._isocket is None:
+            raise NotConnectedError()
+
+        await self._isocket.ping()
+
     async def immediately_close(self):
         self._shutdown_fut = None
         self._intentionally_closed = True
         self._server_rpc = None
         if self._isocket is not None:
             await self._isocket.close()
             self._isocket = None
@@ -834,14 +840,15 @@
         self._isocket = ISocket(
             id=instance_id,
             ws=ws,
             on_close=on_close,
             log_level=self._logger.log_level,
             num_producers=self._num_isocket_producers,
             send_timeout=self._send_timeout_seconds,
+            ping_timeout=self._ping_timeout_seconds,
         )
 
         await self._isocket.connect()
         self._is_connected = True
 
         if self._server_rpc is None:
             return
```

### Comparing `interval_sdk-1.2.0/src/interval_sdk/superjson/main.py` & `interval_sdk-1.3.0/src/interval_sdk/superjson/main.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.2.0/src/interval_sdk/superjson/plainer.py` & `interval_sdk-1.3.0/src/interval_sdk/superjson/plainer.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.2.0/src/interval_sdk/superjson/tests/test_superjson.py` & `interval_sdk-1.3.0/src/interval_sdk/superjson/tests/test_superjson.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.2.0/src/interval_sdk/superjson/transformer.py` & `interval_sdk-1.3.0/src/interval_sdk/superjson/transformer.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.2.0/src/interval_sdk/types.py` & `interval_sdk-1.3.0/src/interval_sdk/types.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.2.0/src/interval_sdk/util.py` & `interval_sdk-1.3.0/src/interval_sdk/util.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.2.0/setup.py` & `interval_sdk-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ['aiohttp>=3.8.1,<4.0.0',
  'pydantic>=1.9.0,<2.0.0',
  'typing-extensions>=4.4.0,<5.0.0',
  'websockets>=10.1,<11.0']
 
 setup_kwargs = {
     'name': 'interval-sdk',
-    'version': '1.2.0',
+    'version': '1.3.0',
     'description': "The frontendless framework for high growth companies. Interval automatically generates apps by inlining the UI in your backend code. It's a faster and more maintainable way to build internal tools, rapid prototypes, and more.",
     'long_description': '<a href="https://interval.com">\n  <img alt="Interval" width="100" height="100" style="border-radius: 6px;" src="https://interval.com/img/readme-assets/interval-avatar.png">\n</a>\n\n# Interval Python SDK\n\n[![pypi version](https://img.shields.io/pypi/v/interval-sdk?style=flat)](https://pypi.org/project/interval-sdk) [![Documentation](https://img.shields.io/badge/documentation-informational)](https://interval.com/docs) [![Twitter](https://img.shields.io/twitter/follow/useinterval.svg?color=%2338A1F3&label=twitter&style=flat)](https://twitter.com/useinterval) [![Discord](https://img.shields.io/badge/discord-join-blueviolet)](https://interval.com/discord)\n\n[Interval](https://interval.com) lets you quickly build internal web apps (think: customer support tools, admin panels, etc.) just by writing backend Python code.\n\nThis is our Python SDK which connects to the interval.com web app. If you don\'t have an Interval account, you can [create one here](https://interval.com/signup). All core features are free to use.\n\n## Why choose Interval?\n\n_"Python code > no-code"_\n\nInterval is an alternative to no-code/low-code UI builders. Modern frontend development is inherently complicated, and teams rightfully want to spend minimal engineering resources on internal dashboards. No-code tools attempt to solve this problem by allowing you to build UIs in a web browser without writing any frontend code.\n\nWe don\'t think this is the right solution. **Building UIs for mission-critical tools in your web browser** — often by non-technical teammates, outside of your codebase, without versioning or code review — **is an anti-pattern.** Apps built in this manner are brittle and break in unexpected ways.\n\nWith Interval, **all of the code for generating your web UIs lives within your app\'s codebase.** Tools built with Interval (we call these [actions](https://interval.com/docs/concepts/actions)) are just asynchronous functions that run in your backend. Because these are plain old functions, you can access the complete power of your Python app. You can loop, conditionally branch, access shared functions, and so on. When you need to request input or display output, `await` any of our [I/O methods](https://interval.com/docs/io-methods/) to present a form to the user and your script will pause execution until input is received.\n\nHere\'s a simple app with a single "Hello, world" action:\n\n```python\nfrom interval_sdk import Interval, IO\n\n# Initialize Interval\ninterval = Interval(api_key="<YOUR API KEY>")\n\n@interval.action\nasync def hello_world(io: IO):\n    name = await io.input.text("Your name")\n    return f"Hello, {name}"\n\n\n# Synchronously listen, blocking forever\ninterval.listen()\n```\n\nTo not block, interval can also be run asynchronously using\n`interval.listen_async()`. You must provide your own event loop.\n\nThe task will complete as soon as connection to Interval completes, so you\nlikely want to run forever or run alongside another permanent task.\n\n```python\nimport asyncio, signal\n\nloop = asyncio.get_event_loop()\ntask = loop.create_task(interval.listen_async())\ndef handle_done(task: asyncio.Task[None]):\n    try:\n        task.result()\n    except:\n        loop.stop()\n\ntask.add_done_callback(handle_done)\nfor sig in {signal.SIGINT, signal.SIGTERM}:\n    loop.add_signal_handler(sig, loop.stop)\nloop.run_forever()\n```\n\nInterval:\n\n- Makes creating full-stack apps as easy as writing CLI scripts.\n- Can scale from a handful of scripts to robust multi-user dashboards.\n- Lets you build faster than no-code, without leaving your codebase & IDE.\n\nWith Interval, you do not need to:\n\n- Write REST or GraphQL API endpoints to connect internal functionality to no-code tools.\n- Give Interval write access to your database (or give us _any_ of your credentials, for that matter).\n- Build web UIs with a drag-and-drop interface.\n\n## More about Interval\n\n- 📖 [Documentation](https://interval.com/docs)\n- 🌐 [Interval website](https://interval.com)\n- 💬 [Discord community](https://interval.com/discord)\n- 📰 [Product updates](https://interval.com/blog)\n\n## Contributing\n\nThis project uses [Poetry](https://python-poetry.org/) for dependency\nmanagement\n\n1. `poetry install` to install dependencies\n2. `poetry shell` to activate the virtual environment\n\nTasks are configured using [poethepoet](https://github.com/nat-n/poethepoet)\n(installed as a dev dependency).\n\n- `poe demo [demo_name]` to run a demo (`basic` by default if `demo_name` omitted)\n- `poe test` to run `pytest` (can also run `pytest` directly in virtual env)\n\nCode is formatted using [Black](https://github.com/psf/black). Please configure\nyour editor to format on save using Black, or run `poe format` to format the\ncode before committing changes.\n\n## Tests\n\n*Note:* Tests currently require a local instance of the Interval backend.\n\nTests use [pytest](https://docs.pytest.org/en/7.1.x/) and\n[playwright](https://playwright.dev/python/).\n\nCurrently assumes the `test-runner@interval.com` user exists already.\nRun `yarn test` in the `web` directory at least once to create it before\nrunning these.\n',
     'author': 'Jacob Mischka',
     'author_email': 'jacob@interval.com',
     'maintainer': 'Jacob Mischka',
     'maintainer_email': 'jacob@interval.com',
     'url': 'https://interval.com',
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['interval_sdk', 'interval_sdk.classes',
 'interval_sdk.components', 'interval_sdk.superjson',
 'interval_sdk.superjson.tests'] package_data = \ {'': ['*']} install_requires =
 \ ['aiohttp>=3.8.1,<4.0.0', 'pydantic>=1.9.0,<2.0.0', 'typing-
 extensions>=4.4.0,<5.0.0', 'websockets>=10.1,<11.0'] setup_kwargs = { 'name':
-'interval-sdk', 'version': '1.2.0', 'description': "The frontendless framework
+'interval-sdk', 'version': '1.3.0', 'description': "The frontendless framework
 for high growth companies. Interval automatically generates apps by inlining
 the UI in your backend code. It's a faster and more maintainable way to build
 internal tools, rapid prototypes, and more.", 'long_description': '\n_
 [Interval]\n\n\n# Interval Python SDK\n\n[![pypi version](https://
 img.shields.io/pypi/v/interval-sdk?style=flat)](https://pypi.org/project/
 interval-sdk) [![Documentation](https://img.shields.io/badge/documentation-
 informational)](https://interval.com/docs) [![Twitter](https://img.shields.io/
```

### Comparing `interval_sdk-1.2.0/PKG-INFO` & `interval_sdk-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interval-sdk
-Version: 1.2.0
+Version: 1.3.0
 Summary: The frontendless framework for high growth companies. Interval automatically generates apps by inlining the UI in your backend code. It's a faster and more maintainable way to build internal tools, rapid prototypes, and more.
 Home-page: https://interval.com
 Keywords: internal tool,app,ui,ui builder
 Author: Jacob Mischka
 Author-email: jacob@interval.com
 Maintainer: Jacob Mischka
 Maintainer-email: jacob@interval.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: interval-sdk Version: 1.2.0 Summary: The
+Metadata-Version: 2.1 Name: interval-sdk Version: 1.3.0 Summary: The
 frontendless framework for high growth companies. Interval automatically
 generates apps by inlining the UI in your backend code. It's a faster and more
 maintainable way to build internal tools, rapid prototypes, and more. Home-
 page: https://interval.com Keywords: internal tool,app,ui,ui builder Author:
 Jacob Mischka Author-email: jacob@interval.com Maintainer: Jacob Mischka
 Maintainer-email: jacob@interval.com Requires-Python: >=3.9,<4.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

