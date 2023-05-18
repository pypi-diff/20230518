# Comparing `tmp/slim-compose-1.0.2.tar.gz` & `tmp/slim-compose-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slim-compose-1.0.2.tar", last modified: Thu Apr 20 06:57:56 2023, max compression
+gzip compressed data, was "slim-compose-1.0.3.tar", last modified: Thu May 18 07:23:02 2023, max compression
```

## Comparing `slim-compose-1.0.2.tar` & `slim-compose-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 foobar    (1000) foobar    (1000)        0 2023-04-20 06:57:56.092924 slim-compose-1.0.2/
--rw-r--r--   0 foobar    (1000) foobar    (1000)     1056 2023-04-20 02:33:29.000000 slim-compose-1.0.2/LICENSE
--rw-r--r--   0 foobar    (1000) foobar    (1000)     2183 2023-04-20 06:57:56.092924 slim-compose-1.0.2/PKG-INFO
--rw-r--r--   0 foobar    (1000) foobar    (1000)      472 2023-04-20 06:49:18.000000 slim-compose-1.0.2/README.md
--rw-r--r--   0 foobar    (1000) foobar    (1000)      553 2023-04-20 06:56:39.000000 slim-compose-1.0.2/pyproject.toml
--rw-r--r--   0 foobar    (1000) foobar    (1000)       38 2023-04-20 06:57:56.092924 slim-compose-1.0.2/setup.cfg
-drwxr-xr-x   0 foobar    (1000) foobar    (1000)        0 2023-04-20 06:57:56.092924 slim-compose-1.0.2/src/
-drwxr-xr-x   0 foobar    (1000) foobar    (1000)        0 2023-04-20 06:57:56.092924 slim-compose-1.0.2/src/slim_compose.egg-info/
--rw-r--r--   0 foobar    (1000) foobar    (1000)     2183 2023-04-20 06:57:56.000000 slim-compose-1.0.2/src/slim_compose.egg-info/PKG-INFO
--rw-r--r--   0 foobar    (1000) foobar    (1000)      255 2023-04-20 06:57:56.000000 slim-compose-1.0.2/src/slim_compose.egg-info/SOURCES.txt
--rw-r--r--   0 foobar    (1000) foobar    (1000)        1 2023-04-20 06:57:56.000000 slim-compose-1.0.2/src/slim_compose.egg-info/dependency_links.txt
--rw-r--r--   0 foobar    (1000) foobar    (1000)       51 2023-04-20 06:57:56.000000 slim-compose-1.0.2/src/slim_compose.egg-info/entry_points.txt
--rw-r--r--   0 foobar    (1000) foobar    (1000)       13 2023-04-20 06:57:56.000000 slim-compose-1.0.2/src/slim_compose.egg-info/top_level.txt
--rwxr-xr-x   0 foobar    (1000) foobar    (1000)    13171 2023-04-20 06:56:29.000000 slim-compose-1.0.2/src/slim_compose.py
+drwxr-xr-x   0 foobar    (1000) foobar    (1000)        0 2023-05-18 07:23:02.432215 slim-compose-1.0.3/
+-rw-r--r--   0 foobar    (1000) foobar    (1000)     1056 2023-04-20 02:33:29.000000 slim-compose-1.0.3/LICENSE
+-rw-r--r--   0 foobar    (1000) foobar    (1000)     2183 2023-05-18 07:23:02.432215 slim-compose-1.0.3/PKG-INFO
+-rw-r--r--   0 foobar    (1000) foobar    (1000)      472 2023-04-20 06:49:18.000000 slim-compose-1.0.3/README.md
+-rw-r--r--   0 foobar    (1000) foobar    (1000)      553 2023-05-18 06:40:27.000000 slim-compose-1.0.3/pyproject.toml
+-rw-r--r--   0 foobar    (1000) foobar    (1000)       38 2023-05-18 07:23:02.432215 slim-compose-1.0.3/setup.cfg
+drwxr-xr-x   0 foobar    (1000) foobar    (1000)        0 2023-05-18 07:23:02.432215 slim-compose-1.0.3/src/
+drwxr-xr-x   0 foobar    (1000) foobar    (1000)        0 2023-05-18 07:23:02.432215 slim-compose-1.0.3/src/slim_compose.egg-info/
+-rw-r--r--   0 foobar    (1000) foobar    (1000)     2183 2023-05-18 07:23:02.000000 slim-compose-1.0.3/src/slim_compose.egg-info/PKG-INFO
+-rw-r--r--   0 foobar    (1000) foobar    (1000)      255 2023-05-18 07:23:02.000000 slim-compose-1.0.3/src/slim_compose.egg-info/SOURCES.txt
+-rw-r--r--   0 foobar    (1000) foobar    (1000)        1 2023-05-18 07:23:02.000000 slim-compose-1.0.3/src/slim_compose.egg-info/dependency_links.txt
+-rw-r--r--   0 foobar    (1000) foobar    (1000)       51 2023-05-18 07:23:02.000000 slim-compose-1.0.3/src/slim_compose.egg-info/entry_points.txt
+-rw-r--r--   0 foobar    (1000) foobar    (1000)       13 2023-05-18 07:23:02.000000 slim-compose-1.0.3/src/slim_compose.egg-info/top_level.txt
+-rwxr-xr-x   0 foobar    (1000) foobar    (1000)    13450 2023-05-18 06:50:44.000000 slim-compose-1.0.3/src/slim_compose.py
```

### Comparing `slim-compose-1.0.2/LICENSE` & `slim-compose-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `slim-compose-1.0.2/PKG-INFO` & `slim-compose-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slim-compose
-Version: 1.0.2
+Version: 1.0.3
 Summary: Simple management tool for podman pods
 Author: xfoobar
 License: MIT License
         
         Copyright (c) 2023
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `slim-compose-1.0.2/pyproject.toml` & `slim-compose-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "slim-compose"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="xfoobar"},
 ]
 description = "Simple management tool for podman pods"
 keywords = ["podman", "compose"]
 readme = "README.md"
 license = { file="LICENSE" }
```

### Comparing `slim-compose-1.0.2/src/slim_compose.egg-info/PKG-INFO` & `slim-compose-1.0.3/src/slim_compose.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slim-compose
-Version: 1.0.2
+Version: 1.0.3
 Summary: Simple management tool for podman pods
 Author: xfoobar
 License: MIT License
         
         Copyright (c) 2023
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `slim-compose-1.0.2/src/slim_compose.py` & `slim-compose-1.0.3/src/slim_compose.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import sys
 from pathlib import Path
 import os
 import subprocess
 import json
 import argparse
 
-APP_VERSION = '1.0.2'
+APP_VERSION = '1.0.3'
 
 ENCODING = 'utf-8'
 
 
 def nvl(*args):
     """
     return first non-null value
@@ -70,16 +70,15 @@
 
 def create_labels() -> list[str]:
     """
     create labels
     :return: list of labels
     """
     cwd = os.getcwd()
-    labels = [f'location={cwd}', 'creator=slim-compose',
-              f'version={APP_VERSION}']
+    labels = [f'location={cwd}', 'creator=slim-compose']
     args = []
     for label in labels:
         args.extend(['--label', label])
     return args
 
 
 def list_relevant_entity(entity_type: str) -> list[str]:
@@ -267,17 +266,14 @@
     """
     config_file = get_config_file()
     with open(config_file) as jf:
         config_data = json.load(jf)
     # load Pod
     pod_config = config_data['pod']
     pod = Pod(name=pod_config['name'])
-    # set default network
-    if not pod.networks:
-        pod.networks = [f'{pod.name}-default']
     load_optional_args(config=pod_config, entity=pod)
     # load Containers
     container_config = config_data['pod']['containers']
     for ctr_config in container_config:
         container = Container(
             name=f"{pod.name}-{ctr_config['name']}",
             image=ctr_config['image'],
@@ -302,22 +298,25 @@
     cmd = ['podman', entity_type, 'exists', name]
     if dry:
         return False
     r, _, _ = exec_cmd(cmd=cmd)
     return True if r == 0 else False
 
 
-def create(pod: Pod, dry: bool):
+def create(pod: Pod, dry: bool, disable_default_network:bool):
     """
     create pod
     :param pod:
     :param dry:
     :return:
     """
     labels = create_labels()
+    # set default network
+    if not pod.networks and not disable_default_network:
+        pod.networks = [f'{pod.name}-default']
     # create network
     for net in nvl(pod.networks, []):
         if not exists('network', net, dry=dry):
             cmd = ['podman', 'network', 'create']
             cmd.extend(labels)
             cmd.append(net)
             exec_cmd(cmd=cmd, ignore_error=False, dry=dry)
@@ -436,30 +435,33 @@
     parser.add_argument('action', choices=[
         'start', 'stop',
         'up', 'down', 'down-all',
         'restart', 'template'
     ], help='Action')
     parser.add_argument('--dry', action='store_true',
                         help='dry run', required=False)
+    parser.add_argument('--disable-default-network', action='store_true',
+                        help='do not create default network', required=False)
     parser.add_argument('--version', action='version',
                         version=f'%(prog)s {APP_VERSION}')
     args = parser.parse_args()
     return args
 
 
 def main():
     """
     main
     :return:
     """
     args = init_args()
     dry = args.dry
+    disable_default_network=args.disable_default_network
     if args.action == 'up':
         pod = load_pod_from_config()
-        create(pod=pod, dry=dry)
+        create(pod=pod, dry=dry,disable_default_network=disable_default_network)
     if args.action == 'down':
         destroy(all=False, dry=dry)
     if args.action == 'down-all':
         destroy(all=True, dry=dry)
     if args.action in ['start', 'stop', 'restart']:
         pod_operate(op=args.action, dry=dry)
     if args.action == 'template':
```

