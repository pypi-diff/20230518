# Comparing `tmp/phidata-1.6.3.tar.gz` & `tmp/phidata-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phidata-1.6.3.tar", last modified: Mon May  8 13:04:37 2023, max compression
+gzip compressed data, was "phidata-1.6.4.tar", last modified: Wed May 17 22:37:04 2023, max compression
```

## Comparing `phidata-1.6.3.tar` & `phidata-1.6.4.tar`

### file list

```diff
@@ -1,510 +1,513 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.872171 phidata-1.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-05-08 13:04:18.000000 phidata-1.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-08 13:04:37.872171 phidata-1.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-08 13:04:18.000000 phidata-1.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.820170 phidata-1.6.3/phidata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.820170 phidata-1.6.3/phidata/airflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/airflow/airflow_installed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.820170 phidata-1.6.3/phidata/airflow/operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/airflow/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/airflow/operators/empty.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.820170 phidata-1.6.3/phidata/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.820170 phidata-1.6.3/phidata/app/airflow/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   100927 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/airflow/airflow_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    30469 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/airflow/airflow_flower.py
--rw-r--r--   0 runner    (1001) docker     (123)    30508 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/airflow/airflow_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    30505 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/airflow/airflow_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    30515 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/airflow/airflow_webserver.py
--rw-r--r--   0 runner    (1001) docker     (123)    30710 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/airflow/airflow_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.820170 phidata-1.6.3/phidata/app/alertmanager/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/alertmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47889 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/alertmanager/alertmanager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.824170 phidata-1.6.3/phidata/app/amundsen/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/amundsen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48031 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/amundsen/frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    48032 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/amundsen/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    47944 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/amundsen/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.824170 phidata-1.6.3/phidata/app/assistant/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49912 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/assistant/assistant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.824170 phidata-1.6.3/phidata/app/cadvisor/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/cadvisor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49678 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/cadvisor/cadvisor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.824170 phidata-1.6.3/phidata/app/databox/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/databox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    86151 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/databox/databox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.824170 phidata-1.6.3/phidata/app/db/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/db/base_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.824170 phidata-1.6.3/phidata/app/elastic/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/elastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/elastic/elastic_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.824170 phidata-1.6.3/phidata/app/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48675 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/elasticsearch/elasticsearch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.824170 phidata-1.6.3/phidata/app/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18446 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/fastapi/fastapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.824170 phidata-1.6.3/phidata/app/grafana/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/grafana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49781 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/grafana/grafana.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.824170 phidata-1.6.3/phidata/app/jupyter/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46942 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/jupyter/jupyter_hub.py
--rw-r--r--   0 runner    (1001) docker     (123)    93432 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/jupyter/jupyter_lab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.824170 phidata-1.6.3/phidata/app/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/k8s/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/k8s/dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/k8s/url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.828170 phidata-1.6.3/phidata/app/mysql/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49110 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/mysql/mysql_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.828170 phidata-1.6.3/phidata/app/neo4j/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/neo4j/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47856 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/neo4j/neo4j.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.828170 phidata-1.6.3/phidata/app/nodeexporter/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/nodeexporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47898 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/nodeexporter/nodeexporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    29897 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/phidata_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.828170 phidata-1.6.3/phidata/app/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53156 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/postgres/postgres_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.828170 phidata-1.6.3/phidata/app/prometheus/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/prometheus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49051 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/prometheus/prometheus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.828170 phidata-1.6.3/phidata/app/redis/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49058 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/redis/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)    53296 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/redis/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.828170 phidata-1.6.3/phidata/app/server/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18427 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/server/api_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    58724 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/server/server_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.828170 phidata-1.6.3/phidata/app/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49424 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/spark/spark_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17222 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/spark/spark_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    17332 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/spark/spark_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.828170 phidata-1.6.3/phidata/app/streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18445 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/streamlit/streamlit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.832170 phidata-1.6.3/phidata/app/superset/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/superset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71570 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/superset/superset_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    22925 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/superset/superset_init.py
--rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/superset/superset_webserver.py
--rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/superset/superset_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    22917 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/superset/superset_worker_beat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.832170 phidata-1.6.3/phidata/app/traefik/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/traefik/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   115905 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/traefik/crds.py
--rw-r--r--   0 runner    (1001) docker     (123)    48190 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/traefik/ingress_route.py
--rw-r--r--   0 runner    (1001) docker     (123)    44972 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/traefik/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.832170 phidata-1.6.3/phidata/asset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/asset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.832170 phidata-1.6.3/phidata/asset/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/asset/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/asset/aws/aws_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/asset/data_asset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.832170 phidata-1.6.3/phidata/asset/local/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/asset/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14564 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/asset/local/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/asset/local/local_asset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.832170 phidata-1.6.3/phidata/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.832170 phidata-1.6.3/phidata/aws/athena/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/athena/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.832170 phidata-1.6.3/phidata/aws/create/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/create/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.832170 phidata-1.6.3/phidata/aws/create/iam/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/create/iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/create/iam/eks_admin_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/create/iam/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.836170 phidata-1.6.3/phidata/aws/enums/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/enums/manager_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.836170 phidata-1.6.3/phidata/aws/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.836170 phidata-1.6.3/phidata/aws/resource/acm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/acm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10630 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/acm/certificate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.836170 phidata-1.6.3/phidata/aws/resource/athena/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/athena/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.836170 phidata-1.6.3/phidata/aws/resource/cloudformation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/cloudformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10882 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/cloudformation/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.836170 phidata-1.6.3/phidata/aws/resource/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/ec2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/ec2/subnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/ec2/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.836170 phidata-1.6.3/phidata/aws/resource/ecs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/ecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/ecs/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    23286 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/ecs/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    16709 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/ecs/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    19957 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/ecs/task_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/ecs/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.836170 phidata-1.6.3/phidata/aws/resource/eks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/eks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/eks/addon.py
--rw-r--r--   0 runner    (1001) docker     (123)    30104 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/eks/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    13731 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/eks/fargate_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    23785 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/eks/kubeconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    23742 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/eks/node_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.840170 phidata-1.6.3/phidata/aws/resource/elasticache/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/elasticache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15043 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/elasticache/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/elasticache/subnet_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.840170 phidata-1.6.3/phidata/aws/resource/elb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/elb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/elb/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/elb/load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/elb/target_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.840170 phidata-1.6.3/phidata/aws/resource/emr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/emr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12777 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/emr/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.840170 phidata-1.6.3/phidata/aws/resource/glue/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12850 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/glue/crawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.840170 phidata-1.6.3/phidata/aws/resource/iam/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/iam/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/iam/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9828 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/iam/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.840170 phidata-1.6.3/phidata/aws/resource/rds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/rds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27957 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/rds/db_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    22247 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/rds/db_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/rds/db_subnet_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.840170 phidata-1.6.3/phidata/aws/resource/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/s3/bucket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.840170 phidata-1.6.3/phidata/aws/resource/secret/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/secret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/secret/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10585 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.844170 phidata-1.6.3/phidata/aws/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21797 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/s3/csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    24100 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/s3/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14394 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/s3/dataset_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/s3/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    22406 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.844170 phidata-1.6.3/phidata/checks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/checks/check.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/checks/not_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.844170 phidata-1.6.3/phidata/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/decorators/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/decorators/validate_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.844170 phidata-1.6.3/phidata/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/docker/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/docker/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/docker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/docker/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/docker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/docker/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.844170 phidata-1.6.3/phidata/docker/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/docker/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/docker/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15539 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/docker/resource/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/docker/resource/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    12126 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/docker/resource/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/docker/resource/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/docker/resource/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/docker/resource/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/docker/resource/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.844170 phidata-1.6.3/phidata/docker/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/docker/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/docker/utils/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    24179 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/docker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.844170 phidata-1.6.3/phidata/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/exceptions/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/exceptions/task.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/exceptions/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.848170 phidata-1.6.3/phidata/infra/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/infra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/infra/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/infra/args.py
--rw-r--r--   0 runner    (1001) docker     (123)    15393 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/infra/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8228 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/infra/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.848170 phidata-1.6.3/phidata/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.848170 phidata-1.6.3/phidata/k8s/create/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.848170 phidata-1.6.3/phidata/k8s/create/apiextensions_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/apiextensions_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.848170 phidata-1.6.3/phidata/k8s/create/apiextensions_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/apiextensions_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.848170 phidata-1.6.3/phidata/k8s/create/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.848170 phidata-1.6.3/phidata/k8s/create/apps/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/apps/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/apps/v1/deployment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.848170 phidata-1.6.3/phidata/k8s/create/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/common/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/common/port.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.848170 phidata-1.6.3/phidata/k8s/create/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.852170 phidata-1.6.3/phidata/k8s/create/core/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/core/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/core/v1/config_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/core/v1/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/core/v1/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/core/v1/persistent_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/core/v1/persistent_volume_claim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/core/v1/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/core/v1/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/core/v1/service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/core/v1/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.852170 phidata-1.6.3/phidata/k8s/create/crb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/crb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/crb/eks_admin_crb.py
--rw-r--r--   0 runner    (1001) docker     (123)    19062 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/kubeconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.852170 phidata-1.6.3/phidata/k8s/create/networking_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/networking_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.852170 phidata-1.6.3/phidata/k8s/create/networking_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/networking_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/networking_k8s_io/v1/ingress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.852170 phidata-1.6.3/phidata/k8s/create/rbac_authorization_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/rbac_authorization_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.852170 phidata-1.6.3/phidata/k8s/create/rbac_authorization_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/rbac_authorization_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.852170 phidata-1.6.3/phidata/k8s/create/storage_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/storage_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.852170 phidata-1.6.3/phidata/k8s/create/storage_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/storage_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/storage_k8s_io/v1/storage_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.852170 phidata-1.6.3/phidata/k8s/enums/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/enums/api_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/enums/api_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/enums/image_pull_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/enums/kind.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/enums/manager_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/enums/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/enums/pv.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/enums/restart_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/enums/service_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/enums/storage_class.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/enums/volume_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.856170 phidata-1.6.3/phidata/k8s/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.856170 phidata-1.6.3/phidata/k8s/resource/apiextensions_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/apiextensions_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.856170 phidata-1.6.3/phidata/k8s/resource/apiextensions_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/apiextensions_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    15390 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.856170 phidata-1.6.3/phidata/k8s/resource/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.856170 phidata-1.6.3/phidata/k8s/resource/apps/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/apps/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/apps/v1/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/apps/v1/deployment_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.856170 phidata-1.6.3/phidata/k8s/resource/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.860170 phidata-1.6.3/phidata/k8s/resource/core/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/config_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    18530 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/local_object_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/node_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/object_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/persistent_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/persistent_volume_claim.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/pod.py
--rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/pod_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/pod_template_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/resource_requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    18982 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/toleration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/topology_spread_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/volume.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/volume_node_affinity.py
--rw-r--r--   0 runner    (1001) docker     (123)    13397 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/volume_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    13385 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/kubeconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.860170 phidata-1.6.3/phidata/k8s/resource/meta/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.860170 phidata-1.6.3/phidata/k8s/resource/meta/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/meta/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/meta/v1/label_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/meta/v1/object_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.860170 phidata-1.6.3/phidata/k8s/resource/networking_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/networking_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.860170 phidata-1.6.3/phidata/k8s/resource/networking_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/networking_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10026 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/networking_k8s_io/v1/ingress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.860170 phidata-1.6.3/phidata/k8s/resource/rbac_authorization_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/rbac_authorization_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.860170 phidata-1.6.3/phidata/k8s/resource/rbac_authorization_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/rbac_authorization_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.860170 phidata-1.6.3/phidata/k8s/resource/storage_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/storage_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.860170 phidata-1.6.3/phidata/k8s/resource/storage_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/storage_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    12678 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.860170 phidata-1.6.3/phidata/k8s/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/utils/pod.py
--rw-r--r--   0 runner    (1001) docker     (123)    43059 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.860170 phidata-1.6.3/phidata/llm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/llm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.860170 phidata-1.6.3/phidata/llm/duckdb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/llm/duckdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/llm/duckdb/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/llm/duckdb/chain.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/llm/duckdb/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/llm/duckdb/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/llm/duckdb/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/llm/duckdb/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.860170 phidata-1.6.3/phidata/product/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/product/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29505 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/product/data_product.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.860170 phidata-1.6.3/phidata/table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.860170 phidata-1.6.3/phidata/table/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/table/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/table/local/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    23516 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/table/local/local_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/table/local/parquet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.864170 phidata-1.6.3/phidata/table/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/table/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/table/s3/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/table/s3/parquet.py
--rw-r--r--   0 runner    (1001) docker     (123)    23064 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/table/s3/s3_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.864170 phidata-1.6.3/phidata/table/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/table/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/table/sql/postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)    35497 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/table/sql/sql_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.864170 phidata-1.6.3/phidata/task/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.864170 phidata-1.6.3/phidata/task/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.864170 phidata-1.6.3/phidata/task/aws/athena/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/aws/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/aws/athena/run_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.864170 phidata-1.6.3/phidata/task/aws/emr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/aws/emr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/aws/emr/create_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/aws/emr/delete_cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.864170 phidata-1.6.3/phidata/task/aws/glue/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/aws/glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/aws/glue/start_crawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.864170 phidata-1.6.3/phidata/task/dev/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/dev/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.864170 phidata-1.6.3/phidata/task/download/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/download/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.864170 phidata-1.6.3/phidata/task/download/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/download/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/download/s3/to_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.864170 phidata-1.6.3/phidata/task/download/url/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/download/url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/download/url/to_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/download/url/to_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/download/url/to_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.864170 phidata-1.6.3/phidata/task/plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/plot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.864170 phidata-1.6.3/phidata/task/plot/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/plot/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/plot/sql/query.py
--rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/python_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.868171 phidata-1.6.3/phidata/task/run/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/run/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.868171 phidata-1.6.3/phidata/task/run/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/run/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/run/sql/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/task_relatives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.868171 phidata-1.6.3/phidata/task/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.868171 phidata-1.6.3/phidata/task/upload/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/upload/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/upload/file/to_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/upload/file/to_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.868171 phidata-1.6.3/phidata/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/types/airflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/types/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/types/phidata_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/types/run_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.868171 phidata-1.6.3/phidata/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/utils/cli_console.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/utils/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/utils/dttm.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/utils/env_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/utils/env_var.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/utils/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/utils/prep_infra_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/utils/print_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/utils/workspace_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.868171 phidata-1.6.3/phidata/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/workflow/decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.868171 phidata-1.6.3/phidata/workflow/dev/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/workflow/dev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42342 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/workflow/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/workflow/workflow_relatives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.872171 phidata-1.6.3/phidata/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/workspace/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/workspace/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.820170 phidata-1.6.3/phidata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-08 13:04:37.000000 phidata-1.6.3/phidata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13440 2023-05-08 13:04:37.000000 phidata-1.6.3/phidata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 13:04:37.000000 phidata-1.6.3/phidata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-08 13:04:37.000000 phidata-1.6.3/phidata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-08 13:04:37.000000 phidata-1.6.3/phidata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-08 13:04:18.000000 phidata-1.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 13:04:37.872171 phidata-1.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-08 13:04:18.000000 phidata-1.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.872171 phidata-1.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-08 13:04:18.000000 phidata-1.6.3/tests/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.217665 phidata-1.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-05-17 22:36:43.000000 phidata-1.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-17 22:37:04.213665 phidata-1.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-17 22:36:43.000000 phidata-1.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.161666 phidata-1.6.4/phidata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.161666 phidata-1.6.4/phidata/airflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/airflow/airflow_installed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.161666 phidata-1.6.4/phidata/airflow/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/airflow/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/airflow/operators/empty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.161666 phidata-1.6.4/phidata/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.165666 phidata-1.6.4/phidata/app/airflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100927 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/airflow/airflow_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30469 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/airflow/airflow_flower.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30508 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/airflow/airflow_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30505 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/airflow/airflow_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30515 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/airflow/airflow_webserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30710 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/airflow/airflow_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.165666 phidata-1.6.4/phidata/app/alertmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/alertmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47889 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/alertmanager/alertmanager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.165666 phidata-1.6.4/phidata/app/amundsen/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/amundsen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48031 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/amundsen/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48032 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/amundsen/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47944 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/amundsen/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.165666 phidata-1.6.4/phidata/app/assistant/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49912 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/assistant/assistant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.165666 phidata-1.6.4/phidata/app/cadvisor/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/cadvisor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49678 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/cadvisor/cadvisor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.165666 phidata-1.6.4/phidata/app/databox/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/databox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86151 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/databox/databox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.169666 phidata-1.6.4/phidata/app/db/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/db/base_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.169666 phidata-1.6.4/phidata/app/django/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30078 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/django/django_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.169666 phidata-1.6.4/phidata/app/elastic/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/elastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/elastic/elastic_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.169666 phidata-1.6.4/phidata/app/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48675 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/elasticsearch/elasticsearch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.169666 phidata-1.6.4/phidata/app/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18446 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/fastapi/fastapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.169666 phidata-1.6.4/phidata/app/grafana/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/grafana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49781 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/grafana/grafana.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.169666 phidata-1.6.4/phidata/app/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46942 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/jupyter/jupyter_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93432 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/jupyter/jupyter_lab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.173666 phidata-1.6.4/phidata/app/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/k8s/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/k8s/dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/k8s/url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.173666 phidata-1.6.4/phidata/app/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49110 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/mysql/mysql_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.173666 phidata-1.6.4/phidata/app/neo4j/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/neo4j/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47856 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/neo4j/neo4j.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.173666 phidata-1.6.4/phidata/app/nodeexporter/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/nodeexporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47898 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/nodeexporter/nodeexporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37941 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/phidata_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.173666 phidata-1.6.4/phidata/app/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53156 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/postgres/postgres_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.173666 phidata-1.6.4/phidata/app/prometheus/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/prometheus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49051 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/prometheus/prometheus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.173666 phidata-1.6.4/phidata/app/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49058 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/redis/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53296 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/redis/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.173666 phidata-1.6.4/phidata/app/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18427 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/server/api_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58717 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/server/server_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.177666 phidata-1.6.4/phidata/app/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49424 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/spark/spark_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17222 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/spark/spark_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17332 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/spark/spark_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.177666 phidata-1.6.4/phidata/app/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18445 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/streamlit/streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.177666 phidata-1.6.4/phidata/app/superset/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/superset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71570 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/superset/superset_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22925 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/superset/superset_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/superset/superset_webserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/superset/superset_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22917 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/superset/superset_worker_beat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.177666 phidata-1.6.4/phidata/app/traefik/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/traefik/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115905 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/traefik/crds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48190 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/traefik/ingress_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44972 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/app/traefik/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.181666 phidata-1.6.4/phidata/asset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/asset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.181666 phidata-1.6.4/phidata/asset/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/asset/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/asset/aws/aws_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/asset/data_asset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.181666 phidata-1.6.4/phidata/asset/local/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/asset/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14564 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/asset/local/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/asset/local/local_asset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.181666 phidata-1.6.4/phidata/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.181666 phidata-1.6.4/phidata/aws/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/athena/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.181666 phidata-1.6.4/phidata/aws/create/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/create/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.181666 phidata-1.6.4/phidata/aws/create/iam/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/create/iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/create/iam/eks_admin_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/create/iam/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.181666 phidata-1.6.4/phidata/aws/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/enums/manager_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.181666 phidata-1.6.4/phidata/aws/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.181666 phidata-1.6.4/phidata/aws/resource/acm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/acm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10630 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/acm/certificate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.181666 phidata-1.6.4/phidata/aws/resource/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/athena/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.181666 phidata-1.6.4/phidata/aws/resource/cloudformation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/cloudformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10882 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/cloudformation/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.185666 phidata-1.6.4/phidata/aws/resource/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/ec2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/ec2/subnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/ec2/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.185666 phidata-1.6.4/phidata/aws/resource/ecs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/ecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/ecs/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23286 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/ecs/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16709 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/ecs/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20858 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/ecs/task_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/ecs/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.185666 phidata-1.6.4/phidata/aws/resource/eks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/eks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/eks/addon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30104 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/eks/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13731 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/eks/fargate_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23785 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/eks/kubeconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23742 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/eks/node_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.185666 phidata-1.6.4/phidata/aws/resource/elasticache/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/elasticache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15043 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/elasticache/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/elasticache/subnet_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.185666 phidata-1.6.4/phidata/aws/resource/elb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/elb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/elb/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/elb/load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/elb/target_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.185666 phidata-1.6.4/phidata/aws/resource/emr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/emr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12777 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/emr/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.185666 phidata-1.6.4/phidata/aws/resource/glue/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12850 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/glue/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.185666 phidata-1.6.4/phidata/aws/resource/iam/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/iam/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/iam/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9828 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/iam/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.185666 phidata-1.6.4/phidata/aws/resource/rds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/rds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27957 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/rds/db_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22247 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/rds/db_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/rds/db_subnet_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.189666 phidata-1.6.4/phidata/aws/resource/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/s3/bucket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.189666 phidata-1.6.4/phidata/aws/resource/secret/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/secret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/secret/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10585 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/resource/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.189666 phidata-1.6.4/phidata/aws/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21797 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/s3/csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24100 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/s3/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14394 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/s3/dataset_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/s3/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22406 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/aws/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.189666 phidata-1.6.4/phidata/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/checks/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/checks/not_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.189666 phidata-1.6.4/phidata/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/decorators/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/decorators/validate_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.189666 phidata-1.6.4/phidata/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/docker/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/docker/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/docker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/docker/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/docker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/docker/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.189666 phidata-1.6.4/phidata/docker/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/docker/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/docker/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15539 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/docker/resource/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/docker/resource/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12126 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/docker/resource/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/docker/resource/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/docker/resource/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/docker/resource/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/docker/resource/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.189666 phidata-1.6.4/phidata/docker/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/docker/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/docker/utils/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24179 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/docker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.189666 phidata-1.6.4/phidata/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/exceptions/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/exceptions/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/exceptions/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.193666 phidata-1.6.4/phidata/infra/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/infra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/infra/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/infra/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15393 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/infra/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8228 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/infra/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.193666 phidata-1.6.4/phidata/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.193666 phidata-1.6.4/phidata/k8s/create/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/create/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.193666 phidata-1.6.4/phidata/k8s/create/apiextensions_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/create/apiextensions_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.193666 phidata-1.6.4/phidata/k8s/create/apiextensions_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/create/apiextensions_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.193666 phidata-1.6.4/phidata/k8s/create/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/create/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.193666 phidata-1.6.4/phidata/k8s/create/apps/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/create/apps/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/create/apps/v1/deployment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.193666 phidata-1.6.4/phidata/k8s/create/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/create/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/create/common/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/create/common/port.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.193666 phidata-1.6.4/phidata/k8s/create/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/create/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.197666 phidata-1.6.4/phidata/k8s/create/core/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/create/core/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/create/core/v1/config_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/create/core/v1/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/create/core/v1/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/create/core/v1/persistent_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/create/core/v1/persistent_volume_claim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/create/core/v1/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/create/core/v1/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/create/core/v1/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/create/core/v1/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.197666 phidata-1.6.4/phidata/k8s/create/crb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/create/crb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/create/crb/eks_admin_crb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19062 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/create/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/create/kubeconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.197666 phidata-1.6.4/phidata/k8s/create/networking_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/create/networking_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.197666 phidata-1.6.4/phidata/k8s/create/networking_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/create/networking_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/create/networking_k8s_io/v1/ingress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.197666 phidata-1.6.4/phidata/k8s/create/rbac_authorization_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/create/rbac_authorization_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.197666 phidata-1.6.4/phidata/k8s/create/rbac_authorization_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/create/rbac_authorization_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.197666 phidata-1.6.4/phidata/k8s/create/storage_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/create/storage_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.197666 phidata-1.6.4/phidata/k8s/create/storage_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/create/storage_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/create/storage_k8s_io/v1/storage_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.201665 phidata-1.6.4/phidata/k8s/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/enums/api_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/enums/api_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/enums/image_pull_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/enums/kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/enums/manager_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/enums/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/enums/pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/enums/restart_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/enums/service_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/enums/storage_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/enums/volume_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.201665 phidata-1.6.4/phidata/k8s/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.201665 phidata-1.6.4/phidata/k8s/resource/apiextensions_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/apiextensions_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.201665 phidata-1.6.4/phidata/k8s/resource/apiextensions_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/apiextensions_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15390 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.201665 phidata-1.6.4/phidata/k8s/resource/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.201665 phidata-1.6.4/phidata/k8s/resource/apps/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/apps/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/apps/v1/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/apps/v1/deployment_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.201665 phidata-1.6.4/phidata/k8s/resource/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.205665 phidata-1.6.4/phidata/k8s/resource/core/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/core/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/core/v1/config_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18530 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/core/v1/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/core/v1/local_object_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/core/v1/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/core/v1/node_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/core/v1/object_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/core/v1/persistent_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/core/v1/persistent_volume_claim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/core/v1/pod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/core/v1/pod_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/core/v1/pod_template_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/core/v1/resource_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/core/v1/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18982 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/core/v1/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/core/v1/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/core/v1/toleration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/core/v1/topology_spread_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/core/v1/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/core/v1/volume_node_affinity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13397 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/core/v1/volume_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13385 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/kubeconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.205665 phidata-1.6.4/phidata/k8s/resource/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.205665 phidata-1.6.4/phidata/k8s/resource/meta/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/meta/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/meta/v1/label_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/meta/v1/object_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.205665 phidata-1.6.4/phidata/k8s/resource/networking_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/networking_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.205665 phidata-1.6.4/phidata/k8s/resource/networking_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/networking_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10026 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/networking_k8s_io/v1/ingress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.205665 phidata-1.6.4/phidata/k8s/resource/rbac_authorization_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/rbac_authorization_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.205665 phidata-1.6.4/phidata/k8s/resource/rbac_authorization_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/rbac_authorization_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.205665 phidata-1.6.4/phidata/k8s/resource/storage_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/storage_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.205665 phidata-1.6.4/phidata/k8s/resource/storage_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/storage_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12678 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/resource/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.205665 phidata-1.6.4/phidata/k8s/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/utils/pod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43059 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/k8s/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.205665 phidata-1.6.4/phidata/llm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/llm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.205665 phidata-1.6.4/phidata/llm/duckdb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/llm/duckdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/llm/duckdb/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/llm/duckdb/chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/llm/duckdb/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/llm/duckdb/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/llm/duckdb/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/llm/duckdb/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.205665 phidata-1.6.4/phidata/product/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/product/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29505 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/product/data_product.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.205665 phidata-1.6.4/phidata/table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.209665 phidata-1.6.4/phidata/table/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/table/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/table/local/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23516 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/table/local/local_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/table/local/parquet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.209665 phidata-1.6.4/phidata/table/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/table/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/table/s3/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/table/s3/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23064 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/table/s3/s3_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.209665 phidata-1.6.4/phidata/table/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/table/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/table/sql/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35497 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/table/sql/sql_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.209665 phidata-1.6.4/phidata/task/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.209665 phidata-1.6.4/phidata/task/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/task/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.209665 phidata-1.6.4/phidata/task/aws/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/task/aws/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/task/aws/athena/run_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.209665 phidata-1.6.4/phidata/task/aws/emr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/task/aws/emr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/task/aws/emr/create_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/task/aws/emr/delete_cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.209665 phidata-1.6.4/phidata/task/aws/glue/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/task/aws/glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/task/aws/glue/start_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/task/decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.209665 phidata-1.6.4/phidata/task/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/task/dev/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.209665 phidata-1.6.4/phidata/task/download/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/task/download/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.209665 phidata-1.6.4/phidata/task/download/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/task/download/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/task/download/s3/to_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.209665 phidata-1.6.4/phidata/task/download/url/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/task/download/url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/task/download/url/to_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/task/download/url/to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/task/download/url/to_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.209665 phidata-1.6.4/phidata/task/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/task/plot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.209665 phidata-1.6.4/phidata/task/plot/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/task/plot/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/task/plot/sql/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/task/python_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.209665 phidata-1.6.4/phidata/task/run/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/task/run/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.213665 phidata-1.6.4/phidata/task/run/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/task/run/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/task/run/sql/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/task/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/task/task_relatives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.213665 phidata-1.6.4/phidata/task/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/task/upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.213665 phidata-1.6.4/phidata/task/upload/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/task/upload/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/task/upload/file/to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/task/upload/file/to_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.213665 phidata-1.6.4/phidata/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/types/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/types/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/types/phidata_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/types/run_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.213665 phidata-1.6.4/phidata/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/utils/cli_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/utils/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/utils/dttm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/utils/env_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/utils/env_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/utils/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/utils/prep_infra_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/utils/print_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/utils/workspace_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.213665 phidata-1.6.4/phidata/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/workflow/decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.213665 phidata-1.6.4/phidata/workflow/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/workflow/dev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42342 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/workflow/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/workflow/workflow_relatives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.213665 phidata-1.6.4/phidata/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/workspace/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-05-17 22:36:43.000000 phidata-1.6.4/phidata/workspace/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.161666 phidata-1.6.4/phidata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-17 22:37:04.000000 phidata-1.6.4/phidata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13504 2023-05-17 22:37:04.000000 phidata-1.6.4/phidata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 22:37:04.000000 phidata-1.6.4/phidata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-17 22:37:04.000000 phidata-1.6.4/phidata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-17 22:37:04.000000 phidata-1.6.4/phidata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-17 22:36:43.000000 phidata-1.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 22:37:04.217665 phidata-1.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-17 22:36:43.000000 phidata-1.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:04.213665 phidata-1.6.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-17 22:36:43.000000 phidata-1.6.4/tests/test_placeholder.py
```

### Comparing `phidata-1.6.3/LICENSE` & `phidata-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/PKG-INFO` & `phidata-1.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phidata
-Version: 1.6.3
+Version: 1.6.4
 Summary: Building blocks for Data Engineering
 Author-email: Ashpreet Bedi <ashpreet@phidata.com>
 Project-URL: homepage, https://www.phidata.com
 Project-URL: documentation, https://www.docs.phidata.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: phidata Version: 1.6.3 Summary: Building blocks for
+Metadata-Version: 2.1 Name: phidata Version: 1.6.4 Summary: Building blocks for
 Data Engineering Author-email: Ashpreet Bedi
 phidata.com> Project-URL: homepage, https://www.phidata.com Project-URL:
 documentation, https://www.docs.phidata.com Requires-Python: >=3.7 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: aws License-
 File: LICENSE
                              ****** phidata ******
                      Building Blocks for Data Engineering
```

### Comparing `phidata-1.6.3/README.md` & `phidata-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/airflow/operators/empty.py` & `phidata-1.6.4/phidata/airflow/operators/empty.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/airflow/airflow_base.py` & `phidata-1.6.4/phidata/app/airflow/airflow_base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/airflow/airflow_flower.py` & `phidata-1.6.4/phidata/app/airflow/airflow_flower.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/airflow/airflow_manager.py` & `phidata-1.6.4/phidata/app/airflow/airflow_manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/airflow/airflow_scheduler.py` & `phidata-1.6.4/phidata/app/airflow/airflow_scheduler.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/airflow/airflow_webserver.py` & `phidata-1.6.4/phidata/app/airflow/airflow_webserver.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/airflow/airflow_worker.py` & `phidata-1.6.4/phidata/app/airflow/airflow_worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/alertmanager/alertmanager.py` & `phidata-1.6.4/phidata/app/alertmanager/alertmanager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/amundsen/frontend.py` & `phidata-1.6.4/phidata/app/amundsen/frontend.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/amundsen/metadata.py` & `phidata-1.6.4/phidata/app/amundsen/metadata.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/amundsen/search.py` & `phidata-1.6.4/phidata/app/amundsen/search.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/assistant/assistant.py` & `phidata-1.6.4/phidata/app/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/cadvisor/cadvisor.py` & `phidata-1.6.4/phidata/app/cadvisor/cadvisor.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/databox/databox.py` & `phidata-1.6.4/phidata/app/databox/databox.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/db/base_db.py` & `phidata-1.6.4/phidata/app/db/base_db.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/elastic/elastic_app.py` & `phidata-1.6.4/phidata/app/elastic/elastic_app.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/elasticsearch/elasticsearch.py` & `phidata-1.6.4/phidata/app/elasticsearch/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/fastapi/fastapi.py` & `phidata-1.6.4/phidata/app/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/grafana/grafana.py` & `phidata-1.6.4/phidata/app/grafana/grafana.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/group.py` & `phidata-1.6.4/phidata/app/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/jupyter/jupyter_hub.py` & `phidata-1.6.4/phidata/app/jupyter/jupyter_hub.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/jupyter/jupyter_lab.py` & `phidata-1.6.4/phidata/app/jupyter/jupyter_lab.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/k8s/app.py` & `phidata-1.6.4/phidata/app/k8s/app.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/k8s/dir.py` & `phidata-1.6.4/phidata/app/k8s/dir.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/k8s/url.py` & `phidata-1.6.4/phidata/app/k8s/url.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/mysql/mysql_db.py` & `phidata-1.6.4/phidata/app/mysql/mysql_db.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/neo4j/neo4j.py` & `phidata-1.6.4/phidata/app/neo4j/neo4j.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/nodeexporter/nodeexporter.py` & `phidata-1.6.4/phidata/app/nodeexporter/nodeexporter.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/phidata_app.py` & `phidata-1.6.4/phidata/app/phidata_app.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from pathlib import Path
 from typing import Optional, Dict, Any, Union, List
 
 from phidata.base import PhidataBase, PhidataBaseArgs
+from phidata.types.context import ContainerPathContext
 from phidata.utils.enums import ExtendedEnum
 from phidata.utils.log import logger
 
 
 class WorkspaceVolumeType(ExtendedEnum):
     HostPath = "HostPath"
     EmptyDir = "EmptyDir"
@@ -62,19 +63,19 @@
     # -*- Debug Mode
     debug_mode: bool = False
 
     # -*- Container Configuration
     # Each PhidataApp has 1 main container and multiple sidecar containers
     # The main container name
     container_name: Optional[str] = None
-    # Overwrite the PYTHONPATH env var
-    # which is usually set to the workspace_root_container_path
+    # Overwrite the PYTHONPATH env var, default: False
+    set_python_path: bool = False
+    # Set the python_path, default: workspace_volume_container_path,
     python_path: Optional[str] = None
     # Add to the PYTHONPATH env var. If python_path is set, this is ignored
-    # Does not overwrite the PYTHONPATH env var - adds to it.
     add_python_path: Optional[str] = None
     # Add labels to the container
     container_labels: Optional[Dict[str, Any]] = None
 
     # Container env passed to the PhidataApp
     # Add env variables to container env
     env: Optional[Dict[str, Any]] = None
@@ -561,20 +562,145 @@
 
         # Update the container env with user provided env
         # this overwrites any existing variables
         if self.args.env is not None and isinstance(self.args.env, dict):
             container_env.update(
                 {k: str(v) for k, v in self.args.env.items() if v is not None}
             )
-        # logger.debug(f"Container env: {container_env}")
 
     ######################################################
     ## Docker functions
     ######################################################
 
+    def get_docker_container_env(
+        self,
+        container_paths: ContainerPathContext,
+        initial_env: Optional[Dict[str, str]] = None,
+    ) -> Dict[str, str]:
+        from phidata.constants import (
+            PYTHONPATH_ENV_VAR,
+            PHIDATA_RUNTIME_ENV_VAR,
+            SCRIPTS_DIR_ENV_VAR,
+            STORAGE_DIR_ENV_VAR,
+            META_DIR_ENV_VAR,
+            PRODUCTS_DIR_ENV_VAR,
+            NOTEBOOKS_DIR_ENV_VAR,
+            WORKFLOWS_DIR_ENV_VAR,
+            WORKSPACE_ROOT_ENV_VAR,
+            WORKSPACE_CONFIG_DIR_ENV_VAR,
+        )
+
+        # Container Environment
+        container_env: Dict[str, str] = initial_env or {}
+        container_env.update(
+            {
+                PHIDATA_RUNTIME_ENV_VAR: "docker",
+                SCRIPTS_DIR_ENV_VAR: container_paths.scripts_dir or "",
+                STORAGE_DIR_ENV_VAR: container_paths.storage_dir or "",
+                META_DIR_ENV_VAR: container_paths.meta_dir or "",
+                PRODUCTS_DIR_ENV_VAR: container_paths.products_dir or "",
+                NOTEBOOKS_DIR_ENV_VAR: container_paths.notebooks_dir or "",
+                WORKFLOWS_DIR_ENV_VAR: container_paths.workflows_dir or "",
+                WORKSPACE_ROOT_ENV_VAR: container_paths.workspace_root or "",
+                WORKSPACE_CONFIG_DIR_ENV_VAR: container_paths.workspace_config_dir
+                or "",
+                "INSTALL_REQUIREMENTS": str(self.args.install_requirements),
+                "REQUIREMENTS_FILE_PATH": container_paths.requirements_file or "",
+                "MOUNT_WORKSPACE": str(self.args.mount_workspace),
+                "PRINT_ENV_ON_LOAD": str(self.args.print_env_on_load),
+            }
+        )
+
+        if self.args.set_python_path:
+            python_path = self.args.python_path
+            if python_path is None:
+                python_path = "{}{}".format(
+                    container_paths.workspace_root,
+                    f":{self.args.add_python_path}"
+                    if self.args.add_python_path
+                    else "",
+                )
+            container_env[PYTHONPATH_ENV_VAR] = python_path
+
+        # Set aws env vars
+        self.set_aws_env_vars(env_dict=container_env)
+
+        # Set container env using env_file, secrets_file or args.env
+        self.set_container_env(container_env=container_env)
+        # logger.debug(f"Container env: {container_env}")
+
+        return container_env
+
+    def get_docker_container_volumes(
+        self, container_paths: ContainerPathContext
+    ) -> Dict[str, dict]:
+        from phidata.utils.common import get_default_volume_name
+
+        # container_volumes is a dictionary which configures the volumes to mount
+        # inside the container. The key is either the host path or a volume name,
+        # and the value is a dictionary with 2 keys:
+        #   bind - The path to mount the volume inside the container
+        #   mode - Either rw to mount the volume read/write, or ro to mount it read-only.
+        # For example:
+        # {
+        #   '/home/user1/': {'bind': '/mnt/vol2', 'mode': 'rw'},
+        #   '/var/www': {'bind': '/mnt/vol1', 'mode': 'ro'}
+        # }
+        container_volumes = self.args.container_volumes_docker or {}
+
+        # Create a volume for the workspace dir
+        if self.args.mount_workspace:
+            workspace_volume_container_path_str = container_paths.workspace_root
+            if (
+                self.args.workspace_volume_type is None
+                or self.args.workspace_volume_type == WorkspaceVolumeType.HostPath
+            ):
+                workspace_volume_host_path = (
+                    self.args.workspace_volume_host_path
+                    or str(self.workspace_root_path)
+                )
+                logger.debug(f"Mounting: {workspace_volume_host_path}")
+                logger.debug(f"\tto: {workspace_volume_container_path_str}")
+                container_volumes[workspace_volume_host_path] = {
+                    "bind": workspace_volume_container_path_str,
+                    "mode": "rw",
+                }
+            elif self.args.workspace_volume_type == WorkspaceVolumeType.EmptyDir:
+                workspace_volume_name = self.args.workspace_volume_name
+                if workspace_volume_name is None:
+                    workspace_volume_name = get_default_volume_name(
+                        container_paths.workspace_name or "ws"
+                    )
+                logger.debug(f"Mounting: {workspace_volume_name}")
+                logger.debug(f"\tto: {workspace_volume_container_path_str}")
+                container_volumes[workspace_volume_name] = {
+                    "bind": workspace_volume_container_path_str,
+                    "mode": "rw",
+                }
+            else:
+                logger.error(f"{self.args.workspace_volume_type.value} not supported")
+
+        return container_volumes
+
+    def get_docker_container_ports(self) -> Dict[str, int]:
+        # container_ports is a dictionary which configures the ports to bind
+        # inside the container. The key is the port to bind inside the container
+        #   either as an integer or a string in the form port/protocol
+        # and the value is the corresponding port to open on the host.
+        # For example:
+        #   {'2222/tcp': 3333} will expose port 2222 inside the container as port 3333 on the host.
+        container_ports: Dict[str, int] = self.args.container_ports_docker or {}
+
+        if self.args.open_container_port:
+            container_ports[
+                str(self.args.container_port)
+            ] = self.args.container_host_port
+
+        return container_ports
+
     def get_container_restart_policy_docker(self) -> Optional[Dict[str, Any]]:
         return self.args.container_restart_policy_docker if self.args else None
 
     def init_docker_resource_groups(self, docker_build_context: Any) -> None:
         logger.debug(f"@init_docker_resource_groups not defined for {self.name}")
 
     def get_docker_resource_groups(
@@ -612,14 +738,73 @@
         #         )
         return self.k8s_resource_groups
 
     ######################################################
     ## AWS functions
     ######################################################
 
+    def get_ecs_container_env(
+        self,
+        container_paths: ContainerPathContext,
+        initial_env: Optional[Dict[str, str]] = None,
+    ) -> Dict[str, str]:
+        from phidata.constants import (
+            PYTHONPATH_ENV_VAR,
+            PHIDATA_RUNTIME_ENV_VAR,
+            SCRIPTS_DIR_ENV_VAR,
+            STORAGE_DIR_ENV_VAR,
+            META_DIR_ENV_VAR,
+            PRODUCTS_DIR_ENV_VAR,
+            NOTEBOOKS_DIR_ENV_VAR,
+            WORKFLOWS_DIR_ENV_VAR,
+            WORKSPACE_ROOT_ENV_VAR,
+            WORKSPACE_CONFIG_DIR_ENV_VAR,
+        )
+
+        # Container Environment
+        container_env: Dict[str, str] = initial_env or {}
+        container_env.update(
+            {
+                PHIDATA_RUNTIME_ENV_VAR: "ecs",
+                SCRIPTS_DIR_ENV_VAR: container_paths.scripts_dir or "",
+                STORAGE_DIR_ENV_VAR: container_paths.storage_dir or "",
+                META_DIR_ENV_VAR: container_paths.meta_dir or "",
+                PRODUCTS_DIR_ENV_VAR: container_paths.products_dir or "",
+                NOTEBOOKS_DIR_ENV_VAR: container_paths.notebooks_dir or "",
+                WORKFLOWS_DIR_ENV_VAR: container_paths.workflows_dir or "",
+                WORKSPACE_ROOT_ENV_VAR: container_paths.workspace_root or "",
+                WORKSPACE_CONFIG_DIR_ENV_VAR: container_paths.workspace_config_dir
+                or "",
+                "INSTALL_REQUIREMENTS": str(self.args.install_requirements),
+                "REQUIREMENTS_FILE_PATH": container_paths.requirements_file or "",
+                "MOUNT_WORKSPACE": str(self.args.mount_workspace),
+                "PRINT_ENV_ON_LOAD": str(self.args.print_env_on_load),
+            }
+        )
+
+        if self.args.set_python_path:
+            python_path = self.args.python_path
+            if python_path is None:
+                python_path = "{}{}".format(
+                    container_paths.workspace_root or "",
+                    f":{self.args.add_python_path}"
+                    if self.args.add_python_path
+                    else "",
+                )
+            container_env[PYTHONPATH_ENV_VAR] = python_path
+
+        # Set aws env vars
+        self.set_aws_env_vars(env_dict=container_env)
+
+        # Set container env using env_file, secrets_file or args.env
+        self.set_container_env(container_env=container_env)
+        # logger.debug(f"Container env: {container_env}")
+
+        return container_env
+
     def init_aws_resource_groups(self, aws_build_context: Any) -> None:
         logger.debug(f"@init_aws_resource_groups not defined for {self.name}")
 
     def get_aws_resource_groups(
         self, aws_build_context: Any
     ) -> Optional[Dict[str, Any]]:
         if self.aws_resource_groups is None:
@@ -634,17 +819,15 @@
                     pass
         return self.aws_resource_groups
 
     ######################################################
     ## Helpers
     ######################################################
 
-    def get_container_paths(
-        self, add_ws_name_to_container_path: bool = True
-    ) -> Optional[Any]:
+    def get_container_paths(self, add_ws_name_to_ws_root: bool = True) -> Optional[Any]:
         if self.workspace_root_path is None:
             return None
 
         workspace_name = self.workspace_root_path.stem
         if workspace_name is None:
             return None
 
@@ -652,15 +835,15 @@
         if workspace_volume_container_path is None:
             return None
 
         from phidata.types.context import ContainerPathContext
 
         workspace_root_container_path = (
             f"{workspace_volume_container_path}/{workspace_name}"
-            if add_ws_name_to_container_path
+            if add_ws_name_to_ws_root
             else workspace_volume_container_path
         )
         container_paths = ContainerPathContext(
             workspace_name=workspace_name,
             workspace_root=workspace_root_container_path,
             workspace_parent=workspace_volume_container_path,
         )
```

### Comparing `phidata-1.6.3/phidata/app/postgres/postgres_db.py` & `phidata-1.6.4/phidata/app/postgres/postgres_db.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/prometheus/prometheus.py` & `phidata-1.6.4/phidata/app/prometheus/prometheus.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/redis/redis.py` & `phidata-1.6.4/phidata/app/redis/redis.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/redis/stack.py` & `phidata-1.6.4/phidata/app/redis/stack.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/server/api_server.py` & `phidata-1.6.4/phidata/app/server/api_server.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/server/server_base.py` & `phidata-1.6.4/phidata/app/server/server_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1103,15 +1103,15 @@
         # Workspace paths
         if self.workspace_root_path is None:
             logger.error("Invalid workspace_root_path")
             return None
 
         workspace_name = self.workspace_root_path.stem
         container_paths: Optional[ContainerPathContext] = self.get_container_paths(
-            add_ws_name_to_container_path=False
+            add_ws_name_to_ws_root=False
         )
         if container_paths is None:
             logger.error("Could not build container paths")
             return None
         logger.debug(f"Container Paths: {container_paths.json(indent=2)}")
 
         # Container pythonpath
```

### Comparing `phidata-1.6.3/phidata/app/spark/spark_base.py` & `phidata-1.6.4/phidata/app/spark/spark_base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/spark/spark_driver.py` & `phidata-1.6.4/phidata/app/spark/spark_driver.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/spark/spark_worker.py` & `phidata-1.6.4/phidata/app/spark/spark_worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/streamlit/streamlit.py` & `phidata-1.6.4/phidata/app/streamlit/streamlit.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/superset/superset_base.py` & `phidata-1.6.4/phidata/app/superset/superset_base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/superset/superset_init.py` & `phidata-1.6.4/phidata/app/superset/superset_init.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/superset/superset_webserver.py` & `phidata-1.6.4/phidata/app/superset/superset_webserver.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/superset/superset_worker.py` & `phidata-1.6.4/phidata/app/superset/superset_worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/superset/superset_worker_beat.py` & `phidata-1.6.4/phidata/app/superset/superset_worker_beat.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/traefik/crds.py` & `phidata-1.6.4/phidata/app/traefik/crds.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/traefik/ingress_route.py` & `phidata-1.6.4/phidata/app/traefik/ingress_route.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/app/traefik/router.py` & `phidata-1.6.4/phidata/app/traefik/router.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/asset/aws/aws_asset.py` & `phidata-1.6.4/phidata/asset/aws/aws_asset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/asset/data_asset.py` & `phidata-1.6.4/phidata/asset/data_asset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/asset/local/file.py` & `phidata-1.6.4/phidata/asset/local/file.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/asset/local/local_asset.py` & `phidata-1.6.4/phidata/asset/local/local_asset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/api_client.py` & `phidata-1.6.4/phidata/aws/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/athena/query.py` & `phidata-1.6.4/phidata/aws/athena/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/config.py` & `phidata-1.6.4/phidata/aws/config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/create/iam/eks_admin_role.py` & `phidata-1.6.4/phidata/aws/create/iam/eks_admin_role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/create/iam/role.py` & `phidata-1.6.4/phidata/aws/create/iam/role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/enums/manager_status.py` & `phidata-1.6.4/phidata/aws/enums/manager_status.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/manager.py` & `phidata-1.6.4/phidata/aws/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/resource/acm/certificate.py` & `phidata-1.6.4/phidata/aws/resource/acm/certificate.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/resource/athena/query.py` & `phidata-1.6.4/phidata/aws/resource/athena/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/resource/base.py` & `phidata-1.6.4/phidata/aws/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/resource/cloudformation/stack.py` & `phidata-1.6.4/phidata/aws/resource/cloudformation/stack.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/resource/ec2/subnet.py` & `phidata-1.6.4/phidata/aws/resource/ec2/subnet.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/resource/ec2/volume.py` & `phidata-1.6.4/phidata/aws/resource/ec2/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/resource/ecs/cluster.py` & `phidata-1.6.4/phidata/aws/resource/ecs/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/resource/ecs/container.py` & `phidata-1.6.4/phidata/aws/resource/ecs/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/resource/ecs/service.py` & `phidata-1.6.4/phidata/aws/resource/ecs/service.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/resource/ecs/task_definition.py` & `phidata-1.6.4/phidata/aws/resource/ecs/task_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Optional, Any, Dict, List, Literal
 
 from phidata.aws.api_client import AwsApiClient
 from phidata.aws.resource.base import AwsResource
 from phidata.aws.resource.ecs.container import EcsContainer
 from phidata.aws.resource.ecs.volume import EcsVolume
 from phidata.aws.resource.iam.role import IamRole
+from phidata.aws.resource.iam.policy import IamPolicy
 from phidata.utils.cli_console import print_info, print_error
 from phidata.utils.log import logger
 
 
 class EcsTaskDefinition(AwsResource):
     """
     # https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html
@@ -45,19 +46,21 @@
     ephemeral_storage: Optional[Dict[str, Any]] = None
     runtime_platform: Optional[Dict[str, Any]] = None
 
     # Amazon ECS IAM roles
     # The short name or full Amazon Resource Name (ARN) of the IAM role that containers in this task can assume.
     task_role_arn: Optional[str] = None
     # If task_role_arn is None, a default role is created if create_task_role is True
-    create_task_role: bool = False
+    create_task_role: bool = True
     # Name for the default role when task_role_arn is None, use "name-task-role" if not provided
     task_role_name: Optional[str] = None
     # Provide a list of policy ARNs to attach to the role
     add_task_role_policy_arns: Optional[List[str]] = None
+    # Add ecs_exec_policy to task role
+    add_ecs_exec_policy: bool = False
 
     # The Amazon Resource Name (ARN) of the task execution role that grants the Amazon ECS container agent permission
     # to make Amazon Web Services API calls on your behalf. The task execution IAM role is required depending on the
     # requirements of your task.
     execution_role_arn: Optional[str] = None
     # If execution_role_arn is None, a default role is created if create_execution_role is True
     create_execution_role: bool = True
@@ -246,14 +249,37 @@
             "arn:aws:iam::aws:policy/CloudWatchFullAccess",
         ]
         if self.add_task_role_policy_arns is not None and isinstance(
             self.add_task_role_policy_arns, list
         ):
             policy_arns.extend(self.add_task_role_policy_arns)
 
+        ecs_exec_policy = IamPolicy(
+            name=f"{self.name}-ecs-exec-policy",
+            policy_document=dedent(
+                """\
+            {
+               "Version": "2012-10-17",
+               "Statement": [
+                   {
+                   "Effect": "Allow",
+                   "Action": [
+                        "ssmmessages:CreateControlChannel",
+                        "ssmmessages:CreateDataChannel",
+                        "ssmmessages:OpenControlChannel",
+                        "ssmmessages:OpenDataChannel"
+                   ],
+                  "Resource": "*"
+                  }
+               ]
+            }
+            """
+            ),
+        )
+
         return IamRole(
             name=self.task_role_name or f"{self.name}-task-role",
             assume_role_policy_document=dedent(
                 """\
             {
               "Version": "2012-10-17",
               "Statement": [
@@ -264,14 +290,15 @@
                   },
                   "Action": "sts:AssumeRole"
                 }
               ]
             }
             """
             ),
+            policies=[ecs_exec_policy] if self.add_ecs_exec_policy else [],
             policy_arns=policy_arns,
         )
 
     def get_execution_role(self) -> IamRole:
         policy_arns = [
             "arn:aws:iam::aws:policy/service-role/AmazonECSTaskExecutionRolePolicy",
             "arn:aws:iam::aws:policy/CloudWatchFullAccess",
```

### Comparing `phidata-1.6.3/phidata/aws/resource/ecs/volume.py` & `phidata-1.6.4/phidata/aws/resource/ecs/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/resource/eks/addon.py` & `phidata-1.6.4/phidata/aws/resource/eks/addon.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/resource/eks/cluster.py` & `phidata-1.6.4/phidata/aws/resource/eks/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/resource/eks/fargate_profile.py` & `phidata-1.6.4/phidata/aws/resource/eks/fargate_profile.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/resource/eks/kubeconfig.py` & `phidata-1.6.4/phidata/aws/resource/eks/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/resource/eks/node_group.py` & `phidata-1.6.4/phidata/aws/resource/eks/node_group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/resource/elasticache/cluster.py` & `phidata-1.6.4/phidata/aws/resource/elasticache/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/resource/elasticache/subnet_group.py` & `phidata-1.6.4/phidata/aws/resource/elasticache/subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/resource/elb/listener.py` & `phidata-1.6.4/phidata/aws/resource/elb/listener.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     name: str
     load_balancer: Optional[LoadBalancer] = None
     target_group: Optional[TargetGroup] = None
     load_balancer_arn: Optional[str] = None
     protocol: Optional[str] = None
     port: Optional[int] = None
     ssl_policy: Optional[str] = None
-    certificates: Optional[List[Dict[str, bool]]]
+    certificates: Optional[List[Dict[str, Any]]]
     default_actions: Optional[List[Dict]]
     alpn_policy: Optional[List[str]]
     tags: Optional[List[Dict[str, str]]]
 
     def _create(self, aws_client: AwsApiClient) -> bool:
         """Creates the Listener
```

### Comparing `phidata-1.6.3/phidata/aws/resource/elb/load_balancer.py` & `phidata-1.6.4/phidata/aws/resource/elb/load_balancer.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,17 @@
     security_groups: Optional[List[str]] = None
     scheme: Optional[str] = None
     tags: Optional[List[Dict[str, str]]] = None
     type: Optional[str] = None
     ip_address_type: Optional[str] = None
     customer_owned_ipv_4_pool: Optional[str] = None
 
+    # Protocol for load_balancer: HTTP or HTTPS
+    protocol: str = "HTTP"
+
     def _create(self, aws_client: AwsApiClient) -> bool:
         """Creates the Load Balancer
 
         Args:
             aws_client: The AwsApiClient for the current Load Balancer
         """
         print_info(f"Creating {self.get_resource_type()}: {self.get_resource_name()}")
@@ -94,15 +97,15 @@
         elb = self._read(aws_client)
         if elb is None:
             print_error(
                 f"Error reading {self.get_resource_type()}. Please get DNS name manually."
             )
         else:
             dns_name = elb.get("DNSName", None)
-            print_info(f"LoadBalancer DNS: http://{dns_name}")
+            print_info(f"LoadBalancer DNS: {self.protocol.lower()}://{dns_name}")
         return True
 
     def _read(self, aws_client: AwsApiClient) -> Optional[Any]:
         """Returns the LoadBalancer
 
         Args:
             aws_client: The AwsApiClient for the current LoadBalancer
```

### Comparing `phidata-1.6.3/phidata/aws/resource/elb/target_group.py` & `phidata-1.6.4/phidata/aws/resource/elb/target_group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/resource/emr/cluster.py` & `phidata-1.6.4/phidata/aws/resource/emr/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/resource/glue/crawler.py` & `phidata-1.6.4/phidata/aws/resource/glue/crawler.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/resource/group.py` & `phidata-1.6.4/phidata/aws/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/resource/iam/group.py` & `phidata-1.6.4/phidata/aws/resource/iam/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/resource/iam/policy.py` & `phidata-1.6.4/phidata/aws/resource/iam/policy.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/resource/iam/role.py` & `phidata-1.6.4/phidata/aws/resource/iam/role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/resource/rds/db_cluster.py` & `phidata-1.6.4/phidata/aws/resource/rds/db_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/resource/rds/db_instance.py` & `phidata-1.6.4/phidata/aws/resource/rds/db_instance.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/resource/rds/db_subnet_group.py` & `phidata-1.6.4/phidata/aws/resource/rds/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/resource/s3/bucket.py` & `phidata-1.6.4/phidata/aws/resource/s3/bucket.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/resource/secret/manager.py` & `phidata-1.6.4/phidata/aws/resource/secret/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/resource/types.py` & `phidata-1.6.4/phidata/aws/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/resource/utils.py` & `phidata-1.6.4/phidata/aws/resource/utils.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/s3/csv_dataset.py` & `phidata-1.6.4/phidata/aws/s3/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/s3/dataset.py` & `phidata-1.6.4/phidata/aws/s3/dataset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/s3/dataset_base.py` & `phidata-1.6.4/phidata/aws/s3/dataset_base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/s3/object.py` & `phidata-1.6.4/phidata/aws/s3/object.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/aws/worker.py` & `phidata-1.6.4/phidata/aws/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/base.py` & `phidata-1.6.4/phidata/base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/checks/check.py` & `phidata-1.6.4/phidata/checks/check.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/checks/not_empty.py` & `phidata-1.6.4/phidata/checks/not_empty.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/constants.py` & `phidata-1.6.4/phidata/constants.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/decorators/timer.py` & `phidata-1.6.4/phidata/decorators/timer.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/decorators/validate_env.py` & `phidata-1.6.4/phidata/decorators/validate_env.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/docker/api_client.py` & `phidata-1.6.4/phidata/docker/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/docker/args.py` & `phidata-1.6.4/phidata/docker/args.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/docker/config.py` & `phidata-1.6.4/phidata/docker/config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/docker/enums.py` & `phidata-1.6.4/phidata/docker/enums.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/docker/manager.py` & `phidata-1.6.4/phidata/docker/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/docker/resource/base.py` & `phidata-1.6.4/phidata/docker/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/docker/resource/container.py` & `phidata-1.6.4/phidata/docker/resource/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/docker/resource/group.py` & `phidata-1.6.4/phidata/docker/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/docker/resource/image.py` & `phidata-1.6.4/phidata/docker/resource/image.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/docker/resource/network.py` & `phidata-1.6.4/phidata/docker/resource/network.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/docker/resource/types.py` & `phidata-1.6.4/phidata/docker/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/docker/resource/utils.py` & `phidata-1.6.4/phidata/docker/resource/utils.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/docker/resource/volume.py` & `phidata-1.6.4/phidata/docker/resource/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/docker/utils/container.py` & `phidata-1.6.4/phidata/docker/utils/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/docker/worker.py` & `phidata-1.6.4/phidata/docker/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/infra/args.py` & `phidata-1.6.4/phidata/infra/args.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/infra/config.py` & `phidata-1.6.4/phidata/infra/config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/infra/resource.py` & `phidata-1.6.4/phidata/infra/resource.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/api_client.py` & `phidata-1.6.4/phidata/k8s/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/args.py` & `phidata-1.6.4/phidata/k8s/args.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/config.py` & `phidata-1.6.4/phidata/k8s/config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py` & `phidata-1.6.4/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py` & `phidata-1.6.4/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/create/apps/v1/deployment.py` & `phidata-1.6.4/phidata/k8s/create/apps/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/create/common/port.py` & `phidata-1.6.4/phidata/k8s/create/common/port.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/create/core/v1/config_map.py` & `phidata-1.6.4/phidata/k8s/create/core/v1/config_map.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/create/core/v1/container.py` & `phidata-1.6.4/phidata/k8s/create/core/v1/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/create/core/v1/namespace.py` & `phidata-1.6.4/phidata/k8s/create/core/v1/namespace.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/create/core/v1/persistent_volume.py` & `phidata-1.6.4/phidata/k8s/create/core/v1/persistent_volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/create/core/v1/persistent_volume_claim.py` & `phidata-1.6.4/phidata/k8s/create/core/v1/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/create/core/v1/secret.py` & `phidata-1.6.4/phidata/k8s/create/core/v1/secret.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/create/core/v1/service.py` & `phidata-1.6.4/phidata/k8s/create/core/v1/service.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/create/core/v1/service_account.py` & `phidata-1.6.4/phidata/k8s/create/core/v1/service_account.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/create/core/v1/volume.py` & `phidata-1.6.4/phidata/k8s/create/core/v1/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/create/crb/eks_admin_crb.py` & `phidata-1.6.4/phidata/k8s/create/crb/eks_admin_crb.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/create/group.py` & `phidata-1.6.4/phidata/k8s/create/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/create/kubeconfig.py` & `phidata-1.6.4/phidata/k8s/create/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/create/networking_k8s_io/v1/ingress.py` & `phidata-1.6.4/phidata/k8s/create/networking_k8s_io/v1/ingress.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py` & `phidata-1.6.4/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py` & `phidata-1.6.4/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/create/storage_k8s_io/v1/storage_class.py` & `phidata-1.6.4/phidata/k8s/create/storage_k8s_io/v1/storage_class.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/enums/api_version.py` & `phidata-1.6.4/phidata/k8s/enums/api_version.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/enums/kind.py` & `phidata-1.6.4/phidata/k8s/enums/kind.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/enums/manager_status.py` & `phidata-1.6.4/phidata/k8s/enums/manager_status.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/enums/pv.py` & `phidata-1.6.4/phidata/k8s/enums/pv.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/manager.py` & `phidata-1.6.4/phidata/k8s/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py` & `phidata-1.6.4/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py` & `phidata-1.6.4/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/resource/apps/v1/deployment.py` & `phidata-1.6.4/phidata/k8s/resource/apps/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/resource/apps/v1/deployment_strategy.py` & `phidata-1.6.4/phidata/k8s/resource/apps/v1/deployment_strategy.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/resource/base.py` & `phidata-1.6.4/phidata/k8s/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/resource/core/v1/config_map.py` & `phidata-1.6.4/phidata/k8s/resource/core/v1/config_map.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/resource/core/v1/container.py` & `phidata-1.6.4/phidata/k8s/resource/core/v1/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/resource/core/v1/local_object_reference.py` & `phidata-1.6.4/phidata/k8s/resource/core/v1/local_object_reference.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/resource/core/v1/namespace.py` & `phidata-1.6.4/phidata/k8s/resource/core/v1/namespace.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/resource/core/v1/node_selector.py` & `phidata-1.6.4/phidata/k8s/resource/core/v1/node_selector.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/resource/core/v1/object_reference.py` & `phidata-1.6.4/phidata/k8s/resource/core/v1/object_reference.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/resource/core/v1/persistent_volume.py` & `phidata-1.6.4/phidata/k8s/resource/core/v1/persistent_volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/resource/core/v1/persistent_volume_claim.py` & `phidata-1.6.4/phidata/k8s/resource/core/v1/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/resource/core/v1/pod.py` & `phidata-1.6.4/phidata/k8s/resource/core/v1/pod.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/resource/core/v1/pod_spec.py` & `phidata-1.6.4/phidata/k8s/resource/core/v1/pod_spec.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/resource/core/v1/pod_template_spec.py` & `phidata-1.6.4/phidata/k8s/resource/core/v1/pod_template_spec.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/resource/core/v1/resource_requirements.py` & `phidata-1.6.4/phidata/k8s/resource/core/v1/resource_requirements.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/resource/core/v1/secret.py` & `phidata-1.6.4/phidata/k8s/resource/core/v1/secret.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/resource/core/v1/service.py` & `phidata-1.6.4/phidata/k8s/resource/core/v1/service.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/resource/core/v1/service_account.py` & `phidata-1.6.4/phidata/k8s/resource/core/v1/service_account.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/resource/core/v1/toleration.py` & `phidata-1.6.4/phidata/k8s/resource/core/v1/toleration.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/resource/core/v1/topology_spread_constraints.py` & `phidata-1.6.4/phidata/k8s/resource/core/v1/topology_spread_constraints.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/resource/core/v1/volume.py` & `phidata-1.6.4/phidata/k8s/resource/core/v1/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/resource/core/v1/volume_node_affinity.py` & `phidata-1.6.4/phidata/k8s/resource/core/v1/volume_node_affinity.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/resource/core/v1/volume_source.py` & `phidata-1.6.4/phidata/k8s/resource/core/v1/volume_source.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/resource/group.py` & `phidata-1.6.4/phidata/k8s/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/resource/kubeconfig.py` & `phidata-1.6.4/phidata/k8s/resource/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/resource/meta/v1/label_selector.py` & `phidata-1.6.4/phidata/k8s/resource/meta/v1/label_selector.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/resource/meta/v1/object_meta.py` & `phidata-1.6.4/phidata/k8s/resource/meta/v1/object_meta.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/resource/networking_k8s_io/v1/ingress.py` & `phidata-1.6.4/phidata/k8s/resource/networking_k8s_io/v1/ingress.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py` & `phidata-1.6.4/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py` & `phidata-1.6.4/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py` & `phidata-1.6.4/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/resource/types.py` & `phidata-1.6.4/phidata/k8s/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/resource/utils.py` & `phidata-1.6.4/phidata/k8s/resource/utils.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/utils/pod.py` & `phidata-1.6.4/phidata/k8s/utils/pod.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/k8s/worker.py` & `phidata-1.6.4/phidata/k8s/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/llm/duckdb/agent.py` & `phidata-1.6.4/phidata/llm/duckdb/agent.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/llm/duckdb/chain.py` & `phidata-1.6.4/phidata/llm/duckdb/chain.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/llm/duckdb/connection.py` & `phidata-1.6.4/phidata/llm/duckdb/connection.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/llm/duckdb/loader.py` & `phidata-1.6.4/phidata/llm/duckdb/loader.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/llm/duckdb/query.py` & `phidata-1.6.4/phidata/llm/duckdb/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/llm/duckdb/tool.py` & `phidata-1.6.4/phidata/llm/duckdb/tool.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/product/data_product.py` & `phidata-1.6.4/phidata/product/data_product.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/table/local/csv.py` & `phidata-1.6.4/phidata/table/local/csv.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/table/local/local_table.py` & `phidata-1.6.4/phidata/table/local/local_table.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/table/local/parquet.py` & `phidata-1.6.4/phidata/table/local/parquet.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/table/s3/csv.py` & `phidata-1.6.4/phidata/table/s3/csv.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/table/s3/parquet.py` & `phidata-1.6.4/phidata/table/s3/parquet.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/table/s3/s3_table.py` & `phidata-1.6.4/phidata/table/s3/s3_table.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/table/sql/postgres.py` & `phidata-1.6.4/phidata/table/sql/postgres.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/table/sql/sql_table.py` & `phidata-1.6.4/phidata/table/sql/sql_table.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/task/aws/athena/run_query.py` & `phidata-1.6.4/phidata/task/aws/athena/run_query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/task/aws/emr/create_cluster.py` & `phidata-1.6.4/phidata/task/aws/emr/create_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/task/aws/emr/delete_cluster.py` & `phidata-1.6.4/phidata/task/aws/emr/delete_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/task/aws/glue/start_crawler.py` & `phidata-1.6.4/phidata/task/aws/glue/start_crawler.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/task/decorator.py` & `phidata-1.6.4/phidata/task/decorator.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/task/download/s3/to_file.py` & `phidata-1.6.4/phidata/task/download/s3/to_file.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/task/download/url/to_file.py` & `phidata-1.6.4/phidata/task/download/url/to_file.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/task/download/url/to_s3.py` & `phidata-1.6.4/phidata/task/download/url/to_s3.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/task/download/url/to_sql.py` & `phidata-1.6.4/phidata/task/download/url/to_sql.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/task/plot/sql/query.py` & `phidata-1.6.4/phidata/task/plot/sql/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/task/python_task.py` & `phidata-1.6.4/phidata/task/python_task.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/task/run/sql/query.py` & `phidata-1.6.4/phidata/task/run/sql/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/task/task.py` & `phidata-1.6.4/phidata/task/task.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/task/task_relatives.py` & `phidata-1.6.4/phidata/task/task_relatives.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/task/upload/file/to_s3.py` & `phidata-1.6.4/phidata/task/upload/file/to_s3.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/task/upload/file/to_sql.py` & `phidata-1.6.4/phidata/task/upload/file/to_sql.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/types/airflow.py` & `phidata-1.6.4/phidata/types/airflow.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/types/context.py` & `phidata-1.6.4/phidata/types/context.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/types/phidata_runtime.py` & `phidata-1.6.4/phidata/types/phidata_runtime.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/utils/cli_console.py` & `phidata-1.6.4/phidata/utils/cli_console.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/utils/common.py` & `phidata-1.6.4/phidata/utils/common.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/utils/compare.py` & `phidata-1.6.4/phidata/utils/compare.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/utils/context.py` & `phidata-1.6.4/phidata/utils/context.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/utils/dttm.py` & `phidata-1.6.4/phidata/utils/dttm.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/utils/enums.py` & `phidata-1.6.4/phidata/utils/enums.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/utils/env_file.py` & `phidata-1.6.4/phidata/utils/env_file.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/utils/env_var.py` & `phidata-1.6.4/phidata/utils/env_var.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/utils/filesystem.py` & `phidata-1.6.4/phidata/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/utils/log.py` & `phidata-1.6.4/phidata/utils/log.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/utils/prep_infra_config.py` & `phidata-1.6.4/phidata/utils/prep_infra_config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/utils/print_table.py` & `phidata-1.6.4/phidata/utils/print_table.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/utils/workspace_path.py` & `phidata-1.6.4/phidata/utils/workspace_path.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/workflow/decorator.py` & `phidata-1.6.4/phidata/workflow/decorator.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/workflow/workflow.py` & `phidata-1.6.4/phidata/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/workflow/workflow_relatives.py` & `phidata-1.6.4/phidata/workflow/workflow_relatives.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/workspace/config.py` & `phidata-1.6.4/phidata/workspace/config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata/workspace/settings.py` & `phidata-1.6.4/phidata/workspace/settings.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.3/phidata.egg-info/PKG-INFO` & `phidata-1.6.4/phidata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phidata
-Version: 1.6.3
+Version: 1.6.4
 Summary: Building blocks for Data Engineering
 Author-email: Ashpreet Bedi <ashpreet@phidata.com>
 Project-URL: homepage, https://www.phidata.com
 Project-URL: documentation, https://www.docs.phidata.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: phidata Version: 1.6.3 Summary: Building blocks for
+Metadata-Version: 2.1 Name: phidata Version: 1.6.4 Summary: Building blocks for
 Data Engineering Author-email: Ashpreet Bedi
 phidata.com> Project-URL: homepage, https://www.phidata.com Project-URL:
 documentation, https://www.docs.phidata.com Requires-Python: >=3.7 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: aws License-
 File: LICENSE
                              ****** phidata ******
                      Building Blocks for Data Engineering
```

### Comparing `phidata-1.6.3/phidata.egg-info/SOURCES.txt` & `phidata-1.6.4/phidata.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 phidata/app/assistant/assistant.py
 phidata/app/cadvisor/__init__.py
 phidata/app/cadvisor/cadvisor.py
 phidata/app/databox/__init__.py
 phidata/app/databox/databox.py
 phidata/app/db/__init__.py
 phidata/app/db/base_db.py
+phidata/app/django/__init__.py
+phidata/app/django/django_app.py
 phidata/app/elastic/__init__.py
 phidata/app/elastic/elastic_app.py
 phidata/app/elasticsearch/__init__.py
 phidata/app/elasticsearch/elasticsearch.py
 phidata/app/fastapi/__init__.py
 phidata/app/fastapi/fastapi.py
 phidata/app/grafana/__init__.py
```

### Comparing `phidata-1.6.3/pyproject.toml` & `phidata-1.6.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [project]
 name = "phidata"
-version = "1.6.3"
+version = "1.6.4"
 description = "Building blocks for Data Engineering"
 requires-python = ">=3.7"
 readme = "README.md"
 authors = [
   {name = "Ashpreet Bedi", email = "ashpreet@phidata.com"}
 ]
 
 dependencies = [
   "boto3",
-  "phiterm==1.6.3",
+  "phiterm==1.6.4",
   "pyarrow",
   "pydantic",
 ]
 
 [project.optional-dependencies]
 dev = [
     "mypy",
```

