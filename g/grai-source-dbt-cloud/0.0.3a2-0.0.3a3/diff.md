# Comparing `tmp/grai_source_dbt_cloud-0.0.3a2.tar.gz` & `tmp/grai_source_dbt_cloud-0.0.3a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_dbt_cloud-0.0.3a2.tar", max compression
+gzip compressed data, was "grai_source_dbt_cloud-0.0.3a3.tar", max compression
```

## Comparing `grai_source_dbt_cloud-0.0.3a2.tar` & `grai_source_dbt_cloud-0.0.3a3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      142 2023-05-03 16:29:40.848719 grai_source_dbt_cloud-0.0.3a2/README.md
--rw-r--r--   0        0        0      933 2023-05-11 13:57:03.250438 grai_source_dbt_cloud-0.0.3a2/pyproject.toml
--rw-r--r--   0        0        0       47 2023-05-03 16:29:40.851280 grai_source_dbt_cloud-0.0.3a2/src/grai_source_dbt_cloud/__init__.py
--rw-r--r--   0        0        0      877 2023-05-10 10:03:30.937728 grai_source_dbt_cloud-0.0.3a2/src/grai_source_dbt_cloud/base.py
--rw-r--r--   0        0        0     1951 2023-05-11 13:55:55.577526 grai_source_dbt_cloud-0.0.3a2/src/grai_source_dbt_cloud/loader.py
--rw-r--r--   0        0        0        0 2023-05-03 16:29:40.852043 grai_source_dbt_cloud-0.0.3a2/src/grai_source_dbt_cloud/py.typed
--rw-r--r--   0        0        0     1066 1970-01-01 00:00:00.000000 grai_source_dbt_cloud-0.0.3a2/PKG-INFO
+-rw-r--r--   0        0        0      142 2023-05-17 10:43:12.453217 grai_source_dbt_cloud-0.0.3a3/README.md
+-rw-r--r--   0        0        0      933 2023-05-18 14:29:08.425794 grai_source_dbt_cloud-0.0.3a3/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-05-17 10:43:12.458689 grai_source_dbt_cloud-0.0.3a3/src/grai_source_dbt_cloud/__init__.py
+-rw-r--r--   0        0        0      929 2023-05-18 13:39:45.657214 grai_source_dbt_cloud-0.0.3a3/src/grai_source_dbt_cloud/base.py
+-rw-r--r--   0        0        0     3729 2023-05-18 14:07:17.461144 grai_source_dbt_cloud-0.0.3a3/src/grai_source_dbt_cloud/loader.py
+-rw-r--r--   0        0        0        0 2023-05-17 10:43:12.459210 grai_source_dbt_cloud-0.0.3a3/src/grai_source_dbt_cloud/py.typed
+-rw-r--r--   0        0        0     1066 1970-01-01 00:00:00.000000 grai_source_dbt_cloud-0.0.3a3/PKG-INFO
```

### Comparing `grai_source_dbt_cloud-0.0.3a2/pyproject.toml` & `grai_source_dbt_cloud-0.0.3a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai_source_dbt_cloud"
-version = "0.0.3-alpha2"
+version = "0.0.3-alpha3"
 description = ""
 authors = ["Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_dbt_cloud", from = "src" },
 ]
 readme = "README.md"
```

### Comparing `grai_source_dbt_cloud-0.0.3a2/PKG-INFO` & `grai_source_dbt_cloud-0.0.3a3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grai-source-dbt-cloud
-Version: 0.0.3a2
+Version: 0.0.3a3
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Edward Louth
 Author-email: edward@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

