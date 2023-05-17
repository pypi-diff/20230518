# Comparing `tmp/adaptive_scheduler-2.0.0.tar.gz` & `tmp/adaptive_scheduler-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adaptive_scheduler-2.0.0.tar", last modified: Thu May 11 23:59:29 2023, max compression
+gzip compressed data, was "adaptive_scheduler-2.0.1.tar", last modified: Wed May 17 22:57:18 2023, max compression
```

## Comparing `adaptive_scheduler-2.0.0.tar` & `adaptive_scheduler-2.0.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:59:29.853717 adaptive_scheduler-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-11 23:59:29.853717 adaptive_scheduler-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8242 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:59:29.857717 adaptive_scheduler-2.0.0/adaptive_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7755 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/_mock_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:59:29.845717 adaptive_scheduler-2.0.0/adaptive_scheduler/_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12733 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/_scheduler/base_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/_scheduler/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/_scheduler/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/_scheduler/pbs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/_scheduler/slurm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:59:29.849717 adaptive_scheduler-2.0.0/adaptive_scheduler/_server_support/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/_server_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/_server_support/base_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/_server_support/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13255 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/_server_support/database_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/_server_support/job_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/_server_support/kill_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/_server_support/launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/_server_support/parse_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21460 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/_server_support/run_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/_server_support/slurm_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-11 23:59:29.857717 adaptive_scheduler-2.0.0/adaptive_scheduler/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/client_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/server_support.py
--rw-r--r--   0 runner    (1001) docker     (123)    35819 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    32694 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:59:29.845717 adaptive_scheduler-2.0.0/adaptive_scheduler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-11 23:59:29.000000 adaptive_scheduler-2.0.0/adaptive_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-11 23:59:29.000000 adaptive_scheduler-2.0.0/adaptive_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 23:59:29.000000 adaptive_scheduler-2.0.0/adaptive_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-11 23:59:29.000000 adaptive_scheduler-2.0.0/adaptive_scheduler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-11 23:59:29.000000 adaptive_scheduler-2.0.0/adaptive_scheduler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 23:59:29.000000 adaptive_scheduler-2.0.0/adaptive_scheduler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-11 23:59:29.853717 adaptive_scheduler-2.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      523 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:59:29.853717 adaptive_scheduler-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/tests/test_base_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/tests/test_client_support.py
--rw-r--r--   0 runner    (1001) docker     (123)    13256 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/tests/test_database_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/tests/test_job_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/tests/test_kill_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/tests/test_launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/tests/test_log_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/tests/test_log_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    10239 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/tests/test_run_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/tests/test_server_support_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     8312 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/tests/test_slurm_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8731 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/tests/test_slurm_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    16970 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10801 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/tests/test_widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:57:18.053563 adaptive_scheduler-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-17 22:57:18.053563 adaptive_scheduler-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8242 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:57:18.053563 adaptive_scheduler-2.0.1/adaptive_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7755 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/_mock_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:57:18.045563 adaptive_scheduler-2.0.1/adaptive_scheduler/_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12733 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/_scheduler/base_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/_scheduler/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/_scheduler/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/_scheduler/pbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/_scheduler/slurm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:57:18.049563 adaptive_scheduler-2.0.1/adaptive_scheduler/_server_support/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/_server_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/_server_support/base_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/_server_support/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13282 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/_server_support/database_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/_server_support/job_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/_server_support/kill_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/_server_support/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/_server_support/parse_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21460 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/_server_support/run_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/_server_support/slurm_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-17 22:57:18.053563 adaptive_scheduler-2.0.1/adaptive_scheduler/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/client_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/server_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35819 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32694 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:57:18.045563 adaptive_scheduler-2.0.1/adaptive_scheduler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-17 22:57:18.000000 adaptive_scheduler-2.0.1/adaptive_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-17 22:57:18.000000 adaptive_scheduler-2.0.1/adaptive_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 22:57:18.000000 adaptive_scheduler-2.0.1/adaptive_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-17 22:57:18.000000 adaptive_scheduler-2.0.1/adaptive_scheduler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-17 22:57:18.000000 adaptive_scheduler-2.0.1/adaptive_scheduler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-17 22:57:18.000000 adaptive_scheduler-2.0.1/adaptive_scheduler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-17 22:57:18.053563 adaptive_scheduler-2.0.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      523 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:57:18.053563 adaptive_scheduler-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/tests/test_base_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/tests/test_client_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13256 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/tests/test_database_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/tests/test_job_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/tests/test_kill_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/tests/test_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/tests/test_log_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/tests/test_log_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10239 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/tests/test_run_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/tests/test_server_support_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8312 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/tests/test_slurm_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8731 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/tests/test_slurm_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16970 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10801 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/tests/test_widgets.py
```

### Comparing `adaptive_scheduler-2.0.0/LICENSE` & `adaptive_scheduler-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.0/PKG-INFO` & `adaptive_scheduler-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptive_scheduler
-Version: 2.0.0
+Version: 2.0.1
 Summary: Run many `adaptive.Learner`s on many cores (>10k) using `mpi4py.futures`, `ipyparallel`, `dask-mpi`, or `process-pool`.
 Maintainer-email: Bas Nijholt <bas@nijho.lt>
 License: BSD-3
 Project-URL: homepage, https://adaptive-scheduler.readthedocs.io/
 Project-URL: documentation, https://adaptive-scheduler.readthedocs.io/
 Project-URL: repository, https://github.com/basnijholt/adaptive-scheduler
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `adaptive_scheduler-2.0.0/README.md` & `adaptive_scheduler-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.0/adaptive_scheduler/_mock_scheduler.py` & `adaptive_scheduler-2.0.1/adaptive_scheduler/_mock_scheduler.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.0/adaptive_scheduler/_scheduler/base_scheduler.py` & `adaptive_scheduler-2.0.1/adaptive_scheduler/_scheduler/base_scheduler.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.0/adaptive_scheduler/_scheduler/common.py` & `adaptive_scheduler-2.0.1/adaptive_scheduler/_scheduler/common.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.0/adaptive_scheduler/_scheduler/local.py` & `adaptive_scheduler-2.0.1/adaptive_scheduler/_scheduler/local.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.0/adaptive_scheduler/_scheduler/pbs.py` & `adaptive_scheduler-2.0.1/adaptive_scheduler/_scheduler/pbs.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.0/adaptive_scheduler/_scheduler/slurm.py` & `adaptive_scheduler-2.0.1/adaptive_scheduler/_scheduler/slurm.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.0/adaptive_scheduler/_server_support/base_manager.py` & `adaptive_scheduler-2.0.1/adaptive_scheduler/_server_support/base_manager.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.0/adaptive_scheduler/_server_support/common.py` & `adaptive_scheduler-2.0.1/adaptive_scheduler/_server_support/common.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.0/adaptive_scheduler/_server_support/database_manager.py` & `adaptive_scheduler-2.0.1/adaptive_scheduler/_server_support/database_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,15 +183,16 @@
             self.learners,
             self.fnames,
             with_progress_bar=True,
         )
 
     def update(self, queue: dict[str, dict[str, str]] | None = None) -> None:
         """If the ``job_id`` isn't running anymore, replace it with None."""
-        assert self._db is not None
+        if self._db is None:
+            return
         if queue is None:
             queue = self.scheduler.queue(me_only=True)
         failed = self._db.get_all(
             lambda e: (e.job_id is not None) and (e.job_id not in queue),  # type: ignore[operator]
         )
         self.failed.extend([asdict(entry) for _, entry in failed])
         indices = [index for index, _ in failed]
@@ -218,15 +219,16 @@
         if self.db_fname.exists():
             self.db_fname.unlink()
         self._db = SimpleDatabase(self.db_fname)
         self._db.insert_multiple(entries)
 
     def as_dicts(self) -> list[dict[str, str]]:
         """Return the database as a list of dictionaries."""
-        assert self._db is not None
+        if self._db is None:
+            return []
         return self._db.as_dicts()
 
     def as_df(self) -> pd.DataFrame:
         """Return the database as a `pandas.DataFrame`."""
         return pd.DataFrame(self.as_dicts())
 
     def _output_logs(self, job_id: str, job_name: str) -> list[Path]:
```

### Comparing `adaptive_scheduler-2.0.0/adaptive_scheduler/_server_support/job_manager.py` & `adaptive_scheduler-2.0.1/adaptive_scheduler/_server_support/job_manager.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.0/adaptive_scheduler/_server_support/kill_manager.py` & `adaptive_scheduler-2.0.1/adaptive_scheduler/_server_support/kill_manager.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.0/adaptive_scheduler/_server_support/launcher.py` & `adaptive_scheduler-2.0.1/adaptive_scheduler/_server_support/launcher.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.0/adaptive_scheduler/_server_support/parse_logs.py` & `adaptive_scheduler-2.0.1/adaptive_scheduler/_server_support/parse_logs.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.0/adaptive_scheduler/_server_support/run_manager.py` & `adaptive_scheduler-2.0.1/adaptive_scheduler/_server_support/run_manager.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.0/adaptive_scheduler/_server_support/slurm_run.py` & `adaptive_scheduler-2.0.1/adaptive_scheduler/_server_support/slurm_run.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.0/adaptive_scheduler/client_support.py` & `adaptive_scheduler-2.0.1/adaptive_scheduler/client_support.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.0/adaptive_scheduler/scheduler.py` & `adaptive_scheduler-2.0.1/adaptive_scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.0/adaptive_scheduler/server_support.py` & `adaptive_scheduler-2.0.1/adaptive_scheduler/server_support.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.0/adaptive_scheduler/utils.py` & `adaptive_scheduler-2.0.1/adaptive_scheduler/utils.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.0/adaptive_scheduler/widgets.py` & `adaptive_scheduler-2.0.1/adaptive_scheduler/widgets.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.0/adaptive_scheduler.egg-info/PKG-INFO` & `adaptive_scheduler-2.0.1/adaptive_scheduler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptive-scheduler
-Version: 2.0.0
+Version: 2.0.1
 Summary: Run many `adaptive.Learner`s on many cores (>10k) using `mpi4py.futures`, `ipyparallel`, `dask-mpi`, or `process-pool`.
 Maintainer-email: Bas Nijholt <bas@nijho.lt>
 License: BSD-3
 Project-URL: homepage, https://adaptive-scheduler.readthedocs.io/
 Project-URL: documentation, https://adaptive-scheduler.readthedocs.io/
 Project-URL: repository, https://github.com/basnijholt/adaptive-scheduler
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `adaptive_scheduler-2.0.0/adaptive_scheduler.egg-info/SOURCES.txt` & `adaptive_scheduler-2.0.1/adaptive_scheduler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.0/pyproject.toml` & `adaptive_scheduler-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.0/setup.py` & `adaptive_scheduler-2.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.0/tests/test_base_scheduler.py` & `adaptive_scheduler-2.0.1/tests/test_base_scheduler.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.0/tests/test_client_support.py` & `adaptive_scheduler-2.0.1/tests/test_client_support.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.0/tests/test_database_manager.py` & `adaptive_scheduler-2.0.1/tests/test_database_manager.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.0/tests/test_job_manager.py` & `adaptive_scheduler-2.0.1/tests/test_job_manager.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.0/tests/test_kill_manager.py` & `adaptive_scheduler-2.0.1/tests/test_kill_manager.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.0/tests/test_launcher.py` & `adaptive_scheduler-2.0.1/tests/test_launcher.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.0/tests/test_log_generation.py` & `adaptive_scheduler-2.0.1/tests/test_log_generation.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.0/tests/test_log_parsing.py` & `adaptive_scheduler-2.0.1/tests/test_log_parsing.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.0/tests/test_run_manager.py` & `adaptive_scheduler-2.0.1/tests/test_run_manager.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.0/tests/test_server_support_common.py` & `adaptive_scheduler-2.0.1/tests/test_server_support_common.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.0/tests/test_slurm_run.py` & `adaptive_scheduler-2.0.1/tests/test_slurm_run.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.0/tests/test_slurm_scheduler.py` & `adaptive_scheduler-2.0.1/tests/test_slurm_scheduler.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.0/tests/test_utils.py` & `adaptive_scheduler-2.0.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.0/tests/test_widgets.py` & `adaptive_scheduler-2.0.1/tests/test_widgets.py`

 * *Files identical despite different names*

