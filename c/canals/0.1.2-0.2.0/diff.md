# Comparing `tmp/canals-0.1.2.tar.gz` & `tmp/canals-0.2.0.tar.gz`

## Comparing `canals-0.1.2.tar` & `canals-0.2.0.tar`

### file list

```diff
@@ -1,62 +1,64 @@
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 canals-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 canals-0.1.2/mkdocs.yml
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 canals-0.1.2/.github/workflows/api-docs.yml
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 canals-0.1.2/.github/workflows/release.yml
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 canals-0.1.2/.github/workflows/tests.yml
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 canals-0.1.2/canals/__about__.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 canals-0.1.2/canals/__init__.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 canals-0.1.2/canals/errors.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 canals-0.1.2/canals/component/__init__.py
--rw-r--r--   0        0        0     8469 2020-02-02 00:00:00.000000 canals-0.1.2/canals/component/component.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 canals-0.1.2/canals/component/save_init_params.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 canals-0.1.2/canals/draw/__init__.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 canals-0.1.2/canals/draw/draw.py
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 canals-0.1.2/canals/draw/graphviz.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 canals-0.1.2/canals/draw/mermaid.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 canals-0.1.2/canals/pipeline/__init__.py
--rw-r--r--   0        0        0     7966 2020-02-02 00:00:00.000000 canals-0.1.2/canals/pipeline/_utils.py
--rw-r--r--   0        0        0    28188 2020-02-02 00:00:00.000000 canals-0.1.2/canals/pipeline/pipeline.py
--rw-r--r--   0        0        0     8637 2020-02-02 00:00:00.000000 canals-0.1.2/canals/pipeline/save_load.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 canals-0.1.2/canals/testing/__init__.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 canals-0.1.2/canals/testing/test_component.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 canals-0.1.2/docs/index.md
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 canals-0.1.2/docs/api-docs/component.md
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.1.2/docs/api-docs/draw.md
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 canals-0.1.2/docs/api-docs/pipeline.md
--rw-r--r--   0        0        0     7458 2020-02-02 00:00:00.000000 canals-0.1.2/docs/concepts/components.md
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 canals-0.1.2/docs/concepts/concepts.md
--rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 canals-0.1.2/docs/concepts/pipelines.md
--rw-r--r--   0        0        0    26250 2020-02-02 00:00:00.000000 canals-0.1.2/images/canals-logo-dark.png
--rw-r--r--   0        0        0    25601 2020-02-02 00:00:00.000000 canals-0.1.2/images/canals-logo-light.png
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 canals-0.1.2/test/__init__.py
--rw-r--r--   0        0        0     6547 2020-02-02 00:00:00.000000 canals-0.1.2/test/test_save_load.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 canals-0.1.2/test/pipelines/integration/__init__.py
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 canals-0.1.2/test/pipelines/integration/test_complex_pipeline.py
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 canals-0.1.2/test/pipelines/integration/test_fixed_decision_and_merge_pipeline.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 canals-0.1.2/test/pipelines/integration/test_fixed_decision_pipeline.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 canals-0.1.2/test/pipelines/integration/test_fixed_merging_pipeline.py
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 canals-0.1.2/test/pipelines/integration/test_linear_pipeline.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 canals-0.1.2/test/pipelines/integration/test_looping_and_merge_pipeline.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 canals-0.1.2/test/pipelines/integration/test_looping_pipeline.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 canals-0.1.2/test/pipelines/integration/test_parallel_branches_pipeline.py
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 canals-0.1.2/test/pipelines/integration/test_variable_decision_and_merge_pipeline.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 canals-0.1.2/test/pipelines/integration/test_variable_decision_pipeline.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 canals-0.1.2/test/pipelines/integration/test_variable_merging_pipeline.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 canals-0.1.2/test/pipelines/unit/__init__.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 canals-0.1.2/test/test_components/__init__.py
--rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 canals-0.1.2/test/test_components/test_accumulate.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 canals-0.1.2/test/test_components/test_add_value.py
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 canals-0.1.2/test/test_components/test_double.py
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 canals-0.1.2/test/test_components/test_greet.py
--rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 canals-0.1.2/test/test_components/test_merge_loop.py
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 canals-0.1.2/test/test_components/test_parity.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 canals-0.1.2/test/test_components/test_remainder.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 canals-0.1.2/test/test_components/test_repeat.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 canals-0.1.2/test/test_components/test_subtract.py
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 canals-0.1.2/test/test_components/test_sum.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 canals-0.1.2/test/test_components/test_threshold.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 canals-0.1.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 canals-0.1.2/LICENSE
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 canals-0.1.2/README.md
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 canals-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3181 2020-02-02 00:00:00.000000 canals-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 canals-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 canals-0.2.0/mkdocs.yml
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 canals-0.2.0/.github/workflows/api-docs.yml
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 canals-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 canals-0.2.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 canals-0.2.0/canals/__about__.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 canals-0.2.0/canals/__init__.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 canals-0.2.0/canals/errors.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 canals-0.2.0/canals/component/__init__.py
+-rw-r--r--   0        0        0    10476 2020-02-02 00:00:00.000000 canals-0.2.0/canals/component/component.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 canals-0.2.0/canals/component/decorators.py
+-rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 canals-0.2.0/canals/component/input_output.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 canals-0.2.0/canals/draw/__init__.py
+-rw-r--r--   0        0        0     3348 2020-02-02 00:00:00.000000 canals-0.2.0/canals/draw/draw.py
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 canals-0.2.0/canals/draw/graphviz.py
+-rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 canals-0.2.0/canals/draw/mermaid.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 canals-0.2.0/canals/pipeline/__init__.py
+-rw-r--r--   0        0        0     9435 2020-02-02 00:00:00.000000 canals-0.2.0/canals/pipeline/_utils.py
+-rw-r--r--   0        0        0    28710 2020-02-02 00:00:00.000000 canals-0.2.0/canals/pipeline/pipeline.py
+-rw-r--r--   0        0        0     8747 2020-02-02 00:00:00.000000 canals-0.2.0/canals/pipeline/save_load.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 canals-0.2.0/canals/testing/__init__.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 canals-0.2.0/canals/testing/test_component.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 canals-0.2.0/docs/index.md
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 canals-0.2.0/docs/api-docs/component.md
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.2.0/docs/api-docs/draw.md
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 canals-0.2.0/docs/api-docs/pipeline.md
+-rw-r--r--   0        0        0     9353 2020-02-02 00:00:00.000000 canals-0.2.0/docs/concepts/components.md
+-rw-r--r--   0        0        0     4024 2020-02-02 00:00:00.000000 canals-0.2.0/docs/concepts/concepts.md
+-rw-r--r--   0        0        0     7171 2020-02-02 00:00:00.000000 canals-0.2.0/docs/concepts/pipelines.md
+-rw-r--r--   0        0        0    26250 2020-02-02 00:00:00.000000 canals-0.2.0/images/canals-logo-dark.png
+-rw-r--r--   0        0        0    25601 2020-02-02 00:00:00.000000 canals-0.2.0/images/canals-logo-light.png
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.2.0/test/__init__.py
+-rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 canals-0.2.0/test/test_save_load.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 canals-0.2.0/test/pipelines/__init__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.2.0/test/pipelines/integration/__init__.py
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 canals-0.2.0/test/pipelines/integration/test_complex_pipeline.py
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 canals-0.2.0/test/pipelines/integration/test_fixed_decision_and_merge_pipeline.py
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 canals-0.2.0/test/pipelines/integration/test_fixed_decision_pipeline.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 canals-0.2.0/test/pipelines/integration/test_fixed_merging_pipeline.py
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 canals-0.2.0/test/pipelines/integration/test_linear_pipeline.py
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 canals-0.2.0/test/pipelines/integration/test_looping_and_merge_pipeline.py
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 canals-0.2.0/test/pipelines/integration/test_looping_pipeline.py
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 canals-0.2.0/test/pipelines/integration/test_parallel_branches_pipeline.py
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 canals-0.2.0/test/pipelines/integration/test_variable_decision_and_merge_pipeline.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 canals-0.2.0/test/pipelines/integration/test_variable_decision_pipeline.py
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 canals-0.2.0/test/pipelines/integration/test_variable_merging_pipeline.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.2.0/test/pipelines/unit/__init__.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 canals-0.2.0/test/sample_components/__init__.py
+-rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 canals-0.2.0/test/sample_components/test_accumulate.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 canals-0.2.0/test/sample_components/test_add_value.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 canals-0.2.0/test/sample_components/test_double.py
+-rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 canals-0.2.0/test/sample_components/test_greet.py
+-rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 canals-0.2.0/test/sample_components/test_merge_loop.py
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 canals-0.2.0/test/sample_components/test_parity.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 canals-0.2.0/test/sample_components/test_remainder.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 canals-0.2.0/test/sample_components/test_repeat.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 canals-0.2.0/test/sample_components/test_subtract.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 canals-0.2.0/test/sample_components/test_sum.py
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 canals-0.2.0/test/sample_components/test_threshold.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 canals-0.2.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 canals-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 canals-0.2.0/README.md
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 canals-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4285 2020-02-02 00:00:00.000000 canals-0.2.0/PKG-INFO
```

### Comparing `canals-0.1.2/.pre-commit-config.yaml` & `canals-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `canals-0.1.2/mkdocs.yml` & `canals-0.2.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `canals-0.1.2/.github/workflows/tests.yml` & `canals-0.2.0/.github/workflows/tests.yml`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,17 @@
   push:
     branches:
       - main
   pull_request:
     paths:
       - "**.py"
       - "**/pyproject.toml"
+    
+env:
+  COVERALLS_NOISY: true
 
 jobs:
   mypy:
     runs-on: ubuntu-latest
     steps:
       - name: Checkout
         uses: actions/checkout@v3
@@ -106,7 +109,15 @@
           python-version: '3.8'
 
       - name: Install Canals
         run: pip install .[mermaid,dev]
 
       - name: Run
         run: hatch run cov
+
+      - name: Coverage
+        if: matrix.os == 'ubuntu-latest'
+        uses: coverallsapp/github-action@v2
+        with:
+          path-to-lcov: coverage.xml
+          parallel: false
+          debug: true
```

### Comparing `canals-0.1.2/canals/component/component.py` & `canals-0.2.0/docs/concepts/components.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,175 +1,265 @@
-import logging
-import inspect
+# Components
 
-from canals.errors import ComponentError
-from canals.component.save_init_params import set_default_component_attributes
+In order to be recognized as components and work in a Pipeline, Components must follow the contract below.
 
+## Requirements
 
-logger = logging.getLogger(__name__)
+### `@component` decorator
 
+All component classes must be decorated with the `@component` decorator. This allows Canals to discover them.
 
-def component(class_):
-    """
-    Marks a class as a component. Any class decorated with `@component` can be used by a Pipeline.
+### `Input`
 
-    All components must follow the contract below. This docstring is the source of truth for components contract.
+```python
+@dataclass
+class Input(ComponentInput / VariadicComponentInput):
+    <expected input fields, typed, with no defaults>
+```
+Semi-mandatory method (either this or `self.input_type(self)`).
 
-    ```python
-    def __init__(self, [... components init parameters ...]):
-    ```
-    Optional method.
+This inner class defines how the input of this component looks like. For example, if the node is expecting
+a list of Documents, the fields of the class should be `documents: List[Document]`
 
-    Components may have an `__init__` method where they define:
+Defaults are allowed, however `Optional`, `Union` and similar "generic" types are not. This is necessary to allow
+proper validation of the connections, which rely on the type of these fields.
 
-    - `self.defaults = {parameter_name: parameter_default_value, ...}`:
-        All values defined here will be sent to the `run()` method when the Pipeline calls it.
-        If any of these parameters is also receiving input from other components, those have precedence.
-        This collection of values is supposed to replace the need for default values in `run()` and make them
-        dynamically configurable.
+If your node expects variadic input, use `VariadicComponentInput`. In all other scenarios, use `ComponentInput`
+as your base class.
 
-    - `self.init_parameters = {same parameters that the __init__ method received}`:
-        In this dictionary you can store any state the components wish to be persisted when they are saved.
-        These values will be given to the `__init__` method of a new instance when the pipeline is loaded.
-        Note that by default the `@component` decorator saves the arguments automatically.
-        However, if a component sets their own `init_parameters` manually in `__init__()`, that will be used instead.
-        Note: all of the values contained here **must be JSON serializable**. Serialize them manually if needed.
+Some components may need more dynamic input. For these scenarios, refer to `self.input_type()`.
 
-    Components should take only "basic" Python types as parameters of their `__init__` function, or iterables and
-    dictionaries containing only such values. Anything else (objects, functions, etc) will raise an exception at init
-    time. If there's the need for such values, consider serializing them to a string.
+Every component should define **either** `Input` or `self.input_type()`.
 
-    _(TODO explain how to use classes and functions in init. In the meantime see `test/components/test_accumulate.py`)_
 
-    The `__init__` must be extrememly lightweight, because it's a frequent operation during the construction and
-    validation of the pipeline. If a component has some heavy state to initialize (models, backends, etc...) refer to
-    the `warm_up()` method.
+### `input_type()`
 
-    ```
-    def warm_up(self):
-    ```
-    Optional method.
+```python
+@property
+def input_type(self) -> ComponentInput / VariadicComponentInput:
+```
+Semi-mandatory method (either this or `class Input`).
 
-    This method is called by Pipeline before the graph execution. Make sure to avoid double-initializations,
-    because Pipeline will not keep track of which components it called `warm_up()` on.
+This method defines how the input of this component looks like. For example, if the node is expecting
+a list of Documents, this method should return a dataclass, subclass of either `ComponentInput` or
+`VariadicComponentInput`, with such fields. For example, it could build the dataclass as
+`make_dataclass("Input", fields=[(f"documents", List[Document], None)], bases=(ComponentInput, ))` and return it.
 
-    ```
-    @dataclass
-    class Output:
-        <expected output fields>
-    ```
-    Semi-mandatory method (either this or `self.output_types(self)`).
+Defaults are allowed, however `Optional`, `Union` and similar "generic" types are not. This is necessary to allow
+proper validation of the connections, which rely on the type of these fields.
+
+Normally the `Input` dataclass is preferred, as it provides autocompletion for the users and is much easier to use.
+
+Every component should define **either** `Input` or `self.input_type()`.
+
+
+### `Output`
+
+```python
+@dataclass
+class Output(ComponentOutput):
+    <expected output fields, typed>
+```
+Semi-mandatory method (either this or `self.output_type()`).
+
+This inner class defines how the output of this component looks like. For example, if the node is producing
+a list of Documents, the fields of the class should be `documents: List[Document]`
+
+Defaults are allowed, however `Optional`, `Union` and similar "generic" types are not. This is necessary to allow
+proper validation of the connections, which rely on the type of these fields.
+
+Some components may need more dynamic output: for example, your component accepts a list of file extensions at
+init time and wants to have one output field for each of those. For these scenarios, refer to `self.output_type()`.
+
+Every component should define **either** `Output` or `self.output_type()`.
+
+
+### `output_type()`
 
-    This inner class defines how the output of this component looks like. For example, if the node is producing
-    a list of Documents, the fields of the class should be `documents: List[Document]`
+```python
+@property
+def output_type(self) -> ComponentOutput:
+```
+Semi-mandatory method (either this or `class Output`).
 
-    Defaults are allowed, however `Optional`, `Union` and similar "generic" types are not. This is necessary to allow
-    proper validation of the connections, which rely on the type of these fields.
+This method defines how the output of this component looks like. For example, if the node is producing
+a list of Documents, this method should return a dataclass with such fields, for example:
+`return make_dataclass("Output", fields=[(f"documents", List[Document], None)], bases=(ComponentOutput, ))`
 
-    Some components may need more dynamic output: for example, your component accepts a list of file extensions at
-    init time and wants to have one output field for each of those. For these scenarios, refer to `self.output_type()`.
+Defaults are allowed, however `Optional`, `Union` and similar "generic" types are not. This is necessary to allow
+proper validation of the connections, which rely on the type of these fields.
 
-    Every component should define **either** `Output` or `self.output_types`.
+If the output is static, normally the `Output` dataclass is preferred, as it provides autocompletion for the users.
 
-    ```
-    def output_types(self) -> dataclass:
-    ```
-    Semi-mandatory method (either this or `class Output`).
+Every component should define **either** `Output` or `self.output_type`.
 
-    This method defines how the output of this component looks like. For example, if the node is producing
-    a list of Documents, this method should return a dataclass with such fields, for example:
-    `return make_dataclass("Output", [(f"documents", List[Document], None)])`
 
-    Defaults are allowed, however `Optional`, `Union` and similar "generic" types are not. This is necessary to allow
-    proper validation of the connections, which rely on the type of these fields.
+### `__init__()`
 
-    If the output is static, normally the `Output` dataclass is preferred, as it provides autocompletion for the users.
+```python
+def __init__(self, [... components init parameters ...]):
+```
+Optional method.
 
-    Every component should define **either** `Output` or `self.output_types`.
+Components may have an `__init__` method where they define:
 
-    ```
-    def run(self, <parameters, typed>) -> Output:
-    ```
-    Mandatory method.
+- `self.defaults = {parameter_name: parameter_default_value, ...}`:
+    All values defined here will be sent to the `run()` method when the Pipeline calls it.
+    If any of these parameters is also receiving input from other components, those have precedence.
+    This collection of values is supposed to replace the need for default values in `run()` and make them
+    dynamically configurable. Keep in mind that only these defaults will count at runtime: defaults given to
+    the `Input` dataclass (see above) will be ignored.
 
-    This is the method where the main functionality of the component should be carried out. It's called by
-    `Pipeline.run()`.
+- `self.init_parameters = {same parameters that the __init__ method received}`:
+    In this dictionary you can store any state the components wish to be persisted when they are saved.
+    These values will be given to the `__init__` method of a new instance when the pipeline is loaded.
+    Note that by default the `@component` decorator saves the arguments automatically.
+    However, if a component sets their own `init_parameters` manually in `__init__()`, that will be used instead.
+    Note: all of the values contained here **must be JSON serializable**. Serialize them manually if needed.
 
-    When the component should run, Pipeline will call this method with:
+Components should take only "basic" Python types as parameters of their `__init__` function, or iterables and
+dictionaries containing only such values. Anything else (objects, functions, etc) will raise an exception at init
+time. If there's the need for such values, consider serializing them to a string.
 
-    - all the input values coming from "upstream" components connected to it,
-    - if any is missing, the corresponding value defined in `self.defaults`, if it exists.
+_(TODO explain how to use classes and functions in init. In the meantime see `test/components/test_accumulate.py`)_
 
-    All parameters of `run()` **must be typed**. The types are used by `Pipeline.connect()` to make sure the two
-    components agree on the type being passed, to try ensure the connection will be successful.
-    Defaults are allowed, however `Optional`, `Union` and similar "generic" types are not, just as for the outputs.
+The `__init__` must be extrememly lightweight, because it's a frequent operation during the construction and
+validation of the pipeline. If a component has some heavy state to initialize (models, backends, etc...) refer to
+the `warm_up()` method.
 
-    `run()` must return a single instance of the dataclass declared through either `Output` or `self.output_types()`.
 
-    A variadic `run()` method is allowed if it respects the following rules:
+### `warm_up()`
 
-    - It can take **either** regular parameters, or a single variadic positional (`*args`), NOT BOTH.
-    - `**kwargs` are not supported
-    - The variadic `*args` must be typed, for example `*args: int` if the component accepts any number of integers.
+```python
+def warm_up(self):
+```
+Optional method.
 
-    Args:
-        class_: the class that Canals should use as a component.
-        serializable: whether to check, at init time, if the component can be saved with
-        `save_pipelines()`.
+This method is called by Pipeline before the graph execution. Make sure to avoid double-initializations,
+because Pipeline will not keep track of which components it called `warm_up()` on.
 
-    Returns:
-        A class that can be recognized as a component.
 
-    Raises:
-        ComponentError: if the class provided has no `run()` method or otherwise doesn't respect the component contract.
+### `run()`
+
+```python
+def run(self, data: <Input if defined, otherwise untyped>) -> <Output if defined, otherwise untyped>:
+```
+Mandatory method.
+
+This is the method where the main functionality of the component should be carried out. It's called by
+`Pipeline.run()`.
+
+When the component should run, Pipeline will call this method with:
+
+- all the input values coming from other components connected to it,
+- if any is missing, the corresponding value defined in `self.defaults`, if it exists.
+
+`run()` must return a single instance of the dataclass declared through either `Output` or `self.output_type()`.
+
+
+## Example components
+
+### Basic
+Here is an example of a simple component that adds two values together and returns their sum.
+
+```python
+from dataclasses import dataclass
+from canals.component import component, ComponentInput, ComponentOutput
+
+@component
+class AddFixedValue:
+    """
+    Adds the value of `add` to `value`. If not given, `add` defaults to 1.
     """
-    logger.debug("Registering %s as a component", class_)
 
-    # '__canals_component__' is used to distinguish components from regular classes.
-    # Its value is set to the desired component name: normally it is the class name, but it can technically be customized.
-    class_.__canals_component__ = class_.__name__
+    @dataclass
+    class Input(ComponentInput):
+        value: int
+        add: int
 
-    # Check for run()
-    if not hasattr(class_, "run"):
-        raise ComponentError(f"{class_.__name__} must have a 'run()' method. See the docs for more information.")
-    run_signature = inspect.signature(class_.run)
+    @dataclass
+    class Output(ComponentOutput):
+        value: int
 
-    # Check the run() signature for keyword variadic arguments
-    if any(run_signature.parameters[param].kind == inspect.Parameter.VAR_KEYWORD for param in run_signature.parameters):
-        raise ComponentError(
-            f"{class_.__name__} can't have variadic keyword arguments like **kwargs in its 'run()' method."
-        )
+    def __init__(self, add: Optional[int] = 1):
+        if add:
+            self.defaults = {"add": add}
 
-    # Check the run() signature for missing types in positional variadic arguments
-    if any(
-        run_signature.parameters[param].kind == inspect.Parameter.VAR_POSITIONAL
-        and run_signature.parameters[param].annotation == inspect.Parameter.empty
-        for param in run_signature.parameters
-    ):
-        raise ComponentError(
-            f"{class_.__name__} must type also variadic arguments like *args in its 'run()' method.\n"
-            "Hint: variadic arguments are typed in singular form, so if your component takes an arbitrary number of "
-            "strings, the signature of run() should look like 'def run(self, *my_strings: str) -> Output:'."
-        )
+    def run(self, data: Input) -> Output:
+        return AddFixedValue.Output(value=data.value + data.add)
+
+```
+
+### Variadic
+
+Here is an example of a variadic component that adds all the incoming values together and returns their sum.
+
+```python
+from dataclasses import dataclass
+from canals.component import component, VariadicComponentInput, ComponentOutput
+
+@component
+class Sum:
+    """
+    Sums the values of all the input connections together.
+    """
+
+    @dataclass
+    class Input(VariadicComponentInput):
+        values: List[int]
+
+    @dataclass
+    class Output(ComponentOutput):
+        total: int
+
+    def run(self, data: Input) -> Output:
+        return Sum.Output(total=sum(data.values))
+
+```
+
+### Dynamic output
+
+Here is an example of a component that returns the incoming value on a different edge depending on its remainder.
+
+This is an example of how to use `self.output_type()` in practice.
+
+```python
+from dataclasses import make_dataclass
+from canals.component import component, ComponentInput, ComponentOutput
+
+
+@component
+class Remainder:
+    """
+    Redirects the value, unchanged, along the connection corresponding to the remainder
+    of a division. For example, if `divisor=3`, the value `5` would be sent along
+    the second output connection.
+    """
+
+    @dataclass
+    class Input(ComponentInput):
+        value: int
+        add: int = 1
+
+    def __init__(self, divisor: int = 2):
+        if divisor == 0:
+            raise ValueError("Can't divide by zero")
+        self.divisor = divisor
 
-    # Check the run() signature for other missing types
-    missing_types = [
-        parameter
-        for parameter in list(run_signature.parameters)[1:]  # First is 'self' and it doesn't matter.
-        if run_signature.parameters[parameter].annotation == inspect.Parameter.empty
-    ]
-    if missing_types:
-        raise ComponentError(
-            f"{class_.__name__}.run() must declare types for all its parameters, "
-            f"but these parameters are not typed: {', '.join(missing_types)}."
+        self._output_type = make_dataclass(
+            "Output", fields=[(f"remainder_is_{val}", int, None) for val in range(divisor)], bases=(ComponentOutput,)
         )
 
-    # Check for the return types
-    if run_signature.return_annotation == inspect.Parameter.empty:
-        if not hasattr(class_, "output_type"):
-            raise ComponentError(f"{class_.__name__}.run() must declare the type of its return value.")
-
-    # Automatically registers all the init parameters in an instance attribute called `_init_parameters`.
-    # See `save_init_parameters()`.
-    class_.__init__ = set_default_component_attributes(class_.__init__)
+    @property
+    def output_type(self):
+        return self._output_type
+
+    def run(self, data: Input):
+        """
+        :param value: the value to check the remainder of.
+        """
+        remainder = data.value % self.divisor
+        output = self.output_type()
+        setattr(output, f"remainder_is_{remainder}", data.value)
+        return output
 
-    return class_
+```
```

### Comparing `canals-0.1.2/canals/component/save_init_params.py` & `canals-0.2.0/canals/component/decorators.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,57 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 # pylint: disable=protected-access
 
 import logging
 import inspect
 from functools import wraps
 
 
 logger = logging.getLogger(__name__)
 
 
-def set_default_component_attributes(init_func):
+def save_init_params(init_func):
     """
-    Decorator that prepares a few default attributes for each component:
-     - saves the init parameters of a component in self._init_parameters
-     - makes sure the `self.defaults` dictionary exists
+    Decorator that saves the init parameters of a component in `self.init_parameters`
     """
 
     @wraps(init_func)
-    def wrapper_save_init_parameters(self, *args, **kwargs):
+    def wrapper_saveinit_parameters(self, *args, **kwargs):
 
         # Call the actual __init__ function with the arguments
         init_func(self, *args, **kwargs)
 
         # Convert all args into kwargs
         sig = inspect.signature(init_func)
         arg_names = list(sig.parameters.keys())
         if any(arg_names) and arg_names[0] in ["self", "cls"]:
             arg_names.pop(0)
         args_as_kwargs = {arg_name: arg for arg, arg_name in zip(args, arg_names)}
 
         # Collect and store all the init parameters, preserving whatever the components might have already added there
-        _init_parameters = {**args_as_kwargs, **kwargs}
-        if hasattr(self, "_init_parameters"):
-            _init_parameters = {**_init_parameters, **self._init_parameters}
-        self._init_parameters = _init_parameters
+        init_parameters = {**args_as_kwargs, **kwargs}
+        if hasattr(self, "init_parameters"):
+            init_parameters = {**init_parameters, **self.init_parameters}
+        self.init_parameters = init_parameters
+
+    return wrapper_saveinit_parameters
+
+
+def init_defaults(init_func):
+    """
+    Decorator that makes sure the `self.defaults` dictionary exists
+    """
+
+    @wraps(init_func)
+    def wrapper_create_defaults_dict(self, *args, **kwargs):
+
+        # Call the actual __init__ function with the arguments
+        init_func(self, *args, **kwargs)
 
         # Makes sure the component has a defaults dictionary the pipeline can use
         if not hasattr(self, "defaults"):
             self.defaults = {}
 
-    return wrapper_save_init_parameters
+    return wrapper_create_defaults_dict
```

### Comparing `canals-0.1.2/canals/draw/draw.py` & `canals-0.2.0/canals/draw/draw.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
 from typing import Literal, Optional, Dict, get_args, Any
 
 import logging
 from pathlib import Path
 
 import networkx
```

### Comparing `canals-0.1.2/canals/draw/graphviz.py` & `canals-0.2.0/canals/draw/graphviz.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
 import logging
 
 import networkx
 from networkx.drawing.nx_agraph import to_agraph as nx_to_agraph
 
 logger = logging.getLogger(__name__)
```

### Comparing `canals-0.1.2/canals/draw/mermaid.py` & `canals-0.2.0/canals/draw/mermaid.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
 import logging
 import base64
 
 import requests
 import networkx
```

### Comparing `canals-0.1.2/canals/pipeline/_utils.py` & `canals-0.2.0/canals/pipeline/_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-from typing import Tuple, Optional, List, Iterable, Dict, Any
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai> SPDX-License-Identifier: Apache-2.0
+from typing import Tuple, Optional, List, Iterable, Dict, Any, get_args
 
 import logging
 import inspect
 import itertools
-from dataclasses import dataclass, fields
+from dataclasses import dataclass
 
 import networkx
 
 from canals.errors import PipelineConnectError, PipelineValidationError
+from canals.component.input_output import fields, ComponentInput
 
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class OutputSocket:
@@ -37,39 +39,57 @@
     return connection, None
 
 
 def find_input_sockets(component) -> Dict[str, InputSocket]:
     """
     Find a component's input sockets.
     """
-    run_signature = inspect.signature(component.run)
+    run_signature = inspect.signature(component.__class__.run)
+
+    input_annotation = run_signature.parameters["data"].annotation
+    if not input_annotation or input_annotation == inspect.Parameter.empty:
+        input_annotation = component.input_type
+    variadic = hasattr(input_annotation, "_variadic_component_input")
 
     input_sockets = {}
-    for param in run_signature.parameters:
-        name = run_signature.parameters[param].name
-        variadic = run_signature.parameters[param].kind == inspect.Parameter.VAR_POSITIONAL
-        annotation = run_signature.parameters[param].annotation
+    for field in fields(input_annotation):
+        # Unwrap List types to get the internal type, if the argument is variadic, and Optionals
+        #   Note: we're forced to use type() == type() due to an explicit limitation of the typing library,
+        #   that disables `issubclass` on typing classes.
+        if variadic or type(field.type) == type(Optional[Any]):  # pylint: disable=unidiomatic-typecheck
+            type_ = get_args(field.type)[0]
+        else:
+            type_ = field.type
 
-        socket = InputSocket(name=name, type=annotation, variadic=variadic)
-        input_sockets[socket.name] = socket
+        input_sockets[field.name] = InputSocket(name=field.name, type=type_, variadic=variadic)
 
     return input_sockets
 
 
 def find_output_sockets(component) -> Dict[str, OutputSocket]:
     """
     Find a component's output sockets.
     """
     run_signature = inspect.signature(component.run)
 
     return_annotation = run_signature.return_annotation
     if return_annotation == inspect.Parameter.empty:
         return_annotation = component.output_type
 
-    output_sockets = {field.name: OutputSocket(name=field.name, type=field.type) for field in fields(return_annotation)}
+    output_sockets = {}
+    for field in fields(return_annotation):
+        # Unwrap Optionals
+        #   Note: we're forced to use type() == type() due to an explicit limitation of the typing library,
+        #   that disables `issubclass` on typing classes.
+        if type(field.type) == type(Optional[Any]):  # pylint: disable=unidiomatic-typecheck
+            type_ = get_args(field.type)[0]
+        else:
+            type_ = field.type
+
+        output_sockets[field.name] = OutputSocket(name=field.name, type=type_)
 
     return output_sockets
 
 
 def connections_status(from_node: str, to_node: str, from_sockets: List[OutputSocket], to_sockets: List[InputSocket]):
     """
     Lists the status of the sockets, for error messages.
@@ -146,60 +166,69 @@
     return {
         node: list(data.get("output_sockets", {}).values())
         for node, data in graph.nodes(data=True)
         if not graph.out_edges(node)
     }
 
 
-def _validate_input_sockets_are_connected(graph: networkx.MultiDiGraph, inputs_values: Dict[str, Dict[str, Any]]):
+def _validate_input_sockets_are_connected(graph: networkx.MultiDiGraph, input_values: Dict[str, ComponentInput]):
+    """
+    Make sure all the inputs nodes are receiving all the values they need, either from the Pipeline's input or from
+    other nodes.
+    """
     valid_inputs = find_pipeline_inputs(graph)
     for node, sockets in valid_inputs.items():
-        if node in inputs_values:
+        if node in input_values:
             for socket in sockets:
                 node_instance = graph.nodes[node]["instance"]
                 input_in_node_defaults = hasattr(node_instance, "defaults") and socket.name in node_instance.defaults
-                if not input_in_node_defaults and not socket.name in inputs_values[node]:
+                if not input_in_node_defaults and not socket.name in input_values[node].names():
                     raise ValueError(f"Missing input: {node}.{socket.name}")
 
 
-def _validate_nodes_receive_only_expected_input(graph: networkx.MultiDiGraph, inputs_values: Dict[str, Dict[str, Any]]):
-    for node, input_data in inputs_values.items():
-        for socket_name in input_data.keys():
+def _validate_nodes_receive_only_expected_input(graph: networkx.MultiDiGraph, input_values: Dict[str, ComponentInput]):
+    """
+    Make sure that every input node is only receiving input values from EITHER the pipeline's input or another node,
+    but never from both.
+    """
+    for node, input_data in input_values.items():
+        for socket_name in input_data.names():
+            if not getattr(input_data, socket_name):
+                continue
             if not socket_name in graph.nodes[node]["input_sockets"].keys():
                 raise ValueError(f"Component {node} is not expecting any input value called {socket_name}")
 
             taken_by = graph.nodes[node]["input_sockets"][socket_name].taken_by
             if taken_by:
                 raise ValueError(f"The input {socket_name} of {node} is already taken by node {taken_by}")
 
 
 def validate_pipeline_input(  # pylint: disable=too-many-branches
-    graph: networkx.MultiDiGraph, inputs_values: Dict[str, Dict[str, Any]]
-) -> Dict[str, Dict[str, Any]]:
+    graph: networkx.MultiDiGraph, input_values: Dict[str, ComponentInput]
+) -> Dict[str, ComponentInput]:
     """
     Make sure the pipeline is properly built and that the input received makes sense.
-
     Returns the input values, validated and updated at need.
     """
     input_components = find_pipeline_inputs(graph)
     if not find_pipeline_inputs(graph):
         raise PipelineValidationError("This pipeline has no inputs.")
 
     # Make sure the input keys are all nodes of the pipeline
-    unknown_components = [key for key in inputs_values.keys() if not key in graph.nodes]
+    unknown_components = [key for key in input_values.keys() if not key in graph.nodes]
     if unknown_components:
         raise ValueError(f"Pipeline received data for unknown component(s): {', '.join(unknown_components)}")
 
     # Make sure all necessary sockets are connected
-    _validate_input_sockets_are_connected(graph, inputs_values)
+    _validate_input_sockets_are_connected(graph, input_values)
 
     # Make sure that the pipeline input is only sent to nodes that won't receive data from other nodes
-    _validate_nodes_receive_only_expected_input(graph, inputs_values)
+    _validate_nodes_receive_only_expected_input(graph, input_values)
 
     # Make sure variadic input components are receiving lists
     for component in input_components.keys():
-        if graph.nodes[component]["variadic_input"] and component in inputs_values.keys():
-            for key, value in inputs_values[component].items():  # should be just one
+        if graph.nodes[component]["variadic_input"] and component in input_values.keys():
+            for key, value in input_values[component].__dict__.items():  # should be just one
                 if not isinstance(value, Iterable):
-                    inputs_values[component][key] = [value]
+                    setattr(input_values[component], key, [value])
 
-    return inputs_values
+    return input_values
```

### Comparing `canals-0.1.2/canals/pipeline/pipeline.py` & `canals-0.2.0/canals/pipeline/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,22 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
 from typing import Optional, Any, Dict, List, Tuple, Literal
 
 import datetime
 import logging
 from pathlib import Path
 from copy import deepcopy
 from collections import OrderedDict
 
 import networkx
 
 from canals.errors import PipelineConnectError, PipelineMaxLoops, PipelineRuntimeError, PipelineValidationError
+from canals.component.input_output import ComponentInput
 from canals.draw import draw, RenderingEngines
 from canals.pipeline._utils import (
     InputSocket,
     OutputSocket,
     find_input_sockets,
     find_output_sockets,
     find_unambiguous_connection,
@@ -271,15 +275,15 @@
         without re-initializing everything.
         """
         for node in self.graph.nodes:
             if hasattr(self.graph.nodes[node]["instance"], "warm_up"):
                 logger.info("Warming up component %s...", node)
                 self.graph.nodes[node]["instance"].warm_up()
 
-    def run(self, data: Dict[str, Dict[str, Any]], debug: bool = False) -> Dict[str, Any]:
+    def run(self, data: Dict[str, ComponentInput], debug: bool = False) -> Dict[str, Any]:
         """
         Runs the pipeline.
 
         Args:
             data: the inputs to give to the input components of the Pipeline.
             parameters: a dictionary with all the parameters of all the components, namespaced by component.
             debug: whether to collect and return debug information.
@@ -314,20 +318,25 @@
         # - Input nodes            # [e[0] for e in self.graph.in_edges(node)]
         # - Output nodes           # [e[1] for e in self.graph.out_edges(node)]
         # - Output edges           # [e[2]["label"] for e in self.graph.out_edges(node, data=True)]
         #
         # if debug:
         #     os.makedirs("debug", exist_ok=True)
 
-        data = validate_pipeline_input(self.graph, inputs_values=data)
+        data = validate_pipeline_input(self.graph, input_values=data)
         self._clear_visits_count()
         self.warm_up()
 
         logger.info("Pipeline execution started.")
-        inputs_buffer = OrderedDict(data)
+        inputs_buffer = OrderedDict(
+            {
+                node: {key: value for key, value in input_data.__dict__.items() if value is not None}
+                for node, input_data in data.items()
+            }
+        )
         pipeline_output: Dict[str, Dict[str, Any]] = {}
 
         if debug:
             logger.info("Debug mode ON.")
             self.debug = {}
 
         # *** PIPELINE EXECUTION LOOP ***
@@ -547,35 +556,38 @@
         """
         self.graph.nodes[name]["visits"] += 1
         instance = self.graph.nodes[name]["instance"]
         try:
             logger.info("* Running %s (visits: %s)", name, self.graph.nodes[name]["visits"])
             logger.debug("   '%s' inputs: %s", name, inputs)
 
+            input_class = instance.Input if hasattr(instance, "Input") else instance.input_type
+
             # If the node is variadic, unpack the input
             if self.graph.nodes[name]["variadic_input"]:
                 inputs = list(inputs.values())[0]
-                output_dataclass = instance.run(*inputs)
+                input_dataclass = input_class(*inputs)
 
             # Otherwise pass the inputs as kwargs after adding the component's own defaults to them
             else:
                 inputs = {**instance.defaults, **inputs}
-                output_dataclass = instance.run(**inputs)
+                input_dataclass = input_class(**inputs)
+
+            output_dataclass = instance.run(input_dataclass)
 
             # Unwrap the output
-            output = output_dataclass.__dict__
-            logger.debug("   '%s' outputs: %s\n", name, output)
+            logger.debug("   '%s' outputs: %s\n", name, output_dataclass.__dict__)
 
         except Exception as e:
             raise PipelineRuntimeError(
                 f"{name} raised '{e.__class__.__name__}: {e}' \nInputs: {inputs}\n\n"
                 "See the stacktrace above for more information."
             ) from e
 
-        return output
+        return output_dataclass
 
     def _route_output(
         self,
         node_name: str,
         node_results: Dict[str, Any],
         inputs_buffer: OrderedDict,
     ) -> OrderedDict:
@@ -592,15 +604,15 @@
         for edge_data in self.graph.out_edges(node_name, data=True):
             to_socket = edge_data[2]["to_socket"]
             from_socket = edge_data[2]["from_socket"]
             target_node = edge_data[1]
 
             # If this is a decision node and a loop is involved, we add to the input buffer only the nodes
             # that received their expected output and we leave the others out of the queue.
-            if is_decision_node_for_loop and node_results[from_socket.name] is None:
+            if is_decision_node_for_loop and getattr(node_results, from_socket.name) is None:
                 if networkx.has_path(self.graph, target_node, node_name):
                     # In case we're choosing to leave a loop, do not put the loop's node in the buffer.
                     logger.debug(
                         "Not adding '%s' to the inputs buffer: we're leaving the loop.",
                         target_node,
                     )
                 else:
@@ -610,16 +622,18 @@
                         target_node,
                     )
             else:
                 # In all other cases, populate the inputs buffer for all downstream nodes, setting None to any
                 # edge that did not receive input.
                 if not target_node in inputs_buffer:
                     inputs_buffer[target_node] = {}  # Create the buffer for the downstream node if it's not there yet
-                if node_results.get(from_socket.name, None):
+
+                value_to_route = getattr(node_results, from_socket.name, None)
+                if value_to_route:
                     if to_socket.variadic:
                         if not to_socket.name in inputs_buffer[target_node].keys():
                             inputs_buffer[target_node][to_socket.name] = []
-                        inputs_buffer[target_node][to_socket.name].append(node_results[from_socket.name])
+                        inputs_buffer[target_node][to_socket.name].append(value_to_route)
                     else:
-                        inputs_buffer[target_node][to_socket.name] = node_results[from_socket.name]
+                        inputs_buffer[target_node][to_socket.name] = value_to_route
 
         return inputs_buffer
```

### Comparing `canals-0.1.2/canals/pipeline/save_load.py` & `canals-0.2.0/canals/pipeline/save_load.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 # pylint: disable=protected-access
 
 from typing import Dict, List, Any, Tuple
 
 import sys
 import json
 import logging
@@ -91,15 +95,15 @@
             # If no pointer was made in the previous step
             if not component_name in pipeline_repr["components"]:
                 # Save the components in the global components list
                 components.append((pipeline_name, component_name, component_instance))
                 # Serialize the components
                 component_repr = {
                     "type": component_instance.__class__.__name__,
-                    "init_parameters": component_instance._init_parameters,
+                    "init_parameters": component_instance.init_parameters,
                 }
                 pipeline_repr["components"][component_name] = component_repr
 
         pipeline_repr["connections"] = list(pipeline.graph.edges)
         schema["pipelines"][pipeline_name] = pipeline_repr
 
     # Collect the dependencies
```

### Comparing `canals-0.1.2/canals/testing/test_component.py` & `canals-0.2.0/canals/testing/test_component.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
 from dataclasses import is_dataclass
 
 import pytest
 
-from canals import Pipeline, save_pipelines, load_pipelines, marshal_pipelines
+from canals.pipeline import Pipeline, save_pipelines, load_pipelines, marshal_pipelines
 
 #
 # TODO right now the tests iterate on components, so it's not always clear which component fails the tests.
 # Can we instead parametrize the tests on the output of the components fixture?
 #
 class BaseTestComponent:
     """
```

### Comparing `canals-0.1.2/docs/index.md` & `canals-0.2.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `canals-0.1.2/docs/concepts/concepts.md` & `canals-0.2.0/docs/concepts/concepts.md`

 * *Files 10% similar despite different names*

```diff
@@ -20,31 +20,36 @@
 3. Have a `run()` method with all the inputs and outputs typed.
 4. Must return a pre-defined dataclass called `Output`.
 
 For example, the following is a Component that sums up two numbers:
 
 ```python
 from dataclasses import dataclass
-from canals import component
+from canals.component import component, ComponentInput, ComponentOutput
 
 @component
-class AddTwoValues:
+class AddFixedValue:
     """
     Adds the value of `add` to `value`. If not given, `add` defaults to 1.
     """
 
     @dataclass
-    class Output:
+    class Input(ComponentInput):
         value: int
 
-    def __init__(self, add: int = 1):
-        self.defaults = {"add": add}
+    @dataclass
+    class Output(ComponentOutput):
+        value: int
+
+    def __init__(self, add: Optional[int] = 1):
+        if add:
+            self.defaults = {"add": add}
 
-    def run(self, value: int, add: int) -> Output:
-        return AddTwoValues.Output(value=value + add)
+    def run(self, data: Input) -> Output:
+        return AddFixedValue.Output(value=data.value + data.add)
 ```
 
 We will see the details of all of these requirements below.
 
 ## What is a Pipeline?
 
 A Pipeline is a network of Components. Pipelines define what components receive and send output to which other, makes
@@ -57,46 +62,46 @@
 For example, if a component produces a value of type `List[Document]` and another component expects an input
 of type `List[Document]`, Pipeline will be able to connect them. Otherwise, it will raise an exception.
 
 This is a simple example of how a Pipeline is created:
 
 
 ```python
-from canals import Pipeline, component
+from canals.pipeline import Pipeline
 
 # Some Canals components
-from my_components import AddTwoValues, MultiplyTwoValues
+from my_components import AddFixedValue, MultiplyBy
 
 pipeline = Pipeline()
 
 # Components can be initialized as standalone objects.
 # These instances can be added to the Pipeline in several places.
 multiplication = MultiplyBy(multiply_by=2)
-addition = AddTwoValues(add=1)
+addition = AddFixedValue(add=1)
 
 # Components are added with a name and an component
 pipeline.add_component("double", multiplication)
 pipeline.add_component("add_one", addition)
 pipeline.add_component("add_one_again", addition)  # Component instances can be reused
-pipeline.add_component("add_two", AddTwoValues(add=2))
+pipeline.add_component("add_two", AddFixedValue(add=2))
 
 # Connect the components together
 pipeline.connect(connect_from="double", connect_to="add_one")
 pipeline.connect(connect_from="add_one", connect_to="add_one_again")
 pipeline.connect(connect_from="add_one_again", connect_to="add_two")
 
 # Pipeline can be drawn
 pipeline.draw("pipeline.jpg")
 
 # Pipelines are run by giving them the data that the input nodes expect.
-results = pipeline.run(data={"double":{"value": 1}})
+results = pipeline.run(data={"double": MultiplyBy.Input(value=1)})
 
 print(results)
 
-# prints {"add_two": {"value": 6}}
+# prints {"add_two": AddFixedValue.Output(value=6)}
 ```
 
 This is how the pipeline's graph looks like:
 
 ```mermaid
 graph TD;
 double -- value -> value --> add_one
```

### Comparing `canals-0.1.2/docs/concepts/pipelines.md` & `canals-0.2.0/docs/concepts/pipelines.md`

 * *Files 3% similar despite different names*

```diff
@@ -22,29 +22,33 @@
 For example, let's imagine we have two components with the following I/O declared:
 
 ```python
 @component
 class ComponentA:
 
     @dataclass
-    class Output:
+    class Input(ComponentInput):
+        input_value: int
+
+    @dataclass
+    class Output(ComponentOutput):
         intermediate_value: str
 
-    def run(self, input_value: int) -> Output:
-        return ComponentA.output(intermediate_value="hello")
+    def run(self, data: Input) -> Output:
+        return ComponentA.Output(intermediate_value="hello")
 
 @component
 class ComponentB:
 
     @dataclass
     class Output:
         output_value: List[int]
 
-    def run(self, intermediate_value: str) -> Output:
-        return ComponentB.output(output_value=[1, 2, 3])
+    def run(self, data: Input) -> Output:
+        return ComponentB.Output(output_value=[1, 2, 3])
 ```
 
 This is the behavior of `Pipeline.connect()`:
 
 ```python
 pipeline.add_component('component_a', ComponentA())
 pipeline.add_component('component_b', ComponentB())
```

### Comparing `canals-0.1.2/images/canals-logo-dark.png` & `canals-0.2.0/images/canals-logo-dark.png`

 * *Files identical despite different names*

### Comparing `canals-0.1.2/images/canals-logo-light.png` & `canals-0.2.0/images/canals-logo-light.png`

 * *Files identical despite different names*

### Comparing `canals-0.1.2/test/test_save_load.py` & `canals-0.2.0/test/test_save_load.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
 import pytest
 
 from canals.pipeline import Pipeline, marshal_pipelines, unmarshal_pipelines
-from test.test_components import AddFixedValue, Double
+from test.sample_components import AddFixedValue, Double
 
 import logging
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 def test_marshal():
```

### Comparing `canals-0.1.2/test/pipelines/integration/test_complex_pipeline.py` & `canals-0.2.0/test/pipelines/integration/test_complex_pipeline.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
 from pathlib import Path
 from pprint import pprint
 import logging
 
 from canals.pipeline import Pipeline
-from test.test_components import (
+from test.sample_components import (
     Accumulate,
     AddFixedValue,
     Greet,
     Parity,
     Threshold,
     Double,
     Sum,
@@ -75,17 +78,17 @@
     pipeline.connect("enumerate.second", "sum")
 
     pipeline.connect("enumerate.first", "add_three.value")
     pipeline.connect("add_three", "sum")
 
     pipeline.draw(tmp_path / "complex_pipeline.png")
 
-    results = pipeline.run({"greet_first": {"value": 1}, "greet_enumerator": {"value": 1}})
+    results = pipeline.run({"greet_first": Greet.Input(value=1), "greet_enumerator": Greet.Input(value=1)})
     pprint(results)
     print("accumulated: ", accumulate.state)
 
-    assert results == {"accumulate_3": {"value": 9}, "add_five": {"value": -7}}
+    assert results == {"accumulate_3": Accumulate.Output(value=9), "add_five": AddFixedValue.Output(value=-7)}
     assert accumulate.state == 9
 
 
 if __name__ == "__main__":
     test_complex_pipeline(Path(__file__).parent)
```

### Comparing `canals-0.1.2/test/pipelines/integration/test_fixed_decision_and_merge_pipeline.py` & `canals-0.2.0/test/pipelines/integration/test_variable_decision_and_merge_pipeline.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,48 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
 import logging
 from pathlib import Path
 from pprint import pprint
 
 from canals.pipeline import Pipeline
-from test.test_components import AddFixedValue, Parity, Double, Subtract
+from test.sample_components import AddFixedValue, Remainder, Double, Sum
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 def test_pipeline(tmp_path):
     add_one = AddFixedValue()
 
     pipeline = Pipeline()
     pipeline.add_component("add_one", add_one)
-    pipeline.add_component("parity", Parity())
+    pipeline.add_component("parity", Remainder())
     pipeline.add_component("add_ten", AddFixedValue(add=10))
     pipeline.add_component("double", Double())
     pipeline.add_component("add_four", AddFixedValue(add=4))
-    pipeline.add_component("add_two", add_one)
-    pipeline.add_component("diff", Subtract())
+    pipeline.add_component("add_one_again", add_one)
+    pipeline.add_component("sum", Sum())
 
     pipeline.connect("add_one", "parity")
-    pipeline.connect("parity.even", "add_four.value")
-    pipeline.connect("parity.odd", "double")
-    pipeline.connect("add_ten", "diff.first_value")
-    pipeline.connect("double", "diff.second_value")
-    pipeline.connect("parity.odd", "add_ten.value")
-    pipeline.connect("add_four", "add_two")
+    pipeline.connect("parity.remainder_is_0", "add_ten.value")
+    pipeline.connect("parity.remainder_is_1", "double")
+    pipeline.connect("add_one", "sum")
+    pipeline.connect("add_ten", "sum")
+    pipeline.connect("double", "sum")
+    pipeline.connect("parity.remainder_is_1", "add_four.value")
+    pipeline.connect("add_four", "add_one_again")
+    pipeline.connect("add_one_again", "sum")
 
-    pipeline.draw(tmp_path / "fixed_decision_and_merge_pipeline.png")
+    pipeline.draw(tmp_path / "variable_decision_and_merge_pipeline.png")
 
-    results = pipeline.run({"add_one": {"value": 1}, "add_two": {"add": 2}})
+    results = pipeline.run({"add_one": AddFixedValue.Input(value=1)})
     pprint(results)
-    assert results == {"add_two": {"value": 8}}
+    assert results == {"sum": Sum.Output(total=14)}
 
-    results = pipeline.run({"add_one": {"value": 2}, "add_two": {"add": 2}})
+    results = pipeline.run({"add_one": AddFixedValue.Input(value=2)})
     pprint(results)
-    assert results == {"diff": {"difference": 7}}
+    assert results == {"sum": Sum.Output(total=17)}
 
 
 if __name__ == "__main__":
     test_pipeline(Path(__file__).parent)
```

### Comparing `canals-0.1.2/test/pipelines/integration/test_fixed_merging_pipeline.py` & `canals-0.2.0/test/pipelines/integration/test_variable_merging_pipeline.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,47 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
 from pathlib import Path
 from pprint import pprint
 
 from canals.pipeline import Pipeline
-from test.test_components import AddFixedValue, Subtract
+from test.sample_components import AddFixedValue, Sum
 
 import logging
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 def test_pipeline(tmp_path):
 
     add_two = AddFixedValue(add=2)
-    diff = Subtract()
+    make_the_sum = Sum()
 
     pipeline = Pipeline()
     pipeline.add_component("first_addition", add_two)
     pipeline.add_component("second_addition", add_two)
     pipeline.add_component("third_addition", add_two)
-    pipeline.add_component("diff", diff)
+    pipeline.add_component("sum", make_the_sum)
     pipeline.add_component("fourth_addition", AddFixedValue(add=1))
 
     pipeline.connect("first_addition", "second_addition")
-    pipeline.connect("second_addition", "diff.first_value")
-    pipeline.connect("third_addition", "diff.second_value")
-    pipeline.connect("diff", "fourth_addition.value")
+    pipeline.connect("first_addition", "sum")
+    pipeline.connect("second_addition", "sum")
+    pipeline.connect("third_addition", "sum")
+    pipeline.connect("sum", "fourth_addition.value")
 
-    pipeline.draw(tmp_path / "fixed_merging_pipeline.png")
+    pipeline.draw(tmp_path / "variable_merging_pipeline.png")
 
     results = pipeline.run(
         {
-            "first_addition": {"value": 1},
-            "third_addition": {"value": 1},
+            "first_addition": AddFixedValue.Input(value=1),
+            "third_addition": AddFixedValue.Input(value=1),
         }
     )
     pprint(results)
 
-    assert results == {"fourth_addition": {"value": 3}}
+    assert results == {"fourth_addition": AddFixedValue.Output(value=12)}
 
 
 if __name__ == "__main__":
     test_pipeline(Path(__file__).parent)
```

### Comparing `canals-0.1.2/test/pipelines/integration/test_linear_pipeline.py` & `canals-0.2.0/test/pipelines/integration/test_fixed_merging_pipeline.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,46 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
 from pathlib import Path
 from pprint import pprint
 
 from canals.pipeline import Pipeline
-from test.test_components import AddFixedValue, Double
+from test.sample_components import AddFixedValue, Subtract
 
 import logging
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 def test_pipeline(tmp_path):
-    pipeline = Pipeline()
-    pipeline.add_component("first_addition", AddFixedValue(add=2))
-    pipeline.add_component("second_addition", AddFixedValue())
-    pipeline.add_component("double", Double())
-    pipeline.connect("first_addition", "double")
-    pipeline.connect("double", "second_addition")
 
-    pipeline.draw(tmp_path / "linear_pipeline.png")
+    add_two = AddFixedValue(add=2)
+    diff = Subtract()
 
-    results = pipeline.run({"first_addition": {"value": 1}})
+    pipeline = Pipeline()
+    pipeline.add_component("first_addition", add_two)
+    pipeline.add_component("second_addition", add_two)
+    pipeline.add_component("third_addition", add_two)
+    pipeline.add_component("diff", diff)
+    pipeline.add_component("fourth_addition", AddFixedValue(add=1))
+
+    pipeline.connect("first_addition", "second_addition")
+    pipeline.connect("second_addition", "diff.first_value")
+    pipeline.connect("third_addition", "diff.second_value")
+    pipeline.connect("diff", "fourth_addition.value")
+
+    pipeline.draw(tmp_path / "fixed_merging_pipeline.png")
+
+    results = pipeline.run(
+        {
+            "first_addition": AddFixedValue.Input(value=1),
+            "third_addition": AddFixedValue.Input(value=1),
+        }
+    )
     pprint(results)
 
-    assert results == {"second_addition": {"value": 7}}
+    assert results == {"fourth_addition": AddFixedValue.Output(value=3)}
 
 
 if __name__ == "__main__":
     test_pipeline(Path(__file__).parent)
```

### Comparing `canals-0.1.2/test/pipelines/integration/test_looping_and_merge_pipeline.py` & `canals-0.2.0/test/pipelines/integration/test_fixed_decision_and_merge_pipeline.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,44 +1,56 @@
-from typing import *
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+import logging
 from pathlib import Path
 from pprint import pprint
 
 from canals.pipeline import Pipeline
-from test.test_components import Accumulate, AddFixedValue, Threshold, Sum, MergeLoop
-
-import logging
+from test.sample_components import AddFixedValue, Parity, Double, Subtract
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 def test_pipeline(tmp_path):
-    accumulator = Accumulate()
+    add_one = AddFixedValue()
 
-    pipeline = Pipeline(max_loops_allowed=10)
-    pipeline.add_component("merge", MergeLoop(expected_type=int))
-    pipeline.add_component("sum", Sum())
-    pipeline.add_component("below_10", Threshold(threshold=10))
-    pipeline.add_component("add_one", AddFixedValue(add=1))
-    pipeline.add_component("counter", accumulator)
-    pipeline.add_component("add_two", AddFixedValue(add=2))
-
-    pipeline.connect("merge", "below_10")
-    pipeline.connect("below_10.below", "add_one.value")
-    pipeline.connect("add_one", "counter")
-    pipeline.connect("counter", "merge")
-    pipeline.connect("below_10.above", "add_two.value")
-    pipeline.connect("add_two", "sum")
+    pipeline = Pipeline()
+    pipeline.add_component("add_one", add_one)
+    pipeline.add_component("parity", Parity())
+    pipeline.add_component("add_ten", AddFixedValue(add=10))
+    pipeline.add_component("double", Double())
+    pipeline.add_component("add_four", AddFixedValue(add=4))
+    pipeline.add_component("add_two", add_one)
+    pipeline.add_component("diff", Subtract())
+
+    pipeline.connect("add_one", "parity")
+    pipeline.connect("parity.even", "add_four.value")
+    pipeline.connect("parity.odd", "double")
+    pipeline.connect("add_ten", "diff.first_value")
+    pipeline.connect("double", "diff.second_value")
+    pipeline.connect("parity.odd", "add_ten.value")
+    pipeline.connect("add_four", "add_two")
 
-    pipeline.draw(tmp_path / "looping_and_merge_pipeline.png")
+    pipeline.draw(tmp_path / "fixed_decision_and_merge_pipeline.png")
 
     results = pipeline.run(
-        {"merge": {"value": 8}, "sum": {"value": 2}},
+        {
+            "add_one": AddFixedValue.Input(value=1),
+            "add_two": AddFixedValue.Input(add=2),
+        }
     )
     pprint(results)
-    print("accumulate: ", accumulator.state)
+    assert results == {"add_two": AddFixedValue.Output(value=8)}
 
-    assert results == {"sum": {"total": 23}}
-    assert accumulator.state == 19
+    results = pipeline.run(
+        {
+            "add_one": AddFixedValue.Input(value=2),
+            "add_two": AddFixedValue.Input(add=2),
+        }
+    )
+    pprint(results)
+    assert results == {"diff": Subtract.Output(difference=7)}
 
 
 if __name__ == "__main__":
     test_pipeline(Path(__file__).parent)
```

### Comparing `canals-0.1.2/test/pipelines/integration/test_looping_pipeline.py` & `canals-0.2.0/test/pipelines/integration/test_looping_and_merge_pipeline.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,48 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
 from typing import *
 from pathlib import Path
 from pprint import pprint
 
 from canals.pipeline import Pipeline
-from test.test_components import Accumulate, AddFixedValue, Threshold, MergeLoop
+from test.sample_components import Accumulate, AddFixedValue, Threshold, Sum, MergeLoop
 
 import logging
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 def test_pipeline(tmp_path):
     accumulator = Accumulate()
+    merge_loop = MergeLoop(expected_type=int)
 
     pipeline = Pipeline(max_loops_allowed=10)
-    pipeline.add_component("merge", MergeLoop(expected_type=int))
+    pipeline.add_component("merge", merge_loop)
+    pipeline.add_component("sum", Sum())
     pipeline.add_component("below_10", Threshold(threshold=10))
-    pipeline.add_component("accumulator", accumulator)
+    pipeline.add_component("add_one", AddFixedValue(add=1))
+    pipeline.add_component("counter", accumulator)
     pipeline.add_component("add_two", AddFixedValue(add=2))
 
     pipeline.connect("merge", "below_10")
-    pipeline.connect("below_10.below", "accumulator")
-    pipeline.connect("accumulator", "merge")
+    pipeline.connect("below_10.below", "add_one.value")
+    pipeline.connect("add_one", "counter")
+    pipeline.connect("counter", "merge")
     pipeline.connect("below_10.above", "add_two.value")
+    pipeline.connect("add_two", "sum")
 
-    pipeline.draw(tmp_path / "looping_pipeline.png")
+    pipeline.draw(tmp_path / "looping_and_merge_pipeline.png")
 
-    results = pipeline.run({"merge": {"value": 4}})
+    results = pipeline.run(
+        {"merge": merge_loop.input_type(8), "sum": Sum.Input(2)},
+    )
     pprint(results)
-    print("accumulator: ", accumulator.state)
+    print("accumulate: ", accumulator.state)
 
-    assert results == {"add_two": {"value": 18}}
-    assert accumulator.state == 16
+    assert results == {"sum": Sum.Output(total=23)}
+    assert accumulator.state == 19
 
 
 if __name__ == "__main__":
     test_pipeline(Path(__file__).parent)
```

### Comparing `canals-0.1.2/test/pipelines/integration/test_parallel_branches_pipeline.py` & `canals-0.2.0/test/pipelines/integration/test_variable_decision_pipeline.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,41 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
 from pathlib import Path
 from pprint import pprint
 
 from canals.pipeline import Pipeline
-from test.test_components import AddFixedValue, Repeat, Double
+from test.sample_components import AddFixedValue, Remainder, Double
 
 import logging
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 def test_pipeline(tmp_path):
     add_one = AddFixedValue(add=1)
 
     pipeline = Pipeline()
     pipeline.add_component("add_one", add_one)
-    pipeline.add_component("repeat", Repeat(outputs=["first", "second"]))
+    pipeline.add_component("remainder", Remainder(divisor=3))
     pipeline.add_component("add_ten", AddFixedValue(add=10))
     pipeline.add_component("double", Double())
     pipeline.add_component("add_three", AddFixedValue(add=3))
     pipeline.add_component("add_one_again", add_one)
 
-    pipeline.connect("add_one.value", "repeat.value")
-    pipeline.connect("repeat.first", "add_ten.value")
-    pipeline.connect("repeat.second", "double")
-    pipeline.connect("repeat.second", "add_three.value")
+    pipeline.connect("add_one", "remainder")
+    pipeline.connect("remainder.remainder_is_0", "add_ten.value")
+    pipeline.connect("remainder.remainder_is_1", "double")
+    pipeline.connect("remainder.remainder_is_2", "add_three.value")
     pipeline.connect("add_three", "add_one_again")
 
-    pipeline.draw(tmp_path / "parallel_branches_pipeline.png")
+    pipeline.draw(tmp_path / "variable_decision_pipeline.png")
 
-    results = pipeline.run({"add_one": {"value": 1}})
+    results = pipeline.run({"add_one": AddFixedValue.Input(value=1)})
     pprint(results)
 
-    assert results == {
-        "add_one_again": {"value": 6},
-        "add_ten": {"value": 12},
-        "double": {"value": 4},
-    }
+    assert results == {"add_one_again": AddFixedValue.Output(value=6)}
 
 
 if __name__ == "__main__":
     test_pipeline(Path(__file__).parent)
```

### Comparing `canals-0.1.2/test/pipelines/integration/test_variable_decision_and_merge_pipeline.py` & `canals-0.2.0/test/pipelines/integration/test_fixed_decision_pipeline.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,42 @@
-import logging
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
 from pathlib import Path
 from pprint import pprint
 
 from canals.pipeline import Pipeline
-from test.test_components import AddFixedValue, Remainder, Double, Sum
+from test.sample_components import AddFixedValue, Parity, Double
+
+import logging
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 def test_pipeline(tmp_path):
-    add_one = AddFixedValue()
+    add_one = AddFixedValue(add=1)
 
     pipeline = Pipeline()
     pipeline.add_component("add_one", add_one)
-    pipeline.add_component("parity", Remainder())
+    pipeline.add_component("parity", Parity())
     pipeline.add_component("add_ten", AddFixedValue(add=10))
     pipeline.add_component("double", Double())
-    pipeline.add_component("add_four", AddFixedValue(add=4))
-    pipeline.add_component("add_one_again", add_one)
-    pipeline.add_component("sum", Sum())
+    pipeline.add_component("add_three", AddFixedValue(add=3))
 
     pipeline.connect("add_one", "parity")
-    pipeline.connect("parity.remainder_is_0", "add_ten.value")
-    pipeline.connect("parity.remainder_is_1", "double")
-    pipeline.connect("add_one", "sum")
-    pipeline.connect("add_ten", "sum")
-    pipeline.connect("double", "sum")
-    pipeline.connect("parity.remainder_is_1", "add_four.value")
-    pipeline.connect("add_four", "add_one_again")
-    pipeline.connect("add_one_again", "sum")
+    pipeline.connect("parity.even", "add_ten.value")
+    pipeline.connect("parity.odd", "double.value")
+    pipeline.connect("add_ten", "add_three")
 
-    pipeline.draw(tmp_path / "variable_decision_and_merge_pipeline.png")
+    pipeline.draw(tmp_path / "fixed_decision_pipeline.png")
 
-    results = pipeline.run({"add_one": {"value": 1}})
+    results = pipeline.run({"add_one": AddFixedValue.Input(value=1)})
     pprint(results)
-    assert results == {"sum": {"total": 14}}
+    assert results == {"add_three": AddFixedValue.Output(value=15)}
 
-    results = pipeline.run({"add_one": {"value": 2}})
+    results = pipeline.run({"add_one": AddFixedValue.Input(value=2)})
     pprint(results)
-    assert results == {"sum": {"total": 17}}
+    assert results == {"double": Double.Output(value=6)}
 
 
 if __name__ == "__main__":
     test_pipeline(Path(__file__).parent)
```

### Comparing `canals-0.1.2/test/test_components/test_accumulate.py` & `canals-0.2.0/test/sample_components/test_accumulate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,37 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
 from typing import Union, Callable, Optional
 import sys
 import builtins
 from importlib import import_module
 from dataclasses import dataclass
 
 import pytest
-from canals import component
+from canals.component import component, ComponentInput, ComponentOutput
 from canals.testing import BaseTestComponent
 
 
 @component
 class Accumulate:
     """
     Accumulates the value flowing through the connection into an internal attribute.
     The sum function can be customized.
 
     Example of how to deal with serialization when some of the parameters
     are not directly serializable.
-
-    Stateful, single input, single output component.
     """
 
     @dataclass
-    class Output:
+    class Input(ComponentInput):
+        value: int
+
+    @dataclass
+    class Output(ComponentOutput):
         value: int
 
     def __init__(self, function: Optional[Union[Callable, str]] = None):
         """
         :param function: the function to use to accumulate the values.
             The function must take exactly two values.
             If it's a callable, it's used as it is.
@@ -36,18 +41,18 @@
         self.state = 0
 
         if function is None:
             self.function = lambda x, y: x + y
         else:
             self.function = self._load_function(function)
             # 'function' is not serializable by default, so we serialize it manually.
-            self._init_parameters = {"function": self._save_function(function)}
+            self.init_parameters = {"function": self._save_function(function)}
 
-    def run(self, value: int) -> Output:
-        self.state = self.function(self.state, value)
+    def run(self, data: Input) -> Output:
+        self.state = self.function(self.state, data.value)
         return Accumulate.Output(value=self.state)
 
     def _load_function(self, function: Union[Callable, str]):
         """
         Loads the function by trying to import it.
         """
         if not isinstance(function, str):
@@ -81,51 +86,51 @@
 
 class TestAccumulate(BaseTestComponent):
     @pytest.fixture
     def components(self):
         return [
             Accumulate(),
             Accumulate(function=my_subtract),
-            Accumulate(function="test.test_components.test_accumulate.my_subtract"),
+            Accumulate(function="test.sample_components.test_accumulate.my_subtract"),
         ]
 
     def test_accumulate_default(self):
         component = Accumulate()
-        results = component.run(value=10)
+        results = component.run(Accumulate.Input(value=10))
         assert results == Accumulate.Output(value=10)
         assert component.state == 10
 
-        results = component.run(value=1)
+        results = component.run(Accumulate.Input(value=1))
         assert results == Accumulate.Output(value=11)
         assert component.state == 11
 
-        assert component._init_parameters == {}
+        assert component.init_parameters == {}
 
     def test_accumulate_callable(self):
         component = Accumulate(function=my_subtract)
 
-        results = component.run(value=10)
+        results = component.run(Accumulate.Input(value=10))
         assert results == Accumulate.Output(value=-10)
         assert component.state == -10
 
-        results = component.run(value=1)
+        results = component.run(Accumulate.Input(value=1))
         assert results == Accumulate.Output(value=-11)
         assert component.state == -11
 
-        assert component._init_parameters == {
-            "function": "test.test_components.test_accumulate.my_subtract",
+        assert component.init_parameters == {
+            "function": "test.sample_components.test_accumulate.my_subtract",
         }
 
     def test_accumulate_string(self):
-        component = Accumulate(function="test.test_components.test_accumulate.my_subtract")
+        component = Accumulate(function="test.sample_components.test_accumulate.my_subtract")
 
-        results = component.run(value=10)
+        results = component.run(Accumulate.Input(value=10))
         assert results == Accumulate.Output(value=-10)
         assert component.state == -10
 
-        results = component.run(value=1)
+        results = component.run(Accumulate.Input(value=1))
         assert results == Accumulate.Output(value=-11)
         assert component.state == -11
 
-        assert component._init_parameters == {
-            "function": "test.test_components.test_accumulate.my_subtract",
+        assert component.init_parameters == {
+            "function": "test.sample_components.test_accumulate.my_subtract",
         }
```

### Comparing `canals-0.1.2/test/test_components/test_double.py` & `canals-0.2.0/test/sample_components/test_double.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,46 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
 from dataclasses import dataclass
 
 import pytest
 
-from canals import component
+from canals.component import component, ComponentInput, ComponentOutput
 from canals.testing import BaseTestComponent
 
 
 @component
 class Double:
     """
-    Doubles the value in input.
-
-    Single input single output component. Doesn't take parameters.
+    Doubles the input value.
     """
 
     @dataclass
-    class Output:
+    class Input(ComponentInput):
+        value: int
+
+    @dataclass
+    class Output(ComponentOutput):
         value: int
 
-    def run(self, value: int) -> Output:
+    def run(self, data: Input) -> Output:
         """
         Doubles the input value
         """
-        return Double.Output(value=value * 2)
+        return Double.Output(value=data.value * 2)
 
 
 import pytest
 from canals.testing import BaseTestComponent
 
 
 class TestDouble(BaseTestComponent):
     @pytest.fixture
     def components(self):
         return [Double()]
 
     def test_double_default(self):
         component = Double()
-        results = component.run(value=10)
+        results = component.run(Double.Input(value=10))
         assert results == Double.Output(value=20)
-        assert component._init_parameters == {}
+        assert component.init_parameters == {}
```

### Comparing `canals-0.1.2/test/test_components/test_greet.py` & `canals-0.2.0/test/sample_components/test_greet.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,64 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+from typing import Optional
 import logging
 
 from dataclasses import dataclass
 
 import pytest
 
 from canals.testing import BaseTestComponent
-from canals import component
+from canals.component import component, ComponentInput, ComponentOutput
 
 
 logger = logging.getLogger(__name__)
 
 
 @component
 class Greet:
     """
     Logs a greeting message without affecting the value passing on the connection.
     """
 
     @dataclass
-    class Output:
+    class Input(ComponentInput):
         value: int
+        message: str
+        log_level: str
 
-    def __init__(self, message: str = "\nGreeting component says: Hi! The value is {value}\n", log_level: str = "INFO"):
+    @dataclass
+    class Output(ComponentOutput):
+        value: int
+
+    def __init__(
+        self,
+        message: Optional[str] = "\nGreeting component says: Hi! The value is {value}\n",
+        log_level: Optional[str] = "INFO",
+    ):
         """
-        :param message: the message to log. Can use {value} to embed the value.
+        :param message: the message to log. Can use `{value}` to embed the value.
         :param log_level: the level to log at.
         """
-        if not getattr(logging, log_level):
+        if log_level and not getattr(logging, log_level):
             raise ValueError(f"This log level does not exist: {log_level}")
         self.defaults = {"message": message, "log_level": log_level}
 
-    def run(self, value: int, message: str, log_level: str) -> Output:
+    def run(self, data: Input) -> Output:
         """
-        :param message: the message to log. Can use {value} to embed the value.
-        :param log_level: the level to log at.
+        Logs a greeting message without affecting the value passing on the connection.
         """
-        level = getattr(logging, log_level, None)
+        print(data.log_level)
+        level = getattr(logging, data.log_level, None)
         if not level:
-            raise ValueError(f"This log level does not exist: {log_level}")
+            raise ValueError(f"This log level does not exist: {data.log_level}")
 
-        logger.log(level=level, msg=message.format(value=value))
-        return Greet.Output(value=value)
+        logger.log(level=level, msg=data.message.format(value=data.value))
+        return Greet.Output(value=data.value)
 
 
 class TestGreet(BaseTestComponent):
     @pytest.fixture
     def components(self):
         return [
             Greet(),
@@ -52,10 +66,10 @@
             Greet(log_level="WARNING"),
             Greet(message="Hello, that's {value}", log_level="WARNING"),
         ]
 
     def test_greet_message(self, caplog):
         caplog.set_level(logging.WARNING)
         component = Greet()
-        results = component.run(value=10, message="Hello, that's {value}", log_level="WARNING")
+        results = component.run(Greet.Input(value=10, message="Hello, that's {value}", log_level="WARNING"))
         assert results == Greet.Output(value=10)
         assert "Hello, that's 10" in caplog.text
```

### Comparing `canals-0.1.2/test/test_components/test_remainder.py` & `canals-0.2.0/test/sample_components/test_remainder.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,54 +1,65 @@
-from dataclasses import make_dataclass
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+from dataclasses import dataclass, make_dataclass
 
 import pytest
 
 from canals.testing import BaseTestComponent
-from canals import component
+from canals.component import component, ComponentInput, ComponentOutput
 
 
 @component
 class Remainder:
     """
     Redirects the value, unchanged, along the connection corresponding to the remainder
     of a division. For example, if `divisor=3`, the value `5` would be sent along
     the second output connection.
     """
 
+    @dataclass
+    class Input(ComponentInput):
+        value: int
+        add: int = 1
+
     def __init__(self, divisor: int = 2):
         if divisor == 0:
             raise ValueError("Can't divide by zero")
         self.divisor = divisor
-        self._output_type = make_dataclass("Output", [(f"remainder_is_{val}", int, None) for val in range(divisor)])
+
+        self._output_type = make_dataclass(
+            "Output", fields=[(f"remainder_is_{val}", int, None) for val in range(divisor)], bases=(ComponentOutput,)
+        )
 
     @property
     def output_type(self):
         return self._output_type
 
-    def run(self, value: int):
+    def run(self, data: Input):
         """
         :param value: the value to check the remainder of.
         """
-        remainder = value % self.divisor
+        remainder = data.value % self.divisor
         output = self.output_type()
-        setattr(output, f"remainder_is_{remainder}", value)
+        setattr(output, f"remainder_is_{remainder}", data.value)
         return output
 
 
 class TestRemainder(BaseTestComponent):
     @pytest.fixture
     def components(self):
         return [Remainder(), Remainder(divisor=1)]
 
     def test_remainder_default(self):
         component = Remainder()
-        results = component.run(value=3)
+        results = component.run(Remainder.Input(value=3))
         assert results == component.output_type(remainder_is_1=3)
 
     def test_remainder_with_divisor(self):
         component = Remainder(divisor=4)
-        results = component.run(value=3)
+        results = component.run(Remainder.Input(value=3))
         assert results == component.output_type(remainder_is_3=3)
 
     def test_remainder_zero(self):
         with pytest.raises(ValueError):
             Remainder(divisor=0)
```

### Comparing `canals-0.1.2/test/test_components/test_repeat.py` & `canals-0.2.0/test/sample_components/test_sum.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,53 @@
-from typing import TypeVar, Any, List
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+from typing import List
 
-from dataclasses import make_dataclass
+from dataclasses import dataclass
 
 import pytest
 
 from canals.testing import BaseTestComponent
-from canals import component
+from canals.component import component, VariadicComponentInput, ComponentOutput
 
 
 @component
-class Repeat:
+class Sum:
     """
-    Repeats the input value on all outputs.
+    Sums the values of all the input connections together.
     """
 
-    def __init__(self, outputs: List[str] = ["output_1", "output_2", "output_3"]):
-        self.outputs = outputs
-        self._output_type = make_dataclass("Output", [(val, int, None) for val in outputs])
-
-    @property
-    def output_type(self):
-        return self._output_type
-
-    def run(self, value: int):
-        output_dataclass = self.output_type()
-        for output in self.outputs:
-            setattr(output_dataclass, output, value)
-        return output_dataclass
+    @dataclass
+    class Input(VariadicComponentInput):
+        values: List[int]
 
+    @dataclass
+    class Output(ComponentOutput):
+        total: int
 
-class TestRepeat(BaseTestComponent):
+    def run(self, data: Input) -> Output:
+        return Sum.Output(total=sum(data.values))
+
+
+class TestSum(BaseTestComponent):
     @pytest.fixture
     def components(self):
-        return [Repeat(), Repeat(outputs=["one", "two"])]
+        return [Sum()]
 
-    def test_repeat_default(self):
-        component = Repeat()
-        results = component.run(value=10)
-        assert results == component.output_type(output_1=10, output_2=10, output_3=10)
-        assert component._init_parameters == {}
-
-    def test_repeat_init(self):
-        component = Repeat(outputs=["one", "two"])
-        results = component.run(value=10)
-        assert results == component.output_type(one=10, two=10)
-        assert component._init_parameters == {"outputs": ["one", "two"]}
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
+
+    def test_sum_few_values(self):
+        component = Sum()
+        results = component.run(Sum.Input(10, 11, 12))
+        assert results == Sum.Output(total=33)
+        assert component.init_parameters == {}
```

### Comparing `canals-0.1.2/.gitignore` & `canals-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `canals-0.1.2/LICENSE` & `canals-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `canals-0.1.2/pyproject.toml` & `canals-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 [tool.hatch.envs.default]
 dependencies = [
   "pytest",
   "pytest-cov",
   "requests",
 ]
 [tool.hatch.envs.default.scripts]
-cov = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=canals --cov=tests {args}"
+cov = "pytest --cov-report xml:coverage.xml --cov-config=pyproject.toml --cov=canals --cov=tests {args}"
 no-cov = "cov --no-cov {args}"
 
 [[tool.hatch.envs.test.matrix]]
 python = ["38", "39", "310", "311"]
 
 [tool.coverage.run]
 branch = true
```

