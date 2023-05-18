# Comparing `tmp/improveai-7.2.1.tar.gz` & `tmp/improveai-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "improveai-7.2.1.tar", last modified: Mon Nov 14 22:17:21 2022, max compression
+gzip compressed data, was "improveai-8.0.0.tar", last modified: Thu May 18 00:30:16 2023, max compression
```

## Comparing `improveai-7.2.1.tar` & `improveai-8.0.0.tar`

### file list

```diff
@@ -1,38 +1,33 @@
-drwxr-xr-x   0 justin     (501) staff       (20)        0 2022-11-14 22:17:21.478109 improveai-7.2.1/
--rw-r--r--   0 justin     (501) staff       (20)      929 2022-09-29 16:47:42.000000 improveai-7.2.1/LICENSE
--rw-r--r--   0 justin     (501) staff       (20)      198 2022-09-29 16:47:42.000000 improveai-7.2.1/MANIFEST.in
--rw-r--r--   0 justin     (501) staff       (20)     7828 2022-11-14 22:17:21.478186 improveai-7.2.1/PKG-INFO
--rwxr-xr-x   0 justin     (501) staff       (20)     6436 2022-11-14 22:14:27.000000 improveai-7.2.1/README.md
-drwxr-xr-x   0 justin     (501) staff       (20)        0 2022-11-14 22:17:21.476328 improveai-7.2.1/improveai/
--rwxr-xr-x   0 justin     (501) staff       (20)     1240 2022-11-14 22:14:27.000000 improveai-7.2.1/improveai/__init__.py
--rw-r--r--   0 justin     (501) staff       (20)    20722 2022-11-14 22:14:27.000000 improveai-7.2.1/improveai/chooser.py
-drwxr-xr-x   0 justin     (501) staff       (20)        0 2022-11-14 22:17:21.477463 improveai-7.2.1/improveai/cythonized_feature_encoding/
--rw-r--r--   0 justin     (501) staff       (20)     1542 2022-09-29 16:47:42.000000 improveai-7.2.1/improveai/cythonized_feature_encoding/__init__.py
--rw-r--r--   0 justin     (501) staff       (20)        0 2022-09-29 16:47:42.000000 improveai-7.2.1/improveai/cythonized_feature_encoding/__init__.pyx
--rw-r--r--   0 justin     (501) staff       (20)    17173 2022-11-14 22:14:27.000000 improveai-7.2.1/improveai/cythonized_feature_encoding/cythonized_feature_encoder.pyx
--rw-r--r--   0 justin     (501) staff       (20)     6129 2022-09-29 16:47:42.000000 improveai-7.2.1/improveai/cythonized_feature_encoding/cythonized_feature_encoding_utils.pyx
--rw-r--r--   0 justin     (501) staff       (20)      340 2022-09-29 16:47:42.000000 improveai-7.2.1/improveai/cythonized_feature_encoding/npy_no_deprecated_api.h
--rwxr-xr-x   0 justin     (501) staff       (20)     4384 2022-11-14 22:14:27.000000 improveai-7.2.1/improveai/decision.py
--rw-r--r--   0 justin     (501) staff       (20)    12351 2022-11-14 22:14:27.000000 improveai-7.2.1/improveai/decision_context.py
--rwxr-xr-x   0 justin     (501) staff       (20)    25254 2022-11-14 22:14:27.000000 improveai-7.2.1/improveai/decision_model.py
--rwxr-xr-x   0 justin     (501) staff       (20)    18438 2022-11-14 22:14:27.000000 improveai-7.2.1/improveai/decision_tracker.py
--rwxr-xr-x   0 justin     (501) staff       (20)    16577 2022-11-14 22:14:27.000000 improveai-7.2.1/improveai/feature_encoder.py
--rw-r--r--   0 justin     (501) staff       (20)      710 2022-11-14 22:14:27.000000 improveai-7.2.1/improveai/givens_provider.py
--rwxr-xr-x   0 justin     (501) staff       (20)     5446 2022-11-14 22:14:27.000000 improveai-7.2.1/improveai/improve_model_cli.py
--rw-r--r--   0 justin     (501) staff       (20)      785 2022-11-14 22:14:27.000000 improveai-7.2.1/improveai/settings.py
-drwxr-xr-x   0 justin     (501) staff       (20)        0 2022-11-14 22:17:21.478012 improveai-7.2.1/improveai/utils/
--rwxr-xr-x   0 justin     (501) staff       (20)        0 2022-09-29 16:47:42.000000 improveai-7.2.1/improveai/utils/__init__.py
--rw-r--r--   0 justin     (501) staff       (20)     2521 2022-09-29 16:47:42.000000 improveai-7.2.1/improveai/utils/choosers_feature_encoding_tools.py
--rwxr-xr-x   0 justin     (501) staff       (20)     5334 2022-11-14 22:14:27.000000 improveai-7.2.1/improveai/utils/general_purpose_tools.py
--rwxr-xr-x   0 justin     (501) staff       (20)     2635 2022-11-14 22:14:27.000000 improveai-7.2.1/improveai/utils/gzip_tools.py
--rwxr-xr-x   0 justin     (501) staff       (20)     1229 2022-09-29 16:47:42.000000 improveai-7.2.1/improveai/utils/url_tools.py
-drwxr-xr-x   0 justin     (501) staff       (20)        0 2022-11-14 22:17:21.476925 improveai-7.2.1/improveai.egg-info/
--rw-r--r--   0 justin     (501) staff       (20)     7828 2022-11-14 22:17:21.000000 improveai-7.2.1/improveai.egg-info/PKG-INFO
--rw-r--r--   0 justin     (501) staff       (20)     1010 2022-11-14 22:17:21.000000 improveai-7.2.1/improveai.egg-info/SOURCES.txt
--rw-r--r--   0 justin     (501) staff       (20)        1 2022-11-14 22:17:21.000000 improveai-7.2.1/improveai.egg-info/dependency_links.txt
--rw-r--r--   0 justin     (501) staff       (20)        1 2022-11-14 22:01:05.000000 improveai-7.2.1/improveai.egg-info/not-zip-safe
--rw-r--r--   0 justin     (501) staff       (20)       79 2022-11-14 22:17:21.000000 improveai-7.2.1/improveai.egg-info/requires.txt
--rw-r--r--   0 justin     (501) staff       (20)       10 2022-11-14 22:17:21.000000 improveai-7.2.1/improveai.egg-info/top_level.txt
--rw-r--r--   0 justin     (501) staff       (20)      135 2022-09-29 16:47:42.000000 improveai-7.2.1/pyproject.toml
--rw-r--r--   0 justin     (501) staff       (20)     1314 2022-11-14 22:17:21.478489 improveai-7.2.1/setup.cfg
--rwxr-xr-x   0 justin     (501) staff       (20)     2215 2022-09-29 16:47:42.000000 improveai-7.2.1/setup.py
+drwxr-xr-x   0 justin     (501) staff       (20)        0 2023-05-18 00:30:16.642102 improveai-8.0.0/
+-rw-r--r--   0 justin     (501) staff       (20)     1076 2023-05-18 00:01:05.000000 improveai-8.0.0/LICENSE
+-rw-r--r--   0 justin     (501) staff       (20)      198 2022-09-29 16:47:42.000000 improveai-8.0.0/MANIFEST.in
+-rw-r--r--   0 justin     (501) staff       (20)    11318 2023-05-18 00:30:16.642166 improveai-8.0.0/PKG-INFO
+-rwxr-xr-x   0 justin     (501) staff       (20)     9963 2023-05-18 00:01:05.000000 improveai-8.0.0/README.md
+drwxr-xr-x   0 justin     (501) staff       (20)        0 2023-05-18 00:30:16.638443 improveai-8.0.0/improveai/
+-rwxr-xr-x   0 justin     (501) staff       (20)     1152 2023-05-17 02:39:37.000000 improveai-8.0.0/improveai/__init__.py
+-rw-r--r--   0 justin     (501) staff       (20)    21743 2023-05-17 02:39:37.000000 improveai-8.0.0/improveai/chooser.py
+drwxr-xr-x   0 justin     (501) staff       (20)        0 2023-05-18 00:30:16.641451 improveai-8.0.0/improveai/cythonized_feature_encoding/
+-rw-r--r--   0 justin     (501) staff       (20)     1352 2023-05-17 02:39:37.000000 improveai-8.0.0/improveai/cythonized_feature_encoding/__init__.py
+-rw-r--r--   0 justin     (501) staff       (20)        0 2022-09-29 16:47:42.000000 improveai-8.0.0/improveai/cythonized_feature_encoding/__init__.pyx
+-rw-r--r--   0 justin     (501) staff       (20)    14707 2023-05-17 02:39:37.000000 improveai-8.0.0/improveai/cythonized_feature_encoding/cythonized_feature_encoder.pyx
+-rw-r--r--   0 justin     (501) staff       (20)      340 2022-09-29 16:47:42.000000 improveai-8.0.0/improveai/cythonized_feature_encoding/npy_no_deprecated_api.h
+-rwxr-xr-x   0 justin     (501) staff       (20)    14325 2023-05-17 02:39:37.000000 improveai-8.0.0/improveai/feature_encoder.py
+-rw-r--r--   0 justin     (501) staff       (20)     3675 2023-05-18 00:01:05.000000 improveai-8.0.0/improveai/ranker.py
+-rw-r--r--   0 justin     (501) staff       (20)    15450 2023-05-18 00:01:05.000000 improveai-8.0.0/improveai/reward_tracker.py
+-rw-r--r--   0 justin     (501) staff       (20)     3275 2023-05-18 00:01:05.000000 improveai-8.0.0/improveai/scorer.py
+-rw-r--r--   0 justin     (501) staff       (20)      785 2023-05-17 02:39:22.000000 improveai-8.0.0/improveai/settings.py
+drwxr-xr-x   0 justin     (501) staff       (20)        0 2023-05-18 00:30:16.642012 improveai-8.0.0/improveai/utils/
+-rwxr-xr-x   0 justin     (501) staff       (20)        0 2022-09-29 16:47:42.000000 improveai-8.0.0/improveai/utils/__init__.py
+-rwxr-xr-x   0 justin     (501) staff       (20)     3023 2023-05-17 02:39:37.000000 improveai-8.0.0/improveai/utils/general_purpose_tools.py
+-rwxr-xr-x   0 justin     (501) staff       (20)     3087 2023-05-17 02:39:37.000000 improveai-8.0.0/improveai/utils/gzip_tools.py
+-rwxr-xr-x   0 justin     (501) staff       (20)     1303 2023-05-17 02:39:37.000000 improveai-8.0.0/improveai/utils/url_tools.py
+drwxr-xr-x   0 justin     (501) staff       (20)        0 2023-05-18 00:30:16.641009 improveai-8.0.0/improveai.egg-info/
+-rw-r--r--   0 justin     (501) staff       (20)    11318 2023-05-18 00:30:16.000000 improveai-8.0.0/improveai.egg-info/PKG-INFO
+-rw-r--r--   0 justin     (501) staff       (20)      781 2023-05-18 00:30:16.000000 improveai-8.0.0/improveai.egg-info/SOURCES.txt
+-rw-r--r--   0 justin     (501) staff       (20)        1 2023-05-18 00:30:16.000000 improveai-8.0.0/improveai.egg-info/dependency_links.txt
+-rw-r--r--   0 justin     (501) staff       (20)        1 2022-11-14 22:01:05.000000 improveai-8.0.0/improveai.egg-info/not-zip-safe
+-rw-r--r--   0 justin     (501) staff       (20)       79 2023-05-18 00:30:16.000000 improveai-8.0.0/improveai.egg-info/requires.txt
+-rw-r--r--   0 justin     (501) staff       (20)       10 2023-05-18 00:30:16.000000 improveai-8.0.0/improveai.egg-info/top_level.txt
+-rw-r--r--   0 justin     (501) staff       (20)      135 2022-09-29 16:47:42.000000 improveai-8.0.0/pyproject.toml
+-rw-r--r--   0 justin     (501) staff       (20)     1314 2023-05-18 00:30:16.642447 improveai-8.0.0/setup.cfg
+-rwxr-xr-x   0 justin     (501) staff       (20)     1606 2023-05-17 02:39:37.000000 improveai-8.0.0/setup.py
```

### Comparing `improveai-7.2.1/improveai/chooser.py` & `improveai-8.0.0/improveai/chooser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,42 @@
-from collections.abc import Iterable
-from copy import deepcopy
 import json
 import numpy as np
 from pathlib import Path
 import pickle
 import re
 from traceback import print_exc
 from xgboost import Booster, DMatrix
 from xgboost.core import XGBoostError
 
 from improveai.feature_encoder import FeatureEncoder
 from improveai.settings import CYTHON_BACKEND_AVAILABLE
-from improveai.utils.choosers_feature_encoding_tools import encoded_variants_to_np
 from improveai.utils.gzip_tools import check_and_get_unzipped_model
 from improveai.utils.url_tools import is_path_http_addr, get_model_bytes_from_url
 
 
 if CYTHON_BACKEND_AVAILABLE:
-    from improveai.cythonized_feature_encoding import cfe, cfeu
+    from improveai.cythonized_feature_encoding import cfe
     FastFeatureEncoder = cfe.FeatureEncoder
-    fast_encoded_variants_to_np = cfeu.encoded_variants_to_np
-    fast_encode_variants_single_givens = cfeu.encode_variants_single_givens
+    fast_encode_candidates_to_matrix = cfe.encode_candidates_to_matrix
 else:
     FastFeatureEncoder = FeatureEncoder
 
 
+USER_DEFINED_METADATA_KEY = 'user_defined_metadata'
+"""
+Key used to store Improve AI metadata inside booster (<booster>.attr(USER_DEFINED_METADATA_KEY))
+"""
+
+FEATURE_NAMES_METADATA_KEY = 'ai.improve.features'
+"""
+Key used to store Improve AI booster feature names. During booster's  save procedure
+feature names are truncated from booster.
+"""
+
+
 class XGBChooser:
     MODEL_NAME_REGEXP = "^[a-zA-Z0-9][\w\-.]{0,63}$"
     """
     Model name regexp used to verify all model names (both user provided and cached in boosters)
     """
 
     @property
@@ -79,86 +87,17 @@
         return self._feature_encoder
 
     @feature_encoder.setter
     def feature_encoder(self, new_val: FeatureEncoder or FastFeatureEncoder):
         self._feature_encoder = new_val
 
     @property
-    def model_metadata_key(self):
-        """
-        'User defined' metadata is stored inside Improve AI Booster. Inside a
-        'user defined' metadata 'model metadata' is stored under `model_metadata_key`
-
-        Returns
-        -------
-        str
-            `model_metadata` key inside `user_defined_metadata`
-
-        """
-        return self._mlmodel_metadata_key
-
-    @model_metadata_key.setter
-    def model_metadata_key(self, new_val: str):
-        self._mlmodel_metadata_key = new_val
-
-    @property
-    def model_seed_key(self) -> str:
-        """
-        `model_seed` key  in `model_metadata` dict
-
-        Returns
-        -------
-        str
-            `model_seed` key  in `model_metadata` dict
-
-        """
-        return self._model_seed_key
-
-    @model_seed_key.setter
-    def model_seed_key(self, new_val: str):
-        self._model_seed_key = new_val
-
-    @property
-    def model_seed(self):
-        """
-        Model seed needed for FeatureEncoder constructor
-
-        Returns
-        -------
-        int
-            Model seed needed for FeatureEncoder constructor
-
-        """
-        return self._model_seed
-
-    @model_seed.setter
-    def model_seed(self, value):
-        self._model_seed = value
-
-    @property
-    def model_name_key(self):
-        """
-        `model_name` key  in `model_metadata` dict
-
-        Returns
-        -------
-        str
-            `model_name` key  in `model_metadata` dict
-
-        """
-        return self._model_name_key
-
-    @model_name_key.setter
-    def model_name_key(self, value):
-        self._model_name_key = value
-
-    @property
     def model_name(self):
         """
-        Model name of this Improve AI model
+        Model name for this Improve AI model
 
         Returns
         -------
         str
             Model name of this Improve AI model
 
         """
@@ -169,51 +108,34 @@
         assert value is not None
         assert isinstance(value, str)
         assert re.search(XGBChooser.MODEL_NAME_REGEXP, value) is not None
 
         self._model_name = value
 
     @property
-    def model_feature_names_key(self) -> str:
-        """
-        `model_feature_names` key  in `model_metadata` dict
-
-        Returns
-        -------
-        str
-            `model_feature_names` key  in `model_metadata` dict
-
-        """
-        return self._model_feature_names_key
-
-    @model_feature_names_key.setter
-    def model_feature_names_key(self, new_val: str):
-        self._model_feature_names_key = new_val
-
-    @property
-    def model_feature_names(self) -> list:
+    def feature_names(self) -> list:
         """
         Feature names of this Improve AI model
 
         Returns
         -------
         list
             Feature names of this Improve AI model
 
         """
         return self._model_feature_names
 
-    @model_feature_names.setter
-    def model_feature_names(self, new_val: list):
+    @feature_names.setter
+    def feature_names(self, new_val: list):
         self._model_feature_names = new_val
 
     @property
     def current_noise(self):
         """
-        Currently used noise value. Needed for SDK + synthetic model validation
+        Currently used noise value. Needed for SDK validation with synthetic models.
 
         Returns
         -------
         float
             Currently used noise
 
         """
@@ -222,15 +144,15 @@
     @current_noise.setter
     def current_noise(self, value):
         self._current_noise = value
 
     @property
     def imposed_noise(self):
         """
-        Forced noise value. Needed for SDK + synthetic model validation
+        Imposed noise value. Needed for SDK validation with synthetic models.
 
         Returns
         -------
         float
             Forced noise value
 
         """
@@ -257,103 +179,145 @@
         return self._improveai_model_version
 
     @improveai_major_version_from_metadata.setter
     def improveai_major_version_from_metadata(self, value):
         self._improveai_model_version = value
 
     @property
-    def MODEL_METADATA_KEY(self):
+    def FEATURE_NAMES_METADATA_KEY(self):
         """
-        Key in booster.attr('user_defined_metadata') storing model metadata
+        Key in model metadata storing feature names
 
         Returns
         -------
         str
-            json string
+            'ai.improve.features'
 
         """
-        return 'json'
+        return FEATURE_NAMES_METADATA_KEY
 
     @property
-    def MODEL_FEATURE_NAMES_KEY(self):
+    def STRING_TABLES_METADATA_KEY(self):
         """
-        Key in model metadata storing feature names
+        Key in model metadata storing string tables
 
         Returns
         -------
         str
-            'feature_names'
+            'ai.improve.string_tables'
 
         """
-        return 'feature_names'
+        return 'ai.improve.string_tables'
 
     @property
-    def MODEL_SEED_KEY(self):
+    def MODEL_SEED_METADATA_KEY(self):
         """
         Key in model metadata storing model seed
 
         Returns
         -------
         str
-            'model_seed'
+            'ai.improve.seed'
 
         """
-        return 'model_seed'
+        return 'ai.improve.seed'
 
     @property
-    def MODEL_NAME_KEY(self):
+    def MODEL_NAME_METADATA_KEY(self):
         """
         Key in model metadata storing model name
 
         Returns
         -------
         str
-            'model_name'
+            'ai.improve.model'
+
+        """
+        return 'ai.improve.model'
+
+    @property
+    def CREATED_AT_METADATA_KEY(self):
+        """
+        Key in model metadata storing model creation time
+
+        Returns
+        -------
+        str
+            'ai.improve.created_at'
 
         """
-        return 'model_name'
+        return 'ai.improve.created_at'
 
     @property
     def IMPROVE_AI_ALLOWED_MAJOR_VERSION(self):
         """
         Latest supported major model version
 
         Returns
         -------
         int
-            7
+            8
 
         """
-        return 7
+        return 8
 
     @property
-    def IMPROVEAI_VERSION_KEY(self):
+    def VERSION_METADATA_KEY(self):
         """
         model metadata key storing model version
 
         Returns
         -------
         str
             'ai.improve.version'
 
         """
         return 'ai.improve.version'
 
+    @property
+    def USER_DEFINED_METADATA_KEY(self):
+        """
+        booster's attribute name storing an entire user defined metadata dict
+
+        Returns
+        -------
+        str
+            'user_defined_metadata'
+
+        """
+        return USER_DEFINED_METADATA_KEY
+
+    @property
+    def REQUIRED_METADATA_KEYS(self):
+        """
+        keys expected / required in model metadata
+
+        Returns
+        -------
+        str
+            list of required keys present in model metadata
+
+        """
+
+        return [
+            self.MODEL_NAME_METADATA_KEY, self.FEATURE_NAMES_METADATA_KEY,
+            self.STRING_TABLES_METADATA_KEY, self.MODEL_SEED_METADATA_KEY,
+            self.CREATED_AT_METADATA_KEY, self.VERSION_METADATA_KEY]
+
     def __init__(self):
         """
         Initialize chooser object
         """
 
         self.model = None
         self.model_metadata = None
 
         self.feature_encoder = None
-        self.model_feature_names = np.empty(shape=(1,))
+        self.feature_names = None
 
-        self.model_seed = None
         self._model_name = None
         self.current_noise = None
         self._imposed_noise = None
         self._improveai_major_version_from_metadata = None
 
     def load_model(self, input_model_src: str, verbose: bool = False):
         """
@@ -361,27 +325,25 @@
 
         Parameters
         ----------
         input_model_src: str
             URL / path to desired model
         verbose: bool
             should I print debug messages
-        Returns
-        -------
-        None
-            None
+
         """
 
         try:
             if verbose:
                 print('Attempting to load: {} model'.format(
                     input_model_src if len(input_model_src) < 100 else
                     str(input_model_src[:10]) + ' ... ' + str(
                         input_model_src[-10:])))
 
+            input_model_src = XGBChooser.get_model_src(model_src=input_model_src)
             model_src = \
                 input_model_src if isinstance(input_model_src, str) or isinstance(input_model_src, Path) \
                 else bytearray(input_model_src)
 
             self.model = Booster()
             self.model.load_model(model_src)
             if verbose:
@@ -395,246 +357,271 @@
             with open(input_model_src, 'rb') as xgbl:
                 self.model = pickle.load(xgbl)
             print_exc()
         except Exception as exc:
             if verbose:
                 print(
                     'When attempting to load the model: {} the following error '
-                    'occured: {}'.format(input_model_src, exc))
-            print_exc()
+                    'occurred: {}'.format(input_model_src, exc))
+            raise exc
 
         model_metadata = self._get_model_metadata()
-        self.model_seed = self._get_model_seed(model_metadata=model_metadata)
+        model_seed = self._get_model_seed(model_metadata=model_metadata)
         self.model_name = self._get_model_name(model_metadata=model_metadata)
-        self.model_feature_names = \
-            self._get_model_feature_names(model_metadata=model_metadata)
+        self.feature_names = self._get_model_feature_names(model_metadata=model_metadata)
+        string_tables = self._get_string_tables(model_metadata=model_metadata)
         self.improveai_major_version_from_metadata = \
             self._get_improveai_major_version(model_metadata=model_metadata)
 
         if CYTHON_BACKEND_AVAILABLE:
-            self.feature_encoder = FastFeatureEncoder(model_seed=self.model_seed)
+            self.feature_encoder = FastFeatureEncoder(
+                feature_names=self.feature_names, string_tables=string_tables, model_seed=model_seed)
         else:
-            self.feature_encoder = FeatureEncoder(model_seed=self.model_seed)
+            self.feature_encoder = FeatureEncoder(
+                feature_names=self.feature_names, string_tables=string_tables, model_seed=model_seed)
 
-    def _get_improveai_major_version(self, model_metadata: dict) -> str or None:
+    def _get_noise(self) -> float:
         """
-        Extract Improve AI version from model metadata and return it if it is valid / allowed
-
-        Parameters
-        ----------
-        model_metadata: dict
-            a dictionary containing model metadata
+        Private noise getter. Noise can be set manually - this was provided for
+        testing purposes. Please note that the 'natural' flow is for
+        noise to be randomly sampled from 0-1 uniform distribution.
 
         Returns
         -------
-        str or None
-            major Improve AI version extracted from loaded improve model
-        """
-        improveai_major_version = None
-        if self.IMPROVEAI_VERSION_KEY in model_metadata.keys():
-            improveai_version = model_metadata[self.IMPROVEAI_VERSION_KEY]
+        float
+            noise used by chooser
 
-            print('### improveai_version ###')
-            print(improveai_version)
+        """
+        if self.imposed_noise is None:
+            noise = np.random.rand()
+        else:
+            noise = self.imposed_noise
 
-            assert improveai_version is not None and isinstance(improveai_version, str)
-            # major version is the first chunk of version string
-            improveai_major_version = int(improveai_version.split('.')[0])
-            assert improveai_major_version == self.IMPROVE_AI_ALLOWED_MAJOR_VERSION
-        return improveai_major_version
+        return noise
 
-    def _get_model_metadata(self) -> dict:
+    def encode_candidates_to_matrix(
+            self, candidates: list or tuple or np.ndarray, context: object, noise: float = 0.0):
         """
-        gets 'model metadata' from 'user defined metadata' of Improve AI model
+        Encodes list of candidates to 2D np.array for a given context with provided noise
+
+        Parameters
+        ----------
+        candidates: list or tuple or np.ndarray
+            list of JSON encodable candidates / items to encode
+        context: object
+            JSON encodable object
+        noise: float
+            noise to be used for sprinkling of encoded features
 
         Returns
         -------
-        dict
-            dict with model metadata
+        np.ndarray
+            2D numpy array with encoded candidates
+
         """
+        into_matrix = np.full((len(candidates), len(self.feature_encoder.feature_indexes)), np.nan)
 
-        assert 'user_defined_metadata' in self.model.attributes().keys()
-        user_defined_metadata_str = self.model.attr('user_defined_metadata')
-        user_defined_metadata = json.loads(user_defined_metadata_str)
-        assert self.MODEL_METADATA_KEY in user_defined_metadata.keys()
+        for item, into_row in zip(candidates, into_matrix):
+            self.feature_encoder.encode_feature_vector(item=item, context=context, into=into_row, noise=noise)
 
-        return user_defined_metadata[self.MODEL_METADATA_KEY]
+        return into_matrix
 
-    def score(self, variants: list or tuple or np.ndarray, givens: dict or None, **kwargs) -> np.ndarray:
+    def score(self, candidates: list or tuple or np.ndarray, context: dict or None, **kwargs) -> np.ndarray:
         """
-        Scores all provided variants
+        Calculates scores for all provided candidates in 2 steps:
+
+        1. encodes candidates to np array
+
+        2. predicts with booster on encoded features
 
         Parameters
         ----------
-        variants: list or tuple or np.ndarray
-            list of variants to scores
-        givens: dict or None
+        candidates: list or tuple or np.ndarray
+            list of candidates to scores
+        context: dict or None
             context dict needed for encoding
         kwargs: dict
             kwargs
 
         Returns
         -------
         np.ndarray
-            2D numpy array which contains (variant, score) pair in each row
+            1D numpy array with scores
         """
 
-        encoded_variants = \
-            self.encode_variants_single_givens(variants=variants, givens=givens)
-
-        encoded_variants_to_np_method = \
-            fast_encoded_variants_to_np if CYTHON_BACKEND_AVAILABLE \
-            else encoded_variants_to_np
-
-        missings_filled_v = \
-            encoded_variants_to_np_method(
-                encoded_variants=encoded_variants,
-                feature_names=self.model_feature_names)
-
-        if CYTHON_BACKEND_AVAILABLE:
-            missings_filled_v = np.asarray(missings_filled_v)
+        encoded_variants_matrix = \
+            self.encode_candidates_with_context(candidates=candidates, context=context)
 
         scores = \
             self.model.predict(
                 DMatrix(
-                    missings_filled_v, feature_names=self.model_feature_names))\
+                    encoded_variants_matrix, feature_names=self.feature_names))\
             .astype('float64')
 
         return scores
 
-    def fill_missing_features(self, encoded_variants):
-        """
-        Fills missing features in encoded variants and packs them into 2D numpy array
-
-        Parameters
-        ----------
-        encoded_variants: list
-            a list of encoded variants (dicts)
-
-        Returns
-        -------
-        np.ndarray
-            2D numpy array with all features for xgb model
-
-        """
-        encoded_variants_to_np_method = \
-            fast_encoded_variants_to_np if CYTHON_BACKEND_AVAILABLE else encoded_variants_to_np
-
-        features_matrix = encoded_variants_to_np_method(
-            encoded_variants=encoded_variants, feature_names=self.model_feature_names)
-
-        if CYTHON_BACKEND_AVAILABLE:
-            features_matrix = np.asarray(features_matrix)
-
-        return features_matrix
-
     def calculate_predictions(self, features_matrix: np.ndarray):
         """
         Calculates predictions on provided matrix with loaded model
 
         Parameters
         ----------
         features_matrix: np.ndarray
             array to be a source for DMatrix
 
         Returns
         -------
+        np.ndarray
+            an array of double scores
 
         """
         # make sure input is a numpy array
         assert isinstance(features_matrix, np.ndarray)
         # make sure input for predictions is not empty
         assert features_matrix.size > 0
         # make sure it is 2D array
         assert len(features_matrix.shape) == 2
         # make sure all features are present
-        assert len(self.model_feature_names) == features_matrix.shape[1]
-        scores = \
-            self.model.predict(
-                DMatrix(features_matrix, feature_names=self.model_feature_names)) \
-            .astype('float64')
-        return scores
+        assert len(self.feature_names) == features_matrix.shape[1]
+        return self.model.predict(
+                DMatrix(features_matrix, feature_names=self.feature_names)).astype('float64')
 
-    def encode_variants_single_givens(
-            self, variants: list or tuple or np.ndarray, givens: dict or None) -> Iterable:
+    def encode_candidates_with_context(
+            self, candidates: list or tuple or np.ndarray, context: object) -> np.ndarray:
         """
-        Implemented as a XGBChooser helper method
-        Cythonized loop over provided variants and a single givens dict.
-        Returns array of encoded dicts.
+        Encodes provided candidates with a given context into numpy 2D matrix.
+        Implemented as a XGBChooser helper method (will use Cython backend to
+        speed things up if possible)
 
         Parameters
         ----------
-        variants: list or tuple or np.ndarray
+        candidates: list or tuple or np.ndarray
             collection of input variants to be encoded
-        givens: dict or None
+        context: dict or None
             context to be encoded with variants
 
         Returns
         -------
         np.ndarray
-            array of encoded dicts
+            2D array of encoded values
         """
 
-        if not (isinstance(givens, dict) or givens is None or givens is {}):
-            raise TypeError(
-                'Unsupported givens` type: {}'.format(type(givens)))
-
-        if self.imposed_noise is None:
-            noise = np.random.rand()
-        else:
-            noise = self.imposed_noise
-
         if CYTHON_BACKEND_AVAILABLE:
-            if isinstance(variants, list):
-                used_variants = variants
-            elif isinstance(variants, tuple) or isinstance(variants, np.ndarray):
-                used_variants = list(variants)
-            else:
-                raise TypeError(
-                    'Variants are of a wrong type: {}'.format(type(variants)))
-
-            return fast_encode_variants_single_givens(
-                variants=used_variants, givens=givens, noise=noise,
-                variants_encoder=self.feature_encoder.encode_variant,
-                givens_encoder=self.feature_encoder.encode_givens)
+            return \
+                np.asarray(fast_encode_candidates_to_matrix(
+                    candidates=candidates, context=context, feature_encoder=self.feature_encoder, noise=self._get_noise()))
         else:
-            encoded_variants = np.empty(len(variants), dtype=object)
+            return self.encode_candidates_to_matrix(candidates=candidates, context=context, noise=self._get_noise())
 
-            encoded_givens = self.feature_encoder.encode_givens(givens=givens, noise=noise)
+    @staticmethod
+    def get_model_src(model_src: str or Path or bytes) -> str or bytearray:
+        """
+        Based on provided `model_src` this method will return:
 
-            encoded_variants[:] = [
-                self.feature_encoder.encode_variant(
-                    variant=variant, noise=noise, into=deepcopy(encoded_givens))
-                for variant in variants]
+        - a FS string path for input FS path to unzipped booster
 
-            return encoded_variants
+        - Path object for input Path object to unzipped booster
 
-    @staticmethod
-    def get_model_src(model_src: str or bytes) -> str or bytes:
-        """
-        Gets model src from provided input path, url or bytes
+        - unzipped bytesarray for input  FS path / Path object to gzipped booster
+
+        - (unzipped) bytesarray for input URL (if URL leads to gzipped booster
+        it will be unzipped)
+
+
+        Output from this method can in be passed directly to Booster.load_model().
 
         Parameters
         ----------
-        model_src: str or bytes
+        model_src: str or Path or bytes
             pth to model, url or bytes
 
         Returns
         -------
-        str or bytes
+        str or Path or bytearray
             path or downloaded model
 
         """
         raw_model_src = model_src
-        if not isinstance(model_src, Path) and is_path_http_addr(pth_to_model=model_src):
+        if not isinstance(model_src, Path) and is_path_http_addr(path=model_src):
             raw_model_src = get_model_bytes_from_url(model_url=model_src)
 
         unzipped_model_src = check_and_get_unzipped_model(model_src=raw_model_src)
         return unzipped_model_src
 
+    def _get_improveai_major_version(self, model_metadata: dict) -> str or None:
+        """
+        Extracts Improve AI version from model metadata and return it if it is valid / allowed
+
+        Parameters
+        ----------
+        model_metadata: dict
+            a dictionary containing model metadata
+
+        Returns
+        -------
+        str or None
+            major Improve AI version extracted from loaded improve model
+        """
+
+        if model_metadata is None or not isinstance(model_metadata, dict):
+            raise IOError('Model metadata is either None or empty')
+
+        # TODO once we completely shift to 8.X we should disallow None values
+        improveai_major_version = None
+        if self.VERSION_METADATA_KEY in model_metadata.keys():
+            improveai_version = model_metadata[self.VERSION_METADATA_KEY]
+
+            if improveai_version is None or not isinstance(improveai_version, str):
+                raise IOError(f'Improve AI version stored in metadata ({improveai_version}) is either None or not a string')
+            # major version is the first chunk of version string
+            try:
+                improveai_major_version = int(improveai_version.split('.')[0])
+            except:
+                raise IOError(f'Improve AI version stored in metadata ({improveai_version}) is invalid')
+
+            if improveai_major_version != self.IMPROVE_AI_ALLOWED_MAJOR_VERSION:
+                raise IOError(f'Attempting to load model from unsupported Improve AI version: {improveai_major_version}.'
+                              f' Currently supported Improve AI major version is: {self.IMPROVE_AI_ALLOWED_MAJOR_VERSION}')
+        return improveai_major_version
+
+    def _get_model_metadata(self) -> dict:
+        """
+        Gets 'model metadata' from JSON string stored in 'user defined metadata'
+        attribute of Improve AI booster
+
+        Returns
+        -------
+        dict
+            dict with model metadata
+        """
+
+        if self.USER_DEFINED_METADATA_KEY not in self.model.attributes().keys():
+            raise IOError(f'Improve AI booster has no: {self.USER_DEFINED_METADATA_KEY} attribute')
+
+        user_defined_metadata_str = self.model.attr(self.USER_DEFINED_METADATA_KEY)
+        try:
+            user_defined_metadata = json.loads(user_defined_metadata_str)
+        except json.JSONDecodeError:
+            raise IOError('Model metadata is not a valid json')
+
+        if not isinstance(user_defined_metadata, dict):
+            raise IOError(f'Model metadata must be a dict '
+                          f'(current type: {type(user_defined_metadata)})')
+
+        if not user_defined_metadata:
+            raise IOError('Model metadata is either None or empty')
+
+        loaded_metadata_keys = set(user_defined_metadata.keys())
+
+        for required_key in self.REQUIRED_METADATA_KEYS:
+            if required_key not in loaded_metadata_keys:
+                raise IOError(f'Improve AI booster`s metadata has no: {required_key} key')
+
+        return user_defined_metadata
+
     def _get_model_feature_names(self, model_metadata: dict) -> list:
         """
         Gets model feature names from model metadata
 
         Parameters
         ----------
         model_metadata: dict
@@ -644,20 +631,23 @@
         -------
         list
             list of feature names
 
         """
 
         if not model_metadata:
-            raise ValueError('Model metadata empty or None!')
+            raise IOError('Model metadata is either None or empty')
 
-        feature_names = model_metadata.get(self.MODEL_FEATURE_NAMES_KEY, None)
+        feature_names = model_metadata.get(self.FEATURE_NAMES_METADATA_KEY, None)
 
         if not feature_names:
-            raise ValueError('Feature names not in model metadata!')
+            raise IOError('Feature names can`t be None or empty collection')
+
+        if not all(isinstance(fn, str) for fn in feature_names):
+            raise IOError('All feature names must be strings')
 
         return feature_names
 
     def _get_model_seed(self, model_metadata: dict) -> int:
         """
         Gets model seed from model metadata
 
@@ -669,21 +659,24 @@
 
         Returns
         -------
         int
             model seed
 
         """
+
         if not model_metadata:
-            raise ValueError('Model metadata empty or None!')
+            raise IOError('Model metadata is either None or empty')
 
-        model_seed = model_metadata.get(self.MODEL_SEED_KEY, None)
+        model_seed = model_metadata.get(self.MODEL_SEED_METADATA_KEY, None)
 
-        if not model_seed:
-            raise ValueError('Feature names not in model metadata!')
+        if not model_seed or not (isinstance(model_seed, int) and not isinstance(model_seed, bool)):
+            raise IOError(
+                f'Wrong {self.MODEL_SEED_METADATA_KEY}: {model_seed} '
+                f'(type: {type(model_seed)}).')
 
         return model_seed
 
     def _get_model_name(self, model_metadata: dict) -> str:
         """
         Gets model name from model metadata
 
@@ -694,48 +687,47 @@
 
         Returns
         -------
         str
             Improve AI model name
 
         """
+
         if not model_metadata:
-            raise ValueError('Model metadata empty or None!')
+            raise IOError('Model metadata is either None or empty')
 
-        model_name = model_metadata.get(self.MODEL_NAME_KEY, None)
+        model_name = model_metadata.get(self.MODEL_NAME_METADATA_KEY, None)
 
-        if not model_name:
-            raise ValueError('Feature names not in model metadata!')
+        if not model_name or not isinstance(model_name, str):
+            raise IOError(f'Wrong {self.MODEL_NAME_METADATA_KEY}: {model_name} (type: {type(model_name)}).')
 
         return model_name
 
-    def sort(
-            self, variants_w_scores: np.ndarray,
-            scores_col_idx: int = 1, class_cols_idx: int = 2) -> np.ndarray:
+    def _get_string_tables(self, model_metadata: dict):
         """
-        Performs sorting of provided variants with scores array
+        Gets string tables from model metadata
 
         Parameters
         ----------
-        variants_w_scores: np.ndarray
-            array with variant, scores rows
-        scores_col_idx: int
-            the index of column with scores
-        class_cols_idx: int
-            index of the class label in a single row
+        model_metadata: dict
+            a dict containing model metadata
 
         Returns
         -------
-        np.ndarray
-            2D sorted array of rows (variant, score)
+        dict
+            dict of lists with string tables
 
         """
 
-        desc_scores_sorting_col = -1 * variants_w_scores[:, scores_col_idx]
-        class_sorting_col = variants_w_scores[:, class_cols_idx]
-
-        ind = np.lexsort((desc_scores_sorting_col, class_sorting_col))
+        if not model_metadata:
+            raise IOError('Model metadata is either None or empty')
 
-        srtd_variants_w_scores = \
-            variants_w_scores[ind]
+        string_tables = model_metadata.get(self.STRING_TABLES_METADATA_KEY, None)
 
-        return srtd_variants_w_scores
+        # empty dict string tables are allowed -> thye just need ot be present in metadata
+        if string_tables is None or not isinstance(string_tables, dict):
+            raise IOError('String tables can`t None or not of a dict type!')
+
+        # make sure that all values of `string_tables` are
+        if not all(isinstance(string_table, list) for string_table in string_tables.values()):
+            raise IOError('At least one of string tables is not a list')
+        return string_tables
```

### Comparing `improveai-7.2.1/improveai/cythonized_feature_encoding/__init__.py` & `improveai-8.0.0/improveai/cythonized_feature_encoding/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,23 +9,21 @@
     CYTHON_ENCODING_DIR_PATH = os.sep.join(__file__.split(os.sep)[:-1])
     CYTHON_MODULE_DIR = 'cythonized_feature_encoding'
     IMPROVE_DIR = 'improveai'
 
     try:
         pyximport.install(setup_args={'include_dirs': [np.get_include(), CYTHON_ENCODING_DIR_PATH]})
         # this might raise a ValueError if numpy version differs from the one which was used to build improveai
-        import improveai.cythonized_feature_encoding.cythonized_feature_encoding_utils as cfeu
         import improveai.cythonized_feature_encoding.cythonized_feature_encoder as cfe
     except ValueError as verr:
         # if numpy current numpy version is different than the one which was used to build improveai
         # numpy headers might not match in compiled files
         # to address this rebuilding of *.c files is needed
         files_to_delete = \
             [file_name for file_name in os.listdir(CYTHON_ENCODING_DIR_PATH)
              if file_name.endswith('.c') or file_name.endswith('.so')]
         [os.remove(os.sep.join([CYTHON_ENCODING_DIR_PATH, cython_compiled_file]))
          for cython_compiled_file in files_to_delete]
         pyximport.install(setup_args={'include_dirs': [np.get_include(), CYTHON_ENCODING_DIR_PATH]})
-        import improveai.cythonized_feature_encoding.cythonized_feature_encoding_utils as cfeu
         import improveai.cythonized_feature_encoding.cythonized_feature_encoder as cfe
```

### Comparing `improveai-7.2.1/improveai/cythonized_feature_encoding/cythonized_feature_encoder.pyx` & `improveai-8.0.0/improveai/feature_encoder.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,572 +1,504 @@
-#!python3
-#cython: language_level=3
-
-cdef extern from "npy_no_deprecated_api.h": pass
-
-import cython
-from libc.math cimport isnan
 import numpy as np
-cimport numpy as np
-import warnings
 import xxhash
 
 
-cdef object xxhash3 = xxhash.xxh3_64_intdigest
-cdef set JSON_SERIALIZABLE_TYPES = {int, float, str, bool, list, tuple, dict}
+ITEM_FEATURE_KEY = 'item'
+"""
+Feature names prefix for features derived from candidates / items, e.g.:
 
-import improveai.cythonized_feature_encoding.cythonized_feature_encoding_utils as cfeu
-import improveai.feature_encoder as fe
+- item == 1 -> feature name is "item"
 
+- item == [1] -> feature names is "item.0"
 
-encoded_variant_into_np_row = cfeu.encoded_variant_into_np_row
-encode_variants_multiple_givens = cfeu.encode_variants_multiple_givens
-encoded_variants_to_np = cfeu.encoded_variants_to_np
+- item == {"a": 1}} - feature name is "item.a"
+"""
 
+CONTEXT_FEATURE_KEY = 'context'
+"""
+Feature names prefix for features derived from context, e.g.:
 
-@cython.boundscheck(False)
-@cython.wraparound(False)
-cpdef _is_object_json_serializable(object object_):
-    """
-    Checks if input value is JSON serializable
+- context == 1 -> feature name is "context"
 
-    Parameters
-    ----------
-    object_: object
-        object to be checked
+- context == [1] -> feature names is "context.0"
 
-    Returns
-    -------
-    bool
-        True if input is JSON serializable False otherwise
-    """
-    return type(object_) in JSON_SERIALIZABLE_TYPES or object_ is None
+- context == {"a": 1}} - feature name is "context.a"
+"""
+
+FIRST_LEVEL_FEATURES_CHUNKS = {ITEM_FEATURE_KEY, CONTEXT_FEATURE_KEY}
 
+xxh3 = xxhash.xxh3_64_intdigest
 
-@cython.boundscheck(False)
-@cython.wraparound(False)
-cpdef _has_top_level_string_keys(dict checked_dict):
+
+class FeatureEncoder:
+    """
+    Encodes JSON encodable objects into float vectors
     """
-    Check if all top level keys are of a string type. This is a helper function 
-    for encode() and since encode recurs in case of nested dicts only top level 
-    keys need to be checked. Return False on first encountered non-string key
 
-    Parameters
-    ----------
-    checked_dict: dict
-        dict which top level keys will be checked
+    @property
+    def feature_indexes(self) -> dict:
+        """
+        A map between feature names and feature indexes. Created by simple
+        iteration with enumeration over feature names
 
-    Returns
-    -------
-    bool
-        True if all keys are strings otherwise False
+        Returns
+        -------
+        dict
+            a mapping between a string feature names and feature index
 
-    """
-    return all([isinstance(k, str) for k in checked_dict.keys()])
+        """
+        return self._feature_indexes
 
+    @feature_indexes.setter
+    def feature_indexes(self, value: dict):
+        self._feature_indexes = value
 
-@cython.boundscheck(False)
-@cython.wraparound(False)
-cpdef warn_about_array_encoding(object object_):
-    """
-    If object is an array warning will be printed (only once so the encoding speed does not suffer)
+    @property
+    def string_tables(self) -> list:
+        """
+        List of StringTable objects. The order of elements follows constructor's
+        `string_tables` parameter.
 
-    Parameters
-    ----------
-    object_: object
-        encoded object
+        Returns
+        -------
+        list
+            list of StringTables
 
-    Returns
-    -------
-    None
-        None
+        """
+        return self._string_tables
 
-    """
-    # check if variant is a list, tuple or array
-    if not fe.WARNED_ABOUT_ARRAY_ENCODING and \
-            (isinstance(object_, list) or isinstance(object_, tuple) or isinstance(object_, np.ndarray)):
-        warnings.warn('Array encoding may change in the near future')
-        fe.WARNED_ABOUT_ARRAY_ENCODING = True
-
-
-@cython.boundscheck(False)
-@cython.wraparound(False)
-cpdef encode(object object_, unsigned long long seed, double small_noise, dict features):
-    """
-    Encodes a JSON serializable object to  a flat key - value pair(s) structure / dict
-    (sometimes a single `object_` will result in 2 features, e.g. strings, lists, etc...).
-    Rules of encoding go as follows:
-    
-    - None, json null, {}, [], nan, are treated as missing feature_names and ignored.  NaN is technically not allowed in JSON but check anyway.
-    
-    - boolean true and false are encoded as 1.0 and 0.0 respectively.
-    
-    - strings are encoded into an additional one-hot feature.
-    
-    - numbers are encoded as-is with up to about 5 decimal places of precision
-    
-    - a small amount of noise is incorporated to avoid overfitting
-    
-    - feature names are 8 hexadecimal characters
-    
+    @string_tables.setter
+    def string_tables(self, value: list):
+        self._string_tables = value
 
-    Parameters
-    ----------
-    object_: object
-        a JSON serializable object to be encoded to a flat key-value structure
-    seed: int
-        seed for xxhash3 to generate feature name
-    small_noise: float
-        a shrunk noise to be added to value of encoded feature
-    features: dict
-        a flat dict of {<feature name>: <feature value>, ...} pairs
+    def __init__(self, feature_names: list, string_tables: dict, model_seed: int):
+        """
+        Initialize the feature encoder for this model
 
-    Returns
-    -------
-    None
-        None
+        Parameters
+        ----------
+        feature_names: list
+            the list of feature names. Order matters - first feature name should
+            be the first feature in the model
+        string_tables: dict
+            a mapping from feature names to string hash tables
+        model_seed: int
+            model seed to be used during string encoding
 
-    """
+        Raises
+        ----------
+        ValueError if feature names or tables are corrupt
+        """
 
-    assert _is_object_json_serializable(object_=object_)
-    warn_about_array_encoding(object_=object_)
+        self.feature_indexes = {}
 
-    cdef str feature_name = None
-    cdef double previous_object_
+        # index feature names for vectorization
+        for i, feature_name in enumerate(feature_names):
+            self.feature_indexes[feature_name] = i
 
-    if isinstance(object_, (int, float)):  # bool is an instanceof int
-        if isnan(object_):  # nan is treated as missing feature, return
-            return
+        # initialize string encoding tables with a shared empty table
+        self.string_tables = [StringTable([], model_seed)] * len(feature_names)
 
-        feature_name = hash_to_feature_name(seed)
+        try:
+            for feature_name, table in string_tables.items():
+                self.string_tables[self.feature_indexes[feature_name]] = StringTable(table, model_seed)
+        except KeyError as exc:
+            raise ValueError("Bad model metadata") from exc
 
-        previous_object_ = \
-            _get_previous_value(feature_name=feature_name, into=features, small_noise=small_noise)
+    def _check_into(self, into: np.ndarray):
+        """
+        Checks if the provided `into` array is an array and has desired
+        np.float64 dtype
 
-        features[feature_name] = sprinkle(object_ + previous_object_, small_noise)
+        Parameters
+        ----------
+        into: np.ndarray
+            array which will store feature values
 
-        return
+        Raises
+        -------
+        ValueError if into is not a numpy array or not of a float64 dtype
 
-    cdef unsigned long long hashed
-    cdef double previous_hashed
-    cdef str hashed_feature_name
-    cdef double previous_hashed_for_feature_name
+        """
 
-    if isinstance(object_, str):
-        hashed = xxhash3(object_, seed=seed)
+        if into is not None:
+            assert len(self.feature_indexes) == len(into)
 
-        feature_name = hash_to_feature_name(seed)
+        if not isinstance(into, np.ndarray) or into.dtype != np.float64:
+            raise ValueError("into must be a float64 array")
 
-        previous_hashed = \
-            _get_previous_value(feature_name=feature_name, into=features, small_noise=small_noise)
+    def encode_item(self, item: object, into: np.ndarray, noise_shift: float = 0.0, noise_scale: float = 1.0):
+        """
+        Encodes provided item to `input` numpy array
 
-        features[feature_name] = \
-            sprinkle(<double>(<long long>(((hashed & 0xffff0000) >> 16) - 0x8000)) + previous_hashed, small_noise)
+        Parameters
+        ----------
+        item: object
+            JSON encodable python object
+        into: np.ndarray
+            array storing results of encoding
+        noise_shift: float
+            value to be added to values of features
+        noise_scale: float
+            multiplier used to scale shifted feature values
 
-        hashed_feature_name = hash_to_feature_name(hashed)
+        """
+        self._encode(item, path=ITEM_FEATURE_KEY, into=into, noise_shift=noise_shift, noise_scale=noise_scale)
 
-        previous_hashed_for_feature_name = \
-            _get_previous_value(feature_name=hashed_feature_name, into=features, small_noise=small_noise)
+    def encode_context(self, context: object, into: np.ndarray, noise_shift: float = 0.0, noise_scale: float = 1.0):
+        """
+        Encodes provided context to `input` numpy array
 
-        features[hashed_feature_name] = \
-            sprinkle(<double>(<long long>((hashed & 0xffff) - 0x8000)) + previous_hashed_for_feature_name, small_noise)
+        Parameters
+        ----------
+        context: object
+            JSON encodable python object
+        into: np.ndarray
+            array storing results of encoding
+        noise_shift: float
+            value to be added to values of features
+        noise_scale: float
+            multiplier used to scale shifted feature values
 
-        return
+        """
+        self._encode(context, path=CONTEXT_FEATURE_KEY, into=into, noise_shift=noise_shift, noise_scale=noise_scale)
 
-    if isinstance(object_, dict):
-        assert _has_top_level_string_keys(object_)
-        for key, value in object_.items():
-            encode(value, xxhash3(key, seed=seed), small_noise, features)
-        return
+    def encode_feature_vector(
+            self, item: object, context: object, into: np.ndarray, noise: float = 0.0):
+        """
+        Fully encodes provided variant and context into a np.ndarray provided as
+        `into` parameter. `into` must not be None
 
-    if isinstance(object_, (list, tuple)):
-        for index, item in enumerate(object_):
-            encode(item, xxhash3(index.to_bytes(8, byteorder='big'), seed=seed), small_noise, features)
+        Parameters
+        ----------
+        item: object
+            a JSON encodable item to be encoded
+        context: object
+            a JSON encodable context to be encoded
+        into: np.ndarray
+            an array into which feature values will be added
+        noise: float
+            value in [0, 1) which will be combined with the feature value
 
-        return
+        """
 
-@cython.boundscheck(False)
-@cython.wraparound(False)
-cpdef double _get_previous_value(str feature_name, dict into, double small_noise):
-    """
-    Gets previous, 'unsprinkled' value of <feature_name> feature
-    from <features> dict
+        noise_shift, noise_scale = get_noise_shift_scale(noise)
 
-    Parameters
-    ----------
-    feature_name: str
-        name of a feature which previous value is desired
-    into: dict
-        dict containing current results of encoding
-    small_noise: float
-        small noise used to sprinkle
+        if item is not None:
+            self.encode_item(item, into, noise_shift, noise_scale)
 
-    Returns
-    -------
-    float
-        'unsprinkled' value of desired feature
+        if context is not None:
+            self.encode_context(context, into, noise_shift, noise_scale)
 
-    """
+        # for 10k calls this takes only 4 ms
+        # if both item and context are None into will not be checked until now.
+        if item is None and context is None:
+            self._check_into(into=into)
 
-    cdef double  previous_sprinkled_object_
+    def _encode(self, obj: object, path: str, into: np.ndarray, noise_shift: float = 0.0, noise_scale: float = 1.0):
+        """
+        Encodes a JSON serializable object to a float vector
+        Rules of encoding go as follows:
 
-    if into.get(feature_name, None) is None:
-        return 0.0
-    else:
-        previous_sprinkled_object_ = into.get(feature_name, None)
-        return reverse_sprinkle(previous_sprinkled_object_, small_noise)
+        - None, json null, {}, [], and nan are treated as missing features and ignored.
 
+        - numbers and booleans are encoded as-is.
 
-@cython.boundscheck(False)
-@cython.wraparound(False)
-cpdef str hash_to_feature_name(unsigned long long hash_):
-    """
-    Converts a hash to string which will become a feature name
+        - strings are encoded using a lookup table
 
-    Parameters
-    ----------
-    hash_: int
-        an integer output from xxhash3
+        Parameters
+        ----------
+        obj: object
+            a JSON serializable object to be encoded to a flat key-value structure
+        path: str
+            the JSON-normalized path to the current object
+        into: np.ndarray
+            an array into which feature values will be encoded
+        noise_shift: float
+            small bias added to the feature value
+        noise_scale: float
+            small multiplier of the feature value
 
-    Returns
-    -------
-    str
-        a string representation of a hex feature name created from int
+        """
+        if path in FIRST_LEVEL_FEATURES_CHUNKS:
+            self._check_into(into)
 
-    """
-    return '%0*x' % (8, (hash_ >> 32))
+        # TODO do we want to check if `obj` is JSON serializable?
+        if isinstance(obj, (int, float)):  # bool is an instanceof int
+            # TODO - do we want to differentiate between np.nan and None in python?
+            if np.isnan(obj):  # nan is treated as missing feature, return
+                return
 
+            feature_index = self.feature_indexes.get(path)
+            if feature_index is None:
+                return
 
-@cython.boundscheck(False)
-@cython.wraparound(False)
-cpdef double shrink(double noise):
-    """
-    Shrinks noise value by a hardcoded factor 2 ** -17
+            into[feature_index] = sprinkle(obj, noise_shift, noise_scale)
 
-    Parameters
-    ----------
-    noise: float
-        value within 0 - 1 range which will be 'shrunk' and added to feature value
+        elif isinstance(obj, str):
+            feature_index = self.feature_indexes.get(path)
+            if feature_index is None:
+                return
 
+            string_table = self.string_tables[feature_index]
 
-    Returns
-    -------
-    float
-        a shrunk noise
+            into[feature_index] = sprinkle(string_table.encode(obj), noise_shift, noise_scale)
 
-    """
-    # return noise * pow(2, -17)
-    # TODO after pypi deploy make sure this is used in the trainer
-    return noise * np.float_power(2, -17)
+        elif isinstance(obj, dict):
+            for key, value in obj.items():
+                self._encode(obj=value, path=path + '.' + key, into=into, noise_shift=noise_shift, noise_scale=noise_scale)
 
+        elif isinstance(obj, (list, tuple)):
+            for index, item in enumerate(obj):
+                self._encode(obj=item, path=path + '.' + str(index), into=into, noise_shift=noise_shift, noise_scale=noise_scale)
+
+        elif obj is None:
+            pass
+
+        else:
+            raise ValueError(f'{obj} not JSON encodable. Must be string, int, float, bool, list, tuple, dict, or None')
 
-@cython.boundscheck(False)
-@cython.wraparound(False)
-cpdef double sprinkle(double x, double small_noise):
+
+def get_noise_shift_scale(noise: float) -> tuple:
     """
-    Slightly modified input valuse using `small_noise`: (x + small_noise) * (1 + small_noise)
+    Returns noise shift (small value added to feature value) and noise scale
+    (value by which shifted feature value is multiplied)
 
     Parameters
     ----------
-    x: float
-        a number to be 'modified'
-    small_noise: float
-        a small number with which `x` will be modified
+    noise: float
+        value in [0, 1) which will be combined with the feature value
+
 
     Returns
     -------
-    float
-        x modified with `small_noise`
+    tuple
+        tuple of floats: (noise_shift, noise_scale)
 
     """
-    return (x + small_noise) * (1 + small_noise)
+    assert noise >= 0.0 and noise < 1.0
+    # x + noise * 2 ** -142 will round to x for most values of x. Used to create
+    # distinct values when x is 0.0 since x * scale would be zero
+    return (noise * 2 ** -142, 1 + noise * 2 ** -17)
 
 
-@cython.boundscheck(False)
-@cython.wraparound(False)
-cpdef double reverse_sprinkle(double sprinkled_x, double small_noise):
+def sprinkle(x: float, noise_shift: float, noise_scale: float) -> float:
     """
-    Retrieves true value from sprinkled one
+    Adds noise shift and scales shifted value
 
     Parameters
     ----------
-    sprinkled_x: float
-        sprinkled value
-    small_noise: float
-        noise used to calculate sprinkled_Xx
+    x: float
+        value to be sprinkled
+    noise_shift: float
+        small bias added to the feature value
+    noise_scale: float
+        small multiplier of the shifted feature value
 
     Returns
     -------
     float
-        true value of x which was used to calculate sprinkled_x
+        sprinkled value
 
     """
-    return sprinkled_x / (1 + small_noise) - small_noise
+    # x + noise_offset will round to x for most values of x
+    # allows different values when x == 0.0
+    return (x + noise_shift) * noise_scale
 
 
-cdef class FeatureEncoder:
+class StringTable:
     """
-    This class serves as a preprocessor which allows to
-    convert event data in form of a JSON line (variants, givens and
-    extra features) to the tabular format expected on input by XGBoost.
-
-    Short summary of methods:
-     - encode_givens() -> encodes givens / variant metadata to dict of
-       feature name -> float pairs
-
-     - encode_variant() -> encodes variant to dict of feature name -> float pairs
-
-     - encode_feature_vector() -> encodes provided variant and givens;
-       appends extra features to the encoded variant dict;
-       converts encoded variant to numpy array using provided feature names
-
-     - add_noise() -> sprinkles each value of the input dict with small noise
-
-     - encode_to_np_matrix()  -> encodes collection of variants with collection
-       of givens and extra features to the numpy 2D array / matrix. If desired
-       uses cython backed (works much faster)
-
-     - add_extra_features() - helper method for adding extra features to already
-       encoded variants
-
+    A class responsible for target encoding of strings for a given feature
     """
 
-    cdef unsigned long long variant_seed
-    cdef unsigned long long value_seed
-    cdef unsigned long long givens_seed
-
-    def __init__(self, long long model_seed):
+    @property
+    def model_seed(self) -> int:
         """
-        Init with params
+        32-bit random integer used to hash strings with xxhash
+
+        Returns
+        -------
+        int
+            model seed
 
-        Parameters
-        ----------
-        model_seed: int
-            model seed to be used during feature encoding
         """
-        if (model_seed < 0):
-            raise TypeError(
-                "xxhash3_64 takes an unsigned 64-bit integer as seed. "
-                "Seed must be greater than or equal to 0.")
+        return self._model_seed
 
-        # memoize commonly used seeds
-        self.variant_seed = xxhash3("variant", seed=model_seed)
-        self.value_seed = xxhash3("$value", seed=self.variant_seed)
-        self.givens_seed = xxhash3("givens", seed=model_seed)
+    @model_seed.setter
+    def model_seed(self, value: int):
+        self._model_seed = value
 
-    cdef void _check_noise_value(self, double noise) except *:
+    @property
+    def mask(self) -> int:
         """
-        Check whether noise value is valid; Raises if `noise` is invalid
-
-        Parameters
-        ----------
-        noise: float
-            checked value of no ise
+        At most 64 bit int representation of a string hash mask e.g., 000..00111
 
         Returns
         -------
-        None
-            None
+        int
+            mask used to 'decrease' hashed string value
+
         """
+        return self._mask
 
-        if noise > 1.0 or noise < 0.0:
-            raise ValueError(
-                'Provided `noise` is out of allowed bounds <0.0, 1.0>')
+    @mask.setter
+    def mask(self, value: int):
+        self._mask = value
 
-    cpdef dict encode_givens(self, dict givens, double noise=0.0, dict into=None):
+    @property
+    def miss_width(self) -> float:
         """
-        Encodes provided givens of arbitrary complexity to a flat feature dict;
-        Givens must be JSON encodable
-
-        Parameters
-        ----------
-        givens: dict or None
-            givens to be encoded
-        noise: float
-            value within 0 - 1 range which will be 'shrunk' and added to feature value
-        into: dict
-            a dict into which new features will be inserted; Can be None
+        Float value representing snap / width of the 'miss interval' - numeric
+        interval into which all missing / unknown values are encoded. It is
+        0-centered.
 
         Returns
         -------
-        dict
-            A dict with results of givens encoding
+        float
+            miss width value
 
         """
+        return self._miss_width
 
-        self._check_noise_value(noise=noise)
+    @miss_width.setter
+    def miss_width(self, value: float):
+        self._miss_width = value
 
-        if givens is not None and not isinstance(givens, dict):
-            raise TypeError(
-                "Only dict type is supported for context encoding. {} type was "
-                "provided.".format(type(givens)))
+    @property
+    def value_table(self) -> dict:
+        """
+        A mapping from masked string hash to target encoding's target value for a given feature
 
-        if into is None:
-            into = {}
+        Returns
+        -------
+        dict
+            a dict with target value encoding
 
-        encode(givens, self.givens_seed, shrink(noise), into)
+        """
+        return self._value_table
 
-        return into
+    @value_table.setter
+    def value_table(self, value: dict):
+        self._value_table = value
 
-    cpdef dict encode_variant(self, object variant, double noise=0.0, dict into=None):
+    def __init__(self, string_table, model_seed):
         """
-        Encodes provided variant of arbitrary complexity to a flat feature dict;
-        Variant must be JSON encodable
+        Init StringTable with params
 
         Parameters
         ----------
-        variant: object
-            variant to be encoded
-        noise: float
-            value within 0 - 1 range which will be 'shrunk' and added to feature value
-        into: dict
-            a dict into which new features will be inserted; Can be None
-
-        Returns
-        -------
-        dict
-            A dict with results of variant encoding
+        string_table: list
+            a list of masked hashed strings for each string feature
+        model_seed: int
+            model seed value
 
         """
 
-        self._check_noise_value(noise=noise)
-
-        if into is None:
-            into = {}
+        if model_seed < 0:
+            raise ValueError(
+                "xxhash3_64 takes an unsigned 64-bit integer as seed. "
+                "Seed must be greater than or equal to 0.")
 
-        small_noise = shrink(noise)
+        self.model_seed = model_seed
+        self.mask = get_mask(string_table)
+        max_position = len(string_table) - 1
 
-        if isinstance(variant, dict):
-            encode(variant, self.variant_seed, small_noise, into)
-        else:
-            encode(variant, self.value_seed, small_noise, into)
+        # empty and single entry tables will have a miss_width of 1 or range [-0.5, 0.5]
+        # 2 / max_position keeps miss values from overlapping with nonzero table values
+        self.miss_width = 1 if max_position < 1 else 2 / max_position
 
-        return into
+        self.value_table = {}
 
+        for index, string_hash in enumerate(reversed(string_table)):
+            # a single entry gets a value of 1.0
+            self.value_table[string_hash] = 1.0 if max_position == 0 else scale(index / max_position)
 
-    cpdef encode_feature_vector(
-            self, object variant = None, dict givens = None,
-            dict extra_features = None, list feature_names = None,
-            double noise = 0.0, np.ndarray into = None):
+    def encode(self, string: str) -> float:
         """
-        Fully encodes provided variant and givens into a np.ndarray provided as `into` parameter.
-        `into` must not be None
+        Encode input string to a target value
 
         Parameters
         ----------
-        variant: object
-            a JSON encodable object to be encoded to flat features' dict
-        givens: dict
-            a dict with givens to be enncoded to flat features' dict (all entries must be JSON encodable)
-        extra_features: dict
-            features to be added to encoded variant with givens
-        feature_names: list or np.ndarray
-            list of model's feature names (only overlapping features will be selected for resulting vector)
-        noise: float
-            value within 0 - 1 range which will be 'shrunk' and added to feature value
-        into: np.ndarray
-            an array into which feature values will be added / inserted
+        string: str
+            string to be encoded
 
         Returns
         -------
-        None
-            None
+        float
+            encoded value
 
         """
+        string_hash = xxh3(string, seed=self.model_seed)
+        value = self.value_table.get(string_hash & self.mask)
+        if value is not None:
+            return value
 
-        if into is None:
-            raise ValueError('`into` can`t be None')
-
-        cdef dict encoded_givens = {}
-        # encode givens
-        encoded_givens = \
-            self.encode_givens(givens=givens, noise=noise, into=dict())
-
-        cdef dict encoded_variant = {}
-        # encoded variant and givens
-        encoded_variant = \
-            self.encode_variant(
-                variant=variant, noise=noise, into=encoded_givens)
+        return self.encode_miss(string_hash)
 
-        if extra_features:
-            if not isinstance(extra_features, dict):
-                raise TypeError(
-                    'Provided `extra_features` is not a dict but: {}'
-                    .format(extra_features))
-
-            encoded_variant.update(extra_features)
-
-        # n + nan = nan so you'll have to check for nan values on into
-        encoded_variant_into_np_row(
-            encoded_variant=encoded_variant, feature_names=feature_names,
-            into=into)
-
-    cpdef double [:, :] encode_to_np_matrix(
-            self, list variants, list multiple_givens,
-            list multiple_extra_features, list feature_names, double noise):
+    def encode_miss(self, string_hash) -> float:
         """
-        Provided list of variants and corresponding lists of givens and extra
-        features encodes variants completely and converts to numpy array
+        Encodes string hash as a miss
 
         Parameters
         ----------
-        variants: list
-            list of variants to be encoded
-        multiple_givens: list
-            list of givens - givens[i] will be used to encode variants[i]
-        multiple_extra_features: list
-            list of extra_features - multiple_extra_features[i] will be used
-            to encode variants[i]
-        feature_names: list
-            names of features expected by the model
-        noise: float
-            noise to be used when encoding data
+        string_hash: int
+            string hash to be encoded as a miss
 
         Returns
         -------
-        np.ndarray
-            2D numpy array of encoded variants
+        float
+            encoded miss value
 
         """
+        # hash to float in range [-miss_width/2, miss_width/2]
+        # 32 bit mask for JS portability
+        return scale((string_hash & 0xFFFFFFFF) * 2 ** -32, self.miss_width)
 
-        encoded_variants = encode_variants_multiple_givens(
-            variants=variants, multiple_givens=multiple_givens,
-            multiple_extra_features=multiple_extra_features, noise=noise,
-            variants_encoder=self.encode_variant,
-            givens_encoder=self.encode_givens)
-        encoded_variants_array = encoded_variants_to_np(
-            encoded_variants=encoded_variants, feature_names=feature_names)
 
-        return encoded_variants_array
+def scale(val: float, width: float = 2) -> float:
+    """
+    Scales input miss value to [-width/2, width/2].
+    Assumes input is within [0, 1] range.
 
-    cpdef void add_extra_features(self, list encoded_variants, list extra_features):
-        """
-        Once variants are encoded this method can be used to quickly append
-        extra features
+    Parameters
+    ----------
+    val: float
+        miss value to be scaled
+    width: float
+        miss range width
 
-        Parameters
-        ----------
-        encoded_variants: list
-            collection of encoded variants to be updated with extra features
-        extra_features: list
-            payload to be appended to encoded variants
+    Returns
+    -------
+    float
+        scaled miss value
 
-        Returns
-        -------
-        None
-            None
+    """
+    assert width >= 0
+    # map value in [0, 1] to [-width/2, width/2]
+    # return val * width - 0.5 * width
+    return width * (val - 0.5)
 
-        """
 
-        if extra_features is None:
-            return
+def get_mask(string_table: list) -> int:
+    """
+    Returns an integer representation of a binary mask for a given string table
+
+    Parameters
+    ----------
+    string_table: list
+        list of hash string values for a given feature
+
+    Returns
+    -------
+    int
+        number of bytes needed to represent string hashed in the table
 
-        if not isinstance(encoded_variants, list):
-            raise TypeError('`encoded_variants` should be of a list type')
+    """
+    if len(string_table) == 0:
+        return 0
 
-        if not isinstance(extra_features, list):
-            raise TypeError('`extra_features` should be of a list type')
+    max_value = max(string_table)
+    if max_value == 0:
+        return 0
 
-        [encoded_variant.update(single_extra_features)
-         if single_extra_features is not None else encoded_variant
-         for encoded_variant, single_extra_features in
-         zip(encoded_variants, extra_features)]
+    # find the most significant bit in the table and create a mask
+    return (1 << int(np.log2(max_value) + 1)) - 1
```

### Comparing `improveai-7.2.1/improveai/settings.py` & `improveai-8.0.0/improveai/settings.py`

 * *Files identical despite different names*

### Comparing `improveai-7.2.1/improveai/utils/gzip_tools.py` & `improveai-8.0.0/improveai/utils/gzip_tools.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,98 +1,106 @@
 from io import BytesIO
 import gzip
 import os
 from pathlib import Path
 from typing import Union
 
 
-def is_gz_bytes(chkd_bytes: bytes) -> bool:
+def is_gz_bytes(checked_bytes: bytes) -> bool:
     """
-    Checks if provided bytes is a gz zipped file stream. If so returns True
+    Checks if provided bytes is a gzipped file stream. If so returns True.
 
     Parameters
     ----------
-    chkd_bytes: bytes
+    checked_bytes: bytes
         bytes to check for being gz zipped file
 
     Returns
     -------
     bool
         flag indicating if provided bytes is a gz compressed bytes
 
     """
 
-    if not isinstance(chkd_bytes, bytes):
+    if not isinstance(checked_bytes, bytes):
         return False
 
-    with gzip.GzipFile(fileobj=BytesIO(chkd_bytes)) as f:
+    with gzip.GzipFile(fileobj=BytesIO(checked_bytes)) as f:
         try:
             f.read(1)
             return True
         except Exception as exc:
             return False
 
 
-def get_unzip_gz(to_be_unzpd_bytes: bytes) -> bytes:
+def get_unzipped_gz(to_be_unzipped_bytes: bytes) -> bytes:
     """
-    Unzips provided input bytes
+    Unzips provided input bytes.
 
     Parameters
     ----------
-    to_be_unzpd_bytes: bytes
+    to_be_unzipped_bytes: bytes
         bytes to be unzipped
 
     Returns
     -------
     bytes
         unzipped bytes
 
     """
 
-    if not isinstance(to_be_unzpd_bytes, bytes):
+    if not isinstance(to_be_unzipped_bytes, bytes):
         raise TypeError('`unzpd_bytes` param should be of bytes type')
 
-    unzipped_buffer = BytesIO(to_be_unzpd_bytes)
+    unzipped_buffer = BytesIO(to_be_unzipped_bytes)
     unzipped_buffer.seek(0)
     res = gzip.decompress(unzipped_buffer.read())
     return res
 
 
-def check_and_get_unzipped_model(model_src: Union[str, bytes]) -> Union[str, bytes, Path]:
+def check_and_get_unzipped_model(model_src: Union[str, bytes, Path]) -> Union[str, bytes, Path]:
     """
-    Checks if provided model is a compressed one and unzips it if so.
+    Checks if provided model is a gzipped one and unzips it if so.
 
     Parameters
     ----------
     model_src: Union[str, bytes]
         model source; cna be bytes or string
 
     Returns
     -------
     Union[str, bytes]
         either decompressed bytes or path to model file
 
     """
 
     if isinstance(model_src, bytes):
-        if is_gz_bytes(chkd_bytes=model_src):
-            return get_unzip_gz(to_be_unzpd_bytes=model_src)
+        if is_gz_bytes(checked_bytes=model_src):
+            return get_unzipped_gz(to_be_unzipped_bytes=model_src)
         else:
             return model_src
     elif isinstance(model_src, str) or isinstance(model_src, Path):
+        if str(model_src).startswith('~'):
+            # append the absolute prefix to the input path
+            abs_model_src = os.path.expanduser(model_src)
+            if isinstance(model_src, Path):
+                # if model_src was of a Path type then we need to convert it back
+                abs_model_src = Path(abs_model_src)
+            # update model_src value
+            model_src = abs_model_src
+            print(f'Model src: {model_src}')
         if not os.path.isfile(model_src):
-            raise ValueError(
+            raise FileNotFoundError(
                 'This is not a proper path: {} and reading model from '
                 'string is not supported'.format(model_src))
 
         try:
             with open(model_src, 'rb') as chkd_bytes:
                 read_chkd_bytes = chkd_bytes.read()
-                if is_gz_bytes(chkd_bytes=read_chkd_bytes):
-                    # print('Returning unzipped file')
+                if is_gz_bytes(checked_bytes=read_chkd_bytes):
                     return gzip.decompress(read_chkd_bytes)
         except Exception as exc:
             print(
                 'When checking file: {} the following error occurred'
                 .format(model_src, exc))
         return model_src
     else:
```

### Comparing `improveai-7.2.1/improveai/utils/url_tools.py` & `improveai-8.0.0/improveai/utils/url_tools.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 import requests as rq
 from urllib.parse import urlparse
 
 
-def is_path_http_addr(pth_to_model: str) -> bool:
+def is_path_http_addr(path: str) -> bool:
     """
-    Checks if provided string is a http address
+    Checks if provided string is a http address.
 
     Parameters
     ----------
-    pth_to_model
+    path: str or Path
+        is this path a URL?
 
     Returns
     -------
+    bool
+        True if path is a URL otherwise False
 
     """
     try:
-        res = urlparse(pth_to_model)
+        res = urlparse(path)
         return all([res.scheme, res.netloc])
     except ValueError:
         return False
 
 
 def get_model_bytes_from_url(model_url: str) -> bytes:
     """
-    Gets model from provided URL
+    Gets model from provided URL.
 
     Parameters
     ----------
     model_url: str
         url to get the model from
 
     Returns
```

### Comparing `improveai-7.2.1/improveai.egg-info/SOURCES.txt` & `improveai-8.0.0/improveai.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -2,31 +2,26 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 improveai/__init__.py
 improveai/chooser.py
-improveai/decision.py
-improveai/decision_context.py
-improveai/decision_model.py
-improveai/decision_tracker.py
 improveai/feature_encoder.py
-improveai/givens_provider.py
-improveai/improve_model_cli.py
+improveai/ranker.py
+improveai/reward_tracker.py
+improveai/scorer.py
 improveai/settings.py
 improveai.egg-info/PKG-INFO
 improveai.egg-info/SOURCES.txt
 improveai.egg-info/dependency_links.txt
 improveai.egg-info/not-zip-safe
 improveai.egg-info/requires.txt
 improveai.egg-info/top_level.txt
 improveai/cythonized_feature_encoding/__init__.py
 improveai/cythonized_feature_encoding/__init__.pyx
 improveai/cythonized_feature_encoding/cythonized_feature_encoder.pyx
-improveai/cythonized_feature_encoding/cythonized_feature_encoding_utils.pyx
 improveai/cythonized_feature_encoding/npy_no_deprecated_api.h
 improveai/utils/__init__.py
-improveai/utils/choosers_feature_encoding_tools.py
 improveai/utils/general_purpose_tools.py
 improveai/utils/gzip_tools.py
 improveai/utils/url_tools.py
```

### Comparing `improveai-7.2.1/setup.cfg` & `improveai-8.0.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = improveai
-version = 7.2.1
+version = 8.0.0
 description = Improve AI: Build self-improving apps that optimize their own variables and data structures.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Improve AI
 author_email = support@improve.ai
 url = https://improve.ai/
 download_urls = https://github.com/improve-ai/python-sdk
```

