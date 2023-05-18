# Comparing `tmp/cerebrium-0.5.0.tar.gz` & `tmp/cerebrium-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerebrium-0.5.0.tar", max compression
+gzip compressed data, was "cerebrium-0.5.1.tar", max compression
```

## Comparing `cerebrium-0.5.0.tar` & `cerebrium-0.5.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    34594 2023-05-15 14:43:19.864846 cerebrium-0.5.0/LICENSE
--rw-r--r--   0        0        0     3055 2023-05-15 14:43:19.868846 cerebrium-0.5.0/README.md
--rw-r--r--   0        0        0      285 2023-05-15 14:48:30.153519 cerebrium-0.5.0/cerebrium/__init__.py
--rw-r--r--   0        0        0    29484 2023-05-15 14:43:19.868846 cerebrium-0.5.0/cerebrium/conduit.py
--rw-r--r--   0        0        0     4451 2023-05-15 14:43:19.868846 cerebrium-0.5.0/cerebrium/core.py
--rw-r--r--   0        0        0     2524 2023-05-15 14:43:19.868846 cerebrium-0.5.0/cerebrium/errors.py
--rw-r--r--   0        0        0    10839 2023-05-15 14:43:19.868846 cerebrium-0.5.0/cerebrium/flow.py
--rw-r--r--   0        0        0     2807 2023-05-15 14:43:19.868846 cerebrium-0.5.0/cerebrium/logging/arize.py
--rw-r--r--   0        0        0      705 2023-05-15 14:43:19.868846 cerebrium-0.5.0/cerebrium/logging/base.py
--rw-r--r--   0        0        0     3855 2023-05-15 14:43:19.868846 cerebrium-0.5.0/cerebrium/logging/censius.py
--rw-r--r--   0        0        0      801 2023-05-15 14:43:19.868846 cerebrium-0.5.0/cerebrium/models/base.py
--rw-r--r--   0        0        0      446 2023-05-15 14:43:19.868846 cerebrium-0.5.0/cerebrium/models/hf_pipeline.py
--rw-r--r--   0        0        0      418 2023-05-15 14:43:19.868846 cerebrium-0.5.0/cerebrium/models/onnx.py
--rw-r--r--   0        0        0     1116 2023-05-15 14:43:19.868846 cerebrium-0.5.0/cerebrium/models/sklearn.py
--rw-r--r--   0        0        0      244 2023-05-15 14:43:19.868846 cerebrium-0.5.0/cerebrium/models/spacy.py
--rw-r--r--   0        0        0      342 2023-05-15 14:43:19.868846 cerebrium-0.5.0/cerebrium/models/torch.py
--rw-r--r--   0        0        0     4555 2023-05-15 14:43:19.868846 cerebrium-0.5.0/cerebrium/requests.py
--rw-r--r--   0        0        0      465 2023-05-15 14:43:19.868846 cerebrium-0.5.0/cerebrium/utils.py
--rw-r--r--   0        0        0     2227 2023-05-15 14:48:30.153519 cerebrium-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     4979 1970-01-01 00:00:00.000000 cerebrium-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    34594 2023-05-18 18:57:55.262934 cerebrium-0.5.1/LICENSE
+-rw-r--r--   0        0        0     3055 2023-05-18 18:57:55.262934 cerebrium-0.5.1/README.md
+-rw-r--r--   0        0        0      285 2023-05-18 19:02:29.891752 cerebrium-0.5.1/cerebrium/__init__.py
+-rw-r--r--   0        0        0    29945 2023-05-18 18:57:55.262934 cerebrium-0.5.1/cerebrium/conduit.py
+-rw-r--r--   0        0        0     4451 2023-05-18 18:57:55.262934 cerebrium-0.5.1/cerebrium/core.py
+-rw-r--r--   0        0        0     2524 2023-05-18 18:57:55.262934 cerebrium-0.5.1/cerebrium/errors.py
+-rw-r--r--   0        0        0    10839 2023-05-18 18:57:55.262934 cerebrium-0.5.1/cerebrium/flow.py
+-rw-r--r--   0        0        0     2807 2023-05-18 18:57:55.262934 cerebrium-0.5.1/cerebrium/logging/arize.py
+-rw-r--r--   0        0        0      705 2023-05-18 18:57:55.262934 cerebrium-0.5.1/cerebrium/logging/base.py
+-rw-r--r--   0        0        0     3855 2023-05-18 18:57:55.262934 cerebrium-0.5.1/cerebrium/logging/censius.py
+-rw-r--r--   0        0        0      801 2023-05-18 18:57:55.262934 cerebrium-0.5.1/cerebrium/models/base.py
+-rw-r--r--   0        0        0      446 2023-05-18 18:57:55.262934 cerebrium-0.5.1/cerebrium/models/hf_pipeline.py
+-rw-r--r--   0        0        0      418 2023-05-18 18:57:55.262934 cerebrium-0.5.1/cerebrium/models/onnx.py
+-rw-r--r--   0        0        0     1116 2023-05-18 18:57:55.262934 cerebrium-0.5.1/cerebrium/models/sklearn.py
+-rw-r--r--   0        0        0      244 2023-05-18 18:57:55.262934 cerebrium-0.5.1/cerebrium/models/spacy.py
+-rw-r--r--   0        0        0      342 2023-05-18 18:57:55.262934 cerebrium-0.5.1/cerebrium/models/torch.py
+-rw-r--r--   0        0        0     4555 2023-05-18 18:57:55.262934 cerebrium-0.5.1/cerebrium/requests.py
+-rw-r--r--   0        0        0      465 2023-05-18 18:57:55.262934 cerebrium-0.5.1/cerebrium/utils.py
+-rw-r--r--   0        0        0     2353 2023-05-18 19:02:29.887751 cerebrium-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     5088 1970-01-01 00:00:00.000000 cerebrium-0.5.1/PKG-INFO
```

### Comparing `cerebrium-0.5.0/LICENSE` & `cerebrium-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cerebrium-0.5.0/README.md` & `cerebrium-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `cerebrium-0.5.0/cerebrium/conduit.py` & `cerebrium-0.5.1/cerebrium/conduit.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,17 +231,15 @@
 
             # If there are processors, create a processors.py file with the respective processors
             # Save the processors.py file in the /usr/local/lib/python3.10/dist-packages/conduit_processors directory
             if self._processors:
                 if not os.path.exists(
                     ".venv/lib/python3.10/site-packages/conduit_processors"
                 ):
-                    os.makedirs(
-                        ".venv/lib/python3.10/site-packages/conduit_processors"
-                    )
+                    os.makedirs(".venv/lib/python3.10/site-packages/conduit_processors")
                 # Create the processors.py file
                 with open(
                     ".venv/lib/python3.10/site-packages/conduit_processors/processors.py",
                     "w",
                 ) as f:
                     f.write(
                         "from cerebrium import save, get, delete, upload\n"
@@ -656,14 +654,15 @@
                 },
                 enable_spinner=(
                     True,
                     ("Authenticating...", "Authenticated with Cerebrium!"),
                 ),
             )
             upload_url = upload_url_response["data"]["uploadUrl"]
+            project_id = upload_url_response["data"]["projectId"]
 
             # If Prebuilt model, register with modal
             if self.flow[0][0] == ModelType.PREBUILT:
                 print("Registering with Cerebrium...")
                 prebuilt_model_response = _cerebrium_request(
                     "pre-built-model",
                     self.api_key,
@@ -685,13 +684,19 @@
             else:
                 # Upload the conduit artefacts to Cerebrium
                 print("⬆️  Uploading conduit artefacts...")
                 self._upload(upload_url)
                 print("✅ Conduit artefacts uploaded successfully.")
                 endpoint = _poll_deployment_status(self.name, self.api_key)
                 print("🌍 Endpoint:", endpoint)
+                print(
+                    "🚀 Conduit deployed successfully! In some cases, it may take a couple of minutes for the new deployment to become warm, but don't hesitate to contact us if you think something has gone wrong!"
+                )
+                print(
+                    f"You can view your runs at https://dashboard.cerebrium.ai/projects/{project_id}/models/{project_id}-{self.name}?tab=runs"
+                )
                 return endpoint
         else:
             if self.flow[0][0] == ModelType.PREBUILT:
                 raise NotImplementedError("Dry run not supported for prebuilt models")
             self.load(direct_from_flow=True)
             return self
```

### Comparing `cerebrium-0.5.0/cerebrium/core.py` & `cerebrium-0.5.1/cerebrium/core.py`

 * *Files identical despite different names*

### Comparing `cerebrium-0.5.0/cerebrium/errors.py` & `cerebrium-0.5.1/cerebrium/errors.py`

 * *Files identical despite different names*

### Comparing `cerebrium-0.5.0/cerebrium/flow.py` & `cerebrium-0.5.1/cerebrium/flow.py`

 * *Files identical despite different names*

### Comparing `cerebrium-0.5.0/cerebrium/logging/arize.py` & `cerebrium-0.5.1/cerebrium/logging/arize.py`

 * *Files identical despite different names*

### Comparing `cerebrium-0.5.0/cerebrium/logging/base.py` & `cerebrium-0.5.1/cerebrium/logging/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-0.5.0/cerebrium/logging/censius.py` & `cerebrium-0.5.1/cerebrium/logging/censius.py`

 * *Files identical despite different names*

### Comparing `cerebrium-0.5.0/cerebrium/models/base.py` & `cerebrium-0.5.1/cerebrium/models/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-0.5.0/cerebrium/models/sklearn.py` & `cerebrium-0.5.1/cerebrium/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `cerebrium-0.5.0/cerebrium/requests.py` & `cerebrium-0.5.1/cerebrium/requests.py`

 * *Files identical despite different names*

### Comparing `cerebrium-0.5.0/pyproject.toml` & `cerebrium-0.5.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cerebrium"
-version = "0.5.0"
+version = "0.5.1"
 description = ""
 authors = ["Elijah Roussos <elijah@cerebrium.ai>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 exclude = ["tests/*", "dist/*", "worker/*"]
 
 [tool.poetry.urls]
@@ -44,14 +44,16 @@
 datadog = { version = ">=0.45.0,<0.51.0", optional= true }
 Pillow = { version = ">=9.4,<10.0.0", optional= true }
 chitra = { version = ">=0.2.0,<0.3.0", optional= true }
 datasets = { version = ">=2.10.0,<2.11.0", optional= true }
 celery = { version = ">=5.2.0,<5.3.0", optional= true }
 accelerate = { version = ">=0.18.0,<0.19.0", optional= true }
 bitsandbytes = { version = ">=0.38.0,<0.39.0", optional= true }
+tensorflow = { version = ">=2.12.0", optional= true }
+keras = { version = ">=2.12.0", optional= true }
 
 [tool.poetry.group.dev.dependencies]
 black = ">=23.1,<23.2"
 ipython = ">=8.9,<8.10"
 ipykernel = ">=6.21,<6.22"
 poetry-dotenv = "0.3.0"
 poetry-dynamic-versioning = {extras = ["plugin"], version = ">=0.21,<0.22"}
@@ -61,12 +63,12 @@
 pytest-cov = ">=4.0,<4.1"
 notebook = ">=6.5,<6.6"
 torchinfo = ">=1.7,<1.8"
 
 [tool.poetry.extras]
 onnxruntime = ["onnxruntime"]
 onnxruntime-gpu = ["onnxruntime-gpu"]
-worker = ["loguru", "ddtrace", "datadog", "Pillow", "chitra", "datasets", "celery", "accelerate", "bitsandbytes"]
+worker = ["loguru", "ddtrace", "datadog", "Pillow", "chitra", "datasets", "celery", "accelerate", "bitsandbytes", "tensorflow", "keras"]
 
 [build-system]
 requires = ["poetry-core", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `cerebrium-0.5.0/PKG-INFO` & `cerebrium-0.5.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerebrium
-Version: 0.5.0
+Version: 0.5.1
 Summary: 
 License: AGPL-3.0-only
 Author: Elijah Roussos
 Author-email: elijah@cerebrium.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
@@ -22,23 +22,25 @@
 Requires-Dist: celery (>=5.2.0,<5.3.0) ; extra == "worker"
 Requires-Dist: censius (>=1.6,<2.0)
 Requires-Dist: chitra (>=0.2.0,<0.3.0) ; extra == "worker"
 Requires-Dist: cloudpickle (>=2.0,<2.1)
 Requires-Dist: datadog (>=0.45.0,<0.51.0) ; extra == "worker"
 Requires-Dist: datasets (>=2.10.0,<2.11.0) ; extra == "worker"
 Requires-Dist: ddtrace (>=1.10.0,<1.11.0) ; extra == "worker"
+Requires-Dist: keras (>=2.12.0) ; extra == "worker"
 Requires-Dist: loguru (>=0.5,<0.6) ; extra == "worker"
 Requires-Dist: numpy (>=1.20,<2.0)
 Requires-Dist: onnxruntime (>=1.13,<2.0) ; extra == "onnxruntime"
 Requires-Dist: onnxruntime-gpu (>=1.14,<2.0) ; extra == "onnxruntime-gpu"
 Requires-Dist: pandas (>=1.5,<3.0)
 Requires-Dist: requests (>=2.28,<3.0)
 Requires-Dist: scikit-learn (>=1.2,<2.0)
 Requires-Dist: spacy (>=3.5.0,<4.0.0)
 Requires-Dist: tenacity (>=8.2,<8.3)
+Requires-Dist: tensorflow (>=2.12.0) ; extra == "worker"
 Requires-Dist: torch (>=1.13,<3.0)
 Requires-Dist: tqdm (>=4.64,<4.65)
 Requires-Dist: transformers (>=4.26,<5.0)
 Requires-Dist: xgboost (>=1.7,<2.0)
 Requires-Dist: yaspin (>=2.3,<2.4)
 Project-URL: Documentation, https://docs.cerebrium.ai/
 Project-URL: Homepage, https://www.cerebrium.ai
```

