# Comparing `tmp/MGP_SDK-1.0.0.tar.gz` & `tmp/MGP_SDK-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\ty027972\Desktop\marianas-team\marianas-team\SDKs\Python\MGP\dist\.tmp-s0movmgn\MGP_SDK-1.0.0.tar", last modified: Thu May 11 17:33:14 2023, max compression
+gzip compressed data, was "C:\Users\ty027972\Desktop\marianas-team\marianas-team\SDKs\Python\MGP\dist\.tmp-mnaqdabj\MGP_SDK-1.1.0.tar", last modified: Thu May 18 21:11:38 2023, max compression
```

## Comparing `MGP_SDK-1.0.0.tar` & `MGP_SDK-1.1.0.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 17:33:14.000000 MGP_SDK-1.0.0/
--rw-rw-rw-   0        0        0     2600 2023-05-11 17:33:14.000000 MGP_SDK-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1752 2023-05-11 17:04:25.000000 MGP_SDK-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-11 17:33:14.000000 MGP_SDK-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1818 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-11 17:33:14.000000 MGP_SDK-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-11 17:33:14.000000 MGP_SDK-1.0.0/src/MGP_SDK/
-drwxrwxrwx   0        0        0        0 2023-05-11 17:33:14.000000 MGP_SDK-1.0.0/src/MGP_SDK/OGC_Spec/
--rw-rw-rw-   0        0        0        0 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/OGC_Spec/__init__.py
--rw-rw-rw-   0        0        0    43338 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/OGC_Spec/interface.py
--rw-rw-rw-   0        0        0     5567 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/OGC_Spec/wfs.py
--rw-rw-rw-   0        0        0     4208 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/OGC_Spec/wms.py
--rw-rw-rw-   0        0        0     7607 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/OGC_Spec/wmts.py
--rw-rw-rw-   0        0        0        0 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 17:33:14.000000 MGP_SDK-1.0.0/src/MGP_SDK/account_service/
--rw-rw-rw-   0        0        0        0 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/account_service/__init__.py
--rw-rw-rw-   0        0        0     3911 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/account_service/accounts.py
--rw-rw-rw-   0        0        0     3885 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/account_service/activations.py
--rw-rw-rw-   0        0        0     5512 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/account_service/addresses.py
--rw-rw-rw-   0        0        0     5759 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/account_service/interface.py
--rw-rw-rw-   0        0        0     2823 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/account_service/products.py
--rw-rw-rw-   0        0        0     3480 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/account_service/rate_tables.py
--rw-rw-rw-   0        0        0     1172 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/account_service/roles.py
--rw-rw-rw-   0        0        0     8249 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/account_service/usage.py
--rw-rw-rw-   0        0        0     9173 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/account_service/users.py
-drwxrwxrwx   0        0        0        0 2023-05-11 17:33:14.000000 MGP_SDK-1.0.0/src/MGP_SDK/analytics_service/
--rw-rw-rw-   0        0        0        0 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/analytics_service/__init__.py
--rw-rw-rw-   0        0        0     6650 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/analytics_service/analytics.py
--rw-rw-rw-   0        0        0     4900 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/analytics_service/interface.py
-drwxrwxrwx   0        0        0        0 2023-05-11 17:33:14.000000 MGP_SDK-1.0.0/src/MGP_SDK/auth/
--rw-rw-rw-   0        0        0        0 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/auth/__init__.py
--rw-rw-rw-   0        0        0     6361 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/auth/auth.py
-drwxrwxrwx   0        0        0        0 2023-05-11 17:33:14.000000 MGP_SDK-1.0.0/src/MGP_SDK/basemap_service/
--rw-rw-rw-   0        0        0        0 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/basemap_service/__init__.py
--rw-rw-rw-   0        0        0     1271 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/basemap_service/basemaps.py
--rw-rw-rw-   0        0        0     7889 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/basemap_service/interface.py
-drwxrwxrwx   0        0        0        0 2023-05-11 17:33:14.000000 MGP_SDK-1.0.0/src/MGP_SDK/discovery_service/
--rw-rw-rw-   0        0        0        0 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/discovery_service/__init__.py
--rw-rw-rw-   0        0        0     7871 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/discovery_service/catalogs.py
--rw-rw-rw-   0        0        0     7974 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/discovery_service/collections.py
--rw-rw-rw-   0        0        0     6263 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/discovery_service/interface.py
--rw-rw-rw-   0        0        0     3139 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/discovery_service/search.py
--rw-rw-rw-   0        0        0     1241 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/discovery_service/server_checks.py
--rw-rw-rw-   0        0        0     1913 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/interface.py
-drwxrwxrwx   0        0        0        0 2023-05-11 17:33:14.000000 MGP_SDK-1.0.0/src/MGP_SDK/monitor_service/
--rw-rw-rw-   0        0        0        0 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/monitor_service/__init__.py
--rw-rw-rw-   0        0        0     3980 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/monitor_service/interface.py
--rw-rw-rw-   0        0        0     7133 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/monitor_service/monitoring.py
-drwxrwxrwx   0        0        0        0 2023-05-11 17:33:14.000000 MGP_SDK-1.0.0/src/MGP_SDK/ordering_service/
--rw-rw-rw-   0        0        0        0 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/ordering_service/__init__.py
--rw-rw-rw-   0        0        0     6003 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/ordering_service/interface.py
--rw-rw-rw-   0        0        0     5932 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/ordering_service/orders.py
--rw-rw-rw-   0        0        0     2946 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/ordering_service/pipelines.py
--rw-rw-rw-   0        0        0    16857 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/process.py
-drwxrwxrwx   0        0        0        0 2023-05-11 17:33:14.000000 MGP_SDK-1.0.0/src/MGP_SDK/streaming/
--rw-rw-rw-   0        0        0        2 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/streaming/__init__.py
--rw-rw-rw-   0        0        0     8370 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/streaming/cli_commands.py
--rw-rw-rw-   0        0        0    10451 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/streaming/interface.py
--rw-rw-rw-   0        0        0     3866 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/streaming/wcs_archive.py
-drwxrwxrwx   0        0        0        0 2023-05-11 17:33:14.000000 MGP_SDK-1.0.0/src/MGP_SDK/tasking_service/
--rw-rw-rw-   0        0        0        0 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/tasking_service/__init__.py
--rw-rw-rw-   0        0        0     3469 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/tasking_service/interface.py
--rw-rw-rw-   0        0        0     4945 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/tasking_service/tasking.py
-drwxrwxrwx   0        0        0        0 2023-05-11 17:33:14.000000 MGP_SDK-1.0.0/src/MGP_SDK/three_d/
--rw-rw-rw-   0        0        0        0 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/three_d/__init__.py
--rw-rw-rw-   0        0        0     2183 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/three_d/interface.py
--rw-rw-rw-   0        0        0     3460 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/three_d/three_d.py
-drwxrwxrwx   0        0        0        0 2023-05-11 17:33:14.000000 MGP_SDK-1.0.0/src/MGP_SDK/token_service/
--rw-rw-rw-   0        0        0        0 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/token_service/__init__.py
--rw-rw-rw-   0        0        0     2783 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/token_service/cli_commands.py
--rw-rw-rw-   0        0        0     2929 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/token_service/token.py
-drwxrwxrwx   0        0        0        0 2023-05-11 17:33:14.000000 MGP_SDK-1.0.0/src/MGP_SDK/usage_service/
--rw-rw-rw-   0        0        0        0 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/usage_service/__init__.py
--rw-rw-rw-   0        0        0      702 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/usage_service/interface.py
--rw-rw-rw-   0        0        0     1563 2023-05-11 17:04:26.000000 MGP_SDK-1.0.0/src/MGP_SDK/usage_service/usage.py
-drwxrwxrwx   0        0        0        0 2023-05-11 17:33:14.000000 MGP_SDK-1.0.0/src/MGP_SDK.egg-info/
--rw-rw-rw-   0        0        0     2600 2023-05-11 17:33:14.000000 MGP_SDK-1.0.0/src/MGP_SDK.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2289 2023-05-11 17:33:14.000000 MGP_SDK-1.0.0/src/MGP_SDK.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 17:33:14.000000 MGP_SDK-1.0.0/src/MGP_SDK.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      395 2023-05-11 17:33:14.000000 MGP_SDK-1.0.0/src/MGP_SDK.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       79 2023-05-11 17:33:14.000000 MGP_SDK-1.0.0/src/MGP_SDK.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-11 17:33:14.000000 MGP_SDK-1.0.0/src/MGP_SDK.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/
+-rw-rw-rw-   0        0        0     2600 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1752 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1845 2023-05-18 21:10:35.000000 MGP_SDK-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK/
+drwxrwxrwx   0        0        0        0 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK/OGC_Spec/
+-rw-rw-rw-   0        0        0        0 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/OGC_Spec/__init__.py
+-rw-rw-rw-   0        0        0    43398 2023-05-18 21:09:42.000000 MGP_SDK-1.1.0/src/MGP_SDK/OGC_Spec/interface.py
+-rw-rw-rw-   0        0        0     5567 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/OGC_Spec/wfs.py
+-rw-rw-rw-   0        0        0     4208 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/OGC_Spec/wms.py
+-rw-rw-rw-   0        0        0     7607 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/OGC_Spec/wmts.py
+-rw-rw-rw-   0        0        0        0 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK/account_service/
+-rw-rw-rw-   0        0        0        0 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/account_service/__init__.py
+-rw-rw-rw-   0        0        0     3911 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/account_service/accounts.py
+-rw-rw-rw-   0        0        0     3885 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/account_service/activations.py
+-rw-rw-rw-   0        0        0     5512 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/account_service/addresses.py
+-rw-rw-rw-   0        0        0     5759 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/account_service/interface.py
+-rw-rw-rw-   0        0        0     2823 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/account_service/products.py
+-rw-rw-rw-   0        0        0     3480 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/account_service/rate_tables.py
+-rw-rw-rw-   0        0        0     1172 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/account_service/roles.py
+-rw-rw-rw-   0        0        0     8249 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/account_service/usage.py
+-rw-rw-rw-   0        0        0     9173 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/account_service/users.py
+drwxrwxrwx   0        0        0        0 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK/analytics_service/
+-rw-rw-rw-   0        0        0        0 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/analytics_service/__init__.py
+-rw-rw-rw-   0        0        0     6650 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/analytics_service/analytics.py
+-rw-rw-rw-   0        0        0     4900 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/analytics_service/interface.py
+drwxrwxrwx   0        0        0        0 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK/auth/
+-rw-rw-rw-   0        0        0        0 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/auth/__init__.py
+-rw-rw-rw-   0        0        0     6387 2023-05-18 21:09:42.000000 MGP_SDK-1.1.0/src/MGP_SDK/auth/auth.py
+drwxrwxrwx   0        0        0        0 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK/basemap_service/
+-rw-rw-rw-   0        0        0        0 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/basemap_service/__init__.py
+-rw-rw-rw-   0        0        0     1271 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/basemap_service/basemaps.py
+-rw-rw-rw-   0        0        0     7889 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/basemap_service/interface.py
+drwxrwxrwx   0        0        0        0 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK/discovery_service/
+-rw-rw-rw-   0        0        0        0 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/discovery_service/__init__.py
+-rw-rw-rw-   0        0        0     7871 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/discovery_service/catalogs.py
+-rw-rw-rw-   0        0        0     7974 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/discovery_service/collections.py
+-rw-rw-rw-   0        0        0     6707 2023-05-18 21:09:42.000000 MGP_SDK-1.1.0/src/MGP_SDK/discovery_service/interface.py
+-rw-rw-rw-   0        0        0     3140 2023-05-18 21:09:42.000000 MGP_SDK-1.1.0/src/MGP_SDK/discovery_service/search.py
+-rw-rw-rw-   0        0        0     1241 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/discovery_service/server_checks.py
+-rw-rw-rw-   0        0        0     1913 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/interface.py
+drwxrwxrwx   0        0        0        0 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK/monitor_service/
+-rw-rw-rw-   0        0        0        0 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/monitor_service/__init__.py
+-rw-rw-rw-   0        0        0     3980 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/monitor_service/interface.py
+-rw-rw-rw-   0        0        0     7133 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/monitor_service/monitoring.py
+drwxrwxrwx   0        0        0        0 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK/ordering_service/
+-rw-rw-rw-   0        0        0        0 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/ordering_service/__init__.py
+-rw-rw-rw-   0        0        0     6264 2023-05-18 21:09:42.000000 MGP_SDK-1.1.0/src/MGP_SDK/ordering_service/interface.py
+-rw-rw-rw-   0        0        0     5932 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/ordering_service/orders.py
+-rw-rw-rw-   0        0        0     3353 2023-05-18 21:09:42.000000 MGP_SDK-1.1.0/src/MGP_SDK/ordering_service/pipelines.py
+-rw-rw-rw-   0        0        0    16857 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/process.py
+drwxrwxrwx   0        0        0        0 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK/streaming/
+-rw-rw-rw-   0        0        0        2 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/streaming/__init__.py
+-rw-rw-rw-   0        0        0     6571 2023-05-18 21:09:42.000000 MGP_SDK-1.1.0/src/MGP_SDK/streaming/cli_commands.py
+-rw-rw-rw-   0        0        0    10859 2023-05-18 21:09:42.000000 MGP_SDK-1.1.0/src/MGP_SDK/streaming/interface.py
+-rw-rw-rw-   0        0        0     3866 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/streaming/wcs_archive.py
+drwxrwxrwx   0        0        0        0 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK/tasking_service/
+-rw-rw-rw-   0        0        0        0 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/tasking_service/__init__.py
+-rw-rw-rw-   0        0        0     3588 2023-05-18 21:09:42.000000 MGP_SDK-1.1.0/src/MGP_SDK/tasking_service/interface.py
+-rw-rw-rw-   0        0        0     5203 2023-05-18 21:09:42.000000 MGP_SDK-1.1.0/src/MGP_SDK/tasking_service/tasking.py
+drwxrwxrwx   0        0        0        0 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK/three_d/
+-rw-rw-rw-   0        0        0        0 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/three_d/__init__.py
+-rw-rw-rw-   0        0        0     2183 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/three_d/interface.py
+-rw-rw-rw-   0        0        0     3460 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/three_d/three_d.py
+drwxrwxrwx   0        0        0        0 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK/token_service/
+-rw-rw-rw-   0        0        0        0 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/token_service/__init__.py
+-rw-rw-rw-   0        0        0     3211 2023-05-18 21:09:42.000000 MGP_SDK-1.1.0/src/MGP_SDK/token_service/cli_commands.py
+-rw-rw-rw-   0        0        0     2929 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/token_service/token.py
+drwxrwxrwx   0        0        0        0 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK/usage_service/
+-rw-rw-rw-   0        0        0        0 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/usage_service/__init__.py
+-rw-rw-rw-   0        0        0      702 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/usage_service/interface.py
+-rw-rw-rw-   0        0        0     1563 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/usage_service/usage.py
+drwxrwxrwx   0        0        0        0 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK.egg-info/
+-rw-rw-rw-   0        0        0     2600 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2289 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      461 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       65 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK.egg-info/top_level.txt
```

### Comparing `MGP_SDK-1.0.0/PKG-INFO` & `MGP_SDK-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MGP_SDK
-Version: 1.0.0
+Version: 1.1.0
 Summary: SDK for interacting with Maxar Geospatial Platform
 Author: MDS Marianas Team
 Author-email: DL-GCS-Marianas@maxar.com
 License: MIT
 Project-URL: Documentation, https://maxar-geospatial-platform.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/Maxar-Corp/maxar-geospatial-platform
 Keywords: OGC,WMS,WFS,WMTS,WCS,MAXAR,IMAGERY,GIS
```

### Comparing `MGP_SDK-1.0.0/README.md` & `MGP_SDK-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.0.0/setup.py` & `MGP_SDK-1.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,36 +3,34 @@
 
 HERE = pathlib.Path(__file__).parent.resolve()
 
 README = (HERE / "README.md").read_text()
 
 setup(
   name = 'MGP_SDK',
-  version = '1.0.0',
+  version = '1.1.0',
   license='MIT',
   description = 'SDK for interacting with Maxar Geospatial Platform',
   long_description=README,
   long_description_content_type="text/markdown",
   author = 'MDS Marianas Team',
   author_email = 'DL-GCS-Marianas@maxar.com',
   project_urls = {
         'Documentation': 'https://maxar-geospatial-platform.readthedocs.io/en/latest/',
         'Source': 'https://github.com/Maxar-Corp/maxar-geospatial-platform'
         },
   keywords = ['OGC', 'WMS', 'WFS', 'WMTS', 'WCS', 'MAXAR', 'IMAGERY', 'GIS'],
   python_requires= '>=3.7',
   install_requires=[
-          'gdal',
           'pyproj',
           'shapely',
           'requests',
           'ipython',
           'pillow',
           'click',
-          'rasterio',
           'beautifulsoup4',
           'lxml'
       ],
   classifiers=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
@@ -45,10 +43,11 @@
     [console_scripts]
     search=MGP_SDK.streaming.cli_commands:search
     config=MGP_SDK.streaming.cli_commands:config_file
     password=MGP_SDK.streaming.cli_commands:reset_password
     download=MGP_SDK.streaming.cli_commands:download
     area=MGP_SDK.streaming.cli_commands:calculate_bbox_sqkm
     token=MGP_SDK.token_service.cli_commands:create_token
-    secret=MGP_SDK.token_service.cli_commands:show_secret
+    get_token=MGP_SDK.token_service.cli_commands:get_tokens
+    delete_token=MGP_SDK.token_service.cli_commands:delete_tokens
     '''
 )
```

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK/OGC_Spec/interface.py` & `MGP_SDK-1.1.0/src/MGP_SDK/OGC_Spec/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -655,17 +655,17 @@
 
         if img_format == 'geotiff':
             try:
                 import rasterio
                 from rasterio.merge import merge
             except:
                 self._pillow_mosaic(base_dir, img_format, img_size=img_size, **kwargs)
-                print("GDAL is not installed on your machine. The downloaded image will not be georeferenced. "
+                print("GDAL and rasterio are not installed on your machine. The downloaded image will not be georeferenced. "
                       " Please refer to the MGP_SDK documentation for steps on how to install GDAL in "
-                      "your environment.")
+                      "your environment. To install rasterio use: pip install rasterio")
             else:
                 srcs_to_mosaic = []
                 for image in os.listdir(base_dir):
                     if image.endswith('.geotiff'):
                         raster = rasterio.open(os.path.join(base_dir, image))
                         srcs_to_mosaic.append(raster)
                         output_data = raster.meta.copy()
```

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK/OGC_Spec/wfs.py` & `MGP_SDK-1.1.0/src/MGP_SDK/OGC_Spec/wfs.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK/OGC_Spec/wms.py` & `MGP_SDK-1.1.0/src/MGP_SDK/OGC_Spec/wms.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK/OGC_Spec/wmts.py` & `MGP_SDK-1.1.0/src/MGP_SDK/OGC_Spec/wmts.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK/account_service/accounts.py` & `MGP_SDK-1.1.0/src/MGP_SDK/account_service/accounts.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK/account_service/activations.py` & `MGP_SDK-1.1.0/src/MGP_SDK/account_service/activations.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK/account_service/addresses.py` & `MGP_SDK-1.1.0/src/MGP_SDK/account_service/addresses.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK/account_service/interface.py` & `MGP_SDK-1.1.0/src/MGP_SDK/account_service/interface.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK/account_service/products.py` & `MGP_SDK-1.1.0/src/MGP_SDK/account_service/products.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK/account_service/rate_tables.py` & `MGP_SDK-1.1.0/src/MGP_SDK/account_service/rate_tables.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK/account_service/roles.py` & `MGP_SDK-1.1.0/src/MGP_SDK/account_service/roles.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK/account_service/usage.py` & `MGP_SDK-1.1.0/src/MGP_SDK/account_service/usage.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK/account_service/users.py` & `MGP_SDK-1.1.0/src/MGP_SDK/account_service/users.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK/analytics_service/analytics.py` & `MGP_SDK-1.1.0/src/MGP_SDK/analytics_service/analytics.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK/analytics_service/interface.py` & `MGP_SDK-1.1.0/src/MGP_SDK/analytics_service/interface.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK/auth/auth.py` & `MGP_SDK-1.1.0/src/MGP_SDK/auth/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         self.base_url = "https://account.maxar.com"
         self.api_base_url = "https://api.maxar.com"
         self.username = username
         self.password = password
         self.client_id = client_id
         self.access = None
         self.refresh = None
-        self.version = "Python1.0.0"
+        self.version = "Python1.1.0"
         self.api_version = 'v1'
         self.SSL = True
 
         if not self.username: #checks if username is provided as argument to class. If not, look for .MGP-config
             dir_path = os.path.expanduser('~')
             file = '.MGP-config'
             full_path = os.path.join(dir_path, file)
@@ -135,13 +135,13 @@
             }
             create_token = requests.request("POST", url, headers=headers, data=json.dumps(payload))
             token = create_token.json()
             return token
         if len(existing_tokens.json()) == 0:
             token = create_token_service_token()
         else:
-            tokens = [i for i in existing_tokens.json() if "SDK_token" in i["name"]]
+            tokens = [i for i in existing_tokens.json() if i["name"] is not None and "SDK_token" in i["name"]]
             if len(tokens) == 0:
                 token = create_token_service_token()
             else:
                 token = existing_tokens.json()[0]
         return token
```

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK/basemap_service/basemaps.py` & `MGP_SDK-1.1.0/src/MGP_SDK/basemap_service/basemaps.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK/basemap_service/interface.py` & `MGP_SDK-1.1.0/src/MGP_SDK/basemap_service/interface.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK/discovery_service/catalogs.py` & `MGP_SDK-1.1.0/src/MGP_SDK/discovery_service/catalogs.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK/discovery_service/collections.py` & `MGP_SDK-1.1.0/src/MGP_SDK/discovery_service/collections.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK/discovery_service/interface.py` & `MGP_SDK-1.1.0/src/MGP_SDK/discovery_service/interface.py`

 * *Files 8% similar despite different names*

```diff
@@ -77,18 +77,29 @@
             limit (int) = Maximum number of items to return
         Returns:
             JSON response
         """
 
         return self.collections.get_collection_definition(**kwargs)
 
+    def get_stac_item(self, collection_id: str, item_id: str):
+        """
+        View details about a specific STAC item
+        Args:
+            collection_id (string) = Name of the collection to search e.g. wv01
+            item_id (string) = Identifier of the desired item
+        Returns:
+            Dictionary of the desired item's information
+        """
+        return self.collections.return_stac_item(collection_id, item_id)
+
     def get_top_level_sub_catalog(self, **kwargs):
         """
         View the available Maxar Sub-Catalogs that can be navigated as a self-contained STAC catalog
-        Keyword Args:
+        Kwargs:
             orderby (string) = SQL-style ORDER BY clause. Only for id and datetime e.g. 'orderby=id ASC' default
             'datetime DESC, id ASC'
             limit (int) = Maximum number of items to return
         Returns:
             JSON response
         """
```

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK/discovery_service/search.py` & `MGP_SDK-1.1.0/src/MGP_SDK/discovery_service/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
                 datetime.strptime(date1, '%Y-%m-%dT%H:%M:%SZ')
                 datetime.strptime(date2, '%Y-%m-%dT%H:%M:%SZ')
             except:
                 try:
                     datetime.strptime(kwargs["datetime"], '%Y-%m-%dT%H:%M:%SZ')
                 except:
                     raise Exception('datetime not in ISO 8601 format or date range not separated by a \'/\'')
-        params_list = ['bbox', 'datetime', 'ids', 'collections' 'intersects', 'where', 'orderby', 'limit']
+        params_list = ['bbox', 'datetime', 'ids', 'collections', 'intersects', 'where', 'orderby', 'limit']
         params = {**{k: v for k, v in kwargs.items() if k in params_list}}
         url = self.base_url
         response = requests.get(url, params=params, headers=self.authorization, verify=self.auth.SSL)
         process._response_handler(response)
         response = response.json()
 
         # pagination
```

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK/discovery_service/server_checks.py` & `MGP_SDK-1.1.0/src/MGP_SDK/discovery_service/server_checks.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK/interface.py` & `MGP_SDK-1.1.0/src/MGP_SDK/interface.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK/monitor_service/interface.py` & `MGP_SDK-1.1.0/src/MGP_SDK/monitor_service/interface.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK/monitor_service/monitoring.py` & `MGP_SDK-1.1.0/src/MGP_SDK/monitor_service/monitoring.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK/ordering_service/interface.py` & `MGP_SDK-1.1.0/src/MGP_SDK/ordering_service/interface.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
     def get_user_orders(self, user_id: str = None, **kwargs):
         """
         Returns a list of a users order by user ID. If no ID is provided, returns a list of the authenticated user's
         orders
 
         Args:
-            user_id (int) = ID of the requested order
+            user_id (string) = The identifier of the desired user
         Kwargs:
             limit (int) = Limits the number of responses returned
             filter (list) = Filter results that match values contained in the given key separated by a colon
             sort (string) = Indicates sort order, desc (default) for descending order (newest first) and asc for
             ascending order (oldest first)
             start_date (string) = ISO-8601 formatted date after which to query orders (inclusive)
             end_date (string) = ISO-8601 formatted date before which to query orders (inclusive)
@@ -122,14 +122,23 @@
             filter (list) = Filter results that match values contained in the given key separated by a colon
         Returns:
             JSON response
         """
 
         return self.orders.get_order_events_by_id(order_id, **kwargs)
 
+    def get_all_pipelines(self):
+        """
+        List out all available pipelines
+        Returns:
+            Dictionary of all available pipelines and their information
+        """
+
+        return self.pipelines.list_all_pipelines()
+
     def get_pipeline_details(self, namespace: str, name: str):
         """
         Gets the details for a pipeline by namespace and name
         Args:
             namespace (string) = A group of pipelines (e.g. 'imagery')
             name (string) = Name of the pipeline to order from (e.g. 'analysis-ready')
         Returns:
```

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK/ordering_service/orders.py` & `MGP_SDK-1.1.0/src/MGP_SDK/ordering_service/orders.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK/ordering_service/pipelines.py` & `MGP_SDK-1.1.0/src/MGP_SDK/ordering_service/pipelines.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,26 @@
     def __init__(self, auth: Auth):
         self.auth = auth
         self.api_version = self.auth.api_version
         self.base_url = f'{self.auth.api_base_url}/ordering/{self.api_version}/pipelines'
         self.token = self.auth.refresh_token()
         self.authorization = {'Authorization': f'Bearer {self.token}'}
 
+    def list_all_pipelines(self):
+        """
+        List out all available pipelines
+        Returns:
+            Dictionary of all available pipelines and their information
+        """
+
+        url = f"{self.base_url}?limit=100"
+        response = requests.get(url, headers=self.authorization, verify=self.auth.SSL)
+        process._response_handler(response)
+        return response.json()
+
     def get_pipeline(self, namespace: str, name: str):
         """
         Get the schema for a specific pipeline
         Args:
             namespace (string) = A group of pipelines (e.g. 'Imagery')
             name (string) = Name of the pipeline to order from (e.g. 'analysis-ready')
         Returns:
```

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK/process.py` & `MGP_SDK-1.1.0/src/MGP_SDK/process.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK/streaming/interface.py` & `MGP_SDK-1.1.0/src/MGP_SDK/streaming/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,7 +197,16 @@
             filename: string, filename of merged image
         Returns:
             None
         """
         # TODO Determine best use case for seamline streaming
         # return self.ogc.create_mosaic(base_dir, img_format, img_size, **kwargs)
 
+    def calculate_sqkm(self, bbox: str):
+        """
+        Function calculates the area in square kilometers of the desired bounding box
+        Args:
+            bbox (string) = Bounding box of AOI. Comma delimited set of coordinates. (miny,minx,maxy,maxx)
+        Returns:
+            Float of bounding box area in square kilometers
+        """
+        return self.ogc.calculate_sqkm(bbox=bbox)
```

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK/streaming/wcs_archive.py` & `MGP_SDK-1.1.0/src/MGP_SDK/streaming/wcs_archive.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK/tasking_service/interface.py` & `MGP_SDK-1.1.0/src/MGP_SDK/tasking_service/interface.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,37 +11,38 @@
     """
 
     def __init__(self, auth):
         self.auth = auth
         self.tasking = Tasking(self.auth)
 
     def new_tasking(self, start_datetime: str, end_datetime: str, aoi_geojson: dict, recipe: str, order_templates: dict,
-                    **kwargs):
+                    validate=False, **kwargs):
         """
         Initiates the creating of a tasking (async) using one of the preconfigured recipes: 50cm_Color, 30cm_Color.
         If a kwarg is null or not provided, default recipe value will be used
         Args:
             start_datetime (string) = ISO-8601 formatted date when the tasking should start
             end_datetime (string) = ISO-8601 formatted date when the tasking should end
             aoi_geojson (dict) = Geojson polygon of area to cover with tasking, e.g.
             {"type":"Polygon","coordinates":[[[...]]]}
             recipe (string) = The name of one of the configured recipes for tasking, e.g. "50cm_Color" or "30cm_Color"
             order_templates (list) = Template for order to be placed. See ordering_service for examples
+            validate (bool) = Binary whether to validate tasking request. Defaults to False
         Kwargs:
             max_cloud_cover (string) = Maximum cloud cover.
             max_off_nadir_angle (string) = Maximum off nadir angle.
             max_sun_elevation_angle (string) = Maximum sun elevation angle.
         Returns:
             Dictionary of submitted tasking request's details
         Throws:
             ValueError: If start or end times are not in ISO-8601 format
         """
 
         return self.tasking.create_new_tasking(start_datetime, end_datetime, aoi_geojson, recipe, order_templates,
-                                               **kwargs)
+                                               validate, **kwargs)
 
     def get_tasking_request(self, tasking_id: str):
         """
         Retrieves a tasking
         Args:
             tasking_id (string) = ID of the requested tasking
         Returns:
```

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK/tasking_service/tasking.py` & `MGP_SDK-1.1.0/src/MGP_SDK/tasking_service/tasking.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,52 +12,57 @@
         self.auth = auth
         self.api_version = self.auth.api_version
         self.base_url = f'{self.auth.api_base_url}/tasking/{self.api_version}/tasking'
         self.token = self.auth.refresh_token()
         self.authorization = {"Authorization": f"Bearer {self.token}"}
 
     def create_new_tasking(self, start_datetime: str, end_datetime: str, aoi_geojson: dict, recipe: str,
-                           order_templates: dict, **kwargs):
+                           order_templates: dict, validate=False, **kwargs):
         """
         Make a tasking request based on imagery recipes
         Args:
             start_datetime (string) = ISO-8601 formatted date when the tasking should start
             end_datetime (string) = ISO-8601 formatted date when the tasking should end
             aoi_geojson (dict) = Geojson polygon of area to cover with tasking, e.g.
             {"type":"Polygon","coordinates":[[[...]]]}
             recipe (string) = The name of one of the configured recipes for tasking, e.g. "50cm_Color" or "30cm_Color"
             order_templates (dict) = Template for order to be placed. See ordering_service for examples
+            validate (bool) = Binary whether to validate tasking request. Defaults to False
         Kwargs:
             max_cloud_cover (string) = Maximum cloud cover.
             max_off_nadir_angle (string) = Maximum off nadir angle.
             max_sun_elevation_angle (string) = Maximum sun elevation angle.
         Returns:
             Dictionary of submitted tasking request's details
         """
 
         time_check = [start_datetime, end_datetime]
         for time in time_check:
             try:
-                datetime.fromisoformat(time)
-            except ValueError:
-                raise ValueError(f'{time} is not in a proper format. Example: 2020-07-10 15:00:00.000')
+                datetime.fromisoformat(time.replace('Z', '+00:00'))
+            except:
+                raise ValueError(f'{time} is not in a proper format. Example: 2020-07-10T15:00:00+00:00')
         if recipe is not '50cm_Color':
             if recipe is not '30cm_color':
                 raise Exception('Recipe must be one of 50cm_Color or 30cm_Color')
         else:
             payload = {
                 'start_datetime': start_datetime,
                 'end_datetime': end_datetime,
                 'aoi_geojson': aoi_geojson,
                 'recipe': recipe,
                 'order_templates': order_templates
             }
             optional_parameters = ['max_cloud_cover', 'max_off_nadir_angle', 'min_sun_elevation_angle']
             data = {**{k: v for k, v in kwargs.items() if k in optional_parameters}, **payload}
-            response = requests.post(self.base_url, data=json.dumps(data), headers=self.authorization,
+            if validate:
+                url = self.base_url + "?validation_only=true"
+            else:
+                url = self.base_url
+            response = requests.post(url, data=json.dumps(data), headers=self.authorization,
                                      verify=self.auth.SSL)
             process._response_handler(response)
             return response.json()
 
     def cancel_tasking(self, tasking_id: str, reason: str = None):
         """
         Cancels a tasking request
```

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK/three_d/interface.py` & `MGP_SDK-1.1.0/src/MGP_SDK/three_d/interface.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK/three_d/three_d.py` & `MGP_SDK-1.1.0/src/MGP_SDK/three_d/three_d.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK/token_service/token.py` & `MGP_SDK-1.1.0/src/MGP_SDK/token_service/token.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK/usage_service/interface.py` & `MGP_SDK-1.1.0/src/MGP_SDK/usage_service/interface.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK/usage_service/usage.py` & `MGP_SDK-1.1.0/src/MGP_SDK/usage_service/usage.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK.egg-info/PKG-INFO` & `MGP_SDK-1.1.0/src/MGP_SDK.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MGP-SDK
-Version: 1.0.0
+Version: 1.1.0
 Summary: SDK for interacting with Maxar Geospatial Platform
 Author: MDS Marianas Team
 Author-email: DL-GCS-Marianas@maxar.com
 License: MIT
 Project-URL: Documentation, https://maxar-geospatial-platform.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/Maxar-Corp/maxar-geospatial-platform
 Keywords: OGC,WMS,WFS,WMTS,WCS,MAXAR,IMAGERY,GIS
```

### Comparing `MGP_SDK-1.0.0/src/MGP_SDK.egg-info/SOURCES.txt` & `MGP_SDK-1.1.0/src/MGP_SDK.egg-info/SOURCES.txt`

 * *Files identical despite different names*

