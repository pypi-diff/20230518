# Comparing `tmp/llm_bot-0.0.3a2.tar.gz` & `tmp/llm_bot-0.0.3a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_bot-0.0.3a2.tar", max compression
+gzip compressed data, was "llm_bot-0.0.3a3.tar", max compression
```

## Comparing `llm_bot-0.0.3a2.tar` & `llm_bot-0.0.3a3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35149 2023-04-26 18:09:51.267170 llm_bot-0.0.3a2/LICENSE
--rw-r--r--   0        0        0       61 2023-04-26 18:09:51.267170 llm_bot-0.0.3a2/README.md
--rw-r--r--   0        0        0        0 2023-04-26 18:09:51.267170 llm_bot-0.0.3a2/llm_bot/__init__.py
--rw-r--r--   0        0        0    18603 2023-05-18 17:31:17.612380 llm_bot-0.0.3a2/llm_bot/core.py
--rw-r--r--   0        0        0      942 2023-05-18 17:32:08.332217 llm_bot-0.0.3a2/pyproject.toml
--rw-r--r--   0        0        0      926 1970-01-01 00:00:00.000000 llm_bot-0.0.3a2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-26 18:09:51.267170 llm_bot-0.0.3a3/LICENSE
+-rw-r--r--   0        0        0       61 2023-04-26 18:09:51.267170 llm_bot-0.0.3a3/README.md
+-rw-r--r--   0        0        0        0 2023-04-26 18:09:51.267170 llm_bot-0.0.3a3/llm_bot/__init__.py
+-rw-r--r--   0        0        0    18638 2023-05-18 18:26:29.979550 llm_bot-0.0.3a3/llm_bot/core.py
+-rw-r--r--   0        0        0      942 2023-05-18 18:27:07.667794 llm_bot-0.0.3a3/pyproject.toml
+-rw-r--r--   0        0        0      926 1970-01-01 00:00:00.000000 llm_bot-0.0.3a3/PKG-INFO
```

### Comparing `llm_bot-0.0.3a2/LICENSE` & `llm_bot-0.0.3a3/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_bot-0.0.3a2/llm_bot/core.py` & `llm_bot-0.0.3a3/llm_bot/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,16 +169,16 @@
             path (Union[str, Path]): The path to load the index and vector store from.
         """
         # Assert that the path exists
         path = Path(path)
         assert path.exists(), f"Path {path} does not exist."
 
         # Get list of files in the path with `index_` and `store_` prefixes
-        index_files = list(path.glob("index_*"))
-        store_files = list(path.glob("store_*"))
+        index_files = [f.stem for f in path.glob("index_*")]
+        store_files = [f.stem for f in path.glob("store_*")]
 
         # Assert that all files have a corresponding index and store file
         for index_file in index_files:
             store_file = path / f"store_{index_file.name[6:]}.pickle"
             assert store_file.exists(), f"Store file {store_file} does not exist."
         for store_file in store_files:
             index_file = path / f"index_{store_file.name[6:]}.faiss"
@@ -186,15 +186,15 @@
 
         # Load the indexes and the vector stores
         self._stores = {}
         for index_file in index_files:
             # Get index name from the index file name
             index_name = index_file.name[6:]
             # Load index
-            index: IndexFlat = faiss.read_index(str(index_file))
+            index: IndexFlat = faiss.read_index(f"{str(index_file)}.faiss")
             # Load vector store
             store_fname = path / f"store_{index_name}.pickle"
             with open(store_fname, "rb") as f:
                 store: FAISS = pickle.load(f)
             store.index = index
             self._stores[index_name] = store
```

### Comparing `llm_bot-0.0.3a2/pyproject.toml` & `llm_bot-0.0.3a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llm-bot"
-version = "0.0.3a2"
+version = "0.0.3a3"
 description = "Python library for developing LLM bots"
 authors = ["Gabriel Gazola Milan <gabriel.gazola@poli.ufrj.br>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://github.com/prefeitura-rio/chatbot-lab"
 repository = "https://github.com/prefeitura-rio/chatbot-lab"
 keywords = ["python", "chatbot", "bot", "llm"]
```

### Comparing `llm_bot-0.0.3a2/PKG-INFO` & `llm_bot-0.0.3a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-bot
-Version: 0.0.3a2
+Version: 0.0.3a3
 Summary: Python library for developing LLM bots
 Home-page: https://github.com/prefeitura-rio/chatbot-lab
 License: GPL-3.0-only
 Keywords: python,chatbot,bot,llm
 Author: Gabriel Gazola Milan
 Author-email: gabriel.gazola@poli.ufrj.br
 Requires-Python: >=3.10,<4.0
```

