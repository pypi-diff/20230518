# Comparing `tmp/antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.1.tar.gz` & `tmp/antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.1.tar", last modified: Tue May 16 03:19:34 2023, max compression
+gzip compressed data, was "dist/antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.2.tar", last modified: Thu May 18 08:47:27 2023, max compression
```

## Comparing `antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.1.tar` & `antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 03:19:34.000000 antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.1/
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-16 03:19:33.000000 antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-16 03:19:33.000000 antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2354 2023-05-16 03:19:34.000000 antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      900 2023-05-16 03:19:33.000000 antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1086 2023-05-16 03:19:33.000000 antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 03:19:34.000000 antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.1/antchain_ak_de45e14cba2c4defbab7659a63578373.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2354 2023-05-16 03:19:34.000000 antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.1/antchain_ak_de45e14cba2c4defbab7659a63578373.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      579 2023-05-16 03:19:34.000000 antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.1/antchain_ak_de45e14cba2c4defbab7659a63578373.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 03:19:34.000000 antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.1/antchain_ak_de45e14cba2c4defbab7659a63578373.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-05-16 03:19:34.000000 antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.1/antchain_ak_de45e14cba2c4defbab7659a63578373.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-05-16 03:19:34.000000 antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.1/antchain_ak_de45e14cba2c4defbab7659a63578373.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 03:19:34.000000 antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.1/antchain_sdk_ak_de45e14cba2c4defbab7659a63578373/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-16 03:19:33.000000 antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.1/antchain_sdk_ak_de45e14cba2c4defbab7659a63578373/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15376 2023-05-16 03:19:33.000000 antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.1/antchain_sdk_ak_de45e14cba2c4defbab7659a63578373/client.py
--rw-r--r--   0 root         (0) root         (0)     8890 2023-05-16 03:19:33.000000 antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.1/antchain_sdk_ak_de45e14cba2c4defbab7659a63578373/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-16 03:19:34.000000 antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2650 2023-05-16 03:19:33.000000 antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 08:47:27.000000 antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-18 08:47:26.000000 antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-18 08:47:26.000000 antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-05-18 08:47:27.000000 antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      900 2023-05-18 08:47:26.000000 antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-05-18 08:47:26.000000 antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 08:47:27.000000 antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.2/antchain_ak_de45e14cba2c4defbab7659a63578373.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-05-18 08:47:27.000000 antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.2/antchain_ak_de45e14cba2c4defbab7659a63578373.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      579 2023-05-18 08:47:27.000000 antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.2/antchain_ak_de45e14cba2c4defbab7659a63578373.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 08:47:27.000000 antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.2/antchain_ak_de45e14cba2c4defbab7659a63578373.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-18 08:47:27.000000 antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.2/antchain_ak_de45e14cba2c4defbab7659a63578373.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-18 08:47:27.000000 antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.2/antchain_ak_de45e14cba2c4defbab7659a63578373.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 08:47:27.000000 antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.2/antchain_sdk_ak_de45e14cba2c4defbab7659a63578373/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-18 08:47:26.000000 antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.2/antchain_sdk_ak_de45e14cba2c4defbab7659a63578373/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18030 2023-05-18 08:47:26.000000 antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.2/antchain_sdk_ak_de45e14cba2c4defbab7659a63578373/client.py
+-rw-r--r--   0 root         (0) root         (0)    11373 2023-05-18 08:47:26.000000 antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.2/antchain_sdk_ak_de45e14cba2c4defbab7659a63578373/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-18 08:47:27.000000 antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2650 2023-05-18 08:47:26.000000 antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.2/setup.py
```

### Comparing `antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.1/LICENSE` & `antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.1/PKG-INFO` & `antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_ak_de45e14cba2c4defbab7659a63578373
-Version: 1.0.1
+Version: 1.0.2
 Summary: Ant Chain Ak_de45e14cba2c4defbab7659a63578373 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.1/README-CN.md` & `antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.1/README.md` & `antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.1/antchain_ak_de45e14cba2c4defbab7659a63578373.egg-info/PKG-INFO` & `antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.2/antchain_ak_de45e14cba2c4defbab7659a63578373.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-ak-de45e14cba2c4defbab7659a63578373
-Version: 1.0.1
+Version: 1.0.2
 Summary: Ant Chain Ak_de45e14cba2c4defbab7659a63578373 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.1/antchain_ak_de45e14cba2c4defbab7659a63578373.egg-info/SOURCES.txt` & `antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.2/antchain_ak_de45e14cba2c4defbab7659a63578373.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.1/antchain_sdk_ak_de45e14cba2c4defbab7659a63578373/models.py` & `antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.2/antchain_sdk_ak_de45e14cba2c4defbab7659a63578373/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -149,71 +149,71 @@
         if m.get('maxRequests') is not None:
             self.max_requests = m.get('maxRequests')
         if m.get('maxRequestsPerHost') is not None:
             self.max_requests_per_host = m.get('maxRequestsPerHost')
         return self
 
 
-class QueryDemoApprovalTestRequest(TeaModel):
+class CreateDemoSaasTestTesthRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
-        input: str = None,
+        name: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
-        # 字符串
-        self.input = input
+        # test
+        self.name = name
 
     def validate(self):
-        self.validate_required(self.input, 'input')
+        self.validate_required(self.name, 'name')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
-        if self.input is not None:
-            result['input'] = self.input
+        if self.name is not None:
+            result['name'] = self.name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
-        if m.get('input') is not None:
-            self.input = m.get('input')
+        if m.get('name') is not None:
+            self.name = m.get('name')
         return self
 
 
-class QueryDemoApprovalTestResponse(TeaModel):
+class CreateDemoSaasTestTesthResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
-        msg: str = None,
+        name: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
-        # 回参
-        self.msg = msg
+        # test
+        self.name = name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -222,24 +222,107 @@
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
-        if self.msg is not None:
-            result['msg'] = self.msg
+        if self.name is not None:
+            result['name'] = self.name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
-        if m.get('msg') is not None:
-            self.msg = m.get('msg')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        return self
+
+
+class CreateDemoSaasTestTestiRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        return self
+
+
+class CreateDemoSaasTestTestiResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        sex: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # test
+        self.sex = sex
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.sex is not None:
+            result['sex'] = self.sex
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('sex') is not None:
+            self.sex = m.get('sex')
         return self
```

### Comparing `antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.1/setup.py` & `antchain_ak_de45e14cba2c4defbab7659a63578373-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_ak_de45e14cba2c4defbab7659a63578373.
 
-Created on 16/05/2023
+Created on 18/05/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_ak_de45e14cba2c4defbab7659a63578373"
 NAME = "antchain_ak_de45e14cba2c4defbab7659a63578373" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain Ak_de45e14cba2c4defbab7659a63578373 SDK Library for Python"
```

