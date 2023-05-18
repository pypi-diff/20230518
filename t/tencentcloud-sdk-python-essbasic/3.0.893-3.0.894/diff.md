# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.893.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.894.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.893.tar", last modified: Wed May 17 03:31:18 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.894.tar", last modified: Thu May 18 00:26:03 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.893.tar` & `tencentcloud-sdk-python-essbasic-3.0.894.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:31:18.000000 tencentcloud-sdk-python-essbasic-3.0.893/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:31:18.000000 tencentcloud-sdk-python-essbasic-3.0.893/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 03:31:18.000000 tencentcloud-sdk-python-essbasic-3.0.893/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      678 2023-05-17 03:31:18.000000 tencentcloud-sdk-python-essbasic-3.0.893/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-05-17 03:31:18.000000 tencentcloud-sdk-python-essbasic-3.0.893/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-17 03:31:18.000000 tencentcloud-sdk-python-essbasic-3.0.893/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      752 2023-05-17 03:31:18.000000 tencentcloud-sdk-python-essbasic-3.0.893/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:31:18.000000 tencentcloud-sdk-python-essbasic-3.0.893/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-17 03:31:18.000000 tencentcloud-sdk-python-essbasic-3.0.893/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:31:18.000000 tencentcloud-sdk-python-essbasic-3.0.893/tencentcloud/essbasic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:31:18.000000 tencentcloud-sdk-python-essbasic-3.0.893/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)    15673 2023-05-17 03:31:18.000000 tencentcloud-sdk-python-essbasic-3.0.893/tencentcloud/essbasic/v20210526/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    50895 2023-05-17 03:31:18.000000 tencentcloud-sdk-python-essbasic-3.0.893/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:31:18.000000 tencentcloud-sdk-python-essbasic-3.0.893/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)   230367 2023-05-17 03:31:18.000000 tencentcloud-sdk-python-essbasic-3.0.893/tencentcloud/essbasic/v20210526/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:31:18.000000 tencentcloud-sdk-python-essbasic-3.0.893/tencentcloud/essbasic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:31:18.000000 tencentcloud-sdk-python-essbasic-3.0.893/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)     5392 2023-05-17 03:31:18.000000 tencentcloud-sdk-python-essbasic-3.0.893/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    53845 2023-05-17 03:31:18.000000 tencentcloud-sdk-python-essbasic-3.0.893/tencentcloud/essbasic/v20201222/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:31:18.000000 tencentcloud-sdk-python-essbasic-3.0.893/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)   171664 2023-05-17 03:31:18.000000 tencentcloud-sdk-python-essbasic-3.0.893/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-05-17 03:31:18.000000 tencentcloud-sdk-python-essbasic-3.0.893/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1016 2023-05-17 03:31:18.000000 tencentcloud-sdk-python-essbasic-3.0.893/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-17 03:31:18.000000 tencentcloud-sdk-python-essbasic-3.0.893/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      678 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      752 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/essbasic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)    15673 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/essbasic/v20210526/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    50895 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   230725 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/essbasic/v20210526/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/essbasic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    53845 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/essbasic/v20201222/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   171664 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/setup.cfg
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.893/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.893/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.893
+Version: 3.0.894
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.893/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.894/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.893/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-essbasic-3.0.893/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.893/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.893/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/essbasic/v20210526/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -748,15 +748,15 @@
         :type Unordered: bool
         :param FlowType: 签署流程的类型，长度不超过255个字符
         :type FlowType: str
         :param FlowDescription: 签署流程的描述，长度不超过1000个字符
         :type FlowDescription: str
         :param CustomShowMap: 合同显示的页卡模板，说明：只支持{合同名称}, {发起方企业}, {发起方姓名}, {签署方N企业}, {签署方N姓名}，且N不能超过签署人的数量，N从1开始
         :type CustomShowMap: str
-        :param CustomerData: 业务信息，最大长度1000个字符。发起自动签署时，需设置对应自动签署场景，目前仅支持场景：处方单-E_PRESCRIPTION_AUTO_SIGN
+        :param CustomerData: 业务信息，最大长度1000个字符。
         :type CustomerData: str
         :param NeedSignReview: 发起方企业的签署人进行签署操作是否需要企业内部审批。 若设置为true,审核结果需通过接口 ChannelCreateFlowSignReview 通知电子签，审核通过后，发起方企业签署人方可进行签署操作，否则会阻塞其签署操作。  注：企业可以通过此功能与企业内部的审批流程进行关联，支持手动、静默签署合同。
         :type NeedSignReview: bool
         :param ApproverVerifyType: 签署人校验方式
 VerifyCheck: 人脸识别（默认）
 MobileCheck：手机号验证
 参数说明：可选人脸识别或手机号验证两种方式，若选择后者，未实名个人签署方在签署合同时，无需经过实名认证和意愿确认两次人脸识别，该能力仅适用于个人签署方。
@@ -765,14 +765,16 @@
         :type SignBeanTag: int
         :param Operator: 操作者的信息，不用传
         :type Operator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
         :param CcInfos: 被抄送人信息列表
         :type CcInfos: list of CcInfo
         :param CcNotifyType: 给关注人发送短信通知的类型，0-合同发起时通知 1-签署完成后通知
         :type CcNotifyType: int
+        :param AutoSignScene: 个人自动签场景。发起自动签署时，需设置对应自动签署场景，目前仅支持场景：处方单-E_PRESCRIPTION_AUTO_SIGN
+        :type AutoSignScene: str
         """
         self.Agent = None
         self.FlowName = None
         self.FlowApprovers = None
         self.FileIds = None
         self.Components = None
         self.Deadline = None
@@ -784,14 +786,15 @@
         self.CustomerData = None
         self.NeedSignReview = None
         self.ApproverVerifyType = None
         self.SignBeanTag = None
         self.Operator = None
         self.CcInfos = None
         self.CcNotifyType = None
+        self.AutoSignScene = None
 
 
     def _deserialize(self, params):
         if params.get("Agent") is not None:
             self.Agent = Agent()
             self.Agent._deserialize(params.get("Agent"))
         self.FlowName = params.get("FlowName")
@@ -824,14 +827,15 @@
         if params.get("CcInfos") is not None:
             self.CcInfos = []
             for item in params.get("CcInfos"):
                 obj = CcInfo()
                 obj._deserialize(item)
                 self.CcInfos.append(obj)
         self.CcNotifyType = params.get("CcNotifyType")
+        self.AutoSignScene = params.get("AutoSignScene")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -4198,41 +4202,44 @@
         :type FormFields: list of FormField
         :param CallbackUrl: 回调地址，最大长度1000个字符
         :type CallbackUrl: str
         :param FlowType: 合同类型，如：1. “劳务”；2. “销售”；3. “租赁”；4. “其他”，最大长度200个字符
         :type FlowType: str
         :param FlowDescription: 合同描述，最大长度1000个字符
         :type FlowDescription: str
-        :param CustomerData:  第三方应用平台的业务信息，最大长度1000个字符。发起自动签署时，需设置对应自动签署场景，目前仅支持场景：处方单-E_PRESCRIPTION_AUTO_SIGN
+        :param CustomerData:  第三方应用平台的业务信息，最大长度1000个字符。
         :type CustomerData: str
         :param CustomShowMap: 合同显示的页卡模板，说明：只支持{合同名称}, {发起方企业}, {发起方姓名}, {签署方N企业}, {签署方N姓名}，且N不能超过签署人的数量，N从1开始
         :type CustomShowMap: str
         :param CcInfos: 被抄送人的信息列表，抄送功能暂不开放
         :type CcInfos: list of CcInfo
         :param NeedSignReview: 发起方企业的签署人进行签署操作是否需要企业内部审批。
 若设置为true,审核结果需通过接口 ChannelCreateFlowSignReview 通知电子签，审核通过后，发起方企业签署人方可进行签署操作，否则会阻塞其签署操作。
 
 注：企业可以通过此功能与企业内部的审批流程进行关联，支持手动、静默签署合同。
         :type NeedSignReview: bool
         :param CcNotifyType: 给关注人发送短信通知的类型，0-合同发起时通知 1-签署完成后通知
         :type CcNotifyType: int
+        :param AutoSignScene: 个人自动签场景。发起自动签署时，需设置对应自动签署场景，目前仅支持场景：处方单-E_PRESCRIPTION_AUTO_SIGN
+        :type AutoSignScene: str
         """
         self.FlowName = None
         self.Deadline = None
         self.TemplateId = None
         self.FlowApprovers = None
         self.FormFields = None
         self.CallbackUrl = None
         self.FlowType = None
         self.FlowDescription = None
         self.CustomerData = None
         self.CustomShowMap = None
         self.CcInfos = None
         self.NeedSignReview = None
         self.CcNotifyType = None
+        self.AutoSignScene = None
 
 
     def _deserialize(self, params):
         self.FlowName = params.get("FlowName")
         self.Deadline = params.get("Deadline")
         self.TemplateId = params.get("TemplateId")
         if params.get("FlowApprovers") is not None:
@@ -4256,14 +4263,15 @@
             self.CcInfos = []
             for item in params.get("CcInfos"):
                 obj = CcInfo()
                 obj._deserialize(item)
                 self.CcInfos.append(obj)
         self.NeedSignReview = params.get("NeedSignReview")
         self.CcNotifyType = params.get("CcNotifyType")
+        self.AutoSignScene = params.get("AutoSignScene")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.893/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.893/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.893/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.893/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.894/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.893
+Version: 3.0.894
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.893/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.894/setup.py`

 * *Files identical despite different names*

