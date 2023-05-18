# Comparing `tmp/tritonv2-0.9.4.tar.gz` & `tmp/tritonv2-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tritonv2-0.9.4.tar", last modified: Wed Apr 12 16:38:26 2023, max compression
+gzip compressed data, was "tritonv2-0.9.5.tar", last modified: Thu May 18 06:55:52 2023, max compression
```

## Comparing `tritonv2-0.9.4.tar` & `tritonv2-0.9.5.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-04-12 16:38:26.794211 tritonv2-0.9.4/
--rw-r--r--   0 jojo       (501) staff       (20)     2406 2023-04-12 16:38:26.794298 tritonv2-0.9.4/PKG-INFO
--rw-r--r--   0 jojo       (501) staff       (20)     1882 2023-04-12 16:38:26.000000 tritonv2-0.9.4/README.md
--rw-r--r--   0 jojo       (501) staff       (20)      713 2023-04-12 16:38:26.794707 tritonv2-0.9.4/setup.cfg
--rw-r--r--   0 jojo       (501) staff       (20)      180 2023-04-12 16:38:26.000000 tritonv2-0.9.4/setup.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-04-12 16:38:26.793222 tritonv2-0.9.4/tritonv2/
--rw-r--r--   0 jojo       (501) staff       (20)      141 2023-04-12 08:56:34.000000 tritonv2-0.9.4/tritonv2/__init__.py
--rw-r--r--   0 jojo       (501) staff       (20)      332 2023-04-12 08:56:34.000000 tritonv2-0.9.4/tritonv2/client.py
--rw-r--r--   0 jojo       (501) staff       (20)     5923 2023-04-12 08:56:34.000000 tritonv2-0.9.4/tritonv2/client_factory.py
--rw-r--r--   0 jojo       (501) staff       (20)      653 2023-04-12 08:56:34.000000 tritonv2-0.9.4/tritonv2/constants.py
--rw-r--r--   0 jojo       (501) staff       (20)      259 2023-04-12 08:56:34.000000 tritonv2-0.9.4/tritonv2/exceptions.py
--rw-r--r--   0 jojo       (501) staff       (20)    16365 2023-04-12 08:56:34.000000 tritonv2-0.9.4/tritonv2/grpc_aio_client.py
--rw-r--r--   0 jojo       (501) staff       (20)    13778 2023-04-12 08:56:34.000000 tritonv2-0.9.4/tritonv2/grpc_client.py
--rw-r--r--   0 jojo       (501) staff       (20)    19189 2023-04-12 08:56:34.000000 tritonv2-0.9.4/tritonv2/http_aio_client.py
--rw-r--r--   0 jojo       (501) staff       (20)    18307 2023-04-12 08:56:34.000000 tritonv2-0.9.4/tritonv2/http_client.py
--rw-r--r--   0 jojo       (501) staff       (20)      180 2023-04-12 08:56:34.000000 tritonv2-0.9.4/tritonv2/setup.py
--rw-r--r--   0 jojo       (501) staff       (20)     1130 2023-04-12 08:56:34.000000 tritonv2-0.9.4/tritonv2/utils.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-04-12 16:38:26.794066 tritonv2-0.9.4/tritonv2.egg-info/
--rw-r--r--   0 jojo       (501) staff       (20)     2406 2023-04-12 16:38:26.000000 tritonv2-0.9.4/tritonv2.egg-info/PKG-INFO
--rw-r--r--   0 jojo       (501) staff       (20)      470 2023-04-12 16:38:26.000000 tritonv2-0.9.4/tritonv2.egg-info/SOURCES.txt
--rw-r--r--   0 jojo       (501) staff       (20)        1 2023-04-12 16:38:26.000000 tritonv2-0.9.4/tritonv2.egg-info/dependency_links.txt
--rw-r--r--   0 jojo       (501) staff       (20)        1 2023-04-12 16:38:26.000000 tritonv2-0.9.4/tritonv2.egg-info/not-zip-safe
--rw-r--r--   0 jojo       (501) staff       (20)       73 2023-04-12 16:38:26.000000 tritonv2-0.9.4/tritonv2.egg-info/requires.txt
--rw-r--r--   0 jojo       (501) staff       (20)        9 2023-04-12 16:38:26.000000 tritonv2-0.9.4/tritonv2.egg-info/top_level.txt
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-18 06:55:52.566917 tritonv2-0.9.5/
+-rw-r--r--   0 jojo       (501) staff       (20)     2406 2023-05-18 06:55:52.566996 tritonv2-0.9.5/PKG-INFO
+-rw-r--r--   0 jojo       (501) staff       (20)     1882 2023-05-18 06:55:51.000000 tritonv2-0.9.5/README.md
+-rw-r--r--   0 jojo       (501) staff       (20)      763 2023-05-18 06:55:52.567383 tritonv2-0.9.5/setup.cfg
+-rw-r--r--   0 jojo       (501) staff       (20)      180 2023-05-18 06:55:51.000000 tritonv2-0.9.5/setup.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-18 06:55:52.565895 tritonv2-0.9.5/tritonv2/
+-rw-r--r--   0 jojo       (501) staff       (20)      141 2023-04-12 08:56:34.000000 tritonv2-0.9.5/tritonv2/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1008 2023-05-17 18:28:29.000000 tritonv2-0.9.5/tritonv2/client.py
+-rw-r--r--   0 jojo       (501) staff       (20)     6421 2023-05-17 18:34:37.000000 tritonv2-0.9.5/tritonv2/client_factory.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1246 2023-05-17 20:16:45.000000 tritonv2-0.9.5/tritonv2/constants.py
+-rw-r--r--   0 jojo       (501) staff       (20)      259 2023-04-12 08:56:34.000000 tritonv2-0.9.5/tritonv2/exceptions.py
+-rw-r--r--   0 jojo       (501) staff       (20)    16981 2023-05-17 20:12:01.000000 tritonv2-0.9.5/tritonv2/grpc_aio_client.py
+-rw-r--r--   0 jojo       (501) staff       (20)    14352 2023-05-17 19:35:44.000000 tritonv2-0.9.5/tritonv2/grpc_client.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1880 2023-05-17 19:53:45.000000 tritonv2-0.9.5/tritonv2/grpc_interceptor.py
+-rw-r--r--   0 jojo       (501) staff       (20)    30819 2023-05-17 18:27:25.000000 tritonv2-0.9.5/tritonv2/http_aio_client.py
+-rw-r--r--   0 jojo       (501) staff       (20)    29292 2023-05-17 18:28:44.000000 tritonv2-0.9.5/tritonv2/http_client.py
+-rw-r--r--   0 jojo       (501) staff       (20)      180 2023-04-12 08:56:34.000000 tritonv2-0.9.5/tritonv2/setup.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1238 2023-05-18 06:48:12.000000 tritonv2-0.9.5/tritonv2/utils.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-18 06:55:52.566796 tritonv2-0.9.5/tritonv2.egg-info/
+-rw-r--r--   0 jojo       (501) staff       (20)     2406 2023-05-18 06:55:52.000000 tritonv2-0.9.5/tritonv2.egg-info/PKG-INFO
+-rw-r--r--   0 jojo       (501) staff       (20)      499 2023-05-18 06:55:52.000000 tritonv2-0.9.5/tritonv2.egg-info/SOURCES.txt
+-rw-r--r--   0 jojo       (501) staff       (20)        1 2023-05-18 06:55:52.000000 tritonv2-0.9.5/tritonv2.egg-info/dependency_links.txt
+-rw-r--r--   0 jojo       (501) staff       (20)        1 2023-05-18 06:55:52.000000 tritonv2-0.9.5/tritonv2.egg-info/not-zip-safe
+-rw-r--r--   0 jojo       (501) staff       (20)      121 2023-05-18 06:55:52.000000 tritonv2-0.9.5/tritonv2.egg-info/requires.txt
+-rw-r--r--   0 jojo       (501) staff       (20)        9 2023-05-18 06:55:52.000000 tritonv2-0.9.5/tritonv2.egg-info/top_level.txt
```

### Comparing `tritonv2-0.9.4/PKG-INFO` & `tritonv2-0.9.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tritonv2
-Version: 0.9.4
+Version: 0.9.5
 Summary: project descriptions here
 Home-page: https://github.com/FlyTOmeLight
 Author: zhoubohan
 Author-email: zhoubohan.pro@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -17,15 +17,15 @@
 
 # tritonv2
 A client library for promote triton official client
 
 ## Installation
 
 ```bash
-pip install tritonv2==0.9.4
+pip install tritonv2==0.9.5
 ```
 
 ## Usage
 
 First, you need to create a client object.
 
 ```python
```

### Comparing `tritonv2-0.9.4/README.md` & `tritonv2-0.9.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # tritonv2
 A client library for promote triton official client
 
 ## Installation
 
 ```bash
-pip install tritonv2==0.9.4
+pip install tritonv2==0.9.5
 ```
 
 ## Usage
 
 First, you need to create a client object.
 
 ```python
```

### Comparing `tritonv2-0.9.4/setup.cfg` & `tritonv2-0.9.5/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = tritonv2
 author = zhoubohan
 author_email = zhoubohan.pro@gmail.com
-version = 0.9.4
+version = 0.9.5
 description = project descriptions here
 long_description = file: README.md
 long_description_content_type = text/markdown
 home_page = https://github.com/FlyTOmeLight
 license = MIT
 classifier = 
 	Programming Language :: Python
@@ -18,14 +18,16 @@
 [options]
 packages = find:
 install_requires = 
 	numpy>=1.23.5
 	tenacity>=8.1.0
 	tritonclient[all]>=2.25.0
 	pydantic>=1.10.2
+	pyrate-limiter>=2.10.0
+	grpc-interceptor>=0.15.1
 python_requires = >=3.7
 include_package_data = True
 zip_safe = False
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `tritonv2-0.9.4/tritonv2/client_factory.py` & `tritonv2-0.9.5/tritonv2/client_factory.py`

 * *Files 16% similar despite different names*

```diff
@@ -51,65 +51,71 @@
                            verbose=False,
                            ssl=None,
                            authority="",
                            root_certificates="",
                            private_key="",
                            certificate_chain="",
                            creds=None,
-                           keepalive_options=None
+                           keepalive_options=None,
+                           limiter_config=None
                            ):
         channel_args = _build_grpc_retry_channel_args(num_retries, max_interval_secs, base_interval_secs)
         return TritonGRPCClient(server_url=server_url,
                                 verbose=verbose,
                                 channel_args=channel_args,
                                 ssl=ssl,
                                 authority=authority,
                                 root_certificates=root_certificates,
                                 private_key=private_key,
                                 certificate_chain=certificate_chain,
                                 creds=creds,
-                                keepalive_options=keepalive_options)
+                                keepalive_options=keepalive_options,
+                                limiter_config=limiter_config)
 
     @staticmethod
     def create_grpc_aio_client(server_url,
                                num_retries=3,
                                max_interval_secs=20,
                                base_interval_secs=0.3,
                                verbose=False,
                                ssl=None,
                                authority="",
                                root_certificates="",
                                private_key="",
                                certificate_chain="",
                                creds=None,
-                               keepalive_options=None):
+                               keepalive_options=None,
+                               limiter_config=None
+                               ):
         channel_args = _build_grpc_retry_channel_args(num_retries, max_interval_secs, base_interval_secs)
         return TritonAioGRPCClient(server_url=server_url,
-                                verbose=verbose,
-                                channel_args=channel_args,
-                                ssl=ssl,
-                                authority=authority,
-                                root_certificates=root_certificates,
-                                private_key=private_key,
-                                certificate_chain=certificate_chain,
-                                creds=creds,
-                                keepalive_options=keepalive_options)
+                                   verbose=verbose,
+                                   channel_args=channel_args,
+                                   ssl=ssl,
+                                   authority=authority,
+                                   root_certificates=root_certificates,
+                                   private_key=private_key,
+                                   certificate_chain=certificate_chain,
+                                   creds=creds,
+                                   keepalive_options=keepalive_options,
+                                   limiter_config=limiter_config)
 
     @staticmethod
     def create_http_client(
             server_url,
             verbose=False,
             concurrency=1,
             connection_timeout=60.0,
             network_timeout=60.0,
             max_greenlets=None,
             ssl=False,
             ssl_options=None,
             ssl_context_factory=None,
-            insecure=False):
+            insecure=False,
+            limiter_config=None):
         """
         Parameters
         :param server_url:
         :param verbose:
         :param concurrency:
         :param connection_timeout:
         :param network_timeout:
@@ -125,33 +131,36 @@
                                 concurrency=concurrency,
                                 connection_timeout=connection_timeout,
                                 network_timeout=network_timeout,
                                 max_greenlets=max_greenlets,
                                 ssl=ssl,
                                 ssl_options=ssl_options,
                                 ssl_context_factory=ssl_context_factory,
-                                insecure=insecure)
+                                insecure=insecure,
+                                limiter_config=limiter_config)
 
     @staticmethod
     def create_http_aio_client(
             server_url,
             verbose=False,
             conn_limit=100,
             conn_timeout=60.0,
             ssl=False,
-            ssl_context=None):
+            ssl_context=None,
+            limiter_config=None):
         """
         Parameters
         :param server_url:
         :param verbose:
         :param conn_limit:
         :param conn_timeout:
         :param ssl:
         :param ssl_context:
         :return:
         """
         return TritonAioHTTPClient(server_url=server_url,
-                                verbose=verbose,
-                                conn_limit=conn_limit,
-                                conn_timeout=conn_timeout,
-                                ssl=ssl,
-                                ssl_context=ssl_context)
+                                   verbose=verbose,
+                                   conn_limit=conn_limit,
+                                   conn_timeout=conn_timeout,
+                                   ssl=ssl,
+                                   ssl_context=ssl_context,
+                                   limiter_config=limiter_config)
```

### Comparing `tritonv2-0.9.4/tritonv2/grpc_aio_client.py` & `tritonv2-0.9.5/tritonv2/grpc_aio_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,22 @@
 # -*- coding: UTF-8 -*-
 #
 # Copyright (c) 2022 Baidu.com, Inc. All Rights Reserved
 """
 triton aio grpc client
 """
 import tritonclient.grpc.aio as grpc_client
+from tritonclient.grpc import service_pb2_grpc
+import grpc
+
 from .client import TritonClient
 from .utils import parse_model
 from .exceptions import TritonClientException
+from .constants import LimiterConfig
+from .grpc_interceptor import async_rate_limit_interceptor
 
 
 class TritonAioGRPCClient(TritonClient):
     """
     Concrete implementation of TritonClient
     for GRPC AIO
     """
@@ -23,28 +28,29 @@
                  verbose=False,
                  ssl=False,
                  authority="",
                  root_certificates="",
                  private_key="",
                  certificate_chain="",
                  creds=None,
-                 keepalive_options=None):
+                 keepalive_options=None,
+                 limiter_config: LimiterConfig = None):
         """
         Parameters
         :param server_url:
         :param channel_args:
         :param ssl:
         :param root_certificates:
         :param private_key:
         :param certificate_chain:
         :param creds:
         :param keepalive_options:
         """
 
-        super().__init__()
+        super().__init__(limiter_config)
 
         if keepalive_options is None:
             keepalive_options = grpc_client.KeepAliveOptions()
 
         channel_args.append(("grpc.max_send_message_length", grpc_client.MAX_GRPC_MESSAGE_SIZE))
         channel_args.append(("grpc.max_receive_message_length", grpc_client.MAX_GRPC_MESSAGE_SIZE))
         channel_args.append(("grpc.keepalive_time_ms", keepalive_options.keepalive_time_ms))
@@ -65,14 +71,24 @@
             private_key=private_key,
             certificate_chain=certificate_chain,
             creds=creds,
             keepalive_options=keepalive_options,
             channel_args=channel_args,
         )
 
+        self._client._channel = grpc.aio.insecure_channel(server_url, options=channel_args, interceptors=[async_rate_limit_interceptor(
+            self._identifier,
+            self._limiter,
+            self._limiter_delay,
+            self._limiter_max_delay,
+        )])
+
+        self._client._client_stub = service_pb2_grpc.GRPCInferenceServiceStub(
+            self._client._channel)
+
     async def close(self):
         """
         Close the client
         :return:
         """
         await self._client.close()
```

### Comparing `tritonv2-0.9.4/tritonv2/grpc_client.py` & `tritonv2-0.9.5/tritonv2/grpc_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,18 +2,22 @@
 # -*- coding: UTF-8 -*-
 #
 # Copyright (c) 2022 Baidu.com, Inc. All Rights Reserved
 """
 triton grpc client
 """
 import tritonclient.grpc as grpc_client
+from tritonclient.grpc import service_pb2_grpc
+import grpc
 
 from .client import TritonClient
 from .exceptions import TritonClientException
 from .utils import parse_model
+from .constants import LimiterConfig
+from .grpc_interceptor import rate_limit_interceptor
 
 
 class TritonGRPCClient(TritonClient):
     """
     Concrete implementation of TritonClient
     for GRPC
     """
@@ -24,28 +28,29 @@
                  verbose=False,
                  ssl=False,
                  authority="",
                  root_certificates="",
                  private_key="",
                  certificate_chain="",
                  creds=None,
-                 keepalive_options=None):
+                 keepalive_options=None,
+                 limiter_config: LimiterConfig = None):
         """
         Parameters
         :param server_url:
         :param channel_args:
         :param ssl:
         :param root_certificates:
         :param private_key:
         :param certificate_chain:
         :param creds:
         :param keepalive_options:
         """
 
-        super().__init__()
+        super().__init__(limiter_config)
 
         if keepalive_options is None:
             keepalive_options = grpc_client.KeepAliveOptions()
 
         channel_args.append(("grpc.max_send_message_length", grpc_client.MAX_GRPC_MESSAGE_SIZE))
         channel_args.append(("grpc.max_receive_message_length", grpc_client.MAX_GRPC_MESSAGE_SIZE))
         channel_args.append(("grpc.keepalive_time_ms", keepalive_options.keepalive_time_ms))
@@ -66,14 +71,23 @@
             private_key=private_key,
             certificate_chain=certificate_chain,
             creds=creds,
             keepalive_options=keepalive_options,
             channel_args=channel_args,
         )
 
+        self._client._channel = grpc.intercept_channel(self._client.channel, *[rate_limit_interceptor(
+            self._identifier,
+            self._limiter,
+            self._limiter_delay,
+            self._limiter_max_delay,
+        )])
+        self._client._client_stub = service_pb2_grpc.GRPCInferenceServiceStub(
+            self._client.channel)
+
     def model_infer(self,
                     model_name,
                     inputs,
                     model_version="",
                     outputs=None,
                     request_id="",
                     sequence_id=0,
```

### Comparing `tritonv2-0.9.4/tritonv2/http_client.py` & `tritonv2-0.9.5/tritonv2/http_client.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from tenacity import retry, stop_after_attempt, stop_after_delay, wait_fixed
 import tritonclient.http as http_client
 
 from .client import TritonClient
 from .exceptions import TritonClientException
 from .utils import parse_model
+from .constants import LimiterConfig
 
 NUMBER_RETRIES = 3
 MAX_INTERVAL_SECS = 20
 BASE_INTERVAL_SECS = 0.3
 
 
 class TritonHTTPClient(TritonClient):
@@ -30,29 +31,31 @@
                  concurrency=1,
                  connection_timeout=60.0,
                  network_timeout=60.0,
                  max_greenlets=None,
                  ssl=False,
                  ssl_options=None,
                  ssl_context_factory=None,
-                 insecure=False):
+                 insecure=False,
+                 limiter_config: LimiterConfig = None):
         """
         Parameters
         :param server_url:
         :param verbose:
         :param concurrency:
         :param connection_timeout:
         :param network_timeout:
         :param max_greenlets:
         :param ssl:
         :param ssl_options:
         :param ssl_context_factory:
         :param insecure:
+        :param request_rate:
         """
-        super().__init__()
+        super().__init__(limiter_config)
 
         self._client = http_client.InferenceServerClient(
             url=server_url,
             verbose=verbose,
             concurrency=concurrency,
             connection_timeout=connection_timeout,
             network_timeout=network_timeout,
@@ -68,14 +71,19 @@
         """
         check if the server is ready
         :param headers:
         :param query_params:
         :return:
         """
         try:
+            if self._limiter is not None:
+                with self._limiter.ratelimit(self._identifier,
+                                             delay=self._limiter_delay,
+                                             max_delay=self._limiter_max_delay):
+                    return self._client.is_server_ready(headers=headers, query_params=query_params)
             return self._client.is_server_ready(headers=headers, query_params=query_params)
         except Exception as e:
             raise TritonClientException(
                 "Failed to check server ready: {}".format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
@@ -83,28 +91,40 @@
         """
         check if the server live
         :param headers:
         :param query_params:
         :return:
         """
         try:
-            return self._client.is_server_live(headers=headers, query_params=query_params)
+            if self._limiter is not None:
+                with self._limiter.ratelimit(self._identifier,
+                                             delay=self._limiter_delay,
+                                             max_delay=self._limiter_max_delay):
+                    return self._client.is_server_live(headers=headers, query_params=query_params)
+            else:
+                return self._client.is_server_live(headers=headers, query_params=query_params)
         except Exception as e:
             raise TritonClientException('Failed to check server live: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     def server_meta(self, headers=None, query_params=None):
         """
         get server metadata
         Returns
         :return:
         """
         try:
-            return self._client.get_server_metadata(headers=headers, query_params=query_params)
+            if self._limiter is not None:
+                with self._limiter.ratelimit(self._identifier,
+                                             delay=self._limiter_delay,
+                                             max_delay=self._limiter_max_delay):
+                    return self._client.get_server_metadata(headers=headers, query_params=query_params)
+            else:
+                return self._client.get_server_metadata(headers=headers, query_params=query_params)
         except Exception as e:
             raise TritonClientException('Failed to get server meta: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     def model_ready(self, model_name, model_version="", headers=None, query_params=None):
         """
@@ -112,15 +132,23 @@
         :param model_name:
         :param model_version:
         :param headers:
         :param query_params:
         :return:
         """
         try:
-            return self._client.is_model_ready(model_name, model_version, headers=headers, query_params=query_params)
+            if self._limiter is not None:
+                with self._limiter.ratelimit(self._identifier,
+                                             delay=self._limiter_delay,
+                                             max_delay=self._limiter_max_delay):
+                    return self._client.is_model_ready(model_name, model_version, headers=headers,
+                                                       query_params=query_params)
+            else:
+                return self._client.is_model_ready(model_name, model_version, headers=headers,
+                                                   query_params=query_params)
         except Exception as e:
             raise TritonClientException('Failed to get model ready: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     def model_meta(self, model_name, model_version="", headers=None, query_params=None):
         """
@@ -129,16 +157,23 @@
         :param model_name:
         :param model_version:
         :param headers:
         :param query_params:
         :return:
         """
         try:
-            return self._client.get_model_metadata(model_name, model_version, headers=headers,
-                                                   query_params=query_params)
+            if self._limiter is not None:
+                with self._limiter.ratelimit(self._identifier,
+                                             delay=self._limiter_delay,
+                                             max_delay=self._limiter_max_delay):
+                    return self._client.get_model_metadata(model_name, model_version, headers=headers,
+                                                           query_params=query_params)
+            else:
+                return self._client.get_model_metadata(model_name, model_version, headers=headers,
+                                                       query_params=query_params)
         except Exception as e:
             raise TritonClientException('Failed to get model meta: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     def model_config(self, model_name, model_version="", headers=None, query_params=None):
         """
@@ -147,15 +182,23 @@
         :param model_name:
         :param model_version:
         :param headers:
         :param query_params:
         :return:
         """
         try:
-            return self._client.get_model_config(model_name, model_version, headers=headers, query_params=query_params)
+            if self._limiter is not None:
+                with self._limiter.ratelimit(self._identifier,
+                                             delay=self._limiter_delay,
+                                             max_delay=self._limiter_max_delay):
+                    return self._client.get_model_config(model_name, model_version, headers=headers,
+                                                         query_params=query_params)
+            else:
+                return self._client.get_model_config(model_name, model_version, headers=headers,
+                                                     query_params=query_params)
         except Exception as e:
             raise TritonClientException('Failed to get model config: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     def model_infer(self,
                     model_name,
@@ -188,29 +231,49 @@
         :param query_params:
         :param request_compression_algorithm:
         :param response_compression_algorithm:
         :return:
         """
 
         try:
-            return self._client.infer(
-                model_name=model_name,
-                inputs=inputs,
-                model_version=model_version,
-                outputs=outputs,
-                request_id=request_id,
-                sequence_id=sequence_id,
-                sequence_start=sequence_start,
-                sequence_end=sequence_end,
-                priority=priority,
-                timeout=timeout,
-                headers=headers,
-                query_params=query_params,
-                request_compression_algorithm=request_compression_algorithm,
-                response_compression_algorithm=response_compression_algorithm)
+            if self._limiter is not None:
+                with self._limiter.ratelimit(self._identifier,
+                                             delay=self._limiter_delay,
+                                             max_delay=self._limiter_max_delay):
+                    return self._client.infer(
+                        model_name=model_name,
+                        inputs=inputs,
+                        model_version=model_version,
+                        outputs=outputs,
+                        request_id=request_id,
+                        sequence_id=sequence_id,
+                        sequence_start=sequence_start,
+                        sequence_end=sequence_end,
+                        priority=priority,
+                        timeout=timeout,
+                        headers=headers,
+                        query_params=query_params,
+                        request_compression_algorithm=request_compression_algorithm,
+                        response_compression_algorithm=response_compression_algorithm)
+            else:
+                return self._client.infer(
+                    model_name=model_name,
+                    inputs=inputs,
+                    model_version=model_version,
+                    outputs=outputs,
+                    request_id=request_id,
+                    sequence_id=sequence_id,
+                    sequence_start=sequence_start,
+                    sequence_end=sequence_end,
+                    priority=priority,
+                    timeout=timeout,
+                    headers=headers,
+                    query_params=query_params,
+                    request_compression_algorithm=request_compression_algorithm,
+                    response_compression_algorithm=response_compression_algorithm)
         except Exception as e:
             raise TritonClientException('Failed to model infer: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     def model_statistics(self, model_name, model_version="", headers=None, query_params=None):
         """
@@ -218,30 +281,43 @@
         :param model_name:
         :param model_version:
         :param headers:
         :param query_params:
         :return:
         """
         try:
-            return self._client.get_inference_statistics(model_name, model_version, headers=headers,
-                                                         query_params=query_params)
+            if self._limiter is not None:
+                with self._limiter.ratelimit(self._identifier,
+                                             delay=self._limiter_delay,
+                                             max_delay=self._limiter_max_delay):
+                    return self._client.get_inference_statistics(model_name, model_version, headers=headers,
+                                                                 query_params=query_params)
+            else:
+                return self._client.get_inference_statistics(model_name, model_version, headers=headers,
+                                                             query_params=query_params)
         except Exception as e:
             raise TritonClientException('Failed to get model statistics: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     def repository_index(self, headers=None, query_params=None):
         """
         get repository index
         :param headers:
         :param query_params:
         :return:
         """
         try:
-            return self._client.get_model_repository_index(headers=headers, query_params=query_params)
+            if self._limiter is not None:
+                with self._limiter.ratelimit(self._identifier,
+                                             delay=self._limiter_delay,
+                                             max_delay=self._limiter_max_delay):
+                    return self._client.get_model_repository_index(headers=headers, query_params=query_params)
+            else:
+                return self._client.get_model_repository_index(headers=headers, query_params=query_params)
         except Exception as e:
             raise TritonClientException('Failed to get repository index: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     def repository_model_load(self, model_name, headers=None, query_params=None, config="", files=None):
         """
@@ -250,19 +326,30 @@
         :param headers:
         :param query_params:
         :param config:
         :param files:
         :return:
         """
         try:
-            return self._client.load_model(model_name=model_name,
-                                           headers=headers,
-                                           query_params=query_params,
-                                           config=config,
-                                           files=files)
+            if self._limiter is not None:
+                with self._limiter.ratelimit(self._identifier,
+                                             delay=self._limiter_delay,
+                                             max_delay=self._limiter_max_delay):
+                    return self._client.load_model(model_name=model_name,
+                                                   headers=headers,
+                                                   query_params=query_params,
+                                                   config=config,
+                                                   files=files)
+
+            else:
+                return self._client.load_model(model_name=model_name,
+                                               headers=headers,
+                                               query_params=query_params,
+                                               config=config,
+                                               files=files)
         except Exception as e:
             raise TritonClientException('Failed to load model: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     def repository_model_unload(self, model_name, headers=None, query_params=None, unload_dependents=False):
         """
@@ -270,34 +357,50 @@
         :param model_name:
         :param headers:
         :param query_params:
         :param unload_dependents:
         :return:
         """
         try:
-            return self._client.unload_model(model_name=model_name,
-                                             headers=headers,
-                                             query_params=query_params,
-                                             unload_dependents=unload_dependents)
+            if self._limiter is not None:
+                with self._limiter.ratelimit(self._identifier,
+                                             delay=self._limiter_delay,
+                                             max_delay=self._limiter_max_delay):
+                    return self._client.unload_model(model_name=model_name,
+                                                     headers=headers,
+                                                     query_params=query_params,
+                                                     unload_dependents=unload_dependents)
+            else:
+                return self._client.unload_model(model_name=model_name,
+                                                 headers=headers,
+                                                 query_params=query_params,
+                                                 unload_dependents=unload_dependents)
         except Exception as e:
             raise TritonClientException('Failed to unload model: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     def system_shared_memory_status(self, region_name="", headers=None, query_params=None):
         """
         get system shared memory status
         :param region_name:
         :param headers:
         :param query_params:
         :return:
         """
         try:
-            return self._client.get_system_shared_memory_status(region_name=region_name, headers=headers,
-                                                                query_params=query_params)
+            if self._limiter is not None:
+                with self._limiter.ratelimit(self._identifier,
+                                             delay=self._limiter_delay,
+                                             max_delay=self._limiter_max_delay):
+                    return self._client.get_system_shared_memory_status(region_name=region_name, headers=headers,
+                                                                        query_params=query_params)
+            else:
+                return self._client.get_system_shared_memory_status(region_name=region_name, headers=headers,
+                                                                    query_params=query_params)
         except Exception as e:
             raise TritonClientException('Failed to get system shared memory status: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     def system_shared_memory_register(self, name, key, byte_size, offset=0, headers=None, query_params=None):
         """
@@ -307,54 +410,81 @@
         :param byte_size:
         :param offset:
         :param headers:
         :param query_params:
         :return:
         """
         try:
-            return self._client.register_system_shared_memory(name=name,
-                                                              key=key,
-                                                              byte_size=byte_size,
-                                                              offset=offset,
-                                                              headers=headers,
-                                                              query_params=query_params)
+            if self._limiter is not None:
+                with self._limiter.ratelimit(self._identifier,
+                                             delay=self._limiter_delay,
+                                             max_delay=self._limiter_max_delay):
+                    return self._client.register_system_shared_memory(name=name,
+                                                                      key=key,
+                                                                      byte_size=byte_size,
+                                                                      offset=offset,
+                                                                      headers=headers,
+                                                                      query_params=query_params)
+            else:
+                return self._client.register_system_shared_memory(name=name,
+                                                                  key=key,
+                                                                  byte_size=byte_size,
+                                                                  offset=offset,
+                                                                  headers=headers,
+                                                                  query_params=query_params)
         except Exception as e:
             raise TritonClientException('Failed to register system shared memory: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     def system_shared_memory_unregister(self, name, headers=None, query_params=None):
         """
         unregister system shared memory
         :param name:
         :param headers:
         :param query_params:
         :return:
         """
         try:
-            return self._client.unregister_system_shared_memory(name=name,
-                                                                headers=headers,
-                                                                query_params=query_params)
+            if self._limiter is not None:
+                with self._limiter.ratelimit(self._identifier,
+                                             delay=self._limiter_delay,
+                                             max_delay=self._limiter_max_delay):
+                    return self._client.unregister_system_shared_memory(name=name,
+                                                                        headers=headers,
+                                                                        query_params=query_params)
+            else:
+                return self._client.unregister_system_shared_memory(name=name,
+                                                                    headers=headers,
+                                                                    query_params=query_params)
         except Exception as e:
             raise TritonClientException('Failed to unregister system shared memory: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     def cuda_shared_memory_status(self, region_name="", headers=None, query_params=None):
         """
         get cuda shared memory status
         :param region_name:
         :param headers:
         :param query_params:
         :return:
         """
         try:
-            return self._client.get_cuda_shared_memory_status(region_name=region_name,
-                                                              headers=headers,
-                                                              query_params=query_params)
+            if self._limiter is not None:
+                with self._limiter.ratelimit(self._identifier,
+                                             delay=self._limiter_delay,
+                                             max_delay=self._limiter_max_delay):
+                    return self._client.get_cuda_shared_memory_status(region_name=region_name,
+                                                                      headers=headers,
+                                                                      query_params=query_params)
+            else:
+                return self._client.get_cuda_shared_memory_status(region_name=region_name,
+                                                                  headers=headers,
+                                                                  query_params=query_params)
         except Exception as e:
             raise TritonClientException('Failed to get cuda shared memory status: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     def cuda_shared_memory_register(self, name, raw_handle, byte_size, device_id, headers=None, query_params=None):
         """
@@ -364,37 +494,56 @@
         :param byte_size:
         :param device_id:
         :param headers:
         :param query_params:
         :return:
         """
         try:
-            return self._client.register_cuda_shared_memory(name=name,
-                                                            raw_handle=raw_handle,
-                                                            device_id=device_id,
-                                                            byte_size=byte_size,
-                                                            headers=headers,
-                                                            query_params=query_params)
+            if self._limiter is not None:
+                with self._limiter.ratelimit(self._identifier,
+                                             delay=self._limiter_delay,
+                                             max_delay=self._limiter_max_delay):
+                    return self._client.register_cuda_shared_memory(name=name,
+                                                                    raw_handle=raw_handle,
+                                                                    device_id=device_id,
+                                                                    byte_size=byte_size,
+                                                                    headers=headers,
+                                                                    query_params=query_params)
+            else:
+                return self._client.register_cuda_shared_memory(name=name,
+                                                                raw_handle=raw_handle,
+                                                                device_id=device_id,
+                                                                byte_size=byte_size,
+                                                                headers=headers,
+                                                                query_params=query_params)
         except Exception as e:
             raise TritonClientException('Failed to register cuda shared memory: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     def cuda_shared_memory_unregister(self, name, headers=None, query_params=None):
         """
         unregister cuda shared memory
         :param name:
         :param headers:
         :param query_params:
         :return:
         """
         try:
-            return self._client.unregister_cuda_shared_memory(name=name,
-                                                              headers=headers,
-                                                              query_params=query_params)
+            if self._limiter is not None:
+                with self._limiter.ratelimit(self._identifier,
+                                             delay=self._limiter_delay,
+                                             max_delay=self._limiter_max_delay):
+                    return self._client.unregister_cuda_shared_memory(name=name,
+                                                                      headers=headers,
+                                                                      query_params=query_params)
+            else:
+                return self._client.unregister_cuda_shared_memory(name=name,
+                                                                  headers=headers,
+                                                                  query_params=query_params)
         except Exception as e:
             raise TritonClientException('Failed to  unregister cuda shared memory: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     def trace_setting(self, model_name="", settings=None, headers=None, query_params=None):
         """
@@ -404,35 +553,52 @@
         :param headers:
         :param query_params:
         :return:
         """
         try:
             if settings is None:
                 settings = {}
-            return self._client.update_trace_settings(model_name=model_name,
-                                                      settings=settings,
-                                                      headers=headers,
-                                                      query_params=query_params)
+            if self._limiter is not None:
+                with self._limiter.ratelimit(self._identifier,
+                                             delay=self._limiter_delay,
+                                             max_delay=self._limiter_max_delay):
+                    return self._client.update_trace_settings(model_name=model_name,
+                                                              settings=settings,
+                                                              headers=headers,
+                                                              query_params=query_params)
+            else:
+                return self._client.update_trace_settings(model_name=model_name,
+                                                          settings=settings,
+                                                          headers=headers,
+                                                          query_params=query_params)
         except Exception as e:
             raise TritonClientException('Failed to update trace setting: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     def get_trace_settings(self, model_name="", headers=None, query_params=None):
         """
         get_trace_settings
         :param model_name:
         :param headers:
         :param query_params:
         :return:
         """
         try:
-            return self._client.get_trace_settings(model_name=model_name,
-                                                   headers=headers,
-                                                   query_params=query_params)
+            if self._limiter is not None:
+                with self._limiter.ratelimit(self._identifier,
+                                             delay=self._limiter_delay,
+                                             max_delay=self._limiter_max_delay):
+                    return self._client.get_trace_settings(model_name=model_name,
+                                                           headers=headers,
+                                                           query_params=query_params)
+            else:
+                return self._client.get_trace_settings(model_name=model_name,
+                                                       headers=headers,
+                                                       query_params=query_params)
         except Exception as e:
             raise TritonClientException('Failed to get trace settings: {}'.format(e)) from None
 
     def get_inputs_and_outputs_detail(self, model_name, model_version):
         """
         get inputs and outputs detail
         :param model_name:
```

### Comparing `tritonv2-0.9.4/tritonv2/utils.py` & `tritonv2-0.9.5/tritonv2/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 # !/usr/bin/env python3
 # -*- coding: UTF-8 -*-
 #
 # Copyright (c) 2022 Baidu.com, Inc. All Rights Reserved
 """
 triton client utils
 """
+import uuid
+
 import numpy as np
 
 
+def gen_unique_id():
+    """
+    Generate unique id
+    """
+    return str(uuid.uuid4().hex)
+
+
 def list_stack_ndarray(arrays) -> np.ndarray:
     """
     Convert list of ndarrays to single ndarray with ndims+=1
     """
     lengths = list(
         map(lambda x, a=arrays: a[x].shape[0], [x for x in range(len(arrays))])
     )
```

### Comparing `tritonv2-0.9.4/tritonv2.egg-info/PKG-INFO` & `tritonv2-0.9.5/tritonv2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tritonv2
-Version: 0.9.4
+Version: 0.9.5
 Summary: project descriptions here
 Home-page: https://github.com/FlyTOmeLight
 Author: zhoubohan
 Author-email: zhoubohan.pro@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -17,15 +17,15 @@
 
 # tritonv2
 A client library for promote triton official client
 
 ## Installation
 
 ```bash
-pip install tritonv2==0.9.4
+pip install tritonv2==0.9.5
 ```
 
 ## Usage
 
 First, you need to create a client object.
 
 ```python
```

