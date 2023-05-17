# Comparing `tmp/lanarky-0.6.0.tar.gz` & `tmp/lanarky-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lanarky-0.6.0.tar", max compression
+gzip compressed data, was "lanarky-0.6.1.tar", max compression
```

## Comparing `lanarky-0.6.0.tar` & `lanarky-0.6.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1073 2023-05-14 15:19:56.923642 lanarky-0.6.0/LICENSE
--rw-r--r--   0        0        0     3493 2023-05-14 15:19:56.923642 lanarky-0.6.0/README.md
--rw-r--r--   0        0        0        0 2023-05-14 15:19:57.127642 lanarky-0.6.0/lanarky/__init__.py
--rw-r--r--   0        0        0     2310 2023-05-14 15:19:57.127642 lanarky-0.6.0/lanarky/callbacks/__init__.py
--rw-r--r--   0        0        0      940 2023-05-14 15:19:57.127642 lanarky-0.6.0/lanarky/callbacks/base.py
--rw-r--r--   0        0        0     1360 2023-05-14 15:19:57.127642 lanarky-0.6.0/lanarky/callbacks/llm.py
--rw-r--r--   0        0        0     2675 2023-05-14 15:19:57.127642 lanarky-0.6.0/lanarky/callbacks/qa_with_sources.py
--rw-r--r--   0        0        0     2853 2023-05-14 15:19:57.127642 lanarky-0.6.0/lanarky/callbacks/retrieval_qa.py
--rw-r--r--   0        0        0     1332 2023-05-14 15:19:57.127642 lanarky-0.6.0/lanarky/register.py
--rw-r--r--   0        0        0       74 2023-05-14 15:19:57.127642 lanarky-0.6.0/lanarky/responses/__init__.py
--rw-r--r--   0        0        0     2771 2023-05-14 15:19:57.127642 lanarky-0.6.0/lanarky/responses/streaming.py
--rw-r--r--   0        0        0      536 2023-05-14 15:19:57.127642 lanarky-0.6.0/lanarky/schemas.py
--rw-r--r--   0        0        0       69 2023-05-14 15:19:57.127642 lanarky-0.6.0/lanarky/testing/__init__.py
--rw-r--r--   0        0        0     3212 2023-05-14 15:19:57.127642 lanarky-0.6.0/lanarky/testing/gradio.py
--rw-r--r--   0        0        0      391 2023-05-14 15:19:57.127642 lanarky-0.6.0/lanarky/testing/settings.py
--rw-r--r--   0        0        0       73 2023-05-14 15:19:57.127642 lanarky-0.6.0/lanarky/websockets/__init__.py
--rw-r--r--   0        0        0     3608 2023-05-14 15:19:57.127642 lanarky-0.6.0/lanarky/websockets/base.py
--rw-r--r--   0        0        0      696 2023-05-14 15:19:57.127642 lanarky-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     4279 1970-01-01 00:00:00.000000 lanarky-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-17 22:56:39.574827 lanarky-0.6.1/LICENSE
+-rw-r--r--   0        0        0     3493 2023-05-17 22:56:39.574827 lanarky-0.6.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-17 22:56:39.758830 lanarky-0.6.1/lanarky/__init__.py
+-rw-r--r--   0        0        0     2867 2023-05-17 22:56:39.758830 lanarky-0.6.1/lanarky/callbacks/__init__.py
+-rw-r--r--   0        0        0      940 2023-05-17 22:56:39.758830 lanarky-0.6.1/lanarky/callbacks/base.py
+-rw-r--r--   0        0        0     1360 2023-05-17 22:56:39.758830 lanarky-0.6.1/lanarky/callbacks/llm.py
+-rw-r--r--   0        0        0     2675 2023-05-17 22:56:39.758830 lanarky-0.6.1/lanarky/callbacks/qa_with_sources.py
+-rw-r--r--   0        0        0     2853 2023-05-17 22:56:39.758830 lanarky-0.6.1/lanarky/callbacks/retrieval_qa.py
+-rw-r--r--   0        0        0     1332 2023-05-17 22:56:39.758830 lanarky-0.6.1/lanarky/register.py
+-rw-r--r--   0        0        0       74 2023-05-17 22:56:39.758830 lanarky-0.6.1/lanarky/responses/__init__.py
+-rw-r--r--   0        0        0     2771 2023-05-17 22:56:39.758830 lanarky-0.6.1/lanarky/responses/streaming.py
+-rw-r--r--   0        0        0      536 2023-05-17 22:56:39.758830 lanarky-0.6.1/lanarky/schemas.py
+-rw-r--r--   0        0        0       69 2023-05-17 22:56:39.758830 lanarky-0.6.1/lanarky/testing/__init__.py
+-rw-r--r--   0        0        0     3212 2023-05-17 22:56:39.758830 lanarky-0.6.1/lanarky/testing/gradio.py
+-rw-r--r--   0        0        0      391 2023-05-17 22:56:39.758830 lanarky-0.6.1/lanarky/testing/settings.py
+-rw-r--r--   0        0        0       73 2023-05-17 22:56:39.758830 lanarky-0.6.1/lanarky/websockets/__init__.py
+-rw-r--r--   0        0        0     3608 2023-05-17 22:56:39.758830 lanarky-0.6.1/lanarky/websockets/base.py
+-rw-r--r--   0        0        0      696 2023-05-17 22:56:39.758830 lanarky-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     4279 1970-01-01 00:00:00.000000 lanarky-0.6.1/PKG-INFO
```

### Comparing `lanarky-0.6.0/LICENSE` & `lanarky-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lanarky-0.6.0/README.md` & `lanarky-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `lanarky-0.6.0/lanarky/callbacks/__init__.py` & `lanarky-0.6.1/lanarky/callbacks/qa_with_sources.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,96 @@
-from langchain.chains.base import Chain
+from lanarky.register import register_streaming_callback, register_websocket_callback
 
-from lanarky.register import STREAMING_CALLBACKS, WEBSOCKET_CALLBACKS
-
-from .base import AsyncStreamingResponseCallback, AsyncWebsocketCallback
-from .llm import (
-    AsyncConversationChainStreamingCallback,
-    AsyncConversationChainWebsocketCallback,
-    AsyncLLMChainStreamingCallback,
-    AsyncLLMChainWebsocketCallback,
-)
-from .qa_with_sources import (
-    AsyncConversationalRetrievalChainStreamingCallback,
-    AsyncConversationalRetrievalChainWebsocketCallback,
-    AsyncQAWithSourcesChainStreamingCallback,
-    AsyncQAWithSourcesChainWebsocketCallback,
-    AsyncRetrievalQAWithSourcesChainStreamingCallback,
-    AsyncRetrievalQAWithSourcesChainWebsocketCallback,
-    AsyncVectorDBQAWithSourcesChainStreamingCallback,
-    AsyncVectorDBQAWithSourcesChainWebsocketCallback,
-)
 from .retrieval_qa import (
-    AsyncRetrievalQAStreamingCallback,
-    AsyncRetrievalQAWebsocketCallback,
-    AsyncVectorDBQAStreamingCallback,
-    AsyncVectorDBQAWebsocketCallback,
+    AsyncBaseRetrievalQAStreamingCallback,
+    AsyncBaseRetrievalQAWebsocketCallback,
 )
 
-__all__ = [
-    "AsyncLLMChainStreamingCallback",
-    "AsyncLLMChainWebsocketCallback",
-    "AsyncConversationChainStreamingCallback",
-    "AsyncConversationChainWebsocketCallback",
-    "AsyncRetrievalQAStreamingCallback",
-    "AsyncRetrievalQAWebsocketCallback",
-    "AsyncVectorDBQAStreamingCallback",
-    "AsyncVectorDBQAWebsocketCallback",
-    "AsyncQAWithSourcesChainStreamingCallback",
-    "AsyncQAWithSourcesChainWebsocketCallback",
-    "AsyncRetrievalQAWithSourcesChainStreamingCallback",
-    "AsyncRetrievalQAWithSourcesChainWebsocketCallback",
-    "AsyncVectorDBQAWithSourcesChainStreamingCallback",
-    "AsyncVectorDBQAWithSourcesChainWebsocketCallback",
-    "AsyncConversationalRetrievalChainStreamingCallback",
-    "AsyncConversationalRetrievalChainWebsocketCallback",
-]
-
-
-def get_streaming_callback(
-    chain: Chain, *args, **kwargs
-) -> AsyncStreamingResponseCallback:
-    """Get the streaming callback for the given chain type."""
-    chain_type = chain.__class__.__name__
-    return STREAMING_CALLBACKS[chain_type](*args, **kwargs)
-
-
-def get_websocket_callback(chain: Chain, *args, **kwargs) -> AsyncWebsocketCallback:
-    """Get the websocket callback for the given chain type."""
-    chain_type = chain.__class__.__name__
-    return WEBSOCKET_CALLBACKS[chain_type](*args, **kwargs)
+
+@register_streaming_callback("BaseQAWithSources")
+class AsyncBaseQAWithSourcesChainStreamingCallback(
+    AsyncBaseRetrievalQAStreamingCallback
+):
+    """AsyncStreamingResponseCallback handler for BaseQAWithSources."""
+
+    pass
+
+
+@register_websocket_callback("BaseQAWithSources")
+class AsyncBaseQAWithSourcesChainWebsocketCallback(
+    AsyncBaseRetrievalQAWebsocketCallback
+):
+    """AsyncWebsocketCallback handler for BaseQAWithSources."""
+
+    pass
+
+
+@register_streaming_callback("QAWithSourcesChain")
+class AsyncQAWithSourcesChainStreamingCallback(
+    AsyncBaseQAWithSourcesChainStreamingCallback
+):
+    """AsyncStreamingResponseCallback handler for QAWithSourcesChain."""
+
+    pass
+
+
+@register_websocket_callback("QAWithSourcesChain")
+class AsyncQAWithSourcesChainWebsocketCallback(
+    AsyncBaseQAWithSourcesChainWebsocketCallback
+):
+    """AsyncWebsocketCallback handler for QAWithSourcesChain."""
+
+    pass
+
+
+@register_streaming_callback("VectorDBQAWithSourcesChain")
+class AsyncVectorDBQAWithSourcesChainStreamingCallback(
+    AsyncBaseQAWithSourcesChainStreamingCallback
+):
+    """AsyncStreamingResponseCallback handler for VectorDBQAWithSourcesChain."""
+
+    pass
+
+
+@register_websocket_callback("VectorDBQAWithSourcesChain")
+class AsyncVectorDBQAWithSourcesChainWebsocketCallback(
+    AsyncBaseQAWithSourcesChainWebsocketCallback
+):
+    """AsyncWebsocketCallback handler for VectorDBQAWithSourcesChain."""
+
+    pass
+
+
+@register_streaming_callback("RetrievalQAWithSourcesChain")
+class AsyncRetrievalQAWithSourcesChainStreamingCallback(
+    AsyncBaseQAWithSourcesChainStreamingCallback
+):
+    """AsyncStreamingResponseCallback handler for RetrievalQAWithSourcesChain."""
+
+    pass
+
+
+@register_websocket_callback("RetrievalQAWithSourcesChain")
+class AsyncRetrievalQAWithSourcesChainWebsocketCallback(
+    AsyncBaseQAWithSourcesChainWebsocketCallback
+):
+    """AsyncWebsocketCallback handler for RetrievalQAWithSourcesChain."""
+
+    pass
+
+
+@register_streaming_callback("ConversationalRetrievalChain")
+class AsyncConversationalRetrievalChainStreamingCallback(
+    AsyncBaseQAWithSourcesChainStreamingCallback
+):
+    """AsyncStreamingResponseCallback handler for ConversationalRetrievalChain."""
+
+    pass
+
+
+@register_websocket_callback("ConversationalRetrievalChain")
+class AsyncConversationalRetrievalChainWebsocketCallback(
+    AsyncBaseQAWithSourcesChainWebsocketCallback
+):
+    """AsyncWebsocketCallback handler for ConversationalRetrievalChain."""
+
+    pass
```

### Comparing `lanarky-0.6.0/lanarky/callbacks/base.py` & `lanarky-0.6.1/lanarky/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.6.0/lanarky/callbacks/llm.py` & `lanarky-0.6.1/lanarky/callbacks/llm.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.6.0/lanarky/callbacks/retrieval_qa.py` & `lanarky-0.6.1/lanarky/callbacks/retrieval_qa.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.6.0/lanarky/register.py` & `lanarky-0.6.1/lanarky/register.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.6.0/lanarky/responses/streaming.py` & `lanarky-0.6.1/lanarky/responses/streaming.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.6.0/lanarky/schemas.py` & `lanarky-0.6.1/lanarky/schemas.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.6.0/lanarky/testing/gradio.py` & `lanarky-0.6.1/lanarky/testing/gradio.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.6.0/lanarky/websockets/base.py` & `lanarky-0.6.1/lanarky/websockets/base.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.6.0/pyproject.toml` & `lanarky-0.6.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "lanarky"
-version = "0.6.0"
+version = "0.6.1"
 description = "Ship production-ready LLM projects with FastAPI"
 authors = ["Ajinkya Indulkar <26824103+ajndkr@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/ajndkr/lanarky"
 repository = "https://github.com/ajndkr/lanarky"
 license = "MIT"
 packages = [{include = "lanarky"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 fastapi = "^0.95.1"
-langchain = ">=0.0.167"
+langchain = ">=0.0.172"
 urllib3 = "<=1.26.15"  # added due to poetry errors
 python-dotenv = "^1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.3.1"
 
 [build-system]
```

### Comparing `lanarky-0.6.0/PKG-INFO` & `lanarky-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: lanarky
-Version: 0.6.0
+Version: 0.6.1
 Summary: Ship production-ready LLM projects with FastAPI
 Home-page: https://github.com/ajndkr/lanarky
 License: MIT
 Author: Ajinkya Indulkar
 Author-email: 26824103+ajndkr@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fastapi (>=0.95.1,<0.96.0)
-Requires-Dist: langchain (>=0.0.167)
+Requires-Dist: langchain (>=0.0.172)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: urllib3 (<=1.26.15)
 Project-URL: Repository, https://github.com/ajndkr/lanarky
 Description-Content-Type: text/markdown
 
 <div align="center">
```

