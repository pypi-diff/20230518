# Comparing `tmp/ctransformers-0.1.0.tar.gz` & `tmp/ctransformers-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctransformers-0.1.0.tar", last modified: Sun May 14 23:22:15 2023, max compression
+gzip compressed data, was "ctransformers-0.1.1.tar", last modified: Thu May 18 20:26:08 2023, max compression
```

## Comparing `ctransformers-0.1.0.tar` & `ctransformers-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-14 23:22:15.399528 ctransformers-0.1.0/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    11947 2023-05-14 23:22:15.399528 ctransformers-0.1.0/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     8359 2023-05-14 23:09:15.000000 ctransformers-0.1.0/README.md
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-14 23:22:15.389528 ctransformers-0.1.0/ctransformers/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       79 2023-05-14 08:13:36.000000 ctransformers-0.1.0/ctransformers/__init__.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     5357 2023-05-14 18:30:56.000000 ctransformers-0.1.0/ctransformers/hub.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2226 2023-05-14 13:20:54.000000 ctransformers-0.1.0/ctransformers/langchain.py
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-14 23:22:15.389528 ctransformers-0.1.0/ctransformers/lib/
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-14 23:22:15.389528 ctransformers-0.1.0/ctransformers/lib/avx/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   402432 2023-05-14 22:26:24.000000 ctransformers-0.1.0/ctransformers/lib/avx/ctransformers.dll
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   905907 2023-05-14 22:26:24.000000 ctransformers-0.1.0/ctransformers/lib/avx/libctransformers.dylib
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   545536 2023-05-14 22:26:24.000000 ctransformers-0.1.0/ctransformers/lib/avx/libctransformers.so
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-14 23:22:15.389528 ctransformers-0.1.0/ctransformers/lib/avx2/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   388608 2023-05-14 22:26:24.000000 ctransformers-0.1.0/ctransformers/lib/avx2/ctransformers.dll
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   905907 2023-05-14 22:26:24.000000 ctransformers-0.1.0/ctransformers/lib/avx2/libctransformers.dylib
--rwxr-xr-x   0 ravindra  (1000) ravindra  (1000)   545536 2023-05-14 22:26:24.000000 ctransformers-0.1.0/ctransformers/lib/avx2/libctransformers.so
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-14 23:22:15.399528 ctransformers-0.1.0/ctransformers/lib/basic/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   394752 2023-05-14 22:26:24.000000 ctransformers-0.1.0/ctransformers/lib/basic/ctransformers.dll
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   889523 2023-05-14 22:26:24.000000 ctransformers-0.1.0/ctransformers/lib/basic/libctransformers.dylib
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   512768 2023-05-14 22:26:24.000000 ctransformers-0.1.0/ctransformers/lib/basic/libctransformers.so
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1033 2023-05-12 14:01:41.000000 ctransformers-0.1.0/ctransformers/lib.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     7966 2023-05-14 18:15:09.000000 ctransformers-0.1.0/ctransformers/llm.py
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-14 23:22:15.389528 ctransformers-0.1.0/ctransformers.egg-info/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    11947 2023-05-14 23:22:15.000000 ctransformers-0.1.0/ctransformers.egg-info/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      744 2023-05-14 23:22:15.000000 ctransformers-0.1.0/ctransformers.egg-info/SOURCES.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-05-14 23:22:15.000000 ctransformers-0.1.0/ctransformers.egg-info/dependency_links.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-05-14 23:22:15.000000 ctransformers-0.1.0/ctransformers.egg-info/not-zip-safe
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       32 2023-05-14 23:22:15.000000 ctransformers-0.1.0/ctransformers.egg-info/requires.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       14 2023-05-14 23:22:15.000000 ctransformers-0.1.0/ctransformers.egg-info/top_level.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-05-14 23:22:15.399528 ctransformers-0.1.0/setup.cfg
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1451 2023-05-14 23:21:28.000000 ctransformers-0.1.0/setup.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-18 20:26:08.126294 ctransformers-0.1.1/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    16975 2023-05-18 20:26:08.126294 ctransformers-0.1.1/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    12435 2023-05-18 20:14:09.000000 ctransformers-0.1.1/README.md
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-18 20:26:08.106294 ctransformers-0.1.1/ctransformers/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       79 2023-05-14 08:13:36.000000 ctransformers-0.1.1/ctransformers/__init__.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     5875 2023-05-18 15:44:53.000000 ctransformers-0.1.1/ctransformers/hub.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1759 2023-05-17 19:24:39.000000 ctransformers-0.1.1/ctransformers/langchain.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-18 20:26:08.106294 ctransformers-0.1.1/ctransformers/lib/
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-18 20:26:08.116294 ctransformers-0.1.1/ctransformers/lib/avx/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   402432 2023-05-17 20:01:06.000000 ctransformers-0.1.1/ctransformers/lib/avx/ctransformers.dll
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   905907 2023-05-14 22:26:24.000000 ctransformers-0.1.1/ctransformers/lib/avx/libctransformers.dylib
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   545536 2023-05-14 22:26:24.000000 ctransformers-0.1.1/ctransformers/lib/avx/libctransformers.so
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-18 20:26:08.116294 ctransformers-0.1.1/ctransformers/lib/avx2/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   388608 2023-05-17 20:01:06.000000 ctransformers-0.1.1/ctransformers/lib/avx2/ctransformers.dll
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   905907 2023-05-14 22:26:24.000000 ctransformers-0.1.1/ctransformers/lib/avx2/libctransformers.dylib
+-rwxr-xr-x   0 ravindra  (1000) ravindra  (1000)   545536 2023-05-14 22:26:24.000000 ctransformers-0.1.1/ctransformers/lib/avx2/libctransformers.so
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-18 20:26:08.126294 ctransformers-0.1.1/ctransformers/lib/basic/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   394752 2023-05-17 20:01:06.000000 ctransformers-0.1.1/ctransformers/lib/basic/ctransformers.dll
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   889523 2023-05-14 22:26:24.000000 ctransformers-0.1.1/ctransformers/lib/basic/libctransformers.dylib
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   512768 2023-05-14 22:26:24.000000 ctransformers-0.1.1/ctransformers/lib/basic/libctransformers.so
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1033 2023-05-12 14:01:41.000000 ctransformers-0.1.1/ctransformers/lib.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    13074 2023-05-18 20:09:31.000000 ctransformers-0.1.1/ctransformers/llm.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-18 20:26:08.106294 ctransformers-0.1.1/ctransformers.egg-info/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    16975 2023-05-18 20:26:08.000000 ctransformers-0.1.1/ctransformers.egg-info/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      744 2023-05-18 20:26:08.000000 ctransformers-0.1.1/ctransformers.egg-info/SOURCES.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-05-18 20:26:08.000000 ctransformers-0.1.1/ctransformers.egg-info/dependency_links.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-05-18 20:26:08.000000 ctransformers-0.1.1/ctransformers.egg-info/not-zip-safe
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       32 2023-05-18 20:26:08.000000 ctransformers-0.1.1/ctransformers.egg-info/requires.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       14 2023-05-18 20:26:08.000000 ctransformers-0.1.1/ctransformers.egg-info/top_level.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-05-18 20:26:08.126294 ctransformers-0.1.1/setup.cfg
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1451 2023-05-18 20:21:47.000000 ctransformers-0.1.1/setup.py
```

### Comparing `ctransformers-0.1.0/PKG-INFO` & `ctransformers-0.1.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,343 +1,437 @@
-Metadata-Version: 2.1
-Name: ctransformers
-Version: 0.1.0
-Summary: Python bindings for the Transformer models implemented in C/C++ using GGML library.
-Home-page: https://github.com/marella/ctransformers
-Author: Ravindra Marella
-Author-email: mv.ravindra007@gmail.com
-License: MIT
-Description: # [C Transformers](https://github.com/marella/ctransformers) [![PyPI](https://img.shields.io/pypi/v/ctransformers)](https://pypi.org/project/ctransformers/) [![tests](https://github.com/marella/ctransformers/actions/workflows/tests.yml/badge.svg)](https://github.com/marella/ctransformers/actions/workflows/tests.yml) [![build](https://github.com/marella/ctransformers/actions/workflows/build.yml/badge.svg)](https://github.com/marella/ctransformers/actions/workflows/build.yml)
-        
-        Python bindings for the Transformer models implemented in C/C++ using [GGML](https://github.com/ggerganov/ggml) library.
-        
-        - [Supported Models](#supported-models)
-        - [Installation](#installation)
-        - [Usage](#usage)
-          - [Hugging Face Hub](#hugging-face-hub)
-          - [LangChain](#langchain)
-        - [Documentation](#documentation)
-        - [License](#license)
-        
-        ## Supported Models
-        
-        | Models             | Model Type  |
-        | :----------------- | ----------- |
-        | GPT-2              | `gpt2`      |
-        | GPT-J, GPT4All-J   | `gptj`      |
-        | GPT-NeoX, StableLM | `gpt_neox`  |
-        | Dolly V2           | `dolly-v2`  |
-        | StarCoder          | `starcoder` |
-        
-        More models coming soon.
-        
-        ## Installation
-        
-        ```sh
-        pip install ctransformers
-        ```
-        
-        ## Usage
-        
-        It provides a unified interface for all models:
-        
-        ```py
-        from ctransformers import AutoModelForCausalLM
-        
-        llm = AutoModelForCausalLM.from_pretrained('/path/to/ggml-gpt-2.bin', model_type='gpt2')
-        
-        print(llm('AI is going to'))
-        ```
-        
-        [Run in Google Colab](https://colab.research.google.com/drive/1GMhYMUAv_TyZkpfvUI1NirM8-9mCXQyL)
-        
-        If you are getting `illegal instruction` error, try using `lib='avx'` or `lib='basic'`:
-        
-        ```py
-        llm = AutoModelForCausalLM.from_pretrained('/path/to/ggml-gpt-2.bin', model_type='gpt2', lib='avx')
-        ```
-        
-        It provides a generator interface for more control:
-        
-        ```py
-        tokens = llm.tokenize('AI is going to')
-        
-        for token in llm.generate(tokens):
-            print(llm.detokenize(token))
-        ```
-        
-        This allows you to use a custom tokenizer.
-        
-        It also provides access to the low-level C API. See [Documentation](#documentation) section below.
-        
-        ### Hugging Face Hub
-        
-        It can be used with models hosted on the Hub:
-        
-        ```py
-        llm = AutoModelForCausalLM.from_pretrained('marella/gpt-2-ggml')
-        ```
-        
-        If a model repo has multiple model files (`.bin` files), specify a model file using:
-        
-        ```py
-        llm = AutoModelForCausalLM.from_pretrained('marella/gpt-2-ggml', model_file='ggml-model.bin')
-        ```
-        
-        It can be used with your own models uploaded on the Hub. For better user experience, upload only one model per repo.
-        
-        To use it with your own model, add `config.json` file to your model repo specifying the `model_type`:
-        
-        ```json
-        {
-          "model_type": "gpt2"
-        }
-        ```
-        
-        You can also specify additional parameters under `task_specific_params.text-generation`:
-        
-        ```json
-        {
-          "model_type": "gpt2",
-          "task_specific_params": {
-            "text-generation": {
-              "top_k": 40,
-              "top_p": 0.95,
-              "temperature": 0.8,
-              "repetition_penalty": 1.1,
-              "last_n_tokens": 64
-            }
-          }
-        }
-        ```
-        
-        See [marella/gpt-2-ggml](https://huggingface.co/marella/gpt-2-ggml/blob/main/config.json) for a minimal example and [marella/gpt-2-ggml-example](https://huggingface.co/marella/gpt-2-ggml-example/blob/main/config.json) for a full example.
-        
-        ### LangChain
-        
-        [LangChain](https://python.langchain.com/) is a framework for developing applications powered by language models. A LangChain LLM object can be created using:
-        
-        ```py
-        from ctransformers.langchain import CTransformers
-        
-        llm = CTransformers(model='/path/to/ggml-gpt-2.bin', model_type='gpt2')
-        
-        print(llm('AI is going to'))
-        ```
-        
-        If you are getting `illegal instruction` error, try using `lib='avx'` or `lib='basic'`:
-        
-        ```py
-        llm = CTransformers(model='/path/to/ggml-gpt-2.bin', model_type='gpt2', lib='avx')
-        ```
-        
-        It can also be used with models hosted on the Hugging Face Hub:
-        
-        ```py
-        llm = CTransformers(model='marella/gpt-2-ggml')
-        ```
-        
-        Additional parameters can be passed using the `config` parameter:
-        
-        ```py
-        config = {'max_new_tokens': 256, 'repetition_penalty': 1.1}
-        
-        llm = CTransformers(model='marella/gpt-2-ggml', config=config)
-        ```
-        
-        It can be used with other LangChain modules:
-        
-        ```py
-        from langchain import PromptTemplate, LLMChain
-        
-        template = """Question: {question}
-        
-        Answer:"""
-        
-        prompt = PromptTemplate(template=template, input_variables=['question'])
-        
-        llm_chain = LLMChain(prompt=prompt, llm=llm)
-        
-        print(llm_chain.run('What is AI?'))
-        ```
-        
-        ## Documentation
-        
-        ### Parameters
-        
-        | Name                 | Type    | Description                                                      | Default |
-        | :------------------- | :------ | :--------------------------------------------------------------- | :------ |
-        | `top_k`              | `int`   | The top-k sampling parameter.                                    | `40`    |
-        | `top_p`              | `float` | The top-p sampling parameter.                                    | `0.95`  |
-        | `temperature`        | `float` | The temperature parameter.                                       | `0.8`   |
-        | `repetition_penalty` | `float` | The repetition penalty parameter.                                | `1.0`   |
-        | `last_n_tokens`      | `int`   | Number of last tokens to use for repetition penalty.             | `64`    |
-        | `seed`               | `int`   | Seed for sampling tokens.                                        | Random  |
-        | `max_new_tokens`     | `int`   | Maximum number of new tokens to generate.                        | `256`   |
-        | `reset`              | `bool`  | Whether to reset the model state before evaluating a new prompt. | `True`  |
-        | `batch_size`         | `int`   | Batch size for evaluating tokens.                                | `8`     |
-        | `threads`            | `int`   | Number of threads to use.                                        | Auto    |
-        
-        <!-- API_DOCS -->
-        
-        ### <kbd>class</kbd> `AutoModelForCausalLM`
-        
-        ---
-        
-        #### <kbd>classmethod</kbd> `AutoModelForCausalLM.from_pretrained`
-        
-        ```python
-        from_pretrained(
-            model_path_or_repo_id: 'str',
-            model_type: 'Optional[str]' = None,
-            model_file: 'Optional[str]' = None,
-            config: 'Optional[AutoConfig]' = None,
-            lib: 'Optional[str]' = None,
-            **kwargs
-        ) → LLM
-        ```
-        
-        ### <kbd>class</kbd> `LLM`
-        
-        ### <kbd>method</kbd> `LLM.__init__`
-        
-        ```python
-        __init__(
-            model_path: str,
-            model_type: str,
-            config: Optional[ctransformers.llm.Config] = None,
-            lib: Optional[str] = None
-        )
-        ```
-        
-        ---
-        
-        ##### <kbd>property</kbd> LLM.config
-        
-        ---
-        
-        ##### <kbd>property</kbd> LLM.model_path
-        
-        ---
-        
-        ##### <kbd>property</kbd> LLM.model_type
-        
-        ---
-        
-        #### <kbd>method</kbd> `LLM.detokenize`
-        
-        ```python
-        detokenize(tokens: Union[Sequence[int], int]) → str
-        ```
-        
-        ---
-        
-        #### <kbd>method</kbd> `LLM.eval`
-        
-        ```python
-        eval(
-            tokens: Sequence[int],
-            batch_size: Optional[int] = None,
-            threads: Optional[int] = None
-        ) → None
-        ```
-        
-        ---
-        
-        #### <kbd>method</kbd> `LLM.generate`
-        
-        ```python
-        generate(
-            tokens: Sequence[int],
-            top_k: Optional[int] = None,
-            top_p: Optional[float] = None,
-            temperature: Optional[float] = None,
-            repetition_penalty: Optional[float] = None,
-            last_n_tokens: Optional[int] = None,
-            seed: Optional[int] = None,
-            batch_size: Optional[int] = None,
-            threads: Optional[int] = None,
-            reset: Optional[bool] = None
-        ) → Generator[int, NoneType, NoneType]
-        ```
-        
-        ---
-        
-        #### <kbd>method</kbd> `LLM.is_eos_token`
-        
-        ```python
-        is_eos_token(token: int) → bool
-        ```
-        
-        ---
-        
-        #### <kbd>method</kbd> `LLM.reset`
-        
-        ```python
-        reset() → None
-        ```
-        
-        ---
-        
-        #### <kbd>method</kbd> `LLM.sample`
-        
-        ```python
-        sample(
-            top_k: Optional[int] = None,
-            top_p: Optional[float] = None,
-            temperature: Optional[float] = None,
-            repetition_penalty: Optional[float] = None,
-            last_n_tokens: Optional[int] = None,
-            seed: Optional[int] = None
-        ) → int
-        ```
-        
-        ---
-        
-        #### <kbd>method</kbd> `LLM.tokenize`
-        
-        ```python
-        tokenize(text: str) → List[int]
-        ```
-        
-        ---
-        
-        #### <kbd>method</kbd> `LLM.__call__`
-        
-        ```python
-        __call__(
-            prompt: str,
-            max_new_tokens: Optional[int] = None,
-            top_k: Optional[int] = None,
-            top_p: Optional[float] = None,
-            temperature: Optional[float] = None,
-            repetition_penalty: Optional[float] = None,
-            last_n_tokens: Optional[int] = None,
-            seed: Optional[int] = None,
-            batch_size: Optional[int] = None,
-            threads: Optional[int] = None,
-            reset: Optional[bool] = None
-        ) → str
-        ```
-        
-        <!-- API_DOCS -->
-        
-        ## License
-        
-        [MIT](https://github.com/marella/ctransformers/blob/main/LICENSE)
-        
-Keywords: ctransformers transformers ai llm
-Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-Provides-Extra: tests
+# [C Transformers](https://github.com/marella/ctransformers) [![PyPI](https://img.shields.io/pypi/v/ctransformers)](https://pypi.org/project/ctransformers/) [![tests](https://github.com/marella/ctransformers/actions/workflows/tests.yml/badge.svg)](https://github.com/marella/ctransformers/actions/workflows/tests.yml) [![build](https://github.com/marella/ctransformers/actions/workflows/build.yml/badge.svg)](https://github.com/marella/ctransformers/actions/workflows/build.yml)
+
+Python bindings for the Transformer models implemented in C/C++ using [GGML](https://github.com/ggerganov/ggml) library.
+
+- [Supported Models](#supported-models)
+- [Installation](#installation)
+- [Usage](#usage)
+  - [Hugging Face Hub](#hugging-face-hub)
+  - [LangChain](#langchain)
+- [Documentation](#documentation)
+- [License](#license)
+
+## Supported Models
+
+| Models             | Model Type  |
+| :----------------- | ----------- |
+| GPT-2              | `gpt2`      |
+| GPT-J, GPT4All-J   | `gptj`      |
+| GPT-NeoX, StableLM | `gpt_neox`  |
+| Dolly V2           | `dolly-v2`  |
+| StarCoder          | `starcoder` |
+
+More models coming soon.
+
+## Installation
+
+```sh
+pip install ctransformers
+```
+
+## Usage
+
+It provides a unified interface for all models:
+
+```py
+from ctransformers import AutoModelForCausalLM
+
+llm = AutoModelForCausalLM.from_pretrained('/path/to/ggml-gpt-2.bin', model_type='gpt2')
+
+print(llm('AI is going to'))
+```
+
+[Run in Google Colab](https://colab.research.google.com/drive/1GMhYMUAv_TyZkpfvUI1NirM8-9mCXQyL)
+
+If you are getting `illegal instruction` error, try using `lib='avx'` or `lib='basic'`:
+
+```py
+llm = AutoModelForCausalLM.from_pretrained('/path/to/ggml-gpt-2.bin', model_type='gpt2', lib='avx')
+```
+
+It provides a generator interface for more control:
+
+```py
+tokens = llm.tokenize('AI is going to')
+
+for token in llm.generate(tokens):
+    print(llm.detokenize(token))
+```
+
+This allows you to use a custom tokenizer.
+
+It also provides access to the low-level C API. See [Documentation](#documentation) section below.
+
+### Hugging Face Hub
+
+It can be used with models hosted on the Hub:
+
+```py
+llm = AutoModelForCausalLM.from_pretrained('marella/gpt-2-ggml')
+```
+
+If a model repo has multiple model files (`.bin` files), specify a model file using:
+
+```py
+llm = AutoModelForCausalLM.from_pretrained('marella/gpt-2-ggml', model_file='ggml-model.bin')
+```
+
+It can be used with your own models uploaded on the Hub. For better user experience, upload only one model per repo.
+
+To use it with your own model, add `config.json` file to your model repo specifying the `model_type`:
+
+```json
+{
+  "model_type": "gpt2"
+}
+```
+
+You can also specify additional parameters under `task_specific_params.text-generation`:
+
+```json
+{
+  "model_type": "gpt2",
+  "task_specific_params": {
+    "text-generation": {
+      "top_k": 40,
+      "top_p": 0.95,
+      "temperature": 0.8,
+      "repetition_penalty": 1.1,
+      "last_n_tokens": 64
+    }
+  }
+}
+```
+
+See [marella/gpt-2-ggml](https://huggingface.co/marella/gpt-2-ggml/blob/main/config.json) for a minimal example and [marella/gpt-2-ggml-example](https://huggingface.co/marella/gpt-2-ggml-example/blob/main/config.json) for a full example.
+
+### LangChain
+
+[LangChain](https://python.langchain.com/) is a framework for developing applications powered by language models. A LangChain LLM object can be created using:
+
+```py
+from ctransformers.langchain import CTransformers
+
+llm = CTransformers(model='/path/to/ggml-gpt-2.bin', model_type='gpt2')
+
+print(llm('AI is going to'))
+```
+
+If you are getting `illegal instruction` error, try using `lib='avx'` or `lib='basic'`:
+
+```py
+llm = CTransformers(model='/path/to/ggml-gpt-2.bin', model_type='gpt2', lib='avx')
+```
+
+It can also be used with models hosted on the Hugging Face Hub:
+
+```py
+llm = CTransformers(model='marella/gpt-2-ggml')
+```
+
+Additional parameters can be passed using the `config` parameter:
+
+```py
+config = {'max_new_tokens': 256, 'repetition_penalty': 1.1}
+
+llm = CTransformers(model='marella/gpt-2-ggml', config=config)
+```
+
+It can be used with other LangChain modules:
+
+```py
+from langchain import PromptTemplate, LLMChain
+
+template = """Question: {question}
+
+Answer:"""
+
+prompt = PromptTemplate(template=template, input_variables=['question'])
+
+llm_chain = LLMChain(prompt=prompt, llm=llm)
+
+print(llm_chain.run('What is AI?'))
+```
+
+## Documentation
+
+### Parameters
+
+| Name                 | Type        | Description                                              | Default |
+| :------------------- | :---------- | :------------------------------------------------------- | :------ |
+| `top_k`              | `int`       | The top-k value to use for sampling.                     | `40`    |
+| `top_p`              | `float`     | The top-p value to use for sampling.                     | `0.95`  |
+| `temperature`        | `float`     | The temperature to use for sampling.                     | `0.8`   |
+| `repetition_penalty` | `float`     | The repetition penalty to use for sampling.              | `1.0`   |
+| `last_n_tokens`      | `int`       | The number of last tokens to use for repetition penalty. | `64`    |
+| `seed`               | `int`       | The seed value to use for sampling tokens.               | Random  |
+| `max_new_tokens`     | `int`       | The maximum number of new tokens to generate.            | `256`   |
+| `stop`               | `List[str]` | A list of sequences to stop generation when encountered. | `[]`    |
+| `reset`              | `bool`      | Whether to reset the model state before generating text. | `True`  |
+| `batch_size`         | `int`       | The batch size to use for evaluating tokens.             | `8`     |
+| `threads`            | `int`       | The number of threads to use for evaluating tokens.      | Auto    |
+
+<!-- API_DOCS -->
+
+### <kbd>class</kbd> `AutoModelForCausalLM`
+
+---
+
+#### <kbd>classmethod</kbd> `AutoModelForCausalLM.from_pretrained`
+
+```python
+from_pretrained(
+    model_path_or_repo_id: str,
+    model_type: Optional[str] = None,
+    model_file: Optional[str] = None,
+    config: Optional[ctransformers.hub.AutoConfig] = None,
+    lib: Optional[str] = None,
+    **kwargs
+) → LLM
+```
+
+Loads the language model from a local file or remote repo.
+
+**Args:**
+
+- <b>`model_path_or_repo_id`</b>: The path to a model file or directory or the name of a Hugging Face Hub model repo.
+- <b>`model_type`</b>: The model type.
+- <b>`model_file`</b>: The name of the model file in repo or directory.
+- <b>`config`</b>: `AutoConfig` object.
+- <b>`lib`</b>: The path to a shared library or one of `avx2`, `avx`, `basic`.
+
+**Returns:**
+`LLM` object.
+
+### <kbd>class</kbd> `LLM`
+
+### <kbd>method</kbd> `LLM.__init__`
+
+```python
+__init__(
+    model_path: str,
+    model_type: str,
+    config: Optional[ctransformers.llm.Config] = None,
+    lib: Optional[str] = None
+)
+```
+
+Loads the language model from a local file.
+
+**Args:**
+
+- <b>`model_path`</b>: The path to a model file.
+- <b>`model_type`</b>: The model type.
+- <b>`config`</b>: `Config` object.
+- <b>`lib`</b>: The path to a shared library or one of `avx2`, `avx`, `basic`.
+
+---
+
+##### <kbd>property</kbd> LLM.config
+
+The config object.
+
+---
+
+##### <kbd>property</kbd> LLM.model_path
+
+The path to the model file.
+
+---
+
+##### <kbd>property</kbd> LLM.model_type
+
+The model type.
+
+---
+
+#### <kbd>method</kbd> `LLM.detokenize`
+
+```python
+detokenize(tokens: Sequence[int]) → str
+```
+
+Converts a list of tokens to text.
+
+**Args:**
+
+- <b>`tokens`</b>: The list of tokens.
+
+**Returns:**
+The combined text of all tokens.
+
+---
+
+#### <kbd>method</kbd> `LLM.eval`
+
+```python
+eval(
+    tokens: Sequence[int],
+    batch_size: Optional[int] = None,
+    threads: Optional[int] = None
+) → None
+```
+
+Evaluates a list of tokens.
+
+**Args:**
+
+- <b>`tokens`</b>: The list of tokens to evaluate.
+- <b>`batch_size`</b>: The batch size to use for evaluating tokens. Default: `8`
+- <b>`threads`</b>: The number of threads to use for evaluating tokens. Default: `-1`
+
+---
+
+#### <kbd>method</kbd> `LLM.generate`
+
+```python
+generate(
+    tokens: Sequence[int],
+    top_k: Optional[int] = None,
+    top_p: Optional[float] = None,
+    temperature: Optional[float] = None,
+    repetition_penalty: Optional[float] = None,
+    last_n_tokens: Optional[int] = None,
+    seed: Optional[int] = None,
+    batch_size: Optional[int] = None,
+    threads: Optional[int] = None,
+    reset: Optional[bool] = None
+) → Generator[int, NoneType, NoneType]
+```
+
+Generates new tokens from a list of tokens.
+
+**Args:**
+
+- <b>`tokens`</b>: The list of tokens to generate tokens from.
+- <b>`top_k`</b>: The top-k value to use for sampling. Default: `40`
+- <b>`top_p`</b>: The top-p value to use for sampling. Default: `0.95`
+- <b>`temperature`</b>: The temperature to use for sampling. Default: `0.8`
+- <b>`repetition_penalty`</b>: The repetition penalty to use for sampling. Default: `1.0`
+- <b>`last_n_tokens`</b>: The number of last tokens to use for repetition penalty. Default: `64`
+- <b>`seed`</b>: The seed value to use for sampling tokens. Default: `-1`
+- <b>`batch_size`</b>: The batch size to use for evaluating tokens. Default: `8`
+- <b>`threads`</b>: The number of threads to use for evaluating tokens. Default: `-1`
+- <b>`reset`</b>: Whether to reset the model state before generating text. Default: `True`
+
+**Returns:**
+The generated tokens.
+
+---
+
+#### <kbd>method</kbd> `LLM.is_eos_token`
+
+```python
+is_eos_token(token: int) → bool
+```
+
+Checks if a token is an end-of-sequence token.
+
+**Args:**
+
+- <b>`token`</b>: The token to check.
+
+**Returns:**
+`True` if the token is an end-of-sequence token else `False`.
+
+---
+
+#### <kbd>method</kbd> `LLM.reset`
+
+```python
+reset() → None
+```
+
+Resets the model state.
+
+---
+
+#### <kbd>method</kbd> `LLM.sample`
+
+```python
+sample(
+    top_k: Optional[int] = None,
+    top_p: Optional[float] = None,
+    temperature: Optional[float] = None,
+    repetition_penalty: Optional[float] = None,
+    last_n_tokens: Optional[int] = None,
+    seed: Optional[int] = None
+) → int
+```
+
+Samples a token from the model.
+
+**Args:**
+
+- <b>`top_k`</b>: The top-k value to use for sampling. Default: `40`
+- <b>`top_p`</b>: The top-p value to use for sampling. Default: `0.95`
+- <b>`temperature`</b>: The temperature to use for sampling. Default: `0.8`
+- <b>`repetition_penalty`</b>: The repetition penalty to use for sampling. Default: `1.0`
+- <b>`last_n_tokens`</b>: The number of last tokens to use for repetition penalty. Default: `64`
+- <b>`seed`</b>: The seed value to use for sampling tokens. Default: `-1`
+
+**Returns:**
+The sampled token.
+
+---
+
+#### <kbd>method</kbd> `LLM.tokenize`
+
+```python
+tokenize(text: str) → List[int]
+```
+
+Converts a text into list of tokens.
+
+**Args:**
+
+- <b>`text`</b>: The text to tokenize.
+
+**Returns:**
+The list of tokens.
+
+---
+
+#### <kbd>method</kbd> `LLM.__call__`
+
+```python
+__call__(
+    prompt: str,
+    max_new_tokens: Optional[int] = None,
+    top_k: Optional[int] = None,
+    top_p: Optional[float] = None,
+    temperature: Optional[float] = None,
+    repetition_penalty: Optional[float] = None,
+    last_n_tokens: Optional[int] = None,
+    seed: Optional[int] = None,
+    batch_size: Optional[int] = None,
+    threads: Optional[int] = None,
+    stop: Optional[Sequence[str]] = None,
+    reset: Optional[bool] = None
+) → str
+```
+
+Generates text from a prompt.
+
+**Args:**
+
+- <b>`prompt`</b>: The prompt to generate text from.
+- <b>`max_new_tokens`</b>: The maximum number of new tokens to generate. Default: `256`
+- <b>`top_k`</b>: The top-k value to use for sampling. Default: `40`
+- <b>`top_p`</b>: The top-p value to use for sampling. Default: `0.95`
+- <b>`temperature`</b>: The temperature to use for sampling. Default: `0.8`
+- <b>`repetition_penalty`</b>: The repetition penalty to use for sampling. Default: `1.0`
+- <b>`last_n_tokens`</b>: The number of last tokens to use for repetition penalty. Default: `64`
+- <b>`seed`</b>: The seed value to use for sampling tokens. Default: `-1`
+- <b>`batch_size`</b>: The batch size to use for evaluating tokens. Default: `8`
+- <b>`threads`</b>: The number of threads to use for evaluating tokens. Default: `-1`
+- <b>`stop`</b>: A list of sequences to stop generation when encountered. Default: `None`
+- <b>`reset`</b>: Whether to reset the model state before generating text. Default: `True`
+
+**Returns:**
+The generated text.
+
+<!-- API_DOCS -->
+
+## License
+
+[MIT](https://github.com/marella/ctransformers/blob/main/LICENSE)
```

### Comparing `ctransformers-0.1.0/ctransformers/hub.py` & `ctransformers-0.1.1/ctransformers/hub.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import annotations
-
 import json
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Optional
 
 from huggingface_hub import snapshot_download
 from huggingface_hub.utils import validate_repo_id, HFValidationError
@@ -30,15 +28,15 @@
     model_type: Optional[str] = None
 
     @classmethod
     def from_pretrained(
         cls,
         model_path_or_repo_id: str,
         **kwargs,
-    ) -> AutoConfig:
+    ) -> 'AutoConfig':
         path_type = get_path_type(model_path_or_repo_id)
         if not path_type:
             raise ValueError(
                 f"Model path '{model_path_or_repo_id}' doesn't exist.")
 
         config = Config()
         auto_config = AutoConfig(config=config)
@@ -54,26 +52,30 @@
                     f"'{k}' is an invalid keyword argument for from_pretrained()"
                 )
             setattr(config, k, v)
 
         return auto_config
 
     @classmethod
-    def _update_from_repo(cls, repo_id: str, auto_config: AutoConfig) -> None:
+    def _update_from_repo(
+        cls,
+        repo_id: str,
+        auto_config: 'AutoConfig',
+    ) -> None:
         path = snapshot_download(repo_id=repo_id, allow_patterns='config.json')
         cls._update_from_dir(path, auto_config)
 
     @classmethod
-    def _update_from_dir(cls, path: str, auto_config: AutoConfig) -> None:
+    def _update_from_dir(cls, path: str, auto_config: 'AutoConfig') -> None:
         path = (Path(path) / 'config.json').resolve()
         if path.is_file():
             cls._update_from_file(path, auto_config)
 
     @classmethod
-    def _update_from_file(cls, path: str, auto_config: AutoConfig) -> None:
+    def _update_from_file(cls, path: str, auto_config: 'AutoConfig') -> None:
         with open(path) as f:
             config = json.load(f)
 
         auto_config.model_type = config.get('model_type')
         params = config.get('task_specific_params', {})
         params = params.get('text-generation', {})
         for name in [
@@ -97,14 +99,28 @@
         *,
         model_type: Optional[str] = None,
         model_file: Optional[str] = None,
         config: Optional[AutoConfig] = None,
         lib: Optional[str] = None,
         **kwargs,
     ) -> LLM:
+        """
+        Loads the language model from a local file or remote repo.
+
+        Args:
+            model_path_or_repo_id: The path to a model file or directory or the
+            name of a Hugging Face Hub model repo.
+            model_type: The model type.
+            model_file: The name of the model file in repo or directory.
+            config: `AutoConfig` object.
+            lib: The path to a shared library or one of `avx2`, `avx`, `basic`.
+
+        Returns:
+            `LLM` object.
+        """
         config = config or AutoConfig.from_pretrained(
             model_path_or_repo_id,
             **kwargs,
         )
         model_type = model_type or config.model_type
         if not model_type:
             raise ValueError(
```

### Comparing `ctransformers-0.1.0/ctransformers/lib/avx/ctransformers.dll` & `ctransformers-0.1.1/ctransformers/lib/avx/ctransformers.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800456dc
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun May 14 22:25:00 2023
+Time/Date		Sun May 14 23:39:08 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		0000000000046000
 SizeOfInitializedData	00000000000be000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000456dc
@@ -91823,17 +91823,19 @@
    18004a1a3:	addb   $0x0,(%rcx)
    18004a1a6:	add    %al,(%rax)
    18004a1a8:	or     %dh,0x4(%rbp)
    18004a1ab:	addb   $0x0,(%rcx)
    18004a1ae:	add    %al,(%rax)
    18004a1b0:	add    %al,(%rax)
    18004a1b2:	add    %al,(%rax)
-   18004a1b4:	mov    $0x64615f,%esp
-   18004a1b9:	add    %al,(%rax)
-   18004a1bb:	add    %cl,0x64000000(%rip)        # 0x1e404a1c1
+   18004a1b4:	sbb    $0x71,%al
+   18004a1b6:	(bad)
+   18004a1b7:	add    %al,%fs:(%rax)
+   18004a1ba:	add    %al,(%rax)
+   18004a1bc:	or     $0x64000000,%eax
    18004a1c1:	add    (%rax),%eax
    18004a1c3:	add    %al,0x4(%rsp,%rsi,4)
    18004a1c7:	add    %al,0x4(%rax,%rbp,4)
 	...
    18004a1ff:	add    %cl,%al
    18004a201:	mov    $0x4,%bh
    18004a203:	addb   $0x0,(%rcx)
```

### Comparing `ctransformers-0.1.0/ctransformers/lib/avx/libctransformers.dylib` & `ctransformers-0.1.1/ctransformers/lib/avx/libctransformers.dylib`

 * *Files identical despite different names*

### Comparing `ctransformers-0.1.0/ctransformers/lib/avx/libctransformers.so` & `ctransformers-0.1.1/ctransformers/lib/avx/libctransformers.so`

 * *Files identical despite different names*

### Comparing `ctransformers-0.1.0/ctransformers/lib/avx2/ctransformers.dll` & `ctransformers-0.1.1/ctransformers/lib/avx2/ctransformers.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018004227c
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun May 14 22:24:23 2023
+Time/Date		Sun May 14 23:39:16 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		0000000000042a00
 SizeOfInitializedData	00000000000be000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000004227c
@@ -88795,16 +88795,15 @@
    1800472c3:	addb   $0x0,(%rcx)
    1800472c6:	add    %al,(%rax)
    1800472c8:	or     %al,0x4(%rbp)
    1800472cb:	addb   $0x0,(%rcx)
    1800472ce:	add    %al,(%rax)
    1800472d0:	add    %al,(%rax)
    1800472d2:	add    %al,(%rax)
-   1800472d4:	xchg   %eax,%edi
-   1800472d5:	pop    %rdi
+   1800472d4:	and    $0x71,%al
    1800472d6:	(bad)
    1800472d7:	add    %al,%fs:(%rax)
    1800472da:	add    %al,(%rax)
    1800472dc:	or     $0x64000000,%eax
    1800472e1:	add    (%rax),%eax
    1800472e3:	add    %al,0x4(%rbp,%rax,4)
    1800472e7:	add    %al,0x4(%rbx,%rsi,2)
```

### Comparing `ctransformers-0.1.0/ctransformers/lib/avx2/libctransformers.dylib` & `ctransformers-0.1.1/ctransformers/lib/avx2/libctransformers.dylib`

 * *Files identical despite different names*

### Comparing `ctransformers-0.1.0/ctransformers/lib/avx2/libctransformers.so` & `ctransformers-0.1.1/ctransformers/lib/avx2/libctransformers.so`

 * *Files identical despite different names*

### Comparing `ctransformers-0.1.0/ctransformers/lib/basic/ctransformers.dll` & `ctransformers-0.1.1/ctransformers/lib/basic/ctransformers.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180043bb8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun May 14 22:24:44 2023
+Time/Date		Sun May 14 23:38:07 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		0000000000044200
 SizeOfInitializedData	00000000000be000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000043bb8
@@ -90906,17 +90906,15 @@
    180049113:	addb   $0x0,(%rcx)
    180049116:	add    %al,(%rax)
    180049118:	sbb    %ah,0x4(%rbp)
    18004911b:	addb   $0x0,(%rcx)
    18004911e:	add    %al,(%rax)
    180049120:	add    %al,(%rax)
    180049122:	add    %al,(%rax)
-   180049124:	lods   %ds:(%rsi),%al
-   180049125:	pop    %rdi
-   180049126:	(bad)
+   180049124:	fbstp  0x61(%rax)
    180049127:	add    %al,%fs:(%rax)
    18004912a:	add    %al,(%rax)
    18004912c:	or     $0x64000000,%eax
    180049131:	add    (%rax),%eax
    180049133:	add    %al,%ah
    180049135:	movabs %eax,0x489c40004
 	...
```

### Comparing `ctransformers-0.1.0/ctransformers/lib/basic/libctransformers.dylib` & `ctransformers-0.1.1/ctransformers/lib/basic/libctransformers.dylib`

 * *Files identical despite different names*

### Comparing `ctransformers-0.1.0/ctransformers/lib/basic/libctransformers.so` & `ctransformers-0.1.1/ctransformers/lib/basic/libctransformers.so`

 * *Files identical despite different names*

### Comparing `ctransformers-0.1.0/ctransformers/lib.py` & `ctransformers-0.1.1/ctransformers/lib.py`

 * *Files identical despite different names*

### Comparing `ctransformers-0.1.0/ctransformers.egg-info/PKG-INFO` & `ctransformers-0.1.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctransformers
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python bindings for the Transformer models implemented in C/C++ using GGML library.
 Home-page: https://github.com/marella/ctransformers
 Author: Ravindra Marella
 Author-email: mv.ravindra007@gmail.com
 License: MIT
 Description: # [C Transformers](https://github.com/marella/ctransformers) [![PyPI](https://img.shields.io/pypi/v/ctransformers)](https://pypi.org/project/ctransformers/) [![tests](https://github.com/marella/ctransformers/actions/workflows/tests.yml/badge.svg)](https://github.com/marella/ctransformers/actions/workflows/tests.yml) [![build](https://github.com/marella/ctransformers/actions/workflows/build.yml/badge.svg)](https://github.com/marella/ctransformers/actions/workflows/build.yml)
         
@@ -160,91 +160,137 @@
         print(llm_chain.run('What is AI?'))
         ```
         
         ## Documentation
         
         ### Parameters
         
-        | Name                 | Type    | Description                                                      | Default |
-        | :------------------- | :------ | :--------------------------------------------------------------- | :------ |
-        | `top_k`              | `int`   | The top-k sampling parameter.                                    | `40`    |
-        | `top_p`              | `float` | The top-p sampling parameter.                                    | `0.95`  |
-        | `temperature`        | `float` | The temperature parameter.                                       | `0.8`   |
-        | `repetition_penalty` | `float` | The repetition penalty parameter.                                | `1.0`   |
-        | `last_n_tokens`      | `int`   | Number of last tokens to use for repetition penalty.             | `64`    |
-        | `seed`               | `int`   | Seed for sampling tokens.                                        | Random  |
-        | `max_new_tokens`     | `int`   | Maximum number of new tokens to generate.                        | `256`   |
-        | `reset`              | `bool`  | Whether to reset the model state before evaluating a new prompt. | `True`  |
-        | `batch_size`         | `int`   | Batch size for evaluating tokens.                                | `8`     |
-        | `threads`            | `int`   | Number of threads to use.                                        | Auto    |
+        | Name                 | Type        | Description                                              | Default |
+        | :------------------- | :---------- | :------------------------------------------------------- | :------ |
+        | `top_k`              | `int`       | The top-k value to use for sampling.                     | `40`    |
+        | `top_p`              | `float`     | The top-p value to use for sampling.                     | `0.95`  |
+        | `temperature`        | `float`     | The temperature to use for sampling.                     | `0.8`   |
+        | `repetition_penalty` | `float`     | The repetition penalty to use for sampling.              | `1.0`   |
+        | `last_n_tokens`      | `int`       | The number of last tokens to use for repetition penalty. | `64`    |
+        | `seed`               | `int`       | The seed value to use for sampling tokens.               | Random  |
+        | `max_new_tokens`     | `int`       | The maximum number of new tokens to generate.            | `256`   |
+        | `stop`               | `List[str]` | A list of sequences to stop generation when encountered. | `[]`    |
+        | `reset`              | `bool`      | Whether to reset the model state before generating text. | `True`  |
+        | `batch_size`         | `int`       | The batch size to use for evaluating tokens.             | `8`     |
+        | `threads`            | `int`       | The number of threads to use for evaluating tokens.      | Auto    |
         
         <!-- API_DOCS -->
         
         ### <kbd>class</kbd> `AutoModelForCausalLM`
         
         ---
         
         #### <kbd>classmethod</kbd> `AutoModelForCausalLM.from_pretrained`
         
         ```python
         from_pretrained(
-            model_path_or_repo_id: 'str',
-            model_type: 'Optional[str]' = None,
-            model_file: 'Optional[str]' = None,
-            config: 'Optional[AutoConfig]' = None,
-            lib: 'Optional[str]' = None,
+            model_path_or_repo_id: str,
+            model_type: Optional[str] = None,
+            model_file: Optional[str] = None,
+            config: Optional[ctransformers.hub.AutoConfig] = None,
+            lib: Optional[str] = None,
             **kwargs
         ) → LLM
         ```
         
+        Loads the language model from a local file or remote repo.
+        
+        **Args:**
+        
+        - <b>`model_path_or_repo_id`</b>: The path to a model file or directory or the name of a Hugging Face Hub model repo.
+        - <b>`model_type`</b>: The model type.
+        - <b>`model_file`</b>: The name of the model file in repo or directory.
+        - <b>`config`</b>: `AutoConfig` object.
+        - <b>`lib`</b>: The path to a shared library or one of `avx2`, `avx`, `basic`.
+        
+        **Returns:**
+        `LLM` object.
+        
         ### <kbd>class</kbd> `LLM`
         
         ### <kbd>method</kbd> `LLM.__init__`
         
         ```python
         __init__(
             model_path: str,
             model_type: str,
             config: Optional[ctransformers.llm.Config] = None,
             lib: Optional[str] = None
         )
         ```
         
+        Loads the language model from a local file.
+        
+        **Args:**
+        
+        - <b>`model_path`</b>: The path to a model file.
+        - <b>`model_type`</b>: The model type.
+        - <b>`config`</b>: `Config` object.
+        - <b>`lib`</b>: The path to a shared library or one of `avx2`, `avx`, `basic`.
+        
         ---
         
         ##### <kbd>property</kbd> LLM.config
         
+        The config object.
+        
         ---
         
         ##### <kbd>property</kbd> LLM.model_path
         
+        The path to the model file.
+        
         ---
         
         ##### <kbd>property</kbd> LLM.model_type
         
+        The model type.
+        
         ---
         
         #### <kbd>method</kbd> `LLM.detokenize`
         
         ```python
-        detokenize(tokens: Union[Sequence[int], int]) → str
+        detokenize(tokens: Sequence[int]) → str
         ```
         
+        Converts a list of tokens to text.
+        
+        **Args:**
+        
+        - <b>`tokens`</b>: The list of tokens.
+        
+        **Returns:**
+        The combined text of all tokens.
+        
         ---
         
         #### <kbd>method</kbd> `LLM.eval`
         
         ```python
         eval(
             tokens: Sequence[int],
             batch_size: Optional[int] = None,
             threads: Optional[int] = None
         ) → None
         ```
         
+        Evaluates a list of tokens.
+        
+        **Args:**
+        
+        - <b>`tokens`</b>: The list of tokens to evaluate.
+        - <b>`batch_size`</b>: The batch size to use for evaluating tokens. Default: `8`
+        - <b>`threads`</b>: The number of threads to use for evaluating tokens. Default: `-1`
+        
         ---
         
         #### <kbd>method</kbd> `LLM.generate`
         
         ```python
         generate(
             tokens: Sequence[int],
@@ -256,30 +302,59 @@
             seed: Optional[int] = None,
             batch_size: Optional[int] = None,
             threads: Optional[int] = None,
             reset: Optional[bool] = None
         ) → Generator[int, NoneType, NoneType]
         ```
         
+        Generates new tokens from a list of tokens.
+        
+        **Args:**
+        
+        - <b>`tokens`</b>: The list of tokens to generate tokens from.
+        - <b>`top_k`</b>: The top-k value to use for sampling. Default: `40`
+        - <b>`top_p`</b>: The top-p value to use for sampling. Default: `0.95`
+        - <b>`temperature`</b>: The temperature to use for sampling. Default: `0.8`
+        - <b>`repetition_penalty`</b>: The repetition penalty to use for sampling. Default: `1.0`
+        - <b>`last_n_tokens`</b>: The number of last tokens to use for repetition penalty. Default: `64`
+        - <b>`seed`</b>: The seed value to use for sampling tokens. Default: `-1`
+        - <b>`batch_size`</b>: The batch size to use for evaluating tokens. Default: `8`
+        - <b>`threads`</b>: The number of threads to use for evaluating tokens. Default: `-1`
+        - <b>`reset`</b>: Whether to reset the model state before generating text. Default: `True`
+        
+        **Returns:**
+        The generated tokens.
+        
         ---
         
         #### <kbd>method</kbd> `LLM.is_eos_token`
         
         ```python
         is_eos_token(token: int) → bool
         ```
         
+        Checks if a token is an end-of-sequence token.
+        
+        **Args:**
+        
+        - <b>`token`</b>: The token to check.
+        
+        **Returns:**
+        `True` if the token is an end-of-sequence token else `False`.
+        
         ---
         
         #### <kbd>method</kbd> `LLM.reset`
         
         ```python
         reset() → None
         ```
         
+        Resets the model state.
+        
         ---
         
         #### <kbd>method</kbd> `LLM.sample`
         
         ```python
         sample(
             top_k: Optional[int] = None,
@@ -287,22 +362,45 @@
             temperature: Optional[float] = None,
             repetition_penalty: Optional[float] = None,
             last_n_tokens: Optional[int] = None,
             seed: Optional[int] = None
         ) → int
         ```
         
+        Samples a token from the model.
+        
+        **Args:**
+        
+        - <b>`top_k`</b>: The top-k value to use for sampling. Default: `40`
+        - <b>`top_p`</b>: The top-p value to use for sampling. Default: `0.95`
+        - <b>`temperature`</b>: The temperature to use for sampling. Default: `0.8`
+        - <b>`repetition_penalty`</b>: The repetition penalty to use for sampling. Default: `1.0`
+        - <b>`last_n_tokens`</b>: The number of last tokens to use for repetition penalty. Default: `64`
+        - <b>`seed`</b>: The seed value to use for sampling tokens. Default: `-1`
+        
+        **Returns:**
+        The sampled token.
+        
         ---
         
         #### <kbd>method</kbd> `LLM.tokenize`
         
         ```python
         tokenize(text: str) → List[int]
         ```
         
+        Converts a text into list of tokens.
+        
+        **Args:**
+        
+        - <b>`text`</b>: The text to tokenize.
+        
+        **Returns:**
+        The list of tokens.
+        
         ---
         
         #### <kbd>method</kbd> `LLM.__call__`
         
         ```python
         __call__(
             prompt: str,
@@ -311,18 +409,39 @@
             top_p: Optional[float] = None,
             temperature: Optional[float] = None,
             repetition_penalty: Optional[float] = None,
             last_n_tokens: Optional[int] = None,
             seed: Optional[int] = None,
             batch_size: Optional[int] = None,
             threads: Optional[int] = None,
+            stop: Optional[Sequence[str]] = None,
             reset: Optional[bool] = None
         ) → str
         ```
         
+        Generates text from a prompt.
+        
+        **Args:**
+        
+        - <b>`prompt`</b>: The prompt to generate text from.
+        - <b>`max_new_tokens`</b>: The maximum number of new tokens to generate. Default: `256`
+        - <b>`top_k`</b>: The top-k value to use for sampling. Default: `40`
+        - <b>`top_p`</b>: The top-p value to use for sampling. Default: `0.95`
+        - <b>`temperature`</b>: The temperature to use for sampling. Default: `0.8`
+        - <b>`repetition_penalty`</b>: The repetition penalty to use for sampling. Default: `1.0`
+        - <b>`last_n_tokens`</b>: The number of last tokens to use for repetition penalty. Default: `64`
+        - <b>`seed`</b>: The seed value to use for sampling tokens. Default: `-1`
+        - <b>`batch_size`</b>: The batch size to use for evaluating tokens. Default: `8`
+        - <b>`threads`</b>: The number of threads to use for evaluating tokens. Default: `-1`
+        - <b>`stop`</b>: A list of sequences to stop generation when encountered. Default: `None`
+        - <b>`reset`</b>: Whether to reset the model state before generating text. Default: `True`
+        
+        **Returns:**
+        The generated text.
+        
         <!-- API_DOCS -->
         
         ## License
         
         [MIT](https://github.com/marella/ctransformers/blob/main/LICENSE)
         
 Keywords: ctransformers transformers ai llm
```

### Comparing `ctransformers-0.1.0/ctransformers.egg-info/SOURCES.txt` & `ctransformers-0.1.1/ctransformers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ctransformers-0.1.0/setup.py` & `ctransformers-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md') as f:
     long_description = f.read()
 
 name = 'ctransformers'
 
 setup(
     name=name,
-    version='0.1.0',
+    version='0.1.1',
     description=
     'Python bindings for the Transformer models implemented in C/C++ using GGML library.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ravindra Marella',
     author_email='mv.ravindra007@gmail.com',
     url='https://github.com/marella/{}'.format(name),
```

