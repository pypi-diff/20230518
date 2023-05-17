# Comparing `tmp/sasctl-1.9.1.tar.gz` & `tmp/sasctl-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sasctl-1.9.1.tar", last modified: Thu May  4 13:12:07 2023, max compression
+gzip compressed data, was "sasctl-1.9.2.tar", last modified: Wed May 17 22:22:28 2023, max compression
```

## Comparing `sasctl-1.9.1.tar` & `sasctl-1.9.2.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:12:07.123613 sasctl-1.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)    18263 2023-05-04 13:11:54.000000 sasctl-1.9.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-04 13:11:54.000000 sasctl-1.9.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-05-04 13:11:54.000000 sasctl-1.9.1/ContributorAgreement.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-04 13:11:54.000000 sasctl-1.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-04 13:11:54.000000 sasctl-1.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-05-04 13:12:07.119613 sasctl-1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-05-04 13:11:54.000000 sasctl-1.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-04 13:11:54.000000 sasctl-1.9.1/SUPPORT.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 13:12:07.123613 sasctl-1.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-04 13:11:55.000000 sasctl-1.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:12:07.095613 sasctl-1.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:12:07.103613 sasctl-1.9.1/src/sasctl/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:12:07.111613 sasctl-1.9.1/src/sasctl/_services/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/_services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19546 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/_services/cas_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/_services/concepts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/_services/data_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/_services/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/_services/folders.py
--rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/_services/microanalytic_score.py
--rw-r--r--   0 runner    (1001) docker     (123)    18619 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/_services/model_management.py
--rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/_services/model_publish.py
--rw-r--r--   0 runner    (1001) docker     (123)    28696 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/_services/model_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/_services/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/_services/relationships.py
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/_services/report_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/_services/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/_services/saslogon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/_services/sentiment_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    13771 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/_services/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/_services/text_categorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/_services/text_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/_services/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    74999 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:12:07.115613 sasctl-1.9.1/src/sasctl/pzmm/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/pzmm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16653 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/pzmm/gitIntegration.py
--rw-r--r--   0 runner    (1001) docker     (123)    17213 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/pzmm/import_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/pzmm/mlflow_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12306 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/pzmm/model_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/pzmm/pickle_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:12:07.115613 sasctl-1.9.1/src/sasctl/pzmm/template_files/
--rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/pzmm/template_files/dmcas_fitstat.json
--rw-r--r--   0 runner    (1001) docker     (123)    51874 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/pzmm/template_files/dmcas_lift.json
--rw-r--r--   0 runner    (1001) docker     (123)   193713 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/pzmm/template_files/dmcas_roc.json
--rw-r--r--   0 runner    (1001) docker     (123)    82150 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/pzmm/write_json_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    63867 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/pzmm/write_score_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/pzmm/zip_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/services.py
--rw-r--r--   0 runner    (1001) docker     (123)    33574 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:12:07.115613 sasctl-1.9.1/src/sasctl/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16435 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/utils/astore.py
--rw-r--r--   0 runner    (1001) docker     (123)     9921 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/utils/model_migration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:12:07.119613 sasctl-1.9.1/src/sasctl/utils/pymas/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/utils/pymas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22824 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/utils/pymas/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    20869 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/utils/pymas/ds2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/utils/pymas/python.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:12:07.119613 sasctl-1.9.1/src/sasctl/utils/pyml2ds/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/utils/pyml2ds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:12:07.119613 sasctl-1.9.1/src/sasctl/utils/pyml2ds/basic/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/utils/pyml2ds/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/utils/pyml2ds/basic/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:12:07.119613 sasctl-1.9.1/src/sasctl/utils/pyml2ds/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/utils/pyml2ds/connectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:12:07.119613 sasctl-1.9.1/src/sasctl/utils/pyml2ds/connectors/ensembles/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/utils/pyml2ds/connectors/ensembles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/utils/pyml2ds/connectors/ensembles/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/utils/pyml2ds/connectors/ensembles/lgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/utils/pyml2ds/connectors/ensembles/pmml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/utils/pyml2ds/connectors/ensembles/xgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/utils/pyml2ds/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:12:07.103613 sasctl-1.9.1/src/sasctl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-05-04 13:12:07.000000 sasctl-1.9.1/src/sasctl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-04 13:12:07.000000 sasctl-1.9.1/src/sasctl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:12:07.000000 sasctl-1.9.1/src/sasctl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-04 13:12:07.000000 sasctl-1.9.1/src/sasctl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-04 13:12:07.000000 sasctl-1.9.1/src/sasctl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-04 13:12:07.000000 sasctl-1.9.1/src/sasctl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:22:28.986489 sasctl-1.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    18706 2023-05-17 22:22:18.000000 sasctl-1.9.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-17 22:22:18.000000 sasctl-1.9.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-05-17 22:22:18.000000 sasctl-1.9.2/ContributorAgreement.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 22:22:18.000000 sasctl-1.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-17 22:22:18.000000 sasctl-1.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-05-17 22:22:28.986489 sasctl-1.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-05-17 22:22:18.000000 sasctl-1.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-17 22:22:18.000000 sasctl-1.9.2/SUPPORT.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 22:22:28.986489 sasctl-1.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-17 22:22:19.000000 sasctl-1.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:22:28.978489 sasctl-1.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:22:28.982489 sasctl-1.9.2/src/sasctl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:22:28.982489 sasctl-1.9.2/src/sasctl/_services/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/_services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19546 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/_services/cas_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/_services/concepts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/_services/data_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/_services/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/_services/folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/_services/microanalytic_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18619 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/_services/model_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/_services/model_publish.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28696 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/_services/model_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/_services/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/_services/relationships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/_services/report_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/_services/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/_services/saslogon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/_services/sentiment_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13771 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/_services/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/_services/text_categorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/_services/text_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/_services/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74999 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:22:28.982489 sasctl-1.9.2/src/sasctl/pzmm/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/pzmm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16653 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/pzmm/gitIntegration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17213 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/pzmm/import_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/pzmm/mlflow_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12306 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/pzmm/model_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/pzmm/pickle_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:22:28.982489 sasctl-1.9.2/src/sasctl/pzmm/template_files/
+-rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/pzmm/template_files/dmcas_fitstat.json
+-rw-r--r--   0 runner    (1001) docker     (123)    51874 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/pzmm/template_files/dmcas_lift.json
+-rw-r--r--   0 runner    (1001) docker     (123)   193713 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/pzmm/template_files/dmcas_roc.json
+-rw-r--r--   0 runner    (1001) docker     (123)    82150 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/pzmm/write_json_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63504 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/pzmm/write_score_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/pzmm/zip_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33574 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:22:28.986489 sasctl-1.9.2/src/sasctl/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16435 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/utils/astore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9921 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/utils/model_migration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:22:28.986489 sasctl-1.9.2/src/sasctl/utils/pymas/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/utils/pymas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22824 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/utils/pymas/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20869 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/utils/pymas/ds2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/utils/pymas/python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:22:28.986489 sasctl-1.9.2/src/sasctl/utils/pyml2ds/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/utils/pyml2ds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:22:28.986489 sasctl-1.9.2/src/sasctl/utils/pyml2ds/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/utils/pyml2ds/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/utils/pyml2ds/basic/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:22:28.986489 sasctl-1.9.2/src/sasctl/utils/pyml2ds/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/utils/pyml2ds/connectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:22:28.986489 sasctl-1.9.2/src/sasctl/utils/pyml2ds/connectors/ensembles/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/utils/pyml2ds/connectors/ensembles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/utils/pyml2ds/connectors/ensembles/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/utils/pyml2ds/connectors/ensembles/lgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/utils/pyml2ds/connectors/ensembles/pmml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/utils/pyml2ds/connectors/ensembles/xgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/utils/pyml2ds/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:22:28.982489 sasctl-1.9.2/src/sasctl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-05-17 22:22:28.000000 sasctl-1.9.2/src/sasctl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-17 22:22:28.000000 sasctl-1.9.2/src/sasctl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 22:22:28.000000 sasctl-1.9.2/src/sasctl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-17 22:22:28.000000 sasctl-1.9.2/src/sasctl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-17 22:22:28.000000 sasctl-1.9.2/src/sasctl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 22:22:28.000000 sasctl-1.9.2/src/sasctl.egg-info/top_level.txt
```

### Comparing `sasctl-1.9.1/CHANGELOG.md` & `sasctl-1.9.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,25 @@
 Unreleased
 ----------
 **Improvements**
  - Refactor `tasks.py` to utilize `sasctl.pzmm` functions.
  - Add `model_info` class to better capture model information.
 
+v1.9.2 (2023-05-17)
+----------
+**Improvements**
+ - Add recursive folder creation and an example.
+ - Add example for migrating models from SAS Viya 3.5 to SAS Viya 4.
+
+**Bugfixes**
+ - Fixed improper json encoding for `pzmm_h2o_model_import.ipynb` example.
+ - Set urllib3 < 2.0.0 to allow requests to update their dependencies.
+ - Set pandas >= 0.24.0 to include df.to_list alias for df.tolist.
+ - Fix minor errors in h2o score code generation
+
 v1.9.1 (2023-05-04)
 ----------
 **Improvements**
  - Updated handling of H2O models in `sasctl.pzmm`.
    - Models are now saved with the appropriate `h2o` functions within the `sasctl.pzmm.PickleModel.pickle_trained_model` function.
    - Example notebooks have been updated to reflect this change.
```

### Comparing `sasctl-1.9.1/CONTRIBUTING.md` & `sasctl-1.9.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/ContributorAgreement.txt` & `sasctl-1.9.2/ContributorAgreement.txt`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/LICENSE` & `sasctl-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/PKG-INFO` & `sasctl-1.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sasctl
-Version: 1.9.1
+Version: 1.9.2
 Summary: SAS Viya Python Client
 Home-page: https://github.com/sassoftware/python-sasctl/
 Author: SAS
 License: Apache v2.0
 Project-URL: Bug Tracker, https://github.com/sassoftware/python-sasctl/issues
 Project-URL: Documentation, https://sassoftware.github.io/python-sasctl/
 Project-URL: Source Code, https://github.com/sassoftware/python-sasctl
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sasctl Version: 1.9.1 Summary: SAS Viya Python
+Metadata-Version: 2.1 Name: sasctl Version: 1.9.2 Summary: SAS Viya Python
 Client Home-page: https://github.com/sassoftware/python-sasctl/ Author: SAS
 License: Apache v2.0 Project-URL: Bug Tracker, https://github.com/sassoftware/
 python-sasctl/issues Project-URL: Documentation, https://sassoftware.github.io/
 python-sasctl/ Project-URL: Source Code, https://github.com/sassoftware/python-
 sasctl Classifier: Development Status :: 5 - Production/Stable Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Environment ::
 Console Classifier: Intended Audience :: Science/Research Classifier: Intended
```

### Comparing `sasctl-1.9.1/README.md` & `sasctl-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/setup.py` & `sasctl-1.9.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         "Documentation": "https://sassoftware.github.io/python-sasctl/",
         "Source Code": "https://github.com/sassoftware/python-sasctl",
     },
     include_package_data=True,
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     python_requires=">=3.6",
-    install_requires=["pandas", "requests", "pyyaml", "packaging"],
+    install_requires=["pandas>=0.24.0", "requests", "pyyaml", "packaging"],
     extras_require={
         "swat": ["swat"],
         "GitPython": ["GitPython"],
         "numpy": ["numpy"],
         "scikit-learn": ["scikit-learn"],
         "kerberos": [
             'kerberos ; platform_system != "Windows"',
```

### Comparing `sasctl-1.9.1/src/sasctl/__init__.py` & `sasctl-1.9.2/src/sasctl/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # encoding: utf-8
 #
 # Copyright © 2019, SAS Institute Inc., Cary, NC, USA.  All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
 
-__version__ = "1.9.1"
+__version__ = "1.9.2"
 __author__ = "SAS"
 __credits__ = [
     "Yi Jian Ching",
     "Lucas De Paula",
     "James Kochuba",
     "Peter Tobac",
     "Chris Toth",
```

### Comparing `sasctl-1.9.1/src/sasctl/_services/cas_management.py` & `sasctl-1.9.2/src/sasctl/_services/cas_management.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/_services/concepts.py` & `sasctl-1.9.2/src/sasctl/_services/concepts.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/_services/data_sources.py` & `sasctl-1.9.2/src/sasctl/_services/data_sources.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/_services/files.py` & `sasctl-1.9.2/src/sasctl/_services/files.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/_services/folders.py` & `sasctl-1.9.2/src/sasctl/_services/folders.py`

 * *Files 13% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
         """
         if parent is not None:
             parent_obj = cls.get_folder(parent)
 
             parent_uri = cls.get_link(parent_obj, "self")
             if parent_uri is None:
-                raise ValueError("`parent` folder '%s' does not exist." % parent)
+                raise ValueError(f"`parent` folder {parent} does not exist.")
             parent_uri = parent_uri["uri"]
         else:
             parent_uri = None
 
         body = {"name": name, "description": description, "folderType": "folder"}
 
         return cls.post(
@@ -131,7 +131,42 @@
 
         # Its possible to lookup special folders by using a handle (called a delegate string in docs)
         # Current values (2022.09) are @myFolder, @appDataFolder, @myHistory, @myFavorites, @public.
         if isinstance(folder, str) and folder.startswith("@"):
             return cls.get(f"/folders/{folder}")
 
         return cls._get_folder(folder, refresh=refresh)
+
+    @classmethod
+    def create_path(cls, folder, description=None):
+        """Create a new folder recursively.
+
+        Parameters
+        ----------
+        folder : str
+            The folder to be created including the path.
+        description: str, optional
+             A description of the folder
+
+        Returns
+        -------
+        RestObj
+            Details of newly-created folder
+
+        """
+        folder = str(folder)
+
+        # Path must include a leading "/"
+        if not folder.startswith("/"):
+            folder = f"/{folder}"
+        path = folder.split("/")
+
+        for level in range(2, len(path) + 1):
+            current_path = path[0:level]
+            name = current_path[-1]
+            parent = "/".join(current_path[0:-1]) or None
+            new_folder = cls.get_folder("/".join(current_path))
+            if not new_folder:
+                new_folder = cls.create_folder(
+                    name, parent=parent, description=description
+                )
+        return new_folder
```

### Comparing `sasctl-1.9.1/src/sasctl/_services/microanalytic_score.py` & `sasctl-1.9.2/src/sasctl/_services/microanalytic_score.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/_services/model_management.py` & `sasctl-1.9.2/src/sasctl/_services/model_management.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/_services/model_publish.py` & `sasctl-1.9.2/src/sasctl/_services/model_publish.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/_services/model_repository.py` & `sasctl-1.9.2/src/sasctl/_services/model_repository.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/_services/projects.py` & `sasctl-1.9.2/src/sasctl/_services/projects.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/_services/relationships.py` & `sasctl-1.9.2/src/sasctl/_services/relationships.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/_services/report_images.py` & `sasctl-1.9.2/src/sasctl/_services/report_images.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/_services/reports.py` & `sasctl-1.9.2/src/sasctl/_services/reports.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/_services/saslogon.py` & `sasctl-1.9.2/src/sasctl/_services/saslogon.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/_services/sentiment_analysis.py` & `sasctl-1.9.2/src/sasctl/_services/sentiment_analysis.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/_services/service.py` & `sasctl-1.9.2/src/sasctl/_services/service.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/_services/text_categorization.py` & `sasctl-1.9.2/src/sasctl/_services/text_categorization.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/_services/text_parsing.py` & `sasctl-1.9.2/src/sasctl/_services/text_parsing.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/_services/workflow.py` & `sasctl-1.9.2/src/sasctl/_services/workflow.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/core.py` & `sasctl-1.9.2/src/sasctl/core.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/exceptions.py` & `sasctl-1.9.2/src/sasctl/exceptions.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/pzmm/gitIntegration.py` & `sasctl-1.9.2/src/sasctl/pzmm/gitIntegration.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/pzmm/import_model.py` & `sasctl-1.9.2/src/sasctl/pzmm/import_model.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/pzmm/mlflow_model.py` & `sasctl-1.9.2/src/sasctl/pzmm/mlflow_model.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/pzmm/model_parameters.py` & `sasctl-1.9.2/src/sasctl/pzmm/model_parameters.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/pzmm/pickle_model.py` & `sasctl-1.9.2/src/sasctl/pzmm/pickle_model.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/pzmm/template_files/dmcas_fitstat.json` & `sasctl-1.9.2/src/sasctl/pzmm/template_files/dmcas_fitstat.json`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/pzmm/template_files/dmcas_lift.json` & `sasctl-1.9.2/src/sasctl/pzmm/template_files/dmcas_lift.json`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/pzmm/template_files/dmcas_roc.json` & `sasctl-1.9.2/src/sasctl/pzmm/template_files/dmcas_roc.json`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/pzmm/write_json_files.py` & `sasctl-1.9.2/src/sasctl/pzmm/write_json_files.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/pzmm/write_score_code.py` & `sasctl-1.9.2/src/sasctl/pzmm/write_score_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,15 +202,15 @@
         # Set the output variables in the line below from score_metrics
         cls.score_code += f"{'':4}\"Output: {', '.join(score_metrics)}\"\n\n"
 
         # Run a try/except block to catch errors for model loading (skip binary string)
         if model_load:
             cls.score_code += (
                 f"{'':4}try:\n{'':8}global model\n{'':4}"
-                f"except NameError:\n{model_load}"
+                f"except NameError:\n{model_load}\n"
             )
 
         if missing_values:
             cls._impute_missing_values(input_data, input_var_list, input_dtypes_list)
 
         # Create the appropriate style of input array and write out the predict method
         if any(x in ["mojo_model", "binary_h2o_model"] for x in kwargs):
@@ -444,37 +444,29 @@
         str
             Preformatted string for the next section of score code.
         """
         pickle_type = pickle_type if pickle_type else "pickle"
 
         if mojo_model:
             cls.score_code += (
-                f'model_path = Path("/models/resources/viya/{model_id}'
-                f'")\nwith gzip.open(model_path / "{model_file_name}'
-                f'", "r") as fileIn, open(model_path / '
-                f"\"{str(Path(model_file_name).with_suffix('.zip'))}\","
-                f" \"wb\") as fileOut:\n{'':4}shutil.copyfileobj(fileIn,"
-                " fileOut)\nos.chmod(model_path / "
-                f"\"{str(Path(model_file_name).with_suffix('.zip'))}\""
-                ", 0o777)\nmodel = h2o.import_mojo(model_path / "
-                f"\"{str(Path(model_file_name).with_suffix('.zip'))}\")"
-                "\n\n"
+                f"model = h2o.import_mojo(str(Path("
+                f'"/models/resources/viya/{model_id}/{model_file_name}")))\n\n'
             )
             return (
-                f"{'':8}model = h2o.import_mojo(model_path / \""
-                f"{str(Path(model_file_name).with_suffix('.zip'))}\")"
+                f"{'':8}model = h2o.import_mojo(str(Path("
+                f'"/models/resources/viya/{model_id}/{model_file_name}")))'
             )
         elif binary_h2o_model:
             cls.score_code += (
-                'model = h2o.load(Path("/models/resources/viya/'
-                f'{model_id}/{model_file_name}"))\n\n'
+                f'model = h2o.load(str(Path("/models/resources/viya/'
+                f'{model_id}/{model_file_name}")))\n\n'
             )
             return (
-                f'        model = h2o.load(Path("/models/resources/viya/'
-                f'{model_id}/{model_file_name}"))'
+                f"{'':8}model = h2o.load(str(Path(\"/models/resources/viya/"
+                f'{model_id}/{model_file_name}")))'
             )
         else:
             cls.score_code += (
                 f'model_path = Path("/models/resources/viya/{model_id}'
                 f'")\nwith open(model_path / "{model_file_name}", '
                 f"\"rb\") as pickle_model:\n{'':4}model = {pickle_type}"
                 ".load(pickle_model)\n\n"
@@ -545,14 +537,15 @@
         data : pandas.DataFrame
             Input dataset for model training or predictions.
         var_list : list of str
             List of variable names
         dtype_list : list of str
             List of variable data types
         """
+        cls.score_code += "\n"
         for var, dtype in zip(var_list, dtype_list):
             # Split up between numeric and character variables
             if any(t in dtype for t in ["int", "float"]):
                 cls._impute_numeric(data, var)
             else:
                 cls._impute_char(var)
         cls.score_code += "\n"
@@ -634,15 +627,15 @@
                 else:
                     col_type = "string"
                 column_types.append(f'"{var}" : "{col_type}"')
             cls.score_code += (
                 f"{'':4}input_array = pd.DataFrame("
                 f"[[{', '.join(var_list)}]],\n{'':31}columns=["
                 f"{column_names}],\n{'':31}dtype=float,\n{'':31}"
-                f"index=[0])\n{'':4}column_types = {{{column_types}}}\n"
+                f"index=[0])\n{'':4}column_types = {{column_types}}\n"
                 f"{'':4}h2o_array = h2o.H2OFrame(input_array, "
                 f"column_types=column_types)\n{'':4}prediction = "
                 f"model.{method.__name__}(h2o_array)\n{'':4}prediction"
                 f" = h2o.as_list(prediction, use_pandas=False)\n"
             )
         # Statsmodels models
         elif statsmodels_model:
@@ -920,15 +913,15 @@
                 )
         else:
             # Classification model including predictions and classification
             if h2o_model:
                 cls.score_code += f"{'':4}{metrics[0]} = prediction[1][0]\n"
                 for i in range(len(metrics) - 1):
                     cls.score_code += (
-                        f"{'':4}{metrics[i + 1]} = prediction[1][{i + 1}]\n"
+                        f"{'':4}{metrics[i + 1]} = float(prediction[1][{i + 1}])\n"
                     )
             else:
                 for i in range(len(metrics)):
                     cls.score_code += f"{'':4}{metrics[i]} = prediction[{i}]\n"
             cls.score_code += f"\n{'':4}return {', '.join(metrics)}"
 
     @classmethod
@@ -1021,15 +1014,17 @@
             # H2O models with two metrics are assumed to be classification + probability
             if h2o_model:
                 warn(
                     "For H2O models, it is assumed if two metrics are provided, the "
                     "score code should output the classification and probability for "
                     "the target event to occur."
                 )
-                cls.score_code += f"{'':4}return prediction[1][0], prediction[1][2]"
+                cls.score_code += (
+                    f"{'':4}return prediction[1][0], " f"float(prediction[1][2])"
+                )
             # Calculate the classification; return the classification and probability
             elif sum(returns) == 0 and len(returns) == 1:
                 warn(
                     "Due to the ambiguity of differentiating the classification and "
                     "probability output metrics, it is assumed that the classification "
                     "metric is returned first."
                 )
@@ -1072,15 +1067,16 @@
                         f"{'':4}return prediction[{class_index}], prediction[0]"
                     )
             else:
                 cls._invalid_predict_config()
         elif len(metrics) == 3:
             if h2o_model:
                 cls.score_code += (
-                    f"{'':4}return prediction[1][0], prediction[1][1], prediction[1][2]"
+                    f"{'':4}return prediction[1][0], float(prediction[1][1]), "
+                    f"float(prediction[1][2])"
                 )
             elif sum(returns) == 0 and len(returns) == 1:
                 warn(
                     "Due to the ambiguity of the provided metrics and prediction return"
                     " types, the score code assumes the return order to be: "
                     "[classification, probability of event, probability of no event]."
                 )
```

### Comparing `sasctl-1.9.1/src/sasctl/pzmm/zip_model.py` & `sasctl-1.9.2/src/sasctl/pzmm/zip_model.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/services.py` & `sasctl-1.9.2/src/sasctl/services.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/tasks.py` & `sasctl-1.9.2/src/sasctl/tasks.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/utils/astore.py` & `sasctl-1.9.2/src/sasctl/utils/astore.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/utils/cli.py` & `sasctl-1.9.2/src/sasctl/utils/cli.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/utils/decorators.py` & `sasctl-1.9.2/src/sasctl/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/utils/misc.py` & `sasctl-1.9.2/src/sasctl/utils/misc.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/utils/model_migration.py` & `sasctl-1.9.2/src/sasctl/utils/model_migration.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/utils/pymas/core.py` & `sasctl-1.9.2/src/sasctl/utils/pymas/core.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/utils/pymas/ds2.py` & `sasctl-1.9.2/src/sasctl/utils/pymas/ds2.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/utils/pymas/python.py` & `sasctl-1.9.2/src/sasctl/utils/pymas/python.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/utils/pyml2ds/basic/tree.py` & `sasctl-1.9.2/src/sasctl/utils/pyml2ds/basic/tree.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/utils/pyml2ds/connectors/ensembles/core.py` & `sasctl-1.9.2/src/sasctl/utils/pyml2ds/connectors/ensembles/core.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/utils/pyml2ds/connectors/ensembles/lgb.py` & `sasctl-1.9.2/src/sasctl/utils/pyml2ds/connectors/ensembles/lgb.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/utils/pyml2ds/connectors/ensembles/pmml.py` & `sasctl-1.9.2/src/sasctl/utils/pyml2ds/connectors/ensembles/pmml.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/utils/pyml2ds/connectors/ensembles/xgb.py` & `sasctl-1.9.2/src/sasctl/utils/pyml2ds/connectors/ensembles/xgb.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl/utils/pyml2ds/core.py` & `sasctl-1.9.2/src/sasctl/utils/pyml2ds/core.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.1/src/sasctl.egg-info/PKG-INFO` & `sasctl-1.9.2/src/sasctl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sasctl
-Version: 1.9.1
+Version: 1.9.2
 Summary: SAS Viya Python Client
 Home-page: https://github.com/sassoftware/python-sasctl/
 Author: SAS
 License: Apache v2.0
 Project-URL: Bug Tracker, https://github.com/sassoftware/python-sasctl/issues
 Project-URL: Documentation, https://sassoftware.github.io/python-sasctl/
 Project-URL: Source Code, https://github.com/sassoftware/python-sasctl
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sasctl Version: 1.9.1 Summary: SAS Viya Python
+Metadata-Version: 2.1 Name: sasctl Version: 1.9.2 Summary: SAS Viya Python
 Client Home-page: https://github.com/sassoftware/python-sasctl/ Author: SAS
 License: Apache v2.0 Project-URL: Bug Tracker, https://github.com/sassoftware/
 python-sasctl/issues Project-URL: Documentation, https://sassoftware.github.io/
 python-sasctl/ Project-URL: Source Code, https://github.com/sassoftware/python-
 sasctl Classifier: Development Status :: 5 - Production/Stable Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Environment ::
 Console Classifier: Intended Audience :: Science/Research Classifier: Intended
```

### Comparing `sasctl-1.9.1/src/sasctl.egg-info/SOURCES.txt` & `sasctl-1.9.2/src/sasctl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

