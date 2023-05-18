# Comparing `tmp/exabyte-api-client-2022.1.9.post0.tar.gz` & `tmp/exabyte-api-client-2023.5.18.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exabyte-api-client-2022.1.9.post0.tar", last modified: Sun Jan  9 00:49:13 2022, max compression
+gzip compressed data, was "exabyte-api-client-2023.5.18.post0.tar", last modified: Thu May 18 19:16:07 2023, max compression
```

## Comparing `exabyte-api-client-2022.1.9.post0.tar` & `exabyte-api-client-2023.5.18.post0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:49:13.809919 exabyte-api-client-2022.1.9.post0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:49:13.801918 exabyte-api-client-2022.1.9.post0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:49:13.805919 exabyte-api-client-2022.1.9.post0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1901 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/.github/workflows/cicd.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2200 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      563 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     2019 2022-01-09 00:49:13.809919 exabyte-api-client-2022.1.9.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1367 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:49:13.805919 exabyte-api-client-2022.1.9.post0/exabyte_api_client/
--rw-r--r--   0 runner    (1001) docker     (121)      816 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/exabyte_api_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-01-09 00:49:13.000000 exabyte-api-client-2022.1.9.post0/exabyte_api_client/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:49:13.805919 exabyte-api-client-2022.1.9.post0/exabyte_api_client/endpoints/
--rw-r--r--   0 runner    (1001) docker     (121)     1654 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/exabyte_api_client/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1526 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/exabyte_api_client/endpoints/bank_entity.py
--rw-r--r--   0 runner    (1001) docker     (121)      928 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/exabyte_api_client/endpoints/bank_materials.py
--rw-r--r--   0 runner    (1001) docker     (121)      928 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/exabyte_api_client/endpoints/bank_workflows.py
--rw-r--r--   0 runner    (1001) docker     (121)     1336 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/exabyte_api_client/endpoints/charges.py
--rw-r--r--   0 runner    (1001) docker     (121)     2914 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/exabyte_api_client/endpoints/entity.py
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/exabyte_api_client/endpoints/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)     5788 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/exabyte_api_client/endpoints/jobs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2191 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/exabyte_api_client/endpoints/login.py
--rw-r--r--   0 runner    (1001) docker     (121)     1110 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/exabyte_api_client/endpoints/logout.py
--rw-r--r--   0 runner    (1001) docker     (121)     2869 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/exabyte_api_client/endpoints/materials.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:49:13.805919 exabyte-api-client-2022.1.9.post0/exabyte_api_client/endpoints/mixins/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/exabyte_api_client/endpoints/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      394 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/exabyte_api_client/endpoints/mixins/default.py
--rw-r--r--   0 runner    (1001) docker     (121)      903 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/exabyte_api_client/endpoints/mixins/set.py
--rw-r--r--   0 runner    (1001) docker     (121)     1309 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/exabyte_api_client/endpoints/projects.py
--rw-r--r--   0 runner    (1001) docker     (121)     2161 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/exabyte_api_client/endpoints/raw_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     1282 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/exabyte_api_client/endpoints/refined_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     1114 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/exabyte_api_client/endpoints/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:49:13.805919 exabyte-api-client-2022.1.9.post0/exabyte_api_client/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/exabyte_api_client/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4140 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/exabyte_api_client/utils/http.py
--rw-r--r--   0 runner    (1001) docker     (121)     1029 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/exabyte_api_client/utils/materials.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:49:13.805919 exabyte-api-client-2022.1.9.post0/exabyte_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2019 2022-01-09 00:49:13.000000 exabyte-api-client-2022.1.9.post0/exabyte_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2747 2022-01-09 00:49:13.000000 exabyte-api-client-2022.1.9.post0/exabyte_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-09 00:49:13.000000 exabyte-api-client-2022.1.9.post0/exabyte_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-01-09 00:49:13.000000 exabyte-api-client-2022.1.9.post0/exabyte_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-01-09 00:49:13.000000 exabyte-api-client-2022.1.9.post0/exabyte_api_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      260 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/requirements-dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)     1221 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (121)      783 2022-01-09 00:49:13.809919 exabyte-api-client-2022.1.9.post0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:49:13.809919 exabyte-api-client-2022.1.9.post0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      616 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:49:13.809919 exabyte-api-client-2022.1.9.post0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/tests/data/login.json
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/tests/data/logout.json
--rw-r--r--   0 runner    (1001) docker     (121)     1430 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/tests/data/material.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:49:13.809919 exabyte-api-client-2022.1.9.post0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (121)      661 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2127 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/tests/integration/entity.py
--rw-r--r--   0 runner    (1001) docker     (121)     2921 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/tests/integration/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1136 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/tests/integration/test_materials.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:49:13.809919 exabyte-api-client-2022.1.9.post0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (121)      746 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1612 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/tests/unit/entity.py
--rw-r--r--   0 runner    (1001) docker     (121)      787 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/tests/unit/test_bank_materials.py
--rw-r--r--   0 runner    (1001) docker     (121)      787 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/tests/unit/test_bank_workflows.py
--rw-r--r--   0 runner    (1001) docker     (121)     1458 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/tests/unit/test_httpBase.py
--rw-r--r--   0 runner    (1001) docker     (121)      980 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/tests/unit/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1081 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/tests/unit/test_login.py
--rw-r--r--   0 runner    (1001) docker     (121)      922 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/tests/unit/test_logout.py
--rw-r--r--   0 runner    (1001) docker     (121)     1015 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/tests/unit/test_materials.py
--rw-r--r--   0 runner    (1001) docker     (121)      807 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/tests/unit/test_refined_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     1015 2022-01-09 00:48:51.000000 exabyte-api-client-2022.1.9.post0/tests/unit/test_workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:16:07.925072 exabyte-api-client-2023.5.18.post0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:16:07.917072 exabyte-api-client-2023.5.18.post0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:16:07.921072 exabyte-api-client-2023.5.18.post0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/.github/workflows/cicd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-18 19:16:07.925072 exabyte-api-client-2023.5.18.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:16:07.917072 exabyte-api-client-2023.5.18.post0/exabyte_api_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-18 19:16:07.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:16:07.921072 exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/bank_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/bank_materials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/bank_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/charges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/logout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/materials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:16:07.921072 exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/mixins/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/mixins/set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/raw_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/refined_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:16:07.921072 exabyte-api-client-2023.5.18.post0/exabyte_api_client/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/utils/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/utils/materials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:16:07.921072 exabyte-api-client-2023.5.18.post0/exabyte_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-18 19:16:07.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-05-18 19:16:07.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 19:16:07.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-18 19:16:07.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-18 19:16:07.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/requirements-dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1221 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-18 19:16:07.925072 exabyte-api-client-2023.5.18.post0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:16:07.921072 exabyte-api-client-2023.5.18.post0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:16:07.921072 exabyte-api-client-2023.5.18.post0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/tests/data/login.json
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/tests/data/logout.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/tests/data/material.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:16:07.921072 exabyte-api-client-2023.5.18.post0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/tests/integration/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/tests/integration/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/tests/integration/test_materials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:16:07.925072 exabyte-api-client-2023.5.18.post0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/tests/unit/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/tests/unit/test_bank_materials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/tests/unit/test_bank_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/tests/unit/test_httpBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/tests/unit/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/tests/unit/test_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/tests/unit/test_logout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/tests/unit/test_materials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/tests/unit/test_refined_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/tests/unit/test_workflows.py
```

### Comparing `exabyte-api-client-2022.1.9.post0/.github/workflows/cicd.yml` & `exabyte-api-client-2023.5.18.post0/.github/workflows/cicd.yml`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 concurrency:
   group: ${{ github.workflow }}-${{ github.event.pull_request.number || github.ref }}
   cancel-in-progress: true
 
 jobs:
 
   run-tests:
-    runs-on: ubuntu-latest
+    runs-on: ubuntu-20.04
     strategy:
       matrix:
         python-version: [3.6, 3.7, 3.8]
 
     steps:
       - name: Checkout this repository
         uses: actions/checkout@v2
@@ -35,15 +35,15 @@
 
       - name: Run integration tests
         if: matrix.python-version == '3.8'
         uses: ./actions/py/test
         with:
           integration-test-directory: tests/integration
         env:
-          TEST_HOST: platform.exabyte.io
+          TEST_HOST: platform.mat3ra.com
           TEST_PORT: 443
           TEST_ACCOUNT_ID: ${{ secrets.DEMO_ACCOUNT_ID }}
           TEST_AUTH_TOKEN: ${{ secrets.DEMO_AUTH_TOKEN }}
           TEST_SECURE: true
 
 
   publish:
```

### Comparing `exabyte-api-client-2022.1.9.post0/.gitignore` & `exabyte-api-client-2023.5.18.post0/.gitignore`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2022.1.9.post0/LICENSE.md` & `exabyte-api-client-2023.5.18.post0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2022.1.9.post0/PKG-INFO` & `exabyte-api-client-2023.5.18.post0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 Metadata-Version: 2.1
 Name: exabyte-api-client
-Version: 2022.1.9.post0
+Version: 2023.5.18.post0
 Summary: Exabyte Python Client for RESTful API
 Home-page: https://github.com/Exabyte-io/api-client
 Author: Exabyte Inc.
-Author-email: info@exabyte.io
-License: UNKNOWN
-Platform: UNKNOWN
+Author-email: info@mat3ra.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
 
 [![PyPI version](https://badge.fury.io/py/exabyte-api-client.svg)](https://badge.fury.io/py/exabyte-api-client)
 
-This package provides access to Exabyte.io [RESTful API](https://docs.exabyte.io/rest-api/overview/).
+This package provides access to Exabyte.io [RESTful API](https://docs.mat3ra.com/rest-api/overview/).
 
 # Installation
 
 We recommend creating a virtual environment before installing:
 
 ```bash
 virtualenv my-virtualenv
@@ -64,9 +62,7 @@
 ```
 (assuming you have a `python2` binary in your PATH environment).
 
 Note that the integration tests require a REST API service against which the live tests will run. See `tests/integration/__init__.py` for the environment variable details.
 
 
 © 2020 Exabyte Inc.
-
-
```

### Comparing `exabyte-api-client-2022.1.9.post0/README.md` & `exabyte-api-client-2023.5.18.post0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [![PyPI version](https://badge.fury.io/py/exabyte-api-client.svg)](https://badge.fury.io/py/exabyte-api-client)
 
-This package provides access to Exabyte.io [RESTful API](https://docs.exabyte.io/rest-api/overview/).
+This package provides access to Exabyte.io [RESTful API](https://docs.mat3ra.com/rest-api/overview/).
 
 # Installation
 
 We recommend creating a virtual environment before installing:
 
 ```bash
 virtualenv my-virtualenv
```

### Comparing `exabyte-api-client-2022.1.9.post0/exabyte_api_client/__init__.py` & `exabyte-api-client-2023.5.18.post0/exabyte_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2022.1.9.post0/exabyte_api_client/endpoints/__init__.py` & `exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2022.1.9.post0/exabyte_api_client/endpoints/bank_entity.py` & `exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/bank_entity.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2022.1.9.post0/exabyte_api_client/endpoints/bank_materials.py` & `exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/bank_materials.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2022.1.9.post0/exabyte_api_client/endpoints/bank_workflows.py` & `exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/bank_workflows.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2022.1.9.post0/exabyte_api_client/endpoints/charges.py` & `exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/charges.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2022.1.9.post0/exabyte_api_client/endpoints/entity.py` & `exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/entity.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2022.1.9.post0/exabyte_api_client/endpoints/jobs.py` & `exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/jobs.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
         """
         response = self.request('GET', '/'.join(('jobs', id_, 'files')), headers=self.headers)
         return response
 
     def insert_output_files(self, id_, data):
         """
         Inserts job output files.
-        Implements https://docs.exabyte.io/api/#!/Job/post_jobs_id_output_files
+        Implements https://docs.mat3ra.com/api/#!/Job/post_jobs_id_output_files
 
         Args:
             id_ (str): job ID.
 
         Returns:
             None
```

### Comparing `exabyte-api-client-2022.1.9.post0/exabyte_api_client/endpoints/login.py` & `exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/login.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2022.1.9.post0/exabyte_api_client/endpoints/logout.py` & `exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/logout.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2022.1.9.post0/exabyte_api_client/endpoints/materials.py` & `exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/materials.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2022.1.9.post0/exabyte_api_client/endpoints/mixins/set.py` & `exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/mixins/set.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2022.1.9.post0/exabyte_api_client/endpoints/projects.py` & `exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/projects.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2022.1.9.post0/exabyte_api_client/endpoints/raw_properties.py` & `exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/raw_properties.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2022.1.9.post0/exabyte_api_client/endpoints/refined_properties.py` & `exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/refined_properties.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2022.1.9.post0/exabyte_api_client/endpoints/workflows.py` & `exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/workflows.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2022.1.9.post0/exabyte_api_client/utils/http.py` & `exabyte-api-client-2023.5.18.post0/exabyte_api_client/utils/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         port (int): Exabyte API port number.
         version (str): Exabyte API version.
         secure (bool): whether to use secure http protocol (https vs http).
         kwargs (dict): a dictionary of HTTP session options.
             timeout (int): session timeout in seconds.
 
     Attributes:
-        preamble (str): common part of URL endpoints, e.g. https://platform.exabyte.io:4000/api/v1/.
+        preamble (str): common part of URL endpoints, e.g. https://platform.mat3ra.com:4000/api/v1/.
     """
 
     def __init__(self, host, port, version, secure, **kwargs):
         self.preamble = '{}://{}:{}/api/{}/'.format('https' if secure else 'http', host, port, version)
         super(Connection, self).__init__(**kwargs)
 
     def request(self, method, endpoint_path, params=None, data=None, headers=None):
```

### Comparing `exabyte-api-client-2022.1.9.post0/exabyte_api_client/utils/materials.py` & `exabyte-api-client-2023.5.18.post0/exabyte_api_client/utils/materials.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2022.1.9.post0/exabyte_api_client.egg-info/PKG-INFO` & `exabyte-api-client-2023.5.18.post0/exabyte_api_client.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 Metadata-Version: 2.1
 Name: exabyte-api-client
-Version: 2022.1.9.post0
+Version: 2023.5.18.post0
 Summary: Exabyte Python Client for RESTful API
 Home-page: https://github.com/Exabyte-io/api-client
 Author: Exabyte Inc.
-Author-email: info@exabyte.io
-License: UNKNOWN
-Platform: UNKNOWN
+Author-email: info@mat3ra.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
 
 [![PyPI version](https://badge.fury.io/py/exabyte-api-client.svg)](https://badge.fury.io/py/exabyte-api-client)
 
-This package provides access to Exabyte.io [RESTful API](https://docs.exabyte.io/rest-api/overview/).
+This package provides access to Exabyte.io [RESTful API](https://docs.mat3ra.com/rest-api/overview/).
 
 # Installation
 
 We recommend creating a virtual environment before installing:
 
 ```bash
 virtualenv my-virtualenv
@@ -64,9 +62,7 @@
 ```
 (assuming you have a `python2` binary in your PATH environment).
 
 Note that the integration tests require a REST API service against which the live tests will run. See `tests/integration/__init__.py` for the environment variable details.
 
 
 © 2020 Exabyte Inc.
-
-
```

### Comparing `exabyte-api-client-2022.1.9.post0/exabyte_api_client.egg-info/SOURCES.txt` & `exabyte-api-client-2023.5.18.post0/exabyte_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2022.1.9.post0/run-tests.sh` & `exabyte-api-client-2023.5.18.post0/run-tests.sh`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2022.1.9.post0/setup.cfg` & `exabyte-api-client-2023.5.18.post0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = exabyte-api-client
 author = Exabyte Inc.
-author_email = info@exabyte.io
+author_email = info@mat3ra.com
 description = Exabyte Python Client for RESTful API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Exabyte-io/api-client
 classifiers = 
 	Programming Language :: Python
 	Programming Language :: Python :: 3
@@ -16,15 +16,15 @@
 
 [options]
 package_dir = 
 	= .
 packages = find:
 python_requires = >= 3.6
 install_requires = 
-	requests==2.20.1
+	requests==2.26.0
 
 [options.extras_require]
 test = 
 	coverage[toml]>=5.3
 	mock>=1.3.0
 
 [options.packages.find]
```

### Comparing `exabyte-api-client-2022.1.9.post0/tests/__init__.py` & `exabyte-api-client-2023.5.18.post0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2022.1.9.post0/tests/data/material.json` & `exabyte-api-client-2023.5.18.post0/tests/data/material.json`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2022.1.9.post0/tests/integration/__init__.py` & `exabyte-api-client-2023.5.18.post0/tests/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2022.1.9.post0/tests/integration/entity.py` & `exabyte-api-client-2023.5.18.post0/tests/integration/entity.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2022.1.9.post0/tests/integration/test_jobs.py` & `exabyte-api-client-2023.5.18.post0/tests/integration/test_jobs.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2022.1.9.post0/tests/integration/test_materials.py` & `exabyte-api-client-2023.5.18.post0/tests/integration/test_materials.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2022.1.9.post0/tests/unit/__init__.py` & `exabyte-api-client-2023.5.18.post0/tests/unit/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Base class for endpoints unit tests.
     """
 
     def __init__(self, *args, **kwargs):
         super(EndpointBaseUnitTest, self).__init__(*args, **kwargs)
         self.port = 4000
         self.version = "2018-10-01"
-        self.host = 'platform.exabyte.io'
+        self.host = 'platform.mat3ra.com'
         self.account_id = 'ubxMkAyx37Rjn8qK9'
         self.auth_token = 'XihOnUA8EqytSui1icz6fYhsJ2tUsJGGTlV03upYPSF'
 
     def mock_response(self, content, status_code=200, reason='OK'):
         response = Response()
         response._content = content.encode()
         response.status_code = status_code
```

### Comparing `exabyte-api-client-2022.1.9.post0/tests/unit/entity.py` & `exabyte-api-client-2023.5.18.post0/tests/unit/entity.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2022.1.9.post0/tests/unit/test_bank_materials.py` & `exabyte-api-client-2023.5.18.post0/tests/unit/test_bank_materials.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2022.1.9.post0/tests/unit/test_bank_workflows.py` & `exabyte-api-client-2023.5.18.post0/tests/unit/test_bank_workflows.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2022.1.9.post0/tests/unit/test_httpBase.py` & `exabyte-api-client-2023.5.18.post0/tests/unit/test_httpBase.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2022.1.9.post0/tests/unit/test_jobs.py` & `exabyte-api-client-2023.5.18.post0/tests/unit/test_jobs.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2022.1.9.post0/tests/unit/test_login.py` & `exabyte-api-client-2023.5.18.post0/tests/unit/test_login.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2022.1.9.post0/tests/unit/test_logout.py` & `exabyte-api-client-2023.5.18.post0/tests/unit/test_logout.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2022.1.9.post0/tests/unit/test_materials.py` & `exabyte-api-client-2023.5.18.post0/tests/unit/test_materials.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2022.1.9.post0/tests/unit/test_refined_properties.py` & `exabyte-api-client-2023.5.18.post0/tests/unit/test_refined_properties.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2022.1.9.post0/tests/unit/test_workflows.py` & `exabyte-api-client-2023.5.18.post0/tests/unit/test_workflows.py`

 * *Files identical despite different names*

