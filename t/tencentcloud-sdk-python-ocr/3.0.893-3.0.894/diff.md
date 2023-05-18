# Comparing `tmp/tencentcloud-sdk-python-ocr-3.0.893.tar.gz` & `tmp/tencentcloud-sdk-python-ocr-3.0.894.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.893.tar", last modified: Wed May 17 03:36:58 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.894.tar", last modified: Thu May 18 00:32:57 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ocr-3.0.893.tar` & `tencentcloud-sdk-python-ocr-3.0.894.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:36:58.000000 tencentcloud-sdk-python-ocr-3.0.893/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:36:58.000000 tencentcloud-sdk-python-ocr-3.0.893/tencentcloud_sdk_python_ocr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 03:36:58.000000 tencentcloud-sdk-python-ocr-3.0.893/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-17 03:36:58.000000 tencentcloud-sdk-python-ocr-3.0.893/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-17 03:36:58.000000 tencentcloud-sdk-python-ocr-3.0.893/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-17 03:36:58.000000 tencentcloud-sdk-python-ocr-3.0.893/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-17 03:36:58.000000 tencentcloud-sdk-python-ocr-3.0.893/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:36:58.000000 tencentcloud-sdk-python-ocr-3.0.893/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:36:58.000000 tencentcloud-sdk-python-ocr-3.0.893/tencentcloud/ocr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:36:58.000000 tencentcloud-sdk-python-ocr-3.0.893/tencentcloud/ocr/v20181119/
--rw-r--r--   0 root         (0) root         (0)   113504 2023-05-17 03:36:58.000000 tencentcloud-sdk-python-ocr-3.0.893/tencentcloud/ocr/v20181119/ocr_client.py
--rw-r--r--   0 root         (0) root         (0)     5764 2023-05-17 03:36:58.000000 tencentcloud-sdk-python-ocr-3.0.893/tencentcloud/ocr/v20181119/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:36:58.000000 tencentcloud-sdk-python-ocr-3.0.893/tencentcloud/ocr/v20181119/__init__.py
--rw-r--r--   0 root         (0) root         (0)   505442 2023-05-17 03:36:58.000000 tencentcloud-sdk-python-ocr-3.0.893/tencentcloud/ocr/v20181119/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:36:58.000000 tencentcloud-sdk-python-ocr-3.0.893/tencentcloud/ocr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-17 03:36:58.000000 tencentcloud-sdk-python-ocr-3.0.893/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-17 03:36:58.000000 tencentcloud-sdk-python-ocr-3.0.893/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-17 03:36:58.000000 tencentcloud-sdk-python-ocr-3.0.893/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-17 03:36:58.000000 tencentcloud-sdk-python-ocr-3.0.893/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:32:57.000000 tencentcloud-sdk-python-ocr-3.0.894/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:32:57.000000 tencentcloud-sdk-python-ocr-3.0.894/tencentcloud_sdk_python_ocr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 00:32:57.000000 tencentcloud-sdk-python-ocr-3.0.894/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-18 00:32:57.000000 tencentcloud-sdk-python-ocr-3.0.894/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-18 00:32:57.000000 tencentcloud-sdk-python-ocr-3.0.894/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-18 00:32:57.000000 tencentcloud-sdk-python-ocr-3.0.894/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-18 00:32:57.000000 tencentcloud-sdk-python-ocr-3.0.894/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:32:57.000000 tencentcloud-sdk-python-ocr-3.0.894/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:32:57.000000 tencentcloud-sdk-python-ocr-3.0.894/tencentcloud/ocr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:32:57.000000 tencentcloud-sdk-python-ocr-3.0.894/tencentcloud/ocr/v20181119/
+-rw-r--r--   0 root         (0) root         (0)   113504 2023-05-18 00:32:57.000000 tencentcloud-sdk-python-ocr-3.0.894/tencentcloud/ocr/v20181119/ocr_client.py
+-rw-r--r--   0 root         (0) root         (0)     5764 2023-05-18 00:32:57.000000 tencentcloud-sdk-python-ocr-3.0.894/tencentcloud/ocr/v20181119/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:32:57.000000 tencentcloud-sdk-python-ocr-3.0.894/tencentcloud/ocr/v20181119/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   505442 2023-05-18 00:32:57.000000 tencentcloud-sdk-python-ocr-3.0.894/tencentcloud/ocr/v20181119/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:32:57.000000 tencentcloud-sdk-python-ocr-3.0.894/tencentcloud/ocr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-18 00:32:57.000000 tencentcloud-sdk-python-ocr-3.0.894/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-18 00:32:57.000000 tencentcloud-sdk-python-ocr-3.0.894/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-18 00:32:57.000000 tencentcloud-sdk-python-ocr-3.0.894/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-18 00:32:57.000000 tencentcloud-sdk-python-ocr-3.0.894/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.893/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.894/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.893
+Version: 3.0.894
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.893/README.rst` & `tencentcloud-sdk-python-ocr-3.0.894/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.893/tencentcloud/ocr/v20181119/ocr_client.py` & `tencentcloud-sdk-python-ocr-3.0.894/tencentcloud/ocr/v20181119/ocr_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.893/tencentcloud/ocr/v20181119/errorcodes.py` & `tencentcloud-sdk-python-ocr-3.0.894/tencentcloud/ocr/v20181119/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.893/tencentcloud/ocr/v20181119/models.py` & `tencentcloud-sdk-python-ocr-3.0.894/tencentcloud/ocr/v20181119/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.893/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ocr-3.0.894/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ocr-3.0.893/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.894/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.893
+Version: 3.0.894
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.893/setup.py` & `tencentcloud-sdk-python-ocr-3.0.894/setup.py`

 * *Files identical despite different names*
