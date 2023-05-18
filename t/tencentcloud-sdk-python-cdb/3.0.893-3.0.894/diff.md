# Comparing `tmp/tencentcloud-sdk-python-cdb-3.0.893.tar.gz` & `tmp/tencentcloud-sdk-python-cdb-3.0.894.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdb-3.0.893.tar", last modified: Wed May 17 03:25:21 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdb-3.0.894.tar", last modified: Thu May 18 00:19:21 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cdb-3.0.893.tar` & `tencentcloud-sdk-python-cdb-3.0.894.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:25:21.000000 tencentcloud-sdk-python-cdb-3.0.893/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-17 03:25:21.000000 tencentcloud-sdk-python-cdb-3.0.893/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:25:21.000000 tencentcloud-sdk-python-cdb-3.0.893/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:25:21.000000 tencentcloud-sdk-python-cdb-3.0.893/tencentcloud/cdb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:25:21.000000 tencentcloud-sdk-python-cdb-3.0.893/tencentcloud/cdb/v20170320/
--rw-r--r--   0 root         (0) root         (0)   151787 2023-05-17 03:25:21.000000 tencentcloud-sdk-python-cdb-3.0.893/tencentcloud/cdb/v20170320/cdb_client.py
--rw-r--r--   0 root         (0) root         (0)    18943 2023-05-17 03:25:21.000000 tencentcloud-sdk-python-cdb-3.0.893/tencentcloud/cdb/v20170320/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:25:21.000000 tencentcloud-sdk-python-cdb-3.0.893/tencentcloud/cdb/v20170320/__init__.py
--rw-r--r--   0 root         (0) root         (0)   528913 2023-05-17 03:25:21.000000 tencentcloud-sdk-python-cdb-3.0.893/tencentcloud/cdb/v20170320/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:25:21.000000 tencentcloud-sdk-python-cdb-3.0.893/tencentcloud/cdb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-17 03:25:21.000000 tencentcloud-sdk-python-cdb-3.0.893/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-17 03:25:21.000000 tencentcloud-sdk-python-cdb-3.0.893/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:25:21.000000 tencentcloud-sdk-python-cdb-3.0.893/tencentcloud_sdk_python_cdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 03:25:21.000000 tencentcloud-sdk-python-cdb-3.0.893/tencentcloud_sdk_python_cdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-17 03:25:21.000000 tencentcloud-sdk-python-cdb-3.0.893/tencentcloud_sdk_python_cdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-17 03:25:21.000000 tencentcloud-sdk-python-cdb-3.0.893/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-17 03:25:21.000000 tencentcloud-sdk-python-cdb-3.0.893/tencentcloud_sdk_python_cdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-17 03:25:21.000000 tencentcloud-sdk-python-cdb-3.0.893/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-17 03:25:21.000000 tencentcloud-sdk-python-cdb-3.0.893/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.894/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-18 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.894/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.894/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.894/tencentcloud/cdb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.894/tencentcloud/cdb/v20170320/
+-rw-r--r--   0 root         (0) root         (0)   151787 2023-05-18 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.894/tencentcloud/cdb/v20170320/cdb_client.py
+-rw-r--r--   0 root         (0) root         (0)    18943 2023-05-18 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.894/tencentcloud/cdb/v20170320/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.894/tencentcloud/cdb/v20170320/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   529181 2023-05-18 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.894/tencentcloud/cdb/v20170320/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.894/tencentcloud/cdb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-18 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.894/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-18 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.894/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.894/tencentcloud_sdk_python_cdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.894/tencentcloud_sdk_python_cdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-18 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.894/tencentcloud_sdk_python_cdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-18 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.894/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-18 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.894/tencentcloud_sdk_python_cdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-18 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.894/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-18 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.894/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.893/README.rst` & `tencentcloud-sdk-python-cdb-3.0.894/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.893/tencentcloud/cdb/v20170320/cdb_client.py` & `tencentcloud-sdk-python-cdb-3.0.894/tencentcloud/cdb/v20170320/cdb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.893/tencentcloud/cdb/v20170320/errorcodes.py` & `tencentcloud-sdk-python-cdb-3.0.894/tencentcloud/cdb/v20170320/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.893/tencentcloud/cdb/v20170320/models.py` & `tencentcloud-sdk-python-cdb-3.0.894/tencentcloud/cdb/v20170320/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6836,24 +6836,28 @@
         :type TotalCount: int
         :param Items: 参数详情
         :type Items: list of ParameterDetail
         :param Description: 参数模板描述
         :type Description: str
         :param TemplateType: 参数模板类型。支持值包括："HIGH_STABILITY" - 高稳定模板，"HIGH_PERFORMANCE" - 高性能模板。
         :type TemplateType: str
+        :param EngineType: 参数模板引擎。支持值包括："InnoDB"，"RocksDB"。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type EngineType: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.TemplateId = None
         self.Name = None
         self.EngineVersion = None
         self.TotalCount = None
         self.Items = None
         self.Description = None
         self.TemplateType = None
+        self.EngineType = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.TemplateId = params.get("TemplateId")
         self.Name = params.get("Name")
         self.EngineVersion = params.get("EngineVersion")
@@ -6862,14 +6866,15 @@
             self.Items = []
             for item in params.get("Items"):
                 obj = ParameterDetail()
                 obj._deserialize(item)
                 self.Items.append(obj)
         self.Description = params.get("Description")
         self.TemplateType = params.get("TemplateType")
+        self.EngineType = params.get("EngineType")
         self.RequestId = params.get("RequestId")
 
 
 class DescribeParamTemplatesRequest(AbstractModel):
     """DescribeParamTemplates请求参数结构体
 
     """
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.893/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdb-3.0.894/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cdb-3.0.893/PKG-INFO` & `tencentcloud-sdk-python-cdb-3.0.894/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdb
-Version: 3.0.893
+Version: 3.0.894
 Summary: Tencent Cloud Cdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.893/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdb-3.0.894/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdb
-Version: 3.0.893
+Version: 3.0.894
 Summary: Tencent Cloud Cdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.893/setup.py` & `tencentcloud-sdk-python-cdb-3.0.894/setup.py`

 * *Files identical despite different names*

