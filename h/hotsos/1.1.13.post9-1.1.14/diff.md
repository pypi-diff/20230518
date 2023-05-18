# Comparing `tmp/hotsos-1.1.13.post9.tar.gz` & `tmp/hotsos-1.1.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hotsos-1.1.13.post9.tar", last modified: Thu Mar 30 21:21:57 2023, max compression
+gzip compressed data, was "hotsos-1.1.14.tar", last modified: Thu May 18 11:55:34 2023, max compression
```

## Comparing `hotsos-1.1.13.post9.tar` & `hotsos-1.1.14.tar`

### file list

```diff
@@ -1,349 +1,397 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.227451 hotsos-1.1.13.post9/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-03-30 21:21:57.227451 hotsos-1.1.13.post9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.171447 hotsos-1.1.13.post9/hotsos/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-30 21:21:43.000000 hotsos-1.1.13.post9/hotsos/.repo-info
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13664 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15453 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.175447 hotsos-1.1.13.post9/hotsos/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10720 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.179448 hotsos-1.1.13.post9/hotsos/core/host_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/host_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33958 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/host_helpers/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/host_helpers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/host_helpers/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/host_helpers/filestat.py
--rw-r--r--   0 runner    (1001) docker     (123)    11025 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/host_helpers/network.py
--rw-r--r--   0 runner    (1001) docker     (123)    13238 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/host_helpers/packaging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/host_helpers/ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/host_helpers/sysctl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/host_helpers/systemd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/host_helpers/uptime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.179448 hotsos-1.1.13.post9/hotsos/core/issues/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/issues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/issues/issue_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/issues/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.179448 hotsos-1.1.13.post9/hotsos/core/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.179448 hotsos-1.1.13.post9/hotsos/core/plugins/juju/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/juju/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/juju/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/juju/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.183448 hotsos-1.1.13.post9/hotsos/core/plugins/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/kernel/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/kernel/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.183448 hotsos-1.1.13.post9/hotsos/core/plugins/kernel/kernlog/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/kernel/kernlog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/kernel/kernlog/calltrace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/kernel/kernlog/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/kernel/kernlog/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/kernel/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    12995 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/kernel/net.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/kernel/sysfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/kubernetes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.183448 hotsos-1.1.13.post9/hotsos/core/plugins/lxd/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/lxd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/lxd/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/maas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/mysql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.183448 hotsos-1.1.13.post9/hotsos/core/plugins/openstack/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/openstack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/openstack/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    63864 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/openstack/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/openstack/neutron.py
--rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/openstack/nova.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/openstack/octavia.py
--rw-r--r--   0 runner    (1001) docker     (123)    17627 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/openstack/openstack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.187448 hotsos-1.1.13.post9/hotsos/core/plugins/openvswitch/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/openvswitch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/openvswitch/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/openvswitch/ovn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/openvswitch/ovs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/pacemaker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.187448 hotsos-1.1.13.post9/hotsos/core/plugins/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/rabbitmq/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/rabbitmq/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/sosreport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.187448 hotsos-1.1.13.post9/hotsos/core/plugins/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/storage/bcache.py
--rw-r--r--   0 runner    (1001) docker     (123)    36154 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/storage/ceph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.187448 hotsos-1.1.13.post9/hotsos/core/plugins/system/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/system/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/system/system.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugins/vault.py
--rw-r--r--   0 runner    (1001) docker     (123)    13784 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/plugintools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.187448 hotsos-1.1.13.post9/hotsos/core/ycheck/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/ycheck/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.187448 hotsos-1.1.13.post9/hotsos/core/ycheck/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/ycheck/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/ycheck/engine/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.191449 hotsos-1.1.13.post9/hotsos/core/ycheck/engine/properties/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/ycheck/engine/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/ycheck/engine/properties/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)    22878 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/ycheck/engine/properties/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     9696 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/ycheck/engine/properties/conclusions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/ycheck/engine/properties/input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.191449 hotsos-1.1.13.post9/hotsos/core/ycheck/engine/properties/requires/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/ycheck/engine/properties/requires/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/ycheck/engine/properties/requires/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/ycheck/engine/properties/requires/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.191449 hotsos-1.1.13.post9/hotsos/core/ycheck/engine/properties/requires/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/ycheck/engine/properties/requires/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/ycheck/engine/properties/requires/types/apt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/ycheck/engine/properties/requires/types/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/ycheck/engine/properties/requires/types/path.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/ycheck/engine/properties/requires/types/property.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/ycheck/engine/properties/requires/types/snap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/ycheck/engine/properties/requires/types/systemd.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/ycheck/engine/properties/requires/types/varops.py
--rw-r--r--   0 runner    (1001) docker     (123)    13326 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/ycheck/engine/properties/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/ycheck/engine/properties/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    13783 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/ycheck/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/core/ycheck/scenarios.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.163447 hotsos-1.1.13.post9/hotsos/defs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.163447 hotsos-1.1.13.post9/hotsos/defs/events/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.191449 hotsos-1.1.13.post9/hotsos/defs/events/openstack/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/events/openstack/apache.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/events/openstack/apparmor.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/events/openstack/http-requests.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.195449 hotsos-1.1.13.post9/hotsos/defs/events/openstack/neutron/
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/events/openstack/neutron/agents.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/events/openstack/neutron/ml2-routers.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.195449 hotsos-1.1.13.post9/hotsos/defs/events/openstack/nova/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/events/openstack/nova/external-events.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.195449 hotsos-1.1.13.post9/hotsos/defs/events/openstack/nova/migrations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.195449 hotsos-1.1.13.post9/hotsos/defs/events/openstack/nova/migrations/live-migration/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/events/openstack/nova/migrations/live-migration/dst-pre-live-migration.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/events/openstack/nova/migrations/live-migration/src-migration.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/events/openstack/nova/migrations/live-migration/src-post-live-migration.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/events/openstack/nova/migrations/migrations.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/events/openstack/nova/nova-compute.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/events/openstack/octavia.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.163447 hotsos-1.1.13.post9/hotsos/defs/events/openvswitch/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.195449 hotsos-1.1.13.post9/hotsos/defs/events/openvswitch/ovn/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/events/openvswitch/ovn/errors-and-warnings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/events/openvswitch/ovn/ovn-central.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/events/openvswitch/ovn/ovn-controller.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.195449 hotsos-1.1.13.post9/hotsos/defs/events/openvswitch/ovs/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/events/openvswitch/ovs/bfd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/events/openvswitch/ovs/datapath-checks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/events/openvswitch/ovs/errors-and-warnings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/events/openvswitch/ovs/ovs-vswitchd.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.163447 hotsos-1.1.13.post9/hotsos/defs/events/storage/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.163447 hotsos-1.1.13.post9/hotsos/defs/events/storage/ceph/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.195449 hotsos-1.1.13.post9/hotsos/defs/events/storage/ceph/mon/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/events/storage/ceph/mon/mon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/events/storage/ceph/mon/monlogs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.195449 hotsos-1.1.13.post9/hotsos/defs/events/storage/ceph/osd/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/events/storage/ceph/osd/osd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/events/storage/ceph/osd/osdlogs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.167447 hotsos-1.1.13.post9/hotsos/defs/scenarios/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.199449 hotsos-1.1.13.post9/hotsos/defs/scenarios/juju/
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/juju/charm_unit_checks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/juju/juju.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/juju/jujud_machine_checks.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.199449 hotsos-1.1.13.post9/hotsos/defs/scenarios/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/kernel/amd_iommu_pt.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/kernel/disk_failure.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/kernel/kernlog_calltrace.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/kernel/memory.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.199449 hotsos-1.1.13.post9/hotsos/defs/scenarios/kernel/network/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/kernel/network/misc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/kernel/network/tcp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/kernel/network/udp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/kernel/qla2xxx.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.199449 hotsos-1.1.13.post9/hotsos/defs/scenarios/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/kubernetes/kubernetes.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/kubernetes/system_cpufreq_mode.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.203449 hotsos-1.1.13.post9/hotsos/defs/scenarios/lxd/
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/lxd/lxcfs_deadlock.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/lxd/lxcfs_lp1807628.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.203449 hotsos-1.1.13.post9/hotsos/defs/scenarios/mysql/
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/mysql/bugs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/mysql/mysql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/mysql/mysql_connections.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/mysql/mysql_router.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.203449 hotsos-1.1.13.post9/hotsos/defs/scenarios/openstack/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.203449 hotsos-1.1.13.post9/hotsos/defs/scenarios/openstack/barbican/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/openstack/barbican/bugs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/openstack/eol.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.203449 hotsos-1.1.13.post9/hotsos/defs/scenarios/openstack/keystone/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/openstack/keystone/bugs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.207450 hotsos-1.1.13.post9/hotsos/defs/scenarios/openstack/masakari/
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/openstack/masakari/pacemaker_remote.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.207450 hotsos-1.1.13.post9/hotsos/defs/scenarios/openstack/neutron/
--rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/openstack/neutron/bugs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/openstack/neutron/neutron_ovs_cleanup.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/openstack/neutron/ovn_stale_db.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.207450 hotsos-1.1.13.post9/hotsos/defs/scenarios/openstack/nova/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/openstack/nova/bugs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/openstack/nova/config_checks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/openstack/nova/cpu_pinning.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.207450 hotsos-1.1.13.post9/hotsos/defs/scenarios/openstack/octavia/
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/openstack/octavia/bugs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/openstack/octavia/hm_port_health.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/openstack/openstack.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/openstack/openstack_apache2_certificates.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/openstack/pkgs_from_mixed_releases_found.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/openstack/system_cpufreq_mode.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/openstack/systemd_masked_services.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.207450 hotsos-1.1.13.post9/hotsos/defs/scenarios/openvswitch/
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/openvswitch/dpif_lost_packets.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/openvswitch/dpif_resubmit_actions.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/openvswitch/openvswitch.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.211450 hotsos-1.1.13.post9/hotsos/defs/scenarios/openvswitch/ovn/
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/openvswitch/ovn/bfd_flapping.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_bugs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_services.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_ssl_certs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_chassis_ssl_certs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_db_upgrade.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/openvswitch/ovn/ovsdb_reconnect_errors.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/openvswitch/ovs_bugs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/openvswitch/tunnels_ct.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.211450 hotsos-1.1.13.post9/hotsos/defs/scenarios/pacemaker/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/pacemaker/bugs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/pacemaker/pacemaker.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.211450 hotsos-1.1.13.post9/hotsos/defs/scenarios/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/rabbitmq/cluster_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/rabbitmq/cluster_logchecks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/rabbitmq/cluster_resources.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/rabbitmq/rabbitmq.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/rabbitmq/rabbitmq_bugs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.211450 hotsos-1.1.13.post9/hotsos/defs/scenarios/sosreport/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/sosreport/plugin_timeouts.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.211450 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.211450 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/bcache/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/bcache/bcache.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/bcache/bdev.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/bcache/cacheset.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.167447 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.211450 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mgr/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mgr/autoscaler_overlap_roots.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.215450 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/auth_insecure_global_id_reclaim_allowed.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/autoscaler_bug.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_size.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_spillover.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph-mon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_address_overlap.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_cluster_health.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_versions_mismatch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/crushmap_bucket_checks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/eol.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/laggy_pgs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/large_omap_objects.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_db_too_big.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_elections_flapping.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_flapping.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_maps_backlog_too_large.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_messenger_v2_protocol.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_heartbeats.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_ops.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_imbalance.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_overdose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/required_osd_release_mismatch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/unresponsive_mon_mgr.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.219451 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bcache_lp1936136.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph-osd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph_address_overlap.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/eol.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/filestore_to_bluestore_upgrade.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/juju_ceph_no_bcache_tuning.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_flapping.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_latency.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_slow_ops.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/pg_overdose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/ssd_osds_no_discard.yaml.disabled
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/system_cpufreq_mode.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/storage.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.219451 hotsos-1.1.13.post9/hotsos/defs/scenarios/system/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/system/system.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/defs/scenarios/system/unattended_upgrades.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.219451 hotsos-1.1.13.post9/hotsos/plugin_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/plugin_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.219451 hotsos-1.1.13.post9/hotsos/plugin_extensions/juju/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/plugin_extensions/juju/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/plugin_extensions/juju/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.219451 hotsos-1.1.13.post9/hotsos/plugin_extensions/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/plugin_extensions/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/plugin_extensions/kernel/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.223451 hotsos-1.1.13.post9/hotsos/plugin_extensions/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/plugin_extensions/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/plugin_extensions/kubernetes/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.223451 hotsos-1.1.13.post9/hotsos/plugin_extensions/lxd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/plugin_extensions/lxd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/plugin_extensions/lxd/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.223451 hotsos-1.1.13.post9/hotsos/plugin_extensions/maas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/plugin_extensions/maas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/plugin_extensions/maas/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.223451 hotsos-1.1.13.post9/hotsos/plugin_extensions/mysql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/plugin_extensions/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/plugin_extensions/mysql/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.223451 hotsos-1.1.13.post9/hotsos/plugin_extensions/openstack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/plugin_extensions/openstack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.223451 hotsos-1.1.13.post9/hotsos/plugin_extensions/openstack/agent/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/plugin_extensions/openstack/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12122 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/plugin_extensions/openstack/agent/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    11569 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/plugin_extensions/openstack/agent/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/plugin_extensions/openstack/nova_external_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/plugin_extensions/openstack/service_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/plugin_extensions/openstack/service_network_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/plugin_extensions/openstack/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    10918 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/plugin_extensions/openstack/vm_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.223451 hotsos-1.1.13.post9/hotsos/plugin_extensions/openvswitch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/plugin_extensions/openvswitch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9942 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/plugin_extensions/openvswitch/event_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/plugin_extensions/openvswitch/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.227451 hotsos-1.1.13.post9/hotsos/plugin_extensions/pacemaker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/plugin_extensions/pacemaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/plugin_extensions/pacemaker/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.227451 hotsos-1.1.13.post9/hotsos/plugin_extensions/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/plugin_extensions/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/plugin_extensions/rabbitmq/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.227451 hotsos-1.1.13.post9/hotsos/plugin_extensions/sosreport/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/plugin_extensions/sosreport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/plugin_extensions/sosreport/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.227451 hotsos-1.1.13.post9/hotsos/plugin_extensions/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/plugin_extensions/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/plugin_extensions/storage/bcache_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/plugin_extensions/storage/ceph_event_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/plugin_extensions/storage/ceph_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.227451 hotsos-1.1.13.post9/hotsos/plugin_extensions/system/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/plugin_extensions/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/plugin_extensions/system/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/plugin_extensions/system/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.227451 hotsos-1.1.13.post9/hotsos/plugin_extensions/vault/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/plugin_extensions/vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/plugin_extensions/vault/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.227451 hotsos-1.1.13.post9/hotsos/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/templates/content_dict.html
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/templates/content_list.html
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/hotsos/templates/header.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:21:57.175447 hotsos-1.1.13.post9/hotsos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-03-30 21:21:57.000000 hotsos-1.1.13.post9/hotsos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12701 2023-03-30 21:21:57.000000 hotsos-1.1.13.post9/hotsos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 21:21:57.000000 hotsos-1.1.13.post9/hotsos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-30 21:21:57.000000 hotsos-1.1.13.post9/hotsos.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-03-30 21:21:57.000000 hotsos-1.1.13.post9/hotsos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-30 21:21:57.000000 hotsos-1.1.13.post9/hotsos.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 21:21:57.227451 hotsos-1.1.13.post9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-30 21:21:36.000000 hotsos-1.1.13.post9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.559392 hotsos-1.1.14/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-18 11:55:12.000000 hotsos-1.1.14/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-18 11:55:12.000000 hotsos-1.1.14/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-05-18 11:55:34.555391 hotsos-1.1.14/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-05-18 11:55:12.000000 hotsos-1.1.14/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.515377 hotsos-1.1.14/hotsos/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-18 11:55:19.000000 hotsos-1.1.14/hotsos/.repo-info
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13956 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15453 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.515377 hotsos-1.1.14/hotsos/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10720 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.519378 hotsos-1.1.14/hotsos/core/host_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/host_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35158 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/host_helpers/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/host_helpers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/host_helpers/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/host_helpers/filestat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11021 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/host_helpers/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13238 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/host_helpers/packaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/host_helpers/pebble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/host_helpers/ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/host_helpers/sysctl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10656 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/host_helpers/systemd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/host_helpers/uptime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.519378 hotsos-1.1.14/hotsos/core/issues/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/issues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/issues/issue_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/issues/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.519378 hotsos-1.1.14/hotsos/core/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.519378 hotsos-1.1.14/hotsos/core/plugins/juju/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/juju/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/juju/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/juju/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.523380 hotsos-1.1.14/hotsos/core/plugins/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/kernel/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/kernel/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.523380 hotsos-1.1.14/hotsos/core/plugins/kernel/kernlog/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/kernel/kernlog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14810 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/kernel/kernlog/calltrace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/kernel/kernlog/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/kernel/kernlog/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/kernel/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20317 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/kernel/net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/kernel/sysfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/kubernetes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.523380 hotsos-1.1.14/hotsos/core/plugins/lxd/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/lxd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/lxd/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/maas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/mysql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.523380 hotsos-1.1.14/hotsos/core/plugins/openstack/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/openstack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/openstack/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63860 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/openstack/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/openstack/neutron.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/openstack/nova.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/openstack/octavia.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18883 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/openstack/openstack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.523380 hotsos-1.1.14/hotsos/core/plugins/openvswitch/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/openvswitch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/openvswitch/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/openvswitch/ovn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/openvswitch/ovs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/pacemaker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.523380 hotsos-1.1.14/hotsos/core/plugins/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/rabbitmq/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/rabbitmq/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/sosreport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.523380 hotsos-1.1.14/hotsos/core/plugins/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/storage/bcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37328 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/storage/ceph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.523380 hotsos-1.1.14/hotsos/core/plugins/system/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/system/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/system/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugins/vault.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13784 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/plugintools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.527381 hotsos-1.1.14/hotsos/core/ycheck/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/ycheck/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.527381 hotsos-1.1.14/hotsos/core/ycheck/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/ycheck/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/ycheck/engine/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.527381 hotsos-1.1.14/hotsos/core/ycheck/engine/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/ycheck/engine/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/ycheck/engine/properties/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22878 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/ycheck/engine/properties/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9696 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/ycheck/engine/properties/conclusions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/ycheck/engine/properties/input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.527381 hotsos-1.1.14/hotsos/core/ycheck/engine/properties/requires/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/ycheck/engine/properties/requires/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/ycheck/engine/properties/requires/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/ycheck/engine/properties/requires/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.527381 hotsos-1.1.14/hotsos/core/ycheck/engine/properties/requires/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/ycheck/engine/properties/requires/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/ycheck/engine/properties/requires/types/apt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/ycheck/engine/properties/requires/types/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/ycheck/engine/properties/requires/types/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/ycheck/engine/properties/requires/types/pebble.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/ycheck/engine/properties/requires/types/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/ycheck/engine/properties/requires/types/snap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/ycheck/engine/properties/requires/types/systemd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/ycheck/engine/properties/requires/types/varops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13326 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/ycheck/engine/properties/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/ycheck/engine/properties/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13783 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/ycheck/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/core/ycheck/scenarios.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.507374 hotsos-1.1.14/hotsos/defs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.507374 hotsos-1.1.14/hotsos/defs/events/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.527381 hotsos-1.1.14/hotsos/defs/events/openstack/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/events/openstack/apache.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/events/openstack/apparmor.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/events/openstack/http-requests.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.527381 hotsos-1.1.14/hotsos/defs/events/openstack/neutron/
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/events/openstack/neutron/agents.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/events/openstack/neutron/ml2-routers.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.531382 hotsos-1.1.14/hotsos/defs/events/openstack/nova/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/events/openstack/nova/external-events.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.531382 hotsos-1.1.14/hotsos/defs/events/openstack/nova/migrations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.531382 hotsos-1.1.14/hotsos/defs/events/openstack/nova/migrations/live-migration/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/events/openstack/nova/migrations/live-migration/dst-pre-live-migration.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/events/openstack/nova/migrations/live-migration/src-migration.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/events/openstack/nova/migrations/live-migration/src-post-live-migration.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/events/openstack/nova/migrations/migrations.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/events/openstack/nova/nova-compute.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/events/openstack/octavia.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.507374 hotsos-1.1.14/hotsos/defs/events/openvswitch/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.531382 hotsos-1.1.14/hotsos/defs/events/openvswitch/ovn/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/events/openvswitch/ovn/errors-and-warnings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/events/openvswitch/ovn/ovn-central.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/events/openvswitch/ovn/ovn-controller.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.531382 hotsos-1.1.14/hotsos/defs/events/openvswitch/ovs/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/events/openvswitch/ovs/bfd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/events/openvswitch/ovs/datapath-checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/events/openvswitch/ovs/errors-and-warnings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/events/openvswitch/ovs/ovs-vswitchd.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.507374 hotsos-1.1.14/hotsos/defs/events/storage/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.507374 hotsos-1.1.14/hotsos/defs/events/storage/ceph/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.531382 hotsos-1.1.14/hotsos/defs/events/storage/ceph/mon/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/events/storage/ceph/mon/mon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/events/storage/ceph/mon/monlogs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.531382 hotsos-1.1.14/hotsos/defs/events/storage/ceph/osd/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/events/storage/ceph/osd/osd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/events/storage/ceph/osd/osdlogs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.511376 hotsos-1.1.14/hotsos/defs/scenarios/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.531382 hotsos-1.1.14/hotsos/defs/scenarios/juju/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.535384 hotsos-1.1.14/hotsos/defs/scenarios/juju/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/juju/bugs/lp1812361.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/juju/bugs/lp1852502.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/juju/bugs/lp1858519.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/juju/bugs/lp1895040.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/juju/bugs/lp1910958.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/juju/bugs/lp1948906.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/juju/bugs/lp1983140.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/juju/bugs/lp1983506.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/juju/bugs/lp1996230.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/juju/charm_unit_checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/juju/juju.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/juju/jujud_machine_checks.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.535384 hotsos-1.1.14/hotsos/defs/scenarios/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/kernel/amd_iommu_pt.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/kernel/disk_failure.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/kernel/kernlog_calltrace.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/kernel/memory.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.535384 hotsos-1.1.14/hotsos/defs/scenarios/kernel/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/kernel/network/misc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/kernel/network/tcp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/kernel/network/udp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/kernel/qla2xxx.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.535384 hotsos-1.1.14/hotsos/defs/scenarios/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/kubernetes/kubernetes.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/kubernetes/system_cpufreq_mode.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.535384 hotsos-1.1.14/hotsos/defs/scenarios/lxd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.535384 hotsos-1.1.14/hotsos/defs/scenarios/lxd/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/lxd/bugs/lp1807628.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/lxd/lxcfs_deadlock.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.535384 hotsos-1.1.14/hotsos/defs/scenarios/mysql/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.535384 hotsos-1.1.14/hotsos/defs/scenarios/mysql/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/mysql/bugs/lp1959861.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/mysql/bugs/lp1971565.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/mysql/bugs/lp372017.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/mysql/mysql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/mysql/mysql_connections.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.535384 hotsos-1.1.14/hotsos/defs/scenarios/openstack/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.511376 hotsos-1.1.14/hotsos/defs/scenarios/openstack/barbican/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.535384 hotsos-1.1.14/hotsos/defs/scenarios/openstack/barbican/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openstack/barbican/bugs/lp1946787.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openstack/eol.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.511376 hotsos-1.1.14/hotsos/defs/scenarios/openstack/keystone/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.535384 hotsos-1.1.14/hotsos/defs/scenarios/openstack/keystone/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openstack/keystone/bugs/lp1896125.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.539385 hotsos-1.1.14/hotsos/defs/scenarios/openstack/masakari/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openstack/masakari/pacemaker_remote.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.539385 hotsos-1.1.14/hotsos/defs/scenarios/openstack/neutron/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.539385 hotsos-1.1.14/hotsos/defs/scenarios/openstack/neutron/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openstack/neutron/bugs/lp1794991.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openstack/neutron/bugs/lp1883089.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openstack/neutron/bugs/lp1896506.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openstack/neutron/bugs/lp1907686.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openstack/neutron/bugs/lp1927868.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openstack/neutron/bugs/lp1928031.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openstack/neutron/bugs/lp1929832.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openstack/neutron/bugs/lp1960319.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openstack/neutron/bugs/lp1965297.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openstack/neutron/bugs/lp1979089.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openstack/neutron/neutron_ovs_cleanup.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openstack/neutron/ovn_stale_db.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.539385 hotsos-1.1.14/hotsos/defs/scenarios/openstack/nova/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.539385 hotsos-1.1.14/hotsos/defs/scenarios/openstack/nova/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openstack/nova/bugs/lp1860743.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openstack/nova/bugs/lp1888395.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openstack/nova/bugs/lp1904580.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openstack/nova/bugs/lp1944619.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openstack/nova/config_checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openstack/nova/cpu_pinning.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.539385 hotsos-1.1.14/hotsos/defs/scenarios/openstack/octavia/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.539385 hotsos-1.1.14/hotsos/defs/scenarios/openstack/octavia/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openstack/octavia/bugs/sb1896125.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openstack/octavia/hm_port_health.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openstack/openstack.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openstack/openstack_apache2_certificates.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openstack/openstack_charm_conflicts.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openstack/pkgs_from_mixed_releases_found.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openstack/system_cpufreq_mode.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openstack/systemd_masked_services.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.539385 hotsos-1.1.14/hotsos/defs/scenarios/openvswitch/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.539385 hotsos-1.1.14/hotsos/defs/scenarios/openvswitch/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openvswitch/bugs/lp1839592.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openvswitch/bugs/lp1978806.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openvswitch/dpif_lost_packets.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openvswitch/dpif_resubmit_actions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openvswitch/openvswitch.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.543387 hotsos-1.1.14/hotsos/defs/scenarios/openvswitch/ovn/
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openvswitch/ovn/bfd_flapping.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.543387 hotsos-1.1.14/hotsos/defs/scenarios/openvswitch/ovn/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1865127.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1917475.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_certs_logs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_services.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openvswitch/ovn/ovn_certs_valid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openvswitch/ovn/ovn_chassis_certs_logs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openvswitch/ovn/ovn_db_upgrade.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/openvswitch/ovn/ovsdb_reconnect_errors.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.543387 hotsos-1.1.14/hotsos/defs/scenarios/pacemaker/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.543387 hotsos-1.1.14/hotsos/defs/scenarios/pacemaker/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/pacemaker/bugs/lp1874719.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/pacemaker/pacemaker.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.543387 hotsos-1.1.14/hotsos/defs/scenarios/rabbitmq/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.543387 hotsos-1.1.14/hotsos/defs/scenarios/rabbitmq/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/rabbitmq/bugs/lp1943937.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/rabbitmq/cluster_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/rabbitmq/cluster_logchecks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/rabbitmq/cluster_resources.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/rabbitmq/rabbitmq.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.543387 hotsos-1.1.14/hotsos/defs/scenarios/sosreport/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/sosreport/plugin_timeouts.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.543387 hotsos-1.1.14/hotsos/defs/scenarios/storage/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.543387 hotsos-1.1.14/hotsos/defs/scenarios/storage/bcache/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/bcache/bcache.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/bcache/bdev.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/bcache/cacheset.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.511376 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.543387 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mgr/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mgr/autoscaler_overlap_roots.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.547388 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/auth_insecure_global_id_reclaim_allowed.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/autoscaler_bug.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_size.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_spillover.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph-mon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_address_overlap.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_cluster_health.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_versions_mismatch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/crushmap_bucket_checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/eol.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/laggy_pgs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/large_omap_objects.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_db_too_big.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_elections_flapping.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_flapping.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_maps_backlog_too_large.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_messenger_v2_protocol.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_heartbeats.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_ops.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_imbalance.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_overdose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/required_osd_release_mismatch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/rgw_frontend.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/unresponsive_mon_mgr.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.551390 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-osd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.551390 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1936136.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1959649.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1996010.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2013960.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2016845.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph-osd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph_address_overlap.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-osd/eol.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-osd/filestore_to_bluestore_upgrade.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-osd/juju_ceph_no_bcache_tuning.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_flapping.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_latency.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_slow_ops.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-osd/pg_overdose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-osd/ssd_osds_no_discard.yaml.disabled
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-osd/system_cpufreq_mode.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.551390 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-rgw/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-rgw/rgw_frontend_rgw.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.551390 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/common/ceph_charm_conflicts.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/storage/storage.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.551390 hotsos-1.1.14/hotsos/defs/scenarios/system/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/system/system.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/defs/scenarios/system/unattended_upgrades.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.551390 hotsos-1.1.14/hotsos/plugin_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/plugin_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.551390 hotsos-1.1.14/hotsos/plugin_extensions/juju/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/plugin_extensions/juju/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/plugin_extensions/juju/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.551390 hotsos-1.1.14/hotsos/plugin_extensions/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/plugin_extensions/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/plugin_extensions/kernel/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.551390 hotsos-1.1.14/hotsos/plugin_extensions/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/plugin_extensions/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/plugin_extensions/kubernetes/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.551390 hotsos-1.1.14/hotsos/plugin_extensions/lxd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/plugin_extensions/lxd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/plugin_extensions/lxd/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.551390 hotsos-1.1.14/hotsos/plugin_extensions/maas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/plugin_extensions/maas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/plugin_extensions/maas/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.551390 hotsos-1.1.14/hotsos/plugin_extensions/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/plugin_extensions/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/plugin_extensions/mysql/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.555391 hotsos-1.1.14/hotsos/plugin_extensions/openstack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/plugin_extensions/openstack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.555391 hotsos-1.1.14/hotsos/plugin_extensions/openstack/agent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/plugin_extensions/openstack/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12122 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/plugin_extensions/openstack/agent/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/plugin_extensions/openstack/agent/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/plugin_extensions/openstack/nova_external_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/plugin_extensions/openstack/service_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/plugin_extensions/openstack/service_network_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/plugin_extensions/openstack/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10918 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/plugin_extensions/openstack/vm_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.555391 hotsos-1.1.14/hotsos/plugin_extensions/openvswitch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/plugin_extensions/openvswitch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9942 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/plugin_extensions/openvswitch/event_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/plugin_extensions/openvswitch/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.555391 hotsos-1.1.14/hotsos/plugin_extensions/pacemaker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/plugin_extensions/pacemaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/plugin_extensions/pacemaker/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.555391 hotsos-1.1.14/hotsos/plugin_extensions/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/plugin_extensions/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/plugin_extensions/rabbitmq/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.555391 hotsos-1.1.14/hotsos/plugin_extensions/sosreport/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/plugin_extensions/sosreport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/plugin_extensions/sosreport/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.555391 hotsos-1.1.14/hotsos/plugin_extensions/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/plugin_extensions/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/plugin_extensions/storage/bcache_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/plugin_extensions/storage/ceph_event_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/plugin_extensions/storage/ceph_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.555391 hotsos-1.1.14/hotsos/plugin_extensions/system/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/plugin_extensions/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/plugin_extensions/system/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/plugin_extensions/system/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.555391 hotsos-1.1.14/hotsos/plugin_extensions/vault/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/plugin_extensions/vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/plugin_extensions/vault/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.555391 hotsos-1.1.14/hotsos/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/templates/content_dict.html
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/templates/content_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-18 11:55:12.000000 hotsos-1.1.14/hotsos/templates/header.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:55:34.515377 hotsos-1.1.14/hotsos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-05-18 11:55:34.000000 hotsos-1.1.14/hotsos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14645 2023-05-18 11:55:34.000000 hotsos-1.1.14/hotsos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 11:55:34.000000 hotsos-1.1.14/hotsos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-18 11:55:34.000000 hotsos-1.1.14/hotsos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-18 11:55:34.000000 hotsos-1.1.14/hotsos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-18 11:55:34.000000 hotsos-1.1.14/hotsos.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-18 11:55:12.000000 hotsos-1.1.14/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 11:55:34.559392 hotsos-1.1.14/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-18 11:55:12.000000 hotsos-1.1.14/setup.py
```

### Comparing `hotsos-1.1.13.post9/LICENSE` & `hotsos-1.1.14/LICENSE`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/PKG-INFO` & `hotsos-1.1.14/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,106 +1,129 @@
 Metadata-Version: 2.1
 Name: hotsos
-Version: 1.1.13.post9
+Version: 1.1.14
 Summary: Software analysis toolkit. Define checks in high-level language and leverage library to perform analysis of common Cloud applications.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Overview
 
-Hotsos is a framework for software-defined analysis. It provides a library of plugins written in Python along with a [high-level language](hotsos/defs/README.md) in which to implement checks and analysis and report problems. Supported plugins include:
+Hotsos is a framework for software-defined analysis. It provides a library of
+plugins written in Python along with a [high-level
+language](hotsos/defs/README.md) in which to implement checks and analysis and
+report problems. Supported plugins include:
+
+* Openstack
+* Kubernetes
+* Ceph
+* Open vSwitch
+* Juju
+* MAAS
+* Vault
+* MySQL
+* RabbitMQ
+* and more
+
+Each plugin has a set of associated checks or "scenarios" that run in the
+context of that plugin and seek to identify issues. The output of running hotsos
+is a summary produced by each plugin including key information about the runtime
+of that application along with any issues detected. This summary also aims to
+contain as much information needed to aid manual analysis beyond the automated
+checks and is easily extensible.
 
-  * Openstack
-  * Kubernetes
-  * Ceph
-  * OpenvSwitch
-  * Juju
-  * MAAS
-  * Vault
-  * MySQL
-  * RabbitMQ
-  * and more
+The default summary format is yaml and a number of other options and formats are
+provided.
 
-Each plugin has a set of associated checks or "scenarios" that run in the context of that plugin and seek to identify issues. The output of running hotsos is a summary produced by each plugin including key information about the runtime of that application along with any issues detected. This summary also aims to contain as much information needed to aid manual analysis beyond the automated checks and is easily extensible.
-
-The default summary format is yaml and a number of other options and formats are provided.
-
-Hotsos is either run directly against a host or a [sosreport](https://github.com/sosreport/sos).
+Hotsos is either run directly against a host or a
+[sosreport](https://github.com/sosreport/sos).
 
 The code has the following structure:
 
-  * core library (includes plugins)
-  * yaml-defined checks (see documentation at [defs](hotsos/defs/README.md))
-  * plugin extensions e.g. summary output
-  * tests
+* core library (includes plugins)
+* yaml-defined checks (see documentation at [defs](hotsos/defs/README.md))
+* plugin extensions e.g. summary output
+* tests
 
 ## Usage
 
-Lets say for example that you are running an Openstack Cloud and one of your hypervisor nodes that also happens to be running part of a Ceph storage cluster is experiencing a problem with network connectivity to workloads. You can simply run hotsos either against a sosreport generated from that node or on that node directly as follows:
+Let's say for example that you are running an Openstack Cloud and one of your
+hypervisor nodes that also happens to be running part of a Ceph storage cluster
+is experiencing a problem with network connectivity to workloads. You can simply
+run hotsos either against a sosreport generated from that node or on that node
+directly as follows:
 
-```
+```console
 ubuntu@ncpu1$ hotsos -s
 INFO: analysing localhost /
 INFO: output saved to hotsos-output-1673868979
 ```
 
-Now you will find a folder called hotsos-output-1673868979 containing a summary of information in a number of different formats. Taking the most common yaml format we can see:
+Now you will find a folder called `hotsos-output-1673868979` containing a
+summary of information in a number of different formats. Taking the most common
+yaml format we can see:
 
-```
+```console
 ubuntu@ncpu1$ cat hotsos-output-1673868979/ncpu1.summary.yaml
 ```
 
-This file will contain a per-plugin summary of information found along with any issues detected. By default hotsos will only look at the last 24 hours of logs. You can increase this with *--all-logs* which will by default give you 7 days worth and if you want more you can use *--max-logrotate-depth <days>*.
-
-Our folder also contains other formats of the same information and one of those is json which can easily be queried using a tool called [jq](https://stedolan.github.io/jq/). Using this useful tool we can easily query for specific information e.g.
+This file will contain a per-plugin summary of information found along with any
+issues detected. By default hotsos will only look at the last 24 hours of logs.
+You can increase this with `--all-logs` which will by default give you 7 days
+worth and if you want more you can use `--max-logrotate-depth <days>`.
+
+Our folder also contains other formats of the same information and one of those
+is json which can easily be queried using a tool called
+[jq](https://stedolan.github.io/jq/). Using this useful tool we can easily query
+for specific information e.g.
 
-```
+```console
 ubuntu@ncpu1$ jq -r '.storage."potential-issues"' hotsos-output-1673868979/ncpu1.summary.json
 {
   "BcacheWarnings": [
     "One or more of the following bcache bdev config assertions failed: sequential_cutoff eq \"0.0k\"/actual=\"4.0M\", cache_mode eq \"writethrough [writeback] writearound none\"/actual=\"writethrough [writeback] writearound none\", writeback_percent ge 10/actual=\"10\" (origin=storage.auto_scenario_check)",
     "One or more of the following bcache cacheset config assertions failed: congested_read_threshold_us eq 0/actual=\"2000\", congested_write_threshold_us eq 0/actual=\"20000\" (origin=storage.auto_scenario_check)"
   ]
 }
 ```
 
 ## Examples
 
-An example **full** (yaml) summary can be found [here](examples/hotsos-example-openstack.summary.yaml)
+An example **full** (yaml) summary can be found
+[here](examples/hotsos-example-openstack.summary.yaml)
 
-An example **short** (yaml) summary can be found [here](examples/hotsos-example-openstack.short.summary.yaml)
+An example **short** (yaml) summary can be found
+[here](examples/hotsos-example-openstack.short.summary.yaml)
 
 ## Install
 
 HotSOS is distributed using the following methods:
 
 ### pypi
 
 You can install using Python pip e.g.
 
-```
-sudo apt install python3-pip
-pip install hotsos
+```console
+$ sudo apt install python3-pip
+$ pip install hotsos
 ```
 
 NOTE: currently requires Python >= 3.8
 
 ### snap
 
 You can install as a snap e.g.
 
-```
-sudo apt install snapd
-sudo snap install hotsos --classic
+```console
+$ sudo apt install snapd
+$ sudo snap install hotsos --classic
 ```
 
-See https://snapcraft.io/hotsos for more info on usage.
+See <https://snapcraft.io/hotsos> for more info on usage.
 
 or run from source e.g.
 
-```
+```console
 $ git clone https://github.com/canonical/hotsos
 $ pip install -r hotsos/requirements.txt
 $ ./hotsos/scripts/hotsos
 ```
-
```

### Comparing `hotsos-1.1.13.post9/README.md` & `hotsos-1.1.14/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,98 +1,121 @@
 # Overview
 
-Hotsos is a framework for software-defined analysis. It provides a library of plugins written in Python along with a [high-level language](hotsos/defs/README.md) in which to implement checks and analysis and report problems. Supported plugins include:
+Hotsos is a framework for software-defined analysis. It provides a library of
+plugins written in Python along with a [high-level
+language](hotsos/defs/README.md) in which to implement checks and analysis and
+report problems. Supported plugins include:
+
+* Openstack
+* Kubernetes
+* Ceph
+* Open vSwitch
+* Juju
+* MAAS
+* Vault
+* MySQL
+* RabbitMQ
+* and more
+
+Each plugin has a set of associated checks or "scenarios" that run in the
+context of that plugin and seek to identify issues. The output of running hotsos
+is a summary produced by each plugin including key information about the runtime
+of that application along with any issues detected. This summary also aims to
+contain as much information needed to aid manual analysis beyond the automated
+checks and is easily extensible.
 
-  * Openstack
-  * Kubernetes
-  * Ceph
-  * OpenvSwitch
-  * Juju
-  * MAAS
-  * Vault
-  * MySQL
-  * RabbitMQ
-  * and more
+The default summary format is yaml and a number of other options and formats are
+provided.
 
-Each plugin has a set of associated checks or "scenarios" that run in the context of that plugin and seek to identify issues. The output of running hotsos is a summary produced by each plugin including key information about the runtime of that application along with any issues detected. This summary also aims to contain as much information needed to aid manual analysis beyond the automated checks and is easily extensible.
-
-The default summary format is yaml and a number of other options and formats are provided.
-
-Hotsos is either run directly against a host or a [sosreport](https://github.com/sosreport/sos).
+Hotsos is either run directly against a host or a
+[sosreport](https://github.com/sosreport/sos).
 
 The code has the following structure:
 
-  * core library (includes plugins)
-  * yaml-defined checks (see documentation at [defs](hotsos/defs/README.md))
-  * plugin extensions e.g. summary output
-  * tests
+* core library (includes plugins)
+* yaml-defined checks (see documentation at [defs](hotsos/defs/README.md))
+* plugin extensions e.g. summary output
+* tests
 
 ## Usage
 
-Lets say for example that you are running an Openstack Cloud and one of your hypervisor nodes that also happens to be running part of a Ceph storage cluster is experiencing a problem with network connectivity to workloads. You can simply run hotsos either against a sosreport generated from that node or on that node directly as follows:
+Let's say for example that you are running an Openstack Cloud and one of your
+hypervisor nodes that also happens to be running part of a Ceph storage cluster
+is experiencing a problem with network connectivity to workloads. You can simply
+run hotsos either against a sosreport generated from that node or on that node
+directly as follows:
 
-```
+```console
 ubuntu@ncpu1$ hotsos -s
 INFO: analysing localhost /
 INFO: output saved to hotsos-output-1673868979
 ```
 
-Now you will find a folder called hotsos-output-1673868979 containing a summary of information in a number of different formats. Taking the most common yaml format we can see:
+Now you will find a folder called `hotsos-output-1673868979` containing a
+summary of information in a number of different formats. Taking the most common
+yaml format we can see:
 
-```
+```console
 ubuntu@ncpu1$ cat hotsos-output-1673868979/ncpu1.summary.yaml
 ```
 
-This file will contain a per-plugin summary of information found along with any issues detected. By default hotsos will only look at the last 24 hours of logs. You can increase this with *--all-logs* which will by default give you 7 days worth and if you want more you can use *--max-logrotate-depth <days>*.
-
-Our folder also contains other formats of the same information and one of those is json which can easily be queried using a tool called [jq](https://stedolan.github.io/jq/). Using this useful tool we can easily query for specific information e.g.
+This file will contain a per-plugin summary of information found along with any
+issues detected. By default hotsos will only look at the last 24 hours of logs.
+You can increase this with `--all-logs` which will by default give you 7 days
+worth and if you want more you can use `--max-logrotate-depth <days>`.
+
+Our folder also contains other formats of the same information and one of those
+is json which can easily be queried using a tool called
+[jq](https://stedolan.github.io/jq/). Using this useful tool we can easily query
+for specific information e.g.
 
-```
+```console
 ubuntu@ncpu1$ jq -r '.storage."potential-issues"' hotsos-output-1673868979/ncpu1.summary.json
 {
   "BcacheWarnings": [
     "One or more of the following bcache bdev config assertions failed: sequential_cutoff eq \"0.0k\"/actual=\"4.0M\", cache_mode eq \"writethrough [writeback] writearound none\"/actual=\"writethrough [writeback] writearound none\", writeback_percent ge 10/actual=\"10\" (origin=storage.auto_scenario_check)",
     "One or more of the following bcache cacheset config assertions failed: congested_read_threshold_us eq 0/actual=\"2000\", congested_write_threshold_us eq 0/actual=\"20000\" (origin=storage.auto_scenario_check)"
   ]
 }
 ```
 
 ## Examples
 
-An example **full** (yaml) summary can be found [here](examples/hotsos-example-openstack.summary.yaml)
+An example **full** (yaml) summary can be found
+[here](examples/hotsos-example-openstack.summary.yaml)
 
-An example **short** (yaml) summary can be found [here](examples/hotsos-example-openstack.short.summary.yaml)
+An example **short** (yaml) summary can be found
+[here](examples/hotsos-example-openstack.short.summary.yaml)
 
 ## Install
 
 HotSOS is distributed using the following methods:
 
 ### pypi
 
 You can install using Python pip e.g.
 
-```
-sudo apt install python3-pip
-pip install hotsos
+```console
+$ sudo apt install python3-pip
+$ pip install hotsos
 ```
 
 NOTE: currently requires Python >= 3.8
 
 ### snap
 
 You can install as a snap e.g.
 
-```
-sudo apt install snapd
-sudo snap install hotsos --classic
+```console
+$ sudo apt install snapd
+$ sudo snap install hotsos --classic
 ```
 
-See https://snapcraft.io/hotsos for more info on usage.
+See <https://snapcraft.io/hotsos> for more info on usage.
 
 or run from source e.g.
 
-```
+```console
 $ git clone https://github.com/canonical/hotsos
 $ pip install -r hotsos/requirements.txt
 $ ./hotsos/scripts/hotsos
 ```
-
```

### Comparing `hotsos-1.1.13.post9/hotsos/cli.py` & `hotsos-1.1.14/hotsos/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -156,14 +156,17 @@
         return os.path.basename(data_root)
 
     return CLIHelper().hostname()
 
 
 def main():
     @click.command(name='hotsos')
+    @click.option('--command-timeout', default=HotSOSConfig.command_timeout,
+                  help=('Amount of time command execution will wait before '
+                        'timing out and moving on.'))
     @click.option('--allow-constraints-for-unverifiable-logs', default=False,
                   is_flag=True)
     @click.option('--output-path', default=None,
                   help=('Optional path to use for saving output (with '
                         '--save).'))
     @click.option('--machine-readable', default=False, is_flag=True,
                   help=("Don't format output for humans."))
@@ -244,15 +247,16 @@
     @set_plugin_options
     @click.argument('data_root', required=False, type=click.Path(exists=True))
     def cli(data_root, version, defs_path, templates_path, all_logs, quiet,
             debug, save, format, html_escape, short, very_short,
             force, full, agent_error_key_by_time, event_tally_granularity,
             max_logrotate_depth, max_parallel_tasks, list_plugins,
             machine_readable, output_path,
-            allow_constraints_for_unverifiable_logs, **kwargs):
+            allow_constraints_for_unverifiable_logs, command_timeout,
+            **kwargs):
         """
         Run this tool on a host or against an unpacked sosreport to perform
         analysis of specific applications and the host itself. A summary of
         information is generated along with any issues or known bugs detected.
         Applications are defined as plugins and support currently includes
         Openstack, Kubernetes, Ceph and more (see --list-plugins). The
         standard output format is yaml to allow easy visual inspection and
@@ -285,14 +289,15 @@
         HotSOSConfig.force_mode = force
         repo_info = get_repo_info()
         if repo_info:
             HotSOSConfig.repo_info = repo_info
 
         _version = get_version()
         HotSOSConfig.hotsos_version = _version
+        HotSOSConfig.command_timeout = command_timeout
 
         if version:
             print(_version)
             return
 
         data_root = fix_data_root(data_root)
         if agent_error_key_by_time:
```

### Comparing `hotsos-1.1.13.post9/hotsos/client.py` & `hotsos-1.1.14/hotsos/client.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -380,20 +380,20 @@
         """ State saved here is specific to a plugin. """
         log.debug("setting up plugin env")
         global_tmp = HotSOSConfig.global_tmp_dir
         HotSOSConfig.plugin_tmp_dir = tempfile.mkdtemp(prefix=plugin,
                                                        dir=global_tmp)
 
     def _run(self, plugin):
-        log.debug("running plugin %s", plugin)
         if plugin not in PLUGIN_CATALOG:
             raise Exception("unknown plugin {}".format(plugin))
 
-        HotSOSConfig.plugin_name = plugin
         log.name = 'plugin.{}'.format(plugin)
+        log.debug("running plugin %s", plugin)
+        HotSOSConfig.plugin_name = plugin
         parts = PLUGIN_CATALOG[plugin]
         return plugintools.PluginRunner(parts).run()
 
     @property
     def summary(self):
         return self._summary
```

### Comparing `hotsos-1.1.13.post9/hotsos/core/analytics.py` & `hotsos-1.1.14/hotsos/core/analytics.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/core/config.py` & `hotsos-1.1.14/hotsos/core/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -98,14 +98,20 @@
         self.add(ConfigOpt(name='event_tally_granularity',
                            description=("By default event tallies are listed "
                                         "by date in the summary. This option "
                                         "can be set to one of 'date' or "
                                         "'time' to get the corresponding "
                                         "granularity of results."),
                            default_value='date'))
+        self.add(ConfigOpt(name='command_timeout',
+                           description=("Maximum time in seconds before "
+                                        "command execution will timeout. Used "
+                                        "by host_helpers.cli when executing "
+                                        "binary commands"),
+                           default_value=300))
 
     @property
     def name(self):
         return 'hotsos'
 
 
 class SearchtoolsConfigOpts(ConfigOptGroupBase):
```

### Comparing `hotsos-1.1.13.post9/hotsos/core/factory.py` & `hotsos-1.1.14/hotsos/core/factory.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/core/host_helpers/__init__.py` & `hotsos-1.1.14/hotsos/core/host_helpers/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,21 +9,23 @@
 )
 from .packaging import (  # noqa: F403,F401
     DPKGVersionCompare,
     APTPackageHelper,
     DockerImageHelper,
     SnapPackageHelper,
 )
+from .pebble import (  # noqa: F403,F401
+    PebbleHelper,
+)
 from .ssl import (  # noqa: F403,F401
     SSLCertificate,
     SSLCertificatesHelper,
 )
 from .systemd import (  # noqa: F403,F401
     SystemdHelper,
-    SVC_EXPR_TEMPLATES,
 )
 from .uptime import (  # noqa: F403,F401
     UptimeHelper,
 )
 from .sysctl import (  # noqa: F403,F401
     SYSCtlFactory,
     SYSCtlConfHelper,
```

### Comparing `hotsos-1.1.13.post9/hotsos/core/host_helpers/cli.py` & `hotsos-1.1.14/hotsos/core/host_helpers/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 import subprocess
 import tempfile
 
 from hotsos.core.log import log
 from hotsos.core.config import HotSOSConfig
 from hotsos.core.host_helpers.common import HostHelpersBase
 
+CLI_COMMON_EXCEPTIONS = (OSError, subprocess.CalledProcessError,
+                         subprocess.TimeoutExpired,
+                         json.JSONDecodeError)
+
 
 class CLIExecError(Exception):
 
     def __init__(self, return_value=None):
         """
         @param return_value: default return value that a command
                              should return if execution fails.
@@ -24,15 +28,20 @@
 
 def catch_exceptions(*exc_types):
     def catch_exceptions_inner1(f):
         def catch_exceptions_inner2(*args, **kwargs):
             try:
                 return f(*args, **kwargs)
             except exc_types as exc:
-                log.debug("%s: %s", type(exc), exc)
+                msg = "{}: {}".format(type(exc), exc)
+                if isinstance(exc, subprocess.TimeoutExpired):
+                    log.info(msg)
+                else:
+                    log.debug(msg)
+
                 if type(exc) == json.JSONDecodeError:
                     raise CLIExecError(return_value={}) from exc
 
                 raise CLIExecError(return_value=[]) from exc
 
         return catch_exceptions_inner2
 
@@ -149,29 +158,30 @@
 
     def reset(self):
         self.cmd = self.original_cmd
         self.original_cmd_extras = []
         self.json_decode = self.original_json_decode
         self.singleline = self.original_singleline
 
-    @catch_exceptions(OSError, subprocess.CalledProcessError,
-                      json.JSONDecodeError)
+    @catch_exceptions(*CLI_COMMON_EXCEPTIONS)
     @reset_command
     @run_post_exec_hooks
     @run_pre_exec_hooks
     def __call__(self, *args, **kwargs):
         cmd = self.cmd
         if args:
             cmd = cmd.format(*args)
 
         if kwargs:
             cmd = cmd.format(**kwargs)
 
         _cmd = cmd.split() + self.original_cmd_extras
-        output = subprocess.check_output(_cmd, stderr=subprocess.STDOUT)
+        output = subprocess.check_output(_cmd,
+                                         timeout=HotSOSConfig.command_timeout,
+                                         stderr=subprocess.STDOUT)
 
         if self.json_decode:
             return json.loads(output.decode('UTF-8'))
 
         if self.singleline:
             return output.decode('UTF-8').strip()
 
@@ -191,16 +201,15 @@
 
     def reset(self):
         self.path = self.original_path
         self.safe_decode = self.original_safe_decode
         self.json_decode = self.original_json_decode
         self.singleline = self.original_singleline
 
-    @catch_exceptions(OSError, subprocess.CalledProcessError,
-                      json.JSONDecodeError)
+    @catch_exceptions(*CLI_COMMON_EXCEPTIONS)
     @reset_command
     @run_post_exec_hooks
     @run_pre_exec_hooks
     def __call__(self, *args, **kwargs):
         if args:
             self.path = self.path.format(*args)
 
@@ -226,16 +235,15 @@
         return output
 
 
 class BinFileCmd(FileCmd):
     """ This is used when we are executing an actual binary/command against a
     file. """
 
-    @catch_exceptions(OSError, subprocess.CalledProcessError,
-                      json.JSONDecodeError)
+    @catch_exceptions(*CLI_COMMON_EXCEPTIONS)
     @reset_command
     @run_post_exec_hooks
     @run_pre_exec_hooks
     def __call__(self, *args, **kwargs):
         # TODO: find a better way to handle this because path may still need
         # formatting.
         if not os.path.exists(self.original_path):
@@ -254,14 +262,15 @@
             env['TZ'] = DateFileCmd('sos_commands/date/date',
                                     singleline=True)(format="+%Z")
         except SourceNotFound:
             pass
 
         # Now split into a command and run
         output = subprocess.check_output(self.path.split(),
+                                         timeout=HotSOSConfig.command_timeout,
                                          stderr=subprocess.STDOUT, env=env)
 
         return output.decode('UTF-8').splitlines(keepends=True)
 
 
 class JournalctlBase(object):
 
@@ -411,15 +420,16 @@
 
         # Include tz if available and then convert to utc
         date = "{} {} {}".format(ret[1], tz, ret[3])
         cmd = ["date", "--utc", "--date={}".format(date)]
         if format:
             cmd.append(format)
 
-        output = subprocess.check_output(cmd)
+        output = subprocess.check_output(cmd,
+                                         timeout=HotSOSConfig.command_timeout)
         # date sometimes adds multiple whitespaces between fields so collapse
         # them.
         output = re.compile(r"\s+").sub(' ', output.decode('UTF-8'))
         ret = output.splitlines(keepends=True)[0]
         # always singleline so always strip trailing newline
         return ret.strip()
 
@@ -499,37 +509,41 @@
             except SourceNotFound:
                 pass
 
         if HotSOSConfig.data_root != '/':
             return NullSource()()
 
         # binary sources only apply if data_root is system root
+        bin_out = None
         for bsource in [s for s in self.sources if s.TYPE == "BIN"]:
             cache = False
             # NOTE: we currently only support caching commands with no
             #       args.
             if not any([args, kwargs]):
                 cache = True
                 out = self.cache.load(self.cmdkey)
                 if out is not None:
                     return out
 
             try:
-                out = bsource(*args, **kwargs)
+                bin_out = bsource(*args, **kwargs)
+                if cache and bin_out is not None:
+                    try:
+                        self.cache.save(self.cmdkey, bin_out)
+                    except pickle.PicklingError as exc:
+                        log.info("unable to cache command '%s' output: %s",
+                                 self.cmdkey, exc)
+
+                # if command executed but returned nothing that still counts
+                # as success.
+                break
             except CLIExecError as exc:
-                return exc.return_value
-
-            if cache and out is not None:
-                try:
-                    self.cache.save(self.cmdkey, out)
-                except pickle.PicklingError as exc:
-                    log.info("unable to cache command '%s' output: %s",
-                             self.cmdkey, exc)
+                bin_out = exc.return_value
 
-            return out
+        return bin_out
 
 
 class CLICacheWrapper(object):
 
     def __init__(self, cache_load_f, cache_save_f):
         self.load_f = cache_load_f
         self.save_f = cache_save_f
@@ -760,14 +774,17 @@
                  JournalctlBinFileCmd('var/log/journal')],
             'ls_lanR_sys_block':
                 [BinCmd('ls -lanR /sys/block/'),
                  FileCmd('sos_commands/block/ls_-lanR_.sys.block')],
             'lscpu':
                 [BinCmd('lscpu'),
                  FileCmd('sos_commands/processor/lscpu')],
+            'lsof_Mnlc':
+                [BinCmd('lsof +M -n -l -c ""'),
+                 FileCmd('sos_commands/process/lsof_M_-n_-l_-c')],
             'lxd_buginfo':
                 [BinCmd('lxd.buginfo'),
                  FileCmd('sos_commands/lxd/lxd.buginfo')],
             'numactl':
                 [BinCmd('numactl --hardware'),
                  FileCmd('sos_commands/numa/numactl_--hardware')],
             'ns_ip_addr':
@@ -820,14 +837,22 @@
                  FileCmd('sos_commands/openvswitch/'
                          'ovs-ofctl_-O_OpenFlow10_show_{bridge}'),
                  FileCmd('sos_commands/openvswitch/'
                          'ovs-ofctl_show_{bridge}')],
             'pacemaker_crm_status':
                 [BinCmd('crm status'),
                  FileCmd('sos_commands/pacemaker/crm_status')],
+            'pebble_services':
+                [BinCmd('pebble services'),
+                 # This is how operator charms run it
+                 BinCmd('/charm/bin/pebble services'),
+                 # The following does not exist in sosreport yet but adding
+                 # since it is useful for testing and will hopefully be
+                 # supported in sos at some point.
+                 FileCmd('sos_commands/pebble/pebble_services')],
             'ps':
                 [BinCmd('ps auxwww'),
                  FileCmd('ps')],
             'ps_axo_flags':
                 [BinCmd('ps axo flags,state,uid,pid,ppid,pgid,sid,cls,'
                         'pri,addr,sz,wchan:20,lstart,tty,time,cmd'),
                  # Older sosrepot uses 'wchan' option while newer ones use
```

### Comparing `hotsos-1.1.13.post9/hotsos/core/host_helpers/config.py` & `hotsos-1.1.14/hotsos/core/host_helpers/config.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/core/host_helpers/filestat.py` & `hotsos-1.1.14/hotsos/core/host_helpers/filestat.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,16 +7,23 @@
 
 class FileObj(object):
 
     def __init__(self, filename):
         self.filename = os.path.join(HotSOSConfig.data_root, filename)
 
     @property
+    def exists(self):
+        if os.path.exists(self.filename):
+            return True
+
+        return False
+
+    @property
     def mtime(self):
-        if not os.path.exists(self.filename):
+        if not self.exists:
             log.debug("mtime %s - file not found", self.filename)
             return 0
 
         mt = os.path.getmtime(self.filename)
         log.debug("mtime %s=%s", self.filename, mt)
         return mt
```

### Comparing `hotsos-1.1.13.post9/hotsos/core/host_helpers/network.py` & `hotsos-1.1.14/hotsos/core/host_helpers/network.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,18 +210,18 @@
                                 tag='ip_addr_show')
         search_obj = FileSearcher()
         if namespaces:
             for ns in self.cli.ip_netns():
                 ns_name = ns.partition(" ")[0]
                 ip_addr = self.cli.ns_ip_addr(namespace=ns_name)
                 prefix = "__ns_start__{}__ns__end__".format(ns_name)
-                path = mktemp_dump('\n'.join(ip_addr), prefix=prefix)
+                path = mktemp_dump(''.join(ip_addr), prefix=prefix)
                 search_obj.add(seq, path)
         else:
-            path = mktemp_dump('\n'.join(self.cli.ip_addr()))
+            path = mktemp_dump(''.join(self.cli.ip_addr()))
             search_obj.add(seq, path)
 
         if not search_obj.files:
             log.debug("no network info found (namespaces=%s)", namespaces)
             return []
 
         r = search_obj.run()
```

### Comparing `hotsos-1.1.13.post9/hotsos/core/host_helpers/packaging.py` & `hotsos-1.1.14/hotsos/core/host_helpers/packaging.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/core/host_helpers/sysctl.py` & `hotsos-1.1.14/hotsos/core/host_helpers/sysctl.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/core/host_helpers/systemd.py` & `hotsos-1.1.14/hotsos/core/host_helpers/systemd.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,22 +4,17 @@
 
 import re
 
 from hotsos.core.log import log
 from hotsos.core.config import HotSOSConfig
 from hotsos.core.factory import FactoryBase
 from hotsos.core.host_helpers import CLIHelper
+from hotsos.core.host_helpers.common import ServiceManagerBase
 from hotsos.core.utils import cached_property, sorted_dict
 
-SVC_EXPR_TEMPLATES = {
-    "absolute": r".+\S+bin/({})(?:\s+.+|$)",
-    "snap": r".+\S+\d+/({})(?:\s+.+|$)",
-    "relative": r".+\s({})(?:\s+.+|$)",
-    }
-
 
 class SystemdService(object):
 
     def __init__(self, name, state, has_instances=False):
         self.name = name
         self.state = state
         self.has_instances = has_instances
@@ -60,27 +55,19 @@
 
     def __repr__(self):
         return ("name={}, state={}, start_time={}, has_instances={}".
                 format(self.name, self.state, self.start_time,
                        self.has_instances))
 
 
-class SystemdHelper(object):
+class SystemdHelper(ServiceManagerBase):
     """ Helper class used to query systemd services. """
 
-    def __init__(self, service_exprs, ps_allow_relative=True):
-        """
-        @param service_exprs: list of python.re expressions used to match
-                              service names.
-        @param ps_allow_relative: whether to allow commands to be identified
-                                  from ps as run using an relative binary
-                                  path e.g. mycmd as opposed to /bin/mycmd.
-        """
-        self._ps_allow_relative = ps_allow_relative
-        self._service_exprs = set(service_exprs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
         self._cached_unit_files_exprs = {}
 
     @cached_property
     def _systemctl_list_units(self):
         return CLIHelper().systemctl_list_units()
 
     @cached_property
@@ -121,15 +108,15 @@
         #       we can search for related units later.
         unit_expr = r'^\s*({}@?)\.service\s+(\S+)'.format(base_expr)
         # match entries in systemctl list-unit-files
         self._cached_unit_files_exprs[svc_name_expr] = re.compile(unit_expr)
         return self._cached_unit_files_exprs[svc_name_expr]
 
     @cached_property
-    def services(self):
+    def services(self):  # pylint: disable=W0236
         """
         Return a dict of identified systemd services and their state.
 
         Service units are either direct or indirect. We unify these types,
         taking the state of whichever is actually in use i.e. has in-memory
         instances. Enabled units are aggregated but masked units are not so
         that they can be identified and reported.
@@ -184,27 +171,15 @@
 
     @property
     def masked_services(self):
         """ Returns a list of masked services. """
         if not self.services:
             return []
 
-        return self._service_info.get('masked', [])
-
-    def get_process_cmd_from_line(self, line, expr):
-        for expr_type, expr_tmplt in SVC_EXPR_TEMPLATES.items():
-            if expr_type == 'relative' and not self._ps_allow_relative:
-                continue
-
-            ret = re.compile(expr_tmplt.format(expr)).match(line)
-            if ret:
-                svc = ret.group(1)
-                log.debug("matched process %s with %s expr", svc,
-                          expr_type)
-                return svc
+        return sorted(self._service_info.get('masked', []))
 
     def get_services_expanded(self, name):
         _expanded = []
         for line in self._systemctl_list_units:
             expr = r'^\s*({}(@\S*)?)\.service'.format(name)
             ret = re.compile(expr).match(line)
             if ret:
@@ -222,14 +197,20 @@
         get their corresponding binary name from ps.
 
         Returns list of lines from ps that match the service pids.
         """
         ps_filtered = []
         path = os.path.join(HotSOSConfig.data_root,
                             'sys/fs/cgroup/unified/system.slice')
+        if not os.path.exists(path):
+            # Seems that this path changed between Ubuntu Focal and Jammy
+            # releases.
+            path = os.path.join(HotSOSConfig.data_root,
+                                'sys/fs/cgroup/system.slice')
+
         for svc in self.services:
             for svc in self.get_services_expanded(svc):
                 _path = os.path.join(path, "{}.service".format(svc),
                                      'cgroup.procs')
                 if not os.path.exists(_path):
                     _path = glob.glob(os.path.join(path, 'system-*.slice',
                                                    "{}.service".format(svc),
@@ -246,19 +227,19 @@
                                         line):
                                 ps_filtered.append(line)
                                 break
 
         return ps_filtered
 
     @cached_property
-    def processes(self):
+    def processes(self):  # pylint: disable=W0236
         """
         Identify running processes from ps that are associated with resolved
-        systemd services. The same search pattern used for identifying systemd
-        services is to match the process binary name.
+        systemd services. The search pattern used to identify a service is also
+        used to match the process binary name.
 
         Returns a dictionary of process names along with the number of each.
         """
         _proc_info = {}
         for line in self._service_filtered_ps:
             for expr in self._service_exprs:
                 """
@@ -268,20 +249,22 @@
                 /snap/<name>/1830/<svc>
                 /usr/bin/<svc>
 
                 and filter e.g.
 
                 /var/lib/<svc> and /var/log/<svc>
                 """
-                cmd = self.get_process_cmd_from_line(line, expr)
-                if cmd:
-                    if cmd in _proc_info:
-                        _proc_info[cmd] += 1
-                    else:
-                        _proc_info[cmd] = 1
+                cmd = self.get_cmd_from_ps_line(line, expr)
+                if not cmd:
+                    continue
+
+                if cmd in _proc_info:
+                    _proc_info[cmd] += 1
+                else:
+                    _proc_info[cmd] = 1
 
         return _proc_info
 
     @property
     def _service_info(self):
         """Return a dictionary of systemd services grouped by state. """
         info = {}
```

### Comparing `hotsos-1.1.13.post9/hotsos/core/host_helpers/uptime.py` & `hotsos-1.1.14/hotsos/core/host_helpers/uptime.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,16 @@
     def __init__(self):
         # unfortunately sosreports dont have proc/uptime otherwise we would use
         # that.
         self.uptime = CLIHelper().uptime() or ""
         # this needs to take into account the different formats supported by
         # https://gitlab.com/procps-ng/procps/-/blob/newlib/library/uptime.c
         etime_expr = r"(?:([\d:]+)|(\d+\s+\S+,\s+[\d:]+)|(\d+\s+\S+)),"
-        expr = r"\s*[\d:]+ up {}.+ load average: (.+)".format(etime_expr)
+        expr = (r"\s*[\d:]+\s+up\s+{}.+\s+load average:\s+(.+)".
+                format(etime_expr))
         ret = re.compile(expr).match(self.uptime)
         self.subgroups = {}
         if ret:
             self.subgroups['hour'] = {'value': ret.group(1),
                                       'expr': r'(\d+):(\d+)'}
             self.subgroups['day'] = {'value': ret.group(2),
                                      'expr': r"(\d+)\s+\S+,\s+(\d+):(\d+)"}
```

### Comparing `hotsos-1.1.13.post9/hotsos/core/issues/issue_types.py` & `hotsos-1.1.14/hotsos/core/issues/issue_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,18 @@
     pass
 
 
 class CephMgrError(IssueTypeBase):
     pass
 
 
+class CephRGWWarning(IssueTypeBase):
+    pass
+
+
 class CephDaemonWarning(IssueTypeBase):
     pass
 
 
 class CephDaemonVersionsError(IssueTypeBase):
     pass
```

### Comparing `hotsos-1.1.13.post9/hotsos/core/issues/utils.py` & `hotsos-1.1.14/hotsos/core/issues/utils.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/core/log.py` & `hotsos-1.1.14/hotsos/core/log.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/core/plugins/juju/common.py` & `hotsos-1.1.14/hotsos/core/plugins/juju/common.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 
 from hotsos.core import plugintools
-from hotsos.core.host_helpers import SystemdHelper
+from hotsos.core.host_helpers import PebbleHelper, SystemdHelper
 from hotsos.core.plugins.juju.resources import JujuBase
 
 # matches date and time at start if log lines
 JUJU_UNIT_LOGS_TS_EXPR = r"^([\d-]+)\s+([\d:]+)"
 
 SVC_VALID_SUFFIX = r'[0-9a-zA-Z-_]*'
 JUJU_SVC_EXPRS = [r'mongod{}'.format(SVC_VALID_SUFFIX),
@@ -15,14 +15,15 @@
                   r'(?:^|[^\s])juju-db{}'.format(SVC_VALID_SUFFIX)]
 
 
 class JujuChecksBase(plugintools.PluginPartBase, JujuBase):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
+        self.pebble = PebbleHelper(service_exprs=JUJU_SVC_EXPRS)
         self.systemd = SystemdHelper(service_exprs=JUJU_SVC_EXPRS)
         # this is needed for juju scenarios
         self.systemd_processes = self.systemd.processes
 
     @property
     def plugin_runnable(self):
         return os.path.exists(self.juju_lib_path)
```

### Comparing `hotsos-1.1.13.post9/hotsos/core/plugins/juju/resources.py` & `hotsos-1.1.14/hotsos/core/plugins/juju/resources.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/core/plugins/kernel/common.py` & `hotsos-1.1.14/hotsos/core/plugins/kernel/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/core/plugins/kernel/config.py` & `hotsos-1.1.14/hotsos/core/plugins/kernel/config.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/core/plugins/kernel/kernlog/calltrace.py` & `hotsos-1.1.14/hotsos/core/plugins/kernel/kernlog/calltrace.py`

 * *Files 14% similar despite different names*

```diff
@@ -254,14 +254,62 @@
         return len(self.deadlocks)
 
     def __iter__(self):
         for deadlocks in self.deadlocks:
             yield deadlocks
 
 
+class FanotifyDeadlockType(TraceTypeBase):
+
+    def __init__(self):
+        self._search_def = None
+        self.fanotify_hangs = []
+
+    @property
+    def name(self):
+        return 'calltrace-fanotify'
+
+    @property
+    def searchdef(self):
+        if self._search_def:
+            return self._search_def
+
+        start = SearchDef(r'.+ blocked for more than (\d+) seconds.')
+        body = SearchDef(r'(\S+) schedule(\S+) fanotify_handle_event(\S+)'
+                         r' fsnotify(\S+)')
+        end = SearchDef(r'.+\s+do_sys_open(\S+)')
+        self._search_def = SequenceSearchDef(start, tag='fanotify', body=body,
+                                             end=end)
+        return self._search_def
+
+    def apply(self, result):
+        """
+        Run through the results.
+        @param results: list of search.SearchResult objects.
+        """
+        log.debug("%s has %s results", self.__class__.__name__, len(result))
+        if len(result) > 0:
+            # we have found at least one fanotify related hang
+            self.fanotify_hangs.append(True)
+
+    @property
+    def heuristics(self):
+        """
+        Register any heuristics we want to run here.
+        """
+        return []
+
+    def __len__(self):
+        return len(self.fanotify_hangs)
+
+    def __iter__(self):
+        for fanotify_hangs in self.fanotify_hangs:
+            yield fanotify_hangs
+
+
 class OOMKillerTraceType(TraceTypeBase):
 
     def __init__(self):
         self._search_def = None
         self.oom_traces = []
 
     @property
@@ -350,21 +398,69 @@
         return len(self.oom_traces)
 
     def __iter__(self):
         for oom_trace in self.oom_traces:
             yield oom_trace
 
 
+class HungtaskTraceType(TraceTypeBase):
+
+    def __init__(self):
+        self._search_def = None
+        self.hungtasks = []
+
+    @property
+    def name(self):
+        return 'calltrace-hungtask'
+
+    @property
+    def searchdef(self):
+        if self._search_def:
+            return self._search_def
+
+        start = SearchDef(r'.+ blocked for more than (\d+) seconds.')
+        body = SearchDef('.+')
+        end = SearchDef(r'.+\s+do_syscall_(\S+)')
+        self._search_def = SequenceSearchDef(start, tag='hungtask', body=body,
+                                             end=end)
+        return self._search_def
+
+    def apply(self, result):
+        """
+        Run through the results.
+        @param results: list of searchtools.SearchResult objects.
+        """
+        log.debug("%s has %s results", self.__class__.__name__, len(result))
+        if len(result) > 0:
+            # we have found at least one blocked task
+            self.hungtasks.append(True)
+
+    @property
+    def heuristics(self):
+        """
+        Register any heuristics we want to run here.
+        """
+        return []
+
+    def __len__(self):
+        return len(self.hungtasks)
+
+    def __iter__(self):
+        for hungtasks in self.hungtasks:
+            yield hungtasks
+
+
 class CallTraceManager(KernLogBase):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         # All trace types should be registered here.
         self.tracetypes = [GenericTraceType(), OOMKillerTraceType(),
-                           BcacheDeadlockType()]
+                           BcacheDeadlockType(), HungtaskTraceType(),
+                           FanotifyDeadlockType()]
         self.run()
 
     def run(self):
         for tracetype in self.tracetypes:
             self.searcher.add(tracetype.searchdef, self.path)
 
         self.results = self.searcher.run()
```

### Comparing `hotsos-1.1.13.post9/hotsos/core/plugins/kernel/kernlog/common.py` & `hotsos-1.1.14/hotsos/core/plugins/kernel/kernlog/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/core/plugins/kernel/kernlog/events.py` & `hotsos-1.1.14/hotsos/core/plugins/kernel/kernlog/events.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/core/plugins/kernel/memory.py` & `hotsos-1.1.14/hotsos/core/plugins/kernel/memory.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/core/plugins/kernel/net.py` & `hotsos-1.1.14/hotsos/core/plugins/kernel/net.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import abc
 import os
 
+from collections import OrderedDict, UserList
+
 from hotsos.core.log import log
 from hotsos.core.config import HotSOSConfig
-from hotsos.core.host_helpers import SYSCtlFactory
+from hotsos.core.host_helpers import SYSCtlFactory, CLIHelper
+from hotsos.core.search import FileSearcher, SearchDef, ResultFieldInfo
+from hotsos.core.utils import mktemp_dump
+from abc import abstractmethod, abstractproperty
 
 
 class ProcNetBase(abc.ABC):
     """
     Provides a common way to extract fields from /proc/net/snmp and netstat.
 
     Expected file format is:
@@ -390,7 +395,218 @@
             return self._get_field(
                 self._fields[fld][0],
                 self._fields[fld][1]
             )
 
         raise AttributeError("{} not found in {}".
                              format(fld, self.__class__.__name__))
+
+
+class STOVParserBase(UserList):
+
+    def __init__(self):
+        self.data = []
+        self._load()
+
+    @abstractmethod
+    def _load(self):
+        """ Load data from source. """
+
+    @abstractproperty
+    def _search_field_info(self):
+        """
+        Returns a ResultFieldInfo object to make columns addressable by their
+        name as well as mapping them to a specific type.
+        """
+
+    @abstractproperty
+    def _header_matcher(self):
+        """ python.re regular expression to match each header. """
+
+    @abstractproperty
+    def _field_matcher(self):
+        """ python.re regular expression to match each row. """
+
+    @abstractproperty
+    def fields(self):
+        """
+        This is a dictionary of fields exposed by this object along with their
+        type. This provides an opportunity to split/translate fields into sub
+        fields but can also mirror _search_field_info.
+        """
+
+
+class FieldTranslator(object):
+
+    def __init__(self, result, translations):
+        self.result = result
+        self.translations = translations
+
+    def __getattr__(self, key):
+        if key in self.translations:
+            return self.translations[key](self.result)
+
+        return getattr(self.result, key)
+
+
+class Lsof(STOVParserBase):
+    """
+    Provides a way to extract fields from lsof output.
+
+    Expected file format is:
+
+    COMMAND PID USER  FD TYPE DEVICE SIZE/OFF  NODE NAME
+    systemd   1 0 cwd  DIR    9,1     4096     2 /
+    systemd   1 0 rtd  DIR    9,1     4096     2 /
+    systemd   1 0 txt  REG    9,1  1589552 54275 /lib/
+    systemd   1 0 mem  REG    9,1    18976 51133 /lib/
+    /*...*/
+    """
+
+    def _load(self):
+        search = FileSearcher()
+        ftmp = mktemp_dump(''.join(CLIHelper().lsof_Mnlc()))
+        search.add(SearchDef(self._header_matcher, tag='header'), ftmp)
+        search.add(SearchDef(self._field_matcher, tag='content',
+                             field_info=self._search_field_info), ftmp)
+        results = search.run()
+        for r in results.find_by_tag('content'):
+            self.data.append(r)
+
+    def _int_if_numeric(self, value):
+        if value.isnumeric():
+            return int(value)
+
+        return value
+
+    def _strip(self, value):
+        return value.strip()
+
+    @property
+    def _search_field_info(self):
+        finfo = OrderedDict({'COMMAND': str, 'PID': int, 'USER': int,
+                             'FD': str, 'TYPE': str, 'DEVICE': str,
+                             'SIZE/OFF': str,
+                             # NOTE(mkg): Although this column is designated as
+                             #            `inode` number, sockets tend to write
+                             #            L4 protocol name (e.g. TCP) here as
+                             #            well..
+                             'NODE': self._int_if_numeric,
+                             'NAME': self._strip})
+        return ResultFieldInfo(finfo)
+
+    @property
+    def _header_matcher(self):
+        return r'\s+'.join(self._search_field_info.keys())
+
+    @property
+    def _field_matcher(self):
+        expr = []
+        for key, vtype in self._search_field_info.items():
+            if vtype == int:
+                _expr = r'(\d+)'
+            elif key == 'NAME':
+                _expr = r'(\S+\s*\S*)'
+            else:
+                _expr = r'(\S+)'
+
+            # These fields can be empty/None
+            if key in ['TYPE', 'DEVICE', 'SIZE/OFF', 'NODE']:
+                _expr = '{}?'.format(_expr)
+
+            expr.append(_expr)
+
+        return r'\s*' + r'\s+'.join(expr)
+
+    @property
+    def fields(self):
+        """ This has a one-to-one mapping. """
+        return self._search_field_info
+
+    def all_with_inode(self, inode):
+        return list(filter(lambda x: (x.NODE == inode), self.data))
+
+
+class NetLink(STOVParserBase):
+    """
+    Provides a way to extract fields from /proc/net/netlink.
+
+    Expected file format is:
+
+    sk               Eth Pid    Groups   Rmem Wmem Dump Locks Drops Inode
+    0000000000000000 0   23984  00000113 0    0    0    2     0     129906
+    0000000000000000 0   142171 00000113 0    0    0    2     0     411370
+    /*...*/
+    """
+
+    def _load(self):
+        search = FileSearcher()
+        path = os.path.join(HotSOSConfig.data_root, 'proc/net/netlink')
+        search.add(SearchDef(self._header_matcher, tag='header'), path)
+        search.add(SearchDef(self._field_matcher, tag='content',
+                             field_info=self._search_field_info), path)
+        results = search.run()
+        for r in results.find_by_tag('content'):
+            self.data.append(FieldTranslator(r, self.fields))
+
+    @property
+    def _search_field_info(self):
+        finfo = OrderedDict({'sk': int, 'Eth': int, 'Pid': int,
+                             'Groups': str, 'Rmem': int, 'Wmem': int,
+                             'Dump': int, 'Locks': int, 'Drops': int,
+                             'Inode': int})
+        return ResultFieldInfo(finfo)
+
+    @property
+    def _header_matcher(self):
+        return r'\s+'.join(self._search_field_info.keys())
+
+    @property
+    def _field_matcher(self):
+        expr = []
+        for vtype in self._search_field_info.values():
+            if vtype == int:
+                _expr = r'(\d+)'
+            else:
+                _expr = r'(\S+)'
+
+            expr.append(_expr)
+
+        return r'\s*' + r'\s+'.join(expr)
+
+    @property
+    def fields(self):
+        return {
+            # socket pointer addr
+            'sk_addr': lambda result: int(str(getattr(result, 'sk')), 16),
+            # which protocol this socket belongs in this network family
+            'sk_protocol': lambda result: getattr(result, 'sk'),
+            # Netlink port id (Pid)
+            'netlink_port_id': lambda result: getattr(result, 'Pid'),
+            # Netlink groups
+            'netlink_groups': lambda result: int(str(getattr(result,
+                                                             'Groups')), 16),
+            # Allocated rmem for the socket
+            'sk_rmem': lambda result: getattr(result, 'Rmem'),
+            # Allocated wmem for the socket
+            'sk_wmem': lambda result: getattr(result, 'Wmem'),
+            # Netlink dump running?
+            'netlink_dump': lambda result: getattr(result, 'Dump'),
+            # Socket reference count
+            'sk_references': lambda result: getattr(result, 'Locks'),
+            # Dropped packet counter
+            'sk_drops': lambda result: getattr(result, 'Drops'),
+            # Socket's inode number
+            'sk_inode_num': lambda result: getattr(result, 'Inode'),
+        }
+
+    def all_with_drops(self):
+        v = list(filter(lambda x: (x.sk_drops > 0), self.data))
+        if v:
+            # Correlate netlink sockets with process id's by inode
+            # only if there's matching data.
+            lsof = Lsof()
+            for nlsock in v:
+                correlate_result = lsof.all_with_inode(nlsock.sk_inode_num)
+                nlsock.procs = set(
+                    [f"{v.COMMAND}/{v.PID}" for v in correlate_result])
+        return v
```

### Comparing `hotsos-1.1.13.post9/hotsos/core/plugins/kernel/sysfs.py` & `hotsos-1.1.14/hotsos/core/plugins/kernel/sysfs.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/core/plugins/kubernetes.py` & `hotsos-1.1.14/hotsos/core/plugins/kubernetes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 import os
 
 from hotsos.core import plugintools
 from hotsos.core.config import HotSOSConfig
 from hotsos.core.host_helpers import (
     APTPackageHelper,
     HostNetworkingHelper,
+    PebbleHelper,
     SnapPackageHelper,
     SystemdHelper,
 )
 from hotsos.core.utils import cached_property
 
 SERVICES = [r"etcd\S*",
             r"calico\S*",
             r"flannel\S*",
             r"containerd\S*",
             r"dockerd\S*",
             r"kubelet\S*",
             r"kube-\S*",
+            r"microk8s\S*",
             ]
 
 # Packages that only exist in a K8s deployment
 K8S_PACKAGES = [r'cdk-addons',
                 r'helm',
                 r'kubernetes-[\S]+',
                 r'kube-[\S]+',
                 r'kubectl',
                 r'kubelet',
                 r'kubeadm',
                 r'kubefed',
+                r'microk8s'
                 ]
 # Packages that are used in a K8s deployment
 K8S_PACKAGE_DEPS = [r'charm[\S]+',
                     r'docker',
                     r'go',
                     r'vault',
                     r'etcd',
@@ -103,14 +106,15 @@
         super().__init__(*args, **kwargs)
         deps = K8S_PACKAGE_DEPS
         # Deployments can use snap or apt versions of packages so we check both
         self.apt = APTPackageHelper(core_pkgs=K8S_PACKAGES, other_pkgs=deps)
         snap_deps = deps + K8S_PACKAGE_DEPS_SNAP
         self.snaps = SnapPackageHelper(core_snaps=K8S_PACKAGES,
                                        other_snaps=snap_deps)
+        self.pebble = PebbleHelper(service_exprs=SERVICES)
         self.systemd = SystemdHelper(service_exprs=SERVICES)
 
     @property
     def plugin_runnable(self):
         if self.apt.core or self.snaps.core:
             return True
```

### Comparing `hotsos-1.1.13.post9/hotsos/core/plugins/lxd/common.py` & `hotsos-1.1.14/hotsos/core/plugins/lxd/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/core/plugins/maas.py` & `hotsos-1.1.14/hotsos/core/plugins/maas.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/core/plugins/mysql.py` & `hotsos-1.1.14/hotsos/core/plugins/rabbitmq/common.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,39 @@
-import os
-import glob
+from hotsos.core import plugintools
 from hotsos.core.host_helpers import (
     APTPackageHelper,
+    PebbleHelper,
     SystemdHelper,
 )
-from hotsos.core import (
-    host_helpers,
-    plugintools,
-)
-from hotsos.core.config import HotSOSConfig
+from hotsos.core.plugins.rabbitmq.report import RabbitMQReport
 
-SVC_VALID_SUFFIX = r'[0-9a-zA-Z-_]*'
-MYSQL_SVC_EXPRS = [r'mysql{}'.format(SVC_VALID_SUFFIX)]
-CORE_APT = ['mysql']
+RMQ_SERVICES_EXPRS = [
+    r"beam.smp",
+    r"epmd",
+    r"rabbitmq-server",
+]
+RMQ_PACKAGES = [
+    r"rabbitmq-server",
+]
 
 
-class MySQLChecksBase(plugintools.PluginPartBase):
+class RabbitMQBase(object):
 
     def __init__(self, *args, **kwargs):
-        super().__init__()
-        self.apt_info = APTPackageHelper(core_pkgs=CORE_APT)
-        self.systemd = SystemdHelper(service_exprs=MYSQL_SVC_EXPRS)
+        super().__init__(*args, **kwargs)
+        self.report = RabbitMQReport()
 
-    @property
-    def plugin_runnable(self):
-        return self.apt_info.core is not None
 
+class RabbitMQChecksBase(RabbitMQBase, plugintools.PluginPartBase):
 
-class MySQLConfig(host_helpers.SectionalConfigBase):
     def __init__(self, *args, **kwargs):
-        path = os.path.join(HotSOSConfig.data_root,
-                            'etc/mysql/mysql.conf.d/mysqld.cnf')
-        super().__init__(*args, path=path, **kwargs)
-
+        super().__init__(*args, **kwargs)
+        self.apt = APTPackageHelper(core_pkgs=RMQ_PACKAGES)
+        self.pebble = PebbleHelper(service_exprs=RMQ_SERVICES_EXPRS)
+        self.systemd = SystemdHelper(service_exprs=RMQ_SERVICES_EXPRS)
 
-class MySQLRouterConfig(host_helpers.SectionalConfigBase):
-    def __init__(self, *args, **kwargs):
-        path = os.path.join(HotSOSConfig.data_root,
-                            'var/lib/mysql/*mysql-router/mysqlrouter.conf')
-        # expect only one
-        for f in glob.glob(path):
-            path = f
+    @property
+    def plugin_runnable(self):
+        if self.apt.core:
+            return True
 
-        super().__init__(*args, path=path, **kwargs)
+        return False
```

### Comparing `hotsos-1.1.13.post9/hotsos/core/plugins/openstack/common.py` & `hotsos-1.1.14/hotsos/core/plugins/openstack/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from hotsos.core.plugins.openstack.octavia import OctaviaBase
 from hotsos.core.ycheck.events import YEventCheckerBase
 from hotsos.core.host_helpers.cli import CLIHelper, CmdBase
 from hotsos.core.host_helpers import (
     APTPackageHelper,
     DockerImageHelper,
     DPKGVersionCompare,
+    PebbleHelper,
     SystemdHelper,
     SSLCertificate,
     SSLCertificatesHelper,
 )
 
 
 class OpenstackBase(object):
@@ -42,63 +43,56 @@
                             'openstack_https_frontend.conf')
 
     @cached_property
     def ssl_enabled(self):
         return os.path.exists(self.apache2_ssl_config_file)
 
     @cached_property
-    def apache2_certificates_list(self):
-        certificate_path_list = []
-        certificate_list = []
-        if self.ssl_enabled:
-            try:
-                with open(self.apache2_ssl_config_file) as fd:
-                    for line in fd:
-                        regex_match = re.search(r'SSLCertificateFile /(.*)',
-                                                line)
-                        if regex_match:
-                            certificate_path = os.path.join(
-                                               HotSOSConfig.data_root,
-                                               regex_match.group(1))
-                            if certificate_path not in certificate_path_list:
-                                certificate_path_list.append(certificate_path)
-            except OSError:
-                log.debug("Unable to open apache2 configuration file %s",
-                          self.apache2_ssl_config_file)
-                return certificate_list
-
-        if len(certificate_path_list) > 0:
-            for certificate_path in certificate_path_list:
-                try:
-                    ssl_certificate = SSLCertificate(certificate_path)
-                    certificate_list.append(ssl_certificate)
-                except OSError:
-                    continue
+    def _apache2_certificates(self):
+        """ Returns list of ssl cert paths relative to data_root. """
+        certificate_paths = []
+        if not self.ssl_enabled:
+            return certificate_paths
+
+        with open(self.apache2_ssl_config_file) as fd:
+            for line in fd:
+                ret = re.search(r'SSLCertificateFile /(\S+)', line)
+                if ret:
+                    path = ret.group(1)
+                    if path not in certificate_paths:
+                        certificate_paths.append(path)
 
-        return certificate_list
+            return certificate_paths
 
     @cached_property
     def apache2_certificates_expiring(self):
         apache2_certificates_expiring = []
-        certificate_list = self.apache2_certificates_list
-        for certificate in certificate_list:
-            ssl_checks = SSLCertificatesHelper(certificate,
-                                               self.certificate_expire_days)
+        max_days = self.certificate_expire_days
+        for path in self._apache2_certificates:
+            try:
+                ssl_checks = SSLCertificatesHelper(SSLCertificate(path),
+                                                   max_days)
+            except OSError:
+                log.info("cert path not found: %s", path)
+                continue
+
             if ssl_checks.certificate_expires_soon:
-                apache2_certificates_expiring.append(certificate.path)
+                apache2_certificates_expiring.append(path)
+
         return apache2_certificates_expiring
 
 
 class OpenstackChecksBase(OpenstackBase, plugintools.PluginPartBase):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.ost_projects = OSTProjectCatalog()
-        self.systemd = SystemdHelper(
-                           service_exprs=self.ost_projects.service_exprs)
+        service_exprs = self.ost_projects.service_exprs
+        self.pebble = PebbleHelper(service_exprs=service_exprs)
+        self.systemd = SystemdHelper(service_exprs=service_exprs)
         self.apt = APTPackageHelper(
                        core_pkgs=self.ost_projects.packages_core_exprs,
                        other_pkgs=self.ost_projects.packages_dep_exprs)
         self.docker = DockerImageHelper(
                           core_pkgs=self.ost_projects.packages_core_exprs,
                           other_pkgs=self.ost_projects.packages_dep_exprs)
 
@@ -178,15 +172,15 @@
         return relname
 
     @cached_property
     def days_to_eol(self):
         if self.release_name != 'unknown':
             eol = OST_EOL_INFO.get(self.release_name)
             if eol is not None:
-                today = datetime.fromtimestamp(int(CLIHelper().date()))
+                today = datetime.utcfromtimestamp(int(CLIHelper().date()))
                 delta = (eol - today).days
                 return delta
             else:
                 log.warning("unable to determine eol info for unknown release "
                             "name '%s'", self.release_name)
 
     @property
@@ -217,15 +211,15 @@
         expect to be masked filtered out.
         """
         masked = set(self.systemd.masked_services)
         if not masked:
             return []
 
         expected_masked = self.ost_projects.default_masked_services
-        return list(masked.difference(expected_masked))
+        return sorted(list(masked.difference(expected_masked)))
 
     @cached_property
     def openstack_installed(self):
         if self.apt.core:
             return True
 
         return False
```

### Comparing `hotsos-1.1.13.post9/hotsos/core/plugins/openstack/exceptions.py` & `hotsos-1.1.14/hotsos/core/plugins/openstack/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,33 +26,33 @@
 #    "FutureWarning",
 #    "GeneratorExit",
     "ImportError",
     "ImportWarning",
 #    "IndentationError",
     "IndexError",
     "InterruptedError",
-#    "IOError",
+    "IOError",
     "IsADirectoryError",
 #    "KeyboardInterrupt",
     "KeyError",
     "LookupError",
     "MemoryError",
-#    "ModuleNotFoundError",
+    "ModuleNotFoundError",
     "NameError",
 #    "NotADirectoryError",
     "NotImplementedError",
-#    "OSError",
+    "OSError",
     "OverflowError",
 #    "PendingDeprecationWarning",
     "PermissionError",
     "ProcessLookupError",
     "RecursionError",
     "ReferenceError",
     "ResourceWarning",
-#    "RuntimeError",
+    "RuntimeError",
 #    "RuntimeWarning",
 #    "StopAsyncIteration",
 #    "StopIteration",
     "SyntaxError",
 #    "SyntaxWarning",
     "SystemError",
     "SystemExit",
```

### Comparing `hotsos-1.1.13.post9/hotsos/core/plugins/openstack/neutron.py` & `hotsos-1.1.14/hotsos/core/plugins/openstack/neutron.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import os
 import re
 
 from hotsos.core.config import HotSOSConfig
-from hotsos.core.plugins.openstack.openstack import OSTServiceBase
+from hotsos.core.plugins.openstack.openstack import (
+    OpenstackConfig,
+    OSTServiceBase,
+)
 from hotsos.core.host_helpers import CLIHelper
 from hotsos.core.utils import cached_property
+from hotsos.core.factory import FactoryBase
 
 
 class NeutronBase(OSTServiceBase):
 
     def __init__(self, *args, **kwargs):
         super().__init__('neutron', *args, **kwargs)
         self.neutron_ovs_config = self.project.config['openvswitch-agent']
@@ -111,7 +115,14 @@
 
         return _routers
 
     def find_router_with_vr_id(self, id):
         for r in self.ha_routers:
             if r.vr_id == id:
                 return r
+
+
+class Config(FactoryBase):
+
+    def __getattr__(self, path):
+        path = os.path.join(HotSOSConfig.data_root, 'etc/neutron', path)
+        return OpenstackConfig(path)
```

### Comparing `hotsos-1.1.13.post9/hotsos/core/plugins/openstack/nova.py` & `hotsos-1.1.14/hotsos/core/plugins/openstack/nova.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/core/plugins/openstack/octavia.py` & `hotsos-1.1.14/hotsos/core/plugins/openstack/octavia.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/core/plugins/openstack/openstack.py` & `hotsos-1.1.14/hotsos/core/plugins/openstack/openstack.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from datetime import datetime
 import os
 
 from hotsos.core import host_helpers
+from hotsos.core.log import log
 from hotsos.core.config import HotSOSConfig
 from hotsos.core.plugins.openstack.exceptions import (
     EXCEPTIONS_COMMON,
     BARBICAN_EXCEPTIONS,
     CASTELLAN_EXCEPTIONS,
     CINDER_EXCEPTIONS,
     DESIGNATE_EXCEPTIONS,
@@ -41,112 +42,113 @@
     'rocky': datetime(2020, 2, 29),
     'queens': datetime(2028, 4, 30),
     'mitaka': datetime(2024, 4, 30)
 }
 
 
 OST_REL_INFO = {
+    'aodh-common': {
+        'antelope': '1:16.0.0',
+        'zed': '1:15.0.0',
+        'yoga': '1:14.0.0',
+        'xena': '1:13.0.0',
+        'wallaby': '1:12.0.0',
+        'victoria': '11.0.0',
+        'ussuri': '10.0.0',
+        'train': '9.0.0',
+        'stein': '8.0.0',
+        'rocky': '7.0.0',
+        'queens': '6.0.0'},
     'barbican-common': {
+        'antelope': '2:16.0.0',
         'zed': '2:15.0.0',
         'yoga': '2:14.0.0',
         'xena': '1:13.0.0',
         'wallaby': '1:12.0.0',
         'victoria': '1:11.0.0',
         'ussuri': '1:10.0.0',
         'train': '1:9.0.0',
         'stein': '1:8.0.0',
         'rocky': '1:7.0.0',
         'queens': '1:6.0.0'},
     'cinder-common': {
+        'antelope': '2:22.0.0',
         'zed': '2:21.0.0',
         'yoga': '2:20.0.0',
         'xena': '2:19.0.0',
         'wallaby': '2:18.0.0',
         'victoria': '2:17.0.0',
         'ussuri': '2:16.0.0',
         'train': '2:15.0.0',
         'stein': '2:14.0.0',
         'rocky': '2:13.0.0',
         'queens': '2:12.0.0'},
     'designate-common': {
+        'antelope': '1:16.0.0',
         'zed': '1:15.0.0',
         'yoga': '1:14.0.0',
         'xena': '1:13.0.0',
         'wallaby': '1:12.0.0',
         'victoria': '1:11.0.0',
         'ussuri': '1:10.0.0',
         'train': '1:9.0.0',
         'stein': '1:8.0.0',
         'rocky': '1:7.0.0',
         'queens': '1:6.0.0'},
     'glance-common': {
+        'antelope': '2:26.0.0',
         'zed': '2:25.0.0',
         'yoga': '2:24.0.0',
         'xena': '2:23.0.0',
         'wallaby': '2:22.0.0',
         'victoria': '2:21.0.0',
         'ussuri': '2:20.0.0',
         'train': '2:19.0.0',
         'stein': '2:18.0.0',
         'rocky': '2:17.0.0',
         'queens': '2:16.0.0'},
     'heat-common': {
+        'antelope': '1:20.0.0',
         'zed': '1:19.0.0',
         'yoga': '1:18.0.0',
         'xena': '1:17.0.0',
         'wallaby': '1:16.0.0',
         'victoria': '1:15.0.0',
         'ussuri': '1:14.0.0',
         'train': '1:13.0.0',
         'stein': '1:12.0.0',
         'rocky': '1:11.0.0',
         'queens': '1:10.0.0'},
     'keystone': {
+        'antelope': '2:23.0.0',
         'zed': '2:22.0.0',
         'yoga': '2:21.0.0',
         'xena': '2:20.0.0',
         'wallaby': '2:19.0.0',
         'victoria': '2:18.0.0',
         'ussuri': '2:17.0.0',
         'train': '2:16.0.0',
         'stein': '2:15.0.0',
         'rocky': '2:14.0.0',
         'queens': '2:13.0.0',
         'pike': '2:12.0.0',
         'ocata': '2:11.0.0'},
-    'nova-common': {
-        'zed': '3:26.0.0',
-        'yoga': '3:25.0.0',
-        'xena': '3:24.0.0',
-        'wallaby': '3:23.0.0',
-        'victoria': '2:22.0.0',
-        'ussuri': '2:21.0.0',
-        'train': '2:20.0.0',
-        'stein': '2:19.0.0',
-        'rocky': '2:18.0.0',
-        'queens': '2:17.0.0',
-        'pike': '2:16.0.0',
-        'ocata': '2:15.0.0',
-        'newton': '2:14.0.0',
-        'mitaka': '2:13.0.0',
-        'liberty': '2:12.0.0',
-        'kilo': '1:2015.1.0',
-        'juno': '1:2014.2.0',
-        'icehouse': '1:2014.1.0'},
     'masakari-common': {
+        'antelope': '15.0.0',
         'zed': '14.0.0',
         'yoga': '13.0.0',
         'xena': '12.0.0',
         'wallaby': '11.0.0',
         'victoria': '10.0.0',
         'ussuri': '9.0.0',
         'train': '8.0.0',
         'stein': '7.0.0',
         'rocky': '6.0.0'},
     'neutron-common': {
+        'antelope': '2:22.0.0',
         'zed': '2:21.0.0',
         'yoga': '2:20.0.0',
         'xena': '2:19.0.0',
         'wallaby': '2:18.0.0',
         'victoria': '2:17.0.0',
         'ussuri': '2:16.0.0',
         'train': '2:15.0.0',
@@ -157,35 +159,67 @@
         'ocata': '2:10.0.0',
         'newton': '2:9.0.0',
         'mitaka': '2:8.0.0',
         'liberty': '2:7.0.0',
         'kilo': '1:2015.1.0',
         'juno': '1:2014.2.0',
         'icehouse': '1:2014.1.0'},
+    'nova-common': {
+        'antelope': '3:27.0.0',
+        'zed': '3:26.0.0',
+        'yoga': '3:25.0.0',
+        'xena': '3:24.0.0',
+        'wallaby': '3:23.0.0',
+        'victoria': '2:22.0.0',
+        'ussuri': '2:21.0.0',
+        'train': '2:20.0.0',
+        'stein': '2:19.0.0',
+        'rocky': '2:18.0.0',
+        'queens': '2:17.0.0',
+        'pike': '2:16.0.0',
+        'ocata': '2:15.0.0',
+        'newton': '2:14.0.0',
+        'mitaka': '2:13.0.0',
+        'liberty': '2:12.0.0',
+        'kilo': '1:2015.1.0',
+        'juno': '1:2014.2.0',
+        'icehouse': '1:2014.1.0'},
     'octavia-common': {
+        'antelope': '1:12.0.0',
         'zed': '1:11.0.0',
         'yoga': '1:10.0.0',
         'xena': '1:9.0.0',
         'wallaby': '1:8.0.0',
         'victoria': '7.0.0',
         'ussuri': '6.0.0',
         'train': '5.0.0',
         'stein': '4.0.0',
         'rocky': '3.0.0'},
     'openstack-dashboard-common': {
+        'antelope': '4:23.1.0',
         'zed': '4:22.2.0',
         'yoga': '4:22.0.0',
         'xena': '4:20.0.0',
         'wallaby': '4:19.0.0',
         'victoria': '4:18.0.0',
         'ussuri': '3:18.0.0',
         'train': '3:16.0.0',
         'stein': '3:15.0.0',
         'rocky': '3:14.0.0',
-        'queens': '3:13.0.0'}
+        'queens': '3:13.0.0'},
+    'placement-common': {
+        'antelope': '1:9.0.0',
+        'zed': '1:8.0.0',
+        'yoga': '1:7.0.0',
+        'xena': '1:6.0.0',
+        'wallaby': '1:5.0.0',
+        'victoria': '4.0.0',
+        'ussuri': '3.0.0',
+        'train': '2.0.0',
+        'stein': '1.0.0'}
     }
 
 OST_EXCEPTIONS = {'barbican': BARBICAN_EXCEPTIONS + CASTELLAN_EXCEPTIONS,
                   'cinder': CINDER_EXCEPTIONS + CASTELLAN_EXCEPTIONS,
                   'designate': DESIGNATE_EXCEPTIONS,
                   'glance': GLANCE_EXCEPTIONS + GLANCE_STORE_EXCEPTIONS,
                   'heat': HEAT_EXCEPTIONS,
@@ -199,15 +233,17 @@
                   'placement': PLACEMENT_EXCEPTIONS,
                   }
 
 OPENSTACK_LOGS_TS_EXPR = r"^([\d-]+\s+[\d:]+)"
 
 
 class OpenstackConfig(host_helpers.SectionalConfigBase):
-    pass
+
+    def __getattr__(self, key):
+        return self.get(key)
 
 
 class OSTProject(object):
     SVC_VALID_SUFFIX = r'[0-9a-zA-Z-_]*'
     PY_CLIENT_PREFIX = r"python3?-{}\S*"
 
     def __init__(self, name, config=None, apt_core_alt=None,
@@ -271,14 +307,19 @@
             exprs += self.systemd_extra_services
         return exprs
 
     @cached_property
     def services(self):
         exprs = self.services_expr
         info = host_helpers.SystemdHelper(service_exprs=exprs)
+        if not info.services:
+            log.debug("no systemd services found for '%s' - trying pebble",
+                      self.name)
+            info = host_helpers.PebbleHelper(service_exprs=exprs)
+
         return info.services
 
     def log_paths(self, include_deprecated_services=True):
         """
         Returns tuples of daemon name, log path for each agent/daemon.
         """
         proj_manage = "{}-manage".format(self.name)
@@ -430,15 +471,15 @@
         Returns a list of services that are expected to be marked as masked in
         systemd.
         """
         masked = []
         for p in self.all.values():
             masked += p.systemd_masked_services
 
-        return masked
+        return sorted(masked)
 
     def add(self, name, *args, **kwargs):
         self._projects[name] = OSTProject(name, *args, **kwargs)
 
     @cached_property
     def packages_core_exprs(self):
         core = set()
```

### Comparing `hotsos-1.1.13.post9/hotsos/core/plugins/openvswitch/common.py` & `hotsos-1.1.14/hotsos/core/plugins/openvswitch/common.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 from hotsos.core import plugintools
-from hotsos.core.host_helpers import APTPackageHelper, SystemdHelper
+from hotsos.core.host_helpers import (
+    APTPackageHelper,
+    PebbleHelper,
+    SystemdHelper,
+)
 from hotsos.core.ycheck.events import YEventCheckerBase
 from hotsos.core.utils import cached_property, sorted_dict
 
 OVS_SERVICES_EXPRS = [r'ovsdb[a-zA-Z-]*',
                       r'ovs-vswitch[a-zA-Z-]*',
                       r'ovn[a-zA-Z-]*',
                       'openvswitch-switch',
@@ -26,14 +30,15 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         p_core = OVS_PKGS_CORE + [PY_CLIENT_PREFIX.format(p)
                                   for p in OVS_PKGS_CORE]
         p_deps = OVS_PKGS_DEPS + [PY_CLIENT_PREFIX.format(p)
                                   for p in OVS_PKGS_DEPS]
         self.apt = APTPackageHelper(core_pkgs=p_core, other_pkgs=p_deps)
+        self.pebble = PebbleHelper(service_exprs=OVS_SERVICES_EXPRS)
         self.systemd = SystemdHelper(service_exprs=OVS_SERVICES_EXPRS)
 
     @cached_property
     def apt_packages_all(self):
         return self.apt.all
 
     @property
```

### Comparing `hotsos-1.1.13.post9/hotsos/core/plugins/openvswitch/ovn.py` & `hotsos-1.1.14/hotsos/core/plugins/openvswitch/ovn.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/core/plugins/openvswitch/ovs.py` & `hotsos-1.1.14/hotsos/core/plugins/openvswitch/ovs.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/core/plugins/pacemaker.py` & `hotsos-1.1.14/hotsos/core/plugins/pacemaker.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/core/plugins/rabbitmq/common.py` & `hotsos-1.1.14/hotsos/core/plugins/vault.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,30 @@
-from hotsos.core import plugintools
-from hotsos.core.host_helpers import APTPackageHelper, SystemdHelper
-from hotsos.core.plugins.rabbitmq.report import RabbitMQReport
-
-RMQ_SERVICES_EXPRS = [
-    r"beam.smp",
-    r"epmd",
-    r"rabbitmq-server",
-]
-RMQ_PACKAGES = [
-    r"rabbitmq-server",
-]
+from hotsos.core.plugintools import PluginPartBase
+from hotsos.core.host_helpers import (
+    PebbleHelper,
+    SnapPackageHelper,
+    SystemdHelper,
+)
+from hotsos.core.utils import cached_property
 
+CORE_SNAPS = ['vault']
+SERVICE_EXPRS = [s + '[A-Za-z0-9-]*' for s in CORE_SNAPS]
 
-class RabbitMQBase(object):
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.report = RabbitMQReport()
 
-
-class RabbitMQChecksBase(RabbitMQBase, plugintools.PluginPartBase):
+class VaultChecksBase(PluginPartBase):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.apt = APTPackageHelper(core_pkgs=RMQ_PACKAGES)
-        self.systemd = SystemdHelper(service_exprs=RMQ_SERVICES_EXPRS)
-
-    @property
-    def plugin_runnable(self):
-        if self.apt.core:
+        self.snaps = SnapPackageHelper(core_snaps=CORE_SNAPS)
+        self.systemd = SystemdHelper(service_exprs=SERVICE_EXPRS)
+        self.pebble = PebbleHelper(service_exprs=SERVICE_EXPRS)
+
+    @cached_property
+    def vault_installed(self):
+        if self.snaps.core:
             return True
 
         return False
+
+    @property
+    def plugin_runnable(self):
+        return self.vault_installed
```

### Comparing `hotsos-1.1.13.post9/hotsos/core/plugins/rabbitmq/report.py` & `hotsos-1.1.14/hotsos/core/plugins/rabbitmq/report.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/core/plugins/sosreport.py` & `hotsos-1.1.14/hotsos/core/plugins/sosreport.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/core/plugins/storage/bcache.py` & `hotsos-1.1.14/hotsos/core/plugins/storage/bcache.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/core/plugins/storage/ceph.py` & `hotsos-1.1.14/hotsos/core/plugins/storage/ceph.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,26 +16,28 @@
 from hotsos.core.config import HotSOSConfig
 from hotsos.core.ycheck.events import YEventCheckerBase
 from hotsos.core.host_helpers import (
     APTPackageHelper,
     CLIHelper,
     DPKGVersionCompare,
     HostNetworkingHelper,
+    PebbleHelper,
     SystemdHelper,
     SectionalConfigBase,
-    SVC_EXPR_TEMPLATES,
 )
 from hotsos.core.host_helpers.cli import get_ps_axo_flags_available
 from hotsos.core.plugins.storage import StorageBase
 from hotsos.core.plugins.storage.bcache import BcacheBase
 from hotsos.core.search import (
     FileSearcher,
     SequenceSearchDef,
     SearchDef
 )
+from hotsos.core.plugins.kernel.net import Lsof
+
 
 CEPH_LOGS_TS_EXPR = r"^([\d-]+)[\sT]([\d:]+)"
 CEPH_SERVICES_EXPRS = [r"ceph-[a-z0-9-]+",
                        r"rados[a-z0-9-:]+"]
 CEPH_PKGS_CORE = [r"ceph",
                   r"rados",
                   r"rbd",
@@ -312,14 +314,29 @@
     def autoscaler_disabled_pools(self):
         if not self.ceph_report:
             return []
 
         pools = self.ceph_report['osdmap']['pools']
         return [p for p in pools if p.get('pg_autoscale_mode') != 'on']
 
+    @cached_property
+    def is_rgw_using_civetweb(self):
+        if not self.ceph_report:
+            return []
+
+        try:
+            rgws = self.ceph_report['servicemap']['services']['rgw']['daemons']
+            for _, outer_d in rgws.items():
+                if isinstance(outer_d, dict):
+                    if outer_d['metadata']['frontend_type#0'] == 'civetweb':
+                        return True
+        except(ValueError, KeyError):
+            pass
+        return False
+
 
 class CephCluster(object):
     OSD_META_LIMIT_PERCENT = 5
     OSD_PG_MAX_LIMIT = 500
     OSD_PG_OPTIMAL_NUM_MAX = 200
     OSD_PG_OPTIMAL_NUM_MIN = 50
     # If a pool's utilisation is below this value, we consider is "empty"
@@ -637,15 +654,16 @@
             if daemon_type == 'overall':
                 continue
 
             if exclude_daemons:
                 if daemon_type in exclude_daemons:
                     continue
 
-            unique_versions[daemon_type] = list(set(versions[daemon_type]))
+            unique_versions[daemon_type] = sorted(
+                list(set(versions[daemon_type])))
 
         return unique_versions
 
     @cached_property
     def ceph_versions_aligned(self):
         versions = self.ceph_daemon_versions_unique()
         if not versions:
@@ -789,15 +807,15 @@
         ps_info = []
         daemon = "ceph-{}".format(self.daemon_type)
         for line in self.cli.ps_axo_flags():
             ret = re.compile(daemon).search(line)
             if not ret:
                 continue
 
-            expt_tmplt = SVC_EXPR_TEMPLATES["absolute"]
+            expt_tmplt = SystemdHelper.PS_CMD_EXPR_TEMPLATES['absolute']
             ret = re.compile(expt_tmplt.format(daemon)).search(line)
             if ret:
                 ps_info.append(ret.group(0))
 
         if not ps_info:
             return
 
@@ -877,17 +895,19 @@
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.ceph_config = CephConfig()
         self.bcache = BcacheBase()
         self.apt = APTPackageHelper(core_pkgs=CEPH_PKGS_CORE,
                                     other_pkgs=CEPH_PKGS_OTHER)
+        self.pebble = PebbleHelper(service_exprs=CEPH_SERVICES_EXPRS)
         self.systemd = SystemdHelper(service_exprs=CEPH_SERVICES_EXPRS)
         self.cluster = CephCluster()
         self.cli = CLIHelper()
+        self.lsof = Lsof()
 
     @property
     def summary_subkey(self):
         return 'ceph'
 
     @property
     def plugin_runnable(self):
@@ -911,15 +931,15 @@
 
         return relname
 
     @cached_property
     def days_to_eol(self):
         if self.release_name != 'unknown':
             eol = CEPH_EOL_INFO[self.release_name]
-            today = datetime.fromtimestamp(int(CLIHelper().date()))
+            today = datetime.utcfromtimestamp(int(CLIHelper().date()))
             delta = (eol - today).days
             return delta
 
     def _get_bind_interfaces(self, type):
         """
         For the given config network type determine what interface ceph is
         binding to.
@@ -1056,14 +1076,31 @@
         for port in self.bind_interfaces.values():
             for stats in port.stats.values():
                 if stats.get('errors'):
                     return True
 
         return False
 
+    @cached_property
+    def linked_with_tcmalloc(self):
+        """
+        Checks that each ceph-osd process has libtcmalloc linked.
+
+        Returns True if every OSD has it linked, otherwise False.
+        """
+        osds = {}
+        tcmalloc_osds = 0
+        for row in self.lsof:
+            if row.COMMAND == 'ceph-osd':
+                osds[row.PID] = 1
+                if re.search("libtcmalloc", row.NAME):
+                    tcmalloc_osds += 1
+
+        return len(osds) == tcmalloc_osds
+
 
 class CephDaemonCommand(object):
     """
     This class is used to run a ceph daemon command that must be supported by
     CLIHelper. Attributes of the output can then be retrieved by calling them
     on the returned object.
     """
```

### Comparing `hotsos-1.1.13.post9/hotsos/core/plugins/system/system.py` & `hotsos-1.1.14/hotsos/core/plugins/system/system.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/core/plugintools.py` & `hotsos-1.1.14/hotsos/core/plugintools.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/core/search.py` & `hotsos-1.1.14/hotsos/core/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 
 from searchkit import (   # noqa: F403,F401, pylint: disable=W0611
     FileSearcher as _FileSearcher,
+    ResultFieldInfo,
     SearchDef,
     SequenceSearchDef,
 )
 from searchkit.constraints import (
     SearchConstraintSearchSince as _SearchConstraintSearchSince
 )
 
@@ -31,14 +32,15 @@
 
             kwargs['days'] = days
 
         current_date = CLIHelper().date(format='+%Y-%m-%d %H:%M:%S')
         if not current_date or type(current_date) != str:
             log.error("current date '%s' being provided to search "
                       "constraints is not valid.", current_date)
+            return
 
         super().__init__(*args,
                          current_date=current_date,
                          cache_path=HotSOSConfig.plugin_tmp_dir,
                          allow_constraints_for_unverifiable_logs=HotSOSConfig.
                          allow_constraints_for_unverifiable_logs,
                          **kwargs)
```

### Comparing `hotsos-1.1.13.post9/hotsos/core/utils.py` & `hotsos-1.1.14/hotsos/core/utils.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/core/ycheck/engine/common.py` & `hotsos-1.1.14/hotsos/core/ycheck/engine/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/core/ycheck/engine/properties/checks.py` & `hotsos-1.1.14/hotsos/core/ycheck/engine/properties/checks.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/core/ycheck/engine/properties/common.py` & `hotsos-1.1.14/hotsos/core/ycheck/engine/properties/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/core/ycheck/engine/properties/conclusions.py` & `hotsos-1.1.14/hotsos/core/ycheck/engine/properties/conclusions.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/core/ycheck/engine/properties/input.py` & `hotsos-1.1.14/hotsos/core/ycheck/engine/properties/input.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/core/ycheck/engine/properties/requires/common.py` & `hotsos-1.1.14/hotsos/core/ycheck/engine/properties/requires/common.py`

 * *Files 16% similar despite different names*

```diff
@@ -189,7 +189,55 @@
 
     @property
     def ops(self):
         if type(self.content) != dict:
             return self.default_ops
 
         return self.content.get('ops', self.default_ops)
+
+
+class ServiceCheckItemsBase(CheckItemsBase):
+
+    @cached_property
+    def _started_after_services(self):
+        svcs = []
+        for _, settings in self:
+            if type(settings) != dict:
+                continue
+
+            svc = settings.get('started-after')
+            if svc:
+                svcs.append(svc)
+
+        return svcs
+
+    @cached_property
+    def _services_to_check(self):
+        return [item[0] for item in self]
+
+    @property
+    def _svcs_all(self):
+        """
+        We include started-after services since if a check has specified one it
+        is expected to exist for that check to pass.
+        """
+        return self._services_to_check + self._started_after_services
+
+    @property
+    @abc.abstractmethod
+    def _svcs_info(self):
+        """ ServiceManagerBase implementation with _svcs_all as input. """
+
+    @cached_property
+    def not_installed(self):
+        _installed = self.installed.keys()
+        return set(_installed).symmetric_difference(self._svcs_all)
+
+    @cached_property
+    def installed(self):
+        return self._svcs_info.services
+
+    def processes_running(self, processes):
+        """ Check any processes provided. """
+        a = set(processes)
+        b = set(self._svcs_info.processes.keys())
+        return a.issubset(b)
```

### Comparing `hotsos-1.1.13.post9/hotsos/core/ycheck/engine/properties/requires/requires.py` & `hotsos-1.1.14/hotsos/core/ycheck/engine/properties/requires/requires.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     LogicalCollectionHandler,
     add_to_property_catalog,
 )
 from hotsos.core.ycheck.engine.properties.requires.types import (
     apt,
     snap,
     config,
+    pebble,
     systemd,
     property as rproperty,
     path,
     varops,
 )
 
 
@@ -19,14 +20,15 @@
                             LogicalCollectionHandler):
 
     @classmethod
     def _override_mapped_member_types(cls):
         return [apt.YRequirementTypeAPT,
                 snap.YRequirementTypeSnap,
                 config.YRequirementTypeConfig,
+                pebble.YRequirementTypePebble,
                 systemd.YRequirementTypeSystemd,
                 rproperty.YRequirementTypeProperty,
                 path.YRequirementTypePath,
                 varops.YPropertyVarOps]
 
     def get_item_result_callback(self, item, is_default_group=False):
         result = item()
```

### Comparing `hotsos-1.1.13.post9/hotsos/core/ycheck/engine/properties/requires/types/apt.py` & `hotsos-1.1.14/hotsos/core/ycheck/engine/properties/requires/types/apt.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,37 +23,41 @@
         for p in self.installed:
             _versions.append(self.packaging_helper.get_version(p))
 
         return _versions
 
     def package_version_within_ranges(self, pkg, versions):
         result = False
-        version = self.packaging_helper.get_version(pkg)
-        for item in sorted(versions, key=lambda i: i['max'],
-                           reverse=True):
-            v_max = str(item['max'])
+        versions = sorted(versions, key=lambda i: i['min'], reverse=True)
+        pkg_version = self.packaging_helper.get_version(pkg)
+        for item in versions:
             v_min = str(item['min'])
-            lte_max = version <= DPKGVersionCompare(v_max)
+            if 'max' in item:
+                v_max = str(item['max'])
+                lte_max = pkg_version <= DPKGVersionCompare(v_max)
+            else:
+                lte_max = True
+
             if v_min:
-                lt_broken = version < DPKGVersionCompare(v_min)
+                lt_broken = pkg_version < DPKGVersionCompare(v_min)
             else:
                 lt_broken = None
 
             if lt_broken:
                 continue
 
             if lte_max:
                 result = True
             else:
                 result = False
 
             break
 
         log.debug("package %s=%s within version ranges %s "
-                  "(result=%s)", pkg, version, versions, result)
+                  "(result=%s)", pkg, pkg_version, versions, result)
         return result
 
 
 class YRequirementTypeAPT(YRequirementTypeBase):
     """ Provides logic to perform checks on APT packages. """
 
     @classmethod
```

### Comparing `hotsos-1.1.13.post9/hotsos/core/ycheck/engine/properties/requires/types/config.py` & `hotsos-1.1.14/hotsos/core/ycheck/engine/properties/requires/types/config.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/core/ycheck/engine/properties/requires/types/path.py` & `hotsos-1.1.14/hotsos/core/ycheck/engine/properties/requires/types/path.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/core/ycheck/engine/properties/requires/types/property.py` & `hotsos-1.1.14/hotsos/core/ycheck/engine/properties/requires/types/property.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/core/ycheck/engine/properties/requires/types/snap.py` & `hotsos-1.1.14/hotsos/core/ycheck/engine/properties/requires/types/snap.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/core/ycheck/engine/properties/requires/types/systemd.py` & `hotsos-1.1.14/hotsos/core/ycheck/engine/properties/requires/types/systemd.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,65 +1,24 @@
 from datetime import timedelta
 
 from hotsos.core.log import log
 from hotsos.core.host_helpers import SystemdHelper
 from hotsos.core.ycheck.engine.properties.requires import (
     intercept_exception,
-    CheckItemsBase,
+    ServiceCheckItemsBase,
     YRequirementTypeBase,
 )
-from hotsos.core.utils import cached_property
 
 
-class ServiceCheckItems(CheckItemsBase):
-
-    @cached_property
-    def _started_after_services(self):
-        svcs = []
-        for _, settings in self:
-            if type(settings) != dict:
-                continue
-
-            svc = settings.get('started-after')
-            if svc:
-                svcs.append(svc)
-
-        return svcs
-
-    @cached_property
-    def _services_to_check(self):
-        return [item[0] for item in self]
+class SystemdServiceCheckItems(ServiceCheckItemsBase):
 
     @property
-    def _svcs_all(self):
-        """
-        We include started-after services since if a check has specified one it
-        is expected to exist for that check to pass.
-        """
-        return self._services_to_check + self._started_after_services
-
-    @cached_property
     def _svcs_info(self):
         return SystemdHelper(self._svcs_all)
 
-    @cached_property
-    def not_installed(self):
-        _installed = self.installed.keys()
-        return set(_installed).symmetric_difference(self._svcs_all)
-
-    @cached_property
-    def installed(self):
-        return self._svcs_info.services
-
-    def processes_running(self, processes):
-        """ Check any processes provided. """
-        a = set(processes)
-        b = set(self._svcs_info.processes.keys())
-        return a.issubset(b)
-
 
 class YRequirementTypeSystemd(YRequirementTypeBase):
     """ Provides logic to perform checks on systemd resources. """
 
     @classmethod
     def _override_keys(cls):
         return ['systemd']
@@ -114,15 +73,15 @@
     @property
     @intercept_exception
     def _result(self):
         cache_info = {}
         default_op = 'eq'
         _result = True
 
-        items = ServiceCheckItems(self.content)
+        items = SystemdServiceCheckItems(self.content)
         if not items.not_installed:
             for svc, settings in items:
                 svc_obj = items.installed[svc]
                 cache_info[svc] = {'actual': svc_obj.state}
                 if settings is None:
                     continue
```

### Comparing `hotsos-1.1.13.post9/hotsos/core/ycheck/engine/properties/requires/types/varops.py` & `hotsos-1.1.14/hotsos/core/ycheck/engine/properties/requires/types/varops.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/core/ycheck/engine/properties/search.py` & `hotsos-1.1.14/hotsos/core/ycheck/engine/properties/search.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/core/ycheck/engine/properties/vars.py` & `hotsos-1.1.14/hotsos/core/ycheck/engine/properties/vars.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/core/ycheck/events.py` & `hotsos-1.1.14/hotsos/core/ycheck/events.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/core/ycheck/scenarios.py` & `hotsos-1.1.14/hotsos/core/ycheck/scenarios.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/events/openstack/neutron/agents.yaml` & `hotsos-1.1.14/hotsos/defs/events/openstack/neutron/agents.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/events/openstack/nova/external-events.yaml` & `hotsos-1.1.14/hotsos/defs/events/openstack/nova/external-events.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/events/openvswitch/ovn/errors-and-warnings.yaml` & `hotsos-1.1.14/hotsos/defs/events/openvswitch/ovn/errors-and-warnings.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ovsdb-server-sb:
   input:
     path: 'var/log/ovn/ovsdb-server-sb.log'
-  hint: '(ERR|WARN)'
-  expr: '([0-9-]+)T[0-9:\.]+Z.+\|(ERR|ERROR|WARN)\|.+'
+  hint: '(ERR|WARN|EMER)'
+  expr: '([0-9-]+)T[0-9:\.]+Z.+\|(ERR|ERROR|WARN|EMER)\|.+'
 ovsdb-server-nb:
   input:
     path: 'var/log/ovn/ovsdb-server-nb.log'
-  hint: '(ERR|WARN)'
-  expr: '([0-9-]+)T[0-9:\.]+Z.+\|(ERR|ERROR|WARN)\|.+'
+  hint: '(ERR|WARN|EMER)'
+  expr: '([0-9-]+)T[0-9:\.]+Z.+\|(ERR|ERROR|WARN|EMER)\|.+'
 ovn-northd:
   input:
     path: 'var/log/ovn/ovn-northd.log'
-  hint: '(ERR|WARN)'
-  expr: '([0-9-]+)T[0-9:\.]+Z.+\|(ERR|ERROR|WARN)\|.+'
+  hint: '(ERR|WARN|EMER)'
+  expr: '([0-9-]+)T[0-9:\.]+Z.+\|(ERR|ERROR|WARN|EMER)\|.+'
 ovn-controller:
   input:
     path: 'var/log/ovn/ovn-controller.log'
-  hint: '(ERR|WARN)'
-  expr: '([0-9-]+)T[0-9:\.]+Z.+\|(ERR|ERROR|WARN)\|.+'
+  hint: '(ERR|WARN|EMER)'
+  expr: '([0-9-]+)T[0-9:\.]+Z.+\|(ERR|ERROR|WARN|EMER)\|.+'
```

### Comparing `hotsos-1.1.13.post9/hotsos/defs/events/openvswitch/ovn/ovn-central.yaml` & `hotsos-1.1.14/hotsos/defs/events/openvswitch/ovn/ovn-central.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/events/openvswitch/ovn/ovn-controller.yaml` & `hotsos-1.1.14/hotsos/defs/events/openvswitch/ovn/ovn-controller.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/events/openvswitch/ovs/ovs-vswitchd.yaml` & `hotsos-1.1.14/hotsos/defs/events/openvswitch/ovs/ovs-vswitchd.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/events/storage/ceph/mon/monlogs.yaml` & `hotsos-1.1.14/hotsos/defs/events/storage/ceph/mon/monlogs.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/kernel/amd_iommu_pt.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/kernel/amd_iommu_pt.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/kernel/memory.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/kernel/memory.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/kernel/network/misc.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/kernel/network/misc.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/kernel/network/tcp.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/kernel/network/tcp.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/kernel/network/udp.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/kernel/network/udp.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/kernel/qla2xxx.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/kernel/qla2xxx.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/kubernetes/system_cpufreq_mode.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/kubernetes/system_cpufreq_mode.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/lxd/lxcfs_deadlock.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/lxd/lxcfs_deadlock.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/lxd/lxcfs_lp1807628.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/lxd/bugs/lp1807628.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/mysql/mysql_connections.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/mysql/mysql_connections.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/mysql/mysql_router.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/mysql/bugs/lp1959861.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/openstack/barbican/bugs.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/openstack/barbican/bugs/lp1946787.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/openstack/eol.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/openstack/eol.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/openstack/keystone/bugs.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/openstack/keystone/bugs/lp1896125.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/openstack/masakari/pacemaker_remote.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/openstack/masakari/pacemaker_remote.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 checks:
   is_compute_host_using_masakari:
     apt: [nova-compute, masakari-host-monitor]
   pr_installed:
     apt: pacemaker-remote
   pr_enabled:
-    systemd:
-      pacemaker_remote: enabled
+    or:
+      systemd:
+        pacemaker_remote: enabled
+      pebble:
+        pacemaker_remote: active 
 conclusions:
   pacemaker_not_installed:
     priority: 2
     decision:
       - is_compute_host_using_masakari
       - not: pr_installed
     raises:
```

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/openstack/neutron/neutron_ovs_cleanup.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/openstack/neutron/neutron_ovs_cleanup.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/openstack/neutron/ovn_stale_db.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/openstack/neutron/ovn_stale_db.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/openstack/nova/config_checks.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/openstack/nova/config_checks.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/openstack/nova/cpu_pinning.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/openstack/nova/cpu_pinning.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/openstack/octavia/bugs.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/openstack/octavia/bugs/sb1896125.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/openstack/octavia/hm_port_health.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/openstack/octavia/hm_port_health.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 checks:
   octavia_worker_installed:
-    - property: hotsos.core.plugins.openstack.octavia.OctaviaBase.installed
-    - systemd: octavia-worker
+    property: hotsos.core.plugins.openstack.octavia.OctaviaBase.installed
+    or:
+      systemd: octavia-worker
+      pebble: octavia-worker
   hm_port_has_no_packet_drops_or_errors:
     property: hotsos.core.plugins.openstack.octavia.OctaviaBase.hm_port_healthy
   hm_port_address_check:
     property: hotsos.core.plugins.openstack.octavia.OctaviaBase.hm_port_has_address
 conclusions:
   no-addr-or-noexist:
     priority: 1
```

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/openstack/openstack_apache2_certificates.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/openstack/openstack_apache2_certificates.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/openstack/system_cpufreq_mode.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/openstack/system_cpufreq_mode.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/openstack/systemd_masked_services.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/openstack/systemd_masked_services.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/openvswitch/dpif_lost_packets.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/openvswitch/dpif_lost_packets.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/openvswitch/dpif_resubmit_actions.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/openvswitch/dpif_resubmit_actions.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/openvswitch/ovn/bfd_flapping.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/openvswitch/ovn/bfd_flapping.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_bugs.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1865127.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -4,30 +4,20 @@
       path: 'var/log/ovn/ovn-controller.log'
     expr: '.+ERR\|bridge not found for localnet port \S+ with network name'
   1865127_broken_package:
     apt:
       ovn-common:
         - min: 0
           max: 20.12.0~1
-  has_1917475:
-    input:
-      path: 'var/log/ovn/ovn-controller.log'
-    expr: '.+transaction error: {"details":"RBAC rules for client \\"\S+\\" role \\"\S+\\" prohibit .+ table\s+\\"\S+\\".","error":"permission error"'
 conclusions:
   lp1865127:
     decision:
       - has_1865127
       - 1865127_broken_package
     raises:
       type: LaunchpadBug
       bug-id: 1865127
       message: >-
         The version of ovn on this node is affected by a known bug where the
         ovn-controller logs are being spammed with error messages containing
         "No bridge for localnet port ..." when that is in fact not an error.
         Upgrading to a version >= 20.12.0 will fix the issue.
-  lp1917475:
-    decision: has_1917475
-    raises:
-      type: LaunchpadBug
-      bug-id: 1917475
-      message: known ovn bug identified - db rbac errors
```

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_services.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_services.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_ssl_certs.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_certs_logs.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_chassis_ssl_certs.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/openvswitch/ovn/ovn_chassis_certs_logs.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_db_upgrade.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/openvswitch/ovn/ovn_db_upgrade.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/openvswitch/ovn/ovsdb_reconnect_errors.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/openvswitch/ovn/ovsdb_reconnect_errors.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/openvswitch/ovs_bugs.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/openvswitch/bugs/lp1839592.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/openvswitch/tunnels_ct.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/openvswitch/bugs/lp1978806.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/pacemaker/bugs.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/pacemaker/bugs/lp1874719.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/rabbitmq/cluster_config.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/rabbitmq/cluster_config.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/rabbitmq/cluster_logchecks.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/rabbitmq/cluster_logchecks.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/rabbitmq/cluster_resources.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/rabbitmq/cluster_resources.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/rabbitmq/rabbitmq_bugs.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/rabbitmq/bugs/lp1943937.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/sosreport/plugin_timeouts.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/sosreport/plugin_timeouts.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/bcache/bdev.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/storage/bcache/bdev.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/bcache/cacheset.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/storage/bcache/cacheset.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mgr/autoscaler_overlap_roots.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mgr/autoscaler_overlap_roots.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/auth_insecure_global_id_reclaim_allowed.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/auth_insecure_global_id_reclaim_allowed.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/autoscaler_bug.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/autoscaler_bug.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -24,17 +24,21 @@
         - min: 17.0.0
           max: 17.2.0-0ubuntu0
         # kinetic
         - min: 17.2.0-0ubuntu0
           max: 17.2.0-0ubuntu4
     # NOTE: this is in fact already checked by the root requirements for ceph-mon checks
     # but since those are not currently loaded by unit tests we do this here as well.
-    systemd:
-      ceph-mon:
-        state: enabled
+    or:
+      systemd:
+        ceph-mon:
+          state: enabled
+      pebble:
+        ceph-mon:
+          state: active
   autoscaler_enabled:
     varops: [[$autoscaler_enabled_pools], [length_hint]]
   autoscaler_disabled:
     varops: [[$autoscaler_enabled_pools], [length_hint], [eq, 0]]
 conclusions:
   cephtracker53729_autoscaler_disabled:
     decision:
```

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_size.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_size.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_spillover.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_spillover.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph-mon.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph-mon.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -5,9 +5,11 @@
 # more than one mon we also do not necessarily want to skip checks that can run
 # if *any* mon is running. To achieve this we make this requirement sufficiently
 # permissive such that the local ceph-mon service need not necessarily be
 # active - checks themselves can apply more restrictive pre-requisites
 # if necessary.
 requires:
   # ensures that a ceph-mon unit is enabled but does not assert that it is active
-  systemd:
-    ceph-mon: enabled
+  or:
+    systemd:
+      ceph-mon: enabled
+    pebble: ceph-mon
```

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_address_overlap.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_address_overlap.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_cluster_health.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_cluster_health.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_versions_mismatch.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_versions_mismatch.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/crushmap_bucket_checks.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/crushmap_bucket_checks.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/eol.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/eol.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/laggy_pgs.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/laggy_pgs.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/large_omap_objects.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/large_omap_objects.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_db_too_big.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_db_too_big.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_elections_flapping.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_elections_flapping.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_flapping.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_flapping.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_maps_backlog_too_large.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_maps_backlog_too_large.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_messenger_v2_protocol.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_messenger_v2_protocol.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_heartbeats.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_heartbeats.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_ops.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_ops.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 checks:
   # NOTE: the following check can be run on a mon or osd node since the same
   # logs should be available on both.
   osd_slow_ops:
     input:
       path: var/log/ceph/ceph*.log
-    expr: '^([\d-]+)[T ]([\d:]+\.\d)\S+ .+ slow ops, oldest one blocked .+'
+    search:
+      expr: '^([\d-]+)[T ]([\d:]+\.\d)\S+ .+ slow ops, oldest one blocked .+'
+      constraints:
+        # i.e. must occur 5 times within same 24 hour period
+        min-results: 5
+        search-period-hours: 1
+        search-result-age-hours: 24
   ceph_interfaces_have_errors:
     property: hotsos.core.plugins.storage.ceph.CephChecksBase.has_interface_errors
 conclusions:
   cause-unknown:
     priority: 1
     decision: osd_slow_ops
     raises:
```

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_imbalance.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_imbalance.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_overdose.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_overdose.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/required_osd_release_mismatch.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/required_osd_release_mismatch.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/unresponsive_mon_mgr.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-mon/unresponsive_mon_mgr.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bcache_lp1936136.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1936136.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1996010.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,11 @@
 vars:
   bluestore_volume_selection_policy: '@hotsos.core.plugins.storage.ceph.CephDaemonAllOSDsFactory.bluestore_volume_selection_policy:CephDaemonConfigShow'
   bluestore_cache_onode: '@hotsos.core.plugins.storage.ceph.CephDaemonAllOSDsFactory.bluestore_cache_onode:CephDaemonDumpMemPools'
 checks:
-  has_1959649:
-    - apt:
-        ceph-osd:
-          - min: 15.2.6
-            max: 15.2.10
-    - varops: [[$bluestore_volume_selection_policy], [ne, [use_some_extra]]]
-    - varops: [[$bluestore_volume_selection_policy], [ne, []]]
   has_1996010_osd_log:
     # NOTE: this needs quite a high debug level to appear - debug_bluestore=30/30
     input: var/log/ceph/ceph-osd.*.log
     expr: '^([\d-]+)[T ]([\d:]+\.\d)\S+ .+ bluestore\.MempoolThread\(\S+\) _resize_shards max_shard_onodes: 0 '
   has_1996010_mempools:
     # this is a hack to check if a value less than 10 exists in the list
     or:
@@ -23,24 +16,14 @@
       - varops: [[$bluestore_cache_onode], [contains, 4]]
       - varops: [[$bluestore_cache_onode], [contains, 5]]
       - varops: [[$bluestore_cache_onode], [contains, 6]]
       - varops: [[$bluestore_cache_onode], [contains, 7]]
       - varops: [[$bluestore_cache_onode], [contains, 8]]
       - varops: [[$bluestore_cache_onode], [contains, 9]]
 conclusions:
-  lp1959649:
-    decision: has_1959649
-    raises:
-      type: LaunchpadBug
-      bug-id: 1959649
-      message: >-
-        This host is vulnerable to known bug https://tracker.ceph.com/issues/38745.
-        RocksDB needs more space than the leveled space available so it is using
-        storage from the data disk.
-        Please set bluestore_volume_selection_policy of all OSDs to use_some_extra
   lp1996010:
     decision:
       or:
         - has_1996010_osd_log
         - has_1996010_mempools
     raises:
       type: LaunchpadBug
```

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph_address_overlap.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph_address_overlap.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/eol.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-osd/eol.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/filestore_to_bluestore_upgrade.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-osd/filestore_to_bluestore_upgrade.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/juju_ceph_no_bcache_tuning.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-osd/juju_ceph_no_bcache_tuning.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_flapping.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_flapping.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_latency.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_latency.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_slow_ops.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_slow_ops.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 checks:
   # NOTE: the following check can be run on a mon or osd node since the same
   # logs should be available on both.
   osd_slow_ops:
     input:
       path: var/log/ceph/ceph*.log
-    expr: '^([\d-]+)[T ]([\d:]+\.\d)\S+ .+ slow ops, oldest one blocked .+'
+    search:
+      expr: '^([\d-]+)[T ]([\d:]+\.\d)\S+ .+ slow ops, oldest one blocked .+'
+      constraints:
+        # i.e. must occur 5 times within same 24 hour period
+        min-results: 5
+        search-period-hours: 1
+        search-result-age-hours: 24
   ceph_interfaces_have_errors:
     property: hotsos.core.plugins.storage.ceph.CephChecksBase.has_interface_errors
 conclusions:
   cause-unknown:
     priority: 1
     decision: osd_slow_ops
     raises:
```

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/pg_overdose.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-osd/pg_overdose.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/ssd_osds_no_discard.yaml.disabled` & `hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-osd/ssd_osds_no_discard.yaml.disabled`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/system_cpufreq_mode.yaml` & `hotsos-1.1.14/hotsos/defs/scenarios/storage/ceph/ceph-osd/system_cpufreq_mode.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/plugin_extensions/juju/summary.py` & `hotsos-1.1.14/hotsos/plugin_extensions/juju/summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,14 +103,16 @@
 
 class JujuSummary(JujuChecksBase):
 
     @idx(0)
     def __summary_services(self):
         if self.systemd.services:
             return self.systemd.summary
+        elif self.pebble.services:
+            return self.pebble.summary
 
     @idx(1)
     def __summary_version(self):
         if self.machine:
             return self.machine.version
 
         return "unknown"
```

### Comparing `hotsos-1.1.13.post9/hotsos/plugin_extensions/kernel/summary.py` & `hotsos-1.1.14/hotsos/plugin_extensions/kernel/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/plugin_extensions/kubernetes/summary.py` & `hotsos-1.1.14/hotsos/plugin_extensions/kubernetes/summary.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 from hotsos.core.plugins.kubernetes import KubernetesChecksBase
 
 
 class KubernetesSummary(KubernetesChecksBase):
 
     @idx(0)
     def __summary_services(self):
-        return self.systemd.summary
+        if self.systemd.services:
+            return self.systemd.summary
+        elif self.pebble.services:
+            return self.pebble.summary
 
     @idx(1)
     def __summary_snaps(self):
         snaps = self.snaps.all_formatted
         if snaps:
             return snaps
```

### Comparing `hotsos-1.1.13.post9/hotsos/plugin_extensions/lxd/summary.py` & `hotsos-1.1.14/hotsos/plugin_extensions/lxd/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/plugin_extensions/openstack/agent/events.py` & `hotsos-1.1.14/hotsos/plugin_extensions/openstack/agent/events.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/plugin_extensions/openstack/agent/exceptions.py` & `hotsos-1.1.14/hotsos/plugin_extensions/openstack/agent/exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 import os
 import re
 
 from collections import UserDict
-from searchkit.utils import MPCache
 
 from hotsos.core.log import log
 from hotsos.core.config import HotSOSConfig
 from hotsos.core.plugins.openstack.common import OpenstackChecksBase
 from hotsos.core.plugins.openstack.openstack import OPENSTACK_LOGS_TS_EXPR
 from hotsos.core.search import (
     FileSearcher,
     SearchDef,
     SearchConstraintSearchSince,
 )
 
 
 class AgentExceptionCheckResults(UserDict):
 
-    def __init__(self, service_obj, results, search_obj):
+    def __init__(self, results, source_id_resolver_callback):
         """
-        @param service_obj: OSTProject object
         @param results: list of searchkit.SearchResult objects grouped by
                         agent/log in which they were found.
-        @param search_obj: FileSearcher object
+        @param source_id_resolver_callback: searchkit results contain a
+                                            reference to the path that matched
+                                            the result and this callback is
+                                            called to resolve back to a path.
         """
-        self.service = service_obj
         self.results = results
-        self.search_obj = search_obj
+        self.source_id_resolver_callback = source_id_resolver_callback
         self.data = {}
         for name, _results in self.results.items():
             self.data[name] = self._tally_results(_results)
 
     @property
     def agents(self):
         """ Returns a list of agents for that have raised exceptions. """
@@ -93,15 +93,15 @@
 
     @property
     def files_w_exceptions(self):
         """ Return a list of files containing exceptions. """
         files = []
         for results in self.results.values():
             sources = set([r.source_id for r in results])
-            files.extend([self.search_obj.resolve_source_id(s)
+            files.extend([self.source_id_resolver_callback(s)
                           for s in sources])
 
         return files
 
 
 class AgentExceptionChecks(OpenstackChecksBase):
     """
@@ -109,16 +109,15 @@
     WARNING log levels depending on who raised them and their
     importance. This class provides a way to identify exceptions in
     logs and provide a per-agent tally by date or time.
     """
 
     def __init__(self):
         super().__init__()
-        self.cache = MPCache('agent_exception_checks', 'openstack_extensions',
-                             HotSOSConfig.global_tmp_dir)
+        self._agent_results = None
         c = SearchConstraintSearchSince(exprs=[OPENSTACK_LOGS_TS_EXPR])
         self.searchobj = FileSearcher(constraint=c)
         # The following are expected to be logged using WARNING log level.
         self._agent_warnings = {
             'nova': ['MessagingTimeout',
                      'DiskNotFound',
                      r"Timeout waiting for \[\('\S+',",
@@ -175,15 +174,15 @@
         if err_exprs:
             values = "(?:{})".format('|'.join(err_exprs))
             expr = expr_template.format(values)
             sd = SearchDef(expr, tag=tag + '.error', hint='ERROR')
             self.searchobj.add(sd, logs_path,
                                allow_global_constraints=constraints)
 
-    def load(self):
+    def _load(self):
         """Register searches for exceptions as well as any other type of issue
         we might want to catch like warnings etc which may not be errors or
         exceptions.
         """
         log.debug("loading exception search defs")
         for project in self.ost_projects.all.values():
             if not project.installed:
@@ -229,26 +228,23 @@
                     path = os.path.join(HotSOSConfig.data_root, path)
                     if HotSOSConfig.use_all_logs:
                         path = "{}*".format(path)
 
                     self._add_agent_searches(project, agent, path,
                                              expr_template)
 
-    def run(self, search_results):
+    def _run(self, search_results):
         """ Process search results to see if we got any hits.
 
         @param search_results: a searchkit.SearchResultsCollection object.
         @return: a dictionary of services and underlying agents with any
                  exceptions they have raised.
         """
-        agent_exceptions = self.cache.get('agent_exceptions') or {}
-        if agent_exceptions:
-            return agent_exceptions
-
         log.debug("processing exception search results")
+        agent_exceptions = {}
         for name, project in self.ost_projects.all.items():
             if not project.installed:
                 continue
 
             for log_level in ['warning', 'error']:
                 agent_results = {}
                 for agent in project.services:
@@ -259,42 +255,43 @@
 
                 if not agent_results:
                     continue
 
                 if log_level not in agent_exceptions:
                     agent_exceptions[log_level] = {}
 
-                _results = AgentExceptionCheckResults(self.ost_projects[name],
-                                                      agent_results,
-                                                      self.searchobj)
+                callback = self.searchobj.catalog.source_id_to_path
+                _results = AgentExceptionCheckResults(agent_results, callback)
                 agent_exceptions[log_level][name] = _results
 
-        self.cache.set('agent_exceptions', agent_exceptions)
         return agent_exceptions
 
-    def execute(self):
-        self.load()
-        return self.run(self.searchobj.run())
+    @property
+    def agent_results(self):
+        if self._agent_results is not None:
+            return self._agent_results
+
+        self._load()
+        self._agent_results = self._run(self.searchobj.run())
+        return self._agent_results
 
     def __summary_agent_warnings(self):
         """
         Only WARNING level exceptions
         """
-        exc_info = self.execute()
-        if exc_info and 'warning' in exc_info:
+        if self.agent_results and 'warning' in self.agent_results:
             _exc_info = {}
-            for svc, results in exc_info['warning'].items():
+            for svc, results in self.agent_results['warning'].items():
                 _exc_info[svc] = dict(results)
 
             return {agent: dict(info) for agent, info in _exc_info.items()}
 
     def __summary_agent_exceptions(self):
         """
         Only ERROR level exceptions
         """
-        exc_info = self.execute()
-        if exc_info and 'error' in exc_info:
+        if self.agent_results and 'error' in self.agent_results:
             _exc_info = {}
-            for svc, results in exc_info['error'].items():
+            for svc, results in self.agent_results['error'].items():
                 _exc_info[svc] = dict(results)
 
             return {agent: dict(info) for agent, info in _exc_info.items()}
```

### Comparing `hotsos-1.1.13.post9/hotsos/plugin_extensions/openstack/nova_external_events.py` & `hotsos-1.1.14/hotsos/plugin_extensions/openstack/nova_external_events.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/plugin_extensions/openstack/service_features.py` & `hotsos-1.1.14/hotsos/plugin_extensions/openstack/service_features.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/plugin_extensions/openstack/service_network_checks.py` & `hotsos-1.1.14/hotsos/plugin_extensions/openstack/service_network_checks.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/plugin_extensions/openstack/summary.py` & `hotsos-1.1.14/hotsos/plugin_extensions/openstack/summary.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,16 @@
                 'days-to-eol': self.days_to_eol}
 
     @idx(1)
     def __summary_services(self):
         """Get string info for running services."""
         if self.systemd.services:
             return self.systemd.summary
+        elif self.pebble.services:
+            return self.pebble.summary
 
     @idx(2)
     def __summary_dpkg(self):
         # require at least one core package to be installed to include
         # this in the report.
         if self.apt.core:
             return self.apt.all_formatted
```

### Comparing `hotsos-1.1.13.post9/hotsos/plugin_extensions/openstack/vm_info.py` & `hotsos-1.1.14/hotsos/plugin_extensions/openstack/vm_info.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/plugin_extensions/openvswitch/event_checks.py` & `hotsos-1.1.14/hotsos/plugin_extensions/openvswitch/event_checks.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/plugin_extensions/openvswitch/summary.py` & `hotsos-1.1.14/hotsos/plugin_extensions/openvswitch/summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,16 @@
         self.ovn = OVNBase()
 
     @idx(0)
     def __summary_services(self):
         """Get string info for running daemons."""
         if self.systemd.services:
             return self.systemd.summary
+        elif self.pebble.services:
+            return self.pebble.summary
 
     @idx(1)
     def __summary_dpkg(self):
         return self.apt.all_formatted
 
     @idx(2)
     def __summary_config(self):
```

### Comparing `hotsos-1.1.13.post9/hotsos/plugin_extensions/pacemaker/summary.py` & `hotsos-1.1.14/hotsos/plugin_extensions/pacemaker/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/plugin_extensions/rabbitmq/summary.py` & `hotsos-1.1.14/hotsos/plugin_extensions/rabbitmq/summary.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 class RabbitMQSummary(RabbitMQChecksBase):
 
     @idx(0)
     def __summary_services(self):
         if self.systemd.services:
             return self.systemd.summary
+        elif self.pebble.services:
+            return self.pebble.summary
 
     @idx(1)
     def __summary_dpkg(self):
         apt = self.apt.all_formatted
         if apt:
             return apt
```

### Comparing `hotsos-1.1.13.post9/hotsos/plugin_extensions/sosreport/summary.py` & `hotsos-1.1.14/hotsos/plugin_extensions/sosreport/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/plugin_extensions/storage/bcache_summary.py` & `hotsos-1.1.14/hotsos/plugin_extensions/storage/bcache_summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/plugin_extensions/storage/ceph_event_checks.py` & `hotsos-1.1.14/hotsos/plugin_extensions/storage/ceph_event_checks.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/plugin_extensions/storage/ceph_summary.py` & `hotsos-1.1.14/hotsos/plugin_extensions/storage/ceph_summary.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,16 @@
                 'days-to-eol': self.days_to_eol}
 
     @idx(1)
     def __summary_services(self):
         """Get string info for running services."""
         if self.systemd.services:
             return self.systemd.summary
+        elif self.pebble.services:
+            return self.pebble.summary
 
     @idx(2)
     def __summary_dpkg(self):
         # require at least one core package to be installed to include
         # this in the report.
         if self.apt.core:
             return self.apt.all_formatted
```

### Comparing `hotsos-1.1.13.post9/hotsos/plugin_extensions/system/checks.py` & `hotsos-1.1.14/hotsos/plugin_extensions/system/checks.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/plugin_extensions/system/summary.py` & `hotsos-1.1.14/hotsos/plugin_extensions/system/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos/templates/header.html` & `hotsos-1.1.14/hotsos/templates/header.html`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.13.post9/hotsos.egg-info/PKG-INFO` & `hotsos-1.1.14/hotsos.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,106 +1,129 @@
 Metadata-Version: 2.1
 Name: hotsos
-Version: 1.1.13.post9
+Version: 1.1.14
 Summary: Software analysis toolkit. Define checks in high-level language and leverage library to perform analysis of common Cloud applications.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Overview
 
-Hotsos is a framework for software-defined analysis. It provides a library of plugins written in Python along with a [high-level language](hotsos/defs/README.md) in which to implement checks and analysis and report problems. Supported plugins include:
+Hotsos is a framework for software-defined analysis. It provides a library of
+plugins written in Python along with a [high-level
+language](hotsos/defs/README.md) in which to implement checks and analysis and
+report problems. Supported plugins include:
+
+* Openstack
+* Kubernetes
+* Ceph
+* Open vSwitch
+* Juju
+* MAAS
+* Vault
+* MySQL
+* RabbitMQ
+* and more
+
+Each plugin has a set of associated checks or "scenarios" that run in the
+context of that plugin and seek to identify issues. The output of running hotsos
+is a summary produced by each plugin including key information about the runtime
+of that application along with any issues detected. This summary also aims to
+contain as much information needed to aid manual analysis beyond the automated
+checks and is easily extensible.
 
-  * Openstack
-  * Kubernetes
-  * Ceph
-  * OpenvSwitch
-  * Juju
-  * MAAS
-  * Vault
-  * MySQL
-  * RabbitMQ
-  * and more
+The default summary format is yaml and a number of other options and formats are
+provided.
 
-Each plugin has a set of associated checks or "scenarios" that run in the context of that plugin and seek to identify issues. The output of running hotsos is a summary produced by each plugin including key information about the runtime of that application along with any issues detected. This summary also aims to contain as much information needed to aid manual analysis beyond the automated checks and is easily extensible.
-
-The default summary format is yaml and a number of other options and formats are provided.
-
-Hotsos is either run directly against a host or a [sosreport](https://github.com/sosreport/sos).
+Hotsos is either run directly against a host or a
+[sosreport](https://github.com/sosreport/sos).
 
 The code has the following structure:
 
-  * core library (includes plugins)
-  * yaml-defined checks (see documentation at [defs](hotsos/defs/README.md))
-  * plugin extensions e.g. summary output
-  * tests
+* core library (includes plugins)
+* yaml-defined checks (see documentation at [defs](hotsos/defs/README.md))
+* plugin extensions e.g. summary output
+* tests
 
 ## Usage
 
-Lets say for example that you are running an Openstack Cloud and one of your hypervisor nodes that also happens to be running part of a Ceph storage cluster is experiencing a problem with network connectivity to workloads. You can simply run hotsos either against a sosreport generated from that node or on that node directly as follows:
+Let's say for example that you are running an Openstack Cloud and one of your
+hypervisor nodes that also happens to be running part of a Ceph storage cluster
+is experiencing a problem with network connectivity to workloads. You can simply
+run hotsos either against a sosreport generated from that node or on that node
+directly as follows:
 
-```
+```console
 ubuntu@ncpu1$ hotsos -s
 INFO: analysing localhost /
 INFO: output saved to hotsos-output-1673868979
 ```
 
-Now you will find a folder called hotsos-output-1673868979 containing a summary of information in a number of different formats. Taking the most common yaml format we can see:
+Now you will find a folder called `hotsos-output-1673868979` containing a
+summary of information in a number of different formats. Taking the most common
+yaml format we can see:
 
-```
+```console
 ubuntu@ncpu1$ cat hotsos-output-1673868979/ncpu1.summary.yaml
 ```
 
-This file will contain a per-plugin summary of information found along with any issues detected. By default hotsos will only look at the last 24 hours of logs. You can increase this with *--all-logs* which will by default give you 7 days worth and if you want more you can use *--max-logrotate-depth <days>*.
-
-Our folder also contains other formats of the same information and one of those is json which can easily be queried using a tool called [jq](https://stedolan.github.io/jq/). Using this useful tool we can easily query for specific information e.g.
+This file will contain a per-plugin summary of information found along with any
+issues detected. By default hotsos will only look at the last 24 hours of logs.
+You can increase this with `--all-logs` which will by default give you 7 days
+worth and if you want more you can use `--max-logrotate-depth <days>`.
+
+Our folder also contains other formats of the same information and one of those
+is json which can easily be queried using a tool called
+[jq](https://stedolan.github.io/jq/). Using this useful tool we can easily query
+for specific information e.g.
 
-```
+```console
 ubuntu@ncpu1$ jq -r '.storage."potential-issues"' hotsos-output-1673868979/ncpu1.summary.json
 {
   "BcacheWarnings": [
     "One or more of the following bcache bdev config assertions failed: sequential_cutoff eq \"0.0k\"/actual=\"4.0M\", cache_mode eq \"writethrough [writeback] writearound none\"/actual=\"writethrough [writeback] writearound none\", writeback_percent ge 10/actual=\"10\" (origin=storage.auto_scenario_check)",
     "One or more of the following bcache cacheset config assertions failed: congested_read_threshold_us eq 0/actual=\"2000\", congested_write_threshold_us eq 0/actual=\"20000\" (origin=storage.auto_scenario_check)"
   ]
 }
 ```
 
 ## Examples
 
-An example **full** (yaml) summary can be found [here](examples/hotsos-example-openstack.summary.yaml)
+An example **full** (yaml) summary can be found
+[here](examples/hotsos-example-openstack.summary.yaml)
 
-An example **short** (yaml) summary can be found [here](examples/hotsos-example-openstack.short.summary.yaml)
+An example **short** (yaml) summary can be found
+[here](examples/hotsos-example-openstack.short.summary.yaml)
 
 ## Install
 
 HotSOS is distributed using the following methods:
 
 ### pypi
 
 You can install using Python pip e.g.
 
-```
-sudo apt install python3-pip
-pip install hotsos
+```console
+$ sudo apt install python3-pip
+$ pip install hotsos
 ```
 
 NOTE: currently requires Python >= 3.8
 
 ### snap
 
 You can install as a snap e.g.
 
-```
-sudo apt install snapd
-sudo snap install hotsos --classic
+```console
+$ sudo apt install snapd
+$ sudo snap install hotsos --classic
 ```
 
-See https://snapcraft.io/hotsos for more info on usage.
+See <https://snapcraft.io/hotsos> for more info on usage.
 
 or run from source e.g.
 
-```
+```console
 $ git clone https://github.com/canonical/hotsos
 $ pip install -r hotsos/requirements.txt
 $ ./hotsos/scripts/hotsos
 ```
-
```

### Comparing `hotsos-1.1.13.post9/hotsos.egg-info/SOURCES.txt` & `hotsos-1.1.14/hotsos.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 hotsos/core/host_helpers/__init__.py
 hotsos/core/host_helpers/cli.py
 hotsos/core/host_helpers/common.py
 hotsos/core/host_helpers/config.py
 hotsos/core/host_helpers/filestat.py
 hotsos/core/host_helpers/network.py
 hotsos/core/host_helpers/packaging.py
+hotsos/core/host_helpers/pebble.py
 hotsos/core/host_helpers/ssl.py
 hotsos/core/host_helpers/sysctl.py
 hotsos/core/host_helpers/systemd.py
 hotsos/core/host_helpers/uptime.py
 hotsos/core/issues/__init__.py
 hotsos/core/issues/issue_types.py
 hotsos/core/issues/utils.py
@@ -93,14 +94,15 @@
 hotsos/core/ycheck/engine/properties/requires/__init__.py
 hotsos/core/ycheck/engine/properties/requires/common.py
 hotsos/core/ycheck/engine/properties/requires/requires.py
 hotsos/core/ycheck/engine/properties/requires/types/__init__.py
 hotsos/core/ycheck/engine/properties/requires/types/apt.py
 hotsos/core/ycheck/engine/properties/requires/types/config.py
 hotsos/core/ycheck/engine/properties/requires/types/path.py
+hotsos/core/ycheck/engine/properties/requires/types/pebble.py
 hotsos/core/ycheck/engine/properties/requires/types/property.py
 hotsos/core/ycheck/engine/properties/requires/types/snap.py
 hotsos/core/ycheck/engine/properties/requires/types/systemd.py
 hotsos/core/ycheck/engine/properties/requires/types/varops.py
 hotsos/defs/events/openstack/apache.yaml
 hotsos/defs/events/openstack/apparmor.yaml
 hotsos/defs/events/openstack/http-requests.yaml
@@ -123,66 +125,91 @@
 hotsos/defs/events/storage/ceph/mon/mon.yaml
 hotsos/defs/events/storage/ceph/mon/monlogs.yaml
 hotsos/defs/events/storage/ceph/osd/osd.yaml
 hotsos/defs/events/storage/ceph/osd/osdlogs.yaml
 hotsos/defs/scenarios/juju/charm_unit_checks.yaml
 hotsos/defs/scenarios/juju/juju.yaml
 hotsos/defs/scenarios/juju/jujud_machine_checks.yaml
+hotsos/defs/scenarios/juju/bugs/lp1812361.yaml
+hotsos/defs/scenarios/juju/bugs/lp1852502.yaml
+hotsos/defs/scenarios/juju/bugs/lp1858519.yaml
+hotsos/defs/scenarios/juju/bugs/lp1895040.yaml
+hotsos/defs/scenarios/juju/bugs/lp1910958.yaml
+hotsos/defs/scenarios/juju/bugs/lp1948906.yaml
+hotsos/defs/scenarios/juju/bugs/lp1983140.yaml
+hotsos/defs/scenarios/juju/bugs/lp1983506.yaml
+hotsos/defs/scenarios/juju/bugs/lp1996230.yaml
 hotsos/defs/scenarios/kernel/amd_iommu_pt.yaml
 hotsos/defs/scenarios/kernel/disk_failure.yaml
 hotsos/defs/scenarios/kernel/kernlog_calltrace.yaml
 hotsos/defs/scenarios/kernel/memory.yaml
 hotsos/defs/scenarios/kernel/qla2xxx.yaml
 hotsos/defs/scenarios/kernel/network/misc.yaml
 hotsos/defs/scenarios/kernel/network/tcp.yaml
 hotsos/defs/scenarios/kernel/network/udp.yaml
 hotsos/defs/scenarios/kubernetes/kubernetes.yaml
 hotsos/defs/scenarios/kubernetes/system_cpufreq_mode.yaml
 hotsos/defs/scenarios/lxd/lxcfs_deadlock.yaml
-hotsos/defs/scenarios/lxd/lxcfs_lp1807628.yaml
-hotsos/defs/scenarios/mysql/bugs.yaml
+hotsos/defs/scenarios/lxd/bugs/lp1807628.yaml
 hotsos/defs/scenarios/mysql/mysql.yaml
 hotsos/defs/scenarios/mysql/mysql_connections.yaml
-hotsos/defs/scenarios/mysql/mysql_router.yaml
+hotsos/defs/scenarios/mysql/bugs/lp1959861.yaml
+hotsos/defs/scenarios/mysql/bugs/lp1971565.yaml
+hotsos/defs/scenarios/mysql/bugs/lp372017.yaml
 hotsos/defs/scenarios/openstack/eol.yaml
 hotsos/defs/scenarios/openstack/openstack.yaml
 hotsos/defs/scenarios/openstack/openstack_apache2_certificates.yaml
+hotsos/defs/scenarios/openstack/openstack_charm_conflicts.yaml
 hotsos/defs/scenarios/openstack/pkgs_from_mixed_releases_found.yaml
 hotsos/defs/scenarios/openstack/system_cpufreq_mode.yaml
 hotsos/defs/scenarios/openstack/systemd_masked_services.yaml
-hotsos/defs/scenarios/openstack/barbican/bugs.yaml
-hotsos/defs/scenarios/openstack/keystone/bugs.yaml
+hotsos/defs/scenarios/openstack/barbican/bugs/lp1946787.yaml
+hotsos/defs/scenarios/openstack/keystone/bugs/lp1896125.yaml
 hotsos/defs/scenarios/openstack/masakari/pacemaker_remote.yaml
-hotsos/defs/scenarios/openstack/neutron/bugs.yaml
 hotsos/defs/scenarios/openstack/neutron/neutron_ovs_cleanup.yaml
 hotsos/defs/scenarios/openstack/neutron/ovn_stale_db.yaml
-hotsos/defs/scenarios/openstack/nova/bugs.yaml
+hotsos/defs/scenarios/openstack/neutron/bugs/lp1794991.yaml
+hotsos/defs/scenarios/openstack/neutron/bugs/lp1883089.yaml
+hotsos/defs/scenarios/openstack/neutron/bugs/lp1896506.yaml
+hotsos/defs/scenarios/openstack/neutron/bugs/lp1907686.yaml
+hotsos/defs/scenarios/openstack/neutron/bugs/lp1927868.yaml
+hotsos/defs/scenarios/openstack/neutron/bugs/lp1928031.yaml
+hotsos/defs/scenarios/openstack/neutron/bugs/lp1929832.yaml
+hotsos/defs/scenarios/openstack/neutron/bugs/lp1960319.yaml
+hotsos/defs/scenarios/openstack/neutron/bugs/lp1965297.yaml
+hotsos/defs/scenarios/openstack/neutron/bugs/lp1979089.yaml
 hotsos/defs/scenarios/openstack/nova/config_checks.yaml
 hotsos/defs/scenarios/openstack/nova/cpu_pinning.yaml
-hotsos/defs/scenarios/openstack/octavia/bugs.yaml
+hotsos/defs/scenarios/openstack/nova/bugs/lp1860743.yaml
+hotsos/defs/scenarios/openstack/nova/bugs/lp1888395.yaml
+hotsos/defs/scenarios/openstack/nova/bugs/lp1904580.yaml
+hotsos/defs/scenarios/openstack/nova/bugs/lp1944619.yaml
 hotsos/defs/scenarios/openstack/octavia/hm_port_health.yaml
+hotsos/defs/scenarios/openstack/octavia/bugs/sb1896125.yaml
 hotsos/defs/scenarios/openvswitch/dpif_lost_packets.yaml
 hotsos/defs/scenarios/openvswitch/dpif_resubmit_actions.yaml
 hotsos/defs/scenarios/openvswitch/openvswitch.yaml
-hotsos/defs/scenarios/openvswitch/ovs_bugs.yaml
-hotsos/defs/scenarios/openvswitch/tunnels_ct.yaml
+hotsos/defs/scenarios/openvswitch/bugs/lp1839592.yaml
+hotsos/defs/scenarios/openvswitch/bugs/lp1978806.yaml
 hotsos/defs/scenarios/openvswitch/ovn/bfd_flapping.yaml
-hotsos/defs/scenarios/openvswitch/ovn/ovn_bugs.yaml
+hotsos/defs/scenarios/openvswitch/ovn/ovn_central_certs_logs.yaml
 hotsos/defs/scenarios/openvswitch/ovn/ovn_central_services.yaml
-hotsos/defs/scenarios/openvswitch/ovn/ovn_central_ssl_certs.yaml
-hotsos/defs/scenarios/openvswitch/ovn/ovn_chassis_ssl_certs.yaml
+hotsos/defs/scenarios/openvswitch/ovn/ovn_certs_valid.yaml
+hotsos/defs/scenarios/openvswitch/ovn/ovn_chassis_certs_logs.yaml
 hotsos/defs/scenarios/openvswitch/ovn/ovn_db_upgrade.yaml
 hotsos/defs/scenarios/openvswitch/ovn/ovsdb_reconnect_errors.yaml
-hotsos/defs/scenarios/pacemaker/bugs.yaml
+hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1865127.yaml
+hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1917475.yaml
 hotsos/defs/scenarios/pacemaker/pacemaker.yaml
+hotsos/defs/scenarios/pacemaker/bugs/lp1874719.yaml
 hotsos/defs/scenarios/rabbitmq/cluster_config.yaml
 hotsos/defs/scenarios/rabbitmq/cluster_logchecks.yaml
 hotsos/defs/scenarios/rabbitmq/cluster_resources.yaml
 hotsos/defs/scenarios/rabbitmq/rabbitmq.yaml
-hotsos/defs/scenarios/rabbitmq/rabbitmq_bugs.yaml
+hotsos/defs/scenarios/rabbitmq/bugs/lp1943937.yaml
 hotsos/defs/scenarios/sosreport/plugin_timeouts.yaml
 hotsos/defs/scenarios/storage/storage.yaml
 hotsos/defs/scenarios/storage/bcache/bcache.yaml
 hotsos/defs/scenarios/storage/bcache/bdev.yaml
 hotsos/defs/scenarios/storage/bcache/cacheset.yaml
 hotsos/defs/scenarios/storage/ceph/ceph-mgr/autoscaler_overlap_roots.yaml
 hotsos/defs/scenarios/storage/ceph/ceph-mon/auth_insecure_global_id_reclaim_allowed.yaml
@@ -203,28 +230,34 @@
 hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_maps_backlog_too_large.yaml
 hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_messenger_v2_protocol.yaml
 hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_heartbeats.yaml
 hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_ops.yaml
 hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_imbalance.yaml
 hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_overdose.yaml
 hotsos/defs/scenarios/storage/ceph/ceph-mon/required_osd_release_mismatch.yaml
+hotsos/defs/scenarios/storage/ceph/ceph-mon/rgw_frontend.yaml
 hotsos/defs/scenarios/storage/ceph/ceph-mon/unresponsive_mon_mgr.yaml
-hotsos/defs/scenarios/storage/ceph/ceph-osd/bcache_lp1936136.yaml
-hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs.yaml
 hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph-osd.yaml
 hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph_address_overlap.yaml
 hotsos/defs/scenarios/storage/ceph/ceph-osd/eol.yaml
 hotsos/defs/scenarios/storage/ceph/ceph-osd/filestore_to_bluestore_upgrade.yaml
 hotsos/defs/scenarios/storage/ceph/ceph-osd/juju_ceph_no_bcache_tuning.yaml
 hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_flapping.yaml
 hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_latency.yaml
 hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_slow_ops.yaml
 hotsos/defs/scenarios/storage/ceph/ceph-osd/pg_overdose.yaml
 hotsos/defs/scenarios/storage/ceph/ceph-osd/ssd_osds_no_discard.yaml.disabled
 hotsos/defs/scenarios/storage/ceph/ceph-osd/system_cpufreq_mode.yaml
+hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1936136.yaml
+hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1959649.yaml
+hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1996010.yaml
+hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2013960.yaml
+hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2016845.yaml
+hotsos/defs/scenarios/storage/ceph/ceph-rgw/rgw_frontend_rgw.yaml
+hotsos/defs/scenarios/storage/ceph/common/ceph_charm_conflicts.yaml
 hotsos/defs/scenarios/system/system.yaml
 hotsos/defs/scenarios/system/unattended_upgrades.yaml
 hotsos/plugin_extensions/__init__.py
 hotsos/plugin_extensions/juju/__init__.py
 hotsos/plugin_extensions/juju/summary.py
 hotsos/plugin_extensions/kernel/__init__.py
 hotsos/plugin_extensions/kernel/summary.py
```

### Comparing `hotsos-1.1.13.post9/pyproject.toml` & `hotsos-1.1.14/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -24,13 +24,13 @@
     'importlib-metadata; python_version >= "3.8"',
     'click',
     'progress',
     'pyyaml',
     'simplejson',
     'jinja2',
     'cryptography',
-    'searchkit >= 0.1.18',
+    'searchkit >= 0.2.3',
     'propertree'
 ]
 
 [project.scripts]
 hotsos = "hotsos.cli:main"
```

