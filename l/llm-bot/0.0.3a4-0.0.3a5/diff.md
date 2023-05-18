# Comparing `tmp/llm_bot-0.0.3a4.tar.gz` & `tmp/llm_bot-0.0.3a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_bot-0.0.3a4.tar", max compression
+gzip compressed data, was "llm_bot-0.0.3a5.tar", max compression
```

## Comparing `llm_bot-0.0.3a4.tar` & `llm_bot-0.0.3a5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35149 2023-04-26 18:09:51.267170 llm_bot-0.0.3a4/LICENSE
--rw-r--r--   0        0        0       61 2023-04-26 18:09:51.267170 llm_bot-0.0.3a4/README.md
--rw-r--r--   0        0        0        0 2023-04-26 18:09:51.267170 llm_bot-0.0.3a4/llm_bot/__init__.py
--rw-r--r--   0        0        0    18628 2023-05-18 18:31:39.421274 llm_bot-0.0.3a4/llm_bot/core.py
--rw-r--r--   0        0        0      942 2023-05-18 18:31:50.757327 llm_bot-0.0.3a4/pyproject.toml
--rw-r--r--   0        0        0      926 1970-01-01 00:00:00.000000 llm_bot-0.0.3a4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-26 18:09:51.267170 llm_bot-0.0.3a5/LICENSE
+-rw-r--r--   0        0        0       61 2023-04-26 18:09:51.267170 llm_bot-0.0.3a5/README.md
+-rw-r--r--   0        0        0        0 2023-04-26 18:09:51.267170 llm_bot-0.0.3a5/llm_bot/__init__.py
+-rw-r--r--   0        0        0    18622 2023-05-18 18:34:36.634042 llm_bot-0.0.3a5/llm_bot/core.py
+-rw-r--r--   0        0        0      942 2023-05-18 18:34:44.750075 llm_bot-0.0.3a5/pyproject.toml
+-rw-r--r--   0        0        0      926 1970-01-01 00:00:00.000000 llm_bot-0.0.3a5/PKG-INFO
```

### Comparing `llm_bot-0.0.3a4/LICENSE` & `llm_bot-0.0.3a5/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_bot-0.0.3a4/llm_bot/core.py` & `llm_bot-0.0.3a5/llm_bot/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
 
         # Load the indexes and the vector stores
         self._stores = {}
         for index_file in index_files:
             # Get index name from the index file name
             index_name = index_file.stem[6:]
             # Load index
-            index: IndexFlat = faiss.read_index(f"{str(index_file)}.faiss")
+            index: IndexFlat = faiss.read_index(f"{str(index_file)}")
             # Load vector store
             store_fname = path / f"store_{index_name}.pickle"
             with open(store_fname, "rb") as f:
                 store: FAISS = pickle.load(f)
             store.index = index
             self._stores[index_name] = store
```

### Comparing `llm_bot-0.0.3a4/pyproject.toml` & `llm_bot-0.0.3a5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llm-bot"
-version = "0.0.3a4"
+version = "0.0.3a5"
 description = "Python library for developing LLM bots"
 authors = ["Gabriel Gazola Milan <gabriel.gazola@poli.ufrj.br>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://github.com/prefeitura-rio/chatbot-lab"
 repository = "https://github.com/prefeitura-rio/chatbot-lab"
 keywords = ["python", "chatbot", "bot", "llm"]
```

### Comparing `llm_bot-0.0.3a4/PKG-INFO` & `llm_bot-0.0.3a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-bot
-Version: 0.0.3a4
+Version: 0.0.3a5
 Summary: Python library for developing LLM bots
 Home-page: https://github.com/prefeitura-rio/chatbot-lab
 License: GPL-3.0-only
 Keywords: python,chatbot,bot,llm
 Author: Gabriel Gazola Milan
 Author-email: gabriel.gazola@poli.ufrj.br
 Requires-Python: >=3.10,<4.0
```

