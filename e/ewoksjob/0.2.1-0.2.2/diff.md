# Comparing `tmp/ewoksjob-0.2.1.tar.gz` & `tmp/ewoksjob-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ewoksjob-0.2.1.tar", last modified: Fri Mar 24 16:25:25 2023, max compression
+gzip compressed data, was "dist/ewoksjob-0.2.2.tar", last modified: Thu May 18 07:29:48 2023, max compression
```

## Comparing `ewoksjob-0.2.1.tar` & `ewoksjob-0.2.2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 16:25:25.000000 ewoksjob-0.2.1/
--rw-rw-rw-   0 root         (0) root         (0)     1102 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     2627 2023-03-24 16:25:25.000000 ewoksjob-0.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1707 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1751 2023-03-24 16:25:25.000000 ewoksjob-0.2.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 16:25:25.000000 ewoksjob-0.2.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 16:25:25.000000 ewoksjob-0.2.1/src/ewoksjob/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-03-24 16:19:17.000000 ewoksjob-0.2.1/src/ewoksjob/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/src/ewoksjob/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 16:25:25.000000 ewoksjob-0.2.1/src/ewoksjob/apps/
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/src/ewoksjob/apps/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1654 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/src/ewoksjob/apps/ewoks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 16:25:25.000000 ewoksjob-0.2.1/src/ewoksjob/client/
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/src/ewoksjob/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 16:25:25.000000 ewoksjob-0.2.1/src/ewoksjob/client/celery/
--rw-rw-rw-   0 root         (0) root         (0)      554 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/src/ewoksjob/client/celery/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1066 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/src/ewoksjob/client/celery/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     1406 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/src/ewoksjob/client/celery/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 16:25:25.000000 ewoksjob-0.2.1/src/ewoksjob/client/local/
--rw-rw-rw-   0 root         (0) root         (0)      374 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/src/ewoksjob/client/local/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4410 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/src/ewoksjob/client/local/pool.py
--rw-rw-rw-   0 root         (0) root         (0)     1940 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/src/ewoksjob/client/local/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     1068 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/src/ewoksjob/client/local/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1081 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/src/ewoksjob/client/test_workflow.py
--rw-rw-rw-   0 root         (0) root         (0)     5172 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/src/ewoksjob/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 16:25:25.000000 ewoksjob-0.2.1/src/ewoksjob/events/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-24 16:25:19.000000 ewoksjob-0.2.1/src/ewoksjob/events/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 16:25:25.000000 ewoksjob-0.2.1/src/ewoksjob/events/handlers/
--rw-rw-rw-   0 root         (0) root         (0)      108 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/src/ewoksjob/events/handlers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1904 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/src/ewoksjob/events/handlers/redis.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 16:25:25.000000 ewoksjob-0.2.1/src/ewoksjob/events/readers/
--rw-rw-rw-   0 root         (0) root         (0)      554 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/src/ewoksjob/events/readers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5423 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/src/ewoksjob/events/readers/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1213 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/src/ewoksjob/events/readers/redis.py
--rw-rw-rw-   0 root         (0) root         (0)     1150 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/src/ewoksjob/events/readers/sqlite3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 16:25:25.000000 ewoksjob-0.2.1/src/ewoksjob/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-24 16:25:19.000000 ewoksjob-0.2.1/src/ewoksjob/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4472 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/src/ewoksjob/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     2092 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/src/ewoksjob/tests/test_cancel.py
--rw-rw-rw-   0 root         (0) root         (0)     2391 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/src/ewoksjob/tests/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)      665 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/src/ewoksjob/tests/test_convert.py
--rw-rw-rw-   0 root         (0) root         (0)     1365 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/src/ewoksjob/tests/test_convert_and_execute.py
--rw-rw-rw-   0 root         (0) root         (0)     2617 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/src/ewoksjob/tests/test_events.py
--rw-rw-rw-   0 root         (0) root         (0)      961 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/src/ewoksjob/tests/test_execute.py
--rw-rw-rw-   0 root         (0) root         (0)      925 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/src/ewoksjob/tests/test_execute_and_upload.py
--rw-rw-rw-   0 root         (0) root         (0)     1808 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/src/ewoksjob/tests/test_feedback.py
--rw-rw-rw-   0 root         (0) root         (0)      626 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/src/ewoksjob/tests/test_future.py
--rw-rw-rw-   0 root         (0) root         (0)      839 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/src/ewoksjob/tests/test_futures.py
--rw-rw-rw-   0 root         (0) root         (0)      482 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/src/ewoksjob/tests/test_task_discovery.py
--rw-rw-rw-   0 root         (0) root         (0)      989 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/src/ewoksjob/tests/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 16:25:25.000000 ewoksjob-0.2.1/src/ewoksjob/worker/
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/src/ewoksjob/worker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1557 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/src/ewoksjob/worker/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     5603 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/src/ewoksjob/worker/options.py
--rw-rw-rw-   0 root         (0) root         (0)     7410 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/src/ewoksjob/worker/process.py
--rw-rw-rw-   0 root         (0) root         (0)      409 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/src/ewoksjob/worker/process_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2637 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/src/ewoksjob/worker/slurm.py
--rw-rw-rw-   0 root         (0) root         (0)      614 2023-03-24 13:10:29.000000 ewoksjob-0.2.1/src/ewoksjob/worker/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 16:25:25.000000 ewoksjob-0.2.1/src/ewoksjob.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2627 2023-03-24 16:25:25.000000 ewoksjob-0.2.1/src/ewoksjob.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1707 2023-03-24 16:25:25.000000 ewoksjob-0.2.1/src/ewoksjob.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-24 16:25:25.000000 ewoksjob-0.2.1/src/ewoksjob.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-03-24 16:25:25.000000 ewoksjob-0.2.1/src/ewoksjob.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      834 2023-03-24 16:25:25.000000 ewoksjob-0.2.1/src/ewoksjob.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-03-24 16:25:25.000000 ewoksjob-0.2.1/src/ewoksjob.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     2627 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1707 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1669 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/src/ewoksjob/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/src/ewoksjob/apps/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/apps/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1654 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/apps/ewoks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/src/ewoksjob/client/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/src/ewoksjob/client/celery/
+-rw-rw-rw-   0 root         (0) root         (0)      554 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/client/celery/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/client/celery/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1406 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/client/celery/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1083 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/client/dummy_workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/src/ewoksjob/client/local/
+-rw-rw-rw-   0 root         (0) root         (0)      374 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/client/local/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4410 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/client/local/pool.py
+-rw-rw-rw-   0 root         (0) root         (0)     1943 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/client/local/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/client/local/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5172 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/src/ewoksjob/events/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-18 07:29:42.000000 ewoksjob-0.2.2/src/ewoksjob/events/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/src/ewoksjob/events/handlers/
+-rw-rw-rw-   0 root         (0) root         (0)      108 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/events/handlers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1904 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/events/handlers/redis.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/src/ewoksjob/events/readers/
+-rw-rw-rw-   0 root         (0) root         (0)      554 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/events/readers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5423 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/events/readers/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1213 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/events/readers/redis.py
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/events/readers/sqlite3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/src/ewoksjob/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-18 07:29:42.000000 ewoksjob-0.2.2/src/ewoksjob/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4472 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2092 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/tests/test_cancel.py
+-rw-rw-rw-   0 root         (0) root         (0)     2391 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/tests/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      665 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/tests/test_convert.py
+-rw-rw-rw-   0 root         (0) root         (0)     1365 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/tests/test_convert_and_execute.py
+-rw-rw-rw-   0 root         (0) root         (0)     2617 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/tests/test_events.py
+-rw-rw-rw-   0 root         (0) root         (0)      961 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/tests/test_execute.py
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/tests/test_execute_and_upload.py
+-rw-rw-rw-   0 root         (0) root         (0)     1814 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/tests/test_feedback.py
+-rw-rw-rw-   0 root         (0) root         (0)      626 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/tests/test_future.py
+-rw-rw-rw-   0 root         (0) root         (0)      839 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/tests/test_futures.py
+-rw-rw-rw-   0 root         (0) root         (0)      482 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/tests/test_task_discovery.py
+-rw-rw-rw-   0 root         (0) root         (0)      989 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/src/ewoksjob/worker/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/worker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1557 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/worker/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     5824 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/worker/options.py
+-rw-rw-rw-   0 root         (0) root         (0)     7410 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/worker/process.py
+-rw-rw-rw-   0 root         (0) root         (0)      409 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/worker/process_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2637 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/worker/slurm.py
+-rw-rw-rw-   0 root         (0) root         (0)      614 2023-05-18 07:24:07.000000 ewoksjob-0.2.2/src/ewoksjob/worker/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/src/ewoksjob.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2627 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/src/ewoksjob.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1708 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/src/ewoksjob.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/src/ewoksjob.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/src/ewoksjob.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      835 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/src/ewoksjob.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-18 07:29:48.000000 ewoksjob-0.2.2/src/ewoksjob.egg-info/top_level.txt
```

### Comparing `ewoksjob-0.2.1/LICENSE.md` & `ewoksjob-0.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.1/PKG-INFO` & `ewoksjob-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksjob
-Version: 0.2.1
+Version: 0.2.2
 Summary: Asynchronous and distributed scheduling of Ewoks workflows from python
 Home-page: https://gitlab.esrf.fr/workflow/ewoks/ewoksjob/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoks/ewoksjob/
 Project-URL: Documentation, https://ewoksjob.readthedocs.io/
```

### Comparing `ewoksjob-0.2.1/README.md` & `ewoksjob-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.1/setup.cfg` & `ewoksjob-0.2.2/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -19,27 +19,27 @@
 
 [options]
 package_dir = 
 	=src
 packages = find:
 python_requires = >=3.6
 install_requires = 
-	celery[tblib] >= 5
+	celery[tblib] >= 5,!=5.3.0rc1
 	importlib-metadata<5.0; python_version<"3.8"
 	ewoksutils >=0.1.1
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 worker = 
 	ewokscore >=0.3.2
 	ewoks >=0.1.5
 redis = 
-	redis <4.5
+	redis <5
 sql = 
 	sqlalchemy <2
 monitor = 
 	flower
 slurm = 
 	pyslurmutils >=0.1.0rc
 	gevent
@@ -75,19 +75,14 @@
 
 [flake8]
 ignore = E501, E203, W503
 max-line-length = 88
 exclude = 
 	.eggs
 
-[build_sphinx]
-project = ewoksjob
-version = attr: ewoksjob.__version__
-source-dir = ./doc
-
 [coverage:run]
 omit = 
 	setup.py
 	*/tests/*
 
 [tool:pytest]
 redis_exec = redis-server
```

### Comparing `ewoksjob-0.2.1/src/ewoksjob/__main__.py` & `ewoksjob-0.2.2/src/ewoksjob/__main__.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.1/src/ewoksjob/apps/ewoks.py` & `ewoksjob-0.2.2/src/ewoksjob/apps/ewoks.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.1/src/ewoksjob/client/celery/__init__.py` & `ewoksjob-0.2.2/src/ewoksjob/client/celery/__init__.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.1/src/ewoksjob/client/celery/tasks.py` & `ewoksjob-0.2.2/src/ewoksjob/client/celery/tasks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from celery.execute import send_task
 from celery.result import AsyncResult
-from ..test_workflow import test_workflow
+from ..dummy_workflow import dummy_workflow
 
 __all__ = [
     "execute_graph",
     "execute_test_graph",
     "convert_workflow",
     "discover_tasks_from_modules",
 ]
@@ -15,15 +15,15 @@
 
 
 def execute_test_graph(
     seconds=0, filename=None, args=None, kwargs=None, **kw
 ) -> AsyncResult:
     if args:
         raise TypeError("execute_test_graph does not take position arguments")
-    args = (test_workflow(),)
+    args = (dummy_workflow(),)
     if kwargs is None:
         kwargs = dict()
     kwargs["inputs"] = [
         {"id": "sleep", "name": 0, "value": seconds},
         {"id": "result", "name": "filename", "value": filename},
     ]
     return execute_graph(args=args, kwargs=kwargs, **kw)
```

### Comparing `ewoksjob-0.2.1/src/ewoksjob/client/celery/utils.py` & `ewoksjob-0.2.2/src/ewoksjob/client/celery/utils.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.1/src/ewoksjob/client/local/pool.py` & `ewoksjob-0.2.2/src/ewoksjob/client/local/pool.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.1/src/ewoksjob/client/local/tasks.py` & `ewoksjob-0.2.2/src/ewoksjob/client/local/tasks.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Callable, Mapping, Optional, Tuple
 from concurrent.futures import Future
 
 import ewoks
 from ewokscore import task_discovery
 
 from .pool import get_active_pool
-from ..test_workflow import test_workflow
+from ..dummy_workflow import dummy_workflow
 
 
 __all__ = [
     "execute_graph",
     "execute_test_graph",
     "convert_workflow",
     "discover_tasks_from_modules",
@@ -22,15 +22,15 @@
 ) -> Future:
     return _submit_with_jobid(ewoks.execute_graph, args=args, kwargs=kwargs)
 
 
 def execute_test_graph(
     seconds=0, filename=None, kwargs: Optional[Mapping] = None
 ) -> Future:
-    args = (test_workflow(),)
+    args = (dummy_workflow(),)
     if kwargs is None:
         kwargs = dict()
     kwargs["inputs"] = [
         {"id": "sleep", "name": 0, "value": seconds},
         {"id": "result", "name": "filename", "value": filename},
     ]
     return execute_graph(args=args, kwargs=kwargs)
```

### Comparing `ewoksjob-0.2.1/src/ewoksjob/client/local/utils.py` & `ewoksjob-0.2.2/src/ewoksjob/client/local/utils.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.1/src/ewoksjob/client/test_workflow.py` & `ewoksjob-0.2.2/src/ewoksjob/client/dummy_workflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 def result(value=False, filename=None):
     if filename:
         with open(filename, "w"):
             pass
     return value is None
 
 
-def test_workflow():
+def dummy_workflow():
     return {
         "graph": {"id": "sleepgraph", "schema_version": "1.0"},
         "nodes": [
             {
                 "id": "sleep",
                 "task_type": "method",
                 "task_identifier": "time.sleep",
                 "default_inputs": [{"name": 0, "value": 0}],
             },
             {
                 "id": "result",
                 "task_type": "method",
-                "task_identifier": "ewoksjob.client.test_workflow.result",
+                "task_identifier": "ewoksjob.client.dummy_workflow.result",
                 "default_inputs": [
                     {"name": "value", "value": None},
                     {"name": "filename", "value": None},
                 ],
             },
         ],
         "links": [
```

### Comparing `ewoksjob-0.2.1/src/ewoksjob/config.py` & `ewoksjob-0.2.2/src/ewoksjob/config.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.1/src/ewoksjob/events/handlers/redis.py` & `ewoksjob-0.2.2/src/ewoksjob/events/handlers/redis.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.1/src/ewoksjob/events/readers/__init__.py` & `ewoksjob-0.2.2/src/ewoksjob/events/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.1/src/ewoksjob/events/readers/base.py` & `ewoksjob-0.2.2/src/ewoksjob/events/readers/base.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.1/src/ewoksjob/events/readers/redis.py` & `ewoksjob-0.2.2/src/ewoksjob/events/readers/redis.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.1/src/ewoksjob/events/readers/sqlite3.py` & `ewoksjob-0.2.2/src/ewoksjob/events/readers/sqlite3.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.1/src/ewoksjob/tests/conftest.py` & `ewoksjob-0.2.2/src/ewoksjob/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.1/src/ewoksjob/tests/test_cancel.py` & `ewoksjob-0.2.2/src/ewoksjob/tests/test_cancel.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.1/src/ewoksjob/tests/test_config.py` & `ewoksjob-0.2.2/src/ewoksjob/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.1/src/ewoksjob/tests/test_convert.py` & `ewoksjob-0.2.2/src/ewoksjob/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.1/src/ewoksjob/tests/test_convert_and_execute.py` & `ewoksjob-0.2.2/src/ewoksjob/tests/test_convert_and_execute.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.1/src/ewoksjob/tests/test_events.py` & `ewoksjob-0.2.2/src/ewoksjob/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.1/src/ewoksjob/tests/test_execute.py` & `ewoksjob-0.2.2/src/ewoksjob/tests/test_execute.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.1/src/ewoksjob/tests/test_execute_and_upload.py` & `ewoksjob-0.2.2/src/ewoksjob/tests/test_execute_and_upload.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 import time
+
 import pytest
 from ewokscore.tests.examples.graphs import get_graph
+
+try:
+    import pyicat_plus  # noqa F401
+
+    ICAT_ERROR_MSG = "The message queue URL's are missing"
+except ImportError:
+    ICAT_ERROR_MSG = "requires pyicat-plus"
+
 from ..client import celery
 from ..client import local
 from .utils import get_result
 
 
 def test_submit(ewoks_worker):
     assert_submit(celery)
@@ -25,9 +34,9 @@
             "dataset": "testdataset",
             "path": "/path/to/localed/dataset",
             "metadata": {"Sample_name": "test"},
             "raw": "/path/to/raw/dataset",
         }
     }
     future1 = mod.submit(args=(graph,), kwargs=kwargs)
-    with pytest.raises(RuntimeError, match="requires pyicat-plus"):
+    with pytest.raises(RuntimeError, match=ICAT_ERROR_MSG):
         get_result(future1, timeout=10)
```

### Comparing `ewoksjob-0.2.1/src/ewoksjob/tests/test_feedback.py` & `ewoksjob-0.2.2/src/ewoksjob/tests/test_feedback.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,8 +54,8 @@
 
     assert len(list(reader.get_events_with_variables())) == 6
 
     evts = list(reader.get_events_with_variables(node_id="task", type="start"))
     assert len(evts) == 1
 
     event_values = evts[0]["outputs"]
-    assert event_values.variable_values == {"sum": 3}
+    assert event_values.get_variable_values() == {"sum": 3}
```

### Comparing `ewoksjob-0.2.1/src/ewoksjob/tests/test_future.py` & `ewoksjob-0.2.2/src/ewoksjob/tests/test_future.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.1/src/ewoksjob/tests/test_futures.py` & `ewoksjob-0.2.2/src/ewoksjob/tests/test_futures.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.1/src/ewoksjob/tests/utils.py` & `ewoksjob-0.2.2/src/ewoksjob/tests/utils.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.1/src/ewoksjob/worker/errors.py` & `ewoksjob-0.2.2/src/ewoksjob/worker/errors.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.1/src/ewoksjob/worker/options.py` & `ewoksjob-0.2.2/src/ewoksjob/worker/options.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import getpass
-from typing import Dict
+import json
+from typing import Dict, Tuple, Any
 from multiprocessing import get_context
 from multiprocessing import get_all_start_methods
 
 from click import Choice
 from celery import Celery
 from celery import bootsteps
 from celery import concurrency
@@ -99,18 +100,18 @@
             required=False,
             help="Script to be executes after each SLURM job",
             help_group="Slurm Pool Options",
         )
     )
     app.user_options["preload"].add(
         CeleryOption(
-            ["-sp", "--slurm-parameters"],
+            ["-sp", "--slurm-parameter", "slurm_parameters"],
             required=False,
             multiple=True,
-            help="SLURM job parameters (-sp NAME=VALUE). See https://slurm.schedmd.com/rest_api.html#v0.0.38_job_properties",
+            help="SLURM job parameters (-sp NAME=VALUE).",
             help_group="Slurm Pool Options",
         )
     )
     app.user_options["preload"].add(
         CeleryOption(
             ["--slurm-python-cmd"],
             required=False,
@@ -158,19 +159,32 @@
 
 def _extract_slurm_options(options: Dict) -> dict:
     slurm_options = {
         name: options.get(option) for option, name in SLURM_NAME_MAP.items()
     }
     parameters = slurm_options.pop("parameters", None)
     if parameters:
-        parameters = [s.partition("=") for s in parameters]
-        slurm_options["parameters"] = {p[0]: p[2] for p in parameters if p[2]}
+        slurm_options["parameters"] = dict(
+            _parse_slurm_parameter(p) for p in parameters
+        )
     return slurm_options
 
 
+def _parse_slurm_parameter(parameter: str) -> Tuple[str, Any]:
+    name, _, value = parameter.partition("=")
+    return name, _parse_value(value)
+
+
+def _parse_value(value: str) -> Any:
+    try:
+        return json.loads(value)
+    except Exception:
+        return value
+
+
 PROCESS_NAME_MAP = {
     "process_context": "context",
     "process_no_precreate": "precreate",
 }
 
 
 def _extract_process_options(options: Dict) -> dict:
```

### Comparing `ewoksjob-0.2.1/src/ewoksjob/worker/process.py` & `ewoksjob-0.2.2/src/ewoksjob/worker/process.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.1/src/ewoksjob/worker/slurm.py` & `ewoksjob-0.2.2/src/ewoksjob/worker/slurm.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.1/src/ewoksjob/worker/task.py` & `ewoksjob-0.2.2/src/ewoksjob/worker/task.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.1/src/ewoksjob.egg-info/PKG-INFO` & `ewoksjob-0.2.2/src/ewoksjob.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksjob
-Version: 0.2.1
+Version: 0.2.2
 Summary: Asynchronous and distributed scheduling of Ewoks workflows from python
 Home-page: https://gitlab.esrf.fr/workflow/ewoks/ewoksjob/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoks/ewoksjob/
 Project-URL: Documentation, https://ewoksjob.readthedocs.io/
```

### Comparing `ewoksjob-0.2.1/src/ewoksjob.egg-info/SOURCES.txt` & `ewoksjob-0.2.2/src/ewoksjob.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 src/ewoksjob.egg-info/dependency_links.txt
 src/ewoksjob.egg-info/entry_points.txt
 src/ewoksjob.egg-info/requires.txt
 src/ewoksjob.egg-info/top_level.txt
 src/ewoksjob/apps/__init__.py
 src/ewoksjob/apps/ewoks.py
 src/ewoksjob/client/__init__.py
-src/ewoksjob/client/test_workflow.py
+src/ewoksjob/client/dummy_workflow.py
 src/ewoksjob/client/celery/__init__.py
 src/ewoksjob/client/celery/tasks.py
 src/ewoksjob/client/celery/utils.py
 src/ewoksjob/client/local/__init__.py
 src/ewoksjob/client/local/pool.py
 src/ewoksjob/client/local/tasks.py
 src/ewoksjob/client/local/utils.py
```

### Comparing `ewoksjob-0.2.1/src/ewoksjob.egg-info/requires.txt` & `ewoksjob-0.2.2/src/ewoksjob.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-celery[tblib]>=5
+celery[tblib]!=5.3.0rc1,>=5
 ewoksutils>=0.1.1
 
 [:python_version < "3.8"]
 importlib-metadata<5.0
 
 [beacon]
 blissdata
 
 [blissworker]
 ewokscore>=0.3.2
 ewoks>=0.1.5
-redis<4.5
+redis<5
 blissdata
 pyslurmutils>=0.1.0rc
 gevent
 flower
 ewoks[esrf-data-portal]
 
 [dev]
 ewokscore>=0.3.2
 ewoks>=0.1.5
-redis<4.5
+redis<5
 blissdata
 pyslurmutils>=0.1.0rc
 gevent
 flower
 ewoks[esrf-data-portal]
 sqlalchemy<2
 pytest>=7
@@ -33,35 +33,35 @@
 pytest-mock
 black>=22
 flake8>=4
 
 [doc]
 ewokscore>=0.3.2
 ewoks>=0.1.5
-redis<4.5
+redis<5
 sphinx>=4.5
 sphinx-autodoc-typehints>=1.16
 
 [monitor]
 flower
 
 [redis]
-redis<4.5
+redis<5
 
 [slurm]
 pyslurmutils>=0.1.0rc
 gevent
 
 [sql]
 sqlalchemy<2
 
 [test]
 ewokscore>=0.3.2
 ewoks>=0.1.5
-redis<4.5
+redis<5
 blissdata
 pyslurmutils>=0.1.0rc
 gevent
 flower
 ewoks[esrf-data-portal]
 sqlalchemy<2
 pytest>=7
```

