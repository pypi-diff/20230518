# Comparing `tmp/chaostoolkit-google-cloud-platform-0.8.2.tar.gz` & `tmp/chaostoolkit-google-cloud-platform-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chaostoolkit-google-cloud-platform-0.8.2.tar", last modified: Wed Feb  8 15:41:44 2023, max compression
+gzip compressed data, was "dist/chaostoolkit-google-cloud-platform-0.9.0.tar", last modified: Thu May 18 21:11:43 2023, max compression
```

## Comparing `chaostoolkit-google-cloud-platform-0.8.2.tar` & `chaostoolkit-google-cloud-platform-0.9.0.tar`

### file list

```diff
@@ -1,71 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:41:44.000000 chaostoolkit-google-cloud-platform-0.8.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:41:44.000000 chaostoolkit-google-cloud-platform-0.8.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:41:44.000000 chaostoolkit-google-cloud-platform-0.8.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/.github/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    12814 2023-02-08 15:41:44.000000 chaostoolkit-google-cloud-platform-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11495 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:41:44.000000 chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/
--rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:41:44.000000 chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/cloudbuild/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/cloudbuild/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/cloudbuild/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/cloudbuild/probes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:41:44.000000 chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/cloudlogging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/cloudlogging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/cloudlogging/probes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:41:44.000000 chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/cloudrun/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/cloudrun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/cloudrun/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/cloudrun/probes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:41:44.000000 chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/gke/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/gke/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:41:44.000000 chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/gke/nodepool/
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/gke/nodepool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/gke/nodepool/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/gke/nodepool/probes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:41:44.000000 chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/monitoring/probes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:41:44.000000 chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12643 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/sql/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/sql/probes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:41:44.000000 chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/storage/probes.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:41:44.000000 chaostoolkit-google-cloud-platform-0.8.2/chaostoolkit_google_cloud_platform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12814 2023-02-08 15:41:43.000000 chaostoolkit-google-cloud-platform-0.8.2/chaostoolkit_google_cloud_platform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-02-08 15:41:43.000000 chaostoolkit-google-cloud-platform-0.8.2/chaostoolkit_google_cloud_platform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 15:41:43.000000 chaostoolkit-google-cloud-platform-0.8.2/chaostoolkit_google_cloud_platform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-02-08 15:41:43.000000 chaostoolkit-google-cloud-platform-0.8.2/chaostoolkit_google_cloud_platform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-08 15:41:43.000000 chaostoolkit-google-cloud-platform-0.8.2/chaostoolkit_google_cloud_platform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-02-08 15:41:44.000000 chaostoolkit-google-cloud-platform-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:41:44.000000 chaostoolkit-google-cloud-platform-0.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:41:44.000000 chaostoolkit-google-cloud-platform-0.8.2/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/tests/fixtures/cloudbuild.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/tests/fixtures/cloudrun.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/tests/fixtures/fake_creds.json
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/tests/fixtures/nodepool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/tests/fixtures/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/tests/fixtures/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/tests/test_cloudbuild.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/tests/test_cloudrun.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/tests/test_creds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/tests/test_nodepool.py
--rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/tests/test_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-02-08 15:41:22.000000 chaostoolkit-google-cloud-platform-0.8.2/tests/test_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:11:43.000000 chaostoolkit-google-cloud-platform-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:11:43.000000 chaostoolkit-google-cloud-platform-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:11:43.000000 chaostoolkit-google-cloud-platform-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    12814 2023-05-18 21:11:43.000000 chaostoolkit-google-cloud-platform-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11495 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:11:43.000000 chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     9213 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:11:43.000000 chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/artifact/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/artifact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/artifact/probes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:11:43.000000 chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/cloudbuild/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/cloudbuild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/cloudbuild/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/cloudbuild/probes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:11:43.000000 chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/cloudlogging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/cloudlogging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/cloudlogging/probes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:11:43.000000 chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/cloudrun/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/cloudrun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/cloudrun/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/cloudrun/probes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:11:43.000000 chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/gke/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/gke/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:11:43.000000 chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/gke/nodepool/
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/gke/nodepool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/gke/nodepool/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/gke/nodepool/probes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:11:43.000000 chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/monitoring/probes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:11:43.000000 chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12643 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/sql/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/sql/probes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:11:43.000000 chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/storage/probes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:11:43.000000 chaostoolkit-google-cloud-platform-0.9.0/chaostoolkit_google_cloud_platform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12814 2023-05-18 21:11:43.000000 chaostoolkit-google-cloud-platform-0.9.0/chaostoolkit_google_cloud_platform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-18 21:11:43.000000 chaostoolkit-google-cloud-platform-0.9.0/chaostoolkit_google_cloud_platform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 21:11:43.000000 chaostoolkit-google-cloud-platform-0.9.0/chaostoolkit_google_cloud_platform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-18 21:11:43.000000 chaostoolkit-google-cloud-platform-0.9.0/chaostoolkit_google_cloud_platform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-18 21:11:43.000000 chaostoolkit-google-cloud-platform-0.9.0/chaostoolkit_google_cloud_platform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-18 21:11:43.000000 chaostoolkit-google-cloud-platform-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:11:43.000000 chaostoolkit-google-cloud-platform-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:11:43.000000 chaostoolkit-google-cloud-platform-0.9.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/tests/fixtures/cloudbuild.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/tests/fixtures/cloudrun.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/tests/fixtures/fake_creds.json
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/tests/fixtures/nodepool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/tests/fixtures/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/tests/fixtures/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/tests/test_cloudbuild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/tests/test_cloudrun.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/tests/test_creds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/tests/test_nodepool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/tests/test_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-18 21:11:30.000000 chaostoolkit-google-cloud-platform-0.9.0/tests/test_storage.py
```

### Comparing `chaostoolkit-google-cloud-platform-0.8.2/.github/workflows/build.yaml` & `chaostoolkit-google-cloud-platform-0.9.0/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `chaostoolkit-google-cloud-platform-0.8.2/.github/workflows/release.yaml` & `chaostoolkit-google-cloud-platform-0.9.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `chaostoolkit-google-cloud-platform-0.8.2/.gitignore` & `chaostoolkit-google-cloud-platform-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `chaostoolkit-google-cloud-platform-0.8.2/CHANGELOG.md` & `chaostoolkit-google-cloud-platform-0.9.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 # Changelog
 
 ## [Unreleased][]
 
-[Unreleased]: https://github.com/chaostoolkit-incubator/chaostoolkit-google-cloud-platform/compare/0.8.2...HEAD
+[Unreleased]: https://github.com/chaostoolkit-incubator/chaostoolkit-google-cloud-platform/compare/0.9.0...HEAD
+
+## [0.9.0][] - 2023-05-18
+
+[0.9.0]: https://github.com/chaostoolkit-incubator/chaostoolkit-google-cloud-platform/compare/0.8.2...0.9.0
+
+### Added
+
+* Probes to list docker images and their vulnerabilities from Artifact Registry
 
 ## [0.8.2][] - 2023-02-08
 
 [0.8.2]: https://github.com/chaostoolkit-incubator/chaostoolkit-google-cloud-platform/compare/0.8.1...0.8.2
 
 ### Changed
```

### Comparing `chaostoolkit-google-cloud-platform-0.8.2/LICENSE` & `chaostoolkit-google-cloud-platform-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chaostoolkit-google-cloud-platform-0.8.2/Makefile` & `chaostoolkit-google-cloud-platform-0.9.0/Makefile`

 * *Files identical despite different names*

### Comparing `chaostoolkit-google-cloud-platform-0.8.2/PKG-INFO` & `chaostoolkit-google-cloud-platform-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaostoolkit-google-cloud-platform
-Version: 0.8.2
+Version: 0.9.0
 Summary: Google Cloud Platform extension for the Chaos Toolkit
 Home-page: https://chaostoolkit.org
 Author: Chaos Toolkit
 Author-email: contact@chaostoolkit.org
 License: Apache License Version 2.0
 Project-URL: Docs: RTD, https://chaostoolkit.org/drivers/gcp/
 Project-URL: GitHub: issues, https://github.com/chaostoolkit-incubator/chaostoolkit-google-cloud-platform/issues
```

### Comparing `chaostoolkit-google-cloud-platform-0.8.2/README.md` & `chaostoolkit-google-cloud-platform-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/__init__.py` & `chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     "get_service",
     "wait_on_operation",
     "load_credentials",
     "to_dict",
     "context_from_parent_path",
     "parse_interval",
 ]
-__version__ = "0.8.2"
+__version__ = "0.9.0"
 
 
 def get_service(
     service_name: str,
     version: str = "v1",
     configuration: Configuration = None,
     secrets: Secrets = None,
@@ -296,8 +296,9 @@
     activities.extend(discover_probes("chaosgcp.storage.probes"))
     activities.extend(discover_actions("chaosgcp.cloudbuild.actions"))
     activities.extend(discover_probes("chaosgcp.cloudbuild.probes"))
     activities.extend(discover_actions("chaosgcp.cloudrun.actions"))
     activities.extend(discover_probes("chaosgcp.cloudrun.probes"))
     activities.extend(discover_probes("chaosgcp.monitoring.probes"))
     activities.extend(discover_probes("chaosgcp.cloudlogging.probes"))
+    activities.extend(discover_probes("chaosgcp.artifact.probes"))
     return activities
```

### Comparing `chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/cloudbuild/actions.py` & `chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/cloudbuild/actions.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/cloudbuild/probes.py` & `chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/cloudbuild/probes.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/cloudlogging/probes.py` & `chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/cloudlogging/probes.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/cloudrun/actions.py` & `chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/cloudrun/actions.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/cloudrun/probes.py` & `chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/cloudrun/probes.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/gke/nodepool/__init__.py` & `chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/gke/nodepool/__init__.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/gke/nodepool/actions.py` & `chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/gke/nodepool/actions.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/gke/nodepool/probes.py` & `chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/gke/nodepool/probes.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/monitoring/probes.py` & `chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/monitoring/probes.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/sql/actions.py` & `chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/sql/actions.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/sql/probes.py` & `chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/sql/probes.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/storage/__init__.py` & `chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/storage/probes.py` & `chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/storage/probes.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-google-cloud-platform-0.8.2/chaosgcp/types.py` & `chaostoolkit-google-cloud-platform-0.9.0/chaosgcp/types.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-google-cloud-platform-0.8.2/chaostoolkit_google_cloud_platform.egg-info/PKG-INFO` & `chaostoolkit-google-cloud-platform-0.9.0/chaostoolkit_google_cloud_platform.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaostoolkit-google-cloud-platform
-Version: 0.8.2
+Version: 0.9.0
 Summary: Google Cloud Platform extension for the Chaos Toolkit
 Home-page: https://chaostoolkit.org
 Author: Chaos Toolkit
 Author-email: contact@chaostoolkit.org
 License: Apache License Version 2.0
 Project-URL: Docs: RTD, https://chaostoolkit.org/drivers/gcp/
 Project-URL: GitHub: issues, https://github.com/chaostoolkit-incubator/chaostoolkit-google-cloud-platform/issues
```

### Comparing `chaostoolkit-google-cloud-platform-0.8.2/chaostoolkit_google_cloud_platform.egg-info/SOURCES.txt` & `chaostoolkit-google-cloud-platform-0.9.0/chaostoolkit_google_cloud_platform.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 requirements.txt
 setup.cfg
 setup.py
 .github/workflows/build.yaml
 .github/workflows/release.yaml
 chaosgcp/__init__.py
 chaosgcp/types.py
+chaosgcp/artifact/__init__.py
+chaosgcp/artifact/probes.py
 chaosgcp/cloudbuild/__init__.py
 chaosgcp/cloudbuild/actions.py
 chaosgcp/cloudbuild/probes.py
 chaosgcp/cloudlogging/__init__.py
 chaosgcp/cloudlogging/probes.py
 chaosgcp/cloudrun/__init__.py
 chaosgcp/cloudrun/actions.py
```

### Comparing `chaostoolkit-google-cloud-platform-0.8.2/setup.cfg` & `chaostoolkit-google-cloud-platform-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `chaostoolkit-google-cloud-platform-0.8.2/tests/fixtures/cloudbuild.py` & `chaostoolkit-google-cloud-platform-0.9.0/tests/fixtures/cloudbuild.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-google-cloud-platform-0.8.2/tests/fixtures/cloudrun.py` & `chaostoolkit-google-cloud-platform-0.9.0/tests/fixtures/cloudrun.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-google-cloud-platform-0.8.2/tests/fixtures/nodepool.py` & `chaostoolkit-google-cloud-platform-0.9.0/tests/fixtures/nodepool.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-google-cloud-platform-0.8.2/tests/fixtures/sql.py` & `chaostoolkit-google-cloud-platform-0.9.0/tests/fixtures/sql.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-google-cloud-platform-0.8.2/tests/test_cloudbuild.py` & `chaostoolkit-google-cloud-platform-0.9.0/tests/test_cloudbuild.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-google-cloud-platform-0.8.2/tests/test_cloudrun.py` & `chaostoolkit-google-cloud-platform-0.9.0/tests/test_cloudrun.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-google-cloud-platform-0.8.2/tests/test_creds.py` & `chaostoolkit-google-cloud-platform-0.9.0/tests/test_creds.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-google-cloud-platform-0.8.2/tests/test_helpers.py` & `chaostoolkit-google-cloud-platform-0.9.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-google-cloud-platform-0.8.2/tests/test_nodepool.py` & `chaostoolkit-google-cloud-platform-0.9.0/tests/test_nodepool.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-google-cloud-platform-0.8.2/tests/test_sql.py` & `chaostoolkit-google-cloud-platform-0.9.0/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-google-cloud-platform-0.8.2/tests/test_storage.py` & `chaostoolkit-google-cloud-platform-0.9.0/tests/test_storage.py`

 * *Files identical despite different names*

