# Comparing `tmp/openai_parallel_toolkit-0.1.tar.gz` & `tmp/openai_parallel_toolkit-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_parallel_toolkit-0.1.tar", last modified: Wed May 17 12:33:23 2023, max compression
+gzip compressed data, was "openai_parallel_toolkit-0.2.tar", last modified: Thu May 18 11:48:41 2023, max compression
```

## Comparing `openai_parallel_toolkit-0.1.tar` & `openai_parallel_toolkit-0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 jellow     (501) staff       (20)        0 2023-05-17 12:33:23.456425 openai_parallel_toolkit-0.1/
--rw-r--r--   0 jellow     (501) staff       (20)     1063 2023-05-14 07:58:47.000000 openai_parallel_toolkit-0.1/LICENSE
--rw-r--r--   0 jellow     (501) staff       (20)    13470 2023-05-17 12:33:23.456222 openai_parallel_toolkit-0.1/PKG-INFO
--rw-r--r--   0 jellow     (501) staff       (20)    12608 2023-05-17 12:18:47.000000 openai_parallel_toolkit-0.1/README.md
-drwxr-xr-x   0 jellow     (501) staff       (20)        0 2023-05-17 12:33:23.449655 openai_parallel_toolkit-0.1/openai_parallel_toolkit/
--rw-r--r--   0 jellow     (501) staff       (20)      213 2023-05-17 02:40:09.000000 openai_parallel_toolkit-0.1/openai_parallel_toolkit/__init__.py
-drwxr-xr-x   0 jellow     (501) staff       (20)        0 2023-05-17 12:33:23.451644 openai_parallel_toolkit-0.1/openai_parallel_toolkit/api/
--rw-r--r--   0 jellow     (501) staff       (20)      113 2023-05-16 08:22:42.000000 openai_parallel_toolkit-0.1/openai_parallel_toolkit/api/__init__.py
--rw-r--r--   0 jellow     (501) staff       (20)     1768 2023-05-17 03:44:29.000000 openai_parallel_toolkit-0.1/openai_parallel_toolkit/api/api.py
--rw-r--r--   0 jellow     (501) staff       (20)     5252 2023-05-17 09:09:50.000000 openai_parallel_toolkit-0.1/openai_parallel_toolkit/api/keys.py
--rw-r--r--   0 jellow     (501) staff       (20)     2899 2023-05-17 09:13:21.000000 openai_parallel_toolkit-0.1/openai_parallel_toolkit/api/request.py
--rw-r--r--   0 jellow     (501) staff       (20)       20 2023-05-17 01:58:51.000000 openai_parallel_toolkit-0.1/openai_parallel_toolkit/config.py
-drwxr-xr-x   0 jellow     (501) staff       (20)        0 2023-05-17 12:33:23.454638 openai_parallel_toolkit-0.1/openai_parallel_toolkit/core/
--rw-r--r--   0 jellow     (501) staff       (20)       95 2023-05-17 01:02:05.000000 openai_parallel_toolkit-0.1/openai_parallel_toolkit/core/__init__.py
--rw-r--r--   0 jellow     (501) staff       (20)     4575 2023-05-17 08:17:14.000000 openai_parallel_toolkit-0.1/openai_parallel_toolkit/core/main.py
--rw-r--r--   0 jellow     (501) staff       (20)     4765 2023-05-17 07:42:13.000000 openai_parallel_toolkit-0.1/openai_parallel_toolkit/core/multithread.py
-drwxr-xr-x   0 jellow     (501) staff       (20)        0 2023-05-17 12:33:23.455852 openai_parallel_toolkit-0.1/openai_parallel_toolkit/utils/
--rw-r--r--   0 jellow     (501) staff       (20)      214 2023-05-17 08:12:20.000000 openai_parallel_toolkit-0.1/openai_parallel_toolkit/utils/__init__.py
--rw-r--r--   0 jellow     (501) staff       (20)     1041 2023-05-16 02:43:32.000000 openai_parallel_toolkit-0.1/openai_parallel_toolkit/utils/logger.py
--rw-r--r--   0 jellow     (501) staff       (20)     3961 2023-05-17 09:38:50.000000 openai_parallel_toolkit-0.1/openai_parallel_toolkit/utils/reader.py
--rw-r--r--   0 jellow     (501) staff       (20)      913 2023-05-17 11:15:47.000000 openai_parallel_toolkit-0.1/openai_parallel_toolkit/utils/token.py
--rw-r--r--   0 jellow     (501) staff       (20)      613 2023-05-17 00:55:13.000000 openai_parallel_toolkit-0.1/openai_parallel_toolkit/utils/tqdm.py
-drwxr-xr-x   0 jellow     (501) staff       (20)        0 2023-05-17 12:33:23.450701 openai_parallel_toolkit-0.1/openai_parallel_toolkit.egg-info/
--rw-r--r--   0 jellow     (501) staff       (20)    13470 2023-05-17 12:33:23.000000 openai_parallel_toolkit-0.1/openai_parallel_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 jellow     (501) staff       (20)      826 2023-05-17 12:33:23.000000 openai_parallel_toolkit-0.1/openai_parallel_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 jellow     (501) staff       (20)        1 2023-05-17 12:33:23.000000 openai_parallel_toolkit-0.1/openai_parallel_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 jellow     (501) staff       (20)       30 2023-05-17 12:33:23.000000 openai_parallel_toolkit-0.1/openai_parallel_toolkit.egg-info/requires.txt
--rw-r--r--   0 jellow     (501) staff       (20)       24 2023-05-17 12:33:23.000000 openai_parallel_toolkit-0.1/openai_parallel_toolkit.egg-info/top_level.txt
--rw-r--r--   0 jellow     (501) staff       (20)       38 2023-05-17 12:33:23.456462 openai_parallel_toolkit-0.1/setup.cfg
--rw-r--r--   0 jellow     (501) staff       (20)     1217 2023-05-15 06:56:17.000000 openai_parallel_toolkit-0.1/setup.py
-drwxr-xr-x   0 jellow     (501) staff       (20)        0 2023-05-17 12:33:23.455989 openai_parallel_toolkit-0.1/test/
--rw-r--r--   0 jellow     (501) staff       (20)      671 2023-05-17 04:44:34.000000 openai_parallel_toolkit-0.1/test/test_multithread.py
+drwxr-xr-x   0 jellow     (501) staff       (20)        0 2023-05-18 11:48:41.875548 openai_parallel_toolkit-0.2/
+-rw-r--r--   0 jellow     (501) staff       (20)     1063 2023-05-14 07:58:47.000000 openai_parallel_toolkit-0.2/LICENSE
+-rw-r--r--   0 jellow     (501) staff       (20)    13470 2023-05-18 11:48:41.875382 openai_parallel_toolkit-0.2/PKG-INFO
+-rw-r--r--   0 jellow     (501) staff       (20)    12608 2023-05-17 12:18:47.000000 openai_parallel_toolkit-0.2/README.md
+drwxr-xr-x   0 jellow     (501) staff       (20)        0 2023-05-18 11:48:41.870508 openai_parallel_toolkit-0.2/openai_parallel_toolkit/
+-rw-r--r--   0 jellow     (501) staff       (20)      213 2023-05-17 02:40:09.000000 openai_parallel_toolkit-0.2/openai_parallel_toolkit/__init__.py
+drwxr-xr-x   0 jellow     (501) staff       (20)        0 2023-05-18 11:48:41.872702 openai_parallel_toolkit-0.2/openai_parallel_toolkit/api/
+-rw-r--r--   0 jellow     (501) staff       (20)      113 2023-05-17 12:36:55.000000 openai_parallel_toolkit-0.2/openai_parallel_toolkit/api/__init__.py
+-rw-r--r--   0 jellow     (501) staff       (20)     1769 2023-05-17 12:36:55.000000 openai_parallel_toolkit-0.2/openai_parallel_toolkit/api/api.py
+-rw-r--r--   0 jellow     (501) staff       (20)     5253 2023-05-17 12:36:55.000000 openai_parallel_toolkit-0.2/openai_parallel_toolkit/api/keys.py
+-rw-r--r--   0 jellow     (501) staff       (20)     2906 2023-05-18 11:47:53.000000 openai_parallel_toolkit-0.2/openai_parallel_toolkit/api/request.py
+-rw-r--r--   0 jellow     (501) staff       (20)       20 2023-05-17 01:58:51.000000 openai_parallel_toolkit-0.2/openai_parallel_toolkit/config.py
+drwxr-xr-x   0 jellow     (501) staff       (20)        0 2023-05-18 11:48:41.873492 openai_parallel_toolkit-0.2/openai_parallel_toolkit/core/
+-rw-r--r--   0 jellow     (501) staff       (20)       95 2023-05-17 01:02:05.000000 openai_parallel_toolkit-0.2/openai_parallel_toolkit/core/__init__.py
+-rw-r--r--   0 jellow     (501) staff       (20)     4575 2023-05-17 08:17:14.000000 openai_parallel_toolkit-0.2/openai_parallel_toolkit/core/main.py
+-rw-r--r--   0 jellow     (501) staff       (20)     4852 2023-05-18 11:47:53.000000 openai_parallel_toolkit-0.2/openai_parallel_toolkit/core/multithread.py
+drwxr-xr-x   0 jellow     (501) staff       (20)        0 2023-05-18 11:48:41.874758 openai_parallel_toolkit-0.2/openai_parallel_toolkit/utils/
+-rw-r--r--   0 jellow     (501) staff       (20)      214 2023-05-17 12:36:55.000000 openai_parallel_toolkit-0.2/openai_parallel_toolkit/utils/__init__.py
+-rw-r--r--   0 jellow     (501) staff       (20)     1042 2023-05-18 11:32:14.000000 openai_parallel_toolkit-0.2/openai_parallel_toolkit/utils/logger.py
+-rw-r--r--   0 jellow     (501) staff       (20)     4005 2023-05-18 11:47:53.000000 openai_parallel_toolkit-0.2/openai_parallel_toolkit/utils/reader.py
+-rw-r--r--   0 jellow     (501) staff       (20)      913 2023-05-17 11:15:47.000000 openai_parallel_toolkit-0.2/openai_parallel_toolkit/utils/token.py
+-rw-r--r--   0 jellow     (501) staff       (20)      753 2023-05-18 11:47:53.000000 openai_parallel_toolkit-0.2/openai_parallel_toolkit/utils/tqdm.py
+drwxr-xr-x   0 jellow     (501) staff       (20)        0 2023-05-18 11:48:41.871591 openai_parallel_toolkit-0.2/openai_parallel_toolkit.egg-info/
+-rw-r--r--   0 jellow     (501) staff       (20)    13470 2023-05-18 11:48:41.000000 openai_parallel_toolkit-0.2/openai_parallel_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 jellow     (501) staff       (20)      826 2023-05-18 11:48:41.000000 openai_parallel_toolkit-0.2/openai_parallel_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 jellow     (501) staff       (20)        1 2023-05-18 11:48:41.000000 openai_parallel_toolkit-0.2/openai_parallel_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 jellow     (501) staff       (20)       33 2023-05-18 11:48:41.000000 openai_parallel_toolkit-0.2/openai_parallel_toolkit.egg-info/requires.txt
+-rw-r--r--   0 jellow     (501) staff       (20)       24 2023-05-18 11:48:41.000000 openai_parallel_toolkit-0.2/openai_parallel_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 jellow     (501) staff       (20)       38 2023-05-18 11:48:41.875589 openai_parallel_toolkit-0.2/setup.cfg
+-rw-r--r--   0 jellow     (501) staff       (20)     1230 2023-05-18 11:47:54.000000 openai_parallel_toolkit-0.2/setup.py
+drwxr-xr-x   0 jellow     (501) staff       (20)        0 2023-05-18 11:48:41.875008 openai_parallel_toolkit-0.2/test/
+-rw-r--r--   0 jellow     (501) staff       (20)      671 2023-05-17 04:44:34.000000 openai_parallel_toolkit-0.2/test/test_multithread.py
```

### Comparing `openai_parallel_toolkit-0.1/LICENSE` & `openai_parallel_toolkit-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_parallel_toolkit-0.1/PKG-INFO` & `openai_parallel_toolkit-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_parallel_toolkit
-Version: 0.1
+Version: 0.2
 Summary: OpenAI-Parallel-Toolkit is a Python library for handling multiple OpenAI API keys and parallel tasks. It provides API key rotation, multithreading for faster task execution, and utility functions to boost your OpenAI integration. Ideal for efficient large-scale OpenAI usage.
 Home-page: https://github.com/CZT0/OpenAI-Parallel-Toolkit
 Author: Jellow
 Author-email: dvdx@foxmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `openai_parallel_toolkit-0.1/README.md` & `openai_parallel_toolkit-0.2/README.md`

 * *Files identical despite different names*

### Comparing `openai_parallel_toolkit-0.1/openai_parallel_toolkit/api/api.py` & `openai_parallel_toolkit-0.2/openai_parallel_toolkit/api/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Import the necessary libraries
-import openai
 from abc import ABC, abstractmethod
 
+import openai
+
 
 class OpenAIModel(ABC):
     """Abstract Base Class (ABC) for OpenAI models."""
 
     @abstractmethod
     def __init__(self, **kwargs):
         """
```

### Comparing `openai_parallel_toolkit-0.1/openai_parallel_toolkit/api/keys.py` & `openai_parallel_toolkit-0.2/openai_parallel_toolkit/api/keys.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # Import the necessary libraries
 import array
+import datetime
 import logging
+import random
 import threading
-import datetime
 import time
-import random
+
 import openai
 
-# Import related local modules
-from .api import OpenAIModel
 from openai_parallel_toolkit.config import LOG_LABEL
 from openai_parallel_toolkit.utils import read_keys, read_api_base
+# Import related local modules
+from .api import OpenAIModel
 
 
 class APIKeyManager:
     """
     Class to manage the API keys of OpenAI. Implements the Singleton pattern.
     """
     _instance = None  # Singleton instance variable
```

### Comparing `openai_parallel_toolkit-0.1/openai_parallel_toolkit/api/request.py` & `openai_parallel_toolkit-0.2/openai_parallel_toolkit/api/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import logging
-from typing import Type
 
 import openai
 
 # Import related local modules
 from .api import OpenAIModel
-from ..config import LOG_LABEL
 from .keys import APIKeyManager
+from ..config import LOG_LABEL
 
 
 def request_openai_api(openai_model: OpenAIModel, keys=None, config_path=None, max_retries=5):
     """Function to handle requests to the OpenAI API.
 
     Args:
         openai_model (OpenAIModel): Instance of the OpenAIModel class that will generate the completion.
@@ -33,15 +32,15 @@
 
         try:
             # Attempt to generate a completion
             completion = openai_model.generate()
             break
         except Exception as e:
             # Handle different types of errors
-            if "exceeded your current quota" in str(e):
+            if "exceeded your current quota" in str(e) or "<empty message>" in str(e):
                 # If the quota has been exceeded, remove the key and try again
                 key_manager.remove_key(key)
                 continue
             if "Rate limit" in str(e):
                 # If the rate limit is hit, switch the API key and try again
                 completion = key_manager.switch_api_key(openai_model)
                 if completion is None:
```

### Comparing `openai_parallel_toolkit-0.1/openai_parallel_toolkit/core/main.py` & `openai_parallel_toolkit-0.2/openai_parallel_toolkit/core/main.py`

 * *Files identical despite different names*

### Comparing `openai_parallel_toolkit-0.1/openai_parallel_toolkit/core/multithread.py` & `openai_parallel_toolkit-0.2/openai_parallel_toolkit/core/multithread.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,19 +2,18 @@
 import logging
 import multiprocessing
 import os
 import traceback
 from concurrent.futures import ThreadPoolExecutor
 from typing import Type
 
+from openai_parallel_toolkit.api import APIKeyManager
 from openai_parallel_toolkit.api import request_openai_api, OpenAIModel
 from openai_parallel_toolkit.config import LOG_LABEL
-from openai_parallel_toolkit.api import APIKeyManager
-from openai_parallel_toolkit.utils import partition_data, read_folder
-from openai_parallel_toolkit.utils import ProgressBar
+from openai_parallel_toolkit.utils import ProgressBar, partition_data, read_folder, logger_init
 
 
 def process_data_chunk(data_chunk, output_path, process_output, process_data):
     """Process a chunk of data and write results to output file.
 
     Args:
         data_chunk (dict): The data chunk to be processed.
@@ -23,15 +22,15 @@
         process_data (function): The function used to process the data.
     """
     for key, value in data_chunk.items():
         data = process_data(value)
         if output_path is not None:
             output_file_without_ext = os.path.join(output_path, key)
             process_output(data, output_file_without_ext)
-            ProgressBar().update()
+            ProgressBar().get_instance().update()
 
 
 def multi_process_one(data: list, openai_model_class: Type[OpenAIModel], threads=multiprocessing.cpu_count() * 5,
                       **kwargs):
     """Request OpenAI API in parallel using multiple threads.
 
     Args:
@@ -47,21 +46,22 @@
         try:
             results = list(
                 executor.map(lambda item: request_openai_api(
                     openai_model_class(prompt=item[0], content=item[1], **kwargs)),
                              data))
         except Exception as e:
             tb = traceback.format_exc()
-            logging.error(f"Error occurred while processing data: {e}\n{tb}")
+            logging.error(f"{LOG_LABEL}Error occurred while processing data: {e}\n{tb}")
             return None
     return results
 
 
 def multi_thread_run(config_path, input_path, file_count, output_path, process_input, process_output, process_data,
                      num_threads=multiprocessing.cpu_count() * 10, name="Progress"):
+    logger_init()
     """Run the processing task using multiple threads.
 
     Args:
         config_path (str): The path of the configuration file.
         input_path (str): The path of the input file.
         file_count (int): The number of files to be processed.
         output_path (str): The path of the output file.
@@ -75,15 +75,15 @@
     if output_path is not None:
         if not os.path.exists(output_path):
             os.makedirs(output_path)
     data = read_folder(input_path=input_path, file_count=file_count, output_path=output_path,
                        process_input=process_input)
     if data is None:
         return
-    ProgressBar(total=len(data), desc=name)  # Initialize the progress bar
+    ProgressBar.get_instance(total=len(data), desc=name)  # Initialize the progress bar
     threads = min(len(data), num_threads)  # Determine the number of threads to use
     data_chunks = partition_data(data, threads)  # Partition the data into chunks for each thread
 
     # Use ThreadPoolExecutor to manage our threads
     with concurrent.futures.ThreadPoolExecutor(max_workers=threads) as executor:
         futures = []
         for i in range(threads):
@@ -96,8 +96,9 @@
         # As each future completes, check if there was an exception and log the error if so
         for future in concurrent.futures.as_completed(futures):
             try:
                 future.result()
             except Exception as e:
                 tb = traceback.format_exc()
                 logging.fatal(f"{LOG_LABEL}Error occurred while processing data: {e}\n{tb}")
-    ProgressBar().close()  # Close the progress bar when all threads are done
+    ProgressBar().get_instance().close()
+    ProgressBar().get_instance().destroy()  # Close the progress bar when all threads are done
```

### Comparing `openai_parallel_toolkit-0.1/openai_parallel_toolkit/utils/logger.py` & `openai_parallel_toolkit-0.2/openai_parallel_toolkit/utils/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 
 from colorlog import ColoredFormatter
+
 from openai_parallel_toolkit.config import LOG_LABEL
 
 
 class LogFilter(logging.Filter):
     def __init__(self, label):
         super().__init__()
         self.label = label
```

### Comparing `openai_parallel_toolkit-0.1/openai_parallel_toolkit/utils/reader.py` & `openai_parallel_toolkit-0.2/openai_parallel_toolkit/utils/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,12 +107,14 @@
 
     Args:
         config_path (str): The path to the configuration file.
 
     Returns:
         str: The 'api_base' field from the configuration file.
     """
+    if not config_path:
+        return None
     with open(config_path, 'r') as f:
         config = json.load(f)
     if 'api_base' in config:
         return config['api_base']
     return None
```

### Comparing `openai_parallel_toolkit-0.1/openai_parallel_toolkit/utils/token.py` & `openai_parallel_toolkit-0.2/openai_parallel_toolkit/utils/token.py`

 * *Files identical despite different names*

### Comparing `openai_parallel_toolkit-0.1/openai_parallel_toolkit.egg-info/PKG-INFO` & `openai_parallel_toolkit-0.2/openai_parallel_toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-parallel-toolkit
-Version: 0.1
+Version: 0.2
 Summary: OpenAI-Parallel-Toolkit is a Python library for handling multiple OpenAI API keys and parallel tasks. It provides API key rotation, multithreading for faster task execution, and utility functions to boost your OpenAI integration. Ideal for efficient large-scale OpenAI usage.
 Home-page: https://github.com/CZT0/OpenAI-Parallel-Toolkit
 Author: Jellow
 Author-email: dvdx@foxmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `openai_parallel_toolkit-0.1/openai_parallel_toolkit.egg-info/SOURCES.txt` & `openai_parallel_toolkit-0.2/openai_parallel_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openai_parallel_toolkit-0.1/setup.py` & `openai_parallel_toolkit-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='openai_parallel_toolkit',
-    version='0.1',
+    version='0.2',
     author='Jellow',
     author_email='dvdx@foxmail.com',
     description='OpenAI-Parallel-Toolkit is a Python library for handling multiple OpenAI API keys and parallel tasks.'
                 ' It provides API key rotation, multithreading for faster task execution, '
                 'and utility functions to boost your OpenAI integration. '
                 'Ideal for efficient large-scale OpenAI usage.',
     long_description=open('README.md').read(),
@@ -23,9 +23,10 @@
         'Programming Language :: Python :: 3.9',
     ],
     install_requires=[
         'openai',
         'colorlog',
         'tqdm',
         'tiktoken',
+        'py'
     ]
 )
```

### Comparing `openai_parallel_toolkit-0.1/test/test_multithread.py` & `openai_parallel_toolkit-0.2/test/test_multithread.py`

 * *Files identical despite different names*

