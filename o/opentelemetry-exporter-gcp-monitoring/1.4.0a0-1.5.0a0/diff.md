# Comparing `tmp/opentelemetry-exporter-gcp-monitoring-1.4.0a0.tar.gz` & `tmp/opentelemetry-exporter-gcp-monitoring-1.5.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentelemetry-exporter-gcp-monitoring-1.4.0a0.tar", last modified: Mon Dec  5 19:53:18 2022, max compression
+gzip compressed data, was "opentelemetry-exporter-gcp-monitoring-1.5.0a0.tar", last modified: Wed May 17 22:49:48 2023, max compression
```

## Comparing `opentelemetry-exporter-gcp-monitoring-1.4.0a0.tar` & `opentelemetry-exporter-gcp-monitoring-1.5.0a0.tar`

### file list

```diff
@@ -1,48 +1,45 @@
-drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2022-12-05 19:53:18.551290 opentelemetry-exporter-gcp-monitoring-1.4.0a0/
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     2936 2022-12-05 19:23:47.000000 opentelemetry-exporter-gcp-monitoring-1.4.0a0/CHANGELOG.md
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)    11357 2022-11-02 23:10:13.000000 opentelemetry-exporter-gcp-monitoring-1.4.0a0/LICENSE
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)      169 2022-11-02 23:10:13.000000 opentelemetry-exporter-gcp-monitoring-1.4.0a0/MANIFEST.in
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     2759 2022-12-05 19:53:18.551290 opentelemetry-exporter-gcp-monitoring-1.4.0a0/PKG-INFO
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1845 2022-11-02 23:10:13.000000 opentelemetry-exporter-gcp-monitoring-1.4.0a0/README.rst
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1078 2022-12-05 19:53:18.551290 opentelemetry-exporter-gcp-monitoring-1.4.0a0/setup.cfg
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)      992 2022-11-02 23:10:13.000000 opentelemetry-exporter-gcp-monitoring-1.4.0a0/setup.py
-drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2022-12-05 19:53:18.539290 opentelemetry-exporter-gcp-monitoring-1.4.0a0/src/
-drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2022-12-05 19:53:18.539290 opentelemetry-exporter-gcp-monitoring-1.4.0a0/src/opentelemetry/
-drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2022-12-05 19:53:18.539290 opentelemetry-exporter-gcp-monitoring-1.4.0a0/src/opentelemetry/exporter/
-drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2022-12-05 19:53:18.539290 opentelemetry-exporter-gcp-monitoring-1.4.0a0/src/opentelemetry/exporter/cloud_monitoring/
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)    13764 2022-12-05 17:05:36.000000 opentelemetry-exporter-gcp-monitoring-1.4.0a0/src/opentelemetry/exporter/cloud_monitoring/__init__.py
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     8089 2022-11-11 23:55:18.000000 opentelemetry-exporter-gcp-monitoring-1.4.0a0/src/opentelemetry/exporter/cloud_monitoring/_resource.py
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)      614 2022-12-05 19:52:57.000000 opentelemetry-exporter-gcp-monitoring-1.4.0a0/src/opentelemetry/exporter/cloud_monitoring/version.py
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)        0 2022-11-02 23:10:13.000000 opentelemetry-exporter-gcp-monitoring-1.4.0a0/src/opentelemetry/py.typed
-drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2022-12-05 19:53:18.543290 opentelemetry-exporter-gcp-monitoring-1.4.0a0/src/opentelemetry_exporter_gcp_monitoring.egg-info/
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     2759 2022-12-05 19:53:18.000000 opentelemetry-exporter-gcp-monitoring-1.4.0a0/src/opentelemetry_exporter_gcp_monitoring.egg-info/PKG-INFO
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1854 2022-12-05 19:53:18.000000 opentelemetry-exporter-gcp-monitoring-1.4.0a0/src/opentelemetry_exporter_gcp_monitoring.egg-info/SOURCES.txt
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)        1 2022-12-05 19:53:18.000000 opentelemetry-exporter-gcp-monitoring-1.4.0a0/src/opentelemetry_exporter_gcp_monitoring.egg-info/dependency_links.txt
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)       83 2022-12-05 19:53:18.000000 opentelemetry-exporter-gcp-monitoring-1.4.0a0/src/opentelemetry_exporter_gcp_monitoring.egg-info/requires.txt
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)       14 2022-12-05 19:53:18.000000 opentelemetry-exporter-gcp-monitoring-1.4.0a0/src/opentelemetry_exporter_gcp_monitoring.egg-info/top_level.txt
-drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2022-12-05 19:53:18.543290 opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/
-drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2022-12-05 19:53:18.543290 opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/__snapshots__/
-drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2022-12-05 19:53:18.551290 opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/__snapshots__/test_cloud_monitoring/
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1473 2022-11-17 17:34:49.000000 opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/__snapshots__/test_cloud_monitoring/test_counter[float].json
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1472 2022-11-17 17:34:49.000000 opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/__snapshots__/test_cloud_monitoring/test_counter[int].json
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     2696 2022-11-17 17:34:49.000000 opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/__snapshots__/test_cloud_monitoring/test_histogram_default_buckets.json
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1891 2022-11-17 17:34:49.000000 opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/__snapshots__/test_cloud_monitoring/test_histogram_single_bucket.json
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1340 2022-11-17 17:34:49.000000 opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/__snapshots__/test_cloud_monitoring/test_invalid_label_keys.json
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1503 2022-11-17 17:34:49.000000 opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/__snapshots__/test_cloud_monitoring/test_observable_counter[float].json
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1502 2022-11-17 17:34:49.000000 opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/__snapshots__/test_cloud_monitoring/test_observable_counter[int].json
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1451 2022-11-17 17:34:49.000000 opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/__snapshots__/test_cloud_monitoring/test_observable_gauge[float].json
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1450 2022-11-17 17:34:49.000000 opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/__snapshots__/test_cloud_monitoring/test_observable_gauge[int].json
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1475 2022-11-17 17:34:49.000000 opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/__snapshots__/test_cloud_monitoring/test_observable_updowncounter[float].json
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1474 2022-11-17 17:34:49.000000 opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/__snapshots__/test_cloud_monitoring/test_observable_updowncounter[int].json
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1445 2022-11-17 17:34:49.000000 opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/__snapshots__/test_cloud_monitoring/test_up_down_counter[float].json
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1444 2022-11-17 17:34:49.000000 opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/__snapshots__/test_cloud_monitoring/test_up_down_counter[int].json
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1582 2022-11-17 17:34:49.000000 opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/__snapshots__/test_cloud_monitoring/test_with_resource.json
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     4708 2022-11-11 20:00:27.000000 opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/__snapshots__/test_resource.ambr
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)      803 2022-11-08 18:21:08.000000 opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/conftest.py
-drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2022-12-05 19:53:18.551290 opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/fixtures/
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     6080 2022-12-05 17:05:36.000000 opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/fixtures/gcmfake.py
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     2638 2022-12-05 17:05:36.000000 opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/fixtures/snapshot_gcmcalls.py
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     7716 2022-11-15 22:43:14.000000 opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/test_cloud_monitoring.py
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1122 2022-11-10 22:28:18.000000 opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/test_normalize_label_key.py
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     7827 2022-11-11 20:00:27.000000 opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/test_resource.py
--rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1301 2022-12-05 17:05:36.000000 opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/test_user_agent.py
+drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2023-05-17 22:49:48.391639 opentelemetry-exporter-gcp-monitoring-1.5.0a0/
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     3100 2023-05-17 22:44:40.000000 opentelemetry-exporter-gcp-monitoring-1.5.0a0/CHANGELOG.md
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)    11357 2022-11-02 23:10:13.000000 opentelemetry-exporter-gcp-monitoring-1.5.0a0/LICENSE
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)      169 2022-11-02 23:10:13.000000 opentelemetry-exporter-gcp-monitoring-1.5.0a0/MANIFEST.in
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     3365 2023-05-17 22:49:48.391639 opentelemetry-exporter-gcp-monitoring-1.5.0a0/PKG-INFO
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     2402 2023-05-10 18:26:28.000000 opentelemetry-exporter-gcp-monitoring-1.5.0a0/README.rst
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1175 2023-05-17 22:49:48.391639 opentelemetry-exporter-gcp-monitoring-1.5.0a0/setup.cfg
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)      992 2022-11-02 23:10:13.000000 opentelemetry-exporter-gcp-monitoring-1.5.0a0/setup.py
+drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2023-05-17 22:49:48.383638 opentelemetry-exporter-gcp-monitoring-1.5.0a0/src/
+drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2023-05-17 22:49:48.387639 opentelemetry-exporter-gcp-monitoring-1.5.0a0/src/opentelemetry/
+drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2023-05-17 22:49:48.383638 opentelemetry-exporter-gcp-monitoring-1.5.0a0/src/opentelemetry/exporter/
+drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2023-05-17 22:49:48.387639 opentelemetry-exporter-gcp-monitoring-1.5.0a0/src/opentelemetry/exporter/cloud_monitoring/
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)    14360 2023-05-12 02:10:55.000000 opentelemetry-exporter-gcp-monitoring-1.5.0a0/src/opentelemetry/exporter/cloud_monitoring/__init__.py
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)      614 2023-05-17 22:48:33.000000 opentelemetry-exporter-gcp-monitoring-1.5.0a0/src/opentelemetry/exporter/cloud_monitoring/version.py
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)        0 2022-11-02 23:10:13.000000 opentelemetry-exporter-gcp-monitoring-1.5.0a0/src/opentelemetry/py.typed
+drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2023-05-17 22:49:48.387639 opentelemetry-exporter-gcp-monitoring-1.5.0a0/src/opentelemetry_exporter_gcp_monitoring.egg-info/
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     3365 2023-05-17 22:49:48.000000 opentelemetry-exporter-gcp-monitoring-1.5.0a0/src/opentelemetry_exporter_gcp_monitoring.egg-info/PKG-INFO
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1735 2023-05-17 22:49:48.000000 opentelemetry-exporter-gcp-monitoring-1.5.0a0/src/opentelemetry_exporter_gcp_monitoring.egg-info/SOURCES.txt
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)        1 2023-05-17 22:49:48.000000 opentelemetry-exporter-gcp-monitoring-1.5.0a0/src/opentelemetry_exporter_gcp_monitoring.egg-info/dependency_links.txt
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)      135 2023-05-17 22:49:48.000000 opentelemetry-exporter-gcp-monitoring-1.5.0a0/src/opentelemetry_exporter_gcp_monitoring.egg-info/requires.txt
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)       14 2023-05-17 22:49:48.000000 opentelemetry-exporter-gcp-monitoring-1.5.0a0/src/opentelemetry_exporter_gcp_monitoring.egg-info/top_level.txt
+drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2023-05-17 22:49:48.387639 opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/
+drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2023-05-17 22:49:48.383638 opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/__snapshots__/
+drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2023-05-17 22:49:48.391639 opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/__snapshots__/test_cloud_monitoring/
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1473 2022-11-17 17:34:49.000000 opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/__snapshots__/test_cloud_monitoring/test_counter[float].json
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1472 2022-11-17 17:34:49.000000 opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/__snapshots__/test_cloud_monitoring/test_counter[int].json
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     2696 2022-11-17 17:34:49.000000 opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/__snapshots__/test_cloud_monitoring/test_histogram_default_buckets.json
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1891 2022-11-17 17:34:49.000000 opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/__snapshots__/test_cloud_monitoring/test_histogram_single_bucket.json
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1340 2022-11-17 17:34:49.000000 opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/__snapshots__/test_cloud_monitoring/test_invalid_label_keys.json
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1503 2022-11-17 17:34:49.000000 opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/__snapshots__/test_cloud_monitoring/test_observable_counter[float].json
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1502 2022-11-17 17:34:49.000000 opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/__snapshots__/test_cloud_monitoring/test_observable_counter[int].json
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1451 2022-11-17 17:34:49.000000 opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/__snapshots__/test_cloud_monitoring/test_observable_gauge[float].json
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1450 2022-11-17 17:34:49.000000 opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/__snapshots__/test_cloud_monitoring/test_observable_gauge[int].json
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1475 2022-11-17 17:34:49.000000 opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/__snapshots__/test_cloud_monitoring/test_observable_updowncounter[float].json
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1474 2022-11-17 17:34:49.000000 opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/__snapshots__/test_cloud_monitoring/test_observable_updowncounter[int].json
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1445 2022-11-17 17:34:49.000000 opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/__snapshots__/test_cloud_monitoring/test_up_down_counter[float].json
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1444 2022-11-17 17:34:49.000000 opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/__snapshots__/test_cloud_monitoring/test_up_down_counter[int].json
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1582 2022-11-17 17:34:49.000000 opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/__snapshots__/test_cloud_monitoring/test_with_resource.json
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)      803 2022-11-08 18:21:08.000000 opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/conftest.py
+drwxr-x---   0 aaronabbott (793466) primarygroup (89939)        0 2023-05-17 22:49:48.391639 opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/fixtures/
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     6080 2022-12-05 17:05:36.000000 opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/fixtures/gcmfake.py
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     2638 2022-12-05 17:05:36.000000 opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/fixtures/snapshot_gcmcalls.py
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     7852 2023-05-12 02:10:55.000000 opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/test_cloud_monitoring.py
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1122 2022-11-10 22:28:18.000000 opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/test_normalize_label_key.py
+-rw-r-----   0 aaronabbott (793466) primarygroup (89939)     1301 2022-12-05 17:05:36.000000 opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/test_user_agent.py
```

### Comparing `opentelemetry-exporter-gcp-monitoring-1.4.0a0/CHANGELOG.md` & `opentelemetry-exporter-gcp-monitoring-1.5.0a0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Changelog
 
 ## Unreleased
 
+## Version 1.5.0a0
+
+Released 2023-05-17
+
+- Add support for Python 3.11
+  ([#240](https://github.com/GoogleCloudPlatform/opentelemetry-operations-python/pull/240))
+
 ## Version 1.4.0a0
 
 Released 2022-12-05
 
 - Set gRPC user-agent when calling google APIs
   ([#216](https://github.com/GoogleCloudPlatform/opentelemetry-operations-python/pull/216))
 - Implement OTel resource to monitored resource mapping
```

### Comparing `opentelemetry-exporter-gcp-monitoring-1.4.0a0/LICENSE` & `opentelemetry-exporter-gcp-monitoring-1.5.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-gcp-monitoring-1.4.0a0/PKG-INFO` & `opentelemetry-exporter-gcp-monitoring-1.5.0a0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-exporter-gcp-monitoring
-Version: 1.4.0a0
+Version: 1.5.0a0
 Summary: Google Cloud Monitoring exporter for OpenTelemetry
 Home-page: https://github.com/GoogleCloudPlatform/opentelemetry-operations-python/tree/main/opentelemetry-exporter-gcp-monitoring
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
 
 OpenTelemetry Google Cloud Monitoring Exporter
 ==============================================
@@ -54,37 +55,48 @@
 
     import time
 
     from opentelemetry import metrics
     from opentelemetry.exporter.cloud_monitoring import (
         CloudMonitoringMetricsExporter,
     )
-    from opentelemetry.sdk.metrics import Counter, MeterProvider
-
-    metrics.set_meter_provider(MeterProvider())
-    meter = metrics.get_meter(__name__)
-    metrics.get_meter_provider().start_pipeline(
-        meter, CloudMonitoringMetricsExporter(), 5
+    from opentelemetry.sdk.metrics import MeterProvider
+    from opentelemetry.sdk.metrics.export import PeriodicExportingMetricReader
+    from opentelemetry.sdk.resources import Resource
+
+    metrics.set_meter_provider(
+        MeterProvider(
+            metric_readers=[
+                PeriodicExportingMetricReader(
+                    CloudMonitoringMetricsExporter(), export_interval_millis=5000
+                )
+            ],
+            resource=Resource.create(
+                {
+                    "service.name": "basic_metrics",
+                    "service.namespace": "examples",
+                    "service.instance.id": "instance123",
+                }
+            ),
+        )
     )
+    meter = metrics.get_meter(__name__)
 
+    # Creates metric workload.googleapis.com/request_counter with monitored resource generic_task
     requests_counter = meter.create_counter(
         name="request_counter",
         description="number of requests",
         unit="1",
-        value_type=int
     )
 
     staging_labels = {"environment": "staging"}
 
     for i in range(20):
         requests_counter.add(25, staging_labels)
-        time.sleep(10)
-
+        time.sleep(5)
 
 
 References
 ----------
 
 * `Cloud Monitoring <https://cloud.google.com/monitoring>`_
 * `OpenTelemetry Project <https://opentelemetry.io/>`_
-
-
```

### Comparing `opentelemetry-exporter-gcp-monitoring-1.4.0a0/README.rst` & `opentelemetry-exporter-gcp-monitoring-1.5.0a0/README.rst`

 * *Files 27% similar despite different names*

```diff
@@ -31,35 +31,48 @@
 
     import time
 
     from opentelemetry import metrics
     from opentelemetry.exporter.cloud_monitoring import (
         CloudMonitoringMetricsExporter,
     )
-    from opentelemetry.sdk.metrics import Counter, MeterProvider
-
-    metrics.set_meter_provider(MeterProvider())
-    meter = metrics.get_meter(__name__)
-    metrics.get_meter_provider().start_pipeline(
-        meter, CloudMonitoringMetricsExporter(), 5
+    from opentelemetry.sdk.metrics import MeterProvider
+    from opentelemetry.sdk.metrics.export import PeriodicExportingMetricReader
+    from opentelemetry.sdk.resources import Resource
+
+    metrics.set_meter_provider(
+        MeterProvider(
+            metric_readers=[
+                PeriodicExportingMetricReader(
+                    CloudMonitoringMetricsExporter(), export_interval_millis=5000
+                )
+            ],
+            resource=Resource.create(
+                {
+                    "service.name": "basic_metrics",
+                    "service.namespace": "examples",
+                    "service.instance.id": "instance123",
+                }
+            ),
+        )
     )
+    meter = metrics.get_meter(__name__)
 
+    # Creates metric workload.googleapis.com/request_counter with monitored resource generic_task
     requests_counter = meter.create_counter(
         name="request_counter",
         description="number of requests",
         unit="1",
-        value_type=int
     )
 
     staging_labels = {"environment": "staging"}
 
     for i in range(20):
         requests_counter.add(25, staging_labels)
-        time.sleep(10)
-
+        time.sleep(5)
 
 
 References
 ----------
 
 * `Cloud Monitoring <https://cloud.google.com/monitoring>`_
 * `OpenTelemetry Project <https://opentelemetry.io/>`_
```

### Comparing `opentelemetry-exporter-gcp-monitoring-1.4.0a0/setup.cfg` & `opentelemetry-exporter-gcp-monitoring-1.5.0a0/setup.cfg`

 * *Files 14% similar despite different names*

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
 	google-cloud-monitoring ~= 2.0
 	opentelemetry-api ~= 1.0
 	opentelemetry-sdk ~= 1.0
+	opentelemetry-resourcedetector-gcp >= 1.5.0dev0, == 1.*
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 test =
```

### Comparing `opentelemetry-exporter-gcp-monitoring-1.4.0a0/setup.py` & `opentelemetry-exporter-gcp-monitoring-1.5.0a0/setup.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-gcp-monitoring-1.4.0a0/src/opentelemetry/exporter/cloud_monitoring/__init__.py` & `opentelemetry-exporter-gcp-monitoring-1.5.0a0/src/opentelemetry/exporter/cloud_monitoring/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 import google.auth
 import pkg_resources
 from google.api.distribution_pb2 import Distribution
 from google.api.label_pb2 import LabelDescriptor
 from google.api.metric_pb2 import Metric as GMetric
 from google.api.metric_pb2 import MetricDescriptor
+from google.api.monitored_resource_pb2 import MonitoredResource
 from google.cloud.monitoring_v3 import (
     CreateMetricDescriptorRequest,
     CreateTimeSeriesRequest,
     MetricServiceClient,
     Point,
     TimeInterval,
     TimeSeries,
@@ -35,18 +36,18 @@
 )
 from google.cloud.monitoring_v3.services.metric_service.transports.grpc import (
     MetricServiceGrpcTransport,
 )
 
 # pylint: disable=no-name-in-module
 from google.protobuf.timestamp_pb2 import Timestamp
-from opentelemetry.exporter.cloud_monitoring._resource import (
+from opentelemetry.exporter.cloud_monitoring.version import __version__
+from opentelemetry.resourcedetector.gcp_resource_detector._mapping import (
     get_monitored_resource,
 )
-from opentelemetry.exporter.cloud_monitoring.version import __version__
 from opentelemetry.sdk.metrics.export import (
     Gauge,
     Histogram,
     HistogramDataPoint,
     Metric,
     MetricExporter,
     MetricExportResult,
@@ -88,21 +89,24 @@
     Args:
         project_id: project id of your Google Cloud project.
         client: Client to upload metrics to Google Cloud Monitoring.
         add_unique_identifier: Add an identifier to each exporter metric. This
             must be used when there exist two (or more) exporters that may
             export to the same metric name within WRITE_INTERVAL seconds of
             each other.
+        prefix: the prefix of the metric. It is "workload.googleapis.com" by
+            default if not specified.
     """
 
     def __init__(
         self,
         project_id: Optional[str] = None,
         client: Optional[MetricServiceClient] = None,
         add_unique_identifier: bool = False,
+        prefix: Optional[str] = "workload.googleapis.com",
     ):
         # Default preferred_temporality is all CUMULATIVE so need to customize
         super().__init__()
 
         self.client = client or MetricServiceClient(
             transport=MetricServiceGrpcTransport(
                 channel=MetricServiceGrpcTransport.create_channel(
@@ -124,14 +128,15 @@
                 random.randint(0, 16**8)
             )
 
         (
             self._exporter_start_time_seconds,
             self._exporter_start_time_nanos,
         ) = divmod(time_ns(), NANOS_PER_SECOND)
+        self._prefix = prefix
 
     def _batch_write(self, series: List[TimeSeries]) -> None:
         """Cloud Monitoring allows writing up to 200 time series at once
 
         :param series: ProtoBuf TimeSeries
         :return:
         """
@@ -154,15 +159,15 @@
         MetricDescriptor.type. We create the MetricDescriptor if it doesn't
         exist already and cache it. Note that recreating MetricDescriptors is
         a no-op if it already exists.
 
         :param record:
         :return:
         """
-        descriptor_type = f"workload.googleapis.com/{metric.name}"
+        descriptor_type = f"{self._prefix}/{metric.name}"
         if descriptor_type in self._metric_descriptors:
             return self._metric_descriptors[descriptor_type]
 
         descriptor = MetricDescriptor(
             type=descriptor_type,
             display_name=metric.name,
             description=metric.description or "",
@@ -292,17 +297,27 @@
         # TODO(aabmass): pass timeout to api calls
         timeout_millis: float = 10_000,
         **kwargs,
     ) -> MetricExportResult:
         all_series = []
 
         for resource_metric in metrics_data.resource_metrics:
-            monitored_resource = get_monitored_resource(
+            monitored_resource_data = get_monitored_resource(
                 resource_metric.resource
             )
+            # convert it to proto
+            monitored_resource = (
+                MonitoredResource(
+                    type=monitored_resource_data.type,
+                    labels=monitored_resource_data.labels,
+                )
+                if monitored_resource_data
+                else None
+            )
+
             for scope_metric in resource_metric.scope_metrics:
                 for metric in scope_metric.metrics:
                     # Convert all data_points to Sequences, see
                     # https://github.com/open-telemetry/opentelemetry-python/issues/3021.
                     # TODO(aabmass): remove once the issue is fixed upstream
                     metric = replace(
                         metric,
```

### Comparing `opentelemetry-exporter-gcp-monitoring-1.4.0a0/src/opentelemetry/exporter/cloud_monitoring/version.py` & `opentelemetry-exporter-gcp-monitoring-1.5.0a0/src/opentelemetry/exporter/cloud_monitoring/version.py`

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

### Comparing `opentelemetry-exporter-gcp-monitoring-1.4.0a0/src/opentelemetry_exporter_gcp_monitoring.egg-info/PKG-INFO` & `opentelemetry-exporter-gcp-monitoring-1.5.0a0/src/opentelemetry_exporter_gcp_monitoring.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-exporter-gcp-monitoring
-Version: 1.4.0a0
+Version: 1.5.0a0
 Summary: Google Cloud Monitoring exporter for OpenTelemetry
 Home-page: https://github.com/GoogleCloudPlatform/opentelemetry-operations-python/tree/main/opentelemetry-exporter-gcp-monitoring
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
 
 OpenTelemetry Google Cloud Monitoring Exporter
 ==============================================
@@ -54,37 +55,48 @@
 
     import time
 
     from opentelemetry import metrics
     from opentelemetry.exporter.cloud_monitoring import (
         CloudMonitoringMetricsExporter,
     )
-    from opentelemetry.sdk.metrics import Counter, MeterProvider
-
-    metrics.set_meter_provider(MeterProvider())
-    meter = metrics.get_meter(__name__)
-    metrics.get_meter_provider().start_pipeline(
-        meter, CloudMonitoringMetricsExporter(), 5
+    from opentelemetry.sdk.metrics import MeterProvider
+    from opentelemetry.sdk.metrics.export import PeriodicExportingMetricReader
+    from opentelemetry.sdk.resources import Resource
+
+    metrics.set_meter_provider(
+        MeterProvider(
+            metric_readers=[
+                PeriodicExportingMetricReader(
+                    CloudMonitoringMetricsExporter(), export_interval_millis=5000
+                )
+            ],
+            resource=Resource.create(
+                {
+                    "service.name": "basic_metrics",
+                    "service.namespace": "examples",
+                    "service.instance.id": "instance123",
+                }
+            ),
+        )
     )
+    meter = metrics.get_meter(__name__)
 
+    # Creates metric workload.googleapis.com/request_counter with monitored resource generic_task
     requests_counter = meter.create_counter(
         name="request_counter",
         description="number of requests",
         unit="1",
-        value_type=int
     )
 
     staging_labels = {"environment": "staging"}
 
     for i in range(20):
         requests_counter.add(25, staging_labels)
-        time.sleep(10)
-
+        time.sleep(5)
 
 
 References
 ----------
 
 * `Cloud Monitoring <https://cloud.google.com/monitoring>`_
 * `OpenTelemetry Project <https://opentelemetry.io/>`_
-
-
```

### Comparing `opentelemetry-exporter-gcp-monitoring-1.4.0a0/src/opentelemetry_exporter_gcp_monitoring.egg-info/SOURCES.txt` & `opentelemetry-exporter-gcp-monitoring-1.5.0a0/src/opentelemetry_exporter_gcp_monitoring.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,27 +2,24 @@
 LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 src/opentelemetry/py.typed
 src/opentelemetry/exporter/cloud_monitoring/__init__.py
-src/opentelemetry/exporter/cloud_monitoring/_resource.py
 src/opentelemetry/exporter/cloud_monitoring/version.py
 src/opentelemetry_exporter_gcp_monitoring.egg-info/PKG-INFO
 src/opentelemetry_exporter_gcp_monitoring.egg-info/SOURCES.txt
 src/opentelemetry_exporter_gcp_monitoring.egg-info/dependency_links.txt
 src/opentelemetry_exporter_gcp_monitoring.egg-info/requires.txt
 src/opentelemetry_exporter_gcp_monitoring.egg-info/top_level.txt
 tests/conftest.py
 tests/test_cloud_monitoring.py
 tests/test_normalize_label_key.py
-tests/test_resource.py
 tests/test_user_agent.py
-tests/__snapshots__/test_resource.ambr
 tests/__snapshots__/test_cloud_monitoring/test_counter[float].json
 tests/__snapshots__/test_cloud_monitoring/test_counter[int].json
 tests/__snapshots__/test_cloud_monitoring/test_histogram_default_buckets.json
 tests/__snapshots__/test_cloud_monitoring/test_histogram_single_bucket.json
 tests/__snapshots__/test_cloud_monitoring/test_invalid_label_keys.json
 tests/__snapshots__/test_cloud_monitoring/test_observable_counter[float].json
 tests/__snapshots__/test_cloud_monitoring/test_observable_counter[int].json
```

### Comparing `opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/__snapshots__/test_cloud_monitoring/test_counter[float].json` & `opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/__snapshots__/test_cloud_monitoring/test_counter[float].json`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/__snapshots__/test_cloud_monitoring/test_counter[int].json` & `opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/__snapshots__/test_cloud_monitoring/test_counter[int].json`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/__snapshots__/test_cloud_monitoring/test_histogram_default_buckets.json` & `opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/__snapshots__/test_cloud_monitoring/test_histogram_default_buckets.json`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/__snapshots__/test_cloud_monitoring/test_histogram_single_bucket.json` & `opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/__snapshots__/test_cloud_monitoring/test_histogram_single_bucket.json`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/__snapshots__/test_cloud_monitoring/test_invalid_label_keys.json` & `opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/__snapshots__/test_cloud_monitoring/test_invalid_label_keys.json`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/__snapshots__/test_cloud_monitoring/test_observable_counter[float].json` & `opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/__snapshots__/test_cloud_monitoring/test_observable_counter[float].json`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/__snapshots__/test_cloud_monitoring/test_observable_counter[int].json` & `opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/__snapshots__/test_cloud_monitoring/test_observable_counter[int].json`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/__snapshots__/test_cloud_monitoring/test_observable_gauge[float].json` & `opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/__snapshots__/test_cloud_monitoring/test_observable_gauge[float].json`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/__snapshots__/test_cloud_monitoring/test_observable_gauge[int].json` & `opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/__snapshots__/test_cloud_monitoring/test_observable_gauge[int].json`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/__snapshots__/test_cloud_monitoring/test_observable_updowncounter[float].json` & `opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/__snapshots__/test_cloud_monitoring/test_observable_updowncounter[float].json`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/__snapshots__/test_cloud_monitoring/test_observable_updowncounter[int].json` & `opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/__snapshots__/test_cloud_monitoring/test_observable_updowncounter[int].json`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/__snapshots__/test_cloud_monitoring/test_up_down_counter[float].json` & `opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/__snapshots__/test_cloud_monitoring/test_up_down_counter[float].json`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/__snapshots__/test_cloud_monitoring/test_up_down_counter[int].json` & `opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/__snapshots__/test_cloud_monitoring/test_up_down_counter[int].json`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/__snapshots__/test_cloud_monitoring/test_with_resource.json` & `opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/__snapshots__/test_cloud_monitoring/test_with_resource.json`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/conftest.py` & `opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/fixtures/gcmfake.py` & `opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/fixtures/gcmfake.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/fixtures/snapshot_gcmcalls.py` & `opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/fixtures/snapshot_gcmcalls.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/test_cloud_monitoring.py` & `opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/test_cloud_monitoring.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,19 @@
     "float": 123.4,
 }
 
 
 def test_create_monitoring_exporter() -> None:
     client = MetricServiceClient(credentials=AnonymousCredentials())
     CloudMonitoringMetricsExporter(project_id=PROJECT_ID, client=client)
+    CloudMonitoringMetricsExporter(
+        project_id=PROJECT_ID,
+        client=client,
+        prefix="custom.googleapis.com",
+    )
 
 
 @pytest.mark.parametrize(
     "value", [pytest.param(123, id="int"), pytest.param(45.6, id="float")]
 )
 def test_counter(
     value: Union[float, int],
```

### Comparing `opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/test_normalize_label_key.py` & `opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/test_normalize_label_key.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-gcp-monitoring-1.4.0a0/tests/test_user_agent.py` & `opentelemetry-exporter-gcp-monitoring-1.5.0a0/tests/test_user_agent.py`

 * *Files identical despite different names*

