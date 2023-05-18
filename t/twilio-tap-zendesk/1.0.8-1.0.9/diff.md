# Comparing `tmp/twilio-tap-zendesk-1.0.8.tar.gz` & `tmp/twilio-tap-zendesk-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/aigupta/custom_singer_taps/twilio-tap-zendesk/dist/tmp6jorarh3/twilio-tap-zendesk-1.0.8.tar", last modified: Mon Oct  4 15:17:39 2021, max compression
+gzip compressed data, was "/Users/aigupta/custom_singer_taps/twilio-tap-zendesk/dist/tmpab4o48c1/twilio-tap-zendesk-1.0.9.tar", last modified: Tue Oct  5 10:32:16 2021, max compression
```

## Comparing `twilio-tap-zendesk-1.0.8.tar` & `twilio-tap-zendesk-1.0.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 aigupta    (501) staff       (20)        0 2021-10-04 15:17:39.000000 twilio-tap-zendesk-1.0.8/
--rw-r--r--   0 aigupta    (501) staff       (20)    32393 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.8/LICENSE
--rw-r--r--   0 aigupta    (501) staff       (20)      145 2021-10-04 15:16:02.000000 twilio-tap-zendesk-1.0.8/MANIFEST.in
--rw-r--r--   0 aigupta    (501) staff       (20)      345 2021-10-04 15:17:39.000000 twilio-tap-zendesk-1.0.8/PKG-INFO
--rw-r--r--   0 aigupta    (501) staff       (20)     2604 2021-10-04 15:16:48.000000 twilio-tap-zendesk-1.0.8/README.md
--rw-r--r--   0 aigupta    (501) staff       (20)       79 2021-10-04 15:17:39.000000 twilio-tap-zendesk-1.0.8/setup.cfg
--rw-r--r--   0 aigupta    (501) staff       (20)      814 2021-10-04 15:16:48.000000 twilio-tap-zendesk-1.0.8/setup.py
-drwxr-xr-x   0 aigupta    (501) staff       (20)        0 2021-10-04 15:17:39.000000 twilio-tap-zendesk-1.0.8/tap_zendesk/
--rwxr-xr-x   0 aigupta    (501) staff       (20)     8197 2021-10-04 15:16:48.000000 twilio-tap-zendesk-1.0.8/tap_zendesk/__init__.py
--rw-r--r--   0 aigupta    (501) staff       (20)     1071 2021-10-04 15:14:52.000000 twilio-tap-zendesk-1.0.8/tap_zendesk/discover.py
--rw-r--r--   0 aigupta    (501) staff       (20)     4101 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.8/tap_zendesk/metrics.py
-drwxr-xr-x   0 aigupta    (501) staff       (20)        0 2021-10-04 15:17:39.000000 twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/
--rw-r--r--   0 aigupta    (501) staff       (20)     3047 2021-10-04 15:16:48.000000 twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/agents_activity.json
--rw-r--r--   0 aigupta    (501) staff       (20)     1758 2021-10-04 15:16:48.000000 twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/articles.json
--rw-r--r--   0 aigupta    (501) staff       (20)     3974 2021-10-04 15:16:48.000000 twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/calls.json
--rw-r--r--   0 aigupta    (501) staff       (20)      694 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/group_memberships.json
--rw-r--r--   0 aigupta    (501) staff       (20)      774 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/groups.json
--rw-r--r--   0 aigupta    (501) staff       (20)     1744 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/macros.json
--rw-r--r--   0 aigupta    (501) staff       (20)     1619 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/organizations.json
--rw-r--r--   0 aigupta    (501) staff       (20)      842 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/satisfaction_ratings.json
-drwxr-xr-x   0 aigupta    (501) staff       (20)        0 2021-10-04 15:17:39.000000 twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/shared/
--rw-r--r--   0 aigupta    (501) staff       (20)     2615 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/shared/attachments.json
--rw-r--r--   0 aigupta    (501) staff       (20)     2493 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/shared/metadata.json
--rw-r--r--   0 aigupta    (501) staff       (20)     2340 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/shared/via.json
-drwxr-xr-x   0 aigupta    (501) staff       (20)        0 2021-10-04 15:17:39.000000 twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/sideload_schemas/
--rw-r--r--   0 aigupta    (501) staff       (20)      228 2021-10-04 15:16:02.000000 twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/sideload_schemas/comment_count.json
--rw-r--r--   0 aigupta    (501) staff       (20)     1265 2021-10-04 15:16:02.000000 twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/sideload_schemas/dates.json
--rw-r--r--   0 aigupta    (501) staff       (20)     4834 2021-10-04 15:16:02.000000 twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/sideload_schemas/metric_sets.json
--rw-r--r--   0 aigupta    (501) staff       (20)      968 2021-10-04 15:16:02.000000 twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/sideload_schemas/slas.json
--rw-r--r--   0 aigupta    (501) staff       (20)     2375 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/sla_policies.json
--rw-r--r--   0 aigupta    (501) staff       (20)      225 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/tags.json
--rw-r--r--   0 aigupta    (501) staff       (20)    18549 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/ticket_audits.json
--rw-r--r--   0 aigupta    (501) staff       (20)     1058 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/ticket_comments.json
--rw-r--r--   0 aigupta    (501) staff       (20)     3004 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/ticket_fields.json
--rw-r--r--   0 aigupta    (501) staff       (20)     1583 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/ticket_forms.json
--rw-r--r--   0 aigupta    (501) staff       (20)     1836 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/ticket_metric_events.json
--rw-r--r--   0 aigupta    (501) staff       (20)     4434 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/ticket_metrics.json
--rw-r--r--   0 aigupta    (501) staff       (20)     8763 2021-07-20 10:51:56.000000 twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/tickets.json
--rw-r--r--   0 aigupta    (501) staff       (20)     6457 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/users.json
--rw-r--r--   0 aigupta    (501) staff       (20)    27796 2021-10-04 15:16:48.000000 twilio-tap-zendesk-1.0.8/tap_zendesk/streams.py
--rw-r--r--   0 aigupta    (501) staff       (20)     2473 2021-08-26 12:10:29.000000 twilio-tap-zendesk-1.0.8/tap_zendesk/sync.py
-drwxr-xr-x   0 aigupta    (501) staff       (20)        0 2021-10-04 15:17:39.000000 twilio-tap-zendesk-1.0.8/test/
--rw-r--r--   0 aigupta    (501) staff       (20)     2992 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.8/test/test_all_streams.py
--rw-r--r--   0 aigupta    (501) staff       (20)     6753 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.8/test/test_bookmarks.py
--rw-r--r--   0 aigupta    (501) staff       (20)     1146 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.8/test/test_custom_fields_discover.py
--rw-r--r--   0 aigupta    (501) staff       (20)     2457 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.8/test/test_minimal_selection.py
-drwxr-xr-x   0 aigupta    (501) staff       (20)        0 2021-10-04 15:17:39.000000 twilio-tap-zendesk-1.0.8/twilio_tap_zendesk.egg-info/
--rw-r--r--   0 aigupta    (501) staff       (20)      345 2021-10-04 15:17:38.000000 twilio-tap-zendesk-1.0.8/twilio_tap_zendesk.egg-info/PKG-INFO
--rw-r--r--   0 aigupta    (501) staff       (20)     1530 2021-10-04 15:17:39.000000 twilio-tap-zendesk-1.0.8/twilio_tap_zendesk.egg-info/SOURCES.txt
--rw-r--r--   0 aigupta    (501) staff       (20)        1 2021-10-04 15:17:38.000000 twilio-tap-zendesk-1.0.8/twilio_tap_zendesk.egg-info/dependency_links.txt
--rw-r--r--   0 aigupta    (501) staff       (20)       74 2021-10-04 15:17:38.000000 twilio-tap-zendesk-1.0.8/twilio_tap_zendesk.egg-info/entry_points.txt
--rw-r--r--   0 aigupta    (501) staff       (20)       83 2021-10-04 15:17:38.000000 twilio-tap-zendesk-1.0.8/twilio_tap_zendesk.egg-info/requires.txt
--rw-r--r--   0 aigupta    (501) staff       (20)       12 2021-10-04 15:17:38.000000 twilio-tap-zendesk-1.0.8/twilio_tap_zendesk.egg-info/top_level.txt
+drwxr-xr-x   0 aigupta    (501) staff       (20)        0 2021-10-05 10:32:16.000000 twilio-tap-zendesk-1.0.9/
+-rw-r--r--   0 aigupta    (501) staff       (20)    32393 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.9/LICENSE
+-rw-r--r--   0 aigupta    (501) staff       (20)      145 2021-10-04 15:16:02.000000 twilio-tap-zendesk-1.0.9/MANIFEST.in
+-rw-r--r--   0 aigupta    (501) staff       (20)      345 2021-10-05 10:32:16.000000 twilio-tap-zendesk-1.0.9/PKG-INFO
+-rw-r--r--   0 aigupta    (501) staff       (20)     2604 2021-10-04 15:16:48.000000 twilio-tap-zendesk-1.0.9/README.md
+-rw-r--r--   0 aigupta    (501) staff       (20)       79 2021-10-05 10:32:16.000000 twilio-tap-zendesk-1.0.9/setup.cfg
+-rw-r--r--   0 aigupta    (501) staff       (20)      814 2021-10-05 10:31:37.000000 twilio-tap-zendesk-1.0.9/setup.py
+drwxr-xr-x   0 aigupta    (501) staff       (20)        0 2021-10-05 10:32:16.000000 twilio-tap-zendesk-1.0.9/tap_zendesk/
+-rwxr-xr-x   0 aigupta    (501) staff       (20)     8197 2021-10-04 15:16:48.000000 twilio-tap-zendesk-1.0.9/tap_zendesk/__init__.py
+-rw-r--r--   0 aigupta    (501) staff       (20)     1071 2021-10-04 15:14:52.000000 twilio-tap-zendesk-1.0.9/tap_zendesk/discover.py
+-rw-r--r--   0 aigupta    (501) staff       (20)     4101 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.9/tap_zendesk/metrics.py
+drwxr-xr-x   0 aigupta    (501) staff       (20)        0 2021-10-05 10:32:16.000000 twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/
+-rw-r--r--   0 aigupta    (501) staff       (20)     3047 2021-10-04 15:16:48.000000 twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/agents_activity.json
+-rw-r--r--   0 aigupta    (501) staff       (20)     1758 2021-10-04 15:16:48.000000 twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/articles.json
+-rw-r--r--   0 aigupta    (501) staff       (20)     4069 2021-10-05 10:31:37.000000 twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/calls.json
+-rw-r--r--   0 aigupta    (501) staff       (20)      694 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/group_memberships.json
+-rw-r--r--   0 aigupta    (501) staff       (20)      774 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/groups.json
+-rw-r--r--   0 aigupta    (501) staff       (20)     1744 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/macros.json
+-rw-r--r--   0 aigupta    (501) staff       (20)     1619 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/organizations.json
+-rw-r--r--   0 aigupta    (501) staff       (20)      842 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/satisfaction_ratings.json
+drwxr-xr-x   0 aigupta    (501) staff       (20)        0 2021-10-05 10:32:16.000000 twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/shared/
+-rw-r--r--   0 aigupta    (501) staff       (20)     2615 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/shared/attachments.json
+-rw-r--r--   0 aigupta    (501) staff       (20)     2493 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/shared/metadata.json
+-rw-r--r--   0 aigupta    (501) staff       (20)     2340 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/shared/via.json
+drwxr-xr-x   0 aigupta    (501) staff       (20)        0 2021-10-05 10:32:16.000000 twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/sideload_schemas/
+-rw-r--r--   0 aigupta    (501) staff       (20)      228 2021-10-04 15:16:02.000000 twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/sideload_schemas/comment_count.json
+-rw-r--r--   0 aigupta    (501) staff       (20)     1265 2021-10-04 15:16:02.000000 twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/sideload_schemas/dates.json
+-rw-r--r--   0 aigupta    (501) staff       (20)     4834 2021-10-04 15:16:02.000000 twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/sideload_schemas/metric_sets.json
+-rw-r--r--   0 aigupta    (501) staff       (20)      968 2021-10-04 15:16:02.000000 twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/sideload_schemas/slas.json
+-rw-r--r--   0 aigupta    (501) staff       (20)     2375 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/sla_policies.json
+-rw-r--r--   0 aigupta    (501) staff       (20)      225 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/tags.json
+-rw-r--r--   0 aigupta    (501) staff       (20)    18549 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/ticket_audits.json
+-rw-r--r--   0 aigupta    (501) staff       (20)     1058 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/ticket_comments.json
+-rw-r--r--   0 aigupta    (501) staff       (20)     3004 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/ticket_fields.json
+-rw-r--r--   0 aigupta    (501) staff       (20)     1583 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/ticket_forms.json
+-rw-r--r--   0 aigupta    (501) staff       (20)     1836 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/ticket_metric_events.json
+-rw-r--r--   0 aigupta    (501) staff       (20)     4434 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/ticket_metrics.json
+-rw-r--r--   0 aigupta    (501) staff       (20)     8763 2021-07-20 10:51:56.000000 twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/tickets.json
+-rw-r--r--   0 aigupta    (501) staff       (20)     6457 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/users.json
+-rw-r--r--   0 aigupta    (501) staff       (20)    27796 2021-10-04 15:16:48.000000 twilio-tap-zendesk-1.0.9/tap_zendesk/streams.py
+-rw-r--r--   0 aigupta    (501) staff       (20)     2473 2021-08-26 12:10:29.000000 twilio-tap-zendesk-1.0.9/tap_zendesk/sync.py
+drwxr-xr-x   0 aigupta    (501) staff       (20)        0 2021-10-05 10:32:16.000000 twilio-tap-zendesk-1.0.9/test/
+-rw-r--r--   0 aigupta    (501) staff       (20)     2992 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.9/test/test_all_streams.py
+-rw-r--r--   0 aigupta    (501) staff       (20)     6753 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.9/test/test_bookmarks.py
+-rw-r--r--   0 aigupta    (501) staff       (20)     1146 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.9/test/test_custom_fields_discover.py
+-rw-r--r--   0 aigupta    (501) staff       (20)     2457 2021-07-15 12:18:12.000000 twilio-tap-zendesk-1.0.9/test/test_minimal_selection.py
+drwxr-xr-x   0 aigupta    (501) staff       (20)        0 2021-10-05 10:32:16.000000 twilio-tap-zendesk-1.0.9/twilio_tap_zendesk.egg-info/
+-rw-r--r--   0 aigupta    (501) staff       (20)      345 2021-10-05 10:32:16.000000 twilio-tap-zendesk-1.0.9/twilio_tap_zendesk.egg-info/PKG-INFO
+-rw-r--r--   0 aigupta    (501) staff       (20)     1530 2021-10-05 10:32:16.000000 twilio-tap-zendesk-1.0.9/twilio_tap_zendesk.egg-info/SOURCES.txt
+-rw-r--r--   0 aigupta    (501) staff       (20)        1 2021-10-05 10:32:16.000000 twilio-tap-zendesk-1.0.9/twilio_tap_zendesk.egg-info/dependency_links.txt
+-rw-r--r--   0 aigupta    (501) staff       (20)       74 2021-10-05 10:32:16.000000 twilio-tap-zendesk-1.0.9/twilio_tap_zendesk.egg-info/entry_points.txt
+-rw-r--r--   0 aigupta    (501) staff       (20)       83 2021-10-05 10:32:16.000000 twilio-tap-zendesk-1.0.9/twilio_tap_zendesk.egg-info/requires.txt
+-rw-r--r--   0 aigupta    (501) staff       (20)       12 2021-10-05 10:32:16.000000 twilio-tap-zendesk-1.0.9/twilio_tap_zendesk.egg-info/top_level.txt
```

### Comparing `twilio-tap-zendesk-1.0.8/LICENSE` & `twilio-tap-zendesk-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `twilio-tap-zendesk-1.0.8/README.md` & `twilio-tap-zendesk-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `twilio-tap-zendesk-1.0.8/setup.py` & `twilio-tap-zendesk-1.0.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import setup
 
 setup(
       name='twilio-tap-zendesk',
-      version='1.0.8',
+      version='1.0.9',
       description='Singer.io tap for extracting data from the Zendesk API',
       author='Twilio',
       url='https://github.com/twilio-labs/twilio-tap-zendesk',
       classifiers=['Programming Language :: Python :: 3 :: Only'],
       py_modules=['tap_zendesk'],
       install_requires=[
           'pipelinewise-singer-python==1.2.0',
```

### Comparing `twilio-tap-zendesk-1.0.8/tap_zendesk/__init__.py` & `twilio-tap-zendesk-1.0.9/tap_zendesk/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-tap-zendesk-1.0.8/tap_zendesk/discover.py` & `twilio-tap-zendesk-1.0.9/tap_zendesk/discover.py`

 * *Files identical despite different names*

### Comparing `twilio-tap-zendesk-1.0.8/tap_zendesk/metrics.py` & `twilio-tap-zendesk-1.0.9/tap_zendesk/metrics.py`

 * *Files identical despite different names*

### Comparing `twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/agents_activity.json` & `twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/agents_activity.json`

 * *Files identical despite different names*

### Comparing `twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/articles.json` & `twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/articles.json`

 * *Files identical despite different names*

### Comparing `twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/calls.json` & `twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/calls.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9939024390243902%*

 * *Differences: {"'properties'": "{'call_group_id': OrderedDict([('type', ['null', 'integer'])])}"}*

```diff
@@ -8,14 +8,20 @@
         },
         "call_charge": {
             "type": [
                 "null",
                 "string"
             ]
         },
+        "call_group_id": {
+            "type": [
+                "null",
+                "integer"
+            ]
+        },
         "call_recording_consent": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "call_recording_consent_action": {
```

### Comparing `twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/group_memberships.json` & `twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/group_memberships.json`

 * *Files identical despite different names*

### Comparing `twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/groups.json` & `twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/groups.json`

 * *Files identical despite different names*

### Comparing `twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/macros.json` & `twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/macros.json`

 * *Files identical despite different names*

### Comparing `twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/organizations.json` & `twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/organizations.json`

 * *Files identical despite different names*

### Comparing `twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/satisfaction_ratings.json` & `twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/satisfaction_ratings.json`

 * *Files identical despite different names*

### Comparing `twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/shared/attachments.json` & `twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/shared/attachments.json`

 * *Files identical despite different names*

### Comparing `twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/shared/metadata.json` & `twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/shared/metadata.json`

 * *Files identical despite different names*

### Comparing `twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/shared/via.json` & `twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/shared/via.json`

 * *Files identical despite different names*

### Comparing `twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/sideload_schemas/dates.json` & `twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/sideload_schemas/dates.json`

 * *Files identical despite different names*

### Comparing `twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/sideload_schemas/metric_sets.json` & `twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/sideload_schemas/metric_sets.json`

 * *Files identical despite different names*

### Comparing `twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/sideload_schemas/slas.json` & `twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/sideload_schemas/slas.json`

 * *Files identical despite different names*

### Comparing `twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/sla_policies.json` & `twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/sla_policies.json`

 * *Files identical despite different names*

### Comparing `twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/ticket_audits.json` & `twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/ticket_audits.json`

 * *Files identical despite different names*

### Comparing `twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/ticket_comments.json` & `twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/ticket_comments.json`

 * *Files identical despite different names*

### Comparing `twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/ticket_fields.json` & `twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/ticket_fields.json`

 * *Files identical despite different names*

### Comparing `twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/ticket_forms.json` & `twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/ticket_forms.json`

 * *Files identical despite different names*

### Comparing `twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/ticket_metric_events.json` & `twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/ticket_metric_events.json`

 * *Files identical despite different names*

### Comparing `twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/ticket_metrics.json` & `twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/ticket_metrics.json`

 * *Files identical despite different names*

### Comparing `twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/tickets.json` & `twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/tickets.json`

 * *Files identical despite different names*

### Comparing `twilio-tap-zendesk-1.0.8/tap_zendesk/schemas/users.json` & `twilio-tap-zendesk-1.0.9/tap_zendesk/schemas/users.json`

 * *Files identical despite different names*

### Comparing `twilio-tap-zendesk-1.0.8/tap_zendesk/streams.py` & `twilio-tap-zendesk-1.0.9/tap_zendesk/streams.py`

 * *Files identical despite different names*

### Comparing `twilio-tap-zendesk-1.0.8/tap_zendesk/sync.py` & `twilio-tap-zendesk-1.0.9/tap_zendesk/sync.py`

 * *Files identical despite different names*

### Comparing `twilio-tap-zendesk-1.0.8/test/test_all_streams.py` & `twilio-tap-zendesk-1.0.9/test/test_all_streams.py`

 * *Files identical despite different names*

### Comparing `twilio-tap-zendesk-1.0.8/test/test_bookmarks.py` & `twilio-tap-zendesk-1.0.9/test/test_bookmarks.py`

 * *Files identical despite different names*

### Comparing `twilio-tap-zendesk-1.0.8/test/test_custom_fields_discover.py` & `twilio-tap-zendesk-1.0.9/test/test_custom_fields_discover.py`

 * *Files identical despite different names*

### Comparing `twilio-tap-zendesk-1.0.8/test/test_minimal_selection.py` & `twilio-tap-zendesk-1.0.9/test/test_minimal_selection.py`

 * *Files identical despite different names*

### Comparing `twilio-tap-zendesk-1.0.8/twilio_tap_zendesk.egg-info/SOURCES.txt` & `twilio-tap-zendesk-1.0.9/twilio_tap_zendesk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

