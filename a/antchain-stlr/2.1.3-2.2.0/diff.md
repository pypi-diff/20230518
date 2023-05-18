# Comparing `tmp/antchain_stlr-2.1.3.tar.gz` & `tmp/antchain_stlr-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_stlr-2.1.3.tar", last modified: Fri Feb 10 08:16:10 2023, max compression
+gzip compressed data, was "dist/antchain_stlr-2.2.0.tar", last modified: Thu May 18 01:53:42 2023, max compression
```

## Comparing `antchain_stlr-2.1.3.tar` & `antchain_stlr-2.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 08:16:10.000000 antchain_stlr-2.1.3/
--rw-r--r--   0 root         (0) root         (0)      600 2023-02-10 08:16:10.000000 antchain_stlr-2.1.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-02-10 08:16:10.000000 antchain_stlr-2.1.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2168 2023-02-10 08:16:10.000000 antchain_stlr-2.1.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      807 2023-02-10 08:16:10.000000 antchain_stlr-2.1.3/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      993 2023-02-10 08:16:10.000000 antchain_stlr-2.1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 08:16:10.000000 antchain_stlr-2.1.3/antchain_sdk_stlr/
--rw-r--r--   0 root         (0) root         (0)       21 2023-02-10 08:16:10.000000 antchain_stlr-2.1.3/antchain_sdk_stlr/__init__.py
--rw-r--r--   0 root         (0) root         (0)    84431 2023-02-10 08:16:10.000000 antchain_stlr-2.1.3/antchain_sdk_stlr/client.py
--rw-r--r--   0 root         (0) root         (0)   199653 2023-02-10 08:16:10.000000 antchain_stlr-2.1.3/antchain_sdk_stlr/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 08:16:10.000000 antchain_stlr-2.1.3/antchain_stlr.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2168 2023-02-10 08:16:10.000000 antchain_stlr-2.1.3/antchain_stlr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      331 2023-02-10 08:16:10.000000 antchain_stlr-2.1.3/antchain_stlr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-10 08:16:10.000000 antchain_stlr-2.1.3/antchain_stlr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-02-10 08:16:10.000000 antchain_stlr-2.1.3/antchain_stlr.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-02-10 08:16:10.000000 antchain_stlr-2.1.3/antchain_stlr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-02-10 08:16:10.000000 antchain_stlr-2.1.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2493 2023-02-10 08:16:10.000000 antchain_stlr-2.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 01:53:42.000000 antchain_stlr-2.2.0/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-18 01:53:42.000000 antchain_stlr-2.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-18 01:53:42.000000 antchain_stlr-2.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-05-18 01:53:42.000000 antchain_stlr-2.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      807 2023-05-18 01:53:42.000000 antchain_stlr-2.2.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      993 2023-05-18 01:53:42.000000 antchain_stlr-2.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 01:53:42.000000 antchain_stlr-2.2.0/antchain_sdk_stlr/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-18 01:53:42.000000 antchain_stlr-2.2.0/antchain_sdk_stlr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    96687 2023-05-18 01:53:42.000000 antchain_stlr-2.2.0/antchain_sdk_stlr/client.py
+-rw-r--r--   0 root         (0) root         (0)   229400 2023-05-18 01:53:42.000000 antchain_stlr-2.2.0/antchain_sdk_stlr/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 01:53:42.000000 antchain_stlr-2.2.0/antchain_stlr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-05-18 01:53:42.000000 antchain_stlr-2.2.0/antchain_stlr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      331 2023-05-18 01:53:42.000000 antchain_stlr-2.2.0/antchain_stlr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 01:53:42.000000 antchain_stlr-2.2.0/antchain_stlr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-18 01:53:42.000000 antchain_stlr-2.2.0/antchain_stlr.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-18 01:53:42.000000 antchain_stlr-2.2.0/antchain_stlr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-18 01:53:42.000000 antchain_stlr-2.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2493 2023-05-18 01:53:42.000000 antchain_stlr-2.2.0/setup.py
```

### Comparing `antchain_stlr-2.1.3/LICENSE` & `antchain_stlr-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_stlr-2.1.3/PKG-INFO` & `antchain_stlr-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_stlr
-Version: 2.1.3
+Version: 2.2.0
 Summary: Ant Chain STLR SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_stlr-2.1.3/README-CN.md` & `antchain_stlr-2.2.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_stlr-2.1.3/README.md` & `antchain_stlr-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `antchain_stlr-2.1.3/antchain_sdk_stlr/client.py` & `antchain_stlr-2.2.0/antchain_sdk_stlr/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,27 +94,27 @@
             'readTimeout': UtilClient.default_number(runtime.read_timeout, self._read_timeout),
             'connectTimeout': UtilClient.default_number(runtime.connect_timeout, self._connect_timeout),
             'httpProxy': UtilClient.default_string(runtime.http_proxy, self._http_proxy),
             'httpsProxy': UtilClient.default_string(runtime.https_proxy, self._https_proxy),
             'noProxy': UtilClient.default_string(runtime.no_proxy, self._no_proxy),
             'maxIdleConns': UtilClient.default_number(runtime.max_idle_conns, self._max_idle_conns),
             'maxIdleTimeMillis': self._max_idle_time_millis,
-            'keepAliveDurationMillis': self._keep_alive_duration_millis,
+            'keepAliveDuration': self._keep_alive_duration_millis,
             'maxRequests': self._max_requests,
             'maxRequestsPerHost': self._max_requests_per_host,
             'retry': {
                 'retryable': runtime.autoretry,
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
                 'policy': UtilClient.default_string(runtime.backoff_policy, 'no'),
                 'period': UtilClient.default_number(runtime.backoff_period, 1)
             },
             'ignoreSSL': runtime.ignore_ssl,
-            # 证书授权产品信息
+            # 数据值条目
         }
         _last_request = None
         _last_exception = None
         _now = time.time()
         _retry_times = 0
         while TeaCore.allow_retry(_runtime.get('retry'), _retry_times, _now):
             if _retry_times > 0:
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '2.1.3',
+                    'sdk_version': '2.2.0',
                     '_prod_code': 'STLR',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -198,27 +198,27 @@
             'readTimeout': UtilClient.default_number(runtime.read_timeout, self._read_timeout),
             'connectTimeout': UtilClient.default_number(runtime.connect_timeout, self._connect_timeout),
             'httpProxy': UtilClient.default_string(runtime.http_proxy, self._http_proxy),
             'httpsProxy': UtilClient.default_string(runtime.https_proxy, self._https_proxy),
             'noProxy': UtilClient.default_string(runtime.no_proxy, self._no_proxy),
             'maxIdleConns': UtilClient.default_number(runtime.max_idle_conns, self._max_idle_conns),
             'maxIdleTimeMillis': self._max_idle_time_millis,
-            'keepAliveDurationMillis': self._keep_alive_duration_millis,
+            'keepAliveDuration': self._keep_alive_duration_millis,
             'maxRequests': self._max_requests,
             'maxRequestsPerHost': self._max_requests_per_host,
             'retry': {
                 'retryable': runtime.autoretry,
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
                 'policy': UtilClient.default_string(runtime.backoff_policy, 'no'),
                 'period': UtilClient.default_number(runtime.backoff_period, 1)
             },
             'ignoreSSL': runtime.ignore_ssl,
-            # 证书授权产品信息
+            # 数据值条目
         }
         _last_request = None
         _last_exception = None
         _now = time.time()
         _retry_times = 0
         while TeaCore.allow_retry(_runtime.get('retry'), _retry_times, _now):
             if _retry_times > 0:
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '2.1.3',
+                    'sdk_version': '2.2.0',
                     '_prod_code': 'STLR',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -1929,14 +1929,294 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             stlr_models.PreviewEcarAvitivedataResponse(),
             await self.do_request_async('1.0', 'antchain.carbon.ecar.avitivedata.preview', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def register_ecar_enterprisemember(
+        self,
+        request: stlr_models.RegisterEcarEnterprisememberRequest,
+    ) -> stlr_models.RegisterEcarEnterprisememberResponse:
+        """
+        Description: 机构会员注册接口，支持根据蚂蚁DID或者姓名+密码注意企业的终端会员
+        Summary: 机构会员注册
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.register_ecar_enterprisemember_ex(request, headers, runtime)
+
+    async def register_ecar_enterprisemember_async(
+        self,
+        request: stlr_models.RegisterEcarEnterprisememberRequest,
+    ) -> stlr_models.RegisterEcarEnterprisememberResponse:
+        """
+        Description: 机构会员注册接口，支持根据蚂蚁DID或者姓名+密码注意企业的终端会员
+        Summary: 机构会员注册
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.register_ecar_enterprisemember_ex_async(request, headers, runtime)
+
+    def register_ecar_enterprisemember_ex(
+        self,
+        request: stlr_models.RegisterEcarEnterprisememberRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.RegisterEcarEnterprisememberResponse:
+        """
+        Description: 机构会员注册接口，支持根据蚂蚁DID或者姓名+密码注意企业的终端会员
+        Summary: 机构会员注册
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.RegisterEcarEnterprisememberResponse(),
+            self.do_request('1.0', 'antchain.carbon.ecar.enterprisemember.register', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def register_ecar_enterprisemember_ex_async(
+        self,
+        request: stlr_models.RegisterEcarEnterprisememberRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.RegisterEcarEnterprisememberResponse:
+        """
+        Description: 机构会员注册接口，支持根据蚂蚁DID或者姓名+密码注意企业的终端会员
+        Summary: 机构会员注册
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.RegisterEcarEnterprisememberResponse(),
+            await self.do_request_async('1.0', 'antchain.carbon.ecar.enterprisemember.register', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def add_ecar_offsetacquisition(
+        self,
+        request: stlr_models.AddEcarOffsetacquisitionRequest,
+    ) -> stlr_models.AddEcarOffsetacquisitionResponse:
+        """
+        Description: 碳补偿数据采集，提供给碳普惠业务相关接口，外围系统提交碳普惠数据
+        Summary: 碳补偿数据采集
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.add_ecar_offsetacquisition_ex(request, headers, runtime)
+
+    async def add_ecar_offsetacquisition_async(
+        self,
+        request: stlr_models.AddEcarOffsetacquisitionRequest,
+    ) -> stlr_models.AddEcarOffsetacquisitionResponse:
+        """
+        Description: 碳补偿数据采集，提供给碳普惠业务相关接口，外围系统提交碳普惠数据
+        Summary: 碳补偿数据采集
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.add_ecar_offsetacquisition_ex_async(request, headers, runtime)
+
+    def add_ecar_offsetacquisition_ex(
+        self,
+        request: stlr_models.AddEcarOffsetacquisitionRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.AddEcarOffsetacquisitionResponse:
+        """
+        Description: 碳补偿数据采集，提供给碳普惠业务相关接口，外围系统提交碳普惠数据
+        Summary: 碳补偿数据采集
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.AddEcarOffsetacquisitionResponse(),
+            self.do_request('1.0', 'antchain.carbon.ecar.offsetacquisition.add', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def add_ecar_offsetacquisition_ex_async(
+        self,
+        request: stlr_models.AddEcarOffsetacquisitionRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.AddEcarOffsetacquisitionResponse:
+        """
+        Description: 碳补偿数据采集，提供给碳普惠业务相关接口，外围系统提交碳普惠数据
+        Summary: 碳补偿数据采集
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.AddEcarOffsetacquisitionResponse(),
+            await self.do_request_async('1.0', 'antchain.carbon.ecar.offsetacquisition.add', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def add_ecar_offsettranslate(
+        self,
+        request: stlr_models.AddEcarOffsettranslateRequest,
+    ) -> stlr_models.AddEcarOffsettranslateResponse:
+        """
+        Description: 碳普惠减碳量转移，减碳量在业务端兑换成权益的场景时可使用此接口
+        Summary: 碳普惠减碳量转移
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.add_ecar_offsettranslate_ex(request, headers, runtime)
+
+    async def add_ecar_offsettranslate_async(
+        self,
+        request: stlr_models.AddEcarOffsettranslateRequest,
+    ) -> stlr_models.AddEcarOffsettranslateResponse:
+        """
+        Description: 碳普惠减碳量转移，减碳量在业务端兑换成权益的场景时可使用此接口
+        Summary: 碳普惠减碳量转移
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.add_ecar_offsettranslate_ex_async(request, headers, runtime)
+
+    def add_ecar_offsettranslate_ex(
+        self,
+        request: stlr_models.AddEcarOffsettranslateRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.AddEcarOffsettranslateResponse:
+        """
+        Description: 碳普惠减碳量转移，减碳量在业务端兑换成权益的场景时可使用此接口
+        Summary: 碳普惠减碳量转移
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.AddEcarOffsettranslateResponse(),
+            self.do_request('1.0', 'antchain.carbon.ecar.offsettranslate.add', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def add_ecar_offsettranslate_ex_async(
+        self,
+        request: stlr_models.AddEcarOffsettranslateRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.AddEcarOffsettranslateResponse:
+        """
+        Description: 碳普惠减碳量转移，减碳量在业务端兑换成权益的场景时可使用此接口
+        Summary: 碳普惠减碳量转移
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.AddEcarOffsettranslateResponse(),
+            await self.do_request_async('1.0', 'antchain.carbon.ecar.offsettranslate.add', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def auth_ecar_offsetdatum(
+        self,
+        request: stlr_models.AuthEcarOffsetdatumRequest,
+    ) -> stlr_models.AuthEcarOffsetdatumResponse:
+        """
+        Description: 碳普惠数据授权，授权三方平台租户可访问相关平台方会员的碳普惠数据
+        Summary: 碳普惠数据授权
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.auth_ecar_offsetdatum_ex(request, headers, runtime)
+
+    async def auth_ecar_offsetdatum_async(
+        self,
+        request: stlr_models.AuthEcarOffsetdatumRequest,
+    ) -> stlr_models.AuthEcarOffsetdatumResponse:
+        """
+        Description: 碳普惠数据授权，授权三方平台租户可访问相关平台方会员的碳普惠数据
+        Summary: 碳普惠数据授权
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.auth_ecar_offsetdatum_ex_async(request, headers, runtime)
+
+    def auth_ecar_offsetdatum_ex(
+        self,
+        request: stlr_models.AuthEcarOffsetdatumRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.AuthEcarOffsetdatumResponse:
+        """
+        Description: 碳普惠数据授权，授权三方平台租户可访问相关平台方会员的碳普惠数据
+        Summary: 碳普惠数据授权
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.AuthEcarOffsetdatumResponse(),
+            self.do_request('1.0', 'antchain.carbon.ecar.offsetdatum.auth', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def auth_ecar_offsetdatum_ex_async(
+        self,
+        request: stlr_models.AuthEcarOffsetdatumRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.AuthEcarOffsetdatumResponse:
+        """
+        Description: 碳普惠数据授权，授权三方平台租户可访问相关平台方会员的碳普惠数据
+        Summary: 碳普惠数据授权
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.AuthEcarOffsetdatumResponse(),
+            await self.do_request_async('1.0', 'antchain.carbon.ecar.offsetdatum.auth', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def list_ecar_offsetdatum(
+        self,
+        request: stlr_models.ListEcarOffsetdatumRequest,
+    ) -> stlr_models.ListEcarOffsetdatumResponse:
+        """
+        Description: 碳普惠数据列表查询，根据账户DID和日期查询碳补偿数据
+        Summary: 碳普惠数据列表查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.list_ecar_offsetdatum_ex(request, headers, runtime)
+
+    async def list_ecar_offsetdatum_async(
+        self,
+        request: stlr_models.ListEcarOffsetdatumRequest,
+    ) -> stlr_models.ListEcarOffsetdatumResponse:
+        """
+        Description: 碳普惠数据列表查询，根据账户DID和日期查询碳补偿数据
+        Summary: 碳普惠数据列表查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.list_ecar_offsetdatum_ex_async(request, headers, runtime)
+
+    def list_ecar_offsetdatum_ex(
+        self,
+        request: stlr_models.ListEcarOffsetdatumRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.ListEcarOffsetdatumResponse:
+        """
+        Description: 碳普惠数据列表查询，根据账户DID和日期查询碳补偿数据
+        Summary: 碳普惠数据列表查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.ListEcarOffsetdatumResponse(),
+            self.do_request('1.0', 'antchain.carbon.ecar.offsetdatum.list', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def list_ecar_offsetdatum_ex_async(
+        self,
+        request: stlr_models.ListEcarOffsetdatumRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.ListEcarOffsetdatumResponse:
+        """
+        Description: 碳普惠数据列表查询，根据账户DID和日期查询碳补偿数据
+        Summary: 碳普惠数据列表查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.ListEcarOffsetdatumResponse(),
+            await self.do_request_async('1.0', 'antchain.carbon.ecar.offsetdatum.list', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def query_third_cert(
         self,
         request: stlr_models.QueryThirdCertRequest,
     ) -> stlr_models.QueryThirdCertResponse:
         """
         Description: 三方平台调用此接口，查询用户的证书信息
         Summary: 证书查询
```

### Comparing `antchain_stlr-2.1.3/antchain_sdk_stlr/models.py` & `antchain_stlr-2.2.0/antchain_sdk_stlr/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -150,14 +150,50 @@
         if m.get('maxRequests') is not None:
             self.max_requests = m.get('maxRequests')
         if m.get('maxRequestsPerHost') is not None:
             self.max_requests_per_host = m.get('maxRequestsPerHost')
         return self
 
 
+class AnyAmountItem(TeaModel):
+    def __init__(
+        self,
+        item_code: str = None,
+        item_amount: str = None,
+    ):
+        # 数据项编码
+        self.item_code = item_code
+        # 数据值，按字符串输出，最多保留6位小数
+        self.item_amount = item_amount
+
+    def validate(self):
+        self.validate_required(self.item_code, 'item_code')
+        self.validate_required(self.item_amount, 'item_amount')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.item_code is not None:
+            result['item_code'] = self.item_code
+        if self.item_amount is not None:
+            result['item_amount'] = self.item_amount
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('item_code') is not None:
+            self.item_code = m.get('item_code')
+        if m.get('item_amount') is not None:
+            self.item_amount = m.get('item_amount')
+        return self
+
+
 class CertProductAuthDO(TeaModel):
     def __init__(
         self,
         product_id: str = None,
         product_name: str = None,
     ):
         # 三方平台产品ID
@@ -813,14 +849,120 @@
         if m.get('tx_hash') is not None:
             self.tx_hash = m.get('tx_hash')
         if m.get('block_number') is not None:
             self.block_number = m.get('block_number')
         return self
 
 
+class CarbonOffsetAcquisitionItem(TeaModel):
+    def __init__(
+        self,
+        acquisition_item_no: str = None,
+        project_no: str = None,
+        account_did: str = None,
+        occurrent_time: str = None,
+        scenario_code: str = None,
+        scenario_name: str = None,
+        platform_no: str = None,
+        active_datum: List[AnyAmountItem] = None,
+        offset_volume: int = None,
+        carbon_energy: int = None,
+    ):
+        # 采集数据单号
+        self.acquisition_item_no = acquisition_item_no
+        # 碳补偿项目编号
+        self.project_no = project_no
+        # 参与账户DID
+        self.account_did = account_did
+        # 发生时间
+        self.occurrent_time = occurrent_time
+        # 发生场景编码
+        self.scenario_code = scenario_code
+        # 发生场景名称
+        self.scenario_name = scenario_name
+        # 碳普惠平台编码，如果非平台采集数据，则显示为自采编码：Self
+        self.platform_no = platform_no
+        # 活动数据原始值，多个活动数据列表
+        self.active_datum = active_datum
+        # 减碳量
+        self.offset_volume = offset_volume
+        # 碳能量值
+        self.carbon_energy = carbon_energy
+
+    def validate(self):
+        self.validate_required(self.acquisition_item_no, 'acquisition_item_no')
+        self.validate_required(self.project_no, 'project_no')
+        self.validate_required(self.account_did, 'account_did')
+        self.validate_required(self.occurrent_time, 'occurrent_time')
+        self.validate_required(self.scenario_code, 'scenario_code')
+        self.validate_required(self.scenario_name, 'scenario_name')
+        self.validate_required(self.platform_no, 'platform_no')
+        if self.active_datum:
+            for k in self.active_datum:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.acquisition_item_no is not None:
+            result['acquisition_item_no'] = self.acquisition_item_no
+        if self.project_no is not None:
+            result['project_no'] = self.project_no
+        if self.account_did is not None:
+            result['account_did'] = self.account_did
+        if self.occurrent_time is not None:
+            result['occurrent_time'] = self.occurrent_time
+        if self.scenario_code is not None:
+            result['scenario_code'] = self.scenario_code
+        if self.scenario_name is not None:
+            result['scenario_name'] = self.scenario_name
+        if self.platform_no is not None:
+            result['platform_no'] = self.platform_no
+        result['active_datum'] = []
+        if self.active_datum is not None:
+            for k in self.active_datum:
+                result['active_datum'].append(k.to_map() if k else None)
+        if self.offset_volume is not None:
+            result['offset_volume'] = self.offset_volume
+        if self.carbon_energy is not None:
+            result['carbon_energy'] = self.carbon_energy
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('acquisition_item_no') is not None:
+            self.acquisition_item_no = m.get('acquisition_item_no')
+        if m.get('project_no') is not None:
+            self.project_no = m.get('project_no')
+        if m.get('account_did') is not None:
+            self.account_did = m.get('account_did')
+        if m.get('occurrent_time') is not None:
+            self.occurrent_time = m.get('occurrent_time')
+        if m.get('scenario_code') is not None:
+            self.scenario_code = m.get('scenario_code')
+        if m.get('scenario_name') is not None:
+            self.scenario_name = m.get('scenario_name')
+        if m.get('platform_no') is not None:
+            self.platform_no = m.get('platform_no')
+        self.active_datum = []
+        if m.get('active_datum') is not None:
+            for k in m.get('active_datum'):
+                temp_model = AnyAmountItem()
+                self.active_datum.append(temp_model.from_map(k))
+        if m.get('offset_volume') is not None:
+            self.offset_volume = m.get('offset_volume')
+        if m.get('carbon_energy') is not None:
+            self.carbon_energy = m.get('carbon_energy')
+        return self
+
+
 class EmissionsCityStatistics(TeaModel):
     def __init__(
         self,
         city_no: str = None,
         city_name: str = None,
         emission_amount: str = None,
         emission_amount_today: str = None,
@@ -989,50 +1131,14 @@
         if m.get('authentication_deetail') is not None:
             self.authentication_deetail = m.get('authentication_deetail')
         if m.get('status') is not None:
             self.status = m.get('status')
         return self
 
 
-class AnyAmountItem(TeaModel):
-    def __init__(
-        self,
-        item_code: str = None,
-        item_amount: str = None,
-    ):
-        # 数据项编码
-        self.item_code = item_code
-        # 数据值，按字符串输出，最多保留6位小数
-        self.item_amount = item_amount
-
-    def validate(self):
-        self.validate_required(self.item_code, 'item_code')
-        self.validate_required(self.item_amount, 'item_amount')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.item_code is not None:
-            result['item_code'] = self.item_code
-        if self.item_amount is not None:
-            result['item_amount'] = self.item_amount
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('item_code') is not None:
-            self.item_code = m.get('item_code')
-        if m.get('item_amount') is not None:
-            self.item_amount = m.get('item_amount')
-        return self
-
-
 class EmissionsScopeStatistics(TeaModel):
     def __init__(
         self,
         inventory_scope_no: str = None,
         inventory_scope_name: str = None,
         emissions: int = None,
         percentage: int = None,
@@ -5018,14 +5124,678 @@
         if m.get('list') is not None:
             for k in m.get('list'):
                 temp_model = AnnualMonthEmissionDatum()
                 self.list.append(temp_model.from_map(k))
         return self
 
 
+class RegisterEcarEnterprisememberRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        account_did: str = None,
+        name: str = None,
+        identity_card_code: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 注册会员在蚂蚁DIS服务的DID账号
+        self.account_did = account_did
+        # 注册会员姓名
+        self.name = name
+        # 注册会员身份证号码
+        self.identity_card_code = identity_card_code
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
+        if self.account_did is not None:
+            result['account_did'] = self.account_did
+        if self.name is not None:
+            result['name'] = self.name
+        if self.identity_card_code is not None:
+            result['identity_card_code'] = self.identity_card_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('account_did') is not None:
+            self.account_did = m.get('account_did')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('identity_card_code') is not None:
+            self.identity_card_code = m.get('identity_card_code')
+        return self
+
+
+class RegisterEcarEnterprisememberResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        account_did: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 蚂蚁DIS服务的DID账号
+        self.account_did = account_did
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
+        if self.account_did is not None:
+            result['account_did'] = self.account_did
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
+        if m.get('account_did') is not None:
+            self.account_did = m.get('account_did')
+        return self
+
+
+class AddEcarOffsetacquisitionRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        acquisition_item_no: str = None,
+        project_no: str = None,
+        account_did: str = None,
+        occurrent_time: str = None,
+        scenario_code: str = None,
+        active_data_list: List[AnyAmountItem] = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 活动数据采集单号
+        self.acquisition_item_no = acquisition_item_no
+        # 碳普惠减碳项目编号
+        self.project_no = project_no
+        # 参与的碳账户DID
+        self.account_did = account_did
+        # 发生时间，格式为yyyy-MM-DD HH:MM:SS（到秒）或 yyyy-MM-DD（按日录入）
+        self.occurrent_time = occurrent_time
+        # 发生场景，需要按照约定的场景编码提交
+        self.scenario_code = scenario_code
+        # 活动数据列表
+        self.active_data_list = active_data_list
+
+    def validate(self):
+        self.validate_required(self.acquisition_item_no, 'acquisition_item_no')
+        self.validate_required(self.project_no, 'project_no')
+        self.validate_required(self.account_did, 'account_did')
+        self.validate_required(self.occurrent_time, 'occurrent_time')
+        self.validate_required(self.scenario_code, 'scenario_code')
+        self.validate_required(self.active_data_list, 'active_data_list')
+        if self.active_data_list:
+            for k in self.active_data_list:
+                if k:
+                    k.validate()
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
+        if self.acquisition_item_no is not None:
+            result['acquisition_item_no'] = self.acquisition_item_no
+        if self.project_no is not None:
+            result['project_no'] = self.project_no
+        if self.account_did is not None:
+            result['account_did'] = self.account_did
+        if self.occurrent_time is not None:
+            result['occurrent_time'] = self.occurrent_time
+        if self.scenario_code is not None:
+            result['scenario_code'] = self.scenario_code
+        result['active_data_list'] = []
+        if self.active_data_list is not None:
+            for k in self.active_data_list:
+                result['active_data_list'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('acquisition_item_no') is not None:
+            self.acquisition_item_no = m.get('acquisition_item_no')
+        if m.get('project_no') is not None:
+            self.project_no = m.get('project_no')
+        if m.get('account_did') is not None:
+            self.account_did = m.get('account_did')
+        if m.get('occurrent_time') is not None:
+            self.occurrent_time = m.get('occurrent_time')
+        if m.get('scenario_code') is not None:
+            self.scenario_code = m.get('scenario_code')
+        self.active_data_list = []
+        if m.get('active_data_list') is not None:
+            for k in m.get('active_data_list'):
+                temp_model = AnyAmountItem()
+                self.active_data_list.append(temp_model.from_map(k))
+        return self
+
+
+class AddEcarOffsetacquisitionResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        acquisition_item_no: str = None,
+        carbon_emission_amount: int = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 活动数据采集单号
+        self.acquisition_item_no = acquisition_item_no
+        # 减碳量
+        self.carbon_emission_amount = carbon_emission_amount
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
+        if self.acquisition_item_no is not None:
+            result['acquisition_item_no'] = self.acquisition_item_no
+        if self.carbon_emission_amount is not None:
+            result['carbon_emission_amount'] = self.carbon_emission_amount
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
+        if m.get('acquisition_item_no') is not None:
+            self.acquisition_item_no = m.get('acquisition_item_no')
+        if m.get('carbon_emission_amount') is not None:
+            self.carbon_emission_amount = m.get('carbon_emission_amount')
+        return self
+
+
+class AddEcarOffsettranslateRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        translation_item_no: str = None,
+        project_no: str = None,
+        drawing_account_did: str = None,
+        receipt_account_did: str = None,
+        translation_ammount: int = None,
+        translation_type: str = None,
+        occurrent_time: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 转移业务流水单号
+        self.translation_item_no = translation_item_no
+        # 碳补偿项目编号
+        self.project_no = project_no
+        # 出账账户DID
+        self.drawing_account_did = drawing_account_did
+        # 转移入账账户DID
+        self.receipt_account_did = receipt_account_did
+        # 转移减碳量额度
+        self.translation_ammount = translation_ammount
+        # 业务类型包括，默认不需要传入，默认值为Translation
+        self.translation_type = translation_type
+        # 发生时间，格式为yyyy-MM-DD HH:MM:SS
+        self.occurrent_time = occurrent_time
+
+    def validate(self):
+        self.validate_required(self.translation_item_no, 'translation_item_no')
+        self.validate_required(self.project_no, 'project_no')
+        self.validate_required(self.drawing_account_did, 'drawing_account_did')
+        self.validate_required(self.receipt_account_did, 'receipt_account_did')
+        self.validate_required(self.translation_ammount, 'translation_ammount')
+        self.validate_required(self.occurrent_time, 'occurrent_time')
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
+        if self.translation_item_no is not None:
+            result['translation_item_no'] = self.translation_item_no
+        if self.project_no is not None:
+            result['project_no'] = self.project_no
+        if self.drawing_account_did is not None:
+            result['drawing_account_did'] = self.drawing_account_did
+        if self.receipt_account_did is not None:
+            result['receipt_account_did'] = self.receipt_account_did
+        if self.translation_ammount is not None:
+            result['translation_ammount'] = self.translation_ammount
+        if self.translation_type is not None:
+            result['translation_type'] = self.translation_type
+        if self.occurrent_time is not None:
+            result['occurrent_time'] = self.occurrent_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('translation_item_no') is not None:
+            self.translation_item_no = m.get('translation_item_no')
+        if m.get('project_no') is not None:
+            self.project_no = m.get('project_no')
+        if m.get('drawing_account_did') is not None:
+            self.drawing_account_did = m.get('drawing_account_did')
+        if m.get('receipt_account_did') is not None:
+            self.receipt_account_did = m.get('receipt_account_did')
+        if m.get('translation_ammount') is not None:
+            self.translation_ammount = m.get('translation_ammount')
+        if m.get('translation_type') is not None:
+            self.translation_type = m.get('translation_type')
+        if m.get('occurrent_time') is not None:
+            self.occurrent_time = m.get('occurrent_time')
+        return self
+
+
+class AddEcarOffsettranslateResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
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
+        return self
+
+
+class AuthEcarOffsetdatumRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        account_did: str = None,
+        carbon_offset_platform_no: str = None,
+        platform_account_id: str = None,
+        auth_keyword_list: List[AnyKeywordItem] = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 会员在蚂蚁DIS服务的账户DID
+        self.account_did = account_did
+        # 碳普惠平台编码，如蚂蚁森林编码为Antforest
+        self.carbon_offset_platform_no = carbon_offset_platform_no
+        # 平台方会员账户ID
+        self.platform_account_id = platform_account_id
+        # 授权关键数据列表，KV结构列表
+        self.auth_keyword_list = auth_keyword_list
+
+    def validate(self):
+        self.validate_required(self.account_did, 'account_did')
+        self.validate_required(self.carbon_offset_platform_no, 'carbon_offset_platform_no')
+        self.validate_required(self.platform_account_id, 'platform_account_id')
+        self.validate_required(self.auth_keyword_list, 'auth_keyword_list')
+        if self.auth_keyword_list:
+            for k in self.auth_keyword_list:
+                if k:
+                    k.validate()
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
+        if self.account_did is not None:
+            result['account_did'] = self.account_did
+        if self.carbon_offset_platform_no is not None:
+            result['carbon_offset_platform_no'] = self.carbon_offset_platform_no
+        if self.platform_account_id is not None:
+            result['platform_account_id'] = self.platform_account_id
+        result['auth_keyword_list'] = []
+        if self.auth_keyword_list is not None:
+            for k in self.auth_keyword_list:
+                result['auth_keyword_list'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('account_did') is not None:
+            self.account_did = m.get('account_did')
+        if m.get('carbon_offset_platform_no') is not None:
+            self.carbon_offset_platform_no = m.get('carbon_offset_platform_no')
+        if m.get('platform_account_id') is not None:
+            self.platform_account_id = m.get('platform_account_id')
+        self.auth_keyword_list = []
+        if m.get('auth_keyword_list') is not None:
+            for k in m.get('auth_keyword_list'):
+                temp_model = AnyKeywordItem()
+                self.auth_keyword_list.append(temp_model.from_map(k))
+        return self
+
+
+class AuthEcarOffsetdatumResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
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
+        return self
+
+
+class ListEcarOffsetdatumRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        project_no: str = None,
+        account_did: str = None,
+        occurrent_start_time: str = None,
+        occurrent_end_time: str = None,
+        carbon_offset_platform_no: str = None,
+        scenario_code: List[str] = None,
+        current: int = None,
+        page_size: int = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 碳补偿项目编码
+        self.project_no = project_no
+        # 账户DID
+        self.account_did = account_did
+        # 发生开始时间
+        self.occurrent_start_time = occurrent_start_time
+        # 数据发生截止时间
+        self.occurrent_end_time = occurrent_end_time
+        # 碳普惠平台编码
+        self.carbon_offset_platform_no = carbon_offset_platform_no
+        # 发生场景编码，需指定相关碳普惠平台的场景编码，可以指定多个场景
+        self.scenario_code = scenario_code
+        # 分页查询数据时的页码，从1开始，不传入时默认值为1
+        self.current = current
+        # 每页数据量，默认值为20，取值范围为[10,100]
+        self.page_size = page_size
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
+        if self.project_no is not None:
+            result['project_no'] = self.project_no
+        if self.account_did is not None:
+            result['account_did'] = self.account_did
+        if self.occurrent_start_time is not None:
+            result['occurrent_start_time'] = self.occurrent_start_time
+        if self.occurrent_end_time is not None:
+            result['occurrent_end_time'] = self.occurrent_end_time
+        if self.carbon_offset_platform_no is not None:
+            result['carbon_offset_platform_no'] = self.carbon_offset_platform_no
+        if self.scenario_code is not None:
+            result['scenario_code'] = self.scenario_code
+        if self.current is not None:
+            result['current'] = self.current
+        if self.page_size is not None:
+            result['page_size'] = self.page_size
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('project_no') is not None:
+            self.project_no = m.get('project_no')
+        if m.get('account_did') is not None:
+            self.account_did = m.get('account_did')
+        if m.get('occurrent_start_time') is not None:
+            self.occurrent_start_time = m.get('occurrent_start_time')
+        if m.get('occurrent_end_time') is not None:
+            self.occurrent_end_time = m.get('occurrent_end_time')
+        if m.get('carbon_offset_platform_no') is not None:
+            self.carbon_offset_platform_no = m.get('carbon_offset_platform_no')
+        if m.get('scenario_code') is not None:
+            self.scenario_code = m.get('scenario_code')
+        if m.get('current') is not None:
+            self.current = m.get('current')
+        if m.get('page_size') is not None:
+            self.page_size = m.get('page_size')
+        return self
+
+
+class ListEcarOffsetdatumResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        current: int = None,
+        page_size: int = None,
+        total: int = None,
+        list: List[CarbonOffsetAcquisitionItem] = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 当前查询的页码
+        self.current = current
+        # 每页记录条数
+        self.page_size = page_size
+        # 记录总条数
+        self.total = total
+        # 碳普惠减碳数据明细
+        self.list = list
+
+    def validate(self):
+        if self.list:
+            for k in self.list:
+                if k:
+                    k.validate()
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
+        if self.current is not None:
+            result['current'] = self.current
+        if self.page_size is not None:
+            result['page_size'] = self.page_size
+        if self.total is not None:
+            result['total'] = self.total
+        result['list'] = []
+        if self.list is not None:
+            for k in self.list:
+                result['list'].append(k.to_map() if k else None)
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
+        if m.get('current') is not None:
+            self.current = m.get('current')
+        if m.get('page_size') is not None:
+            self.page_size = m.get('page_size')
+        if m.get('total') is not None:
+            self.total = m.get('total')
+        self.list = []
+        if m.get('list') is not None:
+            for k in m.get('list'):
+                temp_model = CarbonOffsetAcquisitionItem()
+                self.list.append(temp_model.from_map(k))
+        return self
+
+
 class QueryThirdCertRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         product_id: str = None,
         certification_type: str = None,
```

### Comparing `antchain_stlr-2.1.3/antchain_stlr.egg-info/PKG-INFO` & `antchain_stlr-2.2.0/antchain_stlr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-stlr
-Version: 2.1.3
+Version: 2.2.0
 Summary: Ant Chain STLR SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_stlr-2.1.3/setup.py` & `antchain_stlr-2.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_stlr.
 
-Created on 10/02/2023
+Created on 18/05/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_stlr"
 NAME = "antchain_stlr" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain STLR SDK Library for Python"
```

