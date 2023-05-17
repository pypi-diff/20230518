# Comparing `tmp/capabilities-0.3.2.tar.gz` & `tmp/capabilities-0.3.3.tar.gz`

## Comparing `capabilities-0.3.2.tar` & `capabilities-0.3.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 capabilities-0.3.2/setup.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 capabilities-0.3.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 capabilities-0.3.2/capabilities/__about__.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 capabilities-0.3.2/capabilities/__init__.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 capabilities-0.3.2/capabilities/__main__.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 capabilities-0.3.2/capabilities/cli.py
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 capabilities-0.3.2/capabilities/config.py
--rw-r--r--   0        0        0    16987 2020-02-02 00:00:00.000000 capabilities-0.3.2/capabilities/core.py
--rw-r--r--   0        0        0     8071 2020-02-02 00:00:00.000000 capabilities-0.3.2/capabilities/dec.py
--rw-r--r--   0        0        0    15162 2020-02-02 00:00:00.000000 capabilities-0.3.2/capabilities/example.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 capabilities-0.3.2/capabilities/search/__init__.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 capabilities-0.3.2/capabilities/search/hf.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 capabilities-0.3.2/capabilities/search/loader.py
--rw-r--r--   0        0        0     6082 2020-02-02 00:00:00.000000 capabilities-0.3.2/capabilities/search/nomic_index.py
--rw-r--r--   0        0        0     6286 2020-02-02 00:00:00.000000 capabilities-0.3.2/capabilities/search/oai.py
--rw-r--r--   0        0        0    12426 2020-02-02 00:00:00.000000 capabilities-0.3.2/capabilities/search/search_index.py
--rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 capabilities-0.3.2/capabilities/search/simple_vector_index.py
--rw-r--r--   0        0        0     7076 2020-02-02 00:00:00.000000 capabilities-0.3.2/capabilities/search/types.py
--rw-r--r--   0        0        0     5313 2020-02-02 00:00:00.000000 capabilities-0.3.2/capabilities/search/util.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 capabilities-0.3.2/capabilities/util/__init__.py
--rw-r--r--   0        0        0     9213 2020-02-02 00:00:00.000000 capabilities-0.3.2/capabilities/util/config.py
--rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 capabilities-0.3.2/capabilities/util/misc.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 capabilities-0.3.2/examples/cheese.py
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 capabilities-0.3.2/examples/leansearch.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 capabilities-0.3.2/examples/readme.txt
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 capabilities-0.3.2/examples/tesla10k.py
--rw-r--r--   0        0        0   840980 2020-02-02 00:00:00.000000 capabilities-0.3.2/examples/data/apple10k.pdf
--rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 capabilities-0.3.2/examples/data/sample.md
--rw-r--r--   0        0        0     7945 2020-02-02 00:00:00.000000 capabilities-0.3.2/examples/data/sample.pdf
--rw-r--r--   0        0        0   157134 2020-02-02 00:00:00.000000 capabilities-0.3.2/examples/data/tesla10k.txt
--rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 capabilities-0.3.2/tests/test_dec.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 capabilities-0.3.2/tests/test_document_loader.py
--rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 capabilities-0.3.2/tests/test_search.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 capabilities-0.3.2/tests/test_search_util.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 capabilities-0.3.2/tests/test_tutorial1.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 capabilities-0.3.2/tests/test_vector_idx.py
--rw-r--r--   0        0        0   353564 2020-02-02 00:00:00.000000 capabilities-0.3.2/tests/snapshots/test_search/test_search_e2e/NomicIndex-openai/r0.txt
--rw-r--r--   0        0        0   353563 2020-02-02 00:00:00.000000 capabilities-0.3.2/tests/snapshots/test_search/test_search_e2e/NomicIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt
--rw-r--r--   0        0        0   353563 2020-02-02 00:00:00.000000 capabilities-0.3.2/tests/snapshots/test_search/test_search_e2e/SearchIndex-openai/r0.txt
--rw-r--r--   0        0        0   353565 2020-02-02 00:00:00.000000 capabilities-0.3.2/tests/snapshots/test_search/test_search_e2e/SearchIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 capabilities-0.3.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 capabilities-0.3.2/LICENSE
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 capabilities-0.3.2/README.md
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 capabilities-0.3.2/pyproject.toml
--rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 capabilities-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 capabilities-0.3.3/setup.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 capabilities-0.3.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 capabilities-0.3.3/capabilities/__about__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 capabilities-0.3.3/capabilities/__init__.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 capabilities-0.3.3/capabilities/__main__.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 capabilities-0.3.3/capabilities/cli.py
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 capabilities-0.3.3/capabilities/config.py
+-rw-r--r--   0        0        0    12375 2020-02-02 00:00:00.000000 capabilities-0.3.3/capabilities/core.py
+-rw-r--r--   0        0        0     8071 2020-02-02 00:00:00.000000 capabilities-0.3.3/capabilities/dec.py
+-rw-r--r--   0        0        0    15162 2020-02-02 00:00:00.000000 capabilities-0.3.3/capabilities/example.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 capabilities-0.3.3/capabilities/search/__init__.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 capabilities-0.3.3/capabilities/search/hf.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 capabilities-0.3.3/capabilities/search/loader.py
+-rw-r--r--   0        0        0     6082 2020-02-02 00:00:00.000000 capabilities-0.3.3/capabilities/search/nomic_index.py
+-rw-r--r--   0        0        0     6567 2020-02-02 00:00:00.000000 capabilities-0.3.3/capabilities/search/oai.py
+-rw-r--r--   0        0        0    12426 2020-02-02 00:00:00.000000 capabilities-0.3.3/capabilities/search/search_index.py
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 capabilities-0.3.3/capabilities/search/simple_vector_index.py
+-rw-r--r--   0        0        0     7076 2020-02-02 00:00:00.000000 capabilities-0.3.3/capabilities/search/types.py
+-rw-r--r--   0        0        0     5313 2020-02-02 00:00:00.000000 capabilities-0.3.3/capabilities/search/util.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 capabilities-0.3.3/capabilities/util/__init__.py
+-rw-r--r--   0        0        0     9213 2020-02-02 00:00:00.000000 capabilities-0.3.3/capabilities/util/config.py
+-rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 capabilities-0.3.3/capabilities/util/misc.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 capabilities-0.3.3/examples/cheese.py
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 capabilities-0.3.3/examples/leansearch.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 capabilities-0.3.3/examples/readme.txt
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 capabilities-0.3.3/examples/tesla10k.py
+-rw-r--r--   0        0        0   840980 2020-02-02 00:00:00.000000 capabilities-0.3.3/examples/data/apple10k.pdf
+-rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 capabilities-0.3.3/examples/data/sample.md
+-rw-r--r--   0        0        0     7945 2020-02-02 00:00:00.000000 capabilities-0.3.3/examples/data/sample.pdf
+-rw-r--r--   0        0        0   157134 2020-02-02 00:00:00.000000 capabilities-0.3.3/examples/data/tesla10k.txt
+-rw-r--r--   0        0        0     5476 2020-02-02 00:00:00.000000 capabilities-0.3.3/tests/test_docs.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 capabilities-0.3.3/tests/test_document_loader.py
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 capabilities-0.3.3/tests/test_search.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 capabilities-0.3.3/tests/test_search_util.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 capabilities-0.3.3/tests/test_tutorial1.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 capabilities-0.3.3/tests/test_vector_idx.py
+-rw-r--r--   0        0        0   353564 2020-02-02 00:00:00.000000 capabilities-0.3.3/tests/snapshots/test_search/test_search_e2e/NomicIndex-openai/r0.txt
+-rw-r--r--   0        0        0   353563 2020-02-02 00:00:00.000000 capabilities-0.3.3/tests/snapshots/test_search/test_search_e2e/NomicIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt
+-rw-r--r--   0        0        0   353563 2020-02-02 00:00:00.000000 capabilities-0.3.3/tests/snapshots/test_search/test_search_e2e/SearchIndex-openai/r0.txt
+-rw-r--r--   0        0        0   353565 2020-02-02 00:00:00.000000 capabilities-0.3.3/tests/snapshots/test_search/test_search_e2e/SearchIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 capabilities-0.3.3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 capabilities-0.3.3/LICENSE
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 capabilities-0.3.3/README.md
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 capabilities-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 capabilities-0.3.3/PKG-INFO
```

### Comparing `capabilities-0.3.2/.github/workflows/python-publish.yml` & `capabilities-0.3.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.2/capabilities/cli.py` & `capabilities-0.3.3/capabilities/cli.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.2/capabilities/dec.py` & `capabilities-0.3.3/capabilities/dec.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.2/capabilities/example.py` & `capabilities-0.3.3/capabilities/example.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.2/capabilities/search/hf.py` & `capabilities-0.3.3/capabilities/search/hf.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.2/capabilities/search/loader.py` & `capabilities-0.3.3/capabilities/search/loader.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.2/capabilities/search/nomic_index.py` & `capabilities-0.3.3/capabilities/search/nomic_index.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.2/capabilities/search/oai.py` & `capabilities-0.3.3/capabilities/search/oai.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,34 +14,41 @@
 from rich.progress import track
 import requests
 
 """ A client for the OpenAI API. """
 
 
 class OpenAISettings(BaseSettings):
-    api_key: SecretStr
+    api_key: Optional[SecretStr] = None
     api_url: str = "https://api.openai.com"
 
     class Config:
         env_file = ".env"
         env_file_encoding = "utf-8"
         env_prefix = "OPENAI_"
 
     def create_headers(self):
+        if self.api_key is None:
+            raise ValueError(
+                "OpenAI API key is not set. Either add it to the .env file or to your enviroment."
+            )
         headers = {
             "Content-Type": "application/json",
             "Authorization": f"Bearer {self.api_key.get_secret_value()}",
         }
         return headers
 
     def post(self, path: str, **kwargs):
         url = f"{self.api_url}{path}"
         return requests.post(url, headers=self.create_headers(), **kwargs)
 
 
+CONFIG = OpenAISettings()
+
+
 class Message(BaseModel):
     """OpenAI chat message.
 
     ref: https://platform.openai.com/docs/guides/chat
     """
 
     role: Literal["system", "user", "assistant"]
@@ -117,15 +124,17 @@
 
 # [todo] throttling, retries
 @cache.memoize()
 def embeddings(params: EmbeddingRequest) -> EmbeddingResponse:
     resp = OpenAISettings().post("/v1/embeddings", json=params.dict(exclude_none=True))  # type: ignore
     j = resp.json()
     if resp.status_code // 100 == 4:
-        raise requests.HTTPError(f"{resp.status_code}: {json.dumps(j, indent=2)}", response=resp)
+        raise requests.HTTPError(
+            f"{resp.status_code}: {json.dumps(j, indent=2)}", response=resp
+        )
     resp.raise_for_status()
     r = EmbeddingResponse.parse_obj(j)
     return r
 
 
 @cache.memoize()
 def chat_completions(params: CompletionRequest) -> CompletionResponse:
@@ -181,15 +190,17 @@
         return starts, ends
 
     def encode(self, texts: list[str]):
         lengths = [self.count_tokens(text) for text in texts]
         N = self.max_tokens_per_item
         for i, l in enumerate(lengths):
             if l > N:
-                raise ValueError(f"{i}th text {texts[i]} is too long, please chunk it first")
+                raise ValueError(
+                    f"{i}th text {texts[i]} is too long, please chunk it first"
+                )
         batches = argbatch(lengths, N)
         es = []
         # its = track(batches) if len(batches) > 100 else batches
         its = batches
 
         def process_batch(batch, texts, embeddings, model_name):
             ts = texts[batch.start : batch.stop]
```

### Comparing `capabilities-0.3.2/capabilities/search/search_index.py` & `capabilities-0.3.3/capabilities/search/search_index.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.2/capabilities/search/simple_vector_index.py` & `capabilities-0.3.3/capabilities/search/simple_vector_index.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.2/capabilities/search/types.py` & `capabilities-0.3.3/capabilities/search/types.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.2/capabilities/search/util.py` & `capabilities-0.3.3/capabilities/search/util.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.2/capabilities/util/config.py` & `capabilities-0.3.3/capabilities/util/config.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.2/capabilities/util/misc.py` & `capabilities-0.3.3/capabilities/util/misc.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.2/examples/cheese.py` & `capabilities-0.3.3/examples/cheese.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.2/examples/leansearch.py` & `capabilities-0.3.3/examples/leansearch.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.2/examples/tesla10k.py` & `capabilities-0.3.3/examples/tesla10k.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.2/examples/data/apple10k.pdf` & `capabilities-0.3.3/examples/data/apple10k.pdf`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.2/examples/data/sample.md` & `capabilities-0.3.3/examples/data/sample.md`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.2/examples/data/sample.pdf` & `capabilities-0.3.3/examples/data/sample.pdf`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.2/examples/data/tesla10k.txt` & `capabilities-0.3.3/examples/data/tesla10k.txt`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.2/tests/test_document_loader.py` & `capabilities-0.3.3/tests/test_document_loader.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.2/tests/test_search.py` & `capabilities-0.3.3/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.2/tests/test_search_util.py` & `capabilities-0.3.3/tests/test_search_util.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.2/tests/test_tutorial1.py` & `capabilities-0.3.3/tests/test_tutorial1.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.2/tests/test_vector_idx.py` & `capabilities-0.3.3/tests/test_vector_idx.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.2/tests/snapshots/test_search/test_search_e2e/NomicIndex-openai/r0.txt` & `capabilities-0.3.3/tests/snapshots/test_search/test_search_e2e/NomicIndex-openai/r0.txt`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.2/tests/snapshots/test_search/test_search_e2e/NomicIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt` & `capabilities-0.3.3/tests/snapshots/test_search/test_search_e2e/NomicIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.2/tests/snapshots/test_search/test_search_e2e/SearchIndex-openai/r0.txt` & `capabilities-0.3.3/tests/snapshots/test_search/test_search_e2e/SearchIndex-openai/r0.txt`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.2/tests/snapshots/test_search/test_search_e2e/SearchIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt` & `capabilities-0.3.3/tests/snapshots/test_search/test_search_e2e/SearchIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.2/.gitignore` & `capabilities-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.2/LICENSE` & `capabilities-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.2/pyproject.toml` & `capabilities-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.2/PKG-INFO` & `capabilities-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capabilities
-Version: 0.3.2
+Version: 0.3.3
 Summary: Build trusted, faster, and more powerful applications with the Blazon Capabilities API.
 Author-email: Blazon AI <support@blazon.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

