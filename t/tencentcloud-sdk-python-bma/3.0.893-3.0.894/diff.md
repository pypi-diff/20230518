# Comparing `tmp/tencentcloud-sdk-python-bma-3.0.893.tar.gz` & `tmp/tencentcloud-sdk-python-bma-3.0.894.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-bma-3.0.893.tar", last modified: Wed May 17 03:23:42 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-bma-3.0.894.tar", last modified: Thu May 18 00:17:17 2023, max compression
```

## Comparing `tencentcloud-sdk-python-bma-3.0.893.tar` & `tencentcloud-sdk-python-bma-3.0.894.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:23:42.000000 tencentcloud-sdk-python-bma-3.0.893/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-17 03:23:42.000000 tencentcloud-sdk-python-bma-3.0.893/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:23:42.000000 tencentcloud-sdk-python-bma-3.0.893/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:23:42.000000 tencentcloud-sdk-python-bma-3.0.893/tencentcloud/bma/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:23:42.000000 tencentcloud-sdk-python-bma-3.0.893/tencentcloud/bma/v20210624/
--rw-r--r--   0 root         (0) root         (0)     1829 2023-05-17 03:23:42.000000 tencentcloud-sdk-python-bma-3.0.893/tencentcloud/bma/v20210624/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    25791 2023-05-17 03:23:42.000000 tencentcloud-sdk-python-bma-3.0.893/tencentcloud/bma/v20210624/bma_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:23:42.000000 tencentcloud-sdk-python-bma-3.0.893/tencentcloud/bma/v20210624/__init__.py
--rw-r--r--   0 root         (0) root         (0)    82603 2023-05-17 03:23:42.000000 tencentcloud-sdk-python-bma-3.0.893/tencentcloud/bma/v20210624/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:23:42.000000 tencentcloud-sdk-python-bma-3.0.893/tencentcloud/bma/v20221115/
--rw-r--r--   0 root         (0) root         (0)     3348 2023-05-17 03:23:42.000000 tencentcloud-sdk-python-bma-3.0.893/tencentcloud/bma/v20221115/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    10527 2023-05-17 03:23:42.000000 tencentcloud-sdk-python-bma-3.0.893/tencentcloud/bma/v20221115/bma_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:23:42.000000 tencentcloud-sdk-python-bma-3.0.893/tencentcloud/bma/v20221115/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38994 2023-05-17 03:23:42.000000 tencentcloud-sdk-python-bma-3.0.893/tencentcloud/bma/v20221115/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:23:42.000000 tencentcloud-sdk-python-bma-3.0.893/tencentcloud/bma/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-17 03:23:42.000000 tencentcloud-sdk-python-bma-3.0.893/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-17 03:23:42.000000 tencentcloud-sdk-python-bma-3.0.893/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:23:42.000000 tencentcloud-sdk-python-bma-3.0.893/tencentcloud_sdk_python_bma.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 03:23:42.000000 tencentcloud-sdk-python-bma-3.0.893/tencentcloud_sdk_python_bma.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-05-17 03:23:42.000000 tencentcloud-sdk-python-bma-3.0.893/tencentcloud_sdk_python_bma.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-17 03:23:42.000000 tencentcloud-sdk-python-bma-3.0.893/tencentcloud_sdk_python_bma.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-17 03:23:42.000000 tencentcloud-sdk-python-bma-3.0.893/tencentcloud_sdk_python_bma.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-17 03:23:42.000000 tencentcloud-sdk-python-bma-3.0.893/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-17 03:23:42.000000 tencentcloud-sdk-python-bma-3.0.893/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:17:17.000000 tencentcloud-sdk-python-bma-3.0.894/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-18 00:17:17.000000 tencentcloud-sdk-python-bma-3.0.894/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:17:17.000000 tencentcloud-sdk-python-bma-3.0.894/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:17:17.000000 tencentcloud-sdk-python-bma-3.0.894/tencentcloud/bma/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:17:17.000000 tencentcloud-sdk-python-bma-3.0.894/tencentcloud/bma/v20210624/
+-rw-r--r--   0 root         (0) root         (0)     1829 2023-05-18 00:17:17.000000 tencentcloud-sdk-python-bma-3.0.894/tencentcloud/bma/v20210624/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    25791 2023-05-18 00:17:17.000000 tencentcloud-sdk-python-bma-3.0.894/tencentcloud/bma/v20210624/bma_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:17:17.000000 tencentcloud-sdk-python-bma-3.0.894/tencentcloud/bma/v20210624/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    82603 2023-05-18 00:17:17.000000 tencentcloud-sdk-python-bma-3.0.894/tencentcloud/bma/v20210624/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:17:17.000000 tencentcloud-sdk-python-bma-3.0.894/tencentcloud/bma/v20221115/
+-rw-r--r--   0 root         (0) root         (0)     3348 2023-05-18 00:17:17.000000 tencentcloud-sdk-python-bma-3.0.894/tencentcloud/bma/v20221115/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    10527 2023-05-18 00:17:17.000000 tencentcloud-sdk-python-bma-3.0.894/tencentcloud/bma/v20221115/bma_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:17:17.000000 tencentcloud-sdk-python-bma-3.0.894/tencentcloud/bma/v20221115/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39167 2023-05-18 00:17:17.000000 tencentcloud-sdk-python-bma-3.0.894/tencentcloud/bma/v20221115/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:17:17.000000 tencentcloud-sdk-python-bma-3.0.894/tencentcloud/bma/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-18 00:17:17.000000 tencentcloud-sdk-python-bma-3.0.894/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-18 00:17:17.000000 tencentcloud-sdk-python-bma-3.0.894/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:17:17.000000 tencentcloud-sdk-python-bma-3.0.894/tencentcloud_sdk_python_bma.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 00:17:17.000000 tencentcloud-sdk-python-bma-3.0.894/tencentcloud_sdk_python_bma.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-05-18 00:17:17.000000 tencentcloud-sdk-python-bma-3.0.894/tencentcloud_sdk_python_bma.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-18 00:17:17.000000 tencentcloud-sdk-python-bma-3.0.894/tencentcloud_sdk_python_bma.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-18 00:17:17.000000 tencentcloud-sdk-python-bma-3.0.894/tencentcloud_sdk_python_bma.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-18 00:17:17.000000 tencentcloud-sdk-python-bma-3.0.894/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-18 00:17:17.000000 tencentcloud-sdk-python-bma-3.0.894/setup.cfg
```

### Comparing `tencentcloud-sdk-python-bma-3.0.893/README.rst` & `tencentcloud-sdk-python-bma-3.0.894/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bma-3.0.893/tencentcloud/bma/v20210624/errorcodes.py` & `tencentcloud-sdk-python-bma-3.0.894/tencentcloud/bma/v20210624/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bma-3.0.893/tencentcloud/bma/v20210624/bma_client.py` & `tencentcloud-sdk-python-bma-3.0.894/tencentcloud/bma/v20210624/bma_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bma-3.0.893/tencentcloud/bma/v20210624/models.py` & `tencentcloud-sdk-python-bma-3.0.894/tencentcloud/bma/v20210624/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bma-3.0.893/tencentcloud/bma/v20221115/errorcodes.py` & `tencentcloud-sdk-python-bma-3.0.894/tencentcloud/bma/v20221115/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bma-3.0.893/tencentcloud/bma/v20221115/bma_client.py` & `tencentcloud-sdk-python-bma-3.0.894/tencentcloud/bma/v20221115/bma_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bma-3.0.893/tencentcloud/bma/v20221115/models.py` & `tencentcloud-sdk-python-bma-3.0.894/tencentcloud/bma/v20221115/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,14 +132,16 @@
         :type ProtectURLs: list of str
         :param ProtectAPPs: 保护应用
         :type ProtectAPPs: list of str
         :param ProtectOfficialAccounts: 保护公众号
         :type ProtectOfficialAccounts: list of str
         :param ProtectMiniPrograms: 保护小程序
         :type ProtectMiniPrograms: list of str
+        :param APISource: 请求来源：0-反钓鱼 2-反假冒
+        :type APISource: int
         """
         self.BrandName = None
         self.CompanyName = None
         self.BrandLogo = None
         self.Phone = None
         self.License = None
         self.Authorization = None
@@ -147,14 +149,15 @@
         self.Trademarks = None
         self.IsTransfers = None
         self.Transfers = None
         self.ProtectURLs = None
         self.ProtectAPPs = None
         self.ProtectOfficialAccounts = None
         self.ProtectMiniPrograms = None
+        self.APISource = None
 
 
     def _deserialize(self, params):
         self.BrandName = params.get("BrandName")
         self.CompanyName = params.get("CompanyName")
         self.BrandLogo = params.get("BrandLogo")
         self.Phone = params.get("Phone")
@@ -164,14 +167,15 @@
         self.Trademarks = params.get("Trademarks")
         self.IsTransfers = params.get("IsTransfers")
         self.Transfers = params.get("Transfers")
         self.ProtectURLs = params.get("ProtectURLs")
         self.ProtectAPPs = params.get("ProtectAPPs")
         self.ProtectOfficialAccounts = params.get("ProtectOfficialAccounts")
         self.ProtectMiniPrograms = params.get("ProtectMiniPrograms")
+        self.APISource = params.get("APISource")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-bma-3.0.893/tencentcloud/__init__.py` & `tencentcloud-sdk-python-bma-3.0.894/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-bma-3.0.893/PKG-INFO` & `tencentcloud-sdk-python-bma-3.0.894/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-bma
-Version: 3.0.893
+Version: 3.0.894
 Summary: Tencent Cloud Bma SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-bma-3.0.893/tencentcloud_sdk_python_bma.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-bma-3.0.894/tencentcloud_sdk_python_bma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bma-3.0.893/tencentcloud_sdk_python_bma.egg-info/PKG-INFO` & `tencentcloud-sdk-python-bma-3.0.894/tencentcloud_sdk_python_bma.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-bma
-Version: 3.0.893
+Version: 3.0.894
 Summary: Tencent Cloud Bma SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-bma-3.0.893/setup.py` & `tencentcloud-sdk-python-bma-3.0.894/setup.py`

 * *Files identical despite different names*

