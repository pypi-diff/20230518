# Comparing `tmp/binance-futures-connector-3.3.1.tar.gz` & `tmp/binance-futures-connector-4.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binance-futures-connector-3.3.1.tar", last modified: Tue Mar 21 06:08:44 2023, max compression
+gzip compressed data, was "binance-futures-connector-4.0.0rc1.tar", last modified: Thu May 18 06:40:17 2023, max compression
```

## Comparing `binance-futures-connector-3.3.1.tar` & `binance-futures-connector-4.0.0rc1.tar`

### file list

```diff
@@ -1,48 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:08:44.235689 binance-futures-connector-3.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-03-21 06:08:41.000000 binance-futures-connector-3.3.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-21 06:08:41.000000 binance-futures-connector-3.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-03-21 06:08:44.235689 binance-futures-connector-3.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-03-21 06:08:41.000000 binance-futures-connector-3.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:08:44.231689 binance-futures-connector-3.3.1/binance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 06:08:41.000000 binance-futures-connector-3.3.1/binance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-21 06:08:41.000000 binance-futures-connector-3.3.1/binance/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-03-21 06:08:41.000000 binance-futures-connector-3.3.1/binance/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:08:44.231689 binance-futures-connector-3.3.1/binance/cm_futures/
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-03-21 06:08:41.000000 binance-futures-connector-3.3.1/binance/cm_futures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28001 2023-03-21 06:08:41.000000 binance-futures-connector-3.3.1/binance/cm_futures/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-03-21 06:08:41.000000 binance-futures-connector-3.3.1/binance/cm_futures/data_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)    20057 2023-03-21 06:08:41.000000 binance-futures-connector-3.3.1/binance/cm_futures/market.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-03-21 06:08:41.000000 binance-futures-connector-3.3.1/binance/cm_futures/portfolio_margin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-03-21 06:08:41.000000 binance-futures-connector-3.3.1/binance/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:08:44.231689 binance-futures-connector-3.3.1/binance/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 06:08:41.000000 binance-futures-connector-3.3.1/binance/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-03-21 06:08:41.000000 binance-futures-connector-3.3.1/binance/lib/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-03-21 06:08:41.000000 binance-futures-connector-3.3.1/binance/lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:08:44.231689 binance-futures-connector-3.3.1/binance/um_futures/
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-03-21 06:08:41.000000 binance-futures-connector-3.3.1/binance/um_futures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29832 2023-03-21 06:08:41.000000 binance-futures-connector-3.3.1/binance/um_futures/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-03-21 06:08:41.000000 binance-futures-connector-3.3.1/binance/um_futures/data_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)    18300 2023-03-21 06:08:41.000000 binance-futures-connector-3.3.1/binance/um_futures/market.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-03-21 06:08:41.000000 binance-futures-connector-3.3.1/binance/um_futures/portfolio_margin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:08:44.231689 binance-futures-connector-3.3.1/binance/websocket/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 06:08:41.000000 binance-futures-connector-3.3.1/binance/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-03-21 06:08:41.000000 binance-futures-connector-3.3.1/binance/websocket/binance_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-03-21 06:08:41.000000 binance-futures-connector-3.3.1/binance/websocket/binance_client_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-03-21 06:08:41.000000 binance-futures-connector-3.3.1/binance/websocket/binance_socket_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:08:44.231689 binance-futures-connector-3.3.1/binance/websocket/cm_futures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 06:08:41.000000 binance-futures-connector-3.3.1/binance/websocket/cm_futures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10501 2023-03-21 06:08:41.000000 binance-futures-connector-3.3.1/binance/websocket/cm_futures/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:08:44.231689 binance-futures-connector-3.3.1/binance/websocket/um_futures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 06:08:41.000000 binance-futures-connector-3.3.1/binance/websocket/um_futures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8639 2023-03-21 06:08:41.000000 binance-futures-connector-3.3.1/binance/websocket/um_futures/websocket_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-03-21 06:08:41.000000 binance-futures-connector-3.3.1/binance/websocket/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:08:44.235689 binance-futures-connector-3.3.1/binance_futures_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-03-21 06:08:44.000000 binance-futures-connector-3.3.1/binance_futures_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-03-21 06:08:44.000000 binance-futures-connector-3.3.1/binance_futures_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 06:08:44.000000 binance-futures-connector-3.3.1/binance_futures_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-21 06:08:44.000000 binance-futures-connector-3.3.1/binance_futures_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-21 06:08:44.000000 binance-futures-connector-3.3.1/binance_futures_connector.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:08:44.235689 binance-futures-connector-3.3.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-21 06:08:41.000000 binance-futures-connector-3.3.1/requirements/common.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-03-21 06:08:44.235689 binance-futures-connector-3.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-03-21 06:08:41.000000 binance-futures-connector-3.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:40:17.379776 binance-futures-connector-4.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7932 2023-05-18 06:40:17.379776 binance-futures-connector-4.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:40:17.375776 binance-futures-connector-4.0.0rc1/binance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:40:17.375776 binance-futures-connector-4.0.0rc1/binance/cm_futures/
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/cm_futures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28001 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/cm_futures/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/cm_futures/data_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20057 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/cm_futures/market.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/cm_futures/portfolio_margin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:40:17.379776 binance-futures-connector-4.0.0rc1/binance/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/lib/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:40:17.379776 binance-futures-connector-4.0.0rc1/binance/um_futures/
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/um_futures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29832 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/um_futures/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/um_futures/data_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18300 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/um_futures/market.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/um_futures/portfolio_margin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:40:17.379776 binance-futures-connector-4.0.0rc1/binance/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/websocket/binance_socket_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:40:17.379776 binance-futures-connector-4.0.0rc1/binance/websocket/cm_futures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/websocket/cm_futures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11396 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/websocket/cm_futures/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:40:17.379776 binance-futures-connector-4.0.0rc1/binance/websocket/um_futures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/websocket/um_futures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9226 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/websocket/um_futures/websocket_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/websocket/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:40:17.379776 binance-futures-connector-4.0.0rc1/binance_futures_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7932 2023-05-18 06:40:17.000000 binance-futures-connector-4.0.0rc1/binance_futures_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-18 06:40:17.000000 binance-futures-connector-4.0.0rc1/binance_futures_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 06:40:17.000000 binance-futures-connector-4.0.0rc1/binance_futures_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-18 06:40:17.000000 binance-futures-connector-4.0.0rc1/binance_futures_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-18 06:40:17.000000 binance-futures-connector-4.0.0rc1/binance_futures_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:40:17.379776 binance-futures-connector-4.0.0rc1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/requirements/common.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-18 06:40:17.379776 binance-futures-connector-4.0.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/setup.py
```

### Comparing `binance-futures-connector-3.3.1/LICENSE.md` & `binance-futures-connector-4.0.0rc1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-3.3.1/PKG-INFO` & `binance-futures-connector-4.0.0rc1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: binance-futures-connector
-Version: 3.3.1
-Summary: This is a lightweight library that works as a connector to Binance Futures public API.
-Home-page: https://github.com/binance/binance-futures-connector-python
-License: MIT
-Keywords: Binance futures,Public API
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Financial and Insurance Industry
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # Binance Futures Public API Connector Python
 [![Python version](https://img.shields.io/pypi/pyversions/binance-futures-connector)](https://www.python.org/downloads/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 This is a lightweight library that works as a connector to [Binance Futures public API](https://binance-docs.github.io/apidocs/futures/en/)
 
 - Supported APIs:
@@ -190,44 +172,74 @@
         - `error_message` - Server's error message, e.g. `Unknown order sent.`
         - `header` - Full response header.
 - `binance.error.ServerError`
     - This is thrown when server returns `5XX`, it's an issue from server side.
 
 ## Websocket
 
+### Connector v4
+
+WebSocket can be established through the following connections:
+- USD-M WebSocket Stream (`https://binance-docs.github.io/apidocs/futures/en/#websocket-market-streams`)
+- COIN-M WebSocket Stream (`https://binance-docs.github.io/apidocs/delivery/en/#websocket-market-streams`)
+
 ```python
+# WebSocket Stream Client
 import time
-from binance.websocket.cm_futures.websocket_client import CMFuturesWebsocketClient
+from binance.websocket.um_futures.websocket_client import UMFuturesWebsocketClient
 
-def message_handler(message):
-    print(message)
+def message_handler(_, message):
+    logging.info(message)
+
+my_client = UMFuturesWebsocketClient(on_message=message_handler)
 
-ws_client = CMFuturesWebsocketClient()
-ws_client.start()
+# Subscribe to a single symbol stream
+my_client.agg_trade(symbol="bnbusdt")
+time.sleep(5)
+logging.info("closing ws connection")
+my_client.stop()
+```
 
-ws_client.mini_ticker(
-    symbol='bnbusdt',
-    id=1,
-    callback=message_handler,
-)
-
-# Combine selected streams
-ws_client.instant_subscribe(
-    stream=['bnbusdt@bookTicker', 'ethusdt@bookTicker'],
-    callback=message_handler,
-)
+#### Request Id
 
-time.sleep(10)
+Client can assign a request id to each request. The request id will be returned in the response message. Not mandatory in the library, it generates a uuid format string if not provided.
 
-print("closing ws connection")
-ws_client.stop()
+```python
+# id provided by client
+my_client.agg_trade(symbol="bnbusdt", id="my_request_id")
 
+# library will generate a random uuid string
+my_client.agg_trade(symbol="bnbusdt")
 ```
+
+#### Combined Streams
+- If you set `is_combined` to `True`, `"/stream/"` will be appended to the `baseURL` to allow for Combining streams.
+- `is_combined` defaults to `False` and `"/ws/"` (raw streams) will be appended to the `baseURL`.
+
 More websocket examples are available in the `examples` folder
 
+## Websocket < v4
+
+```python
+import time
+from binance.websocket.um_futures.websocket_client import UMFuturesWebsocketClient
+
+def message_handler(message):
+    print(message)
+
+my_client = UMFuturesWebsocketClient(on_message=message_handler)
+
+# Subscribe to a single symbol stream
+my_client.agg_trade(symbol="bnbusdt")
+time.sleep(5)
+print("closing ws connection")
+my_client.stop()
+
+```
+
 ### Heartbeat
 
 Once connected, the websocket server sends a ping frame every 3 minutes and requires a response pong frame back within
 a 10 minutes period. This package handles the pong responses automatically.
 
 ## License
 MIT
```

### Comparing `binance-futures-connector-3.3.1/README.md` & `binance-futures-connector-4.0.0rc1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: binance-futures-connector
+Version: 4.0.0rc1
+Summary: This is a lightweight library that works as a connector to Binance Futures public API.
+Home-page: https://github.com/binance/binance-futures-connector-python
+License: MIT
+Keywords: Binance futures,Public API
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Financial and Insurance Industry
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
 # Binance Futures Public API Connector Python
 [![Python version](https://img.shields.io/pypi/pyversions/binance-futures-connector)](https://www.python.org/downloads/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 This is a lightweight library that works as a connector to [Binance Futures public API](https://binance-docs.github.io/apidocs/futures/en/)
 
 - Supported APIs:
@@ -172,44 +190,74 @@
         - `error_message` - Server's error message, e.g. `Unknown order sent.`
         - `header` - Full response header.
 - `binance.error.ServerError`
     - This is thrown when server returns `5XX`, it's an issue from server side.
 
 ## Websocket
 
+### Connector v4
+
+WebSocket can be established through the following connections:
+- USD-M WebSocket Stream (`https://binance-docs.github.io/apidocs/futures/en/#websocket-market-streams`)
+- COIN-M WebSocket Stream (`https://binance-docs.github.io/apidocs/delivery/en/#websocket-market-streams`)
+
 ```python
+# WebSocket Stream Client
 import time
-from binance.websocket.cm_futures.websocket_client import CMFuturesWebsocketClient
+from binance.websocket.um_futures.websocket_client import UMFuturesWebsocketClient
 
-def message_handler(message):
-    print(message)
+def message_handler(_, message):
+    logging.info(message)
+
+my_client = UMFuturesWebsocketClient(on_message=message_handler)
 
-ws_client = CMFuturesWebsocketClient()
-ws_client.start()
+# Subscribe to a single symbol stream
+my_client.agg_trade(symbol="bnbusdt")
+time.sleep(5)
+logging.info("closing ws connection")
+my_client.stop()
+```
 
-ws_client.mini_ticker(
-    symbol='bnbusdt',
-    id=1,
-    callback=message_handler,
-)
-
-# Combine selected streams
-ws_client.instant_subscribe(
-    stream=['bnbusdt@bookTicker', 'ethusdt@bookTicker'],
-    callback=message_handler,
-)
+#### Request Id
 
-time.sleep(10)
+Client can assign a request id to each request. The request id will be returned in the response message. Not mandatory in the library, it generates a uuid format string if not provided.
 
-print("closing ws connection")
-ws_client.stop()
+```python
+# id provided by client
+my_client.agg_trade(symbol="bnbusdt", id="my_request_id")
 
+# library will generate a random uuid string
+my_client.agg_trade(symbol="bnbusdt")
 ```
+
+#### Combined Streams
+- If you set `is_combined` to `True`, `"/stream/"` will be appended to the `baseURL` to allow for Combining streams.
+- `is_combined` defaults to `False` and `"/ws/"` (raw streams) will be appended to the `baseURL`.
+
 More websocket examples are available in the `examples` folder
 
+## Websocket < v4
+
+```python
+import time
+from binance.websocket.um_futures.websocket_client import UMFuturesWebsocketClient
+
+def message_handler(message):
+    print(message)
+
+my_client = UMFuturesWebsocketClient(on_message=message_handler)
+
+# Subscribe to a single symbol stream
+my_client.agg_trade(symbol="bnbusdt")
+time.sleep(5)
+print("closing ws connection")
+my_client.stop()
+
+```
+
 ### Heartbeat
 
 Once connected, the websocket server sends a ping frame every 3 minutes and requires a response pong frame back within
 a 10 minutes period. This package handles the pong responses automatically.
 
 ## License
 MIT
```

### Comparing `binance-futures-connector-3.3.1/binance/api.py` & `binance-futures-connector-4.0.0rc1/binance/api.py`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-3.3.1/binance/cm_futures/__init__.py` & `binance-futures-connector-4.0.0rc1/binance/cm_futures/__init__.py`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-3.3.1/binance/cm_futures/account.py` & `binance-futures-connector-4.0.0rc1/binance/cm_futures/account.py`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-3.3.1/binance/cm_futures/data_stream.py` & `binance-futures-connector-4.0.0rc1/binance/cm_futures/data_stream.py`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-3.3.1/binance/cm_futures/market.py` & `binance-futures-connector-4.0.0rc1/binance/cm_futures/market.py`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-3.3.1/binance/error.py` & `binance-futures-connector-4.0.0rc1/binance/error.py`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-3.3.1/binance/lib/authentication.py` & `binance-futures-connector-4.0.0rc1/binance/lib/authentication.py`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-3.3.1/binance/lib/utils.py` & `binance-futures-connector-4.0.0rc1/binance/lib/utils.py`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-3.3.1/binance/um_futures/__init__.py` & `binance-futures-connector-4.0.0rc1/binance/um_futures/__init__.py`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-3.3.1/binance/um_futures/account.py` & `binance-futures-connector-4.0.0rc1/binance/um_futures/account.py`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-3.3.1/binance/um_futures/data_stream.py` & `binance-futures-connector-4.0.0rc1/binance/um_futures/data_stream.py`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-3.3.1/binance/um_futures/market.py` & `binance-futures-connector-4.0.0rc1/binance/um_futures/market.py`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-3.3.1/binance/websocket/um_futures/websocket_client.py` & `binance-futures-connector-4.0.0rc1/binance/websocket/um_futures/websocket_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,68 @@
 from binance.websocket.websocket_client import BinanceWebsocketClient
 
 
 class UMFuturesWebsocketClient(BinanceWebsocketClient):
-    def __init__(self, stream_url="wss://fstream.binance.com"):
-        super().__init__(stream_url)
+    def __init__(
+        self,
+        stream_url="wss://fstream.binance.com",
+        on_message=None,
+        on_open=None,
+        on_close=None,
+        on_error=None,
+        on_ping=None,
+        on_pong=None,
+        is_combined=False,
+    ):
+        if is_combined:
+            stream_url = stream_url + "/stream"
+        else:
+            stream_url = stream_url + "/ws"
+        super().__init__(
+            stream_url,
+            on_message=on_message,
+            on_open=on_open,
+            on_close=on_close,
+            on_error=on_error,
+            on_ping=on_ping,
+            on_pong=on_pong,
+        )
 
-    def agg_trade(self, symbol: str, id: int, callback, **kwargs):
+    def agg_trade(self, symbol: str, id=None, action=None, **kwargs):
         """Aggregate Trade Streams
 
         The Aggregate Trade Streams push market trade information that is aggregated for a single taker order every 100 milliseconds.
         Only market trades will be aggregated, which means the insurance fund trades and ADL trades won't be aggregated.
 
         Stream Name: <symbol>@aggTrade
 
         https://binance-docs.github.io/apidocs/futures/en/#aggregate-trade-streams
 
         Update Speed: 100ms
         """
-        self.live_subscribe(
-            "{}@aggTrade".format(symbol.lower()), id, callback, **kwargs
-        )
+        stream_name = "{}@aggTrade".format(symbol.lower())
 
-    def mark_price(self, symbol: str, id: int, speed: int, callback, **kwargs):
+        self.send_message_to_server(stream_name, action=action, id=id)
+
+    def mark_price(self, symbol: str, speed: int, id=None, action=None, **kwargs):
         """Mark Price Streams
 
         Mark price and funding rate for all symbols pushed every 3 seconds or every second.
 
         Stream Name: <symbol>@markPrice or <symbol>@markPrice@1s
 
         https://binance-docs.github.io/apidocs/futures/en/#mark-price-stream
 
         Update Speed: 3000ms or 1000ms
         """
-        self.live_subscribe(
-            "{}@markPrice@{}s".format(symbol.lower(), speed), id, callback, **kwargs
-        )
+        stream_name = "{}@markPrice@{}s".format(symbol.lower(), speed)
+
+        self.send_message_to_server(stream_name, action=action, id=id)
 
-    def kline(self, symbol: str, id: int, interval: str, callback, **kwargs):
+    def kline(self, symbol: str, interval: str, id=None, action=None, **kwargs):
         """Kline/Candlestick Streams
 
         The Kline/Candlestick Stream push updates to the current klines/candlestick every 250 milliseconds (if existing)
 
         Stream Name: <symbol>@kline_<interval>
 
         https://binance-docs.github.io/apidocs/futures/en/#kline-candlestick-streams
@@ -62,21 +84,26 @@
         - 1d
         - 3d
         - 1w
         - 1M
 
         Update Speed: 250ms
         """
+        stream_name = "{}@kline_{}".format(symbol.lower(), interval)
 
-        self.live_subscribe(
-            "{}@kline_{}".format(symbol.lower(), interval), id, callback, **kwargs
-        )
+        self.send_message_to_server(stream_name, action=action, id=id)
 
     def continuous_kline(
-        self, pair: str, id: int, contractType: str, interval: str, callback, **kwargs
+        self,
+        pair: str,
+        contractType: str,
+        interval: str,
+        id=None,
+        action=None,
+        **kwargs
     ):
         """Continuous Kline/Candlestick Streams
 
         The Kline/Candlestick Stream push updates to Kline/candlestick bars for a specific contract type. every 250 milliseconds
 
         Stream Name: <pair>_<contractType>@continuousKline_<interval>
 
@@ -99,23 +126,21 @@
         - 1d
         - 3d
         - 1w
         - 1M
 
         Update Speed: 250ms
         """
-
-        self.live_subscribe(
-            "{}_{}@continuousKline_{}".format(pair.lower(), contractType, interval),
-            id,
-            callback,
-            **kwargs
+        stream_name = "{}_{}@continuousKline_{}".format(
+            pair.lower(), contractType, interval
         )
 
-    def mini_ticker(self, id: int, callback, symbol=None, **kwargs):
+        self.send_message_to_server(stream_name, action=action, id=id)
+
+    def mini_ticker(self, symbol=None, id=None, action=None, **kwargs):
         """Individual symbol or all symbols mini ticker
 
         24hr rolling window mini-ticker statistics.
         These are NOT the statistics of the UTC day, but a 24hr rolling window for the previous 24hrs
 
         Stream Name: <symbol>@miniTicker or
         Stream Name: !miniTicker@arr
@@ -123,21 +148,21 @@
         https://binance-docs.github.io/apidocs/futures/en/#individual-symbol-mini-ticker-stream
         https://binance-docs.github.io/apidocs/futures/en/#individual-symbol-ticker-streams
 
         Update Speed: 500ms for individual symbol, 1000ms for all market symbols
         """
 
         if symbol is None:
-            self.live_subscribe("!miniTicker@arr", id, callback, **kwargs)
+            stream_name = "!miniTicker@arr"
         else:
-            self.live_subscribe(
-                "{}@miniTicker".format(symbol.lower()), id, callback, **kwargs
-            )
+            stream_name = "{}@miniTicker".format(symbol.lower())
 
-    def ticker(self, id: int, callback, symbol=None, **kwargs):
+        self.send_message_to_server(stream_name, action=action, id=id)
+
+    def ticker(self, symbol=None, id=None, action=None, **kwargs):
         """Individual symbol or all symbols ticker
 
         24hr rolling window ticker statistics for a single symbol.
         These are NOT the statistics of the UTC day, but a 24hr rolling window from requestTime to 24hrs before.
 
         Stream Name: <symbol>@ticker or
         Stream Name: !ticker@arr
@@ -145,109 +170,101 @@
         https://binance-docs.github.io/apidocs/futures/en/#individual-symbol-ticker-streams
         https://binance-docs.github.io/apidocs/futures/en/#all-market-tickers-streams
 
         Update Speed: 500ms for individual symbol, 1000ms for all market symbols
         """
 
         if symbol is None:
-            self.live_subscribe("!ticker@arr", id, callback, **kwargs)
+            stream_name = "!ticker@arr"
         else:
-            self.live_subscribe(
-                "{}@ticker".format(symbol.lower()), id, callback, **kwargs
-            )
+            stream_name = "{}@ticker".format(symbol.lower())
+        self.send_message_to_server(stream_name, action=action, id=id)
 
-    def book_ticker(self, id: int, callback, symbol=None, **kwargs):
+    def book_ticker(self, symbol, id=None, action=None, **kwargs):
         """Individual symbol or all book ticker
 
         Pushes any update to the best bid or ask's price or quantity in real-time for a specified symbol.
 
         Stream Name: <symbol>@bookTicker or
         Stream Name: !bookTicker
 
         https://binance-docs.github.io/apidocs/futures/en/#individual-symbol-book-ticker-streams
         https://binance-docs.github.io/apidocs/futures/en/#all-book-tickers-stream
 
         Update Speed: Real-time
         """
-
         if symbol is None:
-            self.live_subscribe("!bookTicker", id, callback, **kwargs)
+            stream_name = "!bookTicker"
         else:
-            self.live_subscribe(
-                "{}@bookTicker".format(symbol.lower()), id, callback, **kwargs
-            )
+            stream_name = "{}@bookTicker".format(symbol.lower())
+        self.send_message_to_server(stream_name, action=action, id=id)
 
-    def liquidation_order(self, id: int, callback, symbol=None, **kwargs):
-        """The Liquidation Order Snapshot Streams push force liquidation order information for specific symbol.
-        The All Liquidation Order Snapshot Streams push force liquidation order information for all symbols in the market.
-
-        For each symbol，only the latest one liquidation order within 1000ms will be pushed as the snapshot. If no liquidation happens in the interval of 1000ms, no stream will be pushed.
+    def diff_book_depth(self, symbol: str, speed=100, id=None, action=None, **kwargs):
+        """Diff. Depth Stream
+        Order book price and quantity depth updates used to locally manage an order book.
 
-        Stream Name: <symbol>@forceOrder or
-        Stream Name: !forceOrder@arr
+        Stream Name: <symbol>@depth OR <symbol>@depth@500ms OR<symbol>@depth@100ms
 
-        https://binance-docs.github.io/apidocs/futures/en/#liquidation-order-streams
-        https://binance-docs.github.io/apidocs/futures/en/#all-market-liquidation-order-streams
+        https://binance-docs.github.io/apidocs/futures/en/#diff-book-depth-streams
 
-        Update Speed: 1000ms
+        Update Speed: 250ms, 500ms or 100ms
         """
-        if symbol is None:
-            self.live_subscribe("!forceOrder@arr", id, callback, **kwargs)
-        else:
-            self.live_subscribe(
-                "{}@forceOrder".format(symbol.lower()), id, callback, **kwargs
-            )
+
+        self.send_message_to_server(
+            "{}@depth@{}ms".format(symbol.lower(), speed), action=action, id=id
+        )
 
     def partial_book_depth(
-        self, symbol: str, id: int, level, speed, callback, **kwargs
+        self, symbol: str, level=5, speed=500, id=None, action=None, **kwargs
     ):
         """Partial Book Depth Streams
 
         Top bids and asks, Valid are 5, 10, or 20.
 
         Stream Names: <symbol>@depth<levels> OR <symbol>@depth<levels>@500ms OR <symbol>@depth<levels>@100ms
 
         https://binance-docs.github.io/apidocs/futures/en/#partial-book-depth-streams
 
         Update Speed: 250ms, 500ms or 100ms
         """
-
-        self.live_subscribe(
-            "{}@depth{}@{}ms".format(symbol.lower(), level, speed),
-            id,
-            callback,
-            **kwargs
+        self.send_message_to_server(
+            "{}@depth{}@{}ms".format(symbol.lower(), level, speed), id=id, action=action
         )
 
-    def diff_book_depth(self, symbol: str, id: int, speed, callback, **kwargs):
-        """Diff. Depth Stream
-        Order book price and quantity depth updates used to locally manage an order book.
+    def liquidation_order(self, symbol: str, id=None, action=None, **kwargs):
+        """The Liquidation Order Snapshot Streams push force liquidation order information for specific symbol.
+        The All Liquidation Order Snapshot Streams push force liquidation order information for all symbols in the market.
 
-        Stream Name: <symbol>@depth OR <symbol>@depth@500ms OR<symbol>@depth@100ms
+        For each symbol，only the latest one liquidation order within 1000ms will be pushed as the snapshot. If no liquidation happens in the interval of 1000ms, no stream will be pushed.
 
-        https://binance-docs.github.io/apidocs/futures/en/#diff-book-depth-streams
+        Stream Name: <symbol>@forceOrder or
+        Stream Name: !forceOrder@arr
 
-        Update Speed: 250ms, 500ms or 100ms
-        """
+        https://binance-docs.github.io/apidocs/futures/en/#liquidation-order-streams
+        https://binance-docs.github.io/apidocs/futures/en/#all-market-liquidation-order-streams
 
-        self.live_subscribe(
-            "{}@depth@{}ms".format(symbol.lower(), speed), id, callback, **kwargs
-        )
+        Update Speed: 1000ms
+        """
+        if symbol is None:
+            stream_name = "!forceOrder@arr"
+        else:
+            stream_name = "{}@forceOrder".format(symbol.lower())
+        self.send_message_to_server(stream_name, id=id, action=action)
 
-    def composite_index(self, symbol: str, id: int, callback, **kwargs):
+    def composite_index(self, symbol: str, id=None, action=None, **kwargs):
         """Composite Index Info Stream
         Composite index information for index symbols pushed every second.
 
         Stream Name: <symbol>@compositeIndex
 
         https://binance-docs.github.io/apidocs/futures/en/#composite-index-symbol-information-streams
 
         Update Speed: 1000ms
         """
 
-        self.live_subscribe(
-            "{}@compositeIndex".format(symbol.lower()), id, callback, **kwargs
+        self.send_message_to_server(
+            "{}@compositeIndex".format(symbol.lower()), id=id, action=action
         )
 
-    def user_data(self, listen_key: str, id: int, callback, **kwargs):
-        """listen to user data by provided listenkey"""
-        self.live_subscribe(listen_key, id, callback, **kwargs)
+    def user_data(self, listen_key: str, id=None, action=None, **kwargs):
+        """Listen to user data by using the provided listen_key"""
+        self.send_message_to_server(listen_key, action=action, id=id)
```

### Comparing `binance-futures-connector-3.3.1/binance_futures_connector.egg-info/PKG-INFO` & `binance-futures-connector-4.0.0rc1/binance_futures_connector.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binance-futures-connector
-Version: 3.3.1
+Version: 4.0.0rc1
 Summary: This is a lightweight library that works as a connector to Binance Futures public API.
 Home-page: https://github.com/binance/binance-futures-connector-python
 License: MIT
 Keywords: Binance futures,Public API
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
@@ -190,44 +190,74 @@
         - `error_message` - Server's error message, e.g. `Unknown order sent.`
         - `header` - Full response header.
 - `binance.error.ServerError`
     - This is thrown when server returns `5XX`, it's an issue from server side.
 
 ## Websocket
 
+### Connector v4
+
+WebSocket can be established through the following connections:
+- USD-M WebSocket Stream (`https://binance-docs.github.io/apidocs/futures/en/#websocket-market-streams`)
+- COIN-M WebSocket Stream (`https://binance-docs.github.io/apidocs/delivery/en/#websocket-market-streams`)
+
 ```python
+# WebSocket Stream Client
 import time
-from binance.websocket.cm_futures.websocket_client import CMFuturesWebsocketClient
+from binance.websocket.um_futures.websocket_client import UMFuturesWebsocketClient
 
-def message_handler(message):
-    print(message)
+def message_handler(_, message):
+    logging.info(message)
 
-ws_client = CMFuturesWebsocketClient()
-ws_client.start()
+my_client = UMFuturesWebsocketClient(on_message=message_handler)
 
-ws_client.mini_ticker(
-    symbol='bnbusdt',
-    id=1,
-    callback=message_handler,
-)
-
-# Combine selected streams
-ws_client.instant_subscribe(
-    stream=['bnbusdt@bookTicker', 'ethusdt@bookTicker'],
-    callback=message_handler,
-)
+# Subscribe to a single symbol stream
+my_client.agg_trade(symbol="bnbusdt")
+time.sleep(5)
+logging.info("closing ws connection")
+my_client.stop()
+```
 
-time.sleep(10)
+#### Request Id
 
-print("closing ws connection")
-ws_client.stop()
+Client can assign a request id to each request. The request id will be returned in the response message. Not mandatory in the library, it generates a uuid format string if not provided.
 
+```python
+# id provided by client
+my_client.agg_trade(symbol="bnbusdt", id="my_request_id")
+
+# library will generate a random uuid string
+my_client.agg_trade(symbol="bnbusdt")
 ```
+
+#### Combined Streams
+- If you set `is_combined` to `True`, `"/stream/"` will be appended to the `baseURL` to allow for Combining streams.
+- `is_combined` defaults to `False` and `"/ws/"` (raw streams) will be appended to the `baseURL`.
+
 More websocket examples are available in the `examples` folder
 
+## Websocket < v4
+
+```python
+import time
+from binance.websocket.um_futures.websocket_client import UMFuturesWebsocketClient
+
+def message_handler(message):
+    print(message)
+
+my_client = UMFuturesWebsocketClient(on_message=message_handler)
+
+# Subscribe to a single symbol stream
+my_client.agg_trade(symbol="bnbusdt")
+time.sleep(5)
+print("closing ws connection")
+my_client.stop()
+
+```
+
 ### Heartbeat
 
 Once connected, the websocket server sends a ping frame every 3 minutes and requires a response pong frame back within
 a 10 minutes period. This package handles the pong responses automatically.
 
 ## License
 MIT
```

### Comparing `binance-futures-connector-3.3.1/binance_futures_connector.egg-info/SOURCES.txt` & `binance-futures-connector-4.0.0rc1/binance_futures_connector.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -17,16 +17,14 @@
 binance/lib/utils.py
 binance/um_futures/__init__.py
 binance/um_futures/account.py
 binance/um_futures/data_stream.py
 binance/um_futures/market.py
 binance/um_futures/portfolio_margin.py
 binance/websocket/__init__.py
-binance/websocket/binance_client_factory.py
-binance/websocket/binance_client_protocol.py
 binance/websocket/binance_socket_manager.py
 binance/websocket/websocket_client.py
 binance/websocket/cm_futures/__init__.py
 binance/websocket/cm_futures/websocket_client.py
 binance/websocket/um_futures/__init__.py
 binance/websocket/um_futures/websocket_client.py
 binance_futures_connector.egg-info/PKG-INFO
```

### Comparing `binance-futures-connector-3.3.1/setup.py` & `binance-futures-connector-4.0.0rc1/setup.py`

 * *Files identical despite different names*

