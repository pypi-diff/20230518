# Comparing `tmp/azure-kusto-ingest-4.1.4.tar.gz` & `tmp/azure-kusto-ingest-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/azure-kusto-ingest-4.1.4.tar", last modified: Sun Apr 16 10:49:29 2023, max compression
+gzip compressed data, was "dist/azure-kusto-ingest-4.2.0.tar", last modified: Thu May 18 11:53:50 2023, max compression
```

## Comparing `azure-kusto-ingest-4.1.4.tar` & `azure-kusto-ingest-4.2.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:49:29.000000 azure-kusto-ingest-4.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-04-16 10:49:29.000000 azure-kusto-ingest-4.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-16 10:49:17.000000 azure-kusto-ingest-4.1.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:49:29.000000 azure-kusto-ingest-4.1.4/azure/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:49:29.000000 azure-kusto-ingest-4.1.4/azure/kusto/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-16 10:49:17.000000 azure-kusto-ingest-4.1.4/azure/kusto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:49:29.000000 azure-kusto-ingest-4.1.4/azure/kusto/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-16 10:49:17.000000 azure-kusto-ingest-4.1.4/azure/kusto/ingest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-16 10:49:17.000000 azure-kusto-ingest-4.1.4/azure/kusto/ingest/_ingest_telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-04-16 10:49:17.000000 azure-kusto-ingest-4.1.4/azure/kusto/ingest/_resource_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-04-16 10:49:17.000000 azure-kusto-ingest-4.1.4/azure/kusto/ingest/_status_q.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-16 10:49:17.000000 azure-kusto-ingest-4.1.4/azure/kusto/ingest/_stream_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-16 10:49:17.000000 azure-kusto-ingest-4.1.4/azure/kusto/ingest/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-04-16 10:49:17.000000 azure-kusto-ingest-4.1.4/azure/kusto/ingest/base_ingest_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9892 2023-04-16 10:49:17.000000 azure-kusto-ingest-4.1.4/azure/kusto/ingest/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-16 10:49:17.000000 azure-kusto-ingest-4.1.4/azure/kusto/ingest/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9977 2023-04-16 10:49:17.000000 azure-kusto-ingest-4.1.4/azure/kusto/ingest/ingest_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-04-16 10:49:17.000000 azure-kusto-ingest-4.1.4/azure/kusto/ingest/ingestion_blob_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-04-16 10:49:17.000000 azure-kusto-ingest-4.1.4/azure/kusto/ingest/ingestion_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-04-16 10:49:17.000000 azure-kusto-ingest-4.1.4/azure/kusto/ingest/managed_streaming_ingest_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-16 10:49:17.000000 azure-kusto-ingest-4.1.4/azure/kusto/ingest/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-04-16 10:49:17.000000 azure-kusto-ingest-4.1.4/azure/kusto/ingest/streaming_ingest_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:49:29.000000 azure-kusto-ingest-4.1.4/azure_kusto_ingest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-04-16 10:49:29.000000 azure-kusto-ingest-4.1.4/azure_kusto_ingest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-16 10:49:29.000000 azure-kusto-ingest-4.1.4/azure_kusto_ingest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 10:49:29.000000 azure-kusto-ingest-4.1.4/azure_kusto_ingest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-16 10:49:29.000000 azure-kusto-ingest-4.1.4/azure_kusto_ingest.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-16 10:49:29.000000 azure-kusto-ingest-4.1.4/azure_kusto_ingest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-16 10:49:29.000000 azure-kusto-ingest-4.1.4/azure_kusto_ingest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-16 10:49:29.000000 azure-kusto-ingest-4.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-16 10:49:17.000000 azure-kusto-ingest-4.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:53:50.000000 azure-kusto-ingest-4.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-05-18 11:53:50.000000 azure-kusto-ingest-4.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-18 11:53:40.000000 azure-kusto-ingest-4.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:53:50.000000 azure-kusto-ingest-4.2.0/azure/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:53:50.000000 azure-kusto-ingest-4.2.0/azure/kusto/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-18 11:53:40.000000 azure-kusto-ingest-4.2.0/azure/kusto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:53:50.000000 azure-kusto-ingest-4.2.0/azure/kusto/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-18 11:53:40.000000 azure-kusto-ingest-4.2.0/azure/kusto/ingest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-18 11:53:40.000000 azure-kusto-ingest-4.2.0/azure/kusto/ingest/_ingest_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-05-18 11:53:40.000000 azure-kusto-ingest-4.2.0/azure/kusto/ingest/_resource_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-05-18 11:53:40.000000 azure-kusto-ingest-4.2.0/azure/kusto/ingest/_status_q.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-18 11:53:40.000000 azure-kusto-ingest-4.2.0/azure/kusto/ingest/_stream_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-18 11:53:40.000000 azure-kusto-ingest-4.2.0/azure/kusto/ingest/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-05-18 11:53:40.000000 azure-kusto-ingest-4.2.0/azure/kusto/ingest/base_ingest_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9892 2023-05-18 11:53:40.000000 azure-kusto-ingest-4.2.0/azure/kusto/ingest/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-18 11:53:40.000000 azure-kusto-ingest-4.2.0/azure/kusto/ingest/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9899 2023-05-18 11:53:40.000000 azure-kusto-ingest-4.2.0/azure/kusto/ingest/ingest_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-18 11:53:40.000000 azure-kusto-ingest-4.2.0/azure/kusto/ingest/ingestion_blob_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-05-18 11:53:40.000000 azure-kusto-ingest-4.2.0/azure/kusto/ingest/ingestion_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-05-18 11:53:40.000000 azure-kusto-ingest-4.2.0/azure/kusto/ingest/managed_streaming_ingest_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-18 11:53:40.000000 azure-kusto-ingest-4.2.0/azure/kusto/ingest/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-05-18 11:53:40.000000 azure-kusto-ingest-4.2.0/azure/kusto/ingest/streaming_ingest_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:53:50.000000 azure-kusto-ingest-4.2.0/azure_kusto_ingest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-05-18 11:53:50.000000 azure-kusto-ingest-4.2.0/azure_kusto_ingest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-18 11:53:50.000000 azure-kusto-ingest-4.2.0/azure_kusto_ingest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 11:53:50.000000 azure-kusto-ingest-4.2.0/azure_kusto_ingest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 11:53:50.000000 azure-kusto-ingest-4.2.0/azure_kusto_ingest.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-18 11:53:50.000000 azure-kusto-ingest-4.2.0/azure_kusto_ingest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 11:53:50.000000 azure-kusto-ingest-4.2.0/azure_kusto_ingest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-18 11:53:50.000000 azure-kusto-ingest-4.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-18 11:53:40.000000 azure-kusto-ingest-4.2.0/setup.py
```

### Comparing `azure-kusto-ingest-4.1.4/PKG-INFO` & `azure-kusto-ingest-4.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-kusto-ingest
-Version: 4.1.4
+Version: 4.2.0
 Summary: Kusto Ingest Client
 Home-page: https://github.com/Azure/azure-kusto-python
 Author: Microsoft Corporation
 Author-email: kustalk@microsoft.com
 License: MIT
 Description: Microsoft Azure Kusto Ingest Library for Python
         ===============================================
```

### Comparing `azure-kusto-ingest-4.1.4/README.rst` & `azure-kusto-ingest-4.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.1.4/azure/kusto/ingest/__init__.py` & `azure-kusto-ingest-4.2.0/azure/kusto/ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.1.4/azure/kusto/ingest/_ingest_telemetry.py` & `azure-kusto-ingest-4.2.0/azure/kusto/ingest/_ingest_telemetry.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import uuid
 
-from azure.kusto.data._telemetry import KustoTracingAttributes
+from azure.kusto.data._telemetry import Span
 
 from .descriptors import DescriptorBase
 from .ingestion_properties import IngestionProperties
 
 
 class IngestTracingAttributes:
     """
@@ -12,13 +12,13 @@
     """
 
     _BLOB_QUEUE_NAME = "blob_queue_name"
     _SOURCE_ID = "source_id"
 
     @classmethod
     def set_ingest_descriptor_attributes(cls, descriptor: DescriptorBase, ingestion_properties: IngestionProperties) -> None:
-        KustoTracingAttributes.add_attributes(tracing_attributes={**ingestion_properties.get_tracing_attributes(), **descriptor.get_tracing_attributes()})
+        Span.add_attributes(tracing_attributes={**ingestion_properties.get_tracing_attributes(), **descriptor.get_tracing_attributes()})
 
     @classmethod
     def create_enqueue_request_attributes(cls, queue_name: str, source_id: uuid.UUID) -> dict:
         enqueue_request_attributes = {cls._BLOB_QUEUE_NAME: queue_name, cls._SOURCE_ID: str(source_id)}
         return enqueue_request_attributes
```

### Comparing `azure-kusto-ingest-4.1.4/azure/kusto/ingest/_resource_manager.py` & `azure-kusto-ingest-4.2.0/azure/kusto/ingest/_resource_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import List
 from urllib.parse import urlparse
 
 from tenacity import retry_if_exception_type, stop_after_attempt, Retrying, wait_random_exponential
 
 from azure.kusto.data import KustoClient
 from azure.kusto.data._models import KustoResultTable
-from azure.kusto.data._telemetry import KustoTracing, KustoTracingAttributes
+from azure.kusto.data._telemetry import MonitoredActivity, Span
 from azure.kusto.data.exceptions import KustoThrottlingError
 
 _SHOW_VERSION = ".show version"
 _SERVICE_TYPE_COLUMN_NAME = "ServiceType"
 
 
 class _ResourceUri:
@@ -89,20 +89,22 @@
             self._ingest_client_resources_last_update = datetime.utcnow()
 
     def _get_resource_by_name(self, table: KustoResultTable, resource_name: str):
         return [_ResourceUri(row["StorageRoot"]) for row in table if row["ResourceTypeName"] == resource_name]
 
     def _get_ingest_client_resources_from_service(self):
         # trace all calls to get ingestion resources
-        trace_get_ingestion_resources = KustoTracing.prepare_func_tracing(
-            self._kusto_client.execute,
-            name_of_span="_ResourceManager.get_ingestion_resources",
-            tracing_attributes=KustoTracingAttributes.create_cluster_attributes(self._kusto_client._kusto_cluster),
-        )
-        result = self._retryer(trace_get_ingestion_resources, "NetDefaultDB", ".get ingestion resources")
+        def invoker():
+            return MonitoredActivity.invoke(
+                lambda: self._kusto_client.execute("NetDefaultDB", ".get ingestion resources"),
+                name_of_span="_ResourceManager.get_ingestion_resources",
+                tracing_attributes=Span.create_cluster_attributes(self._kusto_client._kusto_cluster),
+            )
+
+        result = self._retryer(invoker)
         table = result.primary_results[0]
 
         secured_ready_for_aggregation_queues = self._get_resource_by_name(table, "SecuredReadyForAggregationQueue")
         failed_ingestions_queues = self._get_resource_by_name(table, "FailedIngestionsQueue")
         successful_ingestions_queues = self._get_resource_by_name(table, "SuccessfulIngestionsQueue")
         containers = self._get_resource_by_name(table, "TempStorage")
         status_tables = self._get_resource_by_name(table, "IngestionsStatusTable")
@@ -116,20 +118,22 @@
             or (self._authorization_context_last_update + self._refresh_period) <= datetime.utcnow()
         ):
             self._authorization_context = self._get_authorization_context_from_service()
             self._authorization_context_last_update = datetime.utcnow()
 
     def _get_authorization_context_from_service(self):
         # trace all calls to get identity token
-        trace_get_identity_token = KustoTracing.prepare_func_tracing(
-            self._kusto_client.execute,
-            name_of_span="_ResourceManager.get_identity_token",
-            tracing_attributes=KustoTracingAttributes.create_cluster_attributes(self._kusto_client._kusto_cluster),
-        )
-        result = self._retryer(trace_get_identity_token, "NetDefaultDB", ".get kusto identity token")
+        def invoker():
+            return MonitoredActivity.invoke(
+                lambda: self._kusto_client.execute("NetDefaultDB", ".get kusto identity token"),
+                name_of_span="_ResourceManager.get_identity_token",
+                tracing_attributes=Span.create_cluster_attributes(self._kusto_client._kusto_cluster),
+            )
+
+        result = self._retryer(invoker)
         return result.primary_results[0][0]["AuthorizationContext"]
 
     def get_ingestion_queues(self) -> List[_ResourceUri]:
         self._refresh_ingest_client_resources()
         return self._ingest_client_resources.secured_ready_for_aggregation_queues
 
     def get_failed_ingestions_queues(self) -> List[_ResourceUri]:
```

### Comparing `azure-kusto-ingest-4.1.4/azure/kusto/ingest/_status_q.py` & `azure-kusto-ingest-4.2.0/azure/kusto/ingest/_status_q.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.1.4/azure/kusto/ingest/_stream_extensions.py` & `azure-kusto-ingest-4.2.0/azure/kusto/ingest/_stream_extensions.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.1.4/azure/kusto/ingest/base_ingest_client.py` & `azure-kusto-ingest-4.2.0/azure/kusto/ingest/base_ingest_client.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.1.4/azure/kusto/ingest/descriptors.py` & `azure-kusto-ingest-4.2.0/azure/kusto/ingest/descriptors.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.1.4/azure/kusto/ingest/exceptions.py` & `azure-kusto-ingest-4.2.0/azure/kusto/ingest/exceptions.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.1.4/azure/kusto/ingest/ingest_client.py` & `azure-kusto-ingest-4.2.0/azure/kusto/ingest/ingest_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from urllib.parse import urlparse
 
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.tracing import SpanKind
 from azure.storage.queue import QueueServiceClient, TextBase64EncodePolicy
 
 from azure.kusto.data import KustoClient, KustoConnectionStringBuilder
-from azure.kusto.data._telemetry import KustoTracing
+from azure.kusto.data._telemetry import MonitoredActivity
 from azure.kusto.data.exceptions import KustoClosedError, KustoServiceError
 
 from ._ingest_telemetry import IngestTracingAttributes
 from ._resource_manager import _ResourceManager, _ResourceUri
 from .base_ingest_client import BaseIngestClient, IngestionResult, IngestionStatus
 from .descriptors import BlobDescriptor, FileDescriptor, StreamDescriptor
 from .exceptions import KustoInvalidEndpointError
@@ -128,22 +128,17 @@
         random_queue = random.choice(queues)
         with QueueServiceClient(random_queue.account_uri, proxies=self._proxy_dict) as queue_service:
             authorization_context = self._resource_manager.get_authorization_context()
             ingestion_blob_info = IngestionBlobInfo(blob_descriptor, ingestion_properties=ingestion_properties, auth_context=authorization_context)
             ingestion_blob_info_json = ingestion_blob_info.to_json()
             with queue_service.get_queue_client(queue=random_queue.object_name, message_encode_policy=TextBase64EncodePolicy()) as queue_client:
                 # trace enqueuing of blob for ingestion
+                invoker = lambda: queue_client.send_message(content=ingestion_blob_info_json, timeout=self._SERVICE_CLIENT_TIMEOUT_SECONDS)
                 enqueue_trace_attributes = IngestTracingAttributes.create_enqueue_request_attributes(queue_client.queue_name, blob_descriptor.source_id)
-                KustoTracing.call_func_tracing(
-                    queue_client.send_message,
-                    content=ingestion_blob_info_json,
-                    timeout=self._SERVICE_CLIENT_TIMEOUT_SECONDS,
-                    name_of_span="QueuedIngestClient.enqueue_request",
-                    tracing_attributes=enqueue_trace_attributes,
-                )
+                MonitoredActivity.invoke(invoker, name_of_span="QueuedIngestClient.enqueue_request", tracing_attributes=enqueue_trace_attributes)
 
         return IngestionResult(
             IngestionStatus.QUEUED, ingestion_properties.database, ingestion_properties.table, blob_descriptor.source_id, blob_descriptor.path
         )
 
     def _get_containers(self) -> List[_ResourceUri]:
         try:
```

### Comparing `azure-kusto-ingest-4.1.4/azure/kusto/ingest/ingestion_blob_info.py` & `azure-kusto-ingest-4.2.0/azure/kusto/ingest/ingestion_blob_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,14 +47,16 @@
             additional_properties["ingestionMappingReference"] = ingestion_properties.ingestion_mapping_reference
         if ingestion_properties.ingestion_mapping_type:
             additional_properties["ingestionMappingType"] = ingestion_properties.ingestion_mapping_type.value
         if ingestion_properties.validation_policy:
             additional_properties["ValidationPolicy"] = _convert_dict_to_json(ingestion_properties.validation_policy)
         if ingestion_properties.format:
             additional_properties["format"] = ingestion_properties.format.kusto_value
+        if ingestion_properties.ignore_first_record:
+            additional_properties["ignoreFirstRecord"] = ingestion_properties.ignore_first_record
 
         if additional_properties:
             self.properties["AdditionalProperties"] = additional_properties
 
     def to_json(self):
         """Converts this object to a json string"""
         return _convert_list_to_json(self.properties)
```

### Comparing `azure-kusto-ingest-4.1.4/azure/kusto/ingest/ingestion_properties.py` & `azure-kusto-ingest-4.2.0/azure/kusto/ingest/ingestion_properties.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.1.4/azure/kusto/ingest/managed_streaming_ingest_client.py` & `azure-kusto-ingest-4.2.0/azure/kusto/ingest/managed_streaming_ingest_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from tenacity import Retrying, _utils, stop_after_attempt, wait_random_exponential
 
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.tracing import SpanKind
 
 from azure.kusto.data import KustoConnectionStringBuilder
 from azure.kusto.data.exceptions import KustoApiError, KustoClosedError
-from azure.kusto.data._telemetry import KustoTracing
+from azure.kusto.data._telemetry import MonitoredActivity
 
 
 from . import BlobDescriptor, FileDescriptor, IngestionProperties, StreamDescriptor
 from ._ingest_telemetry import IngestTracingAttributes
 from ._stream_extensions import chain_streams, read_until_size_or_end
 from .base_ingest_client import BaseIngestClient, IngestionResult
 from .ingest_client import QueuedIngestClient
@@ -119,21 +119,19 @@
             for attempt in Retrying(
                 stop=stop_after_attempt(self._num_of_attempts), wait=wait_random_exponential(max=self._max_seconds_per_retry), reraise=True
             ):
                 with attempt:
                     stream.seek(0, SEEK_SET)
                     client_request_id = ManagedStreamingIngestClient._get_request_id(stream_descriptor.source_id, attempt.retry_state.attempt_number - 1)
                     # trace attempt to ingest from stream
-                    return KustoTracing.call_func_tracing(
-                        self.streaming_client._ingest_from_stream_with_client_request_id,
-                        stream_descriptor,
-                        ingestion_properties,
-                        client_request_id,
-                        name_of_span="ManagedStreamingIngestClient.ingest_from_stream_attempt",
+                    invoker = lambda: self.streaming_client._ingest_from_stream_with_client_request_id(
+                        stream_descriptor, ingestion_properties, client_request_id
                     )
+                    return MonitoredActivity.invoke(invoker, name_of_span="ManagedStreamingIngestClient.ingest_from_stream_attempt")
+
         except KustoApiError as ex:
             error = ex.get_api_error()
             if error.permanent:
                 raise
 
         return self.queued_client.ingest_from_stream(stream_descriptor, ingestion_properties)
```

### Comparing `azure-kusto-ingest-4.1.4/azure/kusto/ingest/status.py` & `azure-kusto-ingest-4.2.0/azure/kusto/ingest/status.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.1.4/azure/kusto/ingest/streaming_ingest_client.py` & `azure-kusto-ingest-4.2.0/azure/kusto/ingest/streaming_ingest_client.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.1.4/azure_kusto_ingest.egg-info/PKG-INFO` & `azure-kusto-ingest-4.2.0/azure_kusto_ingest.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-kusto-ingest
-Version: 4.1.4
+Version: 4.2.0
 Summary: Kusto Ingest Client
 Home-page: https://github.com/Azure/azure-kusto-python
 Author: Microsoft Corporation
 Author-email: kustalk@microsoft.com
 License: MIT
 Description: Microsoft Azure Kusto Ingest Library for Python
         ===============================================
```

### Comparing `azure-kusto-ingest-4.1.4/azure_kusto_ingest.egg-info/SOURCES.txt` & `azure-kusto-ingest-4.2.0/azure_kusto_ingest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.1.4/setup.py` & `azure-kusto-ingest-4.2.0/setup.py`

 * *Files identical despite different names*

