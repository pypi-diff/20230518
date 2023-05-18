# Comparing `tmp/authomize-rest-api-client-4.0.0.tar.gz` & `tmp/authomize-rest-api-client-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authomize-rest-api-client-4.0.0.tar", last modified: Tue May 16 10:03:20 2023, max compression
+gzip compressed data, was "authomize-rest-api-client-4.1.0.tar", last modified: Thu May 18 07:28:33 2023, max compression
```

## Comparing `authomize-rest-api-client-4.0.0.tar` & `authomize-rest-api-client-4.1.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:03:20.656275 authomize-rest-api-client-4.0.0/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      134 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      251 2023-05-16 10:03:20.656275 authomize-rest-api-client-4.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2160 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:03:20.652275 authomize-rest-api-client-4.0.0/authomize/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:03:20.652275 authomize-rest-api-client-4.0.0/authomize/rest_api_client/
--rw-r--r--   0 root         (0) root         (0)      627 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/authomize/rest_api_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:03:20.652275 authomize-rest-api-client-4.0.0/authomize/rest_api_client/client/
--rw-r--r--   0 root         (0) root         (0)       81 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/authomize/rest_api_client/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2631 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/authomize/rest_api_client/client/base_client.py
--rw-r--r--   0 root         (0) root         (0)    10105 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/authomize/rest_api_client/client/client.py
--rw-r--r--   0 root         (0) root         (0)    12633 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/authomize/rest_api_client/client/connectors_client.py
--rw-r--r--   0 root         (0) root         (0)     1102 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/authomize/rest_api_client/client/platform_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:03:20.652275 authomize-rest-api-client-4.0.0/authomize/rest_api_client/configuration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/authomize/rest_api_client/configuration/__init__.py
--rw-r--r--   0 root         (0) root         (0)      330 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/authomize/rest_api_client/configuration/authomize_api_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:03:20.652275 authomize-rest-api-client-4.0.0/authomize/rest_api_client/generated/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/authomize/rest_api_client/generated/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:03:20.656275 authomize-rest-api-client-4.0.0/authomize/rest_api_client/generated/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    73614 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:03:20.656275 authomize-rest-api-client-4.0.0/authomize/rest_api_client/generated/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/authomize/rest_api_client/generated/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24501 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/authomize/rest_api_client/generated/external_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:03:20.656275 authomize-rest-api-client-4.0.0/authomize/rest_api_client/openapi/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/authomize/rest_api_client/openapi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:03:20.656275 authomize-rest-api-client-4.0.0/authomize/rest_api_client/openapi/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   185721 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:03:20.656275 authomize-rest-api-client-4.0.0/authomize/rest_api_client/openapi/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/authomize/rest_api_client/openapi/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    65008 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/authomize/rest_api_client/openapi/external_rest_api/openapi.json
--rw-r--r--   0 root         (0) root         (0)       26 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/authomize/rest_api_client/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:03:20.656275 authomize-rest-api-client-4.0.0/authomize_rest_api_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      251 2023-05-16 10:03:20.000000 authomize-rest-api-client-4.0.0/authomize_rest_api_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1356 2023-05-16 10:03:20.000000 authomize-rest-api-client-4.0.0/authomize_rest_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 10:03:20.000000 authomize-rest-api-client-4.0.0/authomize_rest_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      214 2023-05-16 10:03:20.000000 authomize-rest-api-client-4.0.0/authomize_rest_api_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-16 10:03:20.000000 authomize-rest-api-client-4.0.0/authomize_rest_api_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      336 2023-05-16 10:03:20.656275 authomize-rest-api-client-4.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1161 2023-05-16 10:03:19.000000 authomize-rest-api-client-4.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 07:28:33.050296 authomize-rest-api-client-4.1.0/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-05-18 07:28:07.000000 authomize-rest-api-client-4.1.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2023-05-18 07:28:07.000000 authomize-rest-api-client-4.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      251 2023-05-18 07:28:33.050296 authomize-rest-api-client-4.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2160 2023-05-18 07:28:07.000000 authomize-rest-api-client-4.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 07:28:33.046296 authomize-rest-api-client-4.1.0/authomize/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 07:28:33.046296 authomize-rest-api-client-4.1.0/authomize/rest_api_client/
+-rw-r--r--   0 root         (0) root         (0)      627 2023-05-18 07:28:07.000000 authomize-rest-api-client-4.1.0/authomize/rest_api_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 07:28:33.046296 authomize-rest-api-client-4.1.0/authomize/rest_api_client/client/
+-rw-r--r--   0 root         (0) root         (0)       81 2023-05-18 07:28:07.000000 authomize-rest-api-client-4.1.0/authomize/rest_api_client/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2631 2023-05-18 07:28:07.000000 authomize-rest-api-client-4.1.0/authomize/rest_api_client/client/base_client.py
+-rw-r--r--   0 root         (0) root         (0)    10105 2023-05-18 07:28:07.000000 authomize-rest-api-client-4.1.0/authomize/rest_api_client/client/client.py
+-rw-r--r--   0 root         (0) root         (0)    12633 2023-05-18 07:28:07.000000 authomize-rest-api-client-4.1.0/authomize/rest_api_client/client/connectors_client.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2023-05-18 07:28:07.000000 authomize-rest-api-client-4.1.0/authomize/rest_api_client/client/platform_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 07:28:33.046296 authomize-rest-api-client-4.1.0/authomize/rest_api_client/configuration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 07:28:07.000000 authomize-rest-api-client-4.1.0/authomize/rest_api_client/configuration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      330 2023-05-18 07:28:07.000000 authomize-rest-api-client-4.1.0/authomize/rest_api_client/configuration/authomize_api_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 07:28:33.046296 authomize-rest-api-client-4.1.0/authomize/rest_api_client/generated/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 07:28:07.000000 authomize-rest-api-client-4.1.0/authomize/rest_api_client/generated/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 07:28:33.046296 authomize-rest-api-client-4.1.0/authomize/rest_api_client/generated/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 07:28:07.000000 authomize-rest-api-client-4.1.0/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    73614 2023-05-18 07:28:07.000000 authomize-rest-api-client-4.1.0/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 07:28:33.046296 authomize-rest-api-client-4.1.0/authomize/rest_api_client/generated/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 07:28:07.000000 authomize-rest-api-client-4.1.0/authomize/rest_api_client/generated/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35822 2023-05-18 07:28:07.000000 authomize-rest-api-client-4.1.0/authomize/rest_api_client/generated/external_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 07:28:33.046296 authomize-rest-api-client-4.1.0/authomize/rest_api_client/openapi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 07:28:07.000000 authomize-rest-api-client-4.1.0/authomize/rest_api_client/openapi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 07:28:33.046296 authomize-rest-api-client-4.1.0/authomize/rest_api_client/openapi/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 07:28:07.000000 authomize-rest-api-client-4.1.0/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   185721 2023-05-18 07:28:07.000000 authomize-rest-api-client-4.1.0/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 07:28:33.046296 authomize-rest-api-client-4.1.0/authomize/rest_api_client/openapi/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 07:28:07.000000 authomize-rest-api-client-4.1.0/authomize/rest_api_client/openapi/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89185 2023-05-18 07:28:07.000000 authomize-rest-api-client-4.1.0/authomize/rest_api_client/openapi/external_rest_api/openapi.json
+-rw-r--r--   0 root         (0) root         (0)       26 2023-05-18 07:28:07.000000 authomize-rest-api-client-4.1.0/authomize/rest_api_client/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 07:28:33.050296 authomize-rest-api-client-4.1.0/authomize_rest_api_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      251 2023-05-18 07:28:33.000000 authomize-rest-api-client-4.1.0/authomize_rest_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-05-18 07:28:33.000000 authomize-rest-api-client-4.1.0/authomize_rest_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 07:28:33.000000 authomize-rest-api-client-4.1.0/authomize_rest_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      214 2023-05-18 07:28:33.000000 authomize-rest-api-client-4.1.0/authomize_rest_api_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-18 07:28:33.000000 authomize-rest-api-client-4.1.0/authomize_rest_api_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      336 2023-05-18 07:28:33.050296 authomize-rest-api-client-4.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1161 2023-05-18 07:28:31.000000 authomize-rest-api-client-4.1.0/setup.py
```

### Comparing `authomize-rest-api-client-4.0.0/LICENSE.txt` & `authomize-rest-api-client-4.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.0.0/README.md` & `authomize-rest-api-client-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.0.0/authomize/rest_api_client/__init__.py` & `authomize-rest-api-client-4.1.0/authomize/rest_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.0.0/authomize/rest_api_client/client/base_client.py` & `authomize-rest-api-client-4.1.0/authomize/rest_api_client/client/base_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.0.0/authomize/rest_api_client/client/client.py` & `authomize-rest-api-client-4.1.0/authomize/rest_api_client/client/client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.0.0/authomize/rest_api_client/client/connectors_client.py` & `authomize-rest-api-client-4.1.0/authomize/rest_api_client/client/connectors_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.0.0/authomize/rest_api_client/client/platform_client.py` & `authomize-rest-api-client-4.1.0/authomize/rest_api_client/client/platform_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.0.0/authomize/rest_api_client/generated/connectors_rest_api/schemas.py` & `authomize-rest-api-client-4.1.0/authomize/rest_api_client/generated/connectors_rest_api/schemas.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.0.0/authomize/rest_api_client/generated/external_rest_api/schemas.py` & `authomize-rest-api-client-4.1.0/authomize/rest_api_client/generated/external_rest_api/schemas.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  openapi.json
-#   timestamp: 2023-05-16T09:37:39+00:00
+#   timestamp: 2023-05-17T14:13:00+00:00
 
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 from typing import List, Optional, Union
 
@@ -17,14 +17,18 @@
 
 
 class AccessToType(Enum):
     asset = 'asset'
     grouping = 'grouping'
 
 
+class Object(Enum):
+    account = 'account'
+
+
 class AddIncidentCommentRequestSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     content: constr(max_length=1025) = Field(
         ..., description='Content of comment.', title='Content'
     )
@@ -62,14 +66,41 @@
     Detection = 'Detection'
     Persistence = 'Persistence'
     Evasion = 'Evasion'
     Account_Takeover = 'Account Takeover'
     Account_Impersonation__PE__LM_ = 'Account Impersonation (PE, LM)'
 
 
+class AppIdFilter(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    field_eq: Optional[str] = Field(
+        default=None, alias='$eq', description='Equals To', title='$Eq'
+    )
+
+
+class AssetExpansion(Enum):
+    sourceApp = 'sourceApp'
+    tags = 'tags'
+
+
+class AssetIdFilter(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    field_in: Optional[List[str]] = Field(
+        default=[], alias='$in', description='In', title='$In'
+    )
+
+
+class Object1(Enum):
+    asset = 'asset'
+
+
 class AttackTacticType(Enum):
     Collection = 'Collection'
     Credential_Access = 'Credential Access'
     Defense_Evasion = 'Defense Evasion'
     Discovery = 'Discovery'
     Exfiltration = 'Exfiltration'
     Impact = 'Impact'
@@ -181,14 +212,23 @@
 
     id: str = Field(..., description='Unique ID of comment.', title='Id')
     content: constr(max_length=1025) = Field(
         ..., description='Content of comment.', title='Content'
     )
 
 
+class EmailFilter(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    field_in: Optional[List[str]] = Field(
+        default=[], alias='$in', description='In', title='$In'
+    )
+
+
 class EventStatusType(Enum):
     Open = 'Open'
     InProgress = 'InProgress'
     WaitingForInput = 'WaitingForInput'
     Closed = 'Closed'
 
 
@@ -198,14 +238,32 @@
     startDate = 'startDate'
     endDate = 'endDate'
     createdAt = 'createdAt'
     reviewerType = 'reviewerType'
     templateName = 'templateName'
 
 
+class IdFilter(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    field_in: Optional[List[str]] = Field(
+        default=[], alias='$in', description='In', title='$In'
+    )
+
+
+class IdentityExpansion(Enum):
+    account = 'account'
+    tags = 'tags'
+
+
+class Object2(Enum):
+    identity = 'identity'
+
+
 class IncidentExpansion(Enum):
     policy = 'policy'
     assignee = 'assignee'
 
 
 class IncidentsCreatedAtFilter(BaseModel):
     class Config:
@@ -317,27 +375,36 @@
     A_8_2_3 = 'A.8.2.3'
     A_7_3_1 = 'A.7.3.1'
     A_8_1_4 = 'A.8.1.4'
 
 
 class MeResponse(BaseModel):
     version: Optional[str] = Field(
-        default='4.0.0', description='**version**', title='Version'
+        default='4.1.0', description='**version**', title='Version'
     )
     id: str = Field(..., description='**id**', title='Id')
     tenant: str = Field(..., description='**tenant**', title='Tenant')
 
 
 class NonPaginatedResponseSchemaCommentSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     data: CommentSchema = Field(..., description='Actual Data', title='Data')
 
 
+class OriginIdFilter(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    field_in: Optional[List[str]] = Field(
+        default=[], alias='$in', description='In', title='$In'
+    )
+
+
 class PaginationRequestSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     limit: Optional[int] = Field(default=None, description='Limit', title='Limit')
     nextPage: Optional[str] = Field(
         default=None, description='Starting after', title='NextPage'
@@ -372,14 +439,34 @@
     inactive = 'inactive'
 
 
 class ReviewerExpansion(Enum):
     user = 'user'
 
 
+class SearchAssetsSortFields(Enum):
+    asset_name = 'asset.name'
+
+
+class SearchIdentitiesFilterBody(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    email: Optional[EmailFilter] = Field(
+        default=None, description='Email.', title='Email'
+    )
+    authomizeId: Optional[IdFilter] = Field(
+        default=None, description='Authomize ID for the Identity', title='Authomizeid'
+    )
+
+
+class SearchIdentitiesSortFields(Enum):
+    identity_name = 'identity.name'
+
+
 class SearchIncidentsSortFields(Enum):
     createdAt = 'createdAt'
     updatedAt = 'updatedAt'
     severity = 'severity'
     status = 'status'
     isResolved = 'isResolved'
 
@@ -410,14 +497,38 @@
         ..., description='Sort By Field Name', title='FieldName'
     )
     order: Optional[SortOrder] = Field(
         default='ASC', description='Sort Order', title='Order'
     )
 
 
+class SortSchemaSearchAssetsSortFields(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    fieldName: SearchAssetsSortFields = Field(
+        ..., description='Sort By Field Name', title='FieldName'
+    )
+    order: Optional[SortOrder] = Field(
+        default='ASC', description='Sort Order', title='Order'
+    )
+
+
+class SortSchemaSearchIdentitiesSortFields(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    fieldName: SearchIdentitiesSortFields = Field(
+        ..., description='Sort By Field Name', title='FieldName'
+    )
+    order: Optional[SortOrder] = Field(
+        default='ASC', description='Sort Order', title='Order'
+    )
+
+
 class SortSchemaSearchIncidentsSortFields(BaseModel):
     class Config:
         extra = Extra.forbid
 
     fieldName: SearchIncidentsSortFields = Field(
         ..., description='Sort By Field Name', title='FieldName'
     )
@@ -427,14 +538,29 @@
 
 
 class SourceAppSchema(BaseModel):
     id: str = Field(..., description='Unique ID', title='Id')
     name: str = Field(..., description='Name', title='Name')
 
 
+class TagSchema(BaseModel):
+    id: str = Field(..., description='Id', title='Id')
+    name: str = Field(..., description='Name', title='Name')
+    description: str = Field(..., description='Description', title='Description')
+
+
+class UniqueIdFilter(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    field_in: Optional[List[str]] = Field(
+        default=[], alias='$in', description='In', title='$In'
+    )
+
+
 class UpdateIncidentRequestSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     assigneeId: Optional[str] = Field(
         default=None,
         description='ID of the entity assigned to this incident.',
@@ -469,14 +595,63 @@
         default='aicpaTsc2017', description='UniqueID', title='Id'
     )
     name: Optional[str] = Field(
         default='SOC 2 (TSC 2017)', description='Name', title='Name'
     )
 
 
+class AssetSchema(BaseModel):
+    authomizeId: str = Field(..., description='Unique ID', title='Authomizeid')
+    object: Object1 = Field(
+        ..., description='Type of entity (here `asset`)', title='Object'
+    )
+    name: str = Field(..., description='Name', title='Name')
+    type: str = Field(..., description='Type', title='Type')
+    originType: Optional[str] = Field(
+        default=None,
+        description='The asset type in the source system. The default is the canonical type (if not mentioned).\n',
+        title='Origintype',
+    )
+    sourceAppId: Optional[str] = Field(
+        default=None, description='Source App ID', title='Sourceappid'
+    )
+    sourceApp: Optional[SourceAppSchema] = Field(
+        default=None, description='Source App', title='Sourceapp'
+    )
+    tagIds: Optional[List[str]] = Field(
+        default=[], description='Tag IDs', title='Tagids'
+    )
+    createdAt: Optional[datetime] = Field(
+        default=None,
+        description='The date (in ISO 8601 format) that the asset was created.\n',
+        title='Createdat',
+    )
+    lastUsedAt: Optional[datetime] = Field(
+        default=None,
+        description='The date (in ISO 8601 format) of the last time that the asset was in use.',
+        title='Lastusedat',
+    )
+    href: Optional[str] = Field(default=None, description='HREF', title='Href')
+    isDeleted: bool = Field(..., description='HREF', title='Isdeleted')
+    uniqueId: Optional[str] = Field(
+        default=None, description='The Unique Identifier.', title='Uniqueid'
+    )
+    originId: Optional[str] = Field(
+        default=None,
+        description='The identifier of the asset from the origin system.',
+        title='Originid',
+    )
+    description: Optional[str] = Field(
+        default=None, description='Asset description', title='Description'
+    )
+    tags: Optional[List[TagSchema]] = Field(
+        default=None, description='Expanded Tags', title='Tags'
+    )
+
+
 class CampaignPermissionDecisionFilter(BaseModel):
     class Config:
         extra = Extra.forbid
 
     field_in: Optional[List[Selection]] = Field(
         default=[], alias='$in', description='In'
     )
@@ -537,14 +712,32 @@
     values: List[Ccm402Standard] = Field(..., description='Values')
     id: Optional[str] = Field(default='ccm402', description='UniqueID', title='Id')
     name: Optional[str] = Field(
         default='CSA STAR (CCM 4.0.2)', description='Name', title='Name'
     )
 
 
+class Chainable(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    originId: Optional[OriginIdFilter] = Field(
+        default=None, description='Origin ID of the Asset.', title='Originid'
+    )
+    appId: Optional[AppIdFilter] = Field(
+        default=None, description='ID of the Application.', title='Appid'
+    )
+    uniqueId: Optional[UniqueIdFilter] = Field(
+        default=None, description='Unique ID of the Asset.', title='Uniqueid'
+    )
+    authomizeId: Optional[AssetIdFilter] = Field(
+        default=None, description='Authomize ID for the Asset', title='Authomizeid'
+    )
+
+
 class HTTPValidationError(BaseModel):
     detail: Optional[List[ValidationError]] = Field(default=None, title='Detail')
 
 
 class IncidentEntitiesSchema(BaseModel):
     id: str = Field(..., description='Unique id of entity.', title='Id')
     name: Optional[str] = Field(
@@ -582,26 +775,65 @@
 class NonPaginatedResponseSchemaCampaignSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     data: CampaignSchema = Field(..., description='Actual Data', title='Data')
 
 
+class PaginatedResponseSchemaAssetSchema(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    pagination: Optional[PaginationResponseSchema] = Field(
+        default=None, description='Pagination Metadata', title='Pagination'
+    )
+    data: List[AssetSchema] = Field(
+        ..., description='List of Actual Data', title='Data'
+    )
+
+
 class PaginatedResponseSchemaCampaignSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     pagination: Optional[PaginationResponseSchema] = Field(
         default=None, description='Pagination Metadata', title='Pagination'
     )
     data: List[CampaignSchema] = Field(
         ..., description='List of Actual Data', title='Data'
     )
 
 
+class RawIdentitySchema(BaseModel):
+    authomizeId: str = Field(..., description='Unique ID', title='Authomizeid')
+    object: Object2 = Field(
+        ..., description='Type of entity (here `identity`)', title='Object'
+    )
+    name: Optional[str] = Field(
+        default=None, description='Name of Identity', title='Name'
+    )
+    title: Optional[str] = Field(default=None, description='Title', title='Title')
+    department: Optional[str] = Field(
+        default=None, description='Department', title='Department'
+    )
+    tagIds: Optional[List[str]] = Field(
+        default=[], description='List of tags', title='Tagids'
+    )
+    accountIds: Optional[List[str]] = Field(
+        default=[], description='List of associated account IDs', title='Accountids'
+    )
+    isDeleted: bool = Field(..., description='Is Deleted', title='Isdeleted')
+    email: Optional[str] = Field(
+        default=None, description="User's work email address.\n", title='Email'
+    )
+    tags: Optional[List[TagSchema]] = Field(
+        default=None, description='Expanded Tags', title='Tags'
+    )
+
+
 class ReviewerSchema(BaseModel):
     userId: str = Field(..., description='User ID of the Reviewer', title='Userid')
     campaignId: str = Field(..., description='Campaign ID', title='Campaignid')
     lastNotifiedAt: datetime = Field(
         ..., description='Time of last notified', title='Lastnotifiedat'
     )
     lastActiveAt: datetime = Field(
@@ -612,14 +844,32 @@
     )
     id: str = Field(..., description='Unique ID', title='Id')
     user: Optional[UserSchema] = Field(
         default=None, description='User Schema of the reviewer', title='User'
     )
 
 
+class SearchAssetsRequestSchema(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    sort: Optional[List[SortSchemaSearchAssetsSortFields]] = Field(
+        default=None, description='Sort', title='Sort'
+    )
+    pagination: Optional[PaginationRequestSchema] = Field(
+        default=None, description='Pagination', title='Pagination'
+    )
+    expand: Optional[List[AssetExpansion]] = Field(
+        default=None, description='Expand Fields'
+    )
+    filter: Optional[Chainable] = Field(
+        default=None, description='Search Assets Filter', title='Filter'
+    )
+
+
 class SearchCampaignPermissionsRequestSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     pagination: Optional[PaginationRequestSchema] = Field(
         default=None, description='Pagination', title='Pagination'
     )
@@ -645,14 +895,32 @@
         default=None, description='Pagination', title='Pagination'
     )
     sort: Optional[List[SortSchemaFieldName]] = Field(
         default=None, description='Sort', title='Sort'
     )
 
 
+class SearchIdentitiesRequestSchema(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    sort: Optional[List[SortSchemaSearchIdentitiesSortFields]] = Field(
+        default=None, description='Sort', title='Sort'
+    )
+    pagination: Optional[PaginationRequestSchema] = Field(
+        default=None, description='Pagination', title='Pagination'
+    )
+    expand: Optional[List[IdentityExpansion]] = Field(
+        default=None, description='Expand Fields'
+    )
+    filter: Optional[SearchIdentitiesFilterBody] = Field(
+        default=None, description='Search Identities Filter', title='Filter'
+    )
+
+
 class SearchIncidentsFilter(BaseModel):
     class Config:
         extra = Extra.forbid
 
     createdAt: Optional[IncidentsCreatedAtFilter] = Field(
         default=None, description='Created At date', title='Createdat'
     )
@@ -690,14 +958,54 @@
         default=None, description='Sort', title='Sort'
     )
     pagination: Optional[PaginationRequestSchema] = Field(
         default=None, description='Pagination', title='Pagination'
     )
 
 
+class AccountSchema(BaseModel):
+    authomizeId: str = Field(..., description='Unique ID', title='Authomizeid')
+    originId: Optional[str] = Field(
+        default=None,
+        description='The identifier of the account from the origin system.',
+        title='Originid',
+    )
+    uniqueId: Optional[str] = Field(
+        default=None,
+        description='Unique ID is an identifier coming from the connector that is guaranteed to be unique across all accounts coming from that connector.',
+        title='Uniqueid',
+    )
+    object: Object = Field(
+        ..., description='type of object (here `account`)', title='Object'
+    )
+    name: Optional[str] = Field(default=None, description='Name', title='Name')
+    type: str = Field(..., description='Type', title='Type')
+    isExternal: bool = Field(..., description='Is External', title='Isexternal')
+    email: Optional[str] = Field(default=None, description='Email', title='Email')
+    tagIds: Optional[List[str]] = Field(
+        default=[], description='Tag IDs', title='Tagids'
+    )
+    identityId: Optional[str] = Field(
+        default=None, description='Associated Identity ID ', title='Identityid'
+    )
+    identity: Optional[RawIdentitySchema] = Field(
+        default=None, description='Associated Identity', title='Identity'
+    )
+    sourceAppId: Optional[str] = Field(
+        default=None, description='Source App ID', title='Sourceappid'
+    )
+    sourceApp: Optional[SourceAppSchema] = Field(
+        default=None, description='Source App', title='Sourceapp'
+    )
+    isAdmin: Optional[bool] = Field(
+        default=None, description='Is Admin', title='Isadmin'
+    )
+    isDeleted: bool = Field(..., description='Is Deleted', title='Isdeleted')
+
+
 class CampaignsPermissionSchema(BaseModel):
     id: str = Field(..., description='Campaign ID (unique). \n', title='Id')
     campaignId: str = Field(
         ..., description='ID of the Campaign.\n', title='Campaignid'
     )
     reviewerId: str = Field(..., description='Reviewer ID', title='Reviewerid')
     reviewer: Optional[ReviewerSchema] = Field(
@@ -731,14 +1039,44 @@
     decisionReason: Optional[str] = Field(
         default=None,
         description='Reviewer decision for keeping or revoking the reviewed access.  \n',
         title='Decisionreason',
     )
 
 
+class IdentitySchema(BaseModel):
+    authomizeId: str = Field(..., description='Unique ID', title='Authomizeid')
+    object: Object2 = Field(
+        ..., description='Type of entity (here `identity`)', title='Object'
+    )
+    name: Optional[str] = Field(
+        default=None, description='Name of Identity', title='Name'
+    )
+    title: Optional[str] = Field(default=None, description='Title', title='Title')
+    department: Optional[str] = Field(
+        default=None, description='Department', title='Department'
+    )
+    tagIds: Optional[List[str]] = Field(
+        default=[], description='List of tags', title='Tagids'
+    )
+    accountIds: Optional[List[str]] = Field(
+        default=[], description='List of associated account IDs', title='Accountids'
+    )
+    isDeleted: bool = Field(..., description='Is Deleted', title='Isdeleted')
+    email: Optional[str] = Field(
+        default=None, description="User's work email address.\n", title='Email'
+    )
+    tags: Optional[List[TagSchema]] = Field(
+        default=None, description='Expanded Tags', title='Tags'
+    )
+    accounts: Optional[List[AccountSchema]] = Field(
+        default=[], description='List of associated accounts', title='Accounts'
+    )
+
+
 class IncidentSchema(BaseModel):
     id: str = Field(..., description='Unique id', title='Id')
     createdAt: Optional[datetime] = Field(
         default=None,
         description='The date the incident was first reported.',
         title='Createdat',
     )
@@ -810,14 +1148,26 @@
         default=None, description='Pagination Metadata', title='Pagination'
     )
     data: List[CampaignsPermissionSchema] = Field(
         ..., description='List of Actual Data', title='Data'
     )
 
 
+class PaginatedResponseSchemaIdentitySchema(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    pagination: Optional[PaginationResponseSchema] = Field(
+        default=None, description='Pagination Metadata', title='Pagination'
+    )
+    data: List[IdentitySchema] = Field(
+        ..., description='List of Actual Data', title='Data'
+    )
+
+
 class PaginatedResponseSchemaIncidentSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     pagination: Optional[PaginationResponseSchema] = Field(
         default=None, description='Pagination Metadata', title='Pagination'
     )
```

### Comparing `authomize-rest-api-client-4.0.0/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json` & `authomize-rest-api-client-4.1.0/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.0.0/authomize/rest_api_client/openapi/external_rest_api/openapi.json` & `authomize-rest-api-client-4.1.0/authomize/rest_api_client/openapi/external_rest_api/openapi.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9395142942994505%*

 * *Differences: {"'components'": "{'schemas': {'MeResponse': {'properties': {'version': {'default': '4.1.0'}}}, "*

 * *                 "'AccountSchema': OrderedDict([('title', 'AccountSchema'), ('required', "*

 * *                 "['authomizeId', 'object', 'type', 'isExternal', 'isDeleted']), ('type', "*

 * *                 "'object'), ('properties', OrderedDict([('authomizeId', OrderedDict([('title', "*

 * *                 "'Authomizeid'), ('type', 'string'), ('description', 'Unique ID')])), "*

 * *                 "('originId', OrderedDict([ […]*

```diff
@@ -15,14 +15,117 @@
                 "enum": [
                     "asset",
                     "grouping"
                 ],
                 "title": "AccessToType",
                 "type": "string"
             },
+            "AccountSchema": {
+                "properties": {
+                    "authomizeId": {
+                        "description": "Unique ID",
+                        "title": "Authomizeid",
+                        "type": "string"
+                    },
+                    "email": {
+                        "description": "Email",
+                        "title": "Email",
+                        "type": "string"
+                    },
+                    "identity": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/RawIdentitySchema"
+                            }
+                        ],
+                        "description": "Associated Identity",
+                        "title": "Identity"
+                    },
+                    "identityId": {
+                        "description": "Associated Identity ID ",
+                        "title": "Identityid",
+                        "type": "string"
+                    },
+                    "isAdmin": {
+                        "description": "Is Admin",
+                        "title": "Isadmin",
+                        "type": "boolean"
+                    },
+                    "isDeleted": {
+                        "description": "Is Deleted",
+                        "title": "Isdeleted",
+                        "type": "boolean"
+                    },
+                    "isExternal": {
+                        "description": "Is External",
+                        "title": "Isexternal",
+                        "type": "boolean"
+                    },
+                    "name": {
+                        "description": "Name",
+                        "title": "Name",
+                        "type": "string"
+                    },
+                    "object": {
+                        "description": "type of object (here `account`)",
+                        "enum": [
+                            "account"
+                        ],
+                        "title": "Object",
+                        "type": "string"
+                    },
+                    "originId": {
+                        "description": "The identifier of the account from the origin system.",
+                        "title": "Originid",
+                        "type": "string"
+                    },
+                    "sourceApp": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/SourceAppSchema"
+                            }
+                        ],
+                        "description": "Source App",
+                        "title": "Sourceapp"
+                    },
+                    "sourceAppId": {
+                        "description": "Source App ID",
+                        "title": "Sourceappid",
+                        "type": "string"
+                    },
+                    "tagIds": {
+                        "default": [],
+                        "description": "Tag IDs",
+                        "items": {
+                            "type": "string"
+                        },
+                        "title": "Tagids",
+                        "type": "array"
+                    },
+                    "type": {
+                        "description": "Type",
+                        "title": "Type",
+                        "type": "string"
+                    },
+                    "uniqueId": {
+                        "description": "Unique ID is an identifier coming from the connector that is guaranteed to be unique across all accounts coming from that connector.",
+                        "title": "Uniqueid",
+                        "type": "string"
+                    }
+                },
+                "required": [
+                    "authomizeId",
+                    "object",
+                    "type",
+                    "isExternal",
+                    "isDeleted"
+                ],
+                "title": "AccountSchema",
+                "type": "object"
+            },
             "AddIncidentCommentRequestSchema": {
                 "additionalProperties": false,
                 "description": "Base schema for all incoming API requests.",
                 "properties": {
                     "content": {
                         "description": "Content of comment.",
                         "maxLength": 1025,
@@ -102,14 +205,160 @@
                     "Persistence",
                     "Evasion",
                     "Account Takeover",
                     "Account Impersonation (PE, LM)"
                 ],
                 "title": "AlertCategoryType"
             },
+            "AppIdFilter": {
+                "additionalProperties": false,
+                "properties": {
+                    "$eq": {
+                        "description": "Equals To",
+                        "title": "$Eq",
+                        "type": "string"
+                    }
+                },
+                "title": "AppIdFilter",
+                "type": "object"
+            },
+            "AssetExpansion": {
+                "description": "An enumeration.",
+                "enum": [
+                    "sourceApp",
+                    "tags"
+                ],
+                "title": "AssetExpansion",
+                "type": "string"
+            },
+            "AssetIdFilter": {
+                "additionalProperties": false,
+                "properties": {
+                    "$in": {
+                        "default": [],
+                        "description": "In",
+                        "items": {
+                            "type": "string"
+                        },
+                        "title": "$In",
+                        "type": "array"
+                    }
+                },
+                "title": "AssetIdFilter",
+                "type": "object"
+            },
+            "AssetSchema": {
+                "properties": {
+                    "authomizeId": {
+                        "description": "Unique ID",
+                        "title": "Authomizeid",
+                        "type": "string"
+                    },
+                    "createdAt": {
+                        "description": "The date (in ISO 8601 format) that the asset was created.\n",
+                        "format": "date-time",
+                        "title": "Createdat",
+                        "type": "string"
+                    },
+                    "description": {
+                        "description": "Asset description",
+                        "title": "Description",
+                        "type": "string"
+                    },
+                    "href": {
+                        "description": "HREF",
+                        "title": "Href",
+                        "type": "string"
+                    },
+                    "isDeleted": {
+                        "description": "HREF",
+                        "title": "Isdeleted",
+                        "type": "boolean"
+                    },
+                    "lastUsedAt": {
+                        "description": "The date (in ISO 8601 format) of the last time that the asset was in use.",
+                        "format": "date-time",
+                        "title": "Lastusedat",
+                        "type": "string"
+                    },
+                    "name": {
+                        "description": "Name",
+                        "title": "Name",
+                        "type": "string"
+                    },
+                    "object": {
+                        "description": "Type of entity (here `asset`)",
+                        "enum": [
+                            "asset"
+                        ],
+                        "title": "Object",
+                        "type": "string"
+                    },
+                    "originId": {
+                        "description": "The identifier of the asset from the origin system.",
+                        "title": "Originid",
+                        "type": "string"
+                    },
+                    "originType": {
+                        "description": "The asset type in the source system. The default is the canonical type (if not mentioned).\n",
+                        "title": "Origintype",
+                        "type": "string"
+                    },
+                    "sourceApp": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/SourceAppSchema"
+                            }
+                        ],
+                        "description": "Source App",
+                        "title": "Sourceapp"
+                    },
+                    "sourceAppId": {
+                        "description": "Source App ID",
+                        "title": "Sourceappid",
+                        "type": "string"
+                    },
+                    "tagIds": {
+                        "default": [],
+                        "description": "Tag IDs",
+                        "items": {
+                            "type": "string"
+                        },
+                        "title": "Tagids",
+                        "type": "array"
+                    },
+                    "tags": {
+                        "description": "Expanded Tags",
+                        "items": {
+                            "$ref": "#/components/schemas/TagSchema"
+                        },
+                        "title": "Tags",
+                        "type": "array"
+                    },
+                    "type": {
+                        "description": "Type",
+                        "title": "Type",
+                        "type": "string"
+                    },
+                    "uniqueId": {
+                        "description": "The Unique Identifier.",
+                        "title": "Uniqueid",
+                        "type": "string"
+                    }
+                },
+                "required": [
+                    "authomizeId",
+                    "object",
+                    "name",
+                    "type",
+                    "isDeleted"
+                ],
+                "title": "AssetSchema",
+                "type": "object"
+            },
             "AttackTacticType": {
                 "description": "An enumeration.",
                 "enum": [
                     "Collection",
                     "Credential Access",
                     "Defense Evasion",
                     "Discovery",
@@ -463,14 +712,58 @@
                     "AIS-03",
                     "DSP-17",
                     "DSP-01",
                     "HRS-05"
                 ],
                 "title": "Ccm402Standard"
             },
+            "Chainable": {
+                "additionalProperties": false,
+                "description": "Base schema for all incoming API requests.",
+                "properties": {
+                    "appId": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/AppIdFilter"
+                            }
+                        ],
+                        "description": "ID of the Application.",
+                        "title": "Appid"
+                    },
+                    "authomizeId": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/AssetIdFilter"
+                            }
+                        ],
+                        "description": "Authomize ID for the Asset",
+                        "title": "Authomizeid"
+                    },
+                    "originId": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/OriginIdFilter"
+                            }
+                        ],
+                        "description": "Origin ID of the Asset.",
+                        "title": "Originid"
+                    },
+                    "uniqueId": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/UniqueIdFilter"
+                            }
+                        ],
+                        "description": "Unique ID of the Asset.",
+                        "title": "Uniqueid"
+                    }
+                },
+                "title": "Chainable",
+                "type": "object"
+            },
             "CisV8Standard": {
                 "description": "An enumeration.",
                 "enum": [
                     "3.1",
                     "3.3",
                     "6.8",
                     "5.4",
@@ -535,14 +828,30 @@
                 "required": [
                     "id",
                     "content"
                 ],
                 "title": "CommentSchema",
                 "type": "object"
             },
+            "EmailFilter": {
+                "additionalProperties": false,
+                "properties": {
+                    "$in": {
+                        "default": [],
+                        "description": "In",
+                        "items": {
+                            "type": "string"
+                        },
+                        "title": "$In",
+                        "type": "array"
+                    }
+                },
+                "title": "EmailFilter",
+                "type": "object"
+            },
             "EventStatusType": {
                 "description": "An enumeration.",
                 "enum": [
                     "Open",
                     "InProgress",
                     "WaitingForInput",
                     "Closed"
@@ -571,14 +880,123 @@
                         "title": "Detail",
                         "type": "array"
                     }
                 },
                 "title": "HTTPValidationError",
                 "type": "object"
             },
+            "IdFilter": {
+                "additionalProperties": false,
+                "properties": {
+                    "$in": {
+                        "default": [],
+                        "description": "In",
+                        "items": {
+                            "type": "string"
+                        },
+                        "title": "$In",
+                        "type": "array"
+                    }
+                },
+                "title": "IdFilter",
+                "type": "object"
+            },
+            "IdentityExpansion": {
+                "description": "An enumeration.",
+                "enum": [
+                    "account",
+                    "tags"
+                ],
+                "title": "IdentityExpansion",
+                "type": "string"
+            },
+            "IdentitySchema": {
+                "properties": {
+                    "accountIds": {
+                        "default": [],
+                        "description": "List of associated account IDs",
+                        "items": {
+                            "type": "string"
+                        },
+                        "title": "Accountids",
+                        "type": "array"
+                    },
+                    "accounts": {
+                        "default": [],
+                        "description": "List of associated accounts",
+                        "items": {
+                            "$ref": "#/components/schemas/AccountSchema"
+                        },
+                        "title": "Accounts",
+                        "type": "array"
+                    },
+                    "authomizeId": {
+                        "description": "Unique ID",
+                        "title": "Authomizeid",
+                        "type": "string"
+                    },
+                    "department": {
+                        "description": "Department",
+                        "title": "Department",
+                        "type": "string"
+                    },
+                    "email": {
+                        "description": "User's work email address.\n",
+                        "title": "Email",
+                        "type": "string"
+                    },
+                    "isDeleted": {
+                        "description": "Is Deleted",
+                        "title": "Isdeleted",
+                        "type": "boolean"
+                    },
+                    "name": {
+                        "description": "Name of Identity",
+                        "title": "Name",
+                        "type": "string"
+                    },
+                    "object": {
+                        "description": "Type of entity (here `identity`)",
+                        "enum": [
+                            "identity"
+                        ],
+                        "title": "Object",
+                        "type": "string"
+                    },
+                    "tagIds": {
+                        "default": [],
+                        "description": "List of tags",
+                        "items": {
+                            "type": "string"
+                        },
+                        "title": "Tagids",
+                        "type": "array"
+                    },
+                    "tags": {
+                        "description": "Expanded Tags",
+                        "items": {
+                            "$ref": "#/components/schemas/TagSchema"
+                        },
+                        "title": "Tags",
+                        "type": "array"
+                    },
+                    "title": {
+                        "description": "Title",
+                        "title": "Title",
+                        "type": "string"
+                    }
+                },
+                "required": [
+                    "authomizeId",
+                    "object",
+                    "isDeleted"
+                ],
+                "title": "IdentitySchema",
+                "type": "object"
+            },
             "IncidentEntitiesSchema": {
                 "properties": {
                     "email": {
                         "description": "Email",
                         "title": "Email",
                         "type": "string"
                     },
@@ -1009,15 +1427,15 @@
                     },
                     "tenant": {
                         "description": "**tenant**",
                         "title": "Tenant",
                         "type": "string"
                     },
                     "version": {
-                        "default": "4.0.0",
+                        "default": "4.1.0",
                         "description": "**version**",
                         "title": "Version",
                         "type": "string"
                     }
                 },
                 "required": [
                     "id",
@@ -1098,14 +1516,57 @@
                 },
                 "required": [
                     "data"
                 ],
                 "title": "NonPaginatedResponseSchema[ReviewerSchema]",
                 "type": "object"
             },
+            "OriginIdFilter": {
+                "additionalProperties": false,
+                "properties": {
+                    "$in": {
+                        "default": [],
+                        "description": "In",
+                        "items": {
+                            "type": "string"
+                        },
+                        "title": "$In",
+                        "type": "array"
+                    }
+                },
+                "title": "OriginIdFilter",
+                "type": "object"
+            },
+            "PaginatedResponseSchema_AssetSchema_": {
+                "additionalProperties": false,
+                "properties": {
+                    "data": {
+                        "description": "List of Actual Data",
+                        "items": {
+                            "$ref": "#/components/schemas/AssetSchema"
+                        },
+                        "title": "Data",
+                        "type": "array"
+                    },
+                    "pagination": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/PaginationResponseSchema"
+                            }
+                        ],
+                        "description": "Pagination Metadata",
+                        "title": "Pagination"
+                    }
+                },
+                "required": [
+                    "data"
+                ],
+                "title": "PaginatedResponseSchema[AssetSchema]",
+                "type": "object"
+            },
             "PaginatedResponseSchema_CampaignSchema_": {
                 "additionalProperties": false,
                 "properties": {
                     "data": {
                         "description": "List of Actual Data",
                         "items": {
                             "$ref": "#/components/schemas/CampaignSchema"
@@ -1152,14 +1613,41 @@
                 },
                 "required": [
                     "data"
                 ],
                 "title": "PaginatedResponseSchema[CampaignsPermissionSchema]",
                 "type": "object"
             },
+            "PaginatedResponseSchema_IdentitySchema_": {
+                "additionalProperties": false,
+                "properties": {
+                    "data": {
+                        "description": "List of Actual Data",
+                        "items": {
+                            "$ref": "#/components/schemas/IdentitySchema"
+                        },
+                        "title": "Data",
+                        "type": "array"
+                    },
+                    "pagination": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/PaginationResponseSchema"
+                            }
+                        ],
+                        "description": "Pagination Metadata",
+                        "title": "Pagination"
+                    }
+                },
+                "required": [
+                    "data"
+                ],
+                "title": "PaginatedResponseSchema[IdentitySchema]",
+                "type": "object"
+            },
             "PaginatedResponseSchema_IncidentSchema_": {
                 "additionalProperties": false,
                 "properties": {
                     "data": {
                         "description": "List of Actual Data",
                         "items": {
                             "$ref": "#/components/schemas/IncidentSchema"
@@ -1254,14 +1742,89 @@
                     "id",
                     "name",
                     "templateId"
                 ],
                 "title": "PolicySchema",
                 "type": "object"
             },
+            "RawIdentitySchema": {
+                "properties": {
+                    "accountIds": {
+                        "default": [],
+                        "description": "List of associated account IDs",
+                        "items": {
+                            "type": "string"
+                        },
+                        "title": "Accountids",
+                        "type": "array"
+                    },
+                    "authomizeId": {
+                        "description": "Unique ID",
+                        "title": "Authomizeid",
+                        "type": "string"
+                    },
+                    "department": {
+                        "description": "Department",
+                        "title": "Department",
+                        "type": "string"
+                    },
+                    "email": {
+                        "description": "User's work email address.\n",
+                        "title": "Email",
+                        "type": "string"
+                    },
+                    "isDeleted": {
+                        "description": "Is Deleted",
+                        "title": "Isdeleted",
+                        "type": "boolean"
+                    },
+                    "name": {
+                        "description": "Name of Identity",
+                        "title": "Name",
+                        "type": "string"
+                    },
+                    "object": {
+                        "description": "Type of entity (here `identity`)",
+                        "enum": [
+                            "identity"
+                        ],
+                        "title": "Object",
+                        "type": "string"
+                    },
+                    "tagIds": {
+                        "default": [],
+                        "description": "List of tags",
+                        "items": {
+                            "type": "string"
+                        },
+                        "title": "Tagids",
+                        "type": "array"
+                    },
+                    "tags": {
+                        "description": "Expanded Tags",
+                        "items": {
+                            "$ref": "#/components/schemas/TagSchema"
+                        },
+                        "title": "Tags",
+                        "type": "array"
+                    },
+                    "title": {
+                        "description": "Title",
+                        "title": "Title",
+                        "type": "string"
+                    }
+                },
+                "required": [
+                    "authomizeId",
+                    "object",
+                    "isDeleted"
+                ],
+                "title": "RawIdentitySchema",
+                "type": "object"
+            },
             "ReviewStatus": {
                 "description": "An enumeration.",
                 "enum": [
                     "pending",
                     "completed",
                     "reviewing",
                     "notified",
@@ -1335,14 +1898,63 @@
                     "lastActiveAt",
                     "reviewStatus",
                     "id"
                 ],
                 "title": "ReviewerSchema",
                 "type": "object"
             },
+            "SearchAssetsRequestSchema": {
+                "additionalProperties": false,
+                "description": "Base schema for all incoming API requests.",
+                "properties": {
+                    "expand": {
+                        "description": "Expand Fields",
+                        "items": {
+                            "$ref": "#/components/schemas/AssetExpansion"
+                        },
+                        "type": "array"
+                    },
+                    "filter": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/Chainable"
+                            }
+                        ],
+                        "description": "Search Assets Filter",
+                        "title": "Filter"
+                    },
+                    "pagination": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/PaginationRequestSchema"
+                            }
+                        ],
+                        "description": "Pagination",
+                        "title": "Pagination"
+                    },
+                    "sort": {
+                        "description": "Sort",
+                        "items": {
+                            "$ref": "#/components/schemas/SortSchema_SearchAssetsSortFields_"
+                        },
+                        "title": "Sort",
+                        "type": "array"
+                    }
+                },
+                "title": "SearchAssetsRequestSchema",
+                "type": "object"
+            },
+            "SearchAssetsSortFields": {
+                "description": "An enumeration.",
+                "enum": [
+                    "asset.name"
+                ],
+                "title": "SearchAssetsSortFields",
+                "type": "string"
+            },
             "SearchCampaignPermissionsRequestSchema": {
                 "additionalProperties": false,
                 "description": "Base schema for all incoming API requests.",
                 "properties": {
                     "expand": {
                         "description": "Fields to expand.\n",
                         "items": {
@@ -1409,14 +2021,89 @@
                         "title": "Sort",
                         "type": "array"
                     }
                 },
                 "title": "SearchCampaignsRequestSchema",
                 "type": "object"
             },
+            "SearchIdentitiesFilterBody": {
+                "additionalProperties": false,
+                "description": "Base schema for all incoming API requests.",
+                "properties": {
+                    "authomizeId": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/IdFilter"
+                            }
+                        ],
+                        "description": "Authomize ID for the Identity",
+                        "title": "Authomizeid"
+                    },
+                    "email": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/EmailFilter"
+                            }
+                        ],
+                        "description": "Email.",
+                        "title": "Email"
+                    }
+                },
+                "title": "SearchIdentitiesFilterBody",
+                "type": "object"
+            },
+            "SearchIdentitiesRequestSchema": {
+                "additionalProperties": false,
+                "description": "Base schema for all incoming API requests.",
+                "properties": {
+                    "expand": {
+                        "description": "Expand Fields",
+                        "items": {
+                            "$ref": "#/components/schemas/IdentityExpansion"
+                        },
+                        "type": "array"
+                    },
+                    "filter": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/SearchIdentitiesFilterBody"
+                            }
+                        ],
+                        "description": "Search Identities Filter",
+                        "title": "Filter"
+                    },
+                    "pagination": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/PaginationRequestSchema"
+                            }
+                        ],
+                        "description": "Pagination",
+                        "title": "Pagination"
+                    },
+                    "sort": {
+                        "description": "Sort",
+                        "items": {
+                            "$ref": "#/components/schemas/SortSchema_SearchIdentitiesSortFields_"
+                        },
+                        "title": "Sort",
+                        "type": "array"
+                    }
+                },
+                "title": "SearchIdentitiesRequestSchema",
+                "type": "object"
+            },
+            "SearchIdentitiesSortFields": {
+                "description": "An enumeration.",
+                "enum": [
+                    "identity.name"
+                ],
+                "title": "SearchIdentitiesSortFields",
+                "type": "string"
+            },
             "SearchIncidentsFilter": {
                 "additionalProperties": false,
                 "description": "Base schema for all incoming API requests.",
                 "properties": {
                     "createdAt": {
                         "allOf": [
                             {
@@ -1590,14 +2277,72 @@
                 },
                 "required": [
                     "fieldName"
                 ],
                 "title": "SortSchema[FieldName]",
                 "type": "object"
             },
+            "SortSchema_SearchAssetsSortFields_": {
+                "additionalProperties": false,
+                "properties": {
+                    "fieldName": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/SearchAssetsSortFields"
+                            }
+                        ],
+                        "description": "Sort By Field Name",
+                        "title": "FieldName"
+                    },
+                    "order": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/SortOrder"
+                            }
+                        ],
+                        "default": "ASC",
+                        "description": "Sort Order",
+                        "title": "Order"
+                    }
+                },
+                "required": [
+                    "fieldName"
+                ],
+                "title": "SortSchema[SearchAssetsSortFields]",
+                "type": "object"
+            },
+            "SortSchema_SearchIdentitiesSortFields_": {
+                "additionalProperties": false,
+                "properties": {
+                    "fieldName": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/SearchIdentitiesSortFields"
+                            }
+                        ],
+                        "description": "Sort By Field Name",
+                        "title": "FieldName"
+                    },
+                    "order": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/SortOrder"
+                            }
+                        ],
+                        "default": "ASC",
+                        "description": "Sort Order",
+                        "title": "Order"
+                    }
+                },
+                "required": [
+                    "fieldName"
+                ],
+                "title": "SortSchema[SearchIdentitiesSortFields]",
+                "type": "object"
+            },
             "SortSchema_SearchIncidentsSortFields_": {
                 "additionalProperties": false,
                 "properties": {
                     "fieldName": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/SearchIncidentsSortFields"
@@ -1639,14 +2384,56 @@
                 "required": [
                     "id",
                     "name"
                 ],
                 "title": "SourceAppSchema",
                 "type": "object"
             },
+            "TagSchema": {
+                "properties": {
+                    "description": {
+                        "description": "Description",
+                        "title": "Description",
+                        "type": "string"
+                    },
+                    "id": {
+                        "description": "Id",
+                        "title": "Id",
+                        "type": "string"
+                    },
+                    "name": {
+                        "description": "Name",
+                        "title": "Name",
+                        "type": "string"
+                    }
+                },
+                "required": [
+                    "id",
+                    "name",
+                    "description"
+                ],
+                "title": "TagSchema",
+                "type": "object"
+            },
+            "UniqueIdFilter": {
+                "additionalProperties": false,
+                "properties": {
+                    "$in": {
+                        "default": [],
+                        "description": "In",
+                        "items": {
+                            "type": "string"
+                        },
+                        "title": "$In",
+                        "type": "array"
+                    }
+                },
+                "title": "UniqueIdFilter",
+                "type": "object"
+            },
             "UpdateIncidentRequestSchema": {
                 "additionalProperties": false,
                 "description": "Base schema for all incoming API requests.",
                 "properties": {
                     "assigneeId": {
                         "description": "ID of the entity assigned to this incident.",
                         "title": "Assigneeid",
@@ -1738,15 +2525,15 @@
                 "type": "apiKey"
             }
         }
     },
     "info": {
         "description": "Authomize enables users to integrate your applications with Authomize via custom connectors.\n\nYou can use the APIs described in this document to create your connector.\n\nOnce data is uploaded and processed successfully, your custom connector will function in the same way as the connectors created by Authomize.\n\n## How does Authomize work?\nAuthomize works by gathering information about:\n\n\u00b7 individuals, teams and functions.\n\n\u00b7 apps, assets and accounts.\n\n\u00b7 all the relationships between them.\n\n![img.png](https://storagetry1.blob.core.windows.net/public/78d82650-71b0-4909-8444-022aab79add5.png)\n\n## Connector APIs\n\nAuthomize connector APIs enable pushing data into Authomize from external sources.\n\nThese APIs enable data extracted from outside applications (via application APIs) to be delivered to Authomize.\n\nA connector processes extracted application data to transform it into a format compatible with Authomize.\n\n![img_1.png](https://storagetry1.blob.core.windows.net/public/341bf6ef-2e5b-4284-b715-45105ffbf0f8.png)\n\n## Authentication\nTo Authenticate use the API Token, with the format: `Authorization: API_Token`.\n\nAn API Token is a token you provide when making API calls. \n\n\nThe API Token should be included in every request to the API in an `Authorization` header.\n```\ncurl -v -X POST \\n\n     -H \"Authorization: {API_Token}\" \\n\n     ...\n```\n\n## Limits\nRequests cannot exceed a size of 1MB.\n",
         "title": "Authomize API Reference",
-        "version": "4.0.0",
+        "version": "4.1.0",
         "x-logo": {
             "url": "https://static.authomize.com/public/icons/authomize-green.svg"
         }
     },
     "openapi": "3.0.2",
     "paths": {
         "/is_alive": {
@@ -2304,24 +3091,122 @@
                     }
                 ],
                 "summary": "Retrieve Incidents Extended",
                 "tags": [
                     "Incident"
                 ]
             }
+        },
+        "/v2/inventory/assets/search": {
+            "post": {
+                "description": "Search Assets",
+                "operationId": "search_assets_v2_inventory_assets_search_post",
+                "requestBody": {
+                    "content": {
+                        "application/json": {
+                            "schema": {
+                                "$ref": "#/components/schemas/SearchAssetsRequestSchema"
+                            }
+                        }
+                    },
+                    "required": true
+                },
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/PaginatedResponseSchema_AssetSchema_"
+                                }
+                            }
+                        },
+                        "description": "Successful Response"
+                    },
+                    "422": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/HTTPValidationError"
+                                }
+                            }
+                        },
+                        "description": "Validation Error"
+                    }
+                },
+                "security": [
+                    {
+                        "APIKeyHeader": []
+                    }
+                ],
+                "summary": "Search Assets",
+                "tags": [
+                    "Inventory"
+                ]
+            }
+        },
+        "/v2/inventory/identities/search": {
+            "post": {
+                "description": "Search Identities",
+                "operationId": "search_identities_v2_inventory_identities_search_post",
+                "requestBody": {
+                    "content": {
+                        "application/json": {
+                            "schema": {
+                                "$ref": "#/components/schemas/SearchIdentitiesRequestSchema"
+                            }
+                        }
+                    },
+                    "required": true
+                },
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/PaginatedResponseSchema_IdentitySchema_"
+                                }
+                            }
+                        },
+                        "description": "Successful Response"
+                    },
+                    "422": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/HTTPValidationError"
+                                }
+                            }
+                        },
+                        "description": "Validation Error"
+                    }
+                },
+                "security": [
+                    {
+                        "APIKeyHeader": []
+                    }
+                ],
+                "summary": "Search Identities",
+                "tags": [
+                    "Inventory"
+                ]
+            }
         }
     },
     "tags": [
         {
             "description": "The status of the API.\n",
             "name": "Status"
         },
         {
             "description": "The Incidents APIs enable you to pull Authomize-generated incidents from Authomize into your automated Incident Response system. Once you have responded to the incident you can use Authomize Incident APIs to update (and synchronize) the incident on Authomize.",
             "name": "Incident"
         },
         {
             "description": "Campaign APIs enable you to pull all the decisions from the campaign (keep or revoke) and to automate the revocation process to remove unnecessary permissions.\nCampaign APIs also enable you to pull basic details on the campaigns and to pull a list of all campaigns.\n",
             "name": "Campaign"
+        },
+        {
+            "description": "Inventory APIs",
+            "name": "Inventory"
         }
     ]
 }
```

### Comparing `authomize-rest-api-client-4.0.0/authomize_rest_api_client.egg-info/SOURCES.txt` & `authomize-rest-api-client-4.1.0/authomize_rest_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.0.0/setup.py` & `authomize-rest-api-client-4.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == '__main__':
     setup(
-        version='4.0.0',
+        version='4.1.0',
         name='authomize-rest-api-client',
         author='Authomize inc.',
         license='MIT',
         author_email='info@authomize.com',
         description='Authomize REST API Python Client',
         packages=find_namespace_packages(include=['authomize.*']),
         package_data={
```

