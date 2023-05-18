# Comparing `tmp/tencentcloud-sdk-python-tsf-3.0.893.tar.gz` & `tmp/tencentcloud-sdk-python-tsf-3.0.894.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tsf-3.0.893.tar", last modified: Wed May 17 03:44:16 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tsf-3.0.894.tar", last modified: Thu May 18 00:41:06 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tsf-3.0.893.tar` & `tencentcloud-sdk-python-tsf-3.0.894.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:44:16.000000 tencentcloud-sdk-python-tsf-3.0.893/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-17 03:44:16.000000 tencentcloud-sdk-python-tsf-3.0.893/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:44:16.000000 tencentcloud-sdk-python-tsf-3.0.893/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:44:16.000000 tencentcloud-sdk-python-tsf-3.0.893/tencentcloud/tsf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:44:16.000000 tencentcloud-sdk-python-tsf-3.0.893/tencentcloud/tsf/v20180326/
--rw-r--r--   0 root         (0) root         (0)    49851 2023-05-17 03:44:16.000000 tencentcloud-sdk-python-tsf-3.0.893/tencentcloud/tsf/v20180326/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   194455 2023-05-17 03:44:16.000000 tencentcloud-sdk-python-tsf-3.0.893/tencentcloud/tsf/v20180326/tsf_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:44:16.000000 tencentcloud-sdk-python-tsf-3.0.893/tencentcloud/tsf/v20180326/__init__.py
--rw-r--r--   0 root         (0) root         (0)   800128 2023-05-17 03:44:16.000000 tencentcloud-sdk-python-tsf-3.0.893/tencentcloud/tsf/v20180326/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:44:16.000000 tencentcloud-sdk-python-tsf-3.0.893/tencentcloud/tsf/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-17 03:44:16.000000 tencentcloud-sdk-python-tsf-3.0.893/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:44:16.000000 tencentcloud-sdk-python-tsf-3.0.893/tencentcloud_sdk_python_tsf.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 03:44:16.000000 tencentcloud-sdk-python-tsf-3.0.893/tencentcloud_sdk_python_tsf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-17 03:44:16.000000 tencentcloud-sdk-python-tsf-3.0.893/tencentcloud_sdk_python_tsf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-17 03:44:16.000000 tencentcloud-sdk-python-tsf-3.0.893/tencentcloud_sdk_python_tsf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-17 03:44:16.000000 tencentcloud-sdk-python-tsf-3.0.893/tencentcloud_sdk_python_tsf.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-17 03:44:16.000000 tencentcloud-sdk-python-tsf-3.0.893/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-17 03:44:16.000000 tencentcloud-sdk-python-tsf-3.0.893/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-17 03:44:16.000000 tencentcloud-sdk-python-tsf-3.0.893/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:41:06.000000 tencentcloud-sdk-python-tsf-3.0.894/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-18 00:41:06.000000 tencentcloud-sdk-python-tsf-3.0.894/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:41:06.000000 tencentcloud-sdk-python-tsf-3.0.894/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:41:06.000000 tencentcloud-sdk-python-tsf-3.0.894/tencentcloud/tsf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:41:06.000000 tencentcloud-sdk-python-tsf-3.0.894/tencentcloud/tsf/v20180326/
+-rw-r--r--   0 root         (0) root         (0)    49851 2023-05-18 00:41:06.000000 tencentcloud-sdk-python-tsf-3.0.894/tencentcloud/tsf/v20180326/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   195353 2023-05-18 00:41:06.000000 tencentcloud-sdk-python-tsf-3.0.894/tencentcloud/tsf/v20180326/tsf_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:41:06.000000 tencentcloud-sdk-python-tsf-3.0.894/tencentcloud/tsf/v20180326/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   801873 2023-05-18 00:41:06.000000 tencentcloud-sdk-python-tsf-3.0.894/tencentcloud/tsf/v20180326/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:41:06.000000 tencentcloud-sdk-python-tsf-3.0.894/tencentcloud/tsf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-18 00:41:06.000000 tencentcloud-sdk-python-tsf-3.0.894/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:41:06.000000 tencentcloud-sdk-python-tsf-3.0.894/tencentcloud_sdk_python_tsf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 00:41:06.000000 tencentcloud-sdk-python-tsf-3.0.894/tencentcloud_sdk_python_tsf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-18 00:41:06.000000 tencentcloud-sdk-python-tsf-3.0.894/tencentcloud_sdk_python_tsf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-18 00:41:06.000000 tencentcloud-sdk-python-tsf-3.0.894/tencentcloud_sdk_python_tsf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-18 00:41:06.000000 tencentcloud-sdk-python-tsf-3.0.894/tencentcloud_sdk_python_tsf.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-18 00:41:06.000000 tencentcloud-sdk-python-tsf-3.0.894/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-18 00:41:06.000000 tencentcloud-sdk-python-tsf-3.0.894/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-18 00:41:06.000000 tencentcloud-sdk-python-tsf-3.0.894/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.893/README.rst` & `tencentcloud-sdk-python-tsf-3.0.894/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tsf-3.0.893/tencentcloud/tsf/v20180326/errorcodes.py` & `tencentcloud-sdk-python-tsf-3.0.894/tencentcloud/tsf/v20180326/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tsf-3.0.893/tencentcloud/tsf/v20180326/tsf_client.py` & `tencentcloud-sdk-python-tsf-3.0.894/tencentcloud/tsf/v20180326/tsf_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -827,14 +827,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def CreateUnitNamespaces(self, request):
+        """批量创建单元化命名空间
+
+        :param request: Request instance for CreateUnitNamespaces.
+        :type request: :class:`tencentcloud.tsf.v20180326.models.CreateUnitNamespacesRequest`
+        :rtype: :class:`tencentcloud.tsf.v20180326.models.CreateUnitNamespacesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateUnitNamespaces", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateUnitNamespacesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def CreateUnitRule(self, request):
         """创建单元化规则
 
         :param request: Request instance for CreateUnitRule.
         :type request: :class:`tencentcloud.tsf.v20180326.models.CreateUnitRuleRequest`
         :rtype: :class:`tencentcloud.tsf.v20180326.models.CreateUnitRuleResponse`
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.893/tencentcloud/tsf/v20180326/models.py` & `tencentcloud-sdk-python-tsf-3.0.894/tencentcloud/tsf/v20180326/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -5069,14 +5069,69 @@
 
 
     def _deserialize(self, params):
         self.Result = params.get("Result")
         self.RequestId = params.get("RequestId")
 
 
+class CreateUnitNamespacesRequest(AbstractModel):
+    """CreateUnitNamespaces请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param GatewayInstanceId: 网关实体ID
+        :type GatewayInstanceId: str
+        :param UnitNamespaceList: 单元化命名空间对象列表
+        :type UnitNamespaceList: list of UnitNamespace
+        """
+        self.GatewayInstanceId = None
+        self.UnitNamespaceList = None
+
+
+    def _deserialize(self, params):
+        self.GatewayInstanceId = params.get("GatewayInstanceId")
+        if params.get("UnitNamespaceList") is not None:
+            self.UnitNamespaceList = []
+            for item in params.get("UnitNamespaceList"):
+                obj = UnitNamespace()
+                obj._deserialize(item)
+                self.UnitNamespaceList.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateUnitNamespacesResponse(AbstractModel):
+    """CreateUnitNamespaces返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Result: 是否成功
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Result: bool
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Result = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.Result = params.get("Result")
+        self.RequestId = params.get("RequestId")
+
+
 class CreateUnitRuleRequest(AbstractModel):
     """CreateUnitRule请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.893/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tsf-3.0.894/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tsf-3.0.893/tencentcloud_sdk_python_tsf.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tsf-3.0.894/tencentcloud_sdk_python_tsf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tsf
-Version: 3.0.893
+Version: 3.0.894
 Summary: Tencent Cloud Tsf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.893/PKG-INFO` & `tencentcloud-sdk-python-tsf-3.0.894/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tsf
-Version: 3.0.893
+Version: 3.0.894
 Summary: Tencent Cloud Tsf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.893/setup.py` & `tencentcloud-sdk-python-tsf-3.0.894/setup.py`

 * *Files identical despite different names*

