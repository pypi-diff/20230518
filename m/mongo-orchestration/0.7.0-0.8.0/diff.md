# Comparing `tmp/mongo-orchestration-0.7.0.tar.gz` & `tmp/mongo-orchestration-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mongo-orchestration-0.7.0.tar", last modified: Tue Apr  6 22:04:05 2021, max compression
+gzip compressed data, was "mongo-orchestration-0.8.0.tar", last modified: Thu May 18 15:37:22 2023, max compression
```

## Comparing `mongo-orchestration-0.7.0.tar` & `mongo-orchestration-0.8.0.tar`

### file list

```diff
@@ -1,60 +1,74 @@
-drwxr-xr-x   0 shane      (502) staff       (20)        0 2021-04-06 22:04:05.375729 mongo-orchestration-0.7.0/
--rw-r--r--   0 shane      (502) staff       (20)    11789 2021-04-06 22:04:05.375897 mongo-orchestration-0.7.0/PKG-INFO
--rw-r--r--   0 shane      (502) staff       (20)     8450 2021-04-06 22:01:22.000000 mongo-orchestration-0.7.0/README.rst
-drwxr-xr-x   0 shane      (502) staff       (20)        0 2021-04-06 22:04:05.362006 mongo-orchestration-0.7.0/mongo_orchestration/
--rw-r--r--   0 shane      (502) staff       (20)     1244 2021-04-06 22:01:22.000000 mongo-orchestration-0.7.0/mongo_orchestration/__init__.py
-drwxr-xr-x   0 shane      (502) staff       (20)        0 2021-04-06 22:04:05.368765 mongo-orchestration-0.7.0/mongo_orchestration/apps/
--rw-r--r--   0 shane      (502) staff       (20)     2453 2018-08-08 18:38:15.000000 mongo-orchestration-0.7.0/mongo_orchestration/apps/__init__.py
--rw-r--r--   0 shane      (502) staff       (20)     8008 2018-08-08 18:38:15.000000 mongo-orchestration-0.7.0/mongo_orchestration/apps/links.py
--rw-r--r--   0 shane      (502) staff       (20)    12736 2018-08-08 18:38:15.000000 mongo-orchestration-0.7.0/mongo_orchestration/apps/replica_sets.py
--rw-r--r--   0 shane      (502) staff       (20)     5916 2018-08-08 18:38:15.000000 mongo-orchestration-0.7.0/mongo_orchestration/apps/servers.py
--rw-r--r--   0 shane      (502) staff       (20)    12828 2018-08-08 18:38:15.000000 mongo-orchestration-0.7.0/mongo_orchestration/apps/sharded_clusters.py
--rw-r--r--   0 shane      (502) staff       (20)     6954 2020-03-27 16:44:19.000000 mongo-orchestration-0.7.0/mongo_orchestration/common.py
--rw-r--r--   0 shane      (502) staff       (20)      829 2018-08-08 18:38:15.000000 mongo-orchestration-0.7.0/mongo_orchestration/compat.py
-drwxr-xr-x   0 shane      (502) staff       (20)        0 2021-04-06 22:04:05.357758 mongo-orchestration-0.7.0/mongo_orchestration/configurations/
-drwxr-xr-x   0 shane      (502) staff       (20)        0 2021-04-06 22:04:05.371500 mongo-orchestration-0.7.0/mongo_orchestration/configurations/replica_sets/
--rw-r--r--   0 shane      (502) staff       (20)     1173 2018-08-08 18:38:15.000000 mongo-orchestration-0.7.0/mongo_orchestration/configurations/replica_sets/allengines.json
--rw-r--r--   0 shane      (502) staff       (20)      854 2018-08-09 20:38:13.000000 mongo-orchestration-0.7.0/mongo_orchestration/configurations/replica_sets/arbiter.json
--rw-r--r--   0 shane      (502) staff       (20)     1335 2018-08-09 20:38:13.000000 mongo-orchestration-0.7.0/mongo_orchestration/configurations/replica_sets/auth.json
--rw-r--r--   0 shane      (502) staff       (20)      855 2018-08-09 20:38:13.000000 mongo-orchestration-0.7.0/mongo_orchestration/configurations/replica_sets/basic.json
--rw-r--r--   0 shane      (502) staff       (20)     1260 2018-08-09 20:38:13.000000 mongo-orchestration-0.7.0/mongo_orchestration/configurations/replica_sets/clean.json
--rw-r--r--   0 shane      (502) staff       (20)     1283 2018-08-08 18:38:15.000000 mongo-orchestration-0.7.0/mongo_orchestration/configurations/replica_sets/mmapv1.json
--rw-r--r--   0 shane      (502) staff       (20)     1461 2018-08-09 20:38:13.000000 mongo-orchestration-0.7.0/mongo_orchestration/configurations/replica_sets/ssl.json
--rw-r--r--   0 shane      (502) staff       (20)     1536 2018-08-09 20:38:13.000000 mongo-orchestration-0.7.0/mongo_orchestration/configurations/replica_sets/ssl_auth.json
--rw-r--r--   0 shane      (502) staff       (20)      992 2018-08-08 18:38:15.000000 mongo-orchestration-0.7.0/mongo_orchestration/configurations/replica_sets/wiredtiger.json
-drwxr-xr-x   0 shane      (502) staff       (20)        0 2021-04-06 22:04:05.373232 mongo-orchestration-0.7.0/mongo_orchestration/configurations/servers/
--rw-r--r--   0 shane      (502) staff       (20)      323 2018-08-08 18:38:15.000000 mongo-orchestration-0.7.0/mongo_orchestration/configurations/servers/auth.json
--rw-r--r--   0 shane      (502) staff       (20)      125 2018-08-08 18:38:15.000000 mongo-orchestration-0.7.0/mongo_orchestration/configurations/servers/basic.json
--rw-r--r--   0 shane      (502) staff       (20)      248 2018-08-08 18:38:15.000000 mongo-orchestration-0.7.0/mongo_orchestration/configurations/servers/clean.json
--rw-r--r--   0 shane      (502) staff       (20)      160 2018-08-08 18:38:15.000000 mongo-orchestration-0.7.0/mongo_orchestration/configurations/servers/mmapv1.json
--rw-r--r--   0 shane      (502) staff       (20)      449 2018-08-08 18:38:15.000000 mongo-orchestration-0.7.0/mongo_orchestration/configurations/servers/ssl.json
--rw-r--r--   0 shane      (502) staff       (20)      524 2018-08-08 18:38:15.000000 mongo-orchestration-0.7.0/mongo_orchestration/configurations/servers/ssl_auth.json
--rw-r--r--   0 shane      (502) staff       (20)      164 2018-08-08 18:38:15.000000 mongo-orchestration-0.7.0/mongo_orchestration/configurations/servers/wiredtiger.json
-drwxr-xr-x   0 shane      (502) staff       (20)        0 2021-04-06 22:04:05.375329 mongo-orchestration-0.7.0/mongo_orchestration/configurations/sharded_clusters/
--rw-r--r--   0 shane      (502) staff       (20)     1073 2018-08-08 18:38:15.000000 mongo-orchestration-0.7.0/mongo_orchestration/configurations/sharded_clusters/auth.json
--rw-r--r--   0 shane      (502) staff       (20)      124 2018-08-08 18:38:15.000000 mongo-orchestration-0.7.0/mongo_orchestration/configurations/sharded_clusters/basic.json
--rw-r--r--   0 shane      (502) staff       (20)      998 2018-08-08 18:38:15.000000 mongo-orchestration-0.7.0/mongo_orchestration/configurations/sharded_clusters/clean.json
--rw-r--r--   0 shane      (502) staff       (20)      284 2018-08-08 18:38:15.000000 mongo-orchestration-0.7.0/mongo_orchestration/configurations/sharded_clusters/mmapv1.json
--rw-r--r--   0 shane      (502) staff       (20)     1199 2018-08-08 18:38:15.000000 mongo-orchestration-0.7.0/mongo_orchestration/configurations/sharded_clusters/ssl.json
--rw-r--r--   0 shane      (502) staff       (20)     1273 2018-08-08 18:38:15.000000 mongo-orchestration-0.7.0/mongo_orchestration/configurations/sharded_clusters/ssl_auth.json
--rw-r--r--   0 shane      (502) staff       (20)      288 2018-08-08 18:38:15.000000 mongo-orchestration-0.7.0/mongo_orchestration/configurations/sharded_clusters/wiredtiger.json
--rw-r--r--   0 shane      (502) staff       (20)     3023 2018-08-08 18:38:15.000000 mongo-orchestration-0.7.0/mongo_orchestration/container.py
--rw-r--r--   0 shane      (502) staff       (20)     6407 2020-02-26 17:54:48.000000 mongo-orchestration-0.7.0/mongo_orchestration/daemon.py
--rw-r--r--   0 shane      (502) staff       (20)     1477 2018-08-08 18:38:15.000000 mongo-orchestration-0.7.0/mongo_orchestration/errors.py
-drwxr-xr-x   0 shane      (502) staff       (20)        0 2021-04-06 22:04:05.375550 mongo-orchestration-0.7.0/mongo_orchestration/lib/
--rw-r--r--   0 shane      (502) staff       (20)     3022 2018-08-08 18:38:15.000000 mongo-orchestration-0.7.0/mongo_orchestration/lib/client.pem
--rw-r--r--   0 shane      (502) staff       (20)    12720 2020-03-24 22:00:09.000000 mongo-orchestration-0.7.0/mongo_orchestration/process.py
--rw-r--r--   0 shane      (502) staff       (20)    30696 2021-02-26 23:42:24.000000 mongo-orchestration-0.7.0/mongo_orchestration/replica_sets.py
--rw-r--r--   0 shane      (502) staff       (20)     6955 2020-03-24 22:00:09.000000 mongo-orchestration-0.7.0/mongo_orchestration/server.py
--rw-r--r--   0 shane      (502) staff       (20)    22501 2020-04-29 17:19:38.000000 mongo-orchestration-0.7.0/mongo_orchestration/servers.py
--rw-r--r--   0 shane      (502) staff       (20)    22948 2020-03-26 21:25:08.000000 mongo-orchestration-0.7.0/mongo_orchestration/sharded_clusters.py
--rw-r--r--   0 shane      (502) staff       (20)      884 2018-08-08 18:38:15.000000 mongo-orchestration-0.7.0/mongo_orchestration/singleton.py
-drwxr-xr-x   0 shane      (502) staff       (20)        0 2021-04-06 22:04:05.367270 mongo-orchestration-0.7.0/mongo_orchestration.egg-info/
--rw-r--r--   0 shane      (502) staff       (20)    11789 2021-04-06 22:04:05.000000 mongo-orchestration-0.7.0/mongo_orchestration.egg-info/PKG-INFO
--rw-r--r--   0 shane      (502) staff       (20)     2278 2021-04-06 22:04:05.000000 mongo-orchestration-0.7.0/mongo_orchestration.egg-info/SOURCES.txt
--rw-r--r--   0 shane      (502) staff       (20)        1 2021-04-06 22:04:05.000000 mongo-orchestration-0.7.0/mongo_orchestration.egg-info/dependency_links.txt
--rw-r--r--   0 shane      (502) staff       (20)       73 2021-04-06 22:04:05.000000 mongo-orchestration-0.7.0/mongo_orchestration.egg-info/entry_points.txt
--rw-r--r--   0 shane      (502) staff       (20)      102 2021-04-06 22:04:05.000000 mongo-orchestration-0.7.0/mongo_orchestration.egg-info/requires.txt
--rw-r--r--   0 shane      (502) staff       (20)       20 2021-04-06 22:04:05.000000 mongo-orchestration-0.7.0/mongo_orchestration.egg-info/top_level.txt
--rw-r--r--   0 shane      (502) staff       (20)       67 2021-04-06 22:04:05.376259 mongo-orchestration-0.7.0/setup.cfg
--rw-r--r--   0 shane      (502) staff       (20)     5014 2021-04-06 22:01:22.000000 mongo-orchestration-0.7.0/setup.py
+drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-05-18 15:37:22.012114 mongo-orchestration-0.8.0/
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)    11358 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/LICENSE
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)    10110 2023-05-18 15:37:22.012204 mongo-orchestration-0.8.0/PKG-INFO
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     9014 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/README.rst
+drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-05-18 15:37:22.004373 mongo-orchestration-0.8.0/mongo_orchestration/
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     1274 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/__init__.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)       21 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/_version.py
+drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-05-18 15:37:22.006180 mongo-orchestration-0.8.0/mongo_orchestration/apps/
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     2453 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/apps/__init__.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     8008 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/apps/links.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)    12736 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/apps/replica_sets.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     5916 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/apps/servers.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)    12828 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/apps/sharded_clusters.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     6794 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/common.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      829 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/compat.py
+drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-05-18 15:37:21.997847 mongo-orchestration-0.8.0/mongo_orchestration/configurations/
+drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-05-18 15:37:22.007614 mongo-orchestration-0.8.0/mongo_orchestration/configurations/replica_sets/
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     1173 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/configurations/replica_sets/allengines.json
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      854 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/configurations/replica_sets/arbiter.json
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     1335 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/configurations/replica_sets/auth.json
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      855 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/configurations/replica_sets/basic.json
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     1260 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/configurations/replica_sets/clean.json
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     1283 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/configurations/replica_sets/mmapv1.json
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     1461 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/configurations/replica_sets/ssl.json
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     1536 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/configurations/replica_sets/ssl_auth.json
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      992 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/configurations/replica_sets/wiredtiger.json
+drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-05-18 15:37:22.008740 mongo-orchestration-0.8.0/mongo_orchestration/configurations/servers/
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      323 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/configurations/servers/auth.json
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      125 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/configurations/servers/basic.json
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      248 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/configurations/servers/clean.json
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      160 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/configurations/servers/mmapv1.json
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      449 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/configurations/servers/ssl.json
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      524 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/configurations/servers/ssl_auth.json
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      164 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/configurations/servers/wiredtiger.json
+drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-05-18 15:37:22.009962 mongo-orchestration-0.8.0/mongo_orchestration/configurations/sharded_clusters/
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     1073 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/configurations/sharded_clusters/auth.json
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      124 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/configurations/sharded_clusters/basic.json
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      998 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/configurations/sharded_clusters/clean.json
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      284 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/configurations/sharded_clusters/mmapv1.json
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     1199 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/configurations/sharded_clusters/ssl.json
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     1273 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/configurations/sharded_clusters/ssl_auth.json
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      288 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/configurations/sharded_clusters/wiredtiger.json
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     3023 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/container.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     6407 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/daemon.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     1477 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/errors.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)    10773 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/launch.py
+drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-05-18 15:37:22.010475 mongo-orchestration-0.8.0/mongo_orchestration/lib/
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     1272 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/lib/ca.pem
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     2955 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/lib/client.pem
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     3024 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/lib/server.pem
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)    12415 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/process.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)    30677 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/replica_sets.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     6962 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/server.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)    22579 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/servers.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)    24617 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/sharded_clusters.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      884 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/mongo_orchestration/singleton.py
+drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-05-18 15:37:22.005375 mongo-orchestration-0.8.0/mongo_orchestration.egg-info/
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)    10110 2023-05-18 15:37:21.000000 mongo-orchestration-0.8.0/mongo_orchestration.egg-info/PKG-INFO
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     2611 2023-05-18 15:37:21.000000 mongo-orchestration-0.8.0/mongo_orchestration.egg-info/SOURCES.txt
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)        1 2023-05-18 15:37:21.000000 mongo-orchestration-0.8.0/mongo_orchestration.egg-info/dependency_links.txt
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      119 2023-05-18 15:37:21.000000 mongo-orchestration-0.8.0/mongo_orchestration.egg-info/entry_points.txt
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)       89 2023-05-18 15:37:21.000000 mongo-orchestration-0.8.0/mongo_orchestration.egg-info/requires.txt
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)       20 2023-05-18 15:37:21.000000 mongo-orchestration-0.8.0/mongo_orchestration.egg-info/top_level.txt
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)      182 2023-05-18 15:37:22.012523 mongo-orchestration-0.8.0/setup.cfg
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     2369 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/setup.py
+drwxr-xr-x   0 steve.silvester   (502) wheel        (0)        0 2023-05-18 15:37:22.011943 mongo-orchestration-0.8.0/tests/
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     4634 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/tests/test_container.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     2101 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/tests/test_launch.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)    11582 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/tests/test_process.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)    22611 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/tests/test_replica_set.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)    16922 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/tests/test_replica_sets.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)    22877 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/tests/test_servers.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)    28683 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/tests/test_sharded_clusters.py
+-rw-r--r--   0 steve.silvester   (502) wheel        (0)     1006 2023-05-18 15:36:37.000000 mongo-orchestration-0.8.0/tests/test_singleton.py
```

### Comparing `mongo-orchestration-0.7.0/PKG-INFO` & `mongo-orchestration-0.8.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,280 +1,302 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: mongo-orchestration
-Version: 0.7.0
+Version: 0.8.0
 Summary: Restful service for managing MongoDB servers
 Home-page: https://github.com/10gen/mongo-orchestration
 Author: MongoDB, Inc.
 Author-email: mongodb-user@googlegroups.com
 License: http://www.apache.org/licenses/LICENSE-2.0.html
-Description: -------------------
-        Mongo Orchestration
-        -------------------
-        
-        See the `wiki <https://github.com/10gen/mongo-orchestration/wiki>`__
-        for documentation.
-        
-        Mongo Orchestration is an HTTP server that provides a REST API for
-        creating and managing MongoDB configurations on a single host.
-        
-        **THIS PROJECT IS FOR TESTING OF MONGODB DRIVERS.**
-        
-        Features
-        --------
-        
-        -  Start and stop mongod servers, replica sets, and sharded clusters on the host running mongo-orchestration.
-        -  Add and remove replica set members.
-        -  Add and remove shards and mongos routers.
-        -  Reset replica sets and clusters to restart all members that were
-           stopped.
-        -  Freeze secondary members of replica sets.
-        -  Retrieve information about MongoDB resources.
-        -  Interaction all through REST interface.
-        
-        Requires
-        --------
-        
-        -  `Python 2.6, 2.7, or >= 3.2 <http://www.python.org/download/>`__
-        -  `bottle>=0.12.7 <https://pypi.python.org/pypi/bottle>`__
-        -  `pymongo>=3.0.2,<4 <https://pypi.python.org/pypi/pymongo>`__
-        -  `CherryPy>=3.5.0,<9.0.0 <http://www.cherrypy.org/>`__
-        -  `argparse>=1.2.1 <https://pypi.python.org/pypi/argparse>`__ (Python 2.6 only)
-        -  `simplejson <https://pypi.python.org/pypi/simplejson>`__ (Python 2.6 only)
-        
-        Installation
-        ------------
-        
-        The easiest way to install Mongo Orchestration is with `pip <https://pypi.python.org/pypi/pip>`__:
-        
-        ::
-        
-            pip install mongo-orchestration
-        
-        You can also install the development version of Mongo Orchestration
-        manually:
-        
-        ::
-        
-            git clone https://github.com/10gen/mongo-orchestration.git
-            cd mongo-orchestration
-            pip install .
-        
-        Cloning the `repository <https://github.com/10gen/mongo-orchestration>`__ this way will also give you access to the tests for Mongo Orchestration as well as the ``mo`` script. Note that you may
-        have to run the above commands with ``sudo``, depending on where you're
-        installing Mongo Orchestration and what privileges you have.
-        Installation will place a ``mongo-orchestration`` script on your path.
-        
-        Usage
-        -----
-        
-        ::
-        
-            mongo-orchestration [-h] [-f CONFIG] [-e ENV] [--no-fork] [-b BIND IP="localhost"] [-p PORT]
-                                [-s {cherrypy,wsgiref}] [--socket-timeout-ms MILLIS]
-                                [--pidfile PIDFILE] [--enable-majority-read-concern] {start,stop,restart}
-        
-        
-        Arguments:
-        
-        -  **-h** - show help
-        -  **-f, --config** - path to config file
-        -  **-e, --env** - default release to use, as specified in the config
-           file
-        -  **--no-fork** - run server in foreground
-        -  **-b, --bind** - host on which Mongo Orchestration and subordinate mongo processes should listen for requests. Defaults to "localhost".
-        -  **-s, --server** - HTTP backend to use: one of `cherrypy` or `wsgiref`
-        -  **-p** - port number (8889 by default)
-        -  **--socket-timeout-ms** - socket timeout when connecting to MongoDB servers
-        -  **--pidfile** - location where mongo-orchestration should place its pid file
-        -  **--enable-majority-read-concern** - enable "majority" read concern on server versions that support it.
-        -  **start/stop/restart**: start, stop, or restart the server,
-           respectively
-        
-        In addition, Mongo Orchestration can be influenced by the
-        ``MONGO_ORCHESTRATION_HOME`` environment variable, which informs the
-        server where to find the "configurations" directory for presets as well
-        as where to put the log and pid files.
-        
-        Examples
-        ~~~~~~~~
-        
-        ``mongo-orchestration start``
-        
-        Starts Mongo Orchestration as service on port 8889.
-        
-        ``mongo-orchestration stop``
-        
-        Stop the server.
-        
-        ``mongo-orchestration -f mongo-orchestration.config -e 30-release -p 8888 --no-fork start``
-        
-        Starts Mongo Orchestration on port 8888 using ``30-release`` defined in
-        ``mongo-orchestration.config``. Stops with *Ctrl+C*.
-        
-        If you have installed mongo-orchestration but you're still getting
-        ``command not found: mongo-orchestration`` this means that the script was
-        installed to a directory that is not on your ``PATH``. As an alternative use:
-        
-        ``python -m mongo_orchestration.server start``
-        
-        Configuration File
-        ~~~~~~~~~~~~~~~~~~
-        
-        Mongo Orchestration may be given a JSON configuration file with the
-        ``--config`` option specifying where to find MongoDB binaries. See
-        `mongo-orchestration.config <https://github.com/10gen/mongo-orchestration/blob/master/mongo-orchestration.config>`__
-        for an example. When no configuration file is provided, Mongo
-        Orchestration uses whatever binaries are on the user's PATH.
-        
-        Predefined Configurations
-        -------------------------
-        
-        Mongo Orchestration has a set of predefined
-        `configurations <https://github.com/10gen/mongo-orchestration/tree/master/mongo_orchestration/configurations>`__
-        that can be used to start, restart, or stop MongoDB processes. You can
-        use a tool like ``curl`` to send these files directly to the Mongo
-        Orchestration server, or use the ``mo`` script in the ``scripts``
-        directory (in the `repository <https://github.com/10gen/mongo-orchestration>`__ only). Some examples:
-        
-        -  Start a single node without SSL or auth:
-        
-           ::
-        
-               mo configurations/servers/clean.json start
-        
-        -  Get the status of a single node without SSL or auth:
-        
-           ::
-        
-               mo configurations/servers/clean.json status
-        
-        -  Stop a single node without SSL or auth:
-        
-           ::
-        
-               mo configurations/servers/clean.json stop
-        
-        -  Start a replica set with ssl and auth:
-        
-           ::
-        
-               mo configurations/replica_sets/ssl_auth.json start
-        
-        -  Use ``curl`` to create a basic sharded cluster with the id
-           "myCluster":
-        
-           ::
-        
-               curl -XPUT http://localhost:8889/v1/sharded_clusters/myCluster \
-                          -d@configurations/sharded_clusters/basic.json
-        
-        Note that in order to run the ``mo`` script, you need to be in the same
-        directory as "configurations".
-        
-        **Helpful hint**: You can prettify JSON responses from the server by
-        piping the response into ``python -m json.tool``, e.g.:
-        
-        ::
-        
-            $ curl http://localhost:8889/v1/servers/myServer | python -m json.tool
-        
-            {
-                "id": "myServer",
-                "mongodb_uri": "mongodb://localhost:1025",
-                "orchestration": "servers",
-                "procInfo": {
-                    "alive": true,
-                    "name": "mongod",
-                    "optfile": "/var/folders/v9/spc2j6cx3db71l/T/mongo-KHUACD",
-                    "params": {
-                        "dbpath": "/var/folders/v9/spc2j6cx3db71l/T/mongo-vAgYaQ",
-                        "ipv6": true,
-                        "journal": true,
-                        "logappend": true,
-                        "oplogSize": 100,
-                        "port": 1025
-                    },
-                    "pid": 51320
-                },
-                // etc.
-            }
-        
-        Tests
-        -----
-        
-        In order to run the tests, you should first clone the `repository <https://github.com/10gen/mongo-orchestration>`__. Running the tests has the following additional dependency:
-        
-        -  `unittest2 >= 0.6 <https://pypi.python.org/pypi/unittest2>`__ (Python 2.6 only)
-        
-        Run all tests
-        ~~~~~~~~~~~~~
-        
-        ``python setup.py test``
-        
-        Run a test module
-        ~~~~~~~~~~~~~~~~~
-        
-        ``python -m unittest tests.test_servers``
-        
-        Run a single test case
-        ~~~~~~~~~~~~~~~~~~~~~~
-        
-        ``python -m unittest tests.test_servers.ServerSSLTestCase``
-        
-        Run a single test method
-        ~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        ``python -m unittest tests.test_servers.ServerSSLTestCase.test_ssl_auth``
-        
-        Run a single test example for debugging with verbose and immediate stdout output
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        ``python -m unittest -v tests.test_servers.ServerSSLTestCase``
-        
-        Changelog
-        ---------
-        
-        Changes in Version 0.7.0 (2021-04-06)
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        - Remove support for managing MongoDB 2.4 servers.
-        - Add support for Python 3.8 and 3.9.
-        - Add support for MongoDB 4.2 and 4.4.
-        - Upgrade from pymongo 3.5.1 to 3.X latest. (#284).
-        - Ensure createUser succeeds on all replica set members. (#282)
-        - Create admin user with both SCRAM-SHA-256 and SCRAM-SHA-1. (#281)
-        - Wait for mongo-orchestration server to fully terminate in "stop". (#276)
-        - Allow starting clusters with enableTestCommands=0. (#269)
-        - Decrease transactionLifetimeLimitSeconds on 4.2+ by default. (#267)
-        - Increase maxTransactionLockRequestTimeoutMillis by default. (#270)
-        - Reduce periodicNoopIntervalSecs for faster driver change stream testing. (#283)
-        - Enable ztsd compression by default on 4.2+ (#263)
-        
-        Changes in Version 0.6.12 (2018-12-14)
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        - Allow running the mongo-orchestration server over IPv6 localhost. (#237)
-        - Increase default mongodb server logging verbosity. (#255)
-        - Fixed a bug when shutting down clusters where mongo-orchestration would
-          hang forever if the server had already exited. (#253)
-        
 Keywords: mongo-orchestration,mongodb,mongo,rest,testing
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.2
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: >=3.6
+Provides-Extra: test
+License-File: LICENSE
+
+-------------------
+Mongo Orchestration
+-------------------
+
+See the `wiki <https://github.com/10gen/mongo-orchestration/wiki>`__
+for documentation.
+
+Mongo Orchestration is an HTTP server that provides a REST API for
+creating and managing MongoDB configurations on a single host.
+
+**THIS PROJECT IS FOR TESTING OF MONGODB DRIVERS.**
+
+Features
+--------
+
+-  Start and stop mongod servers, replica sets, and sharded clusters on the host running mongo-orchestration.
+-  Add and remove replica set members.
+-  Add and remove shards and mongos routers.
+-  Reset replica sets and clusters to restart all members that were
+   stopped.
+-  Freeze secondary members of replica sets.
+-  Retrieve information about MongoDB resources.
+-  Interaction all through REST interface.
+-  Launch simple local servers using ``mongo-launch`` CLI tool.
+
+Requires
+--------
+
+-  `Python >=3.7 <http://www.python.org/download/>`__
+-  `bottle>=0.12.7 <https://pypi.python.org/pypi/bottle>`__
+-  `pymongo>=3.0.2,<4 <https://pypi.python.org/pypi/pymongo>`__
+-  `cheroot>=5.11 <https://pypi.python.org/pypi/cheroot/>`__
+
+Installation
+------------
+
+The easiest way to install Mongo Orchestration is with `pip <https://pypi.python.org/pypi/pip>`__:
+
+::
+
+    pip install mongo-orchestration
+
+You can also install the development version of Mongo Orchestration
+manually:
+
+::
+
+    git clone https://github.com/10gen/mongo-orchestration.git
+    cd mongo-orchestration
+    pip install .
+
+Cloning the `repository <https://github.com/10gen/mongo-orchestration>`__ this way will also give you access to the tests for Mongo Orchestration as well as the ``mo`` script. Note that you may
+have to run the above commands with ``sudo``, depending on where you're
+installing Mongo Orchestration and what privileges you have.
+Installation will place a ``mongo-orchestration`` script on your path.
+
+Usage
+-----
+
+::
+
+    mongo-orchestration [-h] [-f CONFIG] [-e ENV] [--no-fork] [-b BIND IP="localhost"] [-p PORT]
+                        [-s {auto,cheroot,wsgiref}] [--socket-timeout-ms MILLIS]
+                        [--pidfile PIDFILE] [--enable-majority-read-concern] {start,stop,restart}
+
+
+Arguments:
+
+-  **-h** - show help
+-  **-f, --config** - path to config file
+-  **-e, --env** - default release to use, as specified in the config
+   file
+-  **--no-fork** - run server in foreground
+-  **-b, --bind** - host on which Mongo Orchestration and subordinate mongo processes should listen for requests. Defaults to "localhost".
+-  **-s, --server** - HTTP backend to use: one of `auto`, `cheroot`, or `wsgiref`. `auto`
+   configures bottle to automatically choose an available backend.
+-  **-p** - port number (8889 by default)
+-  **--socket-timeout-ms** - socket timeout when connecting to MongoDB servers
+-  **--pidfile** - location where mongo-orchestration should place its pid file
+-  **--enable-majority-read-concern** - enable "majority" read concern on server versions that support it.
+-  **start/stop/restart**: start, stop, or restart the server,
+   respectively
+
+In addition, Mongo Orchestration can be influenced by the
+``MONGO_ORCHESTRATION_HOME`` environment variable, which informs the
+server where to find the "configurations" directory for presets as well
+as where to put the log and pid files.
+
+Examples
+~~~~~~~~
+
+``mongo-orchestration start``
+
+Starts Mongo Orchestration as service on port 8889.
+
+``mongo-orchestration stop``
+
+Stop the server.
+
+``mongo-orchestration -f mongo-orchestration.config -e 30-release -p 8888 --no-fork start``
+
+Starts Mongo Orchestration on port 8888 using ``30-release`` defined in
+``mongo-orchestration.config``. Stops with *Ctrl+C*.
+
+If you have installed mongo-orchestration but you're still getting
+``command not found: mongo-orchestration`` this means that the script was
+installed to a directory that is not on your ``PATH``. As an alternative use:
+
+``python -m mongo_orchestration.server start``
+
+Configuration File
+~~~~~~~~~~~~~~~~~~
+
+Mongo Orchestration may be given a JSON configuration file with the
+``--config`` option specifying where to find MongoDB binaries. See
+`mongo-orchestration.config <https://github.com/10gen/mongo-orchestration/blob/master/mongo-orchestration.config>`__
+for an example. When no configuration file is provided, Mongo
+Orchestration uses whatever binaries are on the user's PATH.
+
+Predefined Configurations
+-------------------------
+
+Mongo Orchestration has a set of predefined
+`configurations <https://github.com/10gen/mongo-orchestration/tree/master/mongo_orchestration/configurations>`__
+that can be used to start, restart, or stop MongoDB processes. You can
+use a tool like ``curl`` to send these files directly to the Mongo
+Orchestration server, or use the ``mo`` script in the ``scripts``
+directory (in the `repository <https://github.com/10gen/mongo-orchestration>`__ only). Some examples:
+
+-  Start a single node without SSL or auth:
+
+   ::
+
+       mo configurations/servers/clean.json start
+
+-  Get the status of a single node without SSL or auth:
+
+   ::
+
+       mo configurations/servers/clean.json status
+
+-  Stop a single node without SSL or auth:
+
+   ::
+
+       mo configurations/servers/clean.json stop
+
+-  Start a replica set with ssl and auth:
+
+   ::
+
+       mo configurations/replica_sets/ssl_auth.json start
+
+-  Use ``curl`` to create a basic sharded cluster with the id
+   "myCluster":
+
+   ::
+
+       curl -XPUT http://localhost:8889/v1/sharded_clusters/myCluster \
+                  -d@configurations/sharded_clusters/basic.json
+
+Note that in order to run the ``mo`` script, you need to be in the same
+directory as "configurations".
+
+**Helpful hint**: You can prettify JSON responses from the server by
+piping the response into ``python -m json.tool``, e.g.:
+
+::
+
+    $ curl http://localhost:8889/v1/servers/myServer | python -m json.tool
+
+    {
+        "id": "myServer",
+        "mongodb_uri": "mongodb://localhost:1025",
+        "orchestration": "servers",
+        "procInfo": {
+            "alive": true,
+            "name": "mongod",
+            "optfile": "/var/folders/v9/spc2j6cx3db71l/T/mongo-KHUACD",
+            "params": {
+                "dbpath": "/var/folders/v9/spc2j6cx3db71l/T/mongo-vAgYaQ",
+                "ipv6": true,
+                "journal": true,
+                "logappend": true,
+                "oplogSize": 100,
+                "port": 1025
+            },
+            "pid": 51320
+        },
+        // etc.
+    }
+
+Mongo Launch
+------------
+
+The ``mongo-launch`` CLI tool allows you to spin up servers locally
+with minimal configuration.
+
+..
+
+    mongo-launch --help
+    Usage: launch.py [single|replica|shard] [ssl] [auth]
+
+..
+
+    mongo-orchestration start
+    mongo-launch replica ssl auth
+
+Tests
+-----
+
+In order to run the tests, you should first clone the `repository <https://github.com/10gen/mongo-orchestration>`__.
+
+Run all tests
+~~~~~~~~~~~~~
+
+``python -m unittest``
+
+Run a test module
+~~~~~~~~~~~~~~~~~
+
+``python -m unittest tests.test_servers``
+
+Run a single test case
+~~~~~~~~~~~~~~~~~~~~~~
+
+``python -m unittest tests.test_servers.ServerSSLTestCase``
+
+Run a single test method
+~~~~~~~~~~~~~~~~~~~~~~~~
+
+``python -m unittest tests.test_servers.ServerSSLTestCase.test_ssl_auth``
+
+Run a single test example for debugging with verbose and immediate stdout output
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+``python -m unittest -v tests.test_servers.ServerSSLTestCase``
+
+Changelog
+---------
+
+Changes in Version 0.8.0 (2023-05-16)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+- Add ``mongo-launch`` CLI tool.
+- Upgrade to PyMongo 4.x and set up GitHub Actions testing.
+- Remove support for managing MongoDB 3.4 or earlier servers.
+- Remove support for Python 3.5 or earlier.
+- Replaced dependency on CherryPy with cheroot. `-s auto` is the new default
+  and `-s cherrypy` is no longer supported.
+- Remove transactionLifetimeLimitSeconds default.
+
+Changes in Version 0.7.0 (2021-04-06)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+- Remove support for managing MongoDB 2.4 servers.
+- Add support for Python 3.8 and 3.9.
+- Add support for MongoDB 4.2 and 4.4.
+- Upgrade from pymongo 3.5.1 to 3.X latest. (#284).
+- Ensure createUser succeeds on all replica set members. (#282)
+- Create admin user with both SCRAM-SHA-256 and SCRAM-SHA-1. (#281)
+- Wait for mongo-orchestration server to fully terminate in "stop". (#276)
+- Allow starting clusters with enableTestCommands=0. (#269)
+- Decrease transactionLifetimeLimitSeconds on 4.2+ by default. (#267)
+- Increase maxTransactionLockRequestTimeoutMillis by default. (#270)
+- Reduce periodicNoopIntervalSecs for faster driver change stream testing. (#283)
+- Enable ztsd compression by default on 4.2+ (#263)
+
+Changes in Version 0.6.12 (2018-12-14)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+- Allow running the mongo-orchestration server over IPv6 localhost. (#237)
+- Increase default mongodb server logging verbosity. (#255)
+- Fixed a bug when shutting down clusters where mongo-orchestration would
+  hang forever if the server had already exited. (#253)
```

### Comparing `mongo-orchestration-0.7.0/README.rst` & `mongo-orchestration-0.8.0/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -17,24 +17,23 @@
 -  Add and remove replica set members.
 -  Add and remove shards and mongos routers.
 -  Reset replica sets and clusters to restart all members that were
    stopped.
 -  Freeze secondary members of replica sets.
 -  Retrieve information about MongoDB resources.
 -  Interaction all through REST interface.
+-  Launch simple local servers using ``mongo-launch`` CLI tool.
 
 Requires
 --------
 
--  `Python 2.6, 2.7, or >= 3.2 <http://www.python.org/download/>`__
+-  `Python >=3.7 <http://www.python.org/download/>`__
 -  `bottle>=0.12.7 <https://pypi.python.org/pypi/bottle>`__
 -  `pymongo>=3.0.2,<4 <https://pypi.python.org/pypi/pymongo>`__
--  `CherryPy>=3.5.0,<9.0.0 <http://www.cherrypy.org/>`__
--  `argparse>=1.2.1 <https://pypi.python.org/pypi/argparse>`__ (Python 2.6 only)
--  `simplejson <https://pypi.python.org/pypi/simplejson>`__ (Python 2.6 only)
+-  `cheroot>=5.11 <https://pypi.python.org/pypi/cheroot/>`__
 
 Installation
 ------------
 
 The easiest way to install Mongo Orchestration is with `pip <https://pypi.python.org/pypi/pip>`__:
 
 ::
@@ -57,27 +56,28 @@
 
 Usage
 -----
 
 ::
 
     mongo-orchestration [-h] [-f CONFIG] [-e ENV] [--no-fork] [-b BIND IP="localhost"] [-p PORT]
-                        [-s {cherrypy,wsgiref}] [--socket-timeout-ms MILLIS]
+                        [-s {auto,cheroot,wsgiref}] [--socket-timeout-ms MILLIS]
                         [--pidfile PIDFILE] [--enable-majority-read-concern] {start,stop,restart}
 
 
 Arguments:
 
 -  **-h** - show help
 -  **-f, --config** - path to config file
 -  **-e, --env** - default release to use, as specified in the config
    file
 -  **--no-fork** - run server in foreground
 -  **-b, --bind** - host on which Mongo Orchestration and subordinate mongo processes should listen for requests. Defaults to "localhost".
--  **-s, --server** - HTTP backend to use: one of `cherrypy` or `wsgiref`
+-  **-s, --server** - HTTP backend to use: one of `auto`, `cheroot`, or `wsgiref`. `auto`
+   configures bottle to automatically choose an available backend.
 -  **-p** - port number (8889 by default)
 -  **--socket-timeout-ms** - socket timeout when connecting to MongoDB servers
 -  **--pidfile** - location where mongo-orchestration should place its pid file
 -  **--enable-majority-read-concern** - enable "majority" read concern on server versions that support it.
 -  **start/stop/restart**: start, stop, or restart the server,
    respectively
 
@@ -186,25 +186,39 @@
                 "port": 1025
             },
             "pid": 51320
         },
         // etc.
     }
 
+Mongo Launch
+------------
+
+The ``mongo-launch`` CLI tool allows you to spin up servers locally
+with minimal configuration.
+
+..
+
+    mongo-launch --help
+    Usage: launch.py [single|replica|shard] [ssl] [auth]
+
+..
+
+    mongo-orchestration start
+    mongo-launch replica ssl auth
+
 Tests
 -----
 
-In order to run the tests, you should first clone the `repository <https://github.com/10gen/mongo-orchestration>`__. Running the tests has the following additional dependency:
-
--  `unittest2 >= 0.6 <https://pypi.python.org/pypi/unittest2>`__ (Python 2.6 only)
+In order to run the tests, you should first clone the `repository <https://github.com/10gen/mongo-orchestration>`__.
 
 Run all tests
 ~~~~~~~~~~~~~
 
-``python setup.py test``
+``python -m unittest``
 
 Run a test module
 ~~~~~~~~~~~~~~~~~
 
 ``python -m unittest tests.test_servers``
 
 Run a single test case
@@ -221,14 +235,25 @@
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 ``python -m unittest -v tests.test_servers.ServerSSLTestCase``
 
 Changelog
 ---------
 
+Changes in Version 0.8.0 (2023-05-16)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+- Add ``mongo-launch`` CLI tool.
+- Upgrade to PyMongo 4.x and set up GitHub Actions testing.
+- Remove support for managing MongoDB 3.4 or earlier servers.
+- Remove support for Python 3.5 or earlier.
+- Replaced dependency on CherryPy with cheroot. `-s auto` is the new default
+  and `-s cherrypy` is no longer supported.
+- Remove transactionLifetimeLimitSeconds default.
+
 Changes in Version 0.7.0 (2021-04-06)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 - Remove support for managing MongoDB 2.4 servers.
 - Add support for Python 3.8 and 3.9.
 - Add support for MongoDB 4.2 and 4.4.
 - Upgrade from pymongo 3.5.1 to 3.X latest. (#284).
```

### Comparing `mongo-orchestration-0.7.0/mongo_orchestration/__init__.py` & `mongo-orchestration-0.8.0/mongo_orchestration/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 # coding=utf-8
-# Copyright 2012-2014 MongoDB, Inc.
+# Copyright 2012-2023 MongoDB, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,20 +12,19 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import sys
 
+from mongo_orchestration._version import __version__
 from mongo_orchestration.servers import Servers
 from mongo_orchestration.replica_sets import ReplicaSets
 from mongo_orchestration.sharded_clusters import ShardedClusters
 
-__version__ = '0.7.0'
-
 
 def set_releases(releases=None, default_release=None):
     Servers().set_settings(releases, default_release)
     ReplicaSets().set_settings(releases, default_release)
     ShardedClusters().set_settings(releases, default_release)
```

### Comparing `mongo-orchestration-0.7.0/mongo_orchestration/apps/__init__.py` & `mongo-orchestration-0.8.0/mongo_orchestration/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `mongo-orchestration-0.7.0/mongo_orchestration/apps/links.py` & `mongo-orchestration-0.8.0/mongo_orchestration/apps/links.py`

 * *Files identical despite different names*

### Comparing `mongo-orchestration-0.7.0/mongo_orchestration/apps/replica_sets.py` & `mongo-orchestration-0.8.0/mongo_orchestration/apps/replica_sets.py`

 * *Files identical despite different names*

### Comparing `mongo-orchestration-0.7.0/mongo_orchestration/apps/servers.py` & `mongo-orchestration-0.8.0/mongo_orchestration/apps/servers.py`

 * *Files identical despite different names*

### Comparing `mongo-orchestration-0.7.0/mongo_orchestration/apps/sharded_clusters.py` & `mongo-orchestration-0.8.0/mongo_orchestration/apps/sharded_clusters.py`

 * *Files identical despite different names*

### Comparing `mongo-orchestration-0.7.0/mongo_orchestration/common.py` & `mongo-orchestration-0.8.0/mongo_orchestration/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 # coding=utf-8
-# Copyright 2014 MongoDB, Inc.
+# Copyright 2014-2023 MongoDB, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -27,15 +27,15 @@
 LOG_FILE = os.path.join(WORK_DIR, 'server.log')
 TMP_DIR = os.environ.get('MONGO_ORCHESTRATION_TMP')
 
 LOGGING_FORMAT = '%(asctime)s [%(levelname)s] %(name)s:%(lineno)d - %(message)s'
 
 DEFAULT_BIND = os.environ.get('MO_HOST', 'localhost')
 DEFAULT_PORT = int(os.environ.get('MO_PORT', '8889'))
-DEFAULT_SERVER = 'cherrypy'
+DEFAULT_SERVER = 'auto'
 DEFAULT_SOCKET_TIMEOUT = 20000  # 20 seconds.
 
 # Username for included client x509 certificate.
 DEFAULT_SUBJECT = (
     'C=US,ST=New York,L=New York City,O=MongoDB,OU=KernelUser,'
     'CN=mongo_orchestration'
 )
@@ -43,27 +43,29 @@
     os.environ.get(
         'MONGO_ORCHESTRATION_HOME', os.path.dirname(__file__)),
     'lib',
     'client.pem'
 )
 DEFAULT_SSL_OPTIONS = {
     'ssl': True,
-    'ssl_certfile': DEFAULT_CLIENT_CERT,
-    'ssl_cert_reqs': ssl.CERT_NONE
+    'tlsCertificateKeyFile': DEFAULT_CLIENT_CERT,
+    'tlsAllowInvalidCertificates': True
 }
 
 
 class BaseModel(object):
     """Base object for Server, ReplicaSet, and ShardedCluster."""
 
     _user_role_documents = [
         {'role': 'userAdminAnyDatabase', 'db': 'admin'},
         {'role': 'clusterAdmin', 'db': 'admin'},
         {'role': 'dbAdminAnyDatabase', 'db': 'admin'},
-        {'role': 'readWriteAnyDatabase', 'db': 'admin'}
+        {'role': 'readWriteAnyDatabase', 'db': 'admin'},
+        {'role': 'restore', 'db': 'admin'},
+        {'role': 'backup', 'db': 'admin'}
     ]
     socket_timeout = DEFAULT_SOCKET_TIMEOUT
 
     @property
     def key_file(self):
         """Get the path to the key file containig our auth key, or None."""
         if self.auth_key:
@@ -105,36 +107,31 @@
             return [role['role'] for role in self._user_role_documents]
         return self._user_role_documents
 
     def _add_users(self, db, mongo_version):
         """Add given user, and extra x509 user if necessary."""
         roles = self._user_roles(db.client)
         if self.x509_extra_user:
-            db.add_user(DEFAULT_SUBJECT, roles=roles)
+            db.command('createUser', DEFAULT_SUBJECT, roles=roles,
+                   writeConcern=db.write_concern.document)
             # Fix kwargs to MongoClient.
-            self.kwargs['ssl_certfile'] = DEFAULT_CLIENT_CERT
+            self.kwargs['tlsCertificateKeyFile'] = DEFAULT_CLIENT_CERT
 
         # Add secondary user given from request.
         create_user(db, mongo_version, self.login, self.password, roles)
 
 
 def create_user(db, mongo_version, user, password, roles):
-    if mongo_version >= (3, 7, 2):
-        # Call createUser directly so that the server creates the user with
-        # both SCRAM-SHA-1 and SCRAM-SHA-256 credentials. This ensures that
-        # pymongo < 3.7 (which only supports SCRAM-SHA-1) can authenticate.
-        db.command('createUser', user, pwd=password, roles=roles,
-                   writeConcern=db.write_concern.document)
-    else:
-        db.add_user(user, password=password, roles=roles)
+    db.command('createUser', user, pwd=password, roles=roles,
+               writeConcern=db.write_concern.document)
 
 
 def connected(client):
-    # Await connection in PyMongo 3.0.
-    client.admin.command('ismaster')
+    # Await connection in PyMongo.
+    client.admin.command('isMaster')
     return client
 
 
 def update(d, u):
     for k, v in u.items():
         if isinstance(v, collections.Mapping):
             r = update(d.get(k, {}), v)
```

### Comparing `mongo-orchestration-0.7.0/mongo_orchestration/compat.py` & `mongo-orchestration-0.8.0/mongo_orchestration/compat.py`

 * *Files identical despite different names*

### Comparing `mongo-orchestration-0.7.0/mongo_orchestration/configurations/replica_sets/allengines.json` & `mongo-orchestration-0.8.0/mongo_orchestration/configurations/replica_sets/allengines.json`

 * *Files identical despite different names*

### Comparing `mongo-orchestration-0.7.0/mongo_orchestration/configurations/replica_sets/arbiter.json` & `mongo-orchestration-0.8.0/mongo_orchestration/configurations/replica_sets/arbiter.json`

 * *Files identical despite different names*

### Comparing `mongo-orchestration-0.7.0/mongo_orchestration/configurations/replica_sets/auth.json` & `mongo-orchestration-0.8.0/mongo_orchestration/configurations/replica_sets/auth.json`

 * *Files identical despite different names*

### Comparing `mongo-orchestration-0.7.0/mongo_orchestration/configurations/replica_sets/basic.json` & `mongo-orchestration-0.8.0/mongo_orchestration/configurations/replica_sets/basic.json`

 * *Files identical despite different names*

### Comparing `mongo-orchestration-0.7.0/mongo_orchestration/configurations/replica_sets/clean.json` & `mongo-orchestration-0.8.0/mongo_orchestration/configurations/replica_sets/clean.json`

 * *Files identical despite different names*

### Comparing `mongo-orchestration-0.7.0/mongo_orchestration/configurations/replica_sets/mmapv1.json` & `mongo-orchestration-0.8.0/mongo_orchestration/configurations/replica_sets/mmapv1.json`

 * *Files identical despite different names*

### Comparing `mongo-orchestration-0.7.0/mongo_orchestration/configurations/replica_sets/ssl.json` & `mongo-orchestration-0.8.0/mongo_orchestration/configurations/replica_sets/ssl.json`

 * *Files identical despite different names*

### Comparing `mongo-orchestration-0.7.0/mongo_orchestration/configurations/replica_sets/ssl_auth.json` & `mongo-orchestration-0.8.0/mongo_orchestration/configurations/replica_sets/ssl_auth.json`

 * *Files identical despite different names*

### Comparing `mongo-orchestration-0.7.0/mongo_orchestration/configurations/replica_sets/wiredtiger.json` & `mongo-orchestration-0.8.0/mongo_orchestration/configurations/replica_sets/wiredtiger.json`

 * *Files identical despite different names*

### Comparing `mongo-orchestration-0.7.0/mongo_orchestration/configurations/servers/ssl_auth.json` & `mongo-orchestration-0.8.0/mongo_orchestration/configurations/servers/ssl_auth.json`

 * *Files identical despite different names*

### Comparing `mongo-orchestration-0.7.0/mongo_orchestration/configurations/sharded_clusters/auth.json` & `mongo-orchestration-0.8.0/mongo_orchestration/configurations/sharded_clusters/auth.json`

 * *Files identical despite different names*

### Comparing `mongo-orchestration-0.7.0/mongo_orchestration/configurations/sharded_clusters/clean.json` & `mongo-orchestration-0.8.0/mongo_orchestration/configurations/sharded_clusters/clean.json`

 * *Files identical despite different names*

### Comparing `mongo-orchestration-0.7.0/mongo_orchestration/configurations/sharded_clusters/ssl.json` & `mongo-orchestration-0.8.0/mongo_orchestration/configurations/sharded_clusters/ssl.json`

 * *Files identical despite different names*

### Comparing `mongo-orchestration-0.7.0/mongo_orchestration/configurations/sharded_clusters/ssl_auth.json` & `mongo-orchestration-0.8.0/mongo_orchestration/configurations/sharded_clusters/ssl_auth.json`

 * *Files identical despite different names*

### Comparing `mongo-orchestration-0.7.0/mongo_orchestration/container.py` & `mongo-orchestration-0.8.0/mongo_orchestration/container.py`

 * *Files identical despite different names*

### Comparing `mongo-orchestration-0.7.0/mongo_orchestration/daemon.py` & `mongo-orchestration-0.8.0/mongo_orchestration/daemon.py`

 * *Files identical despite different names*

### Comparing `mongo-orchestration-0.7.0/mongo_orchestration/errors.py` & `mongo-orchestration-0.8.0/mongo_orchestration/errors.py`

 * *Files identical despite different names*

### Comparing `mongo-orchestration-0.7.0/mongo_orchestration/process.py` & `mongo-orchestration-0.8.0/mongo_orchestration/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,36 +27,23 @@
 import tempfile
 
 try:
     from subprocess import DEVNULL
 except ImportError:
     DEVNULL = open(os.devnull, 'wb')
 
-from bottle import request
-
 from mongo_orchestration.common import DEFAULT_BIND, LOG_FILE
 from mongo_orchestration.compat import reraise, PY3
 from mongo_orchestration.errors import TimeoutError, RequestError
 from mongo_orchestration.singleton import Singleton
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 
 
-def _host():
-    """Get the Host from the most recent HTTP request."""
-    host_and_port = request.urlparts[1]
-    try:
-        host, _ = host_and_port.split(':')
-    except ValueError:
-        # No port yet. Host defaults to '127.0.0.1' in bottle.request.
-        return DEFAULT_BIND
-    return host or DEFAULT_BIND
-
-
 class PortPool(Singleton):
 
     __ports = set()
     __closed = set()
     __id = None
 
     def __init__(self, min_port=1025, max_port=2000, port_sequence=None):
@@ -80,15 +67,15 @@
 
     def __check_port(self, port):
         """check port status
         return True if port is free, False else
         """
         s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         try:
-            s.bind((_host(), port))
+            s.bind((DEFAULT_BIND, port))
             return True
         except socket.error:
             return False
         finally:
             s.close()
 
     def release_port(self, port):
@@ -142,15 +129,15 @@
         port_num    - port number
         timeout     - specify how long, in seconds, a command can take before times out.
     return True if process started, return False if not
     """
     s = None
     try:
         s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        s.connect((_host(), port))
+        s.connect((DEFAULT_BIND, port))
         s.close()
         return True
     except (IOError, socket.error):
         if s:
             s.close()
         return False
 
@@ -168,14 +155,15 @@
     sleeps = 0.1
     while time.time() - t_start < timeout:
         if proc.poll() is not None:
             logger.debug("process is not alive")
             raise OSError("Process started, but died immediately")
         if connect_port(port_num):
             return True
+        time.sleep(sleeps)
     return False
 
 
 def repair_mongo(name, dbpath):
     """repair mongodb after usafe shutdown"""
     log_file = os.path.join(dbpath, 'mongod.log')
     cmd = [name, "--dbpath", dbpath, "--logpath", log_file, "--logappend",
@@ -220,15 +208,15 @@
 
     cfg = read_config(config_path)
     cmd = [name, "--config", config_path]
 
     if cfg.get('port', None) is None or port:
         port = port or PortPool().port(check=True)
         cmd.extend(['--port', str(port)])
-    host = "{host}:{port}".format(host=_host(), port=port)
+    host = "{host}:{port}".format(host=DEFAULT_BIND, port=port)
     try:
         logger.debug("execute process: %s", ' '.join(cmd))
         # Redirect server startup errors (written to stdout/stderr) to our log
         with open(LOG_FILE, 'a+') as outfile:
             proc = subprocess.Popen(
                 cmd,
                 stdout=outfile,
```

### Comparing `mongo-orchestration-0.7.0/mongo_orchestration/replica_sets.py` & `mongo-orchestration-0.8.0/mongo_orchestration/replica_sets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 #!/usr/bin/python
 # coding=utf-8
-# Copyright 2012-2014 MongoDB, Inc.
+# Copyright 2012-2023 MongoDB, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
-import sys
 import tempfile
 import time
-import traceback
 
 from uuid import uuid4
 
+from concurrent.futures import ThreadPoolExecutor
+
 import pymongo
 
 from mongo_orchestration.common import (
     BaseModel, connected, DEFAULT_SUBJECT, DEFAULT_SSL_OPTIONS,
     ipv6_enabled_repl, enable_ipv6_single)
 from mongo_orchestration.singleton import Singleton
 from mongo_orchestration.container import Container
@@ -62,21 +62,22 @@
         self.restart_required = self.login or self.auth_key
         self.x509_extra_user = False
 
         if self.sslParams:
             self.kwargs.update(DEFAULT_SSL_OPTIONS)
 
         members = rs_params.get('members', [])
+        self._members = members
         # Enable ipv6 on all members if any have it enabled.
         self.enable_ipv6 = ipv6_enabled_repl(rs_params)
-
-        config = {"_id": self.repl_id, "members": [
-            self.member_create(member, index)
-            for index, member in enumerate(members)
-        ]}
+        with ThreadPoolExecutor(max_workers=10) as executor:
+            futures = [executor.submit(self.member_create, member, i)
+                       for i, member in enumerate(members)]
+            config_members = [f.result() for f in futures]
+        config = {"_id": self.repl_id, "members": config_members}
         if 'rsSettings' in rs_params:
             config['settings'] = rs_params['rsSettings']
         # Explicitly set write concern to number of data-bearing members.
         # If we add a user later, we need to guarantee that every node
         # has the user before we authenticate ('majority' is insufficient).
         self._write_concern = len(
             [m for m in members
@@ -112,53 +113,65 @@
                     self.member_id_to_host(0))
                 version = self._servers.version(server_id)
             else:
                 version = (2, 4, 0)
 
             self._add_users(self.connection()[self.auth_source], version)
         if self.restart_required:
-            # Restart all the servers with auth flags and ssl.
-            for idx, member in enumerate(members):
-                server_id = self._servers.host_to_server_id(
-                    self.member_id_to_host(idx))
-                server = self._servers._storage[server_id]
-                # If this is an arbiter, we can't authenticate as the user,
-                # so don't set the login/password.
-                if not member.get('rsParams', {}).get('arbiterOnly'):
-                    server.x509_extra_user = self.x509_extra_user
-                    server.auth_source = self.auth_source
-                    server.login = self.login
-                    server.password = self.password
-
-                def add_auth(config):
-                    if self.auth_key:
-                        config['keyFile'] = self.key_file
-                    config.update(member.get('procParams', {}))
-                    return config
-
-                server.restart(config_callback=add_auth)
-            self.restart_required = False
+            self.restart_with_auth()
 
         if not self.waiting_member_state() and self.waiting_config_state():
             raise ReplicaSetError(
                 "Could not actualize replica set configuration.")
         for i in range(100):
             if self.connection().primary:
                 break
             time.sleep(0.1)
         else:
             raise ReplicaSetError("No primary was ever elected.")
 
+    def restart_with_auth(self, cluster_auth_mode=None):
+        for server in self.server_instances():
+            server.restart_required = False
+        self.restart_required = False
+        for idx, member in enumerate(self._members):
+            server_id = self._servers.host_to_server_id(
+                self.member_id_to_host(idx))
+            server = self._servers._storage[server_id]
+            # If this is an arbiter, we can't authenticate as the user,
+            # so don't set the login/password.
+            if not member.get('rsParams', {}).get('arbiterOnly'):
+                server.x509_extra_user = self.x509_extra_user
+                server.auth_source = self.auth_source
+                server.ssl_params = self.sslParams
+                server.login = self.login
+                server.password = self.password
+                server.auth_key = self.auth_key
+
+        def add_auth(config):
+            if self.auth_key:
+                config['keyFile'] = self.key_file
+            # Add clusterAuthMode back in.
+            if cluster_auth_mode:
+                config['clusterAuthMode'] = cluster_auth_mode
+            return config
+
+        # Restart all the servers with auth flags and ssl.
+        self.restart(config_callback=add_auth)
+
     def __len__(self):
         return len(self.server_map)
 
     def cleanup(self):
         """remove all members without reconfig"""
-        for item in self.server_map:
-            self.member_del(item, reconfig=False)
+        with ThreadPoolExecutor(max_workers=10) as executor:
+            futures = [executor.submit(self.member_del, item, reconfig=False)
+                       for item in self.server_map]
+            for f in futures:
+                f.result()
         self.server_map.clear()
 
     def member_id_to_host(self, member_id):
         """return hostname by member id"""
         return self.server_map[member_id]
 
     def host2id(self, hostname):
@@ -410,70 +423,51 @@
         return "{host}:{port}".format(**locals())
 
     def get_members_in_state(self, state):
         """return all members of replica set in specific state"""
         members = self.run_command(command='replSetGetStatus', is_eval=False)['members']
         return [member['name'] for member in members if member['state'] == state]
 
-    def _authenticate_client(self, client):
-        """Authenticate the client if necessary."""
-        if self.login and not self.restart_required:
-            try:
-                db = client[self.auth_source]
-                if self.x509_extra_user:
-                    db.authenticate(
-                        DEFAULT_SUBJECT,
-                        mechanism='MONGODB-X509'
-                    )
-                else:
-                    db.authenticate(
-                        self.login, self.password)
-            except Exception:
-                logger.exception(
-                    "Could not authenticate to %r as %s/%s"
-                    % (client, self.login, self.password))
-                raise
-
-    def connection(self, hostname=None, read_preference=pymongo.ReadPreference.PRIMARY, timeout=300):
-        """return MongoReplicaSetClient object if hostname specified
-        return MongoClient object if hostname doesn't specified
+    def connection(self, hostname=None, read_preference=pymongo.ReadPreference.PRIMARY, timeout=60):
+        """Return MongoClient object, if hostname is given it is a directly connected client
         Args:
             hostname - connection uri
             read_preference - default PRIMARY
             timeout - specify how long, in seconds, a command can take before server times out.
         """
         logger.debug("connection({hostname}, {read_preference}, {timeout})".format(**locals()))
         t_start = time.time()
         servers = hostname or ",".join(self.server_map.values())
+        logger.debug("Creating connection to: {servers}".format(**locals()))
+        kwargs = self.kwargs.copy()
+        if self.login and not self.restart_required:
+            kwargs["authSource"] = self.auth_source
+            if self.x509_extra_user:
+                kwargs["username"] = DEFAULT_SUBJECT
+                kwargs["authMechanism"] = "MONGODB-X509"
+            else:
+                kwargs["username"] = self.login
+                kwargs["password"] = self.password
+        if hostname is None:
+            c = pymongo.MongoClient(
+                servers, replicaSet=self.repl_id,
+                read_preference=read_preference,
+                socketTimeoutMS=self.socket_timeout,
+                w=self._write_concern, fsync=True, **kwargs)
+        else:
+            c = pymongo.MongoClient(
+                servers, socketTimeoutMS=self.socket_timeout,
+                directConnection=True,
+                w=self._write_concern, fsync=True, **kwargs)
         while True:
             try:
-                if hostname is None:
-                    c = pymongo.MongoReplicaSetClient(
-                        servers, replicaSet=self.repl_id,
-                        read_preference=read_preference,
-                        socketTimeoutMS=self.socket_timeout,
-                        w=self._write_concern, fsync=True, **self.kwargs)
-                    connected(c)
-                    if c.primary:
-                        self._authenticate_client(c)
-                        return c
-                    raise pymongo.errors.AutoReconnect("No replica set primary available")
-                else:
-                    logger.debug("connection to the {servers}".format(**locals()))
-                    c = pymongo.MongoClient(
-                        servers, socketTimeoutMS=self.socket_timeout,
-                        w=self._write_concern, fsync=True, **self.kwargs)
-                    connected(c)
-                    self._authenticate_client(c)
-                    return c
-            except (pymongo.errors.PyMongoError):
-                exc_type, exc_value, exc_tb = sys.exc_info()
-                err_message = traceback.format_exception(exc_type, exc_value, exc_tb)
-                logger.error("Exception {exc_type} {exc_value}".format(**locals()))
-                logger.error(err_message)
+                connected(c)
+                return c
+            except pymongo.errors.PyMongoError:
+                logger.exception("Error attempting to connect to: {servers}".format(**locals()))
                 if time.time() - t_start > timeout:
                     raise pymongo.errors.AutoReconnect("Couldn't connect while timeout {timeout} second".format(**locals()))
                 time.sleep(1)
 
     def secondaries(self):
         """return list of secondaries members"""
         return [
@@ -603,21 +597,28 @@
             logger.debug("real_member_info({member_id}): {info}".format(member_id=member['_id'], info=info))
             for key in cfg_member_info:
                 if cfg_member_info[key] != real_member_info.get(key, None):
                     logger.debug("{key}: {value1} ! = {value2}".format(key=key, value1=cfg_member_info[key], value2=real_member_info.get(key, None)))
                     return False
         return True
 
+    def server_instances(self):
+        servers = []
+        for host in self.server_map.values():
+            server_id = self._servers.host_to_server_id(host)
+            servers.append(self._servers._storage[server_id])
+        return servers
+
     def restart(self, timeout=300, config_callback=None):
         """Restart each member of the replica set."""
-        for member_id in self.server_map:
-            host = self.server_map[member_id]
-            server_id = self._servers.host_to_server_id(host)
-            server = self._servers._storage[server_id]
-            server.restart(timeout, config_callback)
+        with ThreadPoolExecutor(max_workers=10) as executor:
+            futures = [executor.submit(s.restart, timeout, config_callback)
+                       for s in self.server_instances()]
+            for f in futures:
+                f.result()
         self.waiting_member_state()
 
 
 class ReplicaSets(Singleton, Container):
     """ ReplicaSets is a dict-like collection for replica set"""
     _name = 'rs'
     _obj_type = ReplicaSet
@@ -764,8 +765,8 @@
             params - new member's params
 
         return True if operation success otherwise False
         """
         repl = self[repl_id]
         result = repl.member_update(member_id, params)
         self[repl_id] = repl
-        return result
+        return result
```

### Comparing `mongo-orchestration-0.7.0/mongo_orchestration/server.py` & `mongo-orchestration-0.8.0/mongo_orchestration/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     parser.add_argument('-p', '--port',
                         action='store', dest='port', type=int,
                         default=DEFAULT_PORT)
     parser.add_argument('--enable-majority-read-concern', action='store_true',
                         default=False)
     parser.add_argument('-s', '--server',
                         action='store', dest='server', type=str,
-                        default=DEFAULT_SERVER, choices=('cherrypy', 'wsgiref'))
+                        default=DEFAULT_SERVER, choices=('auto', 'cheroot', 'wsgiref'))
     parser.add_argument('--version', action='version',
                         version='Mongo Orchestration v' + __version__)
     parser.add_argument('--socket-timeout-ms', action='store',
                         dest='socket_timeout',
                         type=int, default=DEFAULT_SOCKET_TIMEOUT)
     parser.add_argument('--pidfile', action='store', type=str, dest='pidfile',
                         default=PID_FILE)
```

### Comparing `mongo-orchestration-0.7.0/mongo_orchestration/servers.py` & `mongo-orchestration-0.8.0/mongo_orchestration/servers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 # coding=utf-8
-# Copyright 2012-2014 MongoDB, Inc.
+# Copyright 2012-2023 MongoDB, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -47,16 +47,16 @@
     enable_majority_read_concern = False
 
     # default params for all mongo instances
     mongod_default = {"oplogSize": 100, "logappend": True, "verbose": "v"}
 
     # regular expression matching MongoDB versions
     version_patt = re.compile(
-        '(?:db version v?|MongoS version v?|mongos db version v?)'
-        '(?P<version>(\d+\.)+\d+)',
+        r'(?:db version v?|MongoS version v?|mongos db version v?)'
+        r'(?P<version>(\d+\.)+\d+)',
         re.IGNORECASE)
 
     def __init_db(self, dbpath):
         if not dbpath:
             dbpath = orchestration_mkdtemp(prefix="mongod-")
         if not os.path.exists(dbpath):
             os.makedirs(dbpath)
@@ -70,17 +70,14 @@
 
     def __init_config_params(self, config):
         """Conditionally enable options in the Server's config file."""
         if self.version >= (2, 4):
             params = config.get('setParameter', {})
             # Set enableTestCommands by default but allow enableTestCommands:0.
             params.setdefault('enableTestCommands', 1)
-            # Reduce transactionLifetimeLimitSeconds for faster driver testing.
-            if self.version >= (4, 1) and not self.is_mongos:
-                params.setdefault('transactionLifetimeLimitSeconds', 3)
             # Increase transaction lock timeout to reduce the chance that tests
             # fail with LockTimeout: "Unable to acquire lock {...} within 5ms".
             if self.version >= (4, 0) and not self.is_mongos:
                 params.setdefault('maxTransactionLockRequestTimeoutMillis', 25)
             # Reduce periodicNoopIntervalSecs for faster driver change stream testing.
             if self.version >= (3, 6) and not self.is_mongos:
                 # SERVER-31132 added periodicNoopIntervalSecs in 3.6.0.
@@ -199,31 +196,27 @@
             self.config_path, self.cfg = None, {}
 
         self.port = self.cfg.get('port', None)  # connection port
 
     @property
     def connection(self):
         """return authenticated connection"""
-        c = pymongo.MongoClient(
-            self.hostname, fsync=True,
-            socketTimeoutMS=self.socket_timeout, **self.kwargs)
-        connected(c)
-        if not self.is_mongos and self.login and not self.restart_required:
-            db = c[self.auth_source]
+        kwargs = self.kwargs.copy()
+        if self.login and not self.restart_required:
+            kwargs["authSource"] = self.auth_source
             if self.x509_extra_user:
-                auth_dict = {
-                    'name': DEFAULT_SUBJECT, 'mechanism': 'MONGODB-X509'}
+                kwargs["username"] = DEFAULT_SUBJECT
+                kwargs["authMechanism"] = "MONGODB-X509"
             else:
-                auth_dict = {'name': self.login, 'password': self.password}
-            try:
-                db.authenticate(**auth_dict)
-            except:
-                logger.exception("Could not authenticate to %s with %r"
-                                 % (self.hostname, auth_dict))
-                raise
+                kwargs["username"] = self.login
+                kwargs["password"] = self.password
+        c = pymongo.MongoClient(
+            self.hostname, fsync=True, directConnection=True,
+            socketTimeoutMS=self.socket_timeout, **kwargs)
+        connected(c)
         return c
 
     @property
     def version(self):
         """Get the version of MongoDB that this Server runs as a tuple."""
         if not self.__version:
             command = (self.name, '--version')
@@ -361,14 +354,21 @@
                     logger.exception('isMaster command failed:')
             else:
                 raise TimeoutError(
                     "Server did not respond to 'isMaster' after %d attempts."
                     % max_attempts)
         except (OSError, TimeoutError):
             logpath = self.cfg.get('logpath')
+            if logpath and not os.path.exists(logpath):
+                 logger.exception(
+                    'Could not start Server')
+                 reraise(TimeoutError,
+                    'Could not start Server. '
+                    'Please check the mongo-orchestration log in ' +
+                    LOG_FILE + ' for more details.')
             if logpath:
                 # Copy the server logs into the mongo-orchestration logs.
                 logger.error(
                     "Could not start Server. Please find server log below.\n"
                     "=====================================================")
                 with open(logpath) as lp:
                     logger.error(lp.read())
@@ -409,15 +409,16 @@
         # Attempt the shutdown command twice, the first attempt might fail due
         # to an election.
         attempts = 2
         for i in range(attempts):
             logger.info("Attempting to send shutdown command to %s",
                         self.hostname)
             try:
-                client.admin.command("shutdown", force=True)
+                # SERVER-46951: Disable quiesce mode which defaults to 15 seconds.
+                client.admin.command("shutdown", force=True, timeoutSecs=0)
             except ConnectionFailure:
                 # A shutdown succeeds by closing the connection but a
                 # connection error does not necessarily mean that the shutdown
                 # has succeeded.
                 pass
             # Wait for the server to exit otherwise rerun the shutdown command.
             try:
@@ -427,15 +428,15 @@
                 continue
         raise ServersError("Server %s failed to shutdown after %s attempts" %
                            (self.hostname, attempts))
 
     def stop(self):
         """stop server"""
         try:
-            self.shutdown()
+            return self.shutdown() == 0
         except (PyMongoError, ServersError) as exc:
             logger.info("Killing %s with signal, shutdown command failed: %r",
                         self.name, exc)
             return process.kill_mprocess(self.proc)
 
     def restart(self, timeout=300, config_callback=None):
         """restart server: stop() and start()
@@ -579,8 +580,8 @@
 
     def host_to_server_id(self, hostname):
         for server_id in self._storage:
             if self._storage[server_id].hostname == hostname:
                 return server_id
 
     def is_alive(self, server_id):
-        return self._storage[server_id].is_alive
+        return self._storage[server_id].is_alive
```

### Comparing `mongo-orchestration-0.7.0/mongo_orchestration/sharded_clusters.py` & `mongo-orchestration-0.8.0/mongo_orchestration/sharded_clusters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 # coding=utf-8
-# Copyright 2012-2014 MongoDB, Inc.
+# Copyright 2012-2023 MongoDB, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -16,21 +16,23 @@
 
 import logging
 import os
 import tempfile
 
 from uuid import uuid4
 
+from concurrent.futures import ThreadPoolExecutor
+
 from mongo_orchestration import common
 from mongo_orchestration.common import (
-    BaseModel, create_user, DEFAULT_SUBJECT, DEFAULT_SSL_OPTIONS)
+    BaseModel, connected, create_user, DEFAULT_SUBJECT, DEFAULT_SSL_OPTIONS)
 from mongo_orchestration.container import Container
 from mongo_orchestration.errors import ShardedClusterError
 from mongo_orchestration.servers import Servers, Server
-from mongo_orchestration.replica_sets import ReplicaSets
+from mongo_orchestration.replica_sets import ReplicaSet, ReplicaSets
 from mongo_orchestration.singleton import Singleton
 from pymongo import MongoClient, write_concern
 
 logger = logging.getLogger(__name__)
 
 
 class ShardedCluster(BaseModel):
@@ -58,63 +60,72 @@
         if self.sslParams:
             self.kwargs.update(DEFAULT_SSL_OPTIONS)
 
         self.enable_ipv6 = common.ipv6_enabled_sharded(params)
         # Determine what to do with config servers via mongos version.
         mongos_name = os.path.join(Servers().bin_path(self._version), 'mongos')
         mongos = Server(name=mongos_name, procParams={})
-        mongos_version = mongos.version
+        self.mongos_version = mongos.version
         mongos.cleanup()
         configsvr_configs = params.get('configsvrs', [{}])
-        self.uses_rs_configdb = (mongos_version >= (3, 1, 2) and
+        self.uses_rs_configdb = (self.mongos_version >= (3, 1, 2) and
                                  len(configsvr_configs) == 1)
         self.configdb_singleton = (
             ReplicaSets() if self.uses_rs_configdb else Servers())
         if self.uses_rs_configdb:
             self.__init_configrs(configsvr_configs[0])
-        elif mongos_version >= (3, 3, 2):
+        elif self.mongos_version >= (3, 3, 2):
             raise ShardedClusterError(
                 'mongos >= 3.3.2 requires the config database to be backed by '
                 'a replica set.')
-        elif mongos_version >= (3, 1, 2) and len(configsvr_configs) != 3:
+        elif self.mongos_version >= (3, 1, 2) and len(configsvr_configs) != 3:
             raise ShardedClusterError(
                 "mongos >= 3.1.2 needs a config replica set or 3 old-style "
                 "config servers.")
         else:
             self.__init_configsvrs(configsvr_configs)
 
-        for r in params.get('routers', [{}]):
-            self.router_add(r)
-        for cfg in params.get('shards', []):
-            shard_params = cfg.get('shardParams', {})
-            shard_tags = shard_params.pop('tags', None)
-            info = self.member_add(cfg.get('id', None), shard_params)
-            if shard_tags:
-                self.tags[info['id']] = shard_tags
+        with ThreadPoolExecutor(max_workers=10) as executor:
+            futures = [executor.submit(self.router_add, r)
+                       for r in params.get('routers', [{}])]
+            for f in futures:
+                f.result()
+
+            def add_shard(cfg):
+                shard_params = cfg.get('shardParams', {})
+                shard_tags = shard_params.pop('tags', None)
+                info = self.member_add(cfg.get('id', None), shard_params)
+                if shard_tags:
+                    self.tags[info['id']] = shard_tags
+
+            futures = [executor.submit(add_shard, cfg)
+                       for cfg in params.get('shards', [])]
+            for f in futures:
+                f.result()
 
         # SERVER-37631 changed 3.6 sharded cluster setup so that it's required
         # to run refreshLogicalSessionCacheNow on the config server followed by
         # each mongos. Only then will each 3.6 mongos correctly report
         # logicalSessionTimeoutMinutes in its isMaster responses.
-        if mongos_version[:2] == (3, 6):
+        if self.mongos_version[:2] == (3, 6):
             router_clients = self.router_connections()
             is_master = router_clients[0].admin.command('isMaster')
             if 'logicalSessionTimeoutMinutes' not in is_master:
                 self.config_connection().admin.command(
                     'refreshLogicalSessionCacheNow')
                 for client in router_clients:
                     client.admin.command('refreshLogicalSessionCacheNow')
 
         if self.tags:
             for sh_id in self.tags:
                 logger.debug('Add tags %r to %s' % (self.tags[sh_id], sh_id))
                 db = self.connection().get_database(
                     'config',
                     write_concern=write_concern.WriteConcern(fsync=True))
-                db.shards.update(
+                db.shards.update_one(
                     {'_id': sh_id},
                     {'$addToSet': {'tags': {'$each': self.tags[sh_id]}}})
 
         shard_configs = [s.get('shardParams', {}).get('procParams', {})
                          for s in params.get('shards', [])]
         if self.login:
             # Do we need to add an extra x509 user?
@@ -138,30 +149,30 @@
                                     any_only_x509(shard_configs) or
                                     any_only_x509(rs_shard_configs) or
                                     any_only_x509(router_configs))
 
             self._add_users(
                 self.connection().get_database(
                     self.auth_source, write_concern=write_concern.WriteConcern(
-                        fsync=True)), mongos_version)
+                        fsync=True)), self.mongos_version)
 
             # Create the user on all the shards.
             roles = self._user_roles(self.connection())
             for shard_id, config in zip(self._shards, shard_configs):
                 shard = self._shards[shard_id]
                 instance_id = shard['_id']
                 if shard.get('isServer'):
                     client = Servers()._storage[instance_id].connection
                 elif shard.get('isReplicaSet'):
                     client = ReplicaSets()._storage[instance_id].connection()
                 db = client[self.auth_source]
                 if self.x509_extra_user:
-                    db.add_user(DEFAULT_SUBJECT, roles=roles)
+                    db.command('createUser', DEFAULT_SUBJECT, roles=roles)
 
-                create_user(db, mongos_version, self.login, self.password,
+                create_user(db, self.mongos_version, self.login, self.password,
                             roles)
 
         if self.restart_required:
             # Do we need to add clusterAuthMode back?
             cluster_auth_mode = None
             for cfg in shard_configs:
                 cam = cfg.get('clusterAuthMode')
@@ -178,34 +189,45 @@
                 server_or_rs.auth_key = self.auth_key
 
                 def add_auth(cfg):
                     if self.auth_key:
                         cfg['keyFile'] = self.key_file
                     # Add clusterAuthMode back in.
                     if cluster_auth_mode:
-                        cfg['clusterAuthMode'] = cam
+                        cfg['clusterAuthMode'] = cluster_auth_mode
                     return cfg
 
-                server_or_rs.restart(config_callback=add_auth)
-
-            for config_id in self._configsvrs:
-                restart_with_auth(self.configdb_singleton._storage[config_id])
+                if isinstance(server_or_rs, ReplicaSet):
+                    server_or_rs.restart_with_auth(cluster_auth_mode=cluster_auth_mode)
+                else:
+                    server_or_rs.restart(config_callback=add_auth)
+                server_or_rs.restart_required = False
+
+            with ThreadPoolExecutor(max_workers=10) as executor:
+                servers = []
+
+                for config_id in self._configsvrs:
+                    servers.append(self.configdb_singleton._storage[config_id])
+
+                for server_id in self._routers:
+                    server = Servers()._storage[server_id]
+                    servers.append(server)
+
+                for shard_id in self._shards:
+                    shard = self._shards[shard_id]
+                    instance_id = shard['_id']
+                    klass = ReplicaSets if shard.get('isReplicaSet') else Servers
+                    server_or_rs = klass()._storage[instance_id]
+                    servers.append(server_or_rs)
+
+                futures = [executor.submit(restart_with_auth, s) for s in servers]
+                for f in futures:
+                    f.result()
 
-            for server_id in self._routers:
-                server = Servers()._storage[server_id]
-                restart_with_auth(server)
-
-            for shard_id in self._shards:
-                shard = self._shards[shard_id]
-                instance_id = shard['_id']
-                klass = ReplicaSets if shard.get('isReplicaSet') else Servers
-                instance = klass()._storage[instance_id]
-                restart_with_auth(instance)
-
-            self.restart_required = False
+                self.restart_required = False
 
     def __init_configrs(self, rs_cfg):
         """Create and start a config replica set."""
         # Use 'rs_id' to set the id for consistency, but need to rename
         # to 'id' to use with ReplicaSets.create()
         rs_cfg['id'] = rs_cfg.pop('rs_id', None)
         for member in rs_cfg.setdefault('members', [{}]):
@@ -262,14 +284,20 @@
         for server in self._routers:
             info = Servers().info(server)
             if info['procInfo'].get('alive', False):
                 return {'id': server, 'hostname': Servers().hostname(server)}
 
     def router_add(self, params):
         """add new router (mongos) into existing configuration"""
+        # featureFlagLoadBalancer was added in 5.0.7 (SERVER-60679) and
+        # removed in 6.1.0 (SERVER-64205).
+        if (5, 0, 7) <= self.mongos_version[:3] <= (6, 1, -1):
+            set_params = params.get('setParameter', {})
+            if 'loadBalancerPort' in set_params:
+                set_params.setdefault('featureFlagLoadBalancer', True)
         if self.uses_rs_configdb:
             # Replica set configdb.
             rs_id = self._configsvrs[0]
             config_members = ReplicaSets().members(rs_id)
             configdb = '%s/%s' % (
                 rs_id, ','.join(m['host'] for m in config_members))
         else:
@@ -280,31 +308,30 @@
         params.update({'configdb': configdb})
 
         if self.enable_ipv6:
             common.enable_ipv6_single(params)
         # Remove flags that turn auth on.
         params = self._strip_auth(params)
 
-        self._routers.append(Servers().create(
+        server_id = Servers().create(
             'mongos', params, sslParams=self.sslParams, autostart=True,
-            version=version, server_id=server_id))
-        return {'id': self._routers[-1], 'hostname': Servers().hostname(self._routers[-1])}
+            version=version, server_id=server_id)
+        self._routers.append(server_id)
+        return {'id': server_id, 'hostname': Servers().hostname(server_id)}
 
     def create_connection(self, host):
+        kwargs = self.kwargs.copy()
+        if self.login and not self.restart_required:
+            kwargs["authSource"] = self.auth_source
+            kwargs["username"] = self.login
+            kwargs["password"] = self.password
         c = MongoClient(
             host, w='majority', fsync=True,
-            socketTimeoutMS=self.socket_timeout, **self.kwargs)
-        if self.login and not self.restart_required:
-            try:
-                c.admin.authenticate(self.login, self.password)
-            except:
-                logger.exception(
-                    "Could not authenticate to %s as %s/%s"
-                    % (host, self.login, self.password))
-                raise
+            socketTimeoutMS=self.socket_timeout, **kwargs)
+        connected(c)
         return c
 
     def connection(self):
         return self.create_connection(self.router['hostname'])
 
     def config_connection(self):
         """Return a MongoClient connected to the replica set config db."""
@@ -442,25 +469,33 @@
                   'orchestration': 'sharded_clusters'}
         if self.login:
             result['mongodb_auth_uri'] = self.mongodb_auth_uri(uri)
         return result
 
     def cleanup(self):
         """cleanup configuration: stop and remove all servers"""
-        for _id, shard in self._shards.items():
-            if shard.get('isServer', False):
-                Servers().remove(shard['_id'])
-            if shard.get('isReplicaSet', False):
-                ReplicaSets().remove(shard['_id'])
+        with ThreadPoolExecutor(max_workers=10) as executor:
+            futures = []
+            for _id, shard in self._shards.items():
+                if shard.get('isServer', False):
+                    futures.append(executor.submit(
+                        Servers().remove, shard['_id']))
+                if shard.get('isReplicaSet', False):
+                    futures.append(executor.submit(
+                        ReplicaSets().remove, shard['_id']))
 
-        for mongos in self._routers:
-            Servers().remove(mongos)
+            for mongos in self._routers:
+                futures.append(executor.submit(Servers().remove, mongos))
 
-        for config_id in self._configsvrs:
-            self.configdb_singleton.remove(config_id)
+            for config_id in self._configsvrs:
+                futures.append(executor.submit(
+                    self.configdb_singleton.remove, config_id))
+
+            for f in futures:
+                f.result()
 
         self._configsvrs = []
         self._routers = []
         self._shards = {}
 
 
 class ShardedClusters(Singleton, Container):
@@ -562,8 +597,8 @@
         return result
 
     def member_add(self, cluster_id, params):
         """add new member into configuration"""
         cluster = self._storage[cluster_id]
         result = cluster.member_add(params.get('id', None), params.get('shardParams', {}))
         self._storage[cluster_id] = cluster
-        return result
+        return result
```

### Comparing `mongo-orchestration-0.7.0/mongo_orchestration/singleton.py` & `mongo-orchestration-0.8.0/mongo_orchestration/singleton.py`

 * *Files identical despite different names*

### Comparing `mongo-orchestration-0.7.0/mongo_orchestration.egg-info/PKG-INFO` & `mongo-orchestration-0.8.0/mongo_orchestration.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,280 +1,302 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: mongo-orchestration
-Version: 0.7.0
+Version: 0.8.0
 Summary: Restful service for managing MongoDB servers
 Home-page: https://github.com/10gen/mongo-orchestration
 Author: MongoDB, Inc.
 Author-email: mongodb-user@googlegroups.com
 License: http://www.apache.org/licenses/LICENSE-2.0.html
-Description: -------------------
-        Mongo Orchestration
-        -------------------
-        
-        See the `wiki <https://github.com/10gen/mongo-orchestration/wiki>`__
-        for documentation.
-        
-        Mongo Orchestration is an HTTP server that provides a REST API for
-        creating and managing MongoDB configurations on a single host.
-        
-        **THIS PROJECT IS FOR TESTING OF MONGODB DRIVERS.**
-        
-        Features
-        --------
-        
-        -  Start and stop mongod servers, replica sets, and sharded clusters on the host running mongo-orchestration.
-        -  Add and remove replica set members.
-        -  Add and remove shards and mongos routers.
-        -  Reset replica sets and clusters to restart all members that were
-           stopped.
-        -  Freeze secondary members of replica sets.
-        -  Retrieve information about MongoDB resources.
-        -  Interaction all through REST interface.
-        
-        Requires
-        --------
-        
-        -  `Python 2.6, 2.7, or >= 3.2 <http://www.python.org/download/>`__
-        -  `bottle>=0.12.7 <https://pypi.python.org/pypi/bottle>`__
-        -  `pymongo>=3.0.2,<4 <https://pypi.python.org/pypi/pymongo>`__
-        -  `CherryPy>=3.5.0,<9.0.0 <http://www.cherrypy.org/>`__
-        -  `argparse>=1.2.1 <https://pypi.python.org/pypi/argparse>`__ (Python 2.6 only)
-        -  `simplejson <https://pypi.python.org/pypi/simplejson>`__ (Python 2.6 only)
-        
-        Installation
-        ------------
-        
-        The easiest way to install Mongo Orchestration is with `pip <https://pypi.python.org/pypi/pip>`__:
-        
-        ::
-        
-            pip install mongo-orchestration
-        
-        You can also install the development version of Mongo Orchestration
-        manually:
-        
-        ::
-        
-            git clone https://github.com/10gen/mongo-orchestration.git
-            cd mongo-orchestration
-            pip install .
-        
-        Cloning the `repository <https://github.com/10gen/mongo-orchestration>`__ this way will also give you access to the tests for Mongo Orchestration as well as the ``mo`` script. Note that you may
-        have to run the above commands with ``sudo``, depending on where you're
-        installing Mongo Orchestration and what privileges you have.
-        Installation will place a ``mongo-orchestration`` script on your path.
-        
-        Usage
-        -----
-        
-        ::
-        
-            mongo-orchestration [-h] [-f CONFIG] [-e ENV] [--no-fork] [-b BIND IP="localhost"] [-p PORT]
-                                [-s {cherrypy,wsgiref}] [--socket-timeout-ms MILLIS]
-                                [--pidfile PIDFILE] [--enable-majority-read-concern] {start,stop,restart}
-        
-        
-        Arguments:
-        
-        -  **-h** - show help
-        -  **-f, --config** - path to config file
-        -  **-e, --env** - default release to use, as specified in the config
-           file
-        -  **--no-fork** - run server in foreground
-        -  **-b, --bind** - host on which Mongo Orchestration and subordinate mongo processes should listen for requests. Defaults to "localhost".
-        -  **-s, --server** - HTTP backend to use: one of `cherrypy` or `wsgiref`
-        -  **-p** - port number (8889 by default)
-        -  **--socket-timeout-ms** - socket timeout when connecting to MongoDB servers
-        -  **--pidfile** - location where mongo-orchestration should place its pid file
-        -  **--enable-majority-read-concern** - enable "majority" read concern on server versions that support it.
-        -  **start/stop/restart**: start, stop, or restart the server,
-           respectively
-        
-        In addition, Mongo Orchestration can be influenced by the
-        ``MONGO_ORCHESTRATION_HOME`` environment variable, which informs the
-        server where to find the "configurations" directory for presets as well
-        as where to put the log and pid files.
-        
-        Examples
-        ~~~~~~~~
-        
-        ``mongo-orchestration start``
-        
-        Starts Mongo Orchestration as service on port 8889.
-        
-        ``mongo-orchestration stop``
-        
-        Stop the server.
-        
-        ``mongo-orchestration -f mongo-orchestration.config -e 30-release -p 8888 --no-fork start``
-        
-        Starts Mongo Orchestration on port 8888 using ``30-release`` defined in
-        ``mongo-orchestration.config``. Stops with *Ctrl+C*.
-        
-        If you have installed mongo-orchestration but you're still getting
-        ``command not found: mongo-orchestration`` this means that the script was
-        installed to a directory that is not on your ``PATH``. As an alternative use:
-        
-        ``python -m mongo_orchestration.server start``
-        
-        Configuration File
-        ~~~~~~~~~~~~~~~~~~
-        
-        Mongo Orchestration may be given a JSON configuration file with the
-        ``--config`` option specifying where to find MongoDB binaries. See
-        `mongo-orchestration.config <https://github.com/10gen/mongo-orchestration/blob/master/mongo-orchestration.config>`__
-        for an example. When no configuration file is provided, Mongo
-        Orchestration uses whatever binaries are on the user's PATH.
-        
-        Predefined Configurations
-        -------------------------
-        
-        Mongo Orchestration has a set of predefined
-        `configurations <https://github.com/10gen/mongo-orchestration/tree/master/mongo_orchestration/configurations>`__
-        that can be used to start, restart, or stop MongoDB processes. You can
-        use a tool like ``curl`` to send these files directly to the Mongo
-        Orchestration server, or use the ``mo`` script in the ``scripts``
-        directory (in the `repository <https://github.com/10gen/mongo-orchestration>`__ only). Some examples:
-        
-        -  Start a single node without SSL or auth:
-        
-           ::
-        
-               mo configurations/servers/clean.json start
-        
-        -  Get the status of a single node without SSL or auth:
-        
-           ::
-        
-               mo configurations/servers/clean.json status
-        
-        -  Stop a single node without SSL or auth:
-        
-           ::
-        
-               mo configurations/servers/clean.json stop
-        
-        -  Start a replica set with ssl and auth:
-        
-           ::
-        
-               mo configurations/replica_sets/ssl_auth.json start
-        
-        -  Use ``curl`` to create a basic sharded cluster with the id
-           "myCluster":
-        
-           ::
-        
-               curl -XPUT http://localhost:8889/v1/sharded_clusters/myCluster \
-                          -d@configurations/sharded_clusters/basic.json
-        
-        Note that in order to run the ``mo`` script, you need to be in the same
-        directory as "configurations".
-        
-        **Helpful hint**: You can prettify JSON responses from the server by
-        piping the response into ``python -m json.tool``, e.g.:
-        
-        ::
-        
-            $ curl http://localhost:8889/v1/servers/myServer | python -m json.tool
-        
-            {
-                "id": "myServer",
-                "mongodb_uri": "mongodb://localhost:1025",
-                "orchestration": "servers",
-                "procInfo": {
-                    "alive": true,
-                    "name": "mongod",
-                    "optfile": "/var/folders/v9/spc2j6cx3db71l/T/mongo-KHUACD",
-                    "params": {
-                        "dbpath": "/var/folders/v9/spc2j6cx3db71l/T/mongo-vAgYaQ",
-                        "ipv6": true,
-                        "journal": true,
-                        "logappend": true,
-                        "oplogSize": 100,
-                        "port": 1025
-                    },
-                    "pid": 51320
-                },
-                // etc.
-            }
-        
-        Tests
-        -----
-        
-        In order to run the tests, you should first clone the `repository <https://github.com/10gen/mongo-orchestration>`__. Running the tests has the following additional dependency:
-        
-        -  `unittest2 >= 0.6 <https://pypi.python.org/pypi/unittest2>`__ (Python 2.6 only)
-        
-        Run all tests
-        ~~~~~~~~~~~~~
-        
-        ``python setup.py test``
-        
-        Run a test module
-        ~~~~~~~~~~~~~~~~~
-        
-        ``python -m unittest tests.test_servers``
-        
-        Run a single test case
-        ~~~~~~~~~~~~~~~~~~~~~~
-        
-        ``python -m unittest tests.test_servers.ServerSSLTestCase``
-        
-        Run a single test method
-        ~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        ``python -m unittest tests.test_servers.ServerSSLTestCase.test_ssl_auth``
-        
-        Run a single test example for debugging with verbose and immediate stdout output
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        ``python -m unittest -v tests.test_servers.ServerSSLTestCase``
-        
-        Changelog
-        ---------
-        
-        Changes in Version 0.7.0 (2021-04-06)
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        - Remove support for managing MongoDB 2.4 servers.
-        - Add support for Python 3.8 and 3.9.
-        - Add support for MongoDB 4.2 and 4.4.
-        - Upgrade from pymongo 3.5.1 to 3.X latest. (#284).
-        - Ensure createUser succeeds on all replica set members. (#282)
-        - Create admin user with both SCRAM-SHA-256 and SCRAM-SHA-1. (#281)
-        - Wait for mongo-orchestration server to fully terminate in "stop". (#276)
-        - Allow starting clusters with enableTestCommands=0. (#269)
-        - Decrease transactionLifetimeLimitSeconds on 4.2+ by default. (#267)
-        - Increase maxTransactionLockRequestTimeoutMillis by default. (#270)
-        - Reduce periodicNoopIntervalSecs for faster driver change stream testing. (#283)
-        - Enable ztsd compression by default on 4.2+ (#263)
-        
-        Changes in Version 0.6.12 (2018-12-14)
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        - Allow running the mongo-orchestration server over IPv6 localhost. (#237)
-        - Increase default mongodb server logging verbosity. (#255)
-        - Fixed a bug when shutting down clusters where mongo-orchestration would
-          hang forever if the server had already exited. (#253)
-        
 Keywords: mongo-orchestration,mongodb,mongo,rest,testing
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.2
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: >=3.6
+Provides-Extra: test
+License-File: LICENSE
+
+-------------------
+Mongo Orchestration
+-------------------
+
+See the `wiki <https://github.com/10gen/mongo-orchestration/wiki>`__
+for documentation.
+
+Mongo Orchestration is an HTTP server that provides a REST API for
+creating and managing MongoDB configurations on a single host.
+
+**THIS PROJECT IS FOR TESTING OF MONGODB DRIVERS.**
+
+Features
+--------
+
+-  Start and stop mongod servers, replica sets, and sharded clusters on the host running mongo-orchestration.
+-  Add and remove replica set members.
+-  Add and remove shards and mongos routers.
+-  Reset replica sets and clusters to restart all members that were
+   stopped.
+-  Freeze secondary members of replica sets.
+-  Retrieve information about MongoDB resources.
+-  Interaction all through REST interface.
+-  Launch simple local servers using ``mongo-launch`` CLI tool.
+
+Requires
+--------
+
+-  `Python >=3.7 <http://www.python.org/download/>`__
+-  `bottle>=0.12.7 <https://pypi.python.org/pypi/bottle>`__
+-  `pymongo>=3.0.2,<4 <https://pypi.python.org/pypi/pymongo>`__
+-  `cheroot>=5.11 <https://pypi.python.org/pypi/cheroot/>`__
+
+Installation
+------------
+
+The easiest way to install Mongo Orchestration is with `pip <https://pypi.python.org/pypi/pip>`__:
+
+::
+
+    pip install mongo-orchestration
+
+You can also install the development version of Mongo Orchestration
+manually:
+
+::
+
+    git clone https://github.com/10gen/mongo-orchestration.git
+    cd mongo-orchestration
+    pip install .
+
+Cloning the `repository <https://github.com/10gen/mongo-orchestration>`__ this way will also give you access to the tests for Mongo Orchestration as well as the ``mo`` script. Note that you may
+have to run the above commands with ``sudo``, depending on where you're
+installing Mongo Orchestration and what privileges you have.
+Installation will place a ``mongo-orchestration`` script on your path.
+
+Usage
+-----
+
+::
+
+    mongo-orchestration [-h] [-f CONFIG] [-e ENV] [--no-fork] [-b BIND IP="localhost"] [-p PORT]
+                        [-s {auto,cheroot,wsgiref}] [--socket-timeout-ms MILLIS]
+                        [--pidfile PIDFILE] [--enable-majority-read-concern] {start,stop,restart}
+
+
+Arguments:
+
+-  **-h** - show help
+-  **-f, --config** - path to config file
+-  **-e, --env** - default release to use, as specified in the config
+   file
+-  **--no-fork** - run server in foreground
+-  **-b, --bind** - host on which Mongo Orchestration and subordinate mongo processes should listen for requests. Defaults to "localhost".
+-  **-s, --server** - HTTP backend to use: one of `auto`, `cheroot`, or `wsgiref`. `auto`
+   configures bottle to automatically choose an available backend.
+-  **-p** - port number (8889 by default)
+-  **--socket-timeout-ms** - socket timeout when connecting to MongoDB servers
+-  **--pidfile** - location where mongo-orchestration should place its pid file
+-  **--enable-majority-read-concern** - enable "majority" read concern on server versions that support it.
+-  **start/stop/restart**: start, stop, or restart the server,
+   respectively
+
+In addition, Mongo Orchestration can be influenced by the
+``MONGO_ORCHESTRATION_HOME`` environment variable, which informs the
+server where to find the "configurations" directory for presets as well
+as where to put the log and pid files.
+
+Examples
+~~~~~~~~
+
+``mongo-orchestration start``
+
+Starts Mongo Orchestration as service on port 8889.
+
+``mongo-orchestration stop``
+
+Stop the server.
+
+``mongo-orchestration -f mongo-orchestration.config -e 30-release -p 8888 --no-fork start``
+
+Starts Mongo Orchestration on port 8888 using ``30-release`` defined in
+``mongo-orchestration.config``. Stops with *Ctrl+C*.
+
+If you have installed mongo-orchestration but you're still getting
+``command not found: mongo-orchestration`` this means that the script was
+installed to a directory that is not on your ``PATH``. As an alternative use:
+
+``python -m mongo_orchestration.server start``
+
+Configuration File
+~~~~~~~~~~~~~~~~~~
+
+Mongo Orchestration may be given a JSON configuration file with the
+``--config`` option specifying where to find MongoDB binaries. See
+`mongo-orchestration.config <https://github.com/10gen/mongo-orchestration/blob/master/mongo-orchestration.config>`__
+for an example. When no configuration file is provided, Mongo
+Orchestration uses whatever binaries are on the user's PATH.
+
+Predefined Configurations
+-------------------------
+
+Mongo Orchestration has a set of predefined
+`configurations <https://github.com/10gen/mongo-orchestration/tree/master/mongo_orchestration/configurations>`__
+that can be used to start, restart, or stop MongoDB processes. You can
+use a tool like ``curl`` to send these files directly to the Mongo
+Orchestration server, or use the ``mo`` script in the ``scripts``
+directory (in the `repository <https://github.com/10gen/mongo-orchestration>`__ only). Some examples:
+
+-  Start a single node without SSL or auth:
+
+   ::
+
+       mo configurations/servers/clean.json start
+
+-  Get the status of a single node without SSL or auth:
+
+   ::
+
+       mo configurations/servers/clean.json status
+
+-  Stop a single node without SSL or auth:
+
+   ::
+
+       mo configurations/servers/clean.json stop
+
+-  Start a replica set with ssl and auth:
+
+   ::
+
+       mo configurations/replica_sets/ssl_auth.json start
+
+-  Use ``curl`` to create a basic sharded cluster with the id
+   "myCluster":
+
+   ::
+
+       curl -XPUT http://localhost:8889/v1/sharded_clusters/myCluster \
+                  -d@configurations/sharded_clusters/basic.json
+
+Note that in order to run the ``mo`` script, you need to be in the same
+directory as "configurations".
+
+**Helpful hint**: You can prettify JSON responses from the server by
+piping the response into ``python -m json.tool``, e.g.:
+
+::
+
+    $ curl http://localhost:8889/v1/servers/myServer | python -m json.tool
+
+    {
+        "id": "myServer",
+        "mongodb_uri": "mongodb://localhost:1025",
+        "orchestration": "servers",
+        "procInfo": {
+            "alive": true,
+            "name": "mongod",
+            "optfile": "/var/folders/v9/spc2j6cx3db71l/T/mongo-KHUACD",
+            "params": {
+                "dbpath": "/var/folders/v9/spc2j6cx3db71l/T/mongo-vAgYaQ",
+                "ipv6": true,
+                "journal": true,
+                "logappend": true,
+                "oplogSize": 100,
+                "port": 1025
+            },
+            "pid": 51320
+        },
+        // etc.
+    }
+
+Mongo Launch
+------------
+
+The ``mongo-launch`` CLI tool allows you to spin up servers locally
+with minimal configuration.
+
+..
+
+    mongo-launch --help
+    Usage: launch.py [single|replica|shard] [ssl] [auth]
+
+..
+
+    mongo-orchestration start
+    mongo-launch replica ssl auth
+
+Tests
+-----
+
+In order to run the tests, you should first clone the `repository <https://github.com/10gen/mongo-orchestration>`__.
+
+Run all tests
+~~~~~~~~~~~~~
+
+``python -m unittest``
+
+Run a test module
+~~~~~~~~~~~~~~~~~
+
+``python -m unittest tests.test_servers``
+
+Run a single test case
+~~~~~~~~~~~~~~~~~~~~~~
+
+``python -m unittest tests.test_servers.ServerSSLTestCase``
+
+Run a single test method
+~~~~~~~~~~~~~~~~~~~~~~~~
+
+``python -m unittest tests.test_servers.ServerSSLTestCase.test_ssl_auth``
+
+Run a single test example for debugging with verbose and immediate stdout output
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+``python -m unittest -v tests.test_servers.ServerSSLTestCase``
+
+Changelog
+---------
+
+Changes in Version 0.8.0 (2023-05-16)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+- Add ``mongo-launch`` CLI tool.
+- Upgrade to PyMongo 4.x and set up GitHub Actions testing.
+- Remove support for managing MongoDB 3.4 or earlier servers.
+- Remove support for Python 3.5 or earlier.
+- Replaced dependency on CherryPy with cheroot. `-s auto` is the new default
+  and `-s cherrypy` is no longer supported.
+- Remove transactionLifetimeLimitSeconds default.
+
+Changes in Version 0.7.0 (2021-04-06)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+- Remove support for managing MongoDB 2.4 servers.
+- Add support for Python 3.8 and 3.9.
+- Add support for MongoDB 4.2 and 4.4.
+- Upgrade from pymongo 3.5.1 to 3.X latest. (#284).
+- Ensure createUser succeeds on all replica set members. (#282)
+- Create admin user with both SCRAM-SHA-256 and SCRAM-SHA-1. (#281)
+- Wait for mongo-orchestration server to fully terminate in "stop". (#276)
+- Allow starting clusters with enableTestCommands=0. (#269)
+- Decrease transactionLifetimeLimitSeconds on 4.2+ by default. (#267)
+- Increase maxTransactionLockRequestTimeoutMillis by default. (#270)
+- Reduce periodicNoopIntervalSecs for faster driver change stream testing. (#283)
+- Enable ztsd compression by default on 4.2+ (#263)
+
+Changes in Version 0.6.12 (2018-12-14)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+- Allow running the mongo-orchestration server over IPv6 localhost. (#237)
+- Increase default mongodb server logging verbosity. (#255)
+- Fixed a bug when shutting down clusters where mongo-orchestration would
+  hang forever if the server had already exited. (#253)
```

### Comparing `mongo-orchestration-0.7.0/mongo_orchestration.egg-info/SOURCES.txt` & `mongo-orchestration-0.8.0/mongo_orchestration.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+LICENSE
 README.rst
 setup.cfg
 setup.py
 mongo_orchestration/__init__.py
+mongo_orchestration/_version.py
 mongo_orchestration/common.py
 mongo_orchestration/compat.py
 mongo_orchestration/container.py
 mongo_orchestration/daemon.py
 mongo_orchestration/errors.py
+mongo_orchestration/launch.py
 mongo_orchestration/process.py
 mongo_orchestration/replica_sets.py
 mongo_orchestration/server.py
 mongo_orchestration/servers.py
 mongo_orchestration/sharded_clusters.py
 mongo_orchestration/singleton.py
 mongo_orchestration.egg-info/PKG-INFO
@@ -43,8 +46,18 @@
 mongo_orchestration/configurations/sharded_clusters/auth.json
 mongo_orchestration/configurations/sharded_clusters/basic.json
 mongo_orchestration/configurations/sharded_clusters/clean.json
 mongo_orchestration/configurations/sharded_clusters/mmapv1.json
 mongo_orchestration/configurations/sharded_clusters/ssl.json
 mongo_orchestration/configurations/sharded_clusters/ssl_auth.json
 mongo_orchestration/configurations/sharded_clusters/wiredtiger.json
-mongo_orchestration/lib/client.pem
+mongo_orchestration/lib/ca.pem
+mongo_orchestration/lib/client.pem
+mongo_orchestration/lib/server.pem
+tests/test_container.py
+tests/test_launch.py
+tests/test_process.py
+tests/test_replica_set.py
+tests/test_replica_sets.py
+tests/test_servers.py
+tests/test_sharded_clusters.py
+tests/test_singleton.py
```

