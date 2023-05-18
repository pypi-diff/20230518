# Comparing `tmp/tencentcloud-sdk-python-cdn-3.0.893.tar.gz` & `tmp/tencentcloud-sdk-python-cdn-3.0.894.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdn-3.0.893.tar", last modified: Wed May 17 03:25:34 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdn-3.0.894.tar", last modified: Thu May 18 00:19:45 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cdn-3.0.893.tar` & `tencentcloud-sdk-python-cdn-3.0.894.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:25:34.000000 tencentcloud-sdk-python-cdn-3.0.893/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-17 03:25:34.000000 tencentcloud-sdk-python-cdn-3.0.893/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:25:34.000000 tencentcloud-sdk-python-cdn-3.0.893/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-17 03:25:34.000000 tencentcloud-sdk-python-cdn-3.0.893/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:25:34.000000 tencentcloud-sdk-python-cdn-3.0.893/tencentcloud/cdn/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:25:34.000000 tencentcloud-sdk-python-cdn-3.0.893/tencentcloud/cdn/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:25:34.000000 tencentcloud-sdk-python-cdn-3.0.893/tencentcloud/cdn/v20180606/
--rw-r--r--   0 root         (0) root         (0)    21972 2023-05-17 03:25:34.000000 tencentcloud-sdk-python-cdn-3.0.893/tencentcloud/cdn/v20180606/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    80657 2023-05-17 03:25:34.000000 tencentcloud-sdk-python-cdn-3.0.893/tencentcloud/cdn/v20180606/cdn_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:25:34.000000 tencentcloud-sdk-python-cdn-3.0.893/tencentcloud/cdn/v20180606/__init__.py
--rw-r--r--   0 root         (0) root         (0)   569936 2023-05-17 03:25:34.000000 tencentcloud-sdk-python-cdn-3.0.893/tencentcloud/cdn/v20180606/models.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-17 03:25:34.000000 tencentcloud-sdk-python-cdn-3.0.893/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:25:34.000000 tencentcloud-sdk-python-cdn-3.0.893/tencentcloud_sdk_python_cdn.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 03:25:34.000000 tencentcloud-sdk-python-cdn-3.0.893/tencentcloud_sdk_python_cdn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-17 03:25:34.000000 tencentcloud-sdk-python-cdn-3.0.893/tencentcloud_sdk_python_cdn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-17 03:25:34.000000 tencentcloud-sdk-python-cdn-3.0.893/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-17 03:25:34.000000 tencentcloud-sdk-python-cdn-3.0.893/tencentcloud_sdk_python_cdn.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-17 03:25:34.000000 tencentcloud-sdk-python-cdn-3.0.893/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-17 03:25:34.000000 tencentcloud-sdk-python-cdn-3.0.893/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:19:45.000000 tencentcloud-sdk-python-cdn-3.0.894/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-18 00:19:45.000000 tencentcloud-sdk-python-cdn-3.0.894/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:19:45.000000 tencentcloud-sdk-python-cdn-3.0.894/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-18 00:19:45.000000 tencentcloud-sdk-python-cdn-3.0.894/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:19:45.000000 tencentcloud-sdk-python-cdn-3.0.894/tencentcloud/cdn/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:19:45.000000 tencentcloud-sdk-python-cdn-3.0.894/tencentcloud/cdn/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:19:45.000000 tencentcloud-sdk-python-cdn-3.0.894/tencentcloud/cdn/v20180606/
+-rw-r--r--   0 root         (0) root         (0)    21972 2023-05-18 00:19:45.000000 tencentcloud-sdk-python-cdn-3.0.894/tencentcloud/cdn/v20180606/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    80657 2023-05-18 00:19:45.000000 tencentcloud-sdk-python-cdn-3.0.894/tencentcloud/cdn/v20180606/cdn_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:19:45.000000 tencentcloud-sdk-python-cdn-3.0.894/tencentcloud/cdn/v20180606/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   570836 2023-05-18 00:19:45.000000 tencentcloud-sdk-python-cdn-3.0.894/tencentcloud/cdn/v20180606/models.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-18 00:19:45.000000 tencentcloud-sdk-python-cdn-3.0.894/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:19:45.000000 tencentcloud-sdk-python-cdn-3.0.894/tencentcloud_sdk_python_cdn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 00:19:45.000000 tencentcloud-sdk-python-cdn-3.0.894/tencentcloud_sdk_python_cdn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-18 00:19:45.000000 tencentcloud-sdk-python-cdn-3.0.894/tencentcloud_sdk_python_cdn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-18 00:19:45.000000 tencentcloud-sdk-python-cdn-3.0.894/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-18 00:19:45.000000 tencentcloud-sdk-python-cdn-3.0.894/tencentcloud_sdk_python_cdn.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-18 00:19:45.000000 tencentcloud-sdk-python-cdn-3.0.894/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-18 00:19:45.000000 tencentcloud-sdk-python-cdn-3.0.894/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.893/README.rst` & `tencentcloud-sdk-python-cdn-3.0.894/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.893/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdn-3.0.894/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cdn-3.0.893/tencentcloud/cdn/v20180606/errorcodes.py` & `tencentcloud-sdk-python-cdn-3.0.894/tencentcloud/cdn/v20180606/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.893/tencentcloud/cdn/v20180606/cdn_client.py` & `tencentcloud-sdk-python-cdn-3.0.894/tencentcloud/cdn/v20180606/cdn_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.893/tencentcloud/cdn/v20180606/models.py` & `tencentcloud-sdk-python-cdn-3.0.894/tencentcloud/cdn/v20180606/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1803,15 +1803,17 @@
 class BotCookie(AbstractModel):
     """Bot cookie策略
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: on|off
+        :param Switch: Bot cookie策略配置开关，取值有：
+on：开启
+off：关闭
         :type Switch: str
         :param RuleType: 规则类型，当前只有all
         :type RuleType: str
         :param RuleValue: 规则值，['*']
         :type RuleValue: list of str
         :param Action: 执行动作，monitor|intercept|redirect|captcha
         :type Action: str
@@ -1849,15 +1851,17 @@
 class BotJavaScript(AbstractModel):
     """Bot js策略
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: on|off
+        :param Switch: Bot js策略配置开关，取值有：
+on：开启
+off：关闭
         :type Switch: str
         :param RuleType: 规则类型，当前只有file
         :type RuleType: str
         :param RuleValue: 规则值，['html', 'htm']
         :type RuleValue: list of str
         :param Action: 执行动作，monitor|intercept|redirect|captcha
         :type Action: str
@@ -9118,15 +9122,15 @@
 class IpFreqLimit(AbstractModel):
     """单节点单 IP 访问限频配置，默认为关闭状态
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: IP 限频配置开关
+        :param Switch: IP 限频配置开关，取值有：
 on：开启
 off：关闭
         :type Switch: str
         :param Qps: 设置每秒请求数限制
 超出限制的请求会直接返回 514
 注意：此字段可能返回 null，表示取不到有效值。
         :type Qps: int
@@ -9191,21 +9195,23 @@
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class Ipv6(AbstractModel):
-    """Ipv6启用配置，不可更改
+    """Ipv6源站启用配置，不可更改
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 域名是否开启ipv6功能，on或off。
+        :param Switch: 域名开启源站ipv6配置开关，取值有：
+on：开启
+off：关闭
 注意：此字段可能返回 null，表示取不到有效值。
         :type Switch: str
         """
         self.Switch = None
 
 
     def _deserialize(self, params):
@@ -9222,15 +9228,17 @@
 class Ipv6Access(AbstractModel):
     """Ipv6访问配置
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 域名是否开启ipv6访问功能，on或off。
+        :param Switch: 域名开启ipv6访问配置开关，取值有：
+on：开启
+off：关闭
 注意：此字段可能返回 null，表示取不到有效值。
         :type Switch: str
         """
         self.Switch = None
 
 
     def _deserialize(self, params):
@@ -10662,15 +10670,15 @@
 class MaxAge(AbstractModel):
     """浏览器缓存规则配置，用于设置 MaxAge 默认值，默认为关闭状态
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 浏览器缓存配置开关
+        :param Switch: 浏览器缓存配置开关，取值有：
 on：开启
 off：关闭
 注意：此字段可能返回 null，表示取不到有效值。
         :type Switch: str
         :param MaxAgeRules: MaxAge 规则
 注意：此字段可能返回 null，表示取不到有效值。
         :type MaxAgeRules: list of MaxAgeRule
@@ -10839,15 +10847,17 @@
 class OfflineCache(AbstractModel):
     """离线缓存是否开启
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: on | off, 离线缓存是否开启
+        :param Switch: 离线缓存配置开关，取值有：
+on：开启
+off：关闭
         :type Switch: str
         """
         self.Switch = None
 
 
     def _deserialize(self, params):
         self.Switch = params.get("Switch")
@@ -11011,15 +11021,18 @@
 class OriginAuthentication(AbstractModel):
     """回源鉴权高级配置
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 鉴权开关，on或off
+        :param Switch: 回源鉴权高级配置开关，取值有：
+on：开启
+off：关闭
+
 注意：此字段可能返回 null，表示取不到有效值。
         :type Switch: str
         :param TypeA: 鉴权类型A配置
 注意：此字段可能返回 null，表示取不到有效值。
         :type TypeA: :class:`tencentcloud.cdn.v20180606.models.OriginAuthenticationTypeA`
         """
         self.Switch = None
@@ -11068,15 +11081,17 @@
 class OriginCombine(AbstractModel):
     """合并回源配置项
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: on|off 是否开启合并回源
+        :param Switch: 合并回源配置开关，取值有：
+on：开启
+off：关闭
         :type Switch: str
         """
         self.Switch = None
 
 
     def _deserialize(self, params):
         self.Switch = params.get("Switch")
@@ -11116,15 +11131,15 @@
 class OriginPullOptimization(AbstractModel):
     """跨国回源优化配置，默认为关闭状态 (已下线)
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 跨国回源优化配置开关
+        :param Switch: 跨国回源优化配置开关，取值有：
 on：开启
 off：关闭
         :type Switch: str
         :param OptimizationType: 跨国类型
 OVToCN：境外回源境内
 CNToOV：境内回源境外
 注意：此字段可能返回 null，表示取不到有效值。
@@ -11179,15 +11194,17 @@
 class OssPrivateAccess(AbstractModel):
     """oss回源鉴权
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 开关， on/off。
+        :param Switch: oss回源鉴权配置开关，取值有：
+on：开启
+off：关闭
         :type Switch: str
         :param AccessKey: 访问ID。
 注意：此字段可能返回 null，表示取不到有效值。
         :type AccessKey: str
         :param SecretKey: 密钥。
 注意：此字段可能返回 null，表示取不到有效值。
         :type SecretKey: str
@@ -11223,15 +11240,17 @@
 class OthersPrivateAccess(AbstractModel):
     """其他厂商对象存储回源鉴权
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 开关， on/off。
+        :param Switch: 其他厂商对象存储回源鉴权配置开关，取值有：
+on：开启
+off：关闭
         :type Switch: str
         :param AccessKey: 访问ID。
 注意：此字段可能返回 null，表示取不到有效值。
         :type AccessKey: str
         :param SecretKey: 密钥。
 注意：此字段可能返回 null，表示取不到有效值。
         :type SecretKey: str
@@ -11946,15 +11965,17 @@
 class QnPrivateAccess(AbstractModel):
     """七牛元对象存储回源鉴权配置
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 开关 on/off
+        :param Switch: 七牛元对象存储回源鉴权配置开关，取值有：
+on：开启
+off：关闭
         :type Switch: str
         :param AccessKey: 访问 ID
 注意：此字段可能返回 null，表示取不到有效值。
         :type AccessKey: str
         :param SecretKey: 密钥
         :type SecretKey: str
         """
@@ -12025,15 +12046,17 @@
 class Quic(AbstractModel):
     """Quic配置项
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 是否启动Quic配置
+        :param Switch: Quic功能配置开关，取值有：
+on：开启
+off：关闭
         :type Switch: str
         """
         self.Switch = None
 
 
     def _deserialize(self, params):
         self.Switch = params.get("Switch")
@@ -12085,15 +12108,15 @@
 class RangeOriginPull(AbstractModel):
     """分片回源配置，默认为开启状态
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 分片回源配置开关
+        :param Switch: 分片回源配置开关，取值有：
 on：开启
 off：关闭
         :type Switch: str
         :param RangeRules: 分路径分片回源配置
 注意：此字段可能返回 null，表示取不到有效值。
         :type RangeRules: list of RangeOriginPullRule
         """
@@ -12121,15 +12144,17 @@
 class RangeOriginPullRule(AbstractModel):
     """分路径分片回源配置
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 分片回源配置开关
+        :param Switch: 分片回源配置开关，取值有：
+on：开启
+off：关闭
         :type Switch: str
         :param RuleType: 规则类型：
 file：指定文件后缀生效
 directory：指定路径生效
 path：指定绝对路径生效
 注意：此字段可能返回 null，表示取不到有效值。
         :type RuleType: str
@@ -12161,15 +12186,17 @@
 class RedirectConfig(AbstractModel):
     """自定义回源302 follow请求host配置
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 配置开关
+        :param Switch: 自定义回源302 follow请求host配置开关，取值有：
+on：开启
+off：关闭
         :type Switch: str
         :param FollowRedirectHost: 主源站follow302请求时带的自定义的host头部
         :type FollowRedirectHost: str
         :param FollowRedirectBackupHost: 备份源站follow302请求时带的自定义的host头部
         :type FollowRedirectBackupHost: str
         """
         self.Switch = None
@@ -12193,15 +12220,15 @@
 class Referer(AbstractModel):
     """Referer 黑白名单配置，默认为关闭状态
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: referer 黑白名单配置开关
+        :param Switch: referer 黑白名单配置开关，取值有：
 on：开启
 off：关闭
         :type Switch: str
         :param RefererRules: referer 黑白名单配置规则
 注意：此字段可能返回 null，表示取不到有效值。
         :type RefererRules: list of RefererRule
         """
@@ -12311,17 +12338,17 @@
     RemoteAuthenticationRules和Server 互斥，只需要配置其中一个。
     若只配置Server ，RemoteAuthenticationRules中详细规则参数将采用默认参数；默认参数值见各个配置项中说明；
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 远程鉴权开关；
-on : 开启;
-off: 关闭；
+        :param Switch: 远程鉴权配置开关，取值有：
+on：开启
+off：关闭
 注意：此字段可能返回 null，表示取不到有效值。
         :type Switch: str
         :param RemoteAuthenticationRules: 远程鉴权规则配置
 注意：此字段可能返回 null，表示取不到有效值。
         :type RemoteAuthenticationRules: list of RemoteAuthenticationRule
         :param Server: 远程鉴权Server
 注意：此字段可能返回 null，表示取不到有效值。
@@ -12460,15 +12487,15 @@
 class RequestHeader(AbstractModel):
     """自定义请求头配置，默认为关闭状态
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 自定义请求头配置开关
+        :param Switch: 自定义请求头配置开关，取值有：
 on：开启
 off：关闭
         :type Switch: str
         :param HeaderRules: 自定义请求头配置规则
 注意：此字段可能返回 null，表示取不到有效值。
         :type HeaderRules: list of HttpHeaderPathRule
         """
@@ -12607,15 +12634,15 @@
 class ResponseHeader(AbstractModel):
     """自定义响应头配置，默认为关闭状态
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 自定义响应头开关
+        :param Switch: 自定义响应头配置开关，取值有：
 on：开启
 off：关闭
         :type Switch: str
         :param HeaderRules: 自定义响应头规则
 注意：此字段可能返回 null，表示取不到有效值。
         :type HeaderRules: list of HttpHeaderPathRule
         """
@@ -12643,15 +12670,15 @@
 class ResponseHeaderCache(AbstractModel):
     """源站头部缓存配置，默认为开启状态，缓存所有头部信息
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 源站头部缓存开关
+        :param Switch: 源站头部缓存配置开关，取值有：
 on：开启
 off：关闭
         :type Switch: str
         """
         self.Switch = None
 
 
@@ -12789,15 +12816,15 @@
 class RuleEngine(AbstractModel):
     """规则引擎配置
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 规则引擎配置开关
+        :param Switch: 规则引擎配置开关，取值有：
 on：开启
 off：关闭
         :type Switch: str
         :param Content: 规则
 注意：此字段可能返回 null，表示取不到有效值。
         :type Content: str
         """
@@ -12855,15 +12882,17 @@
 class ScdnAclConfig(AbstractModel):
     """SCDN访问控制
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 是否开启，on | off
+        :param Switch: SCDN访问控制配置开关，取值有：
+on：开启
+off：关闭
         :type Switch: str
         :param ScriptData: 新版本请使用AdvancedScriptData
 注意：此字段可能返回 null，表示取不到有效值。
         :type ScriptData: list of ScdnAclGroup
         :param ErrorPage: 错误页面配置
 注意：此字段可能返回 null，表示取不到有效值。
         :type ErrorPage: :class:`tencentcloud.cdn.v20180606.models.ScdnErrorPage`
@@ -12986,15 +13015,17 @@
 class ScdnBotConfig(AbstractModel):
     """bot配置类型
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: on|off
+        :param Switch: Scdn bot配置开关，取值有：
+on：开启
+off：关闭
         :type Switch: str
         :param BotCookie: Bot cookie策略
 注意：此字段可能返回 null，表示取不到有效值。
         :type BotCookie: list of BotCookie
         :param BotJavaScript: Bot Js策略
 注意：此字段可能返回 null，表示取不到有效值。
         :type BotJavaScript: list of BotJavaScript
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.893/PKG-INFO` & `tencentcloud-sdk-python-cdn-3.0.894/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdn
-Version: 3.0.893
+Version: 3.0.894
 Summary: Tencent Cloud Cdn SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.893/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdn-3.0.894/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdn
-Version: 3.0.893
+Version: 3.0.894
 Summary: Tencent Cloud Cdn SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.893/setup.py` & `tencentcloud-sdk-python-cdn-3.0.894/setup.py`

 * *Files identical despite different names*

