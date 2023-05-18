# Comparing `tmp/alibabacloud_cloudauth20190307-2.0.5.tar.gz` & `tmp/alibabacloud_cloudauth20190307-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cloudauth20190307-2.0.5.tar", last modified: Wed Nov  2 06:10:13 2022, max compression
+gzip compressed data, was "dist/alibabacloud_cloudauth20190307-2.0.6.tar", last modified: Thu May 18 02:56:41 2023, max compression
```

## Comparing `alibabacloud_cloudauth20190307-2.0.5.tar` & `alibabacloud_cloudauth20190307-2.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-02 06:10:13.000000 alibabacloud_cloudauth20190307-2.0.5/
--rw-r--r--   0 root         (0) root         (0)      711 2022-11-02 06:10:13.000000 alibabacloud_cloudauth20190307-2.0.5/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-11-02 06:10:13.000000 alibabacloud_cloudauth20190307-2.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-11-02 06:10:13.000000 alibabacloud_cloudauth20190307-2.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2370 2022-11-02 06:10:13.000000 alibabacloud_cloudauth20190307-2.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1040 2022-11-02 06:10:13.000000 alibabacloud_cloudauth20190307-2.0.5/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1125 2022-11-02 06:10:13.000000 alibabacloud_cloudauth20190307-2.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-02 06:10:13.000000 alibabacloud_cloudauth20190307-2.0.5/alibabacloud_cloudauth20190307/
--rw-r--r--   0 root         (0) root         (0)       21 2022-11-02 06:10:13.000000 alibabacloud_cloudauth20190307-2.0.5/alibabacloud_cloudauth20190307/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77151 2022-11-02 06:10:13.000000 alibabacloud_cloudauth20190307-2.0.5/alibabacloud_cloudauth20190307/client.py
--rw-r--r--   0 root         (0) root         (0)   128799 2022-11-02 06:10:13.000000 alibabacloud_cloudauth20190307-2.0.5/alibabacloud_cloudauth20190307/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-02 06:10:13.000000 alibabacloud_cloudauth20190307-2.0.5/alibabacloud_cloudauth20190307.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2370 2022-11-02 06:10:13.000000 alibabacloud_cloudauth20190307-2.0.5/alibabacloud_cloudauth20190307.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      468 2022-11-02 06:10:13.000000 alibabacloud_cloudauth20190307-2.0.5/alibabacloud_cloudauth20190307.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-02 06:10:13.000000 alibabacloud_cloudauth20190307-2.0.5/alibabacloud_cloudauth20190307.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      315 2022-11-02 06:10:13.000000 alibabacloud_cloudauth20190307-2.0.5/alibabacloud_cloudauth20190307.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2022-11-02 06:10:13.000000 alibabacloud_cloudauth20190307-2.0.5/alibabacloud_cloudauth20190307.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-11-02 06:10:13.000000 alibabacloud_cloudauth20190307-2.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2837 2022-11-02 06:10:13.000000 alibabacloud_cloudauth20190307-2.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 02:56:41.000000 alibabacloud_cloudauth20190307-2.0.6/
+-rw-r--r--   0 root         (0) root         (0)      756 2023-05-18 02:56:41.000000 alibabacloud_cloudauth20190307-2.0.6/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-18 02:56:41.000000 alibabacloud_cloudauth20190307-2.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-18 02:56:41.000000 alibabacloud_cloudauth20190307-2.0.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2370 2023-05-18 02:56:41.000000 alibabacloud_cloudauth20190307-2.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-05-18 02:56:41.000000 alibabacloud_cloudauth20190307-2.0.6/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-05-18 02:56:41.000000 alibabacloud_cloudauth20190307-2.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 02:56:41.000000 alibabacloud_cloudauth20190307-2.0.6/alibabacloud_cloudauth20190307/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-18 02:56:41.000000 alibabacloud_cloudauth20190307-2.0.6/alibabacloud_cloudauth20190307/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77649 2023-05-18 02:56:41.000000 alibabacloud_cloudauth20190307-2.0.6/alibabacloud_cloudauth20190307/client.py
+-rw-r--r--   0 root         (0) root         (0)   129400 2023-05-18 02:56:41.000000 alibabacloud_cloudauth20190307-2.0.6/alibabacloud_cloudauth20190307/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 02:56:41.000000 alibabacloud_cloudauth20190307-2.0.6/alibabacloud_cloudauth20190307.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2370 2023-05-18 02:56:41.000000 alibabacloud_cloudauth20190307-2.0.6/alibabacloud_cloudauth20190307.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      468 2023-05-18 02:56:41.000000 alibabacloud_cloudauth20190307-2.0.6/alibabacloud_cloudauth20190307.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 02:56:41.000000 alibabacloud_cloudauth20190307-2.0.6/alibabacloud_cloudauth20190307.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      315 2023-05-18 02:56:41.000000 alibabacloud_cloudauth20190307-2.0.6/alibabacloud_cloudauth20190307.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-05-18 02:56:41.000000 alibabacloud_cloudauth20190307-2.0.6/alibabacloud_cloudauth20190307.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-18 02:56:41.000000 alibabacloud_cloudauth20190307-2.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2837 2023-05-18 02:56:41.000000 alibabacloud_cloudauth20190307-2.0.6/setup.py
```

### Comparing `alibabacloud_cloudauth20190307-2.0.5/ChangeLog.md` & `alibabacloud_cloudauth20190307-2.0.6/ChangeLog.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2022-11-02 Version: 2.0.5
+- For 2019-03-07.
+
 2022-10-17 Version: 2.0.4
 - For 2019-03-07.
 
 2022-06-29 Version: 2.0.3
 - For 2019-03-07.
 
 2022-02-23 Version: 1.0.7
```

### Comparing `alibabacloud_cloudauth20190307-2.0.5/LICENSE` & `alibabacloud_cloudauth20190307-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth20190307-2.0.5/PKG-INFO` & `alibabacloud_cloudauth20190307-2.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cloudauth20190307
-Version: 2.0.5
+Version: 2.0.6
 Summary: Alibaba Cloud ID Verification (20190307) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloudauth20190307-2.0.5/README-CN.md` & `alibabacloud_cloudauth20190307-2.0.6/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth20190307-2.0.5/README.md` & `alibabacloud_cloudauth20190307-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth20190307-2.0.5/alibabacloud_cloudauth20190307/client.py` & `alibabacloud_cloudauth20190307-2.0.6/alibabacloud_cloudauth20190307/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1310,20 +1310,24 @@
             query['Mobile'] = request.mobile
         if not UtilClient.is_unset(request.oss_bucket_name):
             query['OssBucketName'] = request.oss_bucket_name
         if not UtilClient.is_unset(request.oss_object_name):
             query['OssObjectName'] = request.oss_object_name
         if not UtilClient.is_unset(request.outer_order_no):
             query['OuterOrderNo'] = request.outer_order_no
+        if not UtilClient.is_unset(request.procedure_priority):
+            query['ProcedurePriority'] = request.procedure_priority
         if not UtilClient.is_unset(request.product_code):
             query['ProductCode'] = request.product_code
         if not UtilClient.is_unset(request.return_url):
             query['ReturnUrl'] = request.return_url
         if not UtilClient.is_unset(request.scene_id):
             query['SceneId'] = request.scene_id
+        if not UtilClient.is_unset(request.suitable_type):
+            query['SuitableType'] = request.suitable_type
         if not UtilClient.is_unset(request.user_id):
             query['UserId'] = request.user_id
         if not UtilClient.is_unset(request.voluntary_customized_content):
             query['VoluntaryCustomizedContent'] = request.voluntary_customized_content
         body = {}
         if not UtilClient.is_unset(request.auth_id):
             body['AuthId'] = request.auth_id
@@ -1386,20 +1390,24 @@
             query['Mobile'] = request.mobile
         if not UtilClient.is_unset(request.oss_bucket_name):
             query['OssBucketName'] = request.oss_bucket_name
         if not UtilClient.is_unset(request.oss_object_name):
             query['OssObjectName'] = request.oss_object_name
         if not UtilClient.is_unset(request.outer_order_no):
             query['OuterOrderNo'] = request.outer_order_no
+        if not UtilClient.is_unset(request.procedure_priority):
+            query['ProcedurePriority'] = request.procedure_priority
         if not UtilClient.is_unset(request.product_code):
             query['ProductCode'] = request.product_code
         if not UtilClient.is_unset(request.return_url):
             query['ReturnUrl'] = request.return_url
         if not UtilClient.is_unset(request.scene_id):
             query['SceneId'] = request.scene_id
+        if not UtilClient.is_unset(request.suitable_type):
+            query['SuitableType'] = request.suitable_type
         if not UtilClient.is_unset(request.user_id):
             query['UserId'] = request.user_id
         if not UtilClient.is_unset(request.voluntary_customized_content):
             query['VoluntaryCustomizedContent'] = request.voluntary_customized_content
         body = {}
         if not UtilClient.is_unset(request.auth_id):
             body['AuthId'] = request.auth_id
```

### Comparing `alibabacloud_cloudauth20190307-2.0.5/alibabacloud_cloudauth20190307/models.py` & `alibabacloud_cloudauth20190307-2.0.6/alibabacloud_cloudauth20190307/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2779,17 +2779,19 @@
         ip: str = None,
         meta_info: str = None,
         mobile: str = None,
         model: str = None,
         oss_bucket_name: str = None,
         oss_object_name: str = None,
         outer_order_no: str = None,
+        procedure_priority: str = None,
         product_code: str = None,
         return_url: str = None,
         scene_id: int = None,
+        suitable_type: str = None,
         user_id: str = None,
         voluntary_customized_content: str = None,
     ):
         self.auth_id = auth_id
         self.callback_token = callback_token
         self.callback_url = callback_url
         self.cert_name = cert_name
@@ -2804,17 +2806,19 @@
         self.ip = ip
         self.meta_info = meta_info
         self.mobile = mobile
         self.model = model
         self.oss_bucket_name = oss_bucket_name
         self.oss_object_name = oss_object_name
         self.outer_order_no = outer_order_no
+        self.procedure_priority = procedure_priority
         self.product_code = product_code
         self.return_url = return_url
         self.scene_id = scene_id
+        self.suitable_type = suitable_type
         self.user_id = user_id
         self.voluntary_customized_content = voluntary_customized_content
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -2857,20 +2861,24 @@
             result['Model'] = self.model
         if self.oss_bucket_name is not None:
             result['OssBucketName'] = self.oss_bucket_name
         if self.oss_object_name is not None:
             result['OssObjectName'] = self.oss_object_name
         if self.outer_order_no is not None:
             result['OuterOrderNo'] = self.outer_order_no
+        if self.procedure_priority is not None:
+            result['ProcedurePriority'] = self.procedure_priority
         if self.product_code is not None:
             result['ProductCode'] = self.product_code
         if self.return_url is not None:
             result['ReturnUrl'] = self.return_url
         if self.scene_id is not None:
             result['SceneId'] = self.scene_id
+        if self.suitable_type is not None:
+            result['SuitableType'] = self.suitable_type
         if self.user_id is not None:
             result['UserId'] = self.user_id
         if self.voluntary_customized_content is not None:
             result['VoluntaryCustomizedContent'] = self.voluntary_customized_content
         return result
 
     def from_map(self, m: dict = None):
@@ -2909,20 +2917,24 @@
             self.model = m.get('Model')
         if m.get('OssBucketName') is not None:
             self.oss_bucket_name = m.get('OssBucketName')
         if m.get('OssObjectName') is not None:
             self.oss_object_name = m.get('OssObjectName')
         if m.get('OuterOrderNo') is not None:
             self.outer_order_no = m.get('OuterOrderNo')
+        if m.get('ProcedurePriority') is not None:
+            self.procedure_priority = m.get('ProcedurePriority')
         if m.get('ProductCode') is not None:
             self.product_code = m.get('ProductCode')
         if m.get('ReturnUrl') is not None:
             self.return_url = m.get('ReturnUrl')
         if m.get('SceneId') is not None:
             self.scene_id = m.get('SceneId')
+        if m.get('SuitableType') is not None:
+            self.suitable_type = m.get('SuitableType')
         if m.get('UserId') is not None:
             self.user_id = m.get('UserId')
         if m.get('VoluntaryCustomizedContent') is not None:
             self.voluntary_customized_content = m.get('VoluntaryCustomizedContent')
         return self
```

### Comparing `alibabacloud_cloudauth20190307-2.0.5/alibabacloud_cloudauth20190307.egg-info/PKG-INFO` & `alibabacloud_cloudauth20190307-2.0.6/alibabacloud_cloudauth20190307.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cloudauth20190307
-Version: 2.0.5
+Version: 2.0.6
 Summary: Alibaba Cloud ID Verification (20190307) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloudauth20190307-2.0.5/setup.py` & `alibabacloud_cloudauth20190307-2.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,34 +20,34 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cloudauth20190307.
 
-Created on 02/11/2022
+Created on 18/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cloudauth20190307"
 NAME = "alibabacloud_cloudauth20190307" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ID Verification (20190307) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.6, <1.0.0",
+    "alibabacloud_tea_util>=0.3.8, <1.0.0",
     "alibabacloud_oss_sdk>=0.1.0, <1.0.0",
     "alibabacloud_openplatform20191219>=2.0.0, <3.0.0",
     "alibabacloud_oss_util>=0.0.5, <1.0.0",
     "alibabacloud_tea_fileform>=0.0.3, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.5, <1.0.0",
-    "alibabacloud_openapi_util>=0.1.6, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

