# Comparing `tmp/zeno_build-0.0.0a0.tar.gz` & `tmp/zeno_build-0.0.0a1.tar.gz`

## Comparing `zeno_build-0.0.0a0.tar` & `zeno_build-0.0.0a1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 zeno_build-0.0.0a0/zeno_build/__init__.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 zeno_build-0.0.0a0/zeno_build/cache_utils.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 zeno_build-0.0.0a0/zeno_build/version.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zeno_build-0.0.0a0/zeno_build/evaluation/__init__.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 zeno_build-0.0.0a0/zeno_build/evaluation/classification_metrics.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 zeno_build-0.0.0a0/zeno_build/evaluation/text_features/__init__.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 zeno_build-0.0.0a0/zeno_build/evaluation/text_features/exact_match.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 zeno_build-0.0.0a0/zeno_build/evaluation/text_features/length.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 zeno_build-0.0.0a0/zeno_build/evaluation/text_metrics/__init__.py
--rw-r--r--   0        0        0    15356 2020-02-02 00:00:00.000000 zeno_build-0.0.0a0/zeno_build/evaluation/text_metrics/critique.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 zeno_build-0.0.0a0/zeno_build/experiments/__init__.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 zeno_build-0.0.0a0/zeno_build/experiments/experiment_run.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 zeno_build-0.0.0a0/zeno_build/experiments/search_space.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 zeno_build-0.0.0a0/zeno_build/models/__init__.py
--rw-r--r--   0        0        0    11088 2020-02-02 00:00:00.000000 zeno_build-0.0.0a0/zeno_build/models/chat_generate.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 zeno_build-0.0.0a0/zeno_build/models/global_models.py
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 zeno_build-0.0.0a0/zeno_build/models/lm_config.py
--rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 zeno_build-0.0.0a0/zeno_build/models/text_generate.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 zeno_build-0.0.0a0/zeno_build/optimizers/__init__.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 zeno_build-0.0.0a0/zeno_build/optimizers/base.py
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 zeno_build-0.0.0a0/zeno_build/optimizers/random.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 zeno_build-0.0.0a0/zeno_build/optimizers/standard.py
--rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 zeno_build-0.0.0a0/zeno_build/optimizers/vizier.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 zeno_build-0.0.0a0/zeno_build/prompts/__init__.py
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 zeno_build-0.0.0a0/zeno_build/prompts/chat_prompt.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 zeno_build-0.0.0a0/zeno_build/prompts/prompt_utils.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 zeno_build-0.0.0a0/zeno_build/reporting/__init__.py
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 zeno_build-0.0.0a0/zeno_build/reporting/aggregate_results.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 zeno_build-0.0.0a0/zeno_build/reporting/visualize.py
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 zeno_build-0.0.0a0/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 zeno_build-0.0.0a0/LICENSE
--rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 zeno_build-0.0.0a0/README.md
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 zeno_build-0.0.0a0/pyproject.toml
--rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 zeno_build-0.0.0a0/PKG-INFO
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 zeno_build-0.0.0a1/zeno_build/__init__.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 zeno_build-0.0.0a1/zeno_build/cache_utils.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 zeno_build-0.0.0a1/zeno_build/version.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zeno_build-0.0.0a1/zeno_build/evaluation/__init__.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 zeno_build-0.0.0a1/zeno_build/evaluation/classification_metrics.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 zeno_build-0.0.0a1/zeno_build/evaluation/text_features/__init__.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 zeno_build-0.0.0a1/zeno_build/evaluation/text_features/exact_match.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 zeno_build-0.0.0a1/zeno_build/evaluation/text_features/length.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 zeno_build-0.0.0a1/zeno_build/evaluation/text_metrics/__init__.py
+-rw-r--r--   0        0        0    15356 2020-02-02 00:00:00.000000 zeno_build-0.0.0a1/zeno_build/evaluation/text_metrics/critique.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 zeno_build-0.0.0a1/zeno_build/experiments/__init__.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 zeno_build-0.0.0a1/zeno_build/experiments/experiment_run.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 zeno_build-0.0.0a1/zeno_build/experiments/search_space.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 zeno_build-0.0.0a1/zeno_build/models/__init__.py
+-rw-r--r--   0        0        0    11088 2020-02-02 00:00:00.000000 zeno_build-0.0.0a1/zeno_build/models/chat_generate.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 zeno_build-0.0.0a1/zeno_build/models/global_models.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 zeno_build-0.0.0a1/zeno_build/models/lm_config.py
+-rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 zeno_build-0.0.0a1/zeno_build/models/text_generate.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 zeno_build-0.0.0a1/zeno_build/optimizers/__init__.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 zeno_build-0.0.0a1/zeno_build/optimizers/base.py
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 zeno_build-0.0.0a1/zeno_build/optimizers/random.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 zeno_build-0.0.0a1/zeno_build/optimizers/standard.py
+-rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 zeno_build-0.0.0a1/zeno_build/optimizers/vizier.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 zeno_build-0.0.0a1/zeno_build/prompts/__init__.py
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 zeno_build-0.0.0a1/zeno_build/prompts/chat_prompt.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 zeno_build-0.0.0a1/zeno_build/prompts/prompt_utils.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 zeno_build-0.0.0a1/zeno_build/reporting/__init__.py
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 zeno_build-0.0.0a1/zeno_build/reporting/aggregate_results.py
+-rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 zeno_build-0.0.0a1/zeno_build/reporting/visualize.py
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 zeno_build-0.0.0a1/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 zeno_build-0.0.0a1/LICENSE
+-rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 zeno_build-0.0.0a1/README.md
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 zeno_build-0.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 zeno_build-0.0.0a1/PKG-INFO
```

### Comparing `zeno_build-0.0.0a0/zeno_build/cache_utils.py` & `zeno_build-0.0.0a1/zeno_build/cache_utils.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.0a0/zeno_build/evaluation/classification_metrics.py` & `zeno_build-0.0.0a1/zeno_build/evaluation/classification_metrics.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.0a0/zeno_build/evaluation/text_features/exact_match.py` & `zeno_build-0.0.0a1/zeno_build/evaluation/text_features/exact_match.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.0a0/zeno_build/evaluation/text_features/length.py` & `zeno_build-0.0.0a1/zeno_build/evaluation/text_features/length.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.0a0/zeno_build/evaluation/text_metrics/critique.py` & `zeno_build-0.0.0a1/zeno_build/evaluation/text_metrics/critique.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.0a0/zeno_build/experiments/search_space.py` & `zeno_build-0.0.0a1/zeno_build/experiments/search_space.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.0a0/zeno_build/models/chat_generate.py` & `zeno_build-0.0.0a1/zeno_build/models/chat_generate.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.0a0/zeno_build/models/lm_config.py` & `zeno_build-0.0.0a1/zeno_build/models/lm_config.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.0a0/zeno_build/models/text_generate.py` & `zeno_build-0.0.0a1/zeno_build/models/text_generate.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.0a0/zeno_build/optimizers/base.py` & `zeno_build-0.0.0a1/zeno_build/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.0a0/zeno_build/optimizers/random.py` & `zeno_build-0.0.0a1/zeno_build/optimizers/random.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.0a0/zeno_build/optimizers/vizier.py` & `zeno_build-0.0.0a1/zeno_build/optimizers/vizier.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.0a0/zeno_build/prompts/chat_prompt.py` & `zeno_build-0.0.0a1/zeno_build/prompts/chat_prompt.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.0a0/zeno_build/reporting/aggregate_results.py` & `zeno_build-0.0.0a1/zeno_build/reporting/aggregate_results.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.0a0/zeno_build/reporting/visualize.py` & `zeno_build-0.0.0a1/zeno_build/reporting/visualize.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,24 +12,26 @@
 def visualize(
     df: pd.DataFrame,
     labels: list[Any],
     results: list[ExperimentRun],
     view: str,
     data_column: str,
     functions: list[Callable],
+    zeno_config: ZenoParameters = ZenoParameters(),
 ) -> None:
     """Run Zeno to visualize the results of a parameter search run.
 
     Args:
         df: DataFrame with the data to visualize. Must contain "data_column" column.
         labels: List of ground truth labels
         results: List of dictionaries with model outputs
         view: The Zeno view to use for the data
         data_column: The column in the DataFrame with the data
         functions: List of functions to use in Zeno
+        zeno_config: Zeno configuration parameters
     """
     if len(df) != len(labels):
         raise ValueError("Length of data and labels must be equal.")
     if data_column not in df.columns:
         raise ValueError(f"Data column {data_column} not in DataFrame.")
     model_results: dict[str, ExperimentRun] = {}
     for i, res in enumerate(results):
@@ -59,9 +61,10 @@
         view=view,
         models=list(model_results.keys()),
         functions=[get_model] + functions,
         data_column=data_column,
         label_column="label",
         batch_size=100000,
     )
+    config = config.copy(update=zeno_config.dict())
 
     zeno(config)
```

### Comparing `zeno_build-0.0.0a0/.gitignore` & `zeno_build-0.0.0a1/.gitignore`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.0a0/LICENSE` & `zeno_build-0.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.0a0/README.md` & `zeno_build-0.0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.0a0/pyproject.toml` & `zeno_build-0.0.0a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.0a0/PKG-INFO` & `zeno_build-0.0.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeno_build
-Version: 0.0.0a0
+Version: 0.0.0a1
 Summary: A library for comparing multiple llm-based systems.
 Author-email: Ángel Alexander Cabrera <alex.cabrera@gmail.com>, Graham Neubig <neubig@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Zeno
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

