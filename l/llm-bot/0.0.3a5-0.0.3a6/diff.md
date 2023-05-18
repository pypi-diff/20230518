# Comparing `tmp/llm_bot-0.0.3a5.tar.gz` & `tmp/llm_bot-0.0.3a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_bot-0.0.3a5.tar", max compression
+gzip compressed data, was "llm_bot-0.0.3a6.tar", max compression
```

## Comparing `llm_bot-0.0.3a5.tar` & `llm_bot-0.0.3a6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35149 2023-04-26 18:09:51.267170 llm_bot-0.0.3a5/LICENSE
--rw-r--r--   0        0        0       61 2023-04-26 18:09:51.267170 llm_bot-0.0.3a5/README.md
--rw-r--r--   0        0        0        0 2023-04-26 18:09:51.267170 llm_bot-0.0.3a5/llm_bot/__init__.py
--rw-r--r--   0        0        0    18622 2023-05-18 18:34:36.634042 llm_bot-0.0.3a5/llm_bot/core.py
--rw-r--r--   0        0        0      942 2023-05-18 18:34:44.750075 llm_bot-0.0.3a5/pyproject.toml
--rw-r--r--   0        0        0      926 1970-01-01 00:00:00.000000 llm_bot-0.0.3a5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-26 18:09:51.267170 llm_bot-0.0.3a6/LICENSE
+-rw-r--r--   0        0        0       61 2023-04-26 18:09:51.267170 llm_bot-0.0.3a6/README.md
+-rw-r--r--   0        0        0        0 2023-04-26 18:09:51.267170 llm_bot-0.0.3a6/llm_bot/__init__.py
+-rw-r--r--   0        0        0    18751 2023-05-18 18:39:18.063063 llm_bot-0.0.3a6/llm_bot/core.py
+-rw-r--r--   0        0        0      942 2023-05-18 18:39:31.515107 llm_bot-0.0.3a6/pyproject.toml
+-rw-r--r--   0        0        0      926 1970-01-01 00:00:00.000000 llm_bot-0.0.3a6/PKG-INFO
```

### Comparing `llm_bot-0.0.3a5/LICENSE` & `llm_bot-0.0.3a6/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_bot-0.0.3a5/llm_bot/core.py` & `llm_bot-0.0.3a6/llm_bot/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,34 +263,35 @@
                 for tmp_source in tmp_sources:
                     sources.append(tmp_source)
                     if len(sources) >= number_of_context_docs:
                         break
 
         # If chat history is provided, add messages for it
         if use_chat_history:
-            messages.append(SystemMessage(content=chat_history_prompt))
-            docs, _ = self.fetch_from_index(
-                query=user_message,
-                n_results=number_of_chat_history_docs,
-                index=use_chat_history,
-            )
-            for doc in docs:
-                messages.append(SystemMessage(content=f"- {doc.page_content}"))
             if use_chat_history in self._stores:
-                self._stores[use_chat_history].add_texts(
-                    texts=[f"User: {user_message}"],
-                    metadatas=[{"source": "user"}],
-                )
-            else:
-                embedding = OpenAIEmbeddings()
-                self._stores[use_chat_history] = FAISS.from_texts(
-                    texts=[f"User: {user_message}"],
-                    embedding=embedding,
-                    metadatas=[{"source": "user"}],
+                messages.append(SystemMessage(content=chat_history_prompt))
+                docs, _ = self.fetch_from_index(
+                    query=user_message,
+                    n_results=number_of_chat_history_docs,
+                    index=use_chat_history,
                 )
+                for doc in docs:
+                    messages.append(SystemMessage(content=f"- {doc.page_content}"))
+                if use_chat_history in self._stores:
+                    self._stores[use_chat_history].add_texts(
+                        texts=[f"User: {user_message}"],
+                        metadatas=[{"source": "user"}],
+                    )
+                else:
+                    embedding = OpenAIEmbeddings()
+                    self._stores[use_chat_history] = FAISS.from_texts(
+                        texts=[f"User: {user_message}"],
+                        embedding=embedding,
+                        metadatas=[{"source": "user"}],
+                    )
 
         # Add the user message
         messages.append(HumanMessage(content=user_message))
 
         return messages, sources
 
     def chat(self, messages: List[BaseMessage], chat_id: str) -> str:
```

### Comparing `llm_bot-0.0.3a5/pyproject.toml` & `llm_bot-0.0.3a6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llm-bot"
-version = "0.0.3a5"
+version = "0.0.3a6"
 description = "Python library for developing LLM bots"
 authors = ["Gabriel Gazola Milan <gabriel.gazola@poli.ufrj.br>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://github.com/prefeitura-rio/chatbot-lab"
 repository = "https://github.com/prefeitura-rio/chatbot-lab"
 keywords = ["python", "chatbot", "bot", "llm"]
```

### Comparing `llm_bot-0.0.3a5/PKG-INFO` & `llm_bot-0.0.3a6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-bot
-Version: 0.0.3a5
+Version: 0.0.3a6
 Summary: Python library for developing LLM bots
 Home-page: https://github.com/prefeitura-rio/chatbot-lab
 License: GPL-3.0-only
 Keywords: python,chatbot,bot,llm
 Author: Gabriel Gazola Milan
 Author-email: gabriel.gazola@poli.ufrj.br
 Requires-Python: >=3.10,<4.0
```

