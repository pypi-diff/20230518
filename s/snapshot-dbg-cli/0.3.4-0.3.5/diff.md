# Comparing `tmp/snapshot-dbg-cli-0.3.4.tar.gz` & `tmp/snapshot-dbg-cli-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snapshot-dbg-cli-0.3.4.tar", last modified: Thu Mar 30 20:41:02 2023, max compression
+gzip compressed data, was "snapshot-dbg-cli-0.3.5.tar", last modified: Thu May 18 18:53:36 2023, max compression
```

## Comparing `snapshot-dbg-cli-0.3.4.tar` & `snapshot-dbg-cli-0.3.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 jcborg   (634821) primarygroup (89939)        0 2023-03-30 20:41:02.696456 snapshot-dbg-cli-0.3.4/
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)    11358 2023-03-30 16:35:20.000000 snapshot-dbg-cli-0.3.4/LICENSE
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)    23693 2023-03-30 20:41:02.696456 snapshot-dbg-cli-0.3.4/PKG-INFO
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)    22542 2023-03-30 16:35:20.000000 snapshot-dbg-cli-0.3.4/README.md
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     1262 2023-03-30 20:41:02.696456 snapshot-dbg-cli-0.3.4/setup.cfg
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)      760 2023-03-30 16:35:20.000000 snapshot-dbg-cli-0.3.4/setup.py
-drwxr-xr-x   0 jcborg   (634821) primarygroup (89939)        0 2023-03-30 20:41:02.696456 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     1105 2023-03-30 16:35:20.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/__init__.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)      703 2023-03-30 16:35:20.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/__main__.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     8566 2023-03-30 16:35:20.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/breakpoint_utils.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)      923 2023-03-30 16:35:20.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/cli.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     5209 2023-03-30 16:35:20.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/cli_common_arguments.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     2862 2023-03-30 16:35:20.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/cli_run.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)    10122 2023-03-30 16:35:20.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/cli_services.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3653 2023-03-30 19:59:07.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/cli_version.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     2399 2023-03-30 16:35:20.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/data_formatter.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     4432 2023-03-30 16:35:20.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/debuggee_utils.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3940 2023-03-30 16:35:20.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/delete_breakpoints.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     6683 2023-03-30 16:35:20.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/delete_debuggees_command.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3379 2023-03-30 16:35:20.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/delete_logpoints_command.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3336 2023-03-30 16:35:20.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/delete_snapshots_command.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)      982 2023-03-30 16:35:20.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/exceptions.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)    11110 2023-03-30 16:35:20.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/firebase_management_rest_service.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3009 2023-03-30 16:35:20.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/firebase_rtdb_rest_service.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     5780 2023-03-30 16:35:20.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/firebase_types.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     7871 2023-03-30 16:35:20.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/gcloud_cli_service.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3690 2023-03-30 16:35:20.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/get_logpoint_command.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     7186 2023-03-30 16:35:20.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/get_snapshot_command.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)    12100 2023-03-30 16:35:20.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/http_service.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)    17028 2023-03-30 16:35:20.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/init_command.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3556 2023-03-30 16:35:20.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/list_debuggees_command.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3678 2023-03-30 16:35:20.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/list_logpoints_command.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3604 2023-03-30 16:35:20.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/list_snapshots_command.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     4436 2023-03-30 16:35:20.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/permissions_rest_service.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     7346 2023-03-30 16:35:20.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/set_logpoint_command.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     4911 2023-03-30 16:35:20.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/set_snapshot_command.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)    12463 2023-03-30 16:35:20.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/snapshot_debugger_rtdb_service.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3878 2023-03-30 16:35:20.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/snapshot_debugger_schema.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     5131 2023-03-30 16:35:20.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/snapshot_parser.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3977 2023-03-30 16:35:20.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/status_message.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     2769 2023-03-30 16:35:20.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/time_utils.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     1091 2023-03-30 16:35:20.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/user_input.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     4357 2023-03-30 16:35:20.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/user_output.py
-drwxr-xr-x   0 jcborg   (634821) primarygroup (89939)        0 2023-03-30 20:41:02.696456 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli.egg-info/
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)    23693 2023-03-30 20:41:02.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli.egg-info/PKG-INFO
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     1606 2023-03-30 20:41:02.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli.egg-info/SOURCES.txt
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)        1 2023-03-30 20:41:02.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli.egg-info/dependency_links.txt
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)       63 2023-03-30 20:41:02.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli.egg-info/entry_points.txt
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)       17 2023-03-30 20:41:02.000000 snapshot-dbg-cli-0.3.4/snapshot_dbg_cli.egg-info/top_level.txt
+drwxr-xr-x   0 jcborg   (634821) primarygroup (89939)        0 2023-05-18 18:53:36.207439 snapshot-dbg-cli-0.3.5/
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)    11358 2023-05-16 20:47:12.000000 snapshot-dbg-cli-0.3.5/LICENSE
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)    26475 2023-05-18 18:53:36.207439 snapshot-dbg-cli-0.3.5/PKG-INFO
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)    25324 2023-05-18 18:18:38.000000 snapshot-dbg-cli-0.3.5/README.md
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     1262 2023-05-18 18:53:36.207439 snapshot-dbg-cli-0.3.5/setup.cfg
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)      760 2023-05-16 20:47:12.000000 snapshot-dbg-cli-0.3.5/setup.py
+drwxr-xr-x   0 jcborg   (634821) primarygroup (89939)        0 2023-05-18 18:53:36.207439 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     1105 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/__init__.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)      703 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/__main__.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     8566 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/breakpoint_utils.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)      923 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/cli.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     5209 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/cli_common_arguments.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     2862 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/cli_run.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)    10122 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/cli_services.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3653 2023-05-18 18:48:59.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/cli_version.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     2399 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/data_formatter.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     4432 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/debuggee_utils.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3940 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/delete_breakpoints.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     6683 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/delete_debuggees_command.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3379 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/delete_logpoints_command.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3336 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/delete_snapshots_command.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)      982 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/exceptions.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)    11830 2023-05-18 18:18:38.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/firebase_management_rest_service.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3009 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/firebase_rtdb_rest_service.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     6212 2023-05-18 18:18:38.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/firebase_types.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     7871 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/gcloud_cli_service.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3690 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/get_logpoint_command.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     7186 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/get_snapshot_command.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)    12100 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/http_service.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)    17906 2023-05-18 18:18:38.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/init_command.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3556 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/list_debuggees_command.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3678 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/list_logpoints_command.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3604 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/list_snapshots_command.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     4436 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/permissions_rest_service.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     7346 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/set_logpoint_command.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     4911 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/set_snapshot_command.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)    12463 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/snapshot_debugger_rtdb_service.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3878 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/snapshot_debugger_schema.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     5131 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/snapshot_parser.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3977 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/status_message.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     2769 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/time_utils.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     1091 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/user_input.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     4357 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/user_output.py
+drwxr-xr-x   0 jcborg   (634821) primarygroup (89939)        0 2023-05-18 18:53:36.207439 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli.egg-info/
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)    26475 2023-05-18 18:53:36.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli.egg-info/PKG-INFO
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     1606 2023-05-18 18:53:36.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)        1 2023-05-18 18:53:36.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)       63 2023-05-18 18:53:36.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli.egg-info/entry_points.txt
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)       17 2023-05-18 18:53:36.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli.egg-info/top_level.txt
```

### Comparing `snapshot-dbg-cli-0.3.4/LICENSE` & `snapshot-dbg-cli-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.4/PKG-INFO` & `snapshot-dbg-cli-0.3.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: snapshot-dbg-cli
-Version: 0.3.4
-Summary: 'Snapshot Debugger CLI tool.'
-Home-page: https://github.com/GoogleCloudPlatform/snapshot-debugger
-Author: Google Inc.
-License: Apache License, Version 2.0
-Project-URL: CLI Source, https://github.com/GoogleCloudPlatform/snapshot-debugger
-Project-URL: Java Agent Source, https://github.com/GoogleCloudPlatform/cloud-debug-java
-Project-URL: Node.js Agent Source, https://github.com/googleapis/cloud-debug-nodejs
-Project-URL: Python Agent Source, https://github.com/GoogleCloudPlatform/cloud-debug-python
-Keywords: cloud,snapshot,debugger
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Debuggers
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Snapshot Debugger
 
 The Snapshot Debugger  lets you inspect the state of a running cloud
 application, at any code location, without stopping or slowing it down. It’s not
 your traditional process debugger but rather an always on, whole app debugger
 taking snapshots from any instance of the app.
 
@@ -270,14 +245,50 @@
   state:        ACTIVE
 ```
 
 Note: The information printed by the `init` command can be accessed from within
 your Firebase project. It’s safe to run the `snapshot-dbg-cli init
 --use-default-rtdb` command multiple times to view this information.
 
+#### Setting up Firebase RTDB in other regions
+
+By default, `snapshot-dbg-cli init` will create a Firebase Realtime Database in
+`us-central1`.  It is possible to create and use a database in any region
+supported by Firebase Realtime Database.  See
+[supported RTDB locations][rtdb_locations].
+
+Setting up your database in a non-default region comes with some trade-offs:
+*  As a positive, you get to control where your snapshot data will be stored.
+   This may be important for compliance reasons.
+*  As a negative, the vsCode extension and agents will be unable to
+   automatically find the database.  The database URL will need to be provided
+   explicitly via configuration, see the following for details:
+   * [Configuring the Java Agent][java_agent_config]
+   * [Configuring the Python Agent][python_agent_config]
+   * [Configuring the Node.js Agent][nodejs_agent_config]
+   * [Configuring the VsCode Extension][extension_config]
+
+You can set up your database in a non-default location as follows:
+```
+snapshot-dbg-cli init --location={YOUR_LOCATION}
+```
+
+For example, you may want to set up your database in Belgium, and so would run
+```snapshot-dbg-cli init --location=europe-west1```
+
+Make note of the database URL provided in the command output; you will need to
+provide this to your debug agent(s) and the vsCode plugin.
+
+[rtdb_locations]: https://firebase.google.com/docs/projects/locations#rtdb-locations
+[java_agent_config]: https://github.com/GoogleCloudPlatform/cloud-debug-java#snapshot-debugger---firebase-realtime-database-backend
+[python_agent_config]: https://github.com/GoogleCloudPlatform/cloud-debug-python/blob/main/README.md#snapshot-debugger---firebase-realtime-database-backend
+[nodejs_agent_config]: https://github.com/googleapis/cloud-debug-nodejs/blob/main/README.md#snapshot-debugger---firebase-realtime-database-backend
+[extension_config]: https://github.com/GoogleCloudPlatform/snapshot-debugger/blob/main/snapshot_dbg_extension/README.md#configuration
+
+
 ## Set up Snapshot Debugger in your Google Cloud project
 
 ### Working Samples
 
 Working examples of using the Snapshot Debugger with Java, Python and Node.js
 applications across different Google Cloud environments can be found in:
 
@@ -695,14 +706,31 @@
 
 
 Do you want to continue (Y/n)?
 Deleted 4 snapshots.
 ```
 
 
+## VSCode Extension
+
+There is a VSCode extension for the Snapshot Debugger.  You can use this
+extension to set logpoints, set breakpoints and view snapshots in the comfort
+of your IDE.  See the [extension's README][extension-readme] for more details.
+
+You can install the extension by downloading it from the
+[most recent release][extension-release], and then running
+`code --install-extension snapshotdbg-*.vsix`.
+
+Note that you will still need to use the Snapshot Debugger CLI to set up your
+environment and to purge old data.  Gcloud needs to be installed for credential
+management.
+
+[extension-release]: https://github.com/GoogleCloudPlatform/snapshot-debugger/releases
+[extension-readme]: https://github.com/GoogleCloudPlatform/snapshot-debugger/blob/main/snapshot_dbg_extension/README.md
+
 ## Troubleshooting
 
 See [Snapshot Debugger Troubleshooting][troubleshooting]
 
 [troubleshooting]: https://github.com/GoogleCloudPlatform/snapshot-debugger/blob/main/docs/troubleshooting.md
 
 ## Firebase DB Schema
```

### Comparing `snapshot-dbg-cli-0.3.4/README.md` & `snapshot-dbg-cli-0.3.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: snapshot-dbg-cli
+Version: 0.3.5
+Summary: 'Snapshot Debugger CLI tool.'
+Home-page: https://github.com/GoogleCloudPlatform/snapshot-debugger
+Author: Google Inc.
+License: Apache License, Version 2.0
+Project-URL: CLI Source, https://github.com/GoogleCloudPlatform/snapshot-debugger
+Project-URL: Java Agent Source, https://github.com/GoogleCloudPlatform/cloud-debug-java
+Project-URL: Node.js Agent Source, https://github.com/googleapis/cloud-debug-nodejs
+Project-URL: Python Agent Source, https://github.com/GoogleCloudPlatform/cloud-debug-python
+Keywords: cloud,snapshot,debugger
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development :: Debuggers
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Snapshot Debugger
 
 The Snapshot Debugger  lets you inspect the state of a running cloud
 application, at any code location, without stopping or slowing it down. It’s not
 your traditional process debugger but rather an always on, whole app debugger
 taking snapshots from any instance of the app.
 
@@ -245,14 +270,50 @@
   state:        ACTIVE
 ```
 
 Note: The information printed by the `init` command can be accessed from within
 your Firebase project. It’s safe to run the `snapshot-dbg-cli init
 --use-default-rtdb` command multiple times to view this information.
 
+#### Setting up Firebase RTDB in other regions
+
+By default, `snapshot-dbg-cli init` will create a Firebase Realtime Database in
+`us-central1`.  It is possible to create and use a database in any region
+supported by Firebase Realtime Database.  See
+[supported RTDB locations][rtdb_locations].
+
+Setting up your database in a non-default region comes with some trade-offs:
+*  As a positive, you get to control where your snapshot data will be stored.
+   This may be important for compliance reasons.
+*  As a negative, the vsCode extension and agents will be unable to
+   automatically find the database.  The database URL will need to be provided
+   explicitly via configuration, see the following for details:
+   * [Configuring the Java Agent][java_agent_config]
+   * [Configuring the Python Agent][python_agent_config]
+   * [Configuring the Node.js Agent][nodejs_agent_config]
+   * [Configuring the VsCode Extension][extension_config]
+
+You can set up your database in a non-default location as follows:
+```
+snapshot-dbg-cli init --location={YOUR_LOCATION}
+```
+
+For example, you may want to set up your database in Belgium, and so would run
+```snapshot-dbg-cli init --location=europe-west1```
+
+Make note of the database URL provided in the command output; you will need to
+provide this to your debug agent(s) and the vsCode plugin.
+
+[rtdb_locations]: https://firebase.google.com/docs/projects/locations#rtdb-locations
+[java_agent_config]: https://github.com/GoogleCloudPlatform/cloud-debug-java#snapshot-debugger---firebase-realtime-database-backend
+[python_agent_config]: https://github.com/GoogleCloudPlatform/cloud-debug-python/blob/main/README.md#snapshot-debugger---firebase-realtime-database-backend
+[nodejs_agent_config]: https://github.com/googleapis/cloud-debug-nodejs/blob/main/README.md#snapshot-debugger---firebase-realtime-database-backend
+[extension_config]: https://github.com/GoogleCloudPlatform/snapshot-debugger/blob/main/snapshot_dbg_extension/README.md#configuration
+
+
 ## Set up Snapshot Debugger in your Google Cloud project
 
 ### Working Samples
 
 Working examples of using the Snapshot Debugger with Java, Python and Node.js
 applications across different Google Cloud environments can be found in:
 
@@ -670,14 +731,31 @@
 
 
 Do you want to continue (Y/n)?
 Deleted 4 snapshots.
 ```
 
 
+## VSCode Extension
+
+There is a VSCode extension for the Snapshot Debugger.  You can use this
+extension to set logpoints, set breakpoints and view snapshots in the comfort
+of your IDE.  See the [extension's README][extension-readme] for more details.
+
+You can install the extension by downloading it from the
+[most recent release][extension-release], and then running
+`code --install-extension snapshotdbg-*.vsix`.
+
+Note that you will still need to use the Snapshot Debugger CLI to set up your
+environment and to purge old data.  Gcloud needs to be installed for credential
+management.
+
+[extension-release]: https://github.com/GoogleCloudPlatform/snapshot-debugger/releases
+[extension-readme]: https://github.com/GoogleCloudPlatform/snapshot-debugger/blob/main/snapshot_dbg_extension/README.md
+
 ## Troubleshooting
 
 See [Snapshot Debugger Troubleshooting][troubleshooting]
 
 [troubleshooting]: https://github.com/GoogleCloudPlatform/snapshot-debugger/blob/main/docs/troubleshooting.md
 
 ## Firebase DB Schema
```

### Comparing `snapshot-dbg-cli-0.3.4/setup.cfg` & `snapshot-dbg-cli-0.3.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.4/setup.py` & `snapshot-dbg-cli-0.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/__init__.py` & `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/__main__.py` & `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/breakpoint_utils.py` & `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/breakpoint_utils.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/cli.py` & `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/cli.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/cli_common_arguments.py` & `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/cli_common_arguments.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/cli_run.py` & `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/cli_run.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/cli_services.py` & `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/cli_services.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/cli_version.py` & `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/cli_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import sys
 
 from snapshot_dbg_cli.data_formatter import DataFormatter
 from snapshot_dbg_cli.exceptions import SilentlyExitError
 from snapshot_dbg_cli.http_service import HttpService
 from snapshot_dbg_cli.user_output import UserOutput
 
-VERSION = 'SNAPSHOT_DEBUGGER_CLI_VERSION_0_3_4'
+VERSION = 'SNAPSHOT_DEBUGGER_CLI_VERSION_0_3_5'
 
 VERSION_PATTERN = 'SNAPSHOT_DEBUGGER_CLI_VERSION_[0-9]+_[0-9]+_[0-9]+'
 
 VERSION_URL = ('https://raw.githubusercontent.com/GoogleCloudPlatform'
                '/snapshot-debugger/main/snapshot_dbg_cli/cli_version.py')
 
 NEWER_VERSION_MESSAGE = """
```

### Comparing `snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/data_formatter.py` & `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/data_formatter.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/debuggee_utils.py` & `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/debuggee_utils.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/delete_breakpoints.py` & `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/delete_breakpoints.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/delete_debuggees_command.py` & `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/delete_debuggees_command.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/delete_logpoints_command.py` & `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/delete_logpoints_command.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/delete_snapshots_command.py` & `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/delete_snapshots_command.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/exceptions.py` & `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/firebase_management_rest_service.py` & `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/firebase_management_rest_service.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,14 +54,17 @@
 RTDB_INSTANCE_GET_STATE_ERROR_MSG = """
   ERROR. Expected to find the 'state' field populated in the database instance
   response with a value of 'ACTIVE'. However the response was the following:
 
   {response}
 """
 
+VALID_LOCATIONS_URL = (
+    "https://firebase.google.com/docs/projects/locations#rtdb-locations")
+
 
 class FirebaseManagementRestService:
   """Implements a service for making Firebase RTDB management REST requests.
 
   This service is for making management/admin related Firebase RTDB
   requests/queries using the REST interface, which is documented at
   https://firebase.google.com/docs/projects/api/reference/rest/v1beta1/projects/.
@@ -278,14 +281,28 @@
       if err.code == 400:
         try:
           parsed_error = json.loads(error_message)
           if parsed_error["error"]["status"] == "FAILED_PRECONDITION":
             self._user_output.debug("Got 400:", parsed_error)
             return DatabaseCreateResponse(
                 DatabaseCreateStatus.FAILED_PRECONDITION)
+
+          if parsed_error["error"]["status"] == "INVALID_ARGUMENT":
+            print_http_error(
+                self._user_output, request, err, error_message=error_message)
+
+            self._user_output.error(
+                "This was attempting to create the database instance. One "
+                "potential reason for this is if an invalid location was "
+                "specified, valid locations for RTDBs can be found at "
+                f"{VALID_LOCATIONS_URL}. To note, valid RTDB locations are a "
+                "subset of valid Google Cloud regions.")
+
+            raise SilentlyExitError from err
+
         except (TypeError, KeyError, ValueError):
           pass
 
       print_http_error(
           self._user_output, request, err, error_message=error_message)
       raise SilentlyExitError from err
     except ValueError as e:
```

### Comparing `snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/firebase_rtdb_rest_service.py` & `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/firebase_rtdb_rest_service.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/firebase_types.py` & `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/firebase_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 """A collection of types representing Firebase entities and responses.
 
 The types here help work with the data and response messages from Firebase.
 """
 
 from enum import Enum
+import re
 
 FIREBASE_MANAGMENT_API_SERVICE = 'firebase.googleapis.com'
 FIREBASE_RTDB_MANAGMENT_API_SERVICE = 'firebasedatabase.googleapis.com'
 
 
 class FirebaseProjectStatus(Enum):
   ENABLED = 1
@@ -119,20 +120,34 @@
     """
     try:
       self.name = database_instance['name']
       self.project = database_instance['project']
       self.database_url = database_instance['databaseUrl']
       self.type = database_instance['type']
       self.state = database_instance['state']
+      self.location = self.extract_location(self.name)
+
+      if self.location is None:
+        raise ValueError(
+            f"Failed to extract location from project name '{self.name}'")
+
     except KeyError as e:
       missing_key = e.args[0]
       error_message = ('DatabaseInstance is missing expected field '
                        f"'{missing_key}' instance: {database_instance}")
       raise ValueError(error_message) from e
 
+  @staticmethod
+  def extract_location(name):
+    location_search = re.search('/locations/([^/]+)/', name)
+    if not location_search or len(location_search.groups()) != 1:
+      return None
+
+    return location_search.groups()[0]
+
 
 class DatabaseCreateResponse:
   """Represents the response of a database create request.
 
   The database_instance field is only valid if the status is SUCCESS, it will
   be None otherwise.
   """
```

### Comparing `snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/gcloud_cli_service.py` & `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/gcloud_cli_service.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/get_logpoint_command.py` & `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/get_logpoint_command.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/get_snapshot_command.py` & `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/get_snapshot_command.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/http_service.py` & `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/http_service.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/init_command.py` & `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/init_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -188,14 +188,29 @@
   name:         {db_name}
   project:      {db_project}
   database url: {db_url}
   type:         {db_type}
   state:        {db_state}
 """
 
+LOCATION_MISMATCH_ERROR_MSG = (
+    "ERROR the following database already exists: '{full_database_name}', "
+    "however its location '{existing_location}' does not match the requested "
+    "location '{requested_location}'.\n\n"
+    "The database ID ('{database_id}' in this case) must be unique across "
+    'locations and projects.\n\n'
+    "If you meant to finalize the initialization of '{database_id}' in "
+    "'{requested_location}' (or verify it is already correctly initialized) "
+    "rerun the init command and specify '--location={existing_location}'.\n\n"
+    "If you meant to create a new database in '{requested_location}', given "
+    "'{database_id}' is already in use, you'll need to use a new name by "
+    "providing the '--database-id' argument to the init command. Note, even "
+    "if you delete '{database_id}', the name will remain reserved and will not "
+    'be available to be reused in a new location, a new name must be chosen.')
+
 
 class InitCommand:
   """This class implements the init command.
 
   The register() method is called by the CLI startup code to install the init
   command information, and the cmd() function will be invoked if the init
   command was specified by the user.
@@ -218,40 +233,27 @@
         help=DATABASE_ID_HELP.format(
             default_database_id=SNAPSHOT_DEBUGGER_DEFAULT_DB_ID))
 
     parser.set_defaults(func=self.cmd)
 
     # Only some locations are supported, see:
     # https://firebase.google.com/docs/projects/locations#rtdb-locations
-    #
-    # If unsupported location is used, this error occurs
-    # "error": {
-    #   "code": 400,
-    #   "message": "Request contains an invalid argument.",
-    #   "status": "INVALID_ARGUMENT"
-    # }
-    # For now however we only support 'us-central1'
     parser.add_argument(
         '-l', '--location', help=LOCATION_HELP, default=DEFAULT_LOCATION)
     self.args_parser = parser
 
   def cmd(self, args, cli_services):
     self.services = cli_services
     self.user_output = cli_services.user_output
     self.firebase_management_service = \
         cli_services.firebase_management_service
     self.gcloud_service = cli_services.gcloud_service
     self.permissions_service = cli_services.permissions_service
     self.project_id = cli_services.project_id
 
-    if args.location != DEFAULT_LOCATION:
-      self.user_output.error('ERROR: Currently the only supported location is '
-                             f"'{DEFAULT_LOCATION}'")
-      raise SilentlyExitError
-
     # If the user does not have the required permissions this will emit an error
     # message and exit.
     self.permissions_service.check_required_permissions(REQUIRED_PERMISSIONS)
 
     # On error in any of the steps an error will be thrown and the cli would
     # exit. That means if the call returns, the step is complete and we can
     # proceed with the next step.
@@ -343,14 +345,24 @@
         database_id)
 
     status = instance_response.status
     database_instance = None
 
     if status == DatabaseGetStatus.EXISTS:
       database_instance = instance_response.database_instance
+      if args.location != database_instance.location:
+        self.user_output.error(
+            LOCATION_MISMATCH_ERROR_MSG.format(
+                full_database_name=database_instance.name,
+                existing_location=database_instance.location,
+                requested_location=args.location,
+                database_id=database_id))
+
+        raise SilentlyExitError
+
     elif status == DatabaseGetStatus.DOES_NOT_EXIST:
       create_response = self.firebase_management_service.rtdb_instance_create(
           database_id=database_id, location=args.location)
 
       if create_response.status != DatabaseCreateStatus.SUCCESS:
         self.handle_database_create_failed(database_id, create_response)
       else:
```

### Comparing `snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/list_debuggees_command.py` & `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/list_debuggees_command.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/list_logpoints_command.py` & `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/list_logpoints_command.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/list_snapshots_command.py` & `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/list_snapshots_command.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/permissions_rest_service.py` & `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/permissions_rest_service.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/set_logpoint_command.py` & `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/set_logpoint_command.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/set_snapshot_command.py` & `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/set_snapshot_command.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/snapshot_debugger_rtdb_service.py` & `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/snapshot_debugger_rtdb_service.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/snapshot_debugger_schema.py` & `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/snapshot_debugger_schema.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/snapshot_parser.py` & `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/snapshot_parser.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/status_message.py` & `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/status_message.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/time_utils.py` & `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/time_utils.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/user_input.py` & `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/user_input.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.4/snapshot_dbg_cli/user_output.py` & `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/user_output.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.4/snapshot_dbg_cli.egg-info/PKG-INFO` & `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snapshot-dbg-cli
-Version: 0.3.4
+Version: 0.3.5
 Summary: 'Snapshot Debugger CLI tool.'
 Home-page: https://github.com/GoogleCloudPlatform/snapshot-debugger
 Author: Google Inc.
 License: Apache License, Version 2.0
 Project-URL: CLI Source, https://github.com/GoogleCloudPlatform/snapshot-debugger
 Project-URL: Java Agent Source, https://github.com/GoogleCloudPlatform/cloud-debug-java
 Project-URL: Node.js Agent Source, https://github.com/googleapis/cloud-debug-nodejs
@@ -270,14 +270,50 @@
   state:        ACTIVE
 ```
 
 Note: The information printed by the `init` command can be accessed from within
 your Firebase project. It’s safe to run the `snapshot-dbg-cli init
 --use-default-rtdb` command multiple times to view this information.
 
+#### Setting up Firebase RTDB in other regions
+
+By default, `snapshot-dbg-cli init` will create a Firebase Realtime Database in
+`us-central1`.  It is possible to create and use a database in any region
+supported by Firebase Realtime Database.  See
+[supported RTDB locations][rtdb_locations].
+
+Setting up your database in a non-default region comes with some trade-offs:
+*  As a positive, you get to control where your snapshot data will be stored.
+   This may be important for compliance reasons.
+*  As a negative, the vsCode extension and agents will be unable to
+   automatically find the database.  The database URL will need to be provided
+   explicitly via configuration, see the following for details:
+   * [Configuring the Java Agent][java_agent_config]
+   * [Configuring the Python Agent][python_agent_config]
+   * [Configuring the Node.js Agent][nodejs_agent_config]
+   * [Configuring the VsCode Extension][extension_config]
+
+You can set up your database in a non-default location as follows:
+```
+snapshot-dbg-cli init --location={YOUR_LOCATION}
+```
+
+For example, you may want to set up your database in Belgium, and so would run
+```snapshot-dbg-cli init --location=europe-west1```
+
+Make note of the database URL provided in the command output; you will need to
+provide this to your debug agent(s) and the vsCode plugin.
+
+[rtdb_locations]: https://firebase.google.com/docs/projects/locations#rtdb-locations
+[java_agent_config]: https://github.com/GoogleCloudPlatform/cloud-debug-java#snapshot-debugger---firebase-realtime-database-backend
+[python_agent_config]: https://github.com/GoogleCloudPlatform/cloud-debug-python/blob/main/README.md#snapshot-debugger---firebase-realtime-database-backend
+[nodejs_agent_config]: https://github.com/googleapis/cloud-debug-nodejs/blob/main/README.md#snapshot-debugger---firebase-realtime-database-backend
+[extension_config]: https://github.com/GoogleCloudPlatform/snapshot-debugger/blob/main/snapshot_dbg_extension/README.md#configuration
+
+
 ## Set up Snapshot Debugger in your Google Cloud project
 
 ### Working Samples
 
 Working examples of using the Snapshot Debugger with Java, Python and Node.js
 applications across different Google Cloud environments can be found in:
 
@@ -695,14 +731,31 @@
 
 
 Do you want to continue (Y/n)?
 Deleted 4 snapshots.
 ```
 
 
+## VSCode Extension
+
+There is a VSCode extension for the Snapshot Debugger.  You can use this
+extension to set logpoints, set breakpoints and view snapshots in the comfort
+of your IDE.  See the [extension's README][extension-readme] for more details.
+
+You can install the extension by downloading it from the
+[most recent release][extension-release], and then running
+`code --install-extension snapshotdbg-*.vsix`.
+
+Note that you will still need to use the Snapshot Debugger CLI to set up your
+environment and to purge old data.  Gcloud needs to be installed for credential
+management.
+
+[extension-release]: https://github.com/GoogleCloudPlatform/snapshot-debugger/releases
+[extension-readme]: https://github.com/GoogleCloudPlatform/snapshot-debugger/blob/main/snapshot_dbg_extension/README.md
+
 ## Troubleshooting
 
 See [Snapshot Debugger Troubleshooting][troubleshooting]
 
 [troubleshooting]: https://github.com/GoogleCloudPlatform/snapshot-debugger/blob/main/docs/troubleshooting.md
 
 ## Firebase DB Schema
```

### Comparing `snapshot-dbg-cli-0.3.4/snapshot_dbg_cli.egg-info/SOURCES.txt` & `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

