# Comparing `tmp/tango_mlflow-1.0.1.tar.gz` & `tmp/tango_mlflow-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tango_mlflow-1.0.1.tar", max compression
+gzip compressed data, was "tango_mlflow-1.1.0.tar", max compression
```

## Comparing `tango_mlflow-1.0.1.tar` & `tango_mlflow-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1064 2023-04-10 04:52:04.195135 tango_mlflow-1.0.1/LICENSE
--rw-r--r--   0        0        0     1773 2023-04-10 04:52:04.199135 tango_mlflow-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       78 2023-04-10 04:52:04.199135 tango_mlflow-1.0.1/tango_mlflow/__init__.py
--rw-r--r--   0        0        0      129 2023-04-10 04:52:04.199135 tango_mlflow-1.0.1/tango_mlflow/__main__.py
--rw-r--r--   0        0        0      569 2023-04-10 04:52:04.199135 tango_mlflow-1.0.1/tango_mlflow/commands/__init__.py
--rw-r--r--   0        0        0     3633 2023-04-10 04:52:04.199135 tango_mlflow-1.0.1/tango_mlflow/commands/subcommand.py
--rw-r--r--   0        0        0    12913 2023-04-10 04:52:04.199135 tango_mlflow-1.0.1/tango_mlflow/commands/tune.py
--rw-r--r--   0        0        0     6306 2023-04-10 04:52:04.199135 tango_mlflow-1.0.1/tango_mlflow/flax_train_callback.py
--rw-r--r--   0        0        0        0 2023-04-10 04:52:04.199135 tango_mlflow-1.0.1/tango_mlflow/py.typed
--rw-r--r--   0        0        0     1988 2023-04-10 04:52:04.199135 tango_mlflow-1.0.1/tango_mlflow/step.py
--rw-r--r--   0        0        0     6090 2023-04-10 04:52:04.199135 tango_mlflow-1.0.1/tango_mlflow/step_cache.py
--rw-r--r--   0        0        0     7535 2023-04-10 04:52:04.199135 tango_mlflow-1.0.1/tango_mlflow/torch_train_callback.py
--rw-r--r--   0        0        0    11867 2023-04-10 04:52:04.199135 tango_mlflow-1.0.1/tango_mlflow/util.py
--rw-r--r--   0        0        0    18306 2023-04-10 04:52:04.199135 tango_mlflow-1.0.1/tango_mlflow/workspace.py
--rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 tango_mlflow-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-18 17:12:06.213088 tango_mlflow-1.1.0/LICENSE
+-rw-r--r--   0        0        0     5364 2023-05-18 17:12:06.213088 tango_mlflow-1.1.0/README.md
+-rw-r--r--   0        0        0     1908 2023-05-18 17:12:06.217088 tango_mlflow-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       78 2023-05-18 17:12:06.217088 tango_mlflow-1.1.0/tango_mlflow/__init__.py
+-rw-r--r--   0        0        0      129 2023-05-18 17:12:06.217088 tango_mlflow-1.1.0/tango_mlflow/__main__.py
+-rw-r--r--   0        0        0      569 2023-05-18 17:12:06.217088 tango_mlflow-1.1.0/tango_mlflow/commands/__init__.py
+-rw-r--r--   0        0        0     3633 2023-05-18 17:12:06.217088 tango_mlflow-1.1.0/tango_mlflow/commands/subcommand.py
+-rw-r--r--   0        0        0    12913 2023-05-18 17:12:06.217088 tango_mlflow-1.1.0/tango_mlflow/commands/tune.py
+-rw-r--r--   0        0        0     6306 2023-05-18 17:12:06.217088 tango_mlflow-1.1.0/tango_mlflow/flax_train_callback.py
+-rw-r--r--   0        0        0        0 2023-05-18 17:12:06.217088 tango_mlflow-1.1.0/tango_mlflow/py.typed
+-rw-r--r--   0        0        0     1988 2023-05-18 17:12:06.217088 tango_mlflow-1.1.0/tango_mlflow/step.py
+-rw-r--r--   0        0        0     6536 2023-05-18 17:12:06.217088 tango_mlflow-1.1.0/tango_mlflow/step_cache.py
+-rw-r--r--   0        0        0     7535 2023-05-18 17:12:06.217088 tango_mlflow-1.1.0/tango_mlflow/torch_train_callback.py
+-rw-r--r--   0        0        0    11867 2023-05-18 17:12:06.217088 tango_mlflow-1.1.0/tango_mlflow/util.py
+-rw-r--r--   0        0        0    18306 2023-05-18 17:12:06.217088 tango_mlflow-1.1.0/tango_mlflow/workspace.py
+-rw-r--r--   0        0        0     6330 1970-01-01 00:00:00.000000 tango_mlflow-1.1.0/PKG-INFO
```

### Comparing `tango_mlflow-1.0.1/LICENSE` & `tango_mlflow-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tango_mlflow-1.0.1/pyproject.toml` & `tango_mlflow-1.1.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 [tool.poetry]
 name = "tango-mlflow"
-version = "1.0.1"
+version = "1.1.0"
 description = "MLflow integration for ai2-tango"
 authors = ["altescy <altescy@fastmail.com>"]
+license = "MIT License"
+readme = "README.md"
+homepage = "https://github.com/altescy/tango-mlflow"
+keywords=["python", "mlflow", "machine-learning"]
 
 [tool.poetry.scripts]
 tango-mlflow = "tango_mlflow.__main__:run"
 
 [tool.poetry.dependencies]
-python = ">=3.8.1,<3.11"
+python = ">=3.8.1,<4.0"
 ai2-tango = "^1.0.0"
 mlflow = ">=1.28,<3.0"
 optuna = {version = "^3.0.5", optional = true}
 torch = {version = "^2.0.0", optional = true}
 flax = {version = "^0.6.8", optional = true}
 
 [tool.poetry.dev-dependencies]
 python-language-server = "^0.36.2"
-pytest = "^7.1.3"
-pysen = {version = "^0.10.2"}
-black = "^22.8.0"
-isort = "^5.10.1"
+pytest = "^7.3.1"
+pysen = "^0.10.4"
+black = "^23.3.0"
+isort = "^5.12.0"
 flake8 = "^5.0.4"
-mypy = "^0.991"
-llvmlite = "^0.39.1"
-numba = "^0.56.4"
+mypy = "^1.2.0"
+llvmlite = "^0.40.0"
+numba = "^0.57.0"
 
 [tool.poetry.extras]
 optuna = ["optuna"]
 torch = ["torch"]
 flax = ["flax"]
 all = ["optuna", "torch", "flax"]
```

### Comparing `tango_mlflow-1.0.1/tango_mlflow/commands/__init__.py` & `tango_mlflow-1.1.0/tango_mlflow/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `tango_mlflow-1.0.1/tango_mlflow/commands/subcommand.py` & `tango_mlflow-1.1.0/tango_mlflow/commands/subcommand.py`

 * *Files identical despite different names*

### Comparing `tango_mlflow-1.0.1/tango_mlflow/commands/tune.py` & `tango_mlflow-1.1.0/tango_mlflow/commands/tune.py`

 * *Files identical despite different names*

### Comparing `tango_mlflow-1.0.1/tango_mlflow/flax_train_callback.py` & `tango_mlflow-1.1.0/tango_mlflow/flax_train_callback.py`

 * *Files identical despite different names*

### Comparing `tango_mlflow-1.0.1/tango_mlflow/step.py` & `tango_mlflow-1.1.0/tango_mlflow/step.py`

 * *Files identical despite different names*

### Comparing `tango_mlflow-1.0.1/tango_mlflow/step_cache.py` & `tango_mlflow-1.1.0/tango_mlflow/step_cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -116,21 +116,29 @@
             result = metadata.format.read(self.step_dir(step))
             self._add_to_cache(key, result)
             return result
 
         # Next check our local on-disk cache
         with self._acquire_step_lock_file(step, read_only_ok=True):
             if self.step_dir(step).is_dir():
-                return load_and_return()
+                try:
+                    return load_and_return()
+                except FileNotFoundError:
+                    logger.info("Spep cache is incomplete, trying to re-download it from MLflow...")
+                    shutil.rmtree(self.step_dir(step))
 
         # Finally, check MLflow for the corresponding artifact.
         with self._acquire_step_lock_file(step):
             # Make sure the step wasn't cached since the last time we checked (above).
             if self.step_dir(step).is_dir():
-                return load_and_return()
+                try:
+                    return load_and_return()
+                except FileNotFoundError:
+                    logger.info("Spep cache is incomplete, trying to re-download it from MLflow...")
+                    shutil.rmtree(self.step_dir(step))
 
             mlflow_run = self.get_step_result_mlflow_run(step)
             if mlflow_run is None:
                 raise KeyError(step)
 
             with tempfile.TemporaryDirectory(dir=self.dir, prefix=key) as temp_dir:
                 mlflow.artifacts.download_artifacts(
```

### Comparing `tango_mlflow-1.0.1/tango_mlflow/torch_train_callback.py` & `tango_mlflow-1.1.0/tango_mlflow/torch_train_callback.py`

 * *Files identical despite different names*

### Comparing `tango_mlflow-1.0.1/tango_mlflow/util.py` & `tango_mlflow-1.1.0/tango_mlflow/util.py`

 * *Files identical despite different names*

### Comparing `tango_mlflow-1.0.1/tango_mlflow/workspace.py` & `tango_mlflow-1.1.0/tango_mlflow/workspace.py`

 * *Files identical despite different names*

