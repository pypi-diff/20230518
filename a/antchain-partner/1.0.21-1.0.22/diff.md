# Comparing `tmp/antchain_partner-1.0.21.tar.gz` & `tmp/antchain_partner-1.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_partner-1.0.21.tar", last modified: Tue Apr 25 03:03:41 2023, max compression
+gzip compressed data, was "dist/antchain_partner-1.0.22.tar", last modified: Thu May 18 02:58:15 2023, max compression
```

## Comparing `antchain_partner-1.0.21.tar` & `antchain_partner-1.0.22.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 03:03:41.000000 antchain_partner-1.0.21/
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-25 03:03:40.000000 antchain_partner-1.0.21/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-25 03:03:40.000000 antchain_partner-1.0.21/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2187 2023-04-25 03:03:41.000000 antchain_partner-1.0.21/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      816 2023-04-25 03:03:40.000000 antchain_partner-1.0.21/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1002 2023-04-25 03:03:40.000000 antchain_partner-1.0.21/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 03:03:41.000000 antchain_partner-1.0.21/antchain_partner.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2187 2023-04-25 03:03:40.000000 antchain_partner-1.0.21/antchain_partner.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      355 2023-04-25 03:03:40.000000 antchain_partner-1.0.21/antchain_partner.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 03:03:40.000000 antchain_partner-1.0.21/antchain_partner.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-04-25 03:03:40.000000 antchain_partner-1.0.21/antchain_partner.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-25 03:03:40.000000 antchain_partner-1.0.21/antchain_partner.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 03:03:41.000000 antchain_partner-1.0.21/antchain_sdk_partner/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-25 03:03:40.000000 antchain_partner-1.0.21/antchain_sdk_partner/__init__.py
--rw-r--r--   0 root         (0) root         (0)    46536 2023-04-25 03:03:40.000000 antchain_partner-1.0.21/antchain_sdk_partner/client.py
--rw-r--r--   0 root         (0) root         (0)   111808 2023-04-25 03:03:40.000000 antchain_partner-1.0.21/antchain_sdk_partner/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-25 03:03:41.000000 antchain_partner-1.0.21/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2508 2023-04-25 03:03:40.000000 antchain_partner-1.0.21/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 02:58:15.000000 antchain_partner-1.0.22/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-18 02:58:15.000000 antchain_partner-1.0.22/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-18 02:58:15.000000 antchain_partner-1.0.22/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2187 2023-05-18 02:58:15.000000 antchain_partner-1.0.22/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      816 2023-05-18 02:58:15.000000 antchain_partner-1.0.22/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-05-18 02:58:15.000000 antchain_partner-1.0.22/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 02:58:15.000000 antchain_partner-1.0.22/antchain_partner.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2187 2023-05-18 02:58:15.000000 antchain_partner-1.0.22/antchain_partner.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      355 2023-05-18 02:58:15.000000 antchain_partner-1.0.22/antchain_partner.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 02:58:15.000000 antchain_partner-1.0.22/antchain_partner.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-18 02:58:15.000000 antchain_partner-1.0.22/antchain_partner.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-18 02:58:15.000000 antchain_partner-1.0.22/antchain_partner.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 02:58:15.000000 antchain_partner-1.0.22/antchain_sdk_partner/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 02:58:15.000000 antchain_partner-1.0.22/antchain_sdk_partner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    46536 2023-05-18 02:58:15.000000 antchain_partner-1.0.22/antchain_sdk_partner/client.py
+-rw-r--r--   0 root         (0) root         (0)   111700 2023-05-18 02:58:15.000000 antchain_partner-1.0.22/antchain_sdk_partner/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-18 02:58:15.000000 antchain_partner-1.0.22/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2508 2023-05-18 02:58:15.000000 antchain_partner-1.0.22/setup.py
```

### Comparing `antchain_partner-1.0.21/LICENSE` & `antchain_partner-1.0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_partner-1.0.21/PKG-INFO` & `antchain_partner-1.0.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_partner
-Version: 1.0.21
+Version: 1.0.22
 Summary: Ant Chain PARTNER SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_partner-1.0.21/README-CN.md` & `antchain_partner-1.0.22/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_partner-1.0.21/README.md` & `antchain_partner-1.0.22/README.md`

 * *Files identical despite different names*

### Comparing `antchain_partner-1.0.21/antchain_partner.egg-info/PKG-INFO` & `antchain_partner-1.0.22/antchain_partner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-partner
-Version: 1.0.21
+Version: 1.0.22
 Summary: Ant Chain PARTNER SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_partner-1.0.21/antchain_sdk_partner/client.py` & `antchain_partner-1.0.22/antchain_sdk_partner/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.21',
+                    'sdk_version': '1.0.22',
                     '_prod_code': 'PARTNER',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.21',
+                    'sdk_version': '1.0.22',
                     '_prod_code': 'PARTNER',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
```

### Comparing `antchain_partner-1.0.21/antchain_sdk_partner/models.py` & `antchain_partner-1.0.22/antchain_sdk_partner/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3072,16 +3072,14 @@
         self.inst_id = inst_id
         # 支行名称关键字
         self.branch_name = branch_name
         # 租户来源-用于租户间功能和数据的隔离
         self.source = source
 
     def validate(self):
-        self.validate_required(self.province, 'province')
-        self.validate_required(self.city, 'city')
         self.validate_required(self.inst_id, 'inst_id')
         self.validate_required(self.branch_name, 'branch_name')
         self.validate_required(self.source, 'source')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
```

### Comparing `antchain_partner-1.0.21/setup.py` & `antchain_partner-1.0.22/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_partner.
 
-Created on 25/04/2023
+Created on 18/05/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_partner"
 NAME = "antchain_partner" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain PARTNER SDK Library for Python"
```

