# Comparing `tmp/tencentcloud-sdk-python-lighthouse-3.0.893.tar.gz` & `tmp/tencentcloud-sdk-python-lighthouse-3.0.894.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-lighthouse-3.0.893.tar", last modified: Wed May 17 03:34:40 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-lighthouse-3.0.894.tar", last modified: Thu May 18 00:29:45 2023, max compression
```

## Comparing `tencentcloud-sdk-python-lighthouse-3.0.893.tar` & `tencentcloud-sdk-python-lighthouse-3.0.894.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:34:40.000000 tencentcloud-sdk-python-lighthouse-3.0.893/
--rw-r--r--   0 root         (0) root         (0)      758 2023-05-17 03:34:40.000000 tencentcloud-sdk-python-lighthouse-3.0.893/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:34:40.000000 tencentcloud-sdk-python-lighthouse-3.0.893/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-17 03:34:40.000000 tencentcloud-sdk-python-lighthouse-3.0.893/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:34:40.000000 tencentcloud-sdk-python-lighthouse-3.0.893/tencentcloud/lighthouse/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:34:40.000000 tencentcloud-sdk-python-lighthouse-3.0.893/tencentcloud/lighthouse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:34:40.000000 tencentcloud-sdk-python-lighthouse-3.0.893/tencentcloud/lighthouse/v20200324/
--rw-r--r--   0 root         (0) root         (0)    25988 2023-05-17 03:34:40.000000 tencentcloud-sdk-python-lighthouse-3.0.893/tencentcloud/lighthouse/v20200324/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    92541 2023-05-17 03:34:40.000000 tencentcloud-sdk-python-lighthouse-3.0.893/tencentcloud/lighthouse/v20200324/lighthouse_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:34:40.000000 tencentcloud-sdk-python-lighthouse-3.0.893/tencentcloud/lighthouse/v20200324/__init__.py
--rw-r--r--   0 root         (0) root         (0)   240429 2023-05-17 03:34:40.000000 tencentcloud-sdk-python-lighthouse-3.0.893/tencentcloud/lighthouse/v20200324/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:34:40.000000 tencentcloud-sdk-python-lighthouse-3.0.893/tencentcloud_sdk_python_lighthouse.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 03:34:40.000000 tencentcloud-sdk-python-lighthouse-3.0.893/tencentcloud_sdk_python_lighthouse.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      515 2023-05-17 03:34:40.000000 tencentcloud-sdk-python-lighthouse-3.0.893/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-05-17 03:34:40.000000 tencentcloud-sdk-python-lighthouse-3.0.893/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-17 03:34:40.000000 tencentcloud-sdk-python-lighthouse-3.0.893/tencentcloud_sdk_python_lighthouse.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-05-17 03:34:40.000000 tencentcloud-sdk-python-lighthouse-3.0.893/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1020 2023-05-17 03:34:40.000000 tencentcloud-sdk-python-lighthouse-3.0.893/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-17 03:34:40.000000 tencentcloud-sdk-python-lighthouse-3.0.893/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:29:45.000000 tencentcloud-sdk-python-lighthouse-3.0.894/
+-rw-r--r--   0 root         (0) root         (0)      758 2023-05-18 00:29:44.000000 tencentcloud-sdk-python-lighthouse-3.0.894/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:29:45.000000 tencentcloud-sdk-python-lighthouse-3.0.894/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-18 00:29:44.000000 tencentcloud-sdk-python-lighthouse-3.0.894/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:29:45.000000 tencentcloud-sdk-python-lighthouse-3.0.894/tencentcloud/lighthouse/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:29:44.000000 tencentcloud-sdk-python-lighthouse-3.0.894/tencentcloud/lighthouse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:29:45.000000 tencentcloud-sdk-python-lighthouse-3.0.894/tencentcloud/lighthouse/v20200324/
+-rw-r--r--   0 root         (0) root         (0)    25956 2023-05-18 00:29:44.000000 tencentcloud-sdk-python-lighthouse-3.0.894/tencentcloud/lighthouse/v20200324/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    92541 2023-05-18 00:29:44.000000 tencentcloud-sdk-python-lighthouse-3.0.894/tencentcloud/lighthouse/v20200324/lighthouse_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:29:44.000000 tencentcloud-sdk-python-lighthouse-3.0.894/tencentcloud/lighthouse/v20200324/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   240429 2023-05-18 00:29:44.000000 tencentcloud-sdk-python-lighthouse-3.0.894/tencentcloud/lighthouse/v20200324/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:29:45.000000 tencentcloud-sdk-python-lighthouse-3.0.894/tencentcloud_sdk_python_lighthouse.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 00:29:45.000000 tencentcloud-sdk-python-lighthouse-3.0.894/tencentcloud_sdk_python_lighthouse.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      515 2023-05-18 00:29:45.000000 tencentcloud-sdk-python-lighthouse-3.0.894/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-05-18 00:29:45.000000 tencentcloud-sdk-python-lighthouse-3.0.894/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-18 00:29:45.000000 tencentcloud-sdk-python-lighthouse-3.0.894/tencentcloud_sdk_python_lighthouse.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-05-18 00:29:45.000000 tencentcloud-sdk-python-lighthouse-3.0.894/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-05-18 00:29:44.000000 tencentcloud-sdk-python-lighthouse-3.0.894/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-18 00:29:45.000000 tencentcloud-sdk-python-lighthouse-3.0.894/setup.cfg
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.893/README.rst` & `tencentcloud-sdk-python-lighthouse-3.0.894/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.893/tencentcloud/__init__.py` & `tencentcloud-sdk-python-lighthouse-3.0.894/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.893'
+__version__ = '3.0.894'
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.893/tencentcloud/lighthouse/v20200324/errorcodes.py` & `tencentcloud-sdk-python-lighthouse-3.0.894/tencentcloud/lighthouse/v20200324/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
 
 # 无法找到此接口。
 INTERNALERROR_INVALIDACTIONNOTFOUND = 'InternalError.InvalidActionNotFound'
 
 # 套餐价格错误。
 INTERNALERROR_INVALIDBUNDLEPRICE = 'InternalError.InvalidBundlePrice'
 
-# 命令 `DescribeInstanceLoginKeyPair` 无法找到。
+# 命令无法找到。
 INTERNALERROR_INVALIDCOMMANDNOTFOUND = 'InternalError.InvalidCommandNotFound'
 
 # 请求出现错误。
 INTERNALERROR_REQUESTERROR = 'InternalError.RequestError'
 
 # 调用计费网关服务失败。
 INTERNALERROR_TRADECALLBILLINGGATEWAYFAILED = 'InternalError.TradeCallBillingGatewayFailed'
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.893/tencentcloud/lighthouse/v20200324/lighthouse_client.py` & `tencentcloud-sdk-python-lighthouse-3.0.894/tencentcloud/lighthouse/v20200324/lighthouse_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1180,15 +1180,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DetachCcn(self, request):
-        """本接口 (AttachCcn) 用于解除与云联网的关联。
+        """本接口 (DetachCcn) 用于解除与云联网的关联。
 
         :param request: Request instance for DetachCcn.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.DetachCcnRequest`
         :rtype: :class:`tencentcloud.lighthouse.v20200324.models.DetachCcnResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.893/tencentcloud/lighthouse/v20200324/models.py` & `tencentcloud-sdk-python-lighthouse-3.0.894/tencentcloud/lighthouse/v20200324/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.893/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-lighthouse-3.0.894/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.893/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO` & `tencentcloud-sdk-python-lighthouse-3.0.894/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lighthouse
-Version: 3.0.893
+Version: 3.0.894
 Summary: Tencent Cloud Lighthouse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.893/PKG-INFO` & `tencentcloud-sdk-python-lighthouse-3.0.894/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lighthouse
-Version: 3.0.893
+Version: 3.0.894
 Summary: Tencent Cloud Lighthouse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.893/setup.py` & `tencentcloud-sdk-python-lighthouse-3.0.894/setup.py`

 * *Files identical despite different names*

