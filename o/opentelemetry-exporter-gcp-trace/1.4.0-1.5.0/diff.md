# Comparing `tmp/opentelemetry-exporter-gcp-trace-1.4.0.tar.gz` & `tmp/opentelemetry-exporter-gcp-trace-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentelemetry-exporter-gcp-trace-1.4.0.tar", last modified: Mon Dec  5 19:53:18 2022, max compression
+gzip compressed data, was "opentelemetry-exporter-gcp-trace-1.5.0.tar", last modified: Wed May 17 22:49:48 2023, max compression
```

## Comparing `opentelemetry-exporter-gcp-trace-1.4.0.tar` & `opentelemetry-exporter-gcp-trace-1.5.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2022-12-05 19:53:18.799289 opentelemetry-exporter-gcp-trace-1.4.0/
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     3275 2022-12-05 19:23:47.000000 opentelemetry-exporter-gcp-trace-1.4.0/CHANGELOG.md
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)    11357 2022-11-02 23:10:13.000000 opentelemetry-exporter-gcp-trace-1.4.0/LICENSE
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)      169 2022-11-02 23:10:13.000000 opentelemetry-exporter-gcp-trace-1.4.0/MANIFEST.in
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     2598 2022-12-05 19:53:18.799289 opentelemetry-exporter-gcp-trace-1.4.0/PKG-INFO
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1701 2022-11-02 23:10:13.000000 opentelemetry-exporter-gcp-trace-1.4.0/README.rst
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1295 2022-12-05 19:53:18.799289 opentelemetry-exporter-gcp-trace-1.4.0/setup.cfg
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)      987 2022-11-02 23:10:13.000000 opentelemetry-exporter-gcp-trace-1.4.0/setup.py
-drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2022-12-05 19:53:18.791289 opentelemetry-exporter-gcp-trace-1.4.0/src/
-drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2022-12-05 19:53:18.795289 opentelemetry-exporter-gcp-trace-1.4.0/src/opentelemetry/
-drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2022-12-05 19:53:18.791289 opentelemetry-exporter-gcp-trace-1.4.0/src/opentelemetry/exporter/
-drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2022-12-05 19:53:18.795289 opentelemetry-exporter-gcp-trace-1.4.0/src/opentelemetry/exporter/cloud_trace/
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)    19040 2022-12-05 17:05:36.000000 opentelemetry-exporter-gcp-trace-1.4.0/src/opentelemetry/exporter/cloud_trace/__init__.py
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1301 2022-11-02 23:10:13.000000 opentelemetry-exporter-gcp-trace-1.4.0/src/opentelemetry/exporter/cloud_trace/environment_variables.py
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)      597 2022-12-05 19:52:57.000000 opentelemetry-exporter-gcp-trace-1.4.0/src/opentelemetry/exporter/cloud_trace/version.py
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)        0 2022-11-02 23:10:13.000000 opentelemetry-exporter-gcp-trace-1.4.0/src/opentelemetry/py.typed
-drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2022-12-05 19:53:18.795289 opentelemetry-exporter-gcp-trace-1.4.0/src/opentelemetry_exporter_gcp_trace.egg-info/
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     2598 2022-12-05 19:53:18.000000 opentelemetry-exporter-gcp-trace-1.4.0/src/opentelemetry_exporter_gcp_trace.egg-info/PKG-INFO
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)      740 2022-12-05 19:53:18.000000 opentelemetry-exporter-gcp-trace-1.4.0/src/opentelemetry_exporter_gcp_trace.egg-info/SOURCES.txt
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)        1 2022-12-05 19:53:18.000000 opentelemetry-exporter-gcp-trace-1.4.0/src/opentelemetry_exporter_gcp_trace.egg-info/dependency_links.txt
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)      211 2022-12-05 19:53:18.000000 opentelemetry-exporter-gcp-trace-1.4.0/src/opentelemetry_exporter_gcp_trace.egg-info/entry_points.txt
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)       78 2022-12-05 19:53:18.000000 opentelemetry-exporter-gcp-trace-1.4.0/src/opentelemetry_exporter_gcp_trace.egg-info/requires.txt
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)       14 2022-12-05 19:53:18.000000 opentelemetry-exporter-gcp-trace-1.4.0/src/opentelemetry_exporter_gcp_trace.egg-info/top_level.txt
-drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2022-12-05 19:53:18.799289 opentelemetry-exporter-gcp-trace-1.4.0/tests/
--rw-r--r--   0 aaronabbott (793466) primarygroup (89939)     1269 2022-11-03 01:25:48.000000 opentelemetry-exporter-gcp-trace-1.4.0/tests/test_cloud_trace_auto_instrument.py
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)    28501 2022-12-05 17:05:36.000000 opentelemetry-exporter-gcp-trace-1.4.0/tests/test_cloud_trace_exporter.py
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     2602 2022-11-02 23:10:13.000000 opentelemetry-exporter-gcp-trace-1.4.0/tests/test_integration_cloud_trace_exporter.py
+drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2023-05-17 22:49:48.719638 opentelemetry-exporter-gcp-trace-1.5.0/
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     3437 2023-05-17 22:44:40.000000 opentelemetry-exporter-gcp-trace-1.5.0/CHANGELOG.md
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)    11357 2022-11-02 23:10:13.000000 opentelemetry-exporter-gcp-trace-1.5.0/LICENSE
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)      169 2022-11-02 23:10:13.000000 opentelemetry-exporter-gcp-trace-1.5.0/MANIFEST.in
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     2647 2023-05-17 22:49:48.719638 opentelemetry-exporter-gcp-trace-1.5.0/PKG-INFO
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1701 2022-11-02 23:10:13.000000 opentelemetry-exporter-gcp-trace-1.5.0/README.rst
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1392 2023-05-17 22:49:48.719638 opentelemetry-exporter-gcp-trace-1.5.0/setup.cfg
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)      987 2022-11-02 23:10:13.000000 opentelemetry-exporter-gcp-trace-1.5.0/setup.py
+drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2023-05-17 22:49:48.715638 opentelemetry-exporter-gcp-trace-1.5.0/src/
+drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2023-05-17 22:49:48.715638 opentelemetry-exporter-gcp-trace-1.5.0/src/opentelemetry/
+drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2023-05-17 22:49:48.715638 opentelemetry-exporter-gcp-trace-1.5.0/src/opentelemetry/exporter/
+drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2023-05-17 22:49:48.715638 opentelemetry-exporter-gcp-trace-1.5.0/src/opentelemetry/exporter/cloud_trace/
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)    18625 2023-05-09 15:30:15.000000 opentelemetry-exporter-gcp-trace-1.5.0/src/opentelemetry/exporter/cloud_trace/__init__.py
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1301 2022-11-02 23:10:13.000000 opentelemetry-exporter-gcp-trace-1.5.0/src/opentelemetry/exporter/cloud_trace/environment_variables.py
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)      597 2023-05-17 22:48:33.000000 opentelemetry-exporter-gcp-trace-1.5.0/src/opentelemetry/exporter/cloud_trace/version.py
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)        0 2022-11-02 23:10:13.000000 opentelemetry-exporter-gcp-trace-1.5.0/src/opentelemetry/py.typed
+drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2023-05-17 22:49:48.719638 opentelemetry-exporter-gcp-trace-1.5.0/src/opentelemetry_exporter_gcp_trace.egg-info/
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     2647 2023-05-17 22:49:48.000000 opentelemetry-exporter-gcp-trace-1.5.0/src/opentelemetry_exporter_gcp_trace.egg-info/PKG-INFO
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)      740 2023-05-17 22:49:48.000000 opentelemetry-exporter-gcp-trace-1.5.0/src/opentelemetry_exporter_gcp_trace.egg-info/SOURCES.txt
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)        1 2023-05-17 22:49:48.000000 opentelemetry-exporter-gcp-trace-1.5.0/src/opentelemetry_exporter_gcp_trace.egg-info/dependency_links.txt
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)      210 2023-05-17 22:49:48.000000 opentelemetry-exporter-gcp-trace-1.5.0/src/opentelemetry_exporter_gcp_trace.egg-info/entry_points.txt
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)      130 2023-05-17 22:49:48.000000 opentelemetry-exporter-gcp-trace-1.5.0/src/opentelemetry_exporter_gcp_trace.egg-info/requires.txt
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)       14 2023-05-17 22:49:48.000000 opentelemetry-exporter-gcp-trace-1.5.0/src/opentelemetry_exporter_gcp_trace.egg-info/top_level.txt
+drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2023-05-17 22:49:48.719638 opentelemetry-exporter-gcp-trace-1.5.0/tests/
+-rw-r--r--   0 aaronabbott (793466) primarygroup (89939)     1269 2022-11-03 01:25:48.000000 opentelemetry-exporter-gcp-trace-1.5.0/tests/test_cloud_trace_auto_instrument.py
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)    27757 2023-02-23 16:04:11.000000 opentelemetry-exporter-gcp-trace-1.5.0/tests/test_cloud_trace_exporter.py
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     2602 2022-11-02 23:10:13.000000 opentelemetry-exporter-gcp-trace-1.5.0/tests/test_integration_cloud_trace_exporter.py
```

### Comparing `opentelemetry-exporter-gcp-trace-1.4.0/CHANGELOG.md` & `opentelemetry-exporter-gcp-trace-1.5.0/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Changelog
 
 ## Unreleased
 
+## Version 1.5.0
+
+Released 2023-05-17
+
+- Add support for Python 3.11
+  ([#240](https://github.com/GoogleCloudPlatform/opentelemetry-operations-python/pull/240))
+
 ## Version 1.4.0
 
 Released 2022-12-05
 
 - Set gRPC user-agent when calling google APIs
   ([#216](https://github.com/GoogleCloudPlatform/opentelemetry-operations-python/pull/216))
 - Drop support for Python 3.6, add 3.10
```

### Comparing `opentelemetry-exporter-gcp-trace-1.4.0/LICENSE` & `opentelemetry-exporter-gcp-trace-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-gcp-trace-1.4.0/PKG-INFO` & `opentelemetry-exporter-gcp-trace-1.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-exporter-gcp-trace
-Version: 1.4.0
+Version: 1.5.0
 Summary: Google Cloud Trace exporter for OpenTelemetry
 Home-page: https://github.com/GoogleCloudPlatform/opentelemetry-operations-python/tree/main/opentelemetry-exporter-gcp-trace
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
 
 OpenTelemetry Google Cloud Integration
 ======================================
@@ -73,9 +74,7 @@
 
 
 References
 ----------
 
 * `Cloud Trace <https://cloud.google.com/trace/>`_
 * `OpenTelemetry Project <https://opentelemetry.io/>`_
-
-
```

### Comparing `opentelemetry-exporter-gcp-trace-1.4.0/README.rst` & `opentelemetry-exporter-gcp-trace-1.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-gcp-trace-1.4.0/setup.cfg` & `opentelemetry-exporter-gcp-trace-1.5.0/setup.cfg`

 * *Files 4% similar despite different names*

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
 	google-cloud-trace ~= 1.1
 	opentelemetry-api ~= 1.0
 	opentelemetry-sdk ~= 1.0
+	opentelemetry-resourcedetector-gcp >= 1.5.0dev0, == 1.*
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 test =
```

### Comparing `opentelemetry-exporter-gcp-trace-1.4.0/setup.py` & `opentelemetry-exporter-gcp-trace-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-gcp-trace-1.4.0/src/opentelemetry/exporter/cloud_trace/__init__.py` & `opentelemetry-exporter-gcp-trace-1.5.0/src/opentelemetry/exporter/cloud_trace/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,14 +98,20 @@
 )
 from google.rpc import code_pb2, status_pb2
 from opentelemetry.exporter.cloud_trace.environment_variables import (
     OTEL_EXPORTER_GCP_TRACE_PROJECT_ID,
     OTEL_EXPORTER_GCP_TRACE_RESOURCE_REGEX,
 )
 from opentelemetry.exporter.cloud_trace.version import __version__
+from opentelemetry.resourcedetector.gcp_resource_detector import (
+    _constants as _resource_constants,
+)
+from opentelemetry.resourcedetector.gcp_resource_detector._mapping import (
+    get_monitored_resource,
+)
 from opentelemetry.sdk.resources import Resource
 from opentelemetry.sdk.trace import Event
 from opentelemetry.sdk.trace.export import (
     ReadableSpan,
     SpanExporter,
     SpanExportResult,
 )
@@ -124,14 +130,15 @@
 # https://github.com/googleapis/python-trace/blob/v1.7.3/google/cloud/trace_v1/services/trace_service/transports/grpc.py#L177-L180
 _OPTIONS = [
     ("grpc.max_send_message_length", -1),
     ("grpc.max_receive_message_length", -1),
     ("grpc.primary_user_agent", _USER_AGENT),
 ]
 
+
 MAX_NUM_LINKS = 128
 MAX_NUM_EVENTS = 32
 MAX_EVENT_ATTRS = 4
 MAX_LINK_ATTRS = 32
 MAX_SPAN_ATTRS = 32
 MAX_ATTR_KEY_BYTES = 128
 MAX_ATTR_VAL_BYTES = 16 * 1024  # 16 kilobytes
@@ -416,63 +423,39 @@
     )
 
 
 def _strip_characters(ot_version):
     return "".join(filter(lambda x: x.isdigit() or x == ".", ot_version))
 
 
-OT_RESOURCE_ATTRIBUTE_TO_GCP = {
-    "gce_instance": {
-        "host.id": "instance_id",
-        "cloud.account.id": "project_id",
-        "cloud.zone": "zone",
-    },
-    "gke_container": {
-        "k8s.cluster.name": "cluster_name",
-        "k8s.namespace.name": "namespace_id",
-        "k8s.pod.name": "pod_id",
-        "host.id": "instance_id",
-        "container.name": "container_name",
-        "cloud.account.id": "project_id",
-        "cloud.zone": "zone",
-    },
-}
-
-
 def _extract_resources(
     resource: Resource, resource_regex: Optional[Pattern] = None
 ) -> Dict[str, str]:
     extracted_attributes = {}
     resource_attributes = resource.attributes
     if resource_regex:
         extracted_attributes.update(
             {
                 k: str(v)
                 for k, v in resource_attributes.items()
                 if resource_regex.match(k)
             }
         )
-    if resource_attributes.get("cloud.provider") != "gcp":
-        return extracted_attributes
-    resource_type = resource_attributes["gcp.resource_type"]
-    if (
-        not isinstance(resource_type, str)
-        or resource_type not in OT_RESOURCE_ATTRIBUTE_TO_GCP
+    monitored_resource = get_monitored_resource(resource)
+    # Do not map generic_task and generic_node to g.co/r/... span labels.
+    if monitored_resource and monitored_resource.type not in (
+        _resource_constants.GENERIC_NODE,
+        _resource_constants.GENERIC_TASK,
     ):
-        return extracted_attributes
-    extracted_attributes.update(
-        {
-            "g.co/r/{}/{}".format(resource_type, gcp_resource_key): str(
-                resource_attributes[ot_resource_key]
-            )
-            for ot_resource_key, gcp_resource_key in OT_RESOURCE_ATTRIBUTE_TO_GCP[
-                resource_type
-            ].items()
-        }
-    )
+        extracted_attributes.update(
+            {
+                "g.co/r/{}/{}".format(monitored_resource.type, k): v
+                for k, v in monitored_resource.labels.items()
+            }
+        )
     return extracted_attributes
 
 
 LABELS_MAPPING = {
     # this one might be http.flavor? I'm not sure
     "http.scheme": "/http/client_protocol",
     "http.host": "/http/host",
```

### Comparing `opentelemetry-exporter-gcp-trace-1.4.0/src/opentelemetry/exporter/cloud_trace/environment_variables.py` & `opentelemetry-exporter-gcp-trace-1.5.0/src/opentelemetry/exporter/cloud_trace/environment_variables.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-gcp-trace-1.4.0/src/opentelemetry/exporter/cloud_trace/version.py` & `opentelemetry-exporter-gcp-trace-1.5.0/src/opentelemetry/exporter/cloud_trace/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "1.4.0"
+__version__ = "1.5.0"
```

### Comparing `opentelemetry-exporter-gcp-trace-1.4.0/src/opentelemetry_exporter_gcp_trace.egg-info/PKG-INFO` & `opentelemetry-exporter-gcp-trace-1.5.0/src/opentelemetry_exporter_gcp_trace.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-exporter-gcp-trace
-Version: 1.4.0
+Version: 1.5.0
 Summary: Google Cloud Trace exporter for OpenTelemetry
 Home-page: https://github.com/GoogleCloudPlatform/opentelemetry-operations-python/tree/main/opentelemetry-exporter-gcp-trace
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
 
 OpenTelemetry Google Cloud Integration
 ======================================
@@ -73,9 +74,7 @@
 
 
 References
 ----------
 
 * `Cloud Trace <https://cloud.google.com/trace/>`_
 * `OpenTelemetry Project <https://opentelemetry.io/>`_
-
-
```

### Comparing `opentelemetry-exporter-gcp-trace-1.4.0/src/opentelemetry_exporter_gcp_trace.egg-info/SOURCES.txt` & `opentelemetry-exporter-gcp-trace-1.5.0/src/opentelemetry_exporter_gcp_trace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-gcp-trace-1.4.0/tests/test_cloud_trace_auto_instrument.py` & `opentelemetry-exporter-gcp-trace-1.5.0/tests/test_cloud_trace_auto_instrument.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-gcp-trace-1.4.0/tests/test_cloud_trace_exporter.py` & `opentelemetry-exporter-gcp-trace-1.5.0/tests/test_cloud_trace_exporter.py`

 * *Files 5% similar despite different names*

```diff
@@ -120,19 +120,22 @@
 
         self.assertIs(exporter.client, client)
         self.assertEqual(exporter.project_id, self.project_id)
 
     def test_export(self):
         resource_info = Resource(
             {
-                "cloud.account.id": 123,
-                "host.id": "host",
-                "cloud.zone": "US",
+                "cloud.account.id": "123",
+                "cloud.platform": "gcp_compute_engine",
                 "cloud.provider": "gcp",
-                "gcp.resource_type": "gce_instance",
+                "cloud.region": "us-east4",
+                "cloud.availability_zone": "us-east4-b",
+                "host.id": "host",
+                "host.name": "fakeName",
+                "host.type": "fakeMachineType",
             }
         )
         span_datas = [
             Span(
                 name="span_name",
                 context=SpanContext(
                     trace_id=int(self.example_trace_id, 16),
@@ -153,21 +156,20 @@
             "span_id": self.example_span_id,
             "parent_span_id": None,
             "display_name": TruncatableString(
                 value="span_name", truncated_byte_count=0
             ),
             "attributes": ProtoSpan.Attributes(
                 attribute_map={
-                    "g.co/r/gce_instance/zone": _format_attribute_value("US"),
+                    "g.co/r/gce_instance/zone": _format_attribute_value(
+                        "us-east4-b"
+                    ),
                     "g.co/r/gce_instance/instance_id": _format_attribute_value(
                         "host"
                     ),
-                    "g.co/r/gce_instance/project_id": _format_attribute_value(
-                        "123"
-                    ),
                     "g.co/agent": self.agent_code,
                     "attr_key": _format_attribute_value("attr_value"),
                 }
             ),
             "links": None,
             "status": None,
             "time_events": None,
@@ -648,121 +650,102 @@
 
         proto_link = _extract_links([attr_link])
         self.assertEqual(
             len(proto_link.link[0].attributes.attribute_map), MAX_LINK_ATTRS
         )
 
     def test_extract_empty_resources(self):
-        self.assertEqual(_extract_resources(Resource.get_empty()), {})
+        self.assertEqual(
+            _extract_resources(Resource.get_empty()),
+            {},
+        )
 
     def test_extract_resource_attributes_with_regex(self):
         resource_regex = re.compile(r"service\..*")
         resource = Resource(
             attributes={
-                "cloud.account.id": 123,
-                "host.id": "host",
-                "cloud.zone": "US",
+                "cloud.account.id": "123",
+                "cloud.availability_zone": "us-east4-b",
+                "cloud.platform": "gcp_compute_engine",
                 "cloud.provider": "gcp",
-                "extra_info": "extra",
-                "gcp.resource_type": "gce_instance",
-                "not_gcp_resource": "value",
+                "cloud.region": "us-east4",
+                "host.id": "host",
+                "host.name": "fakeName",
+                "host.type": "fakeMachineType",
                 "service.name": "my-app",
                 "service.version": "1",
             }
         )
         expected_extract = {
-            "g.co/r/gce_instance/project_id": "123",
             "g.co/r/gce_instance/instance_id": "host",
-            "g.co/r/gce_instance/zone": "US",
+            "g.co/r/gce_instance/zone": "us-east4-b",
             "service.name": "my-app",
             "service.version": "1",
         }
         self.assertEqual(
             _extract_resources(resource, resource_regex), expected_extract
         )
 
     def test_non_matching_regex(self):
         resource_regex = re.compile(r"this-regex-matches-nothing")
         resource = Resource(
             attributes={
-                "cloud.account.id": 123,
-                "host.id": "host",
-                "cloud.zone": "US",
+                "cloud.account.id": "123",
+                "cloud.availability_zone": "us-east4-b",
+                "cloud.platform": "gcp_compute_engine",
                 "cloud.provider": "gcp",
-                "extra_info": "extra",
-                "gcp.resource_type": "gce_instance",
-                "not_gcp_resource": "value",
+                "cloud.region": "us-east4",
+                "host.id": "host",
+                "host.name": "fakeName",
+                "host.type": "fakeMachineType",
             }
         )
         expected_extract = {
-            "g.co/r/gce_instance/project_id": "123",
             "g.co/r/gce_instance/instance_id": "host",
-            "g.co/r/gce_instance/zone": "US",
+            "g.co/r/gce_instance/zone": "us-east4-b",
         }
         self.assertEqual(
             _extract_resources(resource, resource_regex), expected_extract
         )
 
     def test_extract_well_formed_resources(self):
         resource = Resource(
             attributes={
-                "cloud.account.id": 123,
-                "host.id": "host",
-                "cloud.zone": "US",
+                "cloud.account.id": "123",
+                "cloud.availability_zone": "us-east4-b",
+                "cloud.platform": "gcp_compute_engine",
                 "cloud.provider": "gcp",
-                "extra_info": "extra",
-                "gcp.resource_type": "gce_instance",
-                "not_gcp_resource": "value",
+                "cloud.region": "us-east4",
+                "host.id": "host",
+                "host.name": "fakeName",
+                "host.type": "fakeMachineType",
             }
         )
         expected_extract = {
-            "g.co/r/gce_instance/project_id": "123",
             "g.co/r/gce_instance/instance_id": "host",
-            "g.co/r/gce_instance/zone": "US",
+            "g.co/r/gce_instance/zone": "us-east4-b",
         }
         self.assertEqual(_extract_resources(resource), expected_extract)
 
-    def test_extract_malformed_resources(self):
-        # This resource doesn't have all the fields required for a gce_instance
-        # Specifically its missing "host.id", "cloud.zone", "cloud.account.id"
-        resource = Resource(
-            attributes={
-                "gcp.resource_type": "gce_instance",
-                "cloud.provider": "gcp",
-            }
-        )
-        # Should throw when passed a malformed GCP resource dict
-        self.assertRaises(KeyError, _extract_resources, resource)
-
     def test_extract_unsupported_gcp_resources(self):
         # Unsupported gcp resources will be ignored
         resource = Resource(
             attributes={
                 "cloud.account.id": "123",
                 "host.id": "host",
                 "extra_info": "extra",
                 "not_gcp_resource": "value",
-                "gcp.resource_type": "unsupported_gcp_resource",
+                "cloud.platform": "gcp_some_unsupported_thing",
                 "cloud.provider": "gcp",
             }
         )
-        self.assertEqual(_extract_resources(resource), {})
-
-    def test_extract_unsupported_provider_resources(self):
-        # Resources with currently unsupported providers will be ignored
-        resource = Resource(
-            attributes={
-                "cloud.account.id": "123",
-                "host.id": "host",
-                "extra_info": "extra",
-                "not_gcp_resource": "value",
-                "cloud.provider": "aws",
-            }
+        self.assertEqual(
+            _extract_resources(resource),
+            {},
         )
-        self.assertEqual(_extract_resources(resource), {})
 
     def test_truncate_string(self):
         """Cloud Trace API imposes limits on the length of many things,
         e.g. strings, number of events, number of attributes. We truncate
         these things before sending it to the API as an optimization.
         """
         self.assertEqual(_truncate_str("aaaa", limit=1), ("a", 3))
```

### Comparing `opentelemetry-exporter-gcp-trace-1.4.0/tests/test_integration_cloud_trace_exporter.py` & `opentelemetry-exporter-gcp-trace-1.5.0/tests/test_integration_cloud_trace_exporter.py`

 * *Files identical despite different names*

