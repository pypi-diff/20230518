# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.893.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.894.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.893.tar", last modified: Wed May 17 03:31:12 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.894.tar", last modified: Thu May 18 00:25:55 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.893.tar` & `tencentcloud-sdk-python-ess-3.0.894.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:31:12.000000 tencentcloud-sdk-python-ess-3.0.893/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-17 03:31:12.000000 tencentcloud-sdk-python-ess-3.0.893/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:31:12.000000 tencentcloud-sdk-python-ess-3.0.893/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-17 03:31:12.000000 tencentcloud-sdk-python-ess-3.0.893/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:31:12.000000 tencentcloud-sdk-python-ess-3.0.893/tencentcloud/ess/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:31:12.000000 tencentcloud-sdk-python-ess-3.0.893/tencentcloud/ess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:31:12.000000 tencentcloud-sdk-python-ess-3.0.893/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    50630 2023-05-17 03:31:12.000000 tencentcloud-sdk-python-ess-3.0.893/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)    23727 2023-05-17 03:31:12.000000 tencentcloud-sdk-python-ess-3.0.893/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:31:12.000000 tencentcloud-sdk-python-ess-3.0.893/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   222162 2023-05-17 03:31:12.000000 tencentcloud-sdk-python-ess-3.0.893/tencentcloud/ess/v20201111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:31:12.000000 tencentcloud-sdk-python-ess-3.0.893/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 03:31:12.000000 tencentcloud-sdk-python-ess-3.0.893/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-17 03:31:12.000000 tencentcloud-sdk-python-ess-3.0.893/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-17 03:31:12.000000 tencentcloud-sdk-python-ess-3.0.893/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-17 03:31:12.000000 tencentcloud-sdk-python-ess-3.0.893/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-17 03:31:12.000000 tencentcloud-sdk-python-ess-3.0.893/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-17 03:31:12.000000 tencentcloud-sdk-python-ess-3.0.893/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-17 03:31:12.000000 tencentcloud-sdk-python-ess-3.0.893/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:25:55.000000 tencentcloud-sdk-python-ess-3.0.894/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-18 00:25:55.000000 tencentcloud-sdk-python-ess-3.0.894/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:25:55.000000 tencentcloud-sdk-python-ess-3.0.894/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-18 00:25:55.000000 tencentcloud-sdk-python-ess-3.0.894/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:25:55.000000 tencentcloud-sdk-python-ess-3.0.894/tencentcloud/ess/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:25:55.000000 tencentcloud-sdk-python-ess-3.0.894/tencentcloud/ess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:25:55.000000 tencentcloud-sdk-python-ess-3.0.894/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    50642 2023-05-18 00:25:55.000000 tencentcloud-sdk-python-ess-3.0.894/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)    23727 2023-05-18 00:25:55.000000 tencentcloud-sdk-python-ess-3.0.894/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:25:55.000000 tencentcloud-sdk-python-ess-3.0.894/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   222756 2023-05-18 00:25:55.000000 tencentcloud-sdk-python-ess-3.0.894/tencentcloud/ess/v20201111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:25:55.000000 tencentcloud-sdk-python-ess-3.0.894/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 00:25:55.000000 tencentcloud-sdk-python-ess-3.0.894/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-18 00:25:55.000000 tencentcloud-sdk-python-ess-3.0.894/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-18 00:25:55.000000 tencentcloud-sdk-python-ess-3.0.894/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-18 00:25:55.000000 tencentcloud-sdk-python-ess-3.0.894/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-18 00:25:55.000000 tencentcloud-sdk-python-ess-3.0.894/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-18 00:25:55.000000 tencentcloud-sdk-python-ess-3.0.894/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-18 00:25:55.000000 tencentcloud-sdk-python-ess-3.0.894/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ess-3.0.893/README.rst` & `tencentcloud-sdk-python-ess-3.0.894/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.893/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.894/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.893/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.894/tencentcloud/ess/v20201111/ess_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateFlow(self, request):
-        """创建签署流程
+        """通过模板创建签署流程
         适用场景：在标准制式的合同场景中，可通过提前预制好模板文件，每次调用模板文件的id，补充合同内容信息及签署信息生成电子合同。
         注：该接口是通过模板生成合同流程的前置接口，先创建一个不包含签署文件的流程。配合“创建电子文档”接口和“发起流程”接口使用。
 
         :param request: Request instance for CreateFlow.
         :type request: :class:`tencentcloud.ess.v20201111.models.CreateFlowRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.CreateFlowResponse`
```

### Comparing `tencentcloud-sdk-python-ess-3.0.893/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.894/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.893/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.894/tencentcloud/ess/v20201111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1223,14 +1223,16 @@
         :type FlowDescription: str
         :param SignBeanTag: 标识是否允许发起后添加控件。0为不允许1为允许。如果为1，创建的时候不能有签署控件，只能创建后添加。注意发起后添加控件功能不支持添加骑缝章和签批控件
         :type SignBeanTag: int
         :param Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         :param CcNotifyType: 给关注人发送短信通知的类型，0-合同发起时通知 1-签署完成后通知
         :type CcNotifyType: int
+        :param AutoSignScene: 个人自动签场景。发起自动签署时，需设置对应自动签署场景，目前仅支持场景：处方单-E_PRESCRIPTION_AUTO_SIGN
+        :type AutoSignScene: str
         """
         self.Operator = None
         self.FlowName = None
         self.Approvers = None
         self.FileIds = None
         self.FlowType = None
         self.Components = None
@@ -1243,14 +1245,15 @@
         self.NeedSignReview = None
         self.UserData = None
         self.ApproverVerifyType = None
         self.FlowDescription = None
         self.SignBeanTag = None
         self.Agent = None
         self.CcNotifyType = None
+        self.AutoSignScene = None
 
 
     def _deserialize(self, params):
         if params.get("Operator") is not None:
             self.Operator = UserInfo()
             self.Operator._deserialize(params.get("Operator"))
         self.FlowName = params.get("FlowName")
@@ -1284,14 +1287,15 @@
         self.ApproverVerifyType = params.get("ApproverVerifyType")
         self.FlowDescription = params.get("FlowDescription")
         self.SignBeanTag = params.get("SignBeanTag")
         if params.get("Agent") is not None:
             self.Agent = Agent()
             self.Agent._deserialize(params.get("Agent"))
         self.CcNotifyType = params.get("CcNotifyType")
+        self.AutoSignScene = params.get("AutoSignScene")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -1487,14 +1491,16 @@
         :param CallbackUrl: 暂未开放
         :type CallbackUrl: str
         :param Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         :param CcInfos: 被抄送人的信息列表。
 注: 此功能为白名单功能，若有需要，请联系电子签客服开白使用。
         :type CcInfos: list of CcInfo
+        :param AutoSignScene: 个人自动签场景。发起自动签署时，需设置对应自动签署场景，目前仅支持场景：处方单-E_PRESCRIPTION_AUTO_SIGN
+        :type AutoSignScene: str
         """
         self.Operator = None
         self.FlowName = None
         self.Approvers = None
         self.FlowType = None
         self.ClientToken = None
         self.RelatedFlowId = None
@@ -1503,14 +1509,15 @@
         self.FlowDescription = None
         self.Unordered = None
         self.CustomShowMap = None
         self.NeedSignReview = None
         self.CallbackUrl = None
         self.Agent = None
         self.CcInfos = None
+        self.AutoSignScene = None
 
 
     def _deserialize(self, params):
         if params.get("Operator") is not None:
             self.Operator = UserInfo()
             self.Operator._deserialize(params.get("Operator"))
         self.FlowName = params.get("FlowName")
@@ -1535,14 +1542,15 @@
             self.Agent._deserialize(params.get("Agent"))
         if params.get("CcInfos") is not None:
             self.CcInfos = []
             for item in params.get("CcInfos"):
                 obj = CcInfo()
                 obj._deserialize(item)
                 self.CcInfos.append(obj)
+        self.AutoSignScene = params.get("AutoSignScene")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-ess-3.0.893/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.894/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.893
+Version: 3.0.894
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.893/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.894/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.893
+Version: 3.0.894
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.893/setup.py` & `tencentcloud-sdk-python-ess-3.0.894/setup.py`

 * *Files identical despite different names*

