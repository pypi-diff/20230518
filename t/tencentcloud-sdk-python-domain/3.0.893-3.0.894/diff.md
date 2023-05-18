# Comparing `tmp/tencentcloud-sdk-python-domain-3.0.893.tar.gz` & `tmp/tencentcloud-sdk-python-domain-3.0.894.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-domain-3.0.893.tar", last modified: Wed May 17 03:29:43 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-domain-3.0.894.tar", last modified: Thu May 18 00:24:22 2023, max compression
```

## Comparing `tencentcloud-sdk-python-domain-3.0.893.tar` & `tencentcloud-sdk-python-domain-3.0.894.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:29:43.000000 tencentcloud-sdk-python-domain-3.0.893/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:29:43.000000 tencentcloud-sdk-python-domain-3.0.893/tencentcloud_sdk_python_domain.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 03:29:43.000000 tencentcloud-sdk-python-domain-3.0.893/tencentcloud_sdk_python_domain.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-05-17 03:29:43.000000 tencentcloud-sdk-python-domain-3.0.893/tencentcloud_sdk_python_domain.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-05-17 03:29:43.000000 tencentcloud-sdk-python-domain-3.0.893/tencentcloud_sdk_python_domain.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-17 03:29:43.000000 tencentcloud-sdk-python-domain-3.0.893/tencentcloud_sdk_python_domain.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      746 2023-05-17 03:29:43.000000 tencentcloud-sdk-python-domain-3.0.893/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:29:43.000000 tencentcloud-sdk-python-domain-3.0.893/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:29:43.000000 tencentcloud-sdk-python-domain-3.0.893/tencentcloud/domain/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:29:43.000000 tencentcloud-sdk-python-domain-3.0.893/tencentcloud/domain/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:29:43.000000 tencentcloud-sdk-python-domain-3.0.893/tencentcloud/domain/v20180808/
--rw-r--r--   0 root         (0) root         (0)    25103 2023-05-17 03:29:43.000000 tencentcloud-sdk-python-domain-3.0.893/tencentcloud/domain/v20180808/domain_client.py
--rw-r--r--   0 root         (0) root         (0)     8787 2023-05-17 03:29:43.000000 tencentcloud-sdk-python-domain-3.0.893/tencentcloud/domain/v20180808/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:29:43.000000 tencentcloud-sdk-python-domain-3.0.893/tencentcloud/domain/v20180808/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75209 2023-05-17 03:29:43.000000 tencentcloud-sdk-python-domain-3.0.893/tencentcloud/domain/v20180808/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-17 03:29:43.000000 tencentcloud-sdk-python-domain-3.0.893/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1674 2023-05-17 03:29:43.000000 tencentcloud-sdk-python-domain-3.0.893/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1012 2023-05-17 03:29:43.000000 tencentcloud-sdk-python-domain-3.0.893/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-17 03:29:43.000000 tencentcloud-sdk-python-domain-3.0.893/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:24:22.000000 tencentcloud-sdk-python-domain-3.0.894/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:24:22.000000 tencentcloud-sdk-python-domain-3.0.894/tencentcloud_sdk_python_domain.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 00:24:22.000000 tencentcloud-sdk-python-domain-3.0.894/tencentcloud_sdk_python_domain.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-05-18 00:24:22.000000 tencentcloud-sdk-python-domain-3.0.894/tencentcloud_sdk_python_domain.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-05-18 00:24:22.000000 tencentcloud-sdk-python-domain-3.0.894/tencentcloud_sdk_python_domain.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-18 00:24:22.000000 tencentcloud-sdk-python-domain-3.0.894/tencentcloud_sdk_python_domain.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      746 2023-05-18 00:24:22.000000 tencentcloud-sdk-python-domain-3.0.894/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:24:22.000000 tencentcloud-sdk-python-domain-3.0.894/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:24:22.000000 tencentcloud-sdk-python-domain-3.0.894/tencentcloud/domain/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:24:22.000000 tencentcloud-sdk-python-domain-3.0.894/tencentcloud/domain/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:24:22.000000 tencentcloud-sdk-python-domain-3.0.894/tencentcloud/domain/v20180808/
+-rw-r--r--   0 root         (0) root         (0)    25103 2023-05-18 00:24:22.000000 tencentcloud-sdk-python-domain-3.0.894/tencentcloud/domain/v20180808/domain_client.py
+-rw-r--r--   0 root         (0) root         (0)     8787 2023-05-18 00:24:22.000000 tencentcloud-sdk-python-domain-3.0.894/tencentcloud/domain/v20180808/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:24:22.000000 tencentcloud-sdk-python-domain-3.0.894/tencentcloud/domain/v20180808/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75443 2023-05-18 00:24:22.000000 tencentcloud-sdk-python-domain-3.0.894/tencentcloud/domain/v20180808/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-18 00:24:22.000000 tencentcloud-sdk-python-domain-3.0.894/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-05-18 00:24:22.000000 tencentcloud-sdk-python-domain-3.0.894/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-05-18 00:24:22.000000 tencentcloud-sdk-python-domain-3.0.894/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-18 00:24:22.000000 tencentcloud-sdk-python-domain-3.0.894/setup.cfg
```

### Comparing `tencentcloud-sdk-python-domain-3.0.893/tencentcloud_sdk_python_domain.egg-info/PKG-INFO` & `tencentcloud-sdk-python-domain-3.0.894/tencentcloud_sdk_python_domain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-domain
-Version: 3.0.893
+Version: 3.0.894
 Summary: Tencent Cloud Domain SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-domain-3.0.893/README.rst` & `tencentcloud-sdk-python-domain-3.0.894/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-domain-3.0.893/tencentcloud/domain/v20180808/domain_client.py` & `tencentcloud-sdk-python-domain-3.0.894/tencentcloud/domain/v20180808/domain_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-domain-3.0.893/tencentcloud/domain/v20180808/errorcodes.py` & `tencentcloud-sdk-python-domain-3.0.894/tencentcloud/domain/v20180808/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-domain-3.0.893/tencentcloud/domain/v20180808/models.py` & `tencentcloud-sdk-python-domain-3.0.894/tencentcloud/domain/v20180808/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,36 +142,41 @@
 GAJZZ: 中国港澳居住证。
 TWJZZ: 中国台湾居住证。
 QTTYDM: 其他-统一社会信用代码证书。
 GZJGZY: 公证机构执业证。
         :type CertificateType: str
         :param ImgUrl: 证件照片地址。
         :type ImgUrl: str
+        :param OriginImgUrl: 原始照片地址
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OriginImgUrl: str
         :param RegistrantCertificateCode: 联系人证件号码。
 注意：此字段可能返回 null，表示取不到有效值。
         :type RegistrantCertificateCode: str
         :param RegistrantCertificateType: 联系人证件类型。
 注意：此字段可能返回 null，表示取不到有效值。
         :type RegistrantCertificateType: str
         :param RegistrantImgUrl: 联系人证件照片地址。
 注意：此字段可能返回 null，表示取不到有效值。
         :type RegistrantImgUrl: str
         """
         self.CertificateCode = None
         self.CertificateType = None
         self.ImgUrl = None
+        self.OriginImgUrl = None
         self.RegistrantCertificateCode = None
         self.RegistrantCertificateType = None
         self.RegistrantImgUrl = None
 
 
     def _deserialize(self, params):
         self.CertificateCode = params.get("CertificateCode")
         self.CertificateType = params.get("CertificateType")
         self.ImgUrl = params.get("ImgUrl")
+        self.OriginImgUrl = params.get("OriginImgUrl")
         self.RegistrantCertificateCode = params.get("RegistrantCertificateCode")
         self.RegistrantCertificateType = params.get("RegistrantCertificateType")
         self.RegistrantImgUrl = params.get("RegistrantImgUrl")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
```

### Comparing `tencentcloud-sdk-python-domain-3.0.893/tencentcloud/__init__.py` & `tencentcloud-sdk-python-domain-3.0.894/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-domain-3.0.893/PKG-INFO` & `tencentcloud-sdk-python-domain-3.0.894/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-domain
-Version: 3.0.893
+Version: 3.0.894
 Summary: Tencent Cloud Domain SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-domain-3.0.893/setup.py` & `tencentcloud-sdk-python-domain-3.0.894/setup.py`

 * *Files identical despite different names*

