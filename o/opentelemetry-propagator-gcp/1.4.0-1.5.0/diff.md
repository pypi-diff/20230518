# Comparing `tmp/opentelemetry-propagator-gcp-1.4.0.tar.gz` & `tmp/opentelemetry-propagator-gcp-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentelemetry-propagator-gcp-1.4.0.tar", last modified: Mon Dec  5 19:53:19 2022, max compression
+gzip compressed data, was "opentelemetry-propagator-gcp-1.5.0.tar", last modified: Wed May 17 22:49:49 2023, max compression
```

## Comparing `opentelemetry-propagator-gcp-1.4.0.tar` & `opentelemetry-propagator-gcp-1.5.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2022-12-05 19:53:19.031289 opentelemetry-propagator-gcp-1.4.0/
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     2144 2022-12-05 19:23:47.000000 opentelemetry-propagator-gcp-1.4.0/CHANGELOG.md
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)    11357 2022-11-02 23:10:13.000000 opentelemetry-propagator-gcp-1.4.0/LICENSE
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)      169 2022-11-02 23:10:13.000000 opentelemetry-propagator-gcp-1.4.0/MANIFEST.in
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     3255 2022-12-05 19:53:19.031289 opentelemetry-propagator-gcp-1.4.0/PKG-INFO
--rw-r--r--   0 aaronabbott (793466) primarygroup (89939)     2370 2022-11-03 01:25:48.000000 opentelemetry-propagator-gcp-1.4.0/README.rst
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1134 2022-12-05 19:53:19.031289 opentelemetry-propagator-gcp-1.4.0/setup.cfg
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1001 2022-11-02 23:10:13.000000 opentelemetry-propagator-gcp-1.4.0/setup.py
-drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2022-12-05 19:53:19.027289 opentelemetry-propagator-gcp-1.4.0/src/
-drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2022-12-05 19:53:19.027289 opentelemetry-propagator-gcp-1.4.0/src/opentelemetry/
-drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2022-12-05 19:53:19.027289 opentelemetry-propagator-gcp-1.4.0/src/opentelemetry/propagators/
-drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2022-12-05 19:53:19.027289 opentelemetry-propagator-gcp-1.4.0/src/opentelemetry/propagators/cloud_trace_propagator/
--rw-r--r--   0 aaronabbott (793466) primarygroup (89939)     4960 2022-11-03 01:25:48.000000 opentelemetry-propagator-gcp-1.4.0/src/opentelemetry/propagators/cloud_trace_propagator/__init__.py
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)      612 2022-12-05 19:52:57.000000 opentelemetry-propagator-gcp-1.4.0/src/opentelemetry/propagators/cloud_trace_propagator/version.py
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)        0 2022-11-02 23:10:13.000000 opentelemetry-propagator-gcp-1.4.0/src/opentelemetry/py.typed
-drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2022-12-05 19:53:19.027289 opentelemetry-propagator-gcp-1.4.0/src/opentelemetry_propagator_gcp.egg-info/
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     3255 2022-12-05 19:53:19.000000 opentelemetry-propagator-gcp-1.4.0/src/opentelemetry_propagator_gcp.egg-info/PKG-INFO
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)      646 2022-12-05 19:53:19.000000 opentelemetry-propagator-gcp-1.4.0/src/opentelemetry_propagator_gcp.egg-info/SOURCES.txt
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)        1 2022-12-05 19:53:19.000000 opentelemetry-propagator-gcp-1.4.0/src/opentelemetry_propagator_gcp.egg-info/dependency_links.txt
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)      116 2022-12-05 19:53:19.000000 opentelemetry-propagator-gcp-1.4.0/src/opentelemetry_propagator_gcp.egg-info/entry_points.txt
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)       31 2022-12-05 19:53:19.000000 opentelemetry-propagator-gcp-1.4.0/src/opentelemetry_propagator_gcp.egg-info/requires.txt
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)       14 2022-12-05 19:53:19.000000 opentelemetry-propagator-gcp-1.4.0/src/opentelemetry_propagator_gcp.egg-info/top_level.txt
-drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2022-12-05 19:53:19.031289 opentelemetry-propagator-gcp-1.4.0/tests/
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     9291 2022-11-10 23:25:22.000000 opentelemetry-propagator-gcp-1.4.0/tests/test_cloud_trace_propagator.py
--rw-r--r--   0 aaronabbott (793466) primarygroup (89939)     1437 2022-11-03 16:15:35.000000 opentelemetry-propagator-gcp-1.4.0/tests/test_cloud_trace_propagator_auto_instrument.py
+drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2023-05-17 22:49:49.035637 opentelemetry-propagator-gcp-1.5.0/
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     2306 2023-05-17 22:44:40.000000 opentelemetry-propagator-gcp-1.5.0/CHANGELOG.md
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)    11357 2022-11-02 23:10:13.000000 opentelemetry-propagator-gcp-1.5.0/LICENSE
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)      169 2022-11-02 23:10:13.000000 opentelemetry-propagator-gcp-1.5.0/MANIFEST.in
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     3304 2023-05-17 22:49:49.035637 opentelemetry-propagator-gcp-1.5.0/PKG-INFO
+-rw-r--r--   0 aaronabbott (793466) primarygroup (89939)     2370 2022-11-03 01:25:48.000000 opentelemetry-propagator-gcp-1.5.0/README.rst
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1174 2023-05-17 22:49:49.035637 opentelemetry-propagator-gcp-1.5.0/setup.cfg
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1001 2022-11-02 23:10:13.000000 opentelemetry-propagator-gcp-1.5.0/setup.py
+drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2023-05-17 22:49:49.035637 opentelemetry-propagator-gcp-1.5.0/src/
+drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2023-05-17 22:49:49.035637 opentelemetry-propagator-gcp-1.5.0/src/opentelemetry/
+drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2023-05-17 22:49:49.035637 opentelemetry-propagator-gcp-1.5.0/src/opentelemetry/propagators/
+drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2023-05-17 22:49:49.035637 opentelemetry-propagator-gcp-1.5.0/src/opentelemetry/propagators/cloud_trace_propagator/
+-rw-r--r--   0 aaronabbott (793466) primarygroup (89939)     4960 2022-11-03 01:25:48.000000 opentelemetry-propagator-gcp-1.5.0/src/opentelemetry/propagators/cloud_trace_propagator/__init__.py
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)      612 2023-05-17 22:48:33.000000 opentelemetry-propagator-gcp-1.5.0/src/opentelemetry/propagators/cloud_trace_propagator/version.py
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)        0 2022-11-02 23:10:13.000000 opentelemetry-propagator-gcp-1.5.0/src/opentelemetry/py.typed
+drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2023-05-17 22:49:49.035637 opentelemetry-propagator-gcp-1.5.0/src/opentelemetry_propagator_gcp.egg-info/
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     3304 2023-05-17 22:49:49.000000 opentelemetry-propagator-gcp-1.5.0/src/opentelemetry_propagator_gcp.egg-info/PKG-INFO
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)      646 2023-05-17 22:49:49.000000 opentelemetry-propagator-gcp-1.5.0/src/opentelemetry_propagator_gcp.egg-info/SOURCES.txt
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)        1 2023-05-17 22:49:49.000000 opentelemetry-propagator-gcp-1.5.0/src/opentelemetry_propagator_gcp.egg-info/dependency_links.txt
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)      115 2023-05-17 22:49:49.000000 opentelemetry-propagator-gcp-1.5.0/src/opentelemetry_propagator_gcp.egg-info/entry_points.txt
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)       31 2023-05-17 22:49:49.000000 opentelemetry-propagator-gcp-1.5.0/src/opentelemetry_propagator_gcp.egg-info/requires.txt
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)       14 2023-05-17 22:49:49.000000 opentelemetry-propagator-gcp-1.5.0/src/opentelemetry_propagator_gcp.egg-info/top_level.txt
+drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2023-05-17 22:49:49.035637 opentelemetry-propagator-gcp-1.5.0/tests/
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     9291 2022-11-10 23:25:22.000000 opentelemetry-propagator-gcp-1.5.0/tests/test_cloud_trace_propagator.py
+-rw-r--r--   0 aaronabbott (793466) primarygroup (89939)     1437 2022-11-03 16:15:35.000000 opentelemetry-propagator-gcp-1.5.0/tests/test_cloud_trace_propagator_auto_instrument.py
```

### Comparing `opentelemetry-propagator-gcp-1.4.0/CHANGELOG.md` & `opentelemetry-propagator-gcp-1.5.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

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
 
 - Drop support for Python 3.6, add 3.10
   ([#203](https://github.com/GoogleCloudPlatform/opentelemetry-operations-python/pull/203))
 - Create a Readonly Propagator to match the golang "One Way" propagator
```

### Comparing `opentelemetry-propagator-gcp-1.4.0/LICENSE` & `opentelemetry-propagator-gcp-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry-propagator-gcp-1.4.0/PKG-INFO` & `opentelemetry-propagator-gcp-1.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-propagator-gcp
-Version: 1.4.0
+Version: 1.5.0
 Summary: Google Cloud propagator for OpenTelemetry
 Home-page: https://github.com/GoogleCloudPlatform/opentelemetry-operations-python/tree/main/opentelemetry-propagator-gcp
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
 
 OpenTelemetry Google Cloud Propagator
 ======================================
@@ -90,9 +91,7 @@
 
 
 References
 ----------
 
 * `Cloud Trace <https://cloud.google.com/trace/>`_
 * `OpenTelemetry Project <https://opentelemetry.io/>`_
-
-
```

### Comparing `opentelemetry-propagator-gcp-1.4.0/README.rst` & `opentelemetry-propagator-gcp-1.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry-propagator-gcp-1.4.0/setup.cfg` & `opentelemetry-propagator-gcp-1.5.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
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
```

### Comparing `opentelemetry-propagator-gcp-1.4.0/setup.py` & `opentelemetry-propagator-gcp-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-propagator-gcp-1.4.0/src/opentelemetry/propagators/cloud_trace_propagator/__init__.py` & `opentelemetry-propagator-gcp-1.5.0/src/opentelemetry/propagators/cloud_trace_propagator/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-propagator-gcp-1.4.0/src/opentelemetry/propagators/cloud_trace_propagator/version.py` & `opentelemetry-propagator-gcp-1.5.0/src/opentelemetry/propagators/cloud_trace_propagator/version.py`

 * *Files 20% similar despite different names*

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

### Comparing `opentelemetry-propagator-gcp-1.4.0/src/opentelemetry_propagator_gcp.egg-info/PKG-INFO` & `opentelemetry-propagator-gcp-1.5.0/src/opentelemetry_propagator_gcp.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-propagator-gcp
-Version: 1.4.0
+Version: 1.5.0
 Summary: Google Cloud propagator for OpenTelemetry
 Home-page: https://github.com/GoogleCloudPlatform/opentelemetry-operations-python/tree/main/opentelemetry-propagator-gcp
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
 
 OpenTelemetry Google Cloud Propagator
 ======================================
@@ -90,9 +91,7 @@
 
 
 References
 ----------
 
 * `Cloud Trace <https://cloud.google.com/trace/>`_
 * `OpenTelemetry Project <https://opentelemetry.io/>`_
-
-
```

### Comparing `opentelemetry-propagator-gcp-1.4.0/src/opentelemetry_propagator_gcp.egg-info/SOURCES.txt` & `opentelemetry-propagator-gcp-1.5.0/src/opentelemetry_propagator_gcp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opentelemetry-propagator-gcp-1.4.0/tests/test_cloud_trace_propagator.py` & `opentelemetry-propagator-gcp-1.5.0/tests/test_cloud_trace_propagator.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-propagator-gcp-1.4.0/tests/test_cloud_trace_propagator_auto_instrument.py` & `opentelemetry-propagator-gcp-1.5.0/tests/test_cloud_trace_propagator_auto_instrument.py`

 * *Files identical despite different names*

