# Comparing `tmp/daliuge-engine-2.4.0.tar.gz` & `tmp/daliuge-engine-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daliuge-engine-2.4.0.tar", last modified: Sat Mar 11 06:01:21 2023, max compression
+gzip compressed data, was "daliuge-engine-3.0.0.tar", last modified: Thu May 18 12:49:52 2023, max compression
```

## Comparing `daliuge-engine-2.4.0.tar` & `daliuge-engine-3.0.0.tar`

### file list

```diff
@@ -1,264 +1,151 @@
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:21.767352 daliuge-engine-2.4.0/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      661 2023-03-11 06:01:21.767352 daliuge-engine-2.4.0/PKG-INFO
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      136 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/README.md
--rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)     2991 2023-01-03 15:20:24.000000 daliuge-engine-2.4.0/build_engine.sh
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:21.747352 daliuge-engine-2.4.0/daliuge_engine.egg-info/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      661 2023-03-11 06:01:21.000000 daliuge-engine-2.4.0/daliuge_engine.egg-info/PKG-INFO
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6385 2023-03-11 06:01:21.000000 daliuge-engine-2.4.0/daliuge_engine.egg-info/SOURCES.txt
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)        1 2023-03-11 06:01:21.000000 daliuge-engine-2.4.0/daliuge_engine.egg-info/dependency_links.txt
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)       57 2023-03-11 06:01:21.000000 daliuge-engine-2.4.0/daliuge_engine.egg-info/entry_points.txt
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      290 2023-03-11 06:01:21.000000 daliuge-engine-2.4.0/daliuge_engine.egg-info/requires.txt
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)        4 2023-03-11 06:01:21.000000 daliuge-engine-2.4.0/daliuge_engine.egg-info/top_level.txt
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:21.747352 daliuge-engine-2.4.0/dlg/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1275 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/__init__.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:21.747352 daliuge-engine-2.4.0/dlg/apps/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1318 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/apps/__init__.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    17855 2023-02-01 10:20:19.000000 daliuge-engine-2.4.0/dlg/apps/app_base.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7347 2023-02-01 13:00:47.000000 daliuge-engine-2.4.0/dlg/apps/archiving.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    18061 2023-02-01 11:58:30.000000 daliuge-engine-2.4.0/dlg/apps/bash_shell_app.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2088 2023-02-01 10:51:59.000000 daliuge-engine-2.4.0/dlg/apps/branch.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5746 2023-02-01 12:56:38.000000 daliuge-engine-2.4.0/dlg/apps/constructs.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4692 2023-02-01 10:54:43.000000 daliuge-engine-2.4.0/dlg/apps/crc.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5420 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/apps/dlg_app.h
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1825 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/apps/dlg_app2.h
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    33790 2023-02-01 12:03:57.000000 daliuge-engine-2.4.0/dlg/apps/dockerapp.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    18587 2023-02-01 10:53:11.000000 daliuge-engine-2.4.0/dlg/apps/dynlib.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8132 2023-02-01 12:57:20.000000 daliuge-engine-2.4.0/dlg/apps/mpi.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5178 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/apps/plasmaflight.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    31043 2023-03-02 10:50:42.000000 daliuge-engine-2.4.0/dlg/apps/pyfunc.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7283 2023-02-01 12:58:49.000000 daliuge-engine-2.4.0/dlg/apps/scp.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    39355 2023-02-01 10:51:13.000000 daliuge-engine-2.4.0/dlg/apps/simple.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6483 2023-02-01 10:31:56.000000 daliuge-engine-2.4.0/dlg/apps/socket_listener.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    13674 2023-02-01 10:53:48.000000 daliuge-engine-2.4.0/dlg/dask_emulation.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:21.747352 daliuge-engine-2.4.0/dlg/data/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1155 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/data/__init__.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:21.751352 daliuge-engine-2.4.0/dlg/data/drops/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2002 2023-03-11 02:15:45.000000 daliuge-engine-2.4.0/dlg/data/drops/__init__.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2615 2023-02-01 10:21:23.000000 daliuge-engine-2.4.0/dlg/data/drops/container.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    15172 2023-03-02 10:50:42.000000 daliuge-engine-2.4.0/dlg/data/drops/data_base.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4114 2023-02-17 09:16:44.000000 daliuge-engine-2.4.0/dlg/data/drops/directorycontainer.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4090 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/data/drops/environmentvar_drop.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9764 2023-03-02 10:50:42.000000 daliuge-engine-2.4.0/dlg/data/drops/file.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1604 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/data/drops/json_drop.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5980 2023-02-04 14:39:56.000000 daliuge-engine-2.4.0/dlg/data/drops/memory.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6212 2023-02-01 10:34:21.000000 daliuge-engine-2.4.0/dlg/data/drops/ngas.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4140 2023-02-01 10:36:33.000000 daliuge-engine-2.4.0/dlg/data/drops/parset_drop.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5483 2023-02-01 10:34:49.000000 daliuge-engine-2.4.0/dlg/data/drops/plasma.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6204 2023-02-01 10:35:14.000000 daliuge-engine-2.4.0/dlg/data/drops/rdbms.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    13436 2023-02-01 11:47:15.000000 daliuge-engine-2.4.0/dlg/data/drops/s3_drop.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    27445 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/data/io.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4162 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/ddap_protocol.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:21.751352 daliuge-engine-2.4.0/dlg/deploy/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      963 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/deploy/__init__.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6349 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/deploy/common.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:21.751352 daliuge-engine-2.4.0/dlg/deploy/configs/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4724 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/deploy/configs/__init__.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    21792 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/deploy/create_dlg_job.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1162 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/deploy/deployment_constants.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8048 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/deploy/deployment_utils.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    19786 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/deploy/dlg_monitor.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10559 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/deploy/dlg_proxy.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    13963 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/deploy/helm_client.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6345 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/deploy/remotes.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7004 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/deploy/slurm_client.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    23152 2023-01-31 02:20:22.000000 daliuge-engine-2.4.0/dlg/deploy/start_dlg_cluster.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4743 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/deploy/start_helm_cluster.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:21.751352 daliuge-engine-2.4.0/dlg/deploy/utils/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    19873 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/deploy/utils/monitor_replayer.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    46987 2023-02-01 13:32:59.000000 daliuge-engine-2.4.0/dlg/drop.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    17141 2023-02-01 11:51:03.000000 daliuge-engine-2.4.0/dlg/droputils.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4539 2023-01-03 13:41:15.000000 daliuge-engine-2.4.0/dlg/event.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    14781 2023-02-01 10:33:16.000000 daliuge-engine-2.4.0/dlg/graph_loader.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      479 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/group.template
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:21.751352 daliuge-engine-2.4.0/dlg/lifecycle/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/lifecycle/__init__.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    22536 2023-02-01 10:47:49.000000 daliuge-engine-2.4.0/dlg/lifecycle/dlm.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:21.751352 daliuge-engine-2.4.0/dlg/lifecycle/hsm/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/lifecycle/hsm/__init__.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1745 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/lifecycle/hsm/manager.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9905 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/lifecycle/hsm/store.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8491 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/lifecycle/registry.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:21.751352 daliuge-engine-2.4.0/dlg/manager/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1112 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/manager/__init__.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1294 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/manager/client.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    16392 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/manager/cmdline.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    21742 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/manager/composite_manager.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1499 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/manager/constants.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4760 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/manager/drop_manager.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    21104 2023-02-01 10:47:17.000000 daliuge-engine-2.4.0/dlg/manager/node_manager.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    15303 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/manager/proc_daemon.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5087 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/manager/replay.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    25300 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/manager/rest.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    25174 2023-02-01 10:46:53.000000 daliuge-engine-2.4.0/dlg/manager/session.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3063 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/manager/shared_memory_manager.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:21.755352 daliuge-engine-2.4.0/dlg/manager/web/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    26530 2023-01-11 06:34:32.000000 daliuge-engine-2.4.0/dlg/manager/web/LICENSE
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5590 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/manager/web/dim.html
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4107 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/manager/web/dm.html
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    16527 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/manager/web/session.html
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:21.743352 daliuge-engine-2.4.0/dlg/manager/web/static/
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:21.755352 daliuge-engine-2.4.0/dlg/manager/web/static/css/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   155845 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/manager/web/static/css/bootstrap.min.css
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2145 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/manager/web/static/css/dm.css
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      929 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/manager/web/static/css/progressBar.css
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8527 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/manager/web/static/css/session.css
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:21.755352 daliuge-engine-2.4.0/dlg/manager/web/static/fonts/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    20127 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/manager/web/static/fonts/glyphicons-halflings-regular.eot
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   116671 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/manager/web/static/fonts/glyphicons-halflings-regular.svg
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    45404 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/manager/web/static/fonts/glyphicons-halflings-regular.ttf
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    23424 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/manager/web/static/fonts/glyphicons-halflings-regular.woff
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    18028 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/manager/web/static/fonts/glyphicons-halflings-regular.woff2
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:21.755352 daliuge-engine-2.4.0/dlg/manager/web/static/icons/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3660 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/manager/web/static/icons/engine.svg
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5372 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/manager/web/static/icons/liu.svg
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5403 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/manager/web/static/icons/liuFavIcon.svg
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:21.755352 daliuge-engine-2.4.0/dlg/manager/web/static/js/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    15778 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/manager/web/static/js/bootbox.min.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    78743 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/manager/web/static/js/bootstrap.bundle.min.js
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:21.755352 daliuge-engine-2.4.0/dlg/manager/web/static/js/d3/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   243027 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/manager/web/static/js/d3/d3.v5.min.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   894427 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/manager/web/static/js/d3/dagre-d3.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   725181 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/manager/web/static/js/d3/dagre-d3.min.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    26328 2023-02-01 08:50:20.000000 daliuge-engine-2.4.0/dlg/manager/web/static/js/dm.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    89501 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/manager/web/static/js/jquery-3.6.0.min.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2392 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/meta.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9599 2023-03-02 10:50:42.000000 daliuge-engine-2.4.0/dlg/named_port_utils.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5191 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/ngaslite.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2920 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/nm_dim_assigner.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      979 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/passwd.template
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2326 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/prepareUser.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1938 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/process.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4565 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/remote.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1758 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/restserver.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    11238 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/rpc.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:21.759352 daliuge-engine-2.4.0/dlg/runtime/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3371 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/runtime/__init__.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2062 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/runtime/tool_commands.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      190 2023-03-11 06:01:21.000000 daliuge-engine-2.4.0/dlg/runtime/version.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6577 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/shared_memory.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2824 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/testutils.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    16517 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/dlg/utils.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:21.759352 daliuge-engine-2.4.0/docker/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      711 2023-01-03 15:10:22.000000 daliuge-engine-2.4.0/docker/Dockerfile
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3223 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/docker/Dockerfile.casa
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      770 2023-01-03 15:44:36.000000 daliuge-engine-2.4.0/docker/Dockerfile.dev
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1871 2023-01-03 15:23:58.000000 daliuge-engine-2.4.0/docker/Dockerfile.devall
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      832 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/docker/Dockerfile.ray
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      611 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/docker/Dockerfile_incontext
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:21.743352 daliuge-engine-2.4.0/etc/
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:21.759352 daliuge-engine-2.4.0/etc/init-scripts/
--rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)     1946 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/etc/init-scripts/dlg-dim
--rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)     1950 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/etc/init-scripts/dlg-nm
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      994 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/etc/init-scripts/dlg.options
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:21.759352 daliuge-engine-2.4.0/fabfile/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)        0 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/fabfile/APPspecific.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:21.759352 daliuge-engine-2.4.0/headers/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5420 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/headers/dlg_app.h
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1825 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/headers/dlg_app2.h
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)       65 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/lib64_dist.pth
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:21.759352 daliuge-engine-2.4.0/pip/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      405 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/pip/requirements.txt
--rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)     3569 2023-01-03 16:09:08.000000 daliuge-engine-2.4.0/run_engine.sh
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)       38 2023-03-11 06:01:21.767352 daliuge-engine-2.4.0/setup.cfg
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6468 2023-03-11 05:57:46.000000 daliuge-engine-2.4.0/setup.py
--rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)      177 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/show_DIMlogs.sh
--rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)      183 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/show_NMlogs.sh
--rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)      359 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/stop_engine.sh
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:21.759352 daliuge-engine-2.4.0/test/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1496 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/__init__.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:21.759352 daliuge-engine-2.4.0/test/apps/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/apps/__init__.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:21.759352 daliuge-engine-2.4.0/test/apps/data/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   186588 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/apps/data/test_ms.tar.gz
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5909 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/apps/dynlib_example.c
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9088 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/apps/dynlib_example2.c
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1883 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/apps/setp_up.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9711 2023-02-01 12:01:45.000000 daliuge-engine-2.4.0/test/apps/test_bash.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3233 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/apps/test_crc.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8290 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/apps/test_docker.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9387 2023-02-01 10:54:03.000000 daliuge-engine-2.4.0/test/apps/test_dynlib.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10975 2023-02-01 10:53:32.000000 daliuge-engine-2.4.0/test/apps/test_dynlib2.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    15631 2023-02-01 12:06:18.000000 daliuge-engine-2.4.0/test/apps/test_pyfunc.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    13188 2023-02-01 10:52:49.000000 daliuge-engine-2.4.0/test/apps/test_simple.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3429 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/apps/test_socket.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:21.763352 daliuge-engine-2.4.0/test/deploy/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/deploy/__init__.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4673 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/deploy/test_common.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4750 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/deploy/test_helm_deploy.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1499 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/deploy/test_slurm_utils.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:21.763352 daliuge-engine-2.4.0/test/graphs/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    12730 2023-03-02 10:50:42.000000 daliuge-engine-2.4.0/test/graphs/ArrayLoopPG.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1314 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/graphs/HelloWorld_simplePG.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/graphs/__init__.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2113 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/graphs/application_args.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5533 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/graphs/compilePG.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2642 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/graphs/complex.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4632 2023-03-02 10:50:42.000000 daliuge-engine-2.4.0/test/graphs/ddTest.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8163 2023-03-02 10:50:42.000000 daliuge-engine-2.4.0/test/graphs/funcTestPG.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9219 2023-03-02 10:50:42.000000 daliuge-engine-2.4.0/test/graphs/funcTestPG_namedPorts.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10975 2023-03-02 10:50:42.000000 daliuge-engine-2.4.0/test/graphs/pyfunc_glob_testPG.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7571 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/graphs/test_graphExecution.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:21.763352 daliuge-engine-2.4.0/test/integrate/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/integrate/__init__.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:21.763352 daliuge-engine-2.4.0/test/integrate/chiles/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/integrate/chiles/__init__.py
--rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)     6157 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/integrate/chiles/chilesdo.py
--rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)     4411 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/integrate/chiles/chilesdoapp.py
--rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)     5751 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/integrate/chiles/chilesdospec.py
--rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)     6305 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/integrate/chiles/chilesdospec_docker.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2732 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/integrate/example_split.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      434 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/integrate/example_split.sh
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10795 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/integrate/freq_split.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:21.763352 daliuge-engine-2.4.0/test/integrate/msconverter/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      543 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/integrate/msconverter/makefile
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    13468 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/integrate/msconverter/ms_checker.cc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      439 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/integrate/msconverter/ms_converter.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:21.763352 daliuge-engine-2.4.0/test/lifecycle/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/lifecycle/__init__.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6489 2023-02-01 10:48:37.000000 daliuge-engine-2.4.0/test/lifecycle/test_dlm.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3552 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/lifecycle/test_registry.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:21.763352 daliuge-engine-2.4.0/test/manager/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/manager/__init__.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    13744 2023-02-01 12:43:06.000000 daliuge-engine-2.4.0/test/manager/test_daemon.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    15855 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/manager/test_dim.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    22817 2023-02-01 10:48:14.000000 daliuge-engine-2.4.0/test/manager/test_dm.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    14044 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/manager/test_mm.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9309 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/manager/test_rest.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5188 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/manager/test_scalability.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3951 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/manager/test_smm.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2400 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/manager/testutils.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3820 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/memoryUsage.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:21.767352 daliuge-engine-2.4.0/test/reproducibility/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)        0 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/reproducibility/__init__.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4421 2023-03-02 10:50:42.000000 daliuge-engine-2.4.0/test/reproducibility/testSingle.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4858 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/reproducibility/test_drophash.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9811 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/reproducibility/test_lg_blockdag.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    38201 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/reproducibility/test_pg_blockdag.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9278 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/reproducibility/test_toposort.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:21.767352 daliuge-engine-2.4.0/test/reproducibility/topoGraphs/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    13649 2023-03-02 10:50:42.000000 daliuge-engine-2.4.0/test/reproducibility/topoGraphs/computationSandwich.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    19758 2023-03-02 10:50:42.000000 daliuge-engine-2.4.0/test/reproducibility/topoGraphs/dataFan.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    20119 2023-03-02 10:50:42.000000 daliuge-engine-2.4.0/test/reproducibility/topoGraphs/dataFunnel.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    14717 2023-03-02 10:50:42.000000 daliuge-engine-2.4.0/test/reproducibility/topoGraphs/dataSandwich.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    17068 2023-03-02 10:50:42.000000 daliuge-engine-2.4.0/test/reproducibility/topoGraphs/testCycle.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      588 2023-03-02 10:50:42.000000 daliuge-engine-2.4.0/test/reproducibility/topoGraphs/testEmpty.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    16777 2023-03-02 10:50:42.000000 daliuge-engine-2.4.0/test/reproducibility/topoGraphs/testNotDAG.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4421 2023-03-02 10:50:42.000000 daliuge-engine-2.4.0/test/reproducibility/topoGraphs/testSingle.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    12955 2023-03-02 10:50:42.000000 daliuge-engine-2.4.0/test/reproducibility/topoGraphs/testTwoEnd.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    16488 2023-03-02 10:50:42.000000 daliuge-engine-2.4.0/test/reproducibility/topoGraphs/testTwoLines.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    12958 2023-03-02 10:50:42.000000 daliuge-engine-2.4.0/test/reproducibility/topoGraphs/testTwoStart.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4096 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/test_JsonDrop.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2142 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/test_ParameterSetDROP.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3677 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/test_S3Drop.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9068 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/test_dask_emulation.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    48904 2023-03-02 10:50:42.000000 daliuge-engine-2.4.0/test/test_drop.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10061 2023-02-01 11:36:05.000000 daliuge-engine-2.4.0/test/test_droputils.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10116 2023-03-02 10:50:42.000000 daliuge-engine-2.4.0/test/test_environmentvars.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1268 2023-01-03 13:41:15.000000 daliuge-engine-2.4.0/test/test_event.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8479 2023-02-01 10:56:03.000000 daliuge-engine-2.4.0/test/test_graph_loader.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1160 2023-02-01 10:55:08.000000 daliuge-engine-2.4.0/test/test_input_fired_app_drop.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1589 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/test_io.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9716 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/test_session.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4642 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/test_shared_memory.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1672 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/test_tool.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7693 2022-11-30 13:05:02.000000 daliuge-engine-2.4.0/test/test_utils.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:52.384454 daliuge-engine-3.0.0/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      642 2023-05-18 12:49:52.384454 daliuge-engine-3.0.0/PKG-INFO
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      136 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/README.md
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:52.376454 daliuge-engine-3.0.0/daliuge_engine.egg-info/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      642 2023-05-18 12:49:52.000000 daliuge-engine-3.0.0/daliuge_engine.egg-info/PKG-INFO
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3536 2023-05-18 12:49:52.000000 daliuge-engine-3.0.0/daliuge_engine.egg-info/SOURCES.txt
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)        1 2023-05-18 12:49:52.000000 daliuge-engine-3.0.0/daliuge_engine.egg-info/dependency_links.txt
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)       56 2023-05-18 12:49:52.000000 daliuge-engine-3.0.0/daliuge_engine.egg-info/entry_points.txt
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      290 2023-05-18 12:49:52.000000 daliuge-engine-3.0.0/daliuge_engine.egg-info/requires.txt
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)        4 2023-05-18 12:49:52.000000 daliuge-engine-3.0.0/daliuge_engine.egg-info/top_level.txt
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:52.376454 daliuge-engine-3.0.0/dlg/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1275 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/__init__.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:52.376454 daliuge-engine-3.0.0/dlg/apps/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1318 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/apps/__init__.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    18310 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/dlg/apps/app_base.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7656 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/dlg/apps/archiving.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    18567 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/dlg/apps/bash_shell_app.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2399 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/dlg/apps/branch.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4489 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/dlg/apps/constructs.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5002 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/dlg/apps/crc.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5420 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/apps/dlg_app.h
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1825 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/apps/dlg_app2.h
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    34885 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/dlg/apps/dockerapp.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    18700 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/dlg/apps/dynlib.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8551 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/dlg/apps/mpi.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5178 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/apps/plasmaflight.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    27590 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/dlg/apps/pyfunc.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7592 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/dlg/apps/scp.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    42198 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/dlg/apps/simple.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6484 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/dlg/apps/socket_listener.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    13666 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/dlg/dask_emulation.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:52.376454 daliuge-engine-3.0.0/dlg/data/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1155 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/data/__init__.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:52.376454 daliuge-engine-3.0.0/dlg/data/drops/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2002 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/data/drops/__init__.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2615 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/data/drops/container.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    15237 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/dlg/data/drops/data_base.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4259 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/dlg/data/drops/directorycontainer.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4254 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/dlg/data/drops/environmentvar_drop.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9770 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/dlg/data/drops/file.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1604 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/data/drops/json_drop.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6232 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/dlg/data/drops/memory.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6330 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/dlg/data/drops/ngas.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4398 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/dlg/data/drops/parset_drop.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5859 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/dlg/data/drops/plasma.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6323 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/dlg/data/drops/rdbms.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    13921 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/dlg/data/drops/s3_drop.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    27445 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/data/io.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4162 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/ddap_protocol.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:52.380454 daliuge-engine-3.0.0/dlg/deploy/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      963 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/deploy/__init__.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6349 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/deploy/common.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:52.380454 daliuge-engine-3.0.0/dlg/deploy/configs/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4724 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/deploy/configs/__init__.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    22231 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/dlg/deploy/create_dlg_job.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1162 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/deploy/deployment_constants.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8048 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/deploy/deployment_utils.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    19786 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/deploy/dlg_monitor.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10559 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/deploy/dlg_proxy.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    14426 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/dlg/deploy/helm_client.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6345 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/deploy/remotes.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7004 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/deploy/slurm_client.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    23809 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/dlg/deploy/start_dlg_cluster.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4743 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/deploy/start_helm_cluster.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    47489 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/dlg/drop.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    17100 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/dlg/droputils.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4699 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/dlg/event.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    15249 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/dlg/graph_loader.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:52.380454 daliuge-engine-3.0.0/dlg/lifecycle/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/lifecycle/__init__.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    22536 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/lifecycle/dlm.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:52.380454 daliuge-engine-3.0.0/dlg/lifecycle/hsm/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/lifecycle/hsm/__init__.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1745 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/lifecycle/hsm/manager.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9905 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/lifecycle/hsm/store.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8491 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/lifecycle/registry.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:52.380454 daliuge-engine-3.0.0/dlg/manager/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1112 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/manager/__init__.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1294 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/manager/client.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    16588 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/dlg/manager/cmdline.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    22215 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/dlg/manager/composite_manager.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1499 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/manager/constants.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4760 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/manager/drop_manager.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    21104 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/dlg/manager/node_manager.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    15303 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/manager/proc_daemon.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5087 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/manager/replay.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    25859 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/dlg/manager/rest.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    25174 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/manager/session.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3063 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/manager/shared_memory_manager.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:52.380454 daliuge-engine-3.0.0/dlg/manager/web/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5590 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/manager/web/dim.html
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4107 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/manager/web/dm.html
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    16527 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/manager/web/session.html
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:52.372454 daliuge-engine-3.0.0/dlg/manager/web/static/
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:52.380454 daliuge-engine-3.0.0/dlg/manager/web/static/css/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   155845 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/manager/web/static/css/bootstrap.min.css
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2145 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/manager/web/static/css/dm.css
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      929 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/manager/web/static/css/progressBar.css
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8527 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/manager/web/static/css/session.css
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:52.380454 daliuge-engine-3.0.0/dlg/manager/web/static/fonts/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    20127 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/manager/web/static/fonts/glyphicons-halflings-regular.eot
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   116671 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/manager/web/static/fonts/glyphicons-halflings-regular.svg
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    45404 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/manager/web/static/fonts/glyphicons-halflings-regular.ttf
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    23424 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/manager/web/static/fonts/glyphicons-halflings-regular.woff
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    18028 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/manager/web/static/fonts/glyphicons-halflings-regular.woff2
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:52.380454 daliuge-engine-3.0.0/dlg/manager/web/static/icons/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3660 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/manager/web/static/icons/engine.svg
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5372 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/manager/web/static/icons/liu.svg
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5403 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/manager/web/static/icons/liuFavIcon.svg
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:52.380454 daliuge-engine-3.0.0/dlg/manager/web/static/js/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    15778 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/manager/web/static/js/bootbox.min.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    78743 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/manager/web/static/js/bootstrap.bundle.min.js
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:52.384454 daliuge-engine-3.0.0/dlg/manager/web/static/js/d3/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   243027 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/manager/web/static/js/d3/d3.v5.min.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   894427 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/manager/web/static/js/d3/dagre-d3.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   725181 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/manager/web/static/js/d3/dagre-d3.min.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    26332 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/dlg/manager/web/static/js/dm.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    89501 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/manager/web/static/js/jquery-3.6.0.min.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2392 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/meta.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9807 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/dlg/named_port_utils.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5191 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/ngaslite.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2920 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/nm_dim_assigner.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2326 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/prepareUser.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1938 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/process.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4565 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/remote.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1758 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/restserver.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    11238 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/rpc.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:52.384454 daliuge-engine-3.0.0/dlg/runtime/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3371 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/runtime/__init__.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2062 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/runtime/tool_commands.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      190 2023-05-18 12:49:52.000000 daliuge-engine-3.0.0/dlg/runtime/version.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6577 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/shared_memory.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2824 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/dlg/testutils.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)       38 2023-05-18 12:49:52.384454 daliuge-engine-3.0.0/setup.cfg
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6468 2023-05-18 12:43:13.000000 daliuge-engine-3.0.0/setup.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:52.384454 daliuge-engine-3.0.0/test/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4096 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/test/test_JsonDrop.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2142 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/test/test_ParameterSetDROP.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3677 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/test/test_S3Drop.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9239 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/test/test_dask_emulation.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    48904 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/test/test_drop.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10493 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/test/test_droputils.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10122 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/test/test_environmentvars.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1268 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/test/test_event.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8980 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/test/test_graph_loader.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1160 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/test/test_input_fired_app_drop.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1589 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/test/test_io.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10509 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/test/test_session.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4642 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/test/test_shared_memory.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1672 2023-05-18 12:38:53.000000 daliuge-engine-3.0.0/test/test_tool.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7933 2023-05-18 12:40:21.000000 daliuge-engine-3.0.0/test/test_utils.py
```

### Comparing `daliuge-engine-2.4.0/PKG-INFO` & `daliuge-engine-3.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: daliuge-engine
-Version: 2.4.0
+Version: 3.0.0
 Summary: Data Activated 流 (flow) Graph Engine - Execution Engine
 Home-page: https://github.com/ICRAR/daliuge
 Author: ICRAR DIA Group
 Author-email: dfms_prototype@googlegroups.com
 License: LGPLv2+
-Platform: UNKNOWN
 Provides-Extra: spead
 Provides-Extra: drive-casa
 Provides-Extra: MPI
 Provides-Extra: aws
 
 
         The element of the DALiuGE system executing the workflows. This replaces
         the former 'runtime' package (up to version 1.0). For more information 
         see the [Basics section(https://daliuge.readthedocs.io/en/latest/basics.html)]
         of the DALiuGE documentation.
         
-
```

### Comparing `daliuge-engine-2.4.0/daliuge_engine.egg-info/PKG-INFO` & `daliuge-engine-3.0.0/daliuge_engine.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: daliuge-engine
-Version: 2.4.0
+Version: 3.0.0
 Summary: Data Activated 流 (flow) Graph Engine - Execution Engine
 Home-page: https://github.com/ICRAR/daliuge
 Author: ICRAR DIA Group
 Author-email: dfms_prototype@googlegroups.com
 License: LGPLv2+
-Platform: UNKNOWN
 Provides-Extra: spead
 Provides-Extra: drive-casa
 Provides-Extra: MPI
 Provides-Extra: aws
 
 
         The element of the DALiuGE system executing the workflows. This replaces
         the former 'runtime' package (up to version 1.0). For more information 
         see the [Basics section(https://daliuge.readthedocs.io/en/latest/basics.html)]
         of the DALiuGE documentation.
         
-
```

### Comparing `daliuge-engine-2.4.0/dlg/__init__.py` & `daliuge-engine-3.0.0/dlg/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/apps/__init__.py` & `daliuge-engine-3.0.0/dlg/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/apps/app_base.py` & `daliuge-engine-3.0.0/dlg/apps/app_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,14 @@
     to be run at `initialize` time, while other might start during the first invocation
     of `dataWritten`. A common scenario anyway is to start an application only
     after all its inputs have moved to COMPLETED (implying that none of them is
     an streaming input); for these cases see the `BarrierAppDROP`.
     """
 
     def initialize(self, **kwargs):
-
         super(AppDROP, self).initialize(**kwargs)
 
         # Inputs and Outputs are the DROPs that get read from and written
         # to by this AppDROP, respectively. An input DROP will see
         # this AppDROP as one of its consumers, while an output DROP
         # will see this AppDROP as one of its producers.
         #
@@ -141,14 +140,18 @@
         ):
             for i in range(len(self._inputs)):
                 key = list(self.parameters["inputs"][i].values())[0]
                 value = self._inputs[
                     list(self.parameters["inputs"][i].keys())[0]
                 ]
                 named_inputs[key] = value
+        else:
+            for key, field in self.parameters["applicationArgs"].items():
+                if field["usage"] in ["InputPort", "InputOutput"]:
+                    named_inputs[field["name"]] = field
         return named_inputs
 
     def _generateNamedOutputs(self):
         """
         Generates a named mapping of output data drops. Can only be called during run().
         """
         named_outputs: OrderedDict[str, DataDROP] = OrderedDict()
@@ -157,14 +160,18 @@
         ):
             for i in range(len(self._outputs)):
                 key = list(self.parameters["outputs"][i].values())[0]
                 value = self._outputs[
                     list(self.parameters["outputs"][i].keys())[0]
                 ]
                 named_outputs[key] = value
+        else:
+            for key, field in self.parameters["applicationArgs"].items():
+                if field["usage"] in ["OutputPort", "InputOutput"]:
+                    named_outputs[field["name"]] = field
         return named_outputs
 
     def handleEvent(self, e):
         """
         Handles the arrival of a new event. Events are delivered from those
         objects this DROP is subscribed to.
         """
@@ -208,15 +215,17 @@
         """
         is_error = self._execStatus == AppDROPStates.ERROR
         if is_error:
             self.status = DROPStates.ERROR
         else:
             self.status = DROPStates.COMPLETED
         logger.debug(
-            "Moving %r to %s", self, "FINISHED" if not is_error else "ERROR"
+            "Moving %r to %s",
+            self.oid,
+            "FINISHED" if not is_error else "ERROR",
         )
         self._fire(
             "producerFinished", status=self.status, execStatus=self.execStatus
         )
         self.completedrop()
 
     def cancel(self):
@@ -350,15 +359,14 @@
 
         error_len = len(self._errorInputs)
         ok_len = len(self._completedInputs)
         skipped_len = len(self._skippedInputs)
 
         # We have enough inputs to proceed
         if (skipped_len + error_len + ok_len) == n_eff_inputs:
-
             # calculate the number of errors that have already occurred
             percent_failed = math.floor(
                 (error_len / float(n_eff_inputs)) * 100
             )
             if percent_failed > 0:
                 logger.debug(
                     "Error rate on inputs for %r: %d/%d",
@@ -414,15 +422,15 @@
         all its inputs are COMPLETED.
         """
 
         # TODO: We need to be defined more clearly how the state is set in
         #       applications, for the time being they follow their execState.
 
         # Run at most self._n_tries if there are errors during the execution
-        logger.debug("Executing %r", self)
+        logger.debug("Executing %r", self.oid)
         tries = 0
         drop_state = DROPStates.COMPLETED
         self.execStatus = AppDROPStates.RUNNING
         while tries < self.n_tries:
             try:
                 if hasattr(self, "_tp"):
                     proc = DlgProcess(target=self.run, daemon=True)
@@ -442,15 +450,15 @@
                 self.execStatus = AppDROPStates.FINISHED
                 break
             except:
                 if self.execStatus == AppDROPStates.CANCELLED:
                     return
                 tries += 1
                 logger.exception(
-                    "Error while executing %r (try %d/%d)",
+                    "Error while executing %r (try %s/%s)",
                     self,
                     tries,
                     self.n_tries,
                 )
 
         # We gave up running the application, go to error
         if tries == self.n_tries:
```

### Comparing `daliuge-engine-2.4.0/dlg/apps/archiving.py` & `daliuge-engine-3.0.0/dlg/apps/archiving.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,15 +54,14 @@
         "of view of the DALiuGE framework.",
         [dlg_batch_input("binary/*", [])],
         [dlg_batch_output("binary/*", [])],
         [dlg_streaming_input("binary/*")],
     )
 
     def run(self):
-
         # Check that the constrains are correct
         if self.outputs:
             raise Exception(
                 "No outputs should be declared for this application"
             )
         if len(self.inputs) != 1:
             raise Exception("Only one input is expected by this application")
@@ -80,15 +79,17 @@
 
 ##
 # @brief NgasArchivingApp
 # @details Takes an input and archives it in an NGAS server.
 # @par EAGLE_START
 # @param category PythonApp
 # @param tag daliuge
-# @param appclass Application class/dlg.apps.archiving.NgasArchivingApp/String/ComponentParameter/readonly//False/False/Application class
+# @param dropclass Application Class/dlg.apps.archiving.NgasArchivingApp/String/ComponentParameter/readonly//False/False/Application class
+# @param input_parser Input Parser/pickle/Select/ApplicationArgument/readwrite/raw,pickle,eval,npy,path,dataurl/False/False/Input port parsing technique
+# @param output_parser Output Parser/pickle/Select/ApplicationArgument/readwrite/raw,pickle,eval,npy,path,dataurl/False/False/Output port parsing technique
 # @param execution_time Execution Time/5/Float/ComponentParameter/readonly//False/False/Estimated execution time
 # @param num_cpus No. of CPUs/1/Integer/ComponentParameter/readonly//False/False/Number of cores used
 # @param group_start Group start/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the start of a group?
 # @param input_error_threshold "Input error rate (%)"/0/Integer/ComponentParameter/readwrite//False/False/the allowed failure rate of the inputs (in percent), before this component goes to ERROR state and is not executed
 # @param n_tries Number of tries/1/Integer/ComponentParameter/readwrite//False/False/Specifies the number of times the 'run' method will be executed before finally giving up
 # @param ngasSrv NGAS Server URL/localhost/String/ApplicationArgument/readwrite//False/False/URL of the NGAS Server
 # @param ngasPort NGAS Server Port/7777/Integer/ApplicationArgument/readwrite//False/False/TCP/IP Port on the NGAS Server
```

### Comparing `daliuge-engine-2.4.0/dlg/apps/bash_shell_app.py` & `daliuge-engine-3.0.0/dlg/apps/bash_shell_app.py`

 * *Files 4% similar despite different names*

```diff
@@ -198,29 +198,29 @@
         `stdin` indicates at file descriptor or file object to use as the standard
         input of the bash process. If not given no stdin is given to the process.
 
         Similarly, `stdout` is a file descriptor or file object where the standard
         output of the process is piped to. If not given it is consumed by this
         method and potentially logged.
         """
-        # logger.debug("Parameters found: %s", json.dumps(self.parameters))
+        logger.debug("Parameters found: %s", json.dumps(self.parameters))
+        logger.debug("Bash Inputs: %s; Bash Outputs: %s", inputs, outputs)
         # we only support passing a path for bash apps
         fsInputs = {
             uid: i for uid, i in inputs.items() if droputils.has_path(i)
         }
         fsOutputs = {
             uid: o for uid, o in outputs.items() if droputils.has_path(o)
         }
         dataURLInputs = {
             uid: i for uid, i in inputs.items() if not droputils.has_path(i)
         }
         dataURLOutputs = {
             uid: o for uid, o in outputs.items() if not droputils.has_path(o)
         }
-
         # deal with named ports
         inport_names = (
             self.parameters["inputs"] if "inputs" in self.parameters else []
         )
         outport_names = (
             self.parameters["outputs"] if "outputs" in self.parameters else []
         )
@@ -261,15 +261,15 @@
         if self._dlg_session:
             env.update({"DLG_SESSION_ID": self._dlg_session.sessionId})
 
         env.update({"DLG_ROOT": utils.getDlgDir()})
 
         # Wrap everything inside bash
         cmd = ("/bin/bash", "-c", cmd)
-        logger.debug("Command after wrapping is: %s", cmd)
+        logger.info("Command after wrapping is: %s", cmd)
 
         start = time.time()
 
         # Run and wait until it finishes
         process = subprocess.Popen(
             cmd,
             close_fds=True,
@@ -383,14 +383,17 @@
 # @param tag template
 # @param command Command//String/ComponentParameter/readwrite//False/False/The command to be executed
 # @param input_redirection Input Redirection//String/ComponentParameter/readwrite//False/False/The command line argument that specifies the input into this application
 # @param output_redirection Output Redirection//String/ComponentParameter/readwrite//False/False/The command line argument that specifies the output from this application
 # @param command_line_arguments Command Line Arguments//String/ComponentParameter/readwrite//False/False/Additional command line arguments to be added to the command line to be executed
 # @param paramValueSeparator Param value separator/ /String/ComponentParameter/readwrite//False/False/Separator character(s) between parameters on the command line
 # @param argumentPrefix Argument prefix/"--"/String/ComponentParameter/readwrite//False/False/Prefix to each keyed argument on the command line
+# @param dropclass dropclass/dlg.apps.bash_shell_app.BashShellApp/String/ComponentParameter/readwrite//False/False/Drop class
+# @param input_parser Input Parser/pickle/Select/ApplicationArgument/readwrite/raw,pickle,eval,npy,path,dataurl/False/False/Input port parsing technique
+# @param output_parser Output Parser/pickle/Select/ApplicationArgument/readwrite/raw,pickle,eval,npy,path,dataurl/False/False/Output port parsing technique
 # @param execution_time Execution Time/5/Float/ComponentParameter/readonly//False/False/Estimated execution time
 # @param num_cpus No. of CPUs/1/Integer/ComponentParameter/readonly//False/False/Number of cores used
 # @param group_start Group start/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the start of a group?
 # @param input_error_threshold "Input error rate (%)"/0/Integer/ComponentParameter/readwrite//False/False/the allowed failure rate of the inputs (in percent), before this component goes to ERROR state and is not executed
 # @param n_tries Number of tries/1/Integer/ComponentParameter/readwrite//False/False/Specifies the number of times the 'run' method will be executed before finally giving up
 # @par EAGLE_END
 class BashShellApp(BashShellBase, BarrierAppDROP):
```

### Comparing `daliuge-engine-2.4.0/dlg/apps/branch.py` & `daliuge-engine-3.0.0/dlg/apps/branch.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from dlg.drop import track_current_drop
 from dlg.apps.app_base import BarrierAppDROP
 from dlg.exceptions import InvalidDropException
 
+
 ##
 # @brief Branch
 # @details A conditional branch to control flow
 # @par EAGLE_START
 # @param category Branch
 # @param tag template
-# @param appclass Application Class/dlg.apps.simple.SimpleBranch/String/ComponentParameter/readonly//False/False/Application class
+# @param dropclass Application Class/dlg.apps.simple.SimpleBranch/String/ComponentParameter/readonly//False/False/Application class
+# @param input_parser Input Parser/pickle/Select/ApplicationArgument/readwrite/raw,pickle,eval,npy,path,dataurl/False/False/Input port parsing technique
+# @param output_parser Output Parser/pickle/Select/ApplicationArgument/readwrite/raw,pickle,eval,npy,path,dataurl/False/False/Output port parsing technique
 # @param execution_time Execution Time/5/Float/ComponentParameter/readonly//False/False/Estimated execution time
 # @param num_cpus No. of CPUs/1/Integer/ComponentParameter/readonly//False/False/Number of cores used
 # @param group_start Group start/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the start of a group?
 # @param input_error_threshold "Input error rate (%)"/0/Integer/ComponentParameter/readwrite//False/False/the allowed failure rate of the inputs (in percent), before this component goes to ERROR state and is not executed
 # @param n_tries Number of tries/1/Integer/ComponentParameter/readwrite//False/False/Specifies the number of times the 'run' method will be executed before finally giving up
 # @param dummy0 dummy0//Object/OutputPort/readwrite//False/False/Dummy output port
 # @param dummy1 dummy1//Object/OutputPort/readwrite//False/False/Dummy output port
```

### Comparing `daliuge-engine-2.4.0/dlg/apps/crc.py` & `daliuge-engine-3.0.0/dlg/apps/crc.py`

 * *Files 11% similar despite different names*

```diff
@@ -82,15 +82,17 @@
 ##
 # @brief CRCStreamApp
 # @details Calculate CRC in the streaming mode
 # i.e. A "streamingConsumer" of its predecessor in the graph
 # @par EAGLE_START
 # @param category PythonApp
 # @param tag daliuge
-# @param appclass Application Class/dlg.apps.crc.CRCStreamApp/String/ComponentParameter/readonly//False/False/Application class
+# @param dropclass Application Class/dlg.apps.crc.CRCStreamApp/String/ComponentParameter/readonly//False/False/Application class
+# @param input_parser Input Parser/pickle/Select/ApplicationArgument/readwrite/raw,pickle,eval,npy,path,dataurl/False/False/Input port parsing technique
+# @param output_parser Output Parser/pickle/Select/ApplicationArgument/readwrite/raw,pickle,eval,npy,path,dataurl/False/False/Output port parsing technique
 # @param execution_time Execution Time/5/Float/ComponentParameter/readonly//False/False/Estimated execution time
 # @param num_cpus No. of CPUs/1/Integer/ComponentParameter/readonly//False/False/Number of cores used
 # @param group_start Group start/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the start of a group?
 # @param input_error_threshold "Input error rate (%)"/0/Integer/ComponentParameter/readwrite//False/False/the allowed failure rate of the inputs (in percent), before this component goes to ERROR state and is not executed
 # @param n_tries Number of tries/1/Integer/ComponentParameter/readwrite//False/False/Specifies the number of times the 'run' method will be executed before finally giving up
 # @param data Data//String/OutputPort/readwrite//False/False/Input data stream
 # @par EAGLE_END
```

### Comparing `daliuge-engine-2.4.0/dlg/apps/dlg_app.h` & `daliuge-engine-3.0.0/dlg/apps/dlg_app.h`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/apps/dlg_app2.h` & `daliuge-engine-3.0.0/dlg/apps/dlg_app2.h`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/apps/dockerapp.py` & `daliuge-engine-3.0.0/dlg/apps/dockerapp.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,14 +84,17 @@
 # @param digest Digest//String/ComponentParameter/readwrite//False/False/The hexadecimal hash (long version) of the docker image to be used for this application
 # @param command Command//String/ComponentParameter/readwrite//False/False/The command line to run within the docker instance. The specified command will be executed in a bash shell. That means that images will need a bash shell.
 # @param input_redirection Input Redirection//String/ComponentParameter/readwrite//False/False/The command line argument that specifies the input into this application
 # @param output_redirection Output Redirection//String/ComponentParameter/readwrite//False/False/The command line argument that specifies the output from this application
 # @param command_line_arguments Command Line Arguments//String/ComponentParameter/readwrite//False/False/Additional command line arguments to be added to the command line to be executed
 # @param paramValueSeparator Param value separator/ /String/ComponentParameter/readwrite//False/False/Separator character(s) between parameters and their respective values on the command line
 # @param argumentPrefix Argument prefix/"--"/String/ComponentParameter/readwrite//False/False/Prefix to each keyed argument on the command line
+# @param dropclass dropclass/dlg.apps.dockerapp.DockerApp/String/ComponentParameter/readwrite//False/False/Drop class
+# @param input_parser Input Parser/pickle/Select/ApplicationArgument/readwrite/raw,pickle,eval,npy,path,dataurl/False/False/Input port parsing technique
+# @param output_parser Output Parser/pickle/Select/ApplicationArgument/readwrite/raw,pickle,eval,npy,path,dataurl/False/False/Output port parsing technique
 # @param execution_time Execution Time/5/Float/ComponentParameter/readonly//False/False/Estimated execution time
 # @param num_cpus No. of CPUs/1/Integer/ComponentParameter/readonly//False/False/Number of cores used
 # @param group_start Group start/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the start of a group?
 # @param input_error_threshold "Input error rate (%)"/0/Integer/ComponentParameter/readwrite//False/False/the allowed failure rate of the inputs (in percent), before this component goes to ERROR state and is not executed
 # @param n_tries Number of tries/1/Integer/ComponentParameter/readwrite//False/False/Specifies the number of times the 'run' method will be executed before finally giving up
 # @param user User//String/ComponentParameter/readwrite//False/False/Username of the user who will run the application within the docker image
 # @param ensureUserAndSwitch Ensure User And Switch/False/Boolean/ComponentParameter/readwrite//False/False/Make sure the user specified in the User parameter exists and then run the docker container as that user
@@ -235,14 +238,16 @@
 
     def initialize(self, **kwargs):
         self._containerLock = multiprocessing.Lock()
         super().initialize(**kwargs)
 
         self._image = self._popArg(kwargs, "image", None)
         self._env = self._popArg(kwargs, "env", None)
+        self._inputRedirect = self._popArg(kwargs, "input_redirection", "")
+        self._outputRedirect = self._popArg(kwargs, "output_redirection", "")
         self._cmdLineArgs = self._popArg(kwargs, "command_line_arguments", "")
         self._applicationArgs = self._popArg(kwargs, "applicationArgs", {})
         self._argumentPrefix = self._popArg(kwargs, "argumentPrefix", "--")
         self._paramValueSeparator = self._popArg(
             kwargs, "paramValueSeparator", " "
         )
         if not self._image:
@@ -391,15 +396,14 @@
         self._fire("containerIp", containerIp=containerIp)
 
     @property
     def containerId(self):
         return self._containerId
 
     def handleInterest(self, drop):
-
         # The only interest we currently have is the containerIp of other
         # DockerApps, and only if our command actually uses this IP
         if isinstance(drop, DockerApp):
             if "%containerIp[{0}]%".format(drop.uid) in self._command:
                 self._waiters.append(ContainerIpWaiter(drop))
                 logger.debug("%r: Added ContainerIpWaiter for %r", self, drop)
 
@@ -561,37 +565,46 @@
             if cmd:
                 cmd = droputils.replace_path_placeholders(
                     cmd, dockerInputs, dockerOutputs
                 )
                 cmd = droputils.replace_dataurl_placeholders(
                     cmd, dataURLInputs, dataURLOutputs
                 )
+                # if "output_redirection" in self._applicationArgs:
+                #     logger.debug(">>>> outport_names: %s", outport_names)
+                #     out_name = outport_names["output_redirection"]
+                #     cmd = f"{cmd} > {out_name}"
+                # if "input_redirection" in self._applicationArgs:
+                #     in_name = inport_names["input_redirection"]
+                #     cmd = f"cat {in_name} > {cmd}"
             else:
                 cmd = ""
             ###############
             # Wait until the DockerApps this application runtime depends on have
             # started, and replace their IP placeholders by the real IPs
             for waiter in self._waiters:
                 uid, ip = waiter.waitForIp()
                 cmd = cmd.replace("%containerIp[{0}]%".format(uid), ip)
                 logger.debug("Command after IP replacement is: %s", cmd)
 
             # Wrap everything inside bash
             if len(cmd) > 0 and not self._noBash:
-                cmd = '/bin/bash -c "%s"' % (
-                    utils.escapeQuotes(cmd, singleQuotes=False)
+                cmd = (
+                    '/bin/bash -c "%s"'
+                    % (utils.escapeQuotes(cmd, singleQuotes=False)).strip()
                 )
-                logger.debug(
+                logger.info(
                     "Command after user creation and wrapping is: %s", cmd
                 )
             else:
-                logger.debug(
-                    "executing container with default cmd and wrapped arguments"
+                cmd = f"{utils.escapeQuotes(cmd, singleQuotes=False)}".strip()
+                logger.info(
+                    "executing container with default cmd and wrapped arguments: %s",
+                    cmd,
                 )
-                cmd = f"{utils.escapeQuotes(cmd, singleQuotes=False)}"
 
             c = DockerApp._get_client()
             logger.debug(
                 f"Final user for container: {self._user}:{self._userid}"
             )
 
             # Create container
```

### Comparing `daliuge-engine-2.4.0/dlg/apps/dynlib.py` & `daliuge-engine-3.0.0/dlg/apps/dynlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -321,15 +321,14 @@
             raise InvalidDropException(self, e.args[0])
 
         # Have we properly set the outputs in the C application structure yet?
         self._c_outputs_set = False
         self._c_outputs_setting_lock = threading.Lock()
 
     def _ensure_c_outputs_are_set(self):
-
         with self._c_outputs_setting_lock:
             if self._c_outputs_set:
                 return
             prepare_c_outputs(self._c_app, self.outputs)
 
 
 class DynlibStreamApp(DynlibAppBase, AppDROP):
@@ -379,14 +378,15 @@
 ##
 # @brief DynlibApp
 # @details An application component run from a dynamic library
 # @par EAGLE_START
 # @param category DynlibApp
 # @param tag template
 # @param libpath Library Path//String/ComponentParameter/readwrite//False/False/The location of the shared object/DLL that implements this application
+# @param dropclass dropclass/dlg.apps.dynlib.DynlibApp/String/ComponentParameter/readwrite//False/False/Drop class
 # @param execution_time Execution Time/5/Float/ComponentParameter/readonly//False/False/Estimated execution time
 # @param num_cpus No. of CPUs/1/Integer/ComponentParameter/readonly//False/False/Number of cores used
 # @param group_start Group start/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the start of a group?
 # @param input_error_threshold "Input error rate (%)"/0/Integer/ComponentParameter/readwrite//False/False/the allowed failure rate of the inputs (in percent), before this component goes to ERROR state and is not executed
 # @param n_tries Number of tries/1/Integer/ComponentParameter/readwrite//False/False/Specifies the number of times the 'run' method will be executed before finally giving up
 # @par EAGLE_END
 class DynlibApp(DynlibAppBase, BarrierAppDROP):
@@ -493,15 +493,14 @@
             raise InvalidDropException(self, "library not specified")
         self.libname = kwargs.pop("lib")
         self.timeout = self._popArg(kwargs, "timeout", 600)  # 10 minutes
         self.app_params = kwargs
         self.proc = None
 
     def run(self):
-
         if not hasattr(self, "_rpc_server"):
             raise Exception("DynlibProcApp can only run within an RPC server")
 
         # On the sub-process we create DropProxy objects, so we need to extract
         # from our inputs/outputs their contact point (RPC-wise) information.
         # If one of our inputs/outputs is a DropProxy we already have this
         # information; otherwise we must figure it out.
```

### Comparing `daliuge-engine-2.4.0/dlg/apps/mpi.py` & `daliuge-engine-3.0.0/dlg/apps/mpi.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,27 +27,31 @@
 import sys
 
 from dlg.apps.app_base import BarrierAppDROP
 from ..exceptions import InvalidDropException
 
 logger = logging.getLogger(__name__)
 
+
 ##
 # @brief MPI
 # @details An application component using the Message Passing Interface (MPI)
 # @par EAGLE_START
 # @param category Mpi
 # @param tag template
 # @param num_of_procs Num procs/1/Integer/ComponentParameter/readwrite//False/False/Number of processes used for this application
 # @param command Command//String/ComponentParameter/readwrite//False/False/The command to be executed
 # @param input_redirection Input Redirection//String/ComponentParameter/readwrite//False/False/The command line argument that specifies the input into this application
 # @param output_redirection Output Redirection//String/ComponentParameter/readwrite//False/False/The command line argument that specifies the output from this application
 # @param command_line_arguments Command Line Arguments//String/ComponentParameter/readwrite//False/False/Additional command line arguments to be added to the command line to be executed
 # @param paramValueSeparator Param value separator/ /String/ComponentParameter/readwrite//False/False/Separator character(s) between parameters on the command line
 # @param argumentPrefix Argument prefix/"--"/String/ComponentParameter/readwrite//False/False/Prefix to each keyed argument on the command line
+# @param dropclass dropclass/dlg.apps.mpi.MPIApp/String/ComponentParameter/readwrite//False/False/Drop class
+# @param input_parser Input Parser/pickle/Select/ApplicationArgument/readwrite/raw,pickle,eval,npy,path,dataurl/False/False/Input port parsing technique
+# @param output_parser Output Parser/pickle/Select/ApplicationArgument/readwrite/raw,pickle,eval,npy,path,dataurl/False/False/Output port parsing technique
 # @param execution_time Execution Time/5/Float/ComponentParameter/readonly//False/False/Estimated execution time
 # @param num_cpus No. of CPUs/1/Integer/ComponentParameter/readonly//False/False/Number of cores used
 # @param group_end Group end/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the end of a group?
 # @param input_error_threshold "Input error rate (%)"/0/Integer/ComponentParameter/readwrite//False/False/the allowed failure rate of the inputs (in percent), before this component goes to ERROR state and is not executed
 # @param n_tries Number of tries/1/Integer/ComponentParameter/readwrite//False/False/Specifies the number of times the 'run' method will be executed before finally giving up
 # @par EAGLE_END
 class MPIApp(BarrierAppDROP):
```

### Comparing `daliuge-engine-2.4.0/dlg/apps/plasmaflight.py` & `daliuge-engine-3.0.0/dlg/apps/plasmaflight.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/apps/pyfunc.py` & `daliuge-engine-3.0.0/dlg/apps/pyfunc.py`

 * *Files 10% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         )
     logger.debug(f"Introspection of function {f}: {a}")
     logger.debug("Defaults for function %r: %r", f, adefaults)
     return fser, fdefaults
 
 
 def import_using_name(app, fname):
-    logger.debug("Import from %s", fname)
+    logger.debug("Importing %s", fname)
     parts = fname.split(".")
     # If only one part check if builtin
     if len(parts) < 2:
         b = globals()["__builtins__"]
         logger.debug(f"Builtins: {type(b)}")
         logger.debug(f"Function {fname}: {hasattr(b, fname)}")
         if fname in b:
@@ -137,14 +137,15 @@
 
 
 def import_using_code(code):
     return dill.loads(code)
 
 
 class DropParser(Enum):
+    RAW = "raw"
     PICKLE = "pickle"
     EVAL = "eval"
     NPY = "npy"
     # JSON = "json"
     PATH = "path"  # input only
     DATAURL = "dataurl"  # input only
 
@@ -156,25 +157,24 @@
 # Conversely, the output of the function is treated as the output of the
 # application. If the application has more than one output, the result of
 # calling the function is treated as an iterable, with each individual object
 # being written to its corresponding output.
 # @par EAGLE_START
 # @param category PythonApp
 # @param tag template
-# @param appclass Application Class/dlg.apps.pyfunc.PyFuncApp/String/ComponentParameter/readonly//False/False/Application class
+# @param func_name Function Name//String/ApplicationArgument/readwrite//False/False/Python function name
+# @param func_code Function Code//String/ApplicationArgument/readwrite//False/False/Python function code, e.g. 'def function_name(args): return args'
+# @param dropclass Application Class/dlg.apps.pyfunc.PyFuncApp/String/ComponentParameter/readonly//False/False/Application class
 # @param execution_time Execution Time/5/Float/ComponentParameter/readonly//False/False/Estimated execution time
 # @param num_cpus No. of CPUs/1/Integer/ComponentParameter/readonly//False/False/Number of cores used
 # @param group_start Group start/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the start of a group?
 # @param input_error_threshold "Input error rate (%)"/0/Integer/ComponentParameter/readwrite//False/False/The allowed failure rate of the inputs (in percent), before this component goes to ERROR state and is not executed
 # @param n_tries Number of tries/1/Integer/ComponentParameter/readwrite//False/False/Specifies the number of times the 'run' method will be executed before finally giving up
-# @param func_name Function Name//String/ApplicationArgument/readwrite//False/False/Python function name
-# @param func_code Function Code//String/ApplicationArgument/readwrite//False/False/Python function code, e.g. 'def function_name(args): return args'
-# @param input_parser Input Parser/pickle/Select/ApplicationArgument/readwrite/pickle,eval,npy,path,dataurl/False/False/Input port parsing technique
-# @param output_parser Output Parser/pickle/Select/ApplicationArgument/readwrite/pickle,eval,npy/False/False/Output port parsing technique
-# @param func_defaults Function Defaults//String/ApplicationArgument/readwrite//False/False/
+# @param input_parser Input Parser/pickle/Select/ApplicationArgument/readwrite/raw,pickle,eval,npy,path,dataurl/False/False/Input port parsing technique
+# @param output_parser Output Parser/pickle/Select/ApplicationArgument/readwrite/raw,pickle,eval,npy,path,dataurl/False/False/Output port parsing technique
 #     \~English Mapping from argname to default value. Should match only the last part of the argnames list.
 #               Values are interpreted as Python code literals and that means string values need to be quoted.
 # @param func_arg_mapping Function Arguments Mapping//String/ApplicationArgument/readwrite//False/False/
 #     \~English Mapping between argument name and input drop uids
 # @par EAGLE_END
 class PyFuncApp(BarrierAppDROP):
     """
@@ -196,25 +196,14 @@
     DLG_ROOT/code. That directory is always available, even if the engine is
     running in a docker container.
 
     Otherwise, users can also *send* over the python code using the ``func_code``
     parameter. The code needs to be base64-encoded and produced with the marshal
     module of the same Python version used to run DALiuGE.
 
-    Both inputs and outputs are (de-)serialized using the pickle protocol if the value
-    of the respective boolean component parameter is set to True. This is also
-    applied to func_defaults and func_arg_mappings.
-
-    In addition to the input mapping the implementation also allows to set defaults
-    both in the function itself and in a logical graph. If set in the logical graph
-    using the func_defaults parameter, the defaults need to be specified as a
-    dictionary of the form
-
-    ``{"kwargs":{"kw1_name":kw1_value, "kw2_name":kw2_value}, "args":[arg1, arg2]}``
-
     The positional onlyargs will be used in order of appearance.
     """
 
     component_meta = dlg_component(
         "PyFuncApp",
         "Py Func App.",
         [dlg_batch_input("binary/*", [])],
@@ -227,48 +216,24 @@
     input_parser: DropParser = dlg_enum_param(DropParser, "input_parser", DropParser.PICKLE)  # type: ignore
     output_parser: DropParser = dlg_enum_param(DropParser, "output_parser", DropParser.PICKLE)  # type: ignore
     func_arg_mapping = dlg_dict_param("func_arg_mapping", {})
     func_defaults = dlg_dict_param("func_defaults", {})
     f: Callable
     fdefaults: dict
 
-    def _init_func_defaults(self):
+    def _mixin_func_defaults(self):
         """
-        Inititalize self.func_defaults dictionary from values provided.
-        Multiple options exist and some are here for compatibility.
+        func_defaults can be passed in through an argument, but this is only used for
+        dlg_delayed and in combination with passing func_code. For dlg_delayed the function
+        and its parameters might be computed on a different host than the where the delayed
+        function is called and thus the function needs to be serialized.
         """
         logger.debug(
             f"Starting evaluation of func_defaults: {self.func_defaults}"
         )
-        self.arguments = inspect.getfullargspec(self.f)
-        self.argsig = inspect.signature(
-            self.f
-        )  # TODO: Move to using signature only
-        logger.debug("Function inspection revealed %s", self.arguments)
-        logger.debug("Function sigature: %s", self.argsig)
-        self.fn_nargs = len(self.arguments.args)
-        self.fn_npos = sum(
-            [
-                1
-                if p.kind == p.POSITIONAL_OR_KEYWORD
-                and p.default != inspect._empty
-                else 0
-                for p in self.argsig.parameters.values()
-            ]
-        )
-        self.arguments_defaults = [
-            v.default if v.default != inspect._empty else None
-            for v in self.argsig.parameters.values()
-        ]
-        logger.debug("Got signature for function %s %s", self.f, self.argsig)
-        self.fn_defaults = self.arguments_defaults
-
-        self.fn_ndef = (
-            len(self.arguments_defaults) if self.arguments_defaults else 0
-        )
         if (
             isinstance(self.func_defaults, dict)
             and len(self.func_defaults) > 0
             and list(self.func_defaults.keys()) == ["kwargs", "args"]
         ):
             for arg in self.func_defaults["args"]:
                 self.func_defaults["kwargs"][arg] = arg
@@ -288,48 +253,106 @@
                 type(self.func_defaults),
             )
             raise ValueError
         if self.input_parser is DropParser.PICKLE:
             # only values are pickled, get them unpickled
             for name, value in self.func_defaults.items():
                 self.func_defaults[name] = deserialize_data(value)
+        # the fn_defaults are used afterwards, we'll drop the func_defaults
+        logger.debug("fn_defaults %s", self.fn_defaults)
+        logger.debug("func_defaults %s", self.func_defaults)
+        self.fn_defaults = self.func_defaults
 
-        # set the function defaults from introspection
-        if self.arguments:
-            # self.fn_npos = len(self.arguments.args) - self.fn_ndef
-            self.fn_posargs = self.arguments.args[
-                : self.fn_npos
-            ]  # positional arg names
-            self.fn_defaults = {
-                name: None for name in self.arguments.args[: self.fn_npos]
-            }
-            logger.debug(f"initialized fn_defaults with {self.fn_defaults}")
-            # deal with args and kwargs
-            kwargs = (
-                dict(
-                    zip(
-                        self.arguments.args[self.fn_npos :],
-                        self.arguments.defaults,
-                    )
-                )
-                if self.arguments.defaults
-                else {}
-            )
-            self.fn_defaults.update(kwargs)
-            logger.debug(f"fn_defaults updated with {kwargs}")
-            # deal with kwonlyargs
-            if self.arguments.kwonlydefaults:
-                kwonlyargs = dict(
-                    zip(
-                        self.arguments.kwonlyargs,
-                        self.arguments.kwonlydefaults,
-                    )
-                )
-                self.fn_defaults.update(kwonlyargs)
-                logger.debug(f"fn_defaults updated with {kwonlyargs}")
+    def _init_fn_defaults(self):
+        """
+        Inititalize self.fn_defaults dictionary from values provided.
+        Multiple options exist and some are here for compatibility.
+        """
+        logger.debug(f"Starting evaluation of function signature")
+        self.argsig = inspect.signature(self.f)
+        self.argnames = list(self.argsig.parameters.keys())
+        logger.debug("Function signature: %s", self.argsig)
+        args = list(self.argsig.parameters.keys())
+        self.fn_nargs = len(self.argsig.parameters)
+        # set defaults
+        self.fn_nposkw = 0
+        self.poskw = {}
+        self.fn_npos = 0
+        self.posonly = {}
+        self.kwonly = {}
+        self.fn_nkw = 0
+        self.varargs = False
+        self.varkw = False
+        self.fn_ndef = 0
+        for k, p in self.argsig.parameters.items():
+            if not isinstance(p, str):
+                if p.kind == p.POSITIONAL_OR_KEYWORD:
+                    self.fn_nposkw += 1
+                    self.poskw.update({k: p})
+                elif p.kind == p.POSITIONAL_ONLY:
+                    self.fn_npos += 1
+                    self.posonly.update({k: p})
+                elif p.kind == p.KEYWORD_ONLY:
+                    self.fn_nkw += 1
+                    self.kwonly.update({k: p})
+                elif p.kind == p.VAR_POSITIONAL:
+                    self.varargs = True
+                elif p.kind == p.VAR_KEYWORD:
+                    self.varkw = True
+                if p.default != inspect._empty:
+                    self.arguments_defaults.append(p.default)
+                    self.fn_ndef += 1
+                else:
+                    self.arguments_defaults.append(None)
+                    self.fn_ndef += 1
+
+        logger.debug("Got signature for function %s %s", self.f, self.argsig)
+        logger.debug(
+            "Got default values for arguments %s", self.arguments_defaults
+        )
+        self.fn_defaults = self.arguments_defaults
+        logger.debug(f"initialized fn_defaults with {self.fn_defaults}")
+
+    def _clean_applicationArgs(self):
+        """
+        remove function definition arguments in applicationArgs
+        """
+        self.func_def_keywords = [
+            "func_code",
+            "func_name",
+            "func_arg_mapping",
+            "input_parser",
+            "output_parser",
+            "func_defaults",
+            "pickle",
+        ]
+
+        for kw in self.func_def_keywords:
+            if kw in self._applicationArgs:  # these are the preferred ones now
+                if isinstance(
+                    self._applicationArgs[kw]["value"],
+                    bool
+                    or self._applicationArgs[kw]["value"]
+                    or self._applicationArgs[kw]["precious"],
+                ):
+                    # only transfer if there is a value or precious is True
+                    self._applicationArgs.pop(kw)
+
+    def initialize_with_func_code(self):
+        """
+        This function takes over if code is passed in through an argument.
+        """
+        if not isinstance(self.func_code, bytes):
+            self.func_code = base64.b64decode(self.func_code.encode("utf8"))
+        self.f = import_using_code(self.func_code)
+        self._init_fn_defaults()
+        # make sure defaults are dicts
+        self._mixin_func_defaults()
+        if isinstance(self.func_arg_mapping, str):
+            self.func_arg_mapping = ast.literal_eval(self.func_arg_mapping)
 
     def initialize(self, **kwargs):
         """
         The initialization of a function component is mainly dealing with mapping
         inputs and provided applicationArgs to the function arguments. All of this
         should be driven by matching names.
         """
@@ -341,114 +364,82 @@
             env.update({"DLG_SESSION_ID": self._dlg_session.sessionId})
 
         self._applicationArgs = self._popArg(kwargs, "applicationArgs", {})
 
         self.func_code = self._popArg(kwargs, "func_code", None)
         self.arguments_defaults = []
 
-        # check for function definition arguments in applicationArgs
-        self.func_def_keywords = [
-            "func_code",
-            "func_name",
-            "func_arg_mapping",
-            "input_parser",
-            "output_parser",
-            "func_defaults",
-            "pickle",
-        ]
-
         # backwards compatibility
         if "pickle" in self._applicationArgs:
             if self._applicationArgs["pickle"]["value"] == True:
                 self.input_parser = DropParser.PICKLE
                 self.output_parser = DropParser.PICKLE
             else:
                 self.input_parser = DropParser.EVAL
                 self.output_parser = DropParser.EVAL
             self._applicationArgs.pop("pickle")
 
-        for kw in self.func_def_keywords:
-            if kw in self._applicationArgs:  # these are the preferred ones now
-                if isinstance(
-                    self._applicationArgs[kw]["value"],
-                    bool
-                    or self._applicationArgs[kw]["value"]
-                    or self._applicationArgs[kw]["precious"],
-                ):
-                    # only transfer if there is a value or precious is True
-                    self._applicationArgs.pop(kw)
+        self._clean_applicationArgs()
 
         self.num_args = len(
             self._applicationArgs
         )  # number of additional arguments provided
 
         if not self.func_name and not self.func_code:
             raise InvalidDropException(
                 self, "No function specified (either via name or code)"
             )
 
         # Lookup function or import bytecode as a function
         if not self.func_code:
             self.f = import_using_name(self, self.func_name)
+            self._init_fn_defaults()
         else:
-            if not isinstance(self.func_code, bytes):
-                self.func_code = base64.b64decode(
-                    self.func_code.encode("utf8")
-                )
-            self.f = import_using_code(self.func_code)
-        # make sure defaults are dicts
-        if isinstance(self.func_defaults, str):
-            self.func_defaults = ast.literal_eval(self.func_defaults)
-        if isinstance(self.func_arg_mapping, str):
-            self.func_arg_mapping = ast.literal_eval(self.func_arg_mapping)
+            self.initialize_with_func_code()
 
-        self._init_func_defaults()
         logger.info(f"Args summary for '{self.func_name}':")
-        logger.info(f"Args: {self.arguments.args}")
+        logger.info(f"Args: {self.argnames}")
         logger.info(f"Args defaults:  {self.fn_defaults}")
-        logger.info(f"Args positional: {self.arguments.args[:self.fn_npos]}")
-        logger.info(f"Args keyword: {self.arguments.args[self.fn_npos:]}")
-        logger.info(f"Args supplied:  {self.func_defaults}")
-        logger.info(f"VarArgs allowed:  {self.arguments.varargs}")
-        logger.info(f"VarKwds allowed:  {self.arguments.varkw}")
+        logger.info(f"Args pos/kw: {list(self.poskw.keys())}")
+        logger.info(f"Args keyword only: {list(self.kwonly.keys())}")
+        logger.info(f"VarArgs allowed:  {self.varargs}")
+        logger.info(f"VarKwds allowed:  {self.varkw}")
 
         # Mapping between argument name and input drop uids
         logger.debug(f"Input mapping provided: {self.func_arg_mapping}")
         self._recompute_data = {}
 
     def run(self):
         """
         Function positional and keyword argument treatment:
 
         Function arguments can be provided in four different ways:
         1) Through an input port
         2) By specifying ApplicationArgs (one for each argument)
-        3) By specifying a func_defaults dictionary in the ComponentParameters
-        4) Through defaults at the time of function definition
+        3) Through defaults at the time of function definition
 
         The priority follows the list above with input ports overruling the others.
         Function arguments in Python can be passed as positional, kw-value, positional
         only, kw-value only, and catch-all args and kwargs, which don't provide any
         hint about the names of accepted parameters. All of them are now supported. If
         positional arguments or kw-value arguments are provided by the user, but are
         not explicitely defined in the function signiture AND args and/or kwargs are
         allowed then these arguments are passed to the function. For args this is
         somewhat risky, since the order is relevant and in this code derived from the
         order defined in the graph (same order as defined in the component description).
 
-        Input ports will NOT be used by order (anymore), but by the IdText (name field
-        in EAGLE) of the port. Since each input port requires an associated data drop,
-        this provides a unique mapping. This also allows to pass values to any function
-        argument through a port.
+        Input ports will NOT be used by order (anymore), but by the name of the port.
+        Since each input port requires an associated data drop, this provides a unique
+        mapping. This also allows to pass values to any function argument through a port.
 
         Function argument values as well as the function code can be provided in
         serialised (pickle) form by setting the 'pickle' flag. Note that this flag
         is valid for all arguments and the code (if specified) in a global way.
         """
-
+        funcargs = {}
         # Inputs are un-pickled and treated as the arguments of the function
         # Their order must be preserved, so we use an OrderedDict
         if self.input_parser is DropParser.PICKLE:
             # all_contents = lambda x: pickle.loads(droputils.allDropContents(x))
             all_contents = droputils.load_pickle
         elif self.input_parser is DropParser.EVAL:
 
@@ -479,79 +470,93 @@
                 if self.output_parser is DropParser.PATH
                 else None
             )
 
         # Keyword arguments are made up of the default values plus the inputs
         # that match one of the keyword argument names
         # if defaults dict has not been specified at all we'll go ahead anyway
-        n_args = len(self.func_defaults)
-        argnames = self.arguments.args
-
-        # use explicit mapping of inputs to arguments first
-        # TODO: Required by dlg_delayed?? Else, we should really not do this.
-        kwargs = {
-            name: inputs.pop(uid)
-            for name, uid in self.func_arg_mapping.items()
-            if name in self.func_defaults or name not in argnames
-        }
-        logger.debug(f"updating funcargs with {kwargs}")
-        funcargs = kwargs
 
-        # Fill arguments with rest of inputs
+        # 1. Fill arguments with rest of inputs
         logger.debug(f"available inputs: {inputs}")
 
-        # if we have named ports use the inputs with
-        # the correct UIDs
-        logger.debug(f"Parameters found: {self.parameters}")
-        posargs = self.arguments.args[: self.fn_npos]
-        keyargs = self.arguments.args[self.fn_npos :]
+        posargs = list(self.posonly.keys()) + list(self.poskw.keys())
         kwargs = {}
         pargs = []
-        # Initialize pargs dictionary and update with provided argument values
-        pargsDict = collections.OrderedDict(
-            zip(posargs, [None] * len(posargs))
-        )
-        if self.arguments_defaults:
-            keyargsDict = dict(
-                zip(keyargs, self.arguments_defaults[self.fn_npos :])
-            )
-        else:
-            keyargsDict = {}
-        logger.debug("Initial keyargs dictionary: %s", keyargsDict)
+        # fill the pargsDict with positional and poskw arguments and defaults
+        pargsDict = {k: v.default for k, v in self.posonly.items()}
+        pargsDict.update({k: v.default for k, v in self.poskw.items()})
+        logger.debug("Initial pos_kwargs dictionary: %s", pargsDict)
+        # fill the keyargsDict with kwonly arguments and defaults
+        keyargsDict = {k: v.default for k, v in self.kwonly.items()}
+        logger.debug("Initial kwonly dictionary: %s", self.kwonly)
+
+        # replace default argument values with provided values
         if "applicationArgs" in self.parameters:
             appArgs = self.parameters[
                 "applicationArgs"
             ]  # we'll pop the identified ones
             _dum = [
                 appArgs.pop(k) for k in self.func_def_keywords if k in appArgs
             ]
             logger.debug(
                 "Identified keyword arguments removed: %s",
-                [i["text"] for i in _dum],
+                [i for i in _dum],
             )
             pargsDict.update(
                 {
                     k: self.parameters[k]
                     for k in pargsDict
                     if k in self.parameters
                 }
             )
             # if defined in both we use AppArgs values
             pargsDict.update(
                 {k: appArgs[k]["value"] for k in pargsDict if k in appArgs}
             )
-            logger.debug("Initial posargs dictionary: %s", pargsDict)
-        else:
-            appArgs = {}
+            logger.debug("Updated posargs dictionary: %s", pargsDict)
 
+            keyargsDict.update(
+                {k: appArgs[k]["value"] for k in keyargsDict if k in appArgs}
+            )
+            logger.debug("Updated keyargs dictionary: %s", keyargsDict)
+
+            # 2. put all remaining arguments into *args and **kwargs
+            # TODO: This should only be done if the function signature allows it
+            vparg = []
+            vkarg = {}
+            logger.debug(f"Remaining AppArguments {appArgs}")
+            for arg in appArgs:
+                if appArgs[arg]["type"] in ["Json", "Complex"]:
+                    value = ast.literal_eval(appArgs[arg]["value"])
+                else:
+                    value = appArgs[arg]["value"]
+                if appArgs[arg]["positional"]:
+                    vparg.append(value)
+                else:
+                    vkarg.update({arg: value})
+
+            # TODO: check where this is defined in signiture
+            self.arguments = inspect.getfullargspec(self.f)
+            if self.arguments.varargs:
+                logger.debug("Adding remaining *args to pargs %s", vparg)
+                pargs.extend(vparg)
+            if self.arguments.varkw:
+                logger.debug(
+                    "Adding remaining **kwargs to funcargs: %s", vkarg
+                )
+                funcargs.update(vkarg)
+
+        # 3. replace default argument values with named input ports
+        # TODO: investigate performing inputs and outputs in a single call
         if "inputs" in self.parameters and check_ports_dict(
             self.parameters["inputs"]
         ):
             check_len = min(
-                len(inputs), self.fn_nargs + len(self.arguments.kwonlyargs)
+                len(inputs),
+                self.fn_nargs + self.fn_nkw,
             )
             inputs_dict = collections.OrderedDict()
             for inport in self.parameters["inputs"]:
                 key = list(inport.keys())[0]
                 inputs_dict[key] = {"name": inport[key], "path": inputs[key]}
             kwargs.update(
                 identify_named_ports(
@@ -560,25 +565,23 @@
                     pargsDict,
                     keyargsDict,
                     check_len=check_len,
                     mode="inputs",
                 )
             )
         else:
+            # Just as a fallback using the index, but this is risky!
             for i in range(min(len(inputs), self.fn_nargs)):
-                kwargs.update(
-                    {self.arguments.args[i]: list(inputs.values())[i]}
-                )
+                kwargs.update({self.argnames[i]: list(inputs.values())[i]})
 
+        # 4. replace default argument values with named output ports
         if "outputs" in self.parameters and check_ports_dict(
             self.parameters["outputs"]
         ):
-            check_len = min(
-                len(outputs), self.fn_nargs + len(self.arguments.kwonlyargs)
-            )
+            check_len = min(len(outputs), self.fn_nargs + self.fn_nkw)
             outputs_dict = collections.OrderedDict()
             for outport in self.parameters["outputs"]:
                 key = list(outport.keys())[0]
                 outputs_dict[key] = {
                     "name": outport[key],
                     "path": outputs[key],
                 }
@@ -589,129 +592,49 @@
                     posargs,
                     pargsDict,
                     keyargsDict,
                     check_len=check_len,
                     mode="outputs",
                 )
             )
-        logger.debug(f"Updating funcargs with input ports {kwargs}")
-        funcargs.update(kwargs)
-
-        # Try to get values for still missing positional arguments from Application Args
-        if "applicationArgs" in self.parameters:
-            for pa in posargs:
-                if pa != "self" and pa not in funcargs:
-                    if pa in appArgs:
-                        arg = appArgs.pop(pa)
-                        value = arg["value"]
-                        ptype = arg["type"]
-                        if ptype in ["Complex", "Json"]:
-                            try:
-                                value = ast.literal_eval(value)
-                            except Exception as e:
-                                # just go on if this did not work
-                                logger.warning("Eval raised an error: %s", e)
-                        elif ptype in ["Python"]:
-                            try:
-                                import numpy
-
-                                value = eval(value, {"numpy": numpy}, {})
-                            except:
-                                pass
-                        pargsDict.update({pa: value})
-                    elif pa != "self" and pa not in pargsDict:
-                        logger.warning(
-                            f"Required positional argument '{pa}' not found!"
-                        )
-            _dum = [appArgs.pop(k) for k in pargsDict if k in appArgs]
-            logger.debug(
-                "Identified positional arguments removed: %s",
-                [i["text"] for i in _dum],
-            )
-            logger.debug(f"updating posargs with {list(pargsDict.keys())}")
-            pargs.extend(list(pargsDict.values()))
-
-            # Try to get values for still missing kwargs arguments from Application kws
-            kwargs = {}
-            kws = self.arguments.args[self.fn_npos :]
-            for ka in kws:
-                if ka not in funcargs:
-                    if ka in appArgs:
-                        arg = appArgs.pop(ka)
-                        value = arg["value"]
-                        ptype = arg["type"]
-                        if ptype in ["Complex", "Json"]:
-                            try:
-                                value = ast.literal_eval(value)
-                            except:
-                                pass
-                        kwargs.update({ka: value})
-                    else:
-                        logger.warning(f"Keyword argument '{ka}' not found!")
-            logger.debug(f"updating funcargs with {kwargs}")
-            funcargs.update(kwargs)
-
-            # deal with kwonlyargs
-            kwargs = {}
-            kws = self.arguments.kwonlyargs
-            for ka in kws:
-                if ka not in funcargs:
-                    if ka in appArgs:
-                        arg = appArgs.pop(ka)
-                        value = arg["value"]
-                        ptype = arg["type"]
-                        if ptype in ["Complex", "Json"]:
-                            try:
-                                value = ast.literal_eval(value)
-                            except:
-                                pass
-                        kwargs.update({ka: value})
-                    else:
-                        logger.warning(
-                            f"Keyword only argument '{ka}' not found!"
-                        )
-            logger.debug(f"updating funcargs with kwonlyargs: {kwargs}")
-            funcargs.update(kwargs)
-
-            # any remaining application arguments will be used for vargs and vkwargs
-            vparg = []
-            vkarg = {}
-            logger.debug(f"Remaining AppArguments {appArgs}")
-            for arg in appArgs:
-                if appArgs[arg]["type"] in ["Json", "Complex"]:
-                    value = ast.literal_eval(appArgs[arg]["value"])
-                else:
-                    value = appArgs[arg]["value"]
-                if appArgs[arg]["positional"]:
-                    vparg.append(value)
-                else:
-                    vkarg.update({arg: value})
-
-            if self.arguments.varargs:
-                logger.debug("Adding remaining posargs to varargs")
-                pargs.extend(vparg)
-            if self.arguments.varkw:
-                logger.debug("Adding remaining kwargs to varkw")
-                funcargs.update(vkarg)
+        logger.debug(
+            f"Updating funcargs with values from pargsDict {pargsDict}"
+        )
+        funcargs.update(pargsDict)
 
-        # Fill rest with default arguments if there are any more
-        kwargs = {}
-        for kw in self.func_defaults.keys():
-            value = self.func_defaults[kw]
-            if kw not in funcargs:
-                kwargs.update({kw: value})
-        logger.debug(f"updating funcargs with {kwargs}")
+        logger.debug(
+            f"Updating funcargs with values from named ports {kwargs}"
+        )
         funcargs.update(kwargs)
+
         self._recompute_data["args"] = funcargs.copy()
-        logger.debug(f"Running {self.func_name} with *{pargs} **{funcargs}")
 
+        # 5. remove self argument if this is the initializer.
+        if (
+            self.func_name is not None
+            and self.func_name.split(".")[-1] in ["__init__", "__class__"]
+            and "self" in funcargs
+        ):
+            funcargs.pop("self")
+        logger.info(f"Running {self.func_name} with *{pargs} **{funcargs}")
+
+        # 6. prepare for execution
         # we capture and log whatever is produced on STDOUT
         capture = StringIO()
+        try:
+            bind = self.argsig.bind(*pargs, **funcargs)
+            logger.debug("Bound arguments: %s", bind)
+        except TypeError as e:
+            logger.error("Binding of arguments failed: %s", e)
+            raise
+
+        # Here is where the function is actually executed
         with redirect_stdout(capture):
-            result = self.f(*pargs, **funcargs)
+            result = self.f(*bind.args, **bind.kwargs)
+
         logger.debug("Returned result from %s: %s", self.func_name, result)
         logger.info(
             f"Captured output from function app '{self.func_name}': {capture.getvalue()}"
         )
         logger.debug(f"Finished execution of {self.func_name}.")
 
         # Depending on how many outputs we have we treat our result
```

### Comparing `daliuge-engine-2.4.0/dlg/apps/scp.py` & `daliuge-engine-3.0.0/dlg/apps/scp.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,17 @@
 
 ##
 # @brief ScpApp
 # @details A BarrierAppDROP that copies the content of its single input onto its single output via SSH's scp protocol.
 # @par EAGLE_START
 # @param category PythonApp
 # @param tag daliuge
-# @param appclass Application Class/dlg.apps.scp.ScpApp/String/ComponentParameter/readonly//False/False/Application class
+# @param dropclass Application Class/dlg.apps.scp.ScpApp/String/ComponentParameter/readonly//False/False/Application class
+# @param input_parser Input Parser/pickle/Select/ApplicationArgument/readwrite/raw,pickle,eval,npy,path,dataurl/False/False/Input port parsing technique
+# @param output_parser Output Parser/pickle/Select/ApplicationArgument/readwrite/raw,pickle,eval,npy,path,dataurl/False/False/Output port parsing technique
 # @param execution_time Execution Time/5/Float/ComponentParameter/readonly//False/False/Estimated execution time
 # @param num_cpus No. of CPUs/1/Integer/ComponentParameter/readonly//False/False/Number of cores used
 # @param group_start Group start/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the start of a group?
 # @param input_error_threshold "Input error rate (%)"/0/Integer/ComponentParameter/readwrite//False/False/the allowed failure rate of the inputs (in percent), before this component goes to ERROR state and is not executed
 # @param n_tries Number of tries/1/Integer/ComponentParameter/readwrite//False/False/Specifies the number of times the 'run' method will be executed before finally giving up
 # @param remoteUser Remote User//String/ApplicationArgument/readwrite//False/False/Remote user address
 # @param pkeyPath Private Key Path//String/ApplicationArgument/readwrite//False/False/Private key path
@@ -106,15 +108,14 @@
     pkeyPath = dlg_string_param("pkeyPath", None)
     timeout = dlg_float_param("timeout", None)
 
     def initialize(self, **kwargs):
         BarrierAppDROP.initialize(self, **kwargs)
 
     def run(self):
-
         # Check inputs/outputs are of a valid type
         for i in self.inputs + self.outputs:
             # The current only way to check if we are handling a FileDROP
             # or a DirectoryContainer is by checking if they have a `path`
             # attribute. Calling `isinstance(i, (FileDROP, DirectoryContainer))`
             # doesn't work because the input/output might be a proxy object
             # that fails the test
```

### Comparing `daliuge-engine-2.4.0/dlg/apps/simple.py` & `daliuge-engine-3.0.0/dlg/apps/simple.py`

 * *Files 25% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 ##
 # @brief PythonApp
 # @details A placeholder APP to aid construction of new applications.
 # This is mainly useful (and used) when starting a new workflow from scratch.
 # @par EAGLE_START
 # @param category PythonApp
 # @param tag template
-# @param appclass Application Class//String/ComponentParameter/readonly//False/False/Application class
+# @param dropclass Application Class/PythonApp/String/ComponentParameter/readonly//False/False/Application class
 # @param num_cpus No. of CPUs/1/Integer/ComponentParameter/readonly//False/False/Number of cores used
 # @param execution_time Execution Time/5/Float/ComponentParameter/readonly//False/False/Estimated execution time
 # @param group_start Group start/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the start of a group?
 # @par EAGLE_END
 class PythonApp(BarrierAppDROP):
     """A placeholder BarrierAppDrop that just aids the generation of the palette component"""
 
@@ -91,58 +91,71 @@
 # @brief SleepApp
 # @details A simple APP that sleeps the specified amount of time (0 by default).
 # This is mainly useful (and used) to test graph translation and structure
 # without executing real algorithms. Very useful for debugging.
 # @par EAGLE_START
 # @param category PythonApp
 # @param tag daliuge
-# @param sleepTime Sleep Time/5/Integer/ApplicationArgument/readwrite//False/False/The number of seconds to sleep
-# @param appclass Application Class/dlg.apps.simple.SleepApp/String/ComponentParameter/readonly//False/False/Application class
-# @param execution_time Execution Time/5/Float/ComponentParameter/readonly//False/False/Estimated execution time
-# @param num_cpus No. of CPUs/1/Integer/ComponentParameter/readonly//False/False/Number of cores used
-# @param group_start Group start/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the start of a group?
+# @param sleep_time sleep_time/5/Integer/ApplicationArgument/readwrite//False/False/The number of seconds to sleep
+# @param dropclass dropclass/dlg.apps.simple.SleepApp/String/ComponentParameter/readonly//False/False/Application class
+# @param execution_time execution_time/5/Float/ComponentParameter/readonly//False/False/Estimated execution time
+# @param num_cpus num_cpus/1/Integer/ComponentParameter/readonly//False/False/Number of cores used
+# @param group_start group_start/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the start of a group?
 # @par EAGLE_END
 class SleepApp(BarrierAppDROP):
     """A BarrierAppDrop that sleeps the specified amount of time (0 by default)"""
 
     component_meta = dlg_component(
         "SleepApp",
         "Sleep App.",
         [dlg_batch_input("binary/*", [])],
         [dlg_batch_output("binary/*", [])],
         [dlg_streaming_input("binary/*")],
     )
-
-    sleepTime = dlg_float_param("sleep time", 0)
+    pname = "sleep_time"
+    sleep_time = dlg_float_param(pname, 0)
 
     def initialize(self, **kwargs):
         super(SleepApp, self).initialize(**kwargs)
 
     def run(self):
-        time.sleep(self.sleepTime)
+        if self.sleep_time is None:
+            if len(self.inputs) > 0:
+                for inp in self.inputs:
+                    if inp.name == self.pname:
+                        self.sleep_time = pickle.loads(
+                            droputils.allDropContents(inp)
+                        )
+        try:
+            time.sleep(self.sleep_time)
+        except (TypeError, ValueError):
+            self.sleep_time = 0
+            time.sleep(self.sleep_time)
+        logger.debug("%s slept for %s s", self.name, self.sleep_time)
 
 
 ##
 # @brief CopyApp
 # @details A simple APP that copies its inputs into its outputs.
 # All inputs are copied into all outputs in the order they were declared in
 # the graph. If an input is a container (e.g. a directory) it copies the
 # content recursively.
 # @par EAGLE_START
 # @param category PythonApp
 # @param tag daliuge
-# @param appclass Application Class/dlg.apps.simple.CopyApp/String/ComponentParameter/readonly//False/False/Application class
 # @param bufsize buffer size/65536/Integer/ApplicationArgument/readwrite//False/False/Buffer size
-# @param execution_time Execution Time/5/Float/ComponentParameter/readonly//False/False/Estimated execution time
-# @param num_cpus No. of CPUs/1/Integer/ComponentParameter/readonly//False/False/Number of cores used
-# @param group_start Group start/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the start of a group?
-# @param input_error_threshold "Input error rate (%)"/0/Integer/ComponentParameter/readwrite//False/False/the allowed failure rate of the inputs (in percent), before this component goes to ERROR state and is not executed
+# @param dropclass dropclass/dlg.apps.simple.CopyApp/String/ComponentParameter/readonly//False/False/Application class
+# @param execution_time execution_time/5/Float/ComponentParameter/readonly//False/False/Estimated execution time
+# @param num_cpus num_cpus/1/Integer/ComponentParameter/readonly//False/False/Number of cores used
+# @param group_start group_start/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the start of a group?
 # @param n_tries Number of tries/1/Integer/ComponentParameter/readwrite//False/False/Specifies the number of times the 'run' method will be executed before finally giving up
-# @param dummy Dummy//Object/InputPort/readwrite//False/False/Dummy input port
-# @param dummy Dummy//Object/OutputPort/readwrite//False/False/Dummy output port
+# @param dummy_in dummy//Object/InputPort/readwrite//False/False/Dummy input port
+# @param dummy_out dummy//Object/OutputPort/readwrite//False/False/Dummy output port
+# @param input_parser Input Parser/pickle/Select/ApplicationArgument/readwrite/raw,pickle,eval,npy,path,dataurl/False/False/Input port parsing technique
+# @param output_parser Output Parser/pickle/Select/ApplicationArgument/readwrite/raw,pickle,eval,npy,path,dataurl/False/False/Output port parsing technique
 # @par EAGLE_END
 class CopyApp(BarrierAppDROP):
     """
     A BarrierAppDrop that copies its inputs into its outputs.
     All inputs are copied into all outputs in the order they were declared in
     the graph.
     """
@@ -187,21 +200,21 @@
 
 
 ##
 # @brief SleepAndCopyApp
 # @par EAGLE_START
 # @param category PythonApp
 # @param tag daliuge
-# @param sleepTime Sleep Time/5/Integer/ApplicationArgument/readwrite//False/False/The number of seconds to sleep
-# @param appclass Application Class/dlg.apps.simple.SleepAndCopyApp/String/ComponentParameter/readonly//False/False/Application class
-# @param execution_time Execution Time/5/Float/ComponentParameter/readonly//False/False/Estimated execution time
-# @param num_cpus No. of CPUs/1/Integer/ComponentParameter/readonly//False/False/Number of cores used
-# @param group_start Group start/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the start of a group?
-# @param input_error_threshold "Input error rate (%)"/0/Integer/ComponentParameter/readwrite//False/False/the allowed failure rate of the inputs (in percent), before this component goes to ERROR state and is not executed
-# @param n_tries Number of tries/1/Integer/ComponentParameter/readwrite//False/False/Specifies the number of times the 'run' method will be executed before finally giving up
+# @param sleep_time sleep_time/5/Integer/ApplicationArgument/readwrite//False/False/The number of seconds to sleep
+# @param input_parser Input Parser/pickle/Select/ApplicationArgument/readwrite/raw,pickle,eval,npy,path,dataurl/False/False/Input port parsing technique
+# @param output_parser Output Parser/pickle/Select/ApplicationArgument/readwrite/raw,pickle,eval,npy,path,dataurl/False/False/Output port parsing technique
+# @param dropclass dropclass/dlg.apps.simple.SleepAndCopyApp/String/ComponentParameter/readonly//False/False/Application class
+# @param execution_time execution_time/5/Float/ComponentParameter/readonly//False/False/Estimated execution time
+# @param num_cpus num_cpus/1/Integer/ComponentParameter/readonly//False/False/Number of cores used
+# @param group_start group_start/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the start of a group?
 # @par EAGLE_END
 class SleepAndCopyApp(SleepApp, CopyApp):
     """A combination of the SleepApp and the CopyApp. It sleeps, then copies"""
 
     def run(self):
         SleepApp.run(self)
         CopyApp.run(self)
@@ -212,25 +225,25 @@
 # @details A testing APP that does not take any input and produces a random array of
 # type int64, if integer is set to True, else of type float64.
 # size indicates the number of elements ranging between the values low and high.
 # The resulting array will be send to all connected output apps.
 # @par EAGLE_START
 # @param category PythonApp
 # @param tag daliuge
-# @param size Size/100/Integer/ApplicationArgument/readwrite//False/False/The size of the array
-# @param integer Integer/True/Boolean/ApplicationArgument/readwrite//False/False/Generate integer array?
-# @param low Low/0/Float/ApplicationArgument/readwrite//False/False/Low value of range in array [inclusive]
-# @param high High/1/Float/ApplicationArgument/readwrite//False/False/High value of range of array [exclusive]
-# @param appclass Application class/dlg.apps.simple.RandomArrayApp/String/ComponentParameter/readonly//False/False/Application class
-# @param execution_time Execution Time/5/Float/ComponentParameter/readonly//False/False/Estimated execution time
-# @param num_cpus No. of CPUs/1/Integer/ComponentParameter/readonly//False/False/Number of cores used
-# @param group_start Group start/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the start of a group?
-# @param input_error_threshold "Input error rate (%)"/0/Integer/ComponentParameter/readwrite//False/False/the allowed failure rate of the inputs (in percent), before this component goes to ERROR state and is not executed
-# @param n_tries Number of tries/1/Integer/ComponentParameter/readwrite//False/False/Specifies the number of times the 'run' method will be executed before finally giving up
-# @param array Array//Object.Array/OutputPort/readwrite//False/False/Port carrying the averaged array
+# @param size size/100/Integer/ApplicationArgument/readwrite//False/False/The size of the array
+# @param low low/0/Float/ApplicationArgument/readwrite//False/False/Low value of range in array [inclusive]
+# @param high high/1/Float/ApplicationArgument/readwrite//False/False/High value of range of array [exclusive]
+# @param integer integer/True/Boolean/ApplicationArgument/readwrite//False/False/Generate integer array?
+# @param dropclass dropclass/dlg.apps.simple.RandomArrayApp/String/ComponentParameter/readonly//False/False/Application class
+# @param input_parser Input Parser/pickle/Select/ApplicationArgument/readwrite/raw,pickle,eval,npy,path,dataurl/False/False/Input port parsing technique
+# @param output_parser Output Parser/pickle/Select/ApplicationArgument/readwrite/raw,pickle,eval,npy,path,dataurl/False/False/Output port parsing technique
+# @param execution_time execution_time/5/Float/ComponentParameter/readonly//False/False/Estimated execution time
+# @param num_cpus num_cpus/1/Integer/ComponentParameter/readonly//False/False/Number of cores used
+# @param group_start group_start/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the start of a group?
+# @param array array//Object.Array/OutputPort/readwrite//False/False/Port carrying the averaged array
 # @par EAGLE_END
 class RandomArrayApp(BarrierAppDROP):
     """
     A BarrierAppDrop that generates an array of random numbers. It does
     not require any inputs and writes the generated array to all of its
     outputs.
 
@@ -298,23 +311,23 @@
 # @details A testing APP that takes multiple numpy arrays on input and calculates
 # the mean or the median, depending on the value provided in the method parameter.
 # Users can add as many producers to the input array port as required and the resulting array
 # will also be send to all connected output apps.
 # @par EAGLE_START
 # @param category PythonApp
 # @param tag daliuge
-# @param method Method/mean/Select/ApplicationArgument/readwrite/mean,median/False/False/The method used for averaging
-# @param appclass Application Class/dlg.apps.simple.AverageArraysApp/String/ComponentParameter/readonly//False/False/Application class
-# @param execution_time Execution Time/5/Float/ComponentParameter/readonly//False/False/Estimated execution time
-# @param num_cpus No. of CPUs/1/Integer/ComponentParameter/readonly//False/False/Number of cores used
-# @param group_start Group start/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the start of a group?
-# @param input_error_threshold "Input error rate (%)"/0/Integer/ComponentParameter/readwrite//False/False/the allowed failure rate of the inputs (in percent), before this component goes to ERROR state and is not executed
-# @param n_tries Number of tries/1/Integer/ComponentParameter/readwrite//False/False/Specifies the number of times the 'run' method will be executed before finally giving up
-# @param array Array//Object.Array/InputPort/readwrite//False/False/Port for the input array(s)
-# @param array Array//Object.Array/OutputPort/readwrite//False/False/Port carrying the averaged array
+# @param method method/mean/Select/ApplicationArgument/readwrite/mean,median/False/False/The method used for averaging
+# @param dropclass dropclass/dlg.apps.simple.AverageArraysApp/String/ComponentParameter/readonly//False/False/Application class
+# @param input_parser Input Parser/pickle/Select/ApplicationArgument/readwrite/raw,pickle,eval,npy,path,dataurl/False/False/Input port parsing technique
+# @param output_parser Output Parser/pickle/Select/ApplicationArgument/readwrite/raw,pickle,eval,npy,path,dataurl/False/False/Output port parsing technique
+# @param execution_time execution_time/5/Float/ComponentParameter/readonly//False/False/Estimated execution time
+# @param num_cpus num_cpus/1/Integer/ComponentParameter/readonly//False/False/Number of cores used
+# @param group_start group_start/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the start of a group?
+# @param array_in Array//Object.Array/InputPort/readwrite//False/False/Port for the input array(s)
+# @param array_out Array//Object.Array/OutputPort/readwrite//False/False/Port carrying the averaged array
 # @par EAGLE_END
 class AverageArraysApp(BarrierAppDROP):
     """
     A BarrierAppDrop that averages arrays received on input. It requires
     multiple inputs and writes the generated average vector to all of its
     outputs.
     The input arrays are assumed to have the same number of elements and
@@ -387,30 +400,69 @@
 
     def averageArray(self):
         method_to_call = getattr(np, self.method)
         return method_to_call(self.marray, axis=0)
 
 
 ##
+# @brief GenericGatherApp
+# @details App that reads all its inputs and simply writes them in
+# concatenated to all its outputs. This can be used stand-alone or
+# as part of a Gather. It does not do anything to the data, just
+# passing it on.
+#
+# @par EAGLE_START
+# @param category PythonApp
+# @param construct Gather
+# @param tag daliuge
+# @param num_of_inputs num_of_inputs/4/Integer/ConstructParameter/readwrite//False/False/The Gather “width”, stating how many inputs each Gather instance will handle
+# @param dropclass dropclass/dlg.apps.simple.GenericGatherApp/String/ComponentParameter/readonly//False/False/Application class
+# @param input_parser Input Parser/pickle/Select/ApplicationArgument/readwrite/raw,pickle,eval,npy,path,dataurl/False/False/Input port parsing technique
+# @param output_parser Output Parser/pickle/Select/ApplicationArgument/readwrite/raw,pickle,eval,npy,path,dataurl/False/False/Output port parsing technique
+# @param execution_time execution_time/5/Float/ComponentParameter/readonly//False/False/Estimated execution time
+# @param num_cpus num_cpus/1/Integer/ComponentParameter/readonly//False/False/Number of cores used
+# @param group_start group_start/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the start of a group?
+# @param input input//Object/InputPort/readwrite//False/False/0-base placeholder port for inputs
+# @param output output//Object/OutputPort/readwrite//False/False/Placeholder port for outputs
+# @par EAGLE_END
+class GenericGatherApp(BarrierAppDROP):
+    def readWriteData(self):
+        inputs = self.inputs
+        outputs = self.outputs
+        total_len = 0
+        for input in inputs:
+            total_len += input.len
+        for output in outputs:
+            output.len = total_len
+            for input in inputs:
+                d = droputils.allDropContents(input)
+                output.write(d)
+
+    def run(self):
+        self.readWriteData()
+
+
+##
 # @brief GenericNpyGatherApp
 # @details A BarrierAppDrop that combines one or more inputs using cummulative operations.
 # @par EAGLE_START
 # @param category PythonApp
 # @param construct Gather
 # @param tag daliuge
-# @param appclass Application Class/dlg.apps.simple.GenericNpyGatherApp/String/ComponentParameter/readonly//False/False/Application class
-# @param execution_time Execution Time/5/Float/ComponentParameter/readonly//False/False/Estimated execution time
-# @param num_cpus No. of CPUs/1/Integer/ComponentParameter/readonly//False/False/Number of cores used
-# @param group_start Group start/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the start of a group?
-# @param input_error_threshold "Input error rate (%)"/0/Integer/ComponentParameter/readwrite//False/False/the allowed failure rate of the inputs (in percent), before this component goes to ERROR state and is not executed
-# @param n_tries Number of tries/1/Integer/ComponentParameter/readwrite//False/False/Specifies the number of times the 'run' method will be executed before finally giving up
-# @param function Function/sum/Select/ApplicationArgument/readwrite/sum,prod,min,max,add,multiply,maximum,minimum/False/False/The function used for gathering
-# @param reduce_axes "Reduce Axes"/None/String/ApplicationArgument/readonly//False/False/The ndarray axes to reduce, None reduces all axes for sum, prod, max, min functions
-# @param array Array//Object.Array/InputPort/readwrite//False/False/Port for the input array(s)
-# @param array Array//Object.Array/OutputPort/readwrite//False/False/Port carrying the reduced array
+# @param num_of_inputs num_of_inputs/4/Integer/ConstructParameter/readwrite//False/False/The Gather “width”, stating how many inputs each Gather instance will handle
+# @param function function/sum/Select/ApplicationArgument/readwrite/sum,prod,min,max,add,multiply,maximum,minimum/False/False/The function used for gathering
+# @param reduce_axes reduce_axes/None/String/ApplicationArgument/readonly//False/False/The ndarray axes to reduce, None reduces all axes for sum, prod, max, min functions
+# @param dropclass dropclass/dlg.apps.simple.GenericNpyGatherApp/String/ComponentParameter/readonly//False/False/Application class
+# @param input_parser Input Parser/pickle/Select/ApplicationArgument/readwrite/raw,pickle,eval,npy,path,dataurl/False/False/Input port parsing technique
+# @param output_parser Output Parser/pickle/Select/ApplicationArgument/readwrite/raw,pickle,eval,npy,path,dataurl/False/False/Output port parsing technique
+# @param execution_time execution_time/5/Float/ComponentParameter/readonly//False/False/Estimated execution time
+# @param num_cpus num_cpus/1/Integer/ComponentParameter/readonly//False/False/Number of cores used
+# @param group_start group_start/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the start of a group?
+# @param array_in array_in//Object.Array/InputPort/readwrite//False/False/Port for the input array(s)
+# @param array_out array_out//Object.Array/OutputPort/readwrite//False/False/Port carrying the reduced array
 # @par EAGLE_END
 class GenericNpyGatherApp(BarrierAppDROP):
     """
     A BarrierAppDrop that reduces then gathers one or more inputs using cummulative operations.
     function:  string <'sum'|'prod'|'min'|'max'|'add'|'multiply'|'maximum'|'minimum'>.
 
     """
@@ -469,48 +521,56 @@
         result: Optional[Number] = None
         reduce = getattr(np, f"{self.function}")
         gather = getattr(np, f"{self.functions[self.function]}")
         for input in self.inputs:
             data = droputils.load_numpy(input)
             # skip gather for the first input
             result = (
-                reduce(data, axis=self.reduce_axes)
+                reduce(data, axis=self.reduce_axes, allow_pickle=True)
                 if result is None
-                else gather(result, reduce(data, axis=self.reduce_axes))
+                else gather(
+                    result,
+                    reduce(data, axis=self.reduce_axes, allow_pickle=True),
+                    allow_pickle=True,
+                )
             )
         return result
 
     def gather_inputs(self):
         """gathers each input drop interpreted as an npy drop"""
         result: Optional[Number] = None
         gather = getattr(np, f"{self.function}")
         for input in self.inputs:
             data = droputils.load_numpy(input)
             # assign instead of gather for the first input
-            result = data if result is None else gather(result, data)
+            result = (
+                data
+                if result is None
+                else gather(result, data, allow_pickle=True)
+            )
         return result
 
 
 ##
 # @brief HelloWorldApp
 # @details A simple APP that implements the standard Hello World in DALiuGE.
 # It allows to change 'World' with some other string and it also permits
 # to connect the single output port to multiple sinks, which will all receive
 # the same message. App does not require any input.
 # @par EAGLE_START
 # @param category PythonApp
 # @param tag daliuge
-# @param greet Greet/World/String/ApplicationArgument/readwrite//False/False/What appears after 'Hello '
-# @param appclass Application Class/dlg.apps.simple.HelloWorldApp/String/ComponentParameter/readonly//False/False/Application class
-# @param execution_time Execution Time/5/Float/ComponentParameter/readonly//False/False/Estimated execution time
-# @param num_cpus No. of CPUs/1/Integer/ComponentParameter/readonly//False/False/Number of cores used
-# @param group_start Group start/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the start of a group?
-# @param input_error_threshold "Input error rate (%)"/0/Integer/ComponentParameter/readwrite//False/False/the allowed failure rate of the inputs (in percent), before this component goes to ERROR state and is not executed
-# @param n_tries Number of tries/1/Integer/ComponentParameter/readwrite//False/False/Specifies the number of times the 'run' method will be executed before finally giving up
-# @param hello Hello/"world"/String/OutputPort/readwrite//False/False/The port carrying the message produced by the app.
+# @param greet greet/World/String/ApplicationArgument/readwrite//False/False/What appears after 'Hello '
+# @param dropclass dropclass/dlg.apps.simple.HelloWorldApp/String/ComponentParameter/readonly//False/False/Application class
+# @param execution_time execution_time/5/Float/ComponentParameter/readonly//False/False/Estimated execution time
+# @param input_parser Input Parser/pickle/Select/ApplicationArgument/readwrite/raw,pickle,eval,npy,path,dataurl/False/False/Input port parsing technique
+# @param output_parser Output Parser/pickle/Select/ApplicationArgument/readwrite/raw,pickle,eval,npy,path,dataurl/False/False/Output port parsing technique
+# @param num_cpus num_cpus/1/Integer/ComponentParameter/readonly//False/False/Number of cores used
+# @param group_start group_start/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the start of a group?
+# @param hello hello/"world"/Object/OutputPort/readwrite//False/False/The port carrying the message produced by the app.
 # @par EAGLE_END
 class HelloWorldApp(BarrierAppDROP):
     """
     An App that writes 'Hello World!' or 'Hello <greet>!' to all of
     its outputs.
 
     Keywords:
@@ -558,22 +618,22 @@
 ##
 # @brief UrlRetrieveApp
 # @details A simple APP that retrieves the content of a URL and writes
 # it to all outputs.
 # @par EAGLE_START
 # @param category PythonApp
 # @param tag daliuge
-# @param url URL/"https://eagle.icrar.org"/String/ApplicationArgument/readwrite//False/False/The URL to retrieve
-# @param appclass Application Class/dlg.apps.simple.UrlRetrieveApp/String/ComponentParameter/readonly//False/False/Application class
-# @param execution_time Execution Time/5/Float/ComponentParameter/readonly//False/False/Estimated execution time
-# @param num_cpus No. of CPUs/1/Integer/ComponentParameter/readonly//False/False/Number of cores used
-# @param group_start Group start/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the start of a group?
-# @param input_error_threshold "Input error rate (%)"/0/Integer/ComponentParameter/readwrite//False/False/the allowed failure rate of the inputs (in percent), before this component goes to ERROR state and is not executed
-# @param n_tries Number of tries/1/Integer/ComponentParameter/readwrite//False/False/Specifies the number of times the 'run' method will be executed before finally giving up
-# @param content Content//String/OutputPort/readwrite//False/False/The port carrying the content read from the URL
+# @param url url/"https://eagle.icrar.org"/String/ApplicationArgument/readwrite//False/False/The URL to retrieve
+# @param dropclass dropclass/dlg.apps.simple.UrlRetrieveApp/String/ComponentParameter/readonly//False/False/Application class
+# @param execution_time execution_time/5/Float/ComponentParameter/readonly//False/False/Estimated execution time
+# @param input_parser Input Parser/pickle/Select/ApplicationArgument/readwrite/raw,pickle,eval,npy,path,dataurl/False/False/Input port parsing technique
+# @param output_parser Output Parser/pickle/Select/ApplicationArgument/readwrite/raw,pickle,eval,npy,path,dataurl/False/False/Output port parsing technique
+# @param num_cpus num_cpus/1/Integer/ComponentParameter/readonly//False/False/Number of cores used
+# @param group_start group_start/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the start of a group?
+# @param content content//String/OutputPort/readwrite//False/False/The port carrying the content read from the URL
 # @par EAGLE_END
 class UrlRetrieveApp(BarrierAppDROP):
     """
     An App that retrieves the content of a URL
 
     Keywords:
     URL:   string, URL to retrieve.
@@ -615,23 +675,24 @@
 # axis is of length len(outputs). The modulo remainder of the length of the original array and
 # the number of outputs will be distributed across the first len(outputs)-1 elements of the
 # resulting array.
 # @par EAGLE_START
 # @param category PythonApp
 # @param construct Scatter
 # @param tag daliuge
-# @param num_of_copies Scatter dimension/4/Integer/ComponentParameter/readwrite//False/False/Specifies the number of replications of the content of the scatter construct
-# @param group_start Group start/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the start of a group?
-# @param input_error_threshold "Input error rate (%)"/0/Integer/ComponentParameter/readwrite//False/False/the allowed failure rate of the inputs (in percent), before this component goes to ERROR state and is not executed
-# @param n_tries Number of tries/1/Integer/ComponentParameter/readwrite//False/False/Specifies the number of times the 'run' method will be executed before finally giving up
-# @param appclass Application Class/dlg.apps.simple.GenericScatterApp/String/ComponentParameter/readonly//False/False/Application class
-# @param execution_time Execution Time/5/Float/ComponentParameter/readonly//False/False/Estimated execution time
-# @param num_cpus No. of CPUs/1/Integer/ComponentParameter/readonly//False/False/Number of cores used
-# @param array Array//Object.Array/OutputPort/readwrite//False/False/Port carrying the reduced array
-# @param array Array//Object.Array/InputPort/readwrite//False/False/A numpy array of arrays, where the first axis is of length <numSplit>
+# @param num_of_copies num_of_copies/4/Integer/ConstructParameter/readwrite//False/False/Specifies the number of replications of the content of the scatter construct
+# @param group_start group_start/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the start of a group?
+# @param n_tries n_tries/1/Integer/ComponentParameter/readwrite//False/False/Specifies the number of times the 'run' method will be executed before finally giving up
+# @param dropclass dropclass/dlg.apps.simple.GenericScatterApp/String/ComponentParameter/readonly//False/False/Application class
+# @param input_parser Input Parser/pickle/Select/ApplicationArgument/readwrite/raw,pickle,eval,npy,path,dataurl/False/False/Input port parsing technique
+# @param output_parser Output Parser/pickle/Select/ApplicationArgument/readwrite/raw,pickle,eval,npy,path,dataurl/False/False/Output port parsing technique
+# @param execution_time execution_time/5/Float/ComponentParameter/readonly//False/False/Estimated execution time
+# @param num_cpus num_cpus/1/Integer/ComponentParameter/readonly//False/False/Number of cores used
+# @param array_in array_in//Object.Array/InputPort/readwrite//False/False/A numpy array of arrays, where the first axis is of length <numSplit>
+# @param array_out array_out//Object.Array/OutputPort/readwrite//False/False/Port carrying the reduced array
 # @par EAGLE_END
 class GenericScatterApp(BarrierAppDROP):
     """
     An APP that splits an object that has a len attribute into <numSplit> parts and
     returns a numpy array of arrays, where the first axis is of length <numSplit>.
     """
 
@@ -677,26 +738,27 @@
 # @details An APP that splits about any axis on any npy format data drop
 # into as many part./run    s as the app has outputs, provided that the initially converted numpy
 # array has enough elements. The return will be a numpy array of arrays, where the first
 # axis is of length len(outputs). The modulo remainder of the length of the original array and
 # the number of outputs will be distributed across the first len(outputs)-1 elements of the
 # resulting array.
 # @par EAGLE_START
-# @param category PythonApp
 # @param construct Scatter
+# @param category PythonApp
 # @param tag daliuge
-# @param group_start Group start/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the start of a group?
-# @param input_error_threshold "Input error rate (%)"/0/Integer/ComponentParameter/readwrite//False/False/the allowed failure rate of the inputs (in percent), before this component goes to ERROR state and is not executed
-# @param n_tries Number of tries/1/Integer/ComponentParameter/readwrite//False/False/Specifies the number of times the 'run' method will be executed before finally giving up
-# @param appclass Application Class/dlg.apps.simple.GenericNpyScatterApp/String/ComponentParameter/readonly//False/False/Application class
-# @param execution_time Execution Time/5/Float/ComponentParameter/readonly//False/False/Estimated execution time
-# @param num_cpus No. of CPUs/1/Integer/ComponentParameter/readonly//False/False/Number of cores used
-# @param scatter_axes Scatter Axes//String/ApplicationArgument/readwrite//False/False/The axes to split input ndarrays on, e.g. [0,0,0], length must match the number of input ports
-# @param array Object.Array//Object.Array/InputPort/readwrite//False/False/A numpy array of arrays
-# @param array Array//Object.Array/OutputPort/readwrite//False/False/Port carrying the reduced array
+# @param num_of_copies num_of_copies/4/Integer/ConstructParameter/readwrite//False/False/Specifies the number of replications of the content of the scatter construct
+# @param scatter_axes scatter_axes//String/ApplicationArgument/readwrite//False/False/The axes to split input ndarrays on, e.g. [0,0,0], length must match the number of input ports
+# @param group_start group_start/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the start of a group?
+# @param dropclass dropclass/dlg.apps.simple.GenericNpyScatterApp/String/ComponentParameter/readonly//False/False/Application class
+# @param input_parser Input Parser/pickle/Select/ApplicationArgument/readwrite/raw,pickle,eval,npy,path,dataurl/False/False/Input port parsing technique
+# @param output_parser Output Parser/pickle/Select/ApplicationArgument/readwrite/raw,pickle,eval,npy,path,dataurl/False/False/Output port parsing technique
+# @param execution_time execution_time/5/Float/ComponentParameter/readonly//False/False/Estimated execution time
+# @param num_cpus num_cpus/1/Integer/ComponentParameter/readonly//False/False/Number of cores used
+# @param array_in array_in//Object.Array/InputPort/readwrite//False/False/A numpy array of arrays
+# @param array_out array_out//Object.Array/OutputPort/readwrite//False/False/Port carrying the reduced array
 # @par EAGLE_END
 class GenericNpyScatterApp(BarrierAppDROP):
     """
     An APP that splits an object that has a len attribute into <num_of_copies> parts and
     returns a numpy array of arrays.
     """
 
@@ -760,20 +822,24 @@
 # @brief PickOne
 # @details App that picks the first element of an input list, passes that
 # to all outputs, except the first one. The first output is used to pass
 # the remaining array on. This app is useful for a loop.
 #
 # @par EAGLE_START
 # @param category PythonApp
-# @param appclass Application Class/dlg_example_cmpts.apps.PickOne/String/ComponentParameter/readonly//False/False/Import path for application class
-# @param execution_time Execution Time/5/Float/ComponentParameter/readonly//False/False/Estimated execution time # noqa: E501
-# @param num_cpus No. of CPUs/1/Integer/ComponentParameter/readonly//False/False/Number of cores used # noqa: E501
-# @param rest_array rest_array//Object.array/InputPort/readwrite//False/FalseList of elements
+# @param tag daliuge
+# @param dropclass dropclass/dlg.apps.simple.PickOne/String/ComponentParameter/readonly//False/False/Application class
+# @param input_parser Input Parser/pickle/Select/ApplicationArgument/readwrite/raw,pickle,eval,npy,path,dataurl/False/False/Input port parsing technique
+# @param output_parser Output Parser/pickle/Select/ApplicationArgument/readwrite/raw,pickle,eval,npy,path,dataurl/False/False/Output port parsing technique
+# @param execution_time execution_time/5/Float/ComponentParameter/readonly//False/False/Estimated execution time
+# @param num_cpus num_cpus/1/Integer/ComponentParameter/readonly//False/False/Number of cores used
+# @param group_start group_start/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the start of a group?
+# @param rest_array_in rest_array//Object.array/InputPort/readwrite//False/FalseList of elements
+# @param rest_array_out rest_array//Object.array/OutputPort/readwrite//False/False/Port carrying the rest array
 # @param element element//Object.element/OutputPort/readwrite//False/False/Port carrying the first element of input array
-# @param rest_array rest_array//Object.array/OutputPort/readwrite//False/False/Port carrying the rest array
 # @par EAGLE_END
 class PickOne(BarrierAppDROP):
     """
     Simple app picking one element at a time. Good for Loops.
     """
 
     def initialize(self, **kwargs):
@@ -821,22 +887,22 @@
 # @details A testing APP that appends a random integer to a list num times.
 # This is a CPU intensive operation and can thus be used to provide a test for application threading
 # since this operation will not yield.
 # The resulting array will be sent to all connected output apps.
 # @par EAGLE_START
 # @param category PythonApp
 # @param tag daliuge
-# @param size Size/100/Integer/ApplicationArgument/readwrite//False/False/the size of the array
-# @param appclass Application Class/dlg.apps.simple.ListAppendThrashingApp/String/ComponentParameter/readonly//False/False/Application class
-# @param execution_time Execution Time/5/Float/ComponentParameter/readonly//False/False/Estimated execution time
-# @param num_cpus No. of CPUs/1/Integer/ComponentParameter/readonly//False/False/Number of cores used
-# @param group_start Group start/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the start of a group?
-# @param input_error_threshold "Input error rate (%)"/0/Integer/ComponentParameter/readwrite//False/False/the allowed failure rate of the inputs (in percent), before this component goes to ERROR state and is not executed
-# @param n_tries Number of tries/1/Integer/ComponentParameter/readwrite//False/False/Specifies the number of times the 'run' method will be executed before finally giving up
-# @param array Array//Object.Array/OutputPort/readwrite//False/False/Port carrying the random array.
+# @param size size/100/Integer/ApplicationArgument/readwrite//False/False/the size of the array
+# @param dropclass dropclass/dlg.apps.simple.ListAppendThrashingApp/String/ComponentParameter/readonly//False/False/Application class
+# @param input_parser Input Parser/pickle/Select/ApplicationArgument/readwrite/raw,pickle,eval,npy,path,dataurl/False/False/Input port parsing technique
+# @param output_parser Output Parser/pickle/Select/ApplicationArgument/readwrite/raw,pickle,eval,npy,path,dataurl/False/False/Output port parsing technique
+# @param execution_time execution_time/5/Float/ComponentParameter/readonly//False/False/Estimated execution time
+# @param num_cpus num_cpus/1/Integer/ComponentParameter/readonly//False/False/Number of cores used
+# @param group_start group_start/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the start of a group?
+# @param array array//Object.Array/OutputPort/readwrite//False/False/Port carrying the random array.
 # @par EAGLE_END
 class ListAppendThrashingApp(BarrierAppDROP):
     """
     A BarrierAppDrop that appends random integers to a list N times. It does
     not require any inputs and writes the generated array to all of its
     outputs.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `daliuge-engine-2.4.0/dlg/apps/socket_listener.py` & `daliuge-engine-3.0.0/dlg/apps/socket_listener.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 # This application expects no input DROPs, and therefore raises an
 # exception whenever one is added. On the output side, one or more outputs
 # can be specified with the restriction that they are not ContainerDROPs
 # so data can be written into them through the framework.
 # @par EAGLE_START
 # @param category PythonApp
 # @param tag daliuge
-# @param appclass Application Class/dlg.apps.socket_listener.SocketListener/String/ComponentParameter/readonly//False/False/Application class
+# @param dropclass Application Class/dlg.apps.socket_listener.SocketListener/String/ComponentParameter/readonly//False/False/Application class
 # @param execution_time Execution Time/5/Float/ComponentParameter/readonly//False/False/Estimated execution time
 # @param num_cpus No. of CPUs/1/Integer/ComponentParameter/readonly//False/False/Number of cores used
 # @param group_start Group start/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the start of a group?
 # @param input_error_threshold "Input error rate (%)"/0/Integer/ComponentParameter/readwrite//False/False/the allowed failure rate of the inputs (in percent), before this component goes to ERROR state and is not executed
 # @param n_tries Number of tries/1/Integer/ComponentParameter/readwrite//False/False/Specifies the number of times the 'run' method will be executed before finally giving up
 # @param host Host/localhost/String/ApplicationArgument/readwrite//False/False/Host address
 # @param port Port/1111/Integer/ApplicationArgument/readwrite//False/False/Host port
```

### Comparing `daliuge-engine-2.4.0/dlg/dask_emulation.py` & `daliuge-engine-3.0.0/dlg/dask_emulation.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,19 +25,17 @@
 import contextlib
 import logging
 import pickle
 import socket
 import struct
 import time
 
-from dlg.common import CategoryType, DropType
-
 from . import utils, droputils
 from .apps import pyfunc
-from .common import dropdict, Categories
+from .common import dropdict
 from .ddap_protocol import DROPStates
 from .apps.app_base import BarrierAppDROP
 from .exceptions import InvalidDropException
 
 logger = logging.getLogger(__name__)
 
 
@@ -52,15 +50,19 @@
         if self.port is None:
             raise InvalidDropException(self, "Missing port parameter")
 
     def run(self):
         def read_result(x):
             if x.status == DROPStates.ERROR:
                 return "Error"
-            return pickle.loads(droputils.allDropContents(x))
+            try:
+                content = pickle.loads(droputils.allDropContents(x))
+            except EOFError:
+                content = None
+            return content
 
         results = map(read_result, self.inputs)  # @UndefinedVariable
         results = list(results)
         if len(self.inputs) == 1:
             results = results[0]
         results = pickle.dumps(results)
 
@@ -72,15 +74,14 @@
         with contextlib.closing(client):
             client = client.makefile("wb")
             client.write(struct.pack(">i", len(results)))
             client.write(results)
 
 
 def _get_client(**kwargs):
-
     if "client" in kwargs:
         return kwargs["client"]
 
     from .manager.client import NodeManagerClient
     from .manager import constants
 
     host = kwargs.get("host", "localhost")
@@ -108,22 +109,22 @@
     graph = value.get_graph()
     port = 10000
     # Add one final application that will wait for all results
     # and transmit them back to us
     transmitter_oid = "-1"
     transmitter = dropdict(
         {
-            "type": "app",
+            "categoryType": "Application",
             #            "categoryType": CategoryType.APPLICATION,
-            "app": "dlg.dask_emulation.ResultTransmitter",
-            "appclass": "dlg.dask_emulation.ResultTransmitter",
+            # "Application": "dlg.dask_emulation.ResultTransmitter",
+            "dropclass": "dlg.dask_emulation.ResultTransmitter",
             "oid": transmitter_oid,
+            "uid": transmitter_oid,
             "port": port,
-            "nm": "result transmitter",
-            "text": "result transmitter",
+            "name": "result transmitter",
         }
     )
     for leaf_oid in droputils.get_leaves(graph.values()):
         graph[leaf_oid].addConsumer(transmitter)
     graph[transmitter_oid] = transmitter
 
     graph = list(graph.values())
@@ -194,15 +195,14 @@
         dd = self.dropdict
         dd["oid"] = oid
         visited.add(self)
         graph[oid] = dd
         logger.debug("Appended %r/%s to the Physical Graph", self, oid)
 
     def _to_physical_graph(self, visited, graph):
-
         self._append_to_graph(visited, graph)
 
         dependencies = list(self.inputs)
         if self.producer:
             dependencies.append(self.producer)
         for d in dependencies:
             if isinstance(d, list):
@@ -284,19 +284,18 @@
 
     def __getitem__(self, i):
         return self.drops[i]
 
     def make_dropdict(self):
         return dropdict(
             {
-                "type": "app",
-                "categoryType": CategoryType.APPLICATION,
-                "app": "dlg.dask_emulation._Listifier",
-                "nm": "listifier",
-                "text": "listifier",
+                # "oid": uuid.uuid1(),
+                "categoryType": "Application",
+                "dropclass": "dlg.dask_emulation._Listifier",
+                "name": "listifier",
             }
         )
 
     def __repr__(self):
         return "<_DelayedDrops n=%d>" % (len(self.drops),)
 
 
@@ -311,31 +310,28 @@
             self.fname = f.__name__
         self.fcode, self.fdefaults = pyfunc.serialize_func(f)
         self.original_kwarg_names = []
         self.nout = nout
         logger.debug("Created %r", self)
 
     def make_dropdict(self):
-
         self.kwarg_names = list(self.original_kwarg_names)
         self.kwarg_names.reverse()
         my_dropdict = dropdict(
             {
-                "type": "app",
-                "categoryType": CategoryType.APPLICATION,
-                "app": "dlg.apps.pyfunc.PyFuncApp",
-                "appclass": "dlg.apps.pyfunc.PyFuncApp",
+                # "oid": uuid.uuid1(),
+                "categoryType": "Application",
+                "dropclass": "dlg.apps.pyfunc.PyFuncApp",
                 "func_arg_mapping": {},
             }
         )
         if self.fname is not None:
             simple_fname = self.fname.split(".")[-1]
             my_dropdict["func_name"] = self.fname
-            my_dropdict["nm"] = simple_fname
-            my_dropdict["text"] = simple_fname
+            my_dropdict["name"] = simple_fname
         if self.fcode is not None:
             my_dropdict["func_code"] = utils.b2s(base64.b64encode(self.fcode))
         if self.fdefaults:
             my_dropdict["func_defaults"] = self.fdefaults
         return my_dropdict
 
     def _add_upstream(self, dep):
@@ -348,28 +344,26 @@
                     name,
                     dep.oid,
                     self.fname,
                 )
                 self.dropdict["func_arg_mapping"][name] = dep.oid
 
     def _to_delayed_arg(self, arg):
-
         logger.info("Turning into delayed arg for %r: %r", self, arg)
         if isinstance(arg, _DelayedDrop):
             return arg
 
         # Turn lists/tuples of _DataDrop objects into a _DelayedDrops
         if _is_list_of_delayeds(arg):
             return _DelayedDrops(*arg)
 
         # Plain data gets turned into a _DataDrop
         return _DataDrop(pydata=arg)
 
     def __call__(self, *args, **kwargs):
-
         logger.debug(
             "Delayed function %s called with %d args and %d kwargs",
             self.fname,
             len(args),
             len(kwargs),
         )
         for arg in args:
@@ -402,17 +396,17 @@
             raise ValueError("either producer or pydata must be not None")
         self.pydata = pydata
         logger.debug("Created %r", self)
 
     def make_dropdict(self):
         my_dropdict = dropdict(
             {
-                "type": "data",
-                "categoryType": CategoryType.DATA,
-                "storage": Categories.MEMORY,
+                # "oid": uuid.uuid1(),
+                "categoryType": "Data",
+                "dropclass": "dlg.data.drops.memory.InMemoryDROP",
             }
         )
         if not self.producer:
             my_dropdict["pydata"] = pyfunc.serialize_data(self.pydata)
         return my_dropdict
 
     def __repr__(self):
@@ -452,8 +446,9 @@
         nout = kwargs["nout"]
     elif args:
         nout = args[0]
     else:
         nout = None
     if callable(x):
         return _AppDrop(x, nout=nout)
+        # return x(*args, **kwargs)
     return _DataDrop(pydata=x)
```

### Comparing `daliuge-engine-2.4.0/dlg/data/__init__.py` & `daliuge-engine-3.0.0/dlg/data/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/data/drops/__init__.py` & `daliuge-engine-3.0.0/dlg/data/drops/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/data/drops/container.py` & `daliuge-engine-3.0.0/dlg/data/drops/container.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/data/drops/data_base.py` & `daliuge-engine-3.0.0/dlg/data/drops/data_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from abc import abstractmethod, abstractproperty
 import random
 import os
 import logging
 from typing import Union
 
 from dlg.ddap_protocol import DROPStates
+
 from dlg.drop import AbstractDROP, track_current_drop
 from dlg.data.io import (
     DataIO,
     OpenMode,
     NullIO,
 )
 from dlg.ddap_protocol import (
@@ -50,19 +51,19 @@
     _checksumType = ChecksumTypes.CRC_32
 
 logger = logging.getLogger(__name__)
 
 
 ##
 # @brief Data
-# @details A generic Data drop, whose functionality can be provided by an arbitrary class, as specified in the 'dataclass' component parameter
+# @details A generic Data drop, whose functionality can be provided by an arbitrary class, as specified in the 'dropclass' component parameter. It is not useful without additional development.
 # @par EAGLE_START
 # @param category Data
 # @param tag template
-# @param dataclass Data Class/my.awesome.data.Component/String/ComponentParameter/readonly//False/False/The python class that implements this data component
+# @param dropclass Data Class/my.awesome.data.Component/String/ComponentParameter/readonly//False/False/The python class that implements this data component
 # @param data_volume Data volume/5/Float/ComponentParameter/readwrite//False/False/Estimated size of the data contained in this node
 # @param group_end Group end/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the end of a group?
 # @param streaming Streaming/False/Boolean/ComponentParameter/readwrite//False/False/Specifies whether this data component streams input and output data
 # @param persist Persist/False/Boolean/ComponentParameter/readwrite//False/False/Specifies whether this data component contains data that should not be deleted after execution
 # @param dummy dummy//Object/InputPort/readwrite//False/False/Dummy input port
 # @param dummy dummy//Object/OutputPort/readwrite//False/False/Dummy output port
 # @par EAGLE_END
@@ -404,15 +405,15 @@
 
 ##
 # @brief NULL
 # @details A Drop not storing any data (useful for just passing on events)
 # @par EAGLE_START
 # @param category Memory
 # @param tag daliuge
-# @param data_volume Data volume/0/Float/ComponentParameter/readonly//False/False/This never stores any data
+# @param dropclass dropclass/dlg.data.drops.data_base.NullDROP/String/ComponentParameter/readwrite//False/False/Drop class
 # @param group_end Group end/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the end of a group?
 # @param dummy dummy//Object/InputPort/readwrite//False/False/Dummy input port
 # @param dummy dummy//Object/OutputPort/readwrite//False/False/Dummy output port
 # @par EAGLE_END
 class NullDROP(DataDROP):
     """
     A DROP that doesn't store any data.
```

### Comparing `daliuge-engine-2.4.0/dlg/data/drops/directorycontainer.py` & `daliuge-engine-3.0.0/dlg/data/drops/directorycontainer.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,29 +28,31 @@
 from dlg.data.drops.data_base import PathBasedDrop
 from dlg.data.drops.container import ContainerDROP
 from dlg.exceptions import InvalidDropException, InvalidRelationshipException
 from dlg.meta import dlg_bool_param
 
 logger = logging.getLogger(__name__)
 
+
 ##
 # TODO: This needs some more work
 # @brief Directory
 # @details A ContainerDROP that represents a filesystem directory. It only allows
 # FileDROPs and DirectoryContainers to be added as children. Children
 # can only be added if they are placed directly within the directory
 # represented by this DirectoryContainer.
 # @par EAGLE_START
 # @param category Directory
 # @param tag future
+# @param dropclass dropclass/dlg.data.drops.directorycontainer.DirectoryContainer/String/ComponentParameter/readwrite//False/False/Drop class
 # @param data_volume Data volume/5/Float/ComponentParameter/readwrite//False/False/Estimated size of the data contained in this node
 # @param group_end Group end/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the end of a group?
-# @param check_exists Check path exists/True/Boolean/ComponentParameter/readwrite//False/False/Perform a check to make sure the file path exists before proceeding with the application
-# @param dirname Directory name//String/ComponentParameter/readwrite//False/False/"Directory name/path"
-# @param dummy dummy//String/OutputPort/readwrite//False/False/Dummy output port
+# @param check_exists Check path exists/True/Boolean/ApplicationArgument/readwrite//False/False/Perform a check to make sure the file path exists before proceeding with the application
+# @param dirname Directory name//String/ApplicationArgument/readwrite//False/False/"Directory name/path"
+# @param dummy dummy//Object/OutputPort/readwrite//False/False/Dummy output port
 # @par EAGLE_END
 class DirectoryContainer(PathBasedDrop, ContainerDROP):
     """
     A ContainerDROP that represents a filesystem directory. It only allows
     FileDROPs and DirectoryContainers to be added as children. Children
     can only be added if they are placed directly within the directory
     represented by this DirectoryContainer.
```

### Comparing `daliuge-engine-2.4.0/dlg/data/drops/environmentvar_drop.py` & `daliuge-engine-3.0.0/dlg/data/drops/environmentvar_drop.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,15 +62,16 @@
 
 ##
 # @brief EnvironmentVariables
 # @details A set of environment variables, wholly specified in EAGLE and accessible to all drops.
 # @par EAGLE_START
 # @param category EnvironmentVariables
 # @param tag daliuge
-# @param streaming Streaming/False/Boolean/ComponentParameter/readwrite//False/False/Specifies whether this data component streams input and output data 
+# @param dropclass dropclass/dlg.data.drops.environmentvar_drop.EnvironmentVarDROP/String/ComponentParameter/readwrite//False/False/Drop class
+# @param streaming Streaming/False/Boolean/ComponentParameter/readwrite//False/False/Specifies whether this data component streams input and output data
 # @param persist Persist/False/Boolean/ComponentParameter/readwrite//False/False/Specifies whether this data component contains data that should not be deleted after execution
 # @param dummy dummy//Object/OutputPort/readwrite//False/False/Dummy output port
 # @par EAGLE_END
 class EnvironmentVarDROP(AbstractDROP, KeyValueDROP):
     """
     Drop storing static variables for access by all drops.
     Functions effectively like a globally-available Python dictionary
@@ -81,15 +82,17 @@
         Runs through all parameters, putting each into this drop's variable dict
         """
         super(EnvironmentVarDROP, self).initialize(**kwargs)
         self._variables = dict()
         self._variables.update(_filter_parameters(self.parameters))
 
     def getIO(self):
-        return MemoryIO(io.BytesIO(json.dumps(self._variables).encode("utf-8")))
+        return MemoryIO(
+            io.BytesIO(json.dumps(self._variables).encode("utf-8"))
+        )
 
     def get(self, key):
         """
         Fetches key from internal store if present.
         If not present, attempts to fetch variable from environment
         """
         value = self._variables.get(key)
```

### Comparing `daliuge-engine-2.4.0/dlg/data/drops/file.py` & `daliuge-engine-3.0.0/dlg/data/drops/file.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,19 +35,19 @@
 
 ##
 # @brief File
 # @details A standard file on a filesystem mounted to the deployment machine
 # @par EAGLE_START
 # @param category File
 # @param tag daliuge
-# @param filepath File Path//String/ComponentParameter/readwrite//False/False/File path for this file. In many cases this does not need to be specified. If it has a \/ at the end it will be treated as a directory name and the filename will be generated. If it does not have a \/, the last part will be treated as a filename. If filepath does not start with \/ (relative path) then the session directory will be prepended to make the path absolute.
+# @param filepath File Path//String/ApplicationArgument/readwrite//False/False/File path for this file. In many cases this does not need to be specified. If it has a \/ at the end it will be treated as a directory name and the filename will be generated. If it does not have a \/, the last part will be treated as a filename. If filepath does not start with \/ (relative path) then the session directory will be prepended to make the path absolute.
 # @param check_filepath_exists Check existence/False/Boolean/ComponentParameter/readwrite//False/False/Perform a check to make sure the file path exists before proceeding with the application
+# @param dropclass dropclass/dlg.data.drops.file.FileDROP/String/ComponentParameter/readwrite//False/False/Drop class
 # @param streaming Streaming/False/Boolean/ComponentParameter/readwrite//False/False/Specifies whether this data component streams input and output data
 # @param persist Persist/True/Boolean/ComponentParameter/readwrite//False/False/Specifies whether this data component contains data that should not be deleted after execution
-# @param delete_parent_directory Delete parent/False/Boolean/ComponentParameter/readwrite//False/False/Also delete the parent directory of this file when deleting the file itself
 # @param data_volume Data volume/5/Float/ComponentParameter/readwrite//False/False/Estimated size of the data contained in this node
 # @param group_end Group end/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the end of a group?
 # @param dummy dummy//Object/InputPort/readwrite//False/False/Dummy input port
 # @param dummy dummy//Object/OutputPort/readwrite//False/False/Dummy output port
 # @par EAGLE_END
 class FileDROP(DataDROP, PathBasedDrop):
     """
@@ -144,15 +144,17 @@
 
         self._root = self.dirname
         self._path = (
             os.path.join(self.dirname, self.filename)
             if self.filename
             else self.dirname
         )
-        logger.debug(f"Set path of drop {self._uid}: {self._path}")
+        logger.debug(
+            f"Set path of drop {self._uid}: {self._path} check: {check} {os.path.isfile(self._path)}"
+        )
         if check and not os.path.isfile(self._path):
             raise InvalidDropException(
                 self, "File does not exist or is not a file: %s" % self._path
             )
 
         self._wio = None
```

### Comparing `daliuge-engine-2.4.0/dlg/data/drops/json_drop.py` & `daliuge-engine-3.0.0/dlg/data/drops/json_drop.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/data/drops/memory.py` & `daliuge-engine-3.0.0/dlg/data/drops/memory.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 
 ##
 # @brief Memory
 # @details In-memory storage of intermediate data products
 # @par EAGLE_START
 # @param category Memory
 # @param tag daliuge
+# @param dropclass dropclass/dlg.data.drops.memory.InMemoryDROP/String/ComponentParameter/readwrite//False/False/Drop class
 # @param data_volume Data volume/5/Float/ComponentParameter/readwrite//False/False/Estimated size of the data contained in this node
 # @param group_end Group end/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the end of a group?
 # @param streaming Streaming/False/Boolean/ComponentParameter/readwrite//False/False/Specifies whether this data component streams input and output data
 # @param persist Persist/False/Boolean/ComponentParameter/readwrite//False/False/Specifies whether this data component contains data that should not be deleted after execution
 # @param dummy dummy//Object/InputPort/readwrite//False/False/Dummy input port
 # @param dummy dummy//Object/OutputPort/readwrite//False/False/Dummy output port
 # @par EAGLE_END
@@ -97,14 +98,15 @@
 
 ##
 # @brief SharedMemory
 # @details Data stored in shared memory
 # @par EAGLE_START
 # @param category SharedMemory
 # @param tag daliuge
+# @param dropclass dropclass/dlg.data.drops.memory.SharedMemoryDROP/String/ComponentParameter/readwrite//False/False/Drop class
 # @param data_volume Data volume/5/Float/ComponentParameter/readwrite//False/False/Estimated size of the data contained in this node
 # @param group_end Group end/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the end of a group?
 # @param streaming Streaming/False/Boolean/ComponentParameter/readwrite//False/False/Specifies whether this data component streams input and output data
 # @param persist Persist/False/Boolean/ComponentParameter/readwrite//False/False/Specifies whether this data component contains data that should not be deleted after execution
 # @param dummy dummy//Object/InputPort/readwrite//False/False/Dummy input port
 # @param dummy dummy//Object/OutputPort/readwrite//False/False/Dummy output port
 # @par EAGLE_END
```

### Comparing `daliuge-engine-2.4.0/dlg/data/drops/ngas.py` & `daliuge-engine-3.0.0/dlg/data/drops/ngas.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,22 +27,23 @@
 
 ##
 # @brief NGAS
 # @details An archive on the Next Generation Archive System (NGAS).
 # @par EAGLE_START
 # @param category NGAS
 # @param tag daliuge
-# @param data_volume Data volume/5/Float/ComponentParameter/readwrite//False/False/Estimated size of the data contained in this node
-# @param group_end Group end/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the end of a group?
 # @param ngasSrv NGAS Server/localhost/String/ComponentParameter/readwrite//False/False/The URL of the NGAS Server
 # @param ngasPort NGAS Port/7777/Integer/ComponentParameter/readwrite//False/False/The port of the NGAS Server
 # @param ngasFileId File ID//String/ComponentParameter/readwrite//False/False/File ID on NGAS (for retrieval only)
 # @param ngasConnectTimeout Connection timeout/2/Integer/ComponentParameter/readwrite//False/False/Timeout for connecting to the NGAS server
 # @param ngasMime NGAS mime-type/"text/ascii"/String/ComponentParameter/readwrite//False/False/Mime-type to be used for archiving
 # @param ngasTimeout NGAS timeout/2/Integer/ComponentParameter/readwrite//False/False/Timeout for receiving responses for NGAS
+# @param dropclass dropclass/dlg.data.drops.ngas.NgasDROP/String/ComponentParameter/readwrite//False/False/Drop class
+# @param data_volume Data volume/5/Float/ComponentParameter/readwrite//False/False/Estimated size of the data contained in this node
+# @param group_end Group end/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the end of a group?
 # @param streaming Streaming/False/Boolean/ComponentParameter/readwrite//False/False/Specifies whether this data component streams input and output data
 # @param persist Persist/False/Boolean/ComponentParameter/readwrite//False/False/Specifies whether this data component contains data that should not be deleted after execution
 # @param dummy dummy//Object/InputPort/readwrite//False/False/Dummy input port
 # @param dummy dummy//Object/OutputPort/readwrite//False/False/Dummy output port
 # @par EAGLE_END
 class NgasDROP(DataDROP):
     """
```

### Comparing `daliuge-engine-2.4.0/dlg/data/drops/parset_drop.py` & `daliuge-engine-3.0.0/dlg/data/drops/parset_drop.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,16 +34,18 @@
 # @par EAGLE_START
 # @param category ParameterSet
 # @param tag daliuge
 # @param data_volume Data volume/5/Float/ComponentParameter/readwrite//False/False/Estimated size of the data contained in this node
 # @param group_end Group end/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the end of a group?
 # @param mode Parset mode/"YANDA"/String/ComponentParameter/readonly//False/False/To what standard DALiuGE should filter and serialize the parameters.
 # @param config_data ConfigData/""/String/ComponentParameter/readwrite//False/False/Additional configuration information to be mixed in with the initial data
+# @param dropclass dropclass/dlg.data.drops.parset_drop.ParameterSetDROP/String/ComponentParameter/readwrite//False/False/Drop class
 # @param streaming Streaming/False/Boolean/ComponentParameter/readwrite//False/False/Specifies whether this data component streams input and output data
 # @param persist Persist/False/Boolean/ComponentParameter/readwrite//False/False/Specifies whether this data component contains data that should not be deleted after execution
+# @param dropclass dropclass//dlg.data.drops.parset_drop.ParameterSetDROP//readonly//False/False/default class for this DROP
 # @param Config ConfigFile//Object.File/OutputPort/readwrite//False/False/The output configuration file
 # @par EAGLE_END
 class ParameterSetDROP(DataDROP):
     """
     A generic configuration file template wrapper
     This drop opens an (optional) file containing some initial configuration information, then
     appends any additional specified parameters to it, finally serving it as a data object.
```

### Comparing `daliuge-engine-2.4.0/dlg/data/drops/plasma.py` & `daliuge-engine-3.0.0/dlg/data/drops/plasma.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,19 +32,21 @@
 
 ##
 # @brief Plasma
 # @details An object in a Apache Arrow Plasma in-memory object store
 # @par EAGLE_START
 # @param category Plasma
 # @param tag daliuge
+# @param plasma_path Plasma Path//String/ApplicationArgument/readwrite//False/False/Path to the local plasma store
+# @param object_id Object Id//String/ApplicationArgument/readwrite//False/False/PlasmaId of the object for all compute nodes
+# @param dropclass dropclass/dlg.data.drops.plasma.PlasmaDROP/String/ComponentParameter/readwrite//False/False/Drop class
 # @param data_volume Data volume/5/Float/ComponentParameter/readwrite//False/False/Estimated size of the data contained in this node
 # @param group_end Group end/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the end of a group?
-# @param plasma_path Plasma Path//String/ComponentParameter/readwrite//False/False/Path to the local plasma store
-# @param object_id Object Id//String/ComponentParameter/readwrite//False/False/PlasmaId of the object for all compute nodes
 # @param use_staging Use Staging/False/Boolean/ComponentParameter/readwrite//False/False/Enables writing to a dynamically resizeable staging buffer
+# @param dropclass dropclass/dlg.data.drops.plasma.PlasmaDROP/String/ComponentParameter/readwrite//False/False/Drop class
 # @param dummy dummy//Object/InputPort/readwrite//False/False/Dummy input port
 # @param dummy dummy//Object/OutputPort/readwrite//False/False/Dummy output port
 # @par EAGLE_END
 class PlasmaDROP(DataDROP):
     """
     A DROP that points to data stored in a Plasma Store
     """
@@ -83,18 +85,19 @@
 ##
 # @brief PlasmaFlight
 # @details An Apache Arrow Flight server providing distributed access
 # to a Plasma in-memory object store
 # @par EAGLE_START
 # @param category PlasmaFlight
 # @param tag daliuge
+# @param plasma_path Plasma Path//String/ApplicationArgument/readwrite//False/False/Path to the local plasma store
+# @param object_id Object Id//String/ApplicationArgument/readwrite//False/False/PlasmaId of the object for all compute nodes
+# @param dropclass dropclass/dlg.data.drops.plasma.PlasmaFlightDROP/String/ComponentParameter/readwrite//False/False/Drop class
 # @param data_volume Data volume/5/Float/ComponentParameter/readwrite//False/False/Estimated size of the data contained in this node
 # @param group_end Group end/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the end of a group?
-# @param plasma_path Plasma Path//String/ComponentParameter/readwrite//False/False/Path to the local plasma store
-# @param object_id Object Id//String/ComponentParameter/readwrite//False/False/PlasmaId of the object for all compute nodes
 # @param flight_path Flight Path//String/ComponentParameter/readwrite//False/False/IP and flight port of the drop owner
 # @param dummy dummy//Object/InputPort/readwrite//False/False/Dummy input port
 # @param dummy dummy//Object/OutputPort/readwrite//False/False/Dummy output port
 # @par EAGLE_END
 class PlasmaFlightDROP(DataDROP):
     """
     A DROP that points to data stored in a Plasma Store
```

### Comparing `daliuge-engine-2.4.0/dlg/data/drops/rdbms.py` & `daliuge-engine-3.0.0/dlg/data/drops/rdbms.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 # @param data_volume Data volume/5/Float/ComponentParameter/readwrite//False/False/Estimated size of the data contained in this node
 # @param group_end Group end/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the end of a group?
 # @param dbmodule Python DB module//String/ComponentParameter/readwrite//False/False/Load path for python DB module
 # @param dbtable DB table name//String/ComponentParameter/readwrite//False/False/The name of the table to use
 # @param vals Values dictionary/{}/Json/ComponentParameter/readwrite//False/False/Json encoded values dictionary used for INSERT. The keys of ``vals`` are used as the column names.
 # @param condition Whats used after WHERE//String/ComponentParameter/readwrite//False/False/Condition for SELECT. For this the WHERE statement must be written using the "{X}" or "{}" placeholders
 # @param selectVals values for WHERE/{}/Json/ComponentParameter/readwrite//False/False/Values for the WHERE statement
+# @param dropclass dropclass/dlg.data.drops.rdbms.RDBMSDrop/String/ComponentParameter/readwrite//False/False/Drop class
 # @param dummy dummy//Object/InputPort/readwrite//False/False/Dummy input port
 # @param dummy dummy//Object/OutputPort/readwrite//False/False/Dummy output port
 # @par EAGLE_END
 class RDBMSDrop(DataDROP):
     """
     A Drop that stores data in a table of a relational database
     """
@@ -113,15 +114,14 @@
         result set by specifying a list of ``columns`` to be returned (otherwise
         all table columns are returned) and a ``condition`` to be applied,
         in which case a list of ``vals`` to be applied as query parameters can
         also be given.
         """
         with self._connection() as c:
             with self._cursor(c) as cur:
-
                 # Build up SQL with optional columns and conditions
                 columns = columns or ("*",)
                 sql = [
                     "SELECT %s FROM %s" % (",".join(columns), self._db_table)
                 ]
                 if condition:
                     sql.append(" WHERE ")
```

### Comparing `daliuge-engine-2.4.0/dlg/data/drops/s3_drop.py` & `daliuge-engine-3.0.0/dlg/data/drops/s3_drop.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,43 +31,59 @@
 try:
     import boto3
     import botocore
 
 except ImportError:
     logger.warning("BOTO bindings are not available")
 
-from ...data.drops.data_base import DataDROP
+from .data_base import DataDROP
 from dlg.data.io import ErrorIO, OpenMode, DataIO
-from ...meta import dlg_string_param, dlg_list_param
+from dlg.meta import (
+    dlg_component,
+    dlg_batch_input,
+    dlg_batch_output,
+    dlg_streaming_input,
+    dlg_string_param,
+    dlg_list_param,
+)
 
 from dlg.named_port_utils import identify_named_ports, check_ports_dict
 
 
 ##
 # @brief S3
 # @details An object available in a bucket on a S3 (Simple Storage Service) object storage platform
 # @par EAGLE_START
 # @param category S3
 # @param tag daliuge
 # @param data_volume Data volume/5/Float/ComponentParameter/readwrite//False/False/Estimated size of the data contained in this node
 # @param group_end Group end/False/Boolean/ComponentParameter/readwrite//False/False/Is this node the end of a group?
-# @param bucket Bucket//String/ComponentParameter/readwrite//False/False/The S3 Bucket
-# @param object_name Object Name//String/ComponentParameter/readwrite//False/False/The S3 object key
+# @param Bucket Bucket//String/ComponentParameter/readwrite//False/False/The S3 Bucket
+# @param Key Key//String/ComponentParameter/readwrite//False/False/The S3 object key
 # @param profile_name Profile Name//String/ComponentParameter/readwrite//False/False/The S3 profile name
 # @param endpoint_url Endpoint URL//String/ComponentParameter/readwrite//False/False/The URL exposing the S3 REST API
+# @param dropclass dropclass/dlg.data.drops.s3_drop.S3DROP/String/ComponentParameter/readwrite//False/False/The URL exposing the S3 REST API
 # @param streaming Streaming/False/Boolean/ComponentParameter/readwrite//False/False/Specifies whether this data component streams input and output data
 # @param persist Persist/False/Boolean/ComponentParameter/readwrite//False/False/Specifies whether this data component contains data that should not be deleted after execution
 # @param dummy dummy//Object/InputPort/readwrite//False/False/Dummy input port
 # @param dummy dummy//Object/OutputPort/readwrite//False/False/Dummy output port
 # @par EAGLE_END
 class S3DROP(DataDROP):
     """
     A DROP that points to data stored in S3
     """
 
+    component_meta = dlg_component(
+        "S3DROP",
+        "S3 Data Drop",
+        [dlg_batch_input("binary/*", [])],
+        [dlg_batch_output("binary/*", [])],
+        [dlg_streaming_input("binary/*")],
+    )
+
     Bucket = dlg_string_param("Bucket", None)
     Key = dlg_string_param("Key", None)
     storage_class = dlg_string_param("storage_class", "S3")
     tags = dlg_list_param("tags", None)
     # don't change the aws names
     aws_access_key_id = dlg_string_param("aws_access_key_id", None)
     aws_secret_access_key = dlg_string_param("aws_secret_access_key", None)
@@ -81,14 +97,15 @@
             "storage_class": self.storage_class,
             "tags": self.tags,
             "aws_access_key_id": self.aws_access_key_id,
             "aws_secret_access_key": self.aws_secret_access_key,
             "profile_name": self.profile_name,
             "endpoint_url": self.endpoint_url,
         }
+        logger.debug("S3 initializing: %s", self.keyargs)
         self.Key = self.uid if not self.Key else self.Key
         return super().initialize(**kwargs)
 
     @property
     def path(self) -> str:
         """
         Returns the path to the S3 object
@@ -142,15 +159,14 @@
         profile_name=None,
         Bucket=None,
         Key=None,
         endpoint_url=None,
         expectedSize=-1,
         **kwargs,
     ):
-
         super().__init__(**kwargs)
 
         logger.debug(
             (
                 "key_id: %s; key: %s; profile: %s; bucket: %s; object_id: %s; %s",
                 aws_access_key_id,
                 aws_secret_access_key,
```

### Comparing `daliuge-engine-2.4.0/dlg/data/io.py` & `daliuge-engine-3.0.0/dlg/data/io.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/ddap_protocol.py` & `daliuge-engine-3.0.0/dlg/ddap_protocol.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/deploy/__init__.py` & `daliuge-engine-3.0.0/dlg/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/deploy/common.py` & `daliuge-engine-3.0.0/dlg/deploy/common.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/deploy/configs/__init__.py` & `daliuge-engine-3.0.0/dlg/deploy/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/deploy/create_dlg_job.py` & `daliuge-engine-3.0.0/dlg/deploy/create_dlg_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,30 +31,38 @@
 import pwd
 import re
 import socket
 import sys
 import time
 import os
 
-from dlg.deploy.configs import ConfigFactory  # get all available configurations
-from dlg.deploy.deployment_constants import DEFAULT_AWS_MON_PORT, DEFAULT_AWS_MON_HOST
+from dlg.deploy.configs import (
+    ConfigFactory,
+)  # get all available configurations
+from dlg.deploy.deployment_constants import (
+    DEFAULT_AWS_MON_PORT,
+    DEFAULT_AWS_MON_HOST,
+)
 from dlg.deploy.slurm_client import SlurmClient
 
 FACILITIES = ConfigFactory.available()
 
 
 def get_timestamp(line):
     """
     microsecond precision
     """
     split = line.split()
     date_time = "{0}T{1}".format(split[0], split[1])
     pattern = "%Y-%m-%dT%H:%M:%S,%f"
     epoch = time.mktime(time.strptime(date_time, pattern))
-    return datetime.datetime.strptime(date_time, pattern).microsecond / 1e6 + epoch
+    return (
+        datetime.datetime.strptime(date_time, pattern).microsecond / 1e6
+        + epoch
+    )
 
 
 class LogEntryPair:
     """
     Generates log entries
     """
 
@@ -133,15 +141,16 @@
         )
     ]
 
 
 def construct_catchall_pattern(node_type):
     pattern_strs = LogParser.kwords.get(node_type)
     patterns = [
-        x.format(".*").replace("(", r"\(").replace(")", r"\)") for x in pattern_strs
+        x.format(".*").replace("(", r"\(").replace(")", r"\)")
+        for x in pattern_strs
     ]
     catchall = "|".join(["(%s)" % (s,) for s in patterns])
     catchall = ".*(%s).*" % (catchall,)
     return re.compile(catchall)
 
 
 class LogParser:
@@ -201,23 +210,28 @@
         "Creating DROPs for session",  # Drops are being created
         "Session {0} is now RUNNING",  # All drops created and ready
         "Session {0} finished",  # All drops executed
     ]
 
     kwords = dict()
     kwords["dim"] = dim_kl
-    kwords["nm"] = nm_kl
+    kwords["name"] = nm_kl
 
     def __init__(self, log_dir):
         self._dim_log_f = None
         if not self.check_log_dir(log_dir):
             raise Exception("No DIM log found at: {0}".format(log_dir))
         self._log_dir = log_dir
-        self._dim_catchall_pattern = construct_catchall_pattern(node_type="dim")
-        self._nm_catchall_pattern = construct_catchall_pattern(node_type="nm")
+        self._dim_catchall_pattern = construct_catchall_pattern(
+            node_type="dim"
+        )
+        # self._nm_catchall_pattern = construct_catchall_pattern(node_type="nm")
+        self._nm_catchall_pattern = construct_catchall_pattern(
+            node_type="name"
+        )
 
     def parse(self, out_csv=None):
         """
         e.g. lofar_std_N4_2016-08-22T11-52-11
         """
         logb_name = os.path.basename(self._log_dir)
         search_string = re.search("_N[0-9]+_", logb_name)
@@ -267,19 +281,22 @@
         # parse NM logs
         nm_logs = []
         max_node_deploy_time = 0
         num_finished_sess = 0
 
         num_dims = 0
         for log_directory_file_name in os.listdir(self._log_dir):
-
             # Check this is a dir and contains the NM log
-            if not os.path.isdir(os.path.join(self._log_dir, log_directory_file_name)):
+            if not os.path.isdir(
+                os.path.join(self._log_dir, log_directory_file_name)
+            ):
                 continue
-            nm_logf = os.path.join(self._log_dir, log_directory_file_name, "dlgNM.log")
+            nm_logf = os.path.join(
+                self._log_dir, log_directory_file_name, "dlgNM.log"
+            )
             nm_dim_logf = os.path.join(
                 self._log_dir, log_directory_file_name, "dlgDIM.log"
             )
             nm_mm_logf = os.path.join(
                 self._log_dir, log_directory_file_name, "dlgMM.log"
             )
             if not os.path.exists(nm_logf):
@@ -299,15 +316,14 @@
                         continue
                     for lep in nm_log_pairs:
                         lep.check_start(matches, line)
                         lep.check_end(matches, line)
 
             # Looking for the deployment times and counting for finished sessions
             for lep in nm_log_pairs:
-
                 # Consider only valid durations
                 dur = lep.get_duration()
                 if dur is None:
                     continue
 
                 if lep.name in ("completion_time", "completion_time_old"):
                     num_finished_sess += 1
@@ -335,15 +351,14 @@
         # The DIM waits for all NMs to setup before triggering the first drops.
         # This has the effect that the slowest to setup will make the others
         # idle while already in RUNNING state, effectively increasing their
         # "exec_time". We subtract the maximum deploy time to account for this
         # effect
         max_exec_time = 0
         for log_entry_pairs in nm_logs:
-
             indexed_leps = {lep.name: lep for lep in log_entry_pairs}
             deploy_time = indexed_leps["node_deploy_time"].get_duration()
             if deploy_time is None:  # since some node managers failed to start
                 continue
             exec_time = (
                 indexed_leps["completion_time"].get_duration()
                 or indexed_leps["completion_time_old"].get_duration()
@@ -362,15 +377,17 @@
             pip_name,
             do_date,
             num_nodes,
             num_drops,
             git_commit,
         ]
         ret = [str(x) for x in ret]
-        num_dims = num_dims if num_dims == 1 else num_dims - 1  # exclude master manager
+        num_dims = (
+            num_dims if num_dims == 1 else num_dims - 1
+        )  # exclude master manager
         add_line = ",".join(ret + temp_dim + temp_nm + [str(int(num_dims))])
         if out_csv is not None:
             with open(out_csv, "a") as out_file:
                 out_file.write(add_line)
                 out_file.write(os.linesep)
         else:
             print(add_line)
@@ -380,15 +397,17 @@
             os.path.join(log_dir, "0", "dlgDIM.log"),
             os.path.join(log_dir, "0", "dlgMM.log"),
         ]
         for dim_log_f in possible_logs:
             if os.path.exists(dim_log_f):
                 self._dim_log_f = [dim_log_f]
                 if dim_log_f == possible_logs[0]:
-                    cluster_log = os.path.join(log_dir, "0", "start_dlg_cluster.log")
+                    cluster_log = os.path.join(
+                        log_dir, "0", "start_dlg_cluster.log"
+                    )
                     if os.path.exists(cluster_log):
                         self._dim_log_f.append(cluster_log)
                 return True
         return False
 
 
 def main():
@@ -581,15 +600,17 @@
         default=True,
     )
 
     (opts, _) = parser.parse_args(sys.argv)
     if not (opts.action and opts.facility) and not opts.configs:
         parser.error("Missing required parameters!")
     if opts.facility not in FACILITIES:
-        parser.error(f"Unknown facility provided. Please choose from {FACILITIES}")
+        parser.error(
+            f"Unknown facility provided. Please choose from {FACILITIES}"
+        )
 
     if opts.action == 2:
         if opts.log_dir is None:
             # you can specify:
             # either a single directory
             if opts.log_root is None:
                 config = ConfigFactory.create_config(facility=opts.facility)
@@ -605,28 +626,31 @@
                 for log_dir in os.listdir(log_root):
                     log_dir = os.path.join(log_root, log_dir)
                     if os.path.isdir(log_dir):
                         try:
                             log_parser = LogParser(log_dir)
                             log_parser.parse(out_csv=opts.csv_output)
                         except Exception as exp:
-                            print("Fail to parse {0}: {1}".format(log_dir, exp))
+                            print(
+                                "Fail to parse {0}: {1}".format(log_dir, exp)
+                            )
         else:
             log_parser = LogParser(opts.log_dir)
             log_parser.parse(out_csv=opts.csv_output)
     elif opts.action == 1:
-
         if opts.logical_graph and opts.physical_graph:
             parser.error(
                 "Either a logical graph or physical graph filename must be specified"
             )
         for path_to_graph_file in (opts.logical_graph, opts.physical_graph):
             if path_to_graph_file and not os.path.exists(path_to_graph_file):
                 parser.error(
-                    "Cannot locate graph file at '{0}'".format(path_to_graph_file)
+                    "Cannot locate graph file at '{0}'".format(
+                        path_to_graph_file
+                    )
                 )
 
         client = SlurmClient(
             facility=opts.facility,
             job_dur=opts.job_dur,
             num_nodes=opts.num_nodes,
             logv=opts.verbose_level,
```

### Comparing `daliuge-engine-2.4.0/dlg/deploy/deployment_constants.py` & `daliuge-engine-3.0.0/dlg/deploy/deployment_constants.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/deploy/deployment_utils.py` & `daliuge-engine-3.0.0/dlg/deploy/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/deploy/dlg_monitor.py` & `daliuge-engine-3.0.0/dlg/deploy/dlg_monitor.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/deploy/dlg_proxy.py` & `daliuge-engine-3.0.0/dlg/deploy/dlg_proxy.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/deploy/helm_client.py` & `daliuge-engine-3.0.0/dlg/deploy/helm_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,40 +68,46 @@
     keywords: list,
     sources: list,
     kubeVersion: str,
 ):
     chart_info = {
         "apiVersion": "v2",
         "name": chart_name,
-        "type": "application",
+        "categoryType": "Application",
         "version": version,
         "appVersion": app_version,
         "home": home,
         "description": description,
         "keywords": keywords,
         "sources": sources,
         "kubeVersion": kubeVersion,
     }
     # TODO: Fix app_version quotations.
-    with open(f"{chart_dir}{os.sep}{name}", "w", encoding="utf-8") as chart_file:
+    with open(
+        f"{chart_dir}{os.sep}{name}", "w", encoding="utf-8"
+    ) as chart_file:
         yaml.dump(chart_info, chart_file)
 
 
 def _write_values(chart_dir, config):
     with open(
         f"{chart_dir}{os.sep}custom-values.yaml", "w+", encoding="utf-8"
     ) as value_file:
         yaml.dump(config, value_file)
     logger.info("Written custom-values file.")
 
 
 def _read_values(chart_dir):
-    with open(f"{chart_dir}{os.sep}values.yaml", "r", encoding="utf-8") as old_file:
+    with open(
+        f"{chart_dir}{os.sep}values.yaml", "r", encoding="utf-8"
+    ) as old_file:
         data = yaml.safe_load(old_file)
-    with open(f"{chart_dir}{os.sep}values.yaml", "r", encoding="utf-8") as custom_file:
+    with open(
+        f"{chart_dir}{os.sep}values.yaml", "r", encoding="utf-8"
+    ) as custom_file:
         new_data = yaml.safe_load(custom_file)
     data.update(new_data)
     logger.info("Read yaml values file")
     return data
 
 
 def _find_resources(pgt_data):
@@ -154,42 +160,51 @@
         self._k8s_nodes = find_node_ips()
         self._num_machines = 1
         self._pod_details = {}
         if physical_graph_file is not None:
             self._set_physical_graph(physical_graph_file)
 
         # Copy in template files.
-        library_root = pathlib.Path(os.path.dirname(dlg.__file__)).parent.parent
+        library_root = pathlib.Path(
+            os.path.dirname(dlg.__file__)
+        ).parent.parent
         logger.debug(f"Helm chart copied to: {library_root}")
         if sys.version_info >= (3, 8):
             shutil.copytree(
                 os.path.join(library_root, "daliuge-k8s", "helm"),
                 self._deploy_dir,
                 dirs_exist_ok=True,
             )
         else:
             shutil.copytree(
-                os.path.join(library_root, "daliuge-k8s", "helm"), self._deploy_dir
+                os.path.join(library_root, "daliuge-k8s", "helm"),
+                self._deploy_dir,
             )
 
     def _set_physical_graph(self, physical_graph_content, co_host=True):
         self._physical_graph_file = physical_graph_content
         self._islands, self._nodes = _find_resources(self._physical_graph_file)
-        self._num_machines = _num_deployments_required(self._islands, self._nodes) - (
-            1 if co_host else 0
-        )
+        self._num_machines = _num_deployments_required(
+            self._islands, self._nodes
+        ) - (1 if co_host else 0)
 
     def _find_pod_details(self):
         # NOTE: +1 for the master.
         service_ips = find_service_ips(self._num_machines + 1)
         pod_ips = find_pod_ips(self._num_machines + 1)
         labels = sorted([str(x) for x in range(self._num_machines)])
         for i in range(len(labels)):
-            self._pod_details[labels[i]] = {"ip": pod_ips[i], "svc": service_ips[i]}
-        self._pod_details["master"] = {"ip": pod_ips[-1], "svc": service_ips[-1]}
+            self._pod_details[labels[i]] = {
+                "ip": pod_ips[i],
+                "svc": service_ips[i],
+            }
+        self._pod_details["master"] = {
+            "ip": pod_ips[-1],
+            "svc": service_ips[-1],
+        }
         logger.debug(f"Pod details: {self._pod_details}")
 
     def create_helm_chart(self, physical_graph_content, co_host=True):
         """
         Translates a physical graph to a kubernetes helm chart.
         For now, it will just try to run everything in a single container.
         """
@@ -225,18 +240,22 @@
         )
         node_ips = [x["ip"] for x in self._pod_details.values()]
         print(node_ips)
         data = json.dumps({"nodes": node_ips}).encode("utf-8")
         time.sleep(5)
         logger.debug(f"Starting manager on {self._submission_endpoint}")
         client._POST(
-            "/managers/island/start", content=data, content_type="application/json"
+            "/managers/island/start",
+            content=data,
+            content_type="application/json",
         ).read()
         client._POST(
-            "/managers/master/start", content=data, content_type="application/json"
+            "/managers/master/start",
+            content=data,
+            content_type="application/json",
         ).read()
 
     def start_nodes(self):
         if not self._k8s_access:
             raise RuntimeError("Cannot access k8s")
         ips = [x["svc"] for x in self._pod_details.values()]
         ips.remove(self._pod_details["master"]["svc"])
@@ -247,15 +266,17 @@
             time.sleep(5)
             logger.debug(f"Starting node on {ip}")
             # node_ips = ['localhost'] + [x['ip'] for x in self._pod_details.values()]
             node_ips = [x["ip"] for x in self._pod_details.values()]
             # data = json.dumps({'nodes': ['localhost']}).encode('utf-8')
             data = json.dumps({"nodes": node_ips}).encode("utf-8")
             client._POST(
-                "/managers/master/start", content=data, content_type="application/json"
+                "/managers/master/start",
+                content=data,
+                content_type="application/json",
             ).read()
 
     def launch_helm(self, co_host=False):
         """
         Launches the built helm chart using the most straightforward commands possible.
         Assumes all files are prepared and validated.
         """
@@ -273,15 +294,16 @@
             )
             process_return_string = subprocess.check_output(
                 [instruction], shell=True
             ).decode("utf-8")
             logger.info(f"{process_return_string}")
             for i in range(self._num_machines):
                 _write_values(
-                    self._chart_dir, {"deploy_id": i, "name": f"{self._chart_name}-{i}"}
+                    self._chart_dir,
+                    {"deploy_id": i, "name": f"{self._chart_name}-{i}"},
                 )
                 instruction = (
                     f"helm install {self._deploy_name}-{i} {self._chart_name}/  "
                     f"--values {self._chart_name}{os.sep}custom-values.yaml"
                 )
                 process_return_string = subprocess.check_output(
                     [instruction], shell=True
@@ -291,37 +313,47 @@
             self._find_pod_details()
             if wait_for_pods(self._num_machines):
                 self.start_manager("master")
                 # self.start_nodes()
             else:
                 logger.error("K8s pods did not start in timeframe allocated")
                 self.teardown()
-                raise RuntimeWarning("K8s pods did not start in timeframe allocated")
+                raise RuntimeWarning(
+                    "K8s pods did not start in timeframe allocated"
+                )
         else:
-            logger.info(f"Created helm chart {self._chart_name} in {self._deploy_dir}")
+            logger.info(
+                f"Created helm chart {self._chart_name} in {self._deploy_dir}"
+            )
 
     def teardown(self):
         if not self._k8s_access:
             raise RuntimeError("Cannot access k8s")
         for i in range(self._num_machines - 1, -1, -1):
-            subprocess.check_output([f"helm uninstall daliuge-daemon-{i}"], shell=True)
-        subprocess.check_output([f"helm uninstall daliuge-daemon-master"], shell=True)
+            subprocess.check_output(
+                [f"helm uninstall daliuge-daemon-{i}"], shell=True
+            )
+        subprocess.check_output(
+            [f"helm uninstall daliuge-daemon-master"], shell=True
+        )
 
     def _monitor(self, session_id=None):
         def _task():
             while True:
                 try:
                     dlg.deploy.common.monitor_sessions(
                         session_id=session_id,
                         host=self._submission_endpoint,
                         port=NODE_DEFAULT_REST_PORT,
                     )
                     break
                 except:
-                    logger.exception("Monitoring failed, attempting to restart")
+                    logger.exception(
+                        "Monitoring failed, attempting to restart"
+                    )
 
         threads = threading.Thread(target=_task)
         threads.start()
         return threads
 
     def submit_pgt(self):
         """
@@ -332,15 +364,17 @@
             raise RuntimeError("Cannot access k8s")
         # TODO: Check all nodes are operational first.
         pgt_data = json.loads(self._physical_graph_file)
         node_ips = [x["ip"] for x in self._pod_details.values()]
         node_ips.remove(self._pod_details["master"]["ip"])
         node_ips = [self._pod_details["master"]["ip"]] + node_ips
         # node_ips = ['localhost']
-        physical_graph = pg_generator.resource_map(pgt_data, node_ips, co_host_dim=True)
+        physical_graph = pg_generator.resource_map(
+            pgt_data, node_ips, co_host_dim=True
+        )
         # TODO: Add dumping to log-dir
         submit(
             physical_graph,
             self._submission_endpoint,
             port=NODE_DEFAULT_REST_PORT,
             skip_deploy=False,
         )
```

### Comparing `daliuge-engine-2.4.0/dlg/deploy/remotes.py` & `daliuge-engine-3.0.0/dlg/deploy/remotes.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/deploy/slurm_client.py` & `daliuge-engine-3.0.0/dlg/deploy/slurm_client.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/deploy/start_dlg_cluster.py` & `daliuge-engine-3.0.0/dlg/deploy/start_dlg_cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,24 +51,31 @@
 from dlg.manager import cmdline
 from dlg.manager.client import NodeManagerClient
 from dlg.manager.constants import (
     NODE_DEFAULT_REST_PORT,
     ISLAND_DEFAULT_REST_PORT,
     MASTER_DEFAULT_REST_PORT,
 )
-from dlg.common.reproducibility.reproducibility import init_pgt_unroll_repro_data, \
-    init_pgt_partition_repro_data, init_pg_repro_data
+from dlg.common.reproducibility.reproducibility import (
+    init_pgt_unroll_repro_data,
+    init_pgt_partition_repro_data,
+    init_pg_repro_data,
+)
 
 DIM_WAIT_TIME = 60
 MM_WAIT_TIME = DIM_WAIT_TIME
 GRAPH_SUBMIT_WAIT_TIME = 10
 GRAPH_MONITOR_INTERVAL = 5
 VERBOSITY = "5"
 LOGGER = logging.getLogger("deploy.dlg.cluster")
-APPS = (None, "test.graphsRepository.SleepApp", "test.graphsRepository.SleepAndCopyApp")
+APPS = (
+    None,
+    "test.graphsRepository.SleepApp",
+    "test.graphsRepository.SleepAndCopyApp",
+)
 
 
 def check_host(host, port, timeout=5, check_with_session=False):
     """
     Checks if a given host/port is up and running (i.e., it is open).
     If ``check_with_session`` is ``True`` then it is assumed that the
     host/port combination corresponds to a Node Manager and the check is
@@ -93,15 +100,18 @@
     given timeout, and returns the list of IPs that were found to be up.
     """
 
     def check_and_add(ip_addr):
         ntries = retry
         while ntries:
             if check_host(
-                ip_addr, port, timeout=timeout, check_with_session=check_with_session
+                ip_addr,
+                port,
+                timeout=timeout,
+                check_with_session=check_with_session,
             ):
                 LOGGER.info("Host %s:%d is running", ip_addr, port)
                 return ip_addr
             LOGGER.warning("Failed to contact host %s:%d", ip_addr, port)
             ntries -= 1
         return None
 
@@ -113,15 +123,17 @@
 
     return [ip for ip in result_pool if ip]
 
 
 def get_ip_via_ifconfig(iface_index):
     out = subprocess.check_output("ifconfig")
     ifaces_info = list(filter(None, out.split(b"\n\n")))
-    LOGGER.info("Found %d interfaces, getting %d", len(ifaces_info), iface_index)
+    LOGGER.info(
+        "Found %d interfaces, getting %d", len(ifaces_info), iface_index
+    )
     for line in ifaces_info[iface_index].splitlines():
         line = line.strip()
         if line.startswith(b"inet"):
             return utils.b2s(line.split()[1])
     raise ValueError("Interace %d is not an IP interface" % iface_index)
 
 
@@ -133,15 +145,21 @@
     """
     Common workspace dir for all nodes just underneath main session directory
     """
     return f"{os.path.split(log_dir)[0]}/workspace"
 
 
 def start_node_mgr(
-    log_dir, my_ip, logv=1, max_threads=0, host=None, event_listeners="", use_tool=True
+    log_dir,
+    my_ip,
+    logv=1,
+    max_threads=0,
+    host=None,
+    event_listeners="",
+    use_tool=True,
 ):
     """
     Start node manager
     """
     LOGGER.info("Starting node manager on host %s", my_ip)
     host = host or "0.0.0.0"
     log_level = "v" * logv
@@ -160,28 +178,31 @@
         "--no-dlm",
     ]
     if event_listeners:
         args += ["--event-listeners", event_listeners]
 
     if use_tool:
         # This returns immediately
-        proc = tool.start_process("nm", args)
+        # proc = tool.start_process("nm", args)
+        proc = tool.start_process("name", args)
         LOGGER.info("Node manager process started with pid %d", proc.pid)
         return proc
     else:
         # This blocks until NM shutdown externally
         return cmdline.dlgNM(optparse.OptionParser(), args)
 
 
 def start_dim(node_list, log_dir, origin_ip, logv=1):
     """
     Start data island manager
     """
     LOGGER.info(
-        "Starting island manager on host %s for node managers %r", origin_ip, node_list
+        "Starting island manager on host %s for node managers %r",
+        origin_ip,
+        node_list,
     )
     log_level = "v" * logv
     args = [
         "-l",
         log_dir,
         "-w",
         get_workspace_dir(log_dir),
@@ -262,23 +283,30 @@
         if submit:
             session_id = common.submit(
                 physical_graph, host=host, port=port, session_id=opts.ssid
             )
         else:
             session_id = opts.ssid
 
-        LOGGER.info(f"Start monitoring session(s) '{session_id}' on host {host}:{port}")
+        LOGGER.info(
+            f"Start monitoring session(s) '{session_id}' on host {host}:{port}"
+        )
         while True:
             try:
                 common.monitor_sessions(
-                    session_id, host=host, port=port, status_dump_path=dump_path
+                    session_id,
+                    host=host,
+                    port=port,
+                    status_dump_path=dump_path,
                 )
                 break
             except:
-                LOGGER.exception(f"Monitoring {host}:{port} failed, restarting it")
+                LOGGER.exception(
+                    f"Monitoring {host}:{port} failed, restarting it"
+                )
                 time.sleep(5)
 
     threads = threading.Thread(target=_task)
     threads.start()
     return threads
 
 
@@ -300,30 +328,34 @@
         sys.exit(1)
 
 
 def modify_pg(pgt, modifier):
     parts = modifier.split(",")
     func = utils.get_symbol(parts[0])
     args = list(filter(lambda x: "=" not in x, parts[1:]))
-    kwargs = dict(map(lambda x: x.split("="), filter(lambda x: "=" in x, parts[1:])))
+    kwargs = dict(
+        map(lambda x: x.split("="), filter(lambda x: "=" in x, parts[1:]))
+    )
     return func(pgt, *args, **kwargs)
 
 
 def get_pg(opts, nms, dims):
     """Gets the Physical Graph that is eventually submitted to the cluster, if any"""
 
     if not opts.logical_graph and not opts.physical_graph:
         return []
 
     num_nms = len(nms)
     num_dims = len(dims)
     if opts.logical_graph:
-        unrolled = init_pgt_unroll_repro_data(pg_generator.unroll(
-            opts.logical_graph, opts.ssid, opts.zerorun, APPS[opts.app]
-        ))
+        unrolled = init_pgt_unroll_repro_data(
+            pg_generator.unroll(
+                opts.logical_graph, opts.ssid, opts.zerorun, APPS[opts.app]
+            )
+        )
         reprodata = {}
         if not unrolled[-1].get("oid"):
             reprodata = unrolled.pop()
         algo_params = parse_partition_algo_params(opts.algo_params)
         pgt = pg_generator.partition(
             unrolled,
             opts.part_algo,
@@ -347,27 +379,33 @@
     nms = check_hosts(
         nms,
         NODE_DEFAULT_REST_PORT,
         check_with_session=opts.check_with_session,
         timeout=MM_WAIT_TIME,
         retry=3,
     )
-    LOGGER.info(f"Mapping graph to available resources: nms {nms}, dims {dims}")
-    physical_graph = init_pg_repro_data(pg_generator.resource_map(
-        pgt, dims + nms, num_islands=num_dims, co_host_dim=opts.co_host_dim
-    ))
+    LOGGER.info(
+        f"Mapping graph to available resources: nms {nms}, dims {dims}"
+    )
+    physical_graph = init_pg_repro_data(
+        pg_generator.resource_map(
+            pgt, dims + nms, num_islands=num_dims, co_host_dim=opts.co_host_dim
+        )
+    )
     graph_name = os.path.basename(opts.log_dir)
     graph_name = f"{graph_name.split('_')[0]}.json"  # get just the graph name
     with open(os.path.join(opts.log_dir, graph_name), "wt") as pg_file:
         json.dump(physical_graph, pg_file)
     return physical_graph
 
 
 def get_ip(opts):
-    find_ip = get_ip_via_ifconfig if opts.use_ifconfig else get_ip_via_netifaces
+    find_ip = (
+        get_ip_via_ifconfig if opts.use_ifconfig else get_ip_via_netifaces
+    )
     return find_ip(opts.interface)
 
 
 def get_remote(opts):
     my_ip = get_ip(opts)
     if opts.remote_mechanism == "mpi":
         return remotes.MPIRemote(opts, my_ip)
@@ -498,15 +536,15 @@
     )
     parser.add_option(
         "-A",
         "--algo-param",
         action="append",
         dest="algo_params",
         help="Extra name=value parameters used by the algorithms (algorithm-specific)",
-        default=[]
+        default=[],
     )
 
     parser.add_option(
         "--ssid", type="string", dest="ssid", help="session id", default=""
     )
 
     parser.add_option(
@@ -591,15 +629,17 @@
         default=True,
     )
 
     (options, _) = parser.parse_args()
 
     if options.check_interfaces:
         try:
-            print("From netifaces: %s" % get_ip_via_netifaces(options.interface))
+            print(
+                "From netifaces: %s" % get_ip_via_netifaces(options.interface)
+            )
         except:
             LOGGER.exception("Failed to get information via netifaces")
         try:
             print("From ifconfig: %s" % get_ip_via_ifconfig(options.interface))
         except:
             LOGGER.exception("Failed to get information via ifconfig")
         sys.exit(0)
@@ -614,15 +654,17 @@
 
     if bool(options.logical_graph) == bool(options.physical_graph):
         parser.error(
             "Either a logical graph or physical graph filename must be specified"
         )
     for graph_file_name in (options.logical_graph, options.physical_graph):
         if graph_file_name and not os.path.exists(graph_file_name):
-            parser.error("Cannot locate graph file at '{0}'".format(graph_file_name))
+            parser.error(
+                "Cannot locate graph file at '{0}'".format(graph_file_name)
+            )
 
     if options.monitor_host is not None and options.num_islands > 1:
         parser.error("We do not support proxy monitor multiple islands yet")
 
     # if options.ssid == "":
     #     options.ssid = time.
 
@@ -631,29 +673,33 @@
     log_dir = "{0}/{1}".format(options.log_dir, remote.my_ip)
     os.makedirs(log_dir)
     logfile = log_dir + "/start_dlg_cluster.log"
     log_format = (
         "%(asctime)-15s [%(levelname)5.5s] [%(threadName)15.15s] "
         "%(name)s#%(funcName)s:%(lineno)s %(message)s"
     )
-    logging.basicConfig(filename=logfile, level=logging.DEBUG, format=log_format)
+    logging.basicConfig(
+        filename=logfile, level=logging.DEBUG, format=log_format
+    )
 
     LOGGER.info("This node has IP address: %s", remote.my_ip)
 
     envfile_name = os.path.join(log_dir, "env.txt")
     LOGGER.debug("Dumping process' environment to %s", envfile_name)
     with open(envfile_name, "wt") as env_file:
         for name, value in sorted(os.environ.items()):
             env_file.write("%s=%s\n" % (name, value))
 
     logv = max(min(3, options.verbose_level), 1)
 
     # need to dump nodes file first
     if remote.is_highest_level_manager:
-        LOGGER.info(f"Node {remote.my_ip} is hosting the highest level manager")
+        LOGGER.info(
+            f"Node {remote.my_ip} is hosting the highest level manager"
+        )
         nodesfile = os.path.join(log_dir, "nodes.txt")
         LOGGER.debug("Dumping list of nodes to %s", nodesfile)
         with open(nodesfile, "wt") as env_file:
             env_file.write("\n".join(remote.sorted_peers))
     dim_proc = None
     # start the NM
     if options.num_islands == 1:
@@ -671,33 +717,41 @@
                 host=None if options.all_nics else remote.my_ip,
                 event_listeners=options.event_listeners,
                 use_tool=co_hosted,
             )
 
         if remote.is_proxy:
             # Wait until the Island Manager is open
-            if utils.portIsOpen(remote.hl_mgr_ip, ISLAND_DEFAULT_REST_PORT, 100):
+            if utils.portIsOpen(
+                remote.hl_mgr_ip, ISLAND_DEFAULT_REST_PORT, 100
+            ):
                 start_proxy(
                     remote.hl_mgr_ip,
                     ISLAND_DEFAULT_REST_PORT,
                     options.monitor_host,
                     options.monitor_port,
                 )
             else:
                 LOGGER.warning(
                     "Couldn't connect to the main drop manager, proxy not started"
                 )
         elif remote.my_ip in remote.dim_ips:
             LOGGER.info(f"Starting island managers on nodes: {remote.dim_ips}")
-            dim_proc = start_dim(remote.nm_ips, log_dir, remote.my_ip, logv=logv)
+            dim_proc = start_dim(
+                remote.nm_ips, log_dir, remote.my_ip, logv=logv
+            )
             # whichever way we came from, now we have to wait until session is finished
             # we always monitor the island, else we will have race conditions
             physical_graph = get_pg(options, remote.nm_ips, remote.dim_ips)
             monitoring_thread = submit_and_monitor(
-                physical_graph, options, remote.dim_ips[0], REST_PORT, submit=co_hosted
+                physical_graph,
+                options,
+                remote.dim_ips[0],
+                REST_PORT,
+                submit=co_hosted,
             )
             monitoring_thread.join()
             # now the session is finished
 
             # still shutting DIM down first to avoid monitoring conflicts
             stop_dims(remote.dim_ips)
             # now stop all the NMs
@@ -713,15 +767,18 @@
         # TODO: In the case of more than one island the NMs are not yet started
 
         physical_graph = get_pg(options, remote.nm_ips, remote.dim_ips)
         remote.send_dim_nodes(physical_graph)
 
         # 7. make sure all DIMs are up running
         dim_ips_up = check_hosts(
-            remote.dim_ips, ISLAND_DEFAULT_REST_PORT, timeout=MM_WAIT_TIME, retry=10
+            remote.dim_ips,
+            ISLAND_DEFAULT_REST_PORT,
+            timeout=MM_WAIT_TIME,
+            retry=10,
         )
         if len(dim_ips_up) < len(remote.dim_ips):
             LOGGER.warning(
                 "Not all DIMs were up and running: %d/%d",
                 len(dim_ips_up),
                 len(remote.dim_ips),
             )
```

### Comparing `daliuge-engine-2.4.0/dlg/deploy/start_helm_cluster.py` & `daliuge-engine-3.0.0/dlg/deploy/start_helm_cluster.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/drop.py` & `daliuge-engine-3.0.0/dlg/drop.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,23 +49,30 @@
     DROPStates,
     DROPRel,
 )
 from dlg.event import EventFirer, EventHandler
 from dlg.exceptions import InvalidDropException, InvalidRelationshipException
 
 DEFAULT_INTERNAL_PARAMETERS = {
+    "dropclass",
+    "category",
     "storage",
+    "nodeAttributes",
+    "streaming",
+    "persist",
     "rank",
-    "loop_cxt",
-    "dw",
+    "loop_ctx",
+    "weight",
     "iid",
-    "dt",
     "consumers",
     "config_data",
     "mode",
+    "group_end",
+    "applicationArgs",
+    "reprodata",
 }
 
 if sys.version_info >= (3, 8):
     pass
 from dlg.utils import (
     createDirIfMissing,
     isabs,
@@ -180,26 +187,26 @@
         kwargs = dict(kwargs)
         # So far only these three are mandatory
         self._oid = str(oid)
         self._uid = str(uid)
 
         # The physical graph drop type. This is determined
         # by the drop category when generating the drop spec
-        self._type = self._popArg(kwargs, "type", None)
+        self._type = self._popArg(kwargs, "categoryType", None)
 
         # The Session owning this drop, if any
         # In most real-world situations this attribute will be set, but in
         # general it cannot be assumed it will (e.g., unit tests create drops
         # directly outside the context of a session).
         self._dlg_session = self._popArg(kwargs, "dlg_session", None)
 
         # A simple name that the Drop might receive
         # This is usually set in the Logical Graph Editor,
         # but is not necessarily always there
-        self.name = self._popArg(kwargs, "nm", "")
+        self.name = self._popArg(kwargs, "name", "")
 
         # The key of this drop in the original Logical Graph
         # This information might or might not be present depending on how the
         # physical graph was generated (or if this drop is being created as part
         # of a graph, to begin with), so we default it to an empty value
         self.lg_key = self._popArg(kwargs, "lg_key", "")
 
@@ -384,18 +391,28 @@
             if has_component_param and has_app_param:
                 logger.warning(
                     f"Drop has both component and app param {attr_name}. Using component param."
                 )
             if has_component_param:
                 param = kwargs.get(attr_name)
             elif has_app_param:
-                param = kwargs["applicationArgs"].get(attr_name).value
+                if kwargs["applicationArgs"].get(attr_name).usage in [
+                    "InputPort",
+                    "OutputPort",
+                    "InputOutput",
+                ]:
+                    # inp = kwargs["input"]
+                    # param = pickle.loads(
+                    #     droputils.allDropContents()
+                    #     )
+                    pass
+                else:
+                    param = kwargs["applicationArgs"].get(attr_name).value
             else:
                 param = default_value
-            logger.debug(">>>!!! param extracted: %s; %s", attr_name, param)
             return param
 
         # Take a class dlg defined parameter class attribute and create an instanced attribute on object
         for attr_name, member in self._get_members():
             if isinstance(member, dlg_float_param):
                 value = get_param_value(attr_name, member.default_value)
                 if value is not None and value != "":
@@ -849,15 +866,15 @@
 
     @parent.setter
     @track_current_drop
     def parent(self, parent):
         if self._parent and parent:
             logger.warning(
                 "A parent is already set in %r, overwriting with new value",
-                self,
+                self.oid,
             )
         if parent:
             prevParent = self._parent
             self._parent = parent  # a parent is a container
             if hasattr(parent, "addChild") and self not in parent.children:
                 try:
                     parent.addChild(self)
@@ -906,29 +923,29 @@
                 "Consumer already registered as a streaming consumer",
             )
 
         # Add if not already present
         # Add the reverse reference too automatically
         if cuid in self._consumers_uids:
             return
-        logger.debug("Adding new consumer %r to %r", consumer, self)
+        # logger.debug("Adding new consumer %r to %r", consumer.oid, self.oid)
         self._consumers.append(consumer)
 
         # Subscribe the consumer to events sent when this DROP moves to
         # COMPLETED. This way the consumer will be notified that its input has
         # finished.
         # This only happens if this DROP's execution mode is 'DROP'; otherwise
         # an external entity will trigger the execution of the consumer at the
         # right time
         if self.executionMode == ExecutionMode.DROP:
             self.subscribe(consumer, "dropCompleted")
 
         # Automatic back-reference
         if back and hasattr(consumer, "addInput"):
-            logger.debug("Adding back %r as input of %r", self, consumer)
+            logger.debug("Adding back %r as input of %r", self.oid, consumer)
             consumer.addInput(self, False)
 
         # Add reproducibility subscription
         self.subscribe(consumer, "reproducibility")
 
     @property
     def producers(self):
```

### Comparing `daliuge-engine-2.4.0/dlg/droputils.py` & `daliuge-engine-3.0.0/dlg/droputils.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 import traceback
 from typing import Any, Tuple
 import numpy as np
 
 from dlg.ddap_protocol import DROPStates
 from dlg.data.io import IOForURL, OpenMode
 from dlg import common
-from dlg.common import DropType
 from dlg.apps.app_base import AppDROP
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from dlg.drop import AbstractDROP
     from dlg.apps.app_base import AppDROP
@@ -150,15 +149,15 @@
     logger.debug("Copying from %s to %s", repr(source), repr(target))
     sdesc = source.open()
     buf = source.read(sdesc, bufsize)
     logger.debug("Read %d bytes from %s", len(buf), repr(source))
     st = time.time()
     ssize = source.size if source.size is not None else -1
     logger.debug(
-        "Source size: %d; Source checksum: %d", ssize, source.checksum
+        "Source size: %s; Source checksum: %s", ssize, source.checksum
     )
     tot_w = 0
     ofl = True
     # target._expectedSize = ssize
     while buf:
         tot_w += target.write(buf)
         dur = int(time.time() - st)
@@ -232,15 +231,15 @@
     Returns a list of all the "leaf nodes" of the graph pointed by `drops`.
     `drops` is either a single DROP, or a list of DROPs.
     """
     drops = listify(drops)
     return [
         drop
         for drop, _ in breadFirstTraverse(drops)
-        if not getDownstreamObjects(drop) and drop.type != DropType.SERVICE_APP
+        if not getDownstreamObjects(drop) and drop.type != "dropclass"
     ]
 
 
 def depthFirstTraverse(node: "AbstractDROP", visited=[]):
     """
     Depth-first iterator for a DROP graph.
```

### Comparing `daliuge-engine-2.4.0/dlg/event.py` & `daliuge-engine-3.0.0/dlg/event.py`

 * *Files 7% similar despite different names*

```diff
@@ -69,33 +69,43 @@
 
     def __init__(self):
         # Union string key with object to handle __ALL_EVENTS above
         self._listeners: defaultdict[
             Union[str, object], list[EventHandler]
         ] = defaultdict(list)
 
-    def subscribe(self, listener: EventHandler, eventType: Optional[str] = None):
+    def subscribe(
+        self, listener: EventHandler, eventType: Optional[str] = None
+    ):
         """
         Subscribes `listener` to events fired by this object. If `eventType` is
         not `None` then `listener` will only receive events of `eventType` that
         originate from this object, otherwise it will receive all events.
         """
-        logger.debug(
-            "Adding listener to %r eventType=%s: %r", self, eventType, listener
-        )
+        # logger.debug(
+        #     "Adding listener to %r eventType=%s: %r",
+        #     self,
+        #     eventType,
+        #     listener,
+        # )
         eventType = eventType or EventFirer.__ALL_EVENTS
         self._listeners[eventType].append(listener)
 
-    def unsubscribe(self, listener: EventHandler, eventType: Optional[str] = None):
+    def unsubscribe(
+        self, listener: EventHandler, eventType: Optional[str] = None
+    ):
         """
         Unsubscribes `listener` from events fired by this object.
         """
         logger.debug(
-            "Removing listener to %r eventType=%s: %r", self, eventType, listener
-        )
+            "Removing listener to %r eventType=%s: %r",
+            self.oid,
+            eventType,
+            listener.oid,
+        ) if hasattr(listener, "oid") else None
 
         eventType = eventType or EventFirer.__ALL_EVENTS
         if listener in self._listeners[eventType]:
             self._listeners[eventType].remove(listener)
 
     def _fireEvent(self, eventType: str, **attrs):
         """
```

### Comparing `daliuge-engine-2.4.0/dlg/graph_loader.py` & `daliuge-engine-3.0.0/dlg/graph_loader.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,68 +23,41 @@
 Module containing functions to load a fully-functional DROP graph from its
 full JSON representation.
 """
 
 import collections
 import importlib
 import logging
-import json
-from xmlrpc.client import Boolean
 
 from dlg.common.reproducibility.constants import ReproducibilityFlags
 
 from . import droputils
 from .apps.socket_listener import SocketListenerApp
-from .common import Categories
 from .ddap_protocol import DROPRel, DROPLinkType
 from .drop import (
     AbstractDROP,
     LINKTYPE_NTO1_PROPERTY,
     LINKTYPE_1TON_APPEND_METHOD,
 )
-from .data.drops.data_base import NullDROP, EndDROP
+from .data.drops.data_base import NullDROP
 from .data.drops.container import ContainerDROP
 
 from dlg.data.drops.environmentvar_drop import EnvironmentVarDROP
 from dlg.data.drops.parset_drop import ParameterSetDROP
 from .exceptions import InvalidGraphException
 from dlg.data.drops.json_drop import JsonDROP
 from dlg.data.drops import *
-from .common import DropType
 
-try:
-    from .common import CategoryType
-except ImportError:
-
-    class CategoryType:
-        DATA = "dataclass"
-
-
-STORAGE_TYPES = {
-    Categories.MEMORY: InMemoryDROP,
-    Categories.SHMEM: SharedMemoryDROP,
-    Categories.FILE: FileDROP,
-    Categories.NGAS: NgasDROP,
-    Categories.NULL: NullDROP,
-    Categories.END: EndDROP,
-    Categories.JSON: JsonDROP,
-    Categories.PLASMA: PlasmaDROP,
-    Categories.PLASMAFLIGHT: PlasmaFlightDROP,
-    Categories.PARSET: ParameterSetDROP,
-    Categories.ENVIRONMENTVARS: EnvironmentVarDROP,
-}
-
-try:
-    from .data.drops.s3_drop import S3DROP
 
-    STORAGE_TYPES[Categories.S3] = S3DROP
-except ImportError:
-    pass
+class CategoryType:
+    DATA = "dropclass"
 
     # Dictionary for the key used to store 1-to-N relationships between DROPs
+
+
 # in the the DROP specification format
 __TOMANY = {
     DROPLinkType.CONSUMER: "consumers",
     DROPLinkType.STREAMING_CONSUMER: "streamingConsumers",
     DROPLinkType.INPUT: "inputs",
     DROPLinkType.STREAMING_INPUT: "streamingInputs",
     DROPLinkType.OUTPUT: "outputs",
@@ -151,43 +124,42 @@
     for dropSpec in dropSpecList:
         oid = normalise_oid(dropSpec["oid"])
         oids.add(oid)
 
     # Step #2: find unmet relationships and remove them from the original
     # DROP spec, keeping track of them
     for dropSpec in dropSpecList:
-
         this_oid = normalise_oid(dropSpec["oid"])
         to_delete = []
 
         for rel in dropSpec:
-
             # 1-N relationships
             if rel in __TOMANY:
-
                 link = __TOMANY[rel]
 
                 # Find missing OIDs in this relationship and keep track of them,
                 # removing them from the current DROP spec
                 ds = dropSpec[rel]
+                # TODO: In principle all of the ds should be dicts, but they are not
+                # in a loop. Need to check the generation
+                # ds = [next(iter(d)) if isinstance(d, dict) else d for d in ds]
                 if isinstance(ds[0], dict):
                     ds = [next(iter(d)) for d in ds]
                 #                ds = [normalise_oid(d) for d in ds]
                 missingOids = [oid for oid in ds if oid not in oids]
                 for oid in missingOids:
                     unmetRelationships.append(DROPRel(oid, link, this_oid))
                     ds.remove(oid)
 
                 # Remove the relationship list entirely if it has no elements
                 if not ds:
                     to_delete.append(rel)
 
             # N-1 relationships
             elif rel in __TOONE:
-
                 link = __TOONE[rel]
 
                 # Check if OID is missing
                 oid = normalise_oid(dropSpec[rel])
                 if oid in oids:
                     continue
 
@@ -204,17 +176,17 @@
 
 
 def check_dropspec(n, dropSpec):
     if "oid" not in dropSpec:
         raise InvalidGraphException(
             "Drop #%d is missing its 'oid' argument: %r" % (n, dropSpec)
         )
-    if "type" not in dropSpec:
+    if "categoryType" not in dropSpec:
         raise InvalidGraphException(
-            "Drop %s is missing its 'type' argument" % (dropSpec["oid"])
+            "Drop %s is missing its 'categoryType' argument" % (dropSpec)
         )
 
 
 def loadDropSpecs(dropSpecList):
     """
     Loads the DROP definitions from `dropSpectList`, checks that
     the DROPs are correctly specified, and return a dictionary containing
@@ -229,34 +201,31 @@
     dropSpecs = {}
     reprodata = None
     if dropSpecList is None:
         raise InvalidGraphException("DropSpec is empty %r" % dropSpecList)
     if dropSpecList[-1].get("rmode"):
         reprodata = dropSpecList.pop()
     for n, dropSpec in enumerate(dropSpecList):
-
-        # "type" and 'oid' are mandatory
+        # "categoryType" and 'oid' are mandatory
         check_dropspec(n, dropSpec)
-        dropType = dropSpec["type"]
+        dropType = dropSpec["categoryType"].lower()
 
         cf = __CREATION_FUNCTIONS[dropType]
         cf(dropSpec, dryRun=True)
         dropSpecs[dropSpec["oid"]] = dropSpec
 
     logger.debug("Found %d DROP definitions", len(dropSpecs))
 
     # Step #2: check relationships
     # TODO: shouldn't this loop be done the other way around, going through all __TOMANY
     # and __TOONE and directly address the respective dropSpec attribute?
     for dropSpec in dropSpecList:
-
         # 1-N relationships
         for rel in dropSpec:
             if rel in __TOMANY:
-
                 # A KeyError will be raised if a oid has been specified in the
                 # relationship list but doesn't exist in the list of DROPs
                 for oid in dropSpec[rel]:
                     oid = list(oid.keys())[0] if isinstance(oid, dict) else oid
                     dropSpecs[oid]
 
             # N-1 relationships
@@ -276,33 +245,36 @@
 def createGraphFromDropSpecList(dropSpecList, session=None):
     logger.debug("Found %d DROP definitions", len(dropSpecList))
 
     # Step #1: create the actual DROPs
     drops = collections.OrderedDict()
     logger.info("Creating %d drops", len(dropSpecList))
     for n, dropSpec in enumerate(dropSpecList):
-
         check_dropspec(n, dropSpec)
-        #        dropType = dropSpec.pop("type")
-        dropType = dropSpec["type"]
+        #        dropType = dropSpec.pop("categoryType")
+        # backwards compatibility
+        dropType = dropSpec["categoryType"]
+        # if dropType.lower() in ["application", "app"]:
+        #     dropType = "dropclass"
+        # if dropType.lower() == "data":
+        #     dropType = "dropclass"
 
-        cf = __CREATION_FUNCTIONS[dropType]
+        cf = __CREATION_FUNCTIONS[dropType.lower()]
         drop = cf(dropSpec, session=session)
         if session is not None:
             # Now using per-drop reproducibility setting.
             drop.reproducibility_level = ReproducibilityFlags(
                 int(dropSpec.get("reprodata", {}).get("rmode", "0"))
             )
             # session.reprodata['rmode']
         drops[drop.oid] = drop
 
     # Step #2: establish relationships
     logger.info("Establishing relationships between drops")
     for dropSpec in dropSpecList:
-
         # 'oid' is mandatory
         oid = dropSpec["oid"]
         drop = drops[oid]
 
         for attr in dropSpec:
             # 1-N relationships
             if attr in __TOMANY:
@@ -335,49 +307,70 @@
     # We're done! Return the roots of the graph to the caller
     logger.info("Calculating graph roots")
     roots: list[AbstractDROP] = []
     for drop in drops.values():
         if not droputils.getUpstreamObjects(drop):
             roots.append(drop)
     logger.info("%d graph roots found, bye-bye!", len(roots))
-    logger.debug("Graph spec: %s", drops.values())
 
     return roots
 
 
 def _createData(dropSpec, dryRun=False, session=None):
     oid, uid = _getIds(dropSpec)
     kwargs = _getKwargs(dropSpec)
 
-    if DropType.DATACLASS in dropSpec:
-        dataClassName = dropSpec[DropType.DATACLASS]
+    if dropSpec["categoryType"] == "Data":
+        dataClassName = dropSpec["dropclass"]
         parts = dataClassName.split(".")
-        # we don't need to support dfms here
         module = importlib.import_module(".".join(parts[:-1]))
         storageType = getattr(module, parts[-1])
     else:
+        # STORAGE_TYPES are deprecated, but here for backwards compatibility
+
         # Fall back to old behaviour or to FileDROP
         # if nothing else is specified
+        STORAGE_TYPES = {
+            "Memory": InMemoryDROP,
+            "SharedMemory": SharedMemoryDROP,
+            "File": FileDROP,
+            "NGAS": NgasDROP,
+            "null": NullDROP,
+            "json": JsonDROP,
+            "Plasma": PlasmaDROP,
+            "PlasmaFlight": PlasmaFlightDROP,
+            "ParameterSet": ParameterSetDROP,
+            "EnvironmentVariables": EnvironmentVarDROP,
+        }
+
+        try:
+            from .data.drops.s3_drop import S3DROP
+
+            STORAGE_TYPES["S3"] = S3DROP
+        except ImportError:
+            pass
         if "storage" in dropSpec:
             storageType = STORAGE_TYPES[dropSpec["storage"]]
+            # pass
         else:
             storageType = FileDROP
     if dryRun:
         return
-
+    if "self" in kwargs:
+        kwargs.pop("self")
     return storageType(oid, uid, dlg_session=session, **kwargs)
 
 
 def _createContainer(dropSpec, dryRun=False, session=None):
     oid, uid = _getIds(dropSpec)
     kwargs = _getKwargs(dropSpec)
 
     # if no 'container' is specified, we default to ContainerDROP
-    if DropType.CONTAINER in dropSpec:
-        containerTypeName = dropSpec[DropType.CONTAINER]
+    if "dropclass" in dropSpec:
+        containerTypeName = dropSpec["dropclass"]
         parts = containerTypeName.split(".")
 
         # Support old "dfms..." package names (pre-Oct2017)
         if parts[0] == "dfms":
             parts[0] = "dlg"
 
         module = importlib.import_module(".".join(parts[:-1]))
@@ -400,25 +393,28 @@
     return SocketListenerApp(oid, uid, dlg_session=session, **kwargs)
 
 
 def _createApp(dropSpec, dryRun=False, session=None):
     oid, uid = _getIds(dropSpec)
     kwargs = _getKwargs(dropSpec)
 
-    appName = dropSpec[DropType.APP]
+    if "dropclass" in dropSpec:
+        appName = dropSpec["dropclass"]
+    elif "Application" in dropSpec:
+        appName = dropSpec["Application"]
     parts = appName.split(".")
 
     # Support old "dfms..." package names (pre-Oct2017)
     if parts[0] == "dfms":
         parts[0] = "dlg"
 
     try:
         module = importlib.import_module(".".join(parts[:-1]))
         appType = getattr(module, parts[-1])
-    except (ImportError, AttributeError):
+    except (ImportError, AttributeError, ValueError):
         raise InvalidGraphException(
             "drop %s specifies non-existent application: %s" % (oid, appName)
         )
 
     if dryRun:
         return
     return appType(oid, uid, dlg_session=session, **kwargs)
@@ -435,16 +431,20 @@
 
 def _getKwargs(dropSpec):
     kwargs = dict(dropSpec)
 
     REMOVE = [
         "oid",
         "uid",
-        "app",
+        "Application",
+        "dropclass",
         "appclass",
+        "dataclass",
+        "data",
+        "Data",
     ]
     for kw in REMOVE:
         if kw in kwargs:
             del kwargs[kw]
 
     RENAME = {
         "precious": "persist",
@@ -457,15 +457,13 @@
     for name, spec in dropSpec.get("applicationArgs", dict()).items():
         kwargs[name] = spec["value"]
 
     return kwargs
 
 
 __CREATION_FUNCTIONS = {
-    DropType.DATA: _createData,
-    DropType.CONTAINER: _createContainer,
-    DropType.APP: _createApp,
-    DropType.SERVICE_APP: _createApp,
-    DropType.SOCKET: _createSocket,
-    "dataclass": _createData,
-    "appclass": _createApp,
+    "socket": _createSocket,
+    "data": _createData,
+    "application": _createApp,
+    "app": _createApp,
+    "container": _createContainer,
 }
```

### Comparing `daliuge-engine-2.4.0/dlg/lifecycle/__init__.py` & `daliuge-engine-3.0.0/dlg/lifecycle/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/lifecycle/dlm.py` & `daliuge-engine-3.0.0/dlg/lifecycle/dlm.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/lifecycle/hsm/__init__.py` & `daliuge-engine-3.0.0/dlg/lifecycle/hsm/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/lifecycle/hsm/manager.py` & `daliuge-engine-3.0.0/dlg/lifecycle/hsm/manager.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/lifecycle/hsm/store.py` & `daliuge-engine-3.0.0/dlg/lifecycle/hsm/store.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/lifecycle/registry.py` & `daliuge-engine-3.0.0/dlg/lifecycle/registry.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/manager/__init__.py` & `daliuge-engine-3.0.0/dlg/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/manager/client.py` & `daliuge-engine-3.0.0/dlg/manager/client.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/manager/cmdline.py` & `daliuge-engine-3.0.0/dlg/manager/cmdline.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,19 @@
     NODE_DEFAULT_REST_PORT,
     ISLAND_DEFAULT_REST_PORT,
     MASTER_DEFAULT_REST_PORT,
     REPLAY_DEFAULT_REST_PORT,
 )
 from .node_manager import NodeManager
 from .replay import ReplayManager, ReplayManagerServer
-from .rest import NMRestServer, CompositeManagerRestServer, MasterManagerRestServer
+from .rest import (
+    NMRestServer,
+    CompositeManagerRestServer,
+    MasterManagerRestServer,
+)
 from .. import utils
 from ..runtime import version
 
 
 _terminating = False
 
 
@@ -59,26 +63,28 @@
             if field not in record.__dict__:
                 record.__dict__[field] = None
 
         return super().format(record)
 
 
 def launchServer(opts):
-
     # we might be called via __main__, but we want a nice logger name
     logger = logging.getLogger(__name__)
     dmName = opts.dmType.__name__
 
-    logger.info("DALiuGE version %s running at %s", version.full_version, os.getcwd())
+    logger.info(
+        "DALiuGE version %s running at %s", version.full_version, os.getcwd()
+    )
     logger.info("Creating %s", dmName)
     try:
         dm = opts.dmType(*opts.dmArgs, **opts.dmKwargs)
     except:
         logger.exception(
-            "Error while creating/starting our %s, exiting in shame :-(", dmName
+            "Error while creating/starting our %s, exiting in shame :-(",
+            dmName,
         )
         return
 
     server = opts.restType(dm, opts.maxreqsize)
 
     # Signal handling
     def handle_signal(signNo, stack_frame):
@@ -129,15 +135,19 @@
         "--daemon",
         action="store_true",
         dest="daemon",
         help="Run as daemon",
         default=False,
     )
     parser.add_option(
-        "--cwd", action="store_true", dest="cwd", help="Short for '-w .'", default=False
+        "--cwd",
+        action="store_true",
+        dest="cwd",
+        help="Short for '-w .'",
+        default=False,
     )
     parser.add_option(
         "-w",
         "--work-dir",
         help="Working directory, defaults to DLG_ROOT/workspace in daemon mode, '.' in interactive mode",
         default=utils.getDlgWorkDir(),
     )
@@ -198,28 +208,28 @@
         parser.error("-d and --status cannot be specified together")
     if options.stop and options.status:
         parser.error("-s and --status cannot be specified together")
     # -v and -q are exclusive
     if options.verbose and options.quiet:
         parser.error("-v and -q cannot be specified together")
     if options.cwd and options.work_dir:
-        parser.error("--cwd and -w/--work-dir cannot be specified together. Prefer -w")
+        parser.error(
+            "--cwd and -w/--work-dir cannot be specified together. Prefer -w"
+        )
 
 
 def start(options, parser):
-
     # Perform common option checks
     commonOptionsCheck(options, parser)
 
     # Setup the loggers
     fileHandler = setupLogging(options)
 
     # Start daemon?
     if options.daemon:
-
         # Make sure the PID file will be created without problems
         pidDir = utils.getDlgPidDir()
         utils.createDirIfMissing(pidDir)
         pidfile = os.path.join(pidDir, "dlg%s.pid" % (options.dmAcronym))
 
         working_dir = options.work_dir
         if not working_dir:
@@ -239,15 +249,17 @@
 
     # Stop daemon?
     elif options.stop:
         pidDir = utils.getDlgPidDir()
         pidfile = os.path.join(pidDir, "dlg%s.pid" % (options.dmAcronym))
         pid = PIDLockFile(pidfile).read_pid()
         if pid is None:
-            sys.stderr.write("Cannot read PID file, is there an instance running?\n")
+            sys.stderr.write(
+                "Cannot read PID file, is there an instance running?\n"
+            )
         else:
             utils.terminate_or_kill(utils.ExistingProcess(pid), 5)
             if os.path.exists(pidfile):
                 sys.stderr.write(
                     "Process %d does not exist, removing PID file\n" % (pid,)
                 )
                 os.unlink(pidfile)
@@ -295,15 +307,17 @@
 
     # Output to files/stdout uses a command format, which can or not contain
     # optionally a session_id and drop_uid to indicate what is currently being
     # executed. This only applies to the NodeManager logs though, for which a
     # 'no_log_ids' option exists (but can be set to True).
     # We also skip logging IDs when stopping a daemon, as the infrastructure
     # won't have been set
-    log_ids = opts.dmType == NodeManager and not opts.no_log_ids and not opts.stop
+    log_ids = (
+        opts.dmType == NodeManager and not opts.no_log_ids and not opts.stop
+    )
     fmt = "%(asctime)-15s [%(levelname)5.5s] [%(threadName)15.15s] "
     if log_ids:
         fmt += "[%(session_id)10.10s] [%(drop_uid)10.10s] "
     fmt += "%(name)s#%(funcName)s:%(lineno)s %(message)s"
     fmt = DlgFormatter(fmt)
     # fmt = logging.Formatter(fmt)
     fmt.converter = time.gmtime
@@ -352,21 +366,21 @@
         dest="noDLM",
         help="(DEPRECATED) Don't start the Data Lifecycle Manager on this NodeManager",
     )
     parser.add_option(
         "--dlm-check-period",
         type="float",
         help="Time in seconds between background DLM drop status checks (defaults to 10)",
-        default=10
+        default=10,
     )
     parser.add_option(
         "--dlm-cleanup-period",
         type="float",
         help="Time in seconds between background DLM drop automatic cleanups (defaults to 30)",
-        default=30
+        default=30,
     )
     parser.add_option(
         "--dlm-enable-replication",
         action="store_true",
         help="Turn on data drop automatic replication (off by default)",
     )
     parser.add_option(
@@ -402,15 +416,17 @@
         help="Max thread pool size used for executing drops. -1 means use all CPUs. 0 (default) means no threads.",
         default=0,
     )
     (options, args) = parser.parse_args(args)
 
     # No logging setup at this point yet
     if options.noDLM:
-        print("WARNING: --no-dlm is deprecated, use the --dlm-* options instead")
+        print(
+            "WARNING: --no-dlm is deprecated, use the --dlm-* options instead"
+        )
         options.dlm_check_period = 0
         options.dlm_cleanup_period = 0
         options.dlm_enable_replication = False
 
     # Add DM-specific options
     # Note that the host we use to expose the NodeManager itself through Pyro is
     # also used to expose the Sessions it creates
@@ -419,15 +435,17 @@
     options.dmKwargs = {
         "dlm_check_period": options.dlm_check_period,
         "dlm_cleanup_period": options.dlm_cleanup_period,
         "dlm_enable_replication": options.dlm_enable_replication,
         "dlgPath": options.dlgPath,
         "host": options.host,
         "error_listener": options.errorListener,
-        "event_listeners": list(filter(None, options.event_listeners.split(":"))),
+        "event_listeners": list(
+            filter(None, options.event_listeners.split(":"))
+        ),
         "max_threads": options.max_threads,
         "logdir": options.logdir,
     }
     options.dmAcronym = "NM"
     options.restType = NMRestServer
 
     start(options, parser)
@@ -444,15 +462,16 @@
     addCommonOptions(parser, dmPort)
     parser.add_option(
         "-N",
         "--nodes",
         action="store",
         type="string",
         dest="nodes",
-        help="Comma-separated list of node names managed by this %s" % (acronym),
+        help="Comma-separated list of node names managed by this %s"
+        % (acronym),
         default="",
     )
     parser.add_option(
         "-k",
         "--ssh-pkey-path",
         action="store",
         type="string",
```

### Comparing `daliuge-engine-2.4.0/dlg/manager/composite_manager.py` & `daliuge-engine-3.0.0/dlg/manager/composite_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,19 @@
 from . import constants
 from .client import NodeManagerClient
 from .constants import ISLAND_DEFAULT_REST_PORT, NODE_DEFAULT_REST_PORT
 from .drop_manager import DROPManager
 from .. import graph_loader
 from ..common.reproducibility.reproducibility import init_pg_repro_data
 from ..ddap_protocol import DROPRel
-from ..exceptions import InvalidGraphException, DaliugeException, SubManagerException
+from ..exceptions import (
+    InvalidGraphException,
+    DaliugeException,
+    SubManagerException,
+)
 from ..utils import portIsOpen
 
 logger = logging.getLogger(__name__)
 
 
 def uid_for_drop(dropSpec):
     if "uid" in dropSpec:
@@ -123,21 +127,21 @@
     CompositeManager to partition the graph (from its graphSpec) is given at
     construction time.
     """
 
     __metaclass__ = abc.ABCMeta
 
     def __init__(
-            self,
-            dmPort,
-            partitionAttr,
-            subDmId,
-            dmHosts=[],
-            pkeyPath=None,
-            dmCheckTimeout=10,
+        self,
+        dmPort,
+        partitionAttr,
+        subDmId,
+        dmHosts=[],
+        pkeyPath=None,
+        dmCheckTimeout=10,
     ):
         """
         Creates a new CompositeManager. The sub-DMs it manages are to be located
         at `dmHosts`, and should be listening on port `dmPort`.
 
         :param: dmPort The port at which the sub-DMs expose themselves
         :param: partitionAttr The attribute on each dropSpec that specifies the
@@ -232,15 +236,14 @@
     def check_dm(self, host, port=None, timeout=10):
         port = port or self._dmPort
         logger.debug("Checking DM presence at %s:%d", host, port)
         dm_is_there = portIsOpen(host, port, timeout)
         return dm_is_there
 
     def dmAt(self, host, port=None):
-
         if not self.check_dm(host, port):
             raise SubManagerException(
                 f"Manager expected but not running in {host}:{port}"
             )
 
         port = port or self._dmPort
         return NodeManagerClient(host, port, 10)
@@ -249,16 +252,17 @@
         return self._sessionIds
 
     #
     # Replication of commands to underlying drop managers
     # If "collect" is given, then individual results are also kept in the given
     # structure, which is either a dictionary or a list
     #
-    def _do_in_host(self, action, sessionId, exceptions, f, collect, port, iterable):
-
+    def _do_in_host(
+        self, action, sessionId, exceptions, f, collect, port, iterable
+    ):
         host = iterable
         if isinstance(iterable, (list, tuple)):
             host = iterable[0]
 
         try:
             with self.dmAt(host, port) as dm:
                 res = f(dm, iterable, sessionId)
@@ -267,18 +271,23 @@
                 collect.update(res)
             elif isinstance(collect, list):
                 collect.append(res)
 
         except Exception as e:
             exceptions[host] = e
             logger.exception(
-                "Error while %s on host %s, session %s", action, host, sessionId
+                "Error while %s on host %s, session %s",
+                action,
+                host,
+                sessionId,
             )
 
-    def replicate(self, sessionId, f, action, collect=None, iterable=None, port=None):
+    def replicate(
+        self, sessionId, f, action, collect=None, iterable=None, port=None
+    ):
         """
         Replicates the given function call on each of the underlying drop managers
         """
         thrExs = {}
         iterable = iterable or self._dmHosts
         port = port or self._dmPort
         self._tp.map(
@@ -305,87 +314,103 @@
         logger.info("Creating Session %s in all hosts", sessionId)
         self.replicate(sessionId, self._createSession, "creating sessions")
         logger.info("Successfully created session %s in all hosts", sessionId)
         self._sessionIds.append(sessionId)
 
     def _cancelSession(self, dm, host, sessionId):
         dm.cancelSession(sessionId)
-        logger.debug("Successfully cancelled session %s on %s", sessionId, host)
+        logger.debug(
+            "Successfully cancelled session %s on %s", sessionId, host
+        )
 
     def cancelSession(self, sessionId):
         """
         Cancels a session in all underlying DMs.
         """
         logger.info("Cancelled session %s in all hosts", sessionId)
         self.replicate(sessionId, self._cancelSession, "cancelling sessions")
 
     def _destroySession(self, dm, host, sessionId):
         dm.destroySession(sessionId)
-        logger.debug("Successfully destroyed session %s on %s", sessionId, host)
+        logger.debug(
+            "Successfully destroyed session %s on %s", sessionId, host
+        )
 
     def destroySession(self, sessionId):
         """
         Destroy a session in all underlying DMs.
         """
         logger.info("Destroying Session %s in all hosts", sessionId)
         self.replicate(sessionId, self._destroySession, "creating sessions")
         self._sessionIds.remove(sessionId)
 
     def _add_node_subscriptions(self, dm, host_and_subscriptions, sessionId):
         host, subscriptions = host_and_subscriptions
         dm.add_node_subscriptions(sessionId, subscriptions)
         logger.debug(
-            "Successfully added relationship info to session %s on %s", sessionId, host
+            "Successfully added relationship info to session %s on %s",
+            sessionId,
+            host,
         )
 
     def _addGraphSpec(self, dm, host_and_graphspec, sessionId):
         host, graphSpec = host_and_graphspec
         dm.addGraphSpec(sessionId, graphSpec)
-        logger.info("Successfully appended graph to session %s on %s", sessionId, host)
+        logger.info(
+            "Successfully appended graph to session %s on %s", sessionId, host
+        )
 
     def addGraphSpec(self, sessionId, graphSpec):
-
         # The first step is to break down the graph into smaller graphs that
         # belong to the same host, so we can submit that graph into the individual
         # DMs. For this we need to make sure that our graph has a the correct
         # attribute set
-        logger.info("Separating graph using partition attribute %s", self._partitionAttr)
+        logger.info(
+            "Separating graph using partition attribute %s",
+            self._partitionAttr,
+        )
         perPartition = collections.defaultdict(list)
         if "rmode" in graphSpec[-1]:
             init_pg_repro_data(graphSpec)
             self._graph["reprodata"] = graphSpec.pop()
             logger.debug(
                 "Composite manager found reprodata in dropspecList, rmode=%s",
                 self._graph["reprodata"]["rmode"],
             )
         if graphSpec[-1] == {}:
             graphSpec.pop()
         for dropSpec in graphSpec:
             if self._partitionAttr not in dropSpec:
-                msg = f"Drop {dropSpec.get('oid', None)} doesn't specify a {self._partitionAttr} " \
-                      f"attribute"
+                msg = (
+                    f"Drop {dropSpec.get('oid', None)} doesn't specify a {self._partitionAttr} "
+                    f"attribute"
+                )
                 raise InvalidGraphException(msg)
 
             partition = dropSpec[self._partitionAttr]
             if partition not in self._dmHosts:
-                msg = f"Drop {dropSpec.get('oid', None)}'s {self._partitionAttr} {partition} " \
-                      f"does not belong to this DM"
+                msg = (
+                    f"Drop {dropSpec.get('oid', None)}'s {self._partitionAttr} {partition} "
+                    f"does not belong to this DM"
+                )
                 raise InvalidGraphException(msg)
 
             perPartition[partition].append(dropSpec)
 
             # Add the drop specs to our graph
             self._graph[uid_for_drop(dropSpec)] = dropSpec
         # At each partition the relationships between DROPs should be local at the
         # moment of submitting the graph; thus we record the inter-partition
         # relationships separately and remove them from the original graph spec
         logger.info("Graph split into %r", perPartition.keys())
         inter_partition_rels = []
         for dropSpecs in perPartition.values():
-            inter_partition_rels += graph_loader.removeUnmetRelationships(dropSpecs)
+            inter_partition_rels += graph_loader.removeUnmetRelationships(
+                dropSpecs
+            )
         sanitize_relations(inter_partition_rels, self._graph)
         logger.info(
             "Removed (and sanitized) %d inter-dm relationships",
             len(inter_partition_rels),
         )
 
         # Store the inter-partition relationships; later on they have to be
@@ -400,15 +425,17 @@
             drop_rels[rhn][lhn].append(rel)
 
         self._drop_rels[sessionId] = drop_rels
         logger.debug("Calculated NM-level drop relationships: %r", drop_rels)
 
         # Create the individual graphs on each DM now that they are correctly
         # separated.
-        logger.info("Adding individual graphSpec of session %s to each DM", sessionId)
+        logger.info(
+            "Adding individual graphSpec of session %s to each DM", sessionId
+        )
         for partition in perPartition:
             if self._graph.get("reprodata") is not None:
                 perPartition[partition].append(self._graph["reprodata"])
         self.replicate(
             sessionId,
             self._addGraphSpec,
             "appending graphSpec to individual DMs",
@@ -423,32 +450,34 @@
         dm.deploySession(sessionId)
         logger.debug("Successfully deployed session %s on %s", sessionId, host)
 
     def _triggerDrops(self, dm, host_and_uids, sessionId):
         host, uids = host_and_uids
         dm.trigger_drops(sessionId, uids)
         logger.info(
-            "Successfully triggered drops for session %s on %s", sessionId, host
+            "Successfully triggered drops for session %s on %s",
+            sessionId,
+            host,
         )
 
     def deploySession(self, sessionId, completedDrops=[]):
-
         # Indicate the node managers that they have to subscribe to events
         # published by some nodes
         if self._drop_rels.get(sessionId, None):
             self.replicate(
                 sessionId,
                 self._add_node_subscriptions,
                 "adding relationship information",
                 port=constants.NODE_DEFAULT_REST_PORT,
                 iterable=self._drop_rels[sessionId].items(),
             )
             logger.info("Delivered node subscription list to node managers")
             logger.debug(
-                "Number of subscriptions: %s", len(self._drop_rels[sessionId].items())
+                "Number of subscriptions: %s",
+                len(self._drop_rels[sessionId].items()),
             )
 
         logger.info("Deploying Session %s in all hosts", sessionId)
         self.replicate(sessionId, self._deploySession, "deploying session")
         logger.info("Successfully deployed session %s in all hosts", sessionId)
 
         # Now that everything is wired up we move the requested DROPs to COMPLETED
@@ -456,15 +485,17 @@
         # we would certainly miss most of the events)
         if completedDrops:
             not_found = set(completedDrops) - set(self._graph)
             if not_found:
                 raise DaliugeException(
                     "UIDs for completed drops not found: %r", not_found
                 )
-            logger.info("Moving Drops to COMPLETED right away: %r", completedDrops)
+            logger.info(
+                "Moving Drops to COMPLETED right away: %r", completedDrops
+            )
             completed_by_host = group_by_node(completedDrops, self._graph)
             self.replicate(
                 sessionId,
                 self._triggerDrops,
                 "triggering drops",
                 port=constants.NODE_DEFAULT_REST_PORT,
                 iterable=completed_by_host.items(),
@@ -473,23 +504,25 @@
 
     def _getGraphStatus(self, dm, host, sessionId):
         return dm.getGraphStatus(sessionId)
 
     def getGraphStatus(self, sessionId):
         allStatus = {}
         self.replicate(
-            sessionId, self._getGraphStatus, "getting graph status", collect=allStatus
+            sessionId,
+            self._getGraphStatus,
+            "getting graph status",
+            collect=allStatus,
         )
         return allStatus
 
     def _getGraph(self, dm, host, sessionId):
         return dm.getGraph(sessionId)
 
     def getGraph(self, sessionId):
-
         allGraphs = {}
         self.replicate(
             sessionId, self._getGraph, "getting the graph", collect=allGraphs
         )
 
         # The graphs coming from the DMs are not interconnected, we need to
         # add the missing connections to the graph before returning upstream
@@ -521,29 +554,32 @@
 
     def _getGraphSize(self, dm, host, sessionId):
         return dm.getGraphSize(sessionId)
 
     def getGraphSize(self, sessionId):
         allCounts = []
         self.replicate(
-            sessionId, self._getGraphSize, "getting the graph size", collect=allCounts
+            sessionId,
+            self._getGraphSize,
+            "getting the graph size",
+            collect=allCounts,
         )
         return sum(allCounts)
 
 
 class DataIslandManager(CompositeManager):
     """
     The DataIslandManager, which manages a number of NodeManagers.
     """
 
     def __init__(self, dmHosts=[], pkeyPath=None, dmCheckTimeout=10):
         super(DataIslandManager, self).__init__(
             NODE_DEFAULT_REST_PORT,
             "node",
-            "nm",
+            "nm",  # Node manager
             dmHosts=dmHosts,
             pkeyPath=pkeyPath,
             dmCheckTimeout=dmCheckTimeout,
         )
 
         # In the case of the Data Island the dmHosts are the final nodes as well
         self._nodes = dmHosts
```

### Comparing `daliuge-engine-2.4.0/dlg/manager/constants.py` & `daliuge-engine-3.0.0/dlg/manager/constants.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/manager/drop_manager.py` & `daliuge-engine-3.0.0/dlg/manager/drop_manager.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/manager/node_manager.py` & `daliuge-engine-3.0.0/dlg/manager/node_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         self._nm.publish_event(event)
 
 
 class LogEvtListener(object):
     def handleEvent(self, event):
         if event.type == "status":
             logger.debug(
-                "Drop uid=%s, oid=%s changed to state %s",
+                "Data Drop uid=%s, oid=%s changed to state %s",
                 event.uid,
                 event.oid,
                 event.status,
             )
         elif event.type == "execStatus":
             logger.debug(
                 "AppDrop uid=%s, oid=%s changed to execState %s",
@@ -135,15 +135,14 @@
         dlm_enable_replication=False,
         dlgPath=None,
         error_listener=None,
         event_listeners=[],
         max_threads=0,
         logdir=utils.getDlgLogsDir(),
     ):
-
         self._dlm = DataLifecycleManager(
             check_period=dlm_check_period,
             cleanup_period=dlm_cleanup_period,
             enable_drop_replication=dlm_enable_replication,
         )
         self._sessions = {}
         self.logdir = logdir
@@ -336,22 +335,20 @@
             target=self._sessions[sessionId].trigger_drops,
             name="Drop trigger",
             args=(uids,),
         )
         t.start()
 
     def add_node_subscriptions(self, sessionId, relationships):
-
         logger.debug("Received subscription information: %r", relationships)
         self._check_session_id(sessionId)
         self._sessions[sessionId].add_node_subscriptions(relationships)
 
         # Set up event channels subscriptions
         for nodesub in relationships:
-
             host = nodesub
             events_port = constants.NODE_DEFAULT_EVENTS_PORT
             if type(nodesub) is tuple:
                 host, events_port, _ = nodesub
 
             # TODO: we also have to unsubscribe from them at some point
             self.subscribe(host, events_port)
@@ -467,15 +464,14 @@
             self._events_port,
         )
         pub.bind(endpoint)
         logger.info("Publishing events via ZeroMQ on %s", endpoint)
         sock_created.set()
 
         while self._pubsub_running:
-
             try:
                 obj = self._events_out.get_nowait()
             except queue.Empty:
                 time.sleep(0.01)
                 continue
 
             while self._pubsub_running:
@@ -506,15 +502,14 @@
         sub_endpoints = set()
         sub.setsockopt(zmq.SUBSCRIBE, b"")  # @UndefinedVariable
         sub_monitor = sub.get_monitor_socket()
         sock_created.set()
 
         pending_connections = {}
         while self._pubsub_running:
-
             # A new subscription has been requested
             try:
                 subscription = self._subscriptions.get_nowait()
                 if subscription.endpoint in sub_endpoints:
                     subscription.finished_evt.set()
                 else:
                     sub.connect(subscription.endpoint)
```

### Comparing `daliuge-engine-2.4.0/dlg/manager/proc_daemon.py` & `daliuge-engine-3.0.0/dlg/manager/proc_daemon.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/manager/replay.py` & `daliuge-engine-3.0.0/dlg/manager/replay.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/manager/rest.py` & `daliuge-engine-3.0.0/dlg/manager/rest.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,20 +76,22 @@
 
             if res is not None:
                 bottle.response.content_type = "application/json"
                 # set CORS headers
                 origin = bottle.request.headers.raw("Origin")
                 if origin is None:
                     origin = "http://localhost:8084"
-                elif not re.match(r"http://((localhost)|(127.0.0.1)):80[0-9][0-9]", origin):
+                elif not re.match(
+                    r"http://((localhost)|(127.0.0.1)):80[0-9][0-9]", origin
+                ):
                     origin = "http://localhost:8084"
+                bottle.response.headers["Access-Control-Allow-Origin"] = origin
                 bottle.response.headers[
-                    "Access-Control-Allow-Origin"
-                ] = origin
-                bottle.response.headers["Access-Control-Allow-Credentials"] = "true"
+                    "Access-Control-Allow-Credentials"
+                ] = "true"
                 bottle.response.headers[
                     "Access-Control-Allow-Methods"
                 ] = "GET, POST, PUT, OPTIONS"
                 bottle.response.headers[
                     "Access-Control-Allow-Headers"
                 ] = "Origin, Accept, Content-Type, Content-Encoding, X-Requested-With, X-CSRF-Token"
             return json.dumps(res)
@@ -114,15 +116,18 @@
             elif isinstance(e, RestClientException):
                 status, eargs = 556, e.args
             elif isinstance(e, SubManagerException):
                 status = 555
                 eargs = {}
                 # args[1] is a dictionary of host:exception
                 for host, subex in e.args[1].items():
-                    eargs[host] = {"type": subex.__class__.__name__, "args": subex.args}
+                    eargs[host] = {
+                        "type": subex.__class__.__name__,
+                        "args": subex.args,
+                    }
             elif isinstance(e, DaliugeException):
                 status, eargs = 555, e.args
             else:
                 raise
 
             error = {"type": e.__class__.__name__, "args": eargs}
             bottle.response.status = status
@@ -138,47 +143,65 @@
     and runs until the process is shut down.
 
     This REST server currently also serves HTML pages in some of its methods
     (i.e. those not under /api).
     """
 
     def __init__(self, dm, maxreqsize=10):
-
         super(ManagerRestServer, self).__init__()
 
         # Increase maximum file sizes
         bottle.BaseRequest.MEMFILE_MAX = maxreqsize * 1024 * 1024
 
         self.dm = dm
 
         # Mappings
         app = self.app
         app.get("/api/submission_method", callback=self.submit_methods)
         app.post("/api/stop", callback=self.stop_manager)
         app.post("/api/sessions", callback=self.createSession)
         app.get("/api/sessions", callback=self.getSessions)
-        app.get("/api/sessions/<sessionId>", callback=self.getSessionInformation)
+        app.get(
+            "/api/sessions/<sessionId>", callback=self.getSessionInformation
+        )
         app.delete("/api/sessions/<sessionId>", callback=self.destroySession)
         app.get("/api/sessions/<sessionId>/logs", callback=self.getLogFile)
-        app.get("/api/sessions/<sessionId>/status", callback=self.getSessionStatus)
-        app.post("/api/sessions/<sessionId>/deploy", callback=self.deploySession)
-        app.post("/api/sessions/<sessionId>/cancel", callback=self.cancelSession)
+        app.get(
+            "/api/sessions/<sessionId>/status", callback=self.getSessionStatus
+        )
+        app.post(
+            "/api/sessions/<sessionId>/deploy", callback=self.deploySession
+        )
+        app.post(
+            "/api/sessions/<sessionId>/cancel", callback=self.cancelSession
+        )
         app.get("/api/sessions/<sessionId>/graph", callback=self.getGraph)
-        app.get("/api/sessions/<sessionId>/graph/size", callback=self.getGraphSize)
-        app.get("/api/sessions/<sessionId>/graph/status", callback=self.getGraphStatus)
-        app.post("/api/sessions/<sessionId>/graph/append", callback=self.addGraphParts)
         app.get(
-            "/api/sessions/<sessionId>/repro/data", callback=self.getSessionReproData
+            "/api/sessions/<sessionId>/graph/size", callback=self.getGraphSize
+        )
+        app.get(
+            "/api/sessions/<sessionId>/graph/status",
+            callback=self.getGraphStatus,
+        )
+        app.post(
+            "/api/sessions/<sessionId>/graph/append",
+            callback=self.addGraphParts,
+        )
+        app.get(
+            "/api/sessions/<sessionId>/repro/data",
+            callback=self.getSessionReproData,
         )
         app.get(
             "/api/sessions/<sessionId>/repro/status",
             callback=self.getSessionReproStatus,
         )
 
-        app.route("/api/sessions", method="OPTIONS", callback=self.acceptPreflight)
+        app.route(
+            "/api/sessions", method="OPTIONS", callback=self.acceptPreflight
+        )
         app.route(
             "/api/sessions/<sessionId>/graph/append",
             method="OPTIONS",
             callback=self.acceptPreflight2,
         )
 
         # The non-REST mappings that serve HTML-related content
@@ -200,15 +223,15 @@
         return {"methods": [DeploymentMethods.BROWSER]}
 
     def _stop_manager(self):
         self.dm.shutdown()
         self.stop()
         logger.info(
             "Thanks for using our %s, come back again :-)",
-            self.dm.__class__.__name__
+            self.dm.__class__.__name__,
         )
 
     @daliuge_aware
     def stop_manager(self):
         threading.Thread(target=self._stop_manager).start()
 
     @daliuge_aware
@@ -364,20 +387,25 @@
     """
     A REST server for NodeManagers. It includes mappings for NM-specific
     methods and the mapping for the main visualization HTML pages.
     """
 
     def initializeSpecifics(self, app):
         app.get("/api", callback=self.getNMStatus)
-        app.post("/api/sessions/<sessionId>/graph/link", callback=self.linkGraphParts)
+        app.post(
+            "/api/sessions/<sessionId>/graph/link",
+            callback=self.linkGraphParts,
+        )
         app.post(
             "/api/sessions/<sessionId>/subscriptions",
             callback=self.add_node_subscriptions,
         )
-        app.post("/api/sessions/<sessionId>/trigger", callback=self.trigger_drops)
+        app.post(
+            "/api/sessions/<sessionId>/trigger", callback=self.trigger_drops
+        )
         # The non-REST mappings that serve HTML-related content
         app.get("/", callback=self.visualizeDM)
         app.get("/api/shutdown", callback=self.shutdown_node_manager)
 
     @daliuge_aware
     def shutdown_node_manager(self):
         logger.debug("Shutting down node manager")
@@ -394,15 +422,17 @@
     def getLogFile(self, sessionId):
         logger.debug("NM REST call: logfile")
         logdir = self.dm.getLogDir()
         logfile = generateLogFileName(logdir, sessionId)
         if not os.path.isfile(logfile):
             raise NoSessionException(sessionId, "Log file not found.")
         return static_file(
-            os.path.basename(logfile), root=logdir, download=os.path.basename(logfile)
+            os.path.basename(logfile),
+            root=logdir,
+            download=os.path.basename(logfile),
         )
 
     @daliuge_aware
     def linkGraphParts(self, sessionId):
         logger.debug("NM REST call: graph/link")
         params = bottle.request.params
         lhOID = params["lhOID"]
@@ -429,15 +459,18 @@
     # non-REST methods
     # ===========================================================================
     def visualizeDM(self):
         tpl = file_as_string("web/dm.html")
         urlparts = bottle.request.urlparts
         serverUrl = urlparts.scheme + "://" + urlparts.netloc
         return bottle.template(
-            tpl, serverUrl=serverUrl, dmType=self.dm.__class__.__name__, reset="false"
+            tpl,
+            serverUrl=serverUrl,
+            dmType=self.dm.__class__.__name__,
+            reset="false",
         )
 
 
 class CompositeManagerRestServer(ManagerRestServer):
     """
     A REST server for DataIslandManagers. It includes mappings for DIM-specific
     methods.
@@ -456,27 +489,31 @@
             callback=self.getNodeSessionInformation,
         )
         app.get(
             "/api/node/<node>/sessions/<sessionId>/status",
             callback=self.getNodeSessionStatus,
         )
         app.get(
-            "/api/node/<node>/sessions/<sessionId>/graph", callback=self.getNodeGraph
+            "/api/node/<node>/sessions/<sessionId>/graph",
+            callback=self.getNodeGraph,
         )
         app.get(
             "/api/node/<node>/sessions/<sessionId>/graph/status",
             callback=self.getNodeGraphStatus,
         )
 
         # The non-REST mappings that serve HTML-related content
         app.get("/", callback=self.visualizeDIM)
 
     @daliuge_aware
     def getCMStatus(self):
-        return {"hosts": self.dm.dmHosts, "sessionIds": self.dm.getSessionIds()}
+        return {
+            "hosts": self.dm.dmHosts,
+            "sessionIds": self.dm.getSessionIds(),
+        }
 
     @daliuge_aware
     def getCMNodes(self):
         return self.dm.nodes
 
     def getAllCMNodes(self):
         return self.dm.nodes
@@ -567,15 +604,17 @@
     # ===========================================================================
     # non-REST methods
     # ===========================================================================
     def visualizeDIM(self):
         tpl = file_as_string("web/dim.html")
         urlparts = bottle.request.urlparts
         selectedNode = (
-            bottle.request.params["node"] if "node" in bottle.request.params else ""
+            bottle.request.params["node"]
+            if "node" in bottle.request.params
+            else ""
         )
         serverUrl = urlparts.scheme + "://" + urlparts.netloc
         return bottle.template(
             tpl,
             dmType=self.dm.__class__.__name__,
             dmPort=self.dm.dmPort,
             serverUrl=serverUrl,
@@ -646,26 +685,30 @@
         with RestClient(host=host, port=port, timeout=10) as c:
             return json.loads(c._POST("/managers/node/stop").read())
 
     @daliuge_aware
     def addNM(self, host, node):
         port = constants.ISLAND_DEFAULT_REST_PORT
         logger.debug("Adding NM %s to DIM %s", node, host)
-        with RestClient(host=host, port=port, timeout=10, url_prefix="/api") as c:
+        with RestClient(
+            host=host, port=port, timeout=10, url_prefix="/api"
+        ) as c:
             return json.loads(
                 c._POST(
                     f"/node/{node}",
                 ).read()
             )
 
     @daliuge_aware
     def removeNM(self, host, node):
         port = constants.ISLAND_DEFAULT_REST_PORT
         logger.debug("Removing NM %s from DIM %s", node, host)
-        with RestClient(host=host, port=port, timeout=10, url_prefix="/api") as c:
+        with RestClient(
+            host=host, port=port, timeout=10, url_prefix="/api"
+        ) as c:
             return json.loads(c._DELETE(f"/node/{node}").read())
 
     @daliuge_aware
     def getNMInfo(self, host):
         port = constants.DAEMON_DEFAULT_REST_PORT
         logger.debug("Sending request %s:%s/managers/node", host, port)
         with RestClient(host=host, port=port, timeout=10) as c:
```

### Comparing `daliuge-engine-2.4.0/dlg/manager/session.py` & `daliuge-engine-3.0.0/dlg/manager/session.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/manager/shared_memory_manager.py` & `daliuge-engine-3.0.0/dlg/manager/shared_memory_manager.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/manager/web/dim.html` & `daliuge-engine-3.0.0/dlg/manager/web/dim.html`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/manager/web/dm.html` & `daliuge-engine-3.0.0/dlg/manager/web/dm.html`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/manager/web/session.html` & `daliuge-engine-3.0.0/dlg/manager/web/session.html`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/manager/web/static/css/bootstrap.min.css` & `daliuge-engine-3.0.0/dlg/manager/web/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/manager/web/static/css/dm.css` & `daliuge-engine-3.0.0/dlg/manager/web/static/css/dm.css`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/manager/web/static/css/progressBar.css` & `daliuge-engine-3.0.0/dlg/manager/web/static/css/progressBar.css`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/manager/web/static/css/session.css` & `daliuge-engine-3.0.0/dlg/manager/web/static/css/session.css`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/manager/web/static/fonts/glyphicons-halflings-regular.eot` & `daliuge-engine-3.0.0/dlg/manager/web/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/manager/web/static/fonts/glyphicons-halflings-regular.svg` & `daliuge-engine-3.0.0/dlg/manager/web/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/manager/web/static/fonts/glyphicons-halflings-regular.ttf` & `daliuge-engine-3.0.0/dlg/manager/web/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/manager/web/static/fonts/glyphicons-halflings-regular.woff` & `daliuge-engine-3.0.0/dlg/manager/web/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/manager/web/static/fonts/glyphicons-halflings-regular.woff2` & `daliuge-engine-3.0.0/dlg/manager/web/static/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/manager/web/static/icons/engine.svg` & `daliuge-engine-3.0.0/dlg/manager/web/static/icons/engine.svg`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/manager/web/static/icons/liu.svg` & `daliuge-engine-3.0.0/dlg/manager/web/static/icons/liu.svg`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/manager/web/static/icons/liuFavIcon.svg` & `daliuge-engine-3.0.0/dlg/manager/web/static/icons/liuFavIcon.svg`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/manager/web/static/js/bootbox.min.js` & `daliuge-engine-3.0.0/dlg/manager/web/static/js/bootbox.min.js`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/manager/web/static/js/bootstrap.bundle.min.js` & `daliuge-engine-3.0.0/dlg/manager/web/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/manager/web/static/js/d3/d3.v5.min.js` & `daliuge-engine-3.0.0/dlg/manager/web/static/js/d3/d3.v5.min.js`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/manager/web/static/js/d3/dagre-d3.js` & `daliuge-engine-3.0.0/dlg/manager/web/static/js/d3/dagre-d3.js`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/manager/web/static/js/d3/dagre-d3.min.js` & `daliuge-engine-3.0.0/dlg/manager/web/static/js/d3/dagre-d3.min.js`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/manager/web/static/js/dm.js` & `daliuge-engine-3.0.0/dlg/manager/web/static/js/dm.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -588,16 +588,16 @@
         return false;
     }
 
     var typeClass = doSpec.type;
     var typeShape = TYPE_SHAPES[doSpec.type];
     var notes = '';
     // console.log('Drop type', doSpec.type)
-    if (doSpec.nm) {
-        notes = "<span>" + doSpec.nm + "</span>"
+    if (doSpec.name) {
+        notes = "<span>" + doSpec.name + "</span>"
     }
     if (doSpec.type == 'app') {
         var nameParts = doSpec.app.split('.');
         notes += nameParts[nameParts.length - 1];
     } else if (doSpec.type == 'socket') {
         notes += 'port: ' + doSpec.port;
     } else if (doSpec.type == 'plain') {
```

### Comparing `daliuge-engine-2.4.0/dlg/manager/web/static/js/jquery-3.6.0.min.js` & `daliuge-engine-3.0.0/dlg/manager/web/static/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/meta.py` & `daliuge-engine-3.0.0/dlg/meta.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/named_port_utils.py` & `daliuge-engine-3.0.0/dlg/named_port_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,16 +30,14 @@
 
     Returns:
         dict: a dictionary with the relevant arguments only.
     """
     cleanedArgs = {}
     if not isinstance(applicationArgs, dict):
         logger.info("applicationArgs are not passed as a dict. Ignored!")
-    else:
-        logger.info("ApplicationArgs found %s", applicationArgs)
     for name, vdict in applicationArgs.items():
         if vdict in [None, False, ""]:
             continue
         elif isinstance(vdict, bool):
             vdict = {"precious": False, "value": "", "positional": False}
         elif isinstance(vdict, dict):
             precious = vdict["precious"]
@@ -92,15 +90,15 @@
         check_len (int): number of of ports to be checked
         mode (str ["inputs"]): mode, used just for logging messages
 
     Returns:
         dict: port arguments
 
     Side effect:
-        modifies the pargsDict OrderedDict
+        modifies pargsDict
     """
     # p_name = [p["name"] for p in port_dict]
     logger.debug(
         "Using named ports to remove %s from arguments port_dict: %s, check_len: %d)",
         mode,
         port_dict,
         check_len,
@@ -117,25 +115,33 @@
         except KeyError:
             logger.debug("portDict: %s", port_dict)
             raise KeyError
         if value is None:
             value = ""  # make sure we are passing NULL drop events
         if key in posargs:
             pargsDict.update({key: value})
+            # portargs.update({key: value})
             logger.debug("Using %s '%s' for parg %s", mode, value, key)
             posargs.pop(posargs.index(key))
         elif key in keyargs:
             # if not found in appArgs we don't put them into portargs either
             portargs.update({key: value})
+            # pargsDict.update({key: value})
             logger.debug(
                 "Using %s of type %s for kwarg %s", mode, type(value), key
             )
-            _dum = keyargs.pop(key)  # remove from original arg list
+            _ = keyargs.pop(key)  # remove from original arg list
         else:
-            logger.debug("No matching argument found for %s key %s", mode, key)
+            logger.debug(
+                "No matching argument found for %s key %s, %s, %s",
+                mode,
+                key,
+                keyargs,
+                posargs,
+            )
     logger.debug("Returning kw mapped ports: %s", portargs)
     return portargs
 
 
 def check_ports_dict(ports: list) -> bool:
     """
     Checks whether all ports in ports list are of type dict. This is
@@ -204,15 +210,22 @@
     }
     # we will need an ordered dict for all positional arguments
     # thus we create it here and fill it with values
     portPosargsDict = collections.OrderedDict(
         zip(posargs, [None] * len(posargs))
     )
     portkeyargs = {}
-    # logger.debug("posargs: %s; keyargs: %s", posargs, keyargs)
+    logger.debug(
+        "posargs: %s; keyargs: %s, %s",
+        posargs,
+        keyargs,
+        check_ports_dict(inport_names),
+    )
+    ipkeyargs = {}
+    opkeyargs = {}
     if check_ports_dict(inport_names):
         for inport in inport_names:
             key = list(inport.keys())[0]
             inputs_dict[key].update({"name": inport[key]})
 
         ipkeyargs = identify_named_ports(
             inputs_dict,
@@ -221,15 +234,15 @@
             keyargs,
             check_len=len(iitems),
             mode="inputs",
         )
         portkeyargs.update(ipkeyargs)
     else:
         for i in range(min(len(iitems), len(posargs))):
-            portkeyargs.update({posargs[i]: iitems[i][1]})
+            portkeyargs.update({list(posargs)[i]: list(iitems)[i][1]})
 
     if check_ports_dict(outport_names):
         for outport in outport_names:
             key = list(outport.keys())[0]
             outputs_dict[key].update({"name": outport[key]})
         opkeyargs = identify_named_ports(
             outputs_dict,
@@ -238,43 +251,48 @@
             keyargs,
             check_len=len(oitems),
             mode="outputs",
         )
         portkeyargs.update(opkeyargs)
     else:
         for i in range(min(len(oitems), len(posargs))):
-            portkeyargs.update({posargs[i]: oitems[i][1]})
+            portkeyargs.update({posargs[i]: list(oitems)[i][1]})
     # now that we have the mapped ports we can cleanup the appArgs
     # and construct the final keyargs and pargs
-    logger.debug("Arguments from ports: %s %s", portkeyargs, portPosargsDict)
+    logger.debug(
+        "Arguments from ports: %s, %s, %s, %s",
+        portkeyargs,
+        portPosargsDict,
+        ipkeyargs,
+        opkeyargs,
+    )
     appArgs = clean_applicationArgs(appArgs)
     # get cleaned positional args
     posargs = {
         arg: appArgs[arg]["value"]
         for arg in appArgs
         if appArgs[arg]["positional"]
     }
     logger.debug("posargs: %s", posargs)
     # get cleaned kwargs
     keyargs = {
         arg: appArgs[arg]["value"]
         for arg in appArgs
         if not appArgs[arg]["positional"]
     }
-    # update port dictionaries
-    # portkeyargs.update({key:arg for key, arg in keyargs.items()
-    #     if key not in portkeyargs})
-    # portPosargsDict.update({key:arg for key, arg in posargs.items()
-    #     if key not in portPosargsDict})
     for k, v in portkeyargs.items():
         if v not in [None, ""]:
             keyargs.update({k: v})
     for k, v in portPosargsDict.items():
         logger.debug("port posarg %s has value %s", k, v)
-        logger.debug("default posarg %s has value %s", k, posargs[k])
+        # logger.debug("default posarg %s has value %s", k, posargs[k])
+        if k == "input_redirection":
+            v = f"cat {v} > "
+        if k == "output_redirection":
+            v = f"> {v}"
         if v not in [None, ""]:
             posargs.update({k: v})
     keyargs = (
         serialize_kwargs(keyargs, prefix=argumentPrefix, separator=separator)
         if len(keyargs) > 0
         else [""]
     )
```

### Comparing `daliuge-engine-2.4.0/dlg/ngaslite.py` & `daliuge-engine-3.0.0/dlg/ngaslite.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/nm_dim_assigner.py` & `daliuge-engine-3.0.0/dlg/nm_dim_assigner.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/prepareUser.py` & `daliuge-engine-3.0.0/dlg/prepareUser.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/process.py` & `daliuge-engine-3.0.0/dlg/process.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/remote.py` & `daliuge-engine-3.0.0/dlg/remote.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/restserver.py` & `daliuge-engine-3.0.0/dlg/restserver.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/rpc.py` & `daliuge-engine-3.0.0/dlg/rpc.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/runtime/__init__.py` & `daliuge-engine-3.0.0/dlg/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/runtime/tool_commands.py` & `daliuge-engine-3.0.0/dlg/runtime/tool_commands.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/shared_memory.py` & `daliuge-engine-3.0.0/dlg/shared_memory.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/dlg/testutils.py` & `daliuge-engine-3.0.0/dlg/testutils.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/setup.py` & `daliuge-engine-3.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 
 # Version information
 # We do like numpy: we have a major/minor/patch hand-written version written
 # here. If we find the git commit (either via "git" command execution or in a
 # dlg/version.py file) we append it to the VERSION later.
 # The RELEASE flag allows us to create development versions properly supported
 # by setuptools/pkg_resources or "final" versions.
-MAJOR = 2
-MINOR = 4
+MAJOR = 3
+MINOR = 0
 PATCH = 0
 RELEASE = True
 VERSION = "%d.%d.%d" % (MAJOR, MINOR, PATCH)
 VERSION_FILE = "dlg/runtime/version.py"
 PTH_FILE = "lib64_dist.pth"
```

### Comparing `daliuge-engine-2.4.0/test/deploy/test_slurm_utils.py` & `daliuge-engine-3.0.0/test/test_io.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #
 #    ICRAR - International Centre for Radio Astronomy Research
-#    (c) UWA - The University of Western Australia, 2019
+#    (c) UWA - The University of Western Australia, 2015
 #    Copyright by UWA (in the framework of the ICRAR)
 #    All rights reserved
 #
 #    This library is free software; you can redistribute it and/or
 #    modify it under the terms of the GNU Lesser General Public
 #    License as published by the Free Software Foundation; either
 #    version 2.1 of the License, or (at your option) any later version.
@@ -15,25 +15,32 @@
 #    Lesser General Public License for more details.
 #
 #    You should have received a copy of the GNU Lesser General Public
 #    License along with this library; if not, write to the Free Software
 #    Foundation, Inc., 59 Temple Place, Suite 330, Boston,
 #    MA 02111-1307  USA
 #
-
 import unittest
 
-from dlg.deploy import deployment_utils
+from dlg.data.io import NullIO, OpenMode
+
+
+class TestIO(unittest.TestCase):
+    def test_invalidUseCases(self):
+        io = NullIO()
+
+        # Not opened yet
+        self.assertRaises(ValueError, io.write, "")
+        self.assertRaises(ValueError, io.read, "")
+
+        # Opening in read-only mode
+        io.open(OpenMode.OPEN_READ)
+        self.assertRaises(ValueError, io.write, "")
+        io.close()
 
+        # Opening in write-only mode
+        io.open(OpenMode.OPEN_WRITE)
+        self.assertRaises(ValueError, io.read, 1)
+        io.close()
 
-class TestSlurmUtils(unittest.TestCase):
-    def assert_list_as_string(self, s, expected_list):
-        slurm_list = deployment_utils.list_as_string(s)
-        self.assertEqual(expected_list, slurm_list)
-
-    def test_list_as_string(self):
-        self.assert_list_as_string(
-            "a008,b[072-073,076]", ["a008", "b072", "b073", "b076"]
-        )
-        self.assert_list_as_string(
-            "pleiades[03-05]", ["pleiades03", "pleiades04", "pleiades05"]
-        )
+        # It's OK to close it again
+        io.close()
```

### Comparing `daliuge-engine-2.4.0/test/manager/test_rest.py` & `daliuge-engine-3.0.0/test/test_session.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #
 #    ICRAR - International Centre for Radio Astronomy Research
-#    (c) UWA - The University of Western Australia, 2016
+#    (c) UWA - The University of Western Australia, 2015
 #    Copyright by UWA (in the framework of the ICRAR)
 #    All rights reserved
 #
 #    This library is free software; you can redistribute it and/or
 #    modify it under the terms of the GNU Lesser General Public
 #    License as published by the Free Software Foundation; either
 #    version 2.1 of the License, or (at your option) any later version.
@@ -15,262 +15,271 @@
 #    Lesser General Public License for more details.
 #
 #    You should have received a copy of the GNU Lesser General Public
 #    License along with this library; if not, write to the Free Software
 #    Foundation, Inc., 59 Temple Place, Suite 330, Boston,
 #    MA 02111-1307  USA
 #
-import tempfile
-import threading
+import json
 import unittest
 
-from dlg import exceptions
-from dlg.common import Categories
-from dlg.common.deployment_methods import DeploymentMethods
-from dlg.exceptions import InvalidGraphException
+import pkg_resources
 
-from dlg.manager import constants
-from dlg.manager.client import NodeManagerClient, DataIslandManagerClient
-from dlg.manager.composite_manager import DataIslandManager
-from dlg.manager.node_manager import NodeManager
-from dlg.manager.rest import NMRestServer, CompositeManagerRestServer
-from dlg.restutils import RestClient
+from dlg.ddap_protocol import DROPLinkType, DROPStates, AppDROPStates
+from dlg.droputils import DROPWaiterCtx
+from dlg.exceptions import InvalidGraphException
+from dlg.manager.session import SessionStates, Session
 
 default_repro = {
     "rmode": "1",
     "RERUN": {
         "lg_blockhash": "x",
         "pgt_blockhash": "y",
         "pg_blockhash": "z",
-    }
+    },
 }
 default_graph_repro = {
     "rmode": "1",
     "meta_data": {"repro_protocol": 0.1, "hashing_alg": "_sha3.sha3_256"},
     "merkleroot": "a",
     "RERUN": {
         "signature": "b",
-    }
+    },
 }
 
 
 def add_test_reprodata(graph: list):
     for drop in graph:
         drop["reprodata"] = default_repro.copy()
     graph.append(default_graph_repro.copy())
     return graph
 
 
-hostname = "localhost"
+class TestSession(unittest.TestCase):
+    def test_sessionStates(self):
+        with Session("1") as s:
+            self.assertEqual(SessionStates.PRISTINE, s.status)
+            self.assertRaises(Exception, s.linkGraphParts, "", "", 0)
+            s.addGraphSpec(
+                add_test_reprodata([{"oid": "A", "categoryType": "container"}])
+            )
+            self.assertEqual(SessionStates.BUILDING, s.status)
+
+            s.deploy()
+            self.assertEqual(SessionStates.RUNNING, s.status)
+
+            # Now we can't do any of these
+            self.assertRaises(Exception, s.deploy)
+            self.assertRaises(Exception, s.addGraphSpec, "")
+            self.assertRaises(Exception, s.linkGraphParts, "", "", 0)
+
+    def test_sessionStates_noDrops(self):
+        # No drops created, we can deploy right away
+        with Session("1") as s:
+            self.assertEqual(SessionStates.PRISTINE, s.status)
+            s.deploy()
+            self.assertEqual(SessionStates.FINISHED, s.status)
+
+        with Session("2") as s:
+            self.assertRaises(
+                InvalidGraphException, s.deploy, completedDrops=["a"]
+            )
+
+    def test_addGraphSpec(self):
+        with Session("1") as s:
+            s.addGraphSpec(
+                add_test_reprodata([{"oid": "A", "categoryType": "container"}])
+            )
+            s.addGraphSpec(
+                add_test_reprodata([{"oid": "B", "categoryType": "container"}])
+            )
+            s.addGraphSpec(
+                add_test_reprodata([{"oid": "C", "categoryType": "container"}])
+            )
+
+            # Adding an existing DROP
+            self.assertRaises(
+                Exception,
+                s.addGraphSpec,
+                add_test_reprodata(
+                    [{"oid": "A", "categoryType": "container"}]
+                ),
+            )
+
+            # Adding invalid specs
+            self.assertRaises(
+                Exception,
+                s.addGraphSpec,
+                add_test_reprodata(
+                    [{"oid": "D", "categoryType": "Application"}]
+                ),
+            )  # missing "storage"
+            self.assertRaises(
+                Exception,
+                s.addGraphSpec,
+                add_test_reprodata(
+                    [
+                        {
+                            "oid": "D",
+                            "categoryType": "Data",
+                            "dropclass": "invalid",
+                        }
+                    ]
+                ),
+            )  # invalid "storage"
+            self.assertRaises(
+                Exception,
+                s.addGraphSpec,
+                add_test_reprodata([{"oid": "D", "categoryType": "invalid"}]),
+            )  # invalid "categoryType"
+            self.assertRaises(
+                Exception,
+                s.addGraphSpec,
+                add_test_reprodata(
+                    [
+                        {
+                            "oid": "D",
+                            "categoryType": "Application",
+                            "dropclass": "dlg.data.drops.NullDROP",
+                            "outputs": ["X"],
+                        }
+                    ]
+                ),
+            )  # missing X DROP
+
+    def test_addGraphSpec_namedPorts(self):
+        with pkg_resources.resource_stream(
+            "test", "graphs/funcTestPG_namedPorts.graph"
+        ) as f:  # @UndefinedVariable
+            graphSpec = json.load(f)
+        # dropSpecs = graph_loader.loadDropSpecs(graphSpec)
+        with Session("1") as s:
+            s.addGraphSpec(graphSpec)
+            s.deploy()
+
+    def test_linking(self):
+        with Session("1") as s:
+            s.addGraphSpec(
+                add_test_reprodata([{"oid": "A", "categoryType": "container"}])
+            )
+            s.addGraphSpec(
+                add_test_reprodata(
+                    [
+                        {
+                            "oid": "B",
+                            "categoryType": "Application",
+                            # "dropclass": "dlg.data.drops.data_base.NullDROP",
+                            "dropclass": "dlg.apps.crc.CRCApp",
+                        }
+                    ]
+                )
+            )
+            s.addGraphSpec(
+                add_test_reprodata([{"oid": "C", "categoryType": "container"}])
+            )
 
+            # Link them now
+            s.linkGraphParts("A", "B", DROPLinkType.CONSUMER)
+            s.linkGraphParts("B", "C", DROPLinkType.OUTPUT)
+
+            # Deploy and check that the actual DROPs are linked together
+            s.deploy()
+            roots = s.roots
+            self.assertEqual(1, len(roots))
+            a = s.roots[0]
+            self.assertEqual("A", a.oid)
+            self.assertEqual(1, len(a.consumers))
+            b = a.consumers[0]
+            self.assertEqual("B", b.oid)
+            self.assertEqual(1, len(b.outputs))
+            c = b.outputs[0]
+            self.assertEqual("C", c.oid)
+
+    def test_cancel(self):
+        """Cancels a whole graph execution"""
+        with Session("1") as s:
+            s.addGraphSpec(
+                add_test_reprodata(
+                    [
+                        {
+                            "oid": "A",
+                            "categoryType": "Data",
+                            "dropclass": "dlg.data.drops.memory.InMemoryDROP",
+                            "consumers": ["B"],
+                        },
+                        {
+                            "oid": "B",
+                            "categoryType": "Application",
+                            "dropclass": "dlg.apps.simple.SleepApp",
+                            "sleep_time": 2,
+                        },
+                        {
+                            "oid": "C",
+                            "categoryType": "Data",
+                            "dropclass": "dlg.data.drops.memory.InMemoryDROP",
+                            "producers": ["B"],
+                        },
+                    ]
+                )
+            )
+            s.deploy()
+            self.assertEqual(SessionStates.RUNNING, s.status)
+            s.cancel()
+            self.assertEqual(SessionStates.CANCELLED, s.status)
+            for uid in "ABC":
+                self.assertEqual(DROPStates.CANCELLED, s.drops[uid].status)
+            self.assertEqual(AppDROPStates.CANCELLED, s.drops["B"].execStatus)
+
+    def test_partial_cancel(self):
+        """Like test_cancel, but only part of the graph should be cancelled"""
+        with Session("1") as s:
+            s.addGraphSpec(
+                add_test_reprodata(
+                    [
+                        {
+                            "oid": "A",
+                            "categoryType": "Data",
+                            "dropclass": "dlg.data.drops.memory.InMemoryDROP",
+                            "consumers": ["B"],
+                        },
+                        {
+                            "oid": "B",
+                            "categoryType": "Application",
+                            "dropclass": "dlg.apps.simple.SleepApp",
+                            "sleep_time": 0,
+                        },
+                        {
+                            "oid": "C",
+                            "categoryType": "Data",
+                            "dropclass": "dlg.data.drops.memory.InMemoryDROP",
+                            "producers": ["B"],
+                            "consumers": ["D"],
+                        },
+                        {
+                            "oid": "D",
+                            "categoryType": "Application",
+                            "dropclass": "dlg.apps.simple.SleepApp",
+                            "sleep_time": 10,
+                        },
+                        {
+                            "oid": "E",
+                            "categoryType": "Data",
+                            "dropclass": "dlg.data.drops.memory.InMemoryDROP",
+                            "producers": ["D"],
+                        },
+                    ]
+                )
+            )
+            s.deploy()
+            self.assertEqual(SessionStates.RUNNING, s.status)
 
-class TestRest(unittest.TestCase):
-    def setUp(self):
-        unittest.TestCase.setUp(self)
-        self.dm = NodeManager(False)
-        self._dm_server = NMRestServer(self.dm)
-        self._dm_t = threading.Thread(
-            target=self._dm_server.start,
-            args=(hostname, constants.NODE_DEFAULT_REST_PORT),
-        )
-        self._dm_t.start()
-
-        self.dim = DataIslandManager(dmHosts=[hostname])
-        self._dim_server = CompositeManagerRestServer(self.dim)
-        self._dim_t = threading.Thread(
-            target=self._dim_server.start,
-            args=(hostname, constants.ISLAND_DEFAULT_REST_PORT),
-        )
-        self._dim_t.start()
-
-    def tearDown(self):
-        unittest.TestCase.tearDown(self)
-        self._dm_server.stop()
-        self._dm_t.join()
-        self.dm.shutdown()
-        self.assertFalse(self._dm_t.is_alive())
-
-        self._dim_server.stop()
-        self._dim_t.join()
-        self.dim.shutdown()
-        self.assertFalse(self._dim_t.is_alive())
-
-    def test_index(self):
-        # Just check that the HTML pages load properly
-        with RestClient(hostname, constants.NODE_DEFAULT_REST_PORT, timeout=10) as c:
-            c._GET("/")
-            c._GET("/session")
-
-    def test_errtype(self):
-        sid = "lala"
-        c = NodeManagerClient(hostname)
-        c.createSession(sid)
-        gempty = [{}]
-        add_test_reprodata(gempty)
-        # already exists
-        self.assertRaises(
-            exceptions.SessionAlreadyExistsException, c.createSession, sid
-        )
-
-        # different session
-        self.assertRaises(
-            exceptions.NoSessionException, c.addGraphSpec, sid + "x", [{}]
-        )
-
-        # invalid dropspec, it has no oid/type (is completely empty actually)
-        self.assertRaises(exceptions.InvalidGraphException, c.addGraphSpec, sid, gempty)
-
-        # invalid dropspec, app doesn't exist
-        self.assertRaises(
-            exceptions.InvalidGraphException,
-            c.addGraphSpec,
-            sid,
-            [
-                {
-                    "oid": "a",
-                    "type": "app",
-                    "app": "doesnt.exist",
-                    "reprodata": default_repro.copy(),
-                },
-                default_graph_repro.copy(),
-            ],
-        )
-
-        # invalid state, the graph status is only queried when the session is running
-        self.assertRaises(exceptions.InvalidSessionState, c.getGraphStatus, sid)
-
-        # valid dropspec, but the socket listener app doesn't allow inputs
-        c.addGraphSpec(
-            sid,
-            [
-                {
-                    "type": "socket",
-                    "oid": "a",
-                    "inputs": ["b"],
-                    "reprodata": default_repro.copy(),
-                },
-                {
-                    "oid": "b",
-                    "type": "data",
-                    "storage": Categories.MEMORY,
-                    "reprodata": default_repro.copy(),
-                },
-                default_graph_repro.copy(),
-            ],
-        )
-        self.assertRaises(exceptions.InvalidRelationshipException, c.deploySession, sid)
-
-        # And here we point to an unexisting file, making an invalid drop
-        c.destroySession(sid)
-        c.createSession(sid)
-        fname = tempfile.mktemp()
-        c.addGraphSpec(
-            sid,
-            [
-                {
-                    "type": "data",
-                    "storage": Categories.FILE,
-                    "oid": "a",
-                    "filepath": fname,
-                    "check_filepath_exists": True,
-                    "reprodata": default_repro.copy(),
-                },
-                default_graph_repro.copy(),
-            ],
-        )
-        self.assertRaises(exceptions.InvalidDropException, c.deploySession, sid)
-
-    def test_recursive(self):
-        sid = "lala"
-        c = DataIslandManagerClient(hostname)
-        c.createSession(sid)
-
-        # invalid dropspec, app doesn't exist
-        # This is not checked at the DIM level but only at the NM level
-        # The exception should still pass through though
-        with self.assertRaises(exceptions.SubManagerException) as cm:
-            c.addGraphSpec(
-                sid,
-                [
-                    {
-                        "oid": "a",
-                        "type": "app",
-                        "app": "doesnt.exist",
-                        "node": hostname,
-                        "reprodata": default_repro.copy(),
-                    },
-                    default_graph_repro.copy(),
-                ],
-            )
-        ex = cm.exception
-        self.assertTrue(hostname in ex.args[0])
-        self.assertTrue(isinstance(ex.args[0][hostname], InvalidGraphException))
-
-    def test_reprodata_get(self):
-        """
-        Tests deploying an incredibly basic graph with and without reprodata
-        Then querying the manager for that reprodata.
-        """
-        sid = "1234"
-        c = NodeManagerClient(hostname)
-        graph_spec = [
-            {
-                "type": "data",
-                "storage": Categories.MEMORY,
-                "oid": "a",
-                "reprodata": default_repro.copy(),
-            },
-            default_graph_repro.copy(),
-        ]
-        # Test with reprodata
-        c.createSession(sid)
-        c.addGraphSpec(sid, graph_spec)
-        c.deploySession(sid, completed_uids=["a"])
-        response = c.session_repro_data(sid)
-        self.assertIsNotNone(response["graph"]["a"]["reprodata"]["RERUN"]["rg_blockhash"])
-        self.assertIsNotNone(response["reprodata"])
-        c.destroySession(sid)
-        # Test without reprodata
-        graph_spec = graph_spec[0:1]
-        graph_spec[0].pop("reprodata")
-        c.createSession(sid)
-        c.addGraphSpec(sid, graph_spec)
-        c.deploySession(sid, completed_uids=["a"])
-        response = c.session_repro_data(sid)
-        self.assertEqual(
-            {"a": {"oid": "a", "storage": "Memory", "type": "data"}}, response["graph"]
-        )
-        self.assertEqual({}, response["reprodata"])
-
-    def test_reprostatus_get(self):
-        # Test with reprodata
-        sid = "1234"
-        c = NodeManagerClient(hostname)
-        graph_spec = [
-            {
-                "type": "data",
-                "storage": Categories.MEMORY,
-                "oid": "a",
-                "reprodata": default_repro.copy(),
-            },
-            default_graph_repro.copy(),
-        ]
-        c.createSession(sid)
-        c.addGraphSpec(sid, graph_spec)
-        c.deploySession(sid, completed_uids=["a"])
-        response = c.session_repro_status(sid)
-        self.assertTrue(response)
-        c.destroySession(sid)
-        # Test without reprodata
-        graph_spec = graph_spec[0:1]
-        graph_spec[0].pop("reprodata")
-        c.createSession(sid)
-        c.addGraphSpec(sid, graph_spec)
-        c.deploySession(sid, completed_uids=["a"])
-        response = c.session_repro_status(sid)
-        self.assertTrue(response)
-        c.destroySession(sid)
-
-    def test_submit_method(self):
-        c = NodeManagerClient(hostname)
-        response = c.get_submission_method()
-        self.assertEqual({"methods": [DeploymentMethods.BROWSER]}, response)
+            # Move first three drops to completed, D should take longer to execute
+            with DROPWaiterCtx(self, s.drops["C"], 1):
+                s.drops["A"].write(b"x")
+                s.drops["A"].setCompleted()
+            # Cancel the session, A, B and C should remain COMPLETED
+            s.cancel()
+            self.assertEqual(SessionStates.CANCELLED, s.status)
+            for uid in "ABC":
+                self.assertEqual(DROPStates.COMPLETED, s.drops[uid].status)
+            for uid in "DE":
+                self.assertEqual(DROPStates.CANCELLED, s.drops[uid].status)
```

### Comparing `daliuge-engine-2.4.0/test/test_JsonDrop.py` & `daliuge-engine-3.0.0/test/test_JsonDrop.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/test/test_ParameterSetDROP.py` & `daliuge-engine-3.0.0/test/test_ParameterSetDROP.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/test/test_S3Drop.py` & `daliuge-engine-3.0.0/test/test_S3Drop.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/test/test_dask_emulation.py` & `daliuge-engine-3.0.0/test/test_dask_emulation.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,38 +125,49 @@
         compute = self.compute
 
         the_sum = delayed(add)(1.0, 2.0)
         the_sub = delayed(subtract)(4.0, 3.0)
         division = delayed(divide)(the_sum, the_sub)
         parts = delayed(partition, nout=2)(division)
         logger.debug(f"partitions: {type(parts)}")
-        result = 3.0
         result = compute(delayed(add)(*parts))
         self.assertEqual(3.0, result)
 
     def test_args_as_lists(self):
         """Like test_simple, but some arguments are passed down as lists"""
         delayed = self.delayed
         compute = self.compute
 
-        one, two, three, four = delayed(1.0), delayed(2.0), delayed(3.0), delayed(4.0)
+        one, two, three, four = (
+            delayed(1.0),
+            delayed(2.0),
+            delayed(3.0),
+            delayed(4.0),
+        )
         the_sum = delayed(add_list)([one, two])
         the_sub = delayed(subtract_list)([four, three])
         division = delayed(divide)(the_sum, the_sub)
         parts = delayed(partition, nout=2)(division)
         result = compute(delayed(add)(*parts))
         self.assertEqual(3.0, result)
 
     def test_compute_with_lists(self):
         """Make sure we can call compute() directly on the list objects"""
         delayed = self.delayed
         compute = self.compute
 
-        one, two, three, four = delayed(1.0), delayed(2.0), delayed(3.0), delayed(4.0)
-        doubles = [delayed(lambda i: i * 2)(x) for x in (one, two, three, four)]
+        one, two, three, four = (
+            delayed(1.0),
+            delayed(2.0),
+            delayed(3.0),
+            delayed(4.0),
+        )
+        doubles = [
+            delayed(lambda i: i * 2)(x) for x in (one, two, three, four)
+        ]
         result = compute(doubles)
         self.assertEqual([2.0, 4.0, 6.0, 8.0], result)
 
     def test_none_arg(self):
         """Test that calling delayed(f)(None) works"""
         delayed = self.delayed
         compute = self.compute
@@ -175,16 +186,18 @@
 
     def test_with_kwargs(self):
         """Tests that delayed() works correctly with args and kwargs"""
         delayed = self.delayed
         compute = self.compute
 
         self.assertEqual(compute(delayed(sum_with_kwargs)(1)), 1)
-        self.assertEqual(compute(delayed(sum_with_kwargs)(1, b=20)), 21)
-        self.assertEqual(compute(delayed(sum_with_kwargs)(1, b=20, x=-111)), 21)
+        # self.assertEqual(compute(delayed(sum_with_kwargs)(1, b=20)), 21)
+        # self.assertEqual(
+        # compute(delayed(sum_with_kwargs)(1, b=20, x=-111)), 21
+        # )
 
     def test_with_args_and_kwargs(self):
         """Tests that delayed() works correctly with kwargs"""
         delayed = self.delayed
         compute = self.compute
 
         self.assertEqual(compute(delayed(sum_with_args_and_kwarg)(1)), 1)
@@ -196,15 +209,17 @@
         # )
 
     def test_with_user_defined_default(self):
         """Tests that delayed() works with default values that are not json-dumpable"""
         delayed = self.delayed
         compute = self.compute
 
-        self.assertEqual(compute(delayed(sum_with_user_defined_default)(1)), 11)
+        self.assertEqual(
+            compute(delayed(sum_with_user_defined_default)(1)), 11
+        )
         self.assertEqual(
             compute(delayed(sum_with_user_defined_default)(1, MyType(20))), 21
         )
 
     def test_with_noniterable_nout_1(self):
         """Tests that using nout=1 works as expected with non-iterable objects"""
         # Simple call
```

### Comparing `daliuge-engine-2.4.0/test/test_drop.py` & `daliuge-engine-3.0.0/test/test_drop.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/test/test_droputils.py` & `daliuge-engine-3.0.0/test/test_droputils.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 
 import subprocess
 import unittest
 
 import numpy
 
 from dlg import droputils
-from dlg.common import dropdict, Categories
-from dlg.apps.app_base import AppDROP, BarrierAppDROP
+from dlg.common import dropdict
+from dlg.apps.app_base import BarrierAppDROP
 from dlg.data.drops.plasma import PlasmaDROP
 from dlg.data.drops.memory import InMemoryDROP
 from dlg.data.drops.file import FileDROP
 from dlg.droputils import DROPFile
 
 
 class DropUtilsTest(unittest.TestCase):
@@ -224,75 +224,87 @@
 
         """
         A --> B
         """
         pg_spec = [
             {
                 "oid": "A",
-                "type": "data",
-                "storage": Categories.MEMORY,
+                "categoryType": "Data",
+                "dropclass": "dlg.data.drops.memory.InMemoryDROP",
                 "consumers": ["B"],
             },
             {
                 "oid": "B",
-                "type": "app",
-                "app": "test.test_graph_loader.DummyApp",
+                "categoryType": "Application",
+                "Application": "test.test_graph_loader.DummyApp",
             },
         ]
         roots = droputils.get_roots(pg_spec)
         self.assertEqual(1, len(roots))
         self.assertEqual("A", next(iter(roots)))
 
         """
         A --> B
         The same, but now B references A
         """
         pg_spec = [
-            {"oid": "A", "type": "data", "storage": Categories.MEMORY},
+            {
+                "oid": "A",
+                "categoryType": "Data",
+                "dropclass": "dlg.data.drops.memory.InMemoryDROP",
+            },
             {
                 "oid": "B",
-                "type": "app",
-                "app": "test.test_graph_loader.DummyApp",
+                "categoryType": "Application",
+                "dropclass": "test.test_graph_loader.DummyApp",
                 "inputs": ["A"],
             },
         ]
         roots = droputils.get_roots(pg_spec)
         self.assertEqual(1, len(roots))
         self.assertEqual("A", next(iter(roots)))
 
         """
         A --> C --> D --|
                         |--> E --> F
         B --------------|
         """
         pg_spec = [
-            {"oid": "A", "type": "data", "storage": Categories.MEMORY},
-            {"oid": "B", "type": "data", "storage": Categories.MEMORY},
+            {
+                "oid": "A",
+                "categoryType": "Data",
+                "dropclass": "dlg.data.drops.memory.InMemoryDROP",
+            },
+            {
+                "oid": "B",
+                "categoryType": "Data",
+                "dropclass": "dlg.data.drops.memory.InMemoryDROP",
+            },
             {
                 "oid": "C",
-                "type": "app",
-                "app": "dlg.apps.crc.CRCApp",
+                "categoryType": "Application",
+                "dropclass": "dlg.apps.crc.CRCApp",
                 "inputs": ["A"],
             },
             {
                 "oid": "D",
-                "type": "data",
-                "storage": Categories.MEMORY,
+                "categoryType": "Data",
+                "dropclass": "dlg.data.drops.memory.InMemoryDROP",
                 "producers": ["C"],
             },
             {
                 "oid": "E",
-                "type": "app",
-                "app": "test.test_drop.SumupContainerChecksum",
+                "categoryType": "Application",
+                "dropclass": "test.test_drop.SumupContainerChecksum",
                 "inputs": ["D"],
             },
             {
                 "oid": "F",
-                "type": "data",
-                "storage": Categories.MEMORY,
+                "categoryType": "Data",
+                "dropclass": "dlg.data.drops.memory.InMemoryDROP",
                 "producers": ["E"],
             },
         ]
         roots = droputils.get_roots(pg_spec)
         self.assertEqual(2, len(roots))
         self.assertListEqual(["A", "B"], sorted(roots))
```

### Comparing `daliuge-engine-2.4.0/test/test_environmentvars.py` & `daliuge-engine-3.0.0/test/test_environmentvars.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,26 +29,26 @@
 from dlg.utils import getDlgDir
 
 
 def create_std_env_vars(name="env_vars"):
     return EnvironmentVarDROP(
         oid="a",
         uid="a",
-        nm=name,
+        name=name,
         dir_var="/HOME/",
         int_var=3,
         bool_var=False,
         float_var=0.5,
         dict_var={"first": 1, "second": "sec"},
         list_var=[1, 2.0, "3"],
     )
 
 
 def create_empty_env_vars(name="env_vars"):
-    return EnvironmentVarDROP(oid="b", uid="b", nm=name)
+    return EnvironmentVarDROP(oid="b", uid="b", name=name)
 
 
 class TestEnvironmentVarDROP(unittest.TestCase):
     def test_get(self):
         """
         Tests that environment variables are read in and fetched correctly.
         """
@@ -196,15 +196,15 @@
         """
         Tests the AbstractDROP fetch routine with multiple environment drops
         """
         env1_name = "env_vars"
         env2_name = "more_vars"
         env1_drop = create_std_env_vars(name=env1_name)
         env2_drop = EnvironmentVarDROP(
-            oid="d", uid="d", nm=env2_name, dir_var="/DIFFERENT/", int_var=4
+            oid="d", uid="d", name=env2_name, dir_var="/DIFFERENT/", int_var=4
         )
         test_drop = AbstractDROP(uid="c", oid="c")
         test_drop.addProducer(env1_drop)
         test_drop.addProducer(env2_drop)
         self.assertEqual(
             "/HOME/",
             test_drop.get_environment_variable(f"${env1_name}.dir_var"),
```

### Comparing `daliuge-engine-2.4.0/test/test_event.py` & `daliuge-engine-3.0.0/test/test_event.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/test/test_graph_loader.py` & `daliuge-engine-3.0.0/test/test_graph_loader.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,46 +26,62 @@
 from dlg import graph_loader
 from dlg.ddap_protocol import DROPLinkType, DROPRel
 from dlg.data.drops.container import ContainerDROP
 from dlg.apps.app_base import AppDROP
 
 from dlg.data.drops.memory import InMemoryDROP, SharedMemoryDROP
 from dlg.data.drops.directorycontainer import DirectoryContainer
-from dlg.common import Categories
 from dlg.apps.simple import RandomArrayApp
 
 
 # Used in the textual representation of the graphs in these tests
 class DummyApp(AppDROP):
     pass
 
 
 class TestGraphLoader(unittest.TestCase):
     def test_singleMemoryDrop(self):
         dropSpecList = [
-            {"oid": "A", "type": "data", "storage": Categories.MEMORY}
+            {
+                "oid": "A",
+                "categoryType": "Data",
+                "dropclass": "dlg.data.drops.memory.InMemoryDROP",
+            }
         ]
         a = graph_loader.createGraphFromDropSpecList(dropSpecList)[0]
         self.assertIsInstance(a, InMemoryDROP)
         self.assertEqual("A", a.oid)
         self.assertEqual("A", a.uid)
 
     def test_sharedMemoryDrop(self):
         dropSpecList = [
-            {"oid": "A", "type": "data", "storage": Categories.SHMEM}
+            {
+                "oid": "A",
+                "categoryType": "Data",
+                "dropclass": "dlg.data.drops.memory.SharedMemoryDROP",
+            }
         ]
         a = graph_loader.createGraphFromDropSpecList(dropSpecList)[0]
         self.assertIsInstance(a, SharedMemoryDROP)
         self.assertEqual("A", a.oid)
         self.assertEqual("A", a.uid)
 
     def test_containerDrop(self):
         dropSpecList = [
-            {"oid": "A", "type": "data", "storage": Categories.MEMORY},
-            {"oid": "B", "type": "container", "children": ["A"]},
+            {
+                "oid": "A",
+                "categoryType": "Data",
+                "dropclass": "dlg.data.drops.memory.InMemoryDROP",
+            },
+            {
+                "oid": "B",
+                "categoryType": "container",
+                "dropclass": "dlg.data.drops.container.ContainerDROP",
+                "children": ["A"],
+            },
         ]
         a = graph_loader.createGraphFromDropSpecList(dropSpecList)[0]
         self.assertIsInstance(a, InMemoryDROP)
         self.assertEqual("A", a.oid)
         self.assertEqual("A", a.uid)
         self.assertIsNotNone(a.parent)
         b = a.parent
@@ -73,42 +89,42 @@
         self.assertEqual("B", b.oid)
         self.assertEqual("B", b.uid)
 
         # A directory container
         dropSpecList = [
             {
                 "oid": "A",
-                "type": "data",
-                "storage": Categories.FILE,
+                "categoryType": "Data",
+                "dropclass": "dlg.data.drops.file.FileDROP",
                 "dirname": ".",
             },
             {
                 "oid": "B",
-                "type": "container",
-                "container": "dlg.data.drops.DirectoryContainer",
+                "categoryType": "Container",
+                "dropclass": "dlg.data.drops.DirectoryContainer",
                 "children": ["A"],
                 "dirname": ".",
             },
         ]
         a = graph_loader.createGraphFromDropSpecList(dropSpecList)[0]
         b = a.parent
         self.assertIsInstance(b, DirectoryContainer)
 
     def test_consumer(self):
         dropSpecList = [
             {
                 "oid": "A",
-                "type": "data",
-                "storage": Categories.MEMORY,
+                "categoryType": "Data",
+                "dropclass": "dlg.data.drops.memory.InMemoryDROP",
                 "consumers": ["B"],
             },
             {
                 "oid": "B",
-                "type": "app",
-                "app": "test.test_graph_loader.DummyApp",
+                "categoryType": "Application",
+                "dropclass": "test.test_graph_loader.DummyApp",
             },
         ]
         a = graph_loader.createGraphFromDropSpecList(dropSpecList)[0]
         self.assertIsInstance(a, InMemoryDROP)
         self.assertEqual("A", a.oid)
         self.assertEqual("A", a.uid)
         self.assertEqual(1, len(a.consumers))
@@ -154,15 +170,14 @@
         self.assertEqual("B", a["consumers"][0])
         self.assertFalse("producers" in a and len(a["producers"]) > 0)
         self.assertFalse(
             "streamingConsumers" in c and len(c["streamingConsumers"]) > 0
         )
 
     def test_removeUnmetRelationships_named(self):
-
         with pkg_resources.resource_stream(
             "test", "graphs/HelloWorld_simplePG.graph"
         ) as f:  # @UndefinedVariable
             graphDesc = json.load(f)
 
         unmetRelationships = graph_loader.removeUnmetRelationships(graphDesc)
         self.assertEqual(0, len(unmetRelationships))
@@ -219,16 +234,16 @@
             ("persist", False),
             (None, False),  # Default of False is specific to MemoryDrops
         ]
         for key, value in testCases:
             with self.subTest(key=key, value=value):
                 dropSpec = {
                     "oid": "A",
-                    "type": "data",
-                    "storage": Categories.MEMORY,
+                    "categoryType": "Data",
+                    "dropclass": "dlg.data.drops.memory.InMemoryDROP",
                 }
                 if key is not None:
                     dropSpec[key] = value
 
                 graph = graph_loader.createGraphFromDropSpecList([dropSpec])
                 data = graph[0]
                 self.assertIsInstance(data, InMemoryDROP)
```

### Comparing `daliuge-engine-2.4.0/test/test_input_fired_app_drop.py` & `daliuge-engine-3.0.0/test/test_input_fired_app_drop.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/test/test_shared_memory.py` & `daliuge-engine-3.0.0/test/test_shared_memory.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/test/test_tool.py` & `daliuge-engine-3.0.0/test/test_tool.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-2.4.0/test/test_utils.py` & `daliuge-engine-3.0.0/test/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 import zlib
 
 from dlg import utils
 
 
 class TestUtils(unittest.TestCase):
     def test_zlib_uncompressed_stream(self):
-
         fname = tempfile.mktemp()
         with open(fname, "wb") as f:
             f.write(zlib.compress(b"abc"))
 
         # Read parts from the beginning
         for b, n in ((b"abc", 3), (b"ab", 2), (b"a", 1)):
             with open(fname, "rb") as f:
@@ -50,51 +49,54 @@
             self.assertEqual(b"b", s.read(1))
             self.assertEqual(b"c", s.read(1))
             self.assertEqual(0, s.buflen)
 
         os.remove(fname)
 
         # Try now with bigger data sizes
-        for size in [2 ** x + y for x in range(3, 18) for y in (-1, 0, 1)]:
-
+        for size in [2**x + y for x in range(3, 18) for y in (-1, 0, 1)]:
             original_bytes = os.urandom(size)
             compressed_bytes = zlib.compress(original_bytes)
 
             # Try first with whole reads
             compressed_stream = io.BytesIO(compressed_bytes)
-            uncompressed_stream = utils.ZlibUncompressedStream(compressed_stream)
+            uncompressed_stream = utils.ZlibUncompressedStream(
+                compressed_stream
+            )
             b = uncompressed_stream.read()
             self.assertEqual(size, len(b))
             self.assertEqual(original_bytes, b)
 
             # Now read little by little
             read_size = min(size // 4, 1024)
             b = b""
             compressed_stream = io.BytesIO(compressed_bytes)
-            uncompressed_stream = utils.ZlibUncompressedStream(compressed_stream)
-            for u in iter(functools.partial(uncompressed_stream.read, read_size), b""):
+            uncompressed_stream = utils.ZlibUncompressedStream(
+                compressed_stream
+            )
+            for u in iter(
+                functools.partial(uncompressed_stream.read, read_size), b""
+            ):
                 b += u
             self.assertEqual(size, len(b))
             self.assertEqual(original_bytes, b)
 
     def test_zlib_compressed_stream_writer(self):
-
         compressed_ref = zlib.compress(b"abcd")
 
         # Read parts from the beginning
         for x in range(1, len(compressed_ref)):
             bytesio = io.BytesIO(b"abcd")
             s = utils.ZlibCompressedStream(bytesio)
             compressed = s.read(x)
             self.assertEqual(x, len(compressed))
             self.assertEqual(compressed_ref[0:x], compressed[0:x])
 
         # Try now with bigger data sizes
-        for size in [2 ** x + y for x in range(3, 18) for y in (-1, 0, 1)]:
-
+        for size in [2**x + y for x in range(3, 18) for y in (-1, 0, 1)]:
             original_bytes = os.urandom(size)
             compressed_bytes = zlib.compress(original_bytes)
 
             # Try first with whole reads
             uncompressed_stream = io.BytesIO(original_bytes)
             compressed_stream = utils.ZlibCompressedStream(uncompressed_stream)
             b = compressed_stream.read()
@@ -106,15 +108,17 @@
             self.assertEqual(compressed_bytes, b)
 
             # Now read little by little
             read_size = min(size // 4, 1024)
             uncompressed_stream = io.BytesIO(original_bytes)
             compressed_stream = utils.ZlibCompressedStream(uncompressed_stream)
             b = b""
-            for c in iter(functools.partial(compressed_stream.read, read_size), b""):
+            for c in iter(
+                functools.partial(compressed_stream.read, read_size), b""
+            ):
                 b += c
             self.assertEqual(
                 len(compressed_bytes),
                 len(b),
                 "Incorrect size when compressing %d bytes" % (size),
             )
             self.assertEqual(compressed_bytes, b)
@@ -122,80 +126,82 @@
     def test_zlib_streams_combined_randombytes(self):
         self._test_zlib_streams_combined(os.urandom)
 
     def test_zlib_streams_combined_zerobytes(self):
         self._test_zlib_streams_combined(lambda n: b"0" * n)
 
     def _test_zlib_streams_combined(self, gen_bytes):
-
-        sizes = [2 ** x + y for x in range(1, 18) for y in (-1, 0, 1)]
+        sizes = [2**x + y for x in range(1, 18) for y in (-1, 0, 1)]
         for size in sizes:
-
             original_bytes = gen_bytes(size)
 
             # Read the whole thing
             original_stream = io.BytesIO(original_bytes)
             compressed_stream = utils.ZlibCompressedStream(original_stream)
-            uncompressed_stream = utils.ZlibUncompressedStream(compressed_stream)
+            uncompressed_stream = utils.ZlibUncompressedStream(
+                compressed_stream
+            )
             b = uncompressed_stream.read()
             self.assertEqual(size, len(b))
             self.assertEqual(original_bytes, b)
 
             # There's nothing left now to read
             for x in range(10):
                 self.assertEqual(0, len(uncompressed_stream.read(100)))
 
             # Read with given number of bytes
             for n in (1, len(original_bytes) // 2, len(original_bytes)):
-
                 these_bytes = original_bytes[0:n]
 
                 original_stream = io.BytesIO(these_bytes)
                 compressed_stream = utils.ZlibCompressedStream(original_stream)
-                uncompressed_stream = utils.ZlibUncompressedStream(compressed_stream)
+                uncompressed_stream = utils.ZlibUncompressedStream(
+                    compressed_stream
+                )
 
                 b = uncompressed_stream.read(n)
                 self.assertEqual(n, len(b))
                 self.assertEqual(these_bytes, b)
 
                 # There's nothing left now to read
                 for x in range(10):
                     self.assertEqual(0, len(uncompressed_stream.read(100)))
 
     def test_json_stream_simple_sequence(self):
-        for s in ([0], [{}], ["a"], [{"oid": "A", "type": "data"}]):
+        for s in ([0], [{}], ["a"], [{"oid": "A", "categoryType": "Data"}]):
             stream = utils.JSONStream(s)
             self.assertEqual(s, json.loads(stream.read(100).decode("utf8")))
 
     def test_json_stream_sequences(self):
-
         ref = [1, 2, 3]
         objects_list = [1, 2, 3]
         objects_tuple = (1, 2, 3)
 
         def objects_gen():
             yield 1
             yield 2
             yield 3
 
         for objects in (objects_list, objects_tuple, objects_gen()):
             stream = utils.JSONStream(objects)
-            self.assertSequenceEqual(ref, json.loads(stream.read(100).decode("latin1")))
+            self.assertSequenceEqual(
+                ref, json.loads(stream.read(100).decode("latin1"))
+            )
             self.assertEqual(0, len(stream.read(100).decode("latin1")))
 
     def test_json_stream_simpleobj(self):
-
         sessionId = "some_id"
         for obj in (1, {"a": 2}, "b", {"sessionId": sessionId}):
             stream = utils.JSONStream(obj)
-            self.assertEqual(obj, json.loads(stream.read(100).decode("latin1")))
+            self.assertEqual(
+                obj, json.loads(stream.read(100).decode("latin1"))
+            )
             self.assertEqual(0, len(stream.read(100).decode("latin1")))
 
     def test_get_dlg_root(self):
-
         # It should obey the DLG_ROOT environment variable
         old = os.environ.get("DLG_ROOT", None)
         os.environ["DLG_ROOT"] = tempfile.mkdtemp()
         self.assertEqual(utils.getDlgDir(), os.environ["DLG_ROOT"])
         os.rmdir(os.environ["DLG_ROOT"])
         if old:
             os.environ["DLG_ROOT"] = old
```

