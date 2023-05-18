# Comparing `tmp/sse-starlette-1.6.0.tar.gz` & `tmp/sse-starlette-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sse-starlette-1.6.0.tar", last modified: Sun May 14 08:32:32 2023, max compression
+gzip compressed data, was "sse-starlette-1.6.1.tar", last modified: Thu May 18 11:26:14 2023, max compression
```

## Comparing `sse-starlette-1.6.0.tar` & `sse-starlette-1.6.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-05-14 08:32:32.054255 sse-starlette-1.6.0/
--rw-r--r--   0 Q187392    (501) staff       (20)      395 2022-12-16 17:29:08.000000 sse-starlette-1.6.0/AUTHORS
--rw-r--r--   0 Q187392    (501) staff       (20)     1892 2023-03-11 18:12:47.000000 sse-starlette-1.6.0/CHANGELOG.md
--rw-r--r--   0 Q187392    (501) staff       (20)     1511 2022-12-16 17:29:08.000000 sse-starlette-1.6.0/LICENSE
--rw-r--r--   0 Q187392    (501) staff       (20)      103 2022-12-16 17:29:08.000000 sse-starlette-1.6.0/MANIFEST.in
--rw-r--r--   0 Q187392    (501) staff       (20)     6520 2023-05-14 08:32:32.054348 sse-starlette-1.6.0/PKG-INFO
--rw-r--r--   0 Q187392    (501) staff       (20)     4377 2023-05-14 08:31:06.000000 sse-starlette-1.6.0/README.md
--rw-r--r--   0 Q187392    (501) staff       (20)      106 2022-12-16 17:29:08.000000 sse-starlette-1.6.0/pyproject.toml
--rw-r--r--   0 Q187392    (501) staff       (20)     1800 2023-05-14 08:32:32.073549 sse-starlette-1.6.0/setup.cfg
--rw-r--r--   0 Q187392    (501) staff       (20)      152 2022-12-16 17:29:08.000000 sse-starlette-1.6.0/setup.py
-drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-05-14 08:32:32.042767 sse-starlette-1.6.0/sse_starlette/
--rw-r--r--   0 Q187392    (501) staff       (20)      143 2023-05-14 08:31:53.000000 sse-starlette-1.6.0/sse_starlette/__init__.py
--rw-r--r--   0 Q187392    (501) staff       (20)        0 2022-12-16 17:29:08.000000 sse-starlette-1.6.0/sse_starlette/py.typed
--rw-r--r--   0 Q187392    (501) staff       (20)    10910 2023-05-14 08:32:12.000000 sse-starlette-1.6.0/sse_starlette/sse.py
-drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-05-14 08:32:32.052625 sse-starlette-1.6.0/sse_starlette.egg-info/
--rw-r--r--   0 Q187392    (501) staff       (20)     6520 2023-05-14 08:32:30.000000 sse-starlette-1.6.0/sse_starlette.egg-info/PKG-INFO
--rw-r--r--   0 Q187392    (501) staff       (20)      392 2023-05-14 08:32:32.000000 sse-starlette-1.6.0/sse_starlette.egg-info/SOURCES.txt
--rw-r--r--   0 Q187392    (501) staff       (20)        1 2023-05-14 08:32:30.000000 sse-starlette-1.6.0/sse_starlette.egg-info/dependency_links.txt
--rw-r--r--   0 Q187392    (501) staff       (20)       10 2023-05-14 08:32:30.000000 sse-starlette-1.6.0/sse_starlette.egg-info/requires.txt
--rw-r--r--   0 Q187392    (501) staff       (20)       14 2023-05-14 08:32:30.000000 sse-starlette-1.6.0/sse_starlette.egg-info/top_level.txt
-drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-05-14 08:32:32.053874 sse-starlette-1.6.0/tests/
--rw-r--r--   0 Q187392    (501) staff       (20)     6176 2023-05-14 08:32:12.000000 sse-starlette-1.6.0/tests/test_event_source_response.py
--rw-r--r--   0 Q187392    (501) staff       (20)     3028 2023-05-02 20:24:28.000000 sse-starlette-1.6.0/tests/test_sse.py
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-05-18 11:26:14.764451 sse-starlette-1.6.1/
+-rw-r--r--   0 Q187392    (501) staff       (20)      395 2022-12-16 17:29:08.000000 sse-starlette-1.6.1/AUTHORS
+-rw-r--r--   0 Q187392    (501) staff       (20)     1892 2023-03-11 18:12:47.000000 sse-starlette-1.6.1/CHANGELOG.md
+-rw-r--r--   0 Q187392    (501) staff       (20)     1511 2022-12-16 17:29:08.000000 sse-starlette-1.6.1/LICENSE
+-rw-r--r--   0 Q187392    (501) staff       (20)      103 2022-12-16 17:29:08.000000 sse-starlette-1.6.1/MANIFEST.in
+-rw-r--r--   0 Q187392    (501) staff       (20)     6520 2023-05-18 11:26:14.764573 sse-starlette-1.6.1/PKG-INFO
+-rw-r--r--   0 Q187392    (501) staff       (20)     4377 2023-05-14 08:31:06.000000 sse-starlette-1.6.1/README.md
+-rw-r--r--   0 Q187392    (501) staff       (20)      106 2022-12-16 17:29:08.000000 sse-starlette-1.6.1/pyproject.toml
+-rw-r--r--   0 Q187392    (501) staff       (20)     1800 2023-05-18 11:26:14.790040 sse-starlette-1.6.1/setup.cfg
+-rw-r--r--   0 Q187392    (501) staff       (20)      152 2022-12-16 17:29:08.000000 sse-starlette-1.6.1/setup.py
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-05-18 11:26:14.753440 sse-starlette-1.6.1/sse_starlette/
+-rw-r--r--   0 Q187392    (501) staff       (20)      143 2023-05-18 11:25:22.000000 sse-starlette-1.6.1/sse_starlette/__init__.py
+-rw-r--r--   0 Q187392    (501) staff       (20)        0 2022-12-16 17:29:08.000000 sse-starlette-1.6.1/sse_starlette/py.typed
+-rw-r--r--   0 Q187392    (501) staff       (20)    10962 2023-05-18 11:25:07.000000 sse-starlette-1.6.1/sse_starlette/sse.py
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-05-18 11:26:14.760430 sse-starlette-1.6.1/sse_starlette.egg-info/
+-rw-r--r--   0 Q187392    (501) staff       (20)     6520 2023-05-18 11:26:13.000000 sse-starlette-1.6.1/sse_starlette.egg-info/PKG-INFO
+-rw-r--r--   0 Q187392    (501) staff       (20)      392 2023-05-18 11:26:14.000000 sse-starlette-1.6.1/sse_starlette.egg-info/SOURCES.txt
+-rw-r--r--   0 Q187392    (501) staff       (20)        1 2023-05-18 11:26:13.000000 sse-starlette-1.6.1/sse_starlette.egg-info/dependency_links.txt
+-rw-r--r--   0 Q187392    (501) staff       (20)       10 2023-05-18 11:26:13.000000 sse-starlette-1.6.1/sse_starlette.egg-info/requires.txt
+-rw-r--r--   0 Q187392    (501) staff       (20)       14 2023-05-18 11:26:13.000000 sse-starlette-1.6.1/sse_starlette.egg-info/top_level.txt
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-05-18 11:26:14.763943 sse-starlette-1.6.1/tests/
+-rw-r--r--   0 Q187392    (501) staff       (20)     6298 2023-05-18 11:25:07.000000 sse-starlette-1.6.1/tests/test_event_source_response.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     3028 2023-05-02 20:24:28.000000 sse-starlette-1.6.1/tests/test_sse.py
```

### Comparing `sse-starlette-1.6.0/CHANGELOG.md` & `sse-starlette-1.6.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `sse-starlette-1.6.0/LICENSE` & `sse-starlette-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sse-starlette-1.6.0/PKG-INFO` & `sse-starlette-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sse-starlette
-Version: 1.6.0
+Version: 1.6.1
 Summary: "SSE plugin for Starlette"
 Home-page: https://github.com/sysid/sse-starlette
 Author: sysid
 Author-email: sysid@gmx.de
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `sse-starlette-1.6.0/README.md` & `sse-starlette-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `sse-starlette-1.6.0/setup.cfg` & `sse-starlette-1.6.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sse-starlette
-version = 1.6.0
+version = 1.6.1
 description = "SSE plugin for Starlette"
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 author = sysid
 author_email = sysid@gmx.de
 url = https://github.com/sysid/sse-starlette
 classifiers =
```

### Comparing `sse-starlette-1.6.0/sse_starlette/sse.py` & `sse-starlette-1.6.1/sse_starlette/sse.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,15 +200,16 @@
     @staticmethod
     async def listen_for_exit_signal() -> None:
         # Check if should_exit was set before anybody started waiting
         if AppStatus.should_exit:
             return
 
         # Setup an Event
-        AppStatus.should_exit_event = anyio.Event()
+        if AppStatus.should_exit_event is None:
+            AppStatus.should_exit_event = anyio.Event()
 
         # Check if should_exit got set while we set up the event
         if AppStatus.should_exit:
             return
 
         # Await the event
         await AppStatus.should_exit_event.wait()
```

### Comparing `sse-starlette-1.6.0/sse_starlette.egg-info/PKG-INFO` & `sse-starlette-1.6.1/sse_starlette.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sse-starlette
-Version: 1.6.0
+Version: 1.6.1
 Summary: "SSE plugin for Starlette"
 Home-page: https://github.com/sysid/sse-starlette
 Author: sysid
 Author-email: sysid@gmx.de
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `sse-starlette-1.6.0/tests/test_event_source_response.py` & `sse-starlette-1.6.1/tests/test_event_source_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     "input,expected",
     [
         ("integer", b"data: 1\r\n\r\n"),
         ("dict1", b"data: 1\r\n\r\n"),
         ("dict2", b"event: message\r\ndata: 1\r\n\r\n"),
     ],
 )
-def test_sync_event_source_response(input, expected):
+async def test_sync_event_source_response(reset_appstatus_event, input, expected):
     async def app(scope, receive, send):
         async def numbers(minimum, maximum):
             for i in range(minimum, maximum + 1):
                 await asyncio.sleep(0.1)
                 if input == "integer":
                     yield i
                 elif input == "dict1":
@@ -68,15 +68,17 @@
     "input,expected",
     [
         ("integer", b"data: 1\r\n\r\n"),
         ("dict1", b"data: 1\r\n\r\n"),
         ("dict2", b"event: message\r\ndata: 1\r\n\r\n"),
     ],
 )
-def test_sync_memory_channel_event_source_response(input, expected):
+def test_sync_memory_channel_event_source_response(
+    reset_appstatus_event, input, expected
+):
     async def app(scope, receive, send):
         send_chan, recv_chan = anyio.create_memory_object_stream(math.inf)
 
         async def numbers(inner_send_chan, minimum, maximum):
             async with send_chan:
                 for i in range(minimum, maximum + 1):
                     await anyio.sleep(0.1)
@@ -84,26 +86,28 @@
                     if input == "integer":
                         await inner_send_chan.send(i)
                     elif input == "dict1":
                         await inner_send_chan.send(dict(data=i))
                     elif input == "dict2":
                         await inner_send_chan.send(dict(data=i, event="message"))
 
-        response = EventSourceResponse(recv_chan, data_sender_callable=partial(numbers, send_chan, 1, 5), ping=0.2)  # type: ignore
+        response = EventSourceResponse(
+            recv_chan, data_sender_callable=partial(numbers, send_chan, 1, 5), ping=0.2
+        )  # type: ignore
         await response(scope, receive, send)
 
     client = TestClient(app)
     response = client.get("/")
     assert response.content.decode().count("ping") == 2
     assert expected in response.content
     print(response.content)
 
 
 @pytest.mark.anyio
-async def test_endless():
+async def test_endless(reset_appstatus_event):
     async def app(scope, receive, send):
         async def event_publisher():
             i = 0
             try:
                 while True:
                     i += 1
                     _log.info(f"yielding {i=}")
@@ -137,15 +141,15 @@
             finally:
                 # The cancel_called property will be True if timeout was reached
                 assert scope.cancel_called is True
                 assert "chunk: data: 3" in caplog.text
 
 
 @pytest.mark.anyio
-async def test_ping_concurrency():
+async def test_ping_concurrency(reset_appstatus_event):
     # Sequencing here is as follows:
     # t=0.5s - event_publisher sends the first response item,
     #          claiming the lock and going to sleep for 1 second so until t=1.5s.
     # t=1.0s - ping task wakes up and tries to call send while we know
     #          that event_publisher is still blocked inside it and holding the lock
     #
     # If there are concurrent calls to `send` then we will raise the WouldBlock below
```

### Comparing `sse-starlette-1.6.0/tests/test_sse.py` & `sse-starlette-1.6.1/tests/test_sse.py`

 * *Files identical despite different names*

