# Comparing `tmp/kumo-ai-0.1.0.tar.gz` & `tmp/kumo-ai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kumo-ai-0.1.0.tar", last modified: Thu Apr  6 16:42:09 2023, max compression
+gzip compressed data, was "kumo-ai-0.1.1.tar", last modified: Thu May 18 16:28:34 2023, max compression
```

## Comparing `kumo-ai-0.1.0.tar` & `kumo-ai-0.1.1.tar`

### file list

```diff
@@ -1,35 +1,32 @@
-drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-04-06 16:42:09.691613 kumo-ai-0.1.0/
--rw-r--r--   0 siyang     (501) staff       (20)     1800 2023-02-27 18:06:46.000000 kumo-ai-0.1.0/.gitignore
--rw-r--r--   0 siyang     (501) staff       (20)      933 2023-03-17 21:55:08.000000 kumo-ai-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 siyang     (501) staff       (20)     1061 2023-02-23 21:09:43.000000 kumo-ai-0.1.0/LICENSE
--rw-r--r--   0 siyang     (501) staff       (20)      161 2023-03-17 21:55:08.000000 kumo-ai-0.1.0/Makefile
--rw-r--r--   0 siyang     (501) staff       (20)      482 2023-04-06 16:42:09.691486 kumo-ai-0.1.0/PKG-INFO
--rw-r--r--   0 siyang     (501) staff       (20)       39 2023-02-23 21:09:43.000000 kumo-ai-0.1.0/README.md
-drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-04-06 16:42:09.688802 kumo-ai-0.1.0/examples/
--rw-r--r--   0 siyang     (501) staff       (20)        0 2023-03-29 16:49:40.000000 kumo-ai-0.1.0/examples/__init__.py
--rw-r--r--   0 siyang     (501) staff       (20)     4714 2023-04-05 16:11:54.000000 kumo-ai-0.1.0/examples/financial.py
--rw-r--r--   0 siyang     (501) staff       (20)     8950 2023-04-04 17:45:57.000000 kumo-ai-0.1.0/examples/financial_binary_classify_S3.json
--rw-r--r--   0 siyang     (501) staff       (20)     9339 2023-04-04 17:45:36.000000 kumo-ai-0.1.0/examples/financial_binary_classify_SNOWFLAKE.json
--rw-r--r--   0 siyang     (501) staff       (20)     5373 2023-03-29 17:21:11.000000 kumo-ai-0.1.0/examples/hm_churn.json
--rw-r--r--   0 siyang     (501) staff       (20)     3072 2023-04-05 16:17:05.000000 kumo-ai-0.1.0/examples/orchestration.py
--rw-r--r--   0 siyang     (501) staff       (20)     3427 2023-04-05 16:49:00.000000 kumo-ai-0.1.0/examples/save_load_modify_pquery.py
-drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-04-06 16:42:09.689099 kumo-ai-0.1.0/kumo/
--rw-r--r--   0 siyang     (501) staff       (20)        0 2023-02-27 18:06:46.000000 kumo-ai-0.1.0/kumo/__init__.py
--rw-r--r--   0 siyang     (501) staff       (20)    10792 2023-04-06 16:19:12.000000 kumo-ai-0.1.0/kumo/client.py
-drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-04-06 16:42:09.690543 kumo-ai-0.1.0/kumo/datamodel/
--rw-r--r--   0 siyang     (501) staff       (20)        0 2023-02-27 18:06:46.000000 kumo-ai-0.1.0/kumo/datamodel/__init__.py
--rw-r--r--   0 siyang     (501) staff       (20)     2280 2023-03-17 21:55:08.000000 kumo-ai-0.1.0/kumo/datamodel/advanced_options.py
--rw-r--r--   0 siyang     (501) staff       (20)      974 2023-04-03 17:42:04.000000 kumo-ai-0.1.0/kumo/datamodel/data_source.py
--rw-r--r--   0 siyang     (501) staff       (20)     5753 2023-03-17 21:55:08.000000 kumo-ai-0.1.0/kumo/datamodel/jobs.py
--rw-r--r--   0 siyang     (501) staff       (20)      561 2023-04-05 16:11:01.000000 kumo-ai-0.1.0/kumo/datamodel/json_serde.py
--rw-r--r--   0 siyang     (501) staff       (20)     6420 2023-04-04 17:42:54.000000 kumo-ai-0.1.0/kumo/datamodel/pquery.py
-drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-04-06 16:42:09.691299 kumo-ai-0.1.0/kumo_ai.egg-info/
--rw-r--r--   0 siyang     (501) staff       (20)      482 2023-04-06 16:42:09.000000 kumo-ai-0.1.0/kumo_ai.egg-info/PKG-INFO
--rw-r--r--   0 siyang     (501) staff       (20)      694 2023-04-06 16:42:09.000000 kumo-ai-0.1.0/kumo_ai.egg-info/SOURCES.txt
--rw-r--r--   0 siyang     (501) staff       (20)        1 2023-04-06 16:42:09.000000 kumo-ai-0.1.0/kumo_ai.egg-info/dependency_links.txt
--rw-r--r--   0 siyang     (501) staff       (20)       34 2023-04-06 16:42:09.000000 kumo-ai-0.1.0/kumo_ai.egg-info/requires.txt
--rw-r--r--   0 siyang     (501) staff       (20)       14 2023-04-06 16:42:09.000000 kumo-ai-0.1.0/kumo_ai.egg-info/top_level.txt
--rw-r--r--   0 siyang     (501) staff       (20)      993 2023-04-04 16:46:24.000000 kumo-ai-0.1.0/precommit-pyrightconfig.json
--rw-r--r--   0 siyang     (501) staff       (20)      876 2023-03-06 23:37:27.000000 kumo-ai-0.1.0/pyrightconfig.json
--rw-r--r--   0 siyang     (501) staff       (20)       38 2023-04-06 16:42:09.691655 kumo-ai-0.1.0/setup.cfg
--rw-r--r--   0 siyang     (501) staff       (20)      885 2023-04-06 16:41:55.000000 kumo-ai-0.1.0/setup.py
+drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-05-18 16:28:34.091120 kumo-ai-0.1.1/
+-rw-r--r--   0 siyang     (501) staff       (20)     1800 2023-02-27 18:06:46.000000 kumo-ai-0.1.1/.gitignore
+-rw-r--r--   0 siyang     (501) staff       (20)      933 2023-03-17 21:55:08.000000 kumo-ai-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 siyang     (501) staff       (20)     1061 2023-02-23 21:09:43.000000 kumo-ai-0.1.1/LICENSE
+-rw-r--r--   0 siyang     (501) staff       (20)      161 2023-03-17 21:55:08.000000 kumo-ai-0.1.1/Makefile
+-rw-r--r--   0 siyang     (501) staff       (20)      482 2023-05-18 16:28:34.090978 kumo-ai-0.1.1/PKG-INFO
+-rw-r--r--   0 siyang     (501) staff       (20)       39 2023-02-23 21:09:43.000000 kumo-ai-0.1.1/README.md
+drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-05-18 16:28:34.088544 kumo-ai-0.1.1/kumo_ai.egg-info/
+-rw-r--r--   0 siyang     (501) staff       (20)      482 2023-05-18 16:28:34.000000 kumo-ai-0.1.1/kumo_ai.egg-info/PKG-INFO
+-rw-r--r--   0 siyang     (501) staff       (20)      622 2023-05-18 16:28:34.000000 kumo-ai-0.1.1/kumo_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 siyang     (501) staff       (20)        1 2023-05-18 16:28:34.000000 kumo-ai-0.1.1/kumo_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 siyang     (501) staff       (20)       34 2023-05-18 16:28:34.000000 kumo-ai-0.1.1/kumo_ai.egg-info/requires.txt
+-rw-r--r--   0 siyang     (501) staff       (20)        7 2023-05-18 16:28:34.000000 kumo-ai-0.1.1/kumo_ai.egg-info/top_level.txt
+drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-05-18 16:28:34.088760 kumo-ai-0.1.1/kumoai/
+-rw-r--r--   0 siyang     (501) staff       (20)        0 2023-02-27 18:06:46.000000 kumo-ai-0.1.1/kumoai/__init__.py
+-rw-r--r--   0 siyang     (501) staff       (20)    10800 2023-05-18 16:22:45.000000 kumo-ai-0.1.1/kumoai/client.py
+drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-05-18 16:28:34.090007 kumo-ai-0.1.1/kumoai/datamodel/
+-rw-r--r--   0 siyang     (501) staff       (20)        0 2023-02-27 18:06:46.000000 kumo-ai-0.1.1/kumoai/datamodel/__init__.py
+-rw-r--r--   0 siyang     (501) staff       (20)     2280 2023-03-17 21:55:08.000000 kumo-ai-0.1.1/kumoai/datamodel/advanced_options.py
+-rw-r--r--   0 siyang     (501) staff       (20)      974 2023-04-03 17:42:04.000000 kumo-ai-0.1.1/kumoai/datamodel/data_source.py
+-rw-r--r--   0 siyang     (501) staff       (20)     5755 2023-05-18 16:22:45.000000 kumo-ai-0.1.1/kumoai/datamodel/jobs.py
+-rw-r--r--   0 siyang     (501) staff       (20)      561 2023-04-05 16:11:01.000000 kumo-ai-0.1.1/kumoai/datamodel/json_serde.py
+-rw-r--r--   0 siyang     (501) staff       (20)     6422 2023-05-18 16:22:45.000000 kumo-ai-0.1.1/kumoai/datamodel/pquery.py
+drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-05-18 16:28:34.090746 kumo-ai-0.1.1/kumoai/examples/
+-rw-r--r--   0 siyang     (501) staff       (20)        0 2023-03-29 16:49:40.000000 kumo-ai-0.1.1/kumoai/examples/__init__.py
+-rw-r--r--   0 siyang     (501) staff       (20)     4722 2023-05-18 16:22:45.000000 kumo-ai-0.1.1/kumoai/examples/financial.py
+-rw-r--r--   0 siyang     (501) staff       (20)     3076 2023-05-18 16:22:45.000000 kumo-ai-0.1.1/kumoai/examples/orchestration.py
+-rw-r--r--   0 siyang     (501) staff       (20)     3433 2023-05-18 16:22:45.000000 kumo-ai-0.1.1/kumoai/examples/save_load_modify_pquery.py
+-rw-r--r--   0 siyang     (501) staff       (20)      993 2023-04-04 16:46:24.000000 kumo-ai-0.1.1/precommit-pyrightconfig.json
+-rw-r--r--   0 siyang     (501) staff       (20)      876 2023-03-06 23:37:27.000000 kumo-ai-0.1.1/pyrightconfig.json
+-rw-r--r--   0 siyang     (501) staff       (20)       38 2023-05-18 16:28:34.091164 kumo-ai-0.1.1/setup.cfg
+-rw-r--r--   0 siyang     (501) staff       (20)      885 2023-05-18 16:22:30.000000 kumo-ai-0.1.1/setup.py
```

### Comparing `kumo-ai-0.1.0/.gitignore` & `kumo-ai-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.0/.pre-commit-config.yaml` & `kumo-ai-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.0/LICENSE` & `kumo-ai-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.0/examples/financial.py` & `kumo-ai-0.1.1/kumoai/examples/financial.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import logging
 import os
 import sys
 from typing import Dict
 
-from kumo.client import KumoClient
-from kumo.datamodel.data_source import (DataSourceType, SnowflakeConnectorArgs,
+from kumoai.client import KumoClient
+from kumoai.datamodel.data_source import (DataSourceType, SnowflakeConnectorArgs,
                                         SnowflakeConnectorResourceConfig,
                                         UsernamePassword)
-from kumo.datamodel.json_serde import to_json
-from kumo.datamodel.pquery import (ColumnKey, ColumnKeyGroup, GraphDefinition,
+from kumoai.datamodel.json_serde import to_json
+from kumoai.datamodel.pquery import (ColumnKey, ColumnKeyGroup, GraphDefinition,
                                    PQueryResource, SourceTableInfo, TableName)
 
 logging.basicConfig(format='%(asctime)s | %(levelname)s : %(message)s',
                     level=logging.INFO,
                     stream=sys.stdout)
 
 logger = logging.getLogger(__name__)
```

### Comparing `kumo-ai-0.1.0/examples/orchestration.py` & `kumo-ai-0.1.1/kumoai/examples/orchestration.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import sys
 from time import sleep
 
-from kumo.client import KumoClient
-from kumo.datamodel.jobs import (JobStatus, MetadataField,
+from kumoai.client import KumoClient
+from kumoai.datamodel.jobs import (JobStatus, MetadataField,
                                  PredictionArtifactType, PredictionStorageType,
                                  S3PredictionOutput)
 
 logging.basicConfig(format='%(asctime)s | %(levelname)s : %(message)s',
                     level=logging.INFO,
                     stream=sys.stdout)
```

### Comparing `kumo-ai-0.1.0/examples/save_load_modify_pquery.py` & `kumo-ai-0.1.1/kumoai/examples/save_load_modify_pquery.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import os
 import sys
 
 from examples.orchestration import run_training_job
-from kumo.client import KumoClient
-from kumo.datamodel.json_serde import from_json, to_json
-from kumo.datamodel.pquery import Column, PQueryResource, SemanticType
+from kumoai.client import KumoClient
+from kumoai.datamodel.json_serde import from_json, to_json
+from kumoai.datamodel.pquery import Column, PQueryResource, SemanticType
 
 logging.basicConfig(format='%(asctime)s | %(levelname)s : %(message)s',
                     level=logging.INFO,
                     stream=sys.stdout)
 
 logger = logging.getLogger(__name__)
```

### Comparing `kumo-ai-0.1.0/kumo/client.py` & `kumo-ai-0.1.1/kumoai/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import os
 from http import HTTPStatus
 from typing import List, Optional
 
 from requests import Response, Session
 
-from kumo.datamodel.data_source import (ConnectorResponse,
+from kumoai.datamodel.data_source import (ConnectorResponse,
                                         SnowflakeConnectorArgs)
-from kumo.datamodel.jobs import (BatchPredictionJobResource,
+from kumoai.datamodel.jobs import (BatchPredictionJobResource,
                                  BatchPredictionOptions,
                                  BatchPredictionRequest, JobStatus,
                                  PredictionOutputConfig, TrainingJobResource)
-from kumo.datamodel.json_serde import from_json, to_json_dict
-from kumo.datamodel.pquery import (PQueryResource, S3SourceTableRequest,
+from kumoai.datamodel.json_serde import from_json, to_json_dict
+from kumoai.datamodel.pquery import (PQueryResource, S3SourceTableRequest,
                                    SnowflakeSourceTableRequest,
                                    SourceTableInfo)
 
 API_VERSION = 'v1'
 
 
 class KumoClient:
```

### Comparing `kumo-ai-0.1.0/kumo/datamodel/advanced_options.py` & `kumo-ai-0.1.1/kumoai/datamodel/advanced_options.py`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.0/kumo/datamodel/data_source.py` & `kumo-ai-0.1.1/kumoai/datamodel/data_source.py`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.0/kumo/datamodel/jobs.py` & `kumo-ai-0.1.1/kumoai/datamodel/jobs.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from enum import Enum
 from typing import List, Literal, Optional, Union
 
 from pydantic import Field
 from pydantic.dataclasses import dataclass
 from typing_extensions import Annotated
 
-from kumo.datamodel.advanced_options import AdvancedTrainingOptions
+from kumoai.datamodel.advanced_options import AdvancedTrainingOptions
 
 
 # Execution status of a Training or Batch Prediction job.
 class JobStatus(Enum):
     # Job has been submitted and is currently running.
     RUNNING = 'RUNNING'
```

### Comparing `kumo-ai-0.1.0/kumo/datamodel/json_serde.py` & `kumo-ai-0.1.1/kumoai/datamodel/json_serde.py`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.0/kumo/datamodel/pquery.py` & `kumo-ai-0.1.1/kumoai/datamodel/pquery.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dataclasses import field
 from enum import Enum
 from typing import Dict, List, Literal, Optional, Union
 
 from pydantic import Field, validator
 from pydantic.dataclasses import dataclass
 
-from kumo.datamodel.data_source import DataSourceType
+from kumoai.datamodel.data_source import DataSourceType
 
 TableName = str
 
 
 class SemanticType(str, Enum):
     numerical = 'numerical'
     categorical = 'categorical'
```

### Comparing `kumo-ai-0.1.0/precommit-pyrightconfig.json` & `kumo-ai-0.1.1/precommit-pyrightconfig.json`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.0/pyrightconfig.json` & `kumo-ai-0.1.1/pyrightconfig.json`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.0/setup.py` & `kumo-ai-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 DESCRIPTION = 'Kumo.ai Client SDK'
 LONG_DESCRIPTION = """
 SDK/API for Kumo.ai clients to allow programmatic access to Kumo.ai
 """
 
 install_requires = [
     "pydantic==1.10.4",
```

