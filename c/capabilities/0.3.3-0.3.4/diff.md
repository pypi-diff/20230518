# Comparing `tmp/capabilities-0.3.3.tar.gz` & `tmp/capabilities-0.3.4.tar.gz`

## Comparing `capabilities-0.3.3.tar` & `capabilities-0.3.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 capabilities-0.3.3/setup.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 capabilities-0.3.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 capabilities-0.3.3/capabilities/__about__.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 capabilities-0.3.3/capabilities/__init__.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 capabilities-0.3.3/capabilities/__main__.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 capabilities-0.3.3/capabilities/cli.py
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 capabilities-0.3.3/capabilities/config.py
--rw-r--r--   0        0        0    12375 2020-02-02 00:00:00.000000 capabilities-0.3.3/capabilities/core.py
--rw-r--r--   0        0        0     8071 2020-02-02 00:00:00.000000 capabilities-0.3.3/capabilities/dec.py
--rw-r--r--   0        0        0    15162 2020-02-02 00:00:00.000000 capabilities-0.3.3/capabilities/example.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 capabilities-0.3.3/capabilities/search/__init__.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 capabilities-0.3.3/capabilities/search/hf.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 capabilities-0.3.3/capabilities/search/loader.py
--rw-r--r--   0        0        0     6082 2020-02-02 00:00:00.000000 capabilities-0.3.3/capabilities/search/nomic_index.py
--rw-r--r--   0        0        0     6567 2020-02-02 00:00:00.000000 capabilities-0.3.3/capabilities/search/oai.py
--rw-r--r--   0        0        0    12426 2020-02-02 00:00:00.000000 capabilities-0.3.3/capabilities/search/search_index.py
--rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 capabilities-0.3.3/capabilities/search/simple_vector_index.py
--rw-r--r--   0        0        0     7076 2020-02-02 00:00:00.000000 capabilities-0.3.3/capabilities/search/types.py
--rw-r--r--   0        0        0     5313 2020-02-02 00:00:00.000000 capabilities-0.3.3/capabilities/search/util.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 capabilities-0.3.3/capabilities/util/__init__.py
--rw-r--r--   0        0        0     9213 2020-02-02 00:00:00.000000 capabilities-0.3.3/capabilities/util/config.py
--rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 capabilities-0.3.3/capabilities/util/misc.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 capabilities-0.3.3/examples/cheese.py
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 capabilities-0.3.3/examples/leansearch.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 capabilities-0.3.3/examples/readme.txt
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 capabilities-0.3.3/examples/tesla10k.py
--rw-r--r--   0        0        0   840980 2020-02-02 00:00:00.000000 capabilities-0.3.3/examples/data/apple10k.pdf
--rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 capabilities-0.3.3/examples/data/sample.md
--rw-r--r--   0        0        0     7945 2020-02-02 00:00:00.000000 capabilities-0.3.3/examples/data/sample.pdf
--rw-r--r--   0        0        0   157134 2020-02-02 00:00:00.000000 capabilities-0.3.3/examples/data/tesla10k.txt
--rw-r--r--   0        0        0     5476 2020-02-02 00:00:00.000000 capabilities-0.3.3/tests/test_docs.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 capabilities-0.3.3/tests/test_document_loader.py
--rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 capabilities-0.3.3/tests/test_search.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 capabilities-0.3.3/tests/test_search_util.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 capabilities-0.3.3/tests/test_tutorial1.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 capabilities-0.3.3/tests/test_vector_idx.py
--rw-r--r--   0        0        0   353564 2020-02-02 00:00:00.000000 capabilities-0.3.3/tests/snapshots/test_search/test_search_e2e/NomicIndex-openai/r0.txt
--rw-r--r--   0        0        0   353563 2020-02-02 00:00:00.000000 capabilities-0.3.3/tests/snapshots/test_search/test_search_e2e/NomicIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt
--rw-r--r--   0        0        0   353563 2020-02-02 00:00:00.000000 capabilities-0.3.3/tests/snapshots/test_search/test_search_e2e/SearchIndex-openai/r0.txt
--rw-r--r--   0        0        0   353565 2020-02-02 00:00:00.000000 capabilities-0.3.3/tests/snapshots/test_search/test_search_e2e/SearchIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 capabilities-0.3.3/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 capabilities-0.3.3/LICENSE
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 capabilities-0.3.3/README.md
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 capabilities-0.3.3/pyproject.toml
--rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 capabilities-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 capabilities-0.3.4/setup.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 capabilities-0.3.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 capabilities-0.3.4/capabilities/__about__.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 capabilities-0.3.4/capabilities/__init__.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 capabilities-0.3.4/capabilities/__main__.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 capabilities-0.3.4/capabilities/cli.py
+-rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 capabilities-0.3.4/capabilities/config.py
+-rw-r--r--   0        0        0    12240 2020-02-02 00:00:00.000000 capabilities-0.3.4/capabilities/core.py
+-rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 capabilities-0.3.4/capabilities/dec.py
+-rw-r--r--   0        0        0    15164 2020-02-02 00:00:00.000000 capabilities-0.3.4/capabilities/example.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 capabilities-0.3.4/capabilities/search/__init__.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 capabilities-0.3.4/capabilities/search/hf.py
+-rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 capabilities-0.3.4/capabilities/search/loader.py
+-rw-r--r--   0        0        0     6160 2020-02-02 00:00:00.000000 capabilities-0.3.4/capabilities/search/nomic_index.py
+-rw-r--r--   0        0        0     6507 2020-02-02 00:00:00.000000 capabilities-0.3.4/capabilities/search/oai.py
+-rw-r--r--   0        0        0    12504 2020-02-02 00:00:00.000000 capabilities-0.3.4/capabilities/search/search_index.py
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 capabilities-0.3.4/capabilities/search/simple_vector_index.py
+-rw-r--r--   0        0        0     7150 2020-02-02 00:00:00.000000 capabilities-0.3.4/capabilities/search/types.py
+-rw-r--r--   0        0        0     5375 2020-02-02 00:00:00.000000 capabilities-0.3.4/capabilities/search/util.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 capabilities-0.3.4/capabilities/util/__init__.py
+-rw-r--r--   0        0        0     9199 2020-02-02 00:00:00.000000 capabilities-0.3.4/capabilities/util/config.py
+-rw-r--r--   0        0        0     6698 2020-02-02 00:00:00.000000 capabilities-0.3.4/capabilities/util/misc.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 capabilities-0.3.4/examples/cheese.py
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 capabilities-0.3.4/examples/leansearch.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 capabilities-0.3.4/examples/readme.txt
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 capabilities-0.3.4/examples/tesla10k.py
+-rw-r--r--   0        0        0   840980 2020-02-02 00:00:00.000000 capabilities-0.3.4/examples/data/apple10k.pdf
+-rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 capabilities-0.3.4/examples/data/sample.md
+-rw-r--r--   0        0        0     7945 2020-02-02 00:00:00.000000 capabilities-0.3.4/examples/data/sample.pdf
+-rw-r--r--   0        0        0   157134 2020-02-02 00:00:00.000000 capabilities-0.3.4/examples/data/tesla10k.txt
+-rw-r--r--   0        0        0     5476 2020-02-02 00:00:00.000000 capabilities-0.3.4/tests/test_docs.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 capabilities-0.3.4/tests/test_document_loader.py
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 capabilities-0.3.4/tests/test_search.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 capabilities-0.3.4/tests/test_search_util.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 capabilities-0.3.4/tests/test_tutorial1.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 capabilities-0.3.4/tests/test_vector_idx.py
+-rw-r--r--   0        0        0   353564 2020-02-02 00:00:00.000000 capabilities-0.3.4/tests/snapshots/test_search/test_search_e2e/NomicIndex-openai/r0.txt
+-rw-r--r--   0        0        0   353563 2020-02-02 00:00:00.000000 capabilities-0.3.4/tests/snapshots/test_search/test_search_e2e/NomicIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt
+-rw-r--r--   0        0        0   353563 2020-02-02 00:00:00.000000 capabilities-0.3.4/tests/snapshots/test_search/test_search_e2e/SearchIndex-openai/r0.txt
+-rw-r--r--   0        0        0   353565 2020-02-02 00:00:00.000000 capabilities-0.3.4/tests/snapshots/test_search/test_search_e2e/SearchIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 capabilities-0.3.4/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 capabilities-0.3.4/LICENSE
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 capabilities-0.3.4/README.md
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 capabilities-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 capabilities-0.3.4/PKG-INFO
```

### Comparing `capabilities-0.3.3/.github/workflows/python-publish.yml` & `capabilities-0.3.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.3/capabilities/cli.py` & `capabilities-0.3.4/capabilities/cli.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.3/capabilities/config.py` & `capabilities-0.3.4/capabilities/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,17 +25,15 @@
     forward_openai: bool = False
     """ If this value is true, capabilities will forward your OPENAI_API_KEY to the capabilities API if it is present.
 
     This is useful if you want to use credits on your own OpenAI account or want to avoid rate limits.
     The capabilities server only knows this key for the duration of the API call. It is not stored.
     """
 
-    config_dir: Path = pydantic.Field(
-        default_factory=lambda: get_app_config_dir("capabilities")
-    )
+    config_dir: Path = pydantic.Field(default_factory=lambda: get_app_config_dir("capabilities"))
 
     @property
     def secrets_file(self) -> Optional[Path]:
         if self.config_dir.exists():
             return self.config_dir / "secrets.json"
         else:
             return None
```

### Comparing `capabilities-0.3.3/capabilities/core.py` & `capabilities-0.3.4/capabilities/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
 import dataclasses
 import typing
 import dacite
 from dataclasses import dataclass, field, is_dataclass
-from typing import Dict, Any, List, Type, TypeVar, Union, Literal
+from typing import Dict, Any, List, Type, Union, Literal
 from typing import Optional
 
 try:
-    from typing import TypeAlias
+    from typing import TypeAlias, TypeVar
 except:
-    from typing_extensions import TypeAlias
+    from typing_extensions import TypeAlias, TypeVar
 import requests
 import aiohttp
 import asyncio
 import time
 
 import aiohttp
 import dacite
@@ -136,25 +136,21 @@
                 A coroutine that resolves to a dictionary containing the answer returned
                 by the DocumentQA service.
             Raises:
                 Exception: When the retries hit maximum (8) times and nothing was returned.
     """
 
     def __call__(self, document: str, query: str):
-        print(
-            f"[DocumentQA] running query against document with {len(document)} characters"
-        )
+        print(f"[DocumentQA] running query against document with {len(document)} characters")
         return CONFIG.post_sync(
             "/blazon/documentqa", payload={"document": document, "query": query}
         )
 
     async def run_async(self, document: str, query: str):
-        print(
-            f"[DocumentQA] running query against document with {len(document)} characters"
-        )
+        print(f"[DocumentQA] running query against document with {len(document)} characters")
         return CONFIG.post_async(
             "/blazon/documentqa",
             payload={"document": document, "query": query},
         )
 
 
 @register("blazon/summarize")
@@ -182,23 +178,19 @@
                 document (str): The text to be summarized.
                 session (aiohttp.ClientSession, optional): An aiohttp client session. If not provided, a new one is created. Defaults to None.
             Returns:
                 Dict[str, Any]: A dictionary object representing the summary, with keys 'summary' (str) and 'score' (float).
     """
 
     def __call__(self, document: str):
-        print(
-            f"[Summarize] running query against document with {len(document)} characters"
-        )
+        print(f"[Summarize] running query against document with {len(document)} characters")
         return CONFIG.post_sync("/blazon/summarize", {"document": document})
 
     async def run_async(self, document: str):
-        print(
-            f"[Summarize] running query against document with {len(document)} characters"
-        )
+        print(f"[Summarize] running query against document with {len(document)} characters")
         return await CONFIG.post_async("/blazon/summarize", {"document": document})
 
 
 StructuredSchema: TypeAlias = Any
 
 
 def flatten_model(m: Type, path: list[str] = []) -> StructuredSchema:
@@ -219,22 +211,17 @@
                 f"can't deduce list type arg for {m} at {p}, please provide a type annotation to list.",
                 path,
             )
         t = flatten_model(args[0])
         return [t]
     elif isinstance(m, ModelMetaclass):
         fields: dict[str, ModelField] = m.__fields__  # type: ignore
-        return {
-            k: flatten_model(f.annotation, path=path + [k]) for k, f in fields.items()
-        }
+        return {k: flatten_model(f.annotation, path=path + [k]) for k, f in fields.items()}
     elif is_dataclass(m):
-        return {
-            f.name: flatten_model(f.type, path=path + [f.name])
-            for f in dataclasses.fields(m)
-        }
+        return {f.name: flatten_model(f.type, path=path + [f.name]) for f in dataclasses.fields(m)}
     elif m == str:
         return "string"
     elif m == bool:
         return "bool"
     elif m == float:
         return "float"
     elif m == int:
```

### Comparing `capabilities-0.3.3/capabilities/dec.py` & `capabilities-0.3.4/capabilities/dec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import sys
 from termcolor import colored
 import functools
 import ast
 import inspect
 import importlib
-from typing import Callable, Generic, ParamSpec, TypeVar, overload
+from typing import Callable, Generic, overload
+
+try:
+    from typing import ParamSpec, TypeVar
+except:
+    from typing_extensions import ParamSpec, TypeVar
 import warnings
 
 import requests
 from capabilities.config import CONFIG
 
 from capabilities.core import (
     StructuredSchema,
@@ -45,17 +50,15 @@
         else:
             # get instructions from docstring
             self.instructions = inspect.getdoc(func)
             if self.instructions is None:
                 warnings.warn(
                     "using AiFunction without instructions. Please add a docstring to the decorated function."
                 )
-                self.instructions = (
-                    "Please produce the given output from the given input."
-                )
+                self.instructions = "Please produce the given output from the given input."
         self.signature = inspect.signature(func)
         self.input_spec = {
             k: _flatten_param(p, path=[k]) for k, p in self.signature.parameters.items()
         }
         self.output_spec = flatten_model(self.signature.return_annotation)
 
     def __call__(self, *args: P.args, **kwargs: P.kwargs):
@@ -113,15 +116,14 @@
     if callable(args[0]):
         return decorator(args[0])
     else:
         return functools.partial(AiFunction, *args, **kwargs)
 
 
 def llm_inline(regenerate=True, num_tries=3):
-
     @llm
     def complete_code(initial_codes: str, codes_before: str, codes_after: str) -> str:
         """
         Given the initial lines of a function, the codes before the function, and the codes after the function,
         follow the docstring to complete the function so that
         1. the initial lines of the code remain unchanged.
         2. it executes without error in the context.
@@ -145,18 +147,18 @@
         code_before, code_after = get_llm_inline_context(func)
 
         for _ in range(num_tries):  # Try `num_tries` times
             print("[llm_inline] generating code")
             completed = complete_code("\n".join(lines[1:]), code_before, code_after)
 
             # Try to parse out the function body, but if unsuccessful, fall back to the original completion.
-            print("[llm_inline] postprocessing")            
+            print("[llm_inline] postprocessing")
             processed = postprocess(completed, func.__name__)
             completed = processed if processed else completed
-            print("[llm_inline] postprocessing complete")                        
+            print("[llm_inline] postprocessing complete")
             new_decorator = f"@llm_inline(regenerate=False)"
             # if input(f"The following code will be written to your file: \n{completed}\nContinue? (y/n) ") == "y":
             #     with open(inspect.getfile(func), "w") as f:
             #         f.write(f"{code_before}\n{new_decorator}\n{completed}\n{code_after}")
 
             #     # Reload the module and the functions
             #     # todo: reload the script itself could result in ModuleNotFoundError: spec not found for the module '__main__'.
@@ -165,15 +167,22 @@
             #         module = inspect.getmodule(func)
             #         importlib.reload(module)
             #         globals().update(vars(module))
             #         return getattr(module, func.__name__)
             #     except:
             #         exec(completed, globals())
             #         return globals()[func.__name__]
-            if input(colored("The following code will be written to your file: \n", "green") + colored(f"{completed}\n", "blue") + colored("Continue? (y/n) ", "green")) == "y":
+            if (
+                input(
+                    colored("The following code will be written to your file: \n", "green")
+                    + colored(f"{completed}\n", "blue")
+                    + colored("Continue? (y/n) ", "green")
+                )
+                == "y"
+            ):
                 with open(inspect.getfile(func), "w") as f:
                     f.write(f"{code_before}\n{new_decorator}\n{completed}\n{code_after}")
 
                 # Reload the module and the functions
                 # todo: reload the script itself could result in ModuleNotFoundError: spec not found for the module '__main__'.
                 #       Trying an dirty way but may need to explore best-practice later.
                 try:
@@ -181,27 +190,26 @@
                     importlib.reload(module)
                     globals().update(vars(module))
                     return getattr(module, func.__name__)
                 except:
                     exec(completed, globals())
                     return globals()[func.__name__]
 
-
     return wrapper
 
 
 def get_llm_inline_context(func) -> tuple[str, str]:
     source_path = inspect.getfile(func)
     lines, start_lineno = inspect.getsourcelines(func)
     end_lineno = start_lineno + len(lines)
 
     with open(source_path, "r") as f:
         file_content = f.read().split("\n")
 
-    return "\n".join(file_content[:start_lineno - 1]), "\n".join(file_content[end_lineno:])
+    return "\n".join(file_content[: start_lineno - 1]), "\n".join(file_content[end_lineno:])
 
 
 def postprocess(code: str, func_name: str) -> str:
     try:
         parsed = ast.parse(code)
     except SyntaxError:
         return ""
@@ -209,8 +217,7 @@
     for node in parsed.body:
         if isinstance(node, ast.FunctionDef) and node.name == func_name:
             node.decorator_list = []
             completed_func = ast.unparse(node)
             return completed_func
 
     return ""
-
```

### Comparing `capabilities-0.3.3/capabilities/example.py` & `capabilities-0.3.4/capabilities/example.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,16 @@
     class SupportedBulletPoint(BaseModel):
         """
         A class representing a supported bullet point in a document summary.
         A supported bullet point has a bullet point summarizing a passage from the text,
         as well as the supporting text itself, which is a passage of text extracted verbatim from the document.
         """
 
-        bullet_point: str # claim
-        supporting_text: str # verbatim passage fom the original document
+        bullet_point: str  # claim
+        supporting_text: str  # verbatim passage fom the original document
 
     class DocumentSummary(BaseModel):
         """
         A class representing a summary of a document, consisting of a list of supported bullet points.
         """
 
         supportedBulletPoints: List[SupportedBulletPoint]
```

### Comparing `capabilities-0.3.3/capabilities/search/hf.py` & `capabilities-0.3.4/capabilities/search/hf.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.3/capabilities/search/loader.py` & `capabilities-0.3.4/capabilities/search/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,17 +39,15 @@
     def id(self):
         return str(self.doc_id)
 
     def get_text(self) -> str:
         return self.text
 
 
-def create_document(
-    location: Union[str, Path], doc_id: Optional[str] = None
-) -> Document:
+def create_document(location: Union[str, Path], doc_id: Optional[str] = None) -> Document:
     """Create a document from a web url or file path.
 
     Args:
       - location: is a web url, or a path to a pdf, md, or txt file.
       - doc_id: is a unique identifier for the document, if not given then the location string will be used.
     """
     location = str(location)
@@ -64,22 +62,23 @@
         with open(location, "rb") as f:
             byte_content = f.read()
     else:
         raise ValueError(f"{location} is neither a local file nor a valid url")
 
     try:
         import magic
+
         mime = magic.Magic(mime=True)
         filetype = mime.from_buffer(byte_content)
     except ImportError:
         if os.path.isfile(location):
             mime, enc = mimetypes.guess_type(str(location))
             filetype = mime or ""
         else:
-            raise ImportError('Please install https://pypi.org/project/python-magic/')
+            raise ImportError("Please install https://pypi.org/project/python-magic/")
 
     if "application/pdf" in filetype:
         text = extract_text(io.BytesIO(byte_content))
     elif "html" in filetype:
         soup = BeautifulSoup(byte_content.decode(), "lxml")
         text = soup.get_text()
     else:
```

### Comparing `capabilities-0.3.3/capabilities/search/nomic_index.py` & `capabilities-0.3.4/capabilities/search/nomic_index.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 import math
-from typing import Generic, Iterable, Literal, Optional, TypeVar, get_args
+from typing import Generic, Iterable, Literal, Optional, get_args
+
+try:
+    from typing import TypeVar
+except:
+    from typing_extensions import TypeVar
 from .search_index import AbstractSearchIndex, SearchResult, get_chunks
 from .types import EmbeddingModel, TextItem, get_text, Chunk
 import numpy as np
 
 try:
     from nomic import atlas
 except ModuleNotFoundError:
```

### Comparing `capabilities-0.3.3/capabilities/search/oai.py` & `capabilities-0.3.4/capabilities/search/oai.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,17 +124,15 @@
 
 # [todo] throttling, retries
 @cache.memoize()
 def embeddings(params: EmbeddingRequest) -> EmbeddingResponse:
     resp = OpenAISettings().post("/v1/embeddings", json=params.dict(exclude_none=True))  # type: ignore
     j = resp.json()
     if resp.status_code // 100 == 4:
-        raise requests.HTTPError(
-            f"{resp.status_code}: {json.dumps(j, indent=2)}", response=resp
-        )
+        raise requests.HTTPError(f"{resp.status_code}: {json.dumps(j, indent=2)}", response=resp)
     resp.raise_for_status()
     r = EmbeddingResponse.parse_obj(j)
     return r
 
 
 @cache.memoize()
 def chat_completions(params: CompletionRequest) -> CompletionResponse:
@@ -190,17 +188,15 @@
         return starts, ends
 
     def encode(self, texts: list[str]):
         lengths = [self.count_tokens(text) for text in texts]
         N = self.max_tokens_per_item
         for i, l in enumerate(lengths):
             if l > N:
-                raise ValueError(
-                    f"{i}th text {texts[i]} is too long, please chunk it first"
-                )
+                raise ValueError(f"{i}th text {texts[i]} is too long, please chunk it first")
         batches = argbatch(lengths, N)
         es = []
         # its = track(batches) if len(batches) > 100 else batches
         its = batches
 
         def process_batch(batch, texts, embeddings, model_name):
             ts = texts[batch.start : batch.stop]
```

### Comparing `capabilities-0.3.3/capabilities/search/search_index.py` & `capabilities-0.3.4/capabilities/search/search_index.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,20 @@
 import asyncio
 from collections import defaultdict
 from dataclasses import dataclass, field
 import itertools
 import logging
 import math
 import re
-from typing import Any, Dict, Generic, Iterable, Optional, Tuple, TypeVar, Union
+from typing import Any, Dict, Generic, Iterable, Optional, Tuple, Union
+
+try:
+    from typing import TypeVar
+except:
+    from typing_extensions import TypeVar
 from .simple_vector_index import SimpleVectorIndex
 from .types import (
     Chunk,
     EmbeddingModel,
     TextItem,
     VectorIndex,
     get_text,
```

### Comparing `capabilities-0.3.3/capabilities/search/simple_vector_index.py` & `capabilities-0.3.4/capabilities/search/simple_vector_index.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.3/capabilities/search/types.py` & `capabilities-0.3.4/capabilities/search/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,21 @@
     Dict,
     Generic,
     Iterable,
     Optional,
     Protocol,
     Sequence,
     Tuple,
-    TypeVar,
     Union,
 )
+
+try:
+    from typing import TypeVar
+except:
+    from typing_extensions import TypeVar
 from capabilities.search.util import digest
 import numpy as np
 
 
 @dataclass
 class Chunk:
     """A Chunk is a subset of a TextItem.
```

### Comparing `capabilities-0.3.3/capabilities/search/util.py` & `capabilities-0.3.4/capabilities/search/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,21 +9,21 @@
     Callable,
     Iterable,
     Optional,
     Sequence,
     Tuple,
     Union,
     overload,
-    TypeVar,
 )
+
 try:
     from typing import TypeAlias
 except:
     from typing_extensions import TypeAlias
-    
+
 from hashlib import blake2b
 from diskcache import Cache
 
 K = TypeVar("K")
 T = TypeVar("T")
 U = TypeVar("U")
 V = TypeVar("V")
@@ -118,15 +118,20 @@
         yield window_start, window_end
         if window_end >= total_size:
             break
         window_start += step_size
 
 
 from functools import cached_property
-from typing import Callable, Generic, TypeVar
+from typing import Callable, Generic
+
+try:
+    from typing import TypeVar
+except:
+    from typing_extensions import TypeVar
 
 
 @overload
 def unzip(s: Iterable[tuple[U, V]]) -> tuple[list[U], list[V]]:
     ...
```

### Comparing `capabilities-0.3.3/capabilities/util/config.py` & `capabilities-0.3.4/capabilities/util/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,17 +64,15 @@
 
     p = find(cwd, "pyproject.toml")
     if p is not None:
         return p
     git_root = get_git_root()
     if git_root is not None:
         return Path(git_root)
-    logger.debug(
-        f"{cwd} is not in a git repository and no pyproject.toml could be found."
-    )
+    logger.debug(f"{cwd} is not in a git repository and no pyproject.toml could be found.")
     return None
 
 
 @functools.cache
 def get_app_config_dir(app_name: str) -> Path:
     """Get the path to the application directory.
```

### Comparing `capabilities-0.3.3/capabilities/util/misc.py` & `capabilities-0.3.4/capabilities/util/misc.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,19 @@
 import fire
 import os
 import requests
 import openai
 import random
 import tiktoken
 import concurrent.futures
-from typing import Callable, List, Any, TypeVar, Iterable, Optional
+from typing import Callable, List, Any, Iterable, Optional
+try:
+    from typing import TypeVar
+except:
+    from typing_extensions TypeVar
 import time
 from threading import Thread
 
 ENCODER = tiktoken.get_encoding("p50k_base")
 
 
 def tokenize(contents):
```

### Comparing `capabilities-0.3.3/examples/cheese.py` & `capabilities-0.3.4/examples/cheese.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.3/examples/leansearch.py` & `capabilities-0.3.4/examples/leansearch.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.3/examples/tesla10k.py` & `capabilities-0.3.4/examples/tesla10k.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.3/examples/data/apple10k.pdf` & `capabilities-0.3.4/examples/data/apple10k.pdf`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.3/examples/data/sample.md` & `capabilities-0.3.4/examples/data/sample.md`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.3/examples/data/sample.pdf` & `capabilities-0.3.4/examples/data/sample.pdf`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.3/examples/data/tesla10k.txt` & `capabilities-0.3.4/examples/data/tesla10k.txt`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.3/tests/test_docs.py` & `capabilities-0.3.4/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.3/tests/test_document_loader.py` & `capabilities-0.3.4/tests/test_document_loader.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.3/tests/test_search.py` & `capabilities-0.3.4/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.3/tests/test_search_util.py` & `capabilities-0.3.4/tests/test_search_util.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.3/tests/test_tutorial1.py` & `capabilities-0.3.4/tests/test_tutorial1.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.3/tests/test_vector_idx.py` & `capabilities-0.3.4/tests/test_vector_idx.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.3/tests/snapshots/test_search/test_search_e2e/NomicIndex-openai/r0.txt` & `capabilities-0.3.4/tests/snapshots/test_search/test_search_e2e/NomicIndex-openai/r0.txt`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.3/tests/snapshots/test_search/test_search_e2e/NomicIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt` & `capabilities-0.3.4/tests/snapshots/test_search/test_search_e2e/NomicIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.3/tests/snapshots/test_search/test_search_e2e/SearchIndex-openai/r0.txt` & `capabilities-0.3.4/tests/snapshots/test_search/test_search_e2e/SearchIndex-openai/r0.txt`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.3/tests/snapshots/test_search/test_search_e2e/SearchIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt` & `capabilities-0.3.4/tests/snapshots/test_search/test_search_e2e/SearchIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.3/.gitignore` & `capabilities-0.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.3/LICENSE` & `capabilities-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.3/pyproject.toml` & `capabilities-0.3.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "capabilities"
-dynamic = ["version"]
+# dynamic = ["version"]
+version="0.3.4"
 authors = [
   { name="Blazon AI", email="support@blazon.ai" },
 ]
 description = "Build trusted, faster, and more powerful applications with the Blazon Capabilities API."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `capabilities-0.3.3/PKG-INFO` & `capabilities-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capabilities
-Version: 0.3.3
+Version: 0.3.4
 Summary: Build trusted, faster, and more powerful applications with the Blazon Capabilities API.
 Author-email: Blazon AI <support@blazon.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

