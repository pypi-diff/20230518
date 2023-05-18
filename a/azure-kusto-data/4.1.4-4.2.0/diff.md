# Comparing `tmp/azure-kusto-data-4.1.4.tar.gz` & `tmp/azure-kusto-data-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/azure-kusto-data-4.1.4.tar", last modified: Sun Apr 16 10:49:29 2023, max compression
+gzip compressed data, was "dist/azure-kusto-data-4.2.0.tar", last modified: Thu May 18 11:53:49 2023, max compression
```

## Comparing `azure-kusto-data-4.1.4.tar` & `azure-kusto-data-4.2.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:49:29.000000 azure-kusto-data-4.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-04-16 10:49:29.000000 azure-kusto-data-4.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:49:29.000000 azure-kusto-data-4.1.4/azure/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:49:29.000000 azure-kusto-data-4.1.4/azure/kusto/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:49:29.000000 azure-kusto-data-4.1.4/azure/kusto/data/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/_cloud_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/_string_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/_telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)    27136 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/_token_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:49:29.000000 azure-kusto-data-4.1.4/azure/kusto/data/aio/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/aio/_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/aio/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/aio/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/aio/streaming_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    14325 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/client_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/client_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/client_request_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/data_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    28429 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/kcsb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/kusto_trusted_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/security.py
--rw-r--r--   0 runner    (1001) docker     (123)    10738 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/streaming_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/azure/kusto/data/wellKnownKustoEndpoints.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:49:29.000000 azure-kusto-data-4.1.4/azure_kusto_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-04-16 10:49:29.000000 azure-kusto-data-4.1.4/azure_kusto_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-16 10:49:29.000000 azure-kusto-data-4.1.4/azure_kusto_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 10:49:29.000000 azure-kusto-data-4.1.4/azure_kusto_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-16 10:49:29.000000 azure-kusto-data-4.1.4/azure_kusto_data.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-16 10:49:29.000000 azure-kusto-data-4.1.4/azure_kusto_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-16 10:49:29.000000 azure-kusto-data-4.1.4/azure_kusto_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-16 10:49:29.000000 azure-kusto-data-4.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:49:29.000000 azure-kusto-data-4.1.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:49:29.000000 azure-kusto-data-4.1.4/tests/aio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/tests/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16579 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/tests/aio/test_async_token_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8606 2023-04-16 10:49:17.000000 azure-kusto-data-4.1.4/tests/aio/test_kusto_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:53:49.000000 azure-kusto-data-4.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-18 11:53:40.000000 azure-kusto-data-4.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-05-18 11:53:49.000000 azure-kusto-data-4.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-05-18 11:53:40.000000 azure-kusto-data-4.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:53:49.000000 azure-kusto-data-4.2.0/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-18 11:53:40.000000 azure-kusto-data-4.2.0/azure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:53:49.000000 azure-kusto-data-4.2.0/azure/kusto/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-18 11:53:40.000000 azure-kusto-data-4.2.0/azure/kusto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:53:49.000000 azure-kusto-data-4.2.0/azure/kusto/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-18 11:53:40.000000 azure-kusto-data-4.2.0/azure/kusto/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-05-18 11:53:40.000000 azure-kusto-data-4.2.0/azure/kusto/data/_cloud_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-18 11:53:40.000000 azure-kusto-data-4.2.0/azure/kusto/data/_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-18 11:53:40.000000 azure-kusto-data-4.2.0/azure/kusto/data/_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-05-18 11:53:40.000000 azure-kusto-data-4.2.0/azure/kusto/data/_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-18 11:53:40.000000 azure-kusto-data-4.2.0/azure/kusto/data/_string_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-05-18 11:53:40.000000 azure-kusto-data-4.2.0/azure/kusto/data/_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27011 2023-05-18 11:53:40.000000 azure-kusto-data-4.2.0/azure/kusto/data/_token_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-18 11:53:40.000000 azure-kusto-data-4.2.0/azure/kusto/data/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:53:49.000000 azure-kusto-data-4.2.0/azure/kusto/data/aio/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-18 11:53:40.000000 azure-kusto-data-4.2.0/azure/kusto/data/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-18 11:53:40.000000 azure-kusto-data-4.2.0/azure/kusto/data/aio/_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8369 2023-05-18 11:53:40.000000 azure-kusto-data-4.2.0/azure/kusto/data/aio/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-18 11:53:40.000000 azure-kusto-data-4.2.0/azure/kusto/data/aio/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-05-18 11:53:40.000000 azure-kusto-data-4.2.0/azure/kusto/data/aio/streaming_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14958 2023-05-18 11:53:40.000000 azure-kusto-data-4.2.0/azure/kusto/data/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-05-18 11:53:40.000000 azure-kusto-data-4.2.0/azure/kusto/data/client_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-18 11:53:40.000000 azure-kusto-data-4.2.0/azure/kusto/data/client_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-18 11:53:40.000000 azure-kusto-data-4.2.0/azure/kusto/data/client_request_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-18 11:53:40.000000 azure-kusto-data-4.2.0/azure/kusto/data/data_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-05-18 11:53:40.000000 azure-kusto-data-4.2.0/azure/kusto/data/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-18 11:53:40.000000 azure-kusto-data-4.2.0/azure/kusto/data/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30271 2023-05-18 11:53:40.000000 azure-kusto-data-4.2.0/azure/kusto/data/kcsb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-05-18 11:53:40.000000 azure-kusto-data-4.2.0/azure/kusto/data/kusto_trusted_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-05-18 11:53:40.000000 azure-kusto-data-4.2.0/azure/kusto/data/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-05-18 11:53:40.000000 azure-kusto-data-4.2.0/azure/kusto/data/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10738 2023-05-18 11:53:40.000000 azure-kusto-data-4.2.0/azure/kusto/data/streaming_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-05-18 11:53:40.000000 azure-kusto-data-4.2.0/azure/kusto/data/wellKnownKustoEndpoints.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:53:49.000000 azure-kusto-data-4.2.0/azure_kusto_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-05-18 11:53:49.000000 azure-kusto-data-4.2.0/azure_kusto_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-18 11:53:49.000000 azure-kusto-data-4.2.0/azure_kusto_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 11:53:49.000000 azure-kusto-data-4.2.0/azure_kusto_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 11:53:49.000000 azure-kusto-data-4.2.0/azure_kusto_data.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-18 11:53:49.000000 azure-kusto-data-4.2.0/azure_kusto_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-18 11:53:49.000000 azure-kusto-data-4.2.0/azure_kusto_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-18 11:53:49.000000 azure-kusto-data-4.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-18 11:53:40.000000 azure-kusto-data-4.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:53:49.000000 azure-kusto-data-4.2.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:53:49.000000 azure-kusto-data-4.2.0/tests/aio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 11:53:40.000000 azure-kusto-data-4.2.0/tests/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16659 2023-05-18 11:53:40.000000 azure-kusto-data-4.2.0/tests/aio/test_async_token_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8606 2023-05-18 11:53:40.000000 azure-kusto-data-4.2.0/tests/aio/test_kusto_client.py
```

### Comparing `azure-kusto-data-4.1.4/PKG-INFO` & `azure-kusto-data-4.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-kusto-data
-Version: 4.1.4
+Version: 4.2.0
 Summary: Kusto Data Client
 Home-page: https://github.com/Azure/azure-kusto-python
 Author: Microsoft Corporation
 Author-email: kustalk@microsoft.com
 License: MIT
 Description: Microsoft Azure Kusto Library for Python
         ========================================
```

### Comparing `azure-kusto-data-4.1.4/README.rst` & `azure-kusto-data-4.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.4/azure/kusto/data/_cloud_settings.py` & `azure-kusto-data-4.2.0/azure/kusto/data/_cloud_settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from urllib.parse import urljoin
 
 import requests
 
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.tracing import SpanKind
 
-from ._telemetry import KustoTracingAttributes, KustoTracing
+from ._telemetry import Span, MonitoredActivity
 from .exceptions import KustoServiceError
 
 METADATA_ENDPOINT = "v1/rest/auth/metadata"
 
 DEFAULT_AUTH_ENV_VAR_NAME = "AadAuthorityUri"
 DEFAULT_KUSTO_CLIENT_APP_ID = "db662dc1-0cfe-4e1c-a843-19a68e65be58"
 DEFAULT_PUBLIC_LOGIN_URL = "https://login.microsoftonline.com"
@@ -71,30 +71,32 @@
         kusto_service_resource_id=DEFAULT_KUSTO_SERVICE_RESOURCE_ID,
         first_party_authority_url=DEFAULT_FIRST_PARTY_AUTHORITY_URL,
     )
 
     @classmethod
     @distributed_trace(name_of_span="CloudSettings.get_cloud_info", kind=SpanKind.CLIENT)
     def get_cloud_info_for_cluster(cls, kusto_uri: str, proxies: Optional[Dict[str, str]] = None) -> CloudInfo:
+        kusto_uri = cls._normalize_uri(kusto_uri)
+
         # tracing attributes for cloud info
-        KustoTracingAttributes.set_cloud_info_attributes(kusto_uri)
+        Span.set_cloud_info_attributes(kusto_uri)
 
         if kusto_uri in cls._cloud_cache:  # Double-checked locking to avoid unnecessary lock access
             return cls._cloud_cache[kusto_uri]
 
         with cls._cloud_cache_lock:
             if kusto_uri in cls._cloud_cache:
                 return cls._cloud_cache[kusto_uri]
             url = urljoin(kusto_uri, METADATA_ENDPOINT)
 
             # trace http get call for result
-            http_trace_attributes = KustoTracingAttributes.create_http_attributes(url=url, method="GET")
-
-            result = KustoTracing.call_func_tracing(
-                requests.get, url, proxies=proxies, allow_redirects=False, name_of_span="CloudSettings.http_get", tracing_attributes=http_trace_attributes
+            result = MonitoredActivity.invoke(
+                lambda: requests.get(url, proxies=proxies, allow_redirects=False),
+                name_of_span="CloudSettings.http_get",
+                tracing_attributes=Span.create_http_attributes(url=url, method="GET"),
             )
 
             if result.status_code == 200:
                 content = result.json()
                 if content is None or content == {}:
                     raise KustoServiceError("Kusto returned an invalid cloud metadata response", result)
                 root = content["AzureAD"]
@@ -111,7 +113,18 @@
                     cls._cloud_cache[kusto_uri] = cls.DEFAULT_CLOUD
             elif result.status_code == 404:
                 # For now as long not all proxies implement the metadata endpoint, if no endpoint exists return public cloud data
                 cls._cloud_cache[kusto_uri] = cls.DEFAULT_CLOUD
             else:
                 raise KustoServiceError("Kusto returned an invalid cloud metadata response", result)
             return cls._cloud_cache[kusto_uri]
+
+    @classmethod
+    def add_to_cache(cls, url: str, cloud_info: CloudInfo):
+        with cls._cloud_cache_lock:
+            cls._cloud_cache[cls._normalize_uri(url)] = cloud_info
+
+    @classmethod
+    def _normalize_uri(cls, kusto_uri):
+        if not kusto_uri.endswith("/"):
+            kusto_uri += "/"
+        return kusto_uri
```

### Comparing `azure-kusto-data-4.1.4/azure/kusto/data/_converters.py` & `azure-kusto-data-4.2.0/azure/kusto/data/_converters.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.4/azure/kusto/data/_models.py` & `azure-kusto-data-4.2.0/azure/kusto/data/_models.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.4/azure/kusto/data/_telemetry.py` & `azure-kusto-data-4.2.0/azure/kusto/data/_telemetry.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from typing import Callable, Optional
+from typing import Callable, Optional, TypeVar
 
 from azure.core.settings import settings
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.tracing import SpanKind
 
 from .client_request_properties import ClientRequestProperties
 
 
-class KustoTracingAttributes:
+class Span:
     """
     Additional ADX attributes for telemetry spans
     """
 
     _KUSTO_CLUSTER = "kusto_cluster"
     _DATABASE = "database"
     _TABLE = "table"
@@ -93,62 +93,35 @@
 
     @classmethod
     def create_cluster_attributes(cls, cluster_uri: str) -> dict:
         cluster_attributes = {cls._KUSTO_CLUSTER: cluster_uri}
         return cluster_attributes
 
 
-class KustoTracing:
-    @staticmethod
-    def call_func_tracing(func: Callable, *args, **kwargs):
-        """
-        Prepares function for tracing and calls it
-        :param func: function to trace
-        :type func: Callable
-        :key str name_of_span: name of the trace span
-        :key dict tracing_attributes: key/value dictionary of attributes to include in span of trace
-        :key str kind: the type of span
-        :param kwargs: function arguments
-        """
-        name_of_span: str = kwargs.pop("name_of_span", None)
-        tracing_attributes: dict = kwargs.pop("tracing_attributes", {})
-        kind: str = kwargs.pop("kind", SpanKind.CLIENT)
+class MonitoredActivity:
+    """
+    Invoker class for telemetry
+    """
 
-        kusto_trace: Callable = distributed_trace(name_of_span=name_of_span, tracing_attributes=tracing_attributes, kind=kind)
-        kusto_func: Callable = kusto_trace(func)
-        return kusto_func(*args, **kwargs)
+    T = TypeVar("T")
 
     @staticmethod
-    async def call_func_tracing_async(func: Callable, *args, **kwargs):
+    def invoke(invoker: Callable[[], T], name_of_span: str = None, tracing_attributes=None, kind: str = SpanKind.INTERNAL) -> T:
         """
-        Prepares function for tracing and calls it
-        :param func: function to trace
-        :type func: Callable
-        :key str name_of_span: name of the trace span
-        :key dict tracing_attributes: key/value dictionary of attributes to include in span of trace
-        :key str kind: the type of span
-        :param kwargs: function arguments
+        Runs the span on given function
         """
-        name_of_span: str = kwargs.pop("name_of_span", None)
-        tracing_attributes: dict = kwargs.pop("tracing_attributes", {})
-        kind: str = kwargs.pop("kind", SpanKind.CLIENT)
-
-        kusto_trace: Callable = distributed_trace_async(name_of_span=name_of_span, tracing_attributes=tracing_attributes, kind=kind)
-        kusto_func: Callable = kusto_trace(func)
-        return await kusto_func(*args, **kwargs)
+        if tracing_attributes is None:
+            tracing_attributes = {}
+        span_shell: Callable = distributed_trace(name_of_span=name_of_span, tracing_attributes=tracing_attributes, kind=kind)
+        span = span_shell(invoker)
+        return span()
 
     @staticmethod
-    def prepare_func_tracing(func: Callable, **kwargs):
+    async def invoke_async(invoker: Callable[[], T], name_of_span: str = None, tracing_attributes=None, kind: str = SpanKind.INTERNAL) -> T:
         """
-        Prepares function for tracing
-        :param func: function to trace
-        :type func: Callable
-        :key str name_of_span: name of the trace span
-        :key dict tracing_attributes: key/value dictionary of attributes to include in span of trace
-        :key str kind: the type of span
+        Runs a span on given function
         """
-        name_of_span: str = kwargs.pop("name_of_span", None)
-        tracing_attributes: dict = kwargs.pop("tracing_attributes", {})
-        kind: str = kwargs.pop("kind", SpanKind.CLIENT)
-
-        kusto_trace: Callable = distributed_trace(name_of_span=name_of_span, tracing_attributes=tracing_attributes, kind=kind)
-        return kusto_trace(func)
+        if tracing_attributes is None:
+            tracing_attributes = {}
+        span_shell: Callable = distributed_trace_async(name_of_span=name_of_span, tracing_attributes=tracing_attributes, kind=kind)
+        span = span_shell(invoker)
+        return await span()
```

### Comparing `azure-kusto-data-4.1.4/azure/kusto/data/_token_providers.py` & `azure-kusto-data-4.2.0/azure/kusto/data/_token_providers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License
 import abc
 import asyncio
+import inspect
 import time
-import webbrowser
+from datetime import datetime
 from threading import Lock
 from typing import Callable, Coroutine, List, Optional, Any
 
 from azure.core.exceptions import ClientAuthenticationError
+from azure.core.tracing import SpanKind
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.tracing.decorator_async import distributed_trace_async
-from azure.core.tracing import SpanKind
-from azure.identity import AzureCliCredential, ManagedIdentityCredential
+from azure.identity import AzureCliCredential, ManagedIdentityCredential, DeviceCodeCredential
 from msal import ConfidentialClientApplication, PublicClientApplication
 
 from ._cloud_settings import CloudInfo, CloudSettings
-from ._telemetry import KustoTracing
+from ._telemetry import MonitoredActivity
 from .exceptions import KustoAioSyntaxError, KustoAsyncUsageError, KustoClientError
 
+DeviceCallbackType = Callable[[str, str, datetime], None]
+"""A callback enabling control of how authentication
+        instructions are presented. Must accept arguments (``verification_uri``, ``user_code``, ``expires_on``):
+
+        - ``verification_uri`` (str) the URL the user must visit
+        - ``user_code`` (str) the code the user must enter there
+        - ``expires_on`` (datetime.datetime) the UTC time at which the code will expire
+        If this argument isn't provided, the credential will print instructions to stdout."""
+
 try:
     from asgiref.sync import sync_to_async
 except ImportError:
 
     def sync_to_async(f):
         raise KustoAioSyntaxError()
 
@@ -139,18 +149,15 @@
             if self.is_async:
                 raise KustoAsyncUsageError("get_token", self.is_async)
             self._init_once()
 
             token = self._get_token_from_cache_impl()
             if token is None:
                 with self._lock:
-                    token = KustoTracing.call_func_tracing(
-                        self._get_token_impl, name_of_span=f"{self.name()}.get_token_impl", tracing_attributes=self.context()
-                    )
-
+                    token = MonitoredActivity.invoke(self._get_token_impl, name_of_span=f"{self.name()}.get_token_impl", tracing_attributes=self.context())
             return self._valid_token_or_throw(token)
 
         return _get_token()
 
     def context(self) -> dict:
         if self.is_async:
             raise KustoAsyncUsageError("context", self.is_async)
@@ -176,15 +183,15 @@
 
             await self._init_once_async()
 
             token = self._get_token_from_cache_impl()
 
             if token is None:
                 async with self._async_lock:
-                    token = await KustoTracing.call_func_tracing_async(
+                    token = await MonitoredActivity.invoke_async(
                         self._get_token_impl_async, name_of_span=f"{self.name()}.get_token_impl_async", tracing_attributes=context
                     )
 
             return self._valid_token_or_throw(token)
 
         return await _get_token_async()
 
@@ -481,63 +488,14 @@
             if len(accounts) > 0:
                 account = accounts[0]
 
         token = self._msal_client.acquire_token_silent(scopes=self._scopes, account=account)
         return self._valid_token_or_none(token)
 
 
-class DeviceLoginTokenProvider(CloudInfoTokenProvider):
-    """Acquire a token from MSAL with Device Login flow"""
-
-    def __init__(self, kusto_uri: str, authority_id: str, device_code_callback=None, is_async: bool = False):
-        super().__init__(kusto_uri, is_async)
-        self._msal_client = None
-        self._auth = authority_id
-        self._account = None
-        self._device_code_callback = device_code_callback
-
-    @staticmethod
-    def name() -> str:
-        return "DeviceLoginTokenProvider"
-
-    def _context_impl(self) -> dict:
-        return {"authority": self._cloud_info.authority_uri(self._auth), "client_id": self._cloud_info.kusto_client_app_id}
-
-    def _init_impl(self):
-        self._msal_client = PublicClientApplication(
-            client_id=self._cloud_info.kusto_client_app_id, authority=self._cloud_info.authority_uri(self._auth), proxies=self._proxy_dict
-        )
-
-    def _get_token_impl(self) -> Optional[dict]:
-        flow = self._msal_client.initiate_device_flow(scopes=self._scopes)
-        try:
-            if self._device_code_callback:
-                self._device_code_callback(flow[TokenConstants.MSAL_DEVICE_MSG])
-            else:
-                print(flow[TokenConstants.MSAL_DEVICE_MSG])
-
-            webbrowser.open(flow[TokenConstants.MSAL_DEVICE_URI])
-        except KeyError:
-            raise KustoClientError("Failed to initiate device code flow")
-
-        token = self._msal_client.acquire_token_by_device_flow(flow)
-
-        # Keep the account for silent login
-        if self._valid_token_or_none(token) is not None:
-            accounts = self._msal_client.get_accounts()
-            if len(accounts) == 1:
-                self._account = accounts[0]
-
-        return self._valid_token_or_throw(token)
-
-    def _get_token_from_cache_impl(self) -> dict:
-        token = self._msal_client.acquire_token_silent(scopes=self._scopes, account=self._account)
-        return self._valid_token_or_none(token)
-
-
 class InteractiveLoginTokenProvider(CloudInfoTokenProvider):
     """Acquire a token from MSAL with Device Login flow"""
 
     def __init__(
         self,
         kusto_uri: str,
         authority_id: str,
@@ -690,21 +648,54 @@
             self.credential = self.credential_from_login_endpoint(self._cloud_info.login_endpoint)
 
     def _get_token_impl(self) -> Optional[dict]:
         t = self.credential.get_token(self._scopes[0])
         return {TokenConstants.MSAL_TOKEN_TYPE: TokenConstants.BEARER_TYPE, TokenConstants.MSAL_ACCESS_TOKEN: t.token}
 
     async def _get_token_impl_async(self) -> Optional[dict]:
-        t = await self.credential.get_token(self._scopes[0])
+        # check if get_token is async
+        if inspect.iscoroutinefunction(self.credential.get_token):
+            t = await self.credential.get_token(self._scopes[0])
+        else:
+            t = await sync_to_async(self.credential.get_token)(self._scopes[0])
         return {TokenConstants.MSAL_TOKEN_TYPE: TokenConstants.BEARER_TYPE, TokenConstants.MSAL_ACCESS_TOKEN: t.token}
 
     def _get_token_from_cache_impl(self) -> Optional[dict]:
         return None
 
     def close(self):
         if self.credential is not None:
             if self.is_async:
                 asyncio.get_event_loop().run_in_executor(None, self.credential.close())
             else:
                 self.credential.close()
             self.credential = None
             self.credential_from_login_endpoint = None
+
+
+class DeviceLoginTokenProvider(AzureIdentityTokenCredentialProvider):
+    """Acquire a token from MSAL with Device Login flow"""
+
+    def __init__(self, kusto_uri: str, authority_id: str, device_code_callback: DeviceCallbackType = None, is_async: bool = False):
+        self._msal_client = None
+        self._auth = authority_id
+        self._account = None
+        self._device_code_callback = device_code_callback
+
+        def credential_from_login_endpoint(endpoint: str):
+            cred = DeviceCodeCredential(
+                authority=endpoint,
+                tenant_id=self._auth,
+                client_id=self._cloud_info.kusto_client_app_id,
+                prompt_callback=self._device_code_callback,
+            )
+
+            return cred
+
+        super().__init__(kusto_uri, is_async, credential_from_login_endpoint=credential_from_login_endpoint)
+
+    @staticmethod
+    def name() -> str:
+        return "DeviceLoginTokenProvider"
+
+    def _context_impl(self) -> dict:
+        return {"authority": self._cloud_info.authority_uri(self._auth), "client_id": self._cloud_info.kusto_client_app_id}
```

### Comparing `azure-kusto-data-4.1.4/azure/kusto/data/aio/_models.py` & `azure-kusto-data-4.2.0/azure/kusto/data/aio/_models.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.4/azure/kusto/data/aio/client.py` & `azure-kusto-data-4.2.0/azure/kusto/data/aio/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Optional, Union
 
 from azure.core.tracing import SpanKind
 from azure.core.tracing.decorator_async import distributed_trace_async
 
 from .response import KustoStreamingResponseDataSet
 from .._decorators import aio_documented_by, documented_by
-from .._telemetry import KustoTracing, KustoTracingAttributes
+from .._telemetry import MonitoredActivity, Span
 from ..aio.streaming_response import JsonTokenReader, StreamingDataSetEnumerator
 from ..client import KustoClient as KustoClientSync
 from ..client_base import ExecuteRequestParams, _KustoClientBase
 from ..client_request_properties import ClientRequestProperties
 from ..data_format import DataFormat
 from ..exceptions import KustoAioSyntaxError, KustoClosedError
 from ..kcsb import KustoConnectionStringBuilder
@@ -39,76 +39,88 @@
             await self._session.close()
         super().close()
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         await self.close()
 
     @aio_documented_by(KustoClientSync.execute)
-    async def execute(self, database: str, query: str, properties: ClientRequestProperties = None) -> KustoResponseDataSet:
+    async def execute(self, database: Optional[str], query: str, properties: ClientRequestProperties = None) -> KustoResponseDataSet:
         query = query.strip()
         if query.startswith("."):
             return await self.execute_mgmt(database, query, properties)
         return await self.execute_query(database, query, properties)
 
     @distributed_trace_async(name_of_span="KustoClient.query_cmd", kind=SpanKind.CLIENT)
     @aio_documented_by(KustoClientSync.execute_query)
     async def execute_query(self, database: str, query: str, properties: ClientRequestProperties = None) -> KustoResponseDataSet:
-        KustoTracingAttributes.set_query_attributes(self._kusto_cluster, database, properties)
+        database = self._get_database_or_default(database)
+        Span.set_query_attributes(self._kusto_cluster, database, properties)
 
         return await self._execute(self._query_endpoint, database, query, None, KustoClient._query_default_timeout, properties)
 
     @distributed_trace_async(name_of_span="KustoClient.control_cmd", kind=SpanKind.CLIENT)
     @aio_documented_by(KustoClientSync.execute_mgmt)
     async def execute_mgmt(self, database: str, query: str, properties: ClientRequestProperties = None) -> KustoResponseDataSet:
-        KustoTracingAttributes.set_query_attributes(self._kusto_cluster, database, properties)
+        database = self._get_database_or_default(database)
+        Span.set_query_attributes(self._kusto_cluster, database, properties)
 
         return await self._execute(self._mgmt_endpoint, database, query, None, KustoClient._mgmt_default_timeout, properties)
 
     @distributed_trace_async(name_of_span="KustoClient.streaming_ingest", kind=SpanKind.CLIENT)
     @aio_documented_by(KustoClientSync.execute_streaming_ingest)
     async def execute_streaming_ingest(
         self,
-        database: str,
+        database: Optional[str],
         table: str,
         stream: io.IOBase,
         stream_format: Union[DataFormat, str],
         properties: ClientRequestProperties = None,
         mapping_name: str = None,
     ):
-        KustoTracingAttributes.set_streaming_ingest_attributes(self._kusto_cluster, database, table, properties)
+        database = self._get_database_or_default(database)
+        Span.set_streaming_ingest_attributes(self._kusto_cluster, database, table, properties)
 
         stream_format = stream_format.kusto_value if isinstance(stream_format, DataFormat) else DataFormat[stream_format.upper()].kusto_value
         endpoint = self._streaming_ingest_endpoint + database + "/" + table + "?streamFormat=" + stream_format
         if mapping_name is not None:
             endpoint = endpoint + "&mappingName=" + mapping_name
 
         await self._execute(endpoint, database, None, stream, self._streaming_ingest_default_timeout, properties)
 
     @aio_documented_by(KustoClientSync._execute_streaming_query_parsed)
     async def _execute_streaming_query_parsed(
-        self, database: str, query: str, timeout: timedelta = _KustoClientBase._query_default_timeout, properties: Optional[ClientRequestProperties] = None
+        self,
+        database: Optional[str],
+        query: str,
+        timeout: timedelta = _KustoClientBase._query_default_timeout,
+        properties: Optional[ClientRequestProperties] = None,
     ) -> StreamingDataSetEnumerator:
         response = await self._execute(self._query_endpoint, database, query, None, timeout, properties, stream_response=True)
         return StreamingDataSetEnumerator(JsonTokenReader(response.content))
 
     @distributed_trace_async(name_of_span="KustoClient.streaming_query", kind=SpanKind.CLIENT)
     @aio_documented_by(KustoClientSync.execute_streaming_query)
     async def execute_streaming_query(
-        self, database: str, query: str, timeout: timedelta = _KustoClientBase._query_default_timeout, properties: Optional[ClientRequestProperties] = None
+        self,
+        database: Optional[str],
+        query: str,
+        timeout: timedelta = _KustoClientBase._query_default_timeout,
+        properties: Optional[ClientRequestProperties] = None,
     ) -> KustoStreamingResponseDataSet:
-        KustoTracingAttributes.set_query_attributes(self._kusto_cluster, database, properties)
+        database = self._get_database_or_default(database)
+        Span.set_query_attributes(self._kusto_cluster, database, properties)
 
         response = await self._execute_streaming_query_parsed(database, query, timeout, properties)
         return KustoStreamingResponseDataSet(response)
 
     @aio_documented_by(KustoClientSync._execute)
     async def _execute(
         self,
         endpoint: str,
-        database: str,
+        database: Optional[str],
         query: Optional[str],
         payload: Optional[io.IOBase],
         timeout: timedelta,
         properties: ClientRequestProperties = None,
         stream_response: bool = False,
     ) -> Union[KustoResponseDataSet, ClientResponse]:
         """Executes given query against this client"""
@@ -128,26 +140,19 @@
         )
         json_payload = request_params.json_payload
         request_headers = request_params.request_headers
         timeout = request_params.timeout
         if self._aad_helper:
             request_headers["Authorization"] = await self._aad_helper.acquire_authorization_header_async()
 
-        http_trace_attributes = KustoTracingAttributes.create_http_attributes(url=endpoint, method="POST", headers=request_headers)
-        response = await KustoTracing.call_func_tracing_async(
-            self._session.post,
-            endpoint,
-            headers=request_headers,
-            json=json_payload,
-            data=payload,
-            timeout=timeout.seconds,
-            proxy=self._proxy_url,
-            name_of_span="KustoClient.http_post",
-            tracing_attributes=http_trace_attributes,
-            allow_redirects=False,
+        invoker = lambda: self._session.post(
+            endpoint, headers=request_headers, json=json_payload, data=payload, timeout=timeout.seconds, proxy=self._proxy_url, allow_redirects=False
+        )
+        response = await MonitoredActivity.invoke_async(
+            invoker, name_of_span="KustoClient.http_post", tracing_attributes=Span.create_http_attributes("POST", endpoint, request_headers)
         )
 
         if stream_response:
             try:
                 response.raise_for_status()
                 if 300 <= response.status < 400:
                     raise Exception("Unexpected redirection, got status code: " + str(response.status))
@@ -172,9 +177,8 @@
                 response.raise_for_status()
             except Exception as e:
                 try:
                     response_text = await response.text()
                 except Exception:
                     response_text = None
                 raise self._handle_http_error(e, endpoint, payload, response, response.status, response_json, response_text)
-
-            return KustoTracing.call_func_tracing(self._kusto_parse_by_endpoint, endpoint, response_json, name_of_span="KustoClient.processing_response")
+            return MonitoredActivity.invoke(lambda: self._kusto_parse_by_endpoint(endpoint, response_json), name_of_span="KustoClient.processing_response")
```

### Comparing `azure-kusto-data-4.1.4/azure/kusto/data/aio/response.py` & `azure-kusto-data-4.2.0/azure/kusto/data/aio/response.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.4/azure/kusto/data/aio/streaming_response.py` & `azure-kusto-data-4.2.0/azure/kusto/data/aio/streaming_response.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.4/azure/kusto/data/client.py` & `azure-kusto-data-4.2.0/azure/kusto/data/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import requests.adapters
 from requests import Response
 from urllib3.connection import HTTPConnection
 
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.tracing import SpanKind
 
-from azure.kusto.data._telemetry import KustoTracingAttributes, KustoTracing
+from azure.kusto.data._telemetry import Span, MonitoredActivity
 
 from .client_base import ExecuteRequestParams, _KustoClientBase
 from .client_request_properties import ClientRequestProperties
 from .data_format import DataFormat
 from .exceptions import KustoClosedError
 from .kcsb import KustoConnectionStringBuilder
 from .response import KustoResponseDataSet, KustoStreamingResponseDataSet
@@ -141,118 +141,129 @@
             ]
         elif sys.platform == "darwin" and hasattr(socket, "SOL_SOCKET") and hasattr(socket, "SO_KEEPALIVE") and hasattr(socket, "IPPROTO_TCP"):
             TCP_KEEPALIVE = 0x10
             return [(socket.SOL_SOCKET, socket.SO_KEEPALIVE, 1), (socket.IPPROTO_TCP, TCP_KEEPALIVE, INTERVAL_SECONDS)]
         else:
             return []
 
-    def execute(self, database: str, query: str, properties: Optional[ClientRequestProperties] = None) -> KustoResponseDataSet:
+    def execute(self, database: Optional[str], query: str, properties: Optional[ClientRequestProperties] = None) -> KustoResponseDataSet:
         """
         Executes a query or management command.
-        :param str database: Database against query will be executed.
+        :param Optional[str] database: Database against query will be executed. If not provided, will default to the "Initial Catalog" value in the connection string
         :param str query: Query to be executed.
         :param azure.kusto.data.ClientRequestProperties properties: Optional additional properties.
         :return: Kusto response data set.
         :rtype: azure.kusto.data.response.KustoResponseDataSet
         """
         query = query.strip()
         if query.startswith("."):
             return self.execute_mgmt(database, query, properties)
         return self.execute_query(database, query, properties)
 
     @distributed_trace(name_of_span="KustoClient.query_cmd", kind=SpanKind.CLIENT)
-    def execute_query(self, database: str, query: str, properties: Optional[ClientRequestProperties] = None) -> KustoResponseDataSet:
+    def execute_query(self, database: Optional[str], query: str, properties: Optional[ClientRequestProperties] = None) -> KustoResponseDataSet:
         """
         Execute a KQL query.
         To learn more about KQL go to https://docs.microsoft.com/en-us/azure/kusto/query/
-        :param str database: Database against query will be executed.
+        :param Optional[str] database: Database against query will be executed. If not provided, will default to the "Initial Catalog" value in the connection string
         :param str query: Query to be executed.
         :param azure.kusto.data.ClientRequestProperties properties: Optional additional properties.
         :return: Kusto response data set.
         :rtype: azure.kusto.data.response.KustoResponseDataSet
         """
-        KustoTracingAttributes.set_query_attributes(self._kusto_cluster, database, properties)
+        database = self._get_database_or_default(database)
+        Span.set_query_attributes(self._kusto_cluster, database, properties)
 
         return self._execute(self._query_endpoint, database, query, None, self._query_default_timeout, properties)
 
     @distributed_trace(name_of_span="KustoClient.control_cmd", kind=SpanKind.CLIENT)
-    def execute_mgmt(self, database: str, query: str, properties: Optional[ClientRequestProperties] = None) -> KustoResponseDataSet:
+    def execute_mgmt(self, database: Optional[str], query: str, properties: Optional[ClientRequestProperties] = None) -> KustoResponseDataSet:
         """
         Execute a KQL control command.
         To learn more about KQL control commands go to  https://docs.microsoft.com/en-us/azure/kusto/management/
-        :param str database: Database against query will be executed.
+        :param Optional[str] database: Database against query will be executed. If not provided, will default to the "Initial Catalog" value in the connection string
         :param str query: Query to be executed.
         :param azure.kusto.data.ClientRequestProperties properties: Optional additional properties.
         :return: Kusto response data set.
         :rtype: azure.kusto.data.response.KustoResponseDataSet
         """
-        KustoTracingAttributes.set_query_attributes(self._kusto_cluster, database, properties)
+        database = self._get_database_or_default(database)
+        Span.set_query_attributes(self._kusto_cluster, database, properties)
 
         return self._execute(self._mgmt_endpoint, database, query, None, self._mgmt_default_timeout, properties)
 
     @distributed_trace(name_of_span="KustoClient.streaming_ingest", kind=SpanKind.CLIENT)
     def execute_streaming_ingest(
         self,
-        database: str,
+        database: Optional[str],
         table: str,
         stream: IO[AnyStr],
         stream_format: Union[DataFormat, str],
         properties: Optional[ClientRequestProperties] = None,
         mapping_name: str = None,
     ):
         """
         Execute streaming ingest against this client
         If the Kusto service is not configured to allow streaming ingestion, this may raise an error
         To learn more about streaming ingestion go to:
         https://docs.microsoft.com/en-us/azure/data-explorer/ingest-data-streaming
-        :param str database: Target database.
+        :param Optional[str] database: Target database. If not provided, will default to the "Initial Catalog" value in the connection string
         :param str table: Target table.
         :param io.BaseIO stream: stream object which contains the data to ingest.
         :param DataFormat stream_format: Format of the data in the stream.
         :param ClientRequestProperties properties: additional request properties.
         :param str mapping_name: Pre-defined mapping of the table. Required when stream_format is json/avro.
         """
-        KustoTracingAttributes.set_streaming_ingest_attributes(self._kusto_cluster, database, table, properties)
+        database = self._get_database_or_default(database)
+        Span.set_streaming_ingest_attributes(self._kusto_cluster, database, table, properties)
 
         stream_format = stream_format.kusto_value if isinstance(stream_format, DataFormat) else DataFormat[stream_format.upper()].kusto_value
         endpoint = self._streaming_ingest_endpoint + database + "/" + table + "?streamFormat=" + stream_format
         if mapping_name is not None:
             endpoint = endpoint + "&mappingName=" + mapping_name
 
         self._execute(endpoint, database, None, stream, self._streaming_ingest_default_timeout, properties)
 
     def _execute_streaming_query_parsed(
-        self, database: str, query: str, timeout: timedelta = _KustoClientBase._query_default_timeout, properties: Optional[ClientRequestProperties] = None
+        self,
+        database: Optional[str],
+        query: str,
+        timeout: timedelta = _KustoClientBase._query_default_timeout,
+        properties: Optional[ClientRequestProperties] = None,
     ) -> StreamingDataSetEnumerator:
         response = self._execute(self._query_endpoint, database, query, None, timeout, properties, stream_response=True)
         response.raw.decode_content = True
         return StreamingDataSetEnumerator(JsonTokenReader(response.raw))
 
     @distributed_trace(name_of_span="KustoClient.streaming_query", kind=SpanKind.CLIENT)
     def execute_streaming_query(
-        self, database: str, query: str, timeout: timedelta = _KustoClientBase._query_default_timeout, properties: Optional[ClientRequestProperties] = None
+        self,
+        database: Optional[str],
+        query: str,
+        timeout: timedelta = _KustoClientBase._query_default_timeout,
+        properties: Optional[ClientRequestProperties] = None,
     ) -> KustoStreamingResponseDataSet:
         """
         Execute a KQL query without reading it all to memory.
         The resulting KustoStreamingResponseDataSet will stream one table at a time, and the rows can be retrieved sequentially.
 
-        :param str database: Database against query will be executed.
+        :param Optional[str] database: Database against query will be executed. If not provided, will default to the "Initial Catalog" value in the connection string
         :param str query: Query to be executed.
         :param timedelta timeout: timeout for the query to be executed
         :param azure.kusto.data.ClientRequestProperties properties: Optional additional properties.
         :return KustoStreamingResponseDataSet:
         """
-        KustoTracingAttributes.set_query_attributes(self._kusto_cluster, database, properties)
+        Span.set_query_attributes(self._kusto_cluster, database, properties)
 
         return KustoStreamingResponseDataSet(self._execute_streaming_query_parsed(database, query, timeout, properties))
 
     def _execute(
         self,
         endpoint: str,
-        database: str,
+        database: Optional[str],
         query: Optional[str],
         payload: Optional[IO[AnyStr]],
         timeout: timedelta,
         properties: Optional[ClientRequestProperties] = None,
         stream_response: bool = False,
     ) -> Union[KustoResponseDataSet, Response]:
         """Executes given query against this client"""
@@ -273,26 +284,25 @@
         json_payload = request_params.json_payload
         request_headers = request_params.request_headers
         timeout = request_params.timeout
         if self._aad_helper:
             request_headers["Authorization"] = self._aad_helper.acquire_authorization_header()
 
         # trace http post call for response
-        http_trace_attributes = KustoTracingAttributes.create_http_attributes(url=endpoint, method="POST", headers=request_headers)
-        response = KustoTracing.call_func_tracing(
-            self._session.post,
+        invoker = lambda: self._session.post(
             endpoint,
             headers=request_headers,
             json=json_payload,
             data=payload,
             timeout=timeout.seconds,
             stream=stream_response,
             allow_redirects=False,
-            name_of_span="KustoClient.http_post",
-            tracing_attributes=http_trace_attributes,
+        )
+        response = MonitoredActivity.invoke(
+            invoker, name_of_span="KustoClient.http_post", tracing_attributes=Span.create_http_attributes("POST", endpoint, request_headers)
         )
 
         if stream_response:
             try:
                 response.raise_for_status()
                 if 300 <= response.status_code < 400:
                     raise Exception("Unexpected redirection, got status code: " + str(response.status))
@@ -305,8 +315,8 @@
             if 300 <= response.status_code < 400:
                 raise Exception("Unexpected redirection, got status code: " + str(response.status))
             response_json = response.json()
             response.raise_for_status()
         except Exception as e:
             raise self._handle_http_error(e, endpoint, payload, response, response.status_code, response_json, response.text)
         # trace response processing
-        return KustoTracing.call_func_tracing(self._kusto_parse_by_endpoint, endpoint, response_json, name_of_span="KustoClient.processing_response")
+        return MonitoredActivity.invoke(lambda: self._kusto_parse_by_endpoint(endpoint, response_json), name_of_span="KustoClient.processing_response")
```

### Comparing `azure-kusto-data-4.1.4/azure/kusto/data/client_base.py` & `azure-kusto-data-4.2.0/azure/kusto/data/client_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,27 +41,35 @@
         if not isinstance(kcsb, KustoConnectionStringBuilder):
             self._kcsb = KustoConnectionStringBuilder(kcsb)
         self._kusto_cluster = self._kcsb.data_source
 
         # notice that in this context, federated actually just stands for aad auth, not aad federated auth (legacy code)
         self._aad_helper = _AadHelper(self._kcsb, is_async) if self._kcsb.aad_federated_security else None
 
+        if not self._kusto_cluster.endswith("/"):
+            self._kusto_cluster += "/"
+
         # Create a session object for connection pooling
         self._mgmt_endpoint = urljoin(self._kusto_cluster, "v1/rest/mgmt")
         self._query_endpoint = urljoin(self._kusto_cluster, "v2/rest/query")
         self._streaming_ingest_endpoint = urljoin(self._kusto_cluster, "v1/rest/ingest/")
         self._request_headers = {
             "Accept": "application/json",
             "Accept-Encoding": "gzip,deflate",
             "x-ms-version": self.API_VERSION,
         }
 
         self.client_details = self._kcsb.client_details
         self._is_closed: bool = False
 
+        self.default_database = self._kcsb.initial_catalog
+
+    def _get_database_or_default(self, database_name: Optional[str]) -> str:
+        return database_name or self.default_database
+
     def close(self):
         if not self._is_closed:
             if self._aad_helper is not None:
                 self._aad_helper.close()
         self._is_closed = True
 
     def set_proxy(self, proxy_url: str):
```

### Comparing `azure-kusto-data-4.1.4/azure/kusto/data/client_details.py` & `azure-kusto-data-4.2.0/azure/kusto/data/client_details.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.4/azure/kusto/data/client_request_properties.py` & `azure-kusto-data-4.2.0/azure/kusto/data/client_request_properties.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.4/azure/kusto/data/data_format.py` & `azure-kusto-data-4.2.0/azure/kusto/data/data_format.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.4/azure/kusto/data/exceptions.py` & `azure-kusto-data-4.2.0/azure/kusto/data/exceptions.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.4/azure/kusto/data/helpers.py` & `azure-kusto-data-4.2.0/azure/kusto/data/helpers.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.4/azure/kusto/data/kcsb.py` & `azure-kusto-data-4.2.0/azure/kusto/data/kcsb.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 from enum import unique, Enum
 from typing import Union, Callable, Coroutine, Optional, Tuple, List, Any
+from urllib.parse import urlparse
 
 from ._string_utils import assert_string_is_not_empty
+from ._token_providers import DeviceCallbackType
 from .client_details import ClientDetails
 
 
 class KustoConnectionStringBuilder:
     """
     Parses Kusto connection strings.
     For usages, check out the sample at:
         https://github.com/Azure/azure-kusto-python/blob/master/azure-kusto-data/tests/sample.py
     """
 
+    DEFAULT_DATABASE_NAME = "NetDefaultDB"
+    device_callback: DeviceCallbackType = None
     kcsb_invalid_item_error = "%s is not supported as an item in KustoConnectionStringBuilder"
 
     @unique
     class ValidKeywords(Enum):
         """
         Set of properties that can be use in a connection string provided to KustoConnectionStringBuilder.
         For a complete list of properties go to https://docs.microsoft.com/en-us/azure/kusto/api/connection-strings/kusto
         """
 
         data_source = "Data Source"
+        initial_catalog = "Initial Catalog"
         aad_federated_security = "AAD Federated Security"
         aad_user_id = "AAD User ID"
         password = "Password"
         application_client_id = "Application Client Id"
         application_key = "Application Key"
         application_certificate = "Application Certificate"
         application_certificate_thumbprint = "Application Certificate Thumbprint"
@@ -42,14 +47,16 @@
 
         @classmethod
         def parse(cls, key: str) -> "KustoConnectionStringBuilder.ValidKeywords":
             """Create a valid keyword."""
             key = key.lower().strip()
             if key in ["data source", "addr", "address", "network address", "server"]:
                 return cls.data_source
+            if key in ["initial catalog"]:
+                return cls.initial_catalog
             if key in ["aad user id"]:
                 return cls.aad_user_id
             if key in ["password", "pwd"]:
                 return cls.password
             if key in ["application client id", "appclientid"]:
                 return cls.application_client_id
             if key in ["application key", "appkey"]:
@@ -98,14 +105,15 @@
                 self.password,
                 self.application_key,
                 self.authority_id,
                 self.application_token,
                 self.user_token,
                 self.login_hint,
                 self.domain_hint,
+                self.initial_catalog,
             ]
 
         def is_dict_type(self) -> bool:
             return self in [self.msi_params]
 
         def is_bool_type(self) -> bool:
             """States whether a word is of type bool or not."""
@@ -139,22 +147,27 @@
             try:
                 keyword = self.ValidKeywords.parse(key)
             except KeyError:
                 raise KeyError(self.kcsb_invalid_item_error % key)
             value_stripped = value.strip()
             if keyword.is_str_type():
                 self[keyword] = value_stripped.rstrip("/")
+                if keyword == self.ValidKeywords.data_source:
+                    self._parse_data_source(self.data_source)
             elif keyword.is_bool_type():
                 if value_stripped in ["True", "true"]:
                     self[keyword] = True
                 elif value_stripped in ["False", "false"]:
                     self[keyword] = False
                 else:
                     raise KeyError("Expected aad federated security to be bool. Recieved %s" % value)
 
+        if self.initial_catalog is None:
+            self.initial_catalog = self.DEFAULT_DATABASE_NAME
+
     def __setitem__(self, key: "Union[KustoConnectionStringBuilder.ValidKeywords, str]", value: Union[str, bool, dict]):
         try:
             keyword = key if isinstance(key, self.ValidKeywords) else self.ValidKeywords.parse(key)
         except KeyError:
             raise KeyError(self.kcsb_invalid_item_error % key)
 
         if value is None:
@@ -308,24 +321,31 @@
         kcsb = cls(connection_string)
         kcsb[kcsb.ValidKeywords.aad_federated_security] = True
         kcsb[kcsb.ValidKeywords.application_token] = application_token
 
         return kcsb
 
     @classmethod
-    def with_aad_device_authentication(cls, connection_string: str, authority_id: str = "organizations") -> "KustoConnectionStringBuilder":
+    def with_aad_device_authentication(
+        cls, connection_string: str, authority_id: str = "organizations", callback: DeviceCallbackType = None
+    ) -> "KustoConnectionStringBuilder":
         """
         Creates a KustoConnection string builder that will authenticate with AAD application and
         password.
         :param str connection_string: Kusto connection string should be of the format: https://<clusterName>.kusto.windows.net
         :param str authority_id: optional param. defaults to "organizations"
+        :param DeviceCallbackType callback: options callback function to be called when authentication is required, accepts three parameters:
+                - ``verification_uri`` (str) the URL the user must visit
+                - ``user_code`` (str) the code the user must enter there
+                - ``expires_on`` (datetime.datetime) the UTC time at which the code will expire
         """
         kcsb = cls(connection_string)
         kcsb[kcsb.ValidKeywords.aad_federated_security] = True
         kcsb[kcsb.ValidKeywords.authority_id] = authority_id
+        kcsb.device_callback = callback
 
         return kcsb
 
     @classmethod
     def with_az_cli_authentication(cls, connection_string: str) -> "KustoConnectionStringBuilder":
         """
         Creates a KustoConnection string builder that will use existing authenticated az cli profile
@@ -466,14 +486,25 @@
     def data_source(self) -> Optional[str]:
         """The URI specifying the Kusto service endpoint.
         For example, https://kuskus.kusto.windows.net or net.tcp://localhost
         """
         return self._internal_dict.get(self.ValidKeywords.data_source)
 
     @property
+    def initial_catalog(self) -> Optional[str]:
+        """The default database to be used for requests.
+        By default, it is set to 'NetDefaultDB'.
+        """
+        return self._internal_dict.get(self.ValidKeywords.initial_catalog)
+
+    @initial_catalog.setter
+    def initial_catalog(self, value: str) -> None:
+        self._internal_dict[self.ValidKeywords.initial_catalog] = value
+
+    @property
     def aad_user_id(self) -> Optional[str]:
         """The username to use for AAD Federated AuthN."""
         return self._internal_dict.get(self.ValidKeywords.aad_user_id)
 
     @property
     def password(self) -> Optional[str]:
         """The password to use for authentication when username/password authentication is used.
@@ -633,7 +664,16 @@
         return self._build_connection_string(dict_copy)
 
     def __repr__(self) -> str:
         return self._build_connection_string(self._internal_dict)
 
     def _build_connection_string(self, kcsb_as_dict: dict) -> str:
         return ";".join(["{0}={1}".format(word.value, kcsb_as_dict[word]) for word in self.ValidKeywords if word in kcsb_as_dict])
+
+    def _parse_data_source(self, url: str):
+        url = urlparse(url)
+        if not url.netloc:
+            return
+        segments = url.path.lstrip("/").split("/")
+        if len(segments) == 1 and segments[0] and not self.initial_catalog:
+            self.initial_catalog = segments[0]
+            self._internal_dict[self.ValidKeywords.data_source] = url._replace(path="").geturl()
```

### Comparing `azure-kusto-data-4.1.4/azure/kusto/data/kusto_trusted_endpoints.py` & `azure-kusto-data-4.2.0/azure/kusto/data/kusto_trusted_endpoints.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.4/azure/kusto/data/response.py` & `azure-kusto-data-4.2.0/azure/kusto/data/response.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.4/azure/kusto/data/security.py` & `azure-kusto-data-4.2.0/azure/kusto/data/security.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             self.token_provider = AzureIdentityTokenCredentialProvider(
                 self.kusto_uri,
                 is_async=is_async,
                 credential=kcsb.credential,
                 credential_from_login_endpoint=kcsb.credential_from_login_endpoint,
             )
         else:  # TODO - next breaking change - remove this as default, make no auth the default
-            self.token_provider = DeviceLoginTokenProvider(self.kusto_uri, kcsb.authority_id, is_async=is_async)
+            self.token_provider = DeviceLoginTokenProvider(self.kusto_uri, kcsb.authority_id, kcsb.device_callback, is_async=is_async)
 
     def acquire_authorization_header(self):
         try:
             return _get_header_from_dict(self.token_provider.get_token())
         except Exception as error:
             kwargs = self.token_provider.context()
             kwargs["kusto_uri"] = self.kusto_uri
```

### Comparing `azure-kusto-data-4.1.4/azure/kusto/data/streaming_response.py` & `azure-kusto-data-4.2.0/azure/kusto/data/streaming_response.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.4/azure/kusto/data/wellKnownKustoEndpoints.json` & `azure-kusto-data-4.2.0/azure/kusto/data/wellKnownKustoEndpoints.json`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.4/azure_kusto_data.egg-info/PKG-INFO` & `azure-kusto-data-4.2.0/azure_kusto_data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-kusto-data
-Version: 4.1.4
+Version: 4.2.0
 Summary: Kusto Data Client
 Home-page: https://github.com/Azure/azure-kusto-python
 Author: Microsoft Corporation
 Author-email: kustalk@microsoft.com
 License: MIT
 Description: Microsoft Azure Kusto Library for Python
         ========================================
```

### Comparing `azure-kusto-data-4.1.4/azure_kusto_data.egg-info/SOURCES.txt` & `azure-kusto-data-4.2.0/azure_kusto_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.4/setup.py` & `azure-kusto-data-4.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.1.4/tests/aio/test_async_token_providers.py` & `azure-kusto-data-4.2.0/tests/aio/test_async_token_providers.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,17 +207,17 @@
     @aio_documented_by(TokenProviderTests.test_device_auth_provider)
     @pytest.mark.asyncio
     async def test_device_auth_provider(self):
         if not TEST_DEVICE_AUTH:
             print(" *** Skipped User Device Flow Test ***")
             return
 
-        def callback(x):
+        def callback(x, x2, x3):
             # break here if you debug this test, and get the code from 'x'
-            print(x)
+            print(f"Please go to {x} and enter code {x2} to authenticate, expires in {x3}")
 
         with DeviceLoginTokenProvider(KUSTO_URI, "organizations", callback, is_async=True) as provider:
             token = await provider.get_token_async()
             assert self.get_token_value(token) is not None
 
             # Again through cache
             token = provider._get_token_from_cache_impl()
@@ -243,15 +243,15 @@
         else:
             print(" *** Skipped App Id & Key Provider Test ***")
 
     @aio_documented_by(TokenProviderTests.test_app_cert_provider)
     @pytest.mark.asyncio
     async def test_app_cert_provider(self):
         # default details are for kusto-client-e2e-test-app
-        # to run the test download the certs from Azure Portal
+        # to invoke the test download the certs from Azure Portal
         cert_app_id = os.environ.get("CERT_APP_ID", "b699d721-4f6f-4320-bc9a-88d578dfe68f")
         cert_auth = os.environ.get("CERT_AUTH", "72f988bf-86f1-41af-91ab-2d7cd011db47")
         thumbprint = os.environ.get("CERT_THUMBPRINT")
         public_cert_path = os.environ.get("PUBLIC_CERT_PATH")
         pem_key_path = os.environ.get("CERT_PEM_KEY_PATH")
 
         if pem_key_path and thumbprint and cert_app_id:
@@ -291,15 +291,15 @@
             login_endpoint="https://login_endpoint",
             login_mfa_required=False,
             kusto_client_app_id="1234",
             kusto_client_redirect_uri="",
             kusto_service_resource_id="https://fakeurl.kusto.windows.net",
             first_party_authority_url="",
         )
-        CloudSettings._cloud_cache[FAKE_URI] = cloud
+        CloudSettings.add_to_cache(FAKE_URI, cloud)
         authority = "auth_test"
 
         with UserPassTokenProvider(FAKE_URI, authority, "a", "b", is_async=True) as provider:
             await provider._init_once_async(init_only_resources=True)
             context = await provider.context_async()
             assert context["authority"] == "https://login_endpoint/auth_test"
             assert context["client_id"] == "1234"
@@ -313,15 +313,15 @@
             login_endpoint="https://login_endpoint",
             login_mfa_required=True,
             kusto_client_app_id="1234",
             kusto_client_redirect_uri="",
             kusto_service_resource_id="https://fakeurl.kusto.windows.net",
             first_party_authority_url="",
         )
-        CloudSettings._cloud_cache[FAKE_URI] = cloud
+        CloudSettings.add_to_cache(FAKE_URI, cloud)
         authority = "auth_test"
 
         with UserPassTokenProvider(FAKE_URI, authority, "a", "b", is_async=True) as provider:
             await provider._init_once_async(init_only_resources=True)
             context = await provider.context_async()
             assert context["authority"] == "https://login_endpoint/auth_test"
             assert context["client_id"] == "1234"
```

### Comparing `azure-kusto-data-4.1.4/tests/aio/test_kusto_client.py` & `azure-kusto-data-4.2.0/tests/aio/test_kusto_client.py`

 * *Files identical despite different names*

