# Comparing `tmp/tap-mixpanel-1.4.2.tar.gz` & `tmp/tap-mixpanel-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-mixpanel-1.4.2.tar", last modified: Tue May  2 18:04:21 2023, max compression
+gzip compressed data, was "dist/tap-mixpanel-1.4.3.tar", last modified: Thu May 18 11:02:27 2023, max compression
```

## Comparing `tap-mixpanel-1.4.2.tar` & `tap-mixpanel-1.4.3.tar`

### file list

```diff
@@ -1,50 +1,52 @@
-drwxrwxr-x   0 dsprayberry  (1001) dsprayberry  (1001)        0 2023-05-02 18:04:21.593726 tap-mixpanel-1.4.2/
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)    34523 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/LICENSE
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)       52 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/MANIFEST.in
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      249 2023-05-02 18:04:21.593726 tap-mixpanel-1.4.2/PKG-INFO
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)    12637 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/README.md
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      125 2023-05-02 18:04:21.593726 tap-mixpanel-1.4.2/setup.cfg
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      837 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/setup.py
-drwxrwxr-x   0 dsprayberry  (1001) dsprayberry  (1001)        0 2023-05-02 18:04:21.589726 tap-mixpanel-1.4.2/tap_mixpanel/
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     2778 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tap_mixpanel/__init__.py
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)    10077 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tap_mixpanel/client.py
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      686 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tap_mixpanel/discover.py
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     5787 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tap_mixpanel/schema.py
-drwxrwxr-x   0 dsprayberry  (1001) dsprayberry  (1001)        0 2023-05-02 18:04:21.589726 tap-mixpanel-1.4.2/tap_mixpanel/schemas/
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      335 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tap_mixpanel/schemas/annotations.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      199 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tap_mixpanel/schemas/cohort_members.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      510 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tap_mixpanel/schemas/cohorts.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      139 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tap_mixpanel/schemas/engage.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      603 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tap_mixpanel/schemas/export.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     3390 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tap_mixpanel/schemas/funnels.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      449 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tap_mixpanel/schemas/revenue.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)    26299 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tap_mixpanel/streams.py
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     1771 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tap_mixpanel/sync.py
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     3608 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tap_mixpanel/transform.py
-drwxrwxr-x   0 dsprayberry  (1001) dsprayberry  (1001)        0 2023-05-02 18:04:21.589726 tap-mixpanel-1.4.2/tap_mixpanel.egg-info/
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      249 2023-05-02 18:04:21.000000 tap-mixpanel-1.4.2/tap_mixpanel.egg-info/PKG-INFO
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     1258 2023-05-02 18:04:21.000000 tap-mixpanel-1.4.2/tap_mixpanel.egg-info/SOURCES.txt
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)        1 2023-05-02 18:04:21.000000 tap-mixpanel-1.4.2/tap_mixpanel.egg-info/dependency_links.txt
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)       51 2023-05-02 18:04:21.000000 tap-mixpanel-1.4.2/tap_mixpanel.egg-info/entry_points.txt
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)       99 2023-05-02 18:04:21.000000 tap-mixpanel-1.4.2/tap_mixpanel.egg-info/requires.txt
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)       19 2023-05-02 18:04:21.000000 tap-mixpanel-1.4.2/tap_mixpanel.egg-info/top_level.txt
-drwxrwxr-x   0 dsprayberry  (1001) dsprayberry  (1001)        0 2023-05-02 18:04:21.589726 tap-mixpanel-1.4.2/tests/
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)        0 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tests/__init__.py
-drwxrwxr-x   0 dsprayberry  (1001) dsprayberry  (1001)        0 2023-05-02 18:04:21.589726 tap-mixpanel-1.4.2/tests/configuration/
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)        0 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tests/configuration/__init__.py
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      443 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tests/configuration/fixtures.py
-drwxrwxr-x   0 dsprayberry  (1001) dsprayberry  (1001)        0 2023-05-02 18:04:21.593726 tap-mixpanel-1.4.2/tests/tap_tester/
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      164 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tests/tap_tester/__init__.py
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)    14803 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tests/tap_tester/base.py
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     7586 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tests/tap_tester/test_all_fields_pagination.py
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     2555 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tests/tap_tester/test_automatic_fields.py
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     8800 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tests/tap_tester/test_bookmark.py
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     7069 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tests/tap_tester/test_discovery.py
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     7517 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tests/tap_tester/test_start_date.py
-drwxrwxr-x   0 dsprayberry  (1001) dsprayberry  (1001)        0 2023-05-02 18:04:21.593726 tap-mixpanel-1.4.2/tests/unittests/
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)        0 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tests/unittests/__init__.py
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)    22322 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tests/unittests/test_error_handling.py
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     4732 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tests/unittests/test_medium_client.py
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     6150 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tests/unittests/test_request_timeout_param_value.py
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     5633 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tests/unittests/test_support_eu_endpoints.py
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     1107 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tests/unittests/test_transform_event_times.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-18 11:02:27.000000 tap-mixpanel-1.4.3/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       52 2022-10-10 07:35:16.000000 tap-mixpanel-1.4.3/MANIFEST.in
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-18 11:02:27.000000 tap-mixpanel-1.4.3/tests/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-18 11:02:27.000000 tap-mixpanel-1.4.3/tests/tap_tester/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7571 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tests/tap_tester/test_mixpanel_start_date.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2505 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tests/tap_tester/test_mixpanel_automatic_fields.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8220 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tests/tap_tester/test_mixpanel_discovery.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7470 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tests/tap_tester/test_mixpanel_all_fields_pagination.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8779 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tests/tap_tester/test_mixpanel_bookmark.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      164 2022-10-10 07:35:16.000000 tap-mixpanel-1.4.3/tests/tap_tester/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15519 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tests/tap_tester/base.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-10 07:35:16.000000 tap-mixpanel-1.4.3/tests/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-18 11:02:27.000000 tap-mixpanel-1.4.3/tests/unittests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4296 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tests/unittests/test_main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4819 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tests/unittests/test_sync.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2170 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tests/unittests/test_transform.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7646 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tests/unittests/test_support_eu_endpoints.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3438 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tests/unittests/test_request_timeout_param_value.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1523 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tests/unittests/test_transform_event_times.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5065 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tests/unittests/test_client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-10 07:35:16.000000 tap-mixpanel-1.4.3/tests/unittests/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1717 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tests/unittests/test_attribution_window.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11184 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tests/unittests/test_error_handling.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3709 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tests/unittests/test_discover.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      146 2023-05-18 11:02:27.000000 tap-mixpanel-1.4.3/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      304 2023-05-18 11:02:27.000000 tap-mixpanel-1.4.3/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      727 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/setup.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34523 2022-10-10 07:35:16.000000 tap-mixpanel-1.4.3/LICENSE
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-18 11:02:27.000000 tap-mixpanel-1.4.3/tap_mixpanel.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       71 2023-05-18 11:02:26.000000 tap-mixpanel-1.4.3/tap_mixpanel.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-18 11:02:26.000000 tap-mixpanel-1.4.3/tap_mixpanel.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       76 2023-05-18 11:02:26.000000 tap-mixpanel-1.4.3/tap_mixpanel.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      304 2023-05-18 11:02:26.000000 tap-mixpanel-1.4.3/tap_mixpanel.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1400 2023-05-18 11:02:26.000000 tap-mixpanel-1.4.3/tap_mixpanel.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       19 2023-05-18 11:02:26.000000 tap-mixpanel-1.4.3/tap_mixpanel.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12637 2023-05-03 05:08:09.000000 tap-mixpanel-1.4.3/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-18 11:02:27.000000 tap-mixpanel-1.4.3/tap_mixpanel/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5161 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tap_mixpanel/transform.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12294 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tap_mixpanel/client.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-18 11:02:27.000000 tap-mixpanel-1.4.3/tap_mixpanel/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      603 2022-10-10 07:35:16.000000 tap-mixpanel-1.4.3/tap_mixpanel/schemas/export.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      199 2022-10-10 07:35:16.000000 tap-mixpanel-1.4.3/tap_mixpanel/schemas/cohort_members.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3390 2022-10-10 07:35:16.000000 tap-mixpanel-1.4.3/tap_mixpanel/schemas/funnels.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      139 2022-10-10 07:35:16.000000 tap-mixpanel-1.4.3/tap_mixpanel/schemas/engage.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      510 2022-10-10 07:35:16.000000 tap-mixpanel-1.4.3/tap_mixpanel/schemas/cohorts.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      449 2022-10-10 07:35:16.000000 tap-mixpanel-1.4.3/tap_mixpanel/schemas/revenue.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      335 2022-10-10 07:35:16.000000 tap-mixpanel-1.4.3/tap_mixpanel/schemas/annotations.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34143 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tap_mixpanel/streams.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7134 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tap_mixpanel/schema.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3191 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tap_mixpanel/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3548 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tap_mixpanel/sync.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1162 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tap_mixpanel/discover.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `tap-mixpanel-1.4.2/LICENSE` & `tap-mixpanel-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.4.2/README.md` & `tap-mixpanel-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.4.2/setup.py` & `tap-mixpanel-1.4.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(name='tap-mixpanel',
-      version='1.4.2',
+      version='1.4.3',
       description='Singer.io tap for extracting data from the mixpanel API',
       author='jeff.huth@bytecode.io',
       classifiers=['Programming Language :: Python :: 3 :: Only'],
       py_modules=['tap_mixpanel'],
       install_requires=[
           'backoff==1.8.0',
           'requests==2.22.0',
           'singer-python==5.12.1',
           'jsonlines==1.2.0'
       ],
-      extras_require={
-        'dev': [
-            'pytest',
-            'requests_mock',
-        ]
-      },
       entry_points='''
           [console_scripts]
           tap-mixpanel=tap_mixpanel:main
       ''',
       packages=find_packages(),
       package_data={
           'tap_mixpanel': [
```

### Comparing `tap-mixpanel-1.4.2/tap_mixpanel/__init__.py` & `tap-mixpanel-1.4.3/tap_mixpanel/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,87 +1,105 @@
 #!/usr/bin/env python3
 
-import sys
 import json
-import argparse
-from datetime import datetime, timedelta, date
+import sys
+from datetime import timedelta
+
 import singer
-from singer import metadata, utils
-from singer.utils import strptime_to_utc, strftime
+from singer import utils
+from singer.utils import strftime, strptime_to_utc
+
 from tap_mixpanel.client import MixpanelClient
-from tap_mixpanel.discover import discover
-from tap_mixpanel.sync import sync
+from tap_mixpanel.discover import discover as _discover
+from tap_mixpanel.sync import sync as _sync
 
 LOGGER = singer.get_logger()
 
 REQUEST_TIMEOUT = 300
 REQUIRED_CONFIG_KEYS = [
-    'project_timezone',
-    'api_secret',
-    'attribution_window',
-    'start_date',
-    'user_agent'
+    "project_timezone",
+    "api_secret",
+    "attribution_window",
+    "start_date",
+    "user_agent",
 ]
 
 
 def do_discover(client, properties_flag):
-    LOGGER.info('Starting discover')
-    catalog = discover(client, properties_flag)
+    """Call the discovery function.
+
+    Args:
+        client (MixpanelClient): Client object to make http calls.
+        properties_flag (str): Setting this argument to `true` ensures that new properties on
+                               events and engage records are captured.
+    """
+    LOGGER.info("Starting discover")
+    catalog = _discover(client, properties_flag)
     json.dump(catalog.to_dict(), sys.stdout, indent=2)
-    LOGGER.info('Finished discover')
+    LOGGER.info("Finished discover")
 
 
 @singer.utils.handle_top_exception(LOGGER)
 def main():
+    """
+    Run discover mode or sync mode.
+    """
     parsed_args = singer.utils.parse_args(REQUIRED_CONFIG_KEYS)
 
-    start_date = parsed_args.config['start_date']
+    start_date = parsed_args.config["start_date"]
     # Set request timeout to config param `request_timeout` value.
     # If value is 0, "0", "" or not passed then it sets default to 300 seconds.
-    config_request_timeout = parsed_args.config.get('request_timeout')
+    config_request_timeout = parsed_args.config.get("request_timeout")
     if config_request_timeout and float(config_request_timeout):
         request_timeout = float(config_request_timeout)
     else:
         request_timeout = REQUEST_TIMEOUT
 
     start_dttm = strptime_to_utc(start_date)
     now_dttm = utils.now()
-    if parsed_args.config.get('end_date'):
-        now_dttm = strptime_to_utc(parsed_args.config.get('end_date'))
+    if parsed_args.config.get("end_date"):
+        now_dttm = strptime_to_utc(parsed_args.config.get("end_date"))
     delta_days = (now_dttm - start_dttm).days
     if delta_days >= 365:
         delta_days = 365
         start_date = strftime(now_dttm - timedelta(days=delta_days))
-        LOGGER.warning("start_date greater than 1 year maxiumum for API.")
+        LOGGER.warning("start_date greater than 1 year maximum for API.")
         LOGGER.warning("Setting start_date to 1 year ago, %s", start_date)
 
-    #Check support for EU endpoints
-    if str(parsed_args.config.get('eu_residency')).lower() == "true":
+    # Check support for EU endpoints
+    if str(parsed_args.config.get("eu_residency")).lower() == "true":
         api_domain = "eu.mixpanel.com"
     else:
         api_domain = "mixpanel.com"
 
-    with MixpanelClient(parsed_args.config['api_secret'],
-                        api_domain,
-                        request_timeout,
-                        parsed_args.config['user_agent']) as client:
+    with MixpanelClient(
+        parsed_args.config["api_secret"],
+        api_domain,
+        request_timeout,
+        parsed_args.config["user_agent"],
+    ) as client:
 
         state = {}
         if parsed_args.state:
             state = parsed_args.state
 
         config = parsed_args.config
-        properties_flag = config.get('select_properties_by_default')
+        client.__api_domain = api_domain
+        properties_flag = config.get("select_properties_by_default")
 
         if parsed_args.discover:
-            client.__api_domain = api_domain
             do_discover(client, properties_flag)
-        elif parsed_args.catalog:
-            sync(client=client,
-                 config=config,
-                 catalog=parsed_args.catalog,
-                 state=state,
-                 start_date=start_date)
+        else:
+            catalog = parsed_args.catalog
+            if not catalog:
+                catalog = _discover(client, properties_flag)
+            _sync(
+                client=client,
+                config=config,
+                catalog=catalog,
+                state=state,
+                start_date=start_date,
+            )
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `tap-mixpanel-1.4.2/tap_mixpanel/schema.py` & `tap-mixpanel-1.4.3/tap_mixpanel/schema.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,151 +1,194 @@
-import os
 import json
+import os
+
+import singer
 from singer import metadata
+
+from tap_mixpanel.client import MixpanelPaymentRequiredError
 from tap_mixpanel.streams import STREAMS
-import singer
 
 LOGGER = singer.get_logger()
 
+
 # Reference:
 # https://github.com/singer-io/getting-started/blob/master/docs/DISCOVERY_MODE.md#Metadata
 
+
 def get_abs_path(path):
+    """Get the absolute path for the schema files.
+
+    Args:
+        path (str): Path from current folder to schema file.
+
+    Returns:
+        str: Full path to schema file.
+    """
     return os.path.join(os.path.dirname(os.path.realpath(__file__)), path)
 
 
 def get_schema(client, properties_flag, stream_name):
-    schema_path = get_abs_path('schemas/{}.json'.format(stream_name))
+    """Creates schema for a stream by loading schema file and appending dynamic
+    fields schema if necessary.
+
+    Args:
+        client (MixpanelClient): Client to make http calls.
+        properties_flag (str): Setting this argument to `true` ensures that new properties on
+                               events and engage records are captured.
+        stream_name (str): Name of stream whose schema is to create.
+
+    Returns:
+        dict: Returns schema of the stream.
+    """
+    schema_path = get_abs_path(f"schemas/{stream_name}.json")
 
-    with open(schema_path) as file:
+    with open(schema_path, encoding="utf-8") as file:
         schema = json.load(file)
 
     # Set whether to allow additional properties for engage and export endpoints
     # Event and Engage properties are dynamic and depend on the properties provided on upload,
     #   when the Event or Engage (user/person) was created.
     # Depending on the tap config parameter select_properties_by_default,
     #   the json schema should allow additional properties (additionalProperties = true).
-    if stream_name in ('engage', 'export') and str(properties_flag).lower() == 'true':
-        schema['additionalProperties'] = True
+    if stream_name in ("engage", "export") and str(properties_flag).lower() == "true":
+        schema["additionalProperties"] = True
     else:
-        schema['additionalProperties'] = False
+        schema["additionalProperties"] = False
 
-    if stream_name == 'engage':
+    if stream_name == "engage":
         properties = client.request(
-            method='GET',
-            url='https://{}/api/2.0'.format(client.__api_domain),
-            path='engage/properties',
-            params={'limit': 2000},
-            endpoint='engage_properties')
-        if properties.get('status') == 'ok':
-            results = properties.get('results', {})
+            method="GET",
+            url=f"https://{client.__api_domain}/api/2.0",
+            path="engage/properties",
+            params={"limit": 2000},
+            endpoint="engage_properties",
+        )
+        if properties.get("status") == "ok":
+            results = properties.get("results", {})
             for key, val in results.items():
-                if key[0:1] == '$':
-                    new_key = 'mp_reserved_{}'.format(key[1:])
+                if key[0:1] == "$":
+                    new_key = f"mp_reserved_{key[1:]}"
                 else:
                     new_key = key
 
                 # property_type: string, number, boolean, datetime, object, list
                 # Reference:
                 # https://help.mixpanel.com/hc/en-us/articles/115004547063-Properties-Supported-Data-Types
-                property_type = val.get('type')
+                property_type = val.get("type")
 
                 types = {
-                    'boolean': {
-                        'type': ['null', 'boolean']
-                    },
-                    'number': {
-                        'type': ['null', 'string'],
-                        'format': 'singer.decimal'
-                    },
-                    'datetime': {
-                        'type': ['null', 'string'],
-                        'format': 'date-time'
-                    },
-                    'object': {
-                        'type': ['null', 'object'],
-                        'additionalProperties': True
-                    },
-                    'list': {
-                        'type': ['null', 'array'],
-                        'required': False,
-                        'items': {}
+                    "boolean": {
+                        "type": ["null", "boolean"]},
+                    "number": {
+                        "type": ["null", "string"],
+                        "format": "singer.decimal"},
+                    "datetime": {
+                        "type": ["null", "string"],
+                        "format": "date-time"},
+                    "object": {
+                        "type": ["null", "object"],
+                        "additionalProperties": True,
                     },
-                    'string': {
-                        'type': ['null', 'string']
-                    }
+                    "list": {
+                        "type": ["null", "array"],
+                        "required": False,
+                        "items": {}},
+                    "string": {
+                        "type": ["null", "string"]},
                 }
 
-                if property_type in types.keys():
+                if property_type in types:
                     # Make the types a list containing all types starting with the one returned to us by the API
                     this_type = [types.pop(property_type)]
                     this_type += list(types.values())
 
                 else:
                     this_type = list(types.values())
 
+                schema["properties"][new_key] = {"anyOf": this_type}
 
-                schema['properties'][new_key] = {'anyOf': this_type}
-
-    if stream_name == 'export':
+    if stream_name == "export":
         # Event properties endpoint:
         #  https://developer.mixpanel.com/docs/data-export-api#section-hr-span-style-font-family-courier-top-span
         results = client.request(
-            method='GET',
-            url='https://{}/api/2.0'.format(client.__api_domain),
-            path='events/properties/top',
-            params={'limit': 2000},
-            endpoint='event_properties')
+            method="GET",
+            url=f"https://{client.__api_domain}/api/2.0",
+            path="events/properties/top",
+            params={"limit": 2000},
+            endpoint="event_properties",
+        )
         for key, val in results.items():
-            if key[0:1] == '$':
-                new_key = 'mp_reserved_{}'.format(key[1:])
+            if key[0:1] == "$":
+                new_key = f"mp_reserved_{key[1:]}"
             else:
                 new_key = key
 
-            # string ONLY for event properties (no other datatypes)
+            # String ONLY for event properties (no other datatypes)
             # Reference: https://help.mixpanel.com/hc/en-us/articles/360001355266-Event-Properties#field-size-character-limits-for-event-properties
-            schema['properties'][new_key] = {
-                'type': ['null', 'string']
-            }
+            schema["properties"][new_key] = {"type": ["null", "string"]}
 
     return schema
 
+
 def get_schemas(client, properties_flag):
+    """Load the schema references, prepare metadata for each streams and return
+    schema and metadata for the catalog.
+
+    Args:
+        client (MixpanelClient): Client object to make http calls.
+        properties_flag (bool): Setting this argument to true ensures that new properties on
+                                   events and engage records are captured.
+
+    Returns:
+        tuple: Returns tuple of Schemas and metadata.
+    """
     schemas = {}
     field_metadata = {}
 
     for stream_name, stream_metadata in STREAMS.items():
         # When the client detects disable_engage_endpoint, skip discovering the stream
-        if stream_name == 'engage' and client.disable_engage_endpoint:
-            LOGGER.warning('Mixpanel returned a 402 indicating the Engage endpoint and stream is unavailable. Skipping.')
+        if stream_name == "engage" and client.disable_engage_endpoint:
+            LOGGER.warning(
+                "Mixpanel returned a 402 indicating the Engage endpoint and stream is unavailable. Skipping."
+            )
             continue
 
-        schema = get_schema(client, properties_flag, stream_name)
+        try:
+            schema = get_schema(client, properties_flag, stream_name)
+        except MixpanelPaymentRequiredError:
+            LOGGER.warning(
+                "Mixpanel returned a 402 from the %s API so %s stream will be skipped.",
+                stream_name,
+                stream_name,
+            )
+            continue
 
         schemas[stream_name] = schema
         mdata = metadata.new()
 
         # Documentation:
         # https://github.com/singer-io/getting-started/blob/master/docs/DISCOVERY_MODE.md#singer-python-helper-functions
         # Reference:
         # https://github.com/singer-io/singer-python/blob/master/singer/metadata.py#L25-L44
         mdata = metadata.get_standard_metadata(
             schema=schema,
             key_properties=stream_metadata.key_properties,
             valid_replication_keys=stream_metadata.replication_keys,
-            replication_method=stream_metadata.replication_method
+            replication_method=stream_metadata.replication_method,
         )
 
         mdata = metadata.to_map(mdata)
 
         if stream_metadata.replication_keys:
-                mdata = metadata.write(
-                    mdata,
-                    ('properties', stream_metadata.replication_keys[0]),
-                    'inclusion',
-                    'automatic')
+            mdata = metadata.write(
+                mdata,
+                ("properties",
+                 stream_metadata.replication_keys[0]),
+                "inclusion",
+                "automatic",
+            )
 
         mdata = metadata.to_list(mdata)
 
         field_metadata[stream_name] = mdata
 
     return schemas, field_metadata
```

### Comparing `tap-mixpanel-1.4.2/tap_mixpanel/schemas/export.json` & `tap-mixpanel-1.4.3/tap_mixpanel/schemas/export.json`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.4.2/tap_mixpanel/schemas/funnels.json` & `tap-mixpanel-1.4.3/tap_mixpanel/schemas/funnels.json`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.4.2/tap_mixpanel/streams.py` & `tap-mixpanel-1.4.3/tap_mixpanel/streams.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,66 +1,95 @@
-"""
-This module defines the stream classes and their individual sync logic.
-"""
+"""This module defines the stream classes and their individual sync logic."""
 
 import json
 import math
+from copy import deepcopy
 from datetime import datetime, timedelta
 
 import pytz
 import singer
 from singer import Transformer, metadata, metrics, utils
 from singer.utils import strptime_to_utc
 
 from tap_mixpanel.client import MixpanelClient
-from tap_mixpanel.transform import transform_record, transform_datetime
+from tap_mixpanel.transform import transform_datetime, transform_record
 
 LOGGER = singer.get_logger()
 
 
 class MixPanel:
     """
     A base class representing singer streams.
     :param client: The API client used to extract records from external source
     """
+
     tap_stream_id = None
     replication_method = None
     replication_keys = []
     key_properties = []
     to_replicate = True
     date_dictionary = False
     path = None
     params = {}
     parent = None
+    child = None
     data_key = None
     bookmark_query_field_from = None
     bookmark_query_field_to = None
     pagination = False
     parent_path = None
     parent_id_field = None
     url = "https://mixpanel.com/api/2.0"
 
     def __init__(self, client: MixpanelClient):
         self.client = client
 
     def write_schema(self, catalog, stream_name):
+        """Writes the schema of the stream form the catalog.
+
+        Args:
+            catalog (singer.Catalog): Catalog object having schema and metadata of all the streams.
+            stream_name (str): Name of the syncing stream.
+
+        Raises:
+            err: Raises if any error occur while writing schema.
+        """
         stream = catalog.get_stream(stream_name)
         schema = stream.schema.to_dict()
         try:
             singer.write_schema(stream_name, schema, stream.key_properties)
         except OSError as err:
-            LOGGER.error("OS Error writing schema for: %s",stream_name)
+            LOGGER.error("OS Error writing schema for: %s", stream_name)
             raise err
 
     def get_bookmark(self, state, stream, default):
+        """Get the bookmark value from the state if available in the state.
+        Else return start date.
+
+        Args:
+            state (dict): State containing bookmarks of the streams if available.
+            stream (str): Name of the stream to get the bookmark.
+            default (str): Default value to return if bookmark is not available.(start_date)
+
+        Returns:
+            str: Returns bookmark value.
+        """
         if (state is None) or ("bookmarks" not in state):
             return default
         return state.get("bookmarks", {}).get(stream, default)
 
     def write_bookmark(self, state, stream, value):
+        """Updates the stream bookmark value in the state. And writes the
+        state.
+
+        Args:
+            state (dict): State containing bookmarks of the streams if available.
+            stream (str): Name of stream whose bookmark will be written.
+            value (str): Bookmark value of the stream.
+        """
         if "bookmarks" not in state:
             state["bookmarks"] = {}
         state["bookmarks"][stream] = value
         LOGGER.info("Write state for stream: %s, value: %s", stream, value)
         singer.write_state(state)
 
     def process_records(
@@ -69,30 +98,51 @@
         stream_name,
         records,
         time_extracted,
         bookmark_field=None,
         max_bookmark_value=None,
         last_datetime=None,
     ):
+        """Transform the record as per the schema and write the record if
+        replication value > bookmark for incremental stream.
+
+        Args:
+            stream_name (str): Name of the syncing stream.
+            records (dict): Record to be written.
+            time_extracted (datetime): Datetime when the data was extracted from the API
+            bookmark_field (str, optional): Bookmark field in the state if stream is INCREMENTAL.
+                                            Defaults to None.
+            max_bookmark_value (str, optional): Maximum bookmark value if written records if replication key
+                                                is available. Defaults to None.
+            last_datetime (str, optional): Last datetime from which greater replication value records will be written.
+                                           Defaults to None.
+
+        Raises:
+            err: Raises exception if transformation error occurs.
+
+        Returns:
+            tuple: Tuple of maximum bookmark value if written records and written records count.
+        """
         stream = catalog.get_stream(stream_name)
         schema = stream.schema.to_dict()
         stream_metadata = metadata.to_map(stream.metadata)
 
         with metrics.record_counter(stream_name) as counter:
             for record in records:
                 # Transform record for Singer.io
                 with Transformer() as transformer:
                     try:
                         transformed_record = transformer.transform(
                             record, schema, stream_metadata
                         )
                     except Exception as err:
-                        LOGGER.error("Error: %s",str(err))
-                        LOGGER.error("For schema: %s",
-                            json.dumps(schema, sort_keys=True, indent=2)
+                        LOGGER.error("Error: %s", str(err))
+                        LOGGER.error(
+                            "For schema: %s",
+                            json.dumps(schema, sort_keys=True, indent=2),
                         )
                         raise err
 
                     # Reset max_bookmark_value to new value if higher
                     if transformed_record.get(bookmark_field):
                         if max_bookmark_value is None or transformed_record[
                             bookmark_field
@@ -119,296 +169,418 @@
                             time_extracted=time_extracted,
                         )
                         counter.increment()
 
             return max_bookmark_value, counter.value
 
     def get_and_transform_records(
-            self, querystring, project_timezone, max_bookmark_value, catalog, last_datetime, endpoint_total,
-            limit, total_records, parent_total, record_count, page, offset, parent_record, date_total):
-        """
-        Get the records using the client get request and transform it using transform_records
-        and return the max_bookmark_value
+        self,
+        querystring,
+        project_timezone,
+        max_bookmark_value,
+        state,
+        config,
+        catalog,
+        selected_streams,
+        last_datetime,
+        endpoint_total,
+        limit,
+        total_records,
+        parent_total,
+        record_count,
+        page,
+        offset,
+        parent_record,
+        date_total,
+    ):
+        """Get the records using the client get request and transform it using
+        transform_records and return the max_bookmark_value.
+
+        Args:
+            querystring (str): Params in URL query format to join with stream path
+            project_timezone (str): Time zone in which integer date times are stored.
+            max_bookmark_value (str): Maximum bookmark value among written records.
+            catalog (singer.Catalog): Catalog object having schema and metadata of all the streams.
+            last_datetime (str): Last datetime from which greater replication value records will be written.
+            endpoint_total (int): Total number of records written yet.
+            limit (int): Page size.
+            total_records (int): Total number of records available for the sync.
+            parent_total (int): Total records for parent ID
+            record_count (int): Number of records per page written by tap.
+            page (int): Page count.
+            offset (int): Offset value of stream data for the pagination.
+            parent_record (dict): Record of parent stream.
+            date_total (int): Total records written for the date window.
+
+        Raises:
+            Exception: Raises if any key-property is missing.
+
+        Returns:
+            tuple: Returns tuple of parent_total, date_total, offset, page, session_id,
+                   endpoint_total, max_bookmark_value, total_records
         """
 
         session_id = None
         data = self.client.request(
-            method='GET',
+            method="GET",
             url=self.url,
             path=self.path,
             params=querystring,
-            endpoint=self.tap_stream_id)
+            endpoint=self.tap_stream_id,
+        )
 
-        # time_extracted: datetime when the data was extracted from the API
-        time_extracted = utils.now()
-        full_url = '{}/{}{}'.format(
-            self.url,
-            self.path,
-            '?{}'.format(querystring) if querystring else '')
+        full_url = f"{self.url}/{self.path}{f'?{querystring}' if querystring else ''}"
         if not data:
-            LOGGER.info('No data for URL: %s',full_url)
+            LOGGER.info("No data for URL: %s", full_url)
             # No data results
-        else:  # has data
+        else:  # Has data
+
+            # Sync child stream first
+            if self.child and self.child in selected_streams:
+                child_obj = STREAMS[self.child](self.client)
+                child_obj.sync(
+                    state,
+                    catalog,
+                    config,
+                    config["start_date"],
+                    selected_streams,
+                    parent_data=deepcopy(data),
+                )
+
+            # time_extracted: datetime when the data was extracted from the API
+            time_extracted = utils.now()
+
             # Transform data with transform_json from transform.py
             # The data_key identifies the array/list of records below the <root> element
-            # LOGGER.info('data = {}'.format(data)) # TESTING, comment out
             transformed_data = []  # initialize the record list
 
             # Endpoints: funnels, revenue return results as dictionary for each date
             # Standardize results to a list/array
             if self.date_dictionary and self.data_key in data:
                 results = {}
                 results_list = []
                 for key, val in data[self.data_key].items():
-                    # skip $overall summary
-                    if key != '$overall':
-                        val['date'] = key
-                        val['datetime'] = '{}T00:00:00Z'.format(key)
+                    # Skip $overall summary
+                    if key != "$overall":
+                        val["date"] = key
+                        val["datetime"] = f"{key}T00:00:00Z"
                         results_list.append(val)
                 results[self.data_key] = results_list
                 data = results
 
             # Cohorts endpoint returns results as a list/array (no data_key)
             # All other endpoints have a data_key
             if not self.data_key:
-                self.data_key = 'results'
-                new_data = {
-                    'results': data
-                }
+                self.data_key = "results"
+                new_data = {"results": data}
                 data = new_data
 
             transformed_data = []
             # Loop through result records
             for record in data[self.data_key]:
-                # transform record and append to transformed_data array
-                transformed_record = transform_record(record,
-                                                      self.tap_stream_id,
-                                                      project_timezone,
-                                                      parent_record)
+                # Transform record and append to transformed_data array
+                transformed_record = transform_record(
+                    record, self.tap_stream_id, project_timezone, parent_record
+                )
                 transformed_data.append(transformed_record)
 
                 # Check for missing keys
                 for key in self.key_properties:
                     val = transformed_record.get(key)
                     if not val:
-                        LOGGER.error('Error: Missing Key')
-                        raise 'Missing Key'
+                        LOGGER.error("Error: Missing Key")
+                        raise Exception("Missing Key")
 
                 # End data record loop
 
             if not transformed_data:
-                 LOGGER.info('No transformed data for data = %s', data)
-                # No transformed data results
-            else:  # has transformed data
+                LOGGER.info("No transformed data for data = %s", data)
+            # No transformed data results
+            else:  # Has transformed data
                 # Process records and get the max_bookmark_value and record_count
-                max_bookmark_value, record_count = self.process_records(
-                    catalog=catalog,
-                    stream_name=self.tap_stream_id,
-                    records=transformed_data,
-                    time_extracted=time_extracted,
-                    bookmark_field=next(iter(self.replication_keys), None),
-                    max_bookmark_value=max_bookmark_value,
-                    last_datetime=last_datetime)
-                LOGGER.info('Stream %s, batch processed %s records', self.tap_stream_id, record_count)
+                if self.tap_stream_id in selected_streams:
+                    max_bookmark_value, record_count = self.process_records(
+                        catalog=catalog,
+                        stream_name=self.tap_stream_id,
+                        records=transformed_data,
+                        time_extracted=time_extracted,
+                        bookmark_field=next(iter(self.replication_keys), None),
+                        max_bookmark_value=max_bookmark_value,
+                        last_datetime=last_datetime,
+                    )
+                    LOGGER.info(
+                        "Stream %s, batch processed %s records",
+                        self.tap_stream_id,
+                        record_count,
+                    )
 
-                # set total_records and pagination fields
+                # Set total_records and pagination fields
                 if page == 0:
                     if isinstance(data, dict):
-                        total_records = data.get('total', record_count)
+                        total_records = data.get("total", record_count)
                     else:
                         total_records = record_count
                 parent_total = parent_total + record_count
                 date_total = date_total + record_count
                 endpoint_total = endpoint_total + record_count
                 if isinstance(data, dict):
-                    session_id = data.get('session_id', None)
+                    session_id = data.get("session_id", None)
 
                 # to_rec: to record; ending record for the batch page
                 if self.pagination:
                     to_rec = offset + limit
-                    if to_rec > total_records:
-                        to_rec = total_records
+                    to_rec = min(to_rec, total_records)
                 else:
                     to_rec = record_count
 
-                LOGGER.info('Synced Stream: %s, page: %s, %s to %s of total: %s',
-                            self.tap_stream_id,
-                            page,
-                            offset,
-                            to_rec,
-                            total_records)
+                LOGGER.info(
+                    "Synced Stream: %s, page: %s, %s to %s of total: %s",
+                    self.tap_stream_id,
+                    page,
+                    offset,
+                    to_rec,
+                    total_records,
+                )
                 # End has transformed data
             # End has data results
 
         # Pagination: increment the offset by the limit (batch-size) and page
         offset = offset + limit
         page = page + 1
-        return parent_total, date_total, offset, page, session_id, endpoint_total, max_bookmark_value, total_records
+        return (
+            parent_total,
+            date_total,
+            offset,
+            page,
+            session_id,
+            endpoint_total,
+            max_bookmark_value,
+            total_records,
+        )
 
-    def define_bookmark_filters(self, days_interval, last_datetime, now_datetime, attribution_window):
-        """
-        define the params from and to according to the filters provided in
-         the bookmark_query_field_from and bookmark_query_field_to
+    def define_bookmark_filters(
+        self, days_interval, last_datetime, now_datetime, attribution_window, start_date
+    ):
+        """Define the params from and to according to the filters provided in
+        the bookmark_query_field_from and bookmark_query_field_to.
+
+        Args:
+            days_interval (int): Interval in days between start_window and end_window
+            last_datetime (str): Last datetime from records will be fetched.
+            now_datetime (datetime): Current datetime from sync started.
+            attribution_window (int): Latency minimum number of days to look-back to
+                                      account for delays in attributing accurate results.
+
+        Returns:
+            tuple: Returns tuple if start_window, date_window and interval
         """
         if self.bookmark_query_field_from and self.bookmark_query_field_to:
             # days_interval from config date_window_size, default = 60; passed to function from sync
             if not days_interval:
                 days_interval = 30
 
             last_dttm = strptime_to_utc(last_datetime)
             delta_days = (now_datetime - last_dttm).days
             if delta_days <= attribution_window:
                 delta_days = attribution_window
-                LOGGER.info("Start bookmark less than %s day attribution window.", attribution_window)
+                LOGGER.info(
+                    "Start bookmark less than %s day attribution window.",
+                    attribution_window,
+                )
             elif delta_days >= 365:
                 delta_days = 365
-                LOGGER.warning("Start date or bookmark greater than 1 year maxiumum.")
+                LOGGER.warning("Start date or bookmark greater than 1 year maximum.")
                 LOGGER.warning("Setting bookmark start to 1 year ago.")
 
             start_window = now_datetime - timedelta(days=delta_days)
+
+            # Records before start_date should not be queried
+            start_window = max(start_window, strptime_to_utc(start_date))
+
             end_window = start_window + timedelta(days=days_interval)
-            if end_window > now_datetime:
-                end_window = now_datetime
+            end_window = min(end_window, now_datetime)
         else:
             start_window = strptime_to_utc(last_datetime)
             end_window = now_datetime
             diff_sec = (end_window - start_window).seconds
-            # round-up difference to days
+            # Round-up difference to days
             days_interval = math.ceil(diff_sec / (3600 * 24))
 
         return start_window, end_window, days_interval
 
-    def sync(self, state, catalog, config, start_date):
-        # the sync method common to all the streams which internally call methods depending on different endpoints
+    def sync(
+        self, state, catalog, config, start_date, selected_streams, parent_data=None
+    ):
+        """The sync method common to all the streams which internally call
+        methods depending on different endpoints.
+
+        Args:
+            state (dict): State containing bookmarks of the streams if available.
+            catalog (singer.Catalog): Catalog object having schema and metadata of all the streams.
+            config (dict): The tap config file for this tap should include these entries.
+            start_date (str): The default value to use if no bookmark exists for an endpoint
+
+        Returns:
+            int: Returns total number of records.
+        """
 
         bookmark_field = next(iter(self.replication_keys), None)
         project_timezone = config.get("project_timezone", "UTC")
         days_interval = int(config.get("date_window_size", "30"))
         attribution_window = int(config.get("attribution_window", "5"))
 
-        #Update url if eu_residency is selected
-        if str(config.get('eu_residency')).lower() == "true":
-            if self.tap_stream_id == 'export':
-                self.url = 'https://data-eu.mixpanel.com/api/2.0'
+        # Update url if eu_residency is selected
+        if str(config.get("eu_residency")).lower() == "true":
+            if self.tap_stream_id == "export":
+                self.url = "https://data-eu.mixpanel.com/api/2.0"
             else:
-                self.url = 'https://eu.mixpanel.com/api/2.0'
+                self.url = "https://eu.mixpanel.com/api/2.0"
 
         # Get the latest bookmark for the stream and set the last_integer/datetime
-        last_datetime = self.get_bookmark(
-            state, self.tap_stream_id, start_date)
+        last_datetime = self.get_bookmark(state, self.tap_stream_id, start_date)
         max_bookmark_value = last_datetime
 
-        self.write_schema(catalog, self.tap_stream_id)
-
-        # windowing: loop through date days_interval date windows from last_datetime to now_datetime
+        # Windowing: loop through date days_interval date windows from last_datetime to now_datetime
         tzone = pytz.timezone(project_timezone)
         now_datetime = datetime.now(tzone)
-        end_date = config.get('end_date')
+        end_date = config.get("end_date")
 
         if end_date:
             now_datetime = strptime_to_utc(end_date)
 
         start_window, end_window, days_interval = self.define_bookmark_filters(
-            days_interval, last_datetime, now_datetime, attribution_window)
+            days_interval, last_datetime, now_datetime, attribution_window, start_date
+        )
         # LOOP order: Date Windows, Parent IDs, Page
         # Initialize counter
         endpoint_total = 0  # Total for ALL: parents, date windows, and pages
 
         # Begin date windowing loop
         while start_window < now_datetime:
             # Initialize counters
             date_total = 0  # Total records for a date window
             parent_total = 0  # Total records for parent ID
             total_records = 0  # Total records for all pages
             record_count = 0  # Total processed for page
 
-            params = self.params  # adds in endpoint specific, sort, filter params
+            params = self.params  # Adds in endpoint specific, sort, filter params
 
             if self.bookmark_query_field_from and self.bookmark_query_field_to:
                 # Request dates need to be normalized to project timezone or else errors may occur
                 # Errors occur when from_date is > 365 days ago
                 #   and when to_date > today (in project timezone)
                 from_date = str(start_window.astimezone(tzone).date())
                 to_date = str(end_window.astimezone(tzone).date())
                 LOGGER.info("START Sync for Stream: %s", self.tap_stream_id)
                 if self.bookmark_query_field_from:
                     LOGGER.info("Date window from: %s to %s", from_date, to_date)
                 params[self.bookmark_query_field_from] = from_date
                 params[self.bookmark_query_field_to] = to_date
 
-            # funnels and cohorts have a parent endpoint with parent_data and parent_id_field
-            if self.parent_path and self.parent_id_field:
-                # API request data
-                LOGGER.info("URL for Parent Stream %s: %s/%s",
-                            self.tap_stream_id,
-                            self.url,
-                            self.parent_path)
-                parent_data = self.client.request(
-                    method="GET",
-                    url=self.url,
-                    path=self.parent_path,
-                    endpoint="parent_data",
-                )
-            # Other endpoints (not funnels, cohorts): Simulate parent_data with single record
-            else:
-                parent_data = [{"id": "none"}]
-                self.parent_id_field = "id"
+            if not parent_data:
+
+                # Funnels and cohorts have a parent endpoint with parent_data and parent_id_field
+                if self.parent_path and self.parent_id_field:
+                    # API request data
+                    LOGGER.info(
+                        "URL for Parent Stream %s: %s/%s",
+                        self.tap_stream_id,
+                        self.url,
+                        self.parent_path,
+                    )
+                    parent_data = self.client.request(
+                        method="GET",
+                        url=self.url,
+                        path=self.parent_path,
+                        endpoint="parent_data",
+                    )
+                # Other endpoints (not funnels, cohorts): Simulate parent_data with single record
+                else:
+                    parent_data = [{"id": "none"}]
+                    self.parent_id_field = "id"
 
             for parent_record in parent_data:
                 parent_id = parent_record.get(self.parent_id_field)
-                LOGGER.info('START: Stream: %s, parent_id: %s', self.tap_stream_id, parent_id)
+                LOGGER.info(
+                    "START: Stream: %s, parent_id: %s", self.tap_stream_id, parent_id
+                )
 
-                # pagination: loop thru all pages of data using next (if not None)
+                # Pagination: loop thru all pages of data using next (if not None)
                 page = 0  # First page is page=0, second page is page=1, ...
                 offset = 0
                 limit = 250  # Default page_size
                 # Initialize counters
                 parent_total = 0  # Total records for parent ID
                 total_records = 0  # Total records for all pages
                 record_count = 0  # Total processed for page
 
-                session_id = 'initial'
+                session_id = "initial"
                 if self.pagination:
-                    params['page_size'] = limit
+                    params["page_size"] = limit
 
                 # Popped session_id and page number of last parents stream call.
-                params.pop('session_id', None)
-                params.pop('page', None)
+                params.pop("session_id", None)
+                params.pop("page", None)
 
                 while offset <= total_records and session_id is not None:
                     if self.pagination and page != 0:
-                        params['session_id'] = session_id
-                        params['page'] = page
+                        params["session_id"] = session_id
+                        params["page"] = page
 
                     # querystring: Squash query params into string and replace [parent_id]
-                    querystring = '&'.join(['%s=%s' % (key, value) for (key, value) in params.items()])
-                    querystring = querystring.replace('[parent_id]', str(parent_id))
-
-                    full_url = '{}/{}{}'.format(
-                        self.url,
-                        self.path,
-                        '?{}'.format(querystring) if querystring else '')
-
-                    LOGGER.info('URL for Stream %s: %s', self.tap_stream_id, full_url)
-
-                    # API request data
-                    # data = {}
-
-                    parent_total, date_total, offset, page, session_id, endpoint_total, max_bookmark_value, total_records = self.get_and_transform_records(
-                        querystring, project_timezone, max_bookmark_value, catalog, last_datetime, endpoint_total, limit, total_records, parent_total, record_count, page, offset, parent_record, date_total)
-                   # End stream != 'export'
-                LOGGER.info('FINISHED: Stream: %s, parent_id: %s', self.tap_stream_id, parent_id)
-                LOGGER.info('Total records for parent: %s', parent_total)
+                    querystring = "&".join(
+                        [f"{key}={value}" for (key, value) in params.items()]
+                    )
+                    querystring = querystring.replace("[parent_id]", str(parent_id))
+
+                    full_url = f"{self.url}/{self.path}{f'?{querystring}' if querystring else ''}"
+
+                    LOGGER.info("URL for Stream %s: %s", self.tap_stream_id, full_url)
+
+                    (
+                        parent_total,
+                        date_total,
+                        offset,
+                        page,
+                        session_id,
+                        endpoint_total,
+                        max_bookmark_value,
+                        total_records,
+                    ) = self.get_and_transform_records(
+                        querystring,
+                        project_timezone,
+                        max_bookmark_value,
+                        state,
+                        config,
+                        catalog,
+                        selected_streams,
+                        last_datetime,
+                        endpoint_total,
+                        limit,
+                        total_records,
+                        parent_total,
+                        record_count,
+                        page,
+                        offset,
+                        parent_record,
+                        date_total,
+                    )
+                # End stream != 'export'
+                LOGGER.info(
+                    "FINISHED: Stream: %s, parent_id: %s", self.tap_stream_id, parent_id
+                )
+                LOGGER.info("Total records for parent: %s", parent_total)
                 # End parent record loop
-            LOGGER.info("FINISHED Sync for Stream: %s",self.tap_stream_id)
+            LOGGER.info("FINISHED Sync for Stream: %s", self.tap_stream_id)
             if self.bookmark_query_field_from:
-                LOGGER.info("Date window from: %s to %s",from_date, to_date)
+                LOGGER.info("Date window from: %s to %s", from_date, to_date)
             LOGGER.info("Total records for date window: %s", date_total)
             # Increment date window
-            start_window = end_window
+            # Start after the day of end_window
+            start_window = end_window + timedelta(days=1)
             next_end_window = end_window + timedelta(days=days_interval)
             if next_end_window > now_datetime:
                 end_window = now_datetime
             else:
                 end_window = next_end_window
 
             # Update the state with the max_bookmark_value for the stream
@@ -420,66 +592,73 @@
 
 
 class Annotations(MixPanel):
     """
     List the annotations for a given date range.
     Docs: https://developer.mixpanel.com/reference/annotations
     """
+
     tap_stream_id = "annotations"
     key_properties = ["date"]
     path = "annotations"
     data_key = "annotations"
     bookmark_query_field_from = "from_date"
     bookmark_query_field_to = "to_date"
     replication_method = "FULL_TABLE"
     params = {}
     replication_keys = []
 
 
 class CohortMembers(MixPanel):
     """
     The list endpoint returns all of the cohorts in a given project.
-    The JSON formatted return contains the cohort name, id, count, description, creation date, and visibility for every cohort in the project.
+    The JSON formatted return contains the cohort name, id, count,
+    description, creation date, and visibility for every cohort in the project.
     Docs: https://developer.mixpanel.com/reference/engage
     """
+
     tap_stream_id = "cohort_members"
     path = "engage"
     key_properties = ["cohort_id", "distinct_id"]
     params = {"filter_by_cohort": '{"id": [parent_id]}'}
     data_key = "results"
     pagination = True
-    parent_path = "cohorts/list"
+    parent = "cohorts"
     parent_id_field = "id"
     replication_keys = []
     replication_method = "FULL_TABLE"
     bookmark_query_field_from = None
     bookmark_query_field_to = None
 
 
 class Cohorts(MixPanel):
     """
-    Takes a JSON object with a single key called id whose value is the cohort ID. behaviors and filter_by_cohort are mutually exclusive.
+    Takes a JSON object with a single key called id whose value is the cohort ID.
+    behaviors and filter_by_cohort are mutually exclusive.
     Docs: https://developer.mixpanel.com/reference/cohorts
     """
+
     tap_stream_id = "cohorts"
     path = "cohorts/list"
     key_properties = ["id"]
     data_key = None
     replication_method = "FULL_TABLE"
     params = {}
+    child = "cohort_members"
     replication_keys = []
     bookmark_query_field_from = None
     bookmark_query_field_to = None
 
 
 class Engage(MixPanel):
     """
     Query user profile data and return list of users that fit specified parameters.
     Docs: https://developer.mixpanel.com/reference/engage
     """
+
     tap_stream_id = "engage"
     path = "engage"
     data_key = "results"
     pagination = True
     key_properties = ["distinct_id"]
     replication_method = "FULL_TABLE"
     bookmark_query_field_from = None
@@ -491,68 +670,115 @@
 class Export(MixPanel):
     """
     Every data point sent to Mixpanel is stored as JSON in our data store.
     The raw export API allows you to download your event data as it is received and stored within Mixpanel,
     complete with all event properties (including distinct_id) and the exact timestamp the event was fired.
     Docs: https://developer.mixpanel.com/reference/export
     """
+
     tap_stream_id = "export"
     path = "export"
     data_key = "results"
     replication_keys = ["time"]
     url = "https://data.mixpanel.com/api/2.0"
     bookmark_query_field_from = "from_date"
     bookmark_query_field_to = "to_date"
     replication_method = "INCREMENTAL"
     params = {}
 
     def get_and_transform_records(
-            self, querystring, project_timezone, max_bookmark_value, catalog, last_datetime, endpoint_total,
-            limit, total_records, parent_total, record_count, page, offset, parent_record, date_total):
+        self,
+        querystring,
+        project_timezone,
+        max_bookmark_value,
+        state,
+        config,
+        catalog,
+        selected_streams,
+        last_datetime,
+        endpoint_total,
+        limit,
+        total_records,
+        parent_total,
+        record_count,
+        page,
+        offset,
+        parent_record,
+        date_total,
+    ):
         """
         Get the records using the client get request and transform it using transform_records
-        and return the max_bookmark_value
+        and return the max_bookmark_value.
+
+        Args:
+            querystring (str): Params in URL query format to join with stream path
+            project_timezone (str): Time zone in which integer date times are stored.
+            max_bookmark_value (str): Maximum bookmark value among written records.
+            catalog (singer.Catalog): Catalog object having schema and metadata of all the streams.
+            last_datetime (str): Last datetime from which greater replication value records will be written.
+            endpoint_total (int): Total number of records written yet.
+            limit (int): Page size.
+            total_records (int): Total number of records available for the sync.
+            parent_total (int): Total records for parent ID
+            record_count (int): Number of records per page written by tap.
+            page (int): Page count.
+            offset (int): Offset value of stream data for the pagination.
+            parent_record (dict): Record of parent stream.
+            date_total (int): Total records written for the date window.
+
+        Raises:
+            Exception: Raises if any key-property is missing.
+
+        Returns:
+            tuple: Returns tuple of parent_total, date_total, offset, page, session_id,
+                   endpoint_total, max_bookmark_value, total_records
         """
         data = self.client.request_export(
-            method='GET',
+            method="GET",
             url=self.url,
             path=self.path,
             params=querystring,
-            endpoint=self.tap_stream_id)
+            endpoint=self.tap_stream_id,
+        )
 
         # time_extracted: datetime when the data was extracted from the API
         time_extracted = utils.now()
         transformed_data = []
         for record in data:
-            if record and str(record) != '':
-                # transform record and append to transformed_data array
-                transformed_record = transform_record(record,
-                                                      self.tap_stream_id,
-                                                      project_timezone)
+            if record and str(record):
+                # Transform record and append to transformed_data array
+                transformed_record = transform_record(
+                    record, self.tap_stream_id, project_timezone
+                )
                 transformed_data.append(transformed_record)
 
                 # Check for missing keys
                 for key in self.key_properties:
                     val = transformed_record.get(key)
                     if not val:
-                        LOGGER.error('Error: Missing Key')
-                        raise 'Missing Key'
+                        LOGGER.error("Error: Missing Key")
+                        raise Exception("Missing Key")
 
                 if len(transformed_data) == limit:
                     # Process full batch (limit = 250) records
                     #   and get the max_bookmark_value and record_count
                     max_bookmark_value, record_count = self.process_records(
                         catalog=catalog,
                         stream_name=self.tap_stream_id,
                         records=transformed_data,
                         time_extracted=time_extracted,
                         bookmark_field=next(iter(self.replication_keys), None),
                         max_bookmark_value=max_bookmark_value,
-                        last_datetime=last_datetime)
-                    LOGGER.info('Stream %s, batch processed %s records', self.tap_stream_id, record_count)
+                        last_datetime=last_datetime,
+                    )
+                    LOGGER.info(
+                        "Stream %s, batch processed %s records",
+                        self.tap_stream_id,
+                        record_count,
+                    )
 
                     total_records = total_records + record_count
                     parent_total = parent_total + record_count
                     date_total = date_total + record_count
                     endpoint_total = endpoint_total + record_count
                     transformed_data = []
                     # End if (batch = limit 250)
@@ -564,33 +790,49 @@
             max_bookmark_value, record_count = self.process_records(
                 catalog=catalog,
                 stream_name=self.tap_stream_id,
                 records=transformed_data,
                 time_extracted=time_extracted,
                 bookmark_field=next(iter(self.replication_keys), None),
                 max_bookmark_value=max_bookmark_value,
-                last_datetime=last_datetime)
-            LOGGER.info('Stream %s, batch processed %s records', self.tap_stream_id, record_count)
+                last_datetime=last_datetime,
+            )
+            LOGGER.info(
+                "Stream %s, batch processed %s records",
+                self.tap_stream_id,
+                record_count,
+            )
 
             total_records = total_records + record_count
             parent_total = parent_total + record_count
             date_total = date_total + record_count
             endpoint_total = endpoint_total + record_count
             # End if transformed_data
 
         # Export does not provide pagination; session_id = None breaks out of loop.
         session_id = None
-        return parent_total, date_total, offset, page, session_id, endpoint_total, max_bookmark_value, total_records
+        return (
+            parent_total,
+            date_total,
+            offset,
+            page,
+            session_id,
+            endpoint_total,
+            max_bookmark_value,
+            total_records,
+        )
 
 
 class Funnels(MixPanel):
     """
-    Get data for a funnel. funnel_id as a parameter to the API to get the funnel that you wish to get data for.
+    Get data for a funnel.
+    funnel_id as a parameter to the API to get the funnel that you wish to get data for.
     Docs: https://developer.mixpanel.com/reference/funnels
     """
+
     tap_stream_id = "funnels"
     path = "funnels"
     key_properties = ["funnel_id", "date"]
     data_key = "data"
     date_dictionary = True
     bookmark_query_field_from = "from_date"
     bookmark_query_field_to = "to_date"
```

### Comparing `tap-mixpanel-1.4.2/tap_mixpanel.egg-info/SOURCES.txt` & `tap-mixpanel-1.4.3/tap_mixpanel.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -20,22 +20,25 @@
 tap_mixpanel/schemas/cohort_members.json
 tap_mixpanel/schemas/cohorts.json
 tap_mixpanel/schemas/engage.json
 tap_mixpanel/schemas/export.json
 tap_mixpanel/schemas/funnels.json
 tap_mixpanel/schemas/revenue.json
 tests/__init__.py
-tests/configuration/__init__.py
-tests/configuration/fixtures.py
 tests/tap_tester/__init__.py
 tests/tap_tester/base.py
-tests/tap_tester/test_all_fields_pagination.py
-tests/tap_tester/test_automatic_fields.py
-tests/tap_tester/test_bookmark.py
-tests/tap_tester/test_discovery.py
-tests/tap_tester/test_start_date.py
+tests/tap_tester/test_mixpanel_all_fields_pagination.py
+tests/tap_tester/test_mixpanel_automatic_fields.py
+tests/tap_tester/test_mixpanel_bookmark.py
+tests/tap_tester/test_mixpanel_discovery.py
+tests/tap_tester/test_mixpanel_start_date.py
 tests/unittests/__init__.py
+tests/unittests/test_attribution_window.py
+tests/unittests/test_client.py
+tests/unittests/test_discover.py
 tests/unittests/test_error_handling.py
-tests/unittests/test_medium_client.py
+tests/unittests/test_main.py
 tests/unittests/test_request_timeout_param_value.py
 tests/unittests/test_support_eu_endpoints.py
+tests/unittests/test_sync.py
+tests/unittests/test_transform.py
 tests/unittests/test_transform_event_times.py
```

### Comparing `tap-mixpanel-1.4.2/tests/tap_tester/base.py` & `tap-mixpanel-1.4.3/tests/tap_tester/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,80 +1,84 @@
 """
 Test tap combined
 """
 
 import os
-import unittest
 from datetime import datetime as dt
 from datetime import timedelta
 
 import dateutil.parser
 import pytz
-
-from tap_tester import connections
-from tap_tester import runner
-from tap_tester import menagerie
-from tap_tester.logger import LOGGER
+from tap_tester import LOGGER, connections, menagerie, runner
 from tap_tester.base_case import BaseCase
 
 
 class TestMixPanelBase(BaseCase):
-    """ Test the tap combined """
+    """Test the tap combined."""
+
     START_DATE_FORMAT = "%Y-%m-%dT00:00:00Z"
+    BOOKMARK_COMPARISON_FORMAT = "%Y-%m-%dT%H:%M:%S.%fZ"
     REPLICATION_KEYS = "valid-replication-keys"
     PRIMARY_KEYS = "table-key-properties"
     FOREIGN_KEYS = "table-foreign-key-properties"
     REPLICATION_METHOD = "forced-replication-method"
     INCREMENTAL = "INCREMENTAL"
     FULL_TABLE = "FULL_TABLE"
     API_LIMIT = 250
     TYPE = "platform.mixpanel"
+    OBEYS_START_DATE = "obey-start-date"
     start_date = ""
     end_date = ""
     eu_residency = True
 
     def tap_name(self):
-        """The name of the tap"""
+        """The name of the tap."""
         return "tap-mixpanel"
 
     def expected_metadata(self):
-        """The expected streams and metadata about the streams"""
+        """The expected streams and metadata about the streams."""
         return {
-            'export': {
+            "export": {
                 self.PRIMARY_KEYS: set(),
                 self.REPLICATION_METHOD: self.INCREMENTAL,
-                self.REPLICATION_KEYS: {'time'},
+                self.REPLICATION_KEYS: {"time"},
+                self.OBEYS_START_DATE: True,
             },
-            'engage': {
+            "engage": {
                 self.PRIMARY_KEYS: {"distinct_id"},
                 self.REPLICATION_METHOD: self.FULL_TABLE,
+                self.OBEYS_START_DATE: False,
             },
-            'funnels': {
-                self.PRIMARY_KEYS: {'funnel_id', 'date'},
+            "funnels": {
+                self.PRIMARY_KEYS: {"funnel_id", "date"},
                 self.REPLICATION_METHOD: self.INCREMENTAL,
-                self.REPLICATION_KEYS: {'datetime'},
+                self.REPLICATION_KEYS: {"datetime"},
+                self.OBEYS_START_DATE: True,
             },
-            'cohorts': {
+            "cohorts": {
                 self.PRIMARY_KEYS: {"id"},
                 self.REPLICATION_METHOD: self.FULL_TABLE,
+                self.OBEYS_START_DATE: False,
             },
-            'cohort_members': {
+            "cohort_members": {
                 self.PRIMARY_KEYS: {"cohort_id", "distinct_id"},
                 self.REPLICATION_METHOD: self.FULL_TABLE,
+                self.OBEYS_START_DATE: False,
             },
-            'revenue': {
+            "revenue": {
                 self.PRIMARY_KEYS: {"date"},
                 self.REPLICATION_METHOD: self.INCREMENTAL,
-                self.REPLICATION_KEYS: {'datetime'},
+                self.REPLICATION_KEYS: {"datetime"},
+                self.OBEYS_START_DATE: True,
             },
-
-            'annotations': {
+            "annotations": {
                 self.PRIMARY_KEYS: {"date"},
-                self.REPLICATION_METHOD: self.FULL_TABLE
-            }
+                self.REPLICATION_METHOD: self.FULL_TABLE,
+                self.OBEYS_START_DATE: False,
+            },
         }
 
     def setUp(self):
         missing_envs = []
         if self.eu_residency:
             creds = {"api_secret": "TAP_MIXPANEL_EU_RESIDENCY_API_SECRET"}
         else:
@@ -86,92 +90,103 @@
 
         if len(missing_envs) != 0:
             raise Exception("set " + ", ".join(missing_envs))
 
         BaseCase.setUp(self)
 
     def get_type(self):
-        """the expected url route ending"""
+        """The expected url route ending."""
         return "platform.mixpanel"
 
     def get_properties(self, original: bool = True):
         """Configuration properties required for the tap."""
 
         return_value = {
-            'start_date': '2020-02-01T00:00:00Z',
-            'end_date': '2020-03-01T00:00:00Z',
-            'date_window_size': '30',
-            'attribution_window': '5',
-            'project_timezone': 'US/Pacific',
-            "eu_residency": 'false',
-            'select_properties_by_default': 'false'
+            "start_date": "2020-02-01T00:00:00Z",
+            "end_date": "2020-03-01T00:00:00Z",
+            "date_window_size": "30",
+            "attribution_window": "5",
+            "project_timezone": "US/Pacific",
+            "eu_residency": "false",
+            "select_properties_by_default": "false",
         }
         if self.eu_residency:
-            return_value.update({"project_timezone": "Europe/Amsterdam", "eu_residency": 'true'})
+            return_value.update(
+                {"project_timezone": "Europe/Amsterdam", "eu_residency": "true"}
+            )
 
         if original:
             return return_value
 
         return_value["start_date"] = self.start_date
         return return_value
 
     def get_start_date(self):
         return dt.strftime(dt.utcnow() - timedelta(days=30), self.START_DATE_FORMAT)
 
     def get_credentials(self):
-        """Authentication information for the test account. Api secret is expected as a property."""
+        """
+        Authentication information for the test account.
+        Api secret is expected as a property.
+        """
 
         credentials_dict = {}
         if self.eu_residency:
             creds = {"api_secret": "TAP_MIXPANEL_EU_RESIDENCY_API_SECRET"}
         else:
             creds = {"api_secret": "TAP_MIXPANEL_API_SECRET"}
 
         for cred in creds:
             credentials_dict[cred] = os.getenv(creds[cred])
 
         return credentials_dict
 
     def expected_streams(self):
-        """A set of expected stream names"""
+        """A set of expected stream names."""
 
-        # Skip `export` and `revenue` stream for EU recidency server as
-        # revenue stream endpoint returns 400 bad reuqest and
+        # Skip `export` and `revenue` stream for EU residency server as
+        # revenue stream endpoint returns 400 bad request and
         # export stream endpoint returns 200 terminated early response.
         # So, as per discussion decided that let the customer come with the issues
         # that these streams are not working. Skip the streams in the circleci.
         if self.eu_residency:
             return set(self.expected_metadata().keys()) - {"export", "revenue"}
 
         return set(self.expected_metadata().keys())
 
     def expected_pks(self):
-        """return a dictionary with key of table name and value as a set of primary key fields"""
-        return {table: properties.get(self.PRIMARY_KEYS, set())
-                for table, properties
-                in self.expected_metadata().items()}
+        """Return a dictionary with key of table name and value as a set of primary key fields"""
+        return {
+            table: properties.get(self.PRIMARY_KEYS, set())
+            for table, properties in self.expected_metadata().items()
+        }
 
     def expected_replication_keys(self):
-        """return a dictionary with key of table name and value as a set of replication key fields"""
-        return {table: properties.get(self.REPLICATION_KEYS, set())
-                for table, properties
-                in self.expected_metadata().items()}
+        """Return a dictionary with key of table name and value as a set of replication key fields"""
+        return {
+            table: properties.get(self.REPLICATION_KEYS, set())
+            for table, properties in self.expected_metadata().items()
+        }
 
     def expected_replication_method(self):
-        """return a dictionary with key of table name nd value of replication method"""
-        return {table: properties.get(self.REPLICATION_METHOD, None)
-                for table, properties
-                in self.expected_metadata().items()}
+        """Return a dictionary with key of table name and value of replication method"""
+        return {
+            table: properties.get(self.REPLICATION_METHOD, None)
+            for table, properties in self.expected_metadata().items()
+        }
 
     def expected_automatic_fields(self):
-        """return a dictionary with key of table name and value as a set of automatic key fields"""
+        """Return a dictionary with key of table name and value as a set of automatic key fields"""
         auto_fields = {}
         for k, v in self.expected_metadata().items():
-            auto_fields[k] = v.get(self.PRIMARY_KEYS, set()) | v.get(self.REPLICATION_KEYS, set()) \
+            auto_fields[k] = (
+                v.get(self.PRIMARY_KEYS, set())
+                | v.get(self.REPLICATION_KEYS, set())
                 | v.get(self.FOREIGN_KEYS, set())
+            )
         return auto_fields
 
     #########################
     #   Helper Methods      #
     #########################
 
     def run_and_verify_check_mode(self, conn_id):
@@ -184,23 +199,26 @@
         check_job_name = runner.run_check_mode(self, conn_id)
 
         # verify check exit codes
         exit_status = menagerie.get_exit_status(conn_id, check_job_name)
         menagerie.verify_check_exit_status(self, exit_status, check_job_name)
 
         found_catalogs = menagerie.get_catalogs(conn_id)
-        self.assertGreater(len(
-            found_catalogs), 0, msg="unable to locate schemas for connection {}".format(conn_id))
+        self.assertGreater(
+            len(found_catalogs),
+            0,
+            msg=f"Unable to locate schemas for connection {conn_id}",
+        )
 
-        found_catalog_names = set(
-            map(lambda c: c['stream_name'], found_catalogs))
+        found_catalog_names = set(map(lambda c: c["stream_name"], found_catalogs))
 
         subset = self.expected_streams().issubset(found_catalog_names)
         self.assertTrue(
-            subset, msg="Expected check streams are not subset of discovered catalog")
+            subset, msg="Expected check streams are not subset of discovered catalog"
+        )
         LOGGER.info("discovered schemas are OK")
 
         return found_catalogs
 
     def run_and_verify_sync(self, conn_id):
         """
         Run a sync job and make sure it exited properly.
@@ -213,163 +231,185 @@
 
         # Verify tap and target exit codes
         exit_status = menagerie.get_exit_status(conn_id, sync_job_name)
         menagerie.verify_sync_exit_status(self, exit_status, sync_job_name)
 
         # Verify actual rows were synced
         sync_record_count = runner.examine_target_output_file(
-            self, conn_id, self.expected_streams(), self.expected_pks())
+            self, conn_id, self.expected_streams(), self.expected_pks()
+        )
         self.assertGreater(
-            sum(sync_record_count.values()), 0,
-            msg="failed to replicate any data: {}".format(sync_record_count)
+            sum(sync_record_count.values()),
+            0,
+            msg=f"failed to replicate any data: {sync_record_count}",
         )
         LOGGER.info(f"total replicated row count: {sum(sync_record_count.values())}")
 
         return sync_record_count
 
-    def perform_and_verify_table_and_field_selection(self, conn_id, test_catalogs, select_all_fields=True):
+    def perform_and_verify_table_and_field_selection(
+        self, conn_id, test_catalogs, select_all_fields=True
+    ):
         """
         Perform table and field selection based off of the streams to select
         set and field selection parameters.
-        Verify this results in the expected streams selected and all or no
-        fields selected for those streams.
+        Verify this results in the expected streams selected and all or
+        no fields selected for those streams.
         """
 
         # Select all available fields or select no fields from all testable streams
-        self.select_all_streams_and_fields(
-            conn_id, test_catalogs, select_all_fields)
+        self.select_all_streams_and_fields(conn_id, test_catalogs, select_all_fields)
 
         catalogs = menagerie.get_catalogs(conn_id)
 
         # Ensure our selection affects the catalog
-        expected_selected = [tc.get('stream_name') for tc in test_catalogs]
+        expected_selected = [cat.get("stream_name") for cat in test_catalogs]
 
         for cat in catalogs:
-            catalog_entry = menagerie.get_annotated_schema(
-                conn_id, cat['stream_id'])
+            catalog_entry = menagerie.get_annotated_schema(conn_id, cat["stream_id"])
 
             # Verify all testable streams are selected
-            selected = catalog_entry.get('annotated-schema').get('selected')
+            selected = catalog_entry.get("annotated-schema").get("selected")
             LOGGER.info(f"Validating selection on {cat['stream_name']}: {selected}")
 
-            if cat['stream_name'] not in expected_selected:
-                self.assertFalse(
-                    selected, msg="Stream selected, but not testable.")
+            if cat["stream_name"] not in expected_selected:
+                self.assertFalse(selected, msg="Stream selected, but not testable.")
                 continue  # Skip remaining assertions if we aren't selecting this stream
             self.assertTrue(selected, msg="Stream not selected.")
 
             if select_all_fields:
                 # Verify all fields within each selected stream are selected
-                for field, field_props in catalog_entry.get('annotated-schema').get('properties').items():
-                    field_selected = field_props.get('selected')
-                    LOGGER.info(f"\tValidating selection on {cat['stream_name']}.{field}: {field_selected}")
+                for field, field_props in (
+                    catalog_entry.get("annotated-schema").get("properties").items()
+                ):
+                    field_selected = field_props.get("selected")
+                    LOGGER.info(
+                        f"\tValidating selection on {cat['stream_name']}.{field}: {field_selected}"
+                    )
 
                     self.assertTrue(field_selected, msg="Field not selected.")
             else:
                 # Verify only automatic fields are selected
                 expected_automatic_fields = self.expected_automatic_fields().get(
-                    cat['stream_name'])
+                    cat["stream_name"]
+                )
                 selected_fields = self.get_selected_fields_from_metadata(
-                    catalog_entry['metadata'])
+                    catalog_entry["metadata"]
+                )
                 self.assertEqual(expected_automatic_fields, selected_fields)
 
     def get_selected_fields_from_metadata(self, metadata):
         selected_fields = set()
         for field in metadata:
-            is_field_metadata = len(field['breadcrumb']) > 1
+            is_field_metadata = len(field["breadcrumb"]) > 1
             inclusion_automatic_or_selected = (
-                field['metadata']['selected'] is True or
-                field['metadata']['inclusion'] == 'automatic'
+                field["metadata"]["selected"] is True or
+                field["metadata"]["inclusion"] == "automatic"
             )
             if is_field_metadata and inclusion_automatic_or_selected:
-                selected_fields.add(field['breadcrumb'][1])
+                selected_fields.add(field["breadcrumb"][1])
         return selected_fields
 
-    def select_all_streams_and_fields(self, conn_id, catalogs, select_all_fields: bool = True):
-        """Select all streams and all fields within streams"""
+    def select_all_streams_and_fields(
+        self, conn_id, catalogs, select_all_fields: bool = True
+    ):
+        """Select all streams and all fields within streams."""
         for catalog in catalogs:
-            schema = menagerie.get_annotated_schema(
-                conn_id, catalog['stream_id'])
+            schema = menagerie.get_annotated_schema(conn_id, catalog["stream_id"])
 
             non_selected_properties = []
             if not select_all_fields:
                 # get a list of all properties so that none are selected
-                non_selected_properties = schema.get('annotated-schema', {}).get(
-                    'properties', {}).keys()
+                non_selected_properties = (
+                    schema.get("annotated-schema", {}).get("properties", {}).keys()
+                )
 
             connections.select_catalog_and_fields_via_metadata(
-                conn_id, catalog, schema, [], non_selected_properties)
+                conn_id, catalog, schema, [], non_selected_properties
+            )
 
     def parse_date(self, date_value):
         """
         Pass in string-formatted-datetime, parse the value, and return it as an unformatted datetime object.
         """
         date_formats = {
             "%Y-%m-%dT%H:%M:%S.%fZ",
             "%Y-%m-%dT%H:%M:%SZ",
             "%Y-%m-%dT%H:%M:%S.%f+00:00",
             "%Y-%m-%dT%H:%M:%S+00:00",
-            "%Y-%m-%d"
+            "%Y-%m-%d",
         }
         for date_format in date_formats:
             try:
                 date_stripped = dt.strptime(date_value, date_format)
                 return date_stripped
             except ValueError:
                 continue
 
         raise NotImplementedError(
-            "Tests do not account for dates of this format: {}".format(date_value))
+            f"Tests do not account for dates of this format: {date_value}"
+        )
 
     def calculated_states_by_stream(self, current_state):
-        timedelta_by_stream = {stream: [1,0,0]  # {stream_name: [days, hours, minutes], ...}
-                               for stream in self.expected_streams()}
+        timedelta_by_stream = {
+            stream: [1, 0, 0]  # {stream_name: [days, hours, minutes], ...}
+            for stream in self.expected_streams()
+        }
 
-        stream_to_calculated_state = {stream: "" for stream in current_state['bookmarks'].keys()}
-        for stream, state in current_state['bookmarks'].items():
+        stream_to_calculated_state = {
+            stream: "" for stream in current_state["bookmarks"].keys()
+        }
+        for stream, state in current_state["bookmarks"].items():
 
             state_as_datetime = dateutil.parser.parse(state)
 
             days, hours, minutes = timedelta_by_stream[stream]
-            calculated_state_as_datetime = state_as_datetime - timedelta(days=days, hours=hours, minutes=minutes)
+            calculated_state_as_datetime = state_as_datetime - timedelta(
+                days=days, hours=hours, minutes=minutes
+            )
 
-            state_format = '%Y-%m-%dT%H:%M:%S-00:00'
-            calculated_state_formatted = dt.strftime(calculated_state_as_datetime, state_format)
+            state_format = "%Y-%m-%dT%H:%M:%S-00:00"
+            calculated_state_formatted = dt.strftime(
+                calculated_state_as_datetime, state_format
+            )
 
             stream_to_calculated_state[stream] = calculated_state_formatted
 
         return stream_to_calculated_state
 
     ##########################################################################
     # Tap Specific Methods
     ##########################################################################
 
     def convert_state_to_utc(self, date_str):
         """
         Convert a saved bookmark value of the form '2020-08-25T13:17:36-07:00' to
         a string formatted utc datetime,
-        in order to compare aginast json formatted datetime values
+        in order to compare against json formatted datetime values.
         """
         date_object = dateutil.parser.parse(date_str)
         date_object_utc = date_object.astimezone(tz=pytz.UTC)
         return dt.strftime(date_object_utc, "%Y-%m-%dT%H:%M:%SZ")
 
     def timedelta_formatted(self, dtime, days=0):
         try:
             date_stripped = dt.strptime(dtime, self.START_DATE_FORMAT)
             return_date = date_stripped + timedelta(days=days)
 
             return dt.strftime(return_date, self.START_DATE_FORMAT)
 
         except ValueError:
             try:
-                date_stripped = dt.strptime(
-                    dtime, self.BOOKMARK_COMPARISON_FORMAT)
+                date_stripped = dt.strptime(dtime, self.BOOKMARK_COMPARISON_FORMAT)
                 return_date = date_stripped + timedelta(days=days)
 
                 return dt.strftime(return_date, self.BOOKMARK_COMPARISON_FORMAT)
 
             except ValueError:
-                return Exception("Datetime object is not of the format: {}".format(self.START_DATE_FORMAT))
+                return Exception(
+                    f"Datetime object is not of the format: {self.START_DATE_FORMAT}"
+                )
 
     def is_incremental(self, stream):
-        return self.expected_metadata().get(stream).get(self.REPLICATION_METHOD) == self.INCREMENTAL
+        return (
+            self.expected_metadata().get(stream).get(self.REPLICATION_METHOD) == self.INCREMENTAL
+        )
```

### Comparing `tap-mixpanel-1.4.2/tests/tap_tester/test_all_fields_pagination.py` & `tap-mixpanel-1.4.3/tests/tap_tester/test_mixpanel_all_fields_pagination.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,32 @@
 from math import ceil
 
-import tap_tester.connections as connections
-import tap_tester.runner as runner
-import tap_tester.menagerie as menagerie
-from tap_tester.logger import LOGGER
+from tap_tester import connections, menagerie, runner
 
 from base import TestMixPanelBase
 
 
 class MixPanelPaginationAllFieldsTest(TestMixPanelBase):
 
     @staticmethod
     def name():
-        return "mixpanel_pagination_all_fields_test"
+        return "tap_tester_mixpanel_pagination_all_fields_test"
 
     def pagination_test_run(self):
         """
         All Fields Test
-        • and that when all fields are selected more than the automatic fields are replicated.
+        • Verify that when all fields are selected more than the automatic fields are replicated.
         • Verify no unexpected streams were replicated
         • Verify that more than just the automatic fields are replicated for each stream.
-        • verify all fields for each stream are replicated
-        • verify that the automatic fields are sent to the target
-
-
+        • Verify all fields for each stream are replicated
+        • Verify that the automatic fields are sent to the target
         Pagination Test
         • Verify that for each stream you can get multiple pages of data
         • Verify no duplicate pages are replicated
         • Verify no unexpected streams were replicated
-
         PREREQUISITE
         For EACH stream add enough data that you surpass the limit of a single
         fetch of data.  For instance if you have a limit of 250 records ensure
         that 251 (or more) records have been posted for that stream.
         """
 
         # Only following below 2 streams support pagination
@@ -40,32 +34,31 @@
         streams_to_test_pagination = {'engage', 'cohort_members'}
 
         expected_automatic_fields = self.expected_automatic_fields()
         conn_id = connections.ensure_connection(self)
 
         found_catalogs = self.run_and_verify_check_mode(conn_id)
 
-        # table and field selection
+        # Table and field selection
         test_catalogs_all_fields = [catalog for catalog in found_catalogs
                                     if catalog.get('tap_stream_id') in streams_to_test_all_fields]
 
         self.perform_and_verify_table_and_field_selection(
             conn_id, test_catalogs_all_fields)
 
-        # grab metadata after performing table-and-field selection to set expectations
+        # Grab metadata after performing table-and-field selection to set expectations
         # used for asserting all fields are replicated
         stream_to_all_catalog_fields = dict()
         for catalog in test_catalogs_all_fields:
             stream_id, stream_name = catalog['stream_id'], catalog['stream_name']
             catalog_entry = menagerie.get_annotated_schema(conn_id, stream_id)
             fields_from_field_level_md = [md_entry['breadcrumb'][1]
                                           for md_entry in catalog_entry['metadata']
                                           if md_entry['breadcrumb'] != []]
-            stream_to_all_catalog_fields[stream_name] = set(
-                fields_from_field_level_md)
+            stream_to_all_catalog_fields[stream_name] = set(fields_from_field_level_md)
 
         record_count_by_stream = self.run_and_verify_sync(conn_id)
 
         actual_fields_by_stream = runner.examine_target_output_for_fields()
 
         synced_records = runner.get_records_from_target_output()
 
@@ -73,27 +66,26 @@
         synced_stream_names = set(synced_records.keys())
         self.assertSetEqual(streams_to_test_all_fields, synced_stream_names)
 
         # All Fields Test
         for stream in streams_to_test_all_fields:
             with self.subTest(logging="Primary Functional Test", stream=stream):
 
-                # expected values
+                # Expected values
                 expected_all_keys = stream_to_all_catalog_fields[stream]
-                expected_automatic_keys = expected_automatic_fields.get(
-                    stream, set())
+                expected_automatic_keys = expected_automatic_fields.get(stream, set())
 
-                # collect actual values
+                # Collect actual values
                 messages = synced_records.get(stream)
                 actual_all_keys = set()
                 for message in messages['messages']:
                     if message['action'] == 'upsert':
                         actual_all_keys.update(set(message['data'].keys()))
 
-                # verify that the automatic fields are sent to the target
+                # Verify that the automatic fields are sent to the target
                 self.assertTrue(
                     actual_fields_by_stream.get(stream, set()).issuperset(
                         expected_automatic_keys),
                     msg="The fields sent to the target don't include all automatic fields")
 
                 # Verify that more than just the automatic fields are replicated for each stream.
                 if stream != "cohort_members":  # cohort_member has just 2 key and both are automatic
@@ -105,36 +97,36 @@
 
                 # As we can't find the below fields in the docs and also
                 # it won't be generated by mixpanel APIs now so expected.
                 if stream == "export":
                     expected_all_keys = expected_all_keys - {'labels', 'sampling_factor', 'dataset', 'mp_reserved_duration_s', 'mp_reserved_origin_end',
                                                              'mp_reserved_origin_start', 'mp_reserved_event_count'}
 
-                # verify all fields for each stream are replicated
-                if not stream == "engage": #Skip engage as it return records in random manner with dynamic fields.
+                # Verify all fields for each stream are replicated
+                # Skip engage as it return records in random manner with dynamic fields.
+                if not stream == "engage":
                     self.assertSetEqual(expected_all_keys, actual_all_keys)
 
         # Pagination Test
         for stream in streams_to_test_pagination:
             with self.subTest(stream=stream):
 
-                # expected values
+                # Expected values
                 expected_primary_keys = self.expected_pks()[stream]
 
-                # collect actual values
+                # Collect actual values
                 messages = synced_records.get(stream)
                 primary_keys_list = [tuple([message['data'][expected_pk] for expected_pk in expected_primary_keys])
                                      for message in messages['messages'] if message['action'] == 'upsert']
 
-                # verify that we can paginate with all fields selected
+                # Verify that we can paginate with all fields selected
                 record_count_sync = record_count_by_stream.get(stream, 0)
                 self.assertGreater(record_count_sync, self.API_LIMIT,
                                    msg="The number of records is not over the stream max limit")
 
-
                 # Chunk the replicated records (just primary keys) into expected pages
                 pages = []
                 page_count = ceil(len(primary_keys_list) / self.API_LIMIT)
                 page_size = self.API_LIMIT
                 for page_index in range(page_count):
                     page_start = page_index * page_size
                     page_end = (page_index + 1) * page_size
@@ -153,11 +145,10 @@
                             )
 
     def test_run(self):
         # Pagination test for standard server
         self.eu_residency = False
         self.pagination_test_run()
 
-
         # Pagination test for EU residency server
         self.eu_residency = True
         self.pagination_test_run()
```

### Comparing `tap-mixpanel-1.4.2/tests/tap_tester/test_automatic_fields.py` & `tap-mixpanel-1.4.3/tests/tap_tester/test_mixpanel_automatic_fields.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-import tap_tester.connections as connections
-import tap_tester.runner as runner
+from tap_tester import connections, runner
+
 from base import TestMixPanelBase
 
 
 class MixPanelAutomaticFieldsTest(TestMixPanelBase):
     """
-    Ensure running the tap with all streams selected and all fields deselected results in the replication of just the
+    Ensure running the tap with all streams selected and all fields
+    deselected results in the replication of just the
     primary keys and replication keys (automatic fields).
     """
 
     @staticmethod
     def name():
-        return "mix_panel_automatic_fields_test"
+        return "tap_tester_mixpanel_automatic_fields_test"
 
     def automatic_fields_test_run(self):
         """
-        Verify that for each stream you can get enough data
-        when no fields are selected and only the automatic fields are replicated.
+        • Verify we can deselect all fields except when inclusion=automatic,
+          which is handled by base.py methods
+        • Verify that only the automatic fields are sent to the target.
+        • Verify that all replicated records have unique primary key values.
         """
-        streams_to_test = self.expected_streams()
+        expected_streams = self.expected_streams()
 
         conn_id = connections.ensure_connection(self)
 
         found_catalogs = self.run_and_verify_check_mode(conn_id)
 
-        # table and field selection
-        test_catalogs_automatic_fields = [catalog for catalog in found_catalogs
-                                          if catalog.get('tap_stream_id') in streams_to_test]
+        # Table and field selection
+        test_catalogs_automatic_fields = [
+            catalog
+            for catalog in found_catalogs
+            if catalog.get("tap_stream_id") in expected_streams
+        ]
 
         self.perform_and_verify_table_and_field_selection(
             conn_id, test_catalogs_automatic_fields, select_all_fields=False)
 
         record_count_by_stream = self.run_and_verify_sync(conn_id)
         synced_records = runner.get_records_from_target_output()
 
-        for stream in streams_to_test:
+        for stream in expected_streams:
             with self.subTest(stream=stream):
 
-                # expected values
+                # Expected values
                 expected_keys = self.expected_automatic_fields().get(stream)
 
-                # collect actual values
+                # Collect actual values
                 data = synced_records.get(stream, {})
                 record_messages_keys = [set(row['data'].keys())
                                         for row in data.get('messages', [])]
 
                 # Verify that you get some records for each stream
                 self.assertGreater(
                     record_count_by_stream.get(stream, 0), 0,
                     msg="The number of records is not over the stream max limit",
                 )
 
                 # Verify that only the automatic fields are sent to the target
                 for actual_keys in record_messages_keys:
                     self.assertSetEqual(expected_keys, actual_keys)
 
-
     def test_standard_auto_fields(self):
         """Automatic fields test for standard server"""
         self.eu_residency = False
         self.automatic_fields_test_run()
-
-    def test_eu_auto_fields(self):
-        """Automatic fields test for EU recidency server"""
-        self.eu_residency = True
-        self.automatic_fields_test_run()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tap-mixpanel-1.4.2/tests/tap_tester/test_bookmark.py` & `tap-mixpanel-1.4.3/tests/tap_tester/test_mixpanel_bookmark.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-import tap_tester.connections as connections
-import tap_tester.runner as runner
+from tap_tester import menagerie, connections, runner
+
 from base import TestMixPanelBase
-from tap_tester import menagerie
 
 
 class MixPanelBookMarkTest(TestMixPanelBase):
     """Test tap sets a bookmark and respects it for the next sync of a stream"""
 
     @staticmethod
     def name():
-        return "mix_panel_bookmark_test"
+        return "tap_tester_mixpanel_bookmark_test"
 
     def bookmark_test_run(self):
         """
         Verify that for each stream you can do a sync which records bookmarks.
         That the bookmark is the maximum value sent to the target for the replication key.
         That a second sync respects the bookmark
             All data of the second sync is >= the bookmark from the first sync
@@ -36,35 +35,37 @@
         # First Sync
         ##########################################################################
         conn_id = connections.ensure_connection(self)
 
         # Run in check mode
         found_catalogs = self.run_and_verify_check_mode(conn_id)
 
-        # table and field selection
-        catalog_entries = [catalog for catalog in found_catalogs
-                           if catalog.get('tap_stream_id') in expected_streams]
+        # Table and field selection
+        catalog_entries = [
+            catalog
+            for catalog in found_catalogs
+            if catalog.get("tap_stream_id") in expected_streams
+        ]
 
         self.perform_and_verify_table_and_field_selection(
             conn_id, catalog_entries)
 
         # Run a first sync job using orchestrator
         first_sync_record_count = self.run_and_verify_sync(conn_id)
         first_sync_records = runner.get_records_from_target_output()
         first_sync_bookmarks = menagerie.get_state(conn_id)
 
         ##########################################################################
         # Update State Between Syncs
         ##########################################################################
 
-        new_states = {'bookmarks': dict()}
-        simulated_states = self.calculated_states_by_stream(
-            first_sync_bookmarks)
+        new_states = {"bookmarks": dict()}
+        simulated_states = self.calculated_states_by_stream(first_sync_bookmarks)
         for stream, new_state in simulated_states.items():
-            new_states['bookmarks'][stream] = new_state
+            new_states["bookmarks"][stream] = new_state
         menagerie.set_state(conn_id, new_states)
 
         ##########################################################################
         # Second Sync
         ##########################################################################
 
         second_sync_record_count = self.run_and_verify_sync(conn_id)
@@ -74,107 +75,117 @@
         ##########################################################################
         # Test By Stream
         ##########################################################################
 
         for stream in expected_streams:
             with self.subTest(stream=stream):
 
-                # expected values
+                # Expected values
                 expected_replication_method = expected_replication_methods[stream]
 
-                # collect information for assertions from syncs 1 & 2 base on expected values
+                # Collect information for assertions from syncs 1 & 2 base on expected values
                 first_sync_count = first_sync_record_count.get(stream, 0)
                 second_sync_count = second_sync_record_count.get(stream, 0)
-                first_sync_messages = [record.get('data') for record in
-                                       first_sync_records.get(
-                                           stream, {}).get('messages', [])
-                                       if record.get('action') == 'upsert']
-                second_sync_messages = [record.get('data') for record in
-                                        second_sync_records.get(
-                                            stream, {}).get('messages', [])
-                                        if record.get('action') == 'upsert']
+                first_sync_messages = [
+                    record.get("data")
+                    for record in first_sync_records.get(stream, {}).get("messages", [])
+                    if record.get("action") == "upsert"
+                ]
+                second_sync_messages = [
+                    record.get("data")
+                    for record in second_sync_records.get(stream, {}).get(
+                        "messages", []
+                    )
+                    if record.get("action") == "upsert"
+                ]
 
                 first_bookmark_value = first_sync_bookmarks.get(
-                    'bookmarks', {stream: None}).get(stream)
+                    "bookmarks", {stream: None}
+                ).get(stream)
                 second_bookmark_value = second_sync_bookmarks.get(
-                    'bookmarks', {stream: None}).get(stream)
+                    "bookmarks", {stream: None}
+                ).get(stream)
 
                 if expected_replication_method == self.INCREMENTAL:
 
-                    # collect information specific to incremental streams from syncs 1 & 2
-                    replication_key = next(
-                        iter(expected_replication_keys[stream]))
+                    # Collect information specific to incremental streams from syncs 1 & 2
+                    replication_key = next(iter(expected_replication_keys[stream]))
 
                     first_bookmark_value_utc = self.convert_state_to_utc(
                         first_bookmark_value)
                     second_bookmark_value_utc = self.convert_state_to_utc(
                         second_bookmark_value)
 
-                    simulated_bookmark = new_states['bookmarks'][stream]
+                    simulated_bookmark = new_states["bookmarks"][stream]
 
                     # Verify the first sync sets a bookmark of the expected form
                     self.assertIsNotNone(first_bookmark_value)
 
                     # Verify the second sync sets a bookmark of the expected form
                     self.assertIsNotNone(second_bookmark_value)
 
                     # Verify the second sync bookmark is Equal to the first sync bookmark
                     # assumes no changes to data during test
-                    self.assertEqual(second_bookmark_value,
-                                     first_bookmark_value)
+                    self.assertEqual(second_bookmark_value, first_bookmark_value)
 
                     for record in first_sync_messages:
 
                         # Verify the first sync bookmark value is the max replication key value for a given stream
                         replication_key_value = record.get(replication_key)
                         self.assertLessEqual(
-                            replication_key_value, first_bookmark_value_utc,
-                            msg="First sync bookmark was set incorrectly, a record with a greater replication-key value was synced."
+                            replication_key_value,
+                            first_bookmark_value_utc,
+                            msg="First sync bookmark was set incorrectly,"
+                            " a record with a greater replication-key value was synced.",
                         )
 
                     for record in second_sync_messages:
                         # Verify the second sync replication key value is Greater or Equal to the first sync bookmark
                         replication_key_value = record.get(replication_key)
-                        self.assertGreaterEqual(replication_key_value, simulated_bookmark,
-                                                msg="Second sync records do not repect the previous bookmark.")
+                        self.assertGreaterEqual(
+                            replication_key_value,
+                            simulated_bookmark,
+                            msg="Second sync records do not respect the previous bookmark.",
+                        )
 
                         # Verify the second sync bookmark value is the max replication key value for a given stream
                         self.assertLessEqual(
-                            replication_key_value, second_bookmark_value_utc,
-                            msg="Second sync bookmark was set incorrectly, a record with a greater replication-key value was synced."
+                            replication_key_value,
+                            second_bookmark_value_utc,
+                            msg="Second sync bookmark was set incorrectly,"
+                            " a record with a greater replication-key value was synced.",
                         )
 
-                    # verify that you get less data the 2nd time around
+                    # Verify that you get less data the 2nd time around
                     self.assertLess(
                         second_sync_count,
                         first_sync_count,
-                        msg="second syc didn't have less records, bookmark usage not verified")
+                        msg="Second syc didn't have less records, bookmark usage not verified",
+                    )
 
                 elif expected_replication_method == self.FULL_TABLE:
 
                     # Verify the syncs do not set a bookmark for full table streams
                     self.assertIsNone(first_bookmark_value)
                     self.assertIsNone(second_bookmark_value)
 
                     # Verify the number of records in the second sync is the same as the first
                     self.assertEqual(second_sync_count, first_sync_count)
 
                 else:
 
                     raise NotImplementedError(
-                        "INVALID EXPECTATIONS\t\tSTREAM: {} REPLICATION_METHOD: {}".format(
-                            stream, expected_replication_method)
+                        f"INVALID EXPECTATIONS\t\tSTREAM: {stream} REPLICATION_METHOD: "
+                        f"{expected_replication_method}"
                     )
 
                 # Verify at least 1 record was replicated in the second sync
                 self.assertGreater(
-                    second_sync_count, 0, msg="We are not fully testing bookmarking for {}".format(stream))
+                    second_sync_count,
+                    0,
+                    msg=f"We are not fully testing bookmarking for {stream}",
+                )
 
     def test_standard_bookmarks(self):
-        """Bookmark test for standard server"""
+        """Bookmark test for standard server."""
         self.eu_residency = False
         self.bookmark_test_run()
-
-    def test_eu_bookmarks(self):
-        """Bookmark test for EU recidency server"""
-        self.eu_residency = True
-        self.bookmark_test_run()
```

### Comparing `tap-mixpanel-1.4.2/tests/tap_tester/test_discovery.py` & `tap-mixpanel-1.4.3/tests/tap_tester/test_mixpanel_discovery.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 import re
-from tap_tester import menagerie, connections
-from tap_tester.logger import LOGGER
+from tap_tester import menagerie, connections, LOGGER
 
 from base import TestMixPanelBase
 
 class MixPanelDiscoverTest(TestMixPanelBase):
     """
         Testing that discovery creates the appropriate catalog with valid metadata.
         • Verify number of actual streams discovered match expected
         • Verify the stream names discovered were what we expect
         • Verify stream names follow naming convention
           streams should only have lowercase alphas and underscores
-        • verify there is only 1 top level breadcrumb
-        • verify replication key(s)
-        • verify primary key(s)
-        • verify that if there is a replication key we are doing INCREMENTAL otherwise FULL
-        • verify the actual replication matches our expected replication method
-        • verify that primary, replication and foreign keys
+        • Verify there is only 1 top level breadcrumb
+        • Verify replication key(s)
+        • Verify primary key(s)
+        • Verify that if there is a replication key we are doing INCREMENTAL otherwise FULL
+        • Verify the actual replication matches our expected replication method
+        • Verify that primary, replication and foreign keys
           are given the inclusion of automatic.
-        • verify that all other fields have inclusion of available metadata.
+        • Verify that all other fields have inclusion of available metadata.
     """
 
     @staticmethod
     def name():
-        return "mix_panel_discover_test"
+        return "tap_tester_mixpanel_discover_test"
 
     def discovery_test_run(self):
 
         region = "EU" if self.eu_residency else "Standard"
         LOGGER.info(f"Testing against {region} account.")
 
         self.assertion_logging_enabled = True
@@ -37,106 +36,155 @@
         conn_id = connections.ensure_connection(self, payload_hook=None)
 
         # Verify that there are catalogs found
         found_catalogs = self.run_and_verify_check_mode(conn_id)
 
         # Verify stream names follow naming convention
         # streams should only have lowercase alphas and underscores
-        found_catalog_names = {c['tap_stream_id'] for c in found_catalogs}
-        self.assertTrue(all([re.fullmatch(r"[a-z_]+",  name) for name in found_catalog_names]),
-                        logging="asserting all streams defined in catalog follow the naming convention '[a-z_]+'")
+        found_catalog_names = {c["tap_stream_id"] for c in found_catalogs}
+        self.assertTrue(
+            all([re.fullmatch(r"[a-z_]+", name) for name in found_catalog_names]),
+            logging="asserting all streams defined in catalog follow the naming convention '[a-z_]+'",
+        )
 
         for stream in streams_to_test:
             with self.subTest(stream=stream):
 
-                # Verify the caatalog is found for a given stream
-                catalog = next(iter([catalog for catalog in found_catalogs
-                                     if catalog["stream_name"] == stream]))
-                self.assertIsNotNone(catalog, logging="asserting entry is present in catalog")
+                # Verify the catalog is found for a given stream
+                catalog = next(
+                    iter(
+                        [
+                            catalog
+                            for catalog in found_catalogs
+                            if catalog["stream_name"] == stream
+                        ]
+                    )
+                )
+                self.assertIsNotNone(
+                    catalog, logging="Asserting entry is present in catalog"
+                )
 
-                # collecting expected values
+                # Collecting expected values
                 expected_primary_keys = self.expected_pks()[stream]
-                expected_replication_keys = self.expected_replication_keys()[
-                    stream]
+                expected_replication_keys = self.expected_replication_keys()[stream]
                 expected_automatic_fields = self.expected_automatic_fields().get(stream)
-                expected_replication_method = self.expected_replication_method()[
-                    stream]
+                expected_replication_method = self.expected_replication_method()[stream]
 
-                # collecting actual values...
+                # Collecting actual values...
                 schema_and_metadata = menagerie.get_annotated_schema(
-                    conn_id, catalog['stream_id'])
+                    conn_id, catalog["stream_id"]
+                )
                 metadata = schema_and_metadata["metadata"]
                 stream_properties = [
-                    item for item in metadata if item.get("breadcrumb") == []]
+                    item for item in metadata if item.get("breadcrumb") == []
+                ]
                 actual_primary_keys = set(
-                    stream_properties[0].get(
-                        "metadata", {self.PRIMARY_KEYS: []}).get(self.PRIMARY_KEYS, [])
+                    stream_properties[0]
+                    .get("metadata", {self.PRIMARY_KEYS: []})
+                    .get(self.PRIMARY_KEYS, [])
                 )
                 actual_replication_keys = set(
-                    stream_properties[0].get(
-                        "metadata", {self.REPLICATION_KEYS: []}).get(self.REPLICATION_KEYS, [])
+                    stream_properties[0]
+                    .get("metadata", {self.REPLICATION_KEYS: []})
+                    .get(self.REPLICATION_KEYS, [])
                 )
-                actual_replication_method = stream_properties[0].get(
-                    "metadata", {self.REPLICATION_METHOD: None}).get(self.REPLICATION_METHOD)
-                actual_automatic_fields = set(
-                    item.get("breadcrumb", ["properties", None])[1] for item in metadata
-                    if item.get("metadata").get("inclusion") == "automatic"
+                actual_replication_method = (
+                    stream_properties[0]
+                    .get("metadata", {self.REPLICATION_METHOD: None})
+                    .get(self.REPLICATION_METHOD)
                 )
+                actual_automatic_fields = {
+                    item.get("breadcrumb", ["properties", None])[1]
+                    for item in metadata
+                    if item.get("metadata").get("inclusion") == "automatic"
+                }
+
+                actual_fields = []
+                for md_entry in metadata:
+                    if md_entry["breadcrumb"] != []:
+                        actual_fields.append(md_entry["breadcrumb"][1])
 
                 ##########################################################################
-                # metadata assertions
+                # Metadata assertions
                 ##########################################################################
 
-                # verify there is only 1 top level breadcrumb in metadata
-                self.assertEqual(len(stream_properties), 1,
-                                 logging='asserting there is only 1 top level breadcrumb in metadata')
+                # Verify there is only 1 top level breadcrumb in metadata
+                self.assertEqual(
+                    len(stream_properties),
+                    1,
+                    logging="Asserting there is only 1 top level breadcrumb in metadata",
+                )
 
-                # verify that if there is a replication key we are doing INCREMENTAL otherwise FULL
+                # Verify there is no duplicate metadata entries
+                self.assertEqual(
+                    len(actual_fields),
+                    len(set(actual_fields)),
+                    msg="Duplicates in the fields retrieved",
+                )
+
+                # Verify that if there is a replication key we are doing INCREMENTAL otherwise FULL
                 if actual_replication_keys:
                     self.assertEqual(
-                        actual_replication_method, self.INCREMENTAL,
-                        logging=f"asserting replication method is {self.INCREMENTAL} when replication keys are defined"
+                        actual_replication_method,
+                        self.INCREMENTAL,
+                        logging=f"Asserting replication method is {self.INCREMENTAL} when replication keys are defined",
                     )
                 else:
                     self.assertEqual(
-                        actual_replication_method, self.FULL_TABLE,
-                        logging=f"asserting replication method is {self.FULL_TABLE} when replication keys are not defined"
+                        actual_replication_method,
+                        self.FULL_TABLE,
+                        logging=f"Asserting replication method is {self.FULL_TABLE} when replication keys are not defined",
                     )
 
-                # verify the actual replication matches our expected replication method
-                self.assertEqual(expected_replication_method, actual_replication_method,
-                                 logging=f"asserting replication method is {expected_replication_method}")
-
-                # verify replication key(s)
-                self.assertEqual(expected_replication_keys, actual_replication_keys,
-                                 logging=f"asserting replication keys are {expected_replication_keys}")
+                # Verify the actual replication matches our expected replication method
+                self.assertEqual(
+                    expected_replication_method,
+                    actual_replication_method,
+                    logging=f"Asserting replication method is {expected_replication_method}",
+                )
 
+                # Verify replication key(s)
+                self.assertEqual(
+                    expected_replication_keys,
+                    actual_replication_keys,
+                    logging=f"asserting replication keys are {expected_replication_keys}",
+                )
 
-                # verify primary key(s) match expectations
-                self.assertSetEqual(expected_primary_keys, actual_primary_keys,
-                                    logging=f"asserting primary keys are {expected_primary_keys}")
+                # Verify primary key(s) match expectations
+                self.assertSetEqual(
+                    expected_primary_keys,
+                    actual_primary_keys,
+                    logging=f"asserting primary keys are {expected_primary_keys}",
+                )
 
-                # verify that primary keys and replication keys
+                # Verify that primary keys and replication keys
                 # are given the inclusion of automatic in metadata.
-                self.assertSetEqual(expected_automatic_fields, actual_automatic_fields,
-                                    logging=f"asserting primary and replication keys {expected_automatic_fields} are automatic")
+                self.assertSetEqual(
+                    expected_automatic_fields,
+                    actual_automatic_fields,
+                    logging=f"asserting primary and replication keys {expected_automatic_fields} are automatic",
+                )
 
-                # verify that all other fields have inclusion of available
+                # Verify that all other fields have inclusion of available.
                 # This assumes there are no unsupported fields for SaaS sources
                 self.assertTrue(
-                    all({item.get("metadata").get("inclusion") == "available"
+                    all(
+                        {
+                            item.get("metadata").get("inclusion") == "available"
                          for item in metadata
                          if item.get("breadcrumb", []) != []
                          and item.get("breadcrumb", ["properties", None])[1]
-                         not in actual_automatic_fields}),
-                    logging=f"asserting non-key-property fields are available for field selection")
-
+                            not in actual_automatic_fields
+                        }
+                    ),
+                    logging="Asserting non-key-property fields are available for field selection",
+                )
 
     def test_standard_discovery(self):
-        """Discovery test for standard server"""
+        """Discovery test for standard server."""
         self.eu_residency = False
         self.discovery_test_run()
 
     def test_eu_discovery(self):
-        """Discovery test for EU recidency server"""
+        """Discovery test for EU residency server."""
         self.eu_residency = True
         self.discovery_test_run()
```

### Comparing `tap-mixpanel-1.4.2/tests/unittests/test_transform_event_times.py` & `tap-mixpanel-1.4.3/tests/unittests/test_transform_event_times.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,52 @@
-from tap_mixpanel.transform import transform_event_times
 import pytz
 import unittest
+
 from datetime import datetime
+from tap_mixpanel.transform import transform_event_times
 
 UTC = pytz.utc
 
 
 class TestTransformEventTimes(unittest.TestCase):
+    """
+    Test that `transform_event_times` function formats,
+    the Eastern and UTC formatted dates to ISO datetime.
+    """
 
     def test_utc_now(self):
-        
+        """
+        Testcase for the UTC timezone is converted to the given format.
+        """
+
         input_time = datetime.utcnow()
-        
+
         record = {"time": input_time.timestamp()}
         project_timezone = "UTC"
-        
+
         actual = transform_event_times(record, project_timezone)
-        expected = {"time": input_time.astimezone(UTC).strftime("%04Y-%m-%dT%H:%M:%S.000000Z")}
-        
+        expected = {
+            "time": input_time.astimezone(UTC).strftime("%04Y-%m-%dT%H:%M:%S.000000Z")
+        }
+
+        # Verify that record uis converted as expected.
         self.assertEqual(expected, actual)
-        
-        
+
     def test_eastern_time(self):
+        """
+        Testcase for the eastern timezone is converted to given formate.
+        """
+
         project_timezone = "US/Eastern"
         EASTERN = pytz.timezone(project_timezone)
         # This gives us 2021-08-12T11:00:00-4:00
         input_time = EASTERN.localize(datetime(2021, 8, 12, 11, 0, 0))
-        
+
         record = {"time": input_time.timestamp()}
         actual = transform_event_times(record, project_timezone)
-        
-        expected = {"time": input_time.astimezone(UTC).strftime("%04Y-%m-%dT%H:%M:%S.000000Z")}
 
-        self.assertEqual(expected, actual)
+        expected = {
+            "time": input_time.astimezone(UTC).strftime("%04Y-%m-%dT%H:%M:%S.000000Z")
+        }
+
+        # Verify that record uis converted as expected.
+        self.assertEqual(expected, actual)
```

