# Comparing `tmp/pypreql-nlp-0.0.6.tar.gz` & `tmp/pypreql-nlp-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypreql-nlp-0.0.6.tar", last modified: Sat May 13 00:14:31 2023, max compression
+gzip compressed data, was "pypreql-nlp-0.0.7.tar", last modified: Thu May 18 02:09:59 2023, max compression
```

## Comparing `pypreql-nlp-0.0.6.tar` & `pypreql-nlp-0.0.7.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:14:31.230543 pypreql-nlp-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-13 00:14:31.230543 pypreql-nlp-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-13 00:14:16.000000 pypreql-nlp-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:14:31.230543 pypreql-nlp-0.0.6/preql_nlp/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-13 00:14:16.000000 pypreql-nlp-0.0.6/preql_nlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:14:31.230543 pypreql-nlp-0.0.6/preql_nlp/cache_providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 00:14:16.000000 pypreql-nlp-0.0.6/preql_nlp/cache_providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-13 00:14:16.000000 pypreql-nlp-0.0.6/preql_nlp/cache_providers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-13 00:14:16.000000 pypreql-nlp-0.0.6/preql_nlp/cache_providers/local_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-13 00:14:16.000000 pypreql-nlp-0.0.6/preql_nlp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-13 00:14:16.000000 pypreql-nlp-0.0.6/preql_nlp/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-05-13 00:14:16.000000 pypreql-nlp-0.0.6/preql_nlp/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-13 00:14:16.000000 pypreql-nlp-0.0.6/preql_nlp/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-13 00:14:16.000000 pypreql-nlp-0.0.6/preql_nlp/monkeypatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:14:31.230543 pypreql-nlp-0.0.6/preql_nlp/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-13 00:14:16.000000 pypreql-nlp-0.0.6/preql_nlp/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-13 00:14:16.000000 pypreql-nlp-0.0.6/preql_nlp/prompts/final_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7317 2023-05-13 00:14:16.000000 pypreql-nlp-0.0.6/preql_nlp/prompts/prompt_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-13 00:14:16.000000 pypreql-nlp-0.0.6/preql_nlp/prompts/query_semantic_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-13 00:14:16.000000 pypreql-nlp-0.0.6/preql_nlp/prompts/semantic_to_tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:14:31.230543 pypreql-nlp-0.0.6/pypreql_nlp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-13 00:14:31.000000 pypreql-nlp-0.0.6/pypreql_nlp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-13 00:14:31.000000 pypreql-nlp-0.0.6/pypreql_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 00:14:31.000000 pypreql-nlp-0.0.6/pypreql_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-13 00:14:31.000000 pypreql-nlp-0.0.6/pypreql_nlp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-13 00:14:31.000000 pypreql-nlp-0.0.6/pypreql_nlp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-13 00:14:16.000000 pypreql-nlp-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 00:14:31.230543 pypreql-nlp-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-13 00:14:16.000000 pypreql-nlp-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:09:59.578977 pypreql-nlp-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-18 02:09:59.578977 pypreql-nlp-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-18 02:09:47.000000 pypreql-nlp-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:09:59.578977 pypreql-nlp-0.0.7/preql_nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-18 02:09:47.000000 pypreql-nlp-0.0.7/preql_nlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:09:59.578977 pypreql-nlp-0.0.7/preql_nlp/cache_providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 02:09:47.000000 pypreql-nlp-0.0.7/preql_nlp/cache_providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-18 02:09:47.000000 pypreql-nlp-0.0.7/preql_nlp/cache_providers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-18 02:09:47.000000 pypreql-nlp-0.0.7/preql_nlp/cache_providers/local_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-18 02:09:47.000000 pypreql-nlp-0.0.7/preql_nlp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-18 02:09:47.000000 pypreql-nlp-0.0.7/preql_nlp/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-05-18 02:09:47.000000 pypreql-nlp-0.0.7/preql_nlp/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-18 02:09:47.000000 pypreql-nlp-0.0.7/preql_nlp/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-18 02:09:47.000000 pypreql-nlp-0.0.7/preql_nlp/monkeypatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:09:59.578977 pypreql-nlp-0.0.7/preql_nlp/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-18 02:09:47.000000 pypreql-nlp-0.0.7/preql_nlp/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-05-18 02:09:47.000000 pypreql-nlp-0.0.7/preql_nlp/prompts/prompt_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-18 02:09:47.000000 pypreql-nlp-0.0.7/preql_nlp/prompts/prompt_final_concepts.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-18 02:09:47.000000 pypreql-nlp-0.0.7/preql_nlp/prompts/prompt_query_semantic_groupings.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-18 02:09:47.000000 pypreql-nlp-0.0.7/preql_nlp/prompts/prompt_refine_filter.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-18 02:09:47.000000 pypreql-nlp-0.0.7/preql_nlp/prompts/prompt_semantic_to_tokens.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:09:59.578977 pypreql-nlp-0.0.7/pypreql_nlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-18 02:09:59.000000 pypreql-nlp-0.0.7/pypreql_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-18 02:09:59.000000 pypreql-nlp-0.0.7/pypreql_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 02:09:59.000000 pypreql-nlp-0.0.7/pypreql_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-18 02:09:59.000000 pypreql-nlp-0.0.7/pypreql_nlp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-18 02:09:59.000000 pypreql-nlp-0.0.7/pypreql_nlp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-18 02:09:47.000000 pypreql-nlp-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 02:09:59.578977 pypreql-nlp-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-18 02:09:47.000000 pypreql-nlp-0.0.7/setup.py
```

### Comparing `pypreql-nlp-0.0.6/PKG-INFO` & `pypreql-nlp-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypreql-nlp
-Version: 0.0.6
+Version: 0.0.7
 Summary: NLP interface for pypreql.
 Home-page: 
 Author: 
 Author-email: pypreql-community@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pypreql-nlp-0.0.6/README.md` & `pypreql-nlp-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pypreql-nlp-0.0.6/preql_nlp/cache_providers/local_sqlite.py` & `pypreql-nlp-0.0.7/preql_nlp/cache_providers/local_sqlite.py`

 * *Files identical despite different names*

### Comparing `pypreql-nlp-0.0.6/preql_nlp/helpers.py` & `pypreql-nlp-0.0.7/preql_nlp/helpers.py`

 * *Files identical despite different names*

### Comparing `pypreql-nlp-0.0.6/preql_nlp/main.py` & `pypreql-nlp-0.0.7/preql_nlp/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 from preql.core.models import Environment
 from preql_nlp.prompts import (
     run_prompt,
     SemanticToTokensPromptCase,
     SelectionPromptCase,
     SemanticExtractionPromptCase,
+    FilterRefinementCase,
 )
 from preql_nlp.constants import logger, DEFAULT_LIMIT
 from preql_nlp.models import (
     InitialParseResponse,
     OrderResult,
     FilterResult,
     TokenInputs,
@@ -141,62 +142,80 @@
     metrics = build_token_list_by_purpose(concepts, (Purpose.METRIC,))
     dimensions = build_token_list_by_purpose(
         concepts, (Purpose.KEY, Purpose.PROPERTY, Purpose.CONSTANT)
     )
 
     session_uuid = uuid.uuid4()
 
-    parsed: InitialParseResponse = run_prompt(
+    parsed: InitialParseResponse = run_prompt(  # type:ignore
         SemanticExtractionPromptCase(input_text),
         debug=debug,
         log_info=log_info,
         session_uuid=session_uuid,
     )
-    order = [x.concept for x in parsed.order]
-    filtering = [f.concept for f in parsed.filtering]
+    filtering = build_token_list_by_purpose(
+        concepts, (Purpose.METRIC, Purpose.KEY, Purpose.CONSTANT, Purpose.PROPERTY)
+    )
+    order = list(set(filtering + metrics + dimensions))
     token_inputs = TokenInputs(
         metrics=metrics, dimensions=dimensions, order=order, filtering=filtering
     )
 
     output: List[str] = []
     for field in ["metrics", "dimensions", "filtering", "order"]:
         local_phrases = [get_phrase_from_x(x) for x in getattr(parsed, field)]
-        phrase_tokens: SemanticTokenResponse = run_prompt( # type: ignore
-            SemanticToTokensPromptCase(
-                phrases=local_phrases, tokens=getattr(token_inputs, field)
-            ),
+        all_tokens = getattr(token_inputs, field)
+        phrase_tokens: SemanticTokenResponse = run_prompt(  # type: ignore
+            SemanticToTokensPromptCase(phrases=local_phrases, tokens=all_tokens),
             debug=True,
             session_uuid=session_uuid,
             log_info=log_info,
         )
         token_universe = []
         for mapping in phrase_tokens:
             token_universe += mapping.tokens
         for mapping in phrase_tokens:
-            concepts = tokens_to_concept(
-                mapping.tokens,
-                [c for c in final_concept_list],
-                limits=5,
-                universe=token_universe,
-            )
-            logger.info(f"For phrase {mapping.phrase} got {concepts}")
-            if concepts:
-                output += concepts
-            else:
+            found = False
+            for universe in [token_universe]:
+                concepts = tokens_to_concept(
+                    mapping.tokens,
+                    [c for c in final_concept_list],
+                    limits=5,
+                    universe=universe,
+                )
+                if concepts:
+                    logger.info(f"For phrase {mapping.phrase} got {concepts}")
+                    output += concepts
+                    found = True
+                    break
+            if not found:
                 raise ValueError(
                     f"Could not find concept for input {mapping.phrase} with tokens {mapping.tokens}"
                 )
-    selections: ConceptSelectionResponse = run_prompt( # type: ignore
+    selections: ConceptSelectionResponse = run_prompt(  # type: ignore
         SelectionPromptCase(concepts=output, question=input_text),
         debug=debug,
         session_uuid=session_uuid,
         log_info=log_info,
     )
     final = list(set(selections.matches))
 
+    for item in parsed.filtering:
+        instance = input_environment.concepts[item.concept]
+        if instance.metadata:
+            item.values = run_prompt(  # type: ignore
+                FilterRefinementCase(
+                    values=item.values,
+                    description=instance.metadata.description,
+                ),
+                debug=debug,
+                session_uuid=session_uuid,
+                log_info=log_info,
+            ).new_values
+
     return IntermediateParseResults(
         select=final,
         limit=parsed.limit or 20,
         order=parsed.order,
         filtering=parsed.filtering,
     )
 
@@ -236,16 +255,14 @@
     for order in ordering:
         parsed = safe_parse_order_item(order, input_concepts)
         if parsed:
             final.append(parsed)
     return OrderBy(items=final)
 
 
-
-
 def parse_filter(
     input: FilterResult, input_concepts: List[Concept]
 ) -> Comparison | None:
     matched = [c for c in input_concepts if input.concept in c.address]
     if not matched:
         return None
     return Comparison(
```

### Comparing `pypreql-nlp-0.0.6/preql_nlp/models.py` & `pypreql-nlp-0.0.7/preql_nlp/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,15 +32,17 @@
     dimensions:list[str]
     limit:int
     order:list[OrderResult]
     filtering:list[FilterResult]
 
     @property
     def selection(self)->list[str]:
-        return self.metrics + self.dimensions
+        filtering = [f.concept for f in self.filtering]
+        order = [x.concept for x in self.order]
+        return self.metrics + self.dimensions + filtering + order
 
 
 class SemanticTokenMatch(BaseModel):
     phrase: str
     tokens: list[str]
 
 class SemanticTokenResponse(BaseModel):
@@ -59,7 +61,13 @@
 
 
 class IntermediateParseResults(BaseModel):
     select: list[str]
     limit: int
     order: list[OrderResult]
     filtering:list[FilterResult]
+
+
+class FilterRefinementResponse(BaseModel):
+    new_values:list[str]
+    old_values:list[str]
+    reasoning:str
```

### Comparing `pypreql-nlp-0.0.6/preql_nlp/monkeypatch.py` & `pypreql-nlp-0.0.7/preql_nlp/monkeypatch.py`

 * *Files identical despite different names*

### Comparing `pypreql-nlp-0.0.6/preql_nlp/prompts/final_selection.py` & `pypreql-nlp-0.0.7/preql_nlp/prompts/prompt_final_concepts.jinja2`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-SELECTION_TEMPLATE_V1 = """
 System: You are a helpful AI that selects the most relevant matching concepts to answer a question from a provided list.
 
 Guidelines:
 * you can assume the user will always provide a list of phrases
 * you can assume the user will always provide a question
 * only return concepts provided by the user
 * concepts are dot seperated and in quotes, e.g. "sales" or "product.revenue"
@@ -18,12 +17,10 @@
 User: concepts: ["product.color", "order.state", "order.year", "order.revenue.sum", "order.revenue.avg", "product.name", "order.month", "order.day", "product.manufacturer"] question: "What are the sales by state?"
 System:
 {"matches": ["order.state", "order.revenue.sum"],
 "reasoning": "order.state is the best match for state when looking at revenue, and order.revenue.sum would enable aggregating revenue." }
 User: concepts: ["product.color", "order.state", "order.year", "order.revenue.sum", "order.revenue.avg", "product.name", "order.month", "order.day", "product.manufacturer"]  question: "What are the average sales by state?"
 System:
 {"matches": ["order.state", "order.revenue.avg"],
-"reasoning": "order.state is the best match for state, and order.revenue.avg would capture average revenue." }{% endraw %}
+"reasoning": "order.state is the best match for state, and order.revenue.avg references the average of revenue for an order, which is conceptually closest to sales." }{% endraw %}
 User: concepts: [{{ concept_string }}] question: "{{ question }}"
-System:
-
-"""
+System:
```

### Comparing `pypreql-nlp-0.0.6/preql_nlp/prompts/prompt_executor.py` & `pypreql-nlp-0.0.7/preql_nlp/prompts/prompt_executor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,58 @@
 # Brining some "prompt generator" classes - note that you can derive and extend those
 from promptimize.prompt_cases import TemplatedPromptCase
 
 # Bringing some useful eval function that help evaluating and scoring responses
 # eval functions have a handle on the prompt object and are expected
 # to return a score between 0 and 1
 from preql_nlp.constants import logger
-from preql_nlp.prompts.query_semantic_extraction import EXTRACTION_PROMPT_V1
-from preql_nlp.prompts.semantic_to_tokens import STRUCTURED_PROMPT_V1
-from preql_nlp.prompts.final_selection import SELECTION_TEMPLATE_V1
 from preql_nlp.models import (
     InitialParseResponse,
     ConceptSelectionResponse,
     SemanticTokenResponse,
+    FilterRefinementResponse,
 )
 from preql_nlp.cache_providers.base import BaseCache
 from preql_nlp.cache_providers.local_sqlite import SqlliteCache
 from preql_nlp.helpers import retry_with_exponential_backoff
 from pydantic import BaseModel, ValidationError
 from typing import List, Optional, Callable, Union, Type, overload
 import uuid
 import json
 import os
+from jinja2 import FileSystemLoader, Environment, Template
+from os.path import dirname
+
+loader = FileSystemLoader(searchpath=dirname(__file__))
+templates = Environment(loader=loader)
 
 
 def gen_hash(obj, keys: set[str]) -> str:
     """Generate a deterministic hash for an object across multiple runs"""
     import hashlib
 
     m = hashlib.sha256(usedforsecurity=False)
 
     # we need to hash things in a deterministic order
     key_list = sorted(list(keys), key=lambda x: x)
     for key in key_list:
-        s = str(getattr(obj, key))
+        x = getattr(obj, key)
+        if isinstance(x, Template):
+            s = x.render()
+        else:
+            s = str(x)
 
         m.update(s.encode("utf-8"))
 
     return m.digest().hex()
 
 
 class BasePreqlPromptCase(TemplatedPromptCase):
     parse_model: Type[BaseModel]
+    template: Template
 
     def __init__(
         self,
         category: str,
         fail_on_parse_error: bool = True,
         evaluators: Optional[Union[Callable, List[Callable]]] = None,
     ):
@@ -71,22 +79,28 @@
     def get_extra_template_context(self):
         raise NotImplementedError("This class can't be used directly.")
 
     def post_run(self):
         try:
             self.parsed = self.parse_model.parse_raw(self.response)
         except ValidationError as e:
+            print(self.render())
             print("was unable to parse response using ", str(self.parse_model))
             print(self.response)
             if self.fail_on_parse_error:
                 raise e
 
+    def render(
+        self,
+    ):
+        return self.template.render(**self.jinja_context)
+
 
 class SemanticExtractionPromptCase(BasePreqlPromptCase):
-    template = EXTRACTION_PROMPT_V1
+    template = templates.get_template("prompt_query_semantic_groupings.jinja2")
     parse_model = InitialParseResponse
 
     attributes_used_for_hash = {"category", "question", "template"}
 
     def __init__(
         self,
         question: str,
@@ -96,38 +110,38 @@
         super().__init__(category="semantic_extraction", evaluators=evaluators)
 
     def get_extra_template_context(self):
         return {"question": self.question}
 
 
 class SemanticToTokensPromptCase(BasePreqlPromptCase):
-    template = STRUCTURED_PROMPT_V1
+    template = templates.get_template("prompt_semantic_to_tokens.jinja2")
     parse_model = SemanticTokenResponse
 
     attributes_used_for_hash = {"tokens", "phrases", "category", "template"}
 
     def __init__(
         self,
         tokens: List[str],
         phrases: List[str],
         evaluators: Optional[Union[Callable, List[Callable]]] = None,
     ):
-        self.tokens = tokens
-        self.phrases = phrases
+        self.tokens = sorted(tokens)
+        self.phrases = sorted(phrases)
         super().__init__(category="semantic_to_tokens", evaluators=evaluators)
 
     def get_extra_template_context(self):
         return {
-            "tokens": self.tokens,
+            "tokens": ", ".join([f'"{c}"' for c in self.tokens]),
             "phrase_str": ", ".join([f'"{c}"' for c in self.phrases]),
         }
 
 
 class SelectionPromptCase(BasePreqlPromptCase):
-    template = SELECTION_TEMPLATE_V1
+    template = templates.get_template("prompt_final_concepts.jinja2")
     parse_model = ConceptSelectionResponse
 
     attributes_used_for_hash = {"question", "concepts", "category", "template"}
 
     def __init__(
         self,
         question: str,
@@ -142,25 +156,48 @@
     def get_extra_template_context(self):
         return {
             "concept_string": ", ".join([f'"{c}"' for c in self.concepts]),
             "question": self.question,
         }
 
 
+class FilterRefinementCase(BasePreqlPromptCase):
+    template = templates.get_template("prompt_refine_filter.jinja2")
+    parse_model = FilterRefinementResponse
+
+    attributes_used_for_hash = {"values", "description", "template"}
+
+    def __init__(
+        self,
+        values: list[str],
+        description: str,
+        evaluators: Optional[Union[Callable, List[Callable]]] = None,
+    ):
+        self.values = values
+        self.description = description
+        super().__init__(evaluators=evaluators, category="filter_refinement")
+
+    def get_extra_template_context(self):
+        return {
+            "values": ", ".join([f'"{x}"' for x in self.values]),
+            "description": self.description,
+        }
+
+
 DATA_DIR = os.path.join(
     os.path.dirname(os.path.dirname(os.path.abspath(__file__))), "log_data"
 )
 if not os.path.exists(DATA_DIR):
     os.makedirs(DATA_DIR)
 
 
 def log_prompt_info(prompt: TemplatedPromptCase, session_uuid: uuid.UUID):
     prompt_hash = prompt.prompt_hash
     prompt_context = prompt.jinja_context
-    template = prompt.template
+    template = prompt.template.render(**prompt.jinja_context)
     category = prompt.category
 
     data = {
         "prompt_token": prompt_hash,
         "prompt_context": prompt_context,
         "template": template,
         "category": category,
@@ -175,14 +212,24 @@
                 os.path.join(DATA_DIR, str(session_uuid), prompt_hash + ".json")
             )
         )
         json.dump(data, f)
 
 
 @overload
+def run_prompt( # type: ignore
+    prompt: SelectionPromptCase,
+    debug: bool = False,
+    log_info: bool = True,
+    session_uuid: uuid.UUID | None = None,
+) -> ConceptSelectionResponse:
+    ...
+
+
+@overload
 def run_prompt(  # type: ignore
     prompt: SemanticExtractionPromptCase,
     debug: bool = False,
     log_info: bool = True,
     session_uuid: uuid.UUID | None = None,
 ) -> InitialParseResponse:
     ...
@@ -195,29 +242,34 @@
     log_info: bool = True,
     session_uuid: uuid.UUID | None = None,
 ) -> SemanticTokenResponse:
     ...
 
 
 @overload
-def run_prompt(
-    prompt: SelectionPromptCase,
+def run_prompt( # type: ignore
+    prompt: FilterRefinementCase,
     debug: bool = False,
     log_info: bool = True,
     session_uuid: uuid.UUID | None = None,
-) -> ConceptSelectionResponse:
+) -> FilterRefinementResponse:
     ...
 
 
 def run_prompt(
     prompt: BasePreqlPromptCase,
     debug: bool = False,
     log_info: bool = True,
     session_uuid: uuid.UUID | None = None,
-) -> ConceptSelectionResponse | SemanticTokenResponse | InitialParseResponse:
+) -> (
+    ConceptSelectionResponse
+    | SemanticTokenResponse
+    | InitialParseResponse
+    | FilterRefinementResponse
+):
     if not session_uuid:
         session_uuid = uuid.uuid4()
 
     if log_info and not os.path.exists(os.path.join(DATA_DIR, str(session_uuid))):
         os.makedirs(os.path.join(DATA_DIR, str(session_uuid)))
     if debug:
         logger.debug("prompt")
```

### Comparing `pypreql-nlp-0.0.6/preql_nlp/prompts/query_semantic_extraction.py` & `pypreql-nlp-0.0.7/preql_nlp/prompts/prompt_query_semantic_groupings.jinja2`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-
-
-EXTRACTION_PROMPT_V1 = """
 System: You are a helpful AI that translates ambiguous business questions into structured outputs.
 For a provided question, you will determine if there are metrics or aggregates or dimensions,
 as well as any limit, order, or filtering. 
 
 The output should be a VALID JSON blob with the following keys and values:
 - metrics: a list of concepts from the question that should be aggregated
 - dimensions: a list of concepts from the question which are not metrics
@@ -55,9 +52,8 @@
 "dimensions": ["year"],
 "limit": -1,
 "order": [{"concept":"year", "order":"asc"}],
 "filtering": [{"concept":"year", "operator":">=", "values":["2001"]}, {"concept":"year", "operator":"<=", "values":["2020"]}]
 }{% endraw %}
 
 User: "{{ question }}"
-System:
-"""
+System:
```

### Comparing `pypreql-nlp-0.0.6/preql_nlp/prompts/semantic_to_tokens.py` & `pypreql-nlp-0.0.7/preql_nlp/prompts/prompt_semantic_to_tokens.jinja2`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-
-STRUCTURED_PROMPT_V1 = """\
-System: you are an AI that helps a user map phrases to tokens by associating a phrase with tokens related to the words
+System: you are an AI that helps a user map phrases to tokens by associating a phrase with tokens most related to the words
 in the phrase.
 Guidelines:
 * you can assume the user will always provide a list of phrases
 * you can assume the user will always provide a list of tokens
-* only return tokens provided by the user
+* only return tokens that appear in the list provided by the user
 * If a phrase has no matches, return an empty array
 The output should be a VALID JSON list with each entry having the following keys
 * phrase, the input phrase
 * tokens, a list of matching token strings
 
 
 User: given the tokens ["color", "product", "year", "revenue"], match tokens to the phrases ["product revenue", "product color", "product revenue by year", "yearly revenue"]
@@ -42,14 +40,24 @@
       "phrase":"yearly revenue",
       "tokens":[
          "revenue",
          "year"
       ]
    }   
 ]
+User: given the tokens ["product", "count", "order", "year"], match tokens to the phrases ["fairy_dust"]
+System:
+[
+   {
+      "phrase":"fairy_dust",
+      "tokens":[
+         "product"
+      ]
+   }
+]
 User: given the tokens ["product", "count", "order", "year"], match tokens to the phrases ["products sold", "orders"]
 System:
 [
    {
       "phrase":"products_sold",
       "tokens":[
          "product",
@@ -60,11 +68,9 @@
       "phrase":"orders",
       "tokens":[
          "order",
          "count"
       ]
    }
 ]{% endraw %}
-User: Given the tokens {{ tokens }}, match tokens to the phrases [{{ phrase_str }}]
-System:
-"""
-
+User: Given the tokens [{{ tokens }}], match tokens to the phrases [{{ phrase_str }}]
+System:
```

### Comparing `pypreql-nlp-0.0.6/pypreql_nlp.egg-info/PKG-INFO` & `pypreql-nlp-0.0.7/pypreql_nlp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypreql-nlp
-Version: 0.0.6
+Version: 0.0.7
 Summary: NLP interface for pypreql.
 Home-page: 
 Author: 
 Author-email: pypreql-community@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pypreql-nlp-0.0.6/setup.py` & `pypreql-nlp-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             "docs",
             ".github",
             "",
             "examples",
         ]
     ),
     package_data={
-        "": ["*.tf", "*.jinja", "py.typed"],
+        "": ["*.tf", "*.jinja2", "py.typed"],
     },
     install_requires=install_requires,
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
```

