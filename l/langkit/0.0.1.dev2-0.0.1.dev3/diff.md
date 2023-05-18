# Comparing `tmp/langkit-0.0.1.dev2.tar.gz` & `tmp/langkit-0.0.1.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langkit-0.0.1.dev2.tar", max compression
+gzip compressed data, was "langkit-0.0.1.dev3.tar", max compression
```

## Comparing `langkit-0.0.1.dev2.tar` & `langkit-0.0.1.dev3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    11357 2023-04-27 19:37:47.238351 langkit-0.0.1.dev2/LICENSE
--rw-r--r--   0        0        0     2256 2023-05-17 23:35:21.462537 langkit-0.0.1.dev2/README.md
--rw-r--r--   0        0        0      718 2023-05-17 23:35:21.462537 langkit-0.0.1.dev2/langkit/__init__.py
--rw-r--r--   0        0        0     9959 2023-05-17 23:35:21.462537 langkit-0.0.1.dev2/langkit/examples/Batch_to_Whylabs.ipynb
--rw-r--r--   0        0        0   267155 2023-05-17 23:35:00.232537 langkit-0.0.1.dev2/langkit/examples/LLM_to_WhyLabs.ipynb
--rw-r--r--   0        0        0     1719 2023-05-17 23:35:00.232537 langkit-0.0.1.dev2/langkit/examples/Logging_Text.ipynb
--rw-r--r--   0        0        0     5878 2023-05-17 23:35:21.462537 langkit-0.0.1.dev2/langkit/examples/Sentiment_and_Toxicity.ipynb
--rw-r--r--   0        0        0      927 2023-05-12 18:53:48.262898 langkit-0.0.1.dev2/langkit/input_output.py
--rw-r--r--   0        0        0      912 2023-05-16 16:10:15.942898 langkit-0.0.1.dev2/langkit/pattern_groups.json
--rw-r--r--   0        0        0     2509 2023-05-16 16:10:15.942898 langkit-0.0.1.dev2/langkit/regexes.py
--rw-r--r--   0        0        0      488 2023-05-09 23:30:20.252898 langkit-0.0.1.dev2/langkit/sentiment.py
--rw-r--r--   0        0        0      685 2023-05-12 18:53:48.262898 langkit-0.0.1.dev2/langkit/tests/conftest.py
--rw-r--r--   0        0        0     2302 2023-05-17 23:35:00.232537 langkit-0.0.1.dev2/langkit/tests/test_patterns.py
--rw-r--r--   0        0        0     2241 2023-05-12 18:53:48.262898 langkit-0.0.1.dev2/langkit/tests/test_themes.py
--rw-r--r--   0        0        0     2404 2023-05-09 23:30:20.252898 langkit-0.0.1.dev2/langkit/textstat.py
--rw-r--r--   0        0        0     9024 2023-05-17 23:35:21.462537 langkit-0.0.1.dev2/langkit/themes.json
--rw-r--r--   0        0        0      261 2023-05-17 23:35:21.462537 langkit-0.0.1.dev2/langkit/themes.json.txt
--rw-r--r--   0        0        0     2914 2023-05-16 16:10:15.952898 langkit-0.0.1.dev2/langkit/themes.py
--rw-r--r--   0        0        0      705 2023-05-17 23:35:21.462537 langkit-0.0.1.dev2/langkit/toxicity.py
--rw-r--r--   0        0        0      143 2023-05-12 18:53:48.272898 langkit-0.0.1.dev2/langkit/transformer.py
--rw-r--r--   0        0        0      605 2023-05-17 23:35:55.572537 langkit-0.0.1.dev2/pyproject.toml
--rw-r--r--   0        0        0     3135 1970-01-01 00:00:00.000000 langkit-0.0.1.dev2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-27 19:37:47.238351 langkit-0.0.1.dev3/LICENSE
+-rw-r--r--   0        0        0     2256 2023-05-17 23:35:21.462537 langkit-0.0.1.dev3/README.md
+-rw-r--r--   0        0        0      718 2023-05-17 23:35:21.462537 langkit-0.0.1.dev3/langkit/__init__.py
+-rw-r--r--   0        0        0     9959 2023-05-17 23:35:21.462537 langkit-0.0.1.dev3/langkit/examples/Batch_to_Whylabs.ipynb
+-rw-r--r--   0        0        0   267155 2023-05-17 23:35:00.232537 langkit-0.0.1.dev3/langkit/examples/LLM_to_WhyLabs.ipynb
+-rw-r--r--   0        0        0     1719 2023-05-17 23:35:00.232537 langkit-0.0.1.dev3/langkit/examples/Logging_Text.ipynb
+-rw-r--r--   0        0        0     5878 2023-05-17 23:35:21.462537 langkit-0.0.1.dev3/langkit/examples/Sentiment_and_Toxicity.ipynb
+-rw-r--r--   0        0        0      927 2023-05-12 18:53:48.262898 langkit-0.0.1.dev3/langkit/input_output.py
+-rw-r--r--   0        0        0      912 2023-05-16 16:10:15.942898 langkit-0.0.1.dev3/langkit/pattern_groups.json
+-rw-r--r--   0        0        0     2509 2023-05-16 16:10:15.942898 langkit-0.0.1.dev3/langkit/regexes.py
+-rw-r--r--   0        0        0      488 2023-05-09 23:30:20.252898 langkit-0.0.1.dev3/langkit/sentiment.py
+-rw-r--r--   0        0        0      685 2023-05-12 18:53:48.262898 langkit-0.0.1.dev3/langkit/tests/conftest.py
+-rw-r--r--   0        0        0     2302 2023-05-17 23:35:00.232537 langkit-0.0.1.dev3/langkit/tests/test_patterns.py
+-rw-r--r--   0        0        0     2241 2023-05-12 18:53:48.262898 langkit-0.0.1.dev3/langkit/tests/test_themes.py
+-rw-r--r--   0        0        0     2404 2023-05-09 23:30:20.252898 langkit-0.0.1.dev3/langkit/textstat.py
+-rw-r--r--   0        0        0     9024 2023-05-17 23:35:21.462537 langkit-0.0.1.dev3/langkit/themes.json
+-rw-r--r--   0        0        0      261 2023-05-17 23:35:21.462537 langkit-0.0.1.dev3/langkit/themes.json.txt
+-rw-r--r--   0        0        0     2914 2023-05-16 16:10:15.952898 langkit-0.0.1.dev3/langkit/themes.py
+-rw-r--r--   0        0        0      705 2023-05-17 23:35:21.462537 langkit-0.0.1.dev3/langkit/toxicity.py
+-rw-r--r--   0        0        0      143 2023-05-12 18:53:48.272898 langkit-0.0.1.dev3/langkit/transformer.py
+-rw-r--r--   0        0        0      599 2023-05-18 00:02:21.232537 langkit-0.0.1.dev3/pyproject.toml
+-rw-r--r--   0        0        0     3117 1970-01-01 00:00:00.000000 langkit-0.0.1.dev3/PKG-INFO
```

### Comparing `langkit-0.0.1.dev2/LICENSE` & `langkit-0.0.1.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1.dev2/README.md` & `langkit-0.0.1.dev3/README.md`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1.dev2/langkit/__init__.py` & `langkit-0.0.1.dev3/langkit/__init__.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1.dev2/langkit/examples/Batch_to_Whylabs.ipynb` & `langkit-0.0.1.dev3/langkit/examples/Batch_to_Whylabs.ipynb`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1.dev2/langkit/examples/LLM_to_WhyLabs.ipynb` & `langkit-0.0.1.dev3/langkit/examples/LLM_to_WhyLabs.ipynb`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1.dev2/langkit/examples/Logging_Text.ipynb` & `langkit-0.0.1.dev3/langkit/examples/Logging_Text.ipynb`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1.dev2/langkit/examples/Sentiment_and_Toxicity.ipynb` & `langkit-0.0.1.dev3/langkit/examples/Sentiment_and_Toxicity.ipynb`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1.dev2/langkit/input_output.py` & `langkit-0.0.1.dev3/langkit/input_output.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1.dev2/langkit/pattern_groups.json` & `langkit-0.0.1.dev3/langkit/pattern_groups.json`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1.dev2/langkit/regexes.py` & `langkit-0.0.1.dev3/langkit/regexes.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1.dev2/langkit/tests/conftest.py` & `langkit-0.0.1.dev3/langkit/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1.dev2/langkit/tests/test_patterns.py` & `langkit-0.0.1.dev3/langkit/tests/test_patterns.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1.dev2/langkit/tests/test_themes.py` & `langkit-0.0.1.dev3/langkit/tests/test_themes.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1.dev2/langkit/textstat.py` & `langkit-0.0.1.dev3/langkit/textstat.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1.dev2/langkit/themes.json` & `langkit-0.0.1.dev3/langkit/themes.json`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1.dev2/langkit/themes.py` & `langkit-0.0.1.dev3/langkit/themes.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1.dev2/langkit/toxicity.py` & `langkit-0.0.1.dev3/langkit/toxicity.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1.dev2/PKG-INFO` & `langkit-0.0.1.dev3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: langkit
-Version: 0.0.1.dev2
+Version: 0.0.1.dev3
 Summary: A collection of text metric udfs for whylogs profiling and monitoring in WhyLabs
 License: Apache-2.0
 Author: WhyLabs.ai
 Author-email: langkit@whylabs.ai
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: datasets (>=2.12.0,<3.0.0)
+Requires-Dist: datasets
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: openai (>=0.27.6,<0.28.0)
 Requires-Dist: pandas
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0)
 Requires-Dist: textstat (>=0.7.3,<0.8.0)
 Requires-Dist: whylogs (>=1.1.40,<2.0.0)
 Description-Content-Type: text/markdown
```

