# Comparing `tmp/azureml-assets-1.0.0.tar.gz` & `tmp/azureml-assets-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azureml-assets-1.0.0.tar", last modified: Tue May 16 20:28:07 2023, max compression
+gzip compressed data, was "azureml-assets-1.0.1.tar", last modified: Thu May 18 14:11:33 2023, max compression
```

## Comparing `azureml-assets-1.0.0.tar` & `azureml-assets-1.0.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-16 20:28:07.464835 azureml-assets-1.0.0/
--rw-r--r--   0 vsts      (1001) docker     (123)      618 2023-05-16 20:28:07.460835 azureml-assets-1.0.0/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-16 20:28:07.456835 azureml-assets-1.0.0/azureml/
--rw-r--r--   0 vsts      (1001) docker     (123)       75 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-16 20:28:07.460835 azureml-assets-1.0.0/azureml/assets/
--rw-r--r--   0 vsts      (1001) docker     (123)      609 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3788 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/asset_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    35954 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4737 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/copy_assets.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-16 20:28:07.460835 azureml-assets-1.0.0/azureml/assets/environment/
--rw-r--r--   0 vsts      (1001) docker     (123)      244 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/environment/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    15375 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/environment/build.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4773 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/environment/pin_image_versions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5124 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/environment/pin_package_versions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1247 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/environment/pin_versions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4436 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/extract_tagged_assets.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-16 20:28:07.460835 azureml-assets-1.0.0/azureml/assets/model/
--rw-r--r--   0 vsts      (1001) docker     (123)      155 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/model/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1187 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/model/mlflow_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3408 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/model/utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2869 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/tag_released_assets.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10152 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/update_assets.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5934 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/update_spec.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-16 20:28:07.460835 azureml-assets-1.0.0/azureml/assets/util/
--rw-r--r--   0 vsts      (1001) docker     (123)      533 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6906 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/util/logger.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2564 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/util/template.py
--rw-r--r--   0 vsts      (1001) docker     (123)    15565 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/util/util.py
--rw-r--r--   0 vsts      (1001) docker     (123)    15082 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/validate_assets.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-16 20:28:07.460835 azureml-assets-1.0.0/azureml_assets.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      618 2023-05-16 20:28:07.000000 azureml-assets-1.0.0/azureml_assets.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      943 2023-05-16 20:28:07.000000 azureml-assets-1.0.0/azureml_assets.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-16 20:28:07.000000 azureml-assets-1.0.0/azureml_assets.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       44 2023-05-16 20:28:07.000000 azureml-assets-1.0.0/azureml_assets.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        8 2023-05-16 20:28:07.000000 azureml-assets-1.0.0/azureml_assets.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-16 20:28:07.464835 azureml-assets-1.0.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)      954 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:11:33.481663 azureml-assets-1.0.1/
+-rw-r--r--   0 vsts      (1001) docker     (123)      790 2023-05-18 14:11:33.481663 azureml-assets-1.0.1/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:11:33.473663 azureml-assets-1.0.1/azureml/
+-rw-r--r--   0 vsts      (1001) docker     (123)       75 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:11:33.477663 azureml-assets-1.0.1/azureml/assets/
+-rw-r--r--   0 vsts      (1001) docker     (123)      609 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3788 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/asset_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    36250 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4737 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/copy_assets.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:11:33.477663 azureml-assets-1.0.1/azureml/assets/environment/
+-rw-r--r--   0 vsts      (1001) docker     (123)      244 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/environment/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    15375 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/environment/build.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4773 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/environment/pin_image_versions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5124 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/environment/pin_package_versions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1247 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/environment/pin_versions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4436 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/extract_tagged_assets.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:11:33.477663 azureml-assets-1.0.1/azureml/assets/model/
+-rw-r--r--   0 vsts      (1001) docker     (123)      155 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/model/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1187 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/model/mlflow_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3408 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/model/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2869 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/tag_released_assets.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10152 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/update_assets.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5934 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/update_spec.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:11:33.477663 azureml-assets-1.0.1/azureml/assets/util/
+-rw-r--r--   0 vsts      (1001) docker     (123)      533 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6906 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/util/logger.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2564 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/util/template.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    15565 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/util/util.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    15082 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/validate_assets.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:11:33.481663 azureml-assets-1.0.1/azureml_assets.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      790 2023-05-18 14:11:33.000000 azureml-assets-1.0.1/azureml_assets.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      943 2023-05-18 14:11:33.000000 azureml-assets-1.0.1/azureml_assets.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-18 14:11:33.000000 azureml-assets-1.0.1/azureml_assets.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       44 2023-05-18 14:11:33.000000 azureml-assets-1.0.1/azureml_assets.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        8 2023-05-18 14:11:33.000000 azureml-assets-1.0.1/azureml_assets.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-18 14:11:33.481663 azureml-assets-1.0.1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1221 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/setup.py
```

### Comparing `azureml-assets-1.0.0/PKG-INFO` & `azureml-assets-1.0.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: azureml-assets
-Version: 1.0.0
+Version: 1.0.1
 Summary: Utilities for publishing assets to Azure Machine Learning system registries.
 Author: Microsoft Corp
 License: MIT
+Project-URL: Source, https://github.com/Azure/azureml-assets/
+Project-URL: Changelog, https://github.com/Azure/azureml-assets/blob/main/scripts/azureml-assets/CHANGELOG.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `azureml-assets-1.0.0/azureml/assets/__init__.py` & `azureml-assets-1.0.1/azureml/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.0.0/azureml/assets/asset_utils.py` & `azureml-assets-1.0.1/azureml/assets/asset_utils.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.0.0/azureml/assets/config.py` & `azureml-assets-1.0.1/azureml/assets/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import re
 import warnings
 from enum import Enum
 from functools import total_ordering
 from pathlib import Path
 from ruamel.yaml import YAML
 from setuptools._vendor.packaging import version
-from typing import Dict, List, Tuple
+from typing import Dict, List, Tuple, Union
 
 # Ignore setuptools warning about replacing distutils
 warnings.filterwarnings("ignore", message="Setuptools is replacing distutils.", category=UserWarning)
 
 
 class ValidationException(Exception):
     """Validation errors."""
@@ -256,14 +256,24 @@
         """Files that are required to create this asset."""
         release_paths = super().release_paths
         code_dir = self.code_dir_with_path
         if code_dir:
             release_paths.extend(Config._expand_path(code_dir))
         return release_paths
 
+    @property
+    def inference_config(self) -> Dict[str, Dict[str, Union[str, int]]]:
+        """Inference config."""
+        return self._yaml.get('inference_config')
+
+    @property
+    def os_type(self) -> str:
+        """OS type."""
+        return self._yaml.get('os_type')
+
 
 class ModelType(Enum):
     """Enum for the Model Types accepted in ModelConfig."""
 
     MLFLOW = 'mlflow_model'
     CUSTOM = 'custom_model'
     TRITON = 'triton_model'
```

### Comparing `azureml-assets-1.0.0/azureml/assets/copy_assets.py` & `azureml-assets-1.0.1/azureml/assets/copy_assets.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.0.0/azureml/assets/environment/build.py` & `azureml-assets-1.0.1/azureml/assets/environment/build.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.0.0/azureml/assets/environment/pin_image_versions.py` & `azureml-assets-1.0.1/azureml/assets/environment/pin_image_versions.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.0.0/azureml/assets/environment/pin_package_versions.py` & `azureml-assets-1.0.1/azureml/assets/environment/pin_package_versions.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.0.0/azureml/assets/environment/pin_versions.py` & `azureml-assets-1.0.1/azureml/assets/environment/pin_versions.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.0.0/azureml/assets/extract_tagged_assets.py` & `azureml-assets-1.0.1/azureml/assets/extract_tagged_assets.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.0.0/azureml/assets/model/mlflow_utils.py` & `azureml-assets-1.0.1/azureml/assets/model/mlflow_utils.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.0.0/azureml/assets/model/utils.py` & `azureml-assets-1.0.1/azureml/assets/model/utils.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.0.0/azureml/assets/tag_released_assets.py` & `azureml-assets-1.0.1/azureml/assets/tag_released_assets.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.0.0/azureml/assets/update_assets.py` & `azureml-assets-1.0.1/azureml/assets/update_assets.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.0.0/azureml/assets/update_spec.py` & `azureml-assets-1.0.1/azureml/assets/update_spec.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.0.0/azureml/assets/util/__init__.py` & `azureml-assets-1.0.1/azureml/assets/util/__init__.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.0.0/azureml/assets/util/logger.py` & `azureml-assets-1.0.1/azureml/assets/util/logger.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.0.0/azureml/assets/util/template.py` & `azureml-assets-1.0.1/azureml/assets/util/template.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.0.0/azureml/assets/util/util.py` & `azureml-assets-1.0.1/azureml/assets/util/util.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.0.0/azureml/assets/validate_assets.py` & `azureml-assets-1.0.1/azureml/assets/validate_assets.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.0.0/azureml_assets.egg-info/PKG-INFO` & `azureml-assets-1.0.1/azureml_assets.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: azureml-assets
-Version: 1.0.0
+Version: 1.0.1
 Summary: Utilities for publishing assets to Azure Machine Learning system registries.
 Author: Microsoft Corp
 License: MIT
+Project-URL: Source, https://github.com/Azure/azureml-assets/
+Project-URL: Changelog, https://github.com/Azure/azureml-assets/blob/main/scripts/azureml-assets/CHANGELOG.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `azureml-assets-1.0.0/azureml_assets.egg-info/SOURCES.txt` & `azureml-assets-1.0.1/azureml_assets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.0.0/setup.py` & `azureml-assets-1.0.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 """Set up azureml-assets package."""
 
 from setuptools import setup, find_packages
 
 setup(
    name="azureml-assets",
-   version="1.0.0",
+   version="1.0.1",
    description="Utilities for publishing assets to Azure Machine Learning system registries.",
    author="Microsoft Corp",
    packages=find_packages(),
    install_requires=[
       "GitPython>=3.1",
       "ruamel.yaml==0.17.21",
       "pip>=21",
@@ -24,8 +24,13 @@
       "Topic :: Software Development :: Build Tools",
       "License :: OSI Approved :: MIT License",
       "Programming Language :: Python :: 3.8",
       "Programming Language :: Python :: 3.9",
       "Programming Language :: Python :: 3.10",
       "Programming Language :: Python :: 3.11",
    ],
+   project_urls={
+        # 'Documentation': "https://example.com/documentation/",
+        'Source': "https://github.com/Azure/azureml-assets/",
+        'Changelog': "https://github.com/Azure/azureml-assets/blob/main/scripts/azureml-assets/CHANGELOG.md",
+    },
 )
```

