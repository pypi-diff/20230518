# Comparing `tmp/datarobot_bosun-9.1.1b1-py3-none-any.whl.zip` & `tmp/datarobot_bosun-9.1.1rc1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,71 +1,74 @@
-Zip file size: 114437 bytes, number of entries: 69
--rw-r--r--  2.0 unx      583 b- defN 23-Mar-27 23:33 bosun/model_connector/__init__.py
--rw-rw-r--  2.0 unx      399 b- defN 23-Mar-27 23:33 bosun/model_connector/config_external.json
--rw-r--r--  2.0 unx     1507 b- defN 23-Mar-27 23:33 bosun/model_connector/constants.py
--rw-r--r--  2.0 unx     1395 b- defN 23-Mar-27 23:33 bosun/model_connector/file_uri_fetcher.py
--rw-r--r--  2.0 unx     7190 b- defN 23-Mar-27 23:33 bosun/model_connector/mc_bosun.py
--rw-r--r--  2.0 unx     5269 b- defN 23-Mar-27 23:33 bosun/model_connector/mc_runner.py
--rw-r--r--  2.0 unx     5433 b- defN 23-Mar-27 23:33 bosun/model_connector/model_connector_base.py
--rw-r--r--  2.0 unx     2334 b- defN 23-Mar-27 23:33 bosun/model_connector/s3_uri_fetcher.py
--rw-r--r--  2.0 unx      894 b- defN 23-Mar-27 23:33 bosun/model_connector/uri_fetcher_base.py
--rw-r--r--  2.0 unx      583 b- defN 23-Mar-27 23:33 bosun/plugin/__init__.py
--rw-r--r--  2.0 unx     2225 b- defN 23-Mar-27 23:33 bosun/plugin/action_status.py
--rw-r--r--  2.0 unx     5957 b- defN 23-Mar-27 23:33 bosun/plugin/bosun_plugin_base.py
--rw-r--r--  2.0 unx    11466 b- defN 23-Mar-27 23:33 bosun/plugin/bosun_test_plugin.py
--rw-r--r--  2.0 unx     2735 b- defN 23-Mar-27 23:33 bosun/plugin/constants.py
--rw-r--r--  2.0 unx     3354 b- defN 23-Mar-27 23:33 bosun/plugin/deployment_info.py
--rw-r--r--  2.0 unx     1047 b- defN 23-Mar-27 23:33 bosun/plugin/exceptions.py
--rw-r--r--  2.0 unx     2493 b- defN 23-Mar-27 23:33 bosun/plugin/pe_info.py
--rw-r--r--  2.0 unx    16631 b- defN 23-Mar-27 23:33 bosun/plugin/plugin_runner.py
--rw-r--r--  2.0 unx      640 b- defN 23-Mar-27 23:33 bosun/plugin/azureml/__init__.py
--rw-r--r--  2.0 unx     8275 b- defN 23-Mar-27 23:33 bosun/plugin/azureml/azureml_plugin.py
--rw-r--r--  2.0 unx     3058 b- defN 23-Mar-27 23:33 bosun/plugin/azureml/azureml_status_reporter.py
--rw-r--r--  2.0 unx     1504 b- defN 23-Mar-27 23:33 bosun/plugin/azureml/template_renderer.py
--rw-r--r--  2.0 unx    10060 b- defN 23-Mar-27 23:33 bosun/plugin/azureml/client/base_endpoint_client.py
--rw-r--r--  2.0 unx     5885 b- defN 23-Mar-27 23:33 bosun/plugin/azureml/client/batch_endpoint_client.py
--rw-r--r--  2.0 unx    12088 b- defN 23-Mar-27 23:33 bosun/plugin/azureml/client/online_endpoint_client.py
--rw-r--r--  2.0 unx     1680 b- defN 23-Mar-27 23:33 bosun/plugin/azureml/client/scoring_snippets.py
--rw-r--r--  2.0 unx      583 b- defN 23-Mar-27 23:33 bosun/plugin/azureml/config/__init__.py
--rw-r--r--  2.0 unx     8036 b- defN 23-Mar-27 23:33 bosun/plugin/azureml/config/azureml_client_config.py
--rw-r--r--  2.0 unx     3059 b- defN 23-Mar-27 23:33 bosun/plugin/azureml/config/config_keys.py
--rw-r--r--  2.0 unx     3368 b- defN 23-Mar-27 23:33 bosun/plugin/azureml/templates/azureml_batch_endpoint_score.py
--rw-r--r--  2.0 unx     4814 b- defN 23-Mar-27 23:33 bosun/plugin/azureml/templates/azureml_online_endpoint_score.py
--rw-r--r--  2.0 unx      702 b- defN 23-Mar-27 23:33 bosun/plugin/config_samples/__init__.py
--rw-r--r--  2.0 unx      757 b- defN 23-Mar-27 23:33 bosun/plugin/docker/__init__.py
--rw-r--r--  2.0 unx    14934 b- defN 23-Mar-27 23:33 bosun/plugin/docker/docker_helper.py
--rw-r--r--  2.0 unx    23290 b- defN 23-Mar-27 23:33 bosun/plugin/docker/docker_plugin.py
--rw-r--r--  2.0 unx     5419 b- defN 23-Mar-27 23:33 bosun/plugin/docker/docker_plugin_config.py
--rw-r--r--  2.0 unx     7897 b- defN 23-Mar-27 23:33 bosun/plugin/docker/mlops_monitoring.py
--rw-r--r--  2.0 unx      646 b- defN 23-Mar-27 23:33 bosun/plugin/filesystem/__init__.py
--rw-r--r--  2.0 unx    14021 b- defN 23-Mar-27 23:33 bosun/plugin/filesystem/filesystem_plugin.py
--rw-r--r--  2.0 unx      646 b- defN 23-Mar-27 23:33 bosun/plugin/k8s/__init__.py
--rw-r--r--  2.0 unx    37071 b- defN 23-Mar-27 23:33 bosun/plugin/k8s/client.py
--rw-r--r--  2.0 unx    19918 b- defN 23-Mar-27 23:33 bosun/plugin/k8s/config.py
--rw-r--r--  2.0 unx    28164 b- defN 23-Mar-27 23:33 bosun/plugin/k8s/kubernetes_plugin.py
--rw-r--r--  2.0 unx     9170 b- defN 23-Mar-27 23:33 bosun/plugin/k8s/manifests.py
--rw-rw-r--  2.0 unx      303 b- defN 23-Mar-27 23:33 bosun/plugin/k8s/templates/Dockerfile.pps-model.j2
--rw-rw-r--  2.0 unx     2263 b- defN 23-Mar-27 23:33 bosun/plugin/k8s/templates/_helpers.j2
--rw-rw-r--  2.0 unx     4603 b- defN 23-Mar-27 23:33 bosun/plugin/k8s/templates/cm_pps_installer.sh.j2
--rw-rw-r--  2.0 unx     1393 b- defN 23-Mar-27 23:33 bosun/plugin/k8s/templates/image-builder.yaml.j2
--rw-rw-r--  2.0 unx      356 b- defN 23-Mar-27 23:33 bosun/plugin/k8s/templates/mlops-api-secret.yaml.j2
--rw-rw-r--  2.0 unx     1106 b- defN 23-Mar-27 23:33 bosun/plugin/k8s/templates/model-resources.yaml.j2
--rw-rw-r--  2.0 unx     4929 b- defN 23-Mar-27 23:33 bosun/plugin/k8s/templates/model-resources/deployment.yaml.j2
--rw-rw-r--  2.0 unx      119 b- defN 23-Mar-27 23:33 bosun/plugin/k8s/templates/model-resources/extra.yaml.j2
--rw-rw-r--  2.0 unx      842 b- defN 23-Mar-27 23:33 bosun/plugin/k8s/templates/model-resources/hpa.yaml.j2
--rw-rw-r--  2.0 unx     1253 b- defN 23-Mar-27 23:33 bosun/plugin/k8s/templates/model-resources/ingress.yaml.j2
--rw-rw-r--  2.0 unx      484 b- defN 23-Mar-27 23:33 bosun/plugin/k8s/templates/model-resources/pdb.yaml.j2
--rw-rw-r--  2.0 unx      547 b- defN 23-Mar-27 23:33 bosun/plugin/k8s/templates/model-resources/service.yaml.j2
--rw-r--r--  2.0 unx      630 b- defN 23-Mar-27 23:33 bosun/plugin/s3/__init__.py
--rw-r--r--  2.0 unx    11175 b- defN 23-Mar-27 23:33 bosun/plugin/s3/s3_plugin.py
--rw-r--r--  2.0 unx     2705 b- defN 23-Mar-27 23:33 bosun/plugin/s3/s3_plugin_config.py
--rw-r--r--  2.0 unx      644 b- defN 23-Mar-27 23:33 bosun/plugin/snowflake/__init__.py
--rw-r--r--  2.0 unx    10034 b- defN 23-Mar-27 23:33 bosun/plugin/snowflake/snowflake_plugin.py
--rw-r--r--  2.0 unx     5491 b- defN 23-Mar-27 23:33 bosun/plugin/snowflake/snowflake_plugin_config.py
--rwxr-xr-x  2.0 unx      671 b- defN 23-Mar-27 23:41 datarobot_bosun-9.1.1b1.data/scripts/bosun-plugin-runner
--rwxr-xr-x  2.0 unx      676 b- defN 23-Mar-27 23:41 datarobot_bosun-9.1.1b1.data/scripts/mcrunner
--rwxr-xr-x  2.0 unx      671 b- defN 23-Mar-27 23:41 datarobot_bosun-9.1.1b1.data/scripts/plugin-runner
--rw-r--r--  2.0 unx     4470 b- defN 23-Mar-27 23:41 datarobot_bosun-9.1.1b1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-27 23:41 datarobot_bosun-9.1.1b1.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Mar-27 23:41 datarobot_bosun-9.1.1b1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     6689 b- defN 23-Mar-27 23:41 datarobot_bosun-9.1.1b1.dist-info/RECORD
-69 files, 359332 bytes uncompressed, 103523 bytes compressed:  71.2%
+Zip file size: 125605 bytes, number of entries: 72
+-rw-r--r--  2.0 unx      583 b- defN 23-May-18 21:10 bosun/model_connector/__init__.py
+-rw-rw-r--  2.0 unx      399 b- defN 23-May-18 21:10 bosun/model_connector/config_external.json
+-rw-r--r--  2.0 unx     1507 b- defN 23-May-18 21:10 bosun/model_connector/constants.py
+-rw-r--r--  2.0 unx     1395 b- defN 23-May-18 21:10 bosun/model_connector/file_uri_fetcher.py
+-rw-r--r--  2.0 unx     7190 b- defN 23-May-18 21:10 bosun/model_connector/mc_bosun.py
+-rw-r--r--  2.0 unx     5269 b- defN 23-May-18 21:10 bosun/model_connector/mc_runner.py
+-rw-r--r--  2.0 unx     5433 b- defN 23-May-18 21:10 bosun/model_connector/model_connector_base.py
+-rw-r--r--  2.0 unx     2334 b- defN 23-May-18 21:10 bosun/model_connector/s3_uri_fetcher.py
+-rw-r--r--  2.0 unx      894 b- defN 23-May-18 21:10 bosun/model_connector/uri_fetcher_base.py
+-rw-r--r--  2.0 unx      583 b- defN 23-May-18 21:10 bosun/plugin/__init__.py
+-rw-r--r--  2.0 unx     2260 b- defN 23-May-18 21:10 bosun/plugin/action_status.py
+-rw-r--r--  2.0 unx     6147 b- defN 23-May-18 21:10 bosun/plugin/bosun_plugin_base.py
+-rw-r--r--  2.0 unx    11466 b- defN 23-May-18 21:10 bosun/plugin/bosun_test_plugin.py
+-rw-r--r--  2.0 unx     2833 b- defN 23-May-18 21:10 bosun/plugin/constants.py
+-rw-r--r--  2.0 unx     3354 b- defN 23-May-18 21:10 bosun/plugin/deployment_info.py
+-rw-r--r--  2.0 unx     1047 b- defN 23-May-18 21:10 bosun/plugin/exceptions.py
+-rw-r--r--  2.0 unx     2493 b- defN 23-May-18 21:10 bosun/plugin/pe_info.py
+-rw-r--r--  2.0 unx    16799 b- defN 23-May-18 21:10 bosun/plugin/plugin_runner.py
+-rw-r--r--  2.0 unx      640 b- defN 23-May-18 21:10 bosun/plugin/azureml/__init__.py
+-rw-r--r--  2.0 unx    12218 b- defN 23-May-18 21:10 bosun/plugin/azureml/azureml_plugin.py
+-rw-r--r--  2.0 unx     3313 b- defN 23-May-18 21:10 bosun/plugin/azureml/azureml_status_reporter.py
+-rw-r--r--  2.0 unx     1516 b- defN 23-May-18 21:10 bosun/plugin/azureml/template_renderer.py
+-rw-r--r--  2.0 unx    18410 b- defN 23-May-18 21:10 bosun/plugin/azureml/client/base_endpoint_client.py
+-rw-r--r--  2.0 unx     6743 b- defN 23-May-18 21:10 bosun/plugin/azureml/client/batch_endpoint_client.py
+-rw-r--r--  2.0 unx    17972 b- defN 23-May-18 21:10 bosun/plugin/azureml/client/online_endpoint_client.py
+-rw-r--r--  2.0 unx     1394 b- defN 23-May-18 21:10 bosun/plugin/azureml/client/scoring_snippets.py
+-rw-r--r--  2.0 unx      583 b- defN 23-May-18 21:10 bosun/plugin/azureml/config/__init__.py
+-rw-r--r--  2.0 unx    11520 b- defN 23-May-18 21:10 bosun/plugin/azureml/config/azureml_client_config.py
+-rw-r--r--  2.0 unx     3420 b- defN 23-May-18 21:10 bosun/plugin/azureml/config/config_keys.py
+-rw-r--r--  2.0 unx     3767 b- defN 23-May-18 21:10 bosun/plugin/azureml/templates/batch_score.py
+-rw-r--r--  2.0 unx     9634 b- defN 23-May-18 21:10 bosun/plugin/azureml/templates/common.py
+-rw-rw-r--  2.0 unx      697 b- defN 23-May-18 21:10 bosun/plugin/azureml/templates/conda.yml
+-rw-r--r--  2.0 unx     5452 b- defN 23-May-18 21:10 bosun/plugin/azureml/templates/online_score.py
+-rw-rw-r--  2.0 unx      963 b- defN 23-May-18 21:10 bosun/plugin/azureml/templates/scoring_script_builder.py.j2
+-rw-r--r--  2.0 unx      702 b- defN 23-May-18 21:10 bosun/plugin/config_samples/__init__.py
+-rw-r--r--  2.0 unx      757 b- defN 23-May-18 21:10 bosun/plugin/docker/__init__.py
+-rw-r--r--  2.0 unx    14934 b- defN 23-May-18 21:10 bosun/plugin/docker/docker_helper.py
+-rw-r--r--  2.0 unx    23290 b- defN 23-May-18 21:10 bosun/plugin/docker/docker_plugin.py
+-rw-r--r--  2.0 unx     5419 b- defN 23-May-18 21:10 bosun/plugin/docker/docker_plugin_config.py
+-rw-r--r--  2.0 unx     7897 b- defN 23-May-18 21:10 bosun/plugin/docker/mlops_monitoring.py
+-rw-r--r--  2.0 unx      646 b- defN 23-May-18 21:10 bosun/plugin/filesystem/__init__.py
+-rw-r--r--  2.0 unx    14021 b- defN 23-May-18 21:10 bosun/plugin/filesystem/filesystem_plugin.py
+-rw-r--r--  2.0 unx      646 b- defN 23-May-18 21:10 bosun/plugin/k8s/__init__.py
+-rw-r--r--  2.0 unx    37071 b- defN 23-May-18 21:10 bosun/plugin/k8s/client.py
+-rw-r--r--  2.0 unx    20247 b- defN 23-May-18 21:10 bosun/plugin/k8s/config.py
+-rw-r--r--  2.0 unx    28225 b- defN 23-May-18 21:10 bosun/plugin/k8s/kubernetes_plugin.py
+-rw-r--r--  2.0 unx     9170 b- defN 23-May-18 21:10 bosun/plugin/k8s/manifests.py
+-rw-rw-r--  2.0 unx      303 b- defN 23-May-18 21:10 bosun/plugin/k8s/templates/Dockerfile.pps-model.j2
+-rw-rw-r--  2.0 unx     2263 b- defN 23-May-18 21:10 bosun/plugin/k8s/templates/_helpers.j2
+-rw-rw-r--  2.0 unx     4603 b- defN 23-May-18 21:10 bosun/plugin/k8s/templates/cm_pps_installer.sh.j2
+-rw-rw-r--  2.0 unx     1393 b- defN 23-May-18 21:10 bosun/plugin/k8s/templates/image-builder.yaml.j2
+-rw-rw-r--  2.0 unx      356 b- defN 23-May-18 21:10 bosun/plugin/k8s/templates/mlops-api-secret.yaml.j2
+-rw-rw-r--  2.0 unx     1106 b- defN 23-May-18 21:10 bosun/plugin/k8s/templates/model-resources.yaml.j2
+-rw-rw-r--  2.0 unx     4929 b- defN 23-May-18 21:10 bosun/plugin/k8s/templates/model-resources/deployment.yaml.j2
+-rw-rw-r--  2.0 unx      119 b- defN 23-May-18 21:10 bosun/plugin/k8s/templates/model-resources/extra.yaml.j2
+-rw-rw-r--  2.0 unx      842 b- defN 23-May-18 21:10 bosun/plugin/k8s/templates/model-resources/hpa.yaml.j2
+-rw-rw-r--  2.0 unx     1253 b- defN 23-May-18 21:10 bosun/plugin/k8s/templates/model-resources/ingress.yaml.j2
+-rw-rw-r--  2.0 unx      484 b- defN 23-May-18 21:10 bosun/plugin/k8s/templates/model-resources/pdb.yaml.j2
+-rw-rw-r--  2.0 unx      547 b- defN 23-May-18 21:10 bosun/plugin/k8s/templates/model-resources/service.yaml.j2
+-rw-r--r--  2.0 unx      630 b- defN 23-May-18 21:10 bosun/plugin/s3/__init__.py
+-rw-r--r--  2.0 unx    11175 b- defN 23-May-18 21:10 bosun/plugin/s3/s3_plugin.py
+-rw-r--r--  2.0 unx     2705 b- defN 23-May-18 21:10 bosun/plugin/s3/s3_plugin_config.py
+-rw-r--r--  2.0 unx      644 b- defN 23-May-18 21:10 bosun/plugin/snowflake/__init__.py
+-rw-r--r--  2.0 unx    10034 b- defN 23-May-18 21:10 bosun/plugin/snowflake/snowflake_plugin.py
+-rw-r--r--  2.0 unx     5491 b- defN 23-May-18 21:10 bosun/plugin/snowflake/snowflake_plugin_config.py
+-rwxr-xr-x  2.0 unx      671 b- defN 23-May-18 21:18 datarobot_bosun-9.1.1rc1.data/scripts/bosun-plugin-runner
+-rwxr-xr-x  2.0 unx      676 b- defN 23-May-18 21:18 datarobot_bosun-9.1.1rc1.data/scripts/mcrunner
+-rwxr-xr-x  2.0 unx      671 b- defN 23-May-18 21:18 datarobot_bosun-9.1.1rc1.data/scripts/plugin-runner
+-rw-r--r--  2.0 unx     4471 b- defN 23-May-18 21:18 datarobot_bosun-9.1.1rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-18 21:18 datarobot_bosun-9.1.1rc1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-May-18 21:18 datarobot_bosun-9.1.1rc1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     6972 b- defN 23-May-18 21:18 datarobot_bosun-9.1.1rc1.dist-info/RECORD
+72 files, 395689 bytes uncompressed, 114239 bytes compressed:  71.1%
```

## zipnote {}

```diff
@@ -81,18 +81,27 @@
 
 Filename: bosun/plugin/azureml/config/azureml_client_config.py
 Comment: 
 
 Filename: bosun/plugin/azureml/config/config_keys.py
 Comment: 
 
-Filename: bosun/plugin/azureml/templates/azureml_batch_endpoint_score.py
+Filename: bosun/plugin/azureml/templates/batch_score.py
 Comment: 
 
-Filename: bosun/plugin/azureml/templates/azureml_online_endpoint_score.py
+Filename: bosun/plugin/azureml/templates/common.py
+Comment: 
+
+Filename: bosun/plugin/azureml/templates/conda.yml
+Comment: 
+
+Filename: bosun/plugin/azureml/templates/online_score.py
+Comment: 
+
+Filename: bosun/plugin/azureml/templates/scoring_script_builder.py.j2
 Comment: 
 
 Filename: bosun/plugin/config_samples/__init__.py
 Comment: 
 
 Filename: bosun/plugin/docker/__init__.py
 Comment: 
@@ -180,29 +189,29 @@
 
 Filename: bosun/plugin/snowflake/snowflake_plugin.py
 Comment: 
 
 Filename: bosun/plugin/snowflake/snowflake_plugin_config.py
 Comment: 
 
-Filename: datarobot_bosun-9.1.1b1.data/scripts/bosun-plugin-runner
+Filename: datarobot_bosun-9.1.1rc1.data/scripts/bosun-plugin-runner
 Comment: 
 
-Filename: datarobot_bosun-9.1.1b1.data/scripts/mcrunner
+Filename: datarobot_bosun-9.1.1rc1.data/scripts/mcrunner
 Comment: 
 
-Filename: datarobot_bosun-9.1.1b1.data/scripts/plugin-runner
+Filename: datarobot_bosun-9.1.1rc1.data/scripts/plugin-runner
 Comment: 
 
-Filename: datarobot_bosun-9.1.1b1.dist-info/METADATA
+Filename: datarobot_bosun-9.1.1rc1.dist-info/METADATA
 Comment: 
 
-Filename: datarobot_bosun-9.1.1b1.dist-info/WHEEL
+Filename: datarobot_bosun-9.1.1rc1.dist-info/WHEEL
 Comment: 
 
-Filename: datarobot_bosun-9.1.1b1.dist-info/top_level.txt
+Filename: datarobot_bosun-9.1.1rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: datarobot_bosun-9.1.1b1.dist-info/RECORD
+Filename: datarobot_bosun-9.1.1rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bosun/plugin/action_status.py

```diff
@@ -19,14 +19,15 @@
 class ActionDataFields:
     """
     Name of additional fields that the plugin can create inside the data section of the
     ActionStatus Info YAML Bosun will read.
     """
 
     PREDICTION_URL = "predictionUrl"
+    DASHBOARD_URL = "dashboardUrl"
     OLD_MODEL_IN_USE = "oldModelInUse"
     DEPLOYMENTS_STATUS = "deploymentsStatus"
     CURRENT_MODEL_ID = "currentModelId"
 
 
 class ActionStatus:
     OK = "passing"
```

## bosun/plugin/bosun_plugin_base.py

```diff
@@ -40,14 +40,15 @@
         :param pe_info: The PE info dict
         """
         self._plugin_config = plugin_config
         self._private_config_file = private_config_file
         self._pe_info = PEInfo(pe_info) if pe_info else None
         self._logger = logging.getLogger(f"{self.__class__.__module__}.{self.__class__.__name__}")
         self._dry_run = dry_run
+        self._deployment_info = None
 
     @abstractmethod
     def plugin_start(self) -> ActionStatusInfo:
         pass
 
     @abstractmethod
     def plugin_stop(self) -> ActionStatusInfo:
@@ -141,7 +142,10 @@
     @staticmethod
     def get_sanitized_config(parsed_config):
         sanitized = parsed_config.copy()
         if BosunPluginConfigConstants.MLOPS_API_TOKEN_KEY in sanitized:
             masked = sanitized[BosunPluginConfigConstants.MLOPS_API_TOKEN_KEY][:12] + "*******"
             sanitized[BosunPluginConfigConstants.MLOPS_API_TOKEN_KEY] = masked
         return sanitized
+
+    def _set_deployment_info(self, deployment_info: dict):
+        self._deployment_info = DeploymentInfo(deployment_info) if deployment_info else None
```

## bosun/plugin/constants.py

```diff
@@ -75,7 +75,10 @@
 
 
 class DeploymentState:
     READY = "ready"
     STOPPED = "stopped"
     ERROR = "errored"
     LAUNCHING = "launching"
+    REPLACING_MODEL = "replacingModel"
+    SHUTTING_DOWN = "shuttingDown"
+    UNKNOWN = "unknown"
```

## bosun/plugin/plugin_runner.py

```diff
@@ -258,15 +258,17 @@
             self._logger.error(f"Failed to load module: {orig_module_name}")
 
             self._logger.error(
                 f"And no directory structure was detected in module name {orig_module_name}"
             )
             sys.exit(1)
 
-    def load_plugin_object(self, module_name, plugin_config, private_config_file, pe_info):
+    def load_plugin_object(
+        self, module_name, plugin_config, private_config_file, pe_info, deployment_info
+    ):
         try:
             plugin_module = importlib.import_module(module_name)
             self._logger.debug("Plugin was loaded using import statement")
         except ImportError:
             if not os.path.exists(module_name):
                 raise
             plugin_module, module_name = self._load_plugin_from_file(module_name)
@@ -283,15 +285,19 @@
             raise Exception(f"No plugin implementation was detected in module: {module_name}")
 
         if len(possible_plugins) > 1:
             raise Exception(
                 f"Too many implementations of bosun plugin detected: {possible_plugins}"
             )
 
-        return possible_plugins[0](plugin_config, private_config_file, pe_info, self._dry_run)
+        plugin_object = possible_plugins[0](
+            plugin_config, private_config_file, pe_info, self._dry_run
+        )
+        plugin_object._set_deployment_info(deployment_info)
+        return plugin_object
 
     def run(self) -> ActionStatusInfo:
 
         logger = logging.getLogger("main")
 
         require_deployment_info = (
             True if self._action in BosunPluginActions.require_deployment_info() else False
@@ -299,15 +305,15 @@
         plugin_config, pe_info, deployment_info = self.get_configs(
             self._config_file, logger, require_deployment_info
         )
         try:
             plugin_info = self._get_builtin_plugin_by_name(self._plugin)
             plugin_module = plugin_info["module"] if plugin_info else self._plugin
             pbe = self.load_plugin_object(
-                plugin_module, plugin_config, self._private_config_file, pe_info
+                plugin_module, plugin_config, self._private_config_file, pe_info, deployment_info
             )
         except Exception as e:
             msg = "Exception occurred while loading plugin object for action {}: error {}".format(
                 self._action, e
             )
             logger.exception(msg)
             action_status = ActionStatusInfo(ActionStatus.ERROR, msg=msg, state="errored")
```

## bosun/plugin/azureml/azureml_plugin.py

```diff
@@ -6,51 +6,56 @@
 #  This is proprietary source code of DataRobot, Inc. and its affiliates.
 #
 #  This file and its contents are subject to DataRobot Tool and Utility Agreement.
 #  For details, see
 #  https://www.datarobot.com/wp-content/uploads/2021/07/DataRobot-Tool-and-Utility-Agreement.pdf.
 #  ---------------------------------------------------------------------------------
 import logging
-from typing import Optional
 from typing import Union
 
+from azure.ai.ml.exceptions import LocalEndpointNotFoundError
+from azure.core.exceptions import ResourceNotFoundError
+
 from bosun.plugin.action_status import ActionDataFields
 from bosun.plugin.action_status import ActionStatus
 from bosun.plugin.action_status import ActionStatusInfo
 from bosun.plugin.azureml.azureml_status_reporter import MLOpsStatusReporter
 from bosun.plugin.azureml.client.base_endpoint_client import ListOnlyEndpointClient
 from bosun.plugin.azureml.client.batch_endpoint_client import BatchEndpointClient
 from bosun.plugin.azureml.client.online_endpoint_client import OnlineEndpointClient
+from bosun.plugin.azureml.config.azureml_client_config import AZURE_CUSTOM_ENVIRONMENT
 from bosun.plugin.azureml.config.azureml_client_config import EndpointConfig
 from bosun.plugin.azureml.config.config_keys import EndpointType
+from bosun.plugin.azureml.config.config_keys import Key
 from bosun.plugin.bosun_plugin_base import BosunPluginBase
 from bosun.plugin.constants import DeploymentState
 from bosun.plugin.deployment_info import DeploymentInfo
 
 
 class AzureMLPlugin(BosunPluginBase):
     AZURE_CLIENTS = {
-        EndpointType.ONLINE_ENDPOINT: OnlineEndpointClient,
-        EndpointType.BATCH_ENDPOINT: BatchEndpointClient,
-        EndpointType.DEFAULT: ListOnlyEndpointClient,
+        EndpointType.ONLINE: OnlineEndpointClient,
+        EndpointType.BATCH: BatchEndpointClient,
+        EndpointType.UNKNOWN: ListOnlyEndpointClient,
     }
 
     def __init__(self, plugin_config, private_config_file, pe_info, dry_run):
         super().__init__(plugin_config, private_config_file, pe_info, dry_run)
         http_logger = logging.getLogger("azure.core.pipeline.policies.http_logging_policy")
         http_logger.setLevel(logging.WARNING)
 
     def get_azure_client(
-        self, deployment_info: Optional[DeploymentInfo] = None
+        self,
     ) -> Union[OnlineEndpointClient, BatchEndpointClient, ListOnlyEndpointClient]:
         assert self._pe_info is not None
         config = EndpointConfig.read_config(
+            parent_config=self._plugin_config,
             config_file_path=self._private_config_file,
             prediction_environment=self._pe_info,
-            deployment=deployment_info,
+            deployment=self._deployment_info,
         )
         config.validate_config()
         endpoint_type = config.deduce_endpoint_type_by_config()
         self._logger.info("Configuring AzureML client %s...", endpoint_type.name)
         azure_client_cls = self.AZURE_CLIENTS[endpoint_type]
         return azure_client_cls(config)
 
@@ -69,77 +74,159 @@
         deployments_map = {
             deployment_id: ActionStatusInfo(ActionStatus.OK, state=deployment_state).__dict__
             for deployment_id, deployment_state in datarobot_model_deployments.items()
         }
 
         return ActionStatusInfo(ActionStatus.OK, msg=status_msg, data=deployments_map)
 
-    def deployment_start(self, di: DeploymentInfo):
+    def deployment_start(
+        self,
+        di: DeploymentInfo,
+        is_model_replacement: bool = False,
+        deployment_name: str = None,
+        traffic_settings: dict = None,
+        reporter: MLOpsStatusReporter = None,
+    ):
         self._logger.info("Deployment start action invoked for the deployment %s...", di.id)
         if di.model_artifact is None or not di.model_artifact.exists():
             return ActionStatusInfo(
                 ActionStatus.ERROR,
                 "Model must be pulled from DataRobot deployment, before pushing it to AzureML.",
             )
 
-        try:  # TODO set bosun actionTimeoutWorker timeout to 600-900 seconds
-            azure_client = self.get_azure_client(di)
-            reporter = MLOpsStatusReporter(self._plugin_config, di, azure_client.ENDPOINT_TYPE)
+        try:
+            azure_client = self.get_azure_client()
+            reporter = reporter or MLOpsStatusReporter(
+                self._plugin_config, di, azure_client.ENDPOINT_TYPE
+            )
 
             reporter.report_deployment("Registering the model...")
             model = azure_client.register_model(di.model_artifact)
 
-            reporter.report_deployment("Creating a new online endpoint...")
-            azure_client.create_endpoint()
+            if azure_client.ENDPOINT_TYPE == EndpointType.ONLINE and not is_model_replacement:
+                # Traffic settings should be calculated prior to any modifications done to the
+                # endpoint. Otherwise, traffic settings passed from the UI will be considered as
+                # stale and then ignored.
+                traffic_settings = azure_client.get_traffic_settings_set_by_user()
+
+            endpoint_name = azure_client.config[Key.ENDPOINT_NAME]
+            if not is_model_replacement:
+                reporter.report_deployment(f"Configuring the endpoint '{endpoint_name}'...")
+                azure_client.create_or_update_endpoint()
 
             reporter.report_deployment(
-                "Looking for a custom environment. A new one will be created if does not exist..."
+                f"Searching for custom environment: '{AZURE_CUSTOM_ENVIRONMENT}'..."
             )
             environment = azure_client.get_latest_environment()
 
-            reporter.report_deployment("Creating a new deployment...")
-            azure_client.create_deployment(model, environment)
+            reporter.report_deployment(
+                "Creating a new deployment. This action may take up to 20 minutes. "
+                "For more details check the https://ml.azure.com/endpoints page."
+            )
+
+            azure_client.create_deployment(deployment_name, model, environment)
+
             # Need to fetch the endpoint after creating the deployment because it
             # seems otherwise it won't always have the scoring_uri filled in.
             endpoint = azure_client.get_endpoint()
-            if azure_client.ENDPOINT_TYPE == EndpointType.ONLINE_ENDPOINT:
-                reporter.report_deployment("Updating the deployment traffic...")
-                azure_client.update_deployment_traffic(new_traffic_value=100)
-
+            if azure_client.ENDPOINT_TYPE == EndpointType.ONLINE:
+                if traffic_settings:
+                    reporter.report_deployment("Updating the deployment traffic...")
+                    self._logger.info(
+                        "New traffic configuration: %s for the endpoint: %s",
+                        str(traffic_settings),
+                        endpoint_name,
+                    )
+                    azure_client.update_deployment_traffic(endpoint, traffic_settings)
         except Exception as e:
             self._logger.exception("Failed to start the deployment %s", di.id)
             return ActionStatusInfo(ActionStatus.ERROR, msg=str(e))
 
         self._logger.info("Scoring code model is successfully deployed to AzureML.")
         status = self.deployment_status(di)
-        status.data = {ActionDataFields.PREDICTION_URL: endpoint.scoring_uri}
+        status.data = {
+            ActionDataFields.PREDICTION_URL: endpoint.scoring_uri,
+            ActionDataFields.DASHBOARD_URL: azure_client.make_console_url(endpoint),
+        }
         return status
 
-    def deployment_relaunch(self, deployment_info: DeploymentInfo):
-        # TODO do not re-register model. do not update traffic to 100 if it's already set
-        return self.deployment_start(deployment_info)
-
     def deployment_stop(self, deployment_id: str):
-        # TODO 1. check status of each operation
-        # TODO 2. send event to DataRobot after each operation
-        # TODO 3. if the endpoint is shared then we can't delete it but must delete the deployment
         try:
             azure_client = self.get_azure_client()
-            # azure_client.delete_deployment()
-            azure_client.delete_endpoint()
-            azure_client.delete_model()
+            deployments = azure_client.list_deployments_by_endpoint()
+            deployments_in_endpoint = len(deployments)
+            if deployments_in_endpoint == 1:
+                # delete endpoint only if it has one deployment at maximum
+                azure_client.delete_endpoint()
+            else:
+                azure_client.delete_deployment()
+        except (ResourceNotFoundError, LocalEndpointNotFoundError):
+            # nothing to do
+            self._logger.warning(
+                "Deployment does not exist: %s. Skipping deployment stop.", deployment_id
+            )
         except Exception as e:
+            # Deployment can't be deleted if endpoint has multiple deployments and
+            # the deployment traffic settings are not set to zero.
+            #
+            # Deployment traffic can't be set to zero prior to deletion,
+            # since traffic must be redistributed to make sum of all deployment traffic settings
+            # be equal to either 0 or 100.
             self._logger.exception("Error stopping deployment")
             return ActionStatusInfo(ActionStatus.ERROR, msg=str(e))
 
         return ActionStatusInfo(ActionStatus.OK, state=DeploymentState.STOPPED)
 
     def deployment_replace_model(self, deployment_info: DeploymentInfo):
-        # TODO: we should do a "blue/green" deployment strategy
-        return self.deployment_start(deployment_info)
+        """
+        Do model replacement using a blue-green deployment strategy:
+        - old model continues to serve realtime traffic
+        - a new model is deployed with a new unique deployment name suffix
+        - endpoint traffic is flipped from old deployment to the new one
+        - old deployment is stopped
+        """
+        azure_client = self.get_azure_client()
+        traffic_settings = None
+        old_deployment_name = azure_client.get_deployment_name_by_id(deployment_info.id)
+        new_deployment_name = azure_client.config.new_deployment_name
+
+        if azure_client.ENDPOINT_TYPE == EndpointType.ONLINE:
+            (
+                azure_endpoint_last_modified_at,
+                current_traffic_settings,
+            ) = azure_client.get_endpoint_traffic_settings()
+
+            # switch traffic from the old deployment to the new one
+            traffic_settings = dict(**current_traffic_settings)
+            old_deployment_traffic_value = traffic_settings.get(old_deployment_name)
+            if not old_deployment_traffic_value:
+                self._logger.warning(
+                    "No traffic settings found for the deployment %s",
+                    old_deployment_name,
+                )
+
+            traffic_settings[old_deployment_name] = 0
+            traffic_settings[new_deployment_name] = old_deployment_traffic_value or 0
+
+        reporter = MLOpsStatusReporter(
+            self._plugin_config, deployment_info, azure_client.ENDPOINT_TYPE
+        )
+        deployment_start_status = self.deployment_start(
+            deployment_info,
+            is_model_replacement=True,
+            # model replacement requires a new unique deployment name
+            deployment_name=new_deployment_name,
+            traffic_settings=traffic_settings,
+            reporter=reporter,
+        )
+
+        reporter.report_deployment(f"Removing the old deployment '{old_deployment_name}'...")
+        azure_client.delete_deployment(old_deployment_name)
+
+        return deployment_start_status
 
     def pe_status(self):
         try:
             azure_client = self.get_azure_client()
             azure_client.list_deployments()
             status = ActionStatus.OK
             status_msg = "Azure connection successful"
@@ -147,15 +234,15 @@
             status = ActionStatus.ERROR
             status_msg = "Azure connection failed"
             self._logger.exception(status_msg)
 
         return ActionStatusInfo(status=status, msg=status_msg)
 
     def deployment_status(self, deployment_info: DeploymentInfo):
-        azure_client = self.get_azure_client(deployment_info)
+        azure_client = self.get_azure_client()
         try:
             deployment_status = azure_client.deployment_status()
             if deployment_status is None:
                 return ActionStatusInfo(ActionStatus.UNKNOWN, state=DeploymentState.STOPPED)
 
             self._logger.info(
                 "Deployment '%s' (%s) has status '%s'",
@@ -167,15 +254,18 @@
         except Exception as e:
             self._logger.exception("Error checking deployment status")
             return ActionStatusInfo(ActionStatus.ERROR, msg=str(e))
 
     def plugin_start(self):
         """
         Builds a new Custom environment if one does not exist.
-        Azure Custom Environment is expected to be built right after a DataRobot PE is created.
+        AzureML internally blocks a deployment until a custom environment is successfully created,
+        so we don't need to introduce deployment blocks on our side.
+
+        The deployment timeout must include the time needed for image build (>= 10minutes).
         """
         azure_client = self.get_azure_client()
         azure_client.get_latest_environment()
         return ActionStatusInfo(ActionStatus.OK)
 
     def plugin_stop(self):
         # NOOP
```

## bosun/plugin/azureml/azureml_status_reporter.py

```diff
@@ -6,51 +6,54 @@
 #  This is proprietary source code of DataRobot, Inc. and its affiliates.
 #
 #  This file and its contents are subject to DataRobot Tool and Utility Agreement.
 #  For details, see
 #  https://www.datarobot.com/wp-content/uploads/2021/07/DataRobot-Tool-and-Utility-Agreement.pdf.
 #  ---------------------------------------------------------------------------------
 import logging
-import os
 from datetime import datetime
+from datetime import timezone
 
-import pytz
 import requests
 from requests.exceptions import ConnectionError
 from requests.exceptions import HTTPError
 from urllib3.exceptions import MaxRetryError
 
 from bosun.plugin.azureml.config.config_keys import EndpointType
+from bosun.plugin.constants import BosunPluginConfigConstants
 from bosun.plugin.deployment_info import DeploymentInfo
 
 logger = logging.getLogger(__name__)
 
 
 class MLOpsStatusReporter:
     def __init__(
         self, plugin_config: dict, deployment: DeploymentInfo, endpoint_type: EndpointType
     ):
         self.logger = logging.getLogger(f"{self.__class__.__module__}.{self.__class__.__name__}")
-        self.mlops_service_url = os.environ.get("MLOPS_SERVICE_URL", plugin_config.get("mlopsUrl"))
-        self.mlops_api_token = os.environ.get("MLOPS_API_TOKEN", plugin_config.get("mlopsApiToken"))
+        # TODO: I think these MLOps values are only set if monitoring is enabled but we would
+        # always want them set for this usecase and I don't see why Bosun shouldn't
+        # always pass them along to the plugin.
+        self.mlops_service_url = plugin_config.get(BosunPluginConfigConstants.MLOPS_URL_KEY)
+        self.mlops_api_token = plugin_config.get(BosunPluginConfigConstants.MLOPS_API_TOKEN_KEY)
         self.deployment = deployment
         self.endpoint_type = endpoint_type
         self.auth_header = {"Authorization": f"Bearer {self.mlops_api_token}"}
         self.current_stage = 1
         self.is_logged_at_most_once = False
 
     def report_deployment(self, message: str):
         self.logger.info(message)
         remote_events_url = f"{self.mlops_service_url}/api/v2/remoteEvents/"
         total_stages = self._total_deployment_stages_count()
         event_payload = {
             "eventType": "deploymentInfo",
             "title": f"Deployment stage {self.current_stage} out of {total_stages}",
             "message": message,
-            "timestamp": str(datetime.utcnow().replace(tzinfo=pytz.UTC).isoformat()),
+            "timestamp": datetime.now(timezone.utc).isoformat(),
             "deploymentId": self.deployment.id,
         }
         self.current_stage += 1
 
         try:
             requests.post(url=remote_events_url, json=event_payload, headers=self.auth_header)
         except (ConnectionError, HTTPError, MaxRetryError):
@@ -62,10 +65,10 @@
         # [register model, build env, create endpoint, create deployment, update traffic]
         total_online_endpoint_stages = 5
         # [register model, build env, create endpoint, create deployment]
         total_batch_endpoint_stages = 4
 
         return (
             total_online_endpoint_stages
-            if self.endpoint_type == EndpointType.ONLINE_ENDPOINT
+            if self.endpoint_type == EndpointType.ONLINE
             else total_batch_endpoint_stages
         )
```

## bosun/plugin/azureml/template_renderer.py

```diff
@@ -29,16 +29,17 @@
                 PackageLoader(self.PACKAGE_NAME),
             ]
         )
         self.template_env = jinja2.Environment(
             loader=loader, undefined=jinja2.StrictUndefined, autoescape=True
         )
 
-    def template_name(self) -> str:
+    @property
+    def TEMPLATE_NAME(self) -> str:
         raise NotImplementedError("Subclasses need to override this")
 
     def context(self) -> dict:
         return {}
 
     def render(self) -> str:
-        template = self.template_env.get_template(self.template_name())
+        template = self.template_env.get_template(self.TEMPLATE_NAME)
         return template.render(**self.context())
```

## bosun/plugin/azureml/client/base_endpoint_client.py

```diff
@@ -8,66 +8,102 @@
 #  This file and its contents are subject to DataRobot Tool and Utility Agreement.
 #  For details, see
 #  https://www.datarobot.com/wp-content/uploads/2021/07/DataRobot-Tool-and-Utility-Agreement.pdf.
 #  ---------------------------------------------------------------------------------
 import logging
 from abc import ABC
 from abc import abstractmethod
+from datetime import datetime
+from datetime import timezone
+from functools import cached_property
 from pathlib import Path
 from typing import Dict
+from typing import Optional
 from typing import Union
 
 from azure.ai.ml import MLClient
 from azure.ai.ml.constants import AssetTypes
+from azure.ai.ml.entities import BatchEndpoint
+from azure.ai.ml.entities import Deployment
 from azure.ai.ml.entities import Endpoint
 from azure.ai.ml.entities import Environment
 from azure.ai.ml.entities import Model
+from azure.ai.ml.entities import OnlineDeployment
 from azure.core.exceptions import HttpResponseError
 from azure.identity import DefaultAzureCredential
+from dateutil.parser import parser
 
 from bosun.plugin.azureml.config.azureml_client_config import AZURE_BASE_ENVIRONMENT
 from bosun.plugin.azureml.config.azureml_client_config import AZURE_CUSTOM_ENVIRONMENT
 from bosun.plugin.azureml.config.azureml_client_config import AZURE_TEMPLATE_DIR
 from bosun.plugin.azureml.config.azureml_client_config import EndpointConfig
 from bosun.plugin.azureml.config.azureml_client_config import EndpointType
 from bosun.plugin.azureml.config.config_keys import Constants
 from bosun.plugin.azureml.config.config_keys import Key
 from bosun.plugin.azureml.config.config_keys import ProvisioningState
 from bosun.plugin.constants import DeploymentState
+from bosun.plugin.deployment_info import DeploymentInfo
+from bosun.plugin.pe_info import PEInfo
 
 
 class BaseEndpointClient(ABC):
     _EXTERNAL_TO_INTERNAL_STATE_MAP = {
         ProvisioningState.FAILED.value: DeploymentState.ERROR,
         ProvisioningState.SUCCEEDED.value: DeploymentState.READY,
-        ProvisioningState.DELETING.value: DeploymentState.STOPPED,
+        ProvisioningState.DELETING.value: DeploymentState.SHUTTING_DOWN,
         ProvisioningState.CANCELED.value: DeploymentState.STOPPED,
         ProvisioningState.CREATING.value: DeploymentState.LAUNCHING,
         ProvisioningState.SCALING.value: DeploymentState.LAUNCHING,
         ProvisioningState.UPDATING.value: DeploymentState.LAUNCHING,
     }
-    ENDPOINT_TYPE = EndpointType.DEFAULT
+    ENDPOINT_TYPE = EndpointType.UNKNOWN
 
     def __init__(self, config: EndpointConfig):
         self.logger = logging.getLogger(f"{self.__class__.__module__}.{self.__class__.__name__}")
 
         self.config = config
         self.environment_name = config[Key.AZURE_ENVIRONMENT_NAME]
         self.environment_label = config[Key.AZURE_ENVIRONMENT_LABEL]
         self.prediction_environment_tags = config[Key.AZURE_ENVIRONMENT_TAGS]
-        self.prediction_environment = config.prediction_environment
-        self.deployment = config.deployment
+        self.prediction_environment: Optional[PEInfo] = config.prediction_environment
+        self.endpoint_name: Optional[str] = config[Key.ENDPOINT_NAME]
+        self.deployment: Optional[DeploymentInfo] = config.deployment
         self._client = MLClient(
             DefaultAzureCredential(),
             config[Key.AZURE_SUBSCRIPTION_ID],
             config[Key.AZURE_RESOURCE_GROUP],
             config[Key.AZURE_WORKSPACE],
         )
         self._local: bool = self.config[Key.AZURE_LOCAL_TESTING]
 
+    def _get_local_parameter(self, endpoint_type):
+        return {"local": self._local} if endpoint_type == EndpointType.ONLINE else {}
+
+    @cached_property
+    def deployment_name(self):
+        """
+        Returns either existing deployment name or name specified by user if
+        deployment does not exists.
+
+        Original deployment name specified by user may be modified with an unique prefix,
+        which is possible after user executed the model_replacement action. This happens due to
+        two deployments are created in the same endpoint (blue-green deployment) and AzureML
+        requires a deployment name to be uniq.
+        """
+        existing_deployment_name = None
+        if self.config.deployment:
+            datarobot_deployment_id = self.config.deployment.id
+            existing_deployment_name = self.get_deployment_name_by_id(datarobot_deployment_id)
+
+        return existing_deployment_name or self.config[Key.DEPLOYMENT_NAME]
+
+    @property
+    def local_parameter(self):
+        return self._get_local_parameter(self.ENDPOINT_TYPE)
+
     @property
     def datarobot_environment_id(self):
         return self.prediction_environment.id if self.prediction_environment else None
 
     @property
     def datarobot_deployment_id(self):
         return self.deployment.id if self.deployment else None
@@ -84,14 +120,19 @@
         return "dr-" + self.datarobot_model_id if self.datarobot_model_id else None
 
     @property
     def datarobot_model_description(self):
         # TODO bosun mcrunner should pass model description
         return ""
 
+    def get_deployment_name_by_id(self, datarobot_deployment_id) -> str:
+        endpoint_deployments: Dict[str, Deployment] = self.list_deployments_by_endpoint()
+        deployment = endpoint_deployments.get(datarobot_deployment_id)
+        return deployment.name if deployment else None
+
     def get_latest_environment(self):
         self.logger.info("Looking for environment %s in the registry...", self.environment_name)
 
         try:
             return self._client.environments.get(
                 AZURE_CUSTOM_ENVIRONMENT, label=self.environment_label
             )
@@ -121,15 +162,24 @@
 
     def get_latest_model(self):
         self.logger.info("Looking for model %s in the registry...", self.datarobot_model_id)
         return self._client.models.get(
             self.datarobot_model_name, label=Constants.LATEST_VERSION.value
         )
 
-    def delete_model(self):
+    def make_console_url(self, endpoint: Endpoint) -> Optional[str]:
+        if self._local:
+            return None  # Local endpoints don't have a console web address
+
+        assert endpoint.id is not None
+        workspace_id, etype, endpoint_name = endpoint.id.rsplit("/", 2)
+        base = "realtime" if etype == "onlineEndpoints" else "batch"
+        return f"https://ml.azure.com/endpoints/{base}/{endpoint_name}/detail?wsid={workspace_id}"
+
+    def archive_model(self):
         self.logger.info("Deleting DataRobot model %s...", self.datarobot_model_id)
         models = self._client.models.list(self.datarobot_model_name)
         for model in models:
             self._client.models.archive(model.name, model.version)
 
     @classmethod
     def map_state(cls, provisioning_state):
@@ -137,84 +187,198 @@
 
     def list_deployments(self) -> Dict[str, str]:
         self.logger.info(
             "Retrieving list of deployments for prediction environment %s",
             self.prediction_environment.id,
         )
         prediction_environment_deployments = dict()
-        for endpoint_type in (EndpointType.ONLINE_ENDPOINT, EndpointType.BATCH_ENDPOINT):
-            if endpoint_type == EndpointType.BATCH_ENDPOINT and self._local:
+        for endpoint_type in (EndpointType.ONLINE, EndpointType.BATCH):
+            if endpoint_type == EndpointType.BATCH and self._local:
                 self.logger.info("Skipping listing batch endpoints when in local mode...")
                 continue
             deployments = self._list_deployments_by_type(endpoint_type)
             self.logger.info("Found deployments for %s: %s", endpoint_type, deployments)
             prediction_environment_deployments.update(deployments)
         return prediction_environment_deployments
 
     def _list_deployments_by_type(self, endpoint_type: EndpointType) -> Dict[str, str]:
         result = dict()
         # Only OnlineEndpoint APIs support the local= kwarg
-        is_local = {"local": self._local} if endpoint_type == EndpointType.ONLINE_ENDPOINT else {}
         endpoints_api_client, deployments_api_client = self._get_api_clients(endpoint_type)
-        endpoints = endpoints_api_client.list(**is_local)
+        local_parameter = self._get_local_parameter(endpoint_type)
+
+        endpoints = endpoints_api_client.list(**local_parameter)
         for endpoint in endpoints:
             # Multiple PEs can be mapped to a single AzureML workspace so make sure we are only
             # working on endpoints that _this_ PE actually owns.
             tag_value = endpoint.tags.get(Key.DATAROBOT_ENVIRONMENT_ID.value)
             if tag_value is None or tag_value != self.datarobot_environment_id:
                 continue
 
             datarobot_model_deployments = dict()
-            deployments = deployments_api_client.list(endpoint_name=endpoint.name, **is_local)
+            deployments = deployments_api_client.list(
+                endpoint_name=endpoint.name,
+                **local_parameter,
+            )
             for deployment in deployments:
                 deployment_id = deployment.tags.get(Key.DATAROBOT_DEPLOYMENT_ID.value)
                 if deployment_id is None:
+                    self.logger.warning(
+                        "Found deployment %s (endpoint %s) without the `datarobot_deployment_id` tag. "
+                        "This deployment is not maintained by DataRobot.",
+                        deployment.name,
+                        self.endpoint_name,
+                    )
                     continue  # skip non DR deployments
 
-                # batch endpoints don't have a provisioning state, thus use an endpoint state
-                entity = deployment if EndpointType.ONLINE_ENDPOINT else endpoint
+                # batch deployments don't have a provisioning state, thus use an endpoint state
+                entity: Union[OnlineDeployment, BatchEndpoint] = (
+                    deployment if endpoint_type == EndpointType.ONLINE else endpoint
+                )
                 deployment_state = self.map_state(entity.provisioning_state)
                 datarobot_model_deployments[deployment_id] = deployment_state
             result.update(datarobot_model_deployments)
         return result
 
+    def list_deployments_by_endpoint(self) -> Dict[str, Deployment]:
+        """
+        :return:
+            dictionary of DataRobot deployment ID and deployment
+        """
+
+        datarobot_model_deployments = dict()
+        _, deployments_api_client = self._get_api_clients(self.ENDPOINT_TYPE)
+        deployments = deployments_api_client.list(
+            endpoint_name=self.endpoint_name, **self.local_parameter
+        )
+
+        for deployment in deployments:
+            deployment_id = deployment.tags.get(Key.DATAROBOT_DEPLOYMENT_ID.value)
+            if deployment_id is None:
+                self.logger.warning(
+                    "Found deployment %s (endpoint %s) without the `datarobot_deployment_id` tag. "
+                    "This deployment is not maintained by DataRobot.",
+                    deployment.name,
+                    self.endpoint_name,
+                )
+                continue  # skip non DR deployments
+
+            if self._local and (deployment.endpoint_name != self.endpoint_name):
+                # filter deployments by the endpoint name
+                # fix bug in the _local_deployment_helper.py::list
+                # return only endpoint's deployments, instead of ALL the local deployments
+                continue
+
+            duplicate_deployment = datarobot_model_deployments.get(deployment_id)
+            if duplicate_deployment:
+                self.logger.warning(
+                    "Found two deployments %s and %s (endpoint %s) with the same "
+                    "`datarobot_deployment_id` tag value %s. Assuming it's a model replacement.",
+                    deployment.name,
+                    duplicate_deployment.name,
+                    self.endpoint_name,
+                    deployment_id,
+                )
+                # in a model replacement flow, two deployments may have the same deployment ID
+                # return the latest deployment
+                duplicated_deployments = {
+                    self._created_at(deployment): deployment,
+                    self._created_at(duplicate_deployment): duplicate_deployment,
+                }
+                latest_deployment_created_at = max(duplicated_deployments.keys())
+                latest_deployment = duplicated_deployments.get(latest_deployment_created_at)
+                deployment = latest_deployment
+                self.logger.info("Only the latest deployment '%s' will be listed.", deployment.name)
+
+            datarobot_model_deployments[deployment_id] = deployment
+
+        return datarobot_model_deployments
+
+    def _created_at(self, deployment: Deployment) -> datetime:
+        utc_dt_str = deployment.environment_variables.get(Key.DEPLOYMENT_CREATED_AT.value)
+        return parser().parse(utc_dt_str) if utc_dt_str else None
+
     def _get_api_clients(self, endpoint_type: EndpointType):
         endpoints_api_client = None
         deployments_api_client = None
 
-        if endpoint_type == EndpointType.ONLINE_ENDPOINT:
+        if endpoint_type == EndpointType.ONLINE:
             endpoints_api_client = self._client.online_endpoints
             deployments_api_client = self._client.online_deployments
-        elif endpoint_type == EndpointType.BATCH_ENDPOINT:
+        elif endpoint_type == EndpointType.BATCH:
             endpoints_api_client = self._client.batch_endpoints
             deployments_api_client = self._client.batch_deployments
 
         return endpoints_api_client, deployments_api_client
 
+    def _get_env_vars(self, model_filename) -> Dict[str, str]:
+        """Generate env vars to use in deployments we create"""
+        utc_dt = datetime.now(timezone.utc)
+        utc_dt_str = utc_dt.strftime("%Y-%m-%dT%H:%M:%S.%fZ")
+
+        base_vars = {
+            "DATAROBOT_MODEL_FILENAME": str(model_filename),
+            "MONITORING_ENABLED": str(self.config.is_monitoring_enabled),
+            # TODO ask MS team to expose SystemData in Deployment and Endpoint objects
+            Key.DEPLOYMENT_CREATED_AT.value: utc_dt_str,
+            # Our scoring script doesn't need Flask 1.x compatibility and just adds complexity
+            "AML_FLASK_ONE_COMPATIBILITY": "False",
+        }
+        if self.config.is_monitoring_enabled:
+            bootstrap_server = (
+                f"{self.config[Key.AZURE_EVENTHUBS_NAMESPACE]}.servicebus.windows.net:9093"
+            )
+            base_vars.update(
+                {
+                    "MLOPS_DEPLOYMENT_ID": self.datarobot_deployment_id,
+                    "MLOPS_MODEL_ID": self.datarobot_model_id,
+                    "MLOPS_SPOOLER_TYPE": "KAFKA",
+                    "MLOPS_KAFKA_BOOTSTRAP_SERVERS": bootstrap_server,
+                    "MLOPS_KAFKA_TOPIC_NAME": self.config[Key.AZURE_EVENTHUBS_INSTANCE],
+                    # We are using a managed identity to authenticate with EventHubs, so we need to
+                    # set the client_id of the user defined identity and turn on OAuth:
+                    #   https://github.com/Azure/azure-sdk-for-python/blob/azure-identity_1.12.0/sdk/identity/azure-identity/azure/identity/_credentials/managed_identity.py#L70-L72
+                    "MLOPS_KAFKA_SASL_MECHANISM": "OAUTHBEARER",
+                    "MLOPS_KAFKA_SECURITY_PROTOCOL": "SASL_SSL",
+                    "AZURE_CLIENT_ID": self.config[Key.AZURE_MANAGED_IDENTITY_CLIENT_ID],
+                    # Recommended producer settings; see:
+                    #   https://learn.microsoft.com/en-us/azure/event-hubs/apache-kafka-configurations
+                    "MLOPS_KAFKA_METADATA_MAX_AGE_MS": "180000",
+                    "MLOPS_KAFKA_REQUEST_TIMEOUT_MS": "60000",
+                    "MLOPS_KAFKA_MAX_FLUSH_MS": "60000",
+                }  # type: ignore
+            )
+        return base_vars
+
     def get_scoring_snippet(self, model_filename: str) -> str:
-        pass
+        scoring_template = self.SNIPPET_GENERATOR(model_filename=model_filename)
+        return scoring_template.render()
+
+    @property
+    def SNIPPET_GENERATOR(self):
+        raise NotImplementedError("Child classes should define this")
 
     @abstractmethod
-    def create_endpoint(self):
+    def create_or_update_endpoint(self):
         pass
 
     @abstractmethod
     def get_endpoint(self) -> Endpoint:
         pass
 
     @abstractmethod
-    def create_deployment(self, model, environment: Environment):
+    def create_deployment(self, deployment_name: str, model, environment: Environment):
         pass
 
     @abstractmethod
     def delete_endpoint(self):
         pass
 
     @abstractmethod
-    def delete_deployment(self):
+    def delete_deployment(self, deployment_name: str = None):
         pass
 
     @abstractmethod
     def deployment_status(self) -> Union[None, str]:
         pass
 
     def check_permissions(self):
@@ -223,15 +387,22 @@
 
     def check_quota(self):
         # TODO use quota rest api
         raise NotImplementedError()
 
 
 class ListOnlyEndpointClient(BaseEndpointClient):
-    def create_endpoint(self) -> Endpoint:
+    """
+    When action does not provide a DeploymentInfo, specific endpoint client can't be configured,
+    so this "generic" client will be used.
+
+    Used by pe_status and deployments_list actions to get list of deployments in endpoint.
+    """
+
+    def create_or_update_endpoint(self) -> Endpoint:
         raise NotImplementedError
 
     def get_endpoint(self) -> Endpoint:
         raise NotImplementedError
 
     def create_deployment(self, model):
         raise NotImplementedError
```

## bosun/plugin/azureml/client/batch_endpoint_client.py

```diff
@@ -13,52 +13,48 @@
 from pathlib import Path
 from typing import Union
 
 import azure.ai.ml as azureml
 from azure.ai.ml.entities import BatchDeployment
 from azure.ai.ml.entities import BatchEndpoint
 from azure.ai.ml.entities import BatchRetrySettings
+from azure.ai.ml.entities import CodeConfiguration
 from azure.ai.ml.entities import Environment
 from azure.core.exceptions import ResourceNotFoundError
 
 from bosun.plugin.azureml.client.base_endpoint_client import BaseEndpointClient
 from bosun.plugin.azureml.client.scoring_snippets import AzureMLBatchEndpointScoringSnippet
 from bosun.plugin.azureml.config.azureml_client_config import EndpointConfig
 from bosun.plugin.azureml.config.azureml_client_config import Key
 from bosun.plugin.azureml.config.config_keys import EndpointType
 
 
 class BatchEndpointClient(BaseEndpointClient):
-    ENDPOINT_TYPE = EndpointType.BATCH_ENDPOINT
+    ENDPOINT_TYPE = EndpointType.BATCH
+    SNIPPET_GENERATOR = AzureMLBatchEndpointScoringSnippet
 
     def __init__(self, config: EndpointConfig):
         super().__init__(config)
-        self.endpoint_name = self.config[Key.ENDPOINT_NAME]
-        self.deployment_name = self.config[Key.DEPLOYMENT_NAME]
 
-    def get_scoring_snippet(self, model_filename) -> str:
-        scoring_template = AzureMLBatchEndpointScoringSnippet(model_filename=model_filename)
-        return scoring_template.render()
-
-    def create_endpoint(self):
+    def create_or_update_endpoint(self):
         endpoint_tags = {
             Key.DATAROBOT_DEPLOYMENT_ID.value: self.datarobot_deployment_id,
             Key.DATAROBOT_ENVIRONMENT_ID.value: self.datarobot_environment_id,
         }
         endpoint_tags.update(self.prediction_environment_tags)
         endpoint = azureml.entities.BatchEndpoint(name=self.endpoint_name, tags=endpoint_tags)
         # TODO assert status
         self._client.batch_endpoints.begin_create_or_update(endpoint).result(
             self.config[Key.ENDPOINT_CREATION_TIMEOUT]
         )
 
     def get_endpoint(self) -> BatchEndpoint:
         return self._client.batch_endpoints.get(self.endpoint_name)
 
-    def create_deployment(self, model, environment: Environment):
+    def create_deployment(self, deployment_name: str, model, environment: Environment):
         model_filename = Path(model.path).name
         scoring_script_name = "batch_driver.py"
         deployment_tags = {
             Key.DATAROBOT_ENVIRONMENT_ID.value: self.datarobot_environment_id,
             Key.DATAROBOT_DEPLOYMENT_ID.value: self.datarobot_deployment_id,
             Key.DATAROBOT_MODEL_ID.value: self.datarobot_model_id,
         }
@@ -66,52 +62,70 @@
         with tempfile.TemporaryDirectory() as scoring_code_dir, open(
             Path(scoring_code_dir) / scoring_script_name, "w"
         ) as scoring_code_file:
             scoring_code_file.write(self.get_scoring_snippet(model_filename))
             scoring_code_file.flush()
 
             deployment = BatchDeployment(
-                name=self.deployment_name,
+                name=deployment_name or self.deployment_name,
                 endpoint_name=self.endpoint_name,
                 model=model,
-                code_path=scoring_code_dir,
-                scoring_script=scoring_script_name,
+                code_configuration=CodeConfiguration(
+                    code=str(scoring_code_dir), scoring_script=scoring_script_name
+                ),
                 environment=environment,
                 compute=self.config[Key.COMPUTE_CLUSTER],
                 instance_count=self.config[Key.COMPUTE_CLUSTER_INSTANCE_COUNT],
                 max_concurrency_per_instance=self.config[Key.MAX_CONCURRENCY_PER_INSTANCE],
                 mini_batch_size=self.config[Key.MINI_BATCH_SIZE],
                 output_file_name=self.config[Key.OUTPUT_FILE_NAME],
                 output_action=self.config[Key.OUTPUT_ACTION],
                 error_threshold=self.config[Key.ERROR_THRESHOLD],
                 retry_settings=BatchRetrySettings(
                     max_retries=self.config[Key.MAX_RETRIES],
                     timeout=self.config[Key.SCORING_TIMEOUT_SECONDS],
                 ),
                 logging_level=self.config[Key.LOGGING_LEVEL],
+                environment_variables=self._get_env_vars(model_filename),
                 tags=deployment_tags,
             )
             # TODO check status of deployment
-            self._client.batch_deployments.begin_create_or_update(deployment).result(
-                self.config[Key.ENDPOINT_DEPLOYMENT_TIMEOUT]
-            )
+            # TODO make `skip_script_validation` configurable
+            self._client.batch_deployments.begin_create_or_update(
+                deployment, skip_script_validation=True
+            ).result(self.config[Key.ENDPOINT_DEPLOYMENT_TIMEOUT])
 
         # ensure deployment is default in batch endpoint
-        endpoint = self._client.batch_endpoints.get(self.endpoint_name)
-        endpoint.defaults.deployment_name = deployment.name
-        self._client.batch_endpoints.begin_create_or_update(endpoint)
+        self.make_default(deployment.name)
+
+    def make_default(self, deployment_name, await_results=True):
+        endpoint: BatchEndpoint = self._client.batch_endpoints.get(self.endpoint_name)
+        endpoint.defaults.deployment_name = deployment_name
+        poller = self._client.batch_endpoints.begin_create_or_update(endpoint)
+        if await_results:
+            # TODO: the poller is returning the wrong object type
+            # (azure.ai.ml._restclient.v2022_05_01.models._models_py3.BatchEndpointData)
+            # which doesn't have a provisioning state. For now I'm just going to assume
+            # the operation succeeded.
+            poller.result(self.config[Key.ENDPOINT_UPDATE_TIMEOUT])
+            self.logger.info(
+                "Default deployment for endpoint '%s' updated to: %s",
+                self.deployment_name,
+                self.endpoint_name,
+            )
 
     def delete_endpoint(self):
         self._client.batch_endpoints.begin_delete(name=self.endpoint_name).result(
             self.config[Key.ENDPOINT_DELETION_TIMEOUT]
         )
 
-    def delete_deployment(self):
+    def delete_deployment(self, deployment_to_delete: str = None):
+        deployment_name = deployment_to_delete or self.deployment_name
         self._client.batch_deployments.begin_delete(
-            name=self.deployment_name, endpoint_name=self.endpoint_name
+            name=deployment_name, endpoint_name=self.endpoint_name
         ).result(self.config[Key.DEPLOYMENT_DELETION_TIMEOUT])
 
     def deployment_logs(self):
         return ""  # NOOP batch endpoint does not provide logs
 
     def deployment_status(self) -> Union[None, str]:
         try:
```

## bosun/plugin/azureml/client/online_endpoint_client.py

```diff
@@ -5,135 +5,203 @@
 #  DataRobot, Inc. Confidential.
 #  This is proprietary source code of DataRobot, Inc. and its affiliates.
 #
 #  This file and its contents are subject to DataRobot Tool and Utility Agreement.
 #  For details, see
 #  https://www.datarobot.com/wp-content/uploads/2021/07/DataRobot-Tool-and-Utility-Agreement.pdf.
 #  ---------------------------------------------------------------------------------
+import typing
+from contextlib import suppress
+from datetime import datetime
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import Union
 
+from azure.ai.ml._restclient.v2022_02_01_preview.models import OnlineEndpointData
 from azure.ai.ml.constants import AssetTypes
 from azure.ai.ml.entities import CodeConfiguration
 from azure.ai.ml.entities import Environment
+from azure.ai.ml.entities import IdentityConfiguration
+from azure.ai.ml.entities import ManagedIdentityConfiguration
 from azure.ai.ml.entities import ManagedOnlineDeployment
 from azure.ai.ml.entities import ManagedOnlineEndpoint
 from azure.ai.ml.entities import Model
 from azure.ai.ml.entities import OnlineDeployment
 from azure.ai.ml.entities import OnlineEndpoint
 from azure.ai.ml.entities import OnlineRequestSettings
+from azure.ai.ml.entities import SystemData
 from azure.ai.ml.exceptions import LocalEndpointInFailedStateError
 from azure.ai.ml.exceptions import LocalEndpointNotFoundError
+from azure.ai.ml.operations import OnlineEndpointOperations
+from azure.core.exceptions import HttpResponseError
 from azure.core.exceptions import ResourceNotFoundError
 
 from bosun.plugin.azureml.client.base_endpoint_client import BaseEndpointClient
 from bosun.plugin.azureml.client.scoring_snippets import AzureMLOnlineEndpointScoringSnippet
 from bosun.plugin.azureml.config.azureml_client_config import AZURE_BASE_ENVIRONMENT
+from bosun.plugin.azureml.config.azureml_client_config import AZURE_TEMPLATE_DIR
 from bosun.plugin.azureml.config.azureml_client_config import EndpointConfig
 from bosun.plugin.azureml.config.config_keys import Constants
 from bosun.plugin.azureml.config.config_keys import EndpointType
 from bosun.plugin.azureml.config.config_keys import Key
 from bosun.plugin.azureml.config.config_keys import ProvisioningState
+from bosun.plugin.constants import DeploymentState
 
 
 class OnlineEndpointClient(BaseEndpointClient):
-    TEMPLATE_DIR = Path(__file__).parent.parent / "templates"
-    ENDPOINT_TYPE = EndpointType.ONLINE_ENDPOINT
+    ENDPOINT_TYPE = EndpointType.ONLINE
+    SNIPPET_GENERATOR = AzureMLOnlineEndpointScoringSnippet
 
     def __init__(self, config: EndpointConfig):
         super().__init__(config)
-        self.endpoint_name = self.config[Key.ENDPOINT_NAME]
-        self.deployment_name = self.config[Key.DEPLOYMENT_NAME]
         self.compute_virtual_machine = self.config[Key.COMPUTE_VIRTUAL_MACHINE]
         self.compute_instance_count = self.config[Key.COMPUTE_INSTANCE_COUNT]
 
-    def get_scoring_snippet(self, model_filename: str) -> str:
-        scoring_template = AzureMLOnlineEndpointScoringSnippet(model_filename=model_filename)
-        return scoring_template.render()
-
-    def create_endpoint(self):
+    def create_or_update_endpoint(self):
         endpoint_tags = {
             Key.DATAROBOT_DEPLOYMENT_ID.value: self.datarobot_deployment_id,
             Key.DATAROBOT_ENVIRONMENT_ID.value: self.datarobot_environment_id,
         }
         endpoint_tags.update(self.prediction_environment_tags)
-        endpoint = ManagedOnlineEndpoint(
-            name=self.endpoint_name, auth_mode=Constants.AUTH_MODE_KEY.value, tags=endpoint_tags
+        user_identity = (
+            None
+            if not self.config.is_monitoring_enabled
+            else IdentityConfiguration(
+                type=Constants.USER_ASSIGNED_IDENTITY.value,
+                user_assigned_identities=[
+                    ManagedIdentityConfiguration(
+                        resource_id=self.config[Key.AZURE_MANAGED_IDENTITY_ID]
+                    )
+                ],
+            )
         )
 
+        endpoint = None
+        with suppress(ResourceNotFoundError, LocalEndpointNotFoundError):
+            # try to get an existing endpoint to preserve traffic settings during update
+            endpoint = self.get_endpoint()
+
+        if endpoint:
+            endpoint.tags.update(endpoint_tags)
+            endpoint.identity = user_identity
+        else:
+            endpoint = ManagedOnlineEndpoint(
+                name=self.endpoint_name,
+                auth_mode=Constants.AUTH_MODE_KEY.value,
+                tags=endpoint_tags,
+                identity=user_identity,
+            )
+
         result = self._client.online_endpoints.begin_create_or_update(endpoint, local=self._local)
         if not self._local:
             result: OnlineEndpoint = result.result(self.config[Key.ENDPOINT_CREATION_TIMEOUT])
 
         if result.provisioning_state == ProvisioningState.SUCCEEDED.value:
             self.logger.info("Endpoint %s is successfully created.", self.endpoint_name)
         elif self._local:
             # For local, if there was no exception then it was a success
             self.logger.info("Local Endpoint %s is successfully created.", self.endpoint_name)
         else:
             message = (
                 f"Failed to create endpoint {endpoint.name}. Status: {result.provisioning_state}"
             )
             self.logger.error(message)
-            raise RuntimeError(message)  # TODO should raise custom exception
+            raise RuntimeError(message)
 
     def get_endpoint(self) -> OnlineEndpoint:
         return self._client.online_endpoints.get(self.endpoint_name, local=self._local)
 
-    def create_deployment(self, model, environment: Environment):
+    def get_endpoint_traffic_settings(
+        self,
+    ) -> typing.Optional[typing.Tuple[datetime, dict]]:
+
+        endpoints_api: OnlineEndpointOperations = self._client.online_endpoints
+
+        if self._local:
+            modified_at = None
+            endpoint: OnlineEndpoint = endpoints_api.get(
+                name=self.endpoint_name, **self.local_parameter
+            )
+            return modified_at, endpoint.traffic
+
+        # Read JSON response from an endpoint public API in order to get lastModifiedAt field
+        # which is not exposed by the OnlineEndpoint entity. API returns UTC datetime string
+        # in ISO 8601 format: e.g. 2020-01-01T12:34:56.999Z
+        endpoint: OnlineEndpointData = endpoints_api._online_operation.get(
+            resource_group_name=self.config[Key.AZURE_RESOURCE_GROUP],
+            workspace_name=self.config[Key.AZURE_WORKSPACE],
+            endpoint_name=self.endpoint_name,
+            **endpoints_api._init_kwargs,
+        )
+        self.logger.info("Found existing endpoint %s.", self.endpoint_name)
+        system_data: SystemData = endpoint.system_data
+        azure_endpoint_created_at = system_data.created_at if system_data else None
+        azure_endpoint_last_modified_at = system_data.last_modified_at if system_data else None
+        self.logger.info(
+            f"Azure endpoint created_at: {azure_endpoint_created_at}, "
+            f"modified_at: {azure_endpoint_last_modified_at}"
+        )
+        return (
+            azure_endpoint_last_modified_at,
+            endpoint.properties.traffic,
+        )
+
+    def create_deployment(self, deployment_name: str, model, environment: Environment):
         model_filename = Path(model.path).name
         scoring_script_name = "score.py"
         deployment_tags = {
             Key.DATAROBOT_ENVIRONMENT_ID.value: self.datarobot_environment_id,
             Key.DATAROBOT_DEPLOYMENT_ID.value: self.datarobot_deployment_id,
             Key.DATAROBOT_MODEL_ID.value: self.datarobot_model_id,
         }
         deployment_tags.update(self.prediction_environment_tags)
+
         with ScratchDir(cleanup=not self._local) as scoring_code_dir:
             scoring_code_file = scoring_code_dir / scoring_script_name
             scoring_code_file.write_text(self.get_scoring_snippet(model_filename))
             # Fix permissions when running in self._local (e.g. docker bind mount) mode
             scoring_code_dir.chmod(0o755)
             scoring_code_file.chmod(0o644)
 
             # SDK requires scoring timeout to be in millis
             scoring_timeout_ms = self.config[Key.SCORING_TIMEOUT_SECONDS] * 1000
             deployment = ManagedOnlineDeployment(
-                name=self.deployment_name,
+                name=deployment_name or self.deployment_name,
                 endpoint_name=self.endpoint_name,
                 model=model,
                 environment=environment,
                 code_configuration=CodeConfiguration(
                     code=str(scoring_code_dir), scoring_script=scoring_script_name
                 ),
                 request_settings=OnlineRequestSettings(request_timeout_ms=scoring_timeout_ms),
                 instance_type=self.compute_virtual_machine,
                 instance_count=self.compute_instance_count,
-                environment_variables={"DATAROBOT_MODEL_FILENAME": str(model_filename)},
+                environment_variables=self._get_env_vars(model_filename),
                 tags=deployment_tags,
             )
 
             try:
                 result = self._client.online_deployments.begin_create_or_update(
-                    deployment=deployment, local=self._local
+                    # TODO: make `skip_script_validation` configurable
+                    deployment=deployment,
+                    local=self._local,
+                    skip_script_validation=True,
                 )
             except LocalEndpointInFailedStateError as e:
                 self.logger.error("Failed to create local deployment: %s", e)
-                result = type(deployment)(
+                result = ManagedOnlineDeployment(
                     **deployment._to_dict(), provisioning_state=ProvisioningState.FAILED.value
                 )
 
         if not self._local:
-            result: OnlineDeployment = result.result(self.config[Key.ENDPOINT_DEPLOYMENT_TIMEOUT])
+            result = result.result(self.config[Key.ENDPOINT_DEPLOYMENT_TIMEOUT])
 
         if result.provisioning_state == ProvisioningState.SUCCEEDED.value:
             self.logger.info("Deployment %s is successfully created.", self.deployment_name)
         else:
-            # TODO should raise custom exception
             msg = (
                 f"Failed to create deployment {deployment.name}"
                 f" (endpoint={self.endpoint_name};model={model.name})."
                 f" Status: {result.provisioning_state}"
             )
             self.logger.error(msg)
             try:
@@ -166,89 +234,159 @@
         except LocalEndpointNotFoundError:
             # To be idempotent, if the endpoint is already gone then just ignore.
             pass
         else:
             if not self._local:
                 result.result(timeout_seconds)
 
-    def delete_deployment(self):
+    def delete_deployment(self, deployment_to_delete: str = None):
+        deployment_name = deployment_to_delete or self.deployment_name
+
         self.logger.info(
             "Deleting deployment %s from online endpoint %s...",
-            self.deployment_name,
+            deployment_name,
             self.endpoint_name,
         )
         result = self._client.online_deployments.begin_delete(
-            name=self.deployment_name, endpoint_name=self.endpoint_name, local=self._local
+            name=deployment_name, endpoint_name=self.endpoint_name, local=self._local
         )
         if not self._local:
             result.result(self.config[Key.DEPLOYMENT_DELETION_TIMEOUT])
 
     def deployment_logs(self) -> str:
         return self._client.online_deployments.get_logs(
             name=self.deployment_name,
             endpoint_name=self.endpoint_name,
             lines=self.config[Key.DEPLOYMENT_LOG_LINES_COUNT],
             local=self._local,
         )
 
     def deployment_status(self) -> Union[None, str]:
         try:
+            endpoint: OnlineEndpoint = self._client.online_endpoints.get(
+                name=self.endpoint_name, local=self._local
+            )
             deployment: OnlineDeployment = self._client.online_deployments.get(
                 name=self.deployment_name, endpoint_name=self.endpoint_name, local=self._local
             )
         except (LocalEndpointNotFoundError, ResourceNotFoundError):
+            endpoint = None
             deployment = None
 
-        if deployment is None:
+        if endpoint is None or deployment is None:
             return None  # status unknown
 
-        return self.map_state(deployment.provisioning_state)
+        deployment_state = self.map_online_deployment_state(
+            endpoint_state=endpoint.provisioning_state,
+            deployment_state=deployment.provisioning_state,
+        )
+
+        return deployment_state
+
+    @staticmethod
+    def map_online_deployment_state(endpoint_state, deployment_state):
+        # (endpoint_state, deployment_state) -> DR deployment_state
+        state_map = {
+            (  # deployment creation
+                ProvisioningState.UPDATING.value,
+                ProvisioningState.UPDATING.value,
+            ): DeploymentState.LAUNCHING,
+            (  # endpoint traffic update
+                ProvisioningState.UPDATING.value,
+                ProvisioningState.SUCCEEDED.value,
+            ): DeploymentState.LAUNCHING,
+            (  # deployment deletion. this should be an API bug?
+                ProvisioningState.SUCCEEDED.value,
+                ProvisioningState.UPDATING.value,
+            ): DeploymentState.SHUTTING_DOWN,
+            (  # endpoint deletion
+                ProvisioningState.DELETING.value,
+                ProvisioningState.DELETING.value,
+            ): DeploymentState.SHUTTING_DOWN,
+            (
+                ProvisioningState.SUCCEEDED.value,
+                ProvisioningState.SUCCEEDED.value,
+            ): DeploymentState.READY,
+        }
+
+        return state_map.get((endpoint_state, deployment_state), DeploymentState.UNKNOWN)
+
+    def get_traffic_settings_set_by_user(self) -> typing.Dict[str, str]:
+        traffic_settings = {}
+
+        try:
+            datarobot_traffic_last_modified_at = self.config[Key.ENDPOINT_TRAFFIC_LAST_MODIFIED_AT]
+            azure_endpoint_last_modified_at, _ = self.get_endpoint_traffic_settings()
+            if self._local or datarobot_traffic_last_modified_at > azure_endpoint_last_modified_at:
+                traffic_settings = self.config[Key.ENDPOINT_TRAFFIC]
+            else:
+                self.logger.info(
+                    "Traffic settings are stale. Skipping traffic update for the endpoint '%s'."
+                    "DataRobot traffic modified_at: %s, AzureML endpoint modified_at %s.",
+                    self.endpoint_name,
+                    datarobot_traffic_last_modified_at,
+                    azure_endpoint_last_modified_at,
+                )
+
+        except (ResourceNotFoundError, LocalEndpointNotFoundError):
+            # for a new endpoint, always apply the traffic settings set by user on DataRobot UI
+            traffic_settings = self.config[Key.ENDPOINT_TRAFFIC]
+            self.logger.warning(
+                "Endpoint %s not found. A new one will be created.", self.endpoint_name
+            )
 
-    def update_deployment_traffic(self, await_results=True, new_traffic_value=100):
-        endpoint = self._client.online_endpoints.get(self.endpoint_name, local=self._local)
-        endpoint.traffic = {self.deployment_name: new_traffic_value}
+        except HttpResponseError:
+            # do not apply traffic changes if we unsure on it's current state
+            # do not fail the flow of deployment creation/update or deletion
+            self.logger.error("Can't get endpoint %s", self.endpoint_name, exc_info=True)
+        except AttributeError:
+            self.logger.error(
+                "Can't get 'lastModifiedAt' timestamp for endpoint %s",
+                self.endpoint_name,
+                exc_info=True,
+            )
+
+        return traffic_settings
 
+    def update_deployment_traffic(self, endpoint, traffic_settings, await_results=True):
+        endpoint.traffic.update(traffic_settings)
         result = self._client.online_endpoints.begin_create_or_update(endpoint, local=self._local)
 
         if await_results and not self._local:
-            traffic_update_timeout_seconds = self.config[Key.DEPLOYMENT_TRAFFIC_TIMEOUT]
-            result = result.result(traffic_update_timeout_seconds)
+            result = result.result(self.config[Key.ENDPOINT_UPDATE_TIMEOUT])
             if result.provisioning_state == ProvisioningState.SUCCEEDED.value:
-                self.logger.info(
-                    "Deployment traffic is updated to 100% for deployment %s.", self.deployment_name
-                )
+                self.logger.info("Endpoint traffic is updated to %s.", str(traffic_settings))
             else:
-                # TODO should raise custom exception
-                msg = f"Failed to update traffic for the deployment {self.deployment_name}. "
+                msg = f"Failed to update traffic for the endpoint {self.endpoint_name}. "
                 f"Status: {result.provisioning_state}."
                 self.logger.error(msg)
                 raise RuntimeError(msg)
 
     def get_latest_environment(self):
         # Override base method because local mode is only supported for online
         # endpoints currently.
         if self._local:
             return Environment(
-                conda_file=self.TEMPLATE_DIR / "conda.yml", image=AZURE_BASE_ENVIRONMENT
+                conda_file=AZURE_TEMPLATE_DIR / "conda.yml", image=AZURE_BASE_ENVIRONMENT
             )
         return super().get_latest_environment()
 
     def register_model(self, model_path):
         if self._local:
             self.logger.info("Skipping local model registration")
             return Model(
                 name=self.datarobot_model_name, path=model_path, type=AssetTypes.CUSTOM_MODEL
             )
         return super().register_model(model_path)
 
-    def delete_model(self):
+    def archive_model(self):
         if self._local:
             self.logger.info("Skipping local model deletion")
             return
-        super().delete_model()
+        super().archive_model()
 
 
 class ScratchDir(TemporaryDirectory):
     """
     When running in local mode, AzureML bind mounts the scoring script into the container
     so we can't use an actual temporary file/dir. We will still create the dir/file in
     the temp location so hopefully the OS will cleanup the files for us.
```

## bosun/plugin/azureml/client/scoring_snippets.py

```diff
@@ -6,40 +6,31 @@
 #  This is proprietary source code of DataRobot, Inc. and its affiliates.
 #
 #  This file and its contents are subject to DataRobot Tool and Utility Agreement.
 #  For details, see
 #  https://www.datarobot.com/wp-content/uploads/2021/07/DataRobot-Tool-and-Utility-Agreement.pdf.
 #  ---------------------------------------------------------------------------------
 
+from typing import Optional
+
 from bosun.plugin.azureml.template_renderer import TemplateRenderer
 
 
 class AzureMLBatchEndpointScoringSnippet(TemplateRenderer):
-    def __init__(self, model_filename: str, csv_separator: str = ","):
+    SCORING_SCRIPT = "batch_score.py"
+    TEMPLATE_NAME = "scoring_script_builder.py.j2"
+
+    def __init__(self, model_filename: Optional[str] = None, csv_separator: str = ","):
         super().__init__()
         self.datarobot_model_filename = model_filename
         self.csv_separator = csv_separator
 
-    def template_name(self) -> str:
-        return "azureml_batch_endpoint_score.py"
-
     def context(self) -> dict:
         return {
             "datarobot_model_filename": self.datarobot_model_filename,
             "csv_separator": self.csv_separator,
+            "score_script": self.SCORING_SCRIPT,
         }
 
 
-class AzureMLOnlineEndpointScoringSnippet(TemplateRenderer):
-    def __init__(self, model_filename: str, csv_separator: str = ","):
-        super().__init__()
-        self.model_filename = model_filename
-        self.csv_separator = csv_separator
-
-    def template_name(self) -> str:
-        return "azureml_online_endpoint_score.py"
-
-    def context(self) -> dict:
-        return {
-            "datarobot_model_filename": self.model_filename,
-            "csv_separator": self.csv_separator,
-        }
+class AzureMLOnlineEndpointScoringSnippet(AzureMLBatchEndpointScoringSnippet):
+    SCORING_SCRIPT = "online_score.py"
```

## bosun/plugin/azureml/config/azureml_client_config.py

```diff
@@ -10,134 +10,217 @@
 #  https://www.datarobot.com/wp-content/uploads/2021/07/DataRobot-Tool-and-Utility-Agreement.pdf.
 #  ---------------------------------------------------------------------------------
 
 from __future__ import annotations
 
 import os
 import random
+import re
 import string
+from datetime import timedelta
+from functools import cached_property
+from pathlib import Path
 from typing import Optional as Nullable
 
 import yaml
+from dateutil import parser
+from schema import And
 from schema import Optional
 from schema import Or
 from schema import Schema
 from schema import SchemaError
 from schema import Use
 
 from bosun.plugin.azureml.config.config_keys import EndpointType
 from bosun.plugin.azureml.config.config_keys import Key
+from bosun.plugin.constants import BosunPluginConfigConstants
 from bosun.plugin.deployment_info import DeploymentInfo
 from bosun.plugin.pe_info import PEInfo
 
 AZURE_BASE_ENVIRONMENT = (
     "mcr.microsoft.com/azureml/minimal-ubuntu20.04-py38-cpu-inference:20230313.v1"
 )
 AZURE_CUSTOM_ENVIRONMENT = "datarobot-scoring-code"
-AZURE_TEMPLATE_DIR = os.environ.get("BOSUN_AZURE_TEMPLATE_DIR", "/override/templates/")
+AZURE_TEMPLATE_DIR = Path(__file__).parent.parent / "templates"
+
+ENDPOINT_NAME_PATTERN = re.compile(r"[a-z]+[a-z0-9-]*")
 
 
 def output_action_validator(value):
     allowed_values = {"AppendRow", "SummaryOnly"}
     parts = value.split(" ")
     result = "".join(part.capitalize() for part in parts)
     if result not in allowed_values:
         raise SchemaError(None, errors=f"Output action allowed values: [{allowed_values}]")
     return result
 
 
+def kv_validator(kv_pairs: str, field: Key):
+    """
+    DataRobot UI pass key-value pairs using the following format:
+    key_name1:value1;key_name2:;key_name3:value3
+
+    key names are mandatory, values are optional.
+    """
+    result = {}
+    validation_error = SchemaError(
+        None,
+        errors=f"Invalid formatting of the {field.name}. "
+        f"Expected formatting: key-name1:key-value;key-name2:key-value2",
+    )
+
+    kv_pairs = kv_pairs.strip(" ;") if kv_pairs else None
+
+    if not kv_pairs:
+        return result
+
+    try:
+        for pair in kv_pairs.split(";"):
+            kv = pair.split(":")
+            if len(kv) != 2:
+                # key value pairs are separated by ':'
+                raise validation_error
+
+            key = kv[0].strip()
+            value = kv[1].strip()
+
+            if not key:
+                # empty keys are not allowed
+                raise validation_error
+
+            result[key] = value if value else None
+
+        return result
+    except ValueError:
+        raise validation_error
+
+
+def tags_validator(tags):
+    return kv_validator(tags, Key.AZURE_ENVIRONMENT_TAGS)
+
+
+def traffic_validator(traffic_settings):
+    return kv_validator(traffic_settings, Key.ENDPOINT_TRAFFIC)
+
+
 class EndpointConfig:
     # besides of type validation, converts numeric string to int
     optional_int_type = Or(None, Use(int), int)
 
     base_config_schema = {
-        Key.AZURE_CLIENT_ID.name: str,
-        Key.AZURE_CLIENT_SECRET.name: str,
-        Key.AZURE_TENANT_ID.name: str,
         # required subscription/workspace keys
         Key.AZURE_SUBSCRIPTION_ID.name: str,
         Key.AZURE_RESOURCE_GROUP.name: str,
         Key.AZURE_WORKSPACE.name: str,
         Key.AZURE_LOCATION.name: str,
         # optional
         Optional(Key.AZURE_ENVIRONMENT_NAME.name, default=AZURE_CUSTOM_ENVIRONMENT): Or(None, str),
         Optional(Key.AZURE_ENVIRONMENT_LABEL.name, default="latest"): Or(None, str),
-        Optional(Key.AZURE_ENVIRONMENT_TAGS.name, default={}): Or(None, dict),
+        Optional(Key.ENDPOINT_TRAFFIC.name, default={}): Or(None, Use(traffic_validator)),
+        Optional(Key.ENDPOINT_TRAFFIC_LAST_MODIFIED_AT.name): Or(None, Use(parser.parse)),
+        Optional(Key.AZURE_ENVIRONMENT_TAGS.name, default={}): Or(None, Use(tags_validator)),
+        Optional(Key.AZURE_EVENTHUBS_NAMESPACE.name): Or(None, And(str, len)),
+        Optional(Key.AZURE_EVENTHUBS_INSTANCE.name): Or(None, And(str, len)),
         Optional(Key.LOGGING_LEVEL.name, default="info"): Or(None, str),
         Optional(Key.DEPLOYMENT_LOG_LINES_COUNT.name, default=100): optional_int_type,
-        Optional(Key.SCORING_TIMEOUT_SECONDS.name, default=60): optional_int_type,
-        Optional(Key.ENDPOINT_DEPLOYMENT_TIMEOUT.name, default=600): optional_int_type,
-        Optional(Key.ENDPOINT_DELETION_TIMEOUT.name, default=600): optional_int_type,
-        Optional(Key.DEPLOYMENT_DELETION_TIMEOUT.name, default=600): optional_int_type,
-        Optional(Key.ENDPOINT_CREATION_TIMEOUT.name, default=600): optional_int_type,
+        Optional(
+            Key.SCORING_TIMEOUT_SECONDS.name, default=timedelta(seconds=60).total_seconds()
+        ): optional_int_type,
+        # MLOps imposes a strict 30 min max on all actions so make sure we are under that.
+        Optional(
+            Key.ENDPOINT_DEPLOYMENT_TIMEOUT.name, default=timedelta(minutes=27.5).total_seconds()
+        ): optional_int_type,
+        Optional(
+            Key.ENDPOINT_DELETION_TIMEOUT.name, default=timedelta(minutes=28).total_seconds()
+        ): optional_int_type,
+        Optional(
+            Key.ENDPOINT_UPDATE_TIMEOUT.name, default=timedelta(minutes=15).total_seconds()
+        ): optional_int_type,
+        Optional(
+            Key.DEPLOYMENT_DELETION_TIMEOUT.name, default=timedelta(minutes=15).total_seconds()
+        ): optional_int_type,
+        Optional(
+            Key.ENDPOINT_CREATION_TIMEOUT.name, default=timedelta(minutes=10).total_seconds()
+        ): optional_int_type,
         Optional(Key.AZURE_LOCAL_TESTING.name, default=False): bool,
+        Optional(Key.AZURE_MANAGED_IDENTITY_CLIENT_ID.name): Or(None, And(str, len)),
     }
 
     online_endpoint_schema = {
         **base_config_schema,
         Key.ENDPOINT_NAME.name: str,
         Key.DEPLOYMENT_NAME.name: str,
         Key.COMPUTE_VIRTUAL_MACHINE.name: str,
-        # TODO AGENT-4108 UI should store endpoint type in Deployment's additional metadata
-        Optional(Key._ENDPOINT_TYPE.name): Or(None, "online"),
+        Optional(Key.ENDPOINT_TYPE.name): Or(None, EndpointType.ONLINE.value),
         Optional(Key.COMPUTE_INSTANCE_COUNT.name, default=1): optional_int_type,
-        Optional(Key.DEPLOYMENT_TRAFFIC_TIMEOUT.name, default=600): optional_int_type,
+        Optional(Key.AZURE_MANAGED_IDENTITY_ID.name): Or(None, And(str, len)),
     }
 
     batch_endpoint_schema = {
         **base_config_schema,
         Key.ENDPOINT_NAME.name: str,
         Key.DEPLOYMENT_NAME.name: str,
         Key.COMPUTE_CLUSTER.name: str,
         Key.COMPUTE_CLUSTER_INSTANCE_COUNT.name: Use(int),
-        # TODO AGENT-4108 UI should store endpoint type in Deployment's additional metadata
-        Optional(Key._ENDPOINT_TYPE.name): Or(None, "batch"),
+        Optional(Key.ENDPOINT_TYPE.name): Or(None, EndpointType.BATCH.value),
         Optional(Key.OUTPUT_ACTION.name, default="AppendRow"): Or(
             None, Use(output_action_validator)
         ),
         Optional(Key.OUTPUT_FILE_NAME.name, default="predictions.csv"): Or(None, str),
         Optional(Key.MINI_BATCH_SIZE.name, default=10): optional_int_type,
         Optional(Key.MAX_RETRIES.name, default=3): optional_int_type,
         Optional(Key.MAX_CONCURRENCY_PER_INSTANCE.name, default=1): optional_int_type,
         Optional(Key.ERROR_THRESHOLD.name, default=-1): optional_int_type,
         Optional(Key.AZURE_LOCAL_TESTING.name, default=False): False,  # batch doesn't support local
     }
 
     configs = {
-        EndpointType.ONLINE_ENDPOINT: Schema(online_endpoint_schema, ignore_extra_keys=True),
-        EndpointType.BATCH_ENDPOINT: Schema(batch_endpoint_schema, ignore_extra_keys=True),
-        EndpointType.DEFAULT: Schema(base_config_schema, ignore_extra_keys=True),
+        EndpointType.ONLINE: Schema(online_endpoint_schema, ignore_extra_keys=True),
+        EndpointType.BATCH: Schema(batch_endpoint_schema, ignore_extra_keys=True),
+        EndpointType.UNKNOWN: Schema(base_config_schema, ignore_extra_keys=True),
     }
 
     def __init__(
         self,
         plugin_config: dict,
-        endpoint_type: EndpointType = None,
+        parent_config: dict,
         prediction_environment=None,
         deployment=None,
+        is_model_replacement=False,
     ):
         self._config = plugin_config
-        self._endpoint_type = endpoint_type
+        self._bosun_config = parent_config
         self.prediction_environment = prediction_environment
         self.deployment = deployment
+        self.is_model_replacement = is_model_replacement
 
     def __getitem__(self, key: Key):
         return self._config.get(key.name)
 
     def validate_config(self):
         schema = self.configs[self.deduce_endpoint_type_by_config()]
         self._config = schema.validate(self._config)
 
+        # Post validation
+        if self.is_monitoring_enabled:
+            if not self[Key.AZURE_MANAGED_IDENTITY_CLIENT_ID]:
+                raise ValueError(
+                    f"Monitoring requires {Key.AZURE_MANAGED_IDENTITY_CLIENT_ID} to be set"
+                )
+            if self.is_online_endpoint and not self[Key.AZURE_MANAGED_IDENTITY_ID]:
+                raise ValueError(f"Monitoring requires {Key.AZURE_MANAGED_IDENTITY_ID} to be set")
+
     @classmethod
     def read_config(
         cls,
+        parent_config: dict,
         config_file_path: Nullable[str] = None,
-        endpoint_type: EndpointType = None,
-        prediction_environment: PEInfo = None,
+        prediction_environment: Nullable[PEInfo] = None,
         deployment: Nullable[DeploymentInfo] = None,
+        is_model_replacement: bool = False,
     ) -> EndpointConfig:
         def get_kv_config(entity):
             result = {}
             if entity.kv_config:
                 for key in Key.all():
                     if key in entity.kv_config:
                         result[key] = entity.kv_config[key]
@@ -157,44 +240,65 @@
             pe_additional_metadata = get_kv_config(prediction_environment)
             config.update(pe_additional_metadata)
 
         if deployment:
             deployment_additional_metadata = get_kv_config(deployment)
             config.update(deployment_additional_metadata)
 
-        return EndpointConfig(config, endpoint_type, prediction_environment, deployment)
+        return EndpointConfig(
+            config, parent_config, prediction_environment, deployment, is_model_replacement
+        )
 
     def deduce_endpoint_type_by_config(self):
         if self.is_online_endpoint:
-            return EndpointType.ONLINE_ENDPOINT
+            return EndpointType.ONLINE
         elif self.is_batch_endpoint:
-            return EndpointType.BATCH_ENDPOINT
+            return EndpointType.BATCH
         else:
-            return EndpointType.DEFAULT
+            return EndpointType.UNKNOWN
+
+    @property
+    def is_monitoring_enabled(self):
+        return self._bosun_config[
+            BosunPluginConfigConstants.MLOPS_BOSUN_PRED_ENV_ENABLE_MONITORING_KEY
+        ]
 
     @property
     def endpoint_type(self):
-        return self._config.get(Key._ENDPOINT_TYPE.name)
+        return self._config.get(Key.ENDPOINT_TYPE.name)
 
     @property
     def is_online_endpoint(self):
         if self.endpoint_type:
-            return self.endpoint_type == EndpointType.ONLINE_ENDPOINT.value
+            return self.endpoint_type == EndpointType.ONLINE.value
 
         online_endpoint_keys = {Key.COMPUTE_VIRTUAL_MACHINE.name, Key.COMPUTE_INSTANCE_COUNT.name}
 
         return any(key in self._config for key in online_endpoint_keys)
 
     @property
     def is_batch_endpoint(self):
         if self.endpoint_type:
-            return self.endpoint_type == EndpointType.BATCH_ENDPOINT.value
+            return self.endpoint_type == EndpointType.BATCH.value
 
         batch_endpoint_keys = {Key.COMPUTE_CLUSTER.name, Key.COMPUTE_CLUSTER_INSTANCE_COUNT.name}
 
         return any(key in self._config for key in batch_endpoint_keys)
 
-    def generate_default_name(self):
-        postfix_length = 5
-        postfix = "".join(random.choice(string.ascii_letters) for x in range(postfix_length))
-        workspace_name = self._config.get(Key.AZURE_WORKSPACE)
-        return f"{workspace_name}-{postfix}"
+    @cached_property
+    def new_deployment_name(self):
+        """In case of model replacements, a new unique deployment name is required."""
+        user_set_deployment_name = self._config.get(Key.DEPLOYMENT_NAME.name, "")
+        return self.generate_default_name(user_set_deployment_name)
+
+    @staticmethod
+    def generate_default_name(prefix, postfix_length=5):
+        if not ENDPOINT_NAME_PATTERN.match(prefix):
+            raise ValueError(
+                "Names must begin with a lowercase letter, followed by lowercase letters,"
+                " numbers or hyphen."
+            )
+
+        max_name_len = 32
+        trim_name = max_name_len - postfix_length - 1  # minus the dash symbol
+        postfix = "".join(random.choice(string.ascii_lowercase) for _ in range(postfix_length))
+        return f"{prefix[:trim_name]}-{postfix}"
```

## bosun/plugin/azureml/config/config_keys.py

```diff
@@ -12,20 +12,21 @@
 from enum import Enum
 from enum import auto
 
 
 class Constants(Enum):
     LATEST_VERSION = "latest"
     AUTH_MODE_KEY = "key"
+    USER_ASSIGNED_IDENTITY = "user_assigned"
 
 
 class EndpointType(Enum):
-    BATCH_ENDPOINT = "batch"
-    ONLINE_ENDPOINT = "online"
-    DEFAULT = "default"
+    BATCH = "BATCH_ENDPOINT"
+    ONLINE = "ONLINE_ENDPOINT"
+    UNKNOWN = "default"
 
 
 class ProvisioningState(Enum):
     CREATING = "Creating"
     DELETING = "Deleting"
     SCALING = "Scaling"
     UPDATING = "Updating"
@@ -41,36 +42,43 @@
     # fields set from Bosun plugin configuration
     DATAROBOT_ENVIRONMENT_ID = auto()
     DATAROBOT_DEPLOYMENT_ID = auto()
     DATAROBOT_MODEL_ID = auto()
     DATAROBOT_MODEL_NAME = auto()
     DATAROBOT_MODEL_DESCRIPTION = auto()
 
-    # credentials are exported to environmental variables
-    AZURE_CLIENT_ID = auto()
-    AZURE_CLIENT_SECRET = auto()
-    AZURE_TENANT_ID = auto()
+    # TODO ask MS team to expose SystemData in Deployment and Endpoint objects
+    # so we don't need to add workarounds
+    DEPLOYMENT_CREATED_AT = auto()
 
     # fields set from Prediction Environment / additional metadata
     AZURE_SUBSCRIPTION_ID = auto()
     AZURE_RESOURCE_GROUP = auto()
     AZURE_WORKSPACE = auto()
     AZURE_LOCATION = auto()
+    AZURE_ENVIRONMENT_TAGS = auto()
+    AZURE_EVENTHUBS_NAMESPACE = auto()
+    AZURE_EVENTHUBS_INSTANCE = auto()
+    AZURE_MANAGED_IDENTITY_ID = auto()
+    AZURE_MANAGED_IDENTITY_CLIENT_ID = auto()
 
     # fields set from Deployment additional metadata
     # configuration for endpoints [online, batch]
 
     # underscorized property name means it's some internal property and it's not rendered as
     # a list of key-values on UI. It may be rendered as a separate UI element (e.g. endpoint toggle)
-    _ENDPOINT_TYPE = auto()
+    ENDPOINT_TYPE = auto()
     ENDPOINT_NAME = auto()
     DEPLOYMENT_NAME = auto()
     SCORING_TIMEOUT_SECONDS = auto()
 
     # online endpoint settings
+    ENDPOINT_TRAFFIC = auto()
+    # UTC datetime string in ISO 8601 format, e.g. 2020-01-01T12:34:56.999Z
+    ENDPOINT_TRAFFIC_LAST_MODIFIED_AT = auto
     COMPUTE_VIRTUAL_MACHINE = auto()
     COMPUTE_INSTANCE_COUNT = auto()
 
     # batch endpoint settings
     OUTPUT_ACTION = auto()
     OUTPUT_FILE_NAME = auto()
     MINI_BATCH_SIZE = auto()
@@ -80,20 +88,19 @@
     LOGGING_LEVEL = auto()
     COMPUTE_CLUSTER = auto()
     COMPUTE_CLUSTER_INSTANCE_COUNT = auto()
 
     # Properties below are not exposed via UI
     AZURE_ENVIRONMENT_NAME = auto()
     AZURE_ENVIRONMENT_LABEL = auto()
-    AZURE_ENVIRONMENT_TAGS = auto()
     ENDPOINT_CREATION_TIMEOUT = auto()
     ENDPOINT_DELETION_TIMEOUT = auto()
     ENDPOINT_DEPLOYMENT_TIMEOUT = auto()
+    ENDPOINT_UPDATE_TIMEOUT = auto()
     DEPLOYMENT_DELETION_TIMEOUT = auto()
-    DEPLOYMENT_TRAFFIC_TIMEOUT = auto()
     DEPLOYMENT_LOG_LINES_COUNT = auto()
 
     AZURE_LOCAL_TESTING = auto()
 
     @classmethod
     def all(cls):
         return [e.name for e in cls]
```

## bosun/plugin/k8s/config.py

```diff
@@ -45,14 +45,15 @@
     PPS_TOLERATIONS = "ppsTolerations"
     PPS_AFFINITY = "ppsAffinity"
     PPS_EXTRA_ENV = "ppsExtraEnvironment"
     PPS_EXTRA_VOL = "ppsExtraVolumes"
     PPS_EXTRA_VOLM = "ppsExtraVolumeMounts"
     OUTFACING_PREDICTION_URL_PREFIX = "outfacingPredictionURLPrefix"
     GENERATED_IMAGE_REPO = "generatedImageRepo"
+    KUBE_CONFIG_FILE = "kubeConfigFile"
     KUBE_CONFIG_CONTEXT = "kubeConfigContext"
     KUBE_NAMESPACE = "kubeNamespace"
     INGRESS_CLASS = "ingressClass"
     INGRESS_TYPE = "ingressType"
     KANIKO_IMAGE = "kanikoImage"
     KANIKO_CONFIG = "kanikoConfigmapName"
     KANIKO_SECRET = "kanikoSecretName"
@@ -107,14 +108,16 @@
                     r"^https?://.+", error="Not a valid URL: {}"
                 ),
                 Optional(KubernetesPluginConfig.AGENT_SIDECAR, default=True): bool,
                 Optional(KubernetesPluginConfig.AGENT_IMAGE): Or(None, str),
                 Optional(KubernetesPluginConfig.AGENT_RESOURCES, default={}): dict,
                 Optional(KubernetesPluginConfig.AGENT_SECURITY, default={}): dict,
                 Optional(BosunPluginConfigConstants.MLOPS_API_TOKEN_KEY): str,
+                # Null value means use K8s client default logic to find config file.
+                Optional(KubernetesPluginConfig.KUBE_CONFIG_FILE): Or(None, str),
                 # Passing a null value actually has special meaning here. It means use the
                 # default context that the K8s API client wants to use (either set via env var or
                 # defined in the users ~/.kube/config file). By default we assume this plugin is running
                 # inside a k8s Pod.
                 Optional(KubernetesPluginConfig.KUBE_CONFIG_CONTEXT, default="IN_CLUSTER"): Or(
                     None, str
                 ),
@@ -330,14 +333,18 @@
         return self._config[KubernetesPluginConfig.PPS_EXTRA_VOLM]
 
     @property
     def generated_image_repo(self):
         return self._config[KubernetesPluginConfig.GENERATED_IMAGE_REPO]
 
     @property
+    def kubernetes_config_file(self):
+        return self._config[KubernetesPluginConfig.KUBE_CONFIG_FILE]
+
+    @property
     def kubernetes_config_context(self):
         return self._config[KubernetesPluginConfig.KUBE_CONFIG_CONTEXT]
 
     @property
     def kubernetes_namespace(self):
         return self._config.get(KubernetesPluginConfig.KUBE_NAMESPACE)
```

## bosun/plugin/k8s/kubernetes_plugin.py

```diff
@@ -66,14 +66,15 @@
 class KubernetesPlugin(BosunPluginBase):
     def __init__(self, plugin_config, private_config_file, pe_info, dry_run):
         super().__init__(plugin_config, private_config_file, pe_info, dry_run)
         self._config = KubernetesPluginConfig.from_files(
             self._plugin_config, self._private_config_file
         )
         self._client = get_client(
+            config_file=self._config.kubernetes_config_file,
             context=self._config.kubernetes_config_context,
             namespace=self._config.kubernetes_namespace,
         )
         self._renderer = ResourceBuilder(self._config, self._pe_info)
 
     def plugin_start(self):
         """
```

## Comparing `datarobot_bosun-9.1.1b1.data/scripts/bosun-plugin-runner` & `datarobot_bosun-9.1.1rc1.data/scripts/bosun-plugin-runner`

 * *Files identical despite different names*

## Comparing `datarobot_bosun-9.1.1b1.data/scripts/mcrunner` & `datarobot_bosun-9.1.1rc1.data/scripts/mcrunner`

 * *Files identical despite different names*

## Comparing `datarobot_bosun-9.1.1b1.data/scripts/plugin-runner` & `datarobot_bosun-9.1.1rc1.data/scripts/plugin-runner`

 * *Files identical despite different names*

## Comparing `datarobot_bosun-9.1.1b1.dist-info/METADATA` & `datarobot_bosun-9.1.1rc1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarobot-bosun
-Version: 9.1.1b1
+Version: 9.1.1rc1
 Summary: datarobot-bosun module providing MLOps Management framework and plug-ins
 Home-page: http://datarobot.com
 Author: DataRobot
 Author-email: info@datarobot.com
 License: DataRobot
 Project-URL: Documentation, https://docs.datarobot.com/en/docs/release/public-preview/mlops-preview/mgmt-agent.html#mlops-management-agent
 Platform: UNKNOWN
```

## Comparing `datarobot_bosun-9.1.1b1.dist-info/RECORD` & `datarobot_bosun-9.1.1rc1.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -4,47 +4,50 @@
 bosun/model_connector/file_uri_fetcher.py,sha256=voMRhzmZEY23uRh0LqL5w5aZCZxaAmWfgT_O3TBW1QQ,1395
 bosun/model_connector/mc_bosun.py,sha256=lCo6xyXg6YfwsP8Oh2UmFVQgusLwUpDcD98qyEFHACA,7190
 bosun/model_connector/mc_runner.py,sha256=xFxhvllb0W--AoP7m1aN0GyCY2eOQBk4e9D0heKm5R8,5269
 bosun/model_connector/model_connector_base.py,sha256=DSV1DI9n6bPk0J5dzQjQQCRHsIpawGF5miBX3f2hRMY,5433
 bosun/model_connector/s3_uri_fetcher.py,sha256=MAhtLIBhy8T-ACUFQ_-OyRl-Dm4UEpyq2ZlXO210dS4,2334
 bosun/model_connector/uri_fetcher_base.py,sha256=03RVfWSkb_jIa6EpIIwmIOfcw-6EMcW5wzwmIHnvB0Y,894
 bosun/plugin/__init__.py,sha256=jpqAqC1Ils82n2QssUt_W0fcKI6z6JUz4KJ-tyMWTro,583
-bosun/plugin/action_status.py,sha256=3WAqo1_pSw5KzIzvNbhvmgChiC_lX2ViRAGEsl8yUG8,2225
-bosun/plugin/bosun_plugin_base.py,sha256=X2wtg6Zn4QxZEvB7WsnDkweKb2KyaRBrEJzZaixF9_g,5957
+bosun/plugin/action_status.py,sha256=WWgF7KlMZLZN3iKHfPBRHvqNGey-SDZQIIp0aVXWHw0,2260
+bosun/plugin/bosun_plugin_base.py,sha256=H36wBTOyTdvx6qeYD1I8nPAR3IXn4uw0x_YR5cXk56s,6147
 bosun/plugin/bosun_test_plugin.py,sha256=W97oxU9Y__d5e_LGkPV6f2UtZvj3cuyHkZ1AKq1D7Mw,11466
-bosun/plugin/constants.py,sha256=QDr7g31LPrxk5ToCTW129XrWJ1od11hiP0kK1W_GI_Y,2735
+bosun/plugin/constants.py,sha256=EC8rwSudYn9Nj0htnue1gEXjivqEVUlz8FdHASoTW7E,2833
 bosun/plugin/deployment_info.py,sha256=lJOP2S9sQC-bw-X5rMHw3IZbBV4-DcKH2vvGe9OF4QE,3354
 bosun/plugin/exceptions.py,sha256=XiPxJWyRd50MBAO3Ztu4KrlL5oSBjcPBK8IDD1sWHo0,1047
 bosun/plugin/pe_info.py,sha256=ey2Ef1zzK1jHO705xlpZo3jmdA5UW2S6e99mf_Xy4YI,2493
-bosun/plugin/plugin_runner.py,sha256=fvjuJASX6wXNyGROVwUM-SY1CYqbRgQB5mHQZ1f3Wmw,16631
+bosun/plugin/plugin_runner.py,sha256=KpV3LKIYnqdTMaGgGMABiBdRZzTyB3hmjG4mek4Tng4,16799
 bosun/plugin/azureml/__init__.py,sha256=w0FppK0OReL18im5hlOAeWB_NYCFPFaSmnbqIxIspj4,640
-bosun/plugin/azureml/azureml_plugin.py,sha256=QKjTRB4ybxj4E6zYd01Yq7qaLFr0RxmRqnS7vDecJoY,8275
-bosun/plugin/azureml/azureml_status_reporter.py,sha256=z5fSZy1xGfx7eFkR7wcWOlbbwgM2rnfKGI_cvepPax4,3058
-bosun/plugin/azureml/template_renderer.py,sha256=8y5kt4asrvtykNCu7SU-d4_HXJHc_8Nkt6PN-DzpM6I,1504
-bosun/plugin/azureml/client/base_endpoint_client.py,sha256=Iydk78rg395b6xf5skGWb_egNHoxG8GsPZI95tuDI8Q,10060
-bosun/plugin/azureml/client/batch_endpoint_client.py,sha256=prciD-GZ3VrqHSBvPw3puN-ptbXiG28P4jIC-sDqmiA,5885
-bosun/plugin/azureml/client/online_endpoint_client.py,sha256=4sgQmsRKaRsPLGofaoiwzQia_OUiVekPSjLgHUYwOLI,12088
-bosun/plugin/azureml/client/scoring_snippets.py,sha256=kboJhrumqNhJvwTV_LHzkkSel1WONvhuoOx4FS3lWPw,1680
+bosun/plugin/azureml/azureml_plugin.py,sha256=sfF2miMrgviV12u-u3jkX3iAHc7Xp2CBszpFbvSZ5NM,12218
+bosun/plugin/azureml/azureml_status_reporter.py,sha256=62KW9cDxvqKXgsXpbvIQnq28d54h7_xzYA_IjAFv7p4,3313
+bosun/plugin/azureml/template_renderer.py,sha256=IKm8M_4h1CvMN-Ujx3t_EiDMVugmVNUs8DlZqJnT51Q,1516
+bosun/plugin/azureml/client/base_endpoint_client.py,sha256=C6l-Pv1NMQ91AiXrtrt6k6c-V-XsfogeLRjM_SdisIY,18410
+bosun/plugin/azureml/client/batch_endpoint_client.py,sha256=mZV7GddP3RE3IwN54V6kmeqDFxE2ZQsL8hbnukhxBZY,6743
+bosun/plugin/azureml/client/online_endpoint_client.py,sha256=Po6920-XaJh4NqR-MgUmhRs52tTT5qJO4C1oJ9RmUwY,17972
+bosun/plugin/azureml/client/scoring_snippets.py,sha256=DhIxVo2jpKg6F_p5d1fuqNOQQ_pFHYjHyIbDGtUc2bA,1394
 bosun/plugin/azureml/config/__init__.py,sha256=5LKBu0qgbs3MEvPz1MWIyivQ_LsncJV9bDTFdIEqoJk,583
-bosun/plugin/azureml/config/azureml_client_config.py,sha256=f70E3E_qdtB1EtohQ3BPYYKpBd1CrMpK-HY0oRIoZk4,8036
-bosun/plugin/azureml/config/config_keys.py,sha256=LK8HBTgCmGlHa3FjypcNLN77hehb5dj1bZniIpI6gxQ,3059
-bosun/plugin/azureml/templates/azureml_batch_endpoint_score.py,sha256=cpg30f2gjntk6lDhUvZaHv29m-ZhKXzW-F3fDN6pAz4,3368
-bosun/plugin/azureml/templates/azureml_online_endpoint_score.py,sha256=hl0-GjpuW8QiUfqD8AfaO6Hn4nRpPgHrydK5dXOfn6A,4814
+bosun/plugin/azureml/config/azureml_client_config.py,sha256=wBgvfEckS-wP-WNxPU6WrS_bzhc53_1CQt9jRRIvH7w,11520
+bosun/plugin/azureml/config/config_keys.py,sha256=IMKpnVT6Z2NPbc7Q230MZgbckJIw5wqmFCYI0IAOLSQ,3420
+bosun/plugin/azureml/templates/batch_score.py,sha256=aPULuPwZtHRz3ZzykiDbvsrFyVTxOqGlqIMBsJMOPKI,3767
+bosun/plugin/azureml/templates/common.py,sha256=VoN1HfviW9MmPFa9jdgexM2EMRBa7i9ZmNY7FAIN5ck,9634
+bosun/plugin/azureml/templates/conda.yml,sha256=RxGpt6rw4DizjDPht5YWp1p5i0Dx0HCSiIVQXCamYHE,697
+bosun/plugin/azureml/templates/online_score.py,sha256=BeZscUL5Wk0HHX3vb3jmb3B0xEDet3nPIoa24H50EhE,5452
+bosun/plugin/azureml/templates/scoring_script_builder.py.j2,sha256=ggw_rSteAoJM9tNLJxCdu-jjGzC62b7DnL2pUnHj3aI,963
 bosun/plugin/config_samples/__init__.py,sha256=sAc8oDBMnbrQI82jZrO-TKBO4JwXaMPLnO7cZw6GkxM,702
 bosun/plugin/docker/__init__.py,sha256=HBnE1c15RavjXjjlGCEqQm7PgKETJl1cLW3othCfBPU,757
 bosun/plugin/docker/docker_helper.py,sha256=fubvtoFhsJihzazfLk2gsfD_1YgxE0B_aJSoacQEcKU,14934
 bosun/plugin/docker/docker_plugin.py,sha256=LCoEkUCfaVKf4VcGrSM7wWVnRcWMazNBCj2tKPNzFek,23290
 bosun/plugin/docker/docker_plugin_config.py,sha256=haxXV6dkolVNXXxy1uG7e3O7xV32ALibwDVwye2234U,5419
 bosun/plugin/docker/mlops_monitoring.py,sha256=UXtIj4Uybr9SY4m1uFZAoiRpsOAii343rYPpVt2trZ0,7897
 bosun/plugin/filesystem/__init__.py,sha256=DS_gsVTXiCIXCKL6eJe14Jye0Q08EvJoQaFagwvzTJI,646
 bosun/plugin/filesystem/filesystem_plugin.py,sha256=PB675cG9e59i1qSzEd2CbCjXXHRYZrp08X9p-bFXKk0,14021
 bosun/plugin/k8s/__init__.py,sha256=AfSBWxZWkUluB4pI2V6dlvZ1znEdTT8wDx4QHxSQIZ8,646
 bosun/plugin/k8s/client.py,sha256=TX0Zz3z6VPypQLeh5nyIwWF9AjJ2rlMHzRq6XQ2uPSU,37071
-bosun/plugin/k8s/config.py,sha256=RYoz9P034IZXw-CTn4oFxCYgVkbcQA0-P--sZSY1khY,19918
-bosun/plugin/k8s/kubernetes_plugin.py,sha256=nerEx-jAYOap7qMq_m0vSGG3liBU8ToTc3R4aSqqb3k,28164
+bosun/plugin/k8s/config.py,sha256=nGS-Ica0jsElogxiU6sPyQ26Hf_p60qPCfunfUjyx-w,20247
+bosun/plugin/k8s/kubernetes_plugin.py,sha256=-PjgQtmJivFQlSG1AGa6MlvnZDKUoF5brCnNfdDAzEk,28225
 bosun/plugin/k8s/manifests.py,sha256=j0IesWl7nnOAvwphIIYSACrzM6JoGNqBK4tteQxInKg,9170
 bosun/plugin/k8s/templates/Dockerfile.pps-model.j2,sha256=i9mZbUArvs1q4N6z9vtB5CHqya3USqRzK17Zwl-6w1k,303
 bosun/plugin/k8s/templates/_helpers.j2,sha256=arpcrQvzhk-ZH7pyIpNXPqIf1NZ2RlrZxfyuY3DAfZs,2263
 bosun/plugin/k8s/templates/cm_pps_installer.sh.j2,sha256=L5F7pP4M_HqsNP2wTqMMiNDbWB5pndHQi2vHlr4mCDo,4603
 bosun/plugin/k8s/templates/image-builder.yaml.j2,sha256=DjYTQSHq2uSxC0bOPr-fp6nrZEFi1tcmTVIkwpt2dRM,1393
 bosun/plugin/k8s/templates/mlops-api-secret.yaml.j2,sha256=RgnvF5CGVBsq3ThtKU3MjjlALUqD-w1xjkEjZ0sR14g,356
 bosun/plugin/k8s/templates/model-resources.yaml.j2,sha256=A1SW1aNFSswwsHXhh89u4L9p2Bd10jTJItjNFJpRcWA,1106
@@ -56,14 +59,14 @@
 bosun/plugin/k8s/templates/model-resources/service.yaml.j2,sha256=uvp3IeGLMR1slrY9S5jlPH8lm4tRwm1lD3HnAm36jU0,547
 bosun/plugin/s3/__init__.py,sha256=K1whUFDQfXk5zzO_B7cdIf5rFBhBXkKveGb2utt5OAo,630
 bosun/plugin/s3/s3_plugin.py,sha256=EF-orhokbNFCev9P1liSroojc6TdT3A-2wdPGO79CEI,11175
 bosun/plugin/s3/s3_plugin_config.py,sha256=bDKpMgdCEXSiLiAmKlEcw5DP0ShrTZmUbJuA3U6VbRs,2705
 bosun/plugin/snowflake/__init__.py,sha256=DP4zjkZvK-kb975NTxg1HF_UTQYbwQPszpI2QJUbdR8,644
 bosun/plugin/snowflake/snowflake_plugin.py,sha256=HE308wrkeS5Ie1kMrDTKx7KbsRNuDX1qjPapozdaYck,10034
 bosun/plugin/snowflake/snowflake_plugin_config.py,sha256=KclEb3I9xEkJPf-0ZZcH2QCNI1bCRKhmYWy9-aW-GmE,5491
-datarobot_bosun-9.1.1b1.data/scripts/bosun-plugin-runner,sha256=e8YQBceK8QeD8EFh1q5Vb-jlAYxlrzvZllDq3LNnVPg,671
-datarobot_bosun-9.1.1b1.data/scripts/mcrunner,sha256=FPqMPz123TVvMrWf1bBsu17RSoJJwXA0-M9EG5IdpXg,676
-datarobot_bosun-9.1.1b1.data/scripts/plugin-runner,sha256=pe1lGnDyvW82cBjewuRhb6ad6q3j4TYEJLurzG6GNdk,671
-datarobot_bosun-9.1.1b1.dist-info/METADATA,sha256=8h0qjHtlBCZ4xuso6V3HoluqKOoGb74fcE1YWti3vkI,4470
-datarobot_bosun-9.1.1b1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-datarobot_bosun-9.1.1b1.dist-info/top_level.txt,sha256=zNJvGsG32_zF72Xl_00PTybDZE3u5FXDSxJiFEekRd4,6
-datarobot_bosun-9.1.1b1.dist-info/RECORD,,
+datarobot_bosun-9.1.1rc1.data/scripts/bosun-plugin-runner,sha256=e8YQBceK8QeD8EFh1q5Vb-jlAYxlrzvZllDq3LNnVPg,671
+datarobot_bosun-9.1.1rc1.data/scripts/mcrunner,sha256=FPqMPz123TVvMrWf1bBsu17RSoJJwXA0-M9EG5IdpXg,676
+datarobot_bosun-9.1.1rc1.data/scripts/plugin-runner,sha256=pe1lGnDyvW82cBjewuRhb6ad6q3j4TYEJLurzG6GNdk,671
+datarobot_bosun-9.1.1rc1.dist-info/METADATA,sha256=BI-jmSlV9Qpw4mbjZsfspWwsBxyP2hccV9_htvisUJw,4471
+datarobot_bosun-9.1.1rc1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+datarobot_bosun-9.1.1rc1.dist-info/top_level.txt,sha256=zNJvGsG32_zF72Xl_00PTybDZE3u5FXDSxJiFEekRd4,6
+datarobot_bosun-9.1.1rc1.dist-info/RECORD,,
```

