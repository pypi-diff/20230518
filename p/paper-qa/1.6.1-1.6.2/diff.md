# Comparing `tmp/paper-qa-1.6.1.tar.gz` & `tmp/paper-qa-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper-qa-1.6.1.tar", last modified: Wed May 17 03:50:50 2023, max compression
+gzip compressed data, was "paper-qa-1.6.2.tar", last modified: Thu May 18 03:15:18 2023, max compression
```

## Comparing `paper-qa-1.6.1.tar` & `paper-qa-1.6.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:50:50.379257 paper-qa-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 03:50:10.000000 paper-qa-1.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-05-17 03:50:50.375257 paper-qa-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12150 2023-05-17 03:50:10.000000 paper-qa-1.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:50:50.375257 paper-qa-1.6.1/paper_qa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-05-17 03:50:50.000000 paper-qa-1.6.1/paper_qa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-17 03:50:50.000000 paper-qa-1.6.1/paper_qa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 03:50:50.000000 paper-qa-1.6.1/paper_qa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-17 03:50:50.000000 paper-qa-1.6.1/paper_qa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-17 03:50:50.000000 paper-qa-1.6.1/paper_qa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:50:50.375257 paper-qa-1.6.1/paperqa/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-17 03:50:10.000000 paper-qa-1.6.1/paperqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-05-17 03:50:10.000000 paper-qa-1.6.1/paperqa/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:50:50.375257 paper-qa-1.6.1/paperqa/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-17 03:50:10.000000 paper-qa-1.6.1/paperqa/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-05-17 03:50:10.000000 paper-qa-1.6.1/paperqa/contrib/zotero.py
--rw-r--r--   0 runner    (1001) docker     (123)    19465 2023-05-17 03:50:10.000000 paper-qa-1.6.1/paperqa/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-17 03:50:10.000000 paper-qa-1.6.1/paperqa/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-05-17 03:50:10.000000 paper-qa-1.6.1/paperqa/qaprompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-05-17 03:50:10.000000 paper-qa-1.6.1/paperqa/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-17 03:50:10.000000 paper-qa-1.6.1/paperqa/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-17 03:50:10.000000 paper-qa-1.6.1/paperqa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 03:50:10.000000 paper-qa-1.6.1/paperqa/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 03:50:50.379257 paper-qa-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-17 03:50:10.000000 paper-qa-1.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:50:50.375257 paper-qa-1.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-05-17 03:50:10.000000 paper-qa-1.6.1/tests/test_paperqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:15:18.664700 paper-qa-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-18 03:14:41.000000 paper-qa-1.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-05-18 03:15:18.664700 paper-qa-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12150 2023-05-18 03:14:41.000000 paper-qa-1.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:15:18.660700 paper-qa-1.6.2/paper_qa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-05-18 03:15:18.000000 paper-qa-1.6.2/paper_qa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-18 03:15:18.000000 paper-qa-1.6.2/paper_qa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 03:15:18.000000 paper-qa-1.6.2/paper_qa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-18 03:15:18.000000 paper-qa-1.6.2/paper_qa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-18 03:15:18.000000 paper-qa-1.6.2/paper_qa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:15:18.664700 paper-qa-1.6.2/paperqa/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 03:14:41.000000 paper-qa-1.6.2/paperqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-05-18 03:14:41.000000 paper-qa-1.6.2/paperqa/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:15:18.664700 paper-qa-1.6.2/paperqa/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-18 03:14:41.000000 paper-qa-1.6.2/paperqa/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-05-18 03:14:41.000000 paper-qa-1.6.2/paperqa/contrib/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20515 2023-05-18 03:14:41.000000 paper-qa-1.6.2/paperqa/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-18 03:14:41.000000 paper-qa-1.6.2/paperqa/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-18 03:14:41.000000 paper-qa-1.6.2/paperqa/qaprompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-05-18 03:14:41.000000 paper-qa-1.6.2/paperqa/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-18 03:14:41.000000 paper-qa-1.6.2/paperqa/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-18 03:14:41.000000 paper-qa-1.6.2/paperqa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-18 03:14:41.000000 paper-qa-1.6.2/paperqa/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 03:15:18.664700 paper-qa-1.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-18 03:14:41.000000 paper-qa-1.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:15:18.664700 paper-qa-1.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-05-18 03:14:41.000000 paper-qa-1.6.2/tests/test_paperqa.py
```

### Comparing `paper-qa-1.6.1/LICENSE` & `paper-qa-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `paper-qa-1.6.1/PKG-INFO` & `paper-qa-1.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 1.6.1
+Version: 1.6.2
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-1.6.1/README.md` & `paper-qa-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `paper-qa-1.6.1/paper_qa.egg-info/PKG-INFO` & `paper-qa-1.6.2/paper_qa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 1.6.1
+Version: 1.6.2
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-1.6.1/paperqa/agent.py` & `paper-qa-1.6.2/paperqa/agent.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.6.1/paperqa/contrib/zotero.py` & `paper-qa-1.6.2/paperqa/contrib/zotero.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.6.1/paperqa/docs.py` & `paper-qa-1.6.2/paperqa/docs.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,33 +212,51 @@
                 len(doc["texts"]),
                 doc["metadata"][0]["dockey"],
                 doc["metadata"][0]["citation"],
             )
             for doc in self.docs
         ]
 
-    def doc_match(self, query: str, k: int = 25) -> List[str]:
+    async def adoc_match(self, query: str, k: int = 25, callbacks: List[AsyncCallbackHandler] = []) -> List[str]:
         """Return a list of documents that match the query."""
         if len(self.docs) == 0:
             return ""
         if self._doc_index is None:
             texts = [doc["metadata"][0]["citation"] for doc in self.docs]
             metadatas = [{"key": doc["metadata"][0]["dockey"]}
                          for doc in self.docs]
             self._doc_index = FAISS.from_texts(
                 texts, metadatas=metadatas, embedding=self.embeddings
             )
         docs = self._doc_index.max_marginal_relevance_search(query, k=k)
         chain = make_chain(select_paper_prompt, self.summary_llm)
         papers = [f"{d.metadata['key']}: {d.page_content}" for d in docs]
-        result = chain.run(instructions=query, papers="\n".join(papers))
+        result = await chain.arun(instructions=query, papers="\n".join(papers),
+                                  callbacks=callbacks)
         return result
 
-    # to pickle, we have to save the index as a file
 
+    def doc_match(self, query: str, k: int = 25, callbacks: List[AsyncCallbackHandler] = []) -> List[str]:
+        """Return a list of documents that match the query."""
+        if len(self.docs) == 0:
+            return ""
+        if self._doc_index is None:
+            texts = [doc["metadata"][0]["citation"] for doc in self.docs]
+            metadatas = [{"key": doc["metadata"][0]["dockey"]}
+                         for doc in self.docs]
+            self._doc_index = FAISS.from_texts(
+                texts, metadatas=metadatas, embedding=self.embeddings
+            )
+        docs = self._doc_index.max_marginal_relevance_search(query, k=k)
+        chain = make_chain(select_paper_prompt, self.summary_llm)
+        papers = [f"{d.metadata['key']}: {d.page_content}" for d in docs]
+        result = chain.run(instructions=query, papers="\n".join(papers),
+                                  callbacks=callbacks)
+        return result
+            
     def __getstate__(self):
         state = self.__dict__.copy()
         if self._faiss_index is not None:
             state["_faiss_index"].save_local(self.index_path)
         del state["_faiss_index"]
         del state["_doc_index"]
         return state
@@ -347,19 +365,18 @@
                     context_str=doc.page_content,
                     citation=doc.metadata["citation"],
                     callbacks=callbacks,
                 ),
                 text=doc.page_content,
             )
             if "Not applicable" not in c.context:
-                return c, cb
+                return c, callbacks[0]
             return None, None
 
-        with get_openai_callback() as cb:
-            results = await asyncio.gather(*[process(doc) for doc in docs])
+        results = await asyncio.gather(*[process(doc) for doc in docs])
         # filter out failures
         results = [r for r in results if r[0] is not None]
         answer.tokens += sum([cb.total_tokens for _, cb in results])
         answer.cost += sum([cb.total_cost for _, cb in results])
         contexts = [c for c, _ in results if c is not None]
         if len(contexts) == 0:
             return answer
@@ -448,18 +465,18 @@
     ) -> Answer:
         if k < max_sources:
             raise ValueError("k should be greater than max_sources")
         if answer is None:
             answer = Answer(query)
         if len(answer.contexts) == 0:
             if key_filter or (key_filter is None and len(self.docs) > 5):
-                with get_openai_callback() as cb:
-                    keys = self.doc_match(answer.question)
-                answer.tokens += cb.total_tokens
-                answer.cost += cb.total_cost
+                callbacks = [OpenAICallbackHandler()] + get_callbacks("filter")
+                keys = await self.adoc_match(answer.question, callbacks=callbacks)
+                answer.tokens += callbacks[0].total_tokens
+                answer.cost += callbacks[0].total_cost
             answer = await self.aget_evidence(
                 answer,
                 k=k,
                 max_sources=max_sources,
                 marginal_relevance=marginal_relevance,
                 key_filter=keys if key_filter else None,
                 get_callbacks=get_callbacks,
```

### Comparing `paper-qa-1.6.1/paperqa/qaprompts.py` & `paper-qa-1.6.2/paperqa/qaprompts.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         except NotImplementedError as e:
             return self.generate(input_list, run_manager=run_manager)
 
 
 def make_chain(prompt, llm):
     if type(llm) == ChatOpenAI:
         system_message_prompt = SystemMessage(
-            content="You are a scholarly researcher that answers in an unbiased, scholarly tone. "
+            content="You are a scholarly researcher that answers in an unbiased, concise, scholarly tone. "
             "You sometimes refuse to answer if there is insufficient information.",
         )
         human_message_prompt = HumanMessagePromptTemplate(prompt=prompt)
         prompt = ChatPromptTemplate.from_messages(
             [system_message_prompt, human_message_prompt]
         )
     return FallbackLLMChain(prompt=prompt, llm=llm)
```

### Comparing `paper-qa-1.6.1/paperqa/readers.py` & `paper-qa-1.6.2/paperqa/readers.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.6.1/paperqa/types.py` & `paper-qa-1.6.2/paperqa/types.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.6.1/paperqa/utils.py` & `paper-qa-1.6.2/paperqa/utils.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.6.1/setup.py` & `paper-qa-1.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     author="Andrew White",
     author_email="white.d.andrew@gmail.com",
     url="https://github.com/whitead/paper-qa",
     license="MIT",
     packages=["paperqa", "paperqa.contrib"],
     install_requires=[
         "pypdf",
-        "langchain>=0.0.170",
+        "langchain>=0.0.172",
         "openai>=0.27.0",
         "faiss-cpu",
         "PyCryptodome",
         "html2text",
         "tiktoken",
         "rmrkl>=0.0.2",
     ],
```

### Comparing `paper-qa-1.6.1/tests/test_paperqa.py` & `paper-qa-1.6.2/tests/test_paperqa.py`

 * *Files identical despite different names*

