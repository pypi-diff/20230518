# Comparing `tmp/canals-0.2.0.tar.gz` & `tmp/canals-0.2.1.tar.gz`

## Comparing `canals-0.2.0.tar` & `canals-0.2.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 canals-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 canals-0.2.0/mkdocs.yml
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 canals-0.2.0/.github/workflows/api-docs.yml
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 canals-0.2.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 canals-0.2.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 canals-0.2.0/canals/__about__.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 canals-0.2.0/canals/__init__.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 canals-0.2.0/canals/errors.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 canals-0.2.0/canals/component/__init__.py
--rw-r--r--   0        0        0    10476 2020-02-02 00:00:00.000000 canals-0.2.0/canals/component/component.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 canals-0.2.0/canals/component/decorators.py
--rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 canals-0.2.0/canals/component/input_output.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 canals-0.2.0/canals/draw/__init__.py
--rw-r--r--   0        0        0     3348 2020-02-02 00:00:00.000000 canals-0.2.0/canals/draw/draw.py
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 canals-0.2.0/canals/draw/graphviz.py
--rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 canals-0.2.0/canals/draw/mermaid.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 canals-0.2.0/canals/pipeline/__init__.py
--rw-r--r--   0        0        0     9435 2020-02-02 00:00:00.000000 canals-0.2.0/canals/pipeline/_utils.py
--rw-r--r--   0        0        0    28710 2020-02-02 00:00:00.000000 canals-0.2.0/canals/pipeline/pipeline.py
--rw-r--r--   0        0        0     8747 2020-02-02 00:00:00.000000 canals-0.2.0/canals/pipeline/save_load.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 canals-0.2.0/canals/testing/__init__.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 canals-0.2.0/canals/testing/test_component.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 canals-0.2.0/docs/index.md
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 canals-0.2.0/docs/api-docs/component.md
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.2.0/docs/api-docs/draw.md
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 canals-0.2.0/docs/api-docs/pipeline.md
--rw-r--r--   0        0        0     9353 2020-02-02 00:00:00.000000 canals-0.2.0/docs/concepts/components.md
--rw-r--r--   0        0        0     4024 2020-02-02 00:00:00.000000 canals-0.2.0/docs/concepts/concepts.md
--rw-r--r--   0        0        0     7171 2020-02-02 00:00:00.000000 canals-0.2.0/docs/concepts/pipelines.md
--rw-r--r--   0        0        0    26250 2020-02-02 00:00:00.000000 canals-0.2.0/images/canals-logo-dark.png
--rw-r--r--   0        0        0    25601 2020-02-02 00:00:00.000000 canals-0.2.0/images/canals-logo-light.png
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.2.0/test/__init__.py
--rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 canals-0.2.0/test/test_save_load.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 canals-0.2.0/test/pipelines/__init__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.2.0/test/pipelines/integration/__init__.py
--rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 canals-0.2.0/test/pipelines/integration/test_complex_pipeline.py
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 canals-0.2.0/test/pipelines/integration/test_fixed_decision_and_merge_pipeline.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 canals-0.2.0/test/pipelines/integration/test_fixed_decision_pipeline.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 canals-0.2.0/test/pipelines/integration/test_fixed_merging_pipeline.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 canals-0.2.0/test/pipelines/integration/test_linear_pipeline.py
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 canals-0.2.0/test/pipelines/integration/test_looping_and_merge_pipeline.py
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 canals-0.2.0/test/pipelines/integration/test_looping_pipeline.py
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 canals-0.2.0/test/pipelines/integration/test_parallel_branches_pipeline.py
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 canals-0.2.0/test/pipelines/integration/test_variable_decision_and_merge_pipeline.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 canals-0.2.0/test/pipelines/integration/test_variable_decision_pipeline.py
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 canals-0.2.0/test/pipelines/integration/test_variable_merging_pipeline.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.2.0/test/pipelines/unit/__init__.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 canals-0.2.0/test/sample_components/__init__.py
--rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 canals-0.2.0/test/sample_components/test_accumulate.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 canals-0.2.0/test/sample_components/test_add_value.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 canals-0.2.0/test/sample_components/test_double.py
--rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 canals-0.2.0/test/sample_components/test_greet.py
--rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 canals-0.2.0/test/sample_components/test_merge_loop.py
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 canals-0.2.0/test/sample_components/test_parity.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 canals-0.2.0/test/sample_components/test_remainder.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 canals-0.2.0/test/sample_components/test_repeat.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 canals-0.2.0/test/sample_components/test_subtract.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 canals-0.2.0/test/sample_components/test_sum.py
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 canals-0.2.0/test/sample_components/test_threshold.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 canals-0.2.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 canals-0.2.0/LICENSE
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 canals-0.2.0/README.md
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 canals-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4285 2020-02-02 00:00:00.000000 canals-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 canals-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 canals-0.2.1/mkdocs.yml
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 canals-0.2.1/.github/workflows/api-docs.yml
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 canals-0.2.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 canals-0.2.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 canals-0.2.1/canals/__about__.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 canals-0.2.1/canals/__init__.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 canals-0.2.1/canals/errors.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 canals-0.2.1/canals/component/__init__.py
+-rw-r--r--   0        0        0    10476 2020-02-02 00:00:00.000000 canals-0.2.1/canals/component/component.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 canals-0.2.1/canals/component/decorators.py
+-rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 canals-0.2.1/canals/component/input_output.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 canals-0.2.1/canals/draw/__init__.py
+-rw-r--r--   0        0        0     3348 2020-02-02 00:00:00.000000 canals-0.2.1/canals/draw/draw.py
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 canals-0.2.1/canals/draw/graphviz.py
+-rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 canals-0.2.1/canals/draw/mermaid.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 canals-0.2.1/canals/pipeline/__init__.py
+-rw-r--r--   0        0        0     9435 2020-02-02 00:00:00.000000 canals-0.2.1/canals/pipeline/_utils.py
+-rw-r--r--   0        0        0    28710 2020-02-02 00:00:00.000000 canals-0.2.1/canals/pipeline/pipeline.py
+-rw-r--r--   0        0        0     8747 2020-02-02 00:00:00.000000 canals-0.2.1/canals/pipeline/save_load.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 canals-0.2.1/canals/testing/__init__.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 canals-0.2.1/canals/testing/test_component.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 canals-0.2.1/docs/index.md
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 canals-0.2.1/docs/api-docs/component.md
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.2.1/docs/api-docs/draw.md
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 canals-0.2.1/docs/api-docs/pipeline.md
+-rw-r--r--   0        0        0     9353 2020-02-02 00:00:00.000000 canals-0.2.1/docs/concepts/components.md
+-rw-r--r--   0        0        0     4024 2020-02-02 00:00:00.000000 canals-0.2.1/docs/concepts/concepts.md
+-rw-r--r--   0        0        0     7171 2020-02-02 00:00:00.000000 canals-0.2.1/docs/concepts/pipelines.md
+-rw-r--r--   0        0        0    26250 2020-02-02 00:00:00.000000 canals-0.2.1/images/canals-logo-dark.png
+-rw-r--r--   0        0        0    25601 2020-02-02 00:00:00.000000 canals-0.2.1/images/canals-logo-light.png
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.2.1/test/__init__.py
+-rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 canals-0.2.1/test/test_save_load.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 canals-0.2.1/test/pipelines/__init__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.2.1/test/pipelines/integration/__init__.py
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 canals-0.2.1/test/pipelines/integration/test_complex_pipeline.py
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 canals-0.2.1/test/pipelines/integration/test_fixed_decision_and_merge_pipeline.py
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 canals-0.2.1/test/pipelines/integration/test_fixed_decision_pipeline.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 canals-0.2.1/test/pipelines/integration/test_fixed_merging_pipeline.py
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 canals-0.2.1/test/pipelines/integration/test_linear_pipeline.py
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 canals-0.2.1/test/pipelines/integration/test_looping_and_merge_pipeline.py
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 canals-0.2.1/test/pipelines/integration/test_looping_pipeline.py
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 canals-0.2.1/test/pipelines/integration/test_parallel_branches_pipeline.py
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 canals-0.2.1/test/pipelines/integration/test_variable_decision_and_merge_pipeline.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 canals-0.2.1/test/pipelines/integration/test_variable_decision_pipeline.py
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 canals-0.2.1/test/pipelines/integration/test_variable_merging_pipeline.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.2.1/test/pipelines/unit/__init__.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 canals-0.2.1/test/sample_components/__init__.py
+-rw-r--r--   0        0        0     4827 2020-02-02 00:00:00.000000 canals-0.2.1/test/sample_components/test_accumulate.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 canals-0.2.1/test/sample_components/test_add_value.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 canals-0.2.1/test/sample_components/test_double.py
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 canals-0.2.1/test/sample_components/test_greet.py
+-rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 canals-0.2.1/test/sample_components/test_merge_loop.py
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 canals-0.2.1/test/sample_components/test_parity.py
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 canals-0.2.1/test/sample_components/test_remainder.py
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 canals-0.2.1/test/sample_components/test_repeat.py
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 canals-0.2.1/test/sample_components/test_subtract.py
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 canals-0.2.1/test/sample_components/test_sum.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 canals-0.2.1/test/sample_components/test_threshold.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 canals-0.2.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 canals-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 canals-0.2.1/README.md
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 canals-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4295 2020-02-02 00:00:00.000000 canals-0.2.1/PKG-INFO
```

### Comparing `canals-0.2.0/.pre-commit-config.yaml` & `canals-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `canals-0.2.0/mkdocs.yml` & `canals-0.2.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `canals-0.2.0/.github/workflows/tests.yml` & `canals-0.2.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `canals-0.2.0/canals/component/component.py` & `canals-0.2.1/canals/component/component.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.0/canals/component/decorators.py` & `canals-0.2.1/canals/component/decorators.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.0/canals/component/input_output.py` & `canals-0.2.1/canals/component/input_output.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.0/canals/draw/draw.py` & `canals-0.2.1/canals/draw/draw.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.0/canals/draw/graphviz.py` & `canals-0.2.1/canals/draw/graphviz.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.0/canals/draw/mermaid.py` & `canals-0.2.1/canals/draw/mermaid.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.0/canals/pipeline/_utils.py` & `canals-0.2.1/canals/pipeline/_utils.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.0/canals/pipeline/pipeline.py` & `canals-0.2.1/canals/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.0/canals/pipeline/save_load.py` & `canals-0.2.1/canals/pipeline/save_load.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.0/docs/index.md` & `canals-0.2.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `canals-0.2.0/docs/concepts/components.md` & `canals-0.2.1/docs/concepts/components.md`

 * *Files identical despite different names*

### Comparing `canals-0.2.0/docs/concepts/concepts.md` & `canals-0.2.1/docs/concepts/concepts.md`

 * *Files identical despite different names*

### Comparing `canals-0.2.0/docs/concepts/pipelines.md` & `canals-0.2.1/docs/concepts/pipelines.md`

 * *Files identical despite different names*

### Comparing `canals-0.2.0/images/canals-logo-dark.png` & `canals-0.2.1/images/canals-logo-dark.png`

 * *Files identical despite different names*

### Comparing `canals-0.2.0/images/canals-logo-light.png` & `canals-0.2.1/images/canals-logo-light.png`

 * *Files identical despite different names*

### Comparing `canals-0.2.0/test/test_save_load.py` & `canals-0.2.1/test/test_save_load.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.0/test/pipelines/integration/test_complex_pipeline.py` & `canals-0.2.1/test/pipelines/integration/test_complex_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.0/test/pipelines/integration/test_fixed_decision_and_merge_pipeline.py` & `canals-0.2.1/test/pipelines/integration/test_fixed_decision_and_merge_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.0/test/pipelines/integration/test_fixed_decision_pipeline.py` & `canals-0.2.1/test/pipelines/integration/test_fixed_decision_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.0/test/pipelines/integration/test_fixed_merging_pipeline.py` & `canals-0.2.1/test/pipelines/integration/test_fixed_merging_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.0/test/pipelines/integration/test_linear_pipeline.py` & `canals-0.2.1/test/pipelines/integration/test_linear_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.0/test/pipelines/integration/test_looping_and_merge_pipeline.py` & `canals-0.2.1/test/pipelines/integration/test_looping_and_merge_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.0/test/pipelines/integration/test_looping_pipeline.py` & `canals-0.2.1/test/pipelines/integration/test_looping_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.0/test/pipelines/integration/test_parallel_branches_pipeline.py` & `canals-0.2.1/test/pipelines/integration/test_parallel_branches_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.0/test/pipelines/integration/test_variable_decision_and_merge_pipeline.py` & `canals-0.2.1/test/pipelines/integration/test_variable_decision_and_merge_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.0/test/pipelines/integration/test_variable_decision_pipeline.py` & `canals-0.2.1/test/pipelines/integration/test_variable_decision_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.0/test/pipelines/integration/test_variable_merging_pipeline.py` & `canals-0.2.1/test/pipelines/integration/test_variable_merging_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.0/test/sample_components/__init__.py` & `canals-0.2.1/test/sample_components/__init__.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.0/test/sample_components/test_accumulate.py` & `canals-0.2.1/test/sample_components/test_accumulate.py`

 * *Files 9% similar despite different names*

```diff
@@ -81,21 +81,24 @@
 
 
 def my_subtract(first, second):
     return first - second
 
 
 class TestAccumulate(BaseTestComponent):
-    @pytest.fixture
-    def components(self):
-        return [
-            Accumulate(),
-            Accumulate(function=my_subtract),
-            Accumulate(function="test.sample_components.test_accumulate.my_subtract"),
-        ]
+    def test_saveload_default(self, tmp_path):
+        self.assert_can_be_saved_and_loaded_in_pipeline(Accumulate(), tmp_path)
+
+    def test_saveload_function_as_string(self, tmp_path):
+        self.assert_can_be_saved_and_loaded_in_pipeline(
+            Accumulate(function="test.sample_components.test_accumulate.my_subtract"), tmp_path
+        )
+
+    def test_saveload_function_as_callable(self, tmp_path):
+        self.assert_can_be_saved_and_loaded_in_pipeline(Accumulate(function=my_subtract), tmp_path)
 
     def test_accumulate_default(self):
         component = Accumulate()
         results = component.run(Accumulate.Input(value=10))
         assert results == Accumulate.Output(value=10)
         assert component.state == 10
```

### Comparing `canals-0.2.0/test/sample_components/test_add_value.py` & `canals-0.2.1/test/sample_components/test_add_value.py`

 * *Files 25% similar despite different names*

```diff
@@ -31,17 +31,18 @@
             self.defaults = {"add": add}
 
     def run(self, data: Input) -> Output:
         return AddFixedValue.Output(value=data.value + data.add)
 
 
 class TestAddFixedValue(BaseTestComponent):
-    @pytest.fixture
-    def components(self):
-        return [AddFixedValue(), AddFixedValue(add=2)]
+    def test_saveload_default(self, tmp_path):
+        self.assert_can_be_saved_and_loaded_in_pipeline(AddFixedValue(), tmp_path)
 
-    def test_addvalue(self):
+    def test_saveload_add(self, tmp_path):
+        self.assert_can_be_saved_and_loaded_in_pipeline(AddFixedValue(add=2), tmp_path)
 
+    def test_addvalue(self):
         component = AddFixedValue()
         results = component.run(AddFixedValue.Input(value=50, add=10))
         assert results == AddFixedValue.Output(value=60)
         assert component.init_parameters == {}
```

### Comparing `canals-0.2.0/test/sample_components/test_double.py` & `canals-0.2.1/test/sample_components/test_sum.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,52 @@
 # SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
+from typing import List
+
 from dataclasses import dataclass
 
 import pytest
 
-from canals.component import component, ComponentInput, ComponentOutput
 from canals.testing import BaseTestComponent
+from canals.component import component, VariadicComponentInput, ComponentOutput
 
 
 @component
-class Double:
+class Sum:
     """
-    Doubles the input value.
+    Sums the values of all the input connections together.
     """
 
     @dataclass
-    class Input(ComponentInput):
-        value: int
+    class Input(VariadicComponentInput):
+        values: List[int]
 
     @dataclass
     class Output(ComponentOutput):
-        value: int
+        total: int
 
     def run(self, data: Input) -> Output:
-        """
-        Doubles the input value
-        """
-        return Double.Output(value=data.value * 2)
+        return Sum.Output(total=sum(data.values))
 
 
-import pytest
-from canals.testing import BaseTestComponent
+class TestSum(BaseTestComponent):
+    def test_saveload_default(self, tmp_path):
+        self.assert_can_be_saved_and_loaded_in_pipeline(Sum(), tmp_path)
 
+    def test_sum_no_values(self):
+        component = Sum()
+        results = component.run(Sum.Input())
+        assert results == Sum.Output(total=0)
+        assert component.init_parameters == {}
+
+    def test_sum_one_value(self):
+        component = Sum()
+        results = component.run(Sum.Input(10))
+        assert results == Sum.Output(total=10)
+        assert component.init_parameters == {}
 
-class TestDouble(BaseTestComponent):
-    @pytest.fixture
-    def components(self):
-        return [Double()]
-
-    def test_double_default(self):
-        component = Double()
-        results = component.run(Double.Input(value=10))
-        assert results == Double.Output(value=20)
+    def test_sum_few_values(self):
+        component = Sum()
+        results = component.run(Sum.Input(10, 11, 12))
+        assert results == Sum.Output(total=33)
         assert component.init_parameters == {}
```

### Comparing `canals-0.2.0/test/sample_components/test_greet.py` & `canals-0.2.1/test/sample_components/test_greet.py`

 * *Files 17% similar despite different names*

```diff
@@ -54,22 +54,27 @@
             raise ValueError(f"This log level does not exist: {data.log_level}")
 
         logger.log(level=level, msg=data.message.format(value=data.value))
         return Greet.Output(value=data.value)
 
 
 class TestGreet(BaseTestComponent):
-    @pytest.fixture
-    def components(self):
-        return [
-            Greet(),
-            Greet(message="Hello, that's {value}"),
-            Greet(log_level="WARNING"),
-            Greet(message="Hello, that's {value}", log_level="WARNING"),
-        ]
+    def test_saveload_default(self, tmp_path):
+        self.assert_can_be_saved_and_loaded_in_pipeline(Greet(), tmp_path)
+
+    def test_saveload_message(self, tmp_path):
+        self.assert_can_be_saved_and_loaded_in_pipeline(Greet(message="Hello, that's {value}"), tmp_path)
+
+    def test_saveload_loglevel(self, tmp_path):
+        self.assert_can_be_saved_and_loaded_in_pipeline(Greet(log_level="WARNING"), tmp_path)
+
+    def test_saveload_message_and_loglevel(self, tmp_path):
+        self.assert_can_be_saved_and_loaded_in_pipeline(
+            Greet(message="Hello, that's {value}", log_level="WARNING"), tmp_path
+        )
 
     def test_greet_message(self, caplog):
         caplog.set_level(logging.WARNING)
         component = Greet()
         results = component.run(Greet.Input(value=10, message="Hello, that's {value}", log_level="WARNING"))
         assert results == Greet.Output(value=10)
         assert "Hello, that's 10" in caplog.text
```

### Comparing `canals-0.2.0/test/sample_components/test_merge_loop.py` & `canals-0.2.1/test/sample_components/test_merge_loop.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 # SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
-from typing import List
+from typing import List, Union
+import builtins
 
 from dataclasses import dataclass
 
-import pytest
-
 from canals.component import component, VariadicComponentInput, ComponentOutput
 from canals.testing import BaseTestComponent
 
 
 @component
 class MergeLoop:
     """
     Takes two input components and returns the first one that is not None.
     In case both received a value, priority is given to 'first'.
     """
 
-    def __init__(self, expected_type: type):
-        self.expected_type = expected_type
-        self.init_parameters = {"expected_type": expected_type.__name__}
+    def __init__(self, expected_type: Union[type, str]):
+        if isinstance(expected_type, str):
+            type_ = getattr(builtins, expected_type)
+        else:
+            type_ = expected_type
+
+        self.expected_type = type_
+        self.init_parameters = {"expected_type": type_.__name__}
 
     @property
     def input_type(self):
         @dataclass
         class Input(VariadicComponentInput):
             values: List[self.expected_type]  # type: ignore
 
@@ -47,23 +51,24 @@
         for v in data.values:
             if v is not None:
                 return self.output_type(value=v)
         return self.output_type(value=None)
 
 
 class TestMergeLoop(BaseTestComponent):
-    @pytest.fixture
-    def components(self):
+    def test_saveload_builtin_type(self, tmp_path):
+        self.assert_can_be_saved_and_loaded_in_pipeline(MergeLoop(expected_type=int), tmp_path)
 
-        # Serialization is broken :'(
-        return [
-            # MergeLoop(expected_type=int),
-            # MergeLoop(expected_type=str),
-            # MergeLoop(expected_type=List[str])
-        ]
+    # TODO
+    # def test_saveload_complex_type(self, tmp_path):
+    #     self.assert_can_be_saved_and_loaded_in_pipeline(MergeLoop(expected_type=List[int]), tmp_path)
+
+    # def test_saveload_object_type(self, tmp_path):
+    #     class MyObject: ...
+    #     self.assert_can_be_saved_and_loaded_in_pipeline(MergeLoop(expected_type=MyObject()), tmp_path)
 
     def test_merge_first(self):
         component = MergeLoop(expected_type=int)
         results = component.run(component.input_type(5, None))
         assert results.__dict__ == component.output_type(value=5).__dict__
 
     def test_merge_second(self):
```

### Comparing `canals-0.2.0/test/sample_components/test_parity.py` & `canals-0.2.1/test/sample_components/test_parity.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,17 +32,16 @@
         remainder = data.value % 2
         if remainder:
             return Parity.Output(odd=data.value)
         return Parity.Output(even=data.value)
 
 
 class TestParity(BaseTestComponent):
-    @pytest.fixture
-    def components(self):
-        return [Parity()]
+    def test_saveload_default(self, tmp_path):
+        self.assert_can_be_saved_and_loaded_in_pipeline(Parity(), tmp_path)
 
     def test_parity(self):
         component = Parity()
         results = component.run(Parity.Input(value=1))
         assert results == Parity.Output(odd=1)
         results = component.run(Parity.Input(value=2))
         assert results == Parity.Output(even=2)
```

### Comparing `canals-0.2.0/test/sample_components/test_remainder.py` & `canals-0.2.1/test/sample_components/test_remainder.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,17 +42,19 @@
         remainder = data.value % self.divisor
         output = self.output_type()
         setattr(output, f"remainder_is_{remainder}", data.value)
         return output
 
 
 class TestRemainder(BaseTestComponent):
-    @pytest.fixture
-    def components(self):
-        return [Remainder(), Remainder(divisor=1)]
+    def test_saveload_default(self, tmp_path):
+        self.assert_can_be_saved_and_loaded_in_pipeline(Remainder(), tmp_path)
+
+    def test_saveload_divisor(self, tmp_path):
+        self.assert_can_be_saved_and_loaded_in_pipeline(Remainder(divisor=1), tmp_path)
 
     def test_remainder_default(self):
         component = Remainder()
         results = component.run(Remainder.Input(value=3))
         assert results == component.output_type(remainder_is_1=3)
 
     def test_remainder_with_divisor(self):
```

### Comparing `canals-0.2.0/test/sample_components/test_repeat.py` & `canals-0.2.1/test/sample_components/test_repeat.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,17 +35,19 @@
         output_dataclass = self.output_type()
         for output in self.outputs:
             setattr(output_dataclass, output, data.value)
         return output_dataclass
 
 
 class TestRepeat(BaseTestComponent):
-    @pytest.fixture
-    def components(self):
-        return [Repeat(), Repeat(outputs=["one", "two"])]
+    def test_saveload_default(self, tmp_path):
+        self.assert_can_be_saved_and_loaded_in_pipeline(Repeat(), tmp_path)
+
+    def test_saveload_outputs(self, tmp_path):
+        self.assert_can_be_saved_and_loaded_in_pipeline(Repeat(outputs=["one", "two"]), tmp_path)
 
     def test_repeat_default(self):
         component = Repeat()
         results = component.run(Repeat.Input(value=10))
         assert results == component.output_type(output_1=10, output_2=10, output_3=10)
         assert component.init_parameters == {}
```

### Comparing `canals-0.2.0/test/sample_components/test_subtract.py` & `canals-0.2.1/test/sample_components/test_subtract.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,16 +29,15 @@
         :param first_value: name of the connection carrying the value to subtract from.
         :param second_value: name of the connection carrying the value to subtract.
         """
         return Subtract.Output(difference=data.first_value - data.second_value)
 
 
 class TestSubtract(BaseTestComponent):
-    @pytest.fixture
-    def components(self):
-        return [Subtract()]
+    def test_saveload_default(self, tmp_path):
+        self.assert_can_be_saved_and_loaded_in_pipeline(Subtract(), tmp_path)
 
     def test_subtract(self):
         component = Subtract()
         results = component.run(Subtract.Input(first_value=10, second_value=7))
         assert results == Subtract.Output(difference=3)
         assert component.init_parameters == {}
```

### Comparing `canals-0.2.0/test/sample_components/test_threshold.py` & `canals-0.2.1/test/sample_components/test_threshold.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,17 +42,19 @@
     def run(self, data: Input) -> Output:
         if data.value < data.threshold:
             return Threshold.Output(above=None, below=data.value)  # type: ignore
         return Threshold.Output(above=data.value, below=None)  # type: ignore
 
 
 class TestThreshold(BaseTestComponent):
-    @pytest.fixture
-    def components(self):
-        return [Threshold()]
+    def test_saveload_default(self, tmp_path):
+        self.assert_can_be_saved_and_loaded_in_pipeline(Threshold(), tmp_path)
+
+    def test_saveload_threshold(self, tmp_path):
+        self.assert_can_be_saved_and_loaded_in_pipeline(Threshold(threshold=3), tmp_path)
 
     def test_threshold(self):
         component = Threshold()
 
         results = component.run(Threshold.Input(value=5, threshold=10))
         assert results == Threshold.Output(above=None, below=5)
```

### Comparing `canals-0.2.0/.gitignore` & `canals-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `canals-0.2.0/LICENSE` & `canals-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `canals-0.2.0/README.md` & `canals-0.2.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 
 [![PyPI - Version](https://img.shields.io/pypi/v/canals.svg)](https://pypi.org/project/canals)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/canals.svg)](https://pypi.org/project/canals)
 <a href="https://github.com/deepset-ai/canals/actions/workflows/tests.yml">
     <img alt="Tests" src="https://github.com/deepset-ai/canals/workflows/Tests/badge.svg?branch=main">
 </a>
 [![Coverage Status](https://coveralls.io/repos/github/deepset-ai/canals/badge.svg?branch=main)](https://coveralls.io/github/deepset-ai/canals?branch=main)
-<a href="https://docs.haystack.deepset.ai">
+<a href="https://deepset-ai.github.io/canals/">
     <img alt="Documentation" src="https://img.shields.io/website?label=documentation&up_message=online&url=https%3A%2F%2Fdeepset-ai.github.io/canals/">
 </a>
-<a href="https://github.com/deepset-ai/haystack/commits/main">
+<a href="https://github.com/deepset-ai/canals/commits/main">
     <img alt="Last commit" src="https://img.shields.io/github/last-commit/deepset-ai/canals">
 </a>
 <a href="https://pepy.tech/project/canals">
-    <img alt="Downloads" src="https://pepy.tech/badge/canals/month">
+    <img alt="Monthly Downloads" src="https://pepy.tech/badge/canals/month">
 </a>
 <a href="https://github.com/deepset-ai/canals">
     <img alt="Stars" src="https://shields.io/github/stars/deepset-ai/canals?style=social">
 </a>
 <a href="https://ossinsight.io/analyze/deepset-ai/canals">
     <img alt="Stats" src="https://img.shields.io/badge/Stats-updated-blue">
 </a>
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
 # Canals
 
 [![PyPI - Version](https://img.shields.io/pypi/v/canals.svg)](https://pypi.org/
 project/canals) [![PyPI - Python Version](https://img.shields.io/pypi/
 pyversions/canals.svg)](https://pypi.org/project/canals) [Tests] [![Coverage
 Status](https://coveralls.io/repos/github/deepset-ai/canals/
 badge.svg?branch=main)](https://coveralls.io/github/deepset-ai/
-canals?branch=main) [Documentation] [Last_commit] [Downloads] [Stars] [Stats]
-Canals is a **component orchestration engine**. Components are Python objects
-that can execute a task, like reading a file, performing calculations, or
-making API calls. Canals connects these objects together: it builds a graph of
-components and takes care of managing their execution order, making sure that
-each object receives the input it expects from the other components of the
+canals?branch=main) [Documentation] [Last_commit] [Monthly_Downloads] [Stars]
+[Stats] Canals is a **component orchestration engine**. Components are Python
+objects that can execute a task, like reading a file, performing calculations,
+or making API calls. Canals connects these objects together: it builds a graph
+of components and takes care of managing their execution order, making sure
+that each object receives the input it expects from the other components of the
 pipeline. Canals powers version 2.0 of the [Haystack framework](https://
 github.com/deepset-ai/haystack). ## Installation Running: ```console pip
 install canals ``` gives you the bare minimum necessary to run Canals. To be
 able to draw pipelines, please make sure you have either an internet connection
 (to reach the Mermaid graph renderer at `https://mermaid.ink`) or [graphviz]
 (https://graphviz.org/download/) installed and then install Canals as: ###
 Mermaid ```console pip install canals[mermaid] ``` ### GraphViz ```console sudo
```

### Comparing `canals-0.2.0/pyproject.toml` & `canals-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `canals-0.2.0/PKG-INFO` & `canals-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canals
-Version: 0.2.0
+Version: 0.2.1
 Summary: A component orchestration engine for Haystack
 Project-URL: Documentation, https://github.com/deepset-ai/canals#readme
 Project-URL: Issues, https://github.com/deepset-ai/canals/issues
 Project-URL: Source, https://github.com/deepset-ai/canals
 Author-email: ZanSara <sara.zanzottera@deepset.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -47,22 +47,22 @@
 
 [![PyPI - Version](https://img.shields.io/pypi/v/canals.svg)](https://pypi.org/project/canals)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/canals.svg)](https://pypi.org/project/canals)
 <a href="https://github.com/deepset-ai/canals/actions/workflows/tests.yml">
     <img alt="Tests" src="https://github.com/deepset-ai/canals/workflows/Tests/badge.svg?branch=main">
 </a>
 [![Coverage Status](https://coveralls.io/repos/github/deepset-ai/canals/badge.svg?branch=main)](https://coveralls.io/github/deepset-ai/canals?branch=main)
-<a href="https://docs.haystack.deepset.ai">
+<a href="https://deepset-ai.github.io/canals/">
     <img alt="Documentation" src="https://img.shields.io/website?label=documentation&up_message=online&url=https%3A%2F%2Fdeepset-ai.github.io/canals/">
 </a>
-<a href="https://github.com/deepset-ai/haystack/commits/main">
+<a href="https://github.com/deepset-ai/canals/commits/main">
     <img alt="Last commit" src="https://img.shields.io/github/last-commit/deepset-ai/canals">
 </a>
 <a href="https://pepy.tech/project/canals">
-    <img alt="Downloads" src="https://pepy.tech/badge/canals/month">
+    <img alt="Monthly Downloads" src="https://pepy.tech/badge/canals/month">
 </a>
 <a href="https://github.com/deepset-ai/canals">
     <img alt="Stars" src="https://shields.io/github/stars/deepset-ai/canals?style=social">
 </a>
 <a href="https://ossinsight.io/analyze/deepset-ai/canals">
     <img alt="Stats" src="https://img.shields.io/badge/Stats-updated-blue">
 </a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: canals Version: 0.2.0 Summary: A component
+Metadata-Version: 2.1 Name: canals Version: 0.2.1 Summary: A component
 orchestration engine for Haystack Project-URL: Documentation, https://
 github.com/deepset-ai/canals#readme Project-URL: Issues, https://github.com/
 deepset-ai/canals/issues Project-URL: Source, https://github.com/deepset-ai/
 canals Author-email: ZanSara
 zanzottera@deepset.ai> License-Expression: Apache-2.0 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha Classifier: License :: Freely
 Distributable Classifier: License :: OSI Approved :: Apache Software License
@@ -23,20 +23,20 @@
 text/markdown # Canals
 
 [![PyPI - Version](https://img.shields.io/pypi/v/canals.svg)](https://pypi.org/
 project/canals) [![PyPI - Python Version](https://img.shields.io/pypi/
 pyversions/canals.svg)](https://pypi.org/project/canals) [Tests] [![Coverage
 Status](https://coveralls.io/repos/github/deepset-ai/canals/
 badge.svg?branch=main)](https://coveralls.io/github/deepset-ai/
-canals?branch=main) [Documentation] [Last_commit] [Downloads] [Stars] [Stats]
-Canals is a **component orchestration engine**. Components are Python objects
-that can execute a task, like reading a file, performing calculations, or
-making API calls. Canals connects these objects together: it builds a graph of
-components and takes care of managing their execution order, making sure that
-each object receives the input it expects from the other components of the
+canals?branch=main) [Documentation] [Last_commit] [Monthly_Downloads] [Stars]
+[Stats] Canals is a **component orchestration engine**. Components are Python
+objects that can execute a task, like reading a file, performing calculations,
+or making API calls. Canals connects these objects together: it builds a graph
+of components and takes care of managing their execution order, making sure
+that each object receives the input it expects from the other components of the
 pipeline. Canals powers version 2.0 of the [Haystack framework](https://
 github.com/deepset-ai/haystack). ## Installation Running: ```console pip
 install canals ``` gives you the bare minimum necessary to run Canals. To be
 able to draw pipelines, please make sure you have either an internet connection
 (to reach the Mermaid graph renderer at `https://mermaid.ink`) or [graphviz]
 (https://graphviz.org/download/) installed and then install Canals as: ###
 Mermaid ```console pip install canals[mermaid] ``` ### GraphViz ```console sudo
```

