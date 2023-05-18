# Comparing `tmp/s2aff-0.51.tar.gz` & `tmp/s2aff-0.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2aff-0.51.tar", last modified: Wed May 17 22:02:03 2023, max compression
+gzip compressed data, was "s2aff-0.52.tar", last modified: Thu May 18 20:39:28 2023, max compression
```

## Comparing `s2aff-0.51.tar` & `s2aff-0.52.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-17 22:02:03.392484 s2aff-0.51/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.51/LICENSE
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-17 22:02:03.392353 s2aff-0.51/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.51/README.md
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-17 22:02:03.384763 s2aff-0.51/data/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.51/data/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.51/data/combine_gold.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.51/data/download_latest_ror.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-17 22:02:03.385033 s2aff-0.51/data/ner_model/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.51/data/ner_model/__init__.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-17 22:02:03.388792 s2aff-0.51/s2aff/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    11344 2023-05-17 20:13:58.000000 s2aff-0.51/s2aff/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-16 14:48:02.000000 s2aff-0.51/s2aff/consts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.51/s2aff/data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.51/s2aff/features.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.51/s2aff/file_cache.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-15 17:55:03.000000 s2aff-0.51/s2aff/lightgbm_helpers.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    13588 2023-05-15 17:57:22.000000 s2aff-0.51/s2aff/model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    34475 2023-05-16 23:30:17.000000 s2aff-0.51/s2aff/ror.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.51/s2aff/text.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-17 22:02:03.390293 s2aff-0.51/s2aff/timo/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.51/s2aff/timo/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.51/s2aff/timo/integration_test.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-15 17:57:34.000000 s2aff-0.51/s2aff/timo/interface.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-17 22:02:03.389690 s2aff-0.51/s2aff.egg-info/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-17 22:02:02.000000 s2aff-0.51/s2aff.egg-info/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-17 22:02:03.000000 s2aff-0.51/s2aff.egg-info/SOURCES.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-17 22:02:02.000000 s2aff-0.51/s2aff.egg-info/dependency_links.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-17 22:02:03.000000 s2aff-0.51/s2aff.egg-info/requires.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-17 22:02:03.000000 s2aff-0.51/s2aff.egg-info/top_level.txt
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-17 22:02:03.392038 s2aff-0.51/scripts/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.51/scripts/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-15 17:57:54.000000 s2aff-0.51/scripts/approximate_runtime_and_memory_usage.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-15 17:57:54.000000 s2aff-0.51/scripts/evaluate_first_stage_ranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-15 17:57:54.000000 s2aff-0.51/scripts/generate_lightgbm_training_data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.51/scripts/train_lightgbm_reranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.51/scripts/train_ner_model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.51/scripts/update_openalex_works_counts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-17 22:02:03.392530 s2aff-0.51/setup.cfg
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-17 22:01:58.000000 s2aff-0.51/setup.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-18 20:39:28.963023 s2aff-0.52/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.52/LICENSE
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-18 20:39:28.962782 s2aff-0.52/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.52/README.md
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-18 20:39:28.953929 s2aff-0.52/data/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.52/data/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.52/data/combine_gold.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.52/data/download_latest_ror.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-18 20:39:28.954208 s2aff-0.52/data/ner_model/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.52/data/ner_model/__init__.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-18 20:39:28.958120 s2aff-0.52/s2aff/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    11344 2023-05-18 18:48:56.000000 s2aff-0.52/s2aff/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-16 14:48:02.000000 s2aff-0.52/s2aff/consts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.52/s2aff/data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.52/s2aff/features.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.52/s2aff/file_cache.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-15 17:55:03.000000 s2aff-0.52/s2aff/lightgbm_helpers.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    13721 2023-05-18 20:38:26.000000 s2aff-0.52/s2aff/model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    34475 2023-05-16 23:30:17.000000 s2aff-0.52/s2aff/ror.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.52/s2aff/text.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-18 20:39:28.960059 s2aff-0.52/s2aff/timo/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.52/s2aff/timo/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.52/s2aff/timo/integration_test.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-15 17:57:34.000000 s2aff-0.52/s2aff/timo/interface.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-18 20:39:28.959348 s2aff-0.52/s2aff.egg-info/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-18 20:39:28.000000 s2aff-0.52/s2aff.egg-info/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-18 20:39:28.000000 s2aff-0.52/s2aff.egg-info/SOURCES.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-18 20:39:28.000000 s2aff-0.52/s2aff.egg-info/dependency_links.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-18 20:39:28.000000 s2aff-0.52/s2aff.egg-info/requires.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-18 20:39:28.000000 s2aff-0.52/s2aff.egg-info/top_level.txt
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-18 20:39:28.962438 s2aff-0.52/scripts/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.52/scripts/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-15 17:57:54.000000 s2aff-0.52/scripts/approximate_runtime_and_memory_usage.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-15 17:57:54.000000 s2aff-0.52/scripts/evaluate_first_stage_ranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-15 17:57:54.000000 s2aff-0.52/scripts/generate_lightgbm_training_data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.52/scripts/train_lightgbm_reranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.52/scripts/train_ner_model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.52/scripts/update_openalex_works_counts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-18 20:39:28.963091 s2aff-0.52/setup.cfg
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-18 20:39:08.000000 s2aff-0.52/setup.py
```

### Comparing `s2aff-0.51/LICENSE` & `s2aff-0.52/LICENSE`

 * *Files identical despite different names*

### Comparing `s2aff-0.51/README.md` & `s2aff-0.52/README.md`

 * *Files identical despite different names*

### Comparing `s2aff-0.51/data/combine_gold.py` & `s2aff-0.52/data/combine_gold.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.51/data/download_latest_ror.py` & `s2aff-0.52/data/download_latest_ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.51/s2aff/__init__.py` & `s2aff-0.52/s2aff/__init__.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.51/s2aff/consts.py` & `s2aff-0.52/s2aff/consts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.51/s2aff/data.py` & `s2aff-0.52/s2aff/data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.51/s2aff/features.py` & `s2aff-0.52/s2aff/features.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.51/s2aff/file_cache.py` & `s2aff-0.52/s2aff/file_cache.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.51/s2aff/lightgbm_helpers.py` & `s2aff-0.52/s2aff/lightgbm_helpers.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.51/s2aff/model.py` & `s2aff-0.52/s2aff/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import kenlm
 from s2aff.text import fix_text
 from s2aff.features import make_lightgbm_features, parse_ror_entry_into_single_string_lightgbm, FEATURE_NAMES
 from simpletransformers.ner import NERModel, NERArgs
 from blingfire import text_to_words
 from s2aff.consts import PATHS
 from s2aff.text import fix_text, CERTAINLY_MAIN
+import multiprocessing
 
 
 FEATURE_NAMES = list(FEATURE_NAMES)
 
 
 def parse_ner_prediction(ner_prediction, ror_index):
     """Parse the NER prediction that comes out of a NERPredictor
@@ -150,35 +151,35 @@
     """Named Entity Recognition for affiliation strings.
     Uses SimpleTransformers under the hood.
     """
 
     def __init__(self, model_path=PATHS["ner_model"], model_type="roberta", use_cuda=True):
         self.model_path = model_path
         self.model_type = model_type
-        self.use_cuda = use_cuda
+        self.use_cuda = True
         if self.model_path is not None:
             self.load_model(self.model_path, self.model_type)
 
     def load_model(self, model_path=PATHS["ner_model"], model_type="roberta"):
         """Load a model from disk.
 
         model_path (str, optional): Location of the saved NER model.
             Should be what is saved by SimpleTransformers NERModel. Defaults to PATHS["ner_model"].
         model_type (str, optional): Model type such as roberta or bert.
             If you don't know, check the config.json in the model directory. Defaults to "roberta".
         """
         self.model = NERModel(
             model_type,
             model_path,
-            use_cuda=self.use_cuda,
+            use_cuda=self.use_cuda,  # significant potential for speedups here by changing things
             args={
-                "use_multiprocessing": False,
-                "use_multiprocessing_for_evaluation": False,
-                "process_count": 1,
-                "eval_batch_size": 8,
+                "use_multiprocessing": True,
+                "use_multiprocessing_for_evaluation": True,
+                "process_count": multiprocessing.cpu_count(),
+                "eval_batch_size": multiprocessing.cpu_count()*8,
             },
         )
 
     def save_model(self, model_path=PATHS["ner_model"]):
         """Save model to disk
 
         Args:
```

### Comparing `s2aff-0.51/s2aff/ror.py` & `s2aff-0.52/s2aff/ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.51/s2aff/text.py` & `s2aff-0.52/s2aff/text.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.51/s2aff/timo/integration_test.py` & `s2aff-0.52/s2aff/timo/integration_test.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.51/s2aff/timo/interface.py` & `s2aff-0.52/s2aff/timo/interface.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.51/s2aff.egg-info/SOURCES.txt` & `s2aff-0.52/s2aff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `s2aff-0.51/scripts/approximate_runtime_and_memory_usage.py` & `s2aff-0.52/scripts/approximate_runtime_and_memory_usage.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.51/scripts/evaluate_first_stage_ranker.py` & `s2aff-0.52/scripts/evaluate_first_stage_ranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.51/scripts/generate_lightgbm_training_data.py` & `s2aff-0.52/scripts/generate_lightgbm_training_data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.51/scripts/train_lightgbm_reranker.py` & `s2aff-0.52/scripts/train_lightgbm_reranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.51/scripts/train_ner_model.py` & `s2aff-0.52/scripts/train_ner_model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.51/scripts/update_openalex_works_counts.py` & `s2aff-0.52/scripts/update_openalex_works_counts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.51/setup.py` & `s2aff-0.52/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 from os import path
 
 requirements_file = path.join(path.dirname(__file__), "requirements.in")
 requirements = [r for r in open(requirements_file).read().split("\n") if not re.match(r"^\-", r)]
 
 setuptools.setup(
     name="s2aff",
-    version="0.51",
+    version="0.52",
     url="https://github.com/allenai/S2AFF",
     packages=setuptools.find_packages(),
     install_requires=requirements,  # dependencies specified in requirements.in
     description="Semantic Scholar's Affiliation Extraction: Link Your Raw Affiliations to ROR IDs",
 )
```

