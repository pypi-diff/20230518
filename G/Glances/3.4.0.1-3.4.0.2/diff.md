# Comparing `tmp/Glances-3.4.0.1.tar.gz` & `tmp/Glances-3.4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Glances-3.4.0.1.tar", last modified: Wed May 17 09:30:02 2023, max compression
+gzip compressed data, was "Glances-3.4.0.2.tar", last modified: Thu May 18 15:46:21 2023, max compression
```

## Comparing `Glances-3.4.0.1.tar` & `Glances-3.4.0.2.tar`

### file list

```diff
@@ -1,335 +1,335 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.385920 Glances-3.4.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-17 09:29:53.000000 Glances-3.4.0.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-05-17 09:29:53.000000 Glances-3.4.0.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    42098 2023-05-17 09:29:53.000000 Glances-3.4.0.1/COPYING
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.333919 Glances-3.4.0.1/Glances.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-05-17 09:30:02.000000 Glances-3.4.0.1/Glances.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-05-17 09:30:02.000000 Glances-3.4.0.1/Glances.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 09:30:02.000000 Glances-3.4.0.1/Glances.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-17 09:30:02.000000 Glances-3.4.0.1/Glances.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-17 09:30:02.000000 Glances-3.4.0.1/Glances.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-17 09:30:02.000000 Glances-3.4.0.1/Glances.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-17 09:29:53.000000 Glances-3.4.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    70564 2023-05-17 09:29:53.000000 Glances-3.4.0.1/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-05-17 09:30:02.385920 Glances-3.4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16100 2023-05-17 09:29:53.000000 Glances-3.4.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.333919 Glances-3.4.0.1/conf/
--rw-r--r--   0 runner    (1001) docker     (123)    20996 2023-05-17 09:29:53.000000 Glances-3.4.0.1/conf/glances.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.337919 Glances-3.4.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.353919 Glances-3.4.0.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    29273 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/amp-dropbox.png
--rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/amp-python-warning.png
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/amp-python.png
--rw-r--r--   0 runner    (1001) docker     (123)    80498 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/amps.png
--rw-r--r--   0 runner    (1001) docker     (123)    13916 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/aws.png
--rw-r--r--   0 runner    (1001) docker     (123)    44160 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/browser.png
--rw-r--r--   0 runner    (1001) docker     (123)    21111 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/cloud.png
--rw-r--r--   0 runner    (1001) docker     (123)     9442 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/connected.png
--rw-r--r--   0 runner    (1001) docker     (123)    29245 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/connections.png
--rw-r--r--   0 runner    (1001) docker     (123)    34093 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/containers.png
--rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/cpu-wide.png
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/cpu.png
--rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/disconnected.png
--rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/diskio.png
--rw-r--r--   0 runner    (1001) docker     (123)    24808 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/events.png
--rw-r--r--   0 runner    (1001) docker     (123)    13715 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/folders.png
--rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/fs.png
--rw-r--r--   0 runner    (1001) docker     (123)    56273 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/glances-architecture.excalidraw
--rw-r--r--   0 runner    (1001) docker     (123)   123499 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/glances-architecture.png
--rw-r--r--   0 runner    (1001) docker     (123)   215750 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/glances-flame.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/glances-influxdb.png
--rw-r--r--   0 runner    (1001) docker     (123)    33567 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/glances-memory-profiling-with-history.png
--rw-r--r--   0 runner    (1001) docker     (123)    31797 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/glances-memory-profiling-without-history.png
--rw-r--r--   0 runner    (1001) docker     (123)   293649 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/glances-responsive-webdesign.png
--rw-r--r--   0 runner    (1001) docker     (123)   357638 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/glances-summary.png
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/gpu.png
--rw-r--r--   0 runner    (1001) docker     (123)   141657 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/grafana.png
--rw-r--r--   0 runner    (1001) docker     (123)   187140 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/graph-load.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14415 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/hddtemp.png
--rw-r--r--   0 runner    (1001) docker     (123)    19879 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/header.png
--rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/ip.png
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/irq.png
--rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/load.png
--rw-r--r--   0 runner    (1001) docker     (123)    20009 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/loadpercent.png
--rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/mem-wide.png
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/mem.png
--rw-r--r--   0 runner    (1001) docker     (123)    12190 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/monitored.png
--rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/network.png
--rw-r--r--   0 runner    (1001) docker     (123)    21132 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/per-cpu.png
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/pergpu.png
--rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/ports.png
--rw-r--r--   0 runner    (1001) docker     (123)    63154 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/processlist-extended.png
--rw-r--r--   0 runner    (1001) docker     (123)   160408 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/processlist-filter.png
--rw-r--r--   0 runner    (1001) docker     (123)    53684 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/processlist-top.png
--rw-r--r--   0 runner    (1001) docker     (123)   227401 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/processlist-wide.png
--rw-r--r--   0 runner    (1001) docker     (123)   151590 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/processlist.png
--rw-r--r--   0 runner    (1001) docker     (123)    25081 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/prometheus_exporter.png
--rw-r--r--   0 runner    (1001) docker     (123)    91914 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/prometheus_server.png
--rw-r--r--   0 runner    (1001) docker     (123)    27582 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/quicklook-percpu.png
--rw-r--r--   0 runner    (1001) docker     (123)    17789 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/quicklook.png
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/raid.png
--rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/reddit.png
--rw-r--r--   0 runner    (1001) docker     (123)  1089975 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/screencast.gif
--rw-r--r--   0 runner    (1001) docker     (123)   265567 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/screenshot-web.png
--rw-r--r--   0 runner    (1001) docker     (123)    36097 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/screenshot-web2.png
--rw-r--r--   0 runner    (1001) docker     (123)  1098062 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/screenshot-wide.png
--rw-r--r--   0 runner    (1001) docker     (123)   508044 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/screenshot.png
--rw-r--r--   0 runner    (1001) docker     (123)    16125 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/sensors.png
--rw-r--r--   0 runner    (1001) docker     (123)    21500 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/smart.png
--rw-r--r--   0 runner    (1001) docker     (123)    41952 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/sparkline.png
--rw-r--r--   0 runner    (1001) docker     (123)    23021 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/trend.png
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/twitter-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/wifi.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.353919 Glances-3.4.0.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_templates/links.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.357920 Glances-3.4.0.1/docs/aoa/
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/actions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/amps.rst
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/cloud.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/connections.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/containers.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/cpu.rst
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/diskio.rst
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/events.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/folders.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/fs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/gpu.rst
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/hddtemp.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/header.rst
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/irq.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/load.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/memory.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/network.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/ports.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/ps.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/quicklook.rst
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/raid.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/sensors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/smart.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/wifi.rst
--rw-r--r--   0 runner    (1001) docker     (123)    44115 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/api.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/build.sh
--rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/cmds.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9804 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/config.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.357920 Glances-3.4.0.1/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/dev/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)   328258 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/dev/glances-cprofile.png
--rw-r--r--   0 runner    (1001) docker     (123)     7159 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/docker.rst
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/glances.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.361919 Glances-3.4.0.1/docs/gw/
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/gw/cassandra.rst
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/gw/couchdb.rst
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/gw/csv.rst
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/gw/elastic.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/gw/graph.rst
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/gw/graphite.rst
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/gw/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/gw/influxdb.rst
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/gw/json.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/gw/kafka.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/gw/mongodb.rst
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/gw/mqtt.rst
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/gw/opentsdb.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/gw/prometheus.rst
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/gw/rabbitmq.rst
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/gw/restful.rst
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/gw/riemann.rst
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/gw/statsd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/gw/zeromq.rst
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.361919 Glances-3.4.0.1/docs/man/
--rw-r--r--   0 runner    (1001) docker     (123)    17939 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/man/glances.1
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/objects.inv
--rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/support.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.365920 Glances-3.4.0.1/glances/
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/actions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.365920 Glances-3.4.0.1/glances/amps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/amps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/amps/glances_amp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/amps/glances_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/amps/glances_nginx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/amps/glances_systemd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/amps/glances_systemv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/amps_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/autodiscover.py
--rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10078 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/client_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    11671 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/cpu_percent.py
--rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.369920 Glances-3.4.0.1/glances/exports/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/glances_cassandra.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/glances_couchdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/glances_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/glances_elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/glances_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/glances_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/glances_graphite.py
--rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/glances_influxdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/glances_influxdb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/glances_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/glances_kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/glances_mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/glances_mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/glances_opentsdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/glances_prometheus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/glances_rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/glances_restful.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/glances_riemann.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/glances_statsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/glances_zeromq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/folder_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    29248 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outdated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.369920 Glances-3.4.0.1/glances/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/glances_bars.py
--rw-r--r--   0 runner    (1001) docker     (123)    21397 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/glances_bottle.py
--rw-r--r--   0 runner    (1001) docker     (123)    49367 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/glances_curses.py
--rw-r--r--   0 runner    (1001) docker     (123)    12659 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/glances_curses_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/glances_sparklines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/glances_stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/glances_stdout_apidoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/glances_stdout_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/glances_stdout_issue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/glances_stdout_json.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/glances_unicode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.373920 Glances-3.4.0.1/glances/outputs/static/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/.eslintrc.js
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/.prettierrc.js
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.373920 Glances-3.4.0.1/glances/outputs/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/css/bootstrap.less
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/css/style.scss
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/css/variables.less
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.373920 Glances-3.4.0.1/glances/outputs/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    43588 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/images/glances.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.373920 Glances-3.4.0.1/glances/outputs/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    17135 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/App.vue
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/app.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.377920 Glances-3.4.0.1/glances/outputs/static/js/components/
--rw-r--r--   0 runner    (1001) docker     (123)    11318 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/help.vue
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-alert.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-amps.vue
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-cloud.vue
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-connections.vue
--rw-r--r--   0 runner    (1001) docker     (123)     7148 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-containers.vue
--rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-cpu.vue
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-diskio.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-folders.vue
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-fs.vue
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-gpu.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-ip.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-irq.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-load.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-mem-more.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-mem.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-memswap.vue
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-network.vue
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-now.vue
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-percpu.vue
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-ports.vue
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-process.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-processcount.vue
--rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-processlist.vue
--rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-quicklook.vue
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-raid.vue
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-sensors.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-system.vue
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-uptime.vue
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-wifi.vue
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/filters.js
--rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/services.js
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/store.js
--rw-r--r--   0 runner    (1001) docker     (123)   445972 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.377920 Glances-3.4.0.1/glances/outputs/static/public/
--rw-r--r--   0 runner    (1001) docker     (123)    43588 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/public/87708faeed9a66b0fcdb.png
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/public/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)   444157 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/public/glances.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.377920 Glances-3.4.0.1/glances/outputs/static/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/templates/index.html.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/webpack.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/password.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/password_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.385920 Glances-3.4.0.1/glances/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.385920 Glances-3.4.0.1/glances/plugins/containers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13743 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/containers/glances_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)    12923 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/containers/glances_podman.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/containers/stats_streamer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11056 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_amps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_connections.py
--rw-r--r--   0 runner    (1001) docker     (123)    16847 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    15759 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     8920 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_diskio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_folders.py
--rw-r--r--   0 runner    (1001) docker     (123)    10639 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_fs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_help.py
--rw-r--r--   0 runner    (1001) docker     (123)    10957 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_irq.py
--rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_load.py
--rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_mem.py
--rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_memswap.py
--rw-r--r--   0 runner    (1001) docker     (123)    15881 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_now.py
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_percpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    42555 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_ports.py
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_processcount.py
--rw-r--r--   0 runner    (1001) docker     (123)    34269 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_processlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_psutilversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_quicklook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_raid.py
--rw-r--r--   0 runner    (1001) docker     (123)    13757 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_smart.py
--rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_uptime.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_wifi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.385920 Glances-3.4.0.1/glances/plugins/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/sensors/glances_batpercent.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/sensors/glances_hddtemp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/ports_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    23868 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/programs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/secure.py
--rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/snmp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/standalone.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/static_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/stats_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/stats_client_snmp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/stats_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/thresholds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/web_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/webserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-17 09:29:53.000000 Glances-3.4.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 09:30:02.385920 Glances-3.4.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4992 2023-05-17 09:29:53.000000 Glances-3.4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.140455 Glances-3.4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-18 15:46:13.000000 Glances-3.4.0.2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-05-18 15:46:13.000000 Glances-3.4.0.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    42098 2023-05-18 15:46:13.000000 Glances-3.4.0.2/COPYING
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.096455 Glances-3.4.0.2/Glances.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-05-18 15:46:21.000000 Glances-3.4.0.2/Glances.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-05-18 15:46:21.000000 Glances-3.4.0.2/Glances.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:46:21.000000 Glances-3.4.0.2/Glances.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-18 15:46:21.000000 Glances-3.4.0.2/Glances.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-18 15:46:21.000000 Glances-3.4.0.2/Glances.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-18 15:46:21.000000 Glances-3.4.0.2/Glances.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-18 15:46:13.000000 Glances-3.4.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    70747 2023-05-18 15:46:13.000000 Glances-3.4.0.2/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-05-18 15:46:21.140455 Glances-3.4.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16100 2023-05-18 15:46:13.000000 Glances-3.4.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.096455 Glances-3.4.0.2/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)    20996 2023-05-18 15:46:13.000000 Glances-3.4.0.2/conf/glances.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.100455 Glances-3.4.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.112455 Glances-3.4.0.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    29273 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/amp-dropbox.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/amp-python-warning.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/amp-python.png
+-rw-r--r--   0 runner    (1001) docker     (123)    80498 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/amps.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13916 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/aws.png
+-rw-r--r--   0 runner    (1001) docker     (123)    44160 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/browser.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21111 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/cloud.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9442 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/connected.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29245 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/connections.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34093 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/containers.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/cpu-wide.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/cpu.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/disconnected.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/diskio.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24808 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/events.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13715 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/folders.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/fs.png
+-rw-r--r--   0 runner    (1001) docker     (123)    56273 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/glances-architecture.excalidraw
+-rw-r--r--   0 runner    (1001) docker     (123)   123499 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/glances-architecture.png
+-rw-r--r--   0 runner    (1001) docker     (123)   215750 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/glances-flame.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/glances-influxdb.png
+-rw-r--r--   0 runner    (1001) docker     (123)    33567 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/glances-memory-profiling-with-history.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31797 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/glances-memory-profiling-without-history.png
+-rw-r--r--   0 runner    (1001) docker     (123)   293649 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/glances-responsive-webdesign.png
+-rw-r--r--   0 runner    (1001) docker     (123)   357638 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/glances-summary.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/gpu.png
+-rw-r--r--   0 runner    (1001) docker     (123)   141657 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/grafana.png
+-rw-r--r--   0 runner    (1001) docker     (123)   187140 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/graph-load.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14415 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/hddtemp.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19879 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/header.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/ip.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/irq.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/load.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20009 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/loadpercent.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/mem-wide.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/mem.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12190 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/monitored.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/network.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21132 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/per-cpu.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/pergpu.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/ports.png
+-rw-r--r--   0 runner    (1001) docker     (123)    63154 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/processlist-extended.png
+-rw-r--r--   0 runner    (1001) docker     (123)   160408 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/processlist-filter.png
+-rw-r--r--   0 runner    (1001) docker     (123)    53684 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/processlist-top.png
+-rw-r--r--   0 runner    (1001) docker     (123)   227401 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/processlist-wide.png
+-rw-r--r--   0 runner    (1001) docker     (123)   151590 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/processlist.png
+-rw-r--r--   0 runner    (1001) docker     (123)    25081 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/prometheus_exporter.png
+-rw-r--r--   0 runner    (1001) docker     (123)    91914 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/prometheus_server.png
+-rw-r--r--   0 runner    (1001) docker     (123)    27582 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/quicklook-percpu.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17789 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/quicklook.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/raid.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/reddit.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1089975 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/screencast.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   265567 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/screenshot-web.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36097 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/screenshot-web2.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1098062 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/screenshot-wide.png
+-rw-r--r--   0 runner    (1001) docker     (123)   508044 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16125 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/sensors.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21500 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/smart.png
+-rw-r--r--   0 runner    (1001) docker     (123)    41952 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/sparkline.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23021 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/trend.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/twitter-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/wifi.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.112455 Glances-3.4.0.2/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_templates/links.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.116455 Glances-3.4.0.2/docs/aoa/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/actions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/amps.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/cloud.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/connections.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/containers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/cpu.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/diskio.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/events.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/folders.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/fs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/gpu.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/hddtemp.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/header.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/irq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/load.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/memory.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/network.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/ports.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/ps.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/quicklook.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/raid.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/sensors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/smart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/wifi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    44330 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/api.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/build.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/cmds.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9804 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/config.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.116455 Glances-3.4.0.2/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/dev/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   328258 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/dev/glances-cprofile.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7159 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/docker.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/glances.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.116455 Glances-3.4.0.2/docs/gw/
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/gw/cassandra.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/gw/couchdb.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/gw/csv.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/gw/elastic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/gw/graph.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/gw/graphite.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/gw/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/gw/influxdb.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/gw/json.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/gw/kafka.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/gw/mongodb.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/gw/mqtt.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/gw/opentsdb.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/gw/prometheus.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/gw/rabbitmq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/gw/restful.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/gw/riemann.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/gw/statsd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/gw/zeromq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.120455 Glances-3.4.0.2/docs/man/
+-rw-r--r--   0 runner    (1001) docker     (123)    17939 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/man/glances.1
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/objects.inv
+-rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/support.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.124455 Glances-3.4.0.2/glances/
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.124455 Glances-3.4.0.2/glances/amps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/amps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/amps/glances_amp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/amps/glances_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/amps/glances_nginx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/amps/glances_systemd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/amps/glances_systemv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/amps_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/autodiscover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10078 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/client_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11671 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/cpu_percent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.128455 Glances-3.4.0.2/glances/exports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/glances_cassandra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/glances_couchdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/glances_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/glances_elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/glances_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/glances_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/glances_graphite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/glances_influxdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/glances_influxdb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/glances_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/glances_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/glances_mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/glances_mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/glances_opentsdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/glances_prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/glances_rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/glances_restful.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/glances_riemann.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/glances_statsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/glances_zeromq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/folder_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29248 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outdated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.128455 Glances-3.4.0.2/glances/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/glances_bars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21397 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/glances_bottle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49367 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/glances_curses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12659 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/glances_curses_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/glances_sparklines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/glances_stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/glances_stdout_apidoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/glances_stdout_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/glances_stdout_issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/glances_stdout_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/glances_unicode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.128455 Glances-3.4.0.2/glances/outputs/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/.eslintrc.js
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/.prettierrc.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.128455 Glances-3.4.0.2/glances/outputs/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/css/bootstrap.less
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/css/style.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/css/variables.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.128455 Glances-3.4.0.2/glances/outputs/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    43588 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/images/glances.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.132455 Glances-3.4.0.2/glances/outputs/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    17135 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/App.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/app.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.132455 Glances-3.4.0.2/glances/outputs/static/js/components/
+-rw-r--r--   0 runner    (1001) docker     (123)    11318 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/help.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-alert.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-amps.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-cloud.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-connections.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     7148 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-containers.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-cpu.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-diskio.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-folders.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-fs.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-gpu.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-ip.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-irq.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-load.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-mem-more.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-mem.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-memswap.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-network.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-now.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-percpu.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-ports.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-process.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-processcount.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-processlist.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-quicklook.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-raid.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-sensors.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-system.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-uptime.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-wifi.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/filters.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/services.js
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/store.js
+-rw-r--r--   0 runner    (1001) docker     (123)   445972 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.132455 Glances-3.4.0.2/glances/outputs/static/public/
+-rw-r--r--   0 runner    (1001) docker     (123)    43588 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/public/87708faeed9a66b0fcdb.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/public/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)   444157 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/public/glances.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.136455 Glances-3.4.0.2/glances/outputs/static/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/templates/index.html.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/webpack.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/password_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.140455 Glances-3.4.0.2/glances/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.140455 Glances-3.4.0.2/glances/plugins/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13743 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/containers/glances_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12923 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/containers/glances_podman.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/containers/stats_streamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11056 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_amps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16847 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15759 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8920 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_diskio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10639 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10957 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_irq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_mem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_memswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15881 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_now.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_percpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42555 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_processcount.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34269 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_processlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_psutilversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_quicklook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_raid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13757 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_smart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_uptime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_wifi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.140455 Glances-3.4.0.2/glances/plugins/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/sensors/glances_batpercent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/sensors/glances_hddtemp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/ports_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23868 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/programs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/secure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/snmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/standalone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/static_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/stats_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/stats_client_snmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/stats_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/thresholds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/web_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/webserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-18 15:46:13.000000 Glances-3.4.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:46:21.140455 Glances-3.4.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4992 2023-05-18 15:46:13.000000 Glances-3.4.0.2/setup.py
```

### Comparing `Glances-3.4.0.1/AUTHORS` & `Glances-3.4.0.2/AUTHORS`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/CONTRIBUTING.md` & `Glances-3.4.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/COPYING` & `Glances-3.4.0.2/COPYING`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/Glances.egg-info/PKG-INFO` & `Glances-3.4.0.2/Glances.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Glances
-Version: 3.4.0.1
+Version: 3.4.0.2
 Summary: A cross-platform curses-based monitoring tool
 Home-page: https://github.com/nicolargo/glances
 Author: Nicolas Hennion
 Author-email: nicolas@nicolargo.com
 License: LGPLv3
 Keywords: cli curses monitoring system
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Glances-3.4.0.1/Glances.egg-info/SOURCES.txt` & `Glances-3.4.0.2/Glances.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/Glances.egg-info/requires.txt` & `Glances-3.4.0.2/Glances.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/NEWS.rst` & `Glances-3.4.0.2/NEWS.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 ==============================================================================
                                 Glances changelog
 ==============================================================================
 
 ===============
+Version 3.4.0.2
+===============
+
+Bugs corrected:
+
+    * Cannot start Glances 3.4.0.1 on Windows 10: SIGHUP not defined #2408
+    * Influxdb2 export not working #2407
+
+===============
 Version 3.4.0.1
 ===============
 
 Bug corrected:
 
     * 3.4.0 crash on startupwith minimal deps #2401
```

### Comparing `Glances-3.4.0.1/PKG-INFO` & `Glances-3.4.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Glances
-Version: 3.4.0.1
+Version: 3.4.0.2
 Summary: A cross-platform curses-based monitoring tool
 Home-page: https://github.com/nicolargo/glances
 Author: Nicolas Hennion
 Author-email: nicolas@nicolargo.com
 License: LGPLv3
 Keywords: cli curses monitoring system
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Glances-3.4.0.1/README.rst` & `Glances-3.4.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/conf/glances.conf` & `Glances-3.4.0.2/conf/glances.conf`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/Makefile` & `Glances-3.4.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/amp-dropbox.png` & `Glances-3.4.0.2/docs/_static/amp-dropbox.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/amp-python-warning.png` & `Glances-3.4.0.2/docs/_static/amp-python-warning.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/amp-python.png` & `Glances-3.4.0.2/docs/_static/amp-python.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/amps.png` & `Glances-3.4.0.2/docs/_static/amps.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/aws.png` & `Glances-3.4.0.2/docs/_static/aws.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/browser.png` & `Glances-3.4.0.2/docs/_static/browser.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/cloud.png` & `Glances-3.4.0.2/docs/_static/cloud.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/connected.png` & `Glances-3.4.0.2/docs/_static/connected.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/connections.png` & `Glances-3.4.0.2/docs/_static/connections.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/containers.png` & `Glances-3.4.0.2/docs/_static/containers.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/cpu-wide.png` & `Glances-3.4.0.2/docs/_static/cpu-wide.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/cpu.png` & `Glances-3.4.0.2/docs/_static/cpu.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/disconnected.png` & `Glances-3.4.0.2/docs/_static/disconnected.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/diskio.png` & `Glances-3.4.0.2/docs/_static/diskio.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/events.png` & `Glances-3.4.0.2/docs/_static/events.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/folders.png` & `Glances-3.4.0.2/docs/_static/folders.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/fs.png` & `Glances-3.4.0.2/docs/_static/fs.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/glances-architecture.excalidraw` & `Glances-3.4.0.2/docs/_static/glances-architecture.excalidraw`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/glances-architecture.png` & `Glances-3.4.0.2/docs/_static/glances-architecture.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/glances-flame.svg` & `Glances-3.4.0.2/docs/_static/glances-flame.svg`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/glances-influxdb.png` & `Glances-3.4.0.2/docs/_static/glances-influxdb.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/glances-memory-profiling-with-history.png` & `Glances-3.4.0.2/docs/_static/glances-memory-profiling-with-history.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/glances-memory-profiling-without-history.png` & `Glances-3.4.0.2/docs/_static/glances-memory-profiling-without-history.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/glances-responsive-webdesign.png` & `Glances-3.4.0.2/docs/_static/glances-responsive-webdesign.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/glances-summary.png` & `Glances-3.4.0.2/docs/_static/glances-summary.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/gpu.png` & `Glances-3.4.0.2/docs/_static/gpu.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/grafana.png` & `Glances-3.4.0.2/docs/_static/grafana.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/graph-load.svg` & `Glances-3.4.0.2/docs/_static/graph-load.svg`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/hddtemp.png` & `Glances-3.4.0.2/docs/_static/hddtemp.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/header.png` & `Glances-3.4.0.2/docs/_static/header.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/ip.png` & `Glances-3.4.0.2/docs/_static/ip.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/irq.png` & `Glances-3.4.0.2/docs/_static/irq.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/load.png` & `Glances-3.4.0.2/docs/_static/load.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/loadpercent.png` & `Glances-3.4.0.2/docs/_static/loadpercent.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/mem-wide.png` & `Glances-3.4.0.2/docs/_static/mem-wide.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/mem.png` & `Glances-3.4.0.2/docs/_static/mem.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/monitored.png` & `Glances-3.4.0.2/docs/_static/monitored.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/network.png` & `Glances-3.4.0.2/docs/_static/network.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/per-cpu.png` & `Glances-3.4.0.2/docs/_static/per-cpu.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/pergpu.png` & `Glances-3.4.0.2/docs/_static/pergpu.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/ports.png` & `Glances-3.4.0.2/docs/_static/ports.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/processlist-extended.png` & `Glances-3.4.0.2/docs/_static/processlist-extended.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/processlist-filter.png` & `Glances-3.4.0.2/docs/_static/processlist-filter.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/processlist-top.png` & `Glances-3.4.0.2/docs/_static/processlist-top.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/processlist-wide.png` & `Glances-3.4.0.2/docs/_static/processlist-wide.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/processlist.png` & `Glances-3.4.0.2/docs/_static/processlist.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/prometheus_exporter.png` & `Glances-3.4.0.2/docs/_static/prometheus_exporter.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/prometheus_server.png` & `Glances-3.4.0.2/docs/_static/prometheus_server.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/quicklook-percpu.png` & `Glances-3.4.0.2/docs/_static/quicklook-percpu.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/quicklook.png` & `Glances-3.4.0.2/docs/_static/quicklook.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/raid.png` & `Glances-3.4.0.2/docs/_static/raid.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/reddit.png` & `Glances-3.4.0.2/docs/_static/reddit.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/screencast.gif` & `Glances-3.4.0.2/docs/_static/screencast.gif`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/screenshot-web.png` & `Glances-3.4.0.2/docs/_static/screenshot-web.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/screenshot-web2.png` & `Glances-3.4.0.2/docs/_static/screenshot-web2.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/screenshot-wide.png` & `Glances-3.4.0.2/docs/_static/screenshot-wide.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/screenshot.png` & `Glances-3.4.0.2/docs/_static/screenshot.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/sensors.png` & `Glances-3.4.0.2/docs/_static/sensors.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/smart.png` & `Glances-3.4.0.2/docs/_static/smart.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/sparkline.png` & `Glances-3.4.0.2/docs/_static/sparkline.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/trend.png` & `Glances-3.4.0.2/docs/_static/trend.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/twitter-icon.png` & `Glances-3.4.0.2/docs/_static/twitter-icon.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/_static/wifi.png` & `Glances-3.4.0.2/docs/_static/wifi.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/aoa/actions.rst` & `Glances-3.4.0.2/docs/aoa/actions.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/aoa/amps.rst` & `Glances-3.4.0.2/docs/aoa/amps.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/aoa/connections.rst` & `Glances-3.4.0.2/docs/aoa/connections.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/aoa/containers.rst` & `Glances-3.4.0.2/docs/aoa/containers.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/aoa/cpu.rst` & `Glances-3.4.0.2/docs/aoa/cpu.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/aoa/diskio.rst` & `Glances-3.4.0.2/docs/aoa/diskio.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/aoa/events.rst` & `Glances-3.4.0.2/docs/aoa/events.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/aoa/folders.rst` & `Glances-3.4.0.2/docs/aoa/folders.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/aoa/fs.rst` & `Glances-3.4.0.2/docs/aoa/fs.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/aoa/gpu.rst` & `Glances-3.4.0.2/docs/aoa/gpu.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/aoa/hddtemp.rst` & `Glances-3.4.0.2/docs/aoa/hddtemp.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/aoa/header.rst` & `Glances-3.4.0.2/docs/aoa/header.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/aoa/index.rst` & `Glances-3.4.0.2/docs/aoa/index.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/aoa/irq.rst` & `Glances-3.4.0.2/docs/aoa/irq.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/aoa/load.rst` & `Glances-3.4.0.2/docs/aoa/load.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/aoa/memory.rst` & `Glances-3.4.0.2/docs/aoa/memory.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/aoa/network.rst` & `Glances-3.4.0.2/docs/aoa/network.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/aoa/ports.rst` & `Glances-3.4.0.2/docs/aoa/ports.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/aoa/ps.rst` & `Glances-3.4.0.2/docs/aoa/ps.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/aoa/quicklook.rst` & `Glances-3.4.0.2/docs/aoa/quicklook.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/aoa/sensors.rst` & `Glances-3.4.0.2/docs/aoa/sensors.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/aoa/smart.rst` & `Glances-3.4.0.2/docs/aoa/smart.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/aoa/wifi.rst` & `Glances-3.4.0.2/docs/aoa/wifi.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/api.rst` & `Glances-3.4.0.2/docs/api.rst`

 * *Files 12% similar despite different names*

```diff
@@ -70,24 +70,24 @@
       "countmax": None,
       "countmin": 1.0,
       "key": "name",
       "name": "Dropbox",
       "refresh": 3.0,
       "regex": True,
       "result": None,
-      "timer": 1.0500612258911133},
+      "timer": 1.053581953048706},
      {"count": 0,
       "countmax": 20.0,
       "countmin": None,
       "key": "name",
       "name": "Python",
       "refresh": 3.0,
       "regex": True,
       "result": None,
-      "timer": 1.0497639179229736}]
+      "timer": 1.0533969402313232}]
 
 Get a specific field::
 
     # curl http://localhost:61208/api/3/amps/name
     {"name": ["Dropbox", "Python", "Conntrack", "Nginx", "Systemd", "SystemV"]}
 
 Get a specific item when field matchs the given value::
@@ -97,15 +97,15 @@
                   "countmax": None,
                   "countmin": 1.0,
                   "key": "name",
                   "name": "Dropbox",
                   "refresh": 3.0,
                   "regex": True,
                   "result": None,
-                  "timer": 1.0500612258911133}]}
+                  "timer": 1.053581953048706}]}
 
 GET connections
 ---------------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/connections
@@ -124,56 +124,56 @@
     # curl http://localhost:61208/api/3/containers
     {"containers": [{"Command": ["top"],
                      "Created": "2023-05-08T15:29:34.918692365+02:00",
                      "Id": "4b7f732d43e4bc5d92fe5298cba025b550e6a608754c1c38f9a90aaecd46b8f9",
                      "Image": "["docker.io/library/ubuntu:latest"]",
                      "Status": "running",
                      "Uptime": "1 weeks",
-                     "cpu": {"total": 9.174878746049114e-07},
-                     "cpu_percent": 9.174878746049114e-07,
+                     "cpu": {"total": 1.2768348293282041e-06},
+                     "cpu_percent": 1.2768348293282041e-06,
                      "engine": "podman",
                      "io": {"ior": 0.0, "iow": 0.0, "time_since_update": 1},
                      "io_r": 0.0,
                      "io_w": 0.0,
                      "key": "name",
-                     "memory": {"limit": 7836184576.0, "usage": 1548288.0},
-                     "memory_usage": 1548288.0,
+                     "memory": {"limit": 7836184576.0, "usage": 1282048.0},
+                     "memory_usage": 1282048.0,
                      "name": "frosty_bouman",
                      "network": {"rx": 0.0, "time_since_update": 1, "tx": 0.0},
                      "network_rx": 0.0,
                      "network_tx": 0.0,
                      "pod_id": "8d0f1c783def",
                      "pod_name": "frosty_bouman"},
                     {"Command": [],
                      "Created": "2022-10-22T14:23:03.120912374+02:00",
                      "Id": "9491515251edcd5bb5dc17205d7ee573c0be96fe0b08b0a12a7e2cea874565ea",
                      "Image": "["k8s.gcr.io/pause:3.5"]",
                      "Status": "running",
                      "Uptime": "1 weeks",
-                     "cpu": {"total": 2.644991475256057e-10},
-                     "cpu_percent": 2.644991475256057e-10,
+                     "cpu": {"total": 2.6911269370551856e-10},
+                     "cpu_percent": 2.6911269370551856e-10,
                      "engine": "podman",
                      "io": {"ior": 0.0, "iow": 0.0, "time_since_update": 1},
                      "io_r": 0.0,
                      "io_w": 0.0,
                      "key": "name",
-                     "memory": {"limit": 7836184576.0, "usage": 434176.0},
-                     "memory_usage": 434176.0,
+                     "memory": {"limit": 7836184576.0, "usage": 208896.0},
+                     "memory_usage": 208896.0,
                      "name": "8d0f1c783def-infra",
                      "network": {"rx": 0.0, "time_since_update": 1, "tx": 0.0},
                      "network_rx": 0.0,
                      "network_tx": 0.0,
                      "pod_id": "8d0f1c783def",
                      "pod_name": "8d0f1c783def-infra"},
                     {"Command": ["/portainer"],
                      "Created": "2022-10-29T14:59:10.266701439Z",
                      "Id": "3abd51c615968482d9ccff5afc629f267f6dda113ed68b75b432615fae3b49fb",
                      "Image": ["portainer/portainer-ce:2.9.3"],
                      "Status": "running",
-                     "Uptime": "4 days",
+                     "Uptime": "5 days",
                      "cpu": {"total": 0.0},
                      "cpu_percent": 0.0,
                      "engine": "docker",
                      "io": {},
                      "io_r": None,
                      "io_w": None,
                      "key": "name",
@@ -210,27 +210,27 @@
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/cpu
     {"cpucore": 4,
      "ctx_switches": 0,
      "guest": 0.0,
      "guest_nice": 0.0,
-     "idle": 66.1,
+     "idle": 55.9,
      "interrupts": 0,
-     "iowait": 0.2,
+     "iowait": 0.0,
      "irq": 0.0,
      "nice": 0.0,
      "soft_interrupts": 0,
      "softirq": 0.0,
      "steal": 0.0,
      "syscalls": 0,
      "system": 6.6,
      "time_since_update": 1,
-     "total": 35.5,
-     "user": 27.2}
+     "total": 42.1,
+     "user": 37.5}
 
 Fields descriptions:
 
 * **total**: Sum of all CPU percentages (except idle) (unit is *percent*)
 * **system**: percent time spent in kernel space. System CPU time is the time spent running code in the Operating System kernel (unit is *percent*)
 * **user**: CPU percent time spent in user space. User CPU time is the time spent on the processor running your program's code (or code in libraries) (unit is *percent*)
 * **iowait**: *(Linux)*: percent time spent by the CPU waiting for I/O operations to complete (unit is *percent*)
@@ -245,15 +245,15 @@
 * **syscalls**: number of system calls per second. Always 0 on Linux OS (unit is *number*)
 * **cpucore**: Total number of CPU core (unit is *number*)
 * **time_since_update**: Number of seconds since last update (unit is *seconds*)
 
 Get a specific field::
 
     # curl http://localhost:61208/api/3/cpu/total
-    {"total": 35.5}
+    {"total": 42.1}
 
 GET diskio
 ----------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/diskio
@@ -291,21 +291,21 @@
 GET fs
 ------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/fs
     [{"device_name": "/dev/mapper/ubuntu--gnome--vg-root",
-      "free": 8354877440,
+      "free": 3450388480,
       "fs_type": "ext4",
       "key": "mnt_point",
       "mnt_point": "/",
-      "percent": 96.4,
+      "percent": 98.5,
       "size": 243334156288,
-      "used": 222591823872},
+      "used": 227496312832},
      {"device_name": "zsfpool",
       "free": 41811968,
       "fs_type": "zfs",
       "key": "mnt_point",
       "mnt_point": "/zsfpool",
       "percent": 0.3,
       "size": 41943040,
@@ -316,79 +316,76 @@
     # curl http://localhost:61208/api/3/fs/mnt_point
     {"mnt_point": ["/", "/zsfpool", "/var/snap/firefox/common/host-hunspell"]}
 
 Get a specific item when field matchs the given value::
 
     # curl http://localhost:61208/api/3/fs/mnt_point//
     {"/": [{"device_name": "/dev/mapper/ubuntu--gnome--vg-root",
-            "free": 8354877440,
+            "free": 3450388480,
             "fs_type": "ext4",
             "key": "mnt_point",
             "mnt_point": "/",
-            "percent": 96.4,
+            "percent": 98.5,
             "size": 243334156288,
-            "used": 222591823872}]}
+            "used": 227496312832}]}
 
 GET ip
 ------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/ip
-    {"address": "192.168.1.14",
-     "gateway": "192.168.1.1",
+    {"address": "192.168.0.32",
+     "gateway": "192.168.0.254",
      "mask": "255.255.255.0",
      "mask_cidr": 24,
-     "public_address": "92.151.148.66",
+     "public_address": "91.166.228.228",
      "public_info_human": ""}
 
 Get a specific field::
 
     # curl http://localhost:61208/api/3/ip/gateway
-    {"gateway": "192.168.1.1"}
+    {"gateway": "192.168.0.254"}
 
 GET load
 --------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/load
-    {"cpucore": 4,
-     "min1": 2.630859375,
-     "min15": 1.4560546875,
-     "min5": 1.42822265625}
+    {"cpucore": 4, "min1": 1.8046875, "min15": 1.51025390625, "min5": 1.6845703125}
 
 Fields descriptions:
 
 * **min1**: Average sum of the number of processes waiting in the run-queue plus the number currently executing over 1 minute (unit is *float*)
 * **min5**: Average sum of the number of processes waiting in the run-queue plus the number currently executing over 5 minutes (unit is *float*)
 * **min15**: Average sum of the number of processes waiting in the run-queue plus the number currently executing over 15 minutes (unit is *float*)
 * **cpucore**: Total number of CPU core (unit is *number*)
 
 Get a specific field::
 
     # curl http://localhost:61208/api/3/load/min1
-    {"min1": 2.630859375}
+    {"min1": 1.8046875}
 
 GET mem
 -------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/mem
-    {"active": 3263430656,
-     "available": 2511720448,
-     "buffers": 743632896,
-     "cached": 2523037696,
-     "free": 2511720448,
-     "inactive": 3192811520,
-     "percent": 67.9,
-     "shared": 627544064,
+    {"active": 2122240000,
+     "available": 2791682048,
+     "buffers": 85512192,
+     "cached": 2199904256,
+     "free": 2791682048,
+     "inactive": 3360813056,
+     "percent": 64.4,
+     "shared": 575238144,
      "total": 7836184576,
-     "used": 5324464128}
+     "used": 5044502528}
 
 Fields descriptions:
 
 * **total**: Total physical memory available (unit is *bytes*)
 * **available**: The actual amount of available memory that can be given instantly to processes that request more memory in bytes; this is calculated by summing different memory values depending on the platform (e.g. free + buffers + cached on Linux) and it is supposed to be used to monitor actual memory usage in a cross platform fashion (unit is *bytes*)
 * **percent**: The percentage usage calculated as (total - available) / total * 100 (unit is *percent*)
 * **used**: Memory used, calculated differently depending on the platform and designed for informational purposes only (unit is *bytes*)
@@ -407,21 +404,21 @@
 
 GET memswap
 -----------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/memswap
-    {"free": 5526786048,
-     "percent": 31.6,
-     "sin": 2906378240,
-     "sout": 5210710016,
+    {"free": 4049227776,
+     "percent": 49.9,
+     "sin": 4989526016,
+     "sout": 8589299712,
      "time_since_update": 1,
      "total": 8082419712,
-     "used": 2555633664}
+     "used": 4033191936}
 
 Fields descriptions:
 
 * **total**: Total swap memory (unit is *bytes*)
 * **used**: Used swap memory (unit is *bytes*)
 * **free**: Free swap memory (unit is *bytes*)
 * **percent**: Used swap memory in percentage (unit is *percent*)
@@ -437,37 +434,37 @@
 GET network
 -----------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/network
     [{"alias": None,
-      "cumulative_cx": 151835804,
-      "cumulative_rx": 75917902,
-      "cumulative_tx": 75917902,
-      "cx": 6340,
+      "cumulative_cx": 194497112,
+      "cumulative_rx": 97248556,
+      "cumulative_tx": 97248556,
+      "cx": 3794,
       "interface_name": "lo",
       "is_up": True,
       "key": "interface_name",
-      "rx": 3170,
+      "rx": 1897,
       "speed": 0,
       "time_since_update": 1,
-      "tx": 3170},
+      "tx": 1897},
      {"alias": None,
-      "cumulative_cx": 8971420885,
-      "cumulative_rx": 8692531338,
-      "cumulative_tx": 278889547,
-      "cx": 32318,
+      "cumulative_cx": 13127976036,
+      "cumulative_rx": 12705380323,
+      "cumulative_tx": 422595713,
+      "cx": 39560,
       "interface_name": "wlp2s0",
       "is_up": True,
       "key": "interface_name",
-      "rx": 20465,
+      "rx": 26691,
       "speed": 0,
       "time_since_update": 1,
-      "tx": 11853}]
+      "tx": 12869}]
 
 Fields descriptions:
 
 * **interface_name**: Interface name (unit is *string*)
 * **alias**: Interface alias name (optional) (unit is *string*)
 * **rx**: The received/input rate (in bit per second) (unit is *bps*)
 * **tx**: The sent/output rate (in bit per second) (unit is *bps*)
@@ -483,391 +480,401 @@
 
     # curl http://localhost:61208/api/3/network/interface_name
     {"interface_name": ["lo",
                         "wlp2s0",
                         "docker0",
                         "br_grafana",
                         "mpqemubr0",
-                        "vethcddb0e6"]}
+                        "vethcddb0e6",
+                        "vboxnet0"]}
 
 Get a specific item when field matchs the given value::
 
     # curl http://localhost:61208/api/3/network/interface_name/lo
     {"lo": [{"alias": None,
-             "cumulative_cx": 151835804,
-             "cumulative_rx": 75917902,
-             "cumulative_tx": 75917902,
-             "cx": 6340,
+             "cumulative_cx": 194497112,
+             "cumulative_rx": 97248556,
+             "cumulative_tx": 97248556,
+             "cx": 3794,
              "interface_name": "lo",
              "is_up": True,
              "key": "interface_name",
-             "rx": 3170,
+             "rx": 1897,
              "speed": 0,
              "time_since_update": 1,
-             "tx": 3170}]}
+             "tx": 1897}]}
 
 GET now
 -------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/now
-    "2023-05-17 11:24:06 CEST"
+    "2023-05-18 17:40:44 CEST"
 
 GET percpu
 ----------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/percpu
     [{"cpu_number": 0,
       "guest": 0.0,
       "guest_nice": 0.0,
-      "idle": 20.2,
+      "idle": 71.1,
       "iowait": 0.0,
       "irq": 0.0,
       "key": "cpu_number",
       "nice": 0.0,
       "softirq": 0.0,
       "steal": 0.0,
-      "system": 6.7,
-      "total": 79.8,
-      "user": 73.1},
+      "system": 6.2,
+      "total": 28.9,
+      "user": 22.7},
      {"cpu_number": 1,
       "guest": 0.0,
       "guest_nice": 0.0,
-      "idle": 70.6,
+      "idle": 72.1,
       "iowait": 0.0,
       "irq": 0.0,
       "key": "cpu_number",
       "nice": 0.0,
       "softirq": 0.0,
       "steal": 0.0,
-      "system": 6.7,
-      "total": 29.4,
-      "user": 22.7}]
+      "system": 8.5,
+      "total": 27.9,
+      "user": 19.4}]
 
 Get a specific field::
 
     # curl http://localhost:61208/api/3/percpu/cpu_number
     {"cpu_number": [0, 1, 2, 3]}
 
 GET ports
 ---------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/ports
     [{"description": "DefaultGateway",
-      "host": "192.168.1.1",
+      "host": "192.168.0.254",
       "indice": "port_0",
       "port": 0,
       "refresh": 30,
       "rtt_warning": None,
-      "status": 0.005277,
+      "status": 0.004474,
       "timeout": 3}]
 
 Get a specific field::
 
     # curl http://localhost:61208/api/3/ports/host
-    {"host": ["192.168.1.1"]}
+    {"host": ["192.168.0.254"]}
 
 Get a specific item when field matchs the given value::
 
-    # curl http://localhost:61208/api/3/ports/host/192.168.1.1
-    {"192.168.1.1": [{"description": "DefaultGateway",
-                      "host": "192.168.1.1",
-                      "indice": "port_0",
-                      "port": 0,
-                      "refresh": 30,
-                      "rtt_warning": None,
-                      "status": 0.005277,
-                      "timeout": 3}]}
+    # curl http://localhost:61208/api/3/ports/host/192.168.0.254
+    {"192.168.0.254": [{"description": "DefaultGateway",
+                        "host": "192.168.0.254",
+                        "indice": "port_0",
+                        "port": 0,
+                        "refresh": 30,
+                        "rtt_warning": None,
+                        "status": 0.004474,
+                        "timeout": 3}]}
 
 GET processcount
 ----------------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/processcount
-    {"pid_max": 0, "running": 1, "sleeping": 316, "thread": 1601, "total": 384}
+    {"pid_max": 0, "running": 2, "sleeping": 326, "thread": 1750, "total": 392}
 
 Get a specific field::
 
     # curl http://localhost:61208/api/3/processcount/total
-    {"total": 384}
+    {"total": 392}
 
 GET processlist
 ---------------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/processlist
     [{"cmdline": ["/snap/firefox/2605/usr/lib/firefox/firefox"],
       "cpu_percent": 0.0,
-      "cpu_times": [6652.64, 2012.85, 5052.81, 704.23, 0.0],
+      "cpu_times": [9681.14, 2938.04, 7162.98, 1045.12, 0.0],
       "gids": [1000, 1000, 1000],
-      "io_counters": [4205573120, 6936297472, 0, 0, 0],
+      "io_counters": [5914563584, 9486209024, 0, 0, 0],
       "key": "pid",
-      "memory_info": [507658240, 22263525376, 129363968, 618496, 0, 1405198336, 0],
-      "memory_percent": 6.478385432048301,
+      "memory_info": [409571328, 21839839232, 109895680, 618496, 0, 1071738880, 0],
+      "memory_percent": 5.226667698134628,
       "name": "firefox",
       "nice": 0,
-      "num_threads": 168,
+      "num_threads": 174,
       "pid": 10541,
       "status": "S",
       "time_since_update": 1,
       "username": "nicolargo"},
      {"cmdline": ["/snap/firefox/2605/usr/lib/firefox/firefox",
                   "-contentproc",
                   "-childID",
-                  "6",
+                  "2",
                   "-isForBrowser",
                   "-prefsLen",
-                  "38436",
+                  "27003",
                   "-prefMapSize",
                   "241898",
                   "-jsInitLen",
                   "240056",
                   "-parentBuildID",
                   "20230424185118",
                   "-appDir",
                   "/snap/firefox/2605/usr/lib/firefox/browser",
-                  "{c94b5dea-52c6-4c75-a314-5de48bda9cdc}",
+                  "{dbcbe484-8536-44ea-aa85-ba683b538aa8}",
                   "10541",
                   "true",
                   "tab"],
       "cpu_percent": 0.0,
-      "cpu_times": [1100.17, 125.28, 0.0, 0.0, 0.0],
+      "cpu_times": [1257.75, 117.29, 0.0, 0.0, 0.0],
       "gids": [1000, 1000, 1000],
-      "io_counters": [209806336, 0, 0, 0, 0],
+      "io_counters": [301149184, 0, 0, 0, 0],
       "key": "pid",
-      "memory_info": [406437888, 3516469248, 78082048, 618496, 0, 918466560, 0],
-      "memory_percent": 5.186680891167411,
-      "name": "WebExtensions",
+      "memory_info": [371560448, 3219562496, 60375040, 618496, 0, 553922560, 0],
+      "memory_percent": 4.741598980937532,
+      "name": "Isolated Web Co",
       "nice": 0,
-      "num_threads": 20,
-      "pid": 11043,
+      "num_threads": 22,
+      "pid": 10770,
       "status": "S",
       "time_since_update": 1,
       "username": "nicolargo"}]
 
 Get a specific field::
 
     # curl http://localhost:61208/api/3/processlist/pid
     {"pid": [10541,
-             11043,
-             59195,
              10770,
-             10778,
+             59195,
              60503,
-             55857,
+             11043,
+             59454,
              3927,
+             10778,
              10774,
-             59454,
-             250191,
-             181461,
-             10790,
-             195248,
+             55857,
+             296364,
+             277461,
+             293836,
+             261989,
+             307573,
+             297410,
+             11646,
              4288,
+             59069,
+             314895,
+             10790,
+             315078,
+             315445,
+             314927,
+             294622,
              10733,
-             60104,
-             11646,
+             306969,
+             59523,
+             313257,
              421,
-             165661,
-             59069,
-             257253,
-             257768,
-             257484,
-             257543,
              59161,
-             59523,
+             315564,
+             315575,
+             60104,
              60232,
-             2398,
-             11380,
-             257817,
-             4339,
-             257829,
              4385,
-             3810,
+             195248,
              4243,
-             11381,
+             3810,
+             315023,
+             59182,
+             2398,
+             281405,
+             307822,
+             165661,
              59525,
-             59663,
-             10710,
-             195141,
-             250777,
-             60106,
-             143262,
-             257721,
-             60489,
-             143263,
-             60134,
-             1618,
+             56140,
              1771,
-             59182,
-             2636,
-             250733,
              4023,
              60191,
-             3730,
-             250835,
+             313283,
+             1618,
              60192,
-             4666,
-             1584,
-             56140,
+             2636,
+             3730,
+             4339,
+             11380,
              1,
-             17997,
-             227509,
+             60489,
+             1584,
+             3115,
+             299963,
+             195141,
+             4090,
+             4075,
+             4000,
+             313650,
+             4666,
+             59663,
+             3719,
              4179,
+             17997,
+             1630,
+             1605,
+             4086,
              4091,
-             4000,
-             250871,
-             4090,
+             60106,
+             4169,
+             4046,
              4403,
-             4075,
-             3991,
-             3901,
+             3908,
+             143263,
              4308,
-             1605,
-             3115,
-             2554,
+             60134,
+             143262,
+             74953,
+             4126,
              1794,
-             2168,
-             1630,
-             1727,
+             4009,
+             3901,
+             3991,
              36919,
-             4046,
-             1631,
-             3719,
+             3956,
+             4442,
+             11381,
+             4080,
+             1583,
+             3743,
+             4302,
+             2116,
+             3710,
+             4127,
+             4105,
              59126,
+             289122,
              20173,
-             3710,
+             2168,
              2607,
-             4009,
-             1598,
-             2341,
-             3956,
-             4105,
-             74953,
-             59127,
-             3908,
-             1764,
+             3745,
+             10710,
+             56119,
+             4196,
+             4005,
              1379,
-             256714,
-             4086,
              4244,
+             289100,
+             4079,
+             4099,
+             227509,
              1818,
-             1583,
-             4169,
-             3745,
-             4127,
-             14243,
-             4442,
-             4126,
-             14266,
-             1627,
-             2116,
-             4097,
              4078,
-             3989,
-             1628,
+             2341,
+             14266,
+             59127,
              1566,
-             4316,
+             2554,
              4145,
-             4080,
-             3498,
-             4119,
+             1591,
+             16182,
+             14243,
+             1624,
+             1628,
              3925,
+             1764,
+             3947,
+             1612,
+             3939,
+             4119,
+             4316,
+             1598,
+             3819,
+             4074,
+             3952,
+             4098,
+             4107,
              3748,
-             2604,
              3970,
-             3939,
-             1591,
              4033,
-             4005,
-             4099,
+             313277,
              4062,
-             3952,
-             1612,
-             1624,
-             4196,
+             3989,
+             4157,
              3825,
-             3947,
-             1606,
-             4107,
-             3975,
-             4098,
-             4302,
-             1579,
-             2605,
-             4074,
-             3743,
              10848,
-             3819,
-             4157,
-             4079,
+             3975,
              3753,
-             1380,
-             1825,
-             3499,
-             1616,
-             3727,
-             1575,
-             3728,
+             1606,
              461,
-             3888,
+             1631,
              3934,
+             1579,
+             4097,
+             1825,
+             1627,
+             1575,
+             315523,
              1593,
-             56119,
-             1377,
-             1964,
-             257754,
-             1582,
+             1616,
              12480,
-             12489,
+             261973,
+             3888,
              59145,
+             1377,
+             12489,
+             3727,
+             1380,
+             1582,
              18045,
+             1964,
              4332,
-             3118,
+             3728,
              1634,
-             1390,
-             1391,
+             3118,
              2361,
-             3573,
-             16182,
-             20400,
-             1725,
-             1726,
+             1391,
+             1727,
+             2604,
+             1390,
+             2605,
              12483,
              1567,
              20396,
              20180,
-             12492,
+             315563,
+             4072,
+             2358,
+             20400,
              59130,
-             257816,
-             4593,
-             56100,
-             56106,
+             3498,
+             12492,
+             314768,
              56087,
-             3720,
-             3503,
-             56081,
-             4072,
+             56106,
+             1725,
+             1726,
              3794,
-             2358,
-             247115,
-             2382,
+             3499,
+             56100,
+             56081,
+             3503,
+             3720,
              2345,
-             1637,
+             4593,
+             2382,
              2360,
+             20185,
+             1637,
              1392,
              1577,
-             20185,
-             12486,
              2,
              3,
              4,
              5,
              6,
              8,
              10,
@@ -1003,66 +1010,65 @@
              2492,
              2493,
              2506,
              2508,
              2510,
              2515,
              2525,
+             3573,
              3988,
-             193069,
-             193070,
-             193072,
-             249139,
-             249929,
-             250365,
-             250457,
-             250459,
-             250462,
-             250467,
-             250473,
-             250474,
-             250475,
-             250476,
-             250477,
-             250479,
-             250529,
-             255880,
-             256024,
-             256316,
-             256366,
-             256541,
-             256899,
-             256900,
-             256944,
-             256946,
-             257104,
-             257206,
-             257329,
-             257419]}
+             12486,
+             288792,
+             288793,
+             288795,
+             304692,
+             306042,
+             307710,
+             307711,
+             307713,
+             307714,
+             307715,
+             307764,
+             309333,
+             310964,
+             311618,
+             311630,
+             313395,
+             313404,
+             313720,
+             313725,
+             313896,
+             314273,
+             314367,
+             314371,
+             314524,
+             315132,
+             315249,
+             315374]}
 
 Get a specific item when field matchs the given value::
 
     # curl http://localhost:61208/api/3/processlist/pid/10541
     {"10541": [{"cmdline": ["/snap/firefox/2605/usr/lib/firefox/firefox"],
                 "cpu_percent": 0.0,
-                "cpu_times": [6652.64, 2012.85, 5052.81, 704.23, 0.0],
+                "cpu_times": [9681.14, 2938.04, 7162.98, 1045.12, 0.0],
                 "gids": [1000, 1000, 1000],
-                "io_counters": [4205573120, 6936297472, 0, 0, 0],
+                "io_counters": [5914563584, 9486209024, 0, 0, 0],
                 "key": "pid",
-                "memory_info": [507658240,
-                                22263525376,
-                                129363968,
+                "memory_info": [409571328,
+                                21839839232,
+                                109895680,
                                 618496,
                                 0,
-                                1405198336,
+                                1071738880,
                                 0],
-                "memory_percent": 6.478385432048301,
+                "memory_percent": 5.226667698134628,
                 "name": "firefox",
                 "nice": 0,
-                "num_threads": 168,
+                "num_threads": 174,
                 "pid": 10541,
                 "status": "S",
                 "time_since_update": 1,
                 "username": "nicolargo"}]}
 
 GET psutilversion
 -----------------
@@ -1074,77 +1080,77 @@
 
 GET quicklook
 -------------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/quicklook
-    {"cpu": 35.5,
+    {"cpu": 42.1,
      "cpu_hz": 2025000000.0,
-     "cpu_hz_current": 1498956999.9999998,
+     "cpu_hz_current": 1264730000.0,
      "cpu_name": "Intel(R) Core(TM) i7-4500U CPU @ 1.80GHz",
-     "mem": 67.9,
+     "mem": 64.4,
      "percpu": [{"cpu_number": 0,
                  "guest": 0.0,
                  "guest_nice": 0.0,
-                 "idle": 20.2,
+                 "idle": 71.1,
                  "iowait": 0.0,
                  "irq": 0.0,
                  "key": "cpu_number",
                  "nice": 0.0,
                  "softirq": 0.0,
                  "steal": 0.0,
-                 "system": 6.7,
-                 "total": 79.8,
-                 "user": 73.1},
+                 "system": 6.2,
+                 "total": 28.9,
+                 "user": 22.7},
                 {"cpu_number": 1,
                  "guest": 0.0,
                  "guest_nice": 0.0,
-                 "idle": 70.6,
+                 "idle": 72.1,
                  "iowait": 0.0,
                  "irq": 0.0,
                  "key": "cpu_number",
                  "nice": 0.0,
                  "softirq": 0.0,
                  "steal": 0.0,
-                 "system": 6.7,
-                 "total": 29.4,
-                 "user": 22.7},
+                 "system": 8.5,
+                 "total": 27.9,
+                 "user": 19.4},
                 {"cpu_number": 2,
                  "guest": 0.0,
                  "guest_nice": 0.0,
-                 "idle": 85.7,
+                 "idle": 27.9,
                  "iowait": 0.0,
                  "irq": 0.0,
                  "key": "cpu_number",
                  "nice": 0.0,
                  "softirq": 0.0,
                  "steal": 0.0,
-                 "system": 3.4,
-                 "total": 14.3,
-                 "user": 10.9},
+                 "system": 3.3,
+                 "total": 72.1,
+                 "user": 68.9},
                 {"cpu_number": 3,
                  "guest": 0.0,
                  "guest_nice": 0.0,
-                 "idle": 82.0,
+                 "idle": 58.9,
                  "iowait": 0.0,
                  "irq": 0.0,
                  "key": "cpu_number",
                  "nice": 0.0,
                  "softirq": 0.0,
                  "steal": 0.0,
-                 "system": 6.6,
-                 "total": 18.0,
-                 "user": 11.5}],
-     "swap": 31.6}
+                 "system": 4.8,
+                 "total": 41.1,
+                 "user": 36.3}],
+     "swap": 49.9}
 
 Get a specific field::
 
     # curl http://localhost:61208/api/3/quicklook/cpu
-    {"cpu": 35.5}
+    {"cpu": 42.1}
 
 GET sensors
 -----------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/sensors
@@ -1207,15 +1213,15 @@
 
 GET uptime
 ----------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/uptime
-    "8 days, 22:22:23"
+    "10 days, 4:38:59"
 
 GET all stats
 -------------
 
 Get all Glances stats::
 
     # curl http://localhost:61208/api/3/all
@@ -1223,41 +1229,41 @@
 
 GET stats history
 -----------------
 
 History of a plugin::
 
     # curl http://localhost:61208/api/3/cpu/history
-    {"system": [["2023-05-17T11:24:07.350522", 6.6],
-                ["2023-05-17T11:24:08.472521", 6.6],
-                ["2023-05-17T11:24:09.656447", 2.5]],
-     "user": [["2023-05-17T11:24:07.350513", 27.2],
-              ["2023-05-17T11:24:08.472515", 27.2],
-              ["2023-05-17T11:24:09.656439", 10.8]]}
+    {"system": [["2023-05-18T17:40:45.904909", 6.6],
+                ["2023-05-18T17:40:47.072443", 6.6],
+                ["2023-05-18T17:40:48.253286", 3.3]],
+     "user": [["2023-05-18T17:40:45.904887", 37.5],
+              ["2023-05-18T17:40:47.072437", 37.5],
+              ["2023-05-18T17:40:48.253279", 18.3]]}
 
 Limit history to last 2 values::
 
     # curl http://localhost:61208/api/3/cpu/history/2
-    {"system": [["2023-05-17T11:24:08.472521", 6.6],
-                ["2023-05-17T11:24:09.656447", 2.5]],
-     "user": [["2023-05-17T11:24:08.472515", 27.2],
-              ["2023-05-17T11:24:09.656439", 10.8]]}
+    {"system": [["2023-05-18T17:40:47.072443", 6.6],
+                ["2023-05-18T17:40:48.253286", 3.3]],
+     "user": [["2023-05-18T17:40:47.072437", 37.5],
+              ["2023-05-18T17:40:48.253279", 18.3]]}
 
 History for a specific field::
 
     # curl http://localhost:61208/api/3/cpu/system/history
-    {"system": [["2023-05-17T11:24:07.350522", 6.6],
-                ["2023-05-17T11:24:08.472521", 6.6],
-                ["2023-05-17T11:24:09.656447", 2.5]]}
+    {"system": [["2023-05-18T17:40:45.904909", 6.6],
+                ["2023-05-18T17:40:47.072443", 6.6],
+                ["2023-05-18T17:40:48.253286", 3.3]]}
 
 Limit history for a specific field to last 2 values::
 
     # curl http://localhost:61208/api/3/cpu/system/history
-    {"system": [["2023-05-17T11:24:08.472521", 6.6],
-                ["2023-05-17T11:24:09.656447", 2.5]]}
+    {"system": [["2023-05-18T17:40:47.072443", 6.6],
+                ["2023-05-18T17:40:48.253286", 3.3]]}
 
 GET limits (used for thresholds)
 --------------------------------
 
 All limits/thresholds::
 
     # curl http://localhost:61208/api/3/all/limits
```

### Comparing `Glances-3.4.0.1/docs/cmds.rst` & `Glances-3.4.0.2/docs/cmds.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/conf.py` & `Glances-3.4.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/config.rst` & `Glances-3.4.0.2/docs/config.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/dev/glances-cprofile.png` & `Glances-3.4.0.2/docs/dev/glances-cprofile.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/docker.rst` & `Glances-3.4.0.2/docs/docker.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/glances.rst` & `Glances-3.4.0.2/docs/glances.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/gw/cassandra.rst` & `Glances-3.4.0.2/docs/gw/cassandra.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/gw/couchdb.rst` & `Glances-3.4.0.2/docs/gw/couchdb.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/gw/csv.rst` & `Glances-3.4.0.2/docs/gw/csv.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/gw/graph.rst` & `Glances-3.4.0.2/docs/gw/graph.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/gw/graphite.rst` & `Glances-3.4.0.2/docs/gw/graphite.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/gw/influxdb.rst` & `Glances-3.4.0.2/docs/gw/influxdb.rst`

 * *Files 10% similar despite different names*

```diff
@@ -92,14 +92,17 @@
     [influxdb2]
     host=localhost
     port=8086
     protocol=http
     org=nicolargo
     bucket=glances
     token=EjFUTWe8U-MIseEAkaVIgVnej_TrnbdvEcRkaB1imstW7gapSqy6_6-8XD-yd51V0zUUpDy-kAdVD1purDLuxA==
+    # Set the interval between two exports (in seconds)
+    # If the interval is set to 0, the Glances refresh time is used (default behavor)
+    #interval=0
     # Prefix will be added for all measurement name
     # Ex: prefix=foo
     #     => foo.cpu
     #     => foo.mem
     # You can also use dynamic values
     #prefix=foo
     # Following tags will be added for all measurements
```

### Comparing `Glances-3.4.0.1/docs/gw/kafka.rst` & `Glances-3.4.0.2/docs/gw/kafka.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/gw/mongodb.rst` & `Glances-3.4.0.2/docs/gw/mongodb.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/gw/mqtt.rst` & `Glances-3.4.0.2/docs/gw/mqtt.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/gw/prometheus.rst` & `Glances-3.4.0.2/docs/gw/prometheus.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/gw/restful.rst` & `Glances-3.4.0.2/docs/gw/restful.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/gw/statsd.rst` & `Glances-3.4.0.2/docs/gw/statsd.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/gw/zeromq.rst` & `Glances-3.4.0.2/docs/gw/zeromq.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/index.rst` & `Glances-3.4.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/install.rst` & `Glances-3.4.0.2/docs/install.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/make.bat` & `Glances-3.4.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/man/glances.1` & `Glances-3.4.0.2/docs/man/glances.1`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "GLANCES" "1" "May 17, 2023" "3.4.0.1" "Glances"
+.TH "GLANCES" "1" "May 18, 2023" "3.4.0.2" "Glances"
 .SH NAME
 glances \- An eye on your system
 .SH SYNOPSIS
 .sp
 \fBglances\fP [OPTIONS]
 .SH DESCRIPTION
 .sp
```

### Comparing `Glances-3.4.0.1/docs/objects.inv` & `Glances-3.4.0.2/docs/objects.inv`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/docs/quickstart.rst` & `Glances-3.4.0.2/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/__init__.py` & `Glances-3.4.0.2/glances/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import platform
 import signal
 import sys
 
 # Global name
 # Version should start and end with a numerical char
 # See https://packaging.python.org/specifications/core-metadata/#version
-__version__ = '3.4.0.1'
+__version__ = '3.4.0.2'
 __author__ = 'Nicolas Hennion <nicolas@nicolargo.com>'
 __license__ = 'LGPLv3'
 
 # Import psutil
 try:
     from psutil import __version__ as psutil_version
 except ImportError:
@@ -152,16 +152,21 @@
 
 def main():
     """Main entry point for Glances.
 
     Select the mode (standalone, client or server)
     Run it...
     """
+    # SIGHUP not available on Windows (see issue #2408)
+    if sys.platform.startswith('win'):
+        signal_list = (signal.SIGTERM, signal.SIGINT)
+    else:
+        signal_list = (signal.SIGTERM, signal.SIGINT, signal.SIGHUP)
     # Catch the kill signal
-    for sig in (signal.SIGTERM, signal.SIGINT, signal.SIGHUP):
+    for sig in signal_list:
         signal.signal(sig, __signal_handler)
 
     # Log Glances and psutil version
     logger.info('Start Glances {}'.format(__version__))
     logger.info(
         '{} {} ({}) and psutil {} detected'.format(
             platform.python_implementation(), platform.python_version(), sys.executable, psutil_version
```

### Comparing `Glances-3.4.0.1/glances/actions.py` & `Glances-3.4.0.2/glances/actions.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/amps/glances_amp.py` & `Glances-3.4.0.2/glances/amps/glances_amp.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/amps/glances_default.py` & `Glances-3.4.0.2/glances/amps/glances_default.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/amps/glances_nginx.py` & `Glances-3.4.0.2/glances/amps/glances_nginx.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/amps/glances_systemd.py` & `Glances-3.4.0.2/glances/amps/glances_systemd.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/amps/glances_systemv.py` & `Glances-3.4.0.2/glances/amps/glances_systemv.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/amps_list.py` & `Glances-3.4.0.2/glances/amps_list.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/attribute.py` & `Glances-3.4.0.2/glances/attribute.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/autodiscover.py` & `Glances-3.4.0.2/glances/autodiscover.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/client.py` & `Glances-3.4.0.2/glances/client.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/client_browser.py` & `Glances-3.4.0.2/glances/client_browser.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/compat.py` & `Glances-3.4.0.2/glances/compat.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/config.py` & `Glances-3.4.0.2/glances/config.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/cpu_percent.py` & `Glances-3.4.0.2/glances/cpu_percent.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/events.py` & `Glances-3.4.0.2/glances/events.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/exports/glances_cassandra.py` & `Glances-3.4.0.2/glances/exports/glances_cassandra.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/exports/glances_couchdb.py` & `Glances-3.4.0.2/glances/exports/glances_couchdb.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/exports/glances_csv.py` & `Glances-3.4.0.2/glances/exports/glances_csv.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/exports/glances_elasticsearch.py` & `Glances-3.4.0.2/glances/exports/glances_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/exports/glances_export.py` & `Glances-3.4.0.2/glances/exports/glances_export.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/exports/glances_graph.py` & `Glances-3.4.0.2/glances/exports/glances_graph.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/exports/glances_graphite.py` & `Glances-3.4.0.2/glances/exports/glances_graphite.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/exports/glances_influxdb.py` & `Glances-3.4.0.2/glances/exports/glances_influxdb.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/exports/glances_influxdb2.py` & `Glances-3.4.0.2/glances/exports/glances_influxdb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,31 +31,32 @@
         self.token = None
 
         # Optional configuration keys
         self.protocol = 'http'
         self.prefix = None
         self.tags = None
         self.hostname = None
-        self.interval = 0
+        self.interval = None
 
         # Load the InfluxDB configuration file
         self.export_enable = self.load_conf(
             'influxdb2',
             mandatories=['host', 'port', 'user', 'password', 'org', 'bucket', 'token'],
             options=['protocol', 'prefix', 'tags', 'interval'],
         )
         if not self.export_enable:
-            exit('Missing INFLUXDB version 1 config')
+            exit('Missing influxdb2 config')
 
         # Interval between two exports (in seconds)
-        # if export_interval is set to 0, the Glances refresh time is used (default behavor)
+        if self.interval is None:
+            self.interval = 0
         try:
             self.interval = int(self.interval)
         except ValueError:
-            logger.warning("InfluxDB export interval is not an integer, use default value (0)")
+            logger.warning("InfluxDB export interval is not an integer, use default value")
             self.interval = 0
         # and should be set to the Glances refresh time if the value is 0
         self.interval = self.interval if self.interval > 0 else self.args.time
         logger.debug("InfluxDB export interval is set to {} seconds".format(self.interval))
 
         # The hostname is always add as a tag
         self.hostname = node().split('.')[0]
```

### Comparing `Glances-3.4.0.1/glances/exports/glances_json.py` & `Glances-3.4.0.2/glances/exports/glances_json.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/exports/glances_kafka.py` & `Glances-3.4.0.2/glances/exports/glances_kafka.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/exports/glances_mongodb.py` & `Glances-3.4.0.2/glances/exports/glances_mongodb.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/exports/glances_mqtt.py` & `Glances-3.4.0.2/glances/exports/glances_mqtt.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/exports/glances_opentsdb.py` & `Glances-3.4.0.2/glances/exports/glances_opentsdb.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/exports/glances_prometheus.py` & `Glances-3.4.0.2/glances/exports/glances_prometheus.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/exports/glances_rabbitmq.py` & `Glances-3.4.0.2/glances/exports/glances_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/exports/glances_restful.py` & `Glances-3.4.0.2/glances/exports/glances_restful.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/exports/glances_riemann.py` & `Glances-3.4.0.2/glances/exports/glances_riemann.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/exports/glances_statsd.py` & `Glances-3.4.0.2/glances/exports/glances_statsd.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/exports/glances_zeromq.py` & `Glances-3.4.0.2/glances/exports/glances_zeromq.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/filter.py` & `Glances-3.4.0.2/glances/filter.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/folder_list.py` & `Glances-3.4.0.2/glances/folder_list.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/globals.py` & `Glances-3.4.0.2/glances/globals.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/history.py` & `Glances-3.4.0.2/glances/history.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/logger.py` & `Glances-3.4.0.2/glances/logger.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/main.py` & `Glances-3.4.0.2/glances/main.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outdated.py` & `Glances-3.4.0.2/glances/outdated.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/glances_bars.py` & `Glances-3.4.0.2/glances/outputs/glances_bars.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/glances_bottle.py` & `Glances-3.4.0.2/glances/outputs/glances_bottle.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/glances_curses.py` & `Glances-3.4.0.2/glances/outputs/glances_curses.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/glances_curses_browser.py` & `Glances-3.4.0.2/glances/outputs/glances_curses_browser.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/glances_sparklines.py` & `Glances-3.4.0.2/glances/outputs/glances_sparklines.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/glances_stdout.py` & `Glances-3.4.0.2/glances/outputs/glances_stdout.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/glances_stdout_apidoc.py` & `Glances-3.4.0.2/glances/outputs/glances_stdout_apidoc.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/glances_stdout_csv.py` & `Glances-3.4.0.2/glances/outputs/glances_stdout_csv.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/glances_stdout_issue.py` & `Glances-3.4.0.2/glances/outputs/glances_stdout_issue.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/glances_stdout_json.py` & `Glances-3.4.0.2/glances/outputs/glances_stdout_json.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/glances_unicode.py` & `Glances-3.4.0.2/glances/outputs/glances_unicode.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/README.md` & `Glances-3.4.0.2/glances/outputs/static/README.md`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/css/bootstrap.less` & `Glances-3.4.0.2/glances/outputs/static/css/bootstrap.less`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/css/style.scss` & `Glances-3.4.0.2/glances/outputs/static/css/style.scss`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/images/favicon.ico` & `Glances-3.4.0.2/glances/outputs/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/images/glances.png` & `Glances-3.4.0.2/glances/outputs/static/images/glances.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/js/App.vue` & `Glances-3.4.0.2/glances/outputs/static/js/App.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/js/components/help.vue` & `Glances-3.4.0.2/glances/outputs/static/js/components/help.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-alert.vue` & `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-alert.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-amps.vue` & `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-amps.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-cloud.vue` & `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-cloud.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-connections.vue` & `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-connections.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-containers.vue` & `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-containers.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-cpu.vue` & `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-cpu.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-diskio.vue` & `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-diskio.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-folders.vue` & `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-folders.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-fs.vue` & `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-fs.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-gpu.vue` & `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-gpu.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-ip.vue` & `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-ip.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-irq.vue` & `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-irq.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-load.vue` & `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-load.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-mem-more.vue` & `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-mem-more.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-mem.vue` & `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-mem.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-memswap.vue` & `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-memswap.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-network.vue` & `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-network.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-percpu.vue` & `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-percpu.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-ports.vue` & `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-ports.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-process.vue` & `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-process.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-processcount.vue` & `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-processcount.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-processlist.vue` & `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-processlist.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-quicklook.vue` & `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-quicklook.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-raid.vue` & `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-raid.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-sensors.vue` & `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-sensors.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-system.vue` & `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-system.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-wifi.vue` & `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-wifi.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/js/filters.js` & `Glances-3.4.0.2/glances/outputs/static/js/filters.js`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/js/services.js` & `Glances-3.4.0.2/glances/outputs/static/js/services.js`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/package-lock.json` & `Glances-3.4.0.2/glances/outputs/static/package-lock.json`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/package.json` & `Glances-3.4.0.2/glances/outputs/static/package.json`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/public/87708faeed9a66b0fcdb.png` & `Glances-3.4.0.2/glances/outputs/static/public/87708faeed9a66b0fcdb.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/public/favicon.ico` & `Glances-3.4.0.2/glances/outputs/static/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/public/glances.js` & `Glances-3.4.0.2/glances/outputs/static/public/glances.js`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/outputs/static/webpack.config.js` & `Glances-3.4.0.2/glances/outputs/static/webpack.config.js`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/password.py` & `Glances-3.4.0.2/glances/password.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/password_list.py` & `Glances-3.4.0.2/glances/password_list.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/plugins/containers/glances_docker.py` & `Glances-3.4.0.2/glances/plugins/containers/glances_docker.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/plugins/containers/glances_podman.py` & `Glances-3.4.0.2/glances/plugins/containers/glances_podman.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/plugins/containers/stats_streamer.py` & `Glances-3.4.0.2/glances/plugins/containers/stats_streamer.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/plugins/glances_alert.py` & `Glances-3.4.0.2/glances/plugins/glances_alert.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/plugins/glances_amps.py` & `Glances-3.4.0.2/glances/plugins/glances_amps.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/plugins/glances_cloud.py` & `Glances-3.4.0.2/glances/plugins/glances_cloud.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/plugins/glances_connections.py` & `Glances-3.4.0.2/glances/plugins/glances_connections.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/plugins/glances_containers.py` & `Glances-3.4.0.2/glances/plugins/glances_containers.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/plugins/glances_core.py` & `Glances-3.4.0.2/glances/plugins/glances_core.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/plugins/glances_cpu.py` & `Glances-3.4.0.2/glances/plugins/glances_cpu.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/plugins/glances_diskio.py` & `Glances-3.4.0.2/glances/plugins/glances_diskio.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/plugins/glances_folders.py` & `Glances-3.4.0.2/glances/plugins/glances_folders.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/plugins/glances_fs.py` & `Glances-3.4.0.2/glances/plugins/glances_fs.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/plugins/glances_gpu.py` & `Glances-3.4.0.2/glances/plugins/glances_gpu.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/plugins/glances_help.py` & `Glances-3.4.0.2/glances/plugins/glances_help.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/plugins/glances_ip.py` & `Glances-3.4.0.2/glances/plugins/glances_ip.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/plugins/glances_irq.py` & `Glances-3.4.0.2/glances/plugins/glances_irq.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/plugins/glances_load.py` & `Glances-3.4.0.2/glances/plugins/glances_load.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/plugins/glances_mem.py` & `Glances-3.4.0.2/glances/plugins/glances_mem.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/plugins/glances_memswap.py` & `Glances-3.4.0.2/glances/plugins/glances_memswap.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/plugins/glances_network.py` & `Glances-3.4.0.2/glances/plugins/glances_network.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/plugins/glances_now.py` & `Glances-3.4.0.2/glances/plugins/glances_now.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/plugins/glances_percpu.py` & `Glances-3.4.0.2/glances/plugins/glances_percpu.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/plugins/glances_plugin.py` & `Glances-3.4.0.2/glances/plugins/glances_plugin.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/plugins/glances_ports.py` & `Glances-3.4.0.2/glances/plugins/glances_ports.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/plugins/glances_processcount.py` & `Glances-3.4.0.2/glances/plugins/glances_processcount.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/plugins/glances_processlist.py` & `Glances-3.4.0.2/glances/plugins/glances_processlist.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/plugins/glances_psutilversion.py` & `Glances-3.4.0.2/glances/plugins/glances_psutilversion.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/plugins/glances_quicklook.py` & `Glances-3.4.0.2/glances/plugins/glances_quicklook.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/plugins/glances_raid.py` & `Glances-3.4.0.2/glances/plugins/glances_raid.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/plugins/glances_sensors.py` & `Glances-3.4.0.2/glances/plugins/glances_sensors.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/plugins/glances_smart.py` & `Glances-3.4.0.2/glances/plugins/glances_smart.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/plugins/glances_system.py` & `Glances-3.4.0.2/glances/plugins/glances_system.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/plugins/glances_uptime.py` & `Glances-3.4.0.2/glances/plugins/glances_uptime.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/plugins/glances_wifi.py` & `Glances-3.4.0.2/glances/plugins/glances_wifi.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/plugins/sensors/glances_batpercent.py` & `Glances-3.4.0.2/glances/plugins/sensors/glances_batpercent.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/plugins/sensors/glances_hddtemp.py` & `Glances-3.4.0.2/glances/plugins/sensors/glances_hddtemp.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/ports_list.py` & `Glances-3.4.0.2/glances/ports_list.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/processes.py` & `Glances-3.4.0.2/glances/processes.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/programs.py` & `Glances-3.4.0.2/glances/programs.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/secure.py` & `Glances-3.4.0.2/glances/secure.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/server.py` & `Glances-3.4.0.2/glances/server.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/snmp.py` & `Glances-3.4.0.2/glances/snmp.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/standalone.py` & `Glances-3.4.0.2/glances/standalone.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/static_list.py` & `Glances-3.4.0.2/glances/static_list.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/stats.py` & `Glances-3.4.0.2/glances/stats.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/stats_client.py` & `Glances-3.4.0.2/glances/stats_client.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/stats_client_snmp.py` & `Glances-3.4.0.2/glances/stats_client_snmp.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/stats_server.py` & `Glances-3.4.0.2/glances/stats_server.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/thresholds.py` & `Glances-3.4.0.2/glances/thresholds.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/timer.py` & `Glances-3.4.0.2/glances/timer.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/web_list.py` & `Glances-3.4.0.2/glances/web_list.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/glances/webserver.py` & `Glances-3.4.0.2/glances/webserver.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/pyproject.toml` & `Glances-3.4.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.1/setup.py` & `Glances-3.4.0.2/setup.py`

 * *Files identical despite different names*

