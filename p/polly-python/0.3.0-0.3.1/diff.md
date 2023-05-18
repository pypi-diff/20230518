# Comparing `tmp/polly-python-0.3.0.tar.gz` & `tmp/polly-python-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polly-python-0.3.0.tar", last modified: Tue Apr 25 04:43:47 2023, max compression
+gzip compressed data, was "polly-python-0.3.1.tar", last modified: Thu May 18 06:31:08 2023, max compression
```

## Comparing `polly-python-0.3.0.tar` & `polly-python-0.3.1.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:43:47.389971 polly-python-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-04-25 04:42:36.000000 polly-python-0.3.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-25 04:42:36.000000 polly-python-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-25 04:43:47.389971 polly-python-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-25 04:42:36.000000 polly-python-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:43:47.389971 polly-python-0.3.0/polly/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-25 04:42:36.000000 polly-python-0.3.0/polly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-04-25 04:42:36.000000 polly-python-0.3.0/polly/application_error_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-25 04:42:36.000000 polly-python-0.3.0/polly/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    16367 2023-04-25 04:42:36.000000 polly-python-0.3.0/polly/bridge_cohort.py
--rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-04-25 04:42:36.000000 polly-python-0.3.0/polly/cohort.py
--rw-r--r--   0 runner    (1001) docker     (123)    14837 2023-04-25 04:42:36.000000 polly-python-0.3.0/polly/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    31214 2023-04-25 04:42:36.000000 polly-python-0.3.0/polly/core_cohort.py
--rw-r--r--   0 runner    (1001) docker     (123)    20886 2023-04-25 04:42:36.000000 polly-python-0.3.0/polly/curation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10896 2023-04-25 04:42:36.000000 polly-python-0.3.0/polly/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10311 2023-04-25 04:42:36.000000 polly-python-0.3.0/polly/help.py
--rw-r--r--   0 runner    (1001) docker     (123)    33624 2023-04-25 04:42:36.000000 polly-python-0.3.0/polly/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-04-25 04:42:36.000000 polly-python-0.3.0/polly/http_response_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-25 04:42:36.000000 polly-python-0.3.0/polly/index_schema_level_conversion_const.py
--rw-r--r--   0 runner    (1001) docker     (123)    24441 2023-04-25 04:42:36.000000 polly-python-0.3.0/polly/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)   192111 2023-04-25 04:42:36.000000 polly-python-0.3.0/polly/omixatlas.py
--rw-r--r--   0 runner    (1001) docker     (123)    64166 2023-04-25 04:42:36.000000 polly-python-0.3.0/polly/omixatlas_hlpr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-04-25 04:42:36.000000 polly-python-0.3.0/polly/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-25 04:42:36.000000 polly-python-0.3.0/polly/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-04-25 04:42:36.000000 polly-python-0.3.0/polly/tracking.py
--rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-04-25 04:42:36.000000 polly-python-0.3.0/polly/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-04-25 04:42:36.000000 polly-python-0.3.0/polly/validation_hlpr.py
--rw-r--r--   0 runner    (1001) docker     (123)    13003 2023-04-25 04:42:36.000000 polly-python-0.3.0/polly/workspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:43:47.389971 polly-python-0.3.0/polly_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-25 04:43:47.000000 polly-python-0.3.0/polly_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-25 04:43:47.000000 polly-python-0.3.0/polly_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 04:43:47.000000 polly-python-0.3.0/polly_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-25 04:43:47.000000 polly-python-0.3.0/polly_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-25 04:43:47.000000 polly-python-0.3.0/polly_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-25 04:42:36.000000 polly-python-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-25 04:43:47.389971 polly-python-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 04:42:36.000000 polly-python-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:43:47.389971 polly-python-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-04-25 04:42:36.000000 polly-python-0.3.0/tests/test_cohort.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-25 04:42:36.000000 polly-python-0.3.0/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-25 04:42:36.000000 polly-python-0.3.0/tests/test_curation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-25 04:42:36.000000 polly-python-0.3.0/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    83961 2023-04-25 04:42:36.000000 polly-python-0.3.0/tests/test_omixatlas.py
--rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-04-25 04:42:36.000000 polly-python-0.3.0/tests/test_schema_ux.py
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-04-25 04:42:36.000000 polly-python-0.3.0/tests/test_workspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:31:08.262608 polly-python-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-05-18 06:29:34.000000 polly-python-0.3.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-18 06:29:34.000000 polly-python-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-18 06:31:08.262608 polly-python-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-18 06:29:34.000000 polly-python-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:31:08.258608 polly-python-0.3.1/polly/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/application_error_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16367 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/bridge_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/cohort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15398 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31214 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/core_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20886 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/curation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10896 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10311 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34051 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/http_response_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/index_schema_level_conversion_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24441 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   193661 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/omixatlas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67169 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/omixatlas_hlpr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12725 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/validation_hlpr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13003 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/workspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:31:08.262608 polly-python-0.3.1/polly_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-18 06:31:08.000000 polly-python-0.3.1/polly_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-18 06:31:08.000000 polly-python-0.3.1/polly_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 06:31:08.000000 polly-python-0.3.1/polly_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-18 06:31:08.000000 polly-python-0.3.1/polly_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 06:31:08.000000 polly-python-0.3.1/polly_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-18 06:29:34.000000 polly-python-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-18 06:31:08.266608 polly-python-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 06:29:34.000000 polly-python-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:31:08.262608 polly-python-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-05-18 06:29:34.000000 polly-python-0.3.1/tests/test_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-18 06:29:34.000000 polly-python-0.3.1/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-18 06:29:34.000000 polly-python-0.3.1/tests/test_curation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-18 06:29:34.000000 polly-python-0.3.1/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90818 2023-05-18 06:29:34.000000 polly-python-0.3.1/tests/test_omixatlas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-05-18 06:29:34.000000 polly-python-0.3.1/tests/test_schema_ux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-05-18 06:29:34.000000 polly-python-0.3.1/tests/test_workspaces.py
```

### Comparing `polly-python-0.3.0/LICENSE.md` & `polly-python-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.0/PKG-INFO` & `polly-python-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polly-python
-Version: 0.3.0
+Version: 0.3.1
 Summary: Polly SDK
 Home-page: https://github.com/ElucidataInc/polly-python
 Project-URL: Documentation, https://docs.elucidata.io
 Project-URL: Tutorial Notebooks, https://github.com/ElucidataInc/polly-python
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: testing
```

### Comparing `polly-python-0.3.0/README.md` & `polly-python-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.0/polly/application_error_info.py` & `polly-python-0.3.1/polly/application_error_info.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.0/polly/auth.py` & `polly-python-0.3.1/polly/auth.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.0/polly/bridge_cohort.py` & `polly-python-0.3.1/polly/bridge_cohort.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.0/polly/cohort.py` & `polly-python-0.3.1/polly/cohort.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.0/polly/constants.py` & `polly-python-0.3.1/polly/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,16 @@
                     },
                 },
                 {"name": "tcga", "header_mapping": {}},
             ],
         }
     ]
 }
+COHORT_SUPPORTED_DATATYPES = ["Raw Counts Transcriptomics"]
+COHORT_SUPPORTED_DATASOURCES = ["GEO"]
 
 # validation flow files url github
 VALIDATION_FLOW_FILES_URL = (
     "https://raw.githubusercontent.com/ElucidataInc/PublicAssets/master/"
     + "internal-user/validation_full_flow_files"
 )
 
@@ -114,14 +116,18 @@
 
 COMBINED_METADATA_FILE_NAME = "combined_metadata.json"
 
 FILES_PATH_FORMAT = {"metadata": "<metadata_path>", "data": "<data_path>"}
 
 INGESTION_FILES_PATH_DIR_NAMES = ["metadata", "data"]
 
+SCHEMA_CONFIG_KEY_NAMES = ["source", "datatype"]
+
+SCHEMA_CONFIG_FORMAT = {"source": "<source_name", "datatype": "<datatype_name>"}
+
 FORMATTED_METADATA = {"id": "", "type": "", "attributes": {}}
 
 FILE_FORMAT_CONSTANTS_URL = (
     "https://elucidatainc.github.io/PublicAssets/file_format_constants.txt"
 )
 
 VALIDATION_STATUS_FILE_NAME = "validation_status.txt"
@@ -242,14 +248,22 @@
 
 SCHEMA_VERDICT_DICT = {
     "schema_update": SCHEMA_UPDATE_SUCCESS,
     "reingestion": SCHEMA_REINGEST_SUCCESS,
     "no_change": SCHEMA_NO_CHANGE_SUCCESS,
 }
 
+VALIDATION_NOT_EXECUTED = (
+    "Validation not executed on any of the metadata files.  "
+    + "Possible reasons to help you troubleshoot :-"
+    + "\n"
+    + "All the metadata file passed may have `validate flag in the `__index__` dict to be "
+    + "false. Plese set them to true for the files which needs to be validated."
+)
+
 REPORT_GENERATION_SUPPORTED_REPOS = ["geo"]
 
 DELETION_OPERATION_UNSUCCESSFUL_FOR_ALL_DATASET_IDS = (
     "Files not deleted. Possible reasons to help you troubleshoot :- "
     + "\n"
     + "1. All the datasets passed to delete might not be "
     + "present in the Omixatlas. Please check warning message logged during execution. "
```

### Comparing `polly-python-0.3.0/polly/core_cohort.py` & `polly-python-0.3.1/polly/core_cohort.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.0/polly/curation.py` & `polly-python-0.3.1/polly/curation.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.0/polly/errors.py` & `polly-python-0.3.1/polly/errors.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.0/polly/help.py` & `polly-python-0.3.1/polly/help.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.0/polly/helpers.py` & `polly-python-0.3.1/polly/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,15 +314,15 @@
     response = self.session.post(url, data=json.dumps(payload))
     error_handler(response)
     response_data = response.json()
     hits = response_data.get("hits", {}).get("hits")
     if not (hits and isinstance(hits, list)):
         raise paramException(
             title="Param Error",
-            detail="No matches found with the given repo details. Please try again.",
+            detail="No dataset matches found in the given repo. Please retry with the correct dataset ID.",
         )
     dataset = hits[0]
     return dataset
 
 
 def elastic_query(index_name: str, dataset_id: str) -> dict:
     query = {
@@ -1009,7 +1009,25 @@
             }
         },
         # Fetch X many rows at a time (you will still get the full output, which may be greater than 10K)
         # Setting this value to be greater than 10k will result in an error
         "size": page_size,
     }
     return query
+
+
+def read_json(path: str) -> json:
+    """
+    Function to read json content from a file.
+    """
+    with open(path) as filepath:
+        return json.load(filepath)
+
+
+def remove_prefix(text: str, prefix: str) -> str:
+    """
+    Function to remove prefix from text.
+    """
+    if text.startswith(prefix):
+        slice_obj = slice(len(prefix), len(text))
+        return text[slice_obj]
+    return text
```

### Comparing `polly-python-0.3.0/polly/http_response_codes.py` & `polly-python-0.3.1/polly/http_response_codes.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.0/polly/jobs.py` & `polly-python-0.3.1/polly/jobs.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.0/polly/omixatlas.py` & `polly-python-0.3.1/polly/omixatlas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1234,15 +1234,15 @@
                 # converting requests output to JSON
                 resp = resp.json()
                 schema_update_verdict = (
                     resp.get("data", {})
                     .get("attributes", {})
                     .get("schema_update_verdict", "")
                 )
-                # There are 3 cases for schema updation
+                # There are 3 cases for schema updation when done put operation
                 # In case 1 -> if user changes attributes in the field
                 # other than `original_name`, `type`, `is_array`, `is_keyword`
                 # `is_searchable`
                 # In those cases -> schema update is performed instantly
                 # In the schema_update_verdict key -> value is none
 
                 # In case 2 -> If user renames a field or drops a field
@@ -1264,15 +1264,15 @@
 
                 schema_update_verdict_val = const.SCHEMA_VERDICT_DICT.get(
                     schema_update_verdict, ""
                 )
                 if schema_update_verdict_val:
                     print(schema_update_verdict_val)
                 else:
-                    print(const.SCHEMA_UPDATE_GENERIC_MSG)
+                    print(const.SCHEMA_REPLACE_GENERIC_MSG)
         except Exception as err:
             raise err
 
     @Track.track_decorator
     def download_data(self, repo_name, _id: str, internal_call=False):
         """
         To download any dataset, the following function can be used to get the signed URL of the dataset.
@@ -2157,14 +2157,18 @@
             pd.DataFrame: DataFrame showing Upload Status of Files
         """
         try:
             # parameters check
             self._parameter_check_for_add_dataset(
                 repo_id, source_folder_path, destination_folder_path, priority
             )
+            if destination_folder_path:
+                destination_folder_path = omix_hlpr.normalise_destination_path(
+                    self, destination_folder_path, repo_id
+                )
             validation_dataset_lvl = {}
             if validation:
                 validation_dataset_lvl = omix_hlpr.check_status_file(source_folder_path)
             (
                 session_tokens,
                 bucket_name,
                 package_name,
@@ -2257,14 +2261,18 @@
                     omix_hlpr.data_files_whose_metadata_failed_validation,
                     "Invalid Data Files",
                 )
             # reset global variables storing validation results
             # flushes out the previous state of variables and creates
             # new state
             omix_hlpr.reset_global_variables_with_validation_results()
+            if destination_folder_path:
+                print(
+                    f"\nDestination folder path considered for ingestion request: {destination_folder_path}"
+                )
 
             return data_upload_results_df
         except Exception as err:
             raise err
 
     @Track.track_decorator
     def update_datasets(
@@ -2416,26 +2424,20 @@
         When it is returned as a response of list files API in OA in the file_id key
         Merely being a folder present in the s3 bucket of the OA does not make it valid
         destination folder.
         Args:
             destination_folder_path (str): destination folder passed
             repo_id(str): repo_id of the repository
         """
-        list_oa_response = self._list_files_in_oa(repo_id)
-        oa_data_files_list = []
-        for response_data in list_oa_response:
-            for item in response_data:
-                file_id = item.get("id")
-                oa_data_files_list.append(file_id)
 
-        valid_folder_list = helpers.get_folder_list_from_list_of_filepaths(
-            oa_data_files_list
+        pathExists, valid_folder_list = omix_hlpr.return_destination_folder_status(
+            self, destination_folder_path, repo_id
         )
 
-        if destination_folder_path not in valid_folder_list:
+        if not pathExists:
             raise paramException(
                 title="Destination Folder passed does not exist",
                 detail=(
                     "Destination folder passed does not exist. "
                     + "Either wrong destination folder passed for the existing data/metadata."
                     + f"Valid destination folders are {valid_folder_list} in this repository. "
                     + "Or data/metadata passed in update does not exist in this repository "
@@ -4386,10 +4388,39 @@
         except Exception as err:
             print(
                 f" Error in getting the lock status for omixatlas: {repo_key}."
                 + f" ERROR: {err}"
             )
             return
 
+    @Track.track_decorator
+    def _fetch_quilt_metadata(self, repo_key: str, dataset_id: str) -> dict:
+        """
+        This function is used to get the quilt sample level metadata as a dataframe.
+        Args:
+            repo_key(str/int): repo_name/repo_id of the repository.
+            dataset_id(str): dataset_id of the dataset.
+        Raises:
+              paramException:
+              RequestFailureException:
+        Returns:
+            Quilt metadata in json format is returned.
+        """
+        omix_hlpr.check_params_for_fetch_quilt_metadata(repo_key, dataset_id)
+        repo_summary = self.omixatlas_summary(repo_key)
+        repo_id = repo_summary.get("data", "").get("repo_id")  # Extracting repo_id
+        # getting dataset level metadata using download_metadata function
+        with TempDir() as dir_path:
+            self.download_metadata(repo_id, dataset_id, dir_path)
+            filepath = os.path.join(dir_path, f"{dataset_id}.json")
+            metadata = helpers.read_json(filepath)
+        package = metadata["package"] + "/"
+        file_id = helpers.remove_prefix(metadata["key"], package)
+        url = self.discover_url + f"/repositories/{repo_id}/files/{file_id}"
+        # get request to fetch quilt metadata
+        response = self.session.get(url)
+        error_handler(response)
+        return response.json().get("data", "").get("attributes", "").get("metadata")
+
 
 if __name__ == "__main__":
     client = OmixAtlas()
```

### Comparing `polly-python-0.3.0/polly/omixatlas_hlpr.py` & `polly-python-0.3.1/polly/omixatlas_hlpr.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,29 @@
     elif type(repo_id) != str and type(repo_id) != int:
         raise paramException(
             title="Param Error",
             detail=f"repo_id, {repo_id} should be str or int",
         )
 
 
+def parameter_check_for_dataset_id(dataset_id):
+    """Checking for validity of repo id
+    Args:
+        dataset_id (): Dataset Id of the dataset
+
+    Raises:
+        paramException: Error if dataset id is empty or is not str
+    """
+    if not (dataset_id and isinstance(dataset_id, str)):
+        raise paramException(
+            title="Param Error",
+            detail="Argument 'dataset_id' is either empty or invalid. It should be a string. Please try again.",
+        )
+
+
 def make_repo_id_string(repo_id: int) -> str:
     """If repo id is int, change to string
 
     Args:
         repo_id (int/str): repo_id of the omixatlas
 
     Returns:
@@ -1226,17 +1241,19 @@
     # once the pages will end -> next_link will be
     # set to None by the API
     while next_link is not None:
         if next_link:
             next_endpoint = f"{self.discover_url}{next_link}"
             response = self.session.get(next_endpoint)
         else:
-            # getting the response for the first 1000 pages initially
+            # getting the response for the first 100 pages initially
+            # 100 page is set for now -> so that data does not max out
+            # TODO -> need to be optimised for page size and time
             query_params = {
-                "page[size]": 1000,
+                "page[size]": 100,
                 "page[after]": 0,
                 "include_metadata": f"{metadata}",
                 "data": f"{data}",
                 "version": f"{version}",
             }
             response = self.session.get(files_api_endpoint, params=query_params)
         response.raise_for_status()
@@ -1641,7 +1658,73 @@
         raise InvalidSchemaJsonException()
     else:
         (
             title,
             details,
         ) = extract_error_message_details(response)
         raise Exception("Exception Occurred :" + str(details))
+
+
+def normalise_destination_path(self, destination_folder_path: str, repo_id: str) -> str:
+    status_info = return_destination_folder_status(
+        self, destination_folder_path, repo_id
+    )
+    pathExists = status_info[0]
+    # if destination_folder does not exist, then normalise the path, otherwise not
+    if not pathExists:
+        destination_folder_path = return_normalise_destination_path(
+            destination_folder_path
+        )
+    return destination_folder_path
+
+
+def return_normalise_destination_path(destination_folder_path: str) -> str:
+    normalised_path = os.path.normpath(destination_folder_path)
+    return normalised_path
+
+
+def return_destination_folder_status(
+    self, destination_folder_path: str, repo_id: str
+) -> tuple:
+    """
+    Function to check if the destination_folder_path already exist.
+    Args:
+        destination_folder_path (str): destination folder passed
+        repo_id(str): repo_id of the repository
+    """
+    list_oa_response = list_files(self, repo_id, metadata=False)
+    oa_data_files_list = []
+    for response in list_oa_response:
+        response_json = response.json()
+        response_data = response_json.get("data")
+        for item in response_data:
+            file_id = item.get("id")
+            oa_data_files_list.append(file_id)
+
+    valid_folder_list = helpers.get_folder_list_from_list_of_filepaths(
+        oa_data_files_list
+    )
+
+    # return status(whether destination_folder_path exists or not) and valid_folder_list as a tuple
+
+    if destination_folder_path not in valid_folder_list:
+        return False, valid_folder_list
+    return True, valid_folder_list
+
+
+def check_params_for_fetch_quilt_metadata(repo_key, dataset_id):
+    """
+    Args:
+        repo_key(str/int): repo_name/repo_id of the repository.
+        dataset_id(str): dataset_id of the dataset.
+    """
+    if not (repo_key and (isinstance(repo_key, str) or isinstance(repo_key, int))):
+        raise paramException(
+            title="Param Error",
+            detail="Argument 'repo_key' is either empty or invalid. \
+It should either be a string or an integer. Please try again.",
+        )
+    if not (dataset_id and isinstance(dataset_id, str)):
+        raise paramException(
+            title="Param Error",
+            detail="Argument 'dataset_id' is either empty or invalid. It should be a string. Please try again.",
+        )
```

### Comparing `polly-python-0.3.0/polly/schema.py` & `polly-python-0.3.1/polly/schema.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.0/polly/session.py` & `polly-python-0.3.1/polly/session.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.0/polly/tracking.py` & `polly-python-0.3.1/polly/tracking.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.0/polly/workspaces.py` & `polly-python-0.3.1/polly/workspaces.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.0/polly_python.egg-info/PKG-INFO` & `polly-python-0.3.1/polly_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polly-python
-Version: 0.3.0
+Version: 0.3.1
 Summary: Polly SDK
 Home-page: https://github.com/ElucidataInc/polly-python
 Project-URL: Documentation, https://docs.elucidata.io
 Project-URL: Tutorial Notebooks, https://github.com/ElucidataInc/polly-python
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: testing
```

### Comparing `polly-python-0.3.0/polly_python.egg-info/SOURCES.txt` & `polly-python-0.3.1/polly_python.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE.md
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 polly/__init__.py
+polly/analyze.py
 polly/application_error_info.py
 polly/auth.py
 polly/bridge_cohort.py
 polly/cohort.py
 polly/constants.py
 polly/core_cohort.py
 polly/curation.py
```

### Comparing `polly-python-0.3.0/setup.cfg` & `polly-python-0.3.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 	datapane>=0.9.1
 	plotly>=2.0.0
 	python-jose>=3.3.0
 	cryptography>=37.0.1
 	mixpanel>=4.10.0
 	beautifulsoup4
 	elucidatacloudpathlib==0.6.6
-	polly_validator==0.0.1
+	polly_validator==0.0.2
 include_package_data = True
 
 [options.packages.find]
 exclude = 
 	tests*
 	build*
 	dist*
```

### Comparing `polly-python-0.3.0/tests/test_cohort.py` & `polly-python-0.3.1/tests/test_cohort.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.0/tests/test_constants.py` & `polly-python-0.3.1/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.0/tests/test_curation.py` & `polly-python-0.3.1/tests/test_curation.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.0/tests/test_helpers.py` & `polly-python-0.3.1/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.0/tests/test_omixatlas.py` & `polly-python-0.3.1/tests/test_omixatlas.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 from polly.constants import BASE_TEST_FORMAT_CONSTANTS_URL
 from polly.errors import error_handler
 
 # import polly.omixatlas_hlpr as omix_hlpr
 from polly.validation import Validation
 from test_constants import INGESTION_TEST_1_REPO_ID, MOCK_RESPONSE_DOWNLOAD_DATA
 
+from polly_validator.validators import dataset_metadata_validator
+
 # from botocore.exceptions import ClientError
 
 
 key = "POLLY_REFRESH_TOKEN"
 token = os.getenv(key)
 test_key = "TEST_POLLY_REFRESH_TOKEN"
 testpolly_token = os.getenv(test_key)
@@ -1657,14 +1659,16 @@
     destination_folder = "transcriptomics_test"
     with pytest.warns(Warning) as record:
         omix_obj.update_datasets(repo_id, source_folder_path, destination_folder)
         if not record:
             pytest.fail("Expected a warning!")
 
 
+# TODO make changes in the tests when new validation flow of
+# multi source, multi datatype is integrated
 def test_update_dataset_metadata_file_with_wrong_extension():
     Polly.auth(testpolly_token, env="testpolly")
     omix_obj = omixatlas.OmixAtlas()
     # ingestion_test_1
     repo_id = "1654268055800"
 
     metadata_2_name = "incorrect_ext_data_file.txt"
@@ -1694,15 +1698,31 @@
     with pytest.raises(
         paramException,
         match=r".* File format for file .* invalid.It can be =>.*",
     ):
         omix_obj.update_datasets(repo_id, source_folder_path, destination_folder)
 
 
-def test_validation_addition_datasets_full_flow():
+@pytest.fixture()
+def get_validatation_lib_mock_fixture():
+    data = ["a", "b", "c"]
+    empty_df = pd.DataFrame(data)
+
+    err_dataset = empty_df
+    status_dict = {
+        "ACBC_MSKCC_2015_Copy_Number_AdCC10T": False,
+        "ACBC_MSKCC_2015_Copy_Number_AdCC12T": False,
+    }
+
+    return err_dataset, status_dict
+
+
+def test_validation_addition_datasets_full_flow(
+    mocker, get_validatation_lib_mock_fixture
+):
     Polly.auth(testpolly_token, env="testpolly")
     omix_obj = omixatlas.OmixAtlas()
     validation_obj = Validation()
     # ingestion_test_1
     repo_id = "1654268055800"
     base_add_datatest_test_file_path = const.VALIDATION_FLOW_FILES_URL
 
@@ -1790,17 +1810,27 @@
 
     with open(os.path.join(metadata_path, metadata_file_4_name), "w") as meta_file_4:
         metadata_4_content = metadata_resp_4.text
         meta_file_4.write(metadata_4_content)
 
     source_folder_path = {"data": data_path, "metadata": metadata_path}
     destination_folder = "transcriptomics_test"
+    schema_config = {}
+    schema_config["source"] = "geo"
+    schema_config["datatype"] = "all"
+
+    # mock validation library response
+
+    mocker.patch(
+        dataset_metadata_validator.__name__ + ".check_metadata_for_errors",
+        return_value=get_validatation_lib_mock_fixture,
+    )
 
     err_dataset_df, status_dict = validation_obj.validate_datasets(
-        repo_id, source_folder_path
+        repo_id, source_folder_path, schema_config=schema_config
     )
 
     assert isinstance(err_dataset_df, pd.DataFrame)
     assert isinstance(status_dict, dict)
 
     res_df = omix_obj.add_datasets(
         repo_id, source_folder_path, destination_folder, validation=True
@@ -1809,16 +1839,16 @@
 
     # only two files will be uploaded
     # Other two files will not be uploaded as they have failed validation
     # applying assertion on res_df to check only two files
     # coming in `res_df`
     # 1 more file `combined_metadata` file will be uploaded
     # TODO: revert to back to 3 value once the validation lib issues are fixed
-    # assert res_df.shape[0] == 3
-    assert res_df.shape[0] == 5
+    assert res_df.shape[0] == 3
+    # assert res_df.shape[0] == 5
 
 
 # DLS_BB057_CV244_AML_BMMC_ATAC088_ATAC089_GEX062_GEX063_MTDNA073_MTDNA074_0.05rnaclustres_0.05corr.zip
 # this file is there in s3 but not ingested in the infra so it is giving warning that is why test is failing
 # def test_update_dataset_correct_combined_metadata_json():
 #     # test generation of combined_metadata json and content
 #     # json should have ingestion and dataset details.
@@ -1903,21 +1933,56 @@
 #     types_in_metadata_dict = []
 #     for item in combined_metadata_dict["data"]:
 #         types_in_metadata_dict.append(item.get("type"))
 #     assert "ingestion_metadata" in types_in_metadata_dict
 #     assert "file_metadata" in types_in_metadata_dict
 
 
-def test_get_metadata():
+@pytest.fixture()
+def get_metadata_fixture():
+    """Get geo metadata from github"""
+    base_polly_py_test_url = test_const.POLLY_PY_TEST_FILES_URL
+
+    data_file = f"{base_polly_py_test_url}/geo_get_metadata_response.json"
+    data = requests.get(data_file)
+    error_handler(data)
+    return data
+
+
+@pytest.fixture()
+def get_metadata_empty_hits_fixture():
+    """Get response with empty hits from github"""
+    base_polly_py_test_url = test_const.POLLY_PY_TEST_FILES_URL
+
+    data_file = f"{base_polly_py_test_url}/final_pagination_mocked_response.json"
+    data = requests.get(data_file)
+    error_handler(data)
+    return data
+
+
+@pytest.fixture()
+def get_metadata_csv_fixture():
+    """Get geo metadata csv file from github"""
+    base_polly_py_test_url = test_const.POLLY_PY_TEST_FILES_URL
+
+    data_file = f"{base_polly_py_test_url}/geo_get_metadata_test_df.csv"
+    try:
+        data_df = pd.read_csv(data_file)
+    except Exception as err:
+        raise err
+    return data_df
+
+
+def test_get_metadata(mocker, get_metadata_csv_fixture):
     Polly.auth(token)
     obj = omixatlas.OmixAtlas()
     correct_repo_name = "geo"
     correct_repo_id = 9
     incorrect_repo_key = [9]
-    correct_dataset_id = "GSE100053_GPL10558"
+    correct_dataset_id = "GSE199927_GPL19057"
     incorrect_dataset_id = 1234
     correct_table_name = "samples"
     incorrect_table_name = "datasets"
     assert isinstance(
         obj.get_metadata(correct_repo_name, correct_dataset_id, correct_table_name),
         pd.DataFrame,
     )
@@ -1938,14 +2003,90 @@
         obj.get_metadata(correct_repo_id, incorrect_dataset_id, correct_table_name)
 
     with pytest.raises(
         paramException,
         match=r".*Argument 'repo_key' is either empty or invalid. .*",
     ):
         obj.get_metadata(incorrect_repo_key, correct_dataset_id, correct_table_name)
+    dataframe_result = get_metadata_csv_fixture
+    mocker.patch(
+        polly.omixatlas.__name__ + ".OmixAtlas._retrieve_dataframe",
+        return_value=dataframe_result,
+    )
+    result = obj.get_metadata(correct_repo_name, correct_dataset_id, correct_table_name)
+    assert result.equals(dataframe_result) is True
+
+
+def test_retrieve_dataframe(mocker, get_metadata_fixture, get_metadata_csv_fixture):
+    Polly.auth(token)
+    obj = omixatlas.OmixAtlas()
+    index = "geo_gct_col_metadata"
+    discover_url = (
+        f"https://api.datalake.discover.{obj.session.env}.elucidata.io/elastic/v2"
+    )
+    page_size = 1000
+    dataset_id = "GSE199927_GPL19057"
+    intermediate_result = get_metadata_fixture
+    dataframe_result = get_metadata_csv_fixture
+    mocker.patch(
+        polly.omixatlas.__name__ + ".OmixAtlas._initiate_retrieval",
+        return_value=intermediate_result,
+    )
+    mocker.patch(
+        polly.omixatlas.__name__ + ".OmixAtlas._complete_retrieval",
+        return_value=dataframe_result,
+    )
+    result = obj._retrieve_dataframe(discover_url, page_size, dataset_id, index)
+    assert isinstance(result, pd.DataFrame)
+
+
+def test_initiate_retrieval(mocker, get_metadata_fixture):
+    Polly.auth(token)
+    obj = omixatlas.OmixAtlas()
+    dataframe_result = get_metadata_fixture
+    response = mocker.patch.object(obj.session, "post")
+    response.return_value.status_code = 200
+    response.return_value = dataframe_result
+    index = "geo_gct_col_metadata"
+    discover_url = (
+        f"https://api.datalake.discover.{obj.session.env}.elucidata.io/elastic/v2"
+    )
+    page_size = 1000
+    dataset_id = "GSE199927_GPL19057"
+    query = {
+        "query": {
+            "term": {
+                # Count entries for the following key-value pairs
+                "src_dataset_id.keyword": dataset_id
+            }
+        },
+        # Fetch X many rows at a time (you will still get the full output, which may be greater than 10K)
+        # Setting this value to be greater than 10k will result in an error
+        "size": page_size,
+    }
+    result = obj._initiate_retrieval(discover_url, query, index)
+    assert isinstance(result, dict)
+
+
+def test_complete_retrieval(
+    mocker, get_metadata_fixture, get_metadata_empty_hits_fixture
+):
+    Polly.auth(token)
+    obj = omixatlas.OmixAtlas()
+    dataframe_result = get_metadata_empty_hits_fixture
+    response = mocker.patch.object(obj.session, "post")
+    response.return_value.status_code = 200
+    response.return_value = dataframe_result
+    discover_url = (
+        f"https://api.datalake.discover.{obj.session.env}.elucidata.io/elastic/v2"
+    )
+    intermediate_result = get_metadata_fixture
+    json_arg = json.loads(intermediate_result.text)
+    result = obj._complete_retrieval(discover_url, json_arg)
+    assert isinstance(result, pd.DataFrame)
 
 
 @pytest.fixture()
 def get_ingestion_test_1_fixture():
     """Get ingestion_test_1 from github and store it in local"""
     base_polly_py_test_url = test_const.POLLY_PY_TEST_FILES_URL
     parent_dir = os.getcwd()
@@ -2142,14 +2283,76 @@
     with pytest.raises(
         paramException,
         match=r"body should not be empty and it should be of type dict",
     ):
         omix_obj.update_schema(repo_id, body)
 
 
+# replace schema tests
+# replace schema test 1 -> positive case
+def test_replace_schema_positive_case(
+    mocker, validate_schema_mock_fixture, capsys, get_ingestion_test_1_schema_fixture
+):
+    # Doing it on a repo that already exists
+    # 1st -> Mock response of `_get_omixatlas()` call
+    # inside validate schema -> make a seperate mocked function for that
+    mocker.patch(
+        polly.omixatlas.__name__ + ".OmixAtlas.validate_schema",
+        return_value=validate_schema_mock_fixture,
+    )
+
+    # then mocking the response of PUT API CALL for Replace Schema
+    Polly.auth(testpolly_token, env="testpolly")
+    nobj = omixatlas.OmixAtlas()
+    # mocked response with status and no specific value
+    # as no specific response is mocked -> generic message will be printed
+    response = mocker.patch.object(nobj.session, "put")
+    response.return_value.status_code = 200
+
+    # ingestion_test_1
+    repo_id = test_const.INGESTION_TEST_1_REPO_ID
+
+    body = get_ingestion_test_1_schema_fixture
+
+    nobj.replace_schema(repo_id, body)
+    # when successfully run
+    # comparing the print in the function is coming out
+    # in the stdout
+    captured = capsys.readouterr()
+    assert "Schema replace is in progress" in captured.out
+
+
+# replace schema test 2 -> repo_id wrong format
+def test_replace_schema_repo_id_wrong_format(get_ingestion_test_1_schema_fixture):
+    Polly.auth(testpolly_token, env="testpolly")
+    omix_obj = omixatlas.OmixAtlas()
+    repo_id = [test_const.INGESTION_TEST_1_REPO_ID]
+    body = get_ingestion_test_1_schema_fixture
+
+    with pytest.raises(
+        paramException,
+        match=r".should be str or int",
+    ):
+        omix_obj.replace_schema(repo_id, body)
+
+
+# replace schema test 3 -> body wrong format
+def test_replace_schema_body_wrong_format():
+    Polly.auth(testpolly_token, env="testpolly")
+    omix_obj = omixatlas.OmixAtlas()
+    repo_id = test_const.INGESTION_TEST_1_REPO_ID
+    body = "abcd"
+
+    with pytest.raises(
+        paramException,
+        match=r"body should not be empty and it should be of type dict",
+    ):
+        omix_obj.replace_schema(repo_id, body)
+
+
 def test_check_omixatlas_status(mocker, capsys, get_omixatlas_mock_fixture):
     Polly.auth(testpolly_token, env="testpolly")
     obj = omixatlas.OmixAtlas()
     # when the repo is not locked
     mocker.patch(
         polly.omixatlas.__name__ + ".OmixAtlas._get_omixatlas",
         return_value=get_omixatlas_mock_fixture,
```

### Comparing `polly-python-0.3.0/tests/test_schema_ux.py` & `polly-python-0.3.1/tests/test_schema_ux.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.0/tests/test_workspaces.py` & `polly-python-0.3.1/tests/test_workspaces.py`

 * *Files identical despite different names*

