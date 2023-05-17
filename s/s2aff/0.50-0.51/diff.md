# Comparing `tmp/s2aff-0.50.tar.gz` & `tmp/s2aff-0.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2aff-0.50.tar", last modified: Wed May 17 04:09:56 2023, max compression
+gzip compressed data, was "s2aff-0.51.tar", last modified: Wed May 17 22:02:03 2023, max compression
```

## Comparing `s2aff-0.50.tar` & `s2aff-0.51.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-17 04:09:56.128327 s2aff-0.50/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.50/LICENSE
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-17 04:09:56.128130 s2aff-0.50/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.50/README.md
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-17 04:09:56.116906 s2aff-0.50/data/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.50/data/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.50/data/combine_gold.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.50/data/download_latest_ror.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-17 04:09:56.117334 s2aff-0.50/data/ner_model/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.50/data/ner_model/__init__.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-17 04:09:56.122288 s2aff-0.50/s2aff/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    11225 2023-05-17 03:57:37.000000 s2aff-0.50/s2aff/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-16 14:48:02.000000 s2aff-0.50/s2aff/consts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.50/s2aff/data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.50/s2aff/features.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.50/s2aff/file_cache.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-15 17:55:03.000000 s2aff-0.50/s2aff/lightgbm_helpers.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    13588 2023-05-15 17:57:22.000000 s2aff-0.50/s2aff/model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    34475 2023-05-16 23:30:17.000000 s2aff-0.50/s2aff/ror.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.50/s2aff/text.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-17 04:09:56.125683 s2aff-0.50/s2aff/timo/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.50/s2aff/timo/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.50/s2aff/timo/integration_test.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-15 17:57:34.000000 s2aff-0.50/s2aff/timo/interface.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-17 04:09:56.125186 s2aff-0.50/s2aff.egg-info/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-17 04:09:55.000000 s2aff-0.50/s2aff.egg-info/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-17 04:09:56.000000 s2aff-0.50/s2aff.egg-info/SOURCES.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-17 04:09:55.000000 s2aff-0.50/s2aff.egg-info/dependency_links.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-17 04:09:55.000000 s2aff-0.50/s2aff.egg-info/requires.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-17 04:09:55.000000 s2aff-0.50/s2aff.egg-info/top_level.txt
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-17 04:09:56.127786 s2aff-0.50/scripts/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.50/scripts/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-15 17:57:54.000000 s2aff-0.50/scripts/approximate_runtime_and_memory_usage.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-15 17:57:54.000000 s2aff-0.50/scripts/evaluate_first_stage_ranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-15 17:57:54.000000 s2aff-0.50/scripts/generate_lightgbm_training_data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.50/scripts/train_lightgbm_reranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.50/scripts/train_ner_model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.50/scripts/update_openalex_works_counts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-17 04:09:56.128389 s2aff-0.50/setup.cfg
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-17 04:09:51.000000 s2aff-0.50/setup.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-17 22:02:03.392484 s2aff-0.51/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.51/LICENSE
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-17 22:02:03.392353 s2aff-0.51/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.51/README.md
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-17 22:02:03.384763 s2aff-0.51/data/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.51/data/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.51/data/combine_gold.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.51/data/download_latest_ror.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-17 22:02:03.385033 s2aff-0.51/data/ner_model/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.51/data/ner_model/__init__.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-17 22:02:03.388792 s2aff-0.51/s2aff/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    11344 2023-05-17 20:13:58.000000 s2aff-0.51/s2aff/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-16 14:48:02.000000 s2aff-0.51/s2aff/consts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.51/s2aff/data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.51/s2aff/features.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.51/s2aff/file_cache.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-15 17:55:03.000000 s2aff-0.51/s2aff/lightgbm_helpers.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    13588 2023-05-15 17:57:22.000000 s2aff-0.51/s2aff/model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    34475 2023-05-16 23:30:17.000000 s2aff-0.51/s2aff/ror.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.51/s2aff/text.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-17 22:02:03.390293 s2aff-0.51/s2aff/timo/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.51/s2aff/timo/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.51/s2aff/timo/integration_test.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-15 17:57:34.000000 s2aff-0.51/s2aff/timo/interface.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-17 22:02:03.389690 s2aff-0.51/s2aff.egg-info/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-17 22:02:02.000000 s2aff-0.51/s2aff.egg-info/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-17 22:02:03.000000 s2aff-0.51/s2aff.egg-info/SOURCES.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-17 22:02:02.000000 s2aff-0.51/s2aff.egg-info/dependency_links.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-17 22:02:03.000000 s2aff-0.51/s2aff.egg-info/requires.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-17 22:02:03.000000 s2aff-0.51/s2aff.egg-info/top_level.txt
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-17 22:02:03.392038 s2aff-0.51/scripts/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.51/scripts/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-15 17:57:54.000000 s2aff-0.51/scripts/approximate_runtime_and_memory_usage.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-15 17:57:54.000000 s2aff-0.51/scripts/evaluate_first_stage_ranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-15 17:57:54.000000 s2aff-0.51/scripts/generate_lightgbm_training_data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.51/scripts/train_lightgbm_reranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.51/scripts/train_ner_model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.51/scripts/update_openalex_works_counts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-17 22:02:03.392530 s2aff-0.51/setup.cfg
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-17 22:01:58.000000 s2aff-0.51/setup.py
```

### Comparing `s2aff-0.50/LICENSE` & `s2aff-0.51/LICENSE`

 * *Files identical despite different names*

### Comparing `s2aff-0.50/README.md` & `s2aff-0.51/README.md`

 * *Files identical despite different names*

### Comparing `s2aff-0.50/data/combine_gold.py` & `s2aff-0.51/data/combine_gold.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.50/data/download_latest_ror.py` & `s2aff-0.51/data/download_latest_ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.50/s2aff/__init__.py` & `s2aff-0.51/s2aff/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,17 +94,18 @@
 def set_s2aff_vars(ror_index_, look_for_grid_and_isni_, no_candidates_output_text_, pairwise_model_, top_k_first_stage_, pairwise_model_threshold_, no_ror_output_text_, pairwise_model_delta_threshold_, number_of_top_candidates_to_return_):
     global ror_index, look_for_grid_and_isni, no_candidates_output_text, pairwise_model, top_k_first_stage, pairwise_model_threshold, no_ror_output_text, pairwise_model_delta_threshold, number_of_top_candidates_to_return
     ror_index, look_for_grid_and_isni, no_candidates_output_text, pairwise_model, top_k_first_stage, pairwise_model_threshold, no_ror_output_text, pairwise_model_delta_threshold, number_of_top_candidates_to_return = \
         ror_index_, look_for_grid_and_isni_, no_candidates_output_text_, pairwise_model_, top_k_first_stage_, pairwise_model_threshold_, no_ror_output_text_, pairwise_model_delta_threshold_, number_of_top_candidates_to_return_
 
 
 def reranking_multi(inputs, **kwargs):
+    # inputs[-1][-1] will be the batch size
     func = partial(process_item, **kwargs)
     with multiprocessing.get_context("spawn").Pool(multiprocessing.cpu_count()) as pool:
-        generator = pool.imap_unordered(func, inputs, min(100, inputs[-1][-1]))
+        generator = pool.imap_unordered(func, inputs, inputs[-1][-1]//multiprocessing.cpu_count())  # TODO: the batch size (third arg) could use some work
         for result in generator:
             yield result
 
 
 class S2AFF:
     """
     The wrapper class that links a raw affiliation string to a ROR entry.
```

### Comparing `s2aff-0.50/s2aff/consts.py` & `s2aff-0.51/s2aff/consts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.50/s2aff/data.py` & `s2aff-0.51/s2aff/data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.50/s2aff/features.py` & `s2aff-0.51/s2aff/features.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.50/s2aff/file_cache.py` & `s2aff-0.51/s2aff/file_cache.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.50/s2aff/lightgbm_helpers.py` & `s2aff-0.51/s2aff/lightgbm_helpers.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.50/s2aff/model.py` & `s2aff-0.51/s2aff/model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.50/s2aff/ror.py` & `s2aff-0.51/s2aff/ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.50/s2aff/text.py` & `s2aff-0.51/s2aff/text.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.50/s2aff/timo/integration_test.py` & `s2aff-0.51/s2aff/timo/integration_test.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.50/s2aff/timo/interface.py` & `s2aff-0.51/s2aff/timo/interface.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.50/s2aff.egg-info/SOURCES.txt` & `s2aff-0.51/s2aff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `s2aff-0.50/scripts/approximate_runtime_and_memory_usage.py` & `s2aff-0.51/scripts/approximate_runtime_and_memory_usage.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.50/scripts/evaluate_first_stage_ranker.py` & `s2aff-0.51/scripts/evaluate_first_stage_ranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.50/scripts/generate_lightgbm_training_data.py` & `s2aff-0.51/scripts/generate_lightgbm_training_data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.50/scripts/train_lightgbm_reranker.py` & `s2aff-0.51/scripts/train_lightgbm_reranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.50/scripts/train_ner_model.py` & `s2aff-0.51/scripts/train_ner_model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.50/scripts/update_openalex_works_counts.py` & `s2aff-0.51/scripts/update_openalex_works_counts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.50/setup.py` & `s2aff-0.51/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 from os import path
 
 requirements_file = path.join(path.dirname(__file__), "requirements.in")
 requirements = [r for r in open(requirements_file).read().split("\n") if not re.match(r"^\-", r)]
 
 setuptools.setup(
     name="s2aff",
-    version="0.50",
+    version="0.51",
     url="https://github.com/allenai/S2AFF",
     packages=setuptools.find_packages(),
     install_requires=requirements,  # dependencies specified in requirements.in
     description="Semantic Scholar's Affiliation Extraction: Link Your Raw Affiliations to ROR IDs",
 )
```

