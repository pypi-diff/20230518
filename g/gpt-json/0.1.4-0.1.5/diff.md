# Comparing `tmp/gpt_json-0.1.4.tar.gz` & `tmp/gpt_json-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_json-0.1.4.tar", max compression
+gzip compressed data, was "gpt_json-0.1.5.tar", max compression
```

## Comparing `gpt_json-0.1.4.tar` & `gpt_json-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1071 2023-05-04 20:40:27.560806 gpt_json-0.1.4/LICENSE
--rw-r--r--   0        0        0     8446 2023-05-04 20:40:27.560806 gpt_json-0.1.4/README.md
--rw-r--r--   0        0        0       63 2023-05-04 20:40:27.560806 gpt_json-0.1.4/gpt_json/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 20:40:27.560806 gpt_json-0.1.4/gpt_json/enums.py
--rw-r--r--   0        0        0      145 2023-05-04 20:40:27.560806 gpt_json-0.1.4/gpt_json/exceptions.py
--rw-r--r--   0        0        0    11578 2023-05-04 20:40:27.560806 gpt_json-0.1.4/gpt_json/gpt.py
--rw-r--r--   0        0        0      641 2023-05-04 20:40:27.560806 gpt_json-0.1.4/gpt_json/models.py
--rw-r--r--   0        0        0     1483 2023-05-04 20:40:27.560806 gpt_json-0.1.4/gpt_json/parsers.py
--rw-r--r--   0        0        0     1860 2023-05-04 20:40:27.560806 gpt_json-0.1.4/gpt_json/prompts.py
--rw-r--r--   0        0        0        0 2023-05-04 20:40:27.560806 gpt_json-0.1.4/gpt_json/tests/__init__.py
--rw-r--r--   0        0        0      256 2023-05-04 20:40:27.560806 gpt_json-0.1.4/gpt_json/tests/shared.py
--rw-r--r--   0        0        0     7167 2023-05-04 20:40:27.560806 gpt_json-0.1.4/gpt_json/tests/test_gpt.py
--rw-r--r--   0        0        0     1037 2023-05-04 20:40:27.560806 gpt_json-0.1.4/gpt_json/tests/test_parsers.py
--rw-r--r--   0        0        0     1189 2023-05-04 20:40:27.560806 gpt_json-0.1.4/gpt_json/tests/test_prompts.py
--rw-r--r--   0        0        0     3455 2023-05-04 20:40:27.560806 gpt_json-0.1.4/gpt_json/tests/test_transformations.py
--rw-r--r--   0        0        0     2808 2023-05-04 20:40:27.560806 gpt_json-0.1.4/gpt_json/transformations.py
--rw-r--r--   0        0        0      534 2023-05-04 20:40:27.560806 gpt_json-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     8998 1970-01-01 00:00:00.000000 gpt_json-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-18 20:33:26.661816 gpt_json-0.1.5/LICENSE
+-rw-r--r--   0        0        0     8612 2023-05-18 20:33:26.661816 gpt_json-0.1.5/README.md
+-rw-r--r--   0        0        0       63 2023-05-18 20:33:26.661816 gpt_json-0.1.5/gpt_json/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 20:33:26.661816 gpt_json-0.1.5/gpt_json/enums.py
+-rw-r--r--   0        0        0      145 2023-05-18 20:33:26.661816 gpt_json-0.1.5/gpt_json/exceptions.py
+-rw-r--r--   0        0        0    11841 2023-05-18 20:33:26.661816 gpt_json-0.1.5/gpt_json/gpt.py
+-rw-r--r--   0        0        0      656 2023-05-18 20:33:26.661816 gpt_json-0.1.5/gpt_json/models.py
+-rw-r--r--   0        0        0     1483 2023-05-18 20:33:26.661816 gpt_json-0.1.5/gpt_json/parsers.py
+-rw-r--r--   0        0        0     1860 2023-05-18 20:33:26.661816 gpt_json-0.1.5/gpt_json/prompts.py
+-rw-r--r--   0        0        0        0 2023-05-18 20:33:26.661816 gpt_json-0.1.5/gpt_json/tests/__init__.py
+-rw-r--r--   0        0        0      256 2023-05-18 20:33:26.661816 gpt_json-0.1.5/gpt_json/tests/shared.py
+-rw-r--r--   0        0        0     8767 2023-05-18 20:33:26.661816 gpt_json-0.1.5/gpt_json/tests/test_gpt.py
+-rw-r--r--   0        0        0      656 2023-05-18 20:33:26.661816 gpt_json-0.1.5/gpt_json/tests/test_models.py
+-rw-r--r--   0        0        0     1037 2023-05-18 20:33:26.661816 gpt_json-0.1.5/gpt_json/tests/test_parsers.py
+-rw-r--r--   0        0        0     1189 2023-05-18 20:33:26.661816 gpt_json-0.1.5/gpt_json/tests/test_prompts.py
+-rw-r--r--   0        0        0     3455 2023-05-18 20:33:26.661816 gpt_json-0.1.5/gpt_json/tests/test_transformations.py
+-rw-r--r--   0        0        0     2808 2023-05-18 20:33:26.661816 gpt_json-0.1.5/gpt_json/transformations.py
+-rw-r--r--   0        0        0      534 2023-05-18 20:33:26.661816 gpt_json-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     9164 1970-01-01 00:00:00.000000 gpt_json-0.1.5/PKG-INFO
```

### Comparing `gpt_json-0.1.4/LICENSE` & `gpt_json-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.4/README.md` & `gpt_json-0.1.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Specifically this library:
 - Utilizes Pydantic schema definitions for type casting and validations
 - Adds typehinting for both the API and the output schema
 - Allows GPT to respond with both single-objects and lists of objects
 - Includes some lightweight transformations of the output to remove superfluous context and fix broken json
 - Includes retry logic for the most common API failures
 - Formats the JSON schema as a flexible prompt that can be added into any message
-- Supports tempating of prompts to allow for dynamic content
+- Supports templating of prompts to allow for dynamic content
 
 ## Getting Started
 
 ```bash
 pip install gpt-json
 ```
 
@@ -148,17 +148,29 @@
 ## Transformations
 
 GPT (especially GPT-4) is relatively good at formatting responses at JSON, but it's not perfect. Some of the more common issues are:
 
 - *Response truncation*: Since GPT is not internally aware of its response length limit, JSON payloads will sometimes exhaust the available token space. This results in a broken JSON payload where much of the data is valid but the JSON object is not closed, which is not valid syntax. There are many cases where this behavior is actually okay for production applications - for instance, if you list 100 generated strings, it's sometimes okay for you to take the 70 that actually rendered. In this case, `gpt-json` will attempt to fix the truncated payload by recreating the JSON object and closing it.
 - *Boolean variables*: GPT will sometimes confuse valid JSON boolean values with the boolean tokens that are used in other languages. The most common is generating `True` instead of `true`. `gpt-json` will attempt to fix these values.
 
-When calling `gpt_json.run()`, we return a tuple of values. The first object is your generated Pydantic model. The second object is our correction storage object `FixTransforms`. This dataclass contains flags for each of the supported transformation cases that are sketched out above. This allows you to determine whether the response was explicitly parsed from the GPT JSON, or was passed through some middlelayers to get a correct output. From there you can accept or reject the response based on your own business logic.
+When calling `gpt_json.run()`, we return a tuple of values:
 
-*Where you can help*: There are certainly more areas of common (and not-so-common failures). If you see these, please add a test case to the README. If you can write a handler to help solve the general case, please do so. Otherwise flag it as a `pytest.xfail` and we'll add it to the backlog.
+```python
+response, transformations = await gpt_json.run(...)
+
+print(transformations)
+```
+
+```bash
+FixTransforms(fixed_truncation=True, fixed_bools=False)
+```
+
+The first object is your generated Pydantic model. The second object is our correction storage object `FixTransforms`. This dataclass contains flags for each of the supported transformation cases that are sketched out above. This allows you to determine whether the response was explicitly parsed from the GPT JSON, or was passed through some middlelayers to get a correct output. From there you can accept or reject the response based on your own business logic.
+
+*Where you can help*: There are certainly more areas of common (and not-so-common failures). If you see these, please add a test case to the unit tests. If you can write a handler to help solve the general case, please do so. Otherwise flag it as a `pytest.xfail` and we'll add it to the backlog.
 
 ## Testing
 
 We use poetry for package management. To run the bundled tests, clone the package from github.
 
 ```bash
 poetry install
```

### Comparing `gpt_json-0.1.4/gpt_json/gpt.py` & `gpt_json-0.1.5/gpt_json/gpt.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,25 @@
+import logging
 from dataclasses import replace
 from json import loads as json_loads
 from json.decoder import JSONDecodeError
-from typing import Generic, List, Type, TypeVar, get_origin, get_args
+from typing import Any, Generic, List, Type, TypeVar, get_args, get_origin
 
 import backoff
 import openai
 from openai.error import APIConnectionError, RateLimitError
 from openai.error import Timeout as OpenAITimeout
 from pydantic import BaseModel
 from tiktoken import encoding_for_model
-from typing import Any
 
-from gpt_json.models import GPTMessage, GPTModelVersion, ResponseType, FixTransforms
+from gpt_json.models import (FixTransforms, GPTMessage, GPTModelVersion,
+                             ResponseType)
 from gpt_json.parsers import find_json_response
-from gpt_json.transformations import fix_truncated_json, fix_bools
 from gpt_json.prompts import generate_schema_prompt
-
-import logging
+from gpt_json.transformations import fix_bools, fix_truncated_json
 
 logger = logging.getLogger('my_logger')
 handler = logging.StreamHandler()
 formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
 handler.setFormatter(formatter)
 logger.addHandler(handler)
 
@@ -37,30 +36,31 @@
 SCHEMA_PROMPT_TEMPLATE_KEY = "json_schema"
 
 class GPTJSON(Generic[SchemaType]):
     """
     A wrapper over GPT that provides basic JSON parsing and response handling.
 
     """
+    _cls_schema_model: Type[SchemaType] = None
     schema_model: Type[SchemaType] = None
 
     def __init__(
         self,
-        api_key: str,
+        api_key: str | None = None,
         model: GPTModelVersion | str = GPTModelVersion.GPT_4,
         auto_trim: bool = False,
         auto_trim_response_overhead: int = 0,
         # For messages that are relatively deterministic
         temperature = 0.2,
         timeout = 60,
         openai_max_retries=3,
         **kwargs,
     ):
         """
-        :param api_key: OpenAI API key
+        :param api_key: OpenAI API key, if `OPENAI_API_KEY` environment variable is not set
         :param model: GPTModelVersion or string model name
         :param auto_trim: If True, automatically trim messages to fit within the model's token limit
         :param auto_trim_response_overhead: If auto_trim is True, will leave at least `auto_trim_response_overhead` space
             for the output payload. For GPT, initial prompt + response <= allowed tokens.
         :param temperature: Temperature (or variation) of response payload; 0 is the most deterministic, 1 is the most random
         :param timeout: Timeout in seconds for each OpenAI API calls
         :param openai_max_retries: Amount of times to retry failed API calls, caused by often transient load or rate limit issues
@@ -69,14 +69,16 @@
         """
         self.model = model.value if isinstance(model, GPTModelVersion) else model
         self.auto_trim = auto_trim
         self.temperature = temperature
         self.timeout = timeout
         self.openai_max_retries = openai_max_retries
         self.openai_arguments = kwargs
+        self.schema_model = self._cls_schema_model
+        GPTJSON._cls_schema_model = None
 
         if not self.schema_model:
             raise ValueError("GPTJSON needs to be instantiated with a schema model, like GPTJSON[MySchema](...args).")
 
         if get_origin(self.schema_model) in {list, List}:
             self.extract_type = ResponseType.LIST
         elif issubclass(self.schema_model, BaseModel):
@@ -96,15 +98,15 @@
         self.api_key = api_key
 
     async def run(
         self,
         messages: list[GPTMessage],
         max_response_tokens: int | None = None,
         format_variables: dict[str, Any] | None = None,
-    ) -> tuple[SchemaType | None, FixTransforms]:
+    ) -> tuple[SchemaType, FixTransforms] | tuple[None, None]:
         """
         :param messages: List of GPTMessage objects to send to the API
         :param max_response_tokens: Maximum number of tokens allowed in the response
         :param format_variables: Variables to format into the message template. Uses standard
             Python string formatting, like "Hello {name}".format(name="World")
 
         :return: Tuple of (parsed response, fix transforms). The transformations here is a object that
@@ -131,15 +133,15 @@
         logger.debug("------- RAW RESPONSE ----------")
         logger.debug(response["choices"])
         logger.debug("------- END RAW RESPONSE ----------")
         extracted_json, fixed_payload = self.extract_json(response, self.extract_type)
 
         # Cast to schema model
         if extracted_json is None:
-            return None
+            return None, None
 
         # Allow pydantic to handle the validation
         if isinstance(extracted_json, list):
             model = get_args(self.schema_model)[0]
             return [model(**item) for item in extracted_json], fixed_payload
         else:
             return self.schema_model(**extracted_json), fixed_payload
@@ -149,38 +151,38 @@
         Assumes one main block of results, either list of dictionary
 
         """
         choices = completion_response["choices"]
 
         if not choices:
             logger.warning("No choices available, should report error...")
-            return None
+            return None, None
 
         full_response = choices[0]["message"]["content"]
 
         extracted_response = find_json_response(full_response, extract_type)
         if extracted_response is None:
-            return None
+            return None, None
 
         # Save the original response before we start modifying it
         fixed_response = extracted_response
         fixed_response, fixed_truncation = fix_truncated_json(fixed_response)
         fixed_response, fixed_bools = fix_bools(fixed_response)
 
         fixed_payload = FixTransforms(
             fixed_bools=fixed_bools,
             fixed_truncation=fixed_truncation,
         )
 
         try:
             return json_loads(fixed_response), fixed_payload
         except JSONDecodeError as e:
-            logger.debug("Extracted", extracted_response)
-            logger.debug("Did parse", fixed_response)
-            logger.error("JSON decode error, likely malformed json input", e)
+            logger.debug(f"Extracted: {extracted_response}")
+            logger.debug(f"Did parse: {fixed_response}")
+            logger.error(f"JSON decode error, likely malformed json input: {e}")
             return None, fixed_payload
 
     async def submit_request(
         self,
         messages: list[GPTMessage],
         max_response_tokens: int | None,
     ):
@@ -292,9 +294,9 @@
         else:
             logger.debug(f"Skipping trim ({original_token_count}) ({current_token_count})")
 
         return new_messages
 
     def __class_getitem__(cls, item):
         new_cls = super().__class_getitem__(item)
-        new_cls.schema_model = item
+        new_cls._cls_schema_model = item
         return new_cls
```

### Comparing `gpt_json-0.1.4/gpt_json/models.py` & `gpt_json-0.1.5/gpt_json/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from dataclasses import dataclass
 from enum import Enum, unique
 
 
 @unique
-class ResponseType(Enum):
+class ResponseType(str, Enum):
     DICTIONARY = "DICTIONARY"
     LIST = "LIST"
 
 
 @unique
-class GPTMessageRole(Enum):
+class GPTMessageRole(str, Enum):
     SYSTEM = "system"
     USER = "user"
     ASSISTANT = "assistant"
 
 
 @unique
-class GPTModelVersion(Enum):
+class GPTModelVersion(str, Enum):
     GPT_3_5 = "gpt-3.5-turbo"
     GPT_4 = "gpt-4-0314"
 
 
 @dataclass
 class FixTransforms:
     """
```

### Comparing `gpt_json-0.1.4/gpt_json/parsers.py` & `gpt_json-0.1.5/gpt_json/parsers.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.4/gpt_json/prompts.py` & `gpt_json-0.1.5/gpt_json/prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.4/gpt_json/tests/test_gpt.py` & `gpt_json-0.1.5/gpt_json/tests/test_gpt.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from unittest.mock import MagicMock, patch
 
 import openai
 import pytest
+from pydantic import BaseModel, Field
 
 from gpt_json.gpt import GPTJSON
-from gpt_json.models import GPTMessage, GPTMessageRole, FixTransforms, GPTModelVersion
+from gpt_json.models import (FixTransforms, GPTMessage, GPTMessageRole,
+                             GPTModelVersion)
 from gpt_json.tests.shared import MySchema, MySubSchema
-from pydantic import BaseModel, Field
 
 
 def test_throws_error_if_no_model_specified():
     with pytest.raises(ValueError, match="needs to be instantiated with a schema model"):
         GPTJSON(None)
 
 
@@ -146,19 +147,17 @@
                 "index": 0,
                 "finish_reason": "stop",
             }
         ]
     }
 
     # Create the mock
-    with patch.object(openai.ChatCompletion, "acreate", return_value=mock_response) as mock_acreate:
+    with patch.object(openai.ChatCompletion, "acreate") as mock_acreate:
         # Make the mock function asynchronous
-        mock_acreate.__aenter__.return_value = MagicMock()
-        mock_acreate.__aexit__.return_value = MagicMock()
-        mock_acreate.__aenter__.return_value.__aenter__ = MagicMock(return_value=mock_response)
+        mock_acreate.return_value = mock_response
 
         # Call the function and pass the expected parameters
         response, transformations = await model.run(messages=messages)
 
         # Assert that the mock function was called with the expected parameters
         mock_acreate.assert_called_with(
             model=model_version.value,
@@ -212,14 +211,32 @@
 
     assert len(output_messages) == len(expected_output_messages)
 
     for output_message, expected_output_message in zip(output_messages, expected_output_messages):
         assert output_message.role == expected_output_message.role
         assert output_message.content == expected_output_message.content
 
+def test_two_gptjsons():
+    class TestSchema1(BaseModel):
+        field1: str
+    class TestSchema2(BaseModel):
+        field2: str
+    
+    gptjson1 = GPTJSON[TestSchema1](None)
+
+    # shouldn't allow instantion without a schema
+    with pytest.raises(ValueError):
+        gptjson2 = GPTJSON(None)
+    
+    gptjson2 = GPTJSON[TestSchema2](None)
+
+    assert gptjson1.schema_model == TestSchema1
+    assert gptjson2.schema_model == TestSchema2
+
+
 
 def test_fill_message_template():
     class TestTemplateSchema(BaseModel):
         template_field: str = Field(description="Max length {max_length}")
 
     gpt = GPTJSON[TestTemplateSchema](None)
     assert gpt.fill_message_template(
@@ -230,7 +247,38 @@
         dict(
             max_length=100,
         )
     ) == GPTMessage(
         role=GPTMessageRole.USER,
         content="Variable: 100\nMy schema is here: {\n\"template_field\": str // Max length 100\n}"
     )
+
+@pytest.mark.asyncio
+async def test_extracted_json_is_None():
+    gpt = GPTJSON[MySchema](None)
+
+    with patch.object(gpt, 'submit_request', return_value={'choices': [{'message': {'content': 'some content'}}]}), \
+         patch.object(gpt, 'extract_json', return_value=(None, FixTransforms(False, False))):
+        result, _ = await gpt.run([GPTMessage('system', 'message content')])
+        assert result is None
+
+@pytest.mark.asyncio
+async def test_no_valid_results_from_remote_request():
+    gpt = GPTJSON[MySchema](None)
+
+    with patch.object(gpt, 'submit_request', return_value={'choices': []}):
+        result, _ = await gpt.run([GPTMessage('system', 'message content')])
+        assert result is None
+
+@pytest.mark.asyncio
+async def test_unable_to_find_valid_json_payload():
+    gpt = GPTJSON[MySchema](None)
+
+    with patch.object(gpt, 'submit_request', return_value={'choices': [{'message': {'content': 'some content'}}]}), \
+         patch.object(gpt, 'extract_json', return_value=(None, FixTransforms(False, False))):
+        result, _ = await gpt.run([GPTMessage('system', 'message content')])
+        assert result is None
+
+@pytest.mark.asyncio
+async def test_unknown_model_to_infer_max_tokens():
+    with pytest.raises(ValueError):
+        GPTJSON[MySchema](model="UnknownModel", auto_trim=True)
```

### Comparing `gpt_json-0.1.4/gpt_json/tests/test_parsers.py` & `gpt_json-0.1.5/gpt_json/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.4/gpt_json/tests/test_prompts.py` & `gpt_json-0.1.5/gpt_json/tests/test_prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.4/gpt_json/tests/test_transformations.py` & `gpt_json-0.1.5/gpt_json/tests/test_transformations.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.4/gpt_json/transformations.py` & `gpt_json-0.1.5/gpt_json/transformations.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.4/pyproject.toml` & `gpt_json-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gpt-json"
-version = "0.1.4"
+version = "0.1.5"
 description = "Structured and typehinted GPT responses in Python."
 authors = ["Pierce Freeman <pierce@freeman.vc>"]
 readme = "README.md"
 packages = [{include = "gpt_json"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `gpt_json-0.1.4/PKG-INFO` & `gpt_json-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-json
-Version: 0.1.4
+Version: 0.1.5
 Summary: Structured and typehinted GPT responses in Python.
 Author: Pierce Freeman
 Author-email: pierce@freeman.vc
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -21,15 +21,15 @@
 Specifically this library:
 - Utilizes Pydantic schema definitions for type casting and validations
 - Adds typehinting for both the API and the output schema
 - Allows GPT to respond with both single-objects and lists of objects
 - Includes some lightweight transformations of the output to remove superfluous context and fix broken json
 - Includes retry logic for the most common API failures
 - Formats the JSON schema as a flexible prompt that can be added into any message
-- Supports tempating of prompts to allow for dynamic content
+- Supports templating of prompts to allow for dynamic content
 
 ## Getting Started
 
 ```bash
 pip install gpt-json
 ```
 
@@ -164,17 +164,29 @@
 ## Transformations
 
 GPT (especially GPT-4) is relatively good at formatting responses at JSON, but it's not perfect. Some of the more common issues are:
 
 - *Response truncation*: Since GPT is not internally aware of its response length limit, JSON payloads will sometimes exhaust the available token space. This results in a broken JSON payload where much of the data is valid but the JSON object is not closed, which is not valid syntax. There are many cases where this behavior is actually okay for production applications - for instance, if you list 100 generated strings, it's sometimes okay for you to take the 70 that actually rendered. In this case, `gpt-json` will attempt to fix the truncated payload by recreating the JSON object and closing it.
 - *Boolean variables*: GPT will sometimes confuse valid JSON boolean values with the boolean tokens that are used in other languages. The most common is generating `True` instead of `true`. `gpt-json` will attempt to fix these values.
 
-When calling `gpt_json.run()`, we return a tuple of values. The first object is your generated Pydantic model. The second object is our correction storage object `FixTransforms`. This dataclass contains flags for each of the supported transformation cases that are sketched out above. This allows you to determine whether the response was explicitly parsed from the GPT JSON, or was passed through some middlelayers to get a correct output. From there you can accept or reject the response based on your own business logic.
+When calling `gpt_json.run()`, we return a tuple of values:
 
-*Where you can help*: There are certainly more areas of common (and not-so-common failures). If you see these, please add a test case to the README. If you can write a handler to help solve the general case, please do so. Otherwise flag it as a `pytest.xfail` and we'll add it to the backlog.
+```python
+response, transformations = await gpt_json.run(...)
+
+print(transformations)
+```
+
+```bash
+FixTransforms(fixed_truncation=True, fixed_bools=False)
+```
+
+The first object is your generated Pydantic model. The second object is our correction storage object `FixTransforms`. This dataclass contains flags for each of the supported transformation cases that are sketched out above. This allows you to determine whether the response was explicitly parsed from the GPT JSON, or was passed through some middlelayers to get a correct output. From there you can accept or reject the response based on your own business logic.
+
+*Where you can help*: There are certainly more areas of common (and not-so-common failures). If you see these, please add a test case to the unit tests. If you can write a handler to help solve the general case, please do so. Otherwise flag it as a `pytest.xfail` and we'll add it to the backlog.
 
 ## Testing
 
 We use poetry for package management. To run the bundled tests, clone the package from github.
 
 ```bash
 poetry install
```

