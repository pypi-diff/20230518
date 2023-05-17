# Comparing `tmp/langkit-0.0.1.dev1.tar.gz` & `tmp/langkit-0.0.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langkit-0.0.1.dev1.tar", max compression
+gzip compressed data, was "langkit-0.0.1.dev2.tar", max compression
```

## Comparing `langkit-0.0.1.dev1.tar` & `langkit-0.0.1.dev2.tar`

### file list

```diff
@@ -1,14 +1,22 @@
--rw-r--r--   0        0        0    11357 2023-04-27 19:37:47.238351 langkit-0.0.1.dev1/LICENSE
--rw-r--r--   0        0        0     2001 2023-05-10 18:06:28.152898 langkit-0.0.1.dev1/README.md
--rw-r--r--   0        0        0      244 2023-05-09 22:21:18.502898 langkit-0.0.1.dev1/langkit/__init__.py
--rw-r--r--   0        0        0   267008 2023-05-10 18:29:55.652898 langkit-0.0.1.dev1/langkit/examples/LLM_to_WhyLabs.ipynb
--rw-r--r--   0        0        0     1680 2023-05-10 18:06:28.152898 langkit-0.0.1.dev1/langkit/examples/Logging_Text.ipynb
--rw-r--r--   0        0        0        0 2023-05-08 16:31:57.882898 langkit-0.0.1.dev1/langkit/exclusions.py
--rw-r--r--   0        0        0     1097 2023-05-09 23:30:20.252898 langkit-0.0.1.dev1/langkit/input_output.py
--rw-r--r--   0        0        0     1051 2023-05-10 18:06:37.882898 langkit-0.0.1.dev1/langkit/pattern_groups.json
--rw-r--r--   0        0        0     2403 2023-05-10 18:06:37.882898 langkit-0.0.1.dev1/langkit/regexes.py
--rw-r--r--   0        0        0      488 2023-05-09 23:30:20.252898 langkit-0.0.1.dev1/langkit/sentiment.py
--rw-r--r--   0        0        0     2072 2023-05-10 18:06:37.882898 langkit-0.0.1.dev1/langkit/tests/test_patterns.py
--rw-r--r--   0        0        0     2404 2023-05-09 23:30:20.252898 langkit-0.0.1.dev1/langkit/textstat.py
--rw-r--r--   0        0        0      605 2023-05-10 18:19:07.442898 langkit-0.0.1.dev1/pyproject.toml
--rw-r--r--   0        0        0     2880 1970-01-01 00:00:00.000000 langkit-0.0.1.dev1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-27 19:37:47.238351 langkit-0.0.1.dev2/LICENSE
+-rw-r--r--   0        0        0     2256 2023-05-17 23:35:21.462537 langkit-0.0.1.dev2/README.md
+-rw-r--r--   0        0        0      718 2023-05-17 23:35:21.462537 langkit-0.0.1.dev2/langkit/__init__.py
+-rw-r--r--   0        0        0     9959 2023-05-17 23:35:21.462537 langkit-0.0.1.dev2/langkit/examples/Batch_to_Whylabs.ipynb
+-rw-r--r--   0        0        0   267155 2023-05-17 23:35:00.232537 langkit-0.0.1.dev2/langkit/examples/LLM_to_WhyLabs.ipynb
+-rw-r--r--   0        0        0     1719 2023-05-17 23:35:00.232537 langkit-0.0.1.dev2/langkit/examples/Logging_Text.ipynb
+-rw-r--r--   0        0        0     5878 2023-05-17 23:35:21.462537 langkit-0.0.1.dev2/langkit/examples/Sentiment_and_Toxicity.ipynb
+-rw-r--r--   0        0        0      927 2023-05-12 18:53:48.262898 langkit-0.0.1.dev2/langkit/input_output.py
+-rw-r--r--   0        0        0      912 2023-05-16 16:10:15.942898 langkit-0.0.1.dev2/langkit/pattern_groups.json
+-rw-r--r--   0        0        0     2509 2023-05-16 16:10:15.942898 langkit-0.0.1.dev2/langkit/regexes.py
+-rw-r--r--   0        0        0      488 2023-05-09 23:30:20.252898 langkit-0.0.1.dev2/langkit/sentiment.py
+-rw-r--r--   0        0        0      685 2023-05-12 18:53:48.262898 langkit-0.0.1.dev2/langkit/tests/conftest.py
+-rw-r--r--   0        0        0     2302 2023-05-17 23:35:00.232537 langkit-0.0.1.dev2/langkit/tests/test_patterns.py
+-rw-r--r--   0        0        0     2241 2023-05-12 18:53:48.262898 langkit-0.0.1.dev2/langkit/tests/test_themes.py
+-rw-r--r--   0        0        0     2404 2023-05-09 23:30:20.252898 langkit-0.0.1.dev2/langkit/textstat.py
+-rw-r--r--   0        0        0     9024 2023-05-17 23:35:21.462537 langkit-0.0.1.dev2/langkit/themes.json
+-rw-r--r--   0        0        0      261 2023-05-17 23:35:21.462537 langkit-0.0.1.dev2/langkit/themes.json.txt
+-rw-r--r--   0        0        0     2914 2023-05-16 16:10:15.952898 langkit-0.0.1.dev2/langkit/themes.py
+-rw-r--r--   0        0        0      705 2023-05-17 23:35:21.462537 langkit-0.0.1.dev2/langkit/toxicity.py
+-rw-r--r--   0        0        0      143 2023-05-12 18:53:48.272898 langkit-0.0.1.dev2/langkit/transformer.py
+-rw-r--r--   0        0        0      605 2023-05-17 23:35:55.572537 langkit-0.0.1.dev2/pyproject.toml
+-rw-r--r--   0        0        0     3135 1970-01-01 00:00:00.000000 langkit-0.0.1.dev2/PKG-INFO
```

### Comparing `langkit-0.0.1.dev1/LICENSE` & `langkit-0.0.1.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1.dev1/langkit/examples/LLM_to_WhyLabs.ipynb` & `langkit-0.0.1.dev2/langkit/examples/LLM_to_WhyLabs.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9910347155061251%*

 * *Differences: {"'cells'": "{1: {'attachments': OrderedDict()}, 2: {'source': ['[![Open in "*

 * *            "Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/whylabs/LanguageToolkit/blob/main/langkit/examples/LLM_to_WhyLabs.ipynb)'], "*

 * *            "'attachments': OrderedDict()}, 6: {'attachments': OrderedDict()}, 10: {'source': "*

 * *            "{insert: [(1, 'from typing import Optional\\n'), (7, '    def __init__(self, prompt: "*

 * *            "str, response: str, errors: […]*

```diff
@@ -6,25 +6,27 @@
             "metadata": {},
             "source": [
                 ">### \ud83d\udea9 *Create a free WhyLabs account to complete this example!*<br> \n",
                 ">*Did you know you can store, visualize, and monitor whylogs profiles with the [WhyLabs Observability Platform](https://whylabs.ai/whylabs-free-sign-up?utm_source=github&utm_medium=referral&utm_campaign=langkit)? Sign up for a [free WhyLabs account](https://whylabs.ai/whylogs-free-signup?utm_source=github&utm_medium=referral&utm_campaign=LLM_to_WhyLabs) to leverage the power of whylogs and WhyLabs together!*"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Writing Profiles to WhyLabs"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/whylabs/whylogs/blob/mainline/python/examples/integrations/writers/Writing_to_WhyLabs.ipynb)"
+                "[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/whylabs/LanguageToolkit/blob/main/langkit/examples/LLM_to_WhyLabs.ipynb)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -53,14 +55,15 @@
             "outputs": [],
             "source": [
                 "# Note: you may need to restart the kernel to use updated packages.\n",
                 "%pip install langkit"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## \u2714\ufe0f Setting the Environment Variables"
             ]
         },
         {
@@ -141,27 +144,30 @@
         {
             "cell_type": "code",
             "execution_count": 40,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import os\n",
+                "from typing import Optional\n",
                 "import openai\n",
                 "\n",
                 "openai.api_key = os.getenv(\"OPENAI_API_KEY\")\n",
                 "\n",
                 "class ChatLog:\n",
-                "    def __init__(self, prompt: str, response: str):\n",
+                "    def __init__(self, prompt: str, response: str, errors: Optional[str] = None):\n",
                 "        self.prompt = prompt\n",
                 "        self.response = response\n",
+                "        self.errors = errors\n",
                 "\n",
                 "    def to_dict(self):\n",
                 "        return {\n",
                 "            \"prompt\": self.prompt,\n",
                 "            \"response\": self.response,\n",
+                "            \"errors\" : self.errors\n",
                 "        }\n",
                 "\n",
                 "# this is just for demonstration purposes\n",
                 "def send_prompt(prompt: str) -> ChatLog:\n",
                 "    try:\n",
                 "        response = openai.ChatCompletion.create(\n",
                 "            model=\"gpt-3.5-turbo\",\n",
@@ -174,16 +180,15 @@
                 "            }],\n",
                 "            temperature=0.9,\n",
                 "            max_tokens=100,\n",
                 "            frequency_penalty=0,\n",
                 "            presence_penalty=0.6\n",
                 "        )\n",
                 "    except Exception as e:\n",
-                "        response = {}\n",
-                "        response.choices = [f\"{e}\"]\n",
+                "        return ChatLog(prompt, \"\", f\"{e}\")\n",
                 "\n",
                 "    result = ''\n",
                 "    for choice in response.choices:\n",
                 "        result += choice.message.content\n",
                 "\n",
                 "    return ChatLog(prompt, result)\n"
             ]
@@ -224,14 +229,15 @@
                 "\n",
                 "# Lets add the whylabs writer (it will write the aggregate statistics and metrics to WhyLabs)\n",
                 "# you can also use 'local' for local file store, or s3, and various other writers.\n",
                 "telemetry_agent.append_writer(\"whylabs\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## \ud83d\udcca Profiling the Data"
             ]
         },
         {
@@ -249,33 +255,35 @@
             "outputs": [],
             "source": [
                 "INTERACTIVE = False # set to True to test out interacting with ChatGPT\n",
                 "interactive_prompt = \"\"\n",
                 "if INTERACTIVE:\n",
                 "    print(f\"At any time input 'q' or anything that begins with q to quit. enter a question for the LLM\")\n",
                 "    while True:\n",
-                "        interactive_prompt = input(\"ask chat gpt\")\n",
+                "        print()\n",
+                "        interactive_prompt = input(\"ask chat gpt: \")\n",
                 "        if interactive_prompt.startswith('q'):\n",
                 "            break\n",
                 "        response = send_prompt(interactive_prompt)\n",
                 "        # use the agent to log a dictionary, these should be flat\n",
                 "        # to get the best results, in this case we log the prompt and response text\n",
                 "        telemetry_agent.log(response.to_dict())\n",
                 "        print(response.to_dict())\n",
                 "else:\n",
                 "    from datasets import load_dataset, Dataset\n",
                 "    import pandas as pd\n",
                 "\n",
-                "    archived_chats = load_dataset('alespalla/chatbot_instruction_prompts', split=\"test\")\n",
+                "    archived_chats = load_dataset('alespalla/chatbot_instruction_prompts', split=\"test\", streaming=True)\n",
+                "    chats = iter(archived_chats)\n",
+                "    for _ in range(100):\n",
+                "      response = next(chats)\n",
+                "      telemetry_agent.log(response)\n",
+                "      print(response)\n",
                 "    # lets output the dataset metadata from hugging face so we can see how to\n",
                 "    # access some of the contained prompts and responses.\n",
-                "    print(f\"Here's the dataset structure {archived_chats}\")\n",
-                "    for column_name in archived_chats.column_names:\n",
-                "        print(f\"Profiling column: ({column_name})\")\n",
-                "        telemetry_agent.log(pd.DataFrame(archived_chats[column_name][:1000], columns=[column_name]))\n",
                 "    print(\"done profiling\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 43,
             "metadata": {},
@@ -284,14 +292,15 @@
                 "# In practice you can use context manager lifecycle events to automatically close\n",
                 "# loggers, this helps trigger a write ahead of schedule to avoid truncating the last interval\n",
                 "# data seen by the agent.\n",
                 "telemetry_agent.close()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## \ud83d\udd0d A Look on the Other Side"
             ]
         },
         {
```

### Comparing `langkit-0.0.1.dev1/langkit/examples/Logging_Text.ipynb` & `langkit-0.0.1.dev2/langkit/examples/Logging_Text.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996527777777777%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(5, 'from langkit.regexes import *\\n')]}}}"}*

```diff
@@ -24,14 +24,15 @@
             "outputs": [],
             "source": [
                 "from whylogs.experimental.core.metrics.udf_metric import generate_udf_schema\n",
                 "from whylogs.core.schema import DeclarativeSchema\n",
                 "import whylogs as why\n",
                 "from langkit.sentiment import *\n",
                 "from langkit.textstat import *\n",
+                "from langkit.regexes import *\n",
                 "\n",
                 "text_schema = DeclarativeSchema(generate_udf_schema())\n",
                 "results = why.log({\"prompt\": \"hello!\", \"response\": \"world!\"}, schema=text_schema)"
             ]
         },
         {
             "cell_type": "code",
```

### Comparing `langkit-0.0.1.dev1/langkit/input_output.py` & `langkit-0.0.1.dev2/langkit/input_output.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 from typing import Optional, Tuple
 from sentence_transformers import SentenceTransformer, util
 from torch import Tensor
 from whylogs.experimental.core.metrics.udf_metric import (
     register_metric_udf,
 )
+from . import LangKitConfig
+from langkit.transformer import load_model
+
+lang_config = LangKitConfig()
+
 
 _transformer_model = None
 
 
 def init(transformer_name: Optional[str]):
     global _transformer_model
     if transformer_name is None:
-        transformer_name = 'sentence-transformers/all-MiniLM-L6-v2'
-    _transformer_model = SentenceTransformer(transformer_name)
+        transformer_name = lang_config.transformer_name
+    _transformer_model = load_model(transformer_name)
 
 
 init()
 
 
-def get_subject_similarity(text: str, comparison_embedding: Tensor) -> float:
-    embedding = _transformer_model.encode(text, convert_to_tensor=True)
-    similarity = util.pytorch_cos_sim(embedding, comparison_embedding)
-    return similarity.item()
-
-
 @register_metric_udf(col_name="combined")
 def similarity_MiniLM_L6_v2(combined: Tuple[str, str]) -> float:
     x, y = combined
     embedding_1 = _transformer_model.encode(x, convert_to_tensor=True)
     embedding_2 = _transformer_model.encode(y, convert_to_tensor=True)
     similarity = util.pytorch_cos_sim(embedding_1, embedding_2)
     return similarity.item()
```

### Comparing `langkit-0.0.1.dev1/langkit/pattern_groups.json` & `langkit-0.0.1.dev2/langkit/pattern_groups.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.85%*

 * *Differences: {'1': "{'expressions': ['\\\\b(?:\\\\d[ -]*?){13,16}\\\\b']}",*

 * * '2': "{'expressions': ['(?!(\\\\d){3}(-| "*

 * *      '|)\\\\1{2}\\\\2\\\\1{4})(?!666|000|9\\\\d{2})(\\\\b\\\\d{3}(-| '*

 * *      "|)(?!00)\\\\d{2}\\\\4(?!0{4})\\\\d{4}\\\\b)']}",*

 * * '4': "{'expressions': "*

 * *      "['\\\\d+(\\\\s+(N|S|E|W|NE|NW|SE|SW)\\\\.?)?\\\\s+[0-9]{0,5}[a-zA-Z]+\\\\s+(?:Street|St|Road|Rd|Avenue|Ave|Boulevard|Blvd|Drive|Dr|Court|Ct|Lane|Ln|Square|Sq)']}"}*

```diff
@@ -3,30 +3,30 @@
         "expressions": [
             "[A-Za-z0-9._+\\-\\']+@[A-Za-z0-9.\\-]+\\.[A-Za-z]{2,}"
         ],
         "name": "email address"
     },
     {
         "expressions": [
-            "\\b(?:4[0-9]{12}(?:[0-9]{3})?|[25][1-7][0-9]{14}|6(?:011|5[0-9][0-9])[0-9]{12}|3[47][0-9]{13}|3(?:0[0-5]|[68][0-9])[0-9]{11}|(?:2131|1800|35\\d{3})\\d{11})\\b"
+            "\\b(?:\\d[ -]*?){13,16}\\b"
         ],
         "name": "credit card number"
     },
     {
         "expressions": [
-            "\\b(?!000|.+0{4})(?:\\d{9}|\\d{3}-\\d{2}-\\d{4})\\b"
+            "(?!(\\d){3}(-| |)\\1{2}\\2\\1{4})(?!666|000|9\\d{2})(\\b\\d{3}(-| |)(?!00)\\d{2}\\4(?!0{4})\\d{4}\\b)"
         ],
         "name": "SSN"
     },
     {
         "expressions": [
             "((\\+\\d{1,2}\\s)?\\(?\\d{3}\\)?[\\s.-]\\d{3}[\\s.-]\\d{4}|[0-9]{10}|\\+{1}[0-9 ]{11,15}|[0-9]{4} [0-9]{6})"
         ],
         "name": "phone number"
     },
     {
         "expressions": [
-            "\\b\\d{1,8}\\b[\\s\\S]{10,100}?\\b(AK|AL|AR|AZ|CA|CO|CT|DC|DE|FL|GA|HI|IA|ID|IL|IN|KS|KY|LA|MA|MD|ME|MI|MN|MO|MS|MT|NC|ND|NE|NH|NJ|NM|NV|NY|OH|OK|OR|PA|RI|SC|SD|TN|TX|UT|VA|VT|WA|WI|WV|WY)\\b\\s\\d{5}\\b"
+            "\\d+(\\s+(N|S|E|W|NE|NW|SE|SW)\\.?)?\\s+[0-9]{0,5}[a-zA-Z]+\\s+(?:Street|St|Road|Rd|Avenue|Ave|Boulevard|Blvd|Drive|Dr|Court|Ct|Lane|Ln|Square|Sq)"
         ],
         "name": "mailing address"
     }
 ]
```

### Comparing `langkit-0.0.1.dev1/langkit/regexes.py` & `langkit-0.0.1.dev2/langkit/regexes.py`

 * *Files 10% similar despite different names*

```diff
@@ -66,11 +66,12 @@
             for group in regex_groups:
                 for expression in group["expressions"]:
                     if expression.search(text):
                         patterns_info = group["name"]
                         return group["name"]
         return patterns_info
 
-
-def set_config(config: LangKitConfig):
-    pattern_loader.set_config(config)
-    pattern_loader.update_patterns()
+def init(pattern_file_path: Optional[str]=None):
+    if pattern_file_path:
+        lang_config.pattern_file_path = pattern_file_path
+        pattern_loader.set_config(lang_config)
+        pattern_loader.update_patterns()
```

### Comparing `langkit-0.0.1.dev1/langkit/tests/test_patterns.py` & `langkit-0.0.1.dev2/langkit/tests/test_patterns.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 import pandas as pd
 import whylogs as why
-from whylogs.core.resolvers import STANDARD_RESOLVER
 from whylogs.core.schema import DeclarativeSchema
 from whylogs.experimental.core.metrics.udf_metric import generate_udf_schema
-from langkit import regexes, LangKitConfig
+from langkit import LangKitConfig
 import pytest
 import tempfile
 import os
 
 
 @pytest.fixture
 def ptt_df():
     df = pd.DataFrame(
         {
             "input": [
-                "address: 123 Main St Anytown, NY 12345",
+                "address: 123 Main St.",
+                "2255 140th Ave. NE",
+                "535 Bellevue Sq",
+                "15220 SE 37th St, its a nice place",
                 "anemail@address.com",
                 "my phone is +1 309-404-7587",
                 "credit card 4556205848969759",
+                "credit card 3851-6256-0926-7271",
+                "Visa Card Number: 4929 5423 7528 1067 \nExpiration Date: 03/24 \nCVV: 348",
+                "622202049892743 - this is a credit card number",
                 "my ssn is 856-45-6789",
-            ],
-            "output": ["a", "b", "c", "d", "e"],
-        }
+                "ssn - 702-02-9921",
+                "ssn is 702 02 9921",
+                "702029921 (SSN)",
+                "no patterns here.",
+                ]
+            }
     )
     return df
 
 
 user_json = """
 [
     {
@@ -36,32 +44,34 @@
     }
 ]
 """
 
 # log dataframe
 @pytest.mark.parametrize("user_defined_json", [False, True])
 def test_ptt(ptt_df, user_defined_json):
+    from langkit import regexes
     if user_defined_json:
         with tempfile.TemporaryDirectory() as temp_dir:
             json_filename = "user.json"
             json_path = os.path.join(temp_dir, json_filename)
             with open(json_path, "w") as file:
                 file.write(user_json)
-            regexes.set_config(
-                LangKitConfig(pattern_file_path=os.path.join(temp_dir, json_filename))
-            )
+            regexes.init(pattern_file_path=os.path.join(temp_dir, json_filename))
 
-    schema = DeclarativeSchema(STANDARD_RESOLVER + generate_udf_schema())
+    schema = DeclarativeSchema(generate_udf_schema())
     result = why.log(ptt_df, schema=schema)
     fi_input_list = result.view().to_pandas()[
         "udf/has_patterns:frequent_items/frequent_strings"
     ]["input"]
-    fi_output_list = result.view().to_pandas()[
-        "udf/has_patterns:frequent_items/frequent_strings"
-    ]["output"]
     if not user_defined_json:
-        group_names = {"phone number", "email address", "SSN", "mailing address", "credit card number"}
+        group_names = {
+            "",
+            "credit card number",
+            "email address",
+            "SSN",
+            "phone number",
+            "mailing address",
+        }
     else:
         group_names = {"custom_group", ""}
 
     assert set([x.value for x in fi_input_list]) == group_names
-    assert set([x.value for x in fi_output_list]) == {""}
```

### Comparing `langkit-0.0.1.dev1/langkit/textstat.py` & `langkit-0.0.1.dev2/langkit/textstat.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1.dev1/pyproject.toml` & `langkit-0.0.1.dev2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "langkit"
-version = "0.0.1.dev1"
+version = "0.0.1.dev2"
 description = "A collection of text metric udfs for whylogs profiling and monitoring in WhyLabs"
-authors = ["WhyLabs.ai <support@whylabs.ai>"]
+authors = ["WhyLabs.ai <langkit@whylabs.ai>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 whylogs = {version = "^1.1.40"}
```

### Comparing `langkit-0.0.1.dev1/PKG-INFO` & `langkit-0.0.1.dev2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: langkit
-Version: 0.0.1.dev1
+Version: 0.0.1.dev2
 Summary: A collection of text metric udfs for whylogs profiling and monitoring in WhyLabs
 License: Apache-2.0
 Author: WhyLabs.ai
-Author-email: support@whylabs.ai
+Author-email: langkit@whylabs.ai
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -29,19 +29,20 @@
 ## Motivation
 
 Productionizing language models, including LLMs, comes with a range of risks due to the infinite amount of input combinations, which can elicit an infinite amount of outputs. The unstructured nature of text poses a challenge in the ML observability space - a challenge worth solving, since the lack of visibility on the model's behavior can have serious consequences.
 
 ## Features
 
 The currently supported metrics include:
-- readability
-- complexity
-- grade
-- sentiment
-- similarity to a user-defined topic
+- readability score
+- complexity and grade scores
+- sentiment analysis
+- patterns - count of strings matching a user-defined regex pattern group
+- jailbreaks - similarity scores with respect to known jailbreak attempts and prompt injection attacks
+- refusals - similarity scores with respect to known LLM refusal of service responses
 
 ## Installation
 
 To install LangKit, use the Python Package Index (PyPI) as follows:
 ```bash
 pip install langkit
 ```
@@ -59,9 +60,9 @@
 
 text_schema = DeclarativeSchema(generate_udf_schema())
 results = why.log({"prompt": "hello!", "response": "world!"}, schema=text_schema)
 
 ```
 The code above will produce a set of metrics comprised of the default whylogs metrics for text features and all the metrics defined in the imported modules.
 
-More examples available [here](https://github.com/whylabs/LanguageToolkit/tree/main/langkit/examples)
+More examples are available [here](https://github.com/whylabs/LanguageToolkit/tree/main/langkit/examples).
```

