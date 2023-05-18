# Comparing `tmp/pop-ml-0.1.1.tar.gz` & `tmp/pop-ml-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pop-ml-0.1.1.tar", last modified: Thu May 11 23:46:11 2023, max compression
+gzip compressed data, was "pop-ml-0.2.0.tar", last modified: Thu May 18 17:34:11 2023, max compression
```

## Comparing `pop-ml-0.1.1.tar` & `pop-ml-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 23:46:11.622382 pop-ml-0.1.1/
--rw-r--r--   0 root         (0) root         (0)    11342 2023-05-11 23:45:56.000000 pop-ml-0.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5835 2023-05-11 23:46:11.622382 pop-ml-0.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4828 2023-05-11 23:45:56.000000 pop-ml-0.1.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 23:46:11.622382 pop-ml-0.1.1/pop_ml/
--rw-r--r--   0 root         (0) root         (0)     1287 2023-05-11 23:45:56.000000 pop-ml-0.1.1/pop_ml/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 23:46:11.622382 pop-ml-0.1.1/pop_ml/ml/
--rw-r--r--   0 root         (0) root         (0)      823 2023-05-11 23:45:56.000000 pop-ml-0.1.1/pop_ml/ml/dataset.py
--rw-r--r--   0 root         (0) root         (0)     1301 2023-05-11 23:45:56.000000 pop-ml-0.1.1/pop_ml/ml/init.py
--rw-r--r--   0 root         (0) root         (0)     3889 2023-05-11 23:45:56.000000 pop-ml-0.1.1/pop_ml/ml/tokenizer.py
--rw-r--r--   0 root         (0) root         (0)      135 2023-05-11 23:45:56.000000 pop-ml-0.1.1/pop_ml/scripts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 23:46:11.622382 pop-ml-0.1.1/pop_ml/token/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 23:46:11.622382 pop-ml-0.1.1/pop_ml/token/contracts/
--rw-r--r--   0 root         (0) root         (0)      277 2023-05-11 23:45:56.000000 pop-ml-0.1.1/pop_ml/token/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)      410 2023-05-11 23:45:56.000000 pop-ml-0.1.1/pop_ml/token/init.py
--rw-r--r--   0 root         (0) root         (0)       63 2023-05-11 23:45:56.000000 pop-ml-0.1.1/pop_ml/token/python_keywords.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-11 23:46:11.000000 pop-ml-0.1.1/pop_ml/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 23:46:11.622382 pop-ml-0.1.1/pop_ml.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5835 2023-05-11 23:46:11.000000 pop-ml-0.1.1/pop_ml.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      416 2023-05-11 23:46:11.000000 pop-ml-0.1.1/pop_ml.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 23:46:11.000000 pop-ml-0.1.1/pop_ml.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-05-11 23:46:11.000000 pop-ml-0.1.1/pop_ml.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-11 23:46:11.000000 pop-ml-0.1.1/pop_ml.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-11 23:46:11.000000 pop-ml-0.1.1/pop_ml.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-11 23:46:11.622382 pop-ml-0.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2983 2023-05-11 23:45:56.000000 pop-ml-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 17:34:11.267758 pop-ml-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)    11342 2023-05-18 17:33:56.000000 pop-ml-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6013 2023-05-18 17:34:11.267758 pop-ml-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4858 2023-05-18 17:33:56.000000 pop-ml-0.2.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 17:34:11.267758 pop-ml-0.2.0/pop_ml/
+-rw-r--r--   0 root         (0) root         (0)     1456 2023-05-18 17:33:56.000000 pop-ml-0.2.0/pop_ml/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 17:34:11.267758 pop-ml-0.2.0/pop_ml/ml/
+-rw-r--r--   0 root         (0) root         (0)      826 2023-05-18 17:33:56.000000 pop-ml-0.2.0/pop_ml/ml/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1634 2023-05-18 17:33:56.000000 pop-ml-0.2.0/pop_ml/ml/init.py
+-rw-r--r--   0 root         (0) root         (0)     4214 2023-05-18 17:33:56.000000 pop-ml-0.2.0/pop_ml/ml/tokenizer.py
+-rw-r--r--   0 root         (0) root         (0)      393 2023-05-18 17:33:56.000000 pop-ml-0.2.0/pop_ml/scripts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 17:34:11.267758 pop-ml-0.2.0/pop_ml/token/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 17:34:11.267758 pop-ml-0.2.0/pop_ml/token/contracts/
+-rw-r--r--   0 root         (0) root         (0)      386 2023-05-18 17:33:56.000000 pop-ml-0.2.0/pop_ml/token/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)      757 2023-05-18 17:33:56.000000 pop-ml-0.2.0/pop_ml/token/init.py
+-rw-r--r--   0 root         (0) root         (0)     1817 2023-05-18 17:33:56.000000 pop-ml-0.2.0/pop_ml/token/python_keywords.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-18 17:34:10.000000 pop-ml-0.2.0/pop_ml/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 17:34:11.267758 pop-ml-0.2.0/pop_ml.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6013 2023-05-18 17:34:11.000000 pop-ml-0.2.0/pop_ml.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      416 2023-05-18 17:34:11.000000 pop-ml-0.2.0/pop_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 17:34:11.000000 pop-ml-0.2.0/pop_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-05-18 17:34:11.000000 pop-ml-0.2.0/pop_ml.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-18 17:34:11.000000 pop-ml-0.2.0/pop_ml.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-18 17:34:11.000000 pop-ml-0.2.0/pop_ml.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-18 17:34:11.271758 pop-ml-0.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3406 2023-05-18 17:33:56.000000 pop-ml-0.2.0/setup.py
```

### Comparing `pop-ml-0.1.1/LICENSE` & `pop-ml-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pop-ml-0.1.1/PKG-INFO` & `pop-ml-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: pop-ml
-Version: 0.1.1
+Version: 0.2.0
 Summary: Machine learning library for pop projects
-Home-page: https://gitlab.com/vmware/pop/pop-ml
+Home-page: https://vmware.gitlab.io/pop/pop-ml/en/latest/index.html
 Author: VMWare, Inc.
 Author-email: idemproject@vmware.com
 License: Apache Software License 2.0
+Project-URL: Code, https://gitlab.com/vmware/pop/pop-ml
+Project-URL: Issue tracker, https://gitlab.com/vmware/pop/pop-ml/issues
 Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
@@ -28,37 +30,38 @@
 pop-ml
 ======
 
 .. image:: https://img.shields.io/badge/made%20with-pop-teal
    :alt: Made with pop, a Python implementation of Plugin Oriented Programming
    :target: https://pop.readthedocs.io/
 
+.. image:: https://img.shields.io/badge/docs%20on-GitLab%20Pages-blue
+   :alt: Documentation is published with Sphinx on GitLab Pages
+   :target: https://vmware.gitlab.io/pop/pop-ml/en/latest/index.html
+
 .. image:: https://img.shields.io/badge/made%20with-python-yellow
    :alt: Made with Python
    :target: https://www.python.org/
 
 
-pop-ml is a Python library that simplifies the integration of AI-powered translation
-capabilities into any Python project.  It leverages Hugging Face Transformers and pretrained
-tokenizers to provide an accessible translation experience. pop-ml aims to offer a
-straightforward API for translating strings in Python code, ensuring compatibility with
-widely-used projects.
+``pop-ml`` is a Python library that simplifies the integration of AI-powered
+capabilities into any POP-based Python project.
 
 About
 =====
 
+``pop-ml`` is a comprehensive Python library designed to facilitate the integration of AI-
+powered capabilities, such as translation, into POP-based Python projects.
+
+``pop-ml`` currently provides developers with an easy-to-use and seamless translation experience, allowing them
+to translate strings to other languages, such as english to spanish.
 
-pop-ml is a comprehensive Python library designed to facilitate the integration of AI-
-powered translation capabilities into Python projects. The primary goal of pop-ml is to
-provide developers with an easy-to-use and seamless translation experience, allowing them
-to translate strings in their Python code to any language.
-
-The library is built on top of the Hugging Face Transformers library and utilizes pretrained
-tokenizers to deliver accurate and efficient translations. By leveraging state-of-the-art
-language models, pop-ml ensures high-quality translations while maintaining simplicity in
+The library currently supports making use of Hugging Face Transformers library and can utilize pretrained
+tokenizers for delivering accurate and efficient translations. By leveraging state-of-the-art
+language models, ``pop-ml`` ensures high-quality translations while maintaining simplicity in
 its API.
 
 
 What is POP?
 ------------
 
 This project is built with `pop <https://pop.readthedocs.io/>`__, a Python-based
@@ -92,26 +95,26 @@
 
 If wanting to use ``pop-ml``, you can do so by either
 installing from PyPI or from source.
 
 Install from PyPI
 +++++++++++++++++
 
-To install pop-ml from PyPI, simply run the following command:
+To install ``pop-ml`` from PyPI, simply run the following command:
 
 .. code-block:: bash
 
     pip install pop-ml
 
-This will install the latest version of pop-ml, along with all required dependencies.
+This will install the latest version of ``pop-ml``, along with all required dependencies.
 
 Install from source
 +++++++++++++++++++
 
-To install pop-ml from source, first clone the repository from GitLab:
+To install ``pop-ml`` from source, first clone the repository from GitLab:
 
 .. code-block:: bash
 
     git clone https://gitlab.com/vmware/pop/pop-ml.git
 
 Next, navigate to the cloned repository directory:
 
@@ -124,21 +127,21 @@
 .. code-block:: bash
 
     pip install .
 
 Usage
 =====
 
-pop-ml can be used both as a command-line tool (pop-translate) and as a Python library.
-Below are examples of how to use pop-ml in both ways.
+``pop-ml`` can be used both as a command-line tool (``pop-translate``) and as a Python library.
+Below are examples of how to use ``pop-ml`` in both ways.
 
 CLI Examples
 ------------
 
-To use the pop-translate command-line tool, you can pass the text you want to translate as
+To use the ``pop-translate`` command-line tool, you can pass the text you want to translate as
 an argument, along with any additional options:
 
 .. code-block:: bash
 
     pop-translate "Hello, World!" --translate-to es
 
 This command will translate the input text "Hello, world!" from English (en) to Spanish (es).
```

### Comparing `pop-ml-0.1.1/README.rst` & `pop-ml-0.2.0/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -2,37 +2,38 @@
 pop-ml
 ======
 
 .. image:: https://img.shields.io/badge/made%20with-pop-teal
    :alt: Made with pop, a Python implementation of Plugin Oriented Programming
    :target: https://pop.readthedocs.io/
 
+.. image:: https://img.shields.io/badge/docs%20on-GitLab%20Pages-blue
+   :alt: Documentation is published with Sphinx on GitLab Pages
+   :target: https://vmware.gitlab.io/pop/pop-ml/en/latest/index.html
+
 .. image:: https://img.shields.io/badge/made%20with-python-yellow
    :alt: Made with Python
    :target: https://www.python.org/
 
 
-pop-ml is a Python library that simplifies the integration of AI-powered translation
-capabilities into any Python project.  It leverages Hugging Face Transformers and pretrained
-tokenizers to provide an accessible translation experience. pop-ml aims to offer a
-straightforward API for translating strings in Python code, ensuring compatibility with
-widely-used projects.
+``pop-ml`` is a Python library that simplifies the integration of AI-powered
+capabilities into any POP-based Python project.
 
 About
 =====
 
+``pop-ml`` is a comprehensive Python library designed to facilitate the integration of AI-
+powered capabilities, such as translation, into POP-based Python projects.
+
+``pop-ml`` currently provides developers with an easy-to-use and seamless translation experience, allowing them
+to translate strings to other languages, such as english to spanish.
 
-pop-ml is a comprehensive Python library designed to facilitate the integration of AI-
-powered translation capabilities into Python projects. The primary goal of pop-ml is to
-provide developers with an easy-to-use and seamless translation experience, allowing them
-to translate strings in their Python code to any language.
-
-The library is built on top of the Hugging Face Transformers library and utilizes pretrained
-tokenizers to deliver accurate and efficient translations. By leveraging state-of-the-art
-language models, pop-ml ensures high-quality translations while maintaining simplicity in
+The library currently supports making use of Hugging Face Transformers library and can utilize pretrained
+tokenizers for delivering accurate and efficient translations. By leveraging state-of-the-art
+language models, ``pop-ml`` ensures high-quality translations while maintaining simplicity in
 its API.
 
 
 What is POP?
 ------------
 
 This project is built with `pop <https://pop.readthedocs.io/>`__, a Python-based
@@ -66,26 +67,26 @@
 
 If wanting to use ``pop-ml``, you can do so by either
 installing from PyPI or from source.
 
 Install from PyPI
 +++++++++++++++++
 
-To install pop-ml from PyPI, simply run the following command:
+To install ``pop-ml`` from PyPI, simply run the following command:
 
 .. code-block:: bash
 
     pip install pop-ml
 
-This will install the latest version of pop-ml, along with all required dependencies.
+This will install the latest version of ``pop-ml``, along with all required dependencies.
 
 Install from source
 +++++++++++++++++++
 
-To install pop-ml from source, first clone the repository from GitLab:
+To install ``pop-ml`` from source, first clone the repository from GitLab:
 
 .. code-block:: bash
 
     git clone https://gitlab.com/vmware/pop/pop-ml.git
 
 Next, navigate to the cloned repository directory:
 
@@ -98,21 +99,21 @@
 .. code-block:: bash
 
     pip install .
 
 Usage
 =====
 
-pop-ml can be used both as a command-line tool (pop-translate) and as a Python library.
-Below are examples of how to use pop-ml in both ways.
+``pop-ml`` can be used both as a command-line tool (``pop-translate``) and as a Python library.
+Below are examples of how to use ``pop-ml`` in both ways.
 
 CLI Examples
 ------------
 
-To use the pop-translate command-line tool, you can pass the text you want to translate as
+To use the ``pop-translate`` command-line tool, you can pass the text you want to translate as
 an argument, along with any additional options:
 
 .. code-block:: bash
 
     pop-translate "Hello, World!" --translate-to es
 
 This command will translate the input text "Hello, world!" from English (en) to Spanish (es).
```

### Comparing `pop-ml-0.1.1/pop_ml/conf.py` & `pop-ml-0.2.0/pop_ml/conf.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,20 @@
-# https://pop.readthedocs.io/en/latest/tutorial/quickstart.html#adding-configuration-data
+"""POP project configuration data.
+
+``conf.py`` defines:
+
+* How the CLI args are presented
+* All configuration defaults
+* Help documentation
+* And more
+
+Resources:
+
+* `Intro to pop-config`<https://pop-config.readthedocs.io/en/latest/topics/introduction.html>__
+"""
 
 CONFIG = {
     "config": {
         "default": None,
         "help": "Load extra options from a configuration file onto hub.OPT.ml",
     },
     "source_lang": {
@@ -28,13 +40,13 @@
 }
 
 SUBCOMMANDS = {}
 
 CLI_CONFIG = {
     "config": {"options": ["-c"]},
     "source_lang": {"options": ["--translate-from"]},
-    "dest_lang": {"options": ["-T", "--translate-to"]},
+    "dest_lang": {"options": ["--translate-to"]},
     "model_name": {},
     "input_text": {"positional": True},
 }
 
 DYNE = {"ml": ["ml"], "token": ["token"]}
```

### Comparing `pop-ml-0.1.1/pop_ml/ml/dataset.py` & `pop-ml-0.2.0/pop_ml/ml/dataset.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,29 @@
-from typing import Callable
-from typing import Optional
+"""Create and work with datasets."""
+from typing import Callable, Optional
 
 from datasets import Dataset
 
 
 def create_from_generator(
     hub,
     generator: Callable,
     gen_kwargs: Optional[dict] = None,
 ):
-    """
-    Create a new dataset from a custom generator
-    """
+    """Create a new dataset from a custom generator."""
     return Dataset.from_generator(generator, gen_kwargs=gen_kwargs)
 
 
 def pre_process(
     hub,
     dataset: Dataset,
     pre_process_func: Callable,
     pre_process_func_kwargs: Optional[dict] = None,
     format_type: str = "torch",
-    columns: list = [],
+    columns: list = None,
 ):
-    """
-    Pre-process dataset such as tokenization, augmentation or re-sampling using custom processor
-    """
+    """Pre-process dataset such as tokenization, augmentation or re-sampling using custom processor."""
     dataset = dataset.map(
         function=pre_process_func, fn_kwargs=pre_process_func_kwargs, batched=True
     )
     dataset.set_format(type=format_type, columns=columns)
     return dataset
```

### Comparing `pop-ml-0.1.1/pop_ml/ml/init.py` & `pop-ml-0.2.0/pop_ml/ml/init.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,41 @@
-def __init__(hub):
+"""Creates the structure for the entire project."""
+
+
+def __virtual__(hub):  # noqa N807
+    """Ensure that pop-ml's config options get considered as early as possible."""
+    hub.pop.sub.add(dyne_name="config")
+    # Ensure that pop_ml's config gets loaded
+    hub.config.LOAD.insert(0, "pop_ml")
+    return True
+
+
+def __init__(hub):  # noqa N807
+    """Add all of the subs used by pop-ml to the hub."""
     # Perform python imports for the whole project
     hub.pop.sub.add(dyne_name="lib")
+    hub.pop.sub.add(python_import="re", sub=hub.lib)
     hub.pop.sub.add(python_import="transformers", sub=hub.lib)
     hub.pop.sub.add(python_import="dict_tools.data", sub=hub.lib, subname="dtd")
 
     # Add subsystems that are used by pop_ml
-    hub.pop.sub.add(dyne_name="config")
     hub.pop.sub.add(dyne_name="token")
 
-    # Ensure that pop_ml is always loaded onto the config
-    hub.config.LOAD.append("pop_ml")
-
 
 def cli(hub):
-    hub.pop.config.load(hub.config.LOAD, cli="pop_ml")
+    """Setup the project for use by CLI."""
+    hub.pop.config.load(["pop_ml"], cli="pop_ml")
 
     hub.pop.loop.create()
 
     hub.ml.init.run()
 
 
 def run(hub):
-    """
-    This is the entrypoint for the pop-ml cli tool called "pop-translate"
-    """
+    """This is the entrypoint for the pop-ml cli tool called "pop-translate"."""
     # Initialize the tokenizer from config options
     hub.ml.tokenizer.init(
         model_name=hub.OPT.pop_ml.model_name,
         dest_lang=hub.OPT.pop_ml.dest_lang,
         source_lang=hub.OPT.pop_ml.source_lang,
         pretrained_model=hub.OPT.pop_ml.pretrained_model_class,
         pretrained_tokenizer=hub.OPT.pop_ml.pretrained_tokenizer_class,
```

### Comparing `pop-ml-0.1.1/pop_ml/ml/tokenizer.py` & `pop-ml-0.2.0/pop_ml/ml/tokenizer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
+"""Utility to consume a configured tokenizer."""
 from typing import List
 
 import transformers
 
 
-def __init__(hub):
+def __init__(hub):  # noqa: N807
+    """Adding global variables used by this module to the hub."""
     hub.ml.MODEL_NAME = None
     hub.ml.MODEL = None
     hub.ml.TOKENIZER = None
 
 
 def init(
     hub,
     model_name: str = None,
     dest_lang: str = None,
     source_lang: str = None,
     pretrained_model: str = None,
     pretrained_tokenizer: str = None,
 ):
-    """
-    Idempotently initialize the global model and tokenizer
-    """
+    """Idempotently initialize the global model and tokenizer."""
     if hub.ml.MODEL_NAME and hub.ml.MODEL and hub.ml.TOKENIZER:
         # Global initialization is already complete
         return
 
     ret = hub.ml.tokenizer.get(
         model_name=model_name,
         source_lang=source_lang,
@@ -46,46 +46,49 @@
     hub,
     model_name: str = None,
     dest_lang: str = None,
     source_lang: str = None,
     pretrained_model: str = None,
     pretrained_tokenizer: str = None,
 ):
-    """
-    Get a tokenizer based on the given parameters and return it
-    """
+    """Get a tokenizer based on the given parameters and return it."""
     if model_name is None and not (source_lang and dest_lang):
         # Use the global model name
         model_name = hub.ml.MODEL_NAME
     elif not (source_lang and dest_lang):
-        raise ValueError(f"Both a source_lang and dest_lang must be specified")
+        msg = "Both a source_lang and dest_lang must be specified"
+        raise ValueError(msg)
     else:
         # Use the default Hugging Face translation model using the given source and dest languages
         model_name = f"Helsinki-NLP/opus-mt-{source_lang}-{dest_lang}"
 
-    hub.log.debug(f"Using model: {model_name}")
+    hub.log.trace(f"Using model: {model_name}")
 
     model = getattr(hub.lib.transformers, pretrained_model).from_pretrained(model_name)
-    hub.log.debug(f"Initialized pretrained model: {model}")
+    hub.log.trace(f"Initialized pretrained model: {model}")
 
     tokenizer = getattr(hub.lib.transformers, pretrained_tokenizer)
 
-    hub.log.debug(f"Initialized pretrained tokenizer: {tokenizer}")
+    hub.log.trace(f"Initialized pretrained tokenizer: {tokenizer}")
 
     # Wrap the given tokenizer class with our own class that will use plugins to handle custom cases
-    class POPMLTokenizer(tokenizer):
+    class POPMLTokenizer(tokenizer, transformers.PreTrainedTokenizer):
         def tokenize(self, text, **kwargs):
             # Pass the text through the tokenizing plugins
             text: str = hub.token.init.tokenize(text, **kwargs)
 
             # Lastly, use the main tokenizer class
-            hub.log.debug(f"Passing text through the primary tokenizer {tokenizer}")
+            hub.log.trace(f"Passing text through the primary tokenizer {tokenizer}")
             text: List[str] = super().tokenize(text, **kwargs)
             return text
 
+        def convert_tokens_to_string(self, tokens: List[str]) -> str:
+            text: str = super().convert_tokens_to_string(tokens)
+            return hub.token.init.detokenize(text)
+
     custom_tokenizer = POPMLTokenizer.from_pretrained(model_name)
 
     return hub.lib.dtd.NamespaceDict(
         model=model,
         model_name=model_name,
         tokenizer=custom_tokenizer,
     )
@@ -93,36 +96,32 @@
 
 def translate(
     hub,
     texts: List[str],
     model: transformers.PreTrainedModel = None,
     tokenizer: transformers.PreTrainedTokenizerBase = None,
 ) -> List[str]:
-    """
-    Translate the list of strings and return the result
-    """
+    """Translate the list of strings and return the result."""
     if tokenizer is None:
         tokenizer = hub.ml.TOKENIZER
 
     if tokenizer is None:
-        raise RuntimeError(
-            "Tokenizer has not been initialized, please call hub.ml.tokenizer.init(<source_lang>, <dest_lang>)"
-        )
+        msg = "Tokenizer has not been initialized, please call hub.ml.tokenizer.init(<source_lang>, <dest_lang>)"
+        raise RuntimeError(msg)
 
-    hub.log.debug(f"Generating tokens using {tokenizer.__class__.__name__}")
+    hub.log.trace(f"Generating tokens using {tokenizer.__class__.__name__}")
     tokens = tokenizer(list(texts), return_tensors="pt", padding=True)
 
     if model is None:
         model = hub.ml.MODEL
 
     if model is None:
-        raise RuntimeError(
-            "Model has not been initialized, please call hub.ml.tokenizer.init(<source_lang>, <dest_lang>)"
-        )
+        msg = "Model has not been initialized, please call hub.ml.tokenizer.init(<source_lang>, <dest_lang>)"
+        raise RuntimeError(msg)
 
-    hub.log.debug(f"Generating translation tokens using {model.__class__.__name__}")
-    translate_tokens = hub.ml.MODEL.generate(**tokens)
+    hub.log.trace(f"Generating translation tokens using {model.__class__.__name__}")
+    translate_tokens = model.generate(**tokens)
 
     # TODO Can we pass in more special tokens?
     result = [tokenizer.decode(t, skip_special_tokens=True) for t in translate_tokens]
 
     return result
```

### Comparing `pop-ml-0.1.1/pop_ml.egg-info/PKG-INFO` & `pop-ml-0.2.0/pop_ml.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: pop-ml
-Version: 0.1.1
+Version: 0.2.0
 Summary: Machine learning library for pop projects
-Home-page: https://gitlab.com/vmware/pop/pop-ml
+Home-page: https://vmware.gitlab.io/pop/pop-ml/en/latest/index.html
 Author: VMWare, Inc.
 Author-email: idemproject@vmware.com
 License: Apache Software License 2.0
+Project-URL: Code, https://gitlab.com/vmware/pop/pop-ml
+Project-URL: Issue tracker, https://gitlab.com/vmware/pop/pop-ml/issues
 Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
@@ -28,37 +30,38 @@
 pop-ml
 ======
 
 .. image:: https://img.shields.io/badge/made%20with-pop-teal
    :alt: Made with pop, a Python implementation of Plugin Oriented Programming
    :target: https://pop.readthedocs.io/
 
+.. image:: https://img.shields.io/badge/docs%20on-GitLab%20Pages-blue
+   :alt: Documentation is published with Sphinx on GitLab Pages
+   :target: https://vmware.gitlab.io/pop/pop-ml/en/latest/index.html
+
 .. image:: https://img.shields.io/badge/made%20with-python-yellow
    :alt: Made with Python
    :target: https://www.python.org/
 
 
-pop-ml is a Python library that simplifies the integration of AI-powered translation
-capabilities into any Python project.  It leverages Hugging Face Transformers and pretrained
-tokenizers to provide an accessible translation experience. pop-ml aims to offer a
-straightforward API for translating strings in Python code, ensuring compatibility with
-widely-used projects.
+``pop-ml`` is a Python library that simplifies the integration of AI-powered
+capabilities into any POP-based Python project.
 
 About
 =====
 
+``pop-ml`` is a comprehensive Python library designed to facilitate the integration of AI-
+powered capabilities, such as translation, into POP-based Python projects.
+
+``pop-ml`` currently provides developers with an easy-to-use and seamless translation experience, allowing them
+to translate strings to other languages, such as english to spanish.
 
-pop-ml is a comprehensive Python library designed to facilitate the integration of AI-
-powered translation capabilities into Python projects. The primary goal of pop-ml is to
-provide developers with an easy-to-use and seamless translation experience, allowing them
-to translate strings in their Python code to any language.
-
-The library is built on top of the Hugging Face Transformers library and utilizes pretrained
-tokenizers to deliver accurate and efficient translations. By leveraging state-of-the-art
-language models, pop-ml ensures high-quality translations while maintaining simplicity in
+The library currently supports making use of Hugging Face Transformers library and can utilize pretrained
+tokenizers for delivering accurate and efficient translations. By leveraging state-of-the-art
+language models, ``pop-ml`` ensures high-quality translations while maintaining simplicity in
 its API.
 
 
 What is POP?
 ------------
 
 This project is built with `pop <https://pop.readthedocs.io/>`__, a Python-based
@@ -92,26 +95,26 @@
 
 If wanting to use ``pop-ml``, you can do so by either
 installing from PyPI or from source.
 
 Install from PyPI
 +++++++++++++++++
 
-To install pop-ml from PyPI, simply run the following command:
+To install ``pop-ml`` from PyPI, simply run the following command:
 
 .. code-block:: bash
 
     pip install pop-ml
 
-This will install the latest version of pop-ml, along with all required dependencies.
+This will install the latest version of ``pop-ml``, along with all required dependencies.
 
 Install from source
 +++++++++++++++++++
 
-To install pop-ml from source, first clone the repository from GitLab:
+To install ``pop-ml`` from source, first clone the repository from GitLab:
 
 .. code-block:: bash
 
     git clone https://gitlab.com/vmware/pop/pop-ml.git
 
 Next, navigate to the cloned repository directory:
 
@@ -124,21 +127,21 @@
 .. code-block:: bash
 
     pip install .
 
 Usage
 =====
 
-pop-ml can be used both as a command-line tool (pop-translate) and as a Python library.
-Below are examples of how to use pop-ml in both ways.
+``pop-ml`` can be used both as a command-line tool (``pop-translate``) and as a Python library.
+Below are examples of how to use ``pop-ml`` in both ways.
 
 CLI Examples
 ------------
 
-To use the pop-translate command-line tool, you can pass the text you want to translate as
+To use the ``pop-translate`` command-line tool, you can pass the text you want to translate as
 an argument, along with any additional options:
 
 .. code-block:: bash
 
     pop-translate "Hello, World!" --translate-to es
 
 This command will translate the input text "Hello, world!" from English (en) to Spanish (es).
```

### Comparing `pop-ml-0.1.1/setup.py` & `pop-ml-0.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
+"""Setup file."""
 import os
 import pathlib
 import shutil
 
-from setuptools import Command
-from setuptools import setup
+from setuptools import Command, setup
 
 NAME = "pop_ml"
 DESC = "Machine learning library for pop projects"
 
 # Version info -- read without importing
 _locals = {}
 with pathlib.Path(NAME, "version.py").open() as fp:
@@ -31,47 +31,57 @@
     for extra in EXTRA_PATH.iterdir():
         with extra.open("r") as f:
             REQUIREMENTS_EXTRA[extra.stem] = f.read().splitlines()
             REQUIREMENTS_EXTRA["full"].update(REQUIREMENTS_EXTRA[extra.stem])
 
 
 class Clean(Command):
+    """Cleanup any leftover __pychache__ subdirs."""
+
     user_options = []
 
     def initialize_options(self):
+        """Required for initializing."""
         pass
 
     def finalize_options(self):
+        """Required for finalizing."""
         pass
 
     def run(self):
+        """Cleanup any leftover __pychache__ subdirs."""
         for subdir in (NAME, "tests"):
-            for root, dirs, files in os.walk(
+            for root, dirs, _files in os.walk(
                 os.path.join(os.path.dirname(__file__), subdir)
             ):
                 for dir_ in dirs:
                     if dir_ == "__pycache__":
                         shutil.rmtree(os.path.join(root, dir_))
 
 
 def discover_packages():
+    """Discover all packages within the current project."""
     modules = []
     for package in (NAME,):
-        for root, _, files in os.walk(os.path.join(SETUP_DIRNAME, package)):
+        for root, _, _files in os.walk(os.path.join(SETUP_DIRNAME, package)):
             pdir = os.path.relpath(root, SETUP_DIRNAME)
             modname = pdir.replace(os.sep, ".")
             modules.append(modname)
     return modules
 
 
 setup(
     name="pop-ml",
     author="VMWare, Inc.",
     author_email="idemproject@vmware.com",
-    url="https://gitlab.com/vmware/pop/pop-ml",
+    url="https://vmware.gitlab.io/pop/pop-ml/en/latest/index.html",
+    project_urls={
+        "Code": "https://gitlab.com/vmware/pop/pop-ml",
+        "Issue tracker": "https://gitlab.com/vmware/pop/pop-ml/issues",
+    },
     version=VERSION,
     install_requires=REQUIREMENTS,
     extras_require=REQUIREMENTS_EXTRA,
     description=DESC,
     long_description=LONG_DESC,
     long_description_content_type="text/x-rst",
     license="Apache Software License 2.0",
```

