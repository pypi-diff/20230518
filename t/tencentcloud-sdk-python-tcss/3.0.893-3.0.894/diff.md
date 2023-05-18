# Comparing `tmp/tencentcloud-sdk-python-tcss-3.0.893.tar.gz` & `tmp/tencentcloud-sdk-python-tcss-3.0.894.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tcss-3.0.893.tar", last modified: Wed May 17 03:41:34 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tcss-3.0.894.tar", last modified: Thu May 18 00:38:08 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tcss-3.0.893.tar` & `tencentcloud-sdk-python-tcss-3.0.894.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:41:34.000000 tencentcloud-sdk-python-tcss-3.0.893/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-17 03:41:34.000000 tencentcloud-sdk-python-tcss-3.0.893/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:41:34.000000 tencentcloud-sdk-python-tcss-3.0.893/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-17 03:41:34.000000 tencentcloud-sdk-python-tcss-3.0.893/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:41:34.000000 tencentcloud-sdk-python-tcss-3.0.893/tencentcloud/tcss/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:41:34.000000 tencentcloud-sdk-python-tcss-3.0.893/tencentcloud/tcss/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:41:34.000000 tencentcloud-sdk-python-tcss-3.0.893/tencentcloud/tcss/v20201101/
--rw-r--r--   0 root         (0) root         (0)   316128 2023-05-17 03:41:34.000000 tencentcloud-sdk-python-tcss-3.0.893/tencentcloud/tcss/v20201101/tcss_client.py
--rw-r--r--   0 root         (0) root         (0)     3916 2023-05-17 03:41:34.000000 tencentcloud-sdk-python-tcss-3.0.893/tencentcloud/tcss/v20201101/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:41:34.000000 tencentcloud-sdk-python-tcss-3.0.893/tencentcloud/tcss/v20201101/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1015233 2023-05-17 03:41:34.000000 tencentcloud-sdk-python-tcss-3.0.893/tencentcloud/tcss/v20201101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:41:34.000000 tencentcloud-sdk-python-tcss-3.0.893/tencentcloud_sdk_python_tcss.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 03:41:34.000000 tencentcloud-sdk-python-tcss-3.0.893/tencentcloud_sdk_python_tcss.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-05-17 03:41:34.000000 tencentcloud-sdk-python-tcss-3.0.893/tencentcloud_sdk_python_tcss.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-17 03:41:34.000000 tencentcloud-sdk-python-tcss-3.0.893/tencentcloud_sdk_python_tcss.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-17 03:41:34.000000 tencentcloud-sdk-python-tcss-3.0.893/tencentcloud_sdk_python_tcss.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-17 03:41:34.000000 tencentcloud-sdk-python-tcss-3.0.893/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-05-17 03:41:34.000000 tencentcloud-sdk-python-tcss-3.0.893/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-17 03:41:34.000000 tencentcloud-sdk-python-tcss-3.0.893/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:38:08.000000 tencentcloud-sdk-python-tcss-3.0.894/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-18 00:38:08.000000 tencentcloud-sdk-python-tcss-3.0.894/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:38:08.000000 tencentcloud-sdk-python-tcss-3.0.894/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-18 00:38:08.000000 tencentcloud-sdk-python-tcss-3.0.894/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:38:08.000000 tencentcloud-sdk-python-tcss-3.0.894/tencentcloud/tcss/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:38:08.000000 tencentcloud-sdk-python-tcss-3.0.894/tencentcloud/tcss/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:38:08.000000 tencentcloud-sdk-python-tcss-3.0.894/tencentcloud/tcss/v20201101/
+-rw-r--r--   0 root         (0) root         (0)   316128 2023-05-18 00:38:08.000000 tencentcloud-sdk-python-tcss-3.0.894/tencentcloud/tcss/v20201101/tcss_client.py
+-rw-r--r--   0 root         (0) root         (0)     3916 2023-05-18 00:38:08.000000 tencentcloud-sdk-python-tcss-3.0.894/tencentcloud/tcss/v20201101/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:38:08.000000 tencentcloud-sdk-python-tcss-3.0.894/tencentcloud/tcss/v20201101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1015595 2023-05-18 00:38:08.000000 tencentcloud-sdk-python-tcss-3.0.894/tencentcloud/tcss/v20201101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:38:08.000000 tencentcloud-sdk-python-tcss-3.0.894/tencentcloud_sdk_python_tcss.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 00:38:08.000000 tencentcloud-sdk-python-tcss-3.0.894/tencentcloud_sdk_python_tcss.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-05-18 00:38:08.000000 tencentcloud-sdk-python-tcss-3.0.894/tencentcloud_sdk_python_tcss.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-18 00:38:08.000000 tencentcloud-sdk-python-tcss-3.0.894/tencentcloud_sdk_python_tcss.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-18 00:38:08.000000 tencentcloud-sdk-python-tcss-3.0.894/tencentcloud_sdk_python_tcss.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-18 00:38:08.000000 tencentcloud-sdk-python-tcss-3.0.894/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-05-18 00:38:08.000000 tencentcloud-sdk-python-tcss-3.0.894/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-18 00:38:08.000000 tencentcloud-sdk-python-tcss-3.0.894/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.893/README.rst` & `tencentcloud-sdk-python-tcss-3.0.894/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcss-3.0.893/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tcss-3.0.894/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tcss-3.0.893/tencentcloud/tcss/v20201101/tcss_client.py` & `tencentcloud-sdk-python-tcss-3.0.894/tencentcloud/tcss/v20201101/tcss_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcss-3.0.893/tencentcloud/tcss/v20201101/errorcodes.py` & `tencentcloud-sdk-python-tcss-3.0.894/tencentcloud/tcss/v20201101/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcss-3.0.893/tencentcloud/tcss/v20201101/models.py` & `tencentcloud-sdk-python-tcss-3.0.894/tencentcloud/tcss/v20201101/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -14364,24 +14364,28 @@
         :type All: bool
         :param Images: 自定义扫描镜像
 注意：此字段可能返回 null，表示取不到有效值。
         :type Images: list of ImageInfo
         :param Id: 自动以扫描镜像Id
 注意：此字段可能返回 null，表示取不到有效值。
         :type Id: list of int non-negative
+        :param Latest: 是否扫描最新版本镜像
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Latest: bool
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.Enable = None
         self.ScanTime = None
         self.ScanPeriod = None
         self.ScanType = None
         self.All = None
         self.Images = None
         self.Id = None
+        self.Latest = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.Enable = params.get("Enable")
         self.ScanTime = params.get("ScanTime")
         self.ScanPeriod = params.get("ScanPeriod")
@@ -14390,14 +14394,15 @@
         if params.get("Images") is not None:
             self.Images = []
             for item in params.get("Images"):
                 obj = ImageInfo()
                 obj._deserialize(item)
                 self.Images.append(obj)
         self.Id = params.get("Id")
+        self.Latest = params.get("Latest")
         self.RequestId = params.get("RequestId")
 
 
 class DescribeImageRiskSummaryRequest(AbstractModel):
     """DescribeImageRiskSummary请求参数结构体
 
     """
@@ -28141,22 +28146,25 @@
         :type ScanType: list of str
         :param Images: 扫描镜像
         :type Images: list of ImageInfo
         :param All: 是否扫描所有
         :type All: bool
         :param Id: 扫描镜像Id
         :type Id: list of int non-negative
+        :param Latest: 是否扫描最新版本
+        :type Latest: bool
         """
         self.ScanPeriod = None
         self.Enable = None
         self.ScanTime = None
         self.ScanType = None
         self.Images = None
         self.All = None
         self.Id = None
+        self.Latest = None
 
 
     def _deserialize(self, params):
         self.ScanPeriod = params.get("ScanPeriod")
         self.Enable = params.get("Enable")
         self.ScanTime = params.get("ScanTime")
         self.ScanType = params.get("ScanType")
@@ -28164,14 +28172,15 @@
             self.Images = []
             for item in params.get("Images"):
                 obj = ImageInfo()
                 obj._deserialize(item)
                 self.Images.append(obj)
         self.All = params.get("All")
         self.Id = params.get("Id")
+        self.Latest = params.get("Latest")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.893/tencentcloud_sdk_python_tcss.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tcss-3.0.894/tencentcloud_sdk_python_tcss.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcss
-Version: 3.0.893
+Version: 3.0.894
 Summary: Tencent Cloud Tcss SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.893/PKG-INFO` & `tencentcloud-sdk-python-tcss-3.0.894/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcss
-Version: 3.0.893
+Version: 3.0.894
 Summary: Tencent Cloud Tcss SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.893/setup.py` & `tencentcloud-sdk-python-tcss-3.0.894/setup.py`

 * *Files identical despite different names*

