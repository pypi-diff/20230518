# Comparing `tmp/airlift-0.1.2.tar.gz` & `tmp/airlift-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airlift-0.1.2.tar", max compression
+gzip compressed data, was "airlift-0.1.3.tar", max compression
```

## Comparing `airlift-0.1.2.tar` & `airlift-0.1.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1062 2023-05-15 17:57:39.104413 airlift-0.1.2/LICENSE
--rw-r--r--   0        0        0     6509 2023-05-15 17:57:39.104413 airlift-0.1.2/README.md
--rw-r--r--   0        0        0      673 2023-05-15 17:57:39.116413 airlift-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/commands/__init__.py
--rw-r--r--   0        0        0     1364 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/commands/check.py
--rw-r--r--   0        0        0     1033 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/commands/import_variables.py
--rw-r--r--   0        0        0      939 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/commands/pause.py
--rw-r--r--   0        0        0     1161 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/commands/remove.py
--rw-r--r--   0        0        0     1146 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/commands/run_dag.py
--rw-r--r--   0        0        0     6709 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/commands/start.py
--rw-r--r--   0        0        0     1179 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/commands/status.py
--rw-r--r--   0        0        0        0 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/config/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/config/airlift/config.yaml
--rw-r--r--   0        0        0       71 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/config/airlift/required_software.yaml
--rw-r--r--   0        0        0      979 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/config/config.py
--rw-r--r--   0        0        0      176 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/config/docker/Dockerfile
--rw-r--r--   0        0        0        0 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/config/docker/final/.gitkeep
--rw-r--r--   0        0        0     1482 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/config/helm/values.yaml
--rw-r--r--   0        0        0      975 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/config/kind/cluster.yaml
--rw-r--r--   0        0        0     3600 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/main.py
--rw-r--r--   0        0        0        0 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/utils/__init__.py
--rw-r--r--   0        0        0     3676 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/utils/airflow.py
--rw-r--r--   0        0        0      767 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/utils/airlift.py
--rw-r--r--   0        0        0      677 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/utils/command.py
--rw-r--r--   0        0        0     1989 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/utils/docker.py
--rw-r--r--   0        0        0     3087 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/utils/file.py
--rw-r--r--   0        0        0     1606 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/utils/helm.py
--rw-r--r--   0        0        0     2306 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/utils/kind.py
--rw-r--r--   0        0        0      815 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/utils/kubernetes.py
--rw-r--r--   0        0        0     8439 2023-05-15 17:57:39.116413 airlift-0.1.2/src/airlift/utils/parser.py
--rw-r--r--   0        0        0     7252 1970-01-01 00:00:00.000000 airlift-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-17 22:01:59.177948 airlift-0.1.3/LICENSE
+-rw-r--r--   0        0        0     6696 2023-05-17 22:01:59.177948 airlift-0.1.3/README.md
+-rw-r--r--   0        0        0      673 2023-05-17 22:01:59.189948 airlift-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-17 22:01:59.189948 airlift-0.1.3/src/airlift/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 22:01:59.189948 airlift-0.1.3/src/airlift/commands/__init__.py
+-rw-r--r--   0        0        0     1364 2023-05-17 22:01:59.189948 airlift-0.1.3/src/airlift/commands/check.py
+-rw-r--r--   0        0        0     1033 2023-05-17 22:01:59.189948 airlift-0.1.3/src/airlift/commands/import_variables.py
+-rw-r--r--   0        0        0      939 2023-05-17 22:01:59.189948 airlift-0.1.3/src/airlift/commands/pause.py
+-rw-r--r--   0        0        0     1161 2023-05-17 22:01:59.189948 airlift-0.1.3/src/airlift/commands/remove.py
+-rw-r--r--   0        0        0     1146 2023-05-17 22:01:59.189948 airlift-0.1.3/src/airlift/commands/run_dag.py
+-rw-r--r--   0        0        0     6709 2023-05-17 22:01:59.189948 airlift-0.1.3/src/airlift/commands/start.py
+-rw-r--r--   0        0        0     1179 2023-05-17 22:01:59.189948 airlift-0.1.3/src/airlift/commands/status.py
+-rw-r--r--   0        0        0        0 2023-05-17 22:01:59.189948 airlift-0.1.3/src/airlift/config/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 22:01:59.189948 airlift-0.1.3/src/airlift/config/airlift/config.yaml
+-rw-r--r--   0        0        0       71 2023-05-17 22:01:59.189948 airlift-0.1.3/src/airlift/config/airlift/required_software.yaml
+-rw-r--r--   0        0        0      979 2023-05-17 22:01:59.189948 airlift-0.1.3/src/airlift/config/config.py
+-rw-r--r--   0        0        0      176 2023-05-17 22:01:59.189948 airlift-0.1.3/src/airlift/config/docker/Dockerfile
+-rw-r--r--   0        0        0        0 2023-05-17 22:01:59.189948 airlift-0.1.3/src/airlift/config/docker/final/.gitkeep
+-rw-r--r--   0        0        0     1836 2023-05-17 22:01:59.189948 airlift-0.1.3/src/airlift/config/helm/values.yaml
+-rw-r--r--   0        0        0      975 2023-05-17 22:01:59.189948 airlift-0.1.3/src/airlift/config/kind/cluster.yaml
+-rw-r--r--   0        0        0     3600 2023-05-17 22:01:59.189948 airlift-0.1.3/src/airlift/main.py
+-rw-r--r--   0        0        0        0 2023-05-17 22:01:59.189948 airlift-0.1.3/src/airlift/utils/__init__.py
+-rw-r--r--   0        0        0     3676 2023-05-17 22:01:59.189948 airlift-0.1.3/src/airlift/utils/airflow.py
+-rw-r--r--   0        0        0      767 2023-05-17 22:01:59.189948 airlift-0.1.3/src/airlift/utils/airlift.py
+-rw-r--r--   0        0        0      677 2023-05-17 22:01:59.189948 airlift-0.1.3/src/airlift/utils/command.py
+-rw-r--r--   0        0        0     1989 2023-05-17 22:01:59.189948 airlift-0.1.3/src/airlift/utils/docker.py
+-rw-r--r--   0        0        0     3087 2023-05-17 22:01:59.189948 airlift-0.1.3/src/airlift/utils/file.py
+-rw-r--r--   0        0        0     1606 2023-05-17 22:01:59.189948 airlift-0.1.3/src/airlift/utils/helm.py
+-rw-r--r--   0        0        0     2306 2023-05-17 22:01:59.189948 airlift-0.1.3/src/airlift/utils/kind.py
+-rw-r--r--   0        0        0      815 2023-05-17 22:01:59.189948 airlift-0.1.3/src/airlift/utils/kubernetes.py
+-rw-r--r--   0        0        0     8439 2023-05-17 22:01:59.189948 airlift-0.1.3/src/airlift/utils/parser.py
+-rw-r--r--   0        0        0     7439 1970-01-01 00:00:00.000000 airlift-0.1.3/PKG-INFO
```

### Comparing `airlift-0.1.2/LICENSE` & `airlift-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `airlift-0.1.2/README.md` & `airlift-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -205,14 +205,16 @@
   command: ~
   # Args to use when running the Airflow scheduler (templated).
   args: ["bash", "-c", "exec airflow scheduler"]
 ```
 
 You can find all the possible configuration overrides here: <https://artifacthub.io/packages/helm/apache-airflow/airflow?modal=values>
 
+Note: By default, we disable the `livenessProbe` checks for the scheduler & triggerer due to conflicts with Kind. See `./src/airlift/config/helm/values.yaml` for the exact config values
+
 #### Airlift Configuration
 
 The Airlift configuration file overrides all flag values to simplify starting the service.
 
 For example, `$HOME/.config/airlift/config.yaml`:
 
 ```yaml
```

#### html2text {}

```diff
@@ -53,26 +53,28 @@
 timeoutSeconds: 20 failureThreshold: 5 periodSeconds: 60 command: ~ # Airflow
 2.0 allows users to run multiple schedulers, # However this feature is only
 recommended for MySQL 8+ and Postgres replicas: 1 # Max number of old
 replicasets to retain revisionHistoryLimit: ~ # Command to use when running the
 Airflow scheduler (templated). command: ~ # Args to use when running the
 Airflow scheduler (templated). args: ["bash", "-c", "exec airflow scheduler"]
 ``` You can find all the possible configuration overrides here:
-artifacthub.io/packages/helm/apache-airflow/airflow?modal=values> #### Airlift
-Configuration The Airlift configuration file overrides all flag values to
-simplify starting the service. For example, `$HOME/.config/airlift/
-config.yaml`: ```yaml # config.yaml dag_path: /path/to/dags plugin_path: /path/
-to/plugins requirements_file: /path/to/requirements.txt helm_values_file: /
-path/to/values.yaml airlift_config_file: /path/to/airlift/config.yaml
-extra_volume_mounts: - hostPath=/my/cool/path,containerPath=/my/mounted/
-path,name=a_unique_name cluster_config_file: /path/to/cluster/config.yaml
-image: 'apache/airflow:2.6.0' helm_chart_version: '1.0.0' port: 8080
-post_start_dag_id: 'example_dag_id' ``` In this example, `dag_path` in the yaml
-file overrides the `-d` setting, `plugin_path` overrides the `-p` setting, and
-so forth. Using this configuration, you can now start the service using:
+artifacthub.io/packages/helm/apache-airflow/airflow?modal=values> Note: By
+default, we disable the `livenessProbe` checks for the scheduler & triggerer
+due to conflicts with Kind. See `./src/airlift/config/helm/values.yaml` for the
+exact config values #### Airlift Configuration The Airlift configuration file
+overrides all flag values to simplify starting the service. For example,
+`$HOME/.config/airlift/config.yaml`: ```yaml # config.yaml dag_path: /path/to/
+dags plugin_path: /path/to/plugins requirements_file: /path/to/requirements.txt
+helm_values_file: /path/to/values.yaml airlift_config_file: /path/to/airlift/
+config.yaml extra_volume_mounts: - hostPath=/my/cool/path,containerPath=/my/
+mounted/path,name=a_unique_name cluster_config_file: /path/to/cluster/
+config.yaml image: 'apache/airflow:2.6.0' helm_chart_version: '1.0.0' port:
+8080 post_start_dag_id: 'example_dag_id' ``` In this example, `dag_path` in the
+yaml file overrides the `-d` setting, `plugin_path` overrides the `-p` setting,
+and so forth. Using this configuration, you can now start the service using:
 ```bash airlift start -c $HOME/.config/airlift/config.yaml ``` ## Examples [See
 here for examples with common configuration modifications.](./docs/examples/
 ) ## FAQ [See here for Frequently Asked Questions](./docs/faq.md) ## Motivation
 The motivation behind the creation of Airlift is to simplify the process of
 setting up a local development environment for Apache Airflow. It aims to be a
 flexible tool that allows developers to easily configure and manage their
 Airflow instances with unlimited flexibility. ## Support and Contribution If
```

### Comparing `airlift-0.1.2/pyproject.toml` & `airlift-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "airlift"
-version = "0.1.2"
+version = "0.1.3"
 description = "A CLI for creating a flexible Apache Airflow local development environment"
 authors = ["jered.little <jeredlittle1996@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "airlift", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `airlift-0.1.2/src/airlift/commands/check.py` & `airlift-0.1.3/src/airlift/commands/check.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.2/src/airlift/commands/import_variables.py` & `airlift-0.1.3/src/airlift/commands/import_variables.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.2/src/airlift/commands/pause.py` & `airlift-0.1.3/src/airlift/commands/pause.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.2/src/airlift/commands/remove.py` & `airlift-0.1.3/src/airlift/commands/remove.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.2/src/airlift/commands/run_dag.py` & `airlift-0.1.3/src/airlift/commands/run_dag.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.2/src/airlift/commands/start.py` & `airlift-0.1.3/src/airlift/commands/start.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.2/src/airlift/commands/status.py` & `airlift-0.1.3/src/airlift/commands/status.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.2/src/airlift/config/config.py` & `airlift-0.1.3/src/airlift/config/config.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.2/src/airlift/config/helm/values.yaml` & `airlift-0.1.3/src/airlift/config/helm/values.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -20,16 +20,30 @@
   enabled: false
 pgbouncer:
   enabled: false
 workers:
   resources:
     limits:
       memory: 128Mi
+triggerer:
+  livenessProbe:
+    command:
+      - sh
+      - -c
+      - |
+        CONNECTION_CHECK_MAX_COUNT=0 AIRFLOW__LOGGING__LOGGING_LEVEL=ERROR exec /entrypoint \
+        airflow version
 scheduler:
   livenessProbe:
+    command:
+      - sh
+      - -c
+      - |
+        CONNECTION_CHECK_MAX_COUNT=0 AIRFLOW__LOGGING__LOGGING_LEVEL=ERROR exec /entrypoint \
+        airflow version
     initialDelaySeconds: 60
     timeoutSeconds: 120
     failureThreshold: 10
     periodSeconds: 120
   extraVolumes:
     - name: dags
       hostPath:
```

### Comparing `airlift-0.1.2/src/airlift/config/kind/cluster.yaml` & `airlift-0.1.3/src/airlift/config/kind/cluster.yaml`

 * *Files identical despite different names*

### Comparing `airlift-0.1.2/src/airlift/main.py` & `airlift-0.1.3/src/airlift/main.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.2/src/airlift/utils/airflow.py` & `airlift-0.1.3/src/airlift/utils/airflow.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.2/src/airlift/utils/airlift.py` & `airlift-0.1.3/src/airlift/utils/airlift.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.2/src/airlift/utils/command.py` & `airlift-0.1.3/src/airlift/utils/command.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.2/src/airlift/utils/docker.py` & `airlift-0.1.3/src/airlift/utils/docker.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.2/src/airlift/utils/file.py` & `airlift-0.1.3/src/airlift/utils/file.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.2/src/airlift/utils/helm.py` & `airlift-0.1.3/src/airlift/utils/helm.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.2/src/airlift/utils/kind.py` & `airlift-0.1.3/src/airlift/utils/kind.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.2/src/airlift/utils/kubernetes.py` & `airlift-0.1.3/src/airlift/utils/kubernetes.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.2/src/airlift/utils/parser.py` & `airlift-0.1.3/src/airlift/utils/parser.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.2/PKG-INFO` & `airlift-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airlift
-Version: 0.1.2
+Version: 0.1.3
 Summary: A CLI for creating a flexible Apache Airflow local development environment
 Author: jered.little
 Author-email: jeredlittle1996@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -225,14 +225,16 @@
   command: ~
   # Args to use when running the Airflow scheduler (templated).
   args: ["bash", "-c", "exec airflow scheduler"]
 ```
 
 You can find all the possible configuration overrides here: <https://artifacthub.io/packages/helm/apache-airflow/airflow?modal=values>
 
+Note: By default, we disable the `livenessProbe` checks for the scheduler & triggerer due to conflicts with Kind. See `./src/airlift/config/helm/values.yaml` for the exact config values
+
 #### Airlift Configuration
 
 The Airlift configuration file overrides all flag values to simplify starting the service.
 
 For example, `$HOME/.config/airlift/config.yaml`:
 
 ```yaml
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: airlift Version: 0.1.2 Summary: A CLI for creating
+Metadata-Version: 2.1 Name: airlift Version: 0.1.3 Summary: A CLI for creating
 a flexible Apache Airflow local development environment Author: jered.little
 Author-email: jeredlittle1996@gmail.com Requires-Python: >=3.9,<4.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: argparse (>=1.4.0,<2.0.0)
 Requires-Dist: dotmap (>=1.3.30,<2.0.0) Requires-Dist: halo (>=0.0.31,<0.0.32)
 Requires-Dist: hiyapyco (>=0.5.1,<0.6.0) Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
@@ -63,26 +63,28 @@
 timeoutSeconds: 20 failureThreshold: 5 periodSeconds: 60 command: ~ # Airflow
 2.0 allows users to run multiple schedulers, # However this feature is only
 recommended for MySQL 8+ and Postgres replicas: 1 # Max number of old
 replicasets to retain revisionHistoryLimit: ~ # Command to use when running the
 Airflow scheduler (templated). command: ~ # Args to use when running the
 Airflow scheduler (templated). args: ["bash", "-c", "exec airflow scheduler"]
 ``` You can find all the possible configuration overrides here:
-artifacthub.io/packages/helm/apache-airflow/airflow?modal=values> #### Airlift
-Configuration The Airlift configuration file overrides all flag values to
-simplify starting the service. For example, `$HOME/.config/airlift/
-config.yaml`: ```yaml # config.yaml dag_path: /path/to/dags plugin_path: /path/
-to/plugins requirements_file: /path/to/requirements.txt helm_values_file: /
-path/to/values.yaml airlift_config_file: /path/to/airlift/config.yaml
-extra_volume_mounts: - hostPath=/my/cool/path,containerPath=/my/mounted/
-path,name=a_unique_name cluster_config_file: /path/to/cluster/config.yaml
-image: 'apache/airflow:2.6.0' helm_chart_version: '1.0.0' port: 8080
-post_start_dag_id: 'example_dag_id' ``` In this example, `dag_path` in the yaml
-file overrides the `-d` setting, `plugin_path` overrides the `-p` setting, and
-so forth. Using this configuration, you can now start the service using:
+artifacthub.io/packages/helm/apache-airflow/airflow?modal=values> Note: By
+default, we disable the `livenessProbe` checks for the scheduler & triggerer
+due to conflicts with Kind. See `./src/airlift/config/helm/values.yaml` for the
+exact config values #### Airlift Configuration The Airlift configuration file
+overrides all flag values to simplify starting the service. For example,
+`$HOME/.config/airlift/config.yaml`: ```yaml # config.yaml dag_path: /path/to/
+dags plugin_path: /path/to/plugins requirements_file: /path/to/requirements.txt
+helm_values_file: /path/to/values.yaml airlift_config_file: /path/to/airlift/
+config.yaml extra_volume_mounts: - hostPath=/my/cool/path,containerPath=/my/
+mounted/path,name=a_unique_name cluster_config_file: /path/to/cluster/
+config.yaml image: 'apache/airflow:2.6.0' helm_chart_version: '1.0.0' port:
+8080 post_start_dag_id: 'example_dag_id' ``` In this example, `dag_path` in the
+yaml file overrides the `-d` setting, `plugin_path` overrides the `-p` setting,
+and so forth. Using this configuration, you can now start the service using:
 ```bash airlift start -c $HOME/.config/airlift/config.yaml ``` ## Examples [See
 here for examples with common configuration modifications.](./docs/examples/
 ) ## FAQ [See here for Frequently Asked Questions](./docs/faq.md) ## Motivation
 The motivation behind the creation of Airlift is to simplify the process of
 setting up a local development environment for Apache Airflow. It aims to be a
 flexible tool that allows developers to easily configure and manage their
 Airflow instances with unlimited flexibility. ## Support and Contribution If
```

