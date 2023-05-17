# Comparing `tmp/opentelemetry-resourcedetector-gcp-1.4.0a0.tar.gz` & `tmp/opentelemetry-resourcedetector-gcp-1.5.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentelemetry-resourcedetector-gcp-1.4.0a0.tar", last modified: Mon Dec  5 19:53:19 2022, max compression
+gzip compressed data, was "opentelemetry-resourcedetector-gcp-1.5.0a0.tar", last modified: Wed May 17 22:49:49 2023, max compression
```

## Comparing `opentelemetry-resourcedetector-gcp-1.4.0a0.tar` & `opentelemetry-resourcedetector-gcp-1.5.0a0.tar`

### file list

```diff
@@ -1,23 +1,37 @@
-drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2022-12-05 19:53:19.259289 opentelemetry-resourcedetector-gcp-1.4.0a0/
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1769 2022-12-05 19:23:47.000000 opentelemetry-resourcedetector-gcp-1.4.0a0/CHANGELOG.md
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)    11357 2022-11-02 23:10:13.000000 opentelemetry-resourcedetector-gcp-1.4.0a0/LICENSE
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)      169 2022-11-02 23:10:13.000000 opentelemetry-resourcedetector-gcp-1.4.0a0/MANIFEST.in
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1705 2022-12-05 19:53:19.259289 opentelemetry-resourcedetector-gcp-1.4.0a0/PKG-INFO
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)      799 2022-11-02 23:10:13.000000 opentelemetry-resourcedetector-gcp-1.4.0a0/README.rst
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1056 2022-12-05 19:53:19.259289 opentelemetry-resourcedetector-gcp-1.4.0a0/setup.cfg
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1005 2022-11-02 23:10:13.000000 opentelemetry-resourcedetector-gcp-1.4.0a0/setup.py
-drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2022-12-05 19:53:19.255289 opentelemetry-resourcedetector-gcp-1.4.0a0/src/
-drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2022-12-05 19:53:19.255289 opentelemetry-resourcedetector-gcp-1.4.0a0/src/opentelemetry/
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)        0 2022-11-02 23:10:13.000000 opentelemetry-resourcedetector-gcp-1.4.0a0/src/opentelemetry/py.typed
-drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2022-12-05 19:53:19.255289 opentelemetry-resourcedetector-gcp-1.4.0a0/src/opentelemetry/resourcedetector/
-drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2022-12-05 19:53:19.259289 opentelemetry-resourcedetector-gcp-1.4.0a0/src/opentelemetry/resourcedetector/gcp_resource_detector/
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     6400 2022-11-10 23:25:22.000000 opentelemetry-resourcedetector-gcp-1.4.0a0/src/opentelemetry/resourcedetector/gcp_resource_detector/__init__.py
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)      614 2022-12-05 19:52:57.000000 opentelemetry-resourcedetector-gcp-1.4.0a0/src/opentelemetry/resourcedetector/gcp_resource_detector/version.py
-drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2022-12-05 19:53:19.259289 opentelemetry-resourcedetector-gcp-1.4.0a0/src/opentelemetry_resourcedetector_gcp.egg-info/
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1705 2022-12-05 19:53:19.000000 opentelemetry-resourcedetector-gcp-1.4.0a0/src/opentelemetry_resourcedetector_gcp.egg-info/PKG-INFO
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)      571 2022-12-05 19:53:19.000000 opentelemetry-resourcedetector-gcp-1.4.0a0/src/opentelemetry_resourcedetector_gcp.egg-info/SOURCES.txt
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)        1 2022-12-05 19:53:19.000000 opentelemetry-resourcedetector-gcp-1.4.0a0/src/opentelemetry_resourcedetector_gcp.egg-info/dependency_links.txt
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)       69 2022-12-05 19:53:19.000000 opentelemetry-resourcedetector-gcp-1.4.0a0/src/opentelemetry_resourcedetector_gcp.egg-info/requires.txt
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)       14 2022-12-05 19:53:19.000000 opentelemetry-resourcedetector-gcp-1.4.0a0/src/opentelemetry_resourcedetector_gcp.egg-info/top_level.txt
-drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2022-12-05 19:53:19.259289 opentelemetry-resourcedetector-gcp-1.4.0a0/tests/
--rw-r--r--   0 aaronabbott (793466) primarygroup (89939)    20188 2022-11-03 01:25:48.000000 opentelemetry-resourcedetector-gcp-1.4.0a0/tests/test_gcp_resource_detector.py
+drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2023-05-17 22:49:49.355637 opentelemetry-resourcedetector-gcp-1.5.0a0/
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     2060 2023-05-17 22:44:40.000000 opentelemetry-resourcedetector-gcp-1.5.0a0/CHANGELOG.md
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)    11357 2022-11-02 23:10:13.000000 opentelemetry-resourcedetector-gcp-1.5.0a0/LICENSE
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)      169 2022-11-02 23:10:13.000000 opentelemetry-resourcedetector-gcp-1.5.0a0/MANIFEST.in
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1754 2023-05-17 22:49:49.355637 opentelemetry-resourcedetector-gcp-1.5.0a0/PKG-INFO
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)      799 2022-11-02 23:10:13.000000 opentelemetry-resourcedetector-gcp-1.5.0a0/README.rst
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1122 2023-05-17 22:49:49.355637 opentelemetry-resourcedetector-gcp-1.5.0a0/setup.cfg
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1005 2022-11-02 23:10:13.000000 opentelemetry-resourcedetector-gcp-1.5.0a0/setup.py
+drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2023-05-17 22:49:49.347637 opentelemetry-resourcedetector-gcp-1.5.0a0/src/
+drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2023-05-17 22:49:49.347637 opentelemetry-resourcedetector-gcp-1.5.0a0/src/opentelemetry/
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)        0 2022-11-02 23:10:13.000000 opentelemetry-resourcedetector-gcp-1.5.0a0/src/opentelemetry/py.typed
+drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2023-05-17 22:49:49.347637 opentelemetry-resourcedetector-gcp-1.5.0a0/src/opentelemetry/resourcedetector/
+drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2023-05-17 22:49:49.351637 opentelemetry-resourcedetector-gcp-1.5.0a0/src/opentelemetry/resourcedetector/gcp_resource_detector/
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     6400 2022-11-10 23:25:22.000000 opentelemetry-resourcedetector-gcp-1.5.0a0/src/opentelemetry/resourcedetector/gcp_resource_detector/__init__.py
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     2118 2023-02-23 16:04:11.000000 opentelemetry-resourcedetector-gcp-1.5.0a0/src/opentelemetry/resourcedetector/gcp_resource_detector/_constants.py
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     2737 2023-02-23 16:04:11.000000 opentelemetry-resourcedetector-gcp-1.5.0a0/src/opentelemetry/resourcedetector/gcp_resource_detector/_detector.py
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     2074 2023-02-22 17:34:42.000000 opentelemetry-resourcedetector-gcp-1.5.0a0/src/opentelemetry/resourcedetector/gcp_resource_detector/_gce.py
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1677 2023-02-22 17:34:42.000000 opentelemetry-resourcedetector-gcp-1.5.0a0/src/opentelemetry/resourcedetector/gcp_resource_detector/_gke.py
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     7562 2023-02-23 16:04:11.000000 opentelemetry-resourcedetector-gcp-1.5.0a0/src/opentelemetry/resourcedetector/gcp_resource_detector/_mapping.py
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     2390 2023-02-23 17:11:30.000000 opentelemetry-resourcedetector-gcp-1.5.0a0/src/opentelemetry/resourcedetector/gcp_resource_detector/_metadata.py
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)      614 2023-05-17 22:48:33.000000 opentelemetry-resourcedetector-gcp-1.5.0a0/src/opentelemetry/resourcedetector/gcp_resource_detector/version.py
+drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2023-05-17 22:49:49.351637 opentelemetry-resourcedetector-gcp-1.5.0a0/src/opentelemetry_resourcedetector_gcp.egg-info/
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1754 2023-05-17 22:49:49.000000 opentelemetry-resourcedetector-gcp-1.5.0a0/src/opentelemetry_resourcedetector_gcp.egg-info/PKG-INFO
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1157 2023-05-17 22:49:49.000000 opentelemetry-resourcedetector-gcp-1.5.0a0/src/opentelemetry_resourcedetector_gcp.egg-info/SOURCES.txt
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)        1 2023-05-17 22:49:49.000000 opentelemetry-resourcedetector-gcp-1.5.0a0/src/opentelemetry_resourcedetector_gcp.egg-info/dependency_links.txt
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)       92 2023-05-17 22:49:49.000000 opentelemetry-resourcedetector-gcp-1.5.0a0/src/opentelemetry_resourcedetector_gcp.egg-info/requires.txt
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)       14 2023-05-17 22:49:49.000000 opentelemetry-resourcedetector-gcp-1.5.0a0/src/opentelemetry_resourcedetector_gcp.egg-info/top_level.txt
+drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2023-05-17 22:49:49.351637 opentelemetry-resourcedetector-gcp-1.5.0a0/tests/
+drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2023-05-17 22:49:49.351637 opentelemetry-resourcedetector-gcp-1.5.0a0/tests/__snapshots__/
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1482 2023-04-25 23:09:14.000000 opentelemetry-resourcedetector-gcp-1.5.0a0/tests/__snapshots__/test_detector.ambr
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     4708 2023-02-23 16:04:11.000000 opentelemetry-resourcedetector-gcp-1.5.0a0/tests/__snapshots__/test_mapping.ambr
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1067 2023-02-22 17:34:42.000000 opentelemetry-resourcedetector-gcp-1.5.0a0/tests/conftest.py
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     3291 2023-02-22 17:34:42.000000 opentelemetry-resourcedetector-gcp-1.5.0a0/tests/test_detector.py
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     2424 2023-02-22 17:34:42.000000 opentelemetry-resourcedetector-gcp-1.5.0a0/tests/test_gce.py
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)    19601 2023-02-22 17:34:42.000000 opentelemetry-resourcedetector-gcp-1.5.0a0/tests/test_gcp_resource_detector.py
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     2431 2023-02-22 17:34:42.000000 opentelemetry-resourcedetector-gcp-1.5.0a0/tests/test_gke.py
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     7786 2023-02-23 16:04:11.000000 opentelemetry-resourcedetector-gcp-1.5.0a0/tests/test_mapping.py
```

### Comparing `opentelemetry-resourcedetector-gcp-1.4.0a0/CHANGELOG.md` & `opentelemetry-resourcedetector-gcp-1.5.0a0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 # Changelog
 
 ## Unreleased
 
+## Version 1.5.0a0
+
+Released 2023-05-17
+
+- Add spec compliant GCE detection
+  ([#231](https://github.com/GoogleCloudPlatform/opentelemetry-operations-python/pull/231))
+- Add support for Python 3.11
+  ([#240](https://github.com/GoogleCloudPlatform/opentelemetry-operations-python/pull/240))
+
 ## Version 1.4.0a0
 
 Released 2022-12-05
 
 - Drop support for Python 3.6, add 3.10
   ([#203](https://github.com/GoogleCloudPlatform/opentelemetry-operations-python/pull/203))
 - Update no container name behaviour
```

### Comparing `opentelemetry-resourcedetector-gcp-1.4.0a0/LICENSE` & `opentelemetry-resourcedetector-gcp-1.5.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry-resourcedetector-gcp-1.4.0a0/PKG-INFO` & `opentelemetry-resourcedetector-gcp-1.5.0a0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-resourcedetector-gcp
-Version: 1.4.0a0
+Version: 1.5.0a0
 Summary: Google Cloud resource detector for OpenTelemetry
 Home-page: https://github.com/GoogleCloudPlatform/opentelemetry-operations-python/tree/main/opentelemetry-resourcedetector-gcp
 Author: Google
 Author-email: opentelemetry-pypi@google.com
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -12,14 +12,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE
 
 OpenTelemetry Google Cloud Resource Detector
 ============================================
@@ -45,9 +46,7 @@
 
 
 References
 ----------
 
 * `Cloud Monitoring <https://cloud.google.com/monitoring>`_
 * `OpenTelemetry Project <https://opentelemetry.io/>`_
-
-
```

### Comparing `opentelemetry-resourcedetector-gcp-1.4.0a0/README.rst` & `opentelemetry-resourcedetector-gcp-1.5.0a0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry-resourcedetector-gcp-1.4.0a0/setup.cfg` & `opentelemetry-resourcedetector-gcp-1.5.0a0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -14,24 +14,26 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
 python_requires = >=3.7
 package_dir = 
 	=src
 packages = find_namespace:
 install_requires = 
 	opentelemetry-api ~= 1.0
 	opentelemetry-sdk ~= 1.0
 	requests ~= 2.24
+	typing_extensions ~= 4.0
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 test =
```

### Comparing `opentelemetry-resourcedetector-gcp-1.4.0a0/setup.py` & `opentelemetry-resourcedetector-gcp-1.5.0a0/setup.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-resourcedetector-gcp-1.4.0a0/src/opentelemetry/resourcedetector/gcp_resource_detector/__init__.py` & `opentelemetry-resourcedetector-gcp-1.5.0a0/src/opentelemetry/resourcedetector/gcp_resource_detector/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-resourcedetector-gcp-1.4.0a0/src/opentelemetry/resourcedetector/gcp_resource_detector/version.py` & `opentelemetry-resourcedetector-gcp-1.5.0a0/src/opentelemetry/resourcedetector/gcp_resource_detector/version.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "1.4.0a0"
+__version__ = "1.5.0a0"
```

### Comparing `opentelemetry-resourcedetector-gcp-1.4.0a0/src/opentelemetry_resourcedetector_gcp.egg-info/PKG-INFO` & `opentelemetry-resourcedetector-gcp-1.5.0a0/src/opentelemetry_resourcedetector_gcp.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-resourcedetector-gcp
-Version: 1.4.0a0
+Version: 1.5.0a0
 Summary: Google Cloud resource detector for OpenTelemetry
 Home-page: https://github.com/GoogleCloudPlatform/opentelemetry-operations-python/tree/main/opentelemetry-resourcedetector-gcp
 Author: Google
 Author-email: opentelemetry-pypi@google.com
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -12,14 +12,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE
 
 OpenTelemetry Google Cloud Resource Detector
 ============================================
@@ -45,9 +46,7 @@
 
 
 References
 ----------
 
 * `Cloud Monitoring <https://cloud.google.com/monitoring>`_
 * `OpenTelemetry Project <https://opentelemetry.io/>`_
-
-
```

### Comparing `opentelemetry-resourcedetector-gcp-1.4.0a0/src/opentelemetry_resourcedetector_gcp.egg-info/SOURCES.txt` & `opentelemetry-resourcedetector-gcp-1.5.0a0/src/opentelemetry_resourcedetector_gcp.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -2,14 +2,27 @@
 LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 src/opentelemetry/py.typed
 src/opentelemetry/resourcedetector/gcp_resource_detector/__init__.py
+src/opentelemetry/resourcedetector/gcp_resource_detector/_constants.py
+src/opentelemetry/resourcedetector/gcp_resource_detector/_detector.py
+src/opentelemetry/resourcedetector/gcp_resource_detector/_gce.py
+src/opentelemetry/resourcedetector/gcp_resource_detector/_gke.py
+src/opentelemetry/resourcedetector/gcp_resource_detector/_mapping.py
+src/opentelemetry/resourcedetector/gcp_resource_detector/_metadata.py
 src/opentelemetry/resourcedetector/gcp_resource_detector/version.py
 src/opentelemetry_resourcedetector_gcp.egg-info/PKG-INFO
 src/opentelemetry_resourcedetector_gcp.egg-info/SOURCES.txt
 src/opentelemetry_resourcedetector_gcp.egg-info/dependency_links.txt
 src/opentelemetry_resourcedetector_gcp.egg-info/requires.txt
 src/opentelemetry_resourcedetector_gcp.egg-info/top_level.txt
-tests/test_gcp_resource_detector.py
+tests/conftest.py
+tests/test_detector.py
+tests/test_gce.py
+tests/test_gcp_resource_detector.py
+tests/test_gke.py
+tests/test_mapping.py
+tests/__snapshots__/test_detector.ambr
+tests/__snapshots__/test_mapping.ambr
```

### Comparing `opentelemetry-resourcedetector-gcp-1.4.0a0/tests/test_gcp_resource_detector.py` & `opentelemetry-resourcedetector-gcp-1.5.0a0/tests/test_gcp_resource_detector.py`

 * *Files 9% similar despite different names*

```diff
@@ -91,28 +91,23 @@
 
 
 def pop_environ_key(key):
     if key in os.environ:
         os.environ.pop(key)
 
 
-def clear_gke_env_vars():
-    pop_environ_key(CONTAINER_NAME)
-    pop_environ_key(NAMESPACE)
-    pop_environ_key(HOSTNAME)
-    pop_environ_key(POD_NAME)
+patch_env = mock.patch.dict(os.environ, {}, clear=True)
 
 
+@patch_env
 @mock.patch(
     "opentelemetry.resourcedetector.gcp_resource_detector.requests.get",
     **{"return_value.json.return_value": GKE_RESOURCES_JSON_STRING}
 )
 class TestGKEResourceFinder(unittest.TestCase):
-    def tearDown(self) -> None:
-        clear_gke_env_vars()
 
     # pylint: disable=unused-argument
     def test_not_running_on_gke(self, getter):
         pop_environ_key(KUBERNETES_SERVICE_HOST)
         found_resources = get_gke_resources()
         self.assertEqual(found_resources, {})
 
@@ -217,27 +212,20 @@
                 "cloud.zone": "zone",
                 "cloud.provider": "gcp",
                 "gcp.resource_type": "gke_container",
             },
         )
 
 
-def clear_cloudrun_env_vars():
-    pop_environ_key(K_CONFIGURATION)
-    pop_environ_key(K_SERVICE)
-    pop_environ_key(K_REVISION)
-
-
+@patch_env
 @mock.patch(
     "opentelemetry.resourcedetector.gcp_resource_detector.requests.get",
     **{"return_value.json.return_value": CLOUDRUN_RESOURCES_JSON_STRING}
 )
 class TestCloudRunResourceFinder(unittest.TestCase):
-    def tearDown(self) -> None:
-        clear_cloudrun_env_vars()
 
     # pylint: disable=unused-argument
     def test_not_running_on_cloudrun(self, getter):
         pop_environ_key(K_CONFIGURATION)
         found_resources = get_cloudrun_resources()
         self.assertEqual(found_resources, {})
 
@@ -299,28 +287,20 @@
                 "cloud.zone": "zone",
                 "cloud.provider": "gcp",
                 "gcp.resource_type": "cloud_run",
             },
         )
 
 
-def clear_cloudfunctions_env_vars():
-    pop_environ_key(FUNCTION_TARGET)
-    pop_environ_key(K_SERVICE)
-    pop_environ_key(K_REVISION)
-
-
+@patch_env
 @mock.patch(
     "opentelemetry.resourcedetector.gcp_resource_detector.requests.get",
     **{"return_value.json.return_value": CLOUDFUNCTIONS_RESOURCES_JSON_STRING}
 )
 class TestCloudFunctionsResourceFinder(unittest.TestCase):
-    def tearDown(self) -> None:
-        clear_cloudfunctions_env_vars()
-
     # pylint: disable=unused-argument
     def test_not_running_on_cloudfunctions(self, getter):
         pop_environ_key(FUNCTION_TARGET)
         found_resources = get_cloudfunctions_resources()
         self.assertEqual(found_resources, {})
 
     # pylint: disable=unused-argument
@@ -381,21 +361,19 @@
                 "cloud.zone": "zone",
                 "cloud.provider": "gcp",
                 "gcp.resource_type": "cloud_functions",
             },
         )
 
 
+@patch_env
 @mock.patch(
     "opentelemetry.resourcedetector.gcp_resource_detector.requests.get"
 )
 class TestGoogleCloudResourceDetector(unittest.TestCase):
-    def tearDown(self) -> None:
-        clear_gke_env_vars()
-
     def test_finding_gce_resources(self, getter):
         # The necessary env variables were not set for GKE resource detection
         # to succeed. We should be falling back to detecting GCE resources
         pop_environ_key(KUBERNETES_SERVICE_HOST)
         pop_environ_key(K_CONFIGURATION)
         pop_environ_key(FUNCTION_TARGET)
         resource_finder = GoogleCloudResourceDetector()
```

