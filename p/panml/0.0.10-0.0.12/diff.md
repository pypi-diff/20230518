# Comparing `tmp/panml-0.0.10.tar.gz` & `tmp/panml-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panml-0.0.10.tar", last modified: Wed May 17 11:35:21 2023, max compression
+gzip compressed data, was "panml-0.0.12.tar", last modified: Thu May 18 10:57:20 2023, max compression
```

## Comparing `panml-0.0.10.tar` & `panml-0.0.12.tar`

### file list

```diff
@@ -1,8 +1,16 @@
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-17 11:35:21.287263 panml-0.0.10/
--rw-r--r--   0 williamzheng   (501) staff       (20)     1424 2023-05-17 11:35:21.287378 panml-0.0.10/PKG-INFO
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-17 11:35:21.287212 panml-0.0.10/panml/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-02 06:31:00.248295 panml-0.0.10/panml/__init__.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    23754 2023-05-17 11:25:28.807370 panml-0.0.10/panml/models.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     7024 2023-05-16 08:12:47.828416 panml-0.0.10/panml/search.py
--rw-r--r--   0 williamzheng   (501) staff       (20)       39 2023-05-15 13:51:34.871217 panml-0.0.10/setup.cfg
--rw-r--r--   0 williamzheng   (501) staff       (20)     2407 2023-05-17 11:32:56.774669 panml-0.0.10/setup.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-18 10:57:20.407988 panml-0.0.12/
+-rw-r--r--   0 williamzheng   (501) staff       (20)     1063 2023-05-11 06:11:04.000000 panml-0.0.12/LICENSE
+-rw-r--r--   0 williamzheng   (501) staff       (20)     1555 2023-05-18 10:57:20.408161 panml-0.0.12/PKG-INFO
+-rw-r--r--   0 williamzheng   (501) staff       (20)     5031 2023-05-14 05:40:36.000000 panml-0.0.12/README.md
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-18 10:57:20.405510 panml-0.0.12/panml/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-02 06:31:00.000000 panml-0.0.12/panml/__init__.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    27685 2023-05-18 09:03:21.000000 panml-0.0.12/panml/models.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     9713 2023-05-18 09:03:21.000000 panml-0.0.12/panml/search.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-18 10:57:20.407701 panml-0.0.12/panml.egg-info/
+-rw-r--r--   0 williamzheng   (501) staff       (20)     1555 2023-05-18 10:57:20.000000 panml-0.0.12/panml.egg-info/PKG-INFO
+-rw-r--r--   0 williamzheng   (501) staff       (20)      230 2023-05-18 10:57:20.000000 panml-0.0.12/panml.egg-info/SOURCES.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)        1 2023-05-18 10:57:20.000000 panml-0.0.12/panml.egg-info/dependency_links.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)      196 2023-05-18 10:57:20.000000 panml-0.0.12/panml.egg-info/requires.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)        6 2023-05-18 10:57:20.000000 panml-0.0.12/panml.egg-info/top_level.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)       79 2023-05-18 10:57:20.409018 panml-0.0.12/setup.cfg
+-rw-r--r--   0 williamzheng   (501) staff       (20)     2612 2023-05-18 10:57:12.000000 panml-0.0.12/setup.py
```

### Comparing `panml-0.0.10/PKG-INFO` & `panml-0.0.12/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,28 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: panml
-Version: 0.0.10
+Version: 0.0.12
 Summary: PanML is a generative AI/ML development toolkit designed for ease of use and fast experimentation.
 Home-page: https://github.com/Pan-ML/panml
 Author: PanML team
 Author-email: williamxn.z@gmail.com
 License: MIT
-Description: PanML aims to make analysis and experimentation of generative AI/ML models more accessible, by providing a simple and consistent interface to foundation models for Data Scientists, Machine Learning Engineers and Software Developers.                       The package provides various assistive tools to work with generative language models, such as prompt engineering, fine tuning and others.                       
-        
-        Quick start guide: https://github.com/Pan-ML/panml/wiki/1.-Quick-start-guide                       
-        
-        Documentation/Wiki: https://github.com/Pan-ML/panml/wiki
 Keywords: generative AI,generative model,machine learning,large language model,LLM,prompt engineering,fine tuning,prompt tuning,retrieval augmentation,AI safety,AI alignment
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+License-File: LICENSE
+
+PanML aims to make analysis and experimentation of generative AI/ML models more accessible, by providing a simple and consistent interface to foundation models for Data Scientists, Machine Learning Engineers and Software Developers.                       The package provides various assistive tools to work with generative language models, such as prompt engineering, fine tuning and others.                       
+
+Quick start guide: https://github.com/Pan-ML/panml/wiki/1.-Quick-start-guide                       
+
+Documentation/Wiki: https://github.com/Pan-ML/panml/wiki
+
```

### Comparing `panml-0.0.10/panml/models.py` & `panml-0.0.12/panml/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from transformers import AutoModelForCausalLM, AutoModelForSeq2SeqLM, AutoTokenizer
 from transformers import TrainingArguments, Trainer, Seq2SeqTrainer, DataCollatorForLanguageModeling, DataCollatorForSeq2Seq
 import openai
 
 # HuggingFace model class
 class HuggingFaceModelPack:
     '''
-    Generic HuggingFace Hub model pack class
+    HuggingFace Hub model pack class
     '''
     # Initialize class variables
     def __init__(self, model: str, input_block_size: int, padding_length: int, tokenizer_batch: bool, source: str) -> None:
         if source == 'huggingface':
             if 'flan' in model:
                 self.model_hf = AutoModelForSeq2SeqLM.from_pretrained(model)
             else:
@@ -39,14 +39,23 @@
                                    'output_dir', 'logging_dir', 'save_model']
         
         if self.tokenizer.pad_token is None:
             self.tokenizer.pad_token = self.model_hf.config.eos_token_id
     
     # Embed text
     def embedding(self, text: str) -> torch.Tensor:
+        '''
+        Gets the embedding of the text using open source collections of models from HuggingFace Hub
+
+        Args:
+        text: text of the input
+
+        Returns:
+        torch tensor containing the embedding array
+        '''
         token_ids = self.tokenizer.encode(text, return_tensors='pt')
         
         # # Get embeddings
         # if 'flan' in self.model_hf.name_or_path: 
         #     emb = self.model_hf.shared.weight[token_ids[0]] # embeddings for FLAN
         # else: 
         #     emb = self.model_hf.transformer.wte.weight[token_ids[0]] # embeddings for GPT2
@@ -63,15 +72,30 @@
     
     # Generate text
     def predict(self, text: str, max_length: int=50, skip_special_tokens: bool=True, 
                 display_probability: bool=False, num_return_sequences: int=1, temperature: float=0.8, 
                 top_p: float=0.8, top_k: int=0, no_repeat_ngram_size: int=3) -> dict[str, str]:
         '''
         Generates output by prompting a language model from HuggingFace Hub
-        Returns: dict of generated text (text), and token probabilities (probability) and perplexity scores (perplexity) if available
+
+        Args:
+        text: text of the prompt
+        max_length: parameter from HuggingFace Hub, specifies the max length of tokens generated
+        skip_special_tokens: parameter from HuggingFace Hub, specifies whether or not to remove special tokens in the decoding
+        display_probability: show probability of the generated tokens
+        num_return_sequences: parameter from HuggingFace Hub, specifies the number of independently computed returned sequences for each element in the batch
+        temperature: parameter from HuggingFace Hub, specifies the value used to modulate the next token probabilities
+        top_p: parameter from HuggingFace Hub, if set to float < 1, only the smallest set of most probable tokens with probabilities that add up to top_p or higher are kept for generation
+        no_repeat_ngram_size: parameter from HuggingFace Hub, ff set to int > 0, all ngrams of that size can only occur once
+
+        Returns: 
+        dict containing: 
+        text: generated text
+        probability: token probabilities if available
+        perplexity: perplexity score if available
         '''
         # Catch input exceptions
         if not isinstance(text, str):
             raise TypeError('Input text needs to be of type: string')
             
         output_context = {
             'text': None,
@@ -124,15 +148,24 @@
         return tokenized_dataset
     
     # Model training
     def fit(self, x: list[str], y: list[str], train_args: dict[str, Union[str, int, float]]={}, 
             instruct: bool=False, num_proc=4) -> None:
         '''
         Fine tuning of a language model from HuggingFace Hub
-        Returns: None. Trained model is saved in the .result/ folder with name "model_" prepended to the specified title
+
+        Args:
+        x: list of example text for training/fine tuning the language model
+        y: list of example text as targets for training/fine tuning the language model. 
+        Note: For autogressive based training, this parameter is set to be same as x. For instruct based training, this parameter is part of the target examples for supervised fine tuning.
+        train_args: parameters to be fed into HuggingFace Hub's training_args dict, as required for training
+        num_proc: parameter from HuggingFace Hub, specifies max number of processes when generating cache. Already cached shards are loaded sequentially
+
+        Returns: 
+        None. Trained model is saved in the .result/ folder with name "model_" prepended to the specified title
         '''
         # Catch input exceptions
         if not isinstance(x, list):
             raise TypeError('Input data array, x, needs to be of type: list')
         if not isinstance(y, list):
             raise TypeError('Input data array, y, needs to be of type: list')
         if not isinstance(train_args, dict):
@@ -201,15 +234,15 @@
         
         if train_args['save_model']:
             trainer.save_model(f'./results/model_{train_args["title"]}') # Save trained model
     
 # OpenAI model class
 class OpenAIModelPack:
     '''
-    Generic OpenAI model pack class
+    OpenAI model pack class
     '''
     def __init__(self, model: str, api_key: str) -> None:
         self.model = model
         self.model_embedding = 'text-embedding-ada-002'
         openai.api_key = api_key
     
     # Generate text of single model call
@@ -278,16 +311,35 @@
     # Generate text in prompt loop
     def predict(self, text: str, temperature: float=0, max_tokens: int=100, top_p: float=1, n: int=3, 
                 frequency_penalty: float=0, presence_penalty: float=0, display_probability: bool=False, logprobs: int=1, 
                 prompt_modifier: list[dict[str, str]]=[{'prepend': '', 'append': ''}], keep_last: bool=True, 
                 chat_role: str='user') -> dict[str, str]:
         '''
         Generates output by prompting a language model from OpenAI
-        Returns: dict of generated text (text), and token probabilities (probability) and perplexity scores (perplexity) if available
-        Note: probability and peplexity scores are not calculated for gpt-3.5-turbo models
+        
+        Args:
+        text: text of the prompt
+        temperature: temperature of the generated text (for further details please refer to this topic covered in language model text generation)
+        max_tokens: max number of tokens to be generated from OpenAI API
+        top_p: max number of tokens to be generated from OpenAI API
+        n: parameter from OpenAI API (for further details please refer to this topic covered in language model text generation)
+        frequency_penalty: parameter from OpenAI API (for further details please refer to this topic covered in language model text generation)
+        presence_penalty: parameter from OpenAI API (for further details please refer to this topic covered in language model text generation)
+        display_probability: show probability of the generated tokens
+        logprobs: parameter from OpenAI API (for further details please refer to this topic covered in language model text generation)
+        prompt_modifier: list of prompts to be added in the context of multi-stage prompt chaining
+        keep_last: keep or discard the history of responses from the mulit-stage prompt chaining
+        chat_role: parameter from OpenAI API, specifies the role of the LLM assistant. Currently this is available for models of gpt-3.5-turbo or above (for further details please refer to this topic covered in language model text generation)
+
+        Returns: 
+        dict containing: 
+        text: generated text
+        probability: token probabilities if available
+        perplexity: perplexity score if available
+        Note: probability and peplexity scores are calculated only for some OpenAI models in this package
         '''
         # Catch input exceptions
         if not isinstance(text, str):
             raise TypeError('Input text needs to be of type: string')
         if not isinstance(prompt_modifier, list):
             raise TypeError('Input prompt modifier needs to be of type: list')
         if not isinstance(chat_role, str):
@@ -316,27 +368,37 @@
             # Terminate loop for next prompt when context contains no meaningful words (less than 2)
             response_words = output_context['text'].replace('\n', '').replace(' ', '')
             if len(response_words) < 2:
                 break
 
             history.append(output_context)
         
-        if keep_last:
-            return history[-1] # returns last prediction output
-        else:
-            return history # returns all historical prediction output
+        try:
+            if keep_last:
+                return history[-1] # returns last prediction output
+            else:
+                return history # returns all historical prediction output
+        except:
+            return {'text': None} # if there is invalid response from the language model, return None
         
     # Generate and execute code using (LM powered function)
     def predict_code(self, text: str, x: Union[int, float, str, pd.DataFrame], variable_names: dict[str, str]={'input': 'x', 'output': 'y'}, 
                      language: str='python', max_tokens: int=500) -> str:
         '''
         Generates code output by prompting a language model from OpenAI with a constrained command that is specific for code generation.
-        Input variables can be a value, or a pandas dataframe
-        Variable names are passed into the prompt context to allow the generated code to contain the specified variable names.
-        Returns: text of generated code
+        
+        Args:
+        text: text of the prompt
+        x: input variable, can be a value or pandas dataframe
+        variable_names: input variable name, and output variable name of the generated code
+        langauge: programming language of the code to be generated
+        max_tokens: max number of tokens to be generated from OpenAI API
+   
+        Returns: 
+        text of generated code
         '''
         # Catch input exceptions
         if self.model != 'text-davinci-002' and self.model != 'text-davinci-003':
             raise ValueError(f"The specified model is '{self.model}'. Only 'text-davinci-002' and 'text-davinci-002' are supported in this package for code generation")
         if not isinstance(text, str):
             raise TypeError('Input text needs to be of type: string')
         if not isinstance(x, int) and not isinstance(x, float) and \
@@ -366,14 +428,24 @@
         output_context = self.predict(f'{prompt_prepend} {text} {prompt_append}', max_tokens=max_tokens) # Get predicted code snippet
         code_context = f"{input_arg_context}\n{output_context['text']}" # Create code context
 
         return code_context
         
     # Embed text
     def embedding(self, text: str, model: str=None) -> list[float]:
+        '''
+        Gets the embedding of the text using OpenAI language models
+
+        Args:
+        text: text of the input
+        model: name of the OpenAI language model (if not already provided when the class is instantiated)
+
+        Returns:
+        list containing the embedding array
+        '''
         text = text.replace("\n", " ")
         if model is None:
             model = self.model_embedding          
         emb = openai.Embedding.create(input=[text], model=model)['data'][0]['embedding']
         
         return emb
```

### Comparing `panml-0.0.10/setup.py` & `panml-0.0.12/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-
-from distutils.core import setup
+from setuptools import setup, find_packages
 setup(
   name = 'panml', # package name     
-  packages = ['panml'], # package name
-  version = '0.0.10', # version
+  packages = find_packages(exclude=['test']), # package name
+  version = '0.0.12', # version
   license = 'MIT', # license
   description = 'PanML is a generative AI/ML development toolkit designed for ease of use and fast experimentation.', # short description about the package
   long_description = 'PanML aims to make analysis and experimentation of generative AI/ML models more accessible, by providing a simple and consistent interface to foundation models for Data Scientists, Machine Learning Engineers and Software Developers. \
                       The package provides various assistive tools to work with generative language models, such as prompt engineering, fine tuning and others. \
                       \n\nQuick start guide: https://github.com/Pan-ML/panml/wiki/1.-Quick-start-guide \
                       \n\nDocumentation/Wiki: https://github.com/Pan-ML/panml/wiki', # long description
   author = 'PanML team', # team name
@@ -15,15 +14,15 @@
   url = 'https://github.com/Pan-ML/panml', # url link
   # download_url = 'https://github.com/Pan-ML/panml/archive/refs/tags/v0.0.9.tar.gz', # set a release on GitHub (with release tag) -> Assets -> right click and copy the link
   keywords = ['generative AI', 'generative model', 'machine learning', 'large language model', # keywords
               'LLM', 'prompt engineering', 'fine tuning', 'prompt tuning', 'retrieval augmentation', 
               'AI safety', 'AI alignment'], 
   install_requires=[  # dependencies
         'huggingface-hub>=0.14.1',
-        'numpy>=1.24.3',
+        'numpy>=1.22.4',
         'openai>=0.27.6',
         'pandas>=2.0.1',
         'tokenizers>=0.13.3',
         'datasets>=2.12.0',
         'torch>=2.0.0',
         'tqdm>=4.65.0',
         'transformers>=4.29.1',
@@ -32,11 +31,14 @@
       ],
   classifiers=[
     'Development Status :: 4 - Beta', # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of the package
     'Intended Audience :: Developers', # Define the audience type
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License', # license
     'Programming Language :: Python :: 3', # Specify supported Python versions
+    'Programming Language :: Python :: 3.7', # Specify supported Python versions
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
   ],
 )
```

