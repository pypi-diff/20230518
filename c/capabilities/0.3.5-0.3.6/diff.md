# Comparing `tmp/capabilities-0.3.5.tar.gz` & `tmp/capabilities-0.3.6.tar.gz`

## Comparing `capabilities-0.3.5.tar` & `capabilities-0.3.6.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 capabilities-0.3.5/setup.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 capabilities-0.3.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 capabilities-0.3.5/capabilities/__about__.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 capabilities-0.3.5/capabilities/__init__.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 capabilities-0.3.5/capabilities/__main__.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 capabilities-0.3.5/capabilities/cli.py
--rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 capabilities-0.3.5/capabilities/config.py
--rw-r--r--   0        0        0    12240 2020-02-02 00:00:00.000000 capabilities-0.3.5/capabilities/core.py
--rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 capabilities-0.3.5/capabilities/dec.py
--rw-r--r--   0        0        0    15164 2020-02-02 00:00:00.000000 capabilities-0.3.5/capabilities/example.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 capabilities-0.3.5/capabilities/search/__init__.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 capabilities-0.3.5/capabilities/search/hf.py
--rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 capabilities-0.3.5/capabilities/search/loader.py
--rw-r--r--   0        0        0     6160 2020-02-02 00:00:00.000000 capabilities-0.3.5/capabilities/search/nomic_index.py
--rw-r--r--   0        0        0     6507 2020-02-02 00:00:00.000000 capabilities-0.3.5/capabilities/search/oai.py
--rw-r--r--   0        0        0    12504 2020-02-02 00:00:00.000000 capabilities-0.3.5/capabilities/search/search_index.py
--rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 capabilities-0.3.5/capabilities/search/simple_vector_index.py
--rw-r--r--   0        0        0     7150 2020-02-02 00:00:00.000000 capabilities-0.3.5/capabilities/search/types.py
--rw-r--r--   0        0        0     5375 2020-02-02 00:00:00.000000 capabilities-0.3.5/capabilities/search/util.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 capabilities-0.3.5/capabilities/util/__init__.py
--rw-r--r--   0        0        0     9199 2020-02-02 00:00:00.000000 capabilities-0.3.5/capabilities/util/config.py
--rw-r--r--   0        0        0     6705 2020-02-02 00:00:00.000000 capabilities-0.3.5/capabilities/util/misc.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 capabilities-0.3.5/examples/cheese.py
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 capabilities-0.3.5/examples/leansearch.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 capabilities-0.3.5/examples/readme.txt
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 capabilities-0.3.5/examples/tesla10k.py
--rw-r--r--   0        0        0   840980 2020-02-02 00:00:00.000000 capabilities-0.3.5/examples/data/apple10k.pdf
--rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 capabilities-0.3.5/examples/data/sample.md
--rw-r--r--   0        0        0     7945 2020-02-02 00:00:00.000000 capabilities-0.3.5/examples/data/sample.pdf
--rw-r--r--   0        0        0   157134 2020-02-02 00:00:00.000000 capabilities-0.3.5/examples/data/tesla10k.txt
--rw-r--r--   0        0        0     5476 2020-02-02 00:00:00.000000 capabilities-0.3.5/tests/test_docs.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 capabilities-0.3.5/tests/test_document_loader.py
--rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 capabilities-0.3.5/tests/test_search.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 capabilities-0.3.5/tests/test_search_util.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 capabilities-0.3.5/tests/test_tutorial1.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 capabilities-0.3.5/tests/test_vector_idx.py
--rw-r--r--   0        0        0   353564 2020-02-02 00:00:00.000000 capabilities-0.3.5/tests/snapshots/test_search/test_search_e2e/NomicIndex-openai/r0.txt
--rw-r--r--   0        0        0   353563 2020-02-02 00:00:00.000000 capabilities-0.3.5/tests/snapshots/test_search/test_search_e2e/NomicIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt
--rw-r--r--   0        0        0   353563 2020-02-02 00:00:00.000000 capabilities-0.3.5/tests/snapshots/test_search/test_search_e2e/SearchIndex-openai/r0.txt
--rw-r--r--   0        0        0   353565 2020-02-02 00:00:00.000000 capabilities-0.3.5/tests/snapshots/test_search/test_search_e2e/SearchIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 capabilities-0.3.5/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 capabilities-0.3.5/LICENSE
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 capabilities-0.3.5/README.md
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 capabilities-0.3.5/pyproject.toml
--rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 capabilities-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 capabilities-0.3.6/setup.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 capabilities-0.3.6/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 capabilities-0.3.6/capabilities/__about__.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 capabilities-0.3.6/capabilities/__init__.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 capabilities-0.3.6/capabilities/__main__.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 capabilities-0.3.6/capabilities/cli.py
+-rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 capabilities-0.3.6/capabilities/config.py
+-rw-r--r--   0        0        0    12246 2020-02-02 00:00:00.000000 capabilities-0.3.6/capabilities/core.py
+-rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 capabilities-0.3.6/capabilities/dec.py
+-rw-r--r--   0        0        0    15164 2020-02-02 00:00:00.000000 capabilities-0.3.6/capabilities/example.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 capabilities-0.3.6/capabilities/search/__init__.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 capabilities-0.3.6/capabilities/search/hf.py
+-rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 capabilities-0.3.6/capabilities/search/loader.py
+-rw-r--r--   0        0        0     6160 2020-02-02 00:00:00.000000 capabilities-0.3.6/capabilities/search/nomic_index.py
+-rw-r--r--   0        0        0     6507 2020-02-02 00:00:00.000000 capabilities-0.3.6/capabilities/search/oai.py
+-rw-r--r--   0        0        0    12504 2020-02-02 00:00:00.000000 capabilities-0.3.6/capabilities/search/search_index.py
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 capabilities-0.3.6/capabilities/search/simple_vector_index.py
+-rw-r--r--   0        0        0     7150 2020-02-02 00:00:00.000000 capabilities-0.3.6/capabilities/search/types.py
+-rw-r--r--   0        0        0     5375 2020-02-02 00:00:00.000000 capabilities-0.3.6/capabilities/search/util.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 capabilities-0.3.6/capabilities/util/__init__.py
+-rw-r--r--   0        0        0     9199 2020-02-02 00:00:00.000000 capabilities-0.3.6/capabilities/util/config.py
+-rw-r--r--   0        0        0     6705 2020-02-02 00:00:00.000000 capabilities-0.3.6/capabilities/util/misc.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 capabilities-0.3.6/examples/cheese.py
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 capabilities-0.3.6/examples/leansearch.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 capabilities-0.3.6/examples/readme.txt
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 capabilities-0.3.6/examples/tesla10k.py
+-rw-r--r--   0        0        0   840980 2020-02-02 00:00:00.000000 capabilities-0.3.6/examples/data/apple10k.pdf
+-rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 capabilities-0.3.6/examples/data/sample.md
+-rw-r--r--   0        0        0     7945 2020-02-02 00:00:00.000000 capabilities-0.3.6/examples/data/sample.pdf
+-rw-r--r--   0        0        0   157134 2020-02-02 00:00:00.000000 capabilities-0.3.6/examples/data/tesla10k.txt
+-rw-r--r--   0        0        0     5476 2020-02-02 00:00:00.000000 capabilities-0.3.6/tests/test_docs.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 capabilities-0.3.6/tests/test_document_loader.py
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 capabilities-0.3.6/tests/test_search.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 capabilities-0.3.6/tests/test_search_util.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 capabilities-0.3.6/tests/test_tutorial1.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 capabilities-0.3.6/tests/test_vector_idx.py
+-rw-r--r--   0        0        0   353564 2020-02-02 00:00:00.000000 capabilities-0.3.6/tests/snapshots/test_search/test_search_e2e/NomicIndex-openai/r0.txt
+-rw-r--r--   0        0        0   353563 2020-02-02 00:00:00.000000 capabilities-0.3.6/tests/snapshots/test_search/test_search_e2e/NomicIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt
+-rw-r--r--   0        0        0   353563 2020-02-02 00:00:00.000000 capabilities-0.3.6/tests/snapshots/test_search/test_search_e2e/SearchIndex-openai/r0.txt
+-rw-r--r--   0        0        0   353565 2020-02-02 00:00:00.000000 capabilities-0.3.6/tests/snapshots/test_search/test_search_e2e/SearchIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 capabilities-0.3.6/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 capabilities-0.3.6/LICENSE
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 capabilities-0.3.6/README.md
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 capabilities-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 capabilities-0.3.6/PKG-INFO
```

### Comparing `capabilities-0.3.5/.github/workflows/python-publish.yml` & `capabilities-0.3.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.5/capabilities/cli.py` & `capabilities-0.3.6/capabilities/cli.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.5/capabilities/config.py` & `capabilities-0.3.6/capabilities/config.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.5/capabilities/core.py` & `capabilities-0.3.6/capabilities/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,15 +143,15 @@
         print(f"[DocumentQA] running query against document with {len(document)} characters")
         return CONFIG.post_sync(
             "/blazon/documentqa", payload={"document": document, "query": query}
         )
 
     async def run_async(self, document: str, query: str):
         print(f"[DocumentQA] running query against document with {len(document)} characters")
-        return CONFIG.post_async(
+        return await CONFIG.post_async(
             "/blazon/documentqa",
             payload={"document": document, "query": query},
         )
 
 
 @register("blazon/summarize")
 @dataclass
```

### Comparing `capabilities-0.3.5/capabilities/dec.py` & `capabilities-0.3.6/capabilities/dec.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.5/capabilities/example.py` & `capabilities-0.3.6/capabilities/example.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.5/capabilities/search/hf.py` & `capabilities-0.3.6/capabilities/search/hf.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.5/capabilities/search/loader.py` & `capabilities-0.3.6/capabilities/search/loader.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.5/capabilities/search/nomic_index.py` & `capabilities-0.3.6/capabilities/search/nomic_index.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.5/capabilities/search/oai.py` & `capabilities-0.3.6/capabilities/search/oai.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.5/capabilities/search/search_index.py` & `capabilities-0.3.6/capabilities/search/search_index.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.5/capabilities/search/simple_vector_index.py` & `capabilities-0.3.6/capabilities/search/simple_vector_index.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.5/capabilities/search/types.py` & `capabilities-0.3.6/capabilities/search/types.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.5/capabilities/search/util.py` & `capabilities-0.3.6/capabilities/search/util.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.5/capabilities/util/config.py` & `capabilities-0.3.6/capabilities/util/config.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.5/capabilities/util/misc.py` & `capabilities-0.3.6/capabilities/util/misc.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.5/examples/cheese.py` & `capabilities-0.3.6/examples/cheese.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.5/examples/leansearch.py` & `capabilities-0.3.6/examples/leansearch.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.5/examples/tesla10k.py` & `capabilities-0.3.6/examples/tesla10k.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.5/examples/data/apple10k.pdf` & `capabilities-0.3.6/examples/data/apple10k.pdf`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.5/examples/data/sample.md` & `capabilities-0.3.6/examples/data/sample.md`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.5/examples/data/sample.pdf` & `capabilities-0.3.6/examples/data/sample.pdf`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.5/examples/data/tesla10k.txt` & `capabilities-0.3.6/examples/data/tesla10k.txt`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.5/tests/test_docs.py` & `capabilities-0.3.6/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.5/tests/test_document_loader.py` & `capabilities-0.3.6/tests/test_document_loader.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.5/tests/test_search.py` & `capabilities-0.3.6/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.5/tests/test_search_util.py` & `capabilities-0.3.6/tests/test_search_util.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.5/tests/test_tutorial1.py` & `capabilities-0.3.6/tests/test_tutorial1.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.5/tests/test_vector_idx.py` & `capabilities-0.3.6/tests/test_vector_idx.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.5/tests/snapshots/test_search/test_search_e2e/NomicIndex-openai/r0.txt` & `capabilities-0.3.6/tests/snapshots/test_search/test_search_e2e/NomicIndex-openai/r0.txt`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.5/tests/snapshots/test_search/test_search_e2e/NomicIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt` & `capabilities-0.3.6/tests/snapshots/test_search/test_search_e2e/NomicIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.5/tests/snapshots/test_search/test_search_e2e/SearchIndex-openai/r0.txt` & `capabilities-0.3.6/tests/snapshots/test_search/test_search_e2e/SearchIndex-openai/r0.txt`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.5/tests/snapshots/test_search/test_search_e2e/SearchIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt` & `capabilities-0.3.6/tests/snapshots/test_search/test_search_e2e/SearchIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.5/.gitignore` & `capabilities-0.3.6/.gitignore`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.5/LICENSE` & `capabilities-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.5/pyproject.toml` & `capabilities-0.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "capabilities"
 # dynamic = ["version"]
-version="0.3.5"
+version="0.3.6"
 authors = [
   { name="Blazon AI", email="support@blazon.ai" },
 ]
 description = "Build trusted, faster, and more powerful applications with the Blazon Capabilities API."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `capabilities-0.3.5/PKG-INFO` & `capabilities-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capabilities
-Version: 0.3.5
+Version: 0.3.6
 Summary: Build trusted, faster, and more powerful applications with the Blazon Capabilities API.
 Author-email: Blazon AI <support@blazon.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

